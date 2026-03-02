---
description: "DE_AWProduction_BDE_2.01"
---

# A+W Betriebsdatenerfassung H

**A+W Production**

A+W - Software for Glass, Windows and Doors

---

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Änderung |
| :--- | :--- |
| 1.00 / 03-2007 | Ersterstellung |
| 1.01 / 07-2013 | Layout an CI 2013 angepasst. |
| 2.0 / 06-2014 | Komplette Überarbeitung |
| 2.01 / 01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Produktnamen
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen
*   Kontakte

#### Produktnamen

Im Rahmen der strategischen Neuausrichtung wurden das Produktportfolio der A+W Software GmbH neu ausgerichtet. Dabei wurden auch die Produktnamen angepasst. So wird ALCIM in Zukunft A+W Production heißen.

Da im Produktentwicklungszyklus sowohl die alten Produktversionen als auch die neuen Produktversionen angepasst und erweitert wurden, verwenden wir in diesem Dokument ausschließlich die alten Produktnamen - gemeint sind dabei jeweils die alten und die neuen Produktversionen.

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

#### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte

**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim

📞 +49 6404 2051-0
📠 +49 6404 2051-877
✉️ Zentrale@a-w.com
🌐 http://www.a-w.com

---

## Inhalt

*   **Vorspann** (H-3)
    *   Revisionsübersicht (H-3)
    *   Editorial (H-3)
*   **Tutorial** (H-7)
    *   **Überblick** (H-9)
        *   Dokumentation (H-10)
        *   Aufbau des Tutorials (H-10)
        *   Darstellungskonventionen (H-11)
    *   **Grundgedanken** (H-12)
        *   Die Betriebsdatenerfassung (H-13)
        *   Zweck der A+W Production (H-13)
    *   **Buchungselemente** (H-14)
        *   Produkte (H-15)
        *   Grundsätzliches (H-16)
            *   Direkte Objekte (H-16)
            *   Indirekte Objekte (H-16)
            *   Scheiben bzw. Einheiten (H-16)
            *   Buchungsarten (H-17)
        *   Buchungsorte (H-18)
        *   Erfassungsstellen (H-19)
            *   Fehlergestell (Error-Rack) (H-20)
            *   Korrekte Buchung (H-22)
            *   Erfassungsstellen verwalten (H-23)
            *   Erfassungsstelle Lkw (H-25)
        *   Abstellplätze (H-26)
            *   Gestelle (H-27)
            *   Kisten (H-28)
            *   Gestelle verwalten (H-29)
        *   Personal (H-32)
            *   Mitarbeiter (H-33)
            *   Mitarbeiter verwalten (H-34)
        *   Status (H-36)
            *   Zustände (H-37)
            *   Einheit/Gruppe (H-37)
            *   Gestell (H-37)
            *   Erfassungsstelle (H-37)
            *   Aktions-Barcode (H-38)
            *   Zustände verwalten (H-39)
    *   **Datenerfassung** (H-41)
        *   Scanner (H-42)
            *   Scanner-Typen (H-43)
            *   Online-Scanner (H-43)
            *   Denso-Scanner (WLAN) (H-43)
            *   Serielle Scanner (H-44)
            *   Offline-Scanner (H-44)
            *   Konfiguration der Scanner (H-44)
        *   Barcodes (H-45)
    *   **Buchungsbeispiele** (H-46)
        *   Die Reihenfolge des Scannens (H-47)
        *   Scannen von Einheiten (H-49)
        *   Scannen im Versand (H-51)
        *   Erfassungsstellen scannen (H-53)
        *   Erfassungsstelle LKW (H-56)
            *   Übungen: Übung 1: Beladen eines leeren und eines teilbeladenen LKW (H-57)
        *   Gestelle bzw. Kisten scannen (H-59)
        *   Status scannen (H-61)
        *   Korrigieren von Fehlbuchungen (H-62)
    *   **Production Terminals** (H-63)
        *   Production Terminals (H-64)
        *   Einführung (H-65)
    *   **Bruchmanagement** (H-68)
        *   Überblick (H-69)
        *   Bruchbehandlung (intern) (H-70)
    *   **Statistik, Reporting und Monitoring** (H-72)
        *   Überblick (H-73)
        *   BDE-Reporting (H-74)
            *   Aufruf der Reports (H-74)
            *   Beispiele der Standard-Barcode-Reports (H-74)
            *   Abstellliste (H-75)
            *   Auftragsübersicht (H-75)
            *   Auftragsstatus (H-76)
            *   Ladeliste (H-76)
            *   Gestellbelegung pro Scheibe (H-77)
            *   Gestellbelegung pro Position (H-78)
            *   Buchungshistorie (H-78)
        *   Monitoring: A+W Dashboard (H-79)
            *   Überblick (H-80)
        *   Statistik: A+W Discovery (H-83)
            *   Überblick (H-84)
*   **Softwarereferenz** (H-87)
    *   Übersicht (H-89)
    *   Stammdaten (H-90)
        *   Barcode-Optionen (H-91)
        *   Barcode-Typen (H-92)
        *   Erfassungsstellen-Typen (H-93)
        *   Erfassungsstellen (H-94)
        *   Gestelle (H-98)
        *   Gestellfilter (H-102)
        *   Zustandstypen (H-103)
        *   Zustände (H-104)
        *   Mitarbeiter (H-106)
        *   Spaltenzuordnung (H-108)
        *   Spalten (H-109)
        *   Nachbearbeitung (H-110)
*   **Partindex** (H-1)
    *   Index Betriebsdatenerfassung (H-3)

---

## Tutorial

### Überblick

Die Zielgruppe der Schulung zum Modul A+W Production sind Mitarbeiter, die an unterschiedlichen Stationen (Maschinen und Erfassungsstellen) innerhalb der Produktion arbeiten.

Der Vorteil für den Kunden liegt darin, dass er seine Maschinen direkt ansteuern kann. Es entstehen dadurch keine Ausfallzeiten, um eine Form an einer Bearbeitungsmaschine zu digitalisieren. Es müssen auch keine NC-Codes an der Maschine eingegeben werden, was auch einen ständigen Maschineneinsatz bedeutet.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
*   Grundgedanken
*   Buchungselemente
*   Datenerfassung
*   Statistik, Reporting und Monitoring

#### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die an unterschiedlichen Stationen (Bereiche, Maschinen und Erfassungsstellen) innerhalb der Produktion arbeiten. Die Teilnehmer müssen das Konzept der Production Terminals und der Scanner kennen.

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwendung der A+W Production vorausgesetzt.

### Dokumentation

Für die Schulung zum Barcode Manager stehen folgende Unterlagen zur Verfügung:

| Format | Inhalt |
| :--- | :--- |
| **HTML** | Tutorial und Softwarereferenz |
| **Handout** | Ausdruck Schulungsunterlage für die Teilnehmer |
| **PDF** | Vollständige Unterlagen<br>Tutorial<br>Softwarereferenz |
| **Online-Hilfe <F1>** | Kontextsensitive Dialog-Hilfe der A+W Production-Softwarereferenz |

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

*   **Überblick**
    Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    *   **Lernziele:** Was soll vermittelt werden?
    *   **Nutzen:** Wofür können Sie dieses Wissen einsetzen?
    *   **Merksätze:** Welche Zusammenhänge müssen Sie sich merken?

*   **Konzepte**
    Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

*   **Übungen**
    *   Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
    *   Die Übungen helfen Ihnen A+W Production zu verstehen und anwenden zu lernen.

*   **Querverweisteil**
    Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

*   **Lesehinweis**
    Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen. Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht ein roter Faden durch die gesamte Dokumentation.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | Sind Zeichenfolgen ausgezeichnet, die sich auf Elemente der Software beziehen, z. B. der Dialog *Globale Formdaten*. |
| **Fett** | Sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B. geben Sie den Wert **0** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Datei > Importieren > Übergabedatei*. |
| [] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B. mit **[OK]** speichern Sie die Daten. |
| <> | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B. mit **<F1>** öffnen Sie die Online-Hilfe. |

---

## Grundgedanken

Diese Dokumentation gibt Ihnen einen Einblick in die Betriebsdatenerfassung (A+W Production) der A+W Software GmbH und vermittelt ein Grundverständnis für dieses Thema. Die Grundzüge der A+W Production, die zum Einsatz kommenden Werkzeuge und die grundsätzlichen Möglichkeiten und Grenzen werden erläutert.

Das Studium weiterführender Dokumentationen zu Leitrechner (Production Terminals), interner A+W Production Installations- und Konfigurationsanleitungen, Scanner-Installation und Konfiguration usw. wird dringend empfohlen. Diese Themen werden in dieser Dokumentation angeschnitten aber nicht vertieft. Eine eindeutige Abgrenzung der Bereiche ist nicht immer möglich und auch nicht sinnvoll.

Diese Anleitung ersetzt kein grundlegendes Wissen über Produktionsstrukturen, die eingesetzten Production Terminals, Scanner oder andere A+W Software.

### Aufbau dieses Dokumentes

Diese Dokumentation beschreibt allgemeines Wissen zur A+W Production. Was ist die A+W Production, die wichtigsten Komponenten, Erfassungsstellen, welche Scannertypen kommen zum Einsatz, Vorgehensweisen, usw.

### Die Betriebsdatenerfassung

Die A+W Production ist ein Sammelbegriff für die Erfassung von Istdaten über Zustände und Prozesse in Betrieben.

Sie erfasst den Produktionsfluss an den wichtigsten Stellen innerhalb der Produktion, den so genannten Erfassungsstellen und bildet so den Prozessfluss Ihrer Produktion ab. Dies geschieht mit Hilfe von z. B. Barcodes, Scannern, Production Terminals (Leitrechner), usw. Die erfassten Daten werden entweder direkt oder indirekt an eine entsprechende Sammelstelle (AWPort) übermittelt und in der Datenbank (A+W Production-DB) gespeichert.

### Zweck der A+W Production

Die A+W Production dient der Darstellung der aktuellen Ist-Situation: Feststellung des Produktionsstatus eines Auftrages, Verfolgung einer Position oder Einzelscheibe durch die Produktion, Überwachung der Leistung (Maschine und Bediener) bis hin zur Darstellung der Performance.

Im Falle von Bruchscheiben wird neben der Erfassungsstelle auch der Bruchgrund erfasst. Je nach Konfiguration werden automatisch entsprechende Nachläufer generiert. Die Maschinenansteuerung erfolgt ebenfalls automatisch aufgrund von Barcodelesungen.

Ein weiterer wichtiger Aspekt der A+W Production sind die statistischen Auswertungen. Sie können die Produktivität und die Maschinenlaufzeiten messen sowie Produktionsfehler (z. B. Bruch) überwachen. Die mittels der A+W Production gescannten und erfassten Daten können mit Controlling- und Statistik-Werkzeugen von A+W ausgewertet und reported werden. Mit A+W Dashboard (aktuelle Leistung- und Status-Kennzahlen) und A+W Discovery (statistische Kennzahlen).

---

## Buchungselemente

In diesem Themenblock lernen Sie den Umgang mit den unterschiedlichen Objekten der A+W Production.

Dazu gehören folgende Lerneinheiten:
*   "Produkte" auf Seite H-15
*   "Buchungsorte" auf Seite H-18
*   "Abstellplätze" auf Seite H-26
*   "Personal" auf Seite H-32
*   "Status" auf Seite H-36

### Produkte

**Lernziele**
*   Objekte der A+W Production kennenlernen.
*   Was ist verfolgbar und was ist nicht verfolgbar.

**Definitionen**

| Objekt | Beschreibung |
| :--- | :--- |
| **Direkte Objekte** | Haben einen Barcode und werden direkt gebucht. |
| **Indirekte Objekte** | Haben keinen Barcode, da sie automatisch mit gebucht werden. |

**Merke**

| Produkt | Beschreibung |
| :--- | :--- |
| **Verfolgbare Produkte** | Alle Teile einer Stückliste, auf die man einen Barcode kleben kann. |
| **Einzelscheiben-A+W Production** | Jedes Stücklistenteil wird durch einen eigenen Barcode identifiziert. |
| **Mengen-A+W Production** | Alle Teile eines Stücklistenteils haben den gleichen Barcode. |

### Grundsätzliches

Die A+W Production unterscheidet zwei Objekt-Typen:
*   Direkte Objekte
*   Indirekte Objekte

#### Direkte Objekte

Direkte Objekte sind solche, die einen Barcode haben und direkt gebucht werden können. Dazu gehören:
*   Erfassungsstellen (Orte, LKWs und Maschinen)
*   Gestelle und Kisten
*   Scheiben und Einheiten
*   Zustände / Stati
*   Mitarbeiter

#### Indirekte Objekte

Indirekte Objekte sind solche, die automatisch mitgebucht werden. Dazu gehören:
*   Bearbeitungen
*   Chargeninformationen

#### Scheiben bzw. Einheiten

Bei Scheiben und Einheiten handelt es sich um verfolgbare Produkte. Das sind grundsätzlich alle Teile einer Stückliste, auf die man einen Barcode kleben kann. Beispiel: Einzelscheibe, ISO, VSG, Rahmen, Sprosse, etc.

In der Einzelscheiben-A+W Production (Standard) wird jedes Stücklistenteil durch einen eindeutigen Barcode identifiziert. Dadurch kann jederzeit der genaue Ort und Zustand eines Teils bestimmt werden.

In der Mengen-A+W Production haben alle Teile eines Stücklistenteils den gleichen Barcode. Dadurch ist der genaue Ort und Zustand eines Teils nicht mehr exakt bestimmbar. Hier werden nur quantitative Aussagen über Produktionszustände gemacht. Der Buchungsaufwand ist demzufolge wesentlich geringer.

Im Gegensatz zu verfolgbaren Teilen (Scheiben, Sprossen, Rahmen), können andere Stücklistenteile wie bspw. Gas, Silikon, Folien nicht gescannt bzw. verfolgt werden.

> **Daten buchen**
> Um eine möglichst gute Datenbasis für grafische Kontroll-Anzeigen und statistischen Auswertungen zu erhalten, ist es notwendig, in der Produktion kontinuierlich und exakt die Scheiben/Teile/Einheiten an den entsprechenden Erfassungsstellen auf das entsprechende Gestell zu buchen.

### Buchungsarten

Es werden drei verschiedene Buchungsarten unterschieden:

*   **Bewegungsbuchungen:**
    Bewegungsbuchungen dokumentieren die Ortsveränderung eines Gestells, einer Einheit oder einer Scheibe. Dies geschieht durch Buchung eines Gestells (Einheit auf Gestell) oder einer Erfassungsstelle (Gestell oder Einheit auf Erfassungsstelle) sein.
*   **Bearbeitungsbuchungen:**
    Diese Buchungen bilden Bearbeitungen (z. B. Bohren) von Einheiten ab.
*   **Zustandsbuchungen (z.B. Bruch, Wartung):**
    Zustandsbuchungen geben die Zustandsänderung eines Objekts wieder.

Bearbeitungs- und Zustandsbuchungen können auch durch Bewegungsbuchungen implizit ausgelöst werden.

Wichtig in diesem Zusammenhang ist natürlich die Brucherfassung. Bei der Brucherfassung wird neben der Erfassungsstelle und weiteren Informationen auch der Bruchgrund erfasst. Je nach Konfiguration werden automatisch Nachläufer generiert.

Die gewonnenen Daten können u. a. zu Auswertungs-, Statistik- und Inventurzwecken (z. B. BDE-Reports, MS-Excel usw.) verwendet werden. Sie dienen der Produktionssteuerung, der Scheiben-/Einheiten-, Gestellverfolgung u.v.m.

**Ergänzende Informationen**
*   ⇨ "Bruchmanagement" auf Seite H-68
*   ⇨ "BDE-Reporting" auf Seite H-74
*   ⇨ "Scannen von Einheiten" auf Seite H-49

---

## Buchungsorte

**Lernziele**
*   Den Dialog Erfassungsstellen erarbeiten.
*   Die Erfassungsstelle Fehlergestell kennenlernen und verstehen.
*   Die Erfassungsstelle Versand kennenlernen und verstehen.

**Nutzen**
Um Buchungsfehler zu vermeiden, ist es notwendig, die korrekte Buchungsreihenfolge einzuhalten.

**Definitionen**

| Begriff | Definition |
| :--- | :--- |
| **ES** | Abkürzung für Erfassungsstelle |
| **Erfassungsstellen** | Stationen innerhalb der Produktion bzw. des Versands. |
| **Fehlergestell** | Ist eine interne Erfassungsstelle mit der Erfassungsstellennummer 12 und wird automatisch gefüllt. Diese Erfassungsstelle dient zur Aufnahme aller Einheiten, die aufgrund von Fehlern ihre Zuordnung zu einem physikalischen Gestell bzw. einer physikalischen Erfassungsstelle verloren haben. |
| **Triggerzeit** | Die im System hinterlegte Zeitspanne, die festlegt, ab wann die Ladung eines Lkw als ausgeliefert gilt. Sie wird durch die Status-Buchung `<Begin> <Truck>` aktiviert. Die Dauer kann im System konfiguriert werden. |

