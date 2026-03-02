---
description: "DE_AWBusiness_Kapazitaetsplanung_4_1"
---


# A+W Kapazitätsplanung

**A+W Business Pro**

A+W - Software for Glass, Windows and Doors

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 1.00/12-2003 | Ersterstellung |
| 1.01/08-2008 | Rechtschreibkorrekturen, grafische Tabellen umgewandelt, Abbildungen und Part-Nummerierung angepasst |
| 1.02/09-2010 | Layout an Doku-Konzept 2010 angepasst |
| 2.00/05-2012 | Ersterstellung des Tutorials; Softwarereferenz vollständig überarbeitet |
| 3.00/08-2013 | Anpassung der ALFAK-Dokumentation auf A+W Business. |
| 4.00/04-2014 | Vollständige Überarbeitung. |
| 4.01/02-2015 | Anpassung an A+W Business Pro. Rechtschreibkorrekturen |
| 4.02/01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business Pro gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business Pro.

### Urheberrechte
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**

Am Pfahlgraben 4 - 10
D-35415 Pohlheim
Germany

Tel: +49 6404 2051 0
Fax: +6404 2051 877
E-Mail: Zentrale@a-w.com
Web: http://www.a-w.com

## Inhalt

- **Vorspann**
    - Revisionsübersicht (H-3)
    - Editorial (H-3)
- **Tutorial** (H-11)
    - Überblick (H-13)
        - Dokumentation (H-14)
        - Aufbau des Tutorials (H-14)
        - Darstellungskonventionen (H-15)
        - Menü-Übersicht (H-16)
        - Modul Kapazitätsplanung (H-16)
        - Modul Fertigung (H-18)
        - Grundgedanken der Kapazitätsplanung (H-20)
        - Nutzung der Kapazitätsplanung (H-21)
    - Stammdaten (H-22)
        - Maschinen und Produktionsbereiche (H-24)
            - Aggregattypen und Aggregate (H-25)
            - Arbeitsarten (H-29)
            - Produktionsbereiche (Arbeitszentren) (H-31)
            - Produktionsbereich anlegen (H-32)
            - Aggregat anlegen (H-33)
            - Übungen (H-37)
        - Schicht- und Arbeitszeiten (H-38)
            - Arbeitszeiten (H-39)
            - Arbeitstage und Schichten (H-39)
            - Maximale Kapazität pro Tag (H-41)
            - Arbeitseinheiten (H-43)
            - Voreinstellungen für Schichten und Kapazitäten (H-48)
            - Kalender anpassen (H-50)
            - Übungen (H-56)
        - Zeitvorgaben (H-57)
            - Basiskomponenten der Zeitplanung (H-58)
            - Vorgabezeiten (H-60)
            - Sonderzeiten (H-63)
            - Arbeitsarten und Zeitzuschläge (H-64)
            - Fallbeispiel ISO und Modell (H-65)
            - Berechnungsreihenfolge für Zuschläge und Faktoren (H-68)
            - Übergangsmatrix und Übergangszeiten (H-69)
            - Rüstzeiten (H-75)
            - Zeitfaktoren für Serien (H-76)
            - Vorgabezeiten festlegen (H-77)
            - Sonderzeit anlegen (H-81)
            - Übungen (H-85)
        - Auswahl der Aggregate (H-86)
            - Prioritäten (H-87)
            - Restriktionen (H-88)
            - Priorität vs. Restriktion (H-89)
            - Automatische Einlastung (H-90)
            - Maschinenauswahl bei Ausweicharbeitsart (H-94)
            - Sperren (H-95)
            - Fertigungsstraße definieren (H-98)
            - Voreinstellungen zur Aggregatauswahl (H-100)
    - Zuordnen der A+W Business Pro-Stammdaten (H-102)
        - Produktionsreihenfolge (H-103)
        - Kombi-Produktart, Kombi-Produktgruppe (H-107)
        - Zuordnung festlegen (H-108)
        - Übungen (H-111)
    - Kapazitätsplanung (H-112)
        - Einlastung der Aufträge (H-113)
        - Terminberechnung (H-114)
        - Einlastung (H-118)
        - Kapazitätsprobleme (H-119)
        - Voreinstellungen für automatische Einlastung (H-123)
        - Auftrag einlasten (H-124)
        - Kapazitätsproblem lösen (H-130)
        - Übungen (H-135)
    - Produktion (H-136)
        - Rückmeldungen zum Produktionsstand (H-137)
        - Erfassungsstellen (H-139)
        - Statusmeldungen (H-141)
        - Fertigmeldung (H-143)
        - Restmengen vom Vortag (H-144)
        - Bruchrückmeldung (H-145)
        - Produktionspapiere drucken (H-146)
        - Auftrag manuell fertig melden (H-148)
        - Bruchmeldung manuell erfassen (H-151)
        - Fertigungsstand prüfen (H-153)
        - Fertigmeldungen nachholen (H-155)
        - Übungen (H-157)
    - Produktionskosten (H-158)
        - Zeitkosten (H-159)
        - Kostenstellen (H-161)
        - Kostenkalkulation im Auftrag (H-164)
        - Kostenkalkulation für Angebote (H-164)
        - Übungen (H-165)
    - Leitstand (H-166)
        - Konzept des Leitstands (H-167)
        - Leitstand - Auftrag (H-169)
        - Leitstand - Aggregat (H-170)
        - Einlastung für einzelnen Auftrag verschieben (H-171)
        - Aggregat ändern (H-176)
        - Übungen (H-178)
- **Softwarereferenz** (H-179)
    - Übersicht (H-181)
    - Verwaltung (H-182)
        - Voreinstellungen Firmendaten (H-183)
        - Einstellungen Schichten (H-187)
    - Allgemein (H-189)
        - Aggregattypen (H-189)
        - Arbeitsarten (H-192)
        - Zugeordnete Aggregate (H-195)
        - Serienfaktoren (H-196)
        - Übergangszeiten (H-197)
    - Organisation (H-199)
        - Produktionsbereich (H-200)
        - Aggregate (H-201)
            - Aggregate - Allgemein (H-202)
            - Aggregate - Restriktionen (H-208)
        - Kalender (H-211)
            - Menü Funktionen (H-211)
            - Kalender - Auswahl (H-212)
            - Kalender - Kalender (H-214)
            - Kalender kopieren (H-215)
        - Übergangsmatrix (H-216)
        - Besondere technische Restriktionen (H-219)
        - Orga Übersicht (H-222)
    - Vorgabezeiten (H-223)
        - Vorgabezeiten (Dialog) (H-224)
        - Menü Funktionen (H-224)
        - Vorgabezeiten – Zeitauswahl (H-225)
        - Vorgabezeiten – Matrix (H-228)
        - Vorgabezeiten - Vektor (H-230)
        - Vorgabezeiten – Einzelzeit (H-231)
        - Vorgabezeiten – Würfel (H-232)
        - Vorgabezeiten ändern (H-233)
        - Vorgabezeiten kopieren (H-233)
        - Sonderzeiten (H-234)
        - Besondere Prioritäten (H-235)
    - Zuordnen (H-237)
        - Produktarten (H-238)
        - WGR (H-240)
        - Produktgruppe (H-241)
        - Produkte (H-242)
        - Kombi-Produktart (H-243)
        - Sonderzuordnung 1-4 (H-244 - H-249)
        - Kombi-Produktgruppe (H-251)
        - Lagerartikel (H-252)
    - Sperren (H-254)
        - Sperren nach WGR, Produktgruppen, Produkten (H-255 - H-258)
        - Folge-Aggregate überspringen (H-259)
        - Kundenbezogene Sperren (H-260)
        - Fertigungsstraße definieren (H-262)
        - Arbeitsgänge überspringen (H-263)
    - Übersichten (H-265)
        - Statistik (H-266)
        - Grafik-Bereiche (H-267)
        - AV-Bereichsstatistik (H-268 - H-272)
        - Konten (H-272)
        - Kostenstellen-Definitionen (H-274)
        - Schnittstelle Lisec (H-275)
    - Kapazitätsplanung (H-276)
    - Einlastung (H-277)
        - Nummernverwalter (H-277)
        - Einlasten NV (H-278)
            - Menü Funktionen, Optionen (H-278)
            - Einlasten NV (Dialog) (H-279)
            - Kriterien ändern (Modus Terminsuche) (H-281)
            - Lieferdatum (H-283)
        - Einlasten Auftrag (H-284)
            - Menü Funktionen, Optionen (H-285, H-286)
            - Einlasten Auftrag (Dialog) (H-287)
            - Einlasten Ergebnis (H-289)
            - Aggregat-Auswahl bei Engpass (H-291)
            - Auftragsnummern (H-293)
            - Positions-Split (H-294)
            - Positions-Zeiten (H-296)
        - Aggregate Ausfall (H-297)
        - Restmengenübertragung (H-300)
    - Produktionsmeldungen (H-301)
        - Datum, Grafik, Lauf (H-302 - H-306)
        - Manuelle Fertigmeldung (H-308)
    - Produktionslisten (H-312)
    - Fertigungsstand Auftrag (H-317)
    - Einlasten von Bestellteilen (H-327)
    - Übersicht Rückmeldungen (H-328)
    - Produktions-Zeiten ändern (H-329)
    - Leitstand (H-335)
        - Leitstand (Dialog) (H-336)
        - Leitstand - Bereiche, Aggregate, Aufträge, etc. (H-338 - H-353)
        - Leitstand (Aggregat) (H-354)
        - Auslastung zu Datum (H-361)
        - Einstellungen zum Leitstand (H-369)
        - Restmengen anzeigen (H-371)
        - Leitstand (Auftrag) (H-372)
        - Verschieben nicht möglich (H-385)
- **Partindex** (H-387)
    - Index Kapazitätsplanung (H-389)

## Tutorial

### Überblick
Das Tutorial zum Modul *Kapazitätsplanung* beschäftigt sich mit den Grundlagen der Planung von Produktionskapazitäten in *A+W Business Pro*. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zu Dokumenten auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- Stammdaten
- Kapazitätsplanung

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in *A+W Business* die Kapazitäten planen und damit die Auslastung der Maschinen überwachen. Die Teilnehmer müssen das Konzept der Stammdaten in *A+W Business* und das Modul *Dokumente* kennen. Kenntnisse der Module *Fertigung* und *Lagerwirtschaft* sind von Vorteil.

### Dokumentation
Für das Modul *Kapazitätsplanung* stehen folgende Dokumente zur Verfügung:

| Format | Umfang |
| :--- | :--- |
| Handout | Ausdruck des Tutorials für die Schulung |
| PDF | Vollständige Unterlagen<br>- Tutorial<br>- Softwarereferenz<br>- Index |
| Online-Hilfe `<F1>` | Kontextsensitive Dialog-Hilfe der *A+W Business Pro*-Softwarereferenz und Tutorials |

### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

**Überblick**
Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
- **Lernziele:** Was soll vermittelt werden?
- **Nutzen:** Wofür können Sie dieses Wissen einsetzen?
- **Merksätze:** Welche Zusammenhänge müssen Sie sich merken?

**Konzepte**
Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

**Übungen**
Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.

**Querverweise**
Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

- **Kursiv**: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Nummernverwalter*.
- **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
- **>**: Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Fertigung > Kapazitätsplanung > Leitstand*.
- **[]**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten.
- **<>**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Menü-Übersicht
Die Kapazitätsplanung in *A+W Business Pro* gliedert sich in zwei Bereiche: das Einrichten der Kapazitätsplanung und die Planung und Überwachung der Kapazitäten. Die zugehörigen Dialoge finden Sie in den Modulen *Kapazitätsplanung* und *Fertigung*. Diese beiden Module werden im Folgenden kurz vorgestellt.

#### Modul Kapazitätsplanung
Im Modul *Kapazitätsplanung* richten Sie die Stammdaten und weitere Vorgaben für die Planung der Kapazitäten ein.

_Abb. H-1: Modul Kapazitätsplanung_

**Stammdaten**
Das Menü *Stammdaten* ist in drei Untermenüs gegliedert:
- **Allgemein:**
  In diesem Bereich richten Sie die allgemeinen Daten ein, z. B. Aggregat-Typen (Maschinentypen), Arbeitsarten, Übergangzeiten.
  ⇨ Softwarereferenz, "Allgemein" auf Seite H-189
- **Organisation:**
  In diesem Bereich richten Sie die Stammdaten zur betrieblichen Organisation ein, z. B. Produktionsbereiche, Maschinen, Kalender und Restriktionen.
  ⇨ Softwarereferenz, "Organisation" auf Seite H-199
- **Vorgabezeiten:**
  In diesem Bereich richten Sie die Daten zur Berechnung von Produktionszeiten ein, z. B. Vorgabezeiten und Sonderzeiten.
  ⇨ Softwarereferenz, "Vorgabezeiten" auf Seite H-223

**Zuordnen**
Hier ordnen Sie den Arbeitsarten z. B. die Produkte oder Warengruppen (WGR) zu. Zu einigen Arbeitsarten legen Sie einen Faktor für die Berechnung der Zeiten fest, wenn ein besonderer Aufwand dies erforderlich macht, z. B. bei der Fertigung von Modellen.
⇨ Softwarereferenz, "Zuordnen" auf Seite H-237

**Sperren**
Hier legen Sie fest, welche Maschinen nicht eingesetzt werden dürfen, wenn z. B. bestimmte Produkte oder Warengruppen in einem Auftrag erfasst sind.
⇨ Softwarereferenz, "Sperren" auf Seite H-254

**Übersicht**
Hier können Sie sich Übersichten über die Auslastung der Maschinen und Produktionsbereiche erstellen lassen.
⇨ Softwarereferenz, "Übersichten" auf Seite H-265

#### Modul Fertigung
Im Modul *Fertigung* lasten Sie die Aufträge in die Kapazitätsplanung ein und überwachen die Rückmeldungen aus der Produktion.
In diesem Modul finden Sie auch die Programmbereiche, in denen Sie die Aufträge an die Produktion übergeben. Diese werden im Part *Fertigung* beschrieben.

_Abb. H-2: Menü Kapazitätsplanung_

**Einlasten**
Im Menü *Einlasten* finden Sie folgende Dialoge:
- *Nummernverwalter:* Im Nummernverwalter sammeln Sie die Aufträge für die manuelle Einlastung.
- *Einlasten NV:* Über diesen Dialog lasten Sie die Aufträge ein.
- *Einlasten Auftrag:* Über diesen Dialog lasten Sie einen einzelnen Auftrag ein.
- *Aggregate Ausfall:* In diesem Dialog sperren Sie ein Aggregat für die Einlastung.
⇨ Softwarereferenz, "Einlastung" auf Seite H-277

**Fertigmeldung**
Im Menü *Fertigmeldung* finden Sie folgende Dialoge:
- *Datum:* In diesem Dialog melden Sie die Aufträge an einem Aggregat fertig.
- *Lauf:* In diesem Dialog melden Sie Aufträge pro Lauf fertig.
- *Manuell:* In diesem Dialog melden Sie Aufträge komplett oder in Teilen fertig.
⇨ Softwarereferenz, "Produktionsmeldungen" auf Seite H-301

**Produktionslisten**
Hier erstellen Sie pro Maschine Listen über die Stückzahlen, die gefertigt werden müssen.
⇨ Softwarereferenz, “Produktionsmeldungen" auf Seite H-301

**Fertigungsstand Auftrag**
Hier können Sie den aktuellen Stand der Fertigung pro Auftrag prüfen und ggf. ausgelassene Fertigmeldungen nachholen.
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-317

**Leitstand**
Hier prüfen Sie die Auslastung der Maschinen und schichten ggf. Aufträge um, indem Sie zugewiesene Aggregate, Schichten, Produktions- oder Liefertermine ändern.
⇨ Softwarereferenz, "Leitstand" auf Seite H-335