**Merke**
*   **Erfassungsstellen** erhalten eine eindeutige Nummer und einen Namen.

### Erfassungsstellen

Alle Stationen innerhalb der Produktion (Produktionsbereiche, LKW, Maschinen), an denen sich Scanner und/oder Production Terminals befinden, werden als Erfassungsstellen (ES) bezeichnet. Sie erhalten eine eindeutige Nummer und einen Namen.

Eine Maschine muss nicht zwingend eine Erfassungsstelle sein. Sie kann durchaus in mehrere Erfassungsstellen aufgeteilt werden.

**Beispiel: ISO-Linie**
*   1611 > Maschineneingang,
*   1610 > die Maschine selbst und
*   1612 > Maschinenausgang.

Durch die Aufteilung von Maschinen in mehrere Erfassungsstellen ist eine genauere Verfolgung und Analyse der Produktion möglich.

Auf diese Erfassungsstellen können Sie Gestelle, Produkte und Zustände buchen. Je mehr Erfassungsstellen es gibt, um so genauer sind die Auswertungen.

[Image: Screenshot des Dialogs "Erfassungsstellen" mit einer Liste von IDs, Namen, Beschreibungen und Typen. Unten werden Details für die ausgewählte Erfassungsstelle Nr. 10 "Fertig" angezeigt, inklusive Barcode, Texten für Listen, Typ, Gruppierung und Rückmeldungsoptionen.]
*Abb. H-1 Erfassungsstellen*

Die Tabelle oben zeigt Ihnen, welche Erfassungsstellen bereits angelegt sind. Sie können neue Erfassungsstellen anlegen, aber auch Änderungen an bereits angelegten Erfassungsstellen vornehmen.

Bei den Checkboxen im Bereich *Rückmeldung von Buchungen* handelt es sich um Produktionsrückmeldungen, die dazu dienen, den aktuellen Auftragsstatus im übergeordneten Auftragsbearbeitungssystem zu aktualisieren.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

### Fehlergestell (Error-Rack)

Das Fehlergestell (Error-Rack) ist eine interne Erfassungsstelle. Diese Erfassungsstelle dient zur Aufnahme aller Einheiten, die aufgrund von Fehlern ihre Zuordnung zu einem physikalischen Gestell bzw. einer physikalischen Erfassungsstelle verloren haben.

Die interne Erfassungsstelle *Fehlergestell* hat die Erfassungsstellennummer 12.

Die Erfassungsstelle 12 folgt den gleichen Regeln wie jede andere Erfassungsstelle (Reports, Buchungen, Korrekturen, usw.).

Grundsätzlich gibt es zwei Regeln für die Erfassungsstelle Fehlergestell:
*   **Regel 1:** Das Fehlergestell sollte immer leer sein!
*   **Regel 2:** Ist das Fehlergestell nicht leer, liegt ein Bedien- oder Scannerfehler vor.

#### Wie gelangen Einheiten auf das Fehlergestell?

Hierfür gibt es mehrere Gründe. Neben einem defekten Scanner/Etikett, ist dies in der Regel eine Fehlbedienung durch das Personal.

Das Fehlergestell wird immer dann gefüllt, wenn eine Erfassungsstelle oder ein Gestell mit dem Status `<Begin>` gescannt wurde und sich A+W Production-seitig noch Einheiten auf diesem Objekt befanden. Diesen Einheiten wird automatisch die Erfassungsstelle Fehlergestell zugewiesen.

**Mögliche Ursachen:**

*   **Beispiel 1:**
    An einer Erfassungsstelle sind mehrere Gestelle im Zugriff. Im Scanner ist ein physikalisches Gestell angemeldet und es werden Einheiten auf dieses Gestell gebucht `<Gestell 1> <Einheit 1> <Einheit 2>`. Beim Wechsel auf das zweite Gestell wird vergessen, mit dem Scanner dieses Gestell anzumelden. Die Einheiten werden physikalisch auf Gestell 2 gestellt, buchungstechnisch aber auf das falsche Gestell, Gestell 1.
    Wird Gestell 1, welches physikalisch richtig beladen wurde, im weiteren Produktionsprozess regulär verarbeitet, steht dieses Gestell physikalisch leer und für weitere Aufgaben zur Verfügung.
    Nach den Regeln des Scannens wird beim nächsten Verwenden Gestell 1 mit `<Begin> <Rack1>` gescannt. Dies setzt das Gestell BDE-seitig zurück, d. h. auf leer.
    Intern (buchungstechnisch) befanden sich auf dem Gestell1 noch die falsch gescannten (zugeordneten) Einheiten von Gestell 2 (s. o). Diese Einheiten werden automatisch auf die Erfassungsstelle Fehlergestell gebucht.

*   **Beispiel 2:**
    Ein Lkw wird ordnungsgemäß beladen. Nachdem alle Einheiten, Gestelle und Kisten verladen sind, müsste der Lkw mit dem Status Shipped versehen werden `<Ausgeliefert><Lkw1>`.
    Dies unterbleibt jedoch. Der Lkw liefert seine Ware aus und steht am nächsten Tag physikalisch leer für den nächsten Transport zur Verfügung.
    Er wird entsprechend der Scanner-Regeln mit `<Beginn><Lkw1>` zum Beladen angemeldet und zurückgesetzt (leer).
    Da der Lkw durch die fehlende `<Ausgeliefert>`-Buchung vom Vortag buchungstechnisch beladen ist, wird seine komplette Ladung durch die Statusbuchung `<Beginn>` auf die Erfassungsstelle 12 Fehlergestell gebucht.

*   **Beispiel 3:**
    Ein beladenes Gestell wird ohne Einsatz eines Scanners bzw. mit einem defekten Scanner entladen. Physikalisch ist das Gestell leer, BDE-seitig noch beladen. Beim nächsten Einsatz des Gestells, unter Einhaltung der Scanner-Regeln `<Beginn><Gestell>`, werden diese Einheiten auf die Erfassungsstelle 12 Fehlergestell gebucht.

#### Einheiten vom Fehlergestell entfernen

Das Fehlergestell ist eine interne Erfassungsstelle. Einheiten, die sich dort befinden, können wie bei jeder anderen Erfassungsstelle, durch neue Buchungen manipuliert werden.

Es gibt zwei Methoden Einheiten die sich auf einer Erfassungsstelle, hier dem Fehlergestell, befinden, auf eine andere Erfassungsstelle/Gestell zu buchen.

Die manuelle Methode funktioniert über *Terminal Edit*. Sie müssen die Änderung der Erfassungsstelle (des Gestells) manuell im Terminal Edit vornehmen.

Die automatische Methode korrigiert einen Fehler automatisch durch eine weitere korrekte Buchung im Produktionsablauf.

> **Tipp**
> Überprüfen Sie regelmäßig die interne Erfassungsstelle 12 Fehlergestell und nehmen Sie Korrekturen umgehend vor. Für die Überprüfung stehen Ihnen neben *Terminal Edit* die Barcode Manager-Reports zur Verfügung.
> ⇨ "BDE-Reporting" auf Seite H-74
> Bedenken Sie bitte, es handelt sich Barcode-seitig um eine Erfassungsstelle. Sie haben dieselben Möglichkeiten und Werkzeuge wie für jede andere Erfassungsstelle, um Auswertungen und Korrekturen vorzunehmen!

> **Große Anzahl von Einheiten auf dem Fehlergestell**
> Hat sich eine sehr große Anzahl von Einheiten auf der internen Erfassungsstelle 12 Fehlergestell angesammelt, setzen sie sich bitte mit dem A+W-Kundenservice in Verbindung. A+W wird mit Ihnen zusammen eine kundenindividuelle und sachgerechte Lösung des Problems erarbeiten und die Ursachen analysieren.

#### Korrekte Buchung

Einheiten, die auf die interne Erfassungsstelle 12 Fehlergestell gelangt sind, werden von dort automatisch bei der nächsten korrekten Buchung dieser Einheiten an einer Erfassungsstelle, dieser Erfassungsstelle/dem Gestell zu geordnet, und verschwinden von der Erfassungsstelle Fehlergestell.

**Beispiel:**
Ein Gestell wird ohne Einsatz eines Scanners, bzw. mit einem defekten Scanner, entladen. Physikalisch ist das Gestell leer, Barcode-seitig noch beladen.

Beim nächsten Einsatz des Gestells, unter Einhaltung der Scanner-Regeln `<Beginn> <Gestell>`, werden diese Einheiten auf das Fehlergestell gebucht (gilt nur für Einheiten, die in der Zwischenzeit nicht erneut erfasst wurden, s.u.).

Voraussetzung für die automatische Korrektur ist, dass sich die Einheiten noch im Produktionsprozess befinden und bei weiteren Bearbeitungen gescannt werden.

Jeder dieser Scannvorgänge ordnet der Einheit die entsprechende Erfassungsstelle/das Gestell zu, die Einheit verschwindet automatisch von der internen Erfassungsstelle 12 Fehlergestell.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Erfassungsstellen" auf Seite H-94
*   ⇨ "Scannen im Versand" auf Seite H-51
*   ⇨ "Erfassungsstellen scannen" auf Seite H-53

### Erfassungsstellen verwalten

In dieser Einheit lernen Sie, wie Sie neue Erfassungsstellen anlegen, bearbeiten oder auch löschen.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
*   "So legen Sie eine neue Erfassungsstelle an" auf Seite H-23
*   "So löschen Sie eine Erfassungsstelle” auf Seite H-24
*   “So nehmen Sie Änderungen an Erfassungsstellen vor” auf Seite H-24

**So legen Sie eine neue Erfassungsstelle an**
1.  Öffnen Sie den Dialog *Erfassungsstelle*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**.
3.  Geben Sie im Feld *Erfassungsstellennr.* eine eindeutige Nummer für die Erfassungsstelle ein.
4.  Geben Sie im Feld *Barcode* die Barcode-Nummer für die Erfassungsstelle ein.
5.  Geben Sie im Feld *Name* den Namen der Erfassungsstelle ein.
6.  Im Feld *Beschreibung* können Sie eine Information zu der Erfassungsstelle hinterlegen.
7.  Im Feld *Text für Produktionslisten* geben Sie den Text ein, der auf den Produktionslisten erscheinen soll.
8.  Im Feld *Text für Kundenlisten* geben Sie den Text ein, der auf den Kundenlisten erscheinen soll.
9.  Im Feld *Unterzeile für Barcodeetiketten* geben Sie den Text ein, der unterhalb des Barcodes erscheinen soll.
10. Aus der Kombobox *Erfassungsstellen-Typ* wählen Sie aus, zu welchem Typ die Erfassungsstelle gehört.
11. Über das Feld *Gruppierung* können Sie, neben dem Erfassungsstellen-Typ, eine weitere Gruppierung hinterlegen, die zu Auswertungen verwendet wird.
12. Im Feld *Gruppierung für Arbeitsschichten* können Sie einzelne Erfassungsstellen für Arbeitsschichten gruppieren.
13. Im Feld *Aktueller Zustand* wählen Sie aus der Kombobox den entsprechenden Zustand aus.
14. Gibt es für die Erfassungsstelle eine Restriktionsprüfung, wird diese über die Kombobox *Restriktion* aktiviert und gesteuert.
15. Das Feld *Mengenüberschreitung* steht in direktem Zusammenhang mit dem Feld *Restriktion*. Nur, wenn das Feld Restriktion eine solche enthält, können Sie hier den entsprechenden Wert in Prozent hinterlegen.
16. Aktivieren Sie die Checkbox *Produzierte Teile anzeigen*, wenn komplett produzierte Scheiben im Production Terminal angezeigt werden sollen.
17. Sollte die Erfassungsstelle von der aus der Auftragserfassung übergebenen abweichen, dann überschreiben Sie den Eintrag.
18. Aktivieren Sie die Checkbox *Bearbeitungsrückmeldung*, wenn der Bearbeitungsfortschritt scheibengenau an das Auftragsbearbeitungssystem zurück gemeldet werden soll.
19. Aktivieren Sie die Checkbox *Gestellrückmeldung*, wenn die Gestellbelegung an das Auftragsbearbeitungssystem zurück gemeldet werden soll.
20. Aktivieren Sie die Checkbox *Gestellbelegung an Gestellserver melden*, wenn die Gestellbelegung an den Gestellserver zurück gemeldet werden soll.
21. Aktivieren Sie die Checkbox *Einheitenrückmeldung*, wenn fertige Einheiten an das Auftragserfassungssystem zurückgemeldet werden sollen.
22. Aktivieren Sie die Checkbox *Produktionsrückmeldung*, wenn eine Rückmeldung der fertigen Auftragspositionen an das Auftragsbearbeitungssystem erfolgen soll.
23. Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**So löschen Sie eine Erfassungsstelle**
1.  Öffnen Sie den Dialog *Erfassungsstelle*.
2.  Wählen Sie aus der Liste die Erfassungsstelle aus, die gelöscht werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**.
4.  Es folgt eine Sicherheitsabfrage, ob der Datensatz wirklich gelöscht werden soll.
5.  Klicken Sie auf **[Ja]**. Der Datensatz wird gelöscht.

**So nehmen Sie Änderungen an Erfassungsstellen vor**
1.  Öffnen Sie den Dialog *Erfassungsstelle*.
2.  Wählen Sie in der Liste die Erfassungsstelle aus, die geändert werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Ändern]**. Der Dialog wird zur Bearbeitung freigegeben.
4.  Nehmen Sie die gewünschten Änderungen vor.
5.  Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Erfassungsstellen" auf Seite H-94

### Erfassungsstelle Lkw

Jeder Lkw stellt eine Erfassungsstelle dar, die den gleichen Regeln folgt, wie jede andere Erfassungsstelle. Eine Ausnahme stellt das Barcode-seitige Leeren des Lkw dar. Objekte (Gestelle/Kisten usw.) verlassen in der Regel eine Erfassungsstelle dadurch, dass sie an einer anderen Erfassungsstelle angemeldet werden. Beim Lkw ist dies aus praktischen Erwägungen nicht sinnvoll. Es müsste beim Entladen z. B. auf der Baustelle gescannt werden.

Die Objekte müssen durch einen anderen Mechanismus Barcode-seitig von dieser Erfassungsstelle gebucht und der internen Erfassungsstelle 11 (Außer Haus) zugeführt werden. Diese Buchung darf jedoch erst durchgeführt werden, nachdem der Lkw wieder leer zurückgekommen ist!

Um einen komplizierten technischen Aufbau mit Scannern am Ausgangstor zu vermeiden, wird die Buchung auf die Erfassungsstelle 11 (Außer Haus) nach einer im System hinterlegten Zeitspanne durchgeführt, wenn der Lkw nach seiner Rückkehr mit `<Beginn><Lkw>` angemeldet wird.

Die Zeitspanne wird durch das Scannen des Status `<Ausgeliefert> <Lkw>` für den entsprechenden Lkw bzw. dessen Ladung getriggert.

Innerhalb dieser Zeitspanne gilt die Ladung als noch nicht ausgeliefert und befindet sich auf der Erfassungsstelle `<Lkw>` mit dem Status `<Ausgeliefert>`. Erst nach einer BEGINN Lesung NACH Ablauf der Zeitspanne ändert sich die ES auf 11.

Eine Status-Buchung `<Beginn><Lkw>` innerhalb der Zeitspanne würde den Lkw bzw. die Gestelle zurücksetzen und die betroffenen Einheiten auf das Fehlergestell buchen!

Nach der im System hinterlegten Zeitspanne gelten alle Einheiten als ausgeliefert und befinden sich auf der interne Erfassungsstelle 11 mit dem Status `<Ausgeliefert>`, die Gestelle bzw. der Lkw können wieder in den Produktionsprozess übernommen werden.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Erfassungsstellen" auf Seite H-94
*   ⇨ "Erfassungsstelle LKW" auf Seite H-56

---

## Abstellplätze

**Lernziele**
*   Den Dialog *Gestelle* erarbeiten.
*   Den Buchungsablauf kennenlernen und verstehen.

**Nutzen**
Um die BDE zu verstehen, müssen Sie wissen, was auf Abstellplätze gebucht werden kann.

**Definitionen**
*   **Gestell-Typen**: Zu den Gestell-Typen der BDE zählen A-Gestelle, L-Gestelle, Fächerwagen, Kisten und die besonderen Gestelle für Ofenbetten und Autoklaven.

**Merke**
*   **Gestell buchen**: Wird ein Gestell auf eine Erfassungsstelle gebucht, sind automatisch auch alle Einheiten des Gestells auf diese Erfassungsstelle gebucht.
*   **Gestelle anlegen**: Gestelle können in den Stammdaten manuell oder automatisch angelegt werden.
*   **Buchen**: Auf Gestelle können Produkte oder Zustände gebucht werden.
*   **Wo befindet sich ein Gestell**: Ein Gestell befindet sich immer an genau einem Ort (Erfassungsstelle).
*   **Kisten**: Kisten kehren nicht in den Produktionszyklus zurück.