> **A+W Business Pro Capacity Planning vs. A+W Production Capacity Planning**
> In dieser Anleitung wird ist immer die Kapazitätsplanung in *A+W Business Pro* gemeint. Capacity Planning meint die Kapazitätsplanung von *A+W Production*.

### Grundgedanken der Kapazitätsplanung
Mit der Kapazitätsplanung können Sie die Auslastung Ihrer Produktionskapazitäten vorplanen und Produktions- und Zeitkosten ermitteln. Die Planungsdaten helfen Ihnen, Kapazitätsengpässe frühzeitig zu erkennen. Sie können dann in die Planung eingreifen und manuell korrigieren.

Dazu müssen Sie die Stammdaten der Kapazitätsplanung anlegen und so aufeinander abstimmen, dass die Abläufe in Ihrer Produktion abgebildet werden. Die nachfolgende Abbildung zeigt wie diese Stammdaten zusammenwirken am Beispiel der Vorgaben, aus denen die Termine für den Produktionsbeginn errechnet werden.

_Abb. H-3: Zusammenwirken der Stammdaten der Kapazitätsplanung_

In dieser Übersicht sehen Sie, wie z. B. Aggregate (Maschinen) bei der Planung der Kapazitäten eingesetzt werden:
- Für die einzelnen Arbeitsarten sind pro Aggregat Vorgabezeiten hinterlegt, aus denen die (freie) Kapazität und die benötigte Zeit für eine Auftragsposition berechnet werden.
- Pro Aggregat ist festlegt, an welchen Tagen es wie lange verplant werden kann (Schichtzeiten im Kalender).
- Aus den Zeiten, die eine Position in einem Produktionsbereich verweilt (Übergangsmatrix, Übergangzeiten), den Schichtzeiten (Kalender) und Vorgabezeiten wird der Termin für die Fertigung einer Auftragsposition berechnet.

Wenn die Stammdaten der Kapazitätsplanung erfasst sind, können die Aufträge in die Kapazitätsplanung eingelastet werden. Alle Auftragspositionen und deren Stücklisten-Komponenten werden den entsprechenden Arbeitsarten zugeordnet. Danach werden die benötigten Maschinenzeiten und die Kosten berechnet. Gleichzeitig wird der Liefertermin geprüft und der Termin zum Beginn der Produktion berechnet. Während und/oder nach der Einlastung können Sie in die Planung eingreifen und Arbeitsgänge einer Auftragsposition manuell auf andere gleichartige Maschinen umbuchen.

Die aktuelle Planung überwachen Sie im Dialog *Leitstand*. Von diesem Dialog aus können Sie in die Planung eingreifen und sich verschiedenen Übersichten und Grafiken zu Auslastung anzeigen lassen.

Bei Anbindung an die Produktionssoftware *A+W Production* werden die Ergebnisse der Kapazitätsplanung (Grobplanung) an *A+W Production* übergeben. Von *A+W Production* werden wiederum Rückmeldungen an *A+W Business Pro* übergeben, wenn Aufträge bzw. Positionen in der Produktion fertig gemeldet wurden. Dies führt in *A+W Business Pro* u. a. zur Erhöhung des Auftrags- bzw. Positionsstatus. Die Daten über Maschinenkosten und -zeiten werden nach der Fertigstellung des Auftrags aktualisiert.

> **Zeit- und Kostenermittlung**
> Aus den Vorgaben der Kapazitätsplanung werden die Zeit- und Maschinenkosten errechnet. Mit dieser Grobplanung wird auch geprüft, ob die Aufträge termingerecht versandfertig werden. Die Kapazitätsplanung in *A+W Business Pro* hat keinen Einfluss darauf, an welchen realen Maschinen im Produktionsprozess die Aufträge tatsächlich gefertigt werden.

### Nutzung der Kapazitätsplanung
Sie können mit der Kapazitätsplanung die Produktionskapazitäten aufgrund der Auftrags-, Maschinen- und Zeitdaten in *A+W Business Pro* planen. Dazu ist keine Anbindung an *A+W Production* erforderlich.

Folgende Hauptmerkmale charakterisieren die Kapazitätsplanung von *A+W Business Pro*:
- Flexibles Anlegen der Stammdaten für die Kapazitätsplanung
- Ermittlung von Kapazitätsengpässen
- Prüfung des Liefertermins
- Kalkulation der Produktionskosten
- Leitstand mit Übersichten und Funktionen zum Umlasten
- Bei Anbindung an die Produktions-Software *A+W Production*:
    - Übergabe der Plandaten an *A+W Production*
    - Rückmeldung der Ist-Daten an *A+W Business Pro*
    - Vergleich von Soll- und Ist-Werten

> **Begriffsklärung**
> In *A+W Business Pro* und in dieser Dokumentation werden die Begriffe Kapazitätsplanung und Zeitwirtschaft synonym verwendet.

## Stammdaten
Die Kapazitätsplanung kann mit Hilfe der Stammdaten an unterschiedliche Unternehmensstrukturen und Produktionsprozesse angepasst werden.
In diesem Themenblock lernen Sie, wie die Stammdaten der Kapazitätsplanung zusammenwirken und wie Sie diese Daten anlegen und pflegen.

Dazu gehören folgende Lerneinheiten:
- "Maschinen und Produktionsbereiche" auf Seite H-24
- "Schicht- und Arbeitszeiten" auf Seite H-38
- "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Rechteverwaltung
Fast alle Zugriffe auf die Stammdatendialoge der Kapazitätsplanung können über die Rechteverwaltung eingeschränkt werden. Damit kann die Kapazitätsplanung noch besser an die Abläufe in Ihrem Unternehmen angepasst werden. Das bedeutet aber auch, dass Sie die vollen Zugriffsrechte benötigen, wenn Sie die Übungen in diesem Tutorial nachvollziehen möchten.

### Historie
Jede Änderung des Auftragsstatus pro Produktionsbereich wird automatisch in der Auftrags-Historie dokumentiert. Damit können die Mitarbeiter, die nur Zugriffsrechte auf die Dokumente haben, immer erkennen, wann und welche Statusänderung im Auftragskopf durch die Kapazitätsplanung und die Rückmeldungen aus der Produktion verursacht wurde.

> **Stammdaten der Kapazitätsplanung**
> Die Stammdaten für Maschinen und Produktionsbereiche legen Sie im Modul *Kapazitätsplanung* an. Diese Stammdaten können nicht über die Dialoge im Modul *Stammdaten* angelegt werden.
> Wenn Sie die Einstellungen in den Stammdaten der Kapazitätsplanung geändert haben, müssen Sie *A+W Business Pro* neu starten, damit die Daten neu eingelesen werden.

### Reihenfolge zur Erfassung der Stammdaten
Beim Anlegen der maschinenbezogenen Stammdaten ist es sinnvoll, diese Reihenfolge einzuhalten:

1.  **Aggregattypen**, z. B. Schneidtische, ESG-Öfen, Versand usw.: Art und Umfang technischer Restriktionen von Maschinen werden u. a. über die Zuweisung zu Aggregattypen definiert.
2.  **Produktionsbereiche** (Arbeitszentren): Produktion und Versand werden in Bereiche unterteilt, z. B. Zuschnitt, Kantenbearbeitung, Bohren, Kontrolle, Verpacken, usw.
3.  **Arbeitseinheiten**: Zu jedem einzelnen Aggregat wird festgelegt, wie viele Arbeitseinheiten die Berechnungsgrundlage der Kapazität bilden.
4.  **Aggregate**, z. B. Bystronic-Schneidtisch, Lisec-Schneidtisch, ESG-Ofen A, ESG-Ofen B usw.: Nachdem Sie die Produktionsbereiche und Aggregattypen angelegt haben, erfassen Sie die einzelnen Maschinen und ordnen Sie den Produktionsbereichen und Aggregattypen zu.
5.  **Arbeitsarten** (Vorgänge): Alle Arbeiten, für die Zeiten berechnet werden, müssen als Arbeitsart definiert werden, z. B. Schneiden, Schleifen, Bohren, Verpacken usw.
6.  **Vorgabezeiten**: Die Zeiten für Arbeitsarten sind von den jeweiligen Maschinen abhängig. Die Zeiten der Arbeitsart Bohren sind z. B. von der Glasstärke und der Maschine abhängig, mit der gebohrt wird. Pro Maschine und Arbeitsart müssen daher Zeiten gemessen und erfasst werden. Über diese Vorgabezeiten werden den Arbeitsarten die Maschinen zugeordnet.
7.  **Zeitzuschläge**: Zusätzlich zu den Vorgabezeiten können Zeitzuschläge definiert werden, die auf den Basiswert aufgeschlagen werden, z. B. für den Zuschnitt von Modellen.

### Maschinen und Produktionsbereiche
**Lernziele**
- Zusammenhang von Aggregat-Typen und Aggregaten (Maschinen) kennenlernen.
- Produktionsbereiche anlegen.
- Arbeitsarten definieren und anlegen.

**Nutzen**
Mit den Stammdaten der Kapazitätsplanung bilden Sie die Abläufe in Ihrer Produktion ab. Damit beziehen sich die Plandaten auf die vorhandenen Maschinen.

> **Merke**
>
> **Aggregattyp**: Aggregattypen sind die Maschinentypen, die Sie in Ihrer Produktion einsetzen, z. B. Schneidtische, Bohrmaschinen, Schleifmaschinen, ESG-Öfen usw. Ein Aggregattyp kann mehrere einzelne Arbeitsstationen zusammenfassen, z. B. die ISO-Linie. Zu jedem Aggregattyp legen Sie fest, welche Restriktionen jeweils geprüft werden.
>
> **Aggregat**: Aggregate sind alle Stationen, an denen Zeiten verbraucht werden. Neben den eigentlichen Maschinen zum Schneiden, Bohren usw. gilt auch Kontrolle, Versand, Verpacken als Aggregat. In *A+W Business Pro* gibt es keine logischen Maschinen.
>
> **Produktionsbereich**: Produktionsbereiche fassen die Aggregate zusammen, die die gleichen Tätigkeiten ausführen oder in denen eine Folge von Tätigkeiten ausgeführt wird, z. B. ISO-Fertigung.
>
> **Arbeitsart**: Die Arbeitsart bezeichnet die Tätigkeit, die an einem Aggregat ausgeführt wird. Alle Tätigkeit, für die Zeiten berechnet werden, müssen als Arbeitsart definiert werden, z. B. Schneiden, Schleifen, Bohren, Verpacken usw.
>
> **Arbeitsgang**: Der Begriff bezeichnet in dieser Dokumentation, die Ausführung einer Arbeitsart für eine Auftragsposition. In der Regel sind in einer Auftragsposition mehrere Arbeitsgänge nötig.
>
> **Restriktionen**: Einschränkungen bei bestimmten Aggregaten (Maschinen), müssen geprüft werden.
> - Diese Prüfungen werden übergreifend für den Aggregattyp aktiviert.
> - In der Definition eines Aggregats legen Sie die Werte fest, die für die Prüfung herangezogen werden sollen und nicht über- oder unterschritten werden dürfen.

#### Aggregattypen und Aggregate
Als Aggregate werden in der Kapazitätsplanung alle die technischen Arbeitsmittel bezeichnet, an denen die Arbeitsschritte ausgeführt werden. Das können sowohl einzelne Maschinen als auch ganze Linien oder der Versand sein. Da unterschiedliche Maschinen gleiche Arbeitsschritte ausführen können, können jedem Aggregattyp mehrere Maschinen zugeordnet sein.

_Abb. H-4: Beispiel: Aggregattyp Zuschnitt und zugeordnete Aggregate_
_A: Aggregattypen und mögliche Restriktionsprüfungen_
_B: Liste der Aggregate zum Aggregattyp Zuschnitt_

Als Beispiel sehen Sie hier den Aggregattyp *Zuschnitt*, zu dem mehrere Aggregate (Maschinen) (B) gehören.

Bei der Planung der Kapazitäten werden die jeweils zur Verfügung stehenden Aggregate auf ihre Auslastung hin abgefragt. Dabei wird auch geprüft, ob beim jeweiligen Aggregattyp Einschränkungen (Restriktionen) geprüft werden müssen (A) und ob die für die Maschine hinterlegten Werte durch die Auftragsposition verletzt werden.

**Restriktionen**
Zu jedem Aggregattyp legen Sie fest, welche Restriktionen jeweils geprüft werden müssen.

**Beispiel**
Bei Aggregattyp *Zuschnitt* sollen folgende Werte geprüft werden:
- **Maße**: Einer der Schneidtische kann eine bestimmte Größe der Lagerplatten nicht mehr aufnehmen.
- **Einzelstärke**: Der Schneidkopf muss bei bestimmten Glasstärken geändert werden.
- **Gewicht**: Je nach Gewicht ist ein zweiter Werker erforderlich, der an nur einem der Schneidtische arbeitet.
- **Modell**: Der automatische Zuschnitt ist für Modelle nicht geeignet.
- **Drehbarkeit**: Ornamentgläser dürfen nicht gedreht werden.

Bei den Aggregaten sind die Felder freigeschaltet, in denen die Werte für die aktivierten Prüfungen eingetragen werden.

In dem Beispiel sollen für den Aggregattyp *Zuschnitt* die Maße und die Dicke des Glases geprüft werden. Dazu müssen die Werte hinterlegt werden, die nicht über- oder unterschritten werden dürfen.

_Abb. H-5: Prüfungswerte für Aggregat Automatischer Zuschnitt_
_A: Prüfung aktiviert: Werte für Höhe und Breite_
_B: Prüfung aktiviert: Wert für Dicke wird nicht geprüft_

In diesem Beispiel sehen Sie, dass das Aggregat *Zuschnitt* keine Schnitte unter 100 mm (A) machen kann. Außerdem kann es nur Glasstärken von 4 bis 10 mm (B) schneiden. Im *Handzuschnitt* könnte die Glasstärke z. B. zwischen 2 und 99 mm angegeben werden, was bedeutet, dass dann Auftragspositionen mit einer Glasstärke von 12 mm von Hand zugeschnitten werden müssen.

> **Aktivierte Restriktionsprüfungen**
> Wenn eine Restriktion geprüft wird, darf das entsprechende Feld nicht leer bleiben. Wenn der Wert nicht geprüft werden soll, tragen Sie in den Feldern Werte ein, die nicht unter- oder überschritten werden können, z. B. 0,1 und 9999.
> ⇨ "Produktionsbereich anlegen" auf Seite H-32

_Abb. H-6: Prüfungen für Aggregat Zuschnitt_
_A: Scheiben können gedreht werden_
_B: Prüfung aktiviert: Modelle sind nicht möglich_
_C: Prüfung für den Aggregattyp nicht aktiviert_
_D: Gewicht_

In diesem Beispiel sehen Sie, dass der Zuschnitt von Modellen bei dem Aggregat *Zuschnitt* nicht möglich ist. Darum wird die Auftragsposition geprüft und nicht an diese Maschine weitergegeben, wenn ein Modell enthalten ist. Für das Aggregat *Handzuschnitt* wäre der Modellzuschnitt möglich, die Checkbox ist dann markiert.

Beim Aggregat *Handzuschnitt* ist das Gewicht auf 30 kg eingestellt. Für den normalen Zuschnitt könnte hier z. B. das Gewicht 999 kg eintragen sein, weil die Scheiben automatisch transportiert werden.

**Zeit und Kosten pro Aggregat**
Zu jedem Aggregat (Maschine) hinterlegen Sie Angaben, aus denen die Kosten für die Maschine und die Zeit errechnet werden, die bei der Produktion einer Auftragsposition anfallen.
Aus den Angaben für die Zeit werden die Kapazitäten der einzelnen Maschine und des gesamten Produktionsbereichs berechnet.

_Abb. H-7: Angaben zur Berechnung von Zeiten und Kosten pro Aggregat (Maschine)_

Zu jedem Aggregat werden die Kosten hinterlegt, die pro Einheit entstehen. Die Anzahl der Einheiten pro Stunde ergibt sich aus der gemessenen Zeit für die Arbeitsart. Die Kapazität des Aggregats ergibt sich aus:
- Einheiten pro Stunde
- Anzahl der Stunden pro Schicht
- Anzahl der Schichten, in denen das Aggregat arbeitet.

Die Ermittlung der Einheiten pro Aggregat und die Berechnung der Zeit- und Maschinenkosten pro Auftrag sind in separaten Einheiten beschrieben.

Zur Definition der Daten eines neuen Aggregats gehören weitere Angaben, z. B. technische Restriktionen und Prioritäten, die in den folgenden Abschnitten beschrieben werden. Anschließend finden Sie dann eine ausführliche Handlungsanleitung, nach der Sie die Daten erfassen können.

Wie Sie die Auswahl eines Aggregats bei der automatischen Auslastung steuern können, lernen Sie in einer separaten Einheit.

#### Arbeitsarten
Arbeitsarten (Vorgänge, Tätigkeiten) bilden die Grundlage für die Produktionsreihenfolge. Den Arbeitsarten werden jeweils die Aggregate zugeordnet, die diese Arbeitsarten ausführen können. Eine Arbeitsart kann von mehreren Maschinen ausgeführt werden. Manche Aggregate können mehrere Arbeitsarten ausführen.

**Beispiel**
Arbeitsart *Polieren* kann auf mehreren Aggregaten ausgeführt werden:
- Einseitige Schleifmaschine
- Zweiseitige Schleifmaschine
- Schleifmaschine für Serien
- CNC-Maschine

Ein Produktionsprozess kann mehrere Arbeitsarten umfassen, z. B. bei der VSG-Fertigung eine Arbeitsart *VSG-Vorverbund* und eine Arbeitsart *VSG-Autoklav*.

_Abb. H-8: Arbeitsarten_
_A: Arbeitsarten für Zuschnitt_
_B: Reihenfolge-Ordnungsziffer_
_C: Kennzeichen für manuelle Auswahl_
_D: Ausweich-Arbeitsart_

In diesem Beispiel sehen Sie, dass für den Zuschnitt (A) mehrere Arbeitsarten eingerichtet sind: maschineller Zuschnitt, Handzuschnitt und Zuschnitt von VSG-Glas. Diese Unterscheidung ist notwendig, weil für diese Arbeitsarten unterschiedliche Maschinen eingesetzt werden und unterschiedliche Kosten anfallen.

Die Reihenfolge-Ordnungsziffer (B) gibt die Produktionsreihenfolge der einzelnen Arbeitsarten innerhalb der Kapazitätsplanung an. Die ersten Arbeitsarten betreffen in aller Regel den Zuschnitt, die anschließenden Arbeitsarten müssen dann so definiert werden, dass die Reihenfolge stimmt. Da z. B. bei der Fertigung einer ISO-Einheit auch eine ESG-Scheibe verwendet werden könnte, muss die Arbeitsart *ESG-Vorspannen* immer vor der *ISO-Fertigung* ausgeführt werden, sie hat also eine höhere Priorität als *ISO-Fertigung*.

Arbeitsarten, für die bei der Planung eine Maschine nur manuell ausgewählt werden darf, müssen gekennzeichnet werden (C), z. B. da Aggregat *Handzuschnitt*.

Den Arbeitsarten werden die Maschinen über die Vorgabezeiten zugeordnet. Die Vorgabezeiten werden ausführlich in der Einheit *Zeitvorgaben* beschrieben.
⇨ "Zeitvorgaben" auf Seite H-57

**Ausweich-Arbeitsart**
Ausweich-Arbeitsarten (D) werden festgelegt, um auf besondere Situationen zu reagieren, z. B. auf das Bohren dicker Scheiben, für die andere Zeiten und andere Aggregate erforderlich sind. Das System erkennt anhand der technischen Vorgaben und der Auftragsposition, wann die Ausweich-Arbeitsart gewählt werden muss und berechnet die Zeit und die Kosten dann entsprechend.

_Abb. H-9: Ausweicharbeitsart für dicke Scheiben_

In diesem Beispiel sehen Sie, dass die Ausweich-Arbeitsart gewählt wird, weil die Standard-Maschine die dicke Scheibe nicht bohren kann. Die Bohrmaschine II wird gewählt, weil der Ausweicharbeitsart diese Maschine zugewiesen ist.

> **Neue Arbeitsart anlegen**
> Planen Sie Ihre Arbeitsarten so, dass anhand der Nummer eine Gruppierung verwandter Arbeitsarten oder der Arbeitsarten eines Produktionsprozesses zu erkennen ist.

#### Produktionsbereiche (Arbeitszentren)
Ein Betrieb ist in der Regel in verschiedene Produktionsbereiche untergliedert, z. B. Zuschnitt, Schleiferei, Bohren usw. In jedem Produktionsbereich können mehrere Maschinen stehen, die von einer festen Anzahl von Werkern bedient werden. Gleichartige Maschinen können in unterschiedlichen Produktionsbereichen stehen.

_Abb. H-10: Produktionsbereiche_

Von den Produktionsbereichen werden Statusmeldungen aus der Produktion gesendet, wenn die Position fertig produziert ist. Dazu geben Sie die Erfassungsstelle an, von der die Meldung gesendet wird. In diesem Beispiel werden die Meldungen über die Betriebsdatenerfassung (BDE) gesendet.

Sie sehen, dass auch für den Versand ein Produktionsbereich angelegt ist. Dies ist wichtig, damit auch die Zeiten im Versand mit eingeplant werden und die Aufträge versandfertig gemeldet werden können.

Statusmeldungen können nur von Produktionsbereichen gesendet werden, nicht von Aggregaten. Wenn Sie z. B. bei der ESG-Fertigung zwei Statusmeldungen benötigen, müssen Sie dazu zwei Produktionsbereiche einrichten: ESG-Ofen und Heat-Soak.

#### Produktionsbereich anlegen
Wenn Sie die Produktionsbereiche ganz neu einrichten, sollten Sie zunächst planen, welche Maschinen und Arbeitsarten zu ihnen gehören.

**So legen Sie die Daten für einen Produktionsbereich an**
1.  Wählen Sie im Modul *Kapazitätsplanung > Stammdaten > Organisation > Produktionsbereich*. Der Dialog *Produktionsbereiche* wird geöffnet. Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln. Die Nummer des Produktionsbereichs wird automatisch eingesetzt und kann geändert werden.
    _Abb. H-11: Zeile für neuen Produktionsbereich eingefügt_
3.  Tragen Sie den Namen des Produktionsbereichs ein und überschreiben Sie ggf. die Nummer. Wenn Sie die Werte für die übrigen Felder bereits kennen, dann tragen Sie diese in die entsprechenden Felder ein.
4.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert. Sie können jetzt die Aggregate anlegen, die dem neuen Produktionsbereich zugeordnet werden sollen.

#### Aggregat anlegen
Sie können alle Daten eines neuen Aggregats einzeln eingeben. Wenn Sie jedoch bereits ein vergleichbares Aggregat in Ihrem Bestand haben, sollten Sie dessen Daten als Basis verwenden. Sie erleichtern sich damit die Arbeit erheblich. In der folgenden Handlungsanleitung wird dieser Weg vorgeführt.

**So legen Sie die Daten für eine neue Maschine an**
1.  Wählen Sie im Modul *Kapazitätsplanung > Stammdaten > Organisation > Aggregate*.
2.  Wählen Sie den Produktionsbereich aus, dem die neue Maschine zugeordnet werden soll, z. B. *Bearbeitungen*.
    _Abb. H-12: Produktionsbereich auswählen_
3.  Wählen Sie im Menü *Start > Suchen*, um die Daten der Maschinen aus diesem Produktionsbereich einzulesen. In der Übersicht (C) werden alle Aggregate aufgeführt, die diesem Produktionsbereich zugeordnet sind. Die Felder der Werte (A) sind mit den Daten des markierten Aggregats vorbelegt.
    _Abb. H-13: Aggregate im Produktionsbereich_
    _A: Vorbelegung der Felder mit den Daten des markierten Aggregats_
    _B: Nummer und Name des markierten Aggregats_
    _C: Liste der Aggregate im Produktionsbereich_
    _D: Erfassungsstelle, von der eine Fertigmeldung gesendet wird_
4.  Markieren Sie in der Übersicht das Aggregat, dessen Werte Sie übernehmen wollen.
5.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln. Das Feld für die Aggregatnummer (B) wird freigeschaltet.
6.  Überschreiben Sie die Nummer und den Namen des Aggregats.
7.  Wählen ggf. einen anderen Produktionsbereich aus.
8.  Passen in den Feldern für die Kosten (A) die Werte an.
9.  Tragen Sie im Feld *Erfassungsstelle* (D) die ID der Erfassungsstelle ein, von der die Fertigmeldung kommt.
10. Wählen Sie im Menü *Start > Speichern*, um die neuen Daten zu speichern.
    Damit haben Sie die neue Maschine angelegt. Die Maschine wird in der Übersicht aufgeführt. Sie können jetzt die Prüfungen (A) aktivieren und die Angaben für die technischen Restriktionen anpassen.
    _Abb. H-14: Werte für das Aggregat anpassen_
    _A: Prüfungen aktivieren_
    _B: Aggregat sperren_

> **Neues Aggregat sperren**
> Wenn Sie ein neues Aggregat angelegt haben, auf das noch nicht eingelastet werden soll, dann müssen Sie es unbedingt sperren (B).

**So passen Sie die technischen Restriktionen an**
1.  Wechseln Sie zum Register *Restriktionen*.
    _Abb. H-15: Technische Restriktionen anpassen_
    _A: Zugeordnete Arbeitsarten_
    _B: Technische Restriktionen_
2.  Prüfen Sie im Bereich *Technische Restriktionen* (B), welche Werte für die Maschine gelten. Wenn eine benötigte Prüfung gesperrt ist, haben Sie unter Umständen im Register *Aggregat* den falschen Aggregattyp zugewiesen. Wenn der Aggregattyp richtig eingestellt ist, sollten Sie im Dialog *Aggregattypen* prüfen, ob die Checkboxen für die Prüfungen korrekt markiert sind.
    > **Neue Restriktionsprüfung aktiviert**
    > Wenn Sie im Aggregattyp eine Restriktionsprüfung aktivieren, müssen Sie in allen Aggregaten die entsprechenden Felder füllen. Tragen Sie mindestens null (0) ein, damit das Feld nicht leer bleibt.
3.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
    Die Daten werden gespeichert. Die Angaben zu den zugewiesenen Arbeitsarten (A) werden erst angezeigt, wenn Sie diese in den Dialogen zur Zuordnung festgelegt haben.

#### Übungen
- Überlegen Sie, wie die Produktion räumlich organisiert ist und wie Sie diese Organisation in den Stammdaten mit Produktionsbereichen und Maschinen abbilden können.
- Legen Sie einen Produktionsbereich *ISO-2* und die zugehörigen Maschinen an.
- Die Übungen bauen aufeinander auf. Sie sollten sich daher mehrere unterschiedliche Maschinen anlegen, um in den Übungen der nächsten Einheiten Vergleichsmöglichkeiten zu haben.
- Legen Sie eine Arbeitsart für 3-fach-ISO an.

> **Übungen im realen Betrieb**
> Wenn Ihre Kapazitätsplanung bereits im Tagesgeschäft eingesetzt wird, dann müssen Sie neue Maschinen unbedingt sperren, damit diese nicht in der Planung berücksichtigt werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Aggregattypen" auf Seite H-189
⇨ Softwarereferenz, "Arbeitsarten" auf Seite H-192
⇨ Softwarereferenz, "Zugeordnete Aggregate" auf Seite H-195
⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-200
⇨ Softwarereferenz, "Aggregate" auf Seite H-201

### Schicht- und Arbeitszeiten
**Lernziele**
- Schichtzeiten und Kalender einrichten.
- Arbeitseinheiten kennenlernen.
- Kapazitäten pro Produktionsbereich und pro Aggregat berechnen.

**Nutzen**
Mit den hinterlegten Schichten und den Angaben zu Arbeitseinheiten wird die Kapazität eines jeden Produktionsbereichs errechnet. Anhand dieser Kapazität wird die Terminierung der eingelasteten Aufträge durchgeführt.

> **Merke**
>
> **Schicht**: Die Schichten in den verschiedenen Produktionsbereichen können unterschiedlich lang sein. Der Schichtbeginn muss für alle Produktionsbereiche zur selben Uhrzeit festgelegt werden, damit keine Überschneidungen beim Schichtwechsel und Übergang von einem zum nächsten Produktionsbereich entstehen.
>
> **Arbeitseinheit**: Mit Arbeitseinheiten geben Sie an, wie viel pro Stunde gefertigt werden kann. Arbeitseinheiten können als Mannstunden oder als Maschinenstunden angegeben werden.
>
> **Kapazität**: Die Kapazität einer Maschine ist das Produkt aus Arbeitseinheiten und Schichtstunden. Die Kapazität eines Produktionsbereichs ist die Summe aller Maschinenkapazitäten im Produktionsbereich.
>
> **Geschlossene Kapazität**: Bei geschlossenen Kapazitäten wird automatisch nach einem anderen Termin gesucht, wenn die verfügbaren Schichten und Maschinen ausgelastet sind.
>
> **Offene Kapazität**: Bei offenen Kapazitäten wird die Schichtzeit nicht geprüft.
>
> **Voreinstellungen**: Firmendaten: Register *Kapa-Planung > Anzahl der Schichten*.

#### Arbeitszeiten
Für die Berechnung von Terminen werden Vorgaben herangezogen, die Sie in unterschiedlichen Dialogen hinterlegen. Dies sind z. B. Werte für:
- Zeit, die eine Maschine eingesetzt werden kann (Schichtzeit).
- Zeit, die benötigt wird, um ein Stück zu fertigen (Vorgabezeit).
- Zeit, die mehr aufgewendet wird, wenn der Arbeitsgang aufwendiger ist (Zeitzuschlag).
- Rüstzeit.

Im Folgenden werden die Zusammenhänge der unterschiedlichen Zeitvorgaben und der Voreinstellungen für die Arbeitszeiten näher erklärt.

#### Arbeitstage und Schichten
Für die Terminberechnung in der Kapazitätsplanung ist es wichtig, ob Ihr Betrieb in Schichten arbeitet oder nicht.
- Wenn nicht in Schichten gearbeitet wird, greift die Kapazitätsplanung auf den *A+W Business Pro*-Standard-Kalender zu.
- Wenn in Schichten gearbeitet wird, können die Schichtzeiten pro Produktionsbereich hinterlegt werden.

Wenn nicht alle Produktionsbereiche in allen Schichten arbeiten, richtet sich die Anzahl der Schichten nach dem Produktionsbereich mit den meisten Schichten. Die Anzahl der Schichten legen Sie im Modul *Stammdaten > Firma > Firmendaten* fest.

_Abb. H-16: Firmendaten – Register Kapa-Planung_

Die Länge einer Schicht wird im Kalender pro Aggregat oder Produktionsbereich festgelegt. Wenn z. B. mehrere Produktionsbereiche in drei Schichten mit unterschiedlichen Schichtlängen arbeiten, dann müssen Sie die Schichten so einteilen, dass die Schichten 2 und 3 in allen Produktionsbereichen zur gleichen Uhrzeit beginnen.

Die Schichten der verschiedenen Produktionsbereiche dürfen sich zeitlich nicht überlagern, weil sonst der Übergang von einer Schicht in die nächste beim Wechsel des Produktionsbereichs nicht eindeutig ist.

**Beispiel**