### Gestelle

In diesem Bereich legen Sie die Gestelle für die A+W Production an. Es gibt folgende Gestelltypen:
*   A-Gestelle
*   L-Gestelle
*   Fächerwagen
*   Kisten

An einigen Erfassungsstellen sind besondere Gestelle notwendig. Das sind in der Regel Öfen und Autoklaven.

Auf die Gestelle können Produkte oder auch Zustände gebucht werden. Ein Gestell befindet sich immer an genau einem Ort in der Produktion (Erfassungsstelle).

[Image: Screenshot des Dialogs "Gestelle" mit einer Liste von Gestellen (ID, Name, Typ, Anzahl). Darunter Detailansicht für ein ausgewähltes Gestell mit den Bereichen Eigenschaften, Kundendaten und Laufdaten.]
*Abb. H-2 Gestelle*

Die Grafik oben zeigt Ihnen, welche Gestelle bereits angelegt sind. Sie können neue Gestelle anlegen, aber auch Änderungen an bereits angelegten Gestellen vornehmen.

#### Gestelle filtern

Verfügen Sie über eine große Anzahl an Gestellen, können Sie sich Filter anlegen, um die angezeigten Gestelle einzuschränken. Ob ein Filter gesetzt ist, sehen Sie im oberen Bereich des Dialogs.
Bei gesetztem Filter erscheint die Anzeige:

`▲Achtung: Gestellfilter ist gesetzt!`
*Abb. H-3 Gestellfilter gesetzt*

Ist kein Filter gesetzt, erscheint die Anzeige:

`[Filter..] Kein Gestellfilter gesetzt`
*Abb. H-4 Kein Gestellfilter gesetzt*

Um einen Filter zu aktivieren, betätigen Sie die Schaltfläche **[Filter]**. Es öffnet sich der Dialog *Gestellfilter*, in dem Sie einen entsprechenden Filter definieren und aktivieren können.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

### Kisten

Kisten werden zunächst wie Gestelle behandelt, kehren jedoch nicht wieder in den Produktionszyklus zurück. Aus diesem Grund ist es sinnvoll, für Kisten einen separaten Nummernkreis für die Barcodes zu verwenden.

Dieser Barcode-Bereich sollte immer komplett ausgedruckt und aufgebraucht werden. Damit wird sichergestellt, dass ein Barcode in der Produktion nicht mehrfach zeitgleich genutzt werden kann.

Selbstverständlich können Sie auch nacheinander kleinere Bereiche drucken und aufbrauchen z. B. 9000-9099, dann 9100-9199, dann 9200-9299 usw., doch sollte immer der gesamte Nummernkreis bis 9999 ausgenutzt werden.

Die Buchungshistorie für die Kisten bleibt aussagekräftig, wenn der Bereich komplett genutzt wird und die zwangsläufige Wiederholung eines Barcodes zeitlich weit auseinander liegt.

> **Erzeugen von Barcodes**
> Nutzen Sie immer den Report zum Erzeugen von Barcodes. Alternativ können die Barcodes auch über ein Microsoft Word Dokument zur Verfügung gestellt werden.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Gestelle" auf Seite H-98
*   ⇨ Softwarereferenz, "Gestellfilter" auf Seite H-102
*   ⇨ "BDE-Reporting" auf Seite H-74
*   ⇨ "Gestelle bzw. Kisten scannen" auf Seite H-59

### Gestelle verwalten

In dieser Einheit lernen Sie, wie Sie neue Gestelle anlegen, bearbeiten oder auch löschen.

*   "So legen Sie ein neues Gestell an"
*   "So legen Sie mehrere neue Gestell auf einmal an"
*   "So löschen Sie ein Gestell"
*   "So nehmen Sie Änderungen an einem Gestell vor"

**So legen Sie ein neues Gestell an**
1.  Öffnen Sie den Dialog *Gestelle*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**.
3.  Geben Sie im Feld *Name* eine eindeutige Namen für das Gestell ein.
4.  Im Feld *Barcode* geben Sie den Barcode für das Gestell ein.
5.  Wählen Sie aus der Kombobox *Gestellart* aus, ob es sich bei dem Gestell um ein Normales Gestell, ein Fachgestell oder eine Kiste handelt.
6.  Wählen Sie aus der Kombobox *Gestelltyp* aus, ob es sich bei dem Gestell um ein A-Gestell, einen Fächerwagen oder ein spezielles Gestell handelt.
7.  Sollte es sich bei dem Gestell um ein Fachgestell handeln, geben Sie im Feld *Fachnummer von bis* die erste und die letzte zu belegende Nummer an.
8.  Im Feld *Basis-ES* weisen Sie dem Gestell die Basis-Erfassungsstelle zu.
9.  Wenn es sich bei dem Gestell um ein temporäres Gestell handelt, aktivieren Sie die Checkbox *Temporäres Gestell*.
10. Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**So legen Sie mehrere neue Gestell auf einmal an**
1.  Öffnen Sie den Dialog *Gestelle*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**.
3.  Aktivieren Sie die Checkbox *Mehrere Gestelle anlegen*. Unterhalb der Checkbox erscheinen die Felder *Präfix*, *Startwert*, *Endwert* und *BC-Startwert*.
4.  Im Feld *Präfix* können Sie einen Buchstaben oder eine Buchstabenkombination eingeben, die dem Startwert voran gestellt wird.
5.  Im Feld *Startwert* geben Sie erste Nummer für die Gestelle ein.
6.  Im Feld *Endwert* geben Sie letzte Nummer für die Gestelle ein.
7.  Im Feld *BC-Startwert* geben Sie ein, mit welcher Barcode-Nummer begonnen werden soll.
8.  Wählen Sie aus der Kombobox *Gestellart* aus, ob es sich bei den Gestellen um Normale Gestelle, Fachgestelle oder Kisten handelt.
9.  Wählen Sie aus der Kombobox *Gestelltyp* aus, ob es sich bei den Gestellen um A-Gestelle, Fächerwagen oder um spezielle Gestelle handelt.
10. Sollte es sich bei den Gestellen um Fachgestelle handeln, geben Sie im Feld *Fachnummer von bis* die erste und die letzte zu belegende Nummer an.
11. Im Feld *Basis-ES* weisen Sie den Gestellen die Basis-Erfassungsstelle zu.
12. Wenn es sich bei den Gestellen um temporäre Gestelle handelt, aktivieren Sie die Checkbox *Temporäres Gestell*.
13. Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.
14. Es erscheint eine Abfrage, ob Sie wirklich die entsprechende Anzahl an Gestellen einfügen möchten.

**So löschen Sie ein Gestell**
1.  Öffnen Sie den Dialog *Gestelle*.
2.  Wählen Sie aus der Liste das Gestell aus, das gelöscht werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**.
4.  Es folgt eine Sicherheitsabfrage, ob der Datensatz wirklich gelöscht werden soll.
5.  Klicken Sie auf **[Ja]**. Der Datensatz wird gelöscht.

**So nehmen Sie Änderungen an einem Gestell vor**
1.  Öffnen Sie den Dialog *Gestelle*.
2.  Wählen Sie in der Liste der Gestelle das aus, was geändert werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Ändern]**. Der Dialog wird zur Bearbeitung freigegeben.
4.  Nehmen Sie die gewünschten Änderungen vor.
5.  Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**So setzen Sie einen Gestellfilter**
1.  Öffnen Sie den Dialog *Gestelle*.
2.  Betätigen Sie die Schaltfläche **[Filter]**. Es öffnet sich der Dialog *Gestellfilter*.
3.  Sie können nach den folgenden Kriterien filtern:
    *   Erfassungsstellen-Typen
    *   Erfassungsstellen
    *   Gestellnamen
    *   Gestellart
    *   Gestelltyp
4.  Nehmen Sie die gewünschten Einstellungen vor.
5.  Klicken Sie auf die Schaltfläche **[Übernehmen]**, um die Angaben zu speichern.
6.  Klicken Sie auf das **[X]**, um den Dialog zu schließen.

**So löschen Sie einen Gestellfilter**
1.  Öffnen Sie den Dialog *Gestelle*.
2.  Betätigen Sie die Schaltfläche **[Filter]**. Es öffnet sich der Dialog *Gestellfilter*.
3.  Klicken Sie auf die Schaltfläche **[Zurücksetzen]**, um den eingestellten Filter zu löschen.
4.  Klicken Sie auf das **[X]**, um den Dialog zu schließen.
5.  Es werden wieder alle Gestelle angezeigt.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Gestelle" auf Seite H-98
*   ⇨ Softwarereferenz, "Gestellfilter" auf Seite H-102
*   ⇨ "Gestelle bzw. Kisten scannen" auf Seite H-59

---

## Personal

**Lernziele**
*   Den Dialog *Mitarbeiter* erarbeiten.
*   Den Umgang mit den Mitarbeitern kennenlernen und verstehen.
*   Mitarbeiter anlegen und bearbeiten.

**Nutzen**
Für jeden Mitarbeiter können unterschiedliche Kostensätze hinterlegt werden. Damit können die Personalkosten genauer berücksichtigt werden. Darüber hinaus kann ausgewertet werden, wie viele Mitarbeiter an einer Bearbeitung beteiligt waren.

**Merke**
*   **Mitarbeiter anlegen**: Ein Mitarbeiter muss erst angelegt werden, bevor er sich an einer Station anmelden kann.
*   **Angemeldete Person**: Wird der Buchung mitgegeben. Dies ist der für die Buchung verantwortliche Mitarbeiter. Die angemeldete Person bleibt so lange angemeldet, bis ein anderer Namen-Barcode gescannt wird.
*   **Anmeldung zwingend erforderlich**: Scanner und A+W Production Termin können so eingestellt werden, dass eine Personenanmeldung zwingend erforderlich ist.

### Mitarbeiter

Alle Mitarbeiter, die in Ihrem Hause mit der A+W Production zu tun haben, müssen einmal registriert (erfasst) werden. Nachdem ein Mitarbeiter erfasst ist, kann er sich an den einzelnen Stationen anmelden. Er wird dann automatisch den einzelnen Buchungen mitgegeben und ist der für die Buchung verantwortliche Mitarbeiter.

[Image: Screenshot des Dialogs "Personal" mit einer Liste von Mitarbeitern (Nummer, Name, Personal-Nr., Beschreibung, Barcode).]
*Abb. H-5 Mitarbeiter*

Die Tabelle oben zeigt Ihnen, welche Mitarbeiter bereits angelegt sind. Sie können neue Mitarbeiter anlegen, aber auch Änderungen an bereits angelegten Mitarbeitern vornehmen.

Für jeden Mitarbeiter können unterschiedliche Kostensätze hinterlegt werden. Auf diese Weise können die jeweiligen Personalkosten genauer berücksichtigt werden.

Darüber hinaus ist es möglich, dass mehrere Mitarbeiter an einer Station angemeldet werden. Somit wissen Sie, wie viele Mitarbeiter an einer Bearbeitung beteiligt waren.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Mitarbeiter" auf Seite H-106

### Mitarbeiter verwalten

In dieser Einheit lernen Sie, wie Sie neue Mitarbeiter anlegen, bearbeiten oder auch löschen.

*   "So legen Sie einen neuen Mitarbeiter an"
*   "So löschen Sie einen Mitarbeiter"
*   "So nehmen Sie Änderungen an Mitarbeiterdaten vor"

**So legen Sie einen neuen Mitarbeiter an**
1.  Öffnen Sie den Dialog *Mitarbeiter*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**.
3.  Geben Sie im Feld *Nummer* eine eindeutige Nummer für den Mitarbeiter ein.
4.  Geben Sie im Feld *Name* den Namen des Mitarbeiters ein.
5.  Im Feld *Beschreibung* können Sie eine Information zu dem Mitarbeiter hinterlegen.
6.  Im Feld *Personal-Nr.* geben Sie die Personal-Nummer des Mitarbeiters ein. Diese können Sie im Lohnbüro oder der Buchhaltung erfragen.
7.  Geben Sie im Feld *Barcode* die Barcode-Nummer für den Mitarbeiter ein. Bei einem 9stelligen Barcode kann das eine Zusammensetzung aus den Feldern Nummer und Personal-Nr. sein. Beispiel: Der Mitarbeiter hat die Nummer 60 und die Personal-Nr. ist die 51, dann ist der Barcode: 600000051.
8.  Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**So löschen Sie einen Mitarbeiter**
1.  Öffnen Sie den Dialog *Mitarbeiter*.
2.  Wählen Sie aus der Liste den Mitarbeiter aus, der gelöscht werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**.
4.  Es folgt eine Sicherheitsabfrage, ob der Datensatz wirklich gelöscht werden soll.
5.  Klicken Sie auf **[Ja]**. Der Datensatz wird gelöscht.

**So nehmen Sie Änderungen an Mitarbeiterdaten vor**
1.  Öffnen Sie den Dialog *Mitarbeiter*.
2.  Wählen Sie in der Liste den Mitarbeiter aus, der geändert werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Ändern]**. Der Dialog wird zur Bearbeitung freigegeben.
4.  Nehmen Sie die gewünschten Änderungen vor.
5.  Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Mitarbeiter" auf Seite H-106

---

## Status

**Lernziele**
*   Den Dialog *Zustände* erarbeiten.
*   Unterschiedliche Zustand-Typen kennenlernen und verstehen.

**Nutzen**
Um aussagekräftige Auswertungen zu erhalten, muss eine gewisse Buchungsdisziplin eingehalten werden.

**Definitionen**

| Begriff | Beschreibung |
| :--- | :--- |
| **Zustände** | Beschreiben den Zustand eines Objektes |
| **Maschinen-Zustand** | Bereit, Aus, Störung, Wartung, Pause, ... |
| **Produkt-Zustand** | Bruch, Mangel, ... |
| **Gestell-Zustand** | Leer, fertig, ausgeliefert, ... |
| **Erfassungsstellen-Zustand** | Fertig, ausgeliefert, leer, ... |
| **Aktions-Zustand** | OK, abbrechen, übernehmen, ... |

**Merke**
*   **Unterbrechungen**: Arbeitsunterbrechungen müssen immer protokolliert werden.

### Zustände

Die Aufgabe der A+W Production ist es, den IST-Zustand eines Objektes innerhalb der Produktion zu erfassen.

Um aussagekräftige Auswertungen der Daten zu erhalten, müssen die Stammdaten gepflegt werden und es ist zwingend notwendig, Daten (Mengen und Objekte) korrekt und zeitnah zu buchen.

Zustände wirken auf folgende A+W Production-Objekte:
*   Einheit/Gruppe
*   Gestell
*   Erfassungsstellen
*   Personal

#### Einheit/Gruppe

Hier geht es darum, den Status einer Scheibe bzw. Einheit oder eines Produktes zu erfassen.
Hierfür gibt es z. B. folgende Zustände:
*   Noch nicht produziert
*   Bruchscheibe
*   Mangel
*   Versandfertig

#### Gestell

Hier geht es darum, den Status eines Gestells zu erfassen.
Gestelle können sich z. B. in den folgenden Stati befinden:
*   Leer
*   Voll
*   Außer Haus
*   Versandfertig

#### Erfassungsstelle

Hier geht es darum, den Status einer Erfassungsstelle zu buchen.
Erfassungsstellen können sich z. B. in den folgenden Stati befinden:
*   Beginn
*   An
*   Aus

Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit an einer Erfassungsstelle unterbrochen werden muss. Eine solche Unterbrechung muss immer protokolliert werden.

Gründe für eine Unterbrechung können sein:
*   Wartung der Maschine
*   Störung der Maschine
*   Pausenzeiten
*   Rüstzeiten

#### Aktions-Barcode

Neben dem Erfassen der oben genannten Zustände gibt es noch die Möglichkeit, verschiedene Aktionen zu scannen.
Dazu gehören z. B.:
*   OK
*   Abbrechen
*   Rotieren
*   Nächste Zeile

[Image: Screenshot des Dialogs "Zustände" mit einer Liste von IDs, Namen, Beschreibungen. Details für den Zustand "Bruch" werden unten angezeigt.]
*Abb. H-6 Zustände*

Die Tabelle oben zeigt Ihnen, welche Zustände bereits angelegt sind. Sie können neue Zustände anlegen, aber auch Änderungen an bereits angelegten Zustände vornehmen.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Zustände" auf Seite H-104
*   ⇨ "Status scannen" auf Seite H-61

### Zustände verwalten

In dieser Einheit lernen Sie, wie Sie neue Zustände anlegen, bearbeiten oder auch löschen.

*   "So legen Sie einen neuen Zustand an"
*   "So löschen Sie einen Zustand"
*   "So nehmen Sie Änderungen an Zustandsdaten vor”