| Produktions-Bereich | Beginn 1. Schicht | Anzahl Std. | Beginn 2. Schicht | Anzahl Std. | Beginn 3. Schicht | Anzahl Std. | Ende |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Zuschnitt | 06:00 | 6 | 12:00 | 4 | 16:00 | 4 | 20:00 |
| VSG | 08:00 | 4 | 12:00 | 4 | 16:00 | 4 | 20:00 |
| Bohren | 10:00 | 2 | 12:00 | 4 | 16:00 | 2 | 18:00 |
| Heat-Soak-Test | 08:00 | 12 | | 0 | | 0 | 20:00 |

Bei einer solchen Schichtorganisation ist gewährleistet, dass sich keine Arbeitsverzögerungen von einer Schicht zur anderen ergeben, da die Schichtwechsel in den Produktionsbereichen zur selben Zeit stattfinden.

Die Zeiten des Schichtwechsels legen Sie im Modul *Kapazitätsplanung > Stammdaten > Aggregate > Kalender >Menü Funktionen > Schichten* fest.

_Abb. H-17: Einstellungen für Schichtwechsel_

In diesem Beispiel sehen Sie, dass die Schicht 2 um 12:00 Uhr beginnt und um 16:00 Uhr endet. Darauf folgt, dass Schicht 1 bei einer Schichtzeit von 6 Std. um 6:00 Uhr beginnt. Der Übergang von Schicht 2 zu Schicht 3 ist um 16:00 Uhr, was bedeutet, dass die Schicht 2 nur 4 Stunden lang ist.

#### Maximale Kapazität pro Tag
Die Kapazität einer Maschine pro Tag wird in Arbeitseinheiten gerechnet. Die Kapazität für den jeweiligen Produktionsbereich setzt sich aus den Einheiten pro Stunde aller Maschinen zusammen, die zum Produktionsbereich gehören.

_Abb. H-18: Berechnungen von Zeiten pro Aggregat (Maschine) und Produktionsbereich_

Die maximale Kapazität einer Maschine ergibt sich aus den im Kalender eingetragenen Summen der Stunden pro Tag, multipliziert mit den Arbeitseinheiten pro Stunde, die für die Maschine im Dialog *Aggregat* hinterlegt sind.

**Beispiel**
Tag: Dienstag, Produktionsbereich Zuschnitt, Maschine Schneidtisch.
Am Schneidtisch können 4 Arbeitseinheiten pro Stunde gemacht werden.

| Schicht | Stunden | x 4 Arbeitseinh./Std | = Max. Arbeitseinh./Schicht |
| :--- | :--- | :--- | :--- |
| 1. Schicht | 6 Std. | x 4 A.Einh./Std. | = 24 A.Einh./Schicht |
| 2. Schicht | 4 Std. | x 4 A.Einh./Std. | = 16 A.Einh./Schicht |
| 3. Schicht | 4 Std. | x 4 A.Einh./Std. | = 16 A.Einh./Schicht |
| **Max. Kapazität pro Tag am Schneidtisch** | | | **= 56 A.Einh./Tag** |

Die Kapazität eines Produktionsbereichs ergibt sich aus der Summe der Tageskapazitäten aller Maschinen in diesem Produktionsbereich.

Sie müssen dabei jedoch berücksichtigen, ob alle Aggregate jederzeit einsetzbar sind. Wenn Sie z. B. 6 Schleifmaschinen haben, aber nur drei Werker, die an diesen Maschinen arbeiten können, können Sie die Gesamtkapazität nur für drei Maschinen berechnen. Die Prüfung der freien Kapazitäten bezieht sich daher nicht nur auf die Maschinen selbst, sondern auch auf die maximale Anzahl von Einheiten, die in einem Produktionsbereich gefertigt werden können.

_Abb. H-19: Anzahl der Einheiten_
_A: Einheiten im Produktionsbereich_
_B: Einheiten im Aggregat_

Wie Sie die Arbeitseinheiten bestimmen, lernen Sie in der folgenden Einheit.

#### Arbeitseinheiten
Arbeitseinheiten kann sowohl für jedes einzelne Aggregat als auch für den gesamten Produktionsbereich angegeben werden. Für beide Angaben legen Sie dieselbe Berechnungsart der Arbeitseinheit zugrunde.
Bevor Sie die Werte hinterlegen, müssen Sie festlegen, welche Arbeitseinheit verwendet wird. Es gibt viele Möglichkeiten, z. B.:
- Arbeitseinheit = Mannstunde
- Arbeitseinheit = Maschinenstunde

Folgende Fragen müssen Sie beantworten, um die Arbeitseinheiten pro Stunde und die Vorgabezeiten einrichten zu können:
- In welcher Arbeitseinheit soll die Kapazitätsberechnung der Maschine erfolgen? Was ist unter Mannstunde, Maschinenstunde usw. zu verstehen?
  ⇨ "Arbeitseinheit = Mannstunde" auf Seite H-44
  ⇨ "Arbeitseinheit = Maschinenstunde " auf Seite H-47
- Welcher Wert muss für die *Einheit/Std.* eingetragen werden?
  ⇨ Softwarereferenz, "Aggregate" auf Seite H-201
- Wie viel Zeit braucht die Maschine für eine Einheit (lfm, qm, Stück) bezogen auf die Arbeitseinheit?
  ⇨ "Ermittlung der Mannstunden" auf Seite H-45

##### Arbeitseinheit = Mannstunde
Anhand der Arbeitseinheiten wird beim Einlasten geprüft, ob noch Kapazitäten für diesen Tag zur Verfügung stehen.

**Beispiel**
Im Produktionsbereich *Bohren* (5 Maschinen) arbeiten 12 Personen in insgesamt drei Schichten pro Tag. Pro Schicht arbeiten also vier Personen. Diese vier Personen entsprechen vier Arbeitseinheiten im Produktionsbereich *Bohren*.
Auch wenn nur vier Personen im Produktionsbereich für fünf Maschinen zur Verfügung stehen, kann theoretisch jede Maschine die ganze Schichtzeit, z. B. acht Stunden, laufen. Das heißt, Sie tragen bei jeder Maschine die Arbeitseinheit gleich 1 ein. Welche vier der fünf Maschinen jedoch letztlich eingesetzt werden, hängt von den Einlastungsdaten ab.

Folgendes wird geprüft:
- Ist die Maschine ausgelastet?
- Wenn ja, stehen noch andere Maschinen zur Verfügung? Das heißt: Ist die maximale Kapazität des Produktionsbereiches von vier Arbeitseinheiten bereits erreicht?
  - Wenn ja, kann auf eine freie Maschine eingelastet werden.
  - Wenn nein, muss der Arbeitsgang auf den nächsten Tag oder die nächste Schicht verschoben werden oder es wird entschieden, dass Überstunden gemacht werden müssen.

> **Anwesende Werker**
> Die Kapazitätsplanung geht davon aus, dass immer alle Personen (Werker) da sind.

##### Ermittlung der Mannstunden
Um die Mannstunden zu ermitteln, müssen die Zeitwerte mit der Anzahl der Personen, die an der Maschine arbeiten, multipliziert werden. Je nachdem, ob Sie Einzelzeiten oder eine Staffelung, z. B. nach Dicke, definieren, wird die Vorgabezeit anders berechnet.
Die folgenden Beispiele sind reine Berechnungsbeispiele.

**Beispiel: 3 Personen, Einzelzeit**
Berechnung von Mannstunden am Schneidtisch:
- 3 Personen arbeiten am Schneidtisch.
- In einer Stunde können 200 qm zugeschnitten werden.
- Die Vorgabezeit wird als Einzelzeit hinterlegt.

**Formel:**
`Vorgabezeit 1 qm = (1 Std / Anzahl qm pro Stunde) x Anzahl Personen [Mannstunden]`

**Rechenbeispiel:**
`Vorgabezeit 1 qm = (1 Std / 200 qm) x 3 Personen = 0,015 [Mannstunden]`

**Beispiel: gestaffelte Zeit (Vektor)**
Berechnung von Mannstunden am Schneidtisch, gestaffelt nach Dicke:
- 3 Personen arbeiten am Schneidtisch.
- Gestoppte Zeit pro gefertigte Einheit, nach Dicke des Glases gestaffelt.
- Die Vorgabezeiten werden im Vektor-Format hinterlegt.

**Formel:**
`Vorgabezeit 1 qm = gestoppte Zeit x Anzahl Personen [Mannstunden]`

**Rechenbeispiel:**
`Vorgabezeit 1 qm Float 4 mm = 0,009 Std. x 3 Personen = 0,027 Mannstunden`
`Vorgabezeit 1 qm Float 6 mm = 0,010 Std. x 3 Personen = 0,03 Mannstunden`

**Beispiel: 2 Personen, Einzelzeit**
Berechnung von Mannstunden an der Schleifmaschine:
- 2 Personen arbeiten an der Schleifmaschine.
- In einer Stunde können 3 Laufmeter geschliffen werden.
- Die Vorgabezeit wird als Einzelzeit hinterlegt.

**Formel:**
`Vorgabezeit = (1 Std / Anzahl lfm pro Stunde) x Anzahl Personen [Mannstunden]`

**Rechenbeispiel:**
`Vorgabezeit = (1 Std / 3 lfm) x 2 Personen = 0,66 [Mannstunden]`

##### Arbeitseinheit = Maschinenstunde
Wenn die Zeiten unabhängig von der Anzahl der Werker an der Maschine sind, können Sie die Arbeitseinheit *Maschinenstunden* einsetzen.
In diesem Fall muss als Arbeitseinheit für das Aggregat immer eine 1 eingetragen werden.

_Abb. H-20: Dialog Aggregate - Einheiten und Kosten_

Standardmäßig wird der Wert 1 für die Anzahl der Einheiten eingegeben. Damit können Sie besser nachvollziehen, wie die Kapazitäten berechnet werden.

**Arbeitseinheiten pro Produktionsbereich**
Im Normalfall entspricht die Anzahl der Arbeitseinheiten je Produktionsbereich der Anzahl der Maschinen, die dort eingesetzt werden. Wenn 3 Maschinen eingesetzt werden, dann ist die Anzahl der Arbeitseinheiten gleich 3.

Die Bedingungen in einem Betrieb könnten jedoch folgendermaßen eingeschränkt sein:
- Sie setzen in Ihrem Produktionsbereich z. B. 3 Maschinen ein.
- Die Stromversorgung lässt aber nur den gleichzeitigen Betrieb von 2 Maschinen zu. Das heißt, dass eine Maschine immer abgeschaltet sein muss.

In diesem Fall müssen Sie als Arbeitseinheit pro Stunde für den gesamten Produktionsbereich dem Wert 2 eintragen.

_Abb. H-21: Einheiten pro Produktionsbereich_

#### Voreinstellungen für Schichten und Kapazitäten
Im Modul *Stammdaten* legen Sie die Grundeinstellungen für die Kapazitätsplanung in *A+W Business Pro* fest.

_Abb. H-22: Firmendaten – Kapa-Planung_
_A: Anzahl der Schichten_
_B: Auslastungsgrad festlegen_
_C: Einstellung für große Auftragspositionen_

Die Anzahl der Schichten (A) richtet sich nach dem Produktionsbereich, in dem die meisten Schichten gefahren werden. Die Schichten werden u. a. bei der Berechnung von Übergangsmatrix und Übergangszeiten berücksichtigt.

Sie müssen festlegen, ob Sie mit geschlossenen oder offenen Kapazitäten arbeiten wollen.
- Bei geschlossenen Kapazitäten wird automatisch nach einem anderen Termin gesucht, wenn die verfügbaren Schichten und Maschinen ausgelastet sind.
- Bei offenen Kapazitäten wird die Schichtzeit nicht geprüft.

Außerdem müssen Sie festlegen, wie stark eine Schicht ausgelastet werden darf, wenn die Aufträge automatisch an die Kapazitätsplanung übergeben werden. Wenn Sie die Schichten immer voll oder nahezu voll auslasten, haben Sie keinen Spielraum mehr für Umlastungen, für Eilaufträge oder für Restmengen vom Vortag.

Folgende Einstellungen im Feld *Fertigungsterminmodus* (B) stehen für den Auslastungsgrad zur Verfügung.
- **Automatisch Normalkapazität:** Die Aufträge werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung.
- **Automatisch volle Tage:** Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus. Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
- **Nur Aggregatwechsel:** Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet wird, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
- **Einlasten ohne Kontrolle:** Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist.

Große Positionen können auf mehrere Aggregate, Schichten oder Tage verteilt werden. Dazu geben Sie im Feld *Schichtfüllung bei Positionssplit* (C) an, zu wie viel Prozent die Schicht eines Aggregats durch das Splitting gefüllt werden darf, um Platz für andere Aufträge zu behalten.

> **Einstellungen ändern**
> Wenn Sie Einstellungen in den Firmendaten geändert haben, sollten Sie A+W Business Pro neu starten.

Die weiteren Einstellungen für Arbeitstage und Schichten werden Sie in den zugehörigen Lerneinheiten kennenlernen.

#### Kalender anpassen
Standardmäßig geht die Kapazitätsplanung von einer Schicht pro Tag aus. Wenn Sie jedoch in Ihrem Betrieb mit mehr als einer Schicht arbeiten wollen, dann müssen Sie als ersten Schritt die Anzahl der Schichten in den Firmendaten festlegen.

Danach können Sie pro Arbeitsart und Aggregat oder pro Produktionsbereich einen eigenen Kalender mit den jeweiligen Schichten bzw. Schichtzeiten anlegen. Wenn Sie für einen Produktionsbereich oder ein Aggregat keinen eigenen Kalender anlegen, gilt der allgemeine Kalender.

> **Jahreswechsel**
> Wenn Sie die Kapazitäten über den Jahreswechsel hinaus planen wollen, müssen Sie den Kalender für das neue Jahr mit allen Schichtzeiten angelegt haben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So legen Sie die Anzahl der Schichten fest" auf Seite H-50
- "So legen Sie einen neuen Kalender an" auf Seite H-51
- "So richten Sie weitere Schichtzeiten ein" auf Seite H-54
- "So richten Sie eine Sonderschicht ein" auf Seite H-55

> **Kalender ändern**
> Wenn Sie einen Kalender bearbeitet oder angelegt haben, müssen Sie A+W Business Pro neu starten, damit die Daten beim Einlasten zur Verfügung stehen.

**So legen Sie die Anzahl der Schichten fest**
1.  Wählen Sie im Modul *Stammdaten > Firma > Firmendaten*.
2.  Wechseln Sie zum Register *Kapa-Planung*.
3.  Tragen Sie im Bereich *A+W Business Kapazitätsplanung* die Anzahl der Schichten ein.
    _Abb. H-23: Firmendaten - Register Kapa-Planung_
4.  Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
    Die Daten werden gespeichert. Im Kalender der Kapazitätsplanung werden die Felder für die Schichtzeiten freigeschaltet.

**So legen Sie einen neuen Kalender an**
1.  Wählen Sie im Modul *Kapazitätsplanung > Stammdaten > Organisation > Kalender*.
    _Abb. H-24: Kalender anlegen_
2.  Wählen Sie den Modus (C):
    - **Arbeitsart/Aggregat:** Der neue Kalender soll für ein Aggregat und/oder eine Arbeitsart eingerichtet werden.
    - **Produktionsbereich/Mandant:** Der neue Kalender soll für einen Produktionsbereich und/oder einen Mandanten eingerichtet werden.
    Die Beschriftung der Felder (A) hängt vom Modus ab. In diesem Beispiel wird der Kalender für ein Aggregat angelegt.
3.  Wählen Sie die Arbeitsart und das Aggregat aus.
    > **Neues Kalenderjahr**
    > Beachten Sie, dass das neue Kalenderjahr, das Sie mit diesen Arbeitsschritten angelegt haben, nur für Arbeitsarten und Aggregate zur Verfügung steht. Wenn Sie auch für Produktionsbereiche ein neues Kalenderjahr anlegen wollen, wiederholen Sie die gesamte Handlungsanleitung für den jeweiligen Produktionsbereich.