**So legen Sie einen neuen Zustand an**
1.  Öffnen Sie den Dialog *Zustände*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**.
3.  Geben Sie im Feld *Zustandsnummer* eine eindeutige Nummer für den Zustand ein.
4.  Geben Sie im Feld *Name* den Namen des Zustandes ein.
5.  Im Feld *Beschreibung* geben Sie eine Information zu dem Zustand ein, z. B. Werkzeugwechsel.
6.  Im Feld *Text für Listen* geben Sie den Text ein, der auf den Listen erscheinen soll.
7.  Geben Sie im Feld *Barcode* die 9stellige Barcode-Nummer für den Zustand ein.
8.  Wählen Sie aus der Kombobox *Zustandstyp* den entsprechenden Typ aus.
9.  Aktivieren Sie aus der Checkbox *AWRack-Info*, wenn bei Änderung auf diesem Zustand der Gestellserver benachrichtigt werden soll.
10. Wählen Sie aus der Kombobox *AWRack-Status* den entsprechenden Status aus.
11. Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**So löschen Sie einen Zustand**
1.  Öffnen Sie den Dialog *Zustände*.
2.  Wählen Sie aus der Liste den Zustand aus, der gelöscht werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**.
4.  Es folgt eine Sicherheitsabfrage, ob der Datensatz wirklich gelöscht werden soll.
5.  Klicken Sie auf **[Ja]**. Der Datensatz wird gelöscht.

**So nehmen Sie Änderungen an Zustandsdaten vor**
1.  Öffnen Sie den Dialog *Zustände*.
2.  Wählen Sie in der Liste den Zustande aus, der geändert werden soll.
3.  Betätigen Sie die Symbol-Schaltfläche **[Ändern]**. Der Dialog wird zur Bearbeitung freigegeben.
4.  Nehmen Sie die gewünschten Änderungen vor.
5.  Klicken Sie auf die Symbol-Schaltfläche **[Speichern]**, um die Angaben zu speichern.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Zustände" auf Seite H-104
*   ⇨ "Status scannen" auf Seite H-61

---

## Datenerfassung

In diesem Themenblock lernen Sie, auf welche Art und Weise und an welchen Stellen in der Produktion Daten erfasst werden.
Dazu gehören folgende Lerneinheiten:
*   "Scanner" auf Seite H-42
*   "Barcodes" auf Seite H-45

### Scanner

**Lernziele**
*   Unterschiedliche Scanner kennenlernen.
*   Die Funktionsweise kennenlernen und verstehen.
*   Die Konfiguration der Scanner kennenlernen.

**Nutzen**
Die Verwendung von Scannern trägt zu einer enormen Arbeitserleichterung bei und spart Zeit.

**Definitionen**

| Typ | Beschreibung |
| :--- | :--- |
| **Online Scanner** | Besitzen keinen Speicher und die Scandaten müssen direkt an das angeschlossene System weitergeleitet werden. Ist die Verbindung unterbrochen, gehen die gescannten Daten verloren. |
| **Offline Scanner** | Verfügen über einen Speicher, der die gescannten Daten zwischenspeichern kann und bei der Verbindung mit dem System seine Daten übergibt. |
| **Serielle Scanner** | Werden u. a. an den Terminals eingesetzt. Der Scanner speichert keine Informationen zwischen. D. h., wenn keine Verbindung zum Netzwerk besteht, gehen die Daten verloren. |

**Merke**
*   **Konfiguration**: Scanner benötigen neben ihrem Betriebssystem eine Software, die die gewünschten Funktionen ausführt.

### Scanner-Typen

In der BDE kommen verschiedene Scanner-Typen zum Einsatz. Grundsätzlich wird zwischen Online- und Offline-Scannern unterschieden.
*   Online-Scanner
*   Offline-Scanner

Die Auswahl der verschiedenen Scanner ist sehr individuell und hängt von mehreren unterschiedlichen Faktoren ab, z. B.:
*   Wie viele Scanner mit verschiedenen Protokollen sollen zum Einsatz kommen?
*   Wo kommen die Scanner zum Einsatz?
*   Welchen Aktionsradius müssen die Scanner abdecken?

Darüber hinaus gibt es noch eine Reihe weiterer Faktoren, die jeweils im Gespräch mit dem Kunden vor Ort geklärt werden.

#### Online-Scanner

Zu den Online-Scannern gehören die Linienscanner bzw. serielle Scanner, die in der Regel keinen Speicher besitzen und die Scanndaten direkt an das angeschlossene System weiterleiten müssen. Ist die Verbindung unterbrochen, gehen die gescannten Daten verloren.

#### Denso-Scanner (WLAN)

Diese Scanner sind WLAN-fähig und kommunizieren direkt mit AWPort. Sie besitzen ein Display und haben einen Zwischenspeicher zum Puffern der Daten. Meldungen an den Benutzer sind über das eingebaute Display und die Menüstruktur des Scanners möglich. Wird die Datenübertragung unterbrochen (z. B. außerhalb der Reichweite der Empfangsstation), werden die Daten im Scanner zwischengespeichert und bei der nächsten Verbindung übertragen. Diese Scanner kommen u. a. im Versand zum Einsatz.

[Image: Photo of a Denso handheld scanner.]
*Abb. H-7 Denso Online-Scanner*

#### Serielle Scanner

Die seriellen Scanner kommen an den Production Terminals oder in Verbindung mit AWPort-Light als freie Online-Scanner zum Einsatz. In Verbindung mit den Production Terminals sind sie überwiegend der Erfassungsstelle fest zu geordnet (konfigurierbar) und ersetzen die Tastatur. Buchungen übernimmt das angeschlossene Production Terminal.

In Verbindung mit AWPort-Light können diese Scanner auch als freie Online-Scanner überall dort eingesetzt werden, wo ein Production Terminal nicht benötigt wird. Solche Scanner sind robust und günstig. Sie besitzen allerdings kein Display und keinen Zwischenspeicher. Meldungen an den Benutzer sind daher nur sehr eingeschränkt möglich. Da diese Scanner meist keinen Zwischenspeicher besitzen, gehen bei der Unterbrechung der Datenübertragung (z. B. außerhalb der Reichweite der Empfangsstation) die gescannten Daten verloren.

#### Offline-Scanner

Der Einsatz von Offline-Scannern in einer A+W Production-Umgebung unterliegt besonderen Restriktionen. Unter Offline-Scannern werden Barcode-Lesegeräte verstanden, die die Barcode-Lesungen erst sammeln und dann später gesammelt übertragen. Da diese Übertragung in der Regel manuell ausgelöst werden muss, kommen Lesungen durch Offline-Scanner (deutlich) später zur Auswertung als bei Online-Scannern.

Diese Scanner erfordern vom Benutzer eine strukturierte und disziplinierte Arbeitsweise!

### Konfiguration der Scanner

Die Konfiguration der Scanner erfolgt mehrschichtig. Scanner benötigen neben ihrem Betriebssystem eine Software, die die gewünschten Funktionen ausführt. Diese Software wird von A+W zur Verfügung gestellt und muss auf den Scanner übertragen und konfiguriert werden.

Außerdem müssen die Scanner am A+W Production-System angemeldet werden.

Die notwendigen Schritte zur Konfiguration werden in der Regel von A+W durchgeführt, können aber auch von geschultem Fachpersonal ausgeführt werden.

> **Scanner in der Praxis**
> Aktuell werden fast ausschließlich WLAN-Scanner vom Typ BHT800BW eingesetzt. Der Vorteil dieses Typs ist, dass die erfassten Daten immer online zur Verfügung stehen.

> **Dokumentation der Konfiguration**
> Eine Dokumentation mit der kundenindividuellen Konfiguration wird in der Projektierungsphase erstellt und auf dem Kundenrechner gespeichert und gepflegt.

### Barcodes

Scanner benötigen als Eingaben in der Regel Barcodes. Jede Person, jede Erfassungsstelle, jedes Gestell, usw. erhält eine eindeutige Nummer, die als Barcodes für den Scanner kodiert werden. Diese Nummern werden in der Projektierungsphase von A+W Software GmbH zusammen mit dem Kunden festgelegt. Diese Barcodes werden u. a. über einen Report von A+W Production zur Verfügung gestellt.

Benötigen Sie neue Barcodes für Personen, Erfassungsstellen oder Gestelle bzw. Kisten, starten Sie den Report und drucken die gewünschten Barcodes aus.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Barcode-Optionen" auf Seite H-91
*   ⇨ Softwarereferenz, "Barcode-Typen" auf Seite H-92

---

## Buchungsbeispiele

In diesem Themenblock lernen Sie, wie richtig gebucht wird.
Dazu gehören folgende Lerneinheiten:
*   "Die Reihenfolge des Scannens" auf Seite H-47
*   "Scannen von Einheiten" auf Seite H-49
*   "Scannen im Versand" auf Seite H-51
*   "Erfassungsstellen scannen" auf Seite H-53
*   "Erfassungsstelle LKW" auf Seite H-56
*   "Gestelle bzw. Kisten scannen" auf Seite H-59
*   "Status scannen" auf Seite H-61
*   "Korrigieren von Fehlbuchungen" auf Seite H-62

### Die Reihenfolge des Scannens

Die folgenden Beispiele sollen Ihnen einen Überblick über die einzuhaltende Reihenfolge beim Scannen geben. Um die Beispiele übersichtlich zu halten, wurde jeweils auf die komplette Darstellungskette verzichtet, d. h. es wird davon ausgegangen, dass z. B. beim Scannen von Einheiten der Scanner an einer Erfassungsstelle angemeldet wurde, der Mitarbeiter seinen persönlichen Barcode gescannt hat usw. Die Gesamtreihenfolge des Scannens ergibt sich aus der Kombination der aufgeführten Beispiele und ist abhängig von der Erfassungsstelle.

Beim Scannen wird immer zunächst der Scanner vorbereitet, indem die Person, die mit ihm arbeitet, angemeldet wird (optional), die Erfassungsstelle am Scanner angemeldet wird und dann die weiteren Buchungen erfolgen, in der Regel ist dies ein Gestell anmelden.

Das Anmelden der Person, der Erfassungsstelle, das Scannen eines Status usw. hat ausschließlich Auswirkungen auf alle zukünftigen Buchungen z. B. das Scannen einer Einheit, die dann mit all diesen Informationen im System durch ALCIM-Booking gespeichert wird.

**Die Reihenfolge beim Scannen:**
1.  Der **Mitarbeiter**, der den Scanner bedient, sollte seinen persönlichen Barcode am Beginn der Schicht/des Scannens einscannen. Diese Information wird zu jedem Scannvorgang gespeichert und dient späteren Auswertungszwecken. Wird dieser Barcode nicht gescannt, wird ein konfigurierbarer Standardwert in die Datenbank geschrieben. Ein (neuer) Namensbarcode kann jederzeit gescannt werden, auch nachdem der Scanner an der Erfassungsstelle angemeldet wurde, z. B. wegen eines Mitarbeiterwechsels an der Erfassungsstelle.
2.  Die **Erfassungsstelle**, an der der Scanner eingesetzt wird, muss dem Scanner immer aktuell bekannt sein. Jeder Bereich, jede Maschine, jeder Lkw, der/die als Erfassungsstelle eingerichtet wurde, hat einen eigenen Barcode. Beispiele sind: Zuschnitt, ISO-Linie 1, ISO-Linie2, Ofen, Versand, Lkw1, Lkw2, usw.
3.  Das **Gestell** (die Kiste), auf das Einheiten abgestellt werden, muss gescannt, d. h. am Scanner angemeldet werden. Befinden sich mehrere Gestelle an der Erfassungsstelle, muss immer das aktuell zu beladende Gestell am Scanner angemeldet sein/werden. Ausnahme: Im Versand werden Einheiten auch direkt auf die Erfassungsstelle (Lkw) gebucht (siehe auch Sonderfall Lkw).
4.  Die **Einheiten**: nachdem die Punkte 1-3 gescannt wurden, werden die Einheiten gescannt, die abgestellt werden sollen bzw. deren Status sich verändert hat (z. B. Bruchmeldung).

**Erläuterung**
`<Text>` der Text in den spitzen Klammern bezeichnet den zu scannenden Barcode (Erfassungsstelle, Gestell, Status, Einheit usw.).
Die Zeile `<Begin> <Rack> <Unit1> < Unit2> <Unit3 ...>` bedeutet, Scannen Sie den Status `<Begin>`, dann das Gestell `<Rack>`, auf welches z. B. die Einheiten gestellt werden sollen und dann alle Einheiten `<Unit>` in der Reihenfolge, in der sie auf dieses Gestell abgestellt werden sollen.

> **Achtung beim Barcode `<Beginn>`**
> Der Barcode `<Begin>` setzt das Gestell, die Kiste, den Lkw usw. BDE-seitig immer auf leer (Reset)! Befanden sich BDE-seitig noch Einheiten z.B. auf dem Gestell, werden diese der Erfassungsstelle Fehlergestelle (Error-Rack) zugewiesen (siehe Fehlergestell (Error-Rack), Seite 50)!
> Solche BDE-seitig übrig gebliebenen Einheiten können nur durch vergessene Scanns, fehlerhafte Etiketten (Fehllesungen), usw. vorkommen!

### Scannen von Einheiten

In dieser Einheit lernen Sie, wie Sie Einheiten scannen.
Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
*   So scannen Sie eine Einheit auf ein leeres Gestell (Gestell wird BDE-seitig geleert).
*   So scannen Sie eine Einheit auf ein Gestell, auf dem bereits Einheiten stehen.
*   So scannen Sie Bruchmeldung Einheiten.
*   So scannen Sie Auslieferung Einheiten.
*   So scannen Sie Einheiten auf eine leere Erfassungsstelle: Sonderfall LKW.
*   So scannen Sie Einheiten auf eine Erfassungsstelle, die bereits Einheiten enthält.

**So scannen Sie eine Einheit auf ein leeres Gestell (Gestell wird BDE-seitig geleert)**
1.  Melden Sie ein leeres Gestell am Scanner an: `<Beginn> <Gestell>`
    [Image: Barcode for 'begin' and a picture of an empty rack.]
2.  Scannen Sie das Etikett der Einheit:
    [Image: Barcode on a piece of glass.]
    `<Einheit 1>`
    `<Einheit 2>`
    `<Einheit 3>`
    `<Einheit 4>`
    ...

**So scannen Sie eine Einheit auf ein Gestell, auf dem bereits Einheiten stehen**
`<Gestell> <Einheit 1> <Einheit 2> <Einheit ...>`

**So scannen Sie Bruchmeldung Einheiten**
`<Bruch> <Einheit 1> <Bruch> <Einheit 2> <Bruch> < Einheit ...>`

**So scannen Sie Auslieferung Einheiten**
`<Ausgeliefert> <Einheit 1> <Ausgeliefert> <Einheit 2> <Ausgeliefert> <Einheit ...>`

**So scannen Sie Einheiten auf eine leere Erfassungsstelle: Sonderfall LKW**
`<Beginn> <ErfStelle> <Einheit 1> <Einheit 2> <Einheit ...>`

**So scannen Sie Einheiten auf eine Erfassungsstelle, die bereits Einheiten einhält**
`<ErfStelle> <Einheit 1> <Einheit 2> <Einheit ...>`

**Ergänzende Informationen**
*   ⇨ "Scheiben bzw. Einheiten" auf Seite H-16

### Scannen im Versand

Dem Versand muss BDE-seitig besondere Aufmerksamkeit geschenkt werden. Es handelt sich um eine Erfassungsstelle, auf der sich Einheiten, Gestelle, Kisten usw. befinden, aber auch Lkw, die ihrerseits Erfassungsstellen darstellen und letztendlich den Abschluss der Produktion bilden. In der Regel kommen hier Denso Online-Scanner zum Einsatz.

**Grundsätzliche Vorgehensweise:**
1.  Scannen Sie zunächst den Name-Tag (der Name-Tag kann jederzeit neu gelesen werden). `<Schmidt>`
    [Image: Name tag barcode for 'Schmidt'.]
2.  Melden Sie die Erfassungsstelle am Scanner an. Anschließend scannen Sie Versand Bereich von der Liste. `<Versand Bereich>`
    [Image: Barcode for 'Shipping Area'.]
3.  Scannen Sie das Gestell, auf das die Einheiten gestellt werden sollen. `<Gestell 1>`
    [Image: Picture of a glass rack.]
4.  Scannen Sie das Etikett der Einheit.
    [Image: Barcode on a piece of glass.]
    `<Einheit 1>`
    `<Einheit 2>`
    `<Einheit 3>`
    `<Einheit 4>`

> **Hinweis**
> Achten Sie auf die Reihenfolge des Scannens, wenn Sie Einheiten und Gestelle/Kisten in einer beliebigen Reihenfolge laden wollen bzw. müssen!

**Ergänzende Informationen**
*   ⇨ "Scanner" auf Seite H-42
*   ⇨ "Erfassungsstelle Lkw" auf Seite H-25
*   ⇨ Softwarereferenz, "Erfassungsstellen" auf Seite H-94