4.  Wählen Sie das Jahr (B) aus. Wenn Sie eine neue Jahreszahl eingeben, wird der Kalender für dieses Jahr angelegt.
5.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
    _Abb. H-25: Kalender für Aggregat einrichten_
6.  Wechseln Sie zum Register *Kalender*.
    _Abb. H-26: Schichtzeiten eintragen_
7.  Tragen Sie pro Arbeitstag und Schicht die Schichtzeit (B) ein. Achten Sie darauf, dass die Checkboxen (A) der Tage, an denen Sie Schichtzeiten eingetragen haben, markiert sind. Wenn Sie die Zeiten eingetragen haben, werden die Schaltflächen zur Übertragung freigeschaltet.
8.  Klicken Sie auf die Schaltfläche **[Auf Jahr übertragen]** (D). Die Daten werden in die Übersicht *Kalender* (C) übernommen. Wenn Sie eine neue Jahreszahl eingegeben haben, wird der neue Kalender angelegt.
9.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert. Die Schicht wird bei der Planung berücksichtigt, nachdem Sie *A+W Business Pro* neu gestartet haben. Sie können nun die Schichtzeiten weiter bearbeiten.

**So richten Sie weitere Schichtzeiten ein**
1.  Wählen Sie im Modul *Kapazitätsplanung > Stammdaten > Organisation > Kalender*.
2.  Wählen Sie das aktuelle Kalenderjahr aus.
3.  Wählen Sie im Menü *Start > Suchen*, um die Suche zu starten. Alle Kalender, die den Auswahlkriterien entsprechen, werden eingelesen.
4.  Markieren Sie den gewünschten Kalender und wechseln Sie zum Register *Kalender*.
5.  Markieren Sie in der Übersicht *Kalender* eine Woche, damit die Schichtzeiten eingelesen werden.
6.  Tragen Sie im Bereich *Stunden pro Schicht* die Stunden für die neue Schicht ein. Achten Sie darauf, dass Sie die Stunden für alle Schichten eingetragen sein müssen. Wenn Sie die Felder der schon bestehenden Schichtzeiten leer lassen, werden die Zeiten bei der Übertragung auf die Woche oder das Jahr gelöscht.
    _Abb. H-27: Schichtzeiten ergänzen_
7.  Prüfen Sie, ob alle Checkboxen der Wochentage, für die Sie die Stunden eingetragen haben, markiert sind.
8.  Klicken Sie auf die Schaltfläche **[Auf Jahr übertragen]**. Damit werden die Schichtzeiten auf das gesamte Kalenderjahr übertragen.
9.  Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern. Die Daten werden gespeichert. Die Schichtzeiten werden bei der Planung berücksichtigt, nachdem Sie *A+W Business Pro* neu gestartet haben.

**So richten Sie eine Sonderschicht ein**
1.  Wählen Sie den gewünschten Kalender und wechseln Sie zum Register *Kalender*.
    _Abb. H-28: Sonderschicht einrichten_
    _A: Zeiten der Sonderschicht_
    _B: Kalenderwoche der Sonderschicht_
    _C: Zeiten übertragen_
2.  Wählen Sie die Kalenderwoche (B) aus, in der die Sonderschicht gefahren werden soll.
3.  Tragen Sie die Stunden (A) der neuen Sonderschicht ein.
4.  Klicken Sie auf die Schaltfläche **[Auf KW übertragen]** (C). Damit werden die Schichtzeiten nur für die gewählte Kalenderwoche übernommen.
5.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert. Die Sonderschicht wird bei der Planung berücksichtigt, nachdem Sie *A+W Business Pro* neu gestartet haben.

#### Übungen
- Skizzieren Sie auf Papier den Schichtenplan Ihrer Produktionsbereiche.
- Legen Sie fest, dass in 3 Schichten gearbeitet werden soll (Firmendaten!).
- Tragen Sie die Stunden im Kalender ein. Beachten Sie dabei, dass die Arbeitszeit in den verschiedenen Produktionsbereichen und an den verschiedenen Wochentagen unterschiedlich ist. Beispiel Versand: Sind 8 Stunden in Schicht 3 am Freitag sinnvoll?
- Erhöhen Sie die Anzahl der Schichten und prüfen Sie, wie sich dies im Kalender auswirkt.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Voreinstellungen Firmendaten" auf Seite H-183
⇨ Softwarereferenz, "Kalender" auf Seite H-211
⇨ Softwarereferenz, "Einstellungen Schichten" auf Seite H-187

### Zeitvorgaben
**Lernziele**
- Unterschiedliche Konzepte der Zeitberechnung kennenlernen.
- Zeitvorgaben definieren.

**Nutzen**
Anhand der zeitlichen Vorgaben und der freien Kapazitäten wird berechnet, wann welcher Produktionsschritt eines Auftrags ausgeführt werden kann.

> **Merke**
>
> **Vorgabezeiten**: Für alle Tätigkeiten (Arbeitsarten) werden die Zeiten gemessen, die benötigt werden, um diese eine Tätigkeit auszuführen. Diese gemessenen Zeiten werden als Vorgabezeiten angegeben.
>
> **Basiszeit**: Gestoppte Zeit, die eine Arbeitsart an einem Aggregat benötigt, um eine Einheit zu fertigen. Diese Zeit kann durch Zuschläge erhöht oder vermindert werden.
>
> **Zeitzuschlag**: Ein Zeitzuschlag ist ein Erschwerniszuschlag, z. B. für Mehrfach-ISO oder Modelle. Der Zeitzuschlag bezieht sich immer auf die Basiszeit, die für eine Arbeitsart an einem Aggregat hinterlegt ist. Zuschläge werden addiert. Die Basiszeit + 100% ergibt also eine Verdoppelung der Zeit.
>
> **Faktor**: Faktoren werden mit der Basiszeit der Arbeitsart multipliziert. Der Faktor 1 bedeutet, dass die Zeit nicht erhöht wird. Der Faktor 0,5 bedeutet, dass die Zeit um die Hälfte reduziert wird.
>
> **Sonderzeiten**: Sonderzeiten sind immer Zuschläge auf die Basiszeit einer Arbeitsart. Sonderzeiten werden verwendet, um z. B. darauf zu reagieren, wenn zwei Werker statt eines einzelnen eine Maschine bedienen müssen. Sonderzeiten können gestaffelt angegeben werden.
>
> **Übergangszeiten**: Die Übergangszeit gibt an, wie lange eine Einheit braucht, um von einem Arbeitsgang oder einem Produktionsbereich zum nächsten zu kommen. Die Zeit wird in Schichten angegeben.
>
> **Verweilzeiten**: Diese Zeiten geben an, wie lange eine Einheit in einem Produktionsbereich verweilt.
>
> **Rüstzeiten**: Rüstzeiten werden als Arbeitsart definiert und dem Aggregat und der Bearbeitung zugeordnet.

#### Basiskomponenten der Zeitplanung
In die Planung der Zeit fließen neben der Stückzahl aus dem Auftrag folgende Vorgaben ein:

_Abb. H-29: Zeiten_

In dieser Übersicht sehen Sie, welche Zeitvorgaben definiert werden können:
- **Vorgabezeiten**: geben an, wie viel Zeit eine Arbeitsart an einer bestimmten Maschine benötigt. Diese Zeiten werden im Dialog *Vorgabezeiten* hinterlegt.
- **Zeitzuschläge**: sind in der Regel gestaffelte Zuschläge, die unter bestimmten Voraussetzungen die Vorgabezeiten bei rechteckigen Scheiben erhöhen. Diese Zeiten werden im Dialog *Sonderzeiten* hinterlegt.
- **Zeitzuschläge und Faktoren**: erhöhen oder vermindern unter bestimmten Voraussetzungen die Vorgabezeit bei der Fertigung von nicht rechteckigen Scheiben (Modellen). Diese Zeiten werden in den Dialogen im Menü *Zuordnen* hinterlegt.
- **Verweiltage**: geben an, wie lange eine Einheit in einem bestimmten Produktionsbereich verweilt. Diese Zeiten werden im Dialog *Produktionsbereich* hinterlegt.
- **Übergangszeiten**: geben an, wie lange eine Einheit braucht, um von einer bestimmten Arbeitsart zur einer bestimmten anderen oder von einem bestimmten Produktionsbereich in einen bestimmten anderen zu kommen. Diese Zeiten werden in den Dialogen *Übergangsmatrix* und *Übergangszeiten* hinterlegt.
- **Rüstzeiten**: geben an, wie viel Zeit benötigt wird, um eine Maschine für den nächsten Arbeitsgang einzurichten. In der Regel werden Rüstzeiten als Zeitzuschlag festgelegt.

In den folgenden Einheiten werden die Konzepte erläutert, mit denen Sie diese Zeitkomponenten einsetzen. Daran anschließend wird anhand der Dialoge in Handlungsabläufen gezeigt, wie Sie die verschiedenen Vorgaben hinterlegen.

> **Stammdaten bearbeiten**
> Wenn Sie im Modul *Kapazitätsplanung* die Stammdaten - und dabei insbesondere die Zeitvorgaben - bearbeitet haben, sollten Sie die Kapazitätsplanung neu starten.

#### Vorgabezeiten
Vorgabezeiten werden für jede einzelne Arbeitsart pro Aggregat angegeben. Diese Zeiten können mit bis zu drei Grenztypen gestaffelt werden.

_Abb. H-30: Vorgabezeiten_
_A: Register für gestaffelten Zeiten_
_B: Priorität bei gleichartigen Aggregaten_
_C: Auswahl Zuschläge (Sonderzeiten)_
_D: Arbeitsart_
_E: Aggregat, für das die Zeit angelegt ist_
_F: Typ der Vorgabezeit_

Für alle Tätigkeiten werden die Zeiten pro Maschine und Einheit gestoppt. Ob Sie die Zeiten pro Stück, qm oder Kantenlänge stoppen, hängt von dem zu fertigenden Produkt, der Arbeitsart und der Maschine ab. Je nach definierter Arbeitseinheit wird auch die Anzahl der Werker einbezogen, die an der Maschine arbeiten. Diese Zeiten hinterlegen Sie für jede Maschine und alle die Arbeitsart, die an der Maschine ausgeführt werden.

**Typ der Vorgabezeit**
Die Vorgabezeiten können auf unterschiedliche Weise in die Berechnung einfließen. Dabei unterscheidet *A+W Business Pro* vier verschiedene Typen (F):
- **Basiszeit:** Das ist die gestoppte Vorgabezeit für eine Arbeitsart, z. B. für die Arbeitsart *Zuschnitt*. Da der Zeitbedarf für einen Arbeitsgang i. d. R. von der Größe abhängig ist, können diese Zeiten mit bis zu drei Grenztypen gestaffelt werden.
- **Zeitzuschlag:** Ein Zeitzuschlag wird z. B. für das Zuschneiden von Modellen benötigt. Das bedeutet, dass für das Zuschneiden von Modellen keine eigene Vorgabezeit gemessen wird, sondern die normale Vorgabezeit um einen Zuschlag erhöht wird. Die Zeitzuschläge werden ausführlich in einer separaten Einheit besprochen. ⇨ "Arbeitsarten und Zeitzuschläge" auf Seite H-64
- **Alternativer Vorgang:** Diese Vorgabezeit wird nur herangezogen, wenn für die Arbeitsart eine alternative Arbeitsart existiert. In diesem Fall müssen Sie im Feld *altern. Masch.-Nr.* die alternative Maschinennummer eintragen.
- **Alternative ohne Stückliste:** Als VSG-Produzent ist Ihr VSG-Artikel standardmäßig mit einer Stückliste hinterlegt. Wenn aber z. B. eine VSG-Scheibe in einzelnen Fällen nicht produziert, sondern direkt aus einer VSG-Platte geschnitten werden soll, dann darf die Stückliste in der Produktion nicht berücksichtigt werden. Für die Arbeitsart *VSG schneiden* müssen Sie die Option *Alternative ohne Stückliste* einsetzen. In diesem Fall müssen Sie im Feld *altern. Masch.-Nr.* die alternative Maschinennummer eintragen.
- **Vorgang ignorieren:** Bei einem Eckausschnitt fallen z. B. 3 Arbeitsgänge an: 1. Bohren (von Eckloch), 2. Zuschnitt und 3. Schleifen. Die CNC-Maschine kann alle drei Vorgänge als einen Arbeitsgang ausführen, d. h., dass Sie dann nur der Arbeitsart *Bohren* eine Vorgabezeit zuweisen müssen. Den anderen beiden Arbeitsarten weisen Sie auf dieser Maschine den Wert *Vorgang ignorieren* zu.

**Priorität**
Wenn mehrere Maschinen für eine Arbeitsart zur Verfügung stehen, müssen Sie festlegen, welche Maschine bei der Suche nach freien Kapazitäten zuerst abgefragt wird.

Wenn zwei Maschinen die gleiche Priorität (B) haben, dann prüft die Kapazitätsplanung die Kosten, die pro Maschine definiert sind. In diesem Fall wird automatisch die günstigere Maschine ausgewählt.

Wenn Sie keine Kosten pro Maschine hinterlegen, muss die Priorität bei gleichen Maschinen eindeutig sein, d. h. unterschiedlich.
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichwertigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

**Grenztypen und Staffelung**
Die Zeiten können mit bis zu drei Grenztypen gestaffelt werden:
- **Vektor:** Bei einem Vektor erfassen Sie Zeiten in Abhängigkeit von einem Grenztypen, z. B. Meter, Fläche.
- **Matrix:** Bei einer Matrix erfassen Sie Zeiten in Abhängigkeit von zwei Grenztypen, z. B. Breite und Höhe. Dabei haben Sie die Möglichkeit, die Matrix in Dreiecksform anzulegen, so dass die Grenztypen austauschbar sind, z. B. Höhe und Breite.
- **Würfel:** Der Würfel wird ähnlich wie die Matrix-Zeiten aufgebaut, bietet jedoch drei Grenztypen, z. B. Breite, Höhe und Dicke.

Die Grenztypen und Staffelungen haben Sie bei der Preisdefinition in der Schulung der Stammdaten kennengelernt. Eine Übersicht über die verfügbaren Grenztypen finden Sie im Part *Stammdaten*.

**Dreiecksform**
Sie können in einer Matrix oder in einem Würfel Zeiten so erfassen, dass die angegebenen Grenzwerte vertauscht werden dürfen, z. B. Höhe und Breite. Damit müssen Sie nur jeweils eine der Kombinationen erfassen.

**Zeiten in Stunden**
Die Zeiten werden nicht in Minuten sondern in Stunden hinterlegt. Das bedeutet, dass Sie die in Minuten gemessenen Zeiten in Stunden umrechnen müssen.

**Beispiel**

| Minuten | Eintrag des Zeitwerts (in Stunden) |
| :--- | :--- |
| 60 | 1 |
| 30 | 0,5 |
| 15 | 0,25 |
| 7,5 | 0,125 |
| 3,75 | 0,0625 |
| 1,875 | 0,03125 |

Wenn Sie also für eine Arbeitsart die Zeit 2,5 Minuten gemessen haben, tragen Sie dafür den Zeitwert **0,0417** als Basiswert ein.

> **Vorgabezeit kopieren**
> Wenn zwei gleichartige Maschinen die gleiche Zeit benötigen, können Sie mit der Kopierfunktion die Zeiten von einer Maschine auf die andere übertragen und anpassen. Dies ist besonders hilfreich bei gestaffelten Zeiten.

#### Sonderzeiten
Die gemessenen Zeiten können nicht eingehalten werden, wenn z. B. eine besonders große Scheibe in der Produktion mehr Zeit benötigt. Für solche Fälle definieren Sie eine Sonderzeit als Zuschlag, die in der Regel auf die Basisposition aufgeschlagen wird.

Sonderzeiten bieten sich an, wenn Größe, Material oder Dicke der Scheibe eine besondere Herausforderung darstellen.