### Erfassungsstellen scannen

Jede Erfassungsstelle hat einen eigenen Barcode. Beispiele für Erfassungsstellen sind:
*   Zuschnitt,
*   ISO-Linie 1,
*   ISO-Linie2,
*   Ofen,
*   Versand,
*   Lkw1,
*   Lkw2
*   usw.

**Handlungsanweisungen:**
*   "So scannen Sie Einheiten auf eine leere Erfassungsstelle (Erfassungsstelle wird BDE-seitig geleert): Sonderfall LKW"
*   "So scannen Sie Einheiten auf eine Erfassungsstelle:"
*   "So scannen Sie Einheiten auf verschiedene Erfassungsstellen:"
*   "So scannen Sie Gestelle auf eine Erfassungsstelle:"
*   "So scannen Sie Gestelle auf verschiedene Erfassungsstellen:"
*   "So scannen Sie eine Erfassungsstelle fertig:"
*   "So scannen Sie die Auslieferung Lkw oder Auflieger:"

**So scannen Sie Einheiten auf eine leere Erfassungsstelle (Erfassungsstelle wird BDE-seitig geleert): Sonderfall LKW**
1.  Melden Sie eine neue Erfassungsstelle am Scanner an: `<Beginn> <ErfStelle>`
    [Image: Barcode for 'begin'.]
2.  Scannen Sie das Etikett der Scheibe/Einheit.
    [Image: Barcode on a piece of glass.]
    `<Einheit 1>`
    `<Einheit 2>`
    `<Einheit 3>`
    `<Einheit 4>`
    ...

**So scannen Sie Einheiten auf eine Erfassungsstelle:**
1.  Melden Sie die Erfassungsstelle am Scanner an: `<ErfStelle>`
2.  Scannen Sie das Etikett der Scheibe/Einheit: `<Einheit 1> <Einheit 2> <Einheit ...>`

**So scannen Sie Einheiten auf verschiedene Erfassungsstellen:**
`<ErfStelle 1> <Einheit 1> <Einheit 2>`
`<ErfStelle 3> <Einheit 3> <Einheit 4> <Einheit 5>`
`<ErfStelle 1> <Einheit 6>`
`<ErfStelle 2> <Einheit 7> <Einheit 8> <Einheit 9>`
...

**So scannen Sie Gestelle auf eine Erfassungsstelle:**
`<ErfStelle> <Gestell 1> <Gestell 2> <Gestell ...>`

**So scannen Sie Gestelle auf verschiedene Erfassungsstellen:**
`<ErfStelle 1> <Gestell 1> <Gestell 2>`
`<ErfStelle 2> <Gestell 3>`
`<ErfStelle 1> <Gestell 4>`
`<ErfStelle 2> <Gestell 5> Gestell 6>`
`<ErfStelle 3> <Gestell 7>`
...

**So scannen Sie eine Erfassungsstelle fertig:**
`<Fertig> <ErfStelle>`

**So scannen Sie die Auslieferung Lkw oder Auflieger:**
`<Ausgeliefert> <ErfStelle>`

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Erfassungsstellen" auf Seite H-94

### Erfassungsstelle LKW

In dieser Einheit lernen Sie, wie Sie die Erfassungsstelle Lkw scannen.
*   "Grundsätzliche Vorgehensweise:"
*   "Beladen eines leeren und eines teilbeladenen LKW"

**Grundsätzliche Vorgehensweise:**
1.  Scannen Sie zunächst den Name-Tag: `<Schmidt>`
    [Image: Name tag barcode for 'Schmidt'.]
2.  Melden Sie einen neue Lkw am Scanner an: `<Beginn> <Lkw 1>`
    [Image: Barcode for 'begin' and an image of a truck.]
3.  oder melden Sie einen teilbeladenen Lkw am Scanner an: `<Lkw 2>`
4.  Scannen Sie das Etikett der Einheit:
    [Image: Barcode on a piece of glass.]
    `<Einheit 1>`
    `<Einheit 2>`
    `<Einheit 3>`
    `<Einheit 4>`
    ...

#### Übungen: Beladen eines leeren und eines teilbeladenen LKW

Lkw 1 (leer) und Lkw 2 (teilbeladen) sollen beladen werden. Die Reihenfolge der Beladung soll beliebig sein, d.h. die Lkw können in beliebiger Reihenfolge beladen und die Gestelle und Einheiten in beliebiger Reihenfolge geladen werden.

1.  **Lkw 1 (ES) am Scanner anmelden**
    `<Beginn> <Lkw1>`
2.  **Einheiten direkt auf Lkw 1 buchen**
    `<Einheit 1> <Einheit 2> <Einheit 3>`
3.  **Gestelle auf Lkw 1 buchen**
    `<Gestell 1> <Gestell 2>`
4.  **Lkw 1 erneut anmelden.** Das letzte Gestell wird dadurch abgemeldet, die folgenden Einheiten können direkt auf den Lkw gebucht werden. Unterbleibt dieser Schritt, werden die folgenden Einheiten auf das letzte Gestell (Gestell 2 auf dem Lkw 1) gebucht.
    `<Lkw1>`
5.  **Einheiten direkt auf Lkw 1 buchen**
    `<Einheit 4> <Einheit 5>`
6.  **Gestelle auf Lkw 1 buchen**
    `<Gestell 3> <Gestell 4> <Gestell 5> <Gestell 6>`
7.  **Lkw 2 (ES) am Scanner anmelden.** Dadurch wird Lkw 1 automatisch abgemeldet.
    `<Lkw2>`
8.  **Gestelle auf Lkw 2 buchen**
    `<Gestell 9> <Gestell 10> <Gestell 11>`
9.  **Lkw2 erneut anmelden.** Das letzte Gestell wird dadurch abgemeldet, die folgenden Einheiten können direkt auf den Lkw gebucht werden. Unterbleibt dieser Schritt, werden die folgenden Einheiten auf das letzte Gestell (Rack11 auf dem Lkw 2) gebucht.
    `<Gestell 2>`
10. **Einheiten direkt auf Lkw 2 buchen**
    `<Einheit 6> <Einheit 7> <Einheit 8> <Einheit 9>`
11. **Gestelle auf Lkw 2 buchen**
    `<Gestell 12><Gestell 13>`
12. **Lkw 1 (ES) am Scanner anmelden.** Dadurch wird Lkw 2 automatisch abgemeldet.
    `<Lkw1>`
13. **Gestelle auf Lkw 1 buchen**
    `<Gestell 14> <Gestell 15>`
14. **Lkw 1 erneut anmelden.** Das letzte Gestell wird dadurch abgemeldet, die folgenden Einheiten können direkt auf den Lkw gebucht werden.
    `<Lkw1>`
15. **Einheiten direkt auf Lkw 1 buchen**
    `<Einheit 10> <Einheit 11>`
    Die Beladung wird fortgesetzt ...
16. **Die Beladung von Lkw 1 wird abgeschlossen.** Die Triggerzeit für Lkw 1 beginnt zu laufen.
    `<Ausgeliefert> <Lkw1>`
17. **Lkw 2 am Scanner anmelden.** Dadurch wird Lkw 1 automatisch abgemeldet.
    `<Lkw 2>`
18. **Gestelle auf Lkw 2 buchen**
    `<Gestell 9> <Gestell 10> <Gestell 11>`
19. **Die Beladung von Lkw 2 wird abgeschlossen.** Die Triggerzeit für Lkw 2 beginnt zu laufen.
    `<Ausgeliefert> <Lkw2>`

> **Hinweis**
> Achten Sie auf die Reihenfolge des Scannens, wenn Sie Einheiten und Gestelle/Kisten in einer beliebigen Reihenfolge laden wollen bzw. müssen!
> Beim Beladen eines Lkw werden Gestellen, Kisten und Einheiten der Erfassungsstelle Lkw zugeordnet. Dabei muss darauf geachtet werden, dass Einheiten die direkt auf den Lkw (Erfassungsstelle) gestellt werden, buchungstechnisch nicht auf ein zuvor geladenes Gestell/Kiste gebucht werden! Schließen Sie das Beladen eines Lkw immer mit der Statusbuchung `<Ausgeliefert> <Lkw>` ab.

### Gestelle bzw. Kisten scannen

**Voraussetzung:** Der Name des Mitarbeiters und die aktuelle Erfassungsstelle muss gescannt sein.

*   "So scannen Sie eine Einheit auf ein leeres Gestell (Gestell wird BDE-seitig geleert)"
*   "So scannen Sie ein Versandgestell fertig"
*   "So scannen Sie die Auslieferung Gestelle/Versandgestelle"
*   "So scannen Sie Gestelle auf den LKW"

**So scannen Sie eine Einheit auf ein leeres Gestell (Gestell wird BDE-seitig geleert)**
1.  Scannen Sie ein leeres Gestell: `<Beginn> <Gestell>`
    [Image: Barcode for 'begin' and a picture of an empty rack.]
2.  Scannen Sie das Etikett der Einheit:
    [Image: Barcode on a piece of glass.]
    `<Einheit 1>`
    `<Einheit 2>`
    `<Einheit 3>`
    `<Einheit 4>`
    ...

**So scannen Sie ein Versandgestell fertig**
`<Fertig> <Gestell 1> <Fertig> <Gestell 2> <Fertig> <Gestell ...>`

**So scannen Sie die Auslieferung Gestelle/Versandgestelle**
`<Ausgeliefert> <Gestell 1> <Ausgeliefert> <Gestell 2> <Ausgeliefert> <Gestell ...>`

**So scannen Sie Gestelle auf den LKW**
`<ErfStelle> <Gestell 1> <Gestell 2> <Gestell ...>`

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Gestelle" auf Seite H-98

### Status scannen

Das Scannen eines Statusbarcodes setzt im Hintergrund zahlreiche Aktivitäten der BDE in Gang, die für die gesamte Produktionssteuerung von entscheidender Bedeutung sind. Wird z. B. einem Lkw der Status `<Ausgeliefert>` zugewiesen, wird dieser Status auf die gesamte Ladung (Gestelle, Kisten, Einheiten usw.) übertragen, die Ladung wird auf die (System-) interne Erfassungsstelle 11 (Ausgeliefert) gebucht.

Der Statusbarcode beschreibt den Status eines Objektes z. B. einer Einheit (Bruch usw.), eines Gestells (leer, fertig, geliefert/<Beginn>, <Ausgeliefert>, <Bruch>, <Fertig>, usw.).

Der Status muss immer vor dem Objekt (Gestell, Einheit, usw.) gescannt werden. Müssen mehrere Objekte mit dem gleichen Status versehen werden, muss der Status für jedes Objekt gesondert gescannt werden (`<Status> <Objekt> <Status> <Objekt>`).

**Handlungsanweisungen:**
*   "So scannen Sie den Status Bruchmeldung Einheiten"
*   "So scannen Sie den Status Auslieferung Einheiten"
*   "So scannen Sie den Status Auslieferung mehrere Gestelle"
*   "So melden Sie ein leeres Gestell an (Gestell wird BDE-seitig geleert)"
*   "So melden Sie eine leere Erfassungsstelle an (Erfassungsstelle wird BDE-seitig geleert): Sonderfall Lkw"

**So scannen Sie den Status Bruchmeldung Einheiten**
`<Bruch> <Einheit 1> <Bruch> <Einheit 2> <Bruch> <Einheit ...>`

**So scannen Sie den Status Auslieferung Einheiten**
`<Ausgeliefert> <Einheit 1> <Ausgeliefert> <Einheit 2> <Ausgeliefert> <Einheit ...>`

**So scannen Sie den Status Auslieferung mehrere Gestelle**
`<Ausgeliefert> <Rack 1> <Ausgeliefert> <Rack 2> <Ausgeliefert> <Rack ...>`

**So scannen Sie den Status Auslieferung Lkw/Auflieger (abschließen der Beladung) und Start der Triggerzeit**
`<Ausgeliefert> <RegPoint>`

**So melden Sie ein leeres Gestell an (Gestell wird BDE-seitig geleert)**
`<Beginn> <Gestell>`

**So melden Sie eine leere Erfassungsstelle an (Erfassungsstelle wird BDE-seitig geleert): Sonderfall Lkw**
`<Beginn> <ErfStelle>`

> **Bei mehrfach einscannen von `<Status>`**
> Wurde mehrfach der Status hintereinander gescannt `<Status1><Status2><Status3><Objekt>`, wird der letzte gescannte Status auf das Objekt angewendet; im Beispiel `<Status3><Objekt>`. Die BDE-Engine überprüft Buchungen und verwirft nicht plausible Erfassungen, wie z. B. zwei Status-Buchungen hintereinander.

> **Achtung bei Status auf `<Beginn>` setzen**
> Der Status `<Beginn>` setzt das Objekt (Gestell/Lkw usw.) erfassungstechnisch zurück, d. h. auf leer! Befanden sich BDE-seitig noch Einheiten auf dem Objekt (z. B. dem Lkw oder einem Gestell), werden diese Einheiten automatisch auf die Erfassungsstelle Fehlergestelle gebucht.
> Schließen Sie das Beladen eines Lkw immer mit der Statusbuchung `<Ausgeliefert><Lkw>` ab.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Zustände" auf Seite H-104

### Korrigieren von Fehlbuchungen

Fehlbuchungen können grundsätzlich durch eine neue, korrekte Buchung korrigiert werden! Die zusätzliche Buchung wird in der Buchungshistory festgehalten, hat aber außer der Korrektur keine weiteren Auswirkungen.

**Beispiel:**
Wurden Einheiten irrtümlich auf ein Gestell und nicht auf die Erfassungsstelle gebucht, kann dieser Fehler durch Scannen der Erfassungsstelle und anschließendem Scannen der Einheit rückgängig gemacht werden (Wiederholung für jede falsch gescannte Einheit).
`<ErfStelle> <Einheit 1> <Einheit 2> <Einheit ...>`

---

## Production Terminals

Dieser Themenblock verschafft Ihnen einen groben Überblick zu den verschiedenen Production Terminals.
Dazu gehören folgende Lerneinheiten:
*   "Einführung" auf Seite H-65

**Lernziele**
*   Unterschiedliche Terminals kennenlernen.
*   Die Funktionsweise kennenlernen und verstehen.

**Nutzen**
Die Production Terminals helfen Ihnen, die Scheiben einer Einheit in der korrekten Reihenfolge vom Gestell der Produktion (z. B. Linie) zuzuführen. Um effizient arbeiten zu können, müssen Sie die Arbeitsweise der Terminals verstehen und mit täglich auftretenden Situationen entsprechend umgehen können.

**Definitionen**

| Terminal | Einsatzbereich |
| :--- | :--- |
| **Production Terminal IG** | Kommt an der ISO-Linie zum Einsatz. |
| **Production Terminal TG** | Kommt an der ESG-Linie zum Einsatz. |
| **Production Terminal LG** | Kommt an der VSG-Linie zum Einsatz. |
| **Production Terminal Order**| Kommt überall dort zum Einsatz, wo größere Mengen gebucht werden. |
| **Production Terminal Manual Cutting** | Visualisiert am Handzuschnitttisch den Arbeitsplan der zu schneidenden Scheiben. |
| **Production Terminal Processing** | Kommt an den Bearbeitungsmaschinen zum Einsatz. |
| **Production Terminal Edit** | Kommt im Versandbüro zum Einsatz. |

**Merke**
*   **Voraussetzung**: Voraussetzung zur Nutzung der Production Terminals ist ein installierter Barcode Manager (A+W Production).

### Einführung

Bei den Production Terminals handelt es sich um Leitrechner für unterschiedliche Arbeitsstationen. Damit ist es unter anderem möglich, auszuführende Arbeiten an Scheiben nach unterschiedlichen Kriterien dar zu stellen und zu planen, durchgeführte Arbeiten zu buchen, Bruch zu erfassen und automatisch Nachläufer zu erzeugen oder Produktionsstatistiken zu erstellen. Typische Einsatzorte für Production Terminals sind:
*   Zuschnitt
*   ISO-Linie
*   ESG-Ofen
*   VSG-Linie
*   Versand

Leitrechner visualisieren und steuern einzelne Prozessschritte und sind individuell konfigurierbar. Mit den A+W Leitrechnern können online Etiketten und Reports gedruckt und Bruchscheiben mit allen benötigten Informationen erfasst werden. Die Leitrechner zeichnen sich durch eine einfache und durchgängige Handhabung aus. Mit Hilfe dieser intelligenten Systeme sind Sie jederzeit in der Lage, Ihren Kunden gegenüber Auskunft über den momentanen Status der Produkte zu geben. Nachfolgend finden Sie die schematische Darstellung einer möglichen A+W Production-Landschaft:

[Image: A schematic overview of a production floor showing the flow of materials through various terminals such as Manual Cutting, TG-In, TG-Out, LG-In, LG-Out, IG-In, IG-Out, Bender, and IG-Assembly.]
*Abb. H-8 Überblick Production Terminals*