_Abb. H-31: Dialog Sonderzeiten_
_A: Nummer der Zuschlagstabelle_
_B: Gestaffelter Zuschlag_
_C: Grenzwert (1, 2)_
_D: Grenztyp (1, 2)_
_E: Höhe des Zuschlags_
_F: Einheit, auf die sich der Zuschlag bezieht_
_G: Zuschlagsart_

In diesem Beispiel sehen Sie, dass die Zeit der Basisposition um 100% erhöht wird, wenn die Scheibe besonders klein (kleinste Kantenlänge 300 mm) ist oder wenn sie besonders groß (Breite über 1400 mm, Höhe über 2400 mm) ist. Der Bereich zwischen diesen Maßen wird ohne Zeitzuschlag kalkuliert.

Sonderzeiten werden in der gleichen Weise angelegt wie die *Sonstigen Zuschläge* der A+W Business Pro-Stammdaten.

#### Arbeitsarten und Zeitzuschläge
In der Regel legen Sie für jede Tätigkeit eine eigene Arbeitsart an und hinterlegen für diese dann eine Basiszeit (Vorgabezeit). Wenn Sie Tätigkeiten zu einem Arbeitsgang zusammenfassen können, muss die grundlegende Tätigkeit durch einen Faktor erhöht werden.

**Beispiel**
Die Fertigung einer Einheit 3-fach ISO dauert 2,5-mal so lange wie die Fertigung einer ISO-Einheit mit zwei Scheiben.
An der ISO-Linie geben Sie einen Faktor an, der den Wert der Basiszeit (für das 2-Fach-ISO) entsprechend erhöht.
Dazu finden Sie ausführliche Berechnungsbeispiele unter:
⇨ "Fallbeispiel ISO und Modell" auf Seite H-65

Auch ein Mehraufwand für Modelle wird als Vorgabezeit vom Typ *Zeitzuschlag* für die jeweilige Arbeitsart hinterlegt.
Für jeden Zeitzuschlag, den Sie definieren wollen, müssen Sie eine Arbeitsart einrichten. Das bedeutet, dass Sie z. B. eine Arbeitsart für den Zuschnitt von Modellen und eine Arbeitsart für die Bearbeitung von Modellen einrichten müssen.

Einfacher ist es jedoch, wenn Sie eine Arbeitsart *Modellzuschläge* einrichten und die Höhe des jeweiligen Zeitzuschlags für diese Arbeitsart bei den Aggregaten definieren, an denen die Arbeitsart ausgeführt wird.

_Abb. H-32: Arbeitsart Modellzuschläge für Zeitzuschläge an unterschiedlichen Maschinen_

> **Umlasten von Aufträgen bei Engpässen**
> Mit Zeitzuschlägen vereinfachen Sie außerdem die Vorgänge beim Umlasten. Wenn Sie z. B. die Produktion einer (komplexen) ISO-Einheit ohne Zeitzuschläge verschieben müssen, kann das bedeuten, dass Sie alle vorgelagerten Arbeitsgänge einzeln verschieben müssen.

Modelle gehören zur Stammdaten-Produktart *Modelle*. Durch die Zuordnung der Produktart *Modelle* zur Arbeitsart *Modellzuschläge* werden die Modelle beim Einlasten erkannt. Die Zeiten pro Auftragsposition werden dann bei Modellen um den Zuschlag erhöht, der an der jeweiligen Maschine hinterlegt ist. Diese Zuordnungen werden Sie im nächsten Themenblock kennenlernen.
⇨ "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

#### Fallbeispiel ISO und Modell
Die Fertigung von ISO-Einheiten mit drei und mehr Scheiben und als Modell erfordert viele Zeitvorgaben. Ein mögliches Konzept soll in diesem Beispiel vorgestellt werden. Dabei wird angestrebt, die Vorgaben so einzurichten, dass sie zur Berechnung von ISO-Scheiben und Modellen angewendet werden können und der Aufwand zum Einrichten und zur Pflege der Daten verringert wird.

_Abb. H-33: Definition der Vorgaben für Beispiel ISO-Fertigung_

**Vorgaben**
Im Folgenden werden die Vorgaben gezeigt, die in den verschiedenen Dialogen hinterlegt werden müssen. Genauere Handlungsanleitungen finden Sie im Anschluss an das Beispiel. Das Beispiel geht von folgenden Vorgaben aus:
- Die Tageskapazität von 450 ISO-Einheiten ergibt: 8 Std. / 450 Einheiten = 0,018 Std. pro Einheit.
- Für die ISO-Linie ist daher eine Vorgabezeit als Einzelzeit vom Typ *Basiszeit* hinterlegt.
_Abb. H-34: Dialog Vorgabezeit – Einzelzeit für ISO-Einheit_
- Für Modellzuschläge und 3-Fach-ISO sind gleichnamige Arbeitsarten angelegt.
_Abb. H-35: Arbeitsarten für Modelle und 3-fach-ISO_
- Die Produktart *Modelle* ist der Arbeitsart *Modellzuschläge* zugeordnet.
_Abb. H-36: Zuordnung der Produktart zur Arbeitsart Modellzuschläge_
- Als Vorgabezeit für die Arbeitsart *Modellzuschläge* wird ein Zeitzuschlag von 50% am Aggregat *ISO-Linie* berechnet.
_Abb. H-37: Dialog Vorgabezeit – Zeitzuschlag für Modelle_
- 3-fach ISOs sind in der Produktgruppe *Dreifach ISO* zusammengefasst.
- Der Produktgruppe *Dreifach ISO* wird die Arbeitsart *ISO Fertigen* zugeordnet.
- Für 3-fach ISO soll der Faktor 2,5 berechnet werden.
_Abb. H-38: Zuordnungen Dialog Produktgruppe – Faktor für 3-fach ISO_
- Außerdem soll ein Zuschlag für Übergrößen berechnet werden. Dieser ist als Sonderzuschlag angelegt.
_Abb. H-39: Dialog Sonderzeit – Sonderzuschlag für große und kleine Scheiben_

**Faktoren und Zuschläge bei der Berechnung**
Faktoren werden mit der Basiszeit des Arbeitsgangs multipliziert. Der Faktor 1 bedeutet, dass die Zeit nicht erhöht wird. Der Faktor 0,5 bedeutet, dass die Zeit um die Hälfte reduziert wird.

Sonstige Zuschläge werden als prozentuale Zuschläge addiert. Die Basiszeit + 100% ergibt also eine Verdoppelung der Zeit. Diese Zuschläge sind als Sonderzeiten über Zuschlagstabellen angelegt und werden der Vorgabezeit zugeordnet.

Im Einlastungsergebnis werden nur Zeiten für die Arbeitsarten angezeigt für die eine Basiszeit hinterlegt ist. Alle Zeitzuschläge, die auf Basiszeiten aufgeschlagen werden, sind in diesen Ergebnissen enthalten und werden nicht ausgewiesen.

#### Berechnungsreihenfolge für Zuschläge und Faktoren

| Position | Berechnung | Zeit (Std.) |
| :--- | :--- | :--- |
| ISO | Zeit | 0,018 |
| ISO + Modell | 0,018 + Zeitzuschlag 50% | 0,018 + 0,009 = 0,027 |
| ISO + Übergröße | 0,018 + Sonderzuschlag 100% | 0,018 + 0,018 = 0,036 |
| ISO + Modell + Übergröße | 0,018 + Zeitzuschlag 50% = 0,027 + Sonderzuschlag 100% | 0,018 + 0,009 + 0,027 = 0,054 |
| 3-fach ISO | 0,018 x Faktor 2,5 | 0,018 x 2,5 = 0,045 |
| 3-fach ISO + Modell | 0,018 x Faktor 2,5 + Zeitzuschlag 50% | 0,0450 + 0,0225 = 0,0675 |
| 3-fach ISO + Übergröße | 0,018 x Faktor 2,5 + Sonderzuschlag 100% | 0,045 + 0,045 = 0,090 |
| 3-fach ISO + Modell + Übergröße| 0,018 x Faktor 2,5 + Zeitzuschlag 50% + Sonderzuschlag 100%| 0,0450 + 0,0225 = 0,0675 + 0,0675 = 0,1350 |

Aus diesen Beispielen sehen Sie, in welcher Reihenfolge Faktoren, Zuschläge und Sonderzuschläge in die Berechnung einfließen.

#### Übergangsmatrix und Übergangszeiten
Neben der Zeit für den Arbeitsgang benötigen die Einheiten zusätzlich Zeit, um von einem Produktionsbereich zum nächsten zu gelangen.
Diese Zeiten werden als Verweil- und Übergangszeiten in folgenden Dialogen hinterlegt:
- **Produktionsbereich:** Welche Zeit bleibt eine Einheit in einem Produktionsbereich? Die Dauer wird in Tagen oder Bruchteilen von Tagen angegeben. Bei dieser Angabe wird der nachfolgende Produktionsbereich nicht berücksichtigt. ⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-200
- **Übergangszeiten:** Welche Zeit benötigt eine Einheit, um von einer Arbeitsart zur nächsten oder von einem Produktionsbereich in den Folge-Bereich zu kommen? Die Dauer wird in Schichten angegeben. ⇨ Softwarereferenz, “Übergangszeiten" auf Seite H-197
- **Übergangsmatrix:** Welche Zeit benötigt eine Einheit, um von einem Produktionsbereich in den nächsten Produktionsbereich zu gelangen? Die Dauer wird in Tagen oder Bruchteilen von Tagen angegeben. ⇨ Softwarereferenz, “Übergangsmatrix" auf Seite H-216

Wenn zur Zeitkalkulation für eine Auftragsposition in allen drei Dialogen Werte gefunden werden, berücksichtigt das Programm jeweils den größeren Wert. Zusätzlich wird die Anzahl der Schichten berücksichtigt, in denen die einzelnen Bereiche arbeiten.
Schichten und Tage können auch in Werten <1 eingegeben werden. Wie groß die Zeit dann letztlich ist, hängt von den Schichten und den Zeiten des Arbeitstags ab, die im Kalender definiert sind.

**Beispiel**
Wenn für die Übergangzeit der Wert 0,1 (Schichten) eingetragen ist, liegt genau eine Schicht zwischen den Arbeitsgängen.
⇨ Softwarereferenz, "Beispiele für die Berechnung des Übergangs" auf Seite H-218

> **Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität *Normal* auch z. B. die Priorität *Eilt* berücksichtigt werden soll, dann müssen dafür eigene Werte für die Übergangsmatrix und Übergangszeiten eingerichtet sein. Dies gilt für alle Zeiten, die für Eilaufträge auch verkürzt werden können.

**Zusammenwirken von Verweil- und Übergangszeiten**

_Abb. H-40: Beispiel 1: Verweiltage im Bereich + Übergangsmatrix_
Nach dem Zuschnitt am Donnerstag in Schicht 1 verbleibt die Position einen Tag im Produktionsbereich Heat-Soak, bevor sie am Freitag in Schicht 1 in den Versand geht. Berücksichtigt wird hier der größere Wert (1T) aus der Übergangsmatrix und nicht die Verweiltage (0,2 T) im Produktionsbereich.

_Abb. H-41: Beispiel 2: Verweiltage im Bereich + Übergangsmatrix_
Bei einem späteren Zuschnitt am Donnerstag Schicht 3 würde die Position am Freitag in Schicht 1 im Heat-Soak sein und am Freitag in Schicht 3 im Versand.

_Abb. H-42: Beispiel 3: Verweiltage im Bereich + Übergangszeit_
Anders sieht dieses Beispiel aus, wenn das ESG in eine ISO-Einheit eingebaut werden soll und für die Folge-Arbeitsart eine Übergangszeit definiert ist: Nach dem Zuschnitt am Donnerstag in Schicht 1 könnte das ESG zwar am Donnerstag in Schicht 3 in den Folge-Bereich kommen, aber erst am Freitag in Schicht 2 in das ISO eingebaut werden, denn der Übergang zur Folge-Arbeitsart beträgt 3 Schichten.

_Abb. H-43: Beispiel 4: Verweiltage im Bereich + Übergangszeit_
Bei einem späteren Zuschnitt am Donnerstag in Schicht 3 würde das ESG erst am Montag in Schicht 1 in das ISO eingebaut werden.
Weitere Berechnungsbeispiele finden Sie unter: ⇨ "Terminberechnung" auf Seite H-114

**Formel für Übergangszeit**
Wenn z. B. 50 Scheiben vom Zuschnitt zum Nassbereich kommen müssen, wird die Zeit in Tagen oder Schichten nur unzureichend genau berechnet. Für diese Fälle kann eine Formel hinterlegt werden, die die Anzahl der Scheiben berücksichtigt.

_Abb. H-44: Übergangsmatrix und Formel_

In diesem Beispiel sehen Sie, dass für den Wechsel von der ESG-Fertigung zum Versand die Formel 500 eingetragen ist. In der Formel ist festgelegt, dass die Zeit auf 1 (= 1 Tag) gesetzt ist. Ab der Stückzahl 11 soll die Zeit mit 3 Tagen berechnet werden.

Um die Formel im Dialog *Übergangsmatrix* auszuwählen, setzen Sie den Cursor in das Feld *Übergangszeit* und drücken die rechte Maustaste.

Die Formel selbst wird über *A+W Business Pro-Stammdaten > Firma > Formeln* angelegt. Im Dialog *Formelverwaltung > Register Formel* kann die Formel eingetragen und bearbeitet werden.

Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

#### Rüstzeiten
Rüstzeiten werden als Arbeitsart definiert und dem Aggregat und der Bearbeitung zugeordnet. Folgende Schritte sind dazu notwendig:
- Arbeitsart *Rüstzeit* anlegen.
- Arbeitsart *Rüstzeit* dem Aggregat als Typ *Basiszeit* zuordnen, z. B. der CNC-Maschine.
- Einzelzeit mit der Einheit *Stk* (einmal) festlegen, denn die Maschine wird pro Arbeitsgang nur einmal eingerichtet.
- Arbeitsart den Produktgruppen zuordnen, die auf dem Aggregat gefertigt werden, z. B. Produktgruppe Bearbeitungen/Eckausschnitte an der CNC-Maschine.
- Fertigungsstraße definieren, um die Rüstzeit für aufeinanderfolgende Bearbeitungen nicht doppelt zu berechnen.

_Abb. H-45: Arbeitsart Rüstzeit für Folge-Aggregat sperren_

In diesem Beispiel sehen Sie, dass die Rüstzeit für das Aggregat CNC-Maschine übersprungen wird, wenn das Folge-Aggregat wieder die CNC-Maschine ist. Die Maschine wird dann einmal für alle aufeinander folgenden Bearbeitungen eingerichtet.

Wenn die CNC-Maschine für die nachfolgende Bearbeitung aber neu eingerichtet werden muss, müssen die Rüstzeiten gesondert angelegt und berechnet werden. Sie können dann durch die Definition einer Fertigungsstraße gesperrt werden.

#### Zeitfaktoren für Serien
Für Serien kann der normale Zeitbedarf durchaus sinken, da z. B. Rüstzeiten entfallen. Die Maschine steht also früher wieder zur Verfügung und kann für den nächsten Auftrag eingeplant werden.

Für diese Zeitkalkulation legen Sie Serientabellen mit den Faktoren für die Serienfertigung an.

_Abb. H-46: Serienfaktoren_

In diesem Beispiel sehen Sie einen gestaffelten Abschlag für die Berechnung des Zeitbedarfs. Wie hoch die Reduktion tatsächlich ist, hängt von der Vorgabezeit ab, die für den jeweiligen Arbeitsgang angegeben ist.

Serientabellen werden unabhängig von einer bestimmten Maschine oder einer Arbeitsart angelegt. Wenn Sie für die Fertigung mit bestimmten Arbeitsarten unterschiedliche Abschläge einsetzen wollen, müssen Sie also mehrere Tabellen für Serien anlegen. Verwenden Sie dann für die Bezeichnung einen Begriff, aus dem deutlich wird, wofür die Tabelle eingesetzt werden soll, z. B. *Bohren Serie*.

Damit die Serienfaktoren berücksichtigt werden, müssen Sie im Dialog *Aggregat* und im Dialog *Besondere technische Restriktionen* angeben, welche Serientabelle gelten soll.

#### Vorgabezeiten festlegen
Bevor Sie Vorgabezeiten eintragen, sollten Sie sich einen Plan erstellen, in dem folgende Fragen geklärt sind:
- Welche Arbeitsarten kann jede Ihren Maschinen ausführen. Welche Arbeitsart kann die neue Maschine ausführen.
- In welcher Einheit soll die Zeit eintragen werden, z. B. pro Meter, pro Kante, pro Fläche.
- Soll die gestoppte Zeit eingetragen werden (Basiszeit) oder ein Zeitzuschlag.
- Soll die Zeit als Einzelzeit oder mit einer Staffelung eingetragen werden.
- Nach welchen Grenztypen und welchen Grenzwerten soll die Zeit gestaffelt werden.

> **Tipp**
> Wenn Sie zuvor die Vorgabezeit für ein gleichartiges Aggregat oder eine gleichwertige Arbeitsart auswählen, können Sie die Daten als Vorbelegung übernehmen und bearbeiten. In den folgenden Handlungssequenzen wird die Zeit vollständig neu angelegt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So legen Sie die Grunddaten der Vorgabezeit fest" auf Seite H-77
- "So legen Sie die Zeiten für eine Arbeitsart fest" auf Seite H-79

**So legen Sie die Grunddaten der Vorgabezeit fest**
1.  Wählen Sie im Modul *Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten*.
    _Abb. H-47: Vorgabezeit für Arbeitsart anlegen_
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
    _Abb. H-48: Vorgabezeit anlegen: Grunddaten eintragen_
3.  Wählen Sie die zuerst die Arbeitsart und dann das Aggregat (A) aus. Wenn ein Aggregat mehr als eine Arbeitsart ausführen kann, müssen Sie die gesamte Handlungssequenz für jede Arbeitsart wiederholen und die entsprechenden Zeiten festlegen. Alternativ dazu können Sie eine neue Arbeitsart anlegen, die alle Tätigkeiten umfasst, die das Aggregat ausführen kann. Die Vorgabezeit gilt dann für den gesamten Ablauf der Tätigkeiten.
4.  Wählen Sie den Typ (B) der Vorgabezeit. In diesem Beispiel wird *Basiszeit* gewählt. Die Handlungsschritte für Zeitzuschläge unterscheiden sich nicht von denen für Arbeitsgänge.
5.  Legen Sie die Priorität (C) fest. Die Priorität steuert die Auswahl des Aggregats, je nach der Arbeitsart, die für die Fertigung der Auftragsposition erforderlich ist.
6.  Legen Sie das Format der Vorgabezeit fest, indem Sie zu dem entsprechenden Register wechseln. In diesem Beispiel wird eine gestaffelte Vorgabezeit angelegt. Eine Einzelzeit legen Sie auf die gleiche Weise an, wählen dann aber das entsprechende Register.
Damit haben Sie die Grunddaten festgelegt. Sie müssen jetzt die Zeiten eintragen.

**So legen Sie die Zeiten für eine Arbeitsart fest**
1.  Wechseln Sie zum Register *Matrix*. Staffelungen und Zeiten werden in den Registern *Vektor* und *Würfel* auf die gleiche Art eingetragen.
    _Abb. H-49: Grenzwerte für Vorgabezeiten_
2.  Wählen Sie die Grenztypen (B) 1 und 2 aus, z. B. *Dicke* und *qm Rechteck*. Als nächstes müssen Sie die Grenzwerte für die Staffelung festlegen.
3.  Öffnen Sie das Kontextmenü (rechte Maustaste) zum Spaltenkopf (D). Wählen Sie im Kontext-Menü den Eintrag *Einfügen > Vor*. Das Feld für den Grenzwert (A) wird freigeschaltet.
4.  Tragen Sie den ersten Grenzwert ein, z. B. **4,00** für die Dicke, und springen Sie mit der `<Tab>`-Taste in das nächste Feld. Die neue Spalte wird eingefügt.
5.  Wiederholen Sie die Schritte 3 bis 5, bis Sie die gesamte Staffelung für den Grenztyp 1 angelegt haben.
6.  Öffnen Sie das Kontextmenü (rechte Maustaste) zum Zeilenkopf (C) und wiederholen Sie die Schritte 4 und 5 für den Grenztyp 2.
7.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.
8.  Tragen Sie jetzt in jede Zelle der Zeittabelle den entsprechenden Wert ein.
    _Abb. H-50: Neue Vorgabezeiten angelegt_
9.  Prüfen Sie im Feld *Zeiteinheit*, ob der Eintrag richtig gewählt ist. In diesem Beispiel wird die Einheit *qm* gewählt. Das bedeutet, dass die eingetragenen Zeiten sich auf die Fläche beziehen, also z. B. 0,013 Std. pro qm.
10. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert. Die neuen Daten werden im Register *Zeitauswahl* in der Übersicht aufgeführt.

#### Sonderzeit anlegen
Sonderzeiten legen Sie als Zuschläge an, um Besonderheiten berechnen zu können, z. B. ein Zuschlag für Übergrößen. Sie können pro Datensatz zwei Grenztypen berücksichtigen, wobei die Grenztypen zwischen den Datensätzen einer Zuschlagstabelle wechseln können.

In den folgenden Beispielen wird die Tabelle für Größenzuschläge kopiert und angepasst.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So legen Sie eine neue Zuschlagstabelle an" auf Seite H-81
- "So legen Sie weitere Stufen zur Staffelung des Zuschlags an" auf Seite H-83

**So legen Sie eine neue Zuschlagstabelle an**
1.  Wählen Sie im Modul *Kapazitätsplanung > Stammdaten > Vorgabezeiten > Sonderzeiten*.
    _Abb. H-51: Sonderzuschlag anlegen_
    Wenn bereits Tabellen angelegt sind, können Sie einen Eintrag markieren. Die Zuschlagswerte werden dann in die neue Tabelle übernommen.
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
    _Abb. H-52: Neue Tabelle anlegen_
3.  Tragen Sie die Nummer (A) und die Bezeichnung (B) der neuen Tabelle ein. Überschreiben Sie dazu die Einträge in den beiden Feldern.
4.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.
5.  Tragen Sie den Wert für den neuen Zuschlag ein. Sie können die vorhandenen Grenztypen und Zuschlagswerte überschreiben oder durch weitere Werte ergänzen.

In diesem Beispiel basiert die neue Tabelle auf der Größentabelle. Sie soll jetzt angepasst werden für die Kantenbearbeitung. In der folgenden Handlungssequenz werden daher die Grenztypen und die Stufung geändert.

**So legen Sie weitere Stufen zur Staffelung des Zuschlags an**
1.  Lassen Sie sich den Zuschlag anzeigen, den Sie bearbeiten wollen.
    _Abb. H-53: Gestaffelter Sonderzuschlag_
2.  Ändern Sie in der ersten Zeile Grenztyp 1 (B), z. B. in *Dicke* und Grenztyp 2, z. B. in *Größte Kantenlänge*.
3.  Passen Sie die Grenzwerte (A) entsprechend an.
    _Abb. H-54: Zuschlag bearbeiten_
    In diesem Beispiel wird also für die Glasdicke bis 5 mm und die Kantenlänge bis 1200 mm kein Zuschlag erhoben. Bei gleicher Dicke wird für die Kantenlängen zwischen 1201 mm bis 1800 mm ein Zuschlag von 50 % (B) berechnet. Die nächsten Stufen sollen sich auf die gleichen Kantenlängen auf die Dicke 6 mm beziehen.
4.  Überschreiben Sie die letzte Zeile mit den erforderlichen Werten für die Grenztypen, die Grenzwerte und den Zuschlag. Für die nächste Stufe muss eine neue Zeile eingefügt werden.
5.  Klicken Sie doppelt in den Zeilenkopf (A) der letzten Stufe. Das Kontext-Menü wird angezeigt.
6.  Wählen Sie den Eintrag *Einfügen*. Eine neue Zeile wird eingefügt. Die Grenztypen und Zuschlagseinheit sind mit den Einträgen aus der vorigen Zeile vorbelegt.
    _Abb. H-55: Neuen Grenzwert ergänzen_
7.  Ergänzen Sie den neuen Grenzwert im ersten Feld und passen Sie ggf. die Einträge in den übrigen Feldern an.
8.  Legen Sie auf diese Weise die gewünschten Zuschlagsstufen an.
9.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

> **Einträge löschen**
> Um einen Eintrag zu löschen, wählen Sie den entsprechenden Befehl im Kontextmenü. Wenn Sie den Befehl aus dem Menü *Start > Löschen* wählen, wird die gesamte Tabelle gelöscht.

#### Übungen
- Legen Sie zu Ihrem Übungsaggregat die Vorgabezeiten fest.
- Legen Sie einen Zuschlag für Sprossen mit dem Faktor 1,5 an.
- Legen Sie eine Sonderzeit für den Zuschnitt von Drahtglas an. Beachten Sie dabei 2 Grenzwerte.
- Legen Sie einen Zeitzuschlag für 3-fach-ISO an.
- Legen Sie einen Zeitzuschlag für Rüstzeit an, der bei Serien nur einmal berechnet wird.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Serienfaktoren" auf Seite H-196
⇨ Softwarereferenz, “Übergangszeiten" auf Seite H-197
⇨ Softwarereferenz, "Übergangsmatrix" auf Seite H-216
⇨ Softwarereferenz, "Vorgabezeiten (Dialog)" auf Seite H-224
⇨ Softwarereferenz, "Sonderzeiten" auf Seite H-234

### Auswahl der Aggregate
**Lernziele**
- Einschränkungen und Prioritäten der Aggregate so einsetzen, dass der Produktionsfluss gewährleistet ist.
- Einstellungen in den Firmendaten prüfen.

**Nutzen**
Die Aggregate werden beim automatischen Einlasten eines Auftrags geprüft und danach ausgewählt, ob sie technisch und zeitlich in der Lage sind, die erforderlichen Aufgaben auszuführen.

> **Merke**
>
> **Technische Restriktionen**: Einschränkungen zur automatischen Auswahl eines Aggregats werden im Dialog *Aggregate* und im Dialog *Besondere technische Restriktionen* festgelegt.
>
> **Automatisch Einlasten**: Beim automatischen Einlasten von Aufträgen in die Kapazitätsplanung werden die Vorgaben zu Prioritäten und Restriktionen ausgewertet und danach nach einer passenden freien Maschine gesucht.
>
> **Auslastung**: Die mögliche Auslastung eines Aggregats richtet sich nach der Kapazität des Aggregats und den Einstellungen in den Firmendaten. Für die manuelle Einlastung und das Aufarbeiten von Resten aus dem Vortag sollte daher ein Spielraum gelassen werden.
>
> **Manuelle Einlastung**: Ein Auftrag kann manuell eingelastet werden, wenn die Vorgaben für die Auslastung dies zulassen.
>
> **Voreinstellungen**: Firmendaten: Register *Kapa-Planung*

#### Prioritäten
Bei gleichartigen Aggregaten für eine Arbeitsart, z. B. Bohren, hängt die Auswahl durch die Kapazitätsplanung von der Priorität ab, die pro Maschine und Arbeitsart angegeben ist. Bei zwei Maschinen für die gleiche Arbeitsart, die beide die gleiche Priorität haben, entscheidet sich das System für die schnellere und günstigere Maschine.

Über die Prioritäten können Sie außerdem steuern, dass spezielle Aggregate, z. B. der Handzuschnitt, von der automatischen Maschinenzuordnung ausgenommen werden.
Die Prioritäten werden im Dialog *Vorgabezeiten* angegeben.

> **Prioritäten bei gleichwertigen Maschinen**
> Es ist möglich, gleichwertigen Maschinen dieselbe Priorität zu geben, wenn Sie z. B. mit zwei Bistronic-Schneidtischen arbeiten. Wenn diese Maschinen unterschiedlichen AV-Bereichen oder Mandanten zugeordnet sind, ist die Auswahl dennoch eindeutig. Bei gleichwertigen Maschinen, deren Auswahl nicht durch andere Kriterien eingeschränkt ist, sollten die Prioritäten jedoch unterschiedlich vergeben werden.

**Abweichende Prioritäten**
Eine weitere Möglichkeit zum Steuern der Auswahl haben Sie mit abweichenden Prioritäten, die im Dialog *Besondere Prioritäten* angegeben werden.

_Abb. H-56: Besondere Priorität (Beispiel 5, gestrichelte Linie = 40 Stk.)_

In diesem Beispiel sehen Sie, dass die Bohrmaschine II die Priorität -2 hat. Das bedeutet, dass sie nur manuell ausgewählt werden kann. Im Dialog *Besondere Prioritäten* ist jedoch angegeben, dass sie bei Stückzahlen ab 11 die Priorität 9 hat. Damit haben Sie erreicht, dass diese Maschine nur für große Stückzahlen eingesetzt wird. Sie wird auch dann nicht automatisch ausgewählt, wenn die Bohrmaschine I ausgelastet ist.

#### Restriktionen
Eine Restriktion stellt eine Einschränkung für die Auswahl der Maschine dar. Diese Einschränkung kann z. B. mit den Maßen, der Glasstärke, der Geschwindigkeit zusammenhängen. Eine Restriktion liegt z. B. vor, wenn eine Bohrmaschine nur bis zu einer Glasstärke von 12 mm eingesetzt werden kann. Wenn das Rüsten einer Maschine sehr aufwendig ist, wird der Einsatz der Maschine von der Stückzahl abhängig gemacht. Maschinen können durch Restriktionen auch für bestimmte Arbeitsarten gesperrt werden.

Diese einfachen Restriktionen werden beim Anlegen der Maschinendaten angegeben. Komplizierte Restriktionen können nur über Sperrformeln angegeben werden.

**Beispiel**
Auf der Schleifmaschine B sollen nur Modelle, sehr kleine und sehr große Scheiben gefertigt werden, da diese Maschine sehr langsam ist.
Alle Rechteckscheiben mit einer Breite >200 und <2600 mm sowie einer Höhe >300 und <1600 mm sollen nicht auf dieser Maschine geschliffen werden.
Diese Restriktion kann nur über eine Formel angegeben werden.

In diesem Fall geben Sie in den Minimal- und Maximal-Werten für die Maschine an, bis zu welchen Maßen das Schleifen technisch möglich ist, z. B. für die Breite 40 bis 3210 mm und für die Höhe 100 bis 6000 mm. Der Bereich dazwischen (Breite >200 und <2600 mm, Höhe >300 und <3600 mm) wird durch eine Formel gesperrt.

Das Ergebnis für dieses Beispiel könnte zusammengefasst wie folgt aussehen:

_Abb. H-57: Technische Restriktionen und Sperrformel_
_A: Technisch mögliche Werte_
_B: Auswahl der Sperrformel_
_C: Beispiel für Sperrformel (Auszug)_

In den Stammdaten des Aggregats sind im Register *Allgemein* die Werte für Breite und Höhe (A) so angegeben, wie das Aggregat arbeiten kann, also der gesamte Bereich. Im Bereich *Sperre* wird die Nummer der Sperrformel (B) hinterlegt.

Die Sperrformel selbst wird über *A+W Business Pro-Stammdaten > Firma > Formeln* angelegt. Im Dialog *Formelverwaltung > Register Formel* (C) kann die Formel eingetragen und bearbeitet werden.
Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