Da an jedem Arbeitsplatz in der Produktion andere Informationen erforderlich sind, gibt es für verschiedene Prozesse und Arbeitsabläufe entsprechend konfigurierte Standard-Schirme.

**Kurze Erläuterung zu den einzelnen Production Terminals:**

*   **Terminal Manual Cutting**: Visualisiert am Handzuschnitttisch den Arbeitsplan der zu schneidenden Scheiben.
*   **Terminal Order**: Kommt überall dort zum Einsatz, wo größere Mengen gebucht werden.
*   **Terminal Processing**: Ist die Variante des Leitrechners, die an Bearbeitungsmaschinen zum Einsatz kommt und diese automatisch ansteuert. Das Modul gibt Ihnen detaillierte Auskunft über die durchzuführenden Bearbeitungen inklusive maßstabsgetreuer Produktionszeichnungen.
*   **Terminal IG-In**: Visualisiert am Einlauf der Isolierglaslinie den Arbeitsplan der zu produzierenden Scheiben eines Laufes oder eines logischen Produktionsgestelles/ Fächerwagen in Produktionsreihenfolge.
*   **Terminal IG-Assembly**: Wird zwischen optischer Scheibenkontrolle nach der Waschmaschine und vor der Rahmensetzstation installiert und visualisiert die technischen Daten inklusive der Rahmendaten jeder zu fertigenden Einheit.
*   **Terminal IG-Out**: Visualisiert am Auslauf der Isolierglaslinie die technischen und versandorientierten Daten jeder gefertigten Einheit.
*   **Terminal TG-In**: Ist das Anzeigesystem am Ofeneinlauf. Es zeigt die Belegung des Ofenbettes und wird durch den Bediener gesteuert. Alle Scheiben werden per Scanner registriert und ihre Geometrie auf Vollständigkeit der Bearbeitung geprüft.
*   **Terminal TG-Out**: Dabei handelt es sich um das Anzeigesystem am Ofenauslauf. Es werden alle am Ofeneinlauf registrierte Scheiben, entsprechend des Durchlauftaktes angezeigt. Der Bediener erhält, wenn definiert, Hinweise zur weiteren Verwendung oder zu Versandabstellinformationen.
*   **Terminal Edit**: Ist die Variante des Leitrechners, der in der Regel im Versandbüro zum Einsatz kommt, um Einheiten, Scheiben oder Gruppen umzubuchen und Außer-Haus-Gestelle zu verwalten.
*   **Terminal LG-In**: Visualisiert am Einlauf der VSG-Linie den Arbeitsplan der zu produzierenden Scheiben eines Laufes oder eines logischen Produktionsgestelles/ Fächerwagen in Produktionsreihenfolge.
*   **Terminal LG-Assembly**: Visualisiert im Reinraum den Arbeitsplan sobald eine Scheibe oder Einheit am Terminal LG-In gebucht wurde. So ist genug Zeit zur Verfügung, um Folien zu schneiden.

> **Production Terminals**
> Detaillierte Informationen zu den einzelnen Terminals entnehmen Sie bitte dem Handbuch *Production Terminal*.

---

## Bruchmanagement

In diesem Themenblock lernen Sie den Umgang mit zu Bruch gegangenen Scheiben.
*   "Bruchbehandlung (intern)" auf Seite H-70

### Überblick

**Lernziele**
*   Den Umgang mit Brüchen kennenlernen.

**Nutzen**
Es sind keine manuellen Eingaben nötig. Dadurch werden die Bruchscheiben schneller nachgeschnitten. Es ist auch keine zusätzliche Kommunikation zwischen den Mitarbeitern nötig. Dadurch werden Fehler vermieden.

**Definitionen**
*   **Bruchpool**: Im globalen Bruchpool finden Sie eine Übersicht der Bruchscheiben.

**Merke**
*   **Bruchmeldung**: Die Bruchmeldung erfolgt an jedem Production Terminal oder per Scanner.
*   **Etiketten**: Der Etikettendruck erfolgt automatisch an einem zentralen Drucker.
*   **Automatischer Nachschnitt**: Der automatische Nachschnitt findet auf dem Restblatt oder durch eine Tischoptimierung im A+W Realtimeoptimizer statt.

### Bruchbehandlung (intern)

Werden Einheiten als Bruch gemeldet, werden dadurch verschiedene interne Aktionen ausgelöst. In der Datenbank werden bei einer Bruchmeldung alle Informationen über die Ursprungs-Einheit sowie alle Nachläufer und ggf. dessen Nachläufer gespeichert.

Nachläufer erhalten immer die Ursprungs-Barcode-Nummer. Die Barcodenummer der Ursprungsscheibe wird bei einer Bruchmeldung mit einem Index versehen.

In der Tabelle werden die Änderungen dargestellt, die sich durch Bruchmeldungen auf die einzelnen Flags und die Barcode-Nummer ergeben.

**BDE-Bruchbehandlung**

| Barcode | Erfassungsstelle | Gestell | Bruch | Nachläufer-index | Erklärung |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 012345678 | Bohren | 15 | 0 | 0 | E1 |
| 012345678 001 | Bohren | 15 | 1 | 0 | E2 |
| **Bruch 1** | | | | | |
| 012345678 | - | - | 0 | 1 | E3 |
| 012345678 002 | Ofen | 20 | 1 | 1 | E4 |
| **Bruch 2** | | | | | |
| 012345678 | - | - | 0 | 2 | E5 |

*Tab. H-1 BDE-Bruchbehandlung*

**Erläuterung der Tabelle**

*   **E1**: Die Scheibe mit dem Barcode 012345678 befindet sich an der Erfassungsstelle Bohren auf dem Gestell 15. Die Scheibe ist nicht bruchgemeldet; das Bruch-Flag ist Null. Es handelt sich um die Ursprungsscheibe, da der Nachläuferindex den Wert Null hat.
*   **E2**: Die Scheibe mit dem Barcode 012345678 wird an der Erfassungsstelle Bohren als Bruch gemeldet. Das Bruch-Flag wird gesetzt. An die Barcode-Nummer wird ein dreistelliger Index angehängt. Der Index 001 belegt, dass es sich um den ersten Bruch handelt.
*   **E3**: Der Nachläufer wird erzeugt und erhält die Ursprungs-Barcode-Nummer 012345678. Außerdem wird der Nachläuferindex um eins erhöht (1). Der Nachläuferindex unterscheidet den Nachläufer von der Ursprungsscheibe. Da die Einheit noch nicht erfasst wurde, ist noch keine Erfassungsstelle zugeordnet.
*   **E4**: Der Nachläufer hat seinen Weg durch die Produktion bis zum Ofen geschafft und wird dort als Bruch gemeldet. Das Bruch-Flag wird gesetzt. An die Barcode-Nummer wird ein dreistelliger Index angehängt. Der Index 002 belegt, dass es sich hier um den zweiten Bruch handelt.
*   **E5**: Der zweite Nachläufer wird erzeugt und erhält die Ursprungs-Barcode-Nummer 012345678. Außerdem wird der Nachläuferindex um eins erhöht (2). Der Nachläuferindex unterscheidet den Nachläufer von der Ursprungsscheibe. Da die Einheit noch nicht erfasst wurde, ist noch keine Erfassungsstelle zugeordnet.

> **Hinweis**
> Beim Druck der Etiketten für die Nachläufer bzw. beim Reporting können die oben beschriebenen Werte und Flags ausgewertet und berücksichtigt werden. Dies wird in der Regel in der Projektierungsphase festgelegt und kann selbstverständlich an die aktuellen Bedürfnisse angepasst werden. Setzen Sie sich bitte mit der A+W Software GmbH in Verbindung und lassen Sie sich über die Möglichkeiten beraten.

> **Tipp**
> Bei den Ansichten in A+W Production können Filter verwendet werden. Im Bereich der Barcode Manager-Ansichten sind Standardfilter gesetzt, die ggf. Einheiten mit Nachläuferindex nicht anzeigen. Zum Anzeigen dieser Einheiten deaktivieren Sie alle Filter (unfiltered). Der Standartfilter heißt Aktiv!

> **Ansichten und Filter**
> Weitere Informationen zu Ansichten und Filtern entnehmen Sie bitte dem A+W Production-Handbuch.

---

## Statistik, Reporting und Monitoring

In diesem Themenblock lernen Sie die Berichte und die unterschiedlichen Auswertungen kennen.
Dazu gehören folgende Lerneinheiten:
*   "BDE-Reporting" auf Seite H-74
*   "Monitoring: A+W Dashboard" auf Seite H-79
*   "Statistik: A+W Discovery" auf Seite H-83

### Überblick

**Lernziele**
*   Standard-Reports der BDE kennenlernen.

**Nutzen**
*   Mit hilfe der Standard-Reports erhalten Sie jederzeit einen Überblick zu dem Stand Ihrer Produktion. Das spart Zeit und Wege und Sie sind jederzeit Ihrem Kunden gegenüber aussagefähig.

**Definition**
*   **Reports**: Sind flexible Werkzeuge zur Kontrolle und Auswertung der Produktion.

**Merke**
*   **Standard-Reports**: Sind Bestandteil der A+W Production.
*   **Individuelle Reports**: Können auf Kundenwunsch jederzeit erstellt werden.

### BDE-Reporting

Bei den hier beschriebenen Reports handelt es sich um die Standard-Barcode-Reports. Kundenindividuelle Anpassung der Reports sowie neue Reports sind möglich. Die Reports stellen ein sehr flexibles und mächtiges Werkzeug zur Kontrolle und Auswertung der Produktion dar.

Setzen Sie sich bitte mit der A+W Software GmbH in Verbindung, wir beraten Sie gerne und führen die notwendigen Änderungen, Erweiterungen und Anpassungen durch oder erstellen für Sie neue, individuelle Reports.

> **Hinweis**
> Allgemeingültige Reports, die Auswertungen auf eine Erfassungsstelle darstellen, zeigen in der Regel alle Einheiten an, die dieser Erfassungsstelle zugeordnet waren! Wird z. B. ein zum Teil beladenes Gestell am Ausgang der ISO-Linie (Erfassungsstelle 1612) angemeldet, um ISO-Einheiten aufzunehmen, werden die bereits auf dem Gestell vorhanden Einheiten ebenfalls auf die Erfassungsstelle 1612 gebucht! Sollen Auswertungen durchgeführt werden, die ausschließlich z. B. den Durchsatz der ISO-Linie darstellen, müssen angepasste Reports zur Anwendung kommen.

#### Aufruf der Reports

Alle Reports können über die A+W Production-Menü-Struktur aufgerufen werden. Außerdem werden in verschiedenen Production Terminals funktionsabhängig Reports zur Verfügung gestellt. Sie können auch Verknüpfungen zu den Reports auf dem Desktop des PCs ablegen.

> **Hinweis**
> Die A+W Production-Menüstruktur wird dynamisch aufgebaut. Die Menüeinträge für den Barcode Manager sind nur sichtbar, wenn eine Barcode Manager-Ansicht geöffnet ist.

#### Beispiele der Standard-Barcode-Reports

Abhängig vom Report können nach dem Aufruf verschiedene Parameter für den Report eingegeben bzw. gewählt werden. Dies kann der Anzeigezeitraum sein, die Erfassungsstelle für die die Auswertung erfolgen soll usw.

> **Hinweis**
> Die Darstellung der Reports erfolgt ausschnittsweise und soll einen Überblick der A+W Production-Reports geben.

**Abstellliste**
*Listen > Abstellliste*
Die Abstellliste zeigt alle Teile an, die in einer einheitengenauen A+W Production-Ansicht ausgewählt werden. Je nach Filter in der A+W Production-Ansicht, werden auch Rahmen etc. angezeigt.
[Image: Screenshot of the "Abstell-Liste" report, showing columns for Pos, Etikett, Breite, Höhe, Bezeichnung, Erfassungsstelle, Gestell, Status, Person, and Buchungszeit.]
*Abb. H-9 Abstellliste*

**Auftragsübersicht**
*Listen > Auftragsliste*
Die Auftragsübersicht zeigt an, wo sich die einzelnen Positionen (Kopfteile) des Auftrags befinden.
[Image: Screenshot of the "Auftragsübersicht" report, showing details per position for a specific order, including Etikett, Erf-Stelle, Gestell, Status, Buchungszeit, Gewicht, and Fläche.]
*Abb. H-10 Auftragsübersicht*

**Auftragsstatus**
*Listen > Auftragsstatus*
Die Liste gibt Ihnen Auskunft über den Status des Auftrags.
[Image: Screenshot of the "Status für Auftrag" report. It shows the status of different production steps (Soll, Ist, Termin, Erfassungsstelle) for each position of an order.]
*Abb. H-11 Auftragsstatus*

**Ladeliste**
*Listen > Ladeliste*
Die Ladeliste zeigt Ihnen die tatsächlichen Beladung. Über Filter haben Sie die Möglichkeit, die Inhalte zu begrenzen.
[Image: Screenshot of the "Ladeliste" report, organized by customer and delivery address, showing which items (Etikett, Bezeichnung) are on which rack (Gestell).]
*Abb. H-12 Ladeliste*

**Gestellbelegung pro Scheibe**
*Listen > Gestellbelegung pro Scheibe*
Diese Liste zeigt Ihnen für die eingegebene Gestellnummer die Belegung pro Scheibe.
[Image: Screenshot of the "Gestellbelegung" report for a specific rack (Gestell 1000), listing each item on the rack with its details (Auftrag, Pos, Breite, Höhe, Etikett, Bezeichnung, Buchungszeit).]
*Abb. H-13 Gestellbelegung pro Scheibe*

**Gestellbelegung pro Position**
*Listen > Gestellbelegung pro Position*
Diese Liste zeigt Ihnen für die eingegebene Gestellnummer die Belegung pro Position.
[Image: Screenshot of the "Gestellbelegung" report showing a summary per position for a specific rack (Gestell 1000).]
*Abb. H-14 Gestellbelegung pro Position*

**Buchungshistorie**
*Listen > Buchungshistorie*
Diese Liste zeigt Ihnen pro Auftrag, welche Buchungen an welcher Stelle stattgefunden haben.
[Image: Screenshot of the "Historie" report, detailing every booking event for a specific label, including timestamp, location, rack, status, and processing step.]
*Abb. H-15 Buchungshistorie*

### Monitoring: A+W Dashboard

**Lernziele**
*   Kurze Einführung in A+W Dashboard.
*   Die Möglichkeiten kennenlernen.

**Nutzen**
A+W Dashboard zeigt wichtige Kennzahlen von den entscheidenden Stellen der Produktion an und sorgt damit für hohe Transparenz.

**Definitionen**
*   **Ampel**: Die Ampel zeigt den aktuellen Status einer Erfassungsstelle an. Die Bedeutung der Farbe können Sie selbst festlegen.

**Merke**
*   **Zeitraum**: Zur Auswertung werden die Datenbanktabellen mit den A+W Production-Buchungen herangezogen. Dabei wird in der Regel ein Zeitraum von max. 24 Stunden berücksichtigt.
*   **Korrekte Darstellung**: Voraussetzung für aussagekräftige Anzeigen sind lückenlos A+W Production-Buchungen.
*   **Anzeige**: A+W Dashboard kann sowohl auf großen Monitoren in den verschiedenen Abteilungen der Fertigung eingesetzt werden als auch auf mobilen Endgeräten wie Smartphones.
*   **Störungen**: Bei Störungen können Sie die Situation exakt kommunizieren und in vielen Fällen bereits eigene Lösungsansätze vorschlagen.

#### Überblick

A+W Dashboard zeigt wichtige Kennzahlen von den entscheidenden Stellen der Produktion an und sorgt damit für hohe Transparenz.

In Echtzeit erhalten Sie Auskunft über einzelne Produktionsbereiche wie Zuschnitt, ISO-Linien, Bearbeitungen, ESG-Fertigung: Sie sehen z. B. den aktuellen Nutzungsgrad, den Status jeder Maschine, den Verlauf der Produktivität.

Das Programm kann sowohl auf großen Monitoren in den verschiedenen Abteilungen der Fertigung eingesetzt werden als auch auf mobilen Endgeräten wie Smartphones, Tablet-Computern oder PDAs. Voraussetzung ist ein Internet-Browser und ein Zugang zum Programm (Adresse, Benutzer-Account).

Damit dient die Anzeige als Online-Monitoring-Tool und Entscheidungsmittel, wenn sich im Laufe einer Schicht Maschinenzustände ändern oder die zu fertigenden Stückzahlen nicht eingehalten werden können.

Bei Störungen können die Mitarbeiter die Situation exakt kommunizieren und in vielen Fällen bereits eigene Lösungsansätze vorschlagen.

A+W Production enthält vordefinierte Anzeigen, kann aber auch individuell auf die jeweilige Maschine oder Abteilung angepasst werden. Damit können Sie die kritischen Stellen Ihrer Produktion im Auge behalten und notfalls sofort eingreifen.