#### Priorität vs. Restriktion
Die Möglichkeiten, die automatische Auswahl der Maschinen zu steuern, wirken zusammen. Das ist schon im Beispiel mit der Restriktionsformel deutlich geworden. Aber auch ohne Formeln können Sie die Auswahl sehr genau steuern:
- Eine Maschine mit der Priorität 9 und der Restriktion Stückzahl >10 wird immer erst ausgewählt, wenn in der Position mindestens 11 Stück angegeben sind. Liegt die Stückzahl unter oder gleich 10, so wird die Maschine mit der nächstniedrigeren Priorität ausgewählt.
- Wenn eine Maschine mit der Priorität 9 keine großen Scheiben bearbeiten kann, wird sie nur für Positionen mit Standard-Maßen ausgewählt.
Sie können solche Kombinationen im Dialog *Besondere Prioritäten* hinterlegen.

_Abb. H-58: Besondere Prioritäten_

In diesem Beispiel sehen Sie, dass die CNC-Maschine bei einer Stückzahl über 10 mit der Priorität 9 bei Bohrungen eingesetzt werden soll. Standardmäßig hat diese Maschine für die Arbeitsart *Bohren* nur die Priorität 4.

Wenn beim Einlasten eines Auftrags eine Restriktion verletzt wird, wird die Maschine nicht für diesen Auftrag eingesetzt. Sie kann dann auch nicht manuell ausgewählt werden, da sie nicht zur Auswahl angeboten wird.

> **Verfügbare Felder für Prüfwerte (Sperrwerte)**
> Die Eingabefelder für Prüfwerte müssen bei den Aggregattypen freigeschaltet werden. Wenn Sie Prüfungen nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Prüffelder ohne Werte verhindern beim Einlasten die Auswahl des Aggregats - auch dann, wenn es geeignet wäre, die Position zu fertigen.
> ⇨ Softwarereferenz, "Aggregattypen" auf Seite H-189

#### Automatische Einlastung
Bei der automatischen Einlastung werden die Aggregate (Maschinen) ausgewählt, die der jeweiligen Arbeitsart zugeordnet sind. Sie haben die Möglichkeit, einer Arbeitsart, z. B. dem Bohren, mehrere Bohrmaschinen zuzuordnen. Aus der Kombination von Arbeitsart und Aggregat ergeben sich der zeitliche Aufwand (reservierte Kapazität) und die Kosten. Die automatische Auswahl der Bohrmaschine wird u. a. anhand der freien Kapazitäten, der technischen Restriktionen und der Kosten entschieden.

Die Auswahl eines Aggregats kann daher über folgende Einstellungen gesteuert werden:
- Priorität des Aggregats (9 bis -2)
- Arbeitsart
- Sperren der Maschine, z. B. für bestimmte Produktarten
- Restriktionen, die sich auf die Anforderungen aus der Auftragsposition beziehen, z. B. die Maße, Stückzahl.

In den folgenden beiden Grafiken wird gezeigt, wie diese Einstellungen zusammenwirken. Prioritäten und Restriktionen sind anschließend in separaten Einheiten ausführlich beschrieben.

_Abb. H-59: Priorität und Technische Restriktionen (Beispiel 1, gestrichelte Linie = 40 Stk.)_

Im eingelasteten Auftrag wird zunächst geprüft, welche Arbeitsart ausgeführt werden soll. Anhand der Arbeitsart werden die möglichen Maschinen ermittelt und geprüft, welche Restriktionen jeweils vorliegen. Maschinen, die für die Fertigung nicht geeignet sind, werden nach dieser Prüfung nicht mehr zur Auswahl angeboten. Sie stehen dann auch nicht zur manuellen Auswahl zur Verfügung.

In Beispiel 1 sehen Sie, dass die Standard-Maschine mit der Priorität 9 (Bohrmaschine I) nur für die erste Position angesteuert wird. Bei der Prüfung der Restriktionen wird erkannt, dass die 40 Stk. der zweiten Auftragsposition nicht auf Bohrmaschine I gefertigt werden dürfen. Die Bohrmaschine II wird gewählt. Wenn es eine Bohrmaschine III mit derselben Priorität gibt, die ebenfalls große Stückzahlen fertigen kann, dann entscheidet das Programm nach Kosten, benötigter Zeit und freien Kapazitäten.

_Abb. H-60: Priorität und Technische Restriktionen (Beispiel 2, gestrichelte Linie = 40 Stk.)_

In Beispiel 2 sehen Sie, dass die Priorität an der Auswahl der Maschine nichts ändert, da die Restriktionsprüfung bereits entschieden hat, welche Maschine für die zu fertigenden Stückzahlen gewählt werden kann. Die Bohrmaschine I wird aufgrund der Stückzahl gewählt, weil in der ersten Position weniger als 11 Stück gebohrt werden sollen.

_Abb. H-61: Priorität und Technische Restriktionen (Beispiel 3, gestrichelte Linie = 40 Stk.)_

Wenn zusätzlich die technischen Restriktionen geändert werden, ergibt sich folgender Ablauf: Die Restriktionsprüfung lässt das Bohren der ersten Position auf beiden Maschinen zu. Bohrmaschine I wird nur ausgewählt, wenn Bohrmaschine II keine Kapazität frei hat. Bohrmaschine I würde jedoch niemals für die Fertigung der zweiten Position gewählt.

_Abb. H-62: Restriktionen und besondere technische Restriktionen_

Um auszuschließen, dass einzelne Stücke von Bohrmaschine II gefertigt werden, kann eine weitere Einschränkung im Dialog *Besondere technische Restriktionen* eingestellt werden. Im Dialog *Besondere technische Restriktionen* legen Sie Restriktionen einer Maschine in Verbindung mit einer Arbeitsart fest. In unserem Beispiel bleibt die Stückzahl (A) für Bohrmaschine II unverändert (ab 1 Stück), aber in den besonderen technischen Restriktionen (B) wird festgelegt, dass sie erst ab 11 Stück eingesetzt werden soll.

_Abb. H-63: Besondere technische Restriktionen (Beispiel 4, gestrichelte Linie = 40 Stk.)_

In diesem Beispiel sehen Sie, dass durch die besonderen technischen Restriktionen die Fertigung der 6 Stück auf Bohrmaschine II verhindert wird, obwohl sie die Priorität 9 hat und auch einzelne Stücke arbeiten kann. Mit diesen Einstellungen steht die Bohrmaschine II auch für die manuelle Auswahl bei kleinen Stückzahlen zur Verfügung.

#### Maschinenauswahl bei Ausweicharbeitsart
Die Ausweicharbeitsart kann auch für die Umleitung von großen Stückzahlen genutzt werden. Zu diesem Zweck wird eine Ausweicharbeitsart angelegt, die immer dann gewählt werden soll, wenn große Stückzahlen eingeplant werden.

Zusätzlich legen Sie eine Serientabelle mit den Faktoren für die Serienfertigung an. Diese Tabelle muss dem Aggregat an zwei Stellen bekannt gemacht werden: im Dialog *Aggregat* und im Dialog *Besondere technische Restriktionen*.

Im Beispiel 3 aus der Einheit *Automatische Einlastung* soll nun die Fertigung von Serien berücksichtigt werden.

_Abb. H-64: Ausweicharbeitsart für Serien (gestrichelte Linie = Serie)_

Bohrmaschine I wird nur gewählt, wenn die Stückzahl 10 nicht überschritten wird. Zu der Arbeitsart *Bohren* ist die Ausweicharbeitsart *Bohren Serie* angegeben. Dieser Arbeitsart ist die Bohrmaschine II zugeordnet. Die Umleitung wird also durch die Arbeitsart eingeleitet, obwohl beide Maschinen die Priorität 9 haben. Der Bohrmaschine II ist die Serientabelle zugeordnet, in der die Zeiten für Serien gestaffelt sind.

#### Sperren
Sperren müssen definiert werden, um z. B. zu vermeiden, dass bestimmte Arbeiten doppelt ausgeführt werden oder dass eine Maschine angesteuert wird, die eine Leistung für ein bestimmtes Produkt nicht erbringen kann.
- Sie können Produkte, Warengruppen oder Produktgruppen für bestimmte Maschinen sperren, z. B. ESG für den Zuschnitt, denn eine ESG-Scheibe wird niemals zugeschnitten.
- Maschinen können auch für Folge-Bearbeitungen gesperrt werden.
- Wenn ein Aggregat z. B. mehrere Arbeitsarten ausführen kann, dann muss es nicht vollständig gesperrt werden, sondern nur für eine der Arbeitsarten.
- Sperren von Maschinen sind kundenbezogen und teilweise auch abhängig von Arbeitsarten möglich.

**Beispiele**
- Wenn die Bohrmaschine das Glas automatisch wäscht, dann braucht das Glas, bevor es gehärtet wird, nicht noch einmal gewaschen zu werden. Um diesen zweiten Waschvorgang zu unterbinden, können Sie in eine Sperre definieren.
- Ein Kunde besteht darauf, dass für das Bohren seiner Gläser nur eine bestimmte Maschine benutzt wird. Alle anderen Bohrmaschinen werden für diesen Kunden gesperrt.

Je nachdem wie Sie die Arbeitsarten und die Aggregate definiert haben, können Sie die Sperre für das erste Beispiel auf unterschiedliche Weise festlegen:
- **Dialog Folge-Aggregat überspringen:** Am Aggregat *Bohrmaschine* legen Sie fest, dass das Aggregat *Waschmaschine* übersprungen wird.
- **Dialog Arbeitsgänge überspringen:** Am Aggregat *Bohrmaschine* legen Sie fest, dass die Arbeitsart *Waschen* nicht ausgeführt wird.

#### Dialoge für Sperren
Arbeitsarten, die an bestimmten Produktgruppen nicht ausgeführt werden sollen, können über die Zuweisung des Aggregats gesperrt werden.

_Abb. H-65: Totalsperre der Produktgruppe ESG für den automatischen Zuschnitt_

In der Kombination von Produktgruppe und Arbeitsart kann das Aggregat ganz oder teilweise gesperrt werden. Die Totalsperrung (D) bedeutet, dass das Aggregat auch dann gesperrt ist, wenn die Produktgruppe inklusive der Arbeitsart Bestandteil einer Stückliste ist, z. B. das ESG in einem ISO. Die Kapazitätsplanung sucht dann auch nicht nach einem alternativen Aggregat.

Die Dialoge zum Sperren sind analog aufgebaut, unterscheiden sich aber in der Art der Sperre. In der folgenden Übersicht werden diese unterschiedlichen Sperren kurz charakterisiert:
- **Sperren nach WGR (Warengruppe):** Diese Sperre richten Sie für Warengruppen ein, die nicht an einem bestimmten Aggregat gefertigt werden sollen.
- **Sperren nach Produktgruppen:** Diese Sperre richten Sie für Produktgruppen ein, für die eine Arbeitsart nicht an einem bestimmten Aggregat ausgeführt werden soll. Sie können damit steuern, dass die Arbeitsart für die Produktgruppe an einem alternativen Aggregat ausgeführt wird.
- **Sperren nach Produkten:** Diese Sperre richten Sie für Produkte ein, für die eine Arbeitsart nicht an einem bestimmten Aggregat ausgeführt werden soll. Sie können damit steuern, dass die Arbeitsart für das Produkt an einem alternativen Aggregat ausgeführt wird.
- **Folge-Aggregat überspringen:** Diese Sperre richten Sie ein, wenn ein Arbeitsgang an einem Aggregat die nachfolgende Arbeitsart mit ausführt. Wenn z. B. die Bohrmaschine die Scheibe anschließend wäscht, wird das Aggregat *Waschen* gesperrt.
- **Kundenbezogen sperren:** Diese Sperre richten Sie für Kunden ein, für die bestimmte Bearbeitungen an einem alternativen Aggregat ausgeführt werden sollen. Das Aggregat mit der obersten Priorität wird damit gesperrt.
- **Fertigungsstraße definieren:** Diese Sperre richten Sie ein, wenn an einem Aggregat bestimmte Arbeitsarten nicht gesondert berechnet werden sollen, z. B., wenn die Rüstzeit für eine CNC-Maschine für aufeinanderfolgende Bearbeitungen nicht doppelt berechnet werden soll.
- **Arbeitsgänge überspringen:** Diese Sperre richten Sie ein, wenn ein Arbeitsgang an einem Aggregat die nachfolgende Arbeitsart mit ausführt. Wenn z. B. die Bohrmaschine die Scheibe anschließend wäscht, wird die Arbeitsart *Waschen* übersprungen.

#### Aggregat vollständig sperren
Sie können ein Aggregat vollständig sperren, z. B., wenn Sie es neu angelegt haben, aber noch nicht alle Werte eingetragen sind. In diesem Fall markieren Sie im Dialog *Aggregat* die Checkbox *Gesperrt*.

#### Aggregat vorübergehend sperren
Ein Aggregat kann auch vorübergehend gesperrt werden, z. B. für Wartungsarbeiten. Eingelastete Aufträge werden dabei umgelastet.

_Abb. H-66: Aggregat vorübergehend sperren_
_A: Gesperrtes Aggregat_
_B: Zeitraum der Sperre_
_C: Aufträge, die bereits eingelastet sind, müssen manuell umgelastet werden._

#### Fertigungsstraße definieren
Eine Arbeitsart kann gesperrt werden, wenn diese im nachfolgenden Aggregat ebenfalls vorkommt.

**Beispiel**
Auf der CNC-Maschine werden die Arbeitsarten *Eckausschnitt* und *Randausschnitt* gefertigt. Für beide Produktgruppen wurde die Arbeitsart *Rüstzeit* mit dem Faktor 1,2 eingetragen.
Wenn in einem Auftrag Eckausschnitte und Randausschnitte gefertigt werden sollen, dann wird die CNC-Maschine nur einmal gerüstet. Die Zeit darf also nur einmal berechnet werden.

**So definieren Sie eine Fertigungsstraße**
1.  Wählen Sie im Modul *Kapazitätsplanung > Sperren > Fertigungsstraße definieren*.
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln. Die Felder werden freigeschaltet.
3.  Wählen Sie das Aggregat aus, z. B. die CNC-Maschine.
    _Abb. H-67: Aggregat für Fertigungsstraße_
4.  Klicken Sie im Bereich *Aggregate* auf die Schaltfläche **[Neu]** (A). Die Zeile wird freigeschaltet.
5.  Klicken Sie in das Feld *Arbeitsart* und wählen Sie aus der Kombobox (B) die Arbeitsart aus, die Sie sperren wollen. In diesem Beispiel ist das die *Rüstzeit*.
6.  Wählen Sie das Folge-Aggregat (C) aus. Das Folge-Aggregat ist in diesem Beispiel wieder die CNC-Maschine, denn die folgende Bearbeitung wird wieder an ihr ausgeführt.
7.  Markieren Sie die Checkbox *Total* (D), um die Arbeitsart vollständig zu sperren.
8.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
    _Abb. H-69: Aggregat für Fertigungsstraße_

Die Rüstzeit wird nun nur einmal berechnet, wenn mehr als eine Bearbeitung ausgeführt wird. Bei einer neuen Auftragsposition (mit anderen Maßen) wird sie jedoch wieder berechnet.

#### Voreinstellungen zur Aggregatauswahl
Die Einstellungen für die Auslastung der Schichten haben Sie bereits in der Einheit Schicht- und Arbeitszeit kennengelernt.
⇨ "Voreinstellungen für Schichten und Kapazitäten" auf Seite H-48

In diesem Abschnitt werden die Einstellungen für die Auswahl des Aggregats vorgestellt.

_Abb. H-70: Firmendaten – Kapa-Planung_
_A: Art der Auswahl eines Aggregats_

Wenn Sie mit mehreren Maschinen arbeiten, die dieselben Arbeitsarten ausführen können, kann die Planung diese Maschinen auf unterschiedliche Weise berücksichtigen:
- **Automatisch:** Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **Semi-automatisch:** Das Programm bietet die alternativen Maschinen zur Auswahl an, wenn die Standard-Maschine ausgelastet ist.