Zur Auswertung werden die Datenbanktabellen mit den BDE-Buchungen herangezogen. Dabei wird in der Regel ein Zeitraum von max. 24 Stunden berücksichtigt. Damit grenzt sich A+W Dashboard von A+W Discovery ab, das statistische Auswertungen über längere Zeiträume ermöglicht.

Die Auswertungen werden auf verschiedene Arten visualisiert. Sie können in die Anzeigen hinein- und herauszoomen und mit Wischen die Seiten wechseln.

[Image: Five examples of visualization types: A) traffic light (Ampel), B) pie chart (Kreis), C) line graph (Punktediagramm), D) bar chart (Balkendiagramm), E) speedometer/tacho.]
*Abb. 9 Arten der Visualisierung (Beispiele)*

Jede dieser Darstellungsarten können Sie so einrichten, wie es den Erfordernissen des betrachteten Produktionsbereichs und der Überwachung entspricht.

*   **Ampel (A)**: Die Ampel zeigt den aktuellen Status einer Erfassungsstelle an. Die Bedeutung der Farben können Sie selbst festlegen. Diese Anzeige ist für Statusanzeigen über sehr kurze Zeiträume sinnvoll, z. B. um darzustellen, ob eine Maschine in Betrieb oder ausgefallen ist.
*   **Kreisdiagramm (B)**: Das Kreisdiagramm zeigt die Anteile der gemeldeten Maschinenstatus über einen selbst definierten Zeitraum an. Standardmäßig sind das die letzten 24 Stunden. Damit wird die Summe der Ausfallzeiten über alle Schichten im Zeitraum sichtbar. Diese Anzeige ist geeignet, den Betrieb ähnlicher Maschinen miteinander zu vergleichen.
*   **Punktediagramm (C)**: Die Linie zeigt die Buchungen eines vergangenen Zeitraums verteilt auf einen Anzeigezeitraum an, z. B. die Buchungen der letzten Stunde verteilt auf den Anzeigezeitraum. Ein Punkt zeigt die Summe pro Gruppierung, z. B. pro Minute, pro Stunde, pro Tag. Die Ziel-Stückzahl und der Durchschnitt können durch durchgehende waagerechte Linien angezeigt werden.
*   **Balkendiagramm (D)**: Das Balkendiagramm stellt statistische Daten dar, die über SQL-Abfragen erhoben wurden. Für eine Konfiguration der Ansicht müssen diese Statistiken vorhanden sein.
*   **Tacho (E)**: Der Tacho zeigt die aktuelle Auslastung an. Dazu wird die Anzahl der gebuchten Stückzahlen der letzten Stunde betrachtet. Die rot-gelb-grün-Markierung zeigt an, wie die Stückzahlen bewertet sind.

> **Korrekte Darstellung nur mit korrekten BDE-Buchungen**
> Voraussetzung für aussagekräftige Anzeigen sind lückenlose BDE-Buchungen.

> **A+W Dashboard**
> A+W Dashboard verbindet die Produktions-Software A+W Production und das A+W Production Terminal. Die BDE-Daten werden über den PPS-Webservice ausgelesen. Detaillierte Informationen zu diesem Modul entnehmen Sie bitte dem Handbuch *A+W Dashboard*.

### Statistik: A+W Discovery

**Lernziele**
*   Kurze Einführung in A+W Discovery.
*   Die Möglichkeiten kennenlernen.

**Nutzen**
Mit A+W Discovery werden unternehmensübergreifende Daten zusammengeführt, aufbereitet und anschließend angezeigt. Management und Controlling können diese Informationen analysieren und für unternehmensübergreifende Entscheidungen verwenden.

**Definitionen**
*   **Pivot Tabelle**: Ist eine spezielle Art von Tabellen, die die Möglichkeit bieten, Daten auf verschiedene Arten darzustellen.
*   **Fiskaljahr**: Geschäftsjahr, in dem ein Unternehmen das Ergebnis seiner Tätigkeit in einem Jahresabschluss zusammenfasst.

**Merke**
*   **A+W Discovery**: Bietet die Möglichkeit, langfristige Auswertungen von Produktionsdaten zu erstellen.
*   **Auswertungen**: Auswertungen können leicht über Microsoft Excel in Form von Pivot-Tabellen erstellt werden.
*   **Datenbereitstellung**: A+W Discovery kann Daten aus den ERP-Systemen (A+W Enterprise, A+W Business) und dem PPS-System (A+W Production) bereitstellen.
*   **Mandantenübergreifende Auswertungen**: Es können Mandantenübergreifende Auswertungen erstellt werden.

#### Überblick

Steigende Anforderungen an moderne ERP- und PPS-Systeme erfordern immer leistungsfähigere Controlling- und Steuerungsmechanismen. Dies ist zum einen bedingt durch steuerliche und rechtliche Rahmenbedingungen, zum anderen aber auch durch die Notwendigkeit das Produktportfolio, die Produktivität und Auslastung stets aus verschiedenen Betrachtungsweisen heraus auswerten und neu ausrichten zu können.

A+W Discovery ist das moderne Business Intelligence System der A+W Software GmbH, welches abgestimmt und ausgerichtet ist auf die speziellen Anforderungen eines modernen Glasherstellers oder Glasveredlers. Der Aufbau und die Integration mit dem PPS-System A+W Production erlaubt Ihnen die jeweiligen statistischen Kennzahlen und Messgrößen aus verschiedenen Blickrichtungen zu betrachten, zu verrechnen und daraus die notwendigen strategischen, kaufmännischen oder produktionstechnischen Entscheidungen und Maßnahmen abzuleiten.

So können Sie beispielsweise Daten erheben, welche Ihnen den Deckungsbeitrag und das Umsatzvolumen bestimmter Standorte oder Niederlassungen in einem definierten Zeitrahmen (bspw. Monat oder Jahr) anzeigen. Dadurch können Sie ggf. Ihre Kostenstrukturen anpassen und Ihre Mitarbeiter und Vertriebspartner zur Umsatzsteigerung im Folgejahr motivieren. Mit der Version 5.4 wurde darüber hinaus das Fiskaljahr und das Fiskalquartal implementiert.

Auch ist es möglich, produktive Kennzahlen wie Anzahl Bruchscheiben je Arbeitsstation oder Maschinenstillstandszeiten über einen definierten Zeitraum auszuwerten.

[Image: Screenshot of an A+W Discovery dashboard in Excel, showing various pivot tables and charts, such as a pie chart for reject reasons, bar charts for produced quantities, and a line graph for deviations.]
*Abb. 10 A+W Discovery*

Darüber hinaus gibt Ihnen A+W Discovery die Möglichkeit, mittels vordefinierter A+W Standard-Reports sinnvolle PPS-Daten miteinander in Beziehung zu setzen und zu aggregieren. So haben Sie stets die volle Kontrolle über alle kaufmännischen und produktionsrelevanten Daten – Produkte, Ressourcen, Kosten, Zeiten und Kapazitäten.

> **A+W Discovery**
> Detaillierte Informationen zu diesem Modul entnehmen Sie bitte dem Handbuch *A+W Discovery*.

---

## Softwarereferenz

### Übersicht

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   Stammdaten

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass Funktionen und Dialoge auf verschiedenen Wegen geöffnet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.

### Stammdaten

*Menü Stammdaten > BDE öffnen*

Im Menü BDE befinden sich folgende Programmpunkte:

*   **Barcode-Optionen**: Dieser Bereich wird durch die A+W Software GmbH gepflegt.
*   **Barcode-Typen**: Dieser Bereich wird durch die A+W Software GmbH gepflegt.
*   **Erfassungsstellen-Typen**: Dieser Bereich wird durch die A+W Software GmbH gepflegt.
*   **Erfassungsstellen**: In diesem Bereich verwalten Sie Ihre Erfassungsstellen.
    *   ⇨ "Erfassungsstellen" auf Seite H-94
*   **Gestelle**: In diesem Bereich verwalten Sie Ihre Gestelle.
    *   ⇨ "Gestelle" auf Seite H-98
*   **Gestellfilter**: In diesem Bereich definieren Sie Gestellfilter.
    *   ⇨ "Gestellfilter" auf Seite H-102
*   **Zustandstypen**: Dieser Bereich wird durch die A+W Software GmbH gepflegt.
*   **Zustände**: In diesem Bereich verwalten Sie die Zustände.
    *   ⇨ "Zustände" auf Seite H-104
*   **Personal**: In diesem Bereich verwalten Sie Ihr Personal.
    *   ⇨ "Mitarbeiter" auf Seite H-106
*   **Spaltenzuordnung**: Dieser Bereich wird durch die A+W Software GmbH gepflegt.
*   **Spalten**: Dieser Bereich wird durch die A+W Software GmbH gepflegt.
*   **BDE Nachbearbeitung**: In diesem Bereich befindet sich die Nachbearbeitung, falls bei der Verarbeitung der Daten Probleme aufgetreten sind.
    *   ⇨ "Nachbearbeitung" auf Seite H-110

### Barcode-Optionen

*Stammdaten > BDE > Barcode-Optionen*

[Image: Screenshot of the "Barcode-Optionen" dialog with settings for quantity handling, group handling, label mode, and file paths.]
*Abb. H-1 Barcode-Optionen*

Dieser Bereich beschäftigt sich mit den Barcode-Optionen.

> **Systemkritische Daten**
> Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor. Die Daten in diesem Dialog sind systemkritisch.

### Barcode-Typen

*Stammdaten > BDE > Barcode-Typen*

[Image: Screenshot of the "Barcodetypen" dialog listing various types like EINHEIT, GRUPPE, GESTELL, ERF.-STELLE with their properties.]
*Abb. H-2 Barcode-Typen*

Dieser Bereich bestimmt das Verhalten von Barcodes.

> **Systemkritische Daten**
> Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor. Die Daten in diesem Dialog sind systemkritisch.

### Erfassungsstellen-Typen

*Stammdaten > BDE > Erfassungsstellen-Typen*

[Image: Screenshot of the "Erfassungsstellentypen" dialog with a list of types and settings for their behavior upon booking.]
*Abb. H-3 Erfassungsstellen-Typen*

Dieser Bereich bestimmt das Verhalten von Erfassungsstellen.

> **Systemkritische Daten**
> Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor. Die Daten in diesem Dialog sind systemkritisch.

### Erfassungsstellen

*Stammdaten > BDE > Erfassungsstellen*

[Image: Screenshot of the "Erfassungsstellen" dialog showing a list of defined stations and detailed settings for the selected station.]
*Abb. H-4 Erfassungsstellen*

In diesem Dialog legen Sie neue Erfassungsstellen an oder nehmen Änderungen an bestehenden Erfassungsstellen vor.
*Technische Info: Datenbanktabelle: AWBAR_STELLEN*

**Liste der Zustände**
*   **ID**: Die eindeutige Nummer, die der Erfassungsstelle zugewiesen wurde.
*   **Name**: Der Name, der der Erfassungsstelle zugewiesen wurde.
*   **Beschreibung**: Die Beschreibung, die Sie der Erfassungsstelle gegeben haben.
*   **Typ**: Der Typ, den Sie der Erfassungsstelle zugewiesen haben.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

**Erläuterung der Felder**

*   **Erfassungsstellennr**: In diesem Feld geben Sie die Nummer der Erfassungsstelle ein.
    *   *Technische Info: Datenbankfeld: Esnr*
*   **Barcode**: In diesem Feld geben Sie den Barcode der Erfassungsstelle ein.
    *   *Technische Info: Datenbankfeld: Esbc*
*   **Name**: In diesem Feld geben Sie den Namen der Erfassungsstelle ein.
    *   *Technische Info: Datenbankfeld: Esname*
*   **Beschreibung**: In diesem Feld geben Sie eine ausführliche Beschreibung für die Erfassungsstelle ein.
    *   *Technische Info: Datenbankfeld: Allgbez*
*   **Text für Produktionslisten**: In diesem Feld geben Sie den Text ein, der auf den Produktionslisten erscheinen soll.
    *   *Technische Info: Datenbankfeld: Lst1bez*
*   **Text für Kundenlisten**: In diesem Feld geben Sie den Text ein, der auf den Kundenlisten erscheinen soll.
    *   *Technische Info: Datenbankfeld: Lst2bez*
*   **Unterzeile für Barcodeetiketten**: In diesem Feld geben Sie ein, was unterhalb des Barcodes erscheinen soll.
    *   *Technische Info: Datenbankfeld: Barcbez*
*   **Erfassungsstellentyp**: Die Kombobox enthält alle in Ihrem Hause angelegten Erfassungsstellentypen. Wählen Sie den entsprechenden Typ aus.
    *   *Technische Info: Datenbankfeld: Typ*
*   **Gruppierung**: In diesem Feld haben Sie die Möglichkeit, Erfassungsstellen unabhängig von den Erfassungsstellentypen für Auswertungen zusammenzufassen, z. B. alle Öfen in eine Gruppe.
    *   *Technische Info: Datenbankfeld: Gruppe*
*   **Gruppierung für Arbeitsschichten**: In diesem Feld haben Sie die Möglichkeit, Erfassungsstellen zur Bildung von Arbeitsschichten zu gruppieren.
    *   *Technische Info: Datenbankfeld: Shift_Group*
*   **Aktueller Zustand**: In diesem Feld weißen Sie der Erfassungsstelle einen aktuellen Zustand zu.
    *   *Technische Info: Datenbankfeld: Zustandnr*
*   **Restriktionen**: Dieser Wert aktiviert und deaktiviert die Restriktionsprüfung und legt fest, auf welche Menge sich die Restriktionsprüfung bezieht.
    *   **0**: Restriktionsprüfung ist ausgeschaltet.
    *   **1**: Die Restriktionsprüfung bezieht sich auf die technische Produktionsmenge.
    *   **2**: Die Restriktionsprüfung bezieht sich auf die verfügbare Menge (Scheiben, die den direkt vorgelagerten Prozess abgeschlossen haben).
    *   **3**: Die Restriktionsprüfung bezieht sich auf die verfügbare Menge (Scheiben, die alle vorgelagerten Prozesse abgeschlossen haben).
    *   *Technische Info: Datenbankfeld: Restriction*
*   **Mengenüberschreitung**: In diesem Feld geben Sie die Mengenüberschreitung in Prozent ein. Dieser Wert wird nur ausgewertet, wenn die Restriktionsprüfung eingeschaltet ist.
    *   *Technische Info: Datenbankfeld: Overbook*
*   **Produzierte Teile anzeigen**: Diese Checkbox steuert, ob produzierte Teile angezeigt werden oder nicht.
    *   *Technische Info: Datenbankfeld: Show_produced_parts*
*   **Betriebsmittel der Auftragserfassung**: In diesem Feld wird Ihnen das Betriebsmittel der Auftragserfassung angezeigt. Dieses Feld wird an die Auftragserfassung zurück gemeldet.
    *   *Technische Info: Datenbankfeld: Maschinennr*

**Erläuterung der Felder im Bereich Rückmeldung von Buchungen**

*   **Bearbeitungsrückmeldung**: Diese Checkbox steuert, ob Rückmeldungen bezüglich der Bearbeitungen erfolgen oder nicht.
*   **Gestellrückmeldung**: Diese Checkbox steuert, ob Rückmeldungen bezüglich der Gestellbelegung erfolgen oder nicht.
*   **Gestellbelegung an Gestellserver melden**: Diese Checkbox steuert, ob die Gestellbelegung an den Gestellserver gemeldet werden soll oder nicht.
*   **Einheitenrückmeldung (STSU*.asc)**: Über diese Checkbox ist es möglich, im A+W Business eine Zuordnung der A+W Production-Etiketten zur A+W Business-Auftragspositionen vorzunehmen.
*   **Produktionsrückmeldung**: Diese Checkbox dient dazu, den aktuellen Auftragsstatus im A+W Business zu aktualisieren.

**Ergänzende Informationen**
*   ⇨ Tutorial, "Erfassungsstellen" auf Seite H-19
*   ⇨ Tutorial, "Fehlergestell (Error-Rack)" auf Seite H-20
*   ⇨ Tutorial, "Erfassungsstelle Lkw" auf Seite H-25
*   ⇨ "Zustände" auf Seite H-104
*   ⇨ "Erfassungsstellen-Typen" auf Seite H-93

### Gestelle

*Stammdaten > BDE > Gestelle*

[Image: Screenshot of the "Gestelle" dialog, showing a list of racks and detailed properties including type, customer data, and current location/status.]
*Abb. H-5 Gestelle*

In diesem Dialog legen Sie neue Gestelle an oder nehmen Änderungen an bestehenden Gestellen vor.
*Technische Info: Datenbanktabelle: AWBAR_GESTELLE*

**Liste der Gestelle**
*   **Name**: Der Name, der dem Gestell zugewiesen wurde.
*   **Gestell**: Der Barcode, der dem Gestell zugewiesen wurde.
*   **Typ**: Die Gestellart, die Sie dem Gestell zugewiesen haben.
*   **Anzahl**

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

**Erläuterung der Felder**

*   **Mehrere Gestelle anlegen**: Aktivieren Sie diese Checkbox, wenn Sie mehrere Gestelle auf einmal anlegen möchten. Nachdem Sie die Checkbox aktiviert haben, erscheinen darunter die Felder *Präfix*, *Startwert*, *Endwert* und *BC-Startwert*.
*   **Präfix**: Aktivieren Sie diese Checkbox, wenn Sie mehrere Gestelle auf einmal anlegen möchten.
*   **Startwert**: Aktivieren Sie diese Checkbox, wenn Sie mehrere Gestelle auf einmal anlegen möchten.
*   **Endwert**: Aktivieren Sie diese Checkbox, wenn Sie mehrere Gestelle auf einmal anlegen möchten.
*   **BC-Startwert**: Aktivieren Sie diese Checkbox, wenn Sie mehrere Gestelle auf einmal anlegen möchten.

**Erläuterung der Felder im Bereich Eigenschaften**

*   **Gestellart**: In dieser Kombobox können Sie die entsprechende Gestellart auswählen (00 Normal, 01 Fachgestell, 02 Kiste).
    *   *Technische Info: Datenbankfeld: Typ_KZ*
*   **Gestelltyp**: In dieser Kombobox können Sie den entsprechenden Gestelltyp auswählen (0001 Ofenbettl, 0002 A-Gestell, 0003 Fächerwagen, 0004 AutoClav Gestell).
    *   *Technische Info: Datenbankfeld: Typ_KZ*
*   **Fachnummer von ... bis**: Dieses Feld kommt bei Fachgestellen zum Einsatz und zeigt im ersten Feld die Nummer des 1. Faches. Im zweiten Feld sehen Sie die Nummer des letzten belegten Faches in dem Gestell.
    *   *Technische Info: Datenbankfeld: Erstfachnr / Lbelfach*
*   **Basis ES**: In dieser Kombobox können Sie die entsprechende Basiserfassungsstelle auswählen.
    *   *Technische Info: Datenbankfeld: Basisesnr*
*   **Temporäres Gestell**: Über diese Checkbox steuern Sie, ob es sich bei dem Gestell um ein temporäres Gestell handelt oder nicht.
    *   *Technische Info: Datenbankfeld: Tempkz*

**Erläuterung der Felder im Bereich Laufdaten**

*   **Aktuelle ES**: In diesem Feld sehen Sie, auf welcher Erfassungsstelle sich das Gestell gerade befindet.
    *   *Technische Info: Datenbankfeld: Esnr*
*   **Letzte ES**: In diesem Feld sehen Sie, auf welcher Erfassungsstelle das Gestell davor war.
    *   *Technische Info: Datenbankfeld: Esnralt*
*   **Aktueller Zustand**: In diesem Feld wird Ihnen der aktuelle Zustand des Gestells angezeigt (z. B. ausgeliefert, leer, etc.).
    *   *Technische Info: Datenbankfeld: Zustandnr*
*   **Letzter Zustand**: In diesem Feld wird Ihnen der Zustand davor angezeigt.
    *   *Technische Info: Datenbankfeld: Zustandnralt*

**Erläuterung der Felder im Bereich Kundendaten**

*   **Kundennummer**: In dieses Feld tragen Sie (falls bekannt) die Nummer des Kunden ein, dem das Gestell bei "außer Haus"-Meldung zugeordnet wurde.
    *   *Technische Info: Datenbankfeld: Kundennr*
*   **Kundenname**: Hier tragen Sie den Namen des Kunden für "außer Haus"-Gestelle ein.
    *   *Technische Info: Datenbankfeld: Kundenname*
*   **Lieferort**: Hier tragen Sie den Lieferort für "außer-Haus"-Gestelle ein.
    *   *Technische Info: Datenbankfeld: Lieferort*
*   **Tournummer**: Hier tragen Sie die Tournummer für "außer-Haus"-Gestelle ein.
    *   *Technische Info: Datenbankfeld: Tournr*

**Ergänzende Informationen**
*   ⇨ Tutorial, "Gestelle" auf Seite H-27

### Gestellfilter

*Stammdaten > BDE > Gestellfilter*

[Image: Screenshot of the "Gestellfilter" dialog, allowing to filter racks by station type, station, name, rack type, and rack sub-type.]
*Abb. H-6 Gestellfilter*

In diesem Dialog können Sie Filter selber erstellen, um die Anzahl der angezeigten Gestelle zu beschränken. Das ist dann sinnvoll, wenn Sie über eine große Anzahl an Gestellen verfügen.

**Erläuterung der Felder**

*   **Erfassungsstellentyp**: Die Kombobox enthält alle in Ihrem Hause angelegten Erfassungsstellentypen. Wählen Sie den gewünschten Typ aus, nach dem gefiltert werden soll.
*   **Erfassungsstelle**: Die Kombobox enthält alle in Ihrem Hause angelegten Erfassungsstellen. Wählen Sie die gewünschte Erfassungsstelle aus, nach der gefiltert werden soll.
*   **Gestellname von bis**: Hier können Sie einen Bereich eingeben, nach dem gefiltert werden soll.
*   **Gestellart**: Die Kombobox enthält alle angelegten Gestellarten. Wählen Sie die gewünschte Gestellart aus, nach der gefiltert werden soll.
*   **Gestelltyp**: Die Kombobox enthält alle angelegten Gestelltypen. Wählen Sie den gewünschten Gestelltyp aus, nach dem gefiltert werden soll.
*   **Betriebseigene Gestelle**: Aktivieren Sie die Checkbox, wenn Sie nur nach betriebseigenen Gestellen filtern möchten.

**Ergänzende Informationen**
*   ⇨ Tutorial, "Gestelle filtern" auf Seite H-27

### Zustandstypen

*Stammdaten > BDE > Zustandstypen*

[Image: Screenshot of the "Zustandstypen" dialog, showing a list of status types and their detailed configuration options.]
*Abb. H-7 Zustandstypen*

Dieser Bereich bestimmt das Verhalten eines Zustandes.

> **Systemkritische Daten**
> Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor. Die Daten in diesem Dialog sind systemkritisch.

### Zustände

*Stammdaten > BDE > Zustände*

[Image: Screenshot of the "Zustände" dialog with a list of statuses and their detailed properties, including name, description, barcode, and type.]
*Abb. H-8 Zustände*

In diesem Dialog legen Sie neue Zustände an oder nehmen Änderungen an bestehenden Zuständen vor.
*Technische Info: Datenbanktabelle: AWBAR_ZUSTAND*

**Liste der Zustände**
*   **ID**: Die eindeutige Nummer, die dem Zustand zugewiesen wurde.
*   **Name**: Der Name, der dem Zustand zugewiesen wurde.
*   **Beschreibung**: Die Beschreibung, die Sie dem Zustand gegeben haben.
*   **Typ**: Der Typ, den Sie dem Zustand zugewiesen haben.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

**Erläuterung der Felder**

*   **Zustandsnummer**: Eine eindeutige Nummer, die dem Zustand zugewiesen wird. Vom System wird die nächste freie Nummer vorgeschlagen. Sie können diese Nummer überschreiben.
    *   *Technische Info: Datenbankfeld: Zustandnr*
*   **Name**: In diesem Feld vergeben Sie einen Namen für den Zustand.
    *   *Technische Info: Datenbankfeld: Zustandname*
*   **Beschreibung**: In diesem Feld hinterlegen Sie eine ausführliche Beschreibung für den Zustand.
    *   *Technische Info: Datenbankfeld: Beschreibung*
*   **Text für Listen**: In diesem Feld geben Sie den Text ein, der auf den Listen erscheinen soll.
    *   *Technische Info: Datenbankfeld: Listenname*
*   **Barcode**: In diesem Feld geben Sie den Barcode des Zustands ein.
    *   *Technische Info: Datenbankfeld: Zustandbc*
*   **Zustandstyp**: Die Kombobox enthält alle angelegten Zustandstypen. Wählen Sie den entsprechenden Typ aus.
    *   *Technische Info: Datenbankfeld: Typ*
*   **AWRack-Info**: Über diese Checkbox steuern Sie, ob bei Änderung auf diesen Zustand der Gestellserver benachrichtigt werden soll oder nicht.
    *   *Technische Info: Datenbankfeld: Notify*
*   **AWRack-Status**: Die Kombobox enthält alle AWRack-Stati. Wählen Sie aus der Kombobox den Status aus, der diesem Zustand entspricht.
    *   *Technische Info: Datenbankfeld: Awrackstate*

**Ergänzende Informationen**
*   ⇨ "Zustandstypen" auf Seite H-103
*   ⇨ Tutorial, "Zustände" auf Seite H-37

### Mitarbeiter

*Stammdaten > BDE > Mitarbeiter*

[Image: Screenshot of the "Personal" dialog, showing a list of employees with their number, name, personnel number, description, and barcode.]
*Abb. H-9 Mitarbeiter*

In diesem Dialog legen Sie neue Mitarbeiter an oder nehmen Änderungen an bestehenden Mitarbeiterdaten vor.
*Technische Info: Datenbanktabelle: AWBAR_PERSON*

**Liste der Mitarbeiter**
*   **Nummer**: Die eindeutige ID, die dem Mitarbeiter zugewiesen wurde.
*   **Name**: Der Name, der dem Mitarbeiter zugewiesen wurde.
*   **Personal-Nr.**: Der Mitarbeiter-Schlüssel. Dieser ist identisch mit der ID.
*   **Beschreibung**: Die Beschreibung, die Sie dem Mitarbeiter gegeben haben.
*   **Barcode**: Der Barcode, der dem Mitarbeiter zugewiesen haben.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

**Erläuterung der Felder**

*   **Nummer**: In diesem Feld geben Sie eine eindeutige Nummer für den Mitarbeiter ein.
    *   *Technische Info: Datenbankfeld: PersonNr*
*   **Name**: In diesem Feld geben Sie den Namen des Mitarbeiters ein.
    *   *Technische Info: Datenbankfeld: PersonName*
*   **Beschreibung**: In diesem Feld können Sie eine zusätzliche Information zum Mitarbeiter hinterlegen.
    *   *Technische Info: Datenbankfeld: Beschreibung*
*   **Mitarbeiter-Nr.**: In diesem Feld geben Sie die Mitarbeiter-Nummer ein. Diese Nummer erfahren Sie im Lohnbüro oder der Buchhaltung.
    *   *Technische Info: Datenbankfeld: PersonKey*
*   **Barcode**: In diesem Feld geben Sie den Barcode für den Mitarbeiter ein. Dieser setzt sich zusammen aus der Nummer und der Personal-Nr. Beispiel: Sie haben einen 9stelligen Barcode, der Mitarbeiter hat die Nummer 60 und die Personal-Nr. ist die 51, dann ist der Barcode: 600000051.
    *   *Technische Info: Datenbankfeld: Personbc*

**Ergänzende Informationen**
*   ⇨ Tutorial, "Mitarbeiter" auf Seite H-33

### Spaltenzuordnung

*Stammdaten > BDE > Spaltenzuordnung*

[Image: Screenshot of the "Spaltenzuordnung" dialog for assigning processing types to columns/stations.]
*Abb. H-10 Spaltenzuordnung*

Dieser Bereich beschäftigt sich mit der Zuordnung der Spalten.

> **Systemkritische Daten**
> Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor. Die Daten in diesem Dialog sind systemkritisch.

### Spalten

*Stammdaten > BDE > Spalten*

[Image: Screenshot of the "Spalten" dialog, listing defined columns/stations by number and name.]
*Abb. H-11 Spalten*

Dieser Bereich beschäftigt sich mit den Spalten.

> **Systemkritische Daten**
> Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor. Die Daten in diesem Dialog sind systemkritisch.

### Nachbearbeitung

*Stammdaten > BDE > Nachbearbeitung*

[Image: Screenshot of the "BDE Nachbearbeitung" dialog, used to review and correct data processing errors.]
*Abb. H-12 Nachbearbeitung*

Sollten bei der Verarbeitung der BDE-Daten Probleme aufgetreten sein, finden Sie diese hier. Die Fehler müssen korrigiert werden!

**Erläuterung der Felder**

*   **Nur Initialisierung**: Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Fehler angezeigt, die bei der BDE-Initialisierung aufgetreten sind.
*   **Nur Buchungen**: Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Fehler angezeigt, die beim Buchen aufgetreten sind.
*   **Alle**: Über diese Radiotaste haben Sie die Möglichkeit, sich alle zur Nachbearbeitung anstehenden Teile anzeigen zu lassen.
*   **Unbearbeitete**: Über diese Radiotaste haben Sie die Möglichkeit, die angezeigten Daten einzuschränken. Ist die Radiotaste aktiv, werden nur die unbearbeiteten Teile angezeigt.

**Erläuterung der Schaltflächen**

*   **Wiederholen**: Wenn Sie diese Schaltfläche betätigen, wird der Buchungssatz erneut ausgewertet.
*   **Bearbeitet setzen**: Wenn Sie diese Schaltfläche betätigen, wird die Anzeige geleert.
*   **Aktualisieren**: Wenn Sie diese Schaltfläche betätigen, wird die Anzeige aktualisiert.

---

## Partindex

### Index Betriebsdatenerfassung

**B**
*   BDE-Buchungen
    *   lückenlose Buchung H-81

**D**
*   Denso-Scanner H-43
*   Direkte Objekte H-16

**E**
*   Einheiten scannen H-49
*   Erfassungsstelle
    *   Aktueller Zustand H-95
    *   Barcode H-95
    *   Bearbeitungsrückmeldung H-97
    *   Beschreibung H-95
    *   Betriebsmittel für Auftragserfassung H-97
    *   Einheitenrückmeldung H-97
    *   Erfassungsstellentyp H-95
    *   Gestellbelegung melden H-97
    *   Gestellrückmeldung H-97
    *   Gruppierung H-95
    *   Gruppierung für Schichten H-95
    *   LKW H-25
    *   Mengenüberschreitung H-96
    *   Name H-95
    *   Nummer H-94
    *   Produktionsrückmeldung H-97
    *   Produzierte Teile H-96
    *   Restriktionen H-96
    *   Text für Kundenlisten H-95
    *   Text für Produktionslisten H-95
    *   Unterzeile für Etiketten H-95
*   Erfassungsstellen
    *   Verwalten H-23
*   Expertenmodus
    *   Überblick H-73

**F**
*   Fehlergestell H-20

**G**
*   Gestelle H-27
    *   Aktuelle ES H-100
    *   Aktueller Zustand H-100
    *   Basis ES H-100
    *   BC-Startwert H-99
    *   Endwert H-99
    *   Fachnummer von ... bis H-99
    *   Filtern H-27
    *   Gestellart H-99
    *   Gestelltyp H-99
    *   Kundenname H-100
    *   Kundennummer H-100
    *   Letzte ES H-100
    *   Letzter Zustand H-100
    *   Lieferort H-101
    *   Mehrere Gestelle anlegen H-98
    *   Präfix H-99
    *   Startwert H-99
    *   Temporäres Gestell H-100
    *   Tournummer H-101
*   Gestellfilter
    *   Betriebseigene Gestelle H-102
    *   Erfassungsstelle H-102
    *   Erfassungsstellentyp H-102
    *   Gestellart H-102
    *   Gestellname von ... bis H-102
    *   Gestelltyp H-102

**I**
*   Indirekte Objekte H-16

**K**
*   Kisten H-28
*   Korrekte Daten H-81

**M**
*   Modul
    *   Funktion H-9

**O**
*   Offline-Scanner H-44
*   Online-Scanner H-43

**P**
*   Personal H-106

**S**
*   Scannen
    *   Einheiten H-49
*   Scanner
    *   Konfiguration H-44
*   Serielle Scanner H-44
*   Standard-Report
    *   Abstellliste H-75
    *   Auftragsstatus H-76
    *   Auftragsübersicht H-75
    *   Buchungshistorie H-78
    *   Gestellbelegung pro Position H-78
    *   Gestellbelegung pro Scheibe H-77
    *   Ladeliste H-76
*   Statusbarcode
    *   Scannen H-61
*   Systemkritische Daten
    *   Barcode-Optionen H-91
    *   Barcode-Typen H-92
    *   Erfassungsstellen-Typen H-93
    *   Spalten H-109
    *   Spaltenzuordnung H-108
    *   Zustandstypen H-103

**U**
*   Überblick
    *   Expertenmodus H-73

**V**
*   Versand H-51
*   Vorausgesetzte Kenntnisse H-9

**Z**
*   Zustand
    *   Aktions-Barcode H-38
    *   Einheit/Gruppe H-37
    *   Erfassungsstelle H-37
    *   Gestell H-37
*   Zustände
    *   AWRack-Info H-105
    *   AWRack-Status H-105
    *   Barcode H-105
    *   Beschreibung H-104
    *   Text für Listen H-105
    *   Zustandsname H-104
    *   Zustandsnummer H-104
