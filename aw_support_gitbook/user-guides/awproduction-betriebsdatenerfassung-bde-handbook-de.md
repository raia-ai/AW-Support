---
description: "DE_HB_AWProduction_10"
---


# A+W Production: Maschinenzuordnung (MZO)

---
## In diesem Kapitel finden Sie folgende Themen:

- Informationen zu den Help Cards
- Maschinenzuordnung (MZO)

| Thema | Seite |
| :--- | :--- |
| Informationen zu den Help Cards | G-903 |
| Maschinenzuordnung (MZO) | G-904 |
| Neue Maschine einfügen | G-905 |
| Neue Maschine einfügen | G-906 |
| Neue Maschine für Production Terminal | G-907 |

---

## Informationen zu den Help Cards

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W Production. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

---

## Maschinenzuordnung (MZO)

| Help Card | Themen |
| :--- | :--- |
| **Neue Maschine einfügen** | Sie fügen eine neue Maschine in eine bestehende MZO ein. |
| **Neue Maschine für Production Terminal** | Sie konfigurieren eine neue Maschine für das Production Terminal. |

---

## Neue Maschine einfügen (MZO 01-001)

### Ziel der Handlung
Sie fügen eine neue Maschine in eine bestehende MZO ein.

### Voraussetzungen
(Keine angegeben)

### Zusatzinfo
- **Logische Maschinen** dienen zur Unterscheidung zweier möglicher Prozesse oder Werkzeuge, welche auf einer physikalischen Maschine durchgeführt werden können (z. B. CNC-Maschine kann Bohren und Schleifen). An der physikalischen Maschine werden die physikalischen Restriktionen hinterlegt (z. B. zulässige Glasdicken). An der logischen Maschine werden die Maschinentreiber hinterlegt um den richtigen Prozess / das richtige Werkzeug anzusteuern.
- **Einstellungen und Restriktionen** werden explizit ausgewertet. D. h., sind keine Begrenzungen hinterlegt, kann die Maschine alles. Sonst kann die Maschine nur innerhalb der hinterlegten Parameter arbeiten, z. B. nur Rechtecke, keine Modelle.
- Nach Änderungen an den Maschinenstammdaten muss der Einlastungsdient Items4Alcim neu gestartet werden.

### Workflow

1. Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen > [Neu].
2. Geben Sie eine ID aus dem Nummernbereich ein, den Sie für diesen Maschinentyp vorgesehen haben.
3. Geben Sie einen Namen ein, der die Maschine eindeutig beschreibt.
4. Wählen Sie den zugehörigen Maschinentyp.
5. Für Zuschnitt-Tische, ISO-Linien und Bieger geben Sie eine Komponenten-ID ein, um die direkte Ansteuerung aus MZO zu gewährleisten.
6. Klicken Sie auf [OK], um die Daten zu speichern.
7. Markieren Sie in der Liste die Maschine, die Sie soeben angelegt haben. Klicken Sie auf die Schaltfläche [Bearbeiten].
8. Ergänzen Sie die erforderlichen Daten für Ihre neue physikalische Maschine. Im oberen Bereich können Sie generelle Einstellungen vornehmen, z. B. eine Erfassungsstelle zuweisen.
9. Klicken Sie doppelt auf [...]. Ein [Pfeil] wird angezeigt. Klicken Sie auf den [Pfeil], um eine Restriktion für die minimale Dicke einzugeben. Geben Sie den Wert der minimalen Dicke in Millimetern ein. Klicken Sie auf die Schaltfläche [OK], um den Wert zu speichern.
10. Wiederholen Sie Schritt 9 um die Restriktionen für die maximale Dicke zu bearbeiten.
11. Klicken Sie im Feld Abmessungen auf das [Stift-Symbol], um den Dialog Abmessungsrestriktionen zu öffnen. Aktivieren Sie die Checkboxen der Eingabefelder, die Sie bearbeiten möchten. Geben Sie die Werte in die Eingabefelder ein. Klicken Sie auf die Schaltfläche [OK], um die Änderungen der Abmessungsrestriktionen zu speichern.
12. Bearbeiten Sie auf die gleiche Weise die Restriktionen für den/die SZR.
13. Im unteren Bereich des Dialoges können Sie zusätzliche Bedingungen hinterlegen. Mittels der Lupe können Sie hier eine entsprechende Formel zuweisen (z. B. Glas wurde bereits Flächenentschichtet).

---

## Neue Maschine für Production Terminal (MZO 01-002)

### Ziel der Handlung
Sie konfigurieren eine neue Maschine für das Production Terminal.

### Voraussetzungen
- Sie arbeiten in Ihrem Hause mit den A+W Production Terminals.
- Sie haben die Help Card *Neue Maschine einfügen* durchgearbeitet.

### Zusatzinfo
Die Original A+W Production Terminals-Anzeigen (zu erkennen am Namen AUW ...) dürfen bzw. können nicht verändert werden. Damit wird sichergestellt, dass die Original-Schirme immer funktionieren und nicht durch Änderungen zerstört werden können.

### Workflow
1. Legen Sie die neue Maschine wie in der Help Card *Neue Maschine einfügen* beschrieben, an.
2. Weisen Sie der Maschine im Dialog Maschine - XYZ eine Erfassungsstelle zu.
3. Schließen Sie den Dialog MZO-Editor.
4. Wählen Sie im Menü Stammdaten > Konfiguration. Es öffnet sich der Dialog Parameter-Administrator.
5. Öffnen Sie die Baumstruktur ToolTV und wählen Sie die Variante des Production Terminals, dem Sie die Maschine hinzufügen möchten.
6. Nach dem Markieren des Production Terminals, welches Sie ändern wollen, muss dieses mit der Kopierfunktion kopiert werden. Der Kopie geben Sie einen neuen, sprechenden Namen. Die Kopie können Sie dann ändern bspw. die neue Erfassungsstelle hinzufügen. Das Original A+W Production Terminal darf aus den oben erwähnten Gründen nicht geändert werden.
7. Wählen Sie zu den bereits markierten Erfassungsstellen noch die aus, die Sie neu angelegt haben.
8. Klicken Sie auf [OK], um den Dialog zu schließen. Im Dialog Parameter-Administrator klicken Sie auf [Übernehmen] und dann auf [Beenden], um den Dialog zu schließen.

---

# A+W Production: Betriebsdatenerfassung

## Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| **01-2017** | Produkt- und Firmennamen angepasst. |
| **06-2014** | Komplette Überarbeitung. |
| **07-2013** | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production. |
| **03-2007** | Ersterstellung. |

### Zu diesem Modul finden Sie folgende Kapitel:
- Tutorial
- Softwarereferenz

---

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:
- Überblick
- Grundgedanken
- Buchungselemente
- Datenerfassung
- Buchungsbeispiele
- Production Terminals
- Bruchmanagement
- Statistik, Reporting und Monitoring

### Inhaltsverzeichnis

- **Überblick** (H-914)
  - Aufbau des Tutorials (H-915)
- **Grundgedanken** (H-916)
  - Die Betriebsdatenerfassung (H-917)
  - Zweck der AWP (H-917)
- **Buchungselemente** (H-918)
  - Produkte (H-919)
    - Grundsätzliches (H-920)
    - Direkte Objekte (H-920)
    - Indirekte Objekte (H-920)
    - Scheiben bzw. Einheiten (H-920)
    - Buchungsarten (H-921)
  - Buchungsorte (H-922)
    - Erfassungsstellen (H-923)
    - Fehlergestell (Error-Rack) (H-924)
    - Korrekte Buchung (H-926)
    - Erfassungsstellen verwalten (H-927)
    - Erfassungsstelle Lkw (H-929)
  - Abstellplätze (H-930)
    - Gestelle (H-931)
    - Kisten (H-932)
    - Gestelle verwalten (H-933)
  - Personal (H-936)
    - Mitarbeiter (H-937)
    - Mitarbeiter verwalten (H-938)
  - Status (H-940)
    - Zustände (H-941)
    - Zustände verwalten (H-943)
- **Datenerfassung** (H-945)
  - Scanner (H-946)
    - Scanner-Typen (H-947)
    - Konfiguration der Scanner (H-948)
  - Barcodes (H-949)
- **Buchungsbeispiele** (H-950)
  - Die Reihenfolge des Scannens (H-951)
  - Scannen von Einheiten (H-953)
  - Scannen im Versand (H-955)
  - Erfassungsstellen scannen (H-957)
  - Erfassungsstelle LKW (H-960)
  - Gestelle bzw. Kisten scannen (H-963)
  - Status scannen (H-965)
  - Korrigieren von Fehlbuchungen (H-966)
- **Production Terminals** (H-967)
  - Einführung (H-969)
- **Bruchmanagement** (H-972)
  - Überblick (H-973)
  - Bruchbehandlung (intern) (H-974)
- **Statistik, Reporting und Monitoring** (H-976)
  - Überblick (H-977)
  - BDE-Reporting (H-978)
  - Monitoring: A+W Dashboard (H-983)
  - Statistik: A+W Discovery (H-987)

---

### Überblick

Die Zielgruppe der Schulung zum Modul A+W Production sind Mitarbeiter, die an unterschiedlichen Stationen (Maschinen und Erfassungsstellen) innerhalb der Produktion arbeiten.

Der Vorteil für den Kunden liegt darin, dass er seine Maschinen direkt ansteuern kann. Es entstehen dadurch keine Ausfallzeiten, um eine Form an einer Bearbeitungsmaschine zu digitalisieren. Es müssen auch keine NC-Codes an der Maschine eingegeben werden, was auch einen ständigen Maschineneinsatz bedeutet.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- Grundgedanken
- Buchungselemente
- Datenerfassung
- Statistik, Reporting und Monitoring

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die an unterschiedlichen Stationen (Bereiche, Maschinen und Erfassungsstellen) innerhalb der Produktion arbeiten. Die Teilnehmer müssen das Konzept der Production Terminals und der Scanner kennen.

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwendung der AWP vorausgesetzt.

---

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - **Lernziele**: Was soll vermittelt werden?
  - **Nutzen**: Wofür können Sie dieses Wissen einsetzen?
  - **Merksätze**: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen. Die Übungen helfen Ihnen A+W Production zu verstehen und anwenden zu lernen.
- **Querverweisteil**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht ein roter Faden durch die gesamte Dokumentation.

---

### Grundgedanken

Diese Dokumentation gibt Ihnen einen Einblick in die Betriebsdatenerfassung (AWP) der A+W Software GmbH und vermittelt ein Grundverständnis für dieses Thema. Die Grundzüge der AWP, die zum Einsatz kommenden Werkzeuge und die grundsätzlichen Möglichkeiten und Grenzen werden erläutert.

Das Studium weiterführender Dokumentationen zu Leitrechner (Production Terminals), interner AWP Installations- und Konfigurationsanleitungen, Scanner-Installation und Konfiguration usw. wird dringend empfohlen. Diese Themen werden in dieser Dokumentation angeschnitten aber nicht vertieft. Eine eindeutige Abgrenzung der Bereiche ist nicht immer möglich und auch nicht sinnvoll.

Diese Anleitung ersetzt kein grundlegendes Wissen über Produktionsstrukturen, die eingesetzten Production Terminals, Scanner oder andere A+W Software.

#### Aufbau dieses Dokumentes
Diese Dokumentation beschreibt allgemeines Wissen zur AWP. Was ist die AWP, die wichtigsten Komponenten, Erfassungsstellen, welche Scannertypen kommen zum Einsatz, Vorgehensweisen, usw.

---

### Die Betriebsdatenerfassung

Die AWP ist ein Sammelbegriff für die Erfassung von Istdaten über Zustände und Prozesse in Betrieben.

Sie erfasst den Produktionsfluss an den wichtigsten Stellen innerhalb der Produktion, den so genannten Erfassungsstellen und bildet so den Prozessfluss Ihrer Produktion ab. Dies geschieht mit Hilfe von z. B. Barcodes, Scannern, Production Terminals (Leitrechner), usw. Die erfassten Daten werden entweder direkt oder indirekt an eine entsprechende Sammelstelle (AWPort) übermittelt und in der Datenbank (A+W Production-DB) gespeichert.

### Zweck der AWP

Die AWP dient der Darstellung der aktuellen Ist-Situation: Feststellung des Produktionsstatus eines Auftrages, Verfolgung einer Position oder Einzelscheibe durch die Produktion, Überwachung der Leistung (Maschine und Bediener) bis hin zur Darstellung der Performance.

Im Falle von Bruchscheiben wird neben der Erfassungsstelle auch der Bruchgrund erfasst. Je nach Konfiguration werden automatisch entsprechende Nachläufer generiert. Die Maschinenansteuerung erfolgt ebenfalls automatisch aufgrund von Barcodelesungen.

Ein weiterer wichtiger Aspekt der AWP sind die statistischen Auswertungen. Sie können die Produktivität und die Maschinenlaufzeiten messen sowie Produktionsfehler (z. B. Bruch) überwachen. Die mittels der AWP gescannten und erfassten Daten können mit Controlling- und Statistik-Werkzeugen von A+W ausgewertet und reported werden. Mit A+W Dashboard (aktuelle Leistung- und Status-Kennzahlen) und A+W Discovery (statistische Kennzahlen).

---

### Buchungselemente

In diesem Themenblock lernen Sie den Umgang mit den unterschiedlichen Objekten der AWP.

Dazu gehören folgende Lerneinheiten:
- "Produkte" auf Seite H-919
- "Buchungsorte" auf Seite H-922
- "Abstellplätze" auf Seite H-930
- "Personal" auf Seite H-936
- "Status" auf Seite H-940

#### Produkte

**Lernziele**
- Objekte der AWP kennenlernen.
- Was ist verfolgbar und was ist nicht verfolgbar.

**Definitionen**
- **Direkte Objekte**: Haben einen Barcode und werden direkt gebucht.
- **Indirekte Objekte**: Haben keinen Barcode, da sie automatisch mit gebucht werden.

**Merke**
- **Verfolgbare Produkte**: Alle Teile einer Stückliste, auf die man einen Barcode kleben kann.
- **Einzelscheiben-AWP**: Jedes Stücklistenteil wird durch einen eigenen Barcode identifiziert.
- **Mengen-AWP**: Alle Teile eines Stücklistenteils haben den gleichen Barcode.

#### Grundsätzliches

Die AWP unterscheidet zwei Objekt-Typen:
- **Direkte Objekte**: Solche, die einen Barcode haben und direkt gebucht werden können. Dazu gehören:
  - Erfassungsstellen (Orte, LKWs und Maschinen)
  - Gestelle und Kisten
  - Scheiben und Einheiten
  - Zustände / Stati
  - Mitarbeiter
- **Indirekte Objekte**: Solche, die automatisch mitgebucht werden. Dazu gehören:
  - Bearbeitungen
  - Chargeninformationen

#### Scheiben bzw. Einheiten

Bei Scheiben und Einheiten handelt es sich um verfolgbare Produkte. Das sind grundsätzlich alle Teile einer Stückliste, auf die man einen Barcode kleben kann. Beispiel: Einzelscheibe, ISO, VSG, Rahmen, Sprosse, etc.

In der **Einzelscheiben-AWP (Standard)** wird jedes Stücklistenteil durch einen eindeutigen Barcode identifiziert. Dadurch kann jederzeit der genaue Ort und Zustand eines Teils bestimmt werden.

In der **Mengen-AWP** haben alle Teile eines Stücklistenteils den gleichen Barcode. Dadurch ist der genaue Ort und Zustand eines Teils nicht mehr exakt bestimmbar. Hier werden nur quantitative Aussagen über Produktionszustände gemacht. Der Buchungsaufwand ist demzufolge wesentlich geringer.

Im Gegensatz zu verfolgbaren Teilen (Scheiben, Sprossen, Rahmen), können andere Stücklistenteile wie bspw. Gas, Silikon, Folien nicht gescannt bzw. verfolgt werden.

> **Daten buchen**
> Um eine möglichst gute Datenbasis für grafische Kontroll-Anzeigen und statistischen Auswertungen zu erhalten, ist es notwendig, in der Produktion kontinuierlich und exakt die Scheiben/Teile/Einheiten an den entsprechenden Erfassungsstellen auf das entsprechende Gestell zu buchen.

#### Buchungsarten

Es werden drei verschiedene Buchungsarten unterschieden:
- **Bewegungsbuchungen**: Dokumentieren die Ortsveränderung eines Gestells, einer Einheit oder einer Scheibe. Dies geschieht durch Buchung eines Gestells (Einheit auf Gestell) oder einer Erfassungsstelle (Gestell oder Einheit auf Erfassungsstelle).
- **Bearbeitungsbuchungen**: Bilden Bearbeitungen (z. B. Bohren) von Einheiten ab.
- **Zustandsbuchungen**: (z.B. Bruch, Wartung) geben die Zustandsänderung eines Objekts wieder.

Bearbeitungs- und Zustandsbuchungen können auch durch Bewegungsbuchungen implizit ausgelöst werden.

Wichtig in diesem Zusammenhang ist natürlich die Brucherfassung. Bei der Brucherfassung wird neben der Erfassungsstelle und weiteren Informationen auch der Bruchgrund erfasst. Je nach Konfiguration werden automatisch Nachläufer generiert.

Die gewonnenen Daten können u. a. zu Auswertungs-, Statistik- und Inventurzwecken (z. B. BDE-Reports, MS-Excel usw.) verwendet werden. Sie dienen der Produktionssteuerung, der Scheiben-/Einheiten-, Gestellverfolgung u.v.m.

**Ergänzende Informationen**
- "Bruchmanagement" auf Seite H-972
- "BDE-Reporting" auf Seite H-978
- "Scannen von Einheiten" auf Seite H-953

---

### Buchungsorte

**Lernziele**
- Den Dialog Erfassungsstellen erarbeiten.
- Die Erfassungsstelle Fehlergestell kennenlernen und verstehen.
- Die Erfassungsstelle Versand kennenlernen und verstehen.

**Nutzen**
Um Buchungsfehler zu vermeiden, ist es notwendig, die korrekte Buchungsreihenfolge einzuhalten.

**Definitionen**
- **ES**: Abkürzung für Erfassungsstelle.
- **Erfassungsstellen**: Stationen innerhalb der Produktion bzw. des Versands.
- **Fehlergestell**: Ist eine interne Erfassungsstelle mit der Erfassungsstellennummer 12 und wird automatisch gefüllt. Diese Erfassungsstelle dient zur Aufnahme aller Einheiten, die aufgrund von Fehlern ihre Zuordnung zu einem physikalischen Gestell bzw. einer physikalischen Erfassungsstelle verloren haben.
- **Triggerzeit**: Die im System hinterlegte Zeitspanne, die festlegt, ab wann die Ladung eines Lkw als ausgeliefert gilt. Sie wird durch die Status-Buchung `<Begin> <Truck>` aktiviert. Die Dauer kann im System konfiguriert werden.

**Merke**
- **Erfassungsstellen**: Erhalten eine eindeutige Nummer und einen Namen.

#### Erfassungsstellen

Alle Stationen innerhalb der Produktion (Produktionsbereiche, LKW, Maschinen), an denen sich Scanner und/oder Production Terminals befinden, werden als Erfassungsstellen (ES) bezeichnet. Sie erhalten eine eindeutige Nummer und einen Namen.

Eine Maschine muss nicht zwingend eine Erfassungsstelle sein. Sie kann durchaus in mehrere Erfassungsstellen aufgeteilt werden.

**Beispiel: ISO-Linie**
- 1611 > Maschineneingang,
- 1610 > die Maschine selbst und
- 1612 > Maschinenausgang.

Durch die Aufteilung von Maschinen in mehrere Erfassungsstellen ist eine genauere Verfolgung und Analyse der Produktion möglich. Auf diese Erfassungsstellen können Sie Gestelle, Produkte und Zustände buchen. Je mehr Erfassungsstellen es gibt, umso genauer sind die Auswertungen.

**Abb. H-1 Erfassungsstellen**
(Dialogfenster "Erfassungsstellen" mit Liste und Details zu einer Erfassungsstelle)

Die Tabelle zeigt, welche Erfassungsstellen bereits angelegt sind. Sie können neue Erfassungsstellen anlegen, aber auch Änderungen an bereits angelegten Erfassungsstellen vornehmen.

Bei den Checkboxen im Bereich *Rückmeldung von Buchungen* handelt es sich um Produktionsrückmeldungen, die dazu dienen, den aktuellen Auftragsstatus im übergeordneten Auftragsbearbeitungssystem zu aktualisieren.

> **Spaltenüberschriften frei konfigurierbar**
> Die Überschriften der einzelnen Spalten sind frei konfigurierbar. Somit ist es möglich, dass die Überschriften, die hier gezeigt werden, nicht mit den Überschriften in Ihrer Installation übereinstimmen.

#### Fehlergestell (Error-Rack)

Das Fehlergestell (Error-Rack) ist eine interne Erfassungsstelle. Diese Erfassungsstelle dient zur Aufnahme aller Einheiten, die aufgrund von Fehlern ihre Zuordnung zu einem physikalischen Gestell bzw. einer physikalischen Erfassungsstelle verloren haben. Die interne Erfassungsstelle *Fehlergestell* hat die Erfassungsstellennummer 12.

Grundsätzlich gibt es zwei Regeln für die Erfassungsstelle Fehlergestell:
- **Regel 1**: Das Fehlergestell sollte immer leer sein!
- **Regel 2**: Ist das Fehlergestell nicht leer, liegt ein Bedien- oder Scannerfehler vor.

**Wie gelangen Einheiten auf das Fehlergestell?**
Hierfür gibt es mehrere Gründe. Neben einem defekten Scanner/Etikett, ist dies in der Regel eine Fehlbedienung durch das Personal. Das Fehlergestell wird immer dann gefüllt, wenn eine Erfassungsstelle oder ein Gestell mit dem Status `<Begin>` gescannt wurde und sich AWP-seitig noch Einheiten auf diesem Objekt befanden. Diesen Einheiten wird automatisch die Erfassungsstelle Fehlergestell zugewiesen.

**Mögliche Ursachen:**
- **Beispiel 1:** An einer Erfassungsstelle sind mehrere Gestelle im Zugriff. Ein Gestell wird angemeldet, Einheiten gebucht. Beim Wechsel auf das zweite Gestell wird vergessen, dieses anzumelden. Die Einheiten werden physikalisch auf Gestell 2 gestellt, buchungstechnisch aber auf das falsche Gestell 1. Wird Gestell 1 später als leer gescannt (`<Begin> <Rack1>`), werden die buchungstechnisch noch darauf befindlichen Einheiten auf das Fehlergestell gebucht.
- **Beispiel 2:** Ein Lkw wird beladen, aber die `<Ausgeliefert>`-Buchung unterbleibt. Am nächsten Tag wird der Lkw mit `<Beginn>` neu angemeldet. Die alte Ladung wird buchungstechnisch auf das Fehlergestell verschoben.
- **Beispiel 3:** Ein beladenes Gestell wird ohne Scanner entladen. Beim nächsten Einsatz wird es mit `<Beginn>` angemeldet und die alten Einheiten werden auf das Fehlergestell gebucht.

**Einheiten vom Fehlergestell entfernen**
Einheiten auf dem Fehlergestell können wie bei jeder anderen Erfassungsstelle durch neue Buchungen manipuliert werden.
- **Manuelle Methode:** Über *Terminal Edit* die Erfassungsstelle (des Gestells) manuell ändern.
- **Automatische Methode:** Korrigiert einen Fehler automatisch durch eine weitere korrekte Buchung im Produktionsablauf.

> **Tipp**
> Überprüfen Sie regelmäßig die interne Erfassungsstelle 12 *Fehlergestell* und nehmen Sie Korrekturen umgehend vor. Nutzen Sie hierfür *Terminal Edit* oder die *Barcode Manager-Reports*.

#### Korrekte Buchung

Einheiten, die auf die interne Erfassungsstelle 12 *Fehlergestell* gelangt sind, werden von dort automatisch bei der nächsten korrekten Buchung dieser Einheiten an einer Erfassungsstelle/dem Gestell zugeordnet und verschwinden von der Erfassungsstelle Fehlergestell.

Voraussetzung für die automatische Korrektur ist, dass sich die Einheiten noch im Produktionsprozess befinden und bei weiteren Bearbeitungen gescannt werden. Jeder dieser Scannvorgänge ordnet der Einheit die entsprechende Erfassungsstelle/das Gestell zu, die Einheit verschwindet automatisch von der internen Erfassungsstelle 12 Fehlergestell.

**Ergänzende Informationen**
- Softwarereferenz, "Erfassungsstellen" auf Seite H-998
- "Scannen im Versand" auf Seite H-955
- "Erfassungsstellen scannen" auf Seite H-957

#### Erfassungsstellen verwalten

In dieser Einheit lernen Sie, wie Sie neue Erfassungsstellen anlegen, bearbeiten oder auch löschen.

##### So legen Sie eine neue Erfassungsstelle an
1. Öffnen Sie den Dialog Erfassungsstelle.
2. Betätigen Sie die Symbol-Schaltfläche [Neu].
3. Geben Sie im Feld *Erfassungsstellennr.* eine eindeutige Nummer ein.
4. Geben Sie im Feld *Barcode* die Barcode-Nummer ein.
5. Geben Sie im Feld *Name* den Namen ein.
6. Hinterlegen Sie eine *Beschreibung*.
7. Geben Sie Texte für *Produktionslisten* und *Kundenlisten* ein.
8. Geben Sie Text für *Unterzeile für Barcodeetiketten* ein.
9. Wählen Sie den *Erfassungsstellen-Typ* aus.
10. Hinterlegen Sie optional eine *Gruppierung* oder *Gruppierung für Arbeitsschichten*.
11. Wählen Sie den *Aktuellen Zustand* aus.
12. Aktivieren und steuern Sie bei Bedarf die *Restriktion*.
13. Geben Sie bei aktivierter Restriktion eine *Mengenüberschreitung* in Prozent an.
14. Aktivieren Sie die Checkbox *Produzierte Teile anzeigen*, wenn komplett produzierte Scheiben im Production Terminal angezeigt werden sollen.
15. Aktivieren Sie die verschiedenen Checkboxen für *Rückmeldungen*, falls erforderlich (Bearbeitungsrückmeldung, Gestellrückmeldung etc.).
16. Klicken Sie auf [Speichern].

##### So löschen Sie eine Erfassungsstelle
1. Öffnen Sie den Dialog Erfassungsstelle.
2. Wählen Sie die zu löschende Erfassungsstelle aus.
3. Betätigen Sie die Symbol-Schaltfläche [Löschen].
4. Bestätigen Sie die Sicherheitsabfrage mit [Ja].

##### So nehmen Sie Änderungen an Erfassungsstellen vor
1. Öffnen Sie den Dialog Erfassungsstelle.
2. Wählen Sie die zu ändernde Erfassungsstelle aus.
3. Betätigen Sie die Symbol-Schaltfläche [Ändern].
4. Nehmen Sie die gewünschten Änderungen vor.
5. Klicken Sie auf die Symbol-Schaltfläche [Speichern].

#### Erfassungsstelle Lkw

Jeder Lkw stellt eine Erfassungsstelle dar. Eine Ausnahme ist das Barcode-seitige Leeren des Lkw. Objekte verlassen eine Erfassungsstelle normalerweise, indem sie an einer anderen angemeldet werden. Beim Lkw ist das unpraktikabel (z.B. Scannen auf der Baustelle).

Die Objekte müssen Barcode-seitig von dieser Erfassungsstelle gebucht und der internen Erfassungsstelle 11 (Außer Haus) zugeführt werden. Dies geschieht nach einer im System hinterlegten Zeitspanne, die durch das Scannen des Status `<Ausgeliefert> <Lkw>` getriggert wird.

Eine Status-Buchung `<Beginn><Lkw>` innerhalb der Zeitspanne würde den Lkw/die Gestelle zurücksetzen und die betroffenen Einheiten auf das Fehlergestell buchen.

Nach Ablauf der Zeitspanne gelten alle Einheiten als ausgeliefert (auf ES 11) und der Lkw kann wieder in den Produktionsprozess übernommen werden.

---

### Abstellplätze

**Lernziele**
- Den Dialog Gestelle erarbeiten.
- Den Buchungsablauf kennenlernen und verstehen.

**Nutzen**
Um die BDE zu verstehen, müssen Sie wissen, was auf Abstellplätze gebucht werden kann.

**Definitionen**
- **Gestell-Typen**: A-Gestelle, L-Gestelle, Fächerwagen, Kisten und besondere Gestelle für Ofenbetten und Autoklaven.

**Merke**
- **Gestell buchen**: Wird ein Gestell auf eine Erfassungsstelle gebucht, sind automatisch auch alle Einheiten des Gestells auf diese Erfassungsstelle gebucht.
- **Gestelle anlegen**: Können in den Stammdaten manuell oder automatisch angelegt werden.
- **Buchen**: Auf Gestelle können Produkte oder Zustände gebucht werden.
- **Wo befindet sich ein Gestell**: Ein Gestell befindet sich immer an genau einem Ort (Erfassungsstelle).
- **Kisten**: Kehren nicht in den Produktionszyklus zurück.

#### Gestelle
In diesem Bereich legen Sie die Gestelle für die AWP an. Es gibt folgende Gestelltypen:
- A-Gestelle
- L-Gestelle
- Fächerwagen
- Kisten
An einigen Erfassungsstellen (Öfen, Autoklaven) sind besondere Gestelle notwendig. Ein Gestell befindet sich immer an genau einem Ort in der Produktion (Erfassungsstelle).

**Abb. H-2 Gestelle**
(Dialogfenster "Gestelle" mit Liste und Details zu einem Gestell)

**Gestelle filtern**
Verfügen Sie über eine große Anzahl an Gestellen, können Sie sich Filter anlegen. Bei gesetztem Filter erscheint die Anzeige: **Achtung: Gestellfilter ist gesetzt!**

**Abb. H-3 Gestellfilter gesetzt**

#### Kisten
Kisten werden wie Gestelle behandelt, kehren aber nicht in den Produktionszyklus zurück. Es ist sinnvoll, für Kisten einen separaten Nummernkreis für Barcodes zu verwenden, der komplett aufgebraucht wird.

> **Erzeugen von Barcodes**
> Nutzen Sie immer den Report zum Erzeugen von Barcodes. Alternativ können die Barcodes auch über ein Microsoft Word Dokument zur Verfügung gestellt werden.

**Ergänzende Informationen**
- Softwarereferenz, "Gestelle" auf Seite H-1002
- Softwarereferenz, "Gestellfilter" auf Seite H-1006
- "Gestelle bzw. Kisten scannen" auf Seite H-963

#### Gestelle verwalten

##### So legen Sie ein neues Gestell an
1. Öffnen Sie den Dialog Gestelle.
2. Betätigen Sie [Neu].
3. Geben Sie einen *Namen* und *Barcode* ein.
4. Wählen Sie *Gestellart* und *Gestelltyp* aus.
5. Bei Fachgestellen, geben Sie die erste und letzte Fachnummer an.
6. Weisen Sie die *Basis-ES* zu.
7. Aktivieren Sie ggf. *Temporäres Gestell*.
8. Klicken Sie auf [Speichern].

##### So legen Sie mehrere neue Gestelle auf einmal an
1. Öffnen Sie den Dialog Gestelle und betätigen Sie [Neu].
2. Aktivieren Sie die Checkbox *Mehrere Gestelle anlegen*.
3. Geben Sie *Präfix*, *Startwert*, *Endwert* und *BC-Startwert* ein.
4. Wählen Sie *Gestellart* und *Gestelltyp*.
5. Geben Sie ggf. Fachnummern an.
6. Weisen Sie die *Basis-ES* zu.
7. Aktivieren Sie ggf. *Temporäres Gestell*.
8. Klicken Sie auf [Speichern] und bestätigen Sie die Abfrage.

##### So löschen Sie ein Gestell
1. Öffnen Sie den Dialog Gestelle.
2. Wählen Sie das zu löschende Gestell aus.
3. Betätigen Sie [Löschen] und bestätigen Sie mit [Ja].

##### So nehmen Sie Änderungen an einem Gestell vor
1. Öffnen Sie den Dialog Gestelle.
2. Wählen Sie das zu ändernde Gestell aus.
3. Betätigen Sie [Ändern].
4. Nehmen Sie die Änderungen vor und klicken Sie auf [Speichern].

##### So setzen Sie einen Gestellfilter
1. Öffnen Sie den Dialog Gestelle.
2. Betätigen Sie die Schaltfläche [Filter], um den Dialog *Gestellfilter* zu öffnen.
3. Filtern Sie nach Kriterien wie *Erfassungsstellen-Typen*, *Erfassungsstellen*, *Gestellnamen* etc.
4. Klicken Sie auf [Übernehmen].

##### So löschen Sie einen Gestellfilter
1. Öffnen Sie den Dialog Gestelle und betätigen Sie [Filter].
2. Klicken Sie auf [Zurücksetzen].
3. Schließen Sie den Dialog. Alle Gestelle werden wieder angezeigt.

---

### Personal

**Lernziele**
- Den Dialog Mitarbeiter erarbeiten.
- Den Umgang mit den Mitarbeitern kennenlernen und verstehen.
- Mitarbeiter anlegen und bearbeiten.

**Nutzen**
Für jeden Mitarbeiter können unterschiedliche Kostensätze hinterlegt werden. Damit können die Personalkosten genauer berücksichtigt werden. Darüber hinaus kann ausgewertet werden, wie viele Mitarbeiter an einer Bearbeitung beteiligt waren.

**Merke**
- **Mitarbeiter anlegen**: Ein Mitarbeiter muss erst angelegt werden, bevor er sich an einer Station anmelden kann.
- **Angemeldete Person**: Wird der Buchung mitgegeben. Bleibt angemeldet, bis ein anderer Namen-Barcode gescannt wird.
- **Anmeldung zwingend erforderlich**: Scanner und A+W Production Terminal können so eingestellt werden, dass eine Personenanmeldung zwingend erforderlich ist.

#### Mitarbeiter
Alle Mitarbeiter, die mit der AWP zu tun haben, müssen einmal registriert werden. Nachdem ein Mitarbeiter erfasst ist, kann er sich an den einzelnen Stationen anmelden. Er wird dann automatisch den einzelnen Buchungen mitgegeben und ist der für die Buchung verantwortliche Mitarbeiter.

**Abb. H-5 Mitarbeiter**
(Dialogfenster "Personal" mit Liste von Mitarbeitern)

Für jeden Mitarbeiter können unterschiedliche Kostensätze hinterlegt werden. Es ist auch möglich, dass mehrere Mitarbeiter an einer Station angemeldet werden.

#### Mitarbeiter verwalten

##### So legen Sie einen neuen Mitarbeiter an
1. Öffnen Sie den Dialog Mitarbeiter.
2. Betätigen Sie [Neu].
3. Geben Sie eine eindeutige *Nummer* und den *Namen* ein.
4. Hinterlegen Sie optional eine *Beschreibung*.
5. Geben Sie die *Personal-Nr.* ein.
6. Geben Sie die *Barcode*-Nummer ein (kann sich aus Nummer und Personal-Nr. zusammensetzen).
7. Klicken Sie auf [Speichern].

##### So löschen Sie einen Mitarbeiter
1. Öffnen Sie den Dialog Mitarbeiter.
2. Wählen Sie den zu löschenden Mitarbeiter aus.
3. Betätigen Sie [Löschen] und bestätigen Sie mit [Ja].

##### So nehmen Sie Änderungen an Mitarbeiterdaten vor
1. Öffnen Sie den Dialog Mitarbeiter.
2. Wählen Sie den zu ändernden Mitarbeiter aus.
3. Betätigen Sie [Ändern].
4. Nehmen Sie die Änderungen vor und klicken Sie auf [Speichern].

---

### Status

**Lernziele**
- Den Dialog Zustände erarbeiten.
- Unterschiedliche Zustand-Typen kennenlernen und verstehen.

**Nutzen**
Um aussagekräftige Auswertungen zu erhalten, muss eine gewisse Buchungsdisziplin eingehalten werden.

**Definitionen**
- **Zustände**: Beschreiben den Zustand eines Objektes.
- **Maschinen-Zustand**: Bereit, Aus, Störung, Wartung, Pause, ...
- **Produkt-Zustand**: Bruch, Mangel, ...
- **Gestell-Zustand**: Leer, fertig, ausgeliefert, ...
- **Erfassungsstellen-Zustand**: Fertig, ausgeliefert, leer, ...
- **Aktions-Zustand**: OK, abbrechen, übernehmen, ...

**Merke**
- **Unterbrechungen**: Arbeitsunterbrechungen müssen immer protokolliert werden.

#### Zustände
Die Aufgabe der AWP ist es, den IST-Zustand eines Objektes innerhalb der Produktion zu erfassen. Zustände wirken auf folgende AWP-Objekte:
- Einheit/Gruppe
- Gestell
- Erfassungsstellen
- Personal

**Einheit/Gruppe**: Status einer Scheibe/Einheit. z.B. *Noch nicht produziert*, *Bruchscheibe*, *Mangel*, *Versandfertig*.

**Gestell**: Status eines Gestells. z.B. *Leer*, *Voll*, *Außer Haus*, *Versandfertig*.

**Erfassungsstelle**: Status einer Erfassungsstelle. z.B. *Beginn*, *An*, *Aus*. Arbeitsunterbrechungen (Wartung, Störung, Pause, Rüstzeiten) müssen immer protokolliert werden.

**Aktions-Barcode**: Ermöglicht das Scannen von Aktionen wie *OK*, *Abbrechen*, *Rotieren*, *Nächste Zeile*.

**Abb. H-6 Zustände**
(Dialogfenster "Zustände" mit Liste von Zuständen)

#### Zustände verwalten

##### So legen Sie einen neuen Zustand an
1. Öffnen Sie den Dialog Zustände.
2. Betätigen Sie [Neu].
3. Geben Sie eine eindeutige *Zustandsnummer* und einen *Namen* ein.
4. Geben Sie eine *Beschreibung* und *Text für Listen* ein.
5. Geben Sie die 9-stellige *Barcode*-Nummer ein.
6. Wählen Sie den *Zustandstyp*.
7. Aktivieren Sie ggf. *AWRack-Info* und wählen den *AWRack-Status*.
8. Klicken Sie auf [Speichern].

##### So löschen Sie einen Zustand
1. Öffnen Sie den Dialog Zustände.
2. Wählen Sie den zu löschenden Zustand aus.
3. Betätigen Sie [Löschen] und bestätigen Sie mit [Ja].

##### So nehmen Sie Änderungen an Zustandsdaten vor
1. Öffnen Sie den Dialog Zustände.
2. Wählen Sie den zu ändernden Zustand aus.
3. Betätigen Sie [Ändern].
4. Nehmen Sie die Änderungen vor und klicken Sie auf [Speichern].

---

### Datenerfassung

In diesem Themenblock lernen Sie, auf welche Art und Weise und an welchen Stellen in der Produktion Daten erfasst werden.
- "Scanner" auf Seite H-946
- "Barcodes" auf Seite H-949

#### Scanner

**Lernziele**
- Unterschiedliche Scanner kennenlernen.
- Die Funktionsweise kennenlernen und verstehen.
- Die Konfiguration der Scanner kennenlernen.

**Nutzen**
Die Verwendung von Scannern trägt zu einer enormen Arbeitserleichterung bei und spart Zeit.

**Definitionen**
- **Online Scanner**: Besitzen keinen Speicher, Scandaten müssen direkt weitergeleitet werden.
- **Offline Scanner**: Verfügen über einen Speicher, der die gescannten Daten zwischenspeichern kann.
- **Serielle Scanner**: Werden u. a. an Terminals eingesetzt, speichern keine Informationen zwischen.

**Merke**
- **Konfiguration**: Scanner benötigen neben ihrem Betriebssystem eine Software, die die gewünschten Funktionen ausführt.

#### Scanner-Typen
Grundsätzlich wird zwischen Online- und Offline-Scannern unterschieden. Die Auswahl hängt von Faktoren ab wie:
- Anzahl der Scanner und Protokolle
- Einsatzort
- Aktionsradius

**Online-Scanner**
Gehören die Linienscanner bzw. serielle Scanner, die Scandaten direkt weiterleiten müssen. Ist die Verbindung unterbrochen, gehen die Daten verloren.

**Denso-Scanner (WLAN)**
Diese Scanner sind WLAN-fähig und kommunizieren direkt mit AWPort. Sie besitzen ein Display und einen Zwischenspeicher. Wird die Datenübertragung unterbrochen, werden die Daten im Scanner zwischengespeichert und bei der nächsten Verbindung übertragen. Diese Scanner kommen u. a. im Versand zum Einsatz.

**Abb. H-7 Denso Online-Scanner**

**Serielle Scanner**
Kommen an Production Terminals oder mit AWPort-Light zum Einsatz. Sie sind robust und günstig, haben aber kein Display und keinen Zwischenspeicher.

**Offline-Scanner**
Der Einsatz unterliegt besonderen Restriktionen. Die Barcode-Lesungen werden erst gesammelt und später manuell übertragen. Dies erfordert eine strukturierte und disziplinierte Arbeitsweise.

**Konfiguration der Scanner**
Die Konfiguration erfolgt mehrschichtig. Die Software wird von A+W zur Verfügung gestellt und auf dem Scanner konfiguriert. Außerdem müssen die Scanner am A+W Production-System angemeldet werden.

> **Scanner in der Praxis**: Aktuell werden fast ausschließlich WLAN-Scanner vom Typ BHT800BW eingesetzt, da die erfassten Daten immer online zur Verfügung stehen.
> **Dokumentation der Konfiguration**: Eine kundenindividuelle Konfigurationsdoku wird in der Projektierungsphase erstellt und gepflegt.

#### Barcodes
Scanner benötigen als Eingaben in der Regel Barcodes. Jede Person, Erfassungsstelle, Gestell etc. erhält eine eindeutige Nummer, die als Barcode kodiert wird. Diese Nummern werden in der Projektierungsphase festgelegt. Benötigen Sie neue Barcodes, starten Sie den Report von A+W Production und drucken die gewünschten Barcodes aus.

---

### Buchungsbeispiele

In diesem Themenblock lernen Sie, wie richtig gebucht wird.
- "Die Reihenfolge des Scannens" auf Seite H-951
- "Scannen von Einheiten" auf Seite H-953
- "Scannen im Versand" auf Seite H-955
- "Erfassungsstellen scannen" auf Seite H-957
- "Gestelle bzw. Kisten scannen" auf Seite H-963
- "Status scannen" auf Seite H-965
- "Korrigieren von Fehlbuchungen" auf Seite H-966

#### Die Reihenfolge des Scannens
Die folgenden Beispiele geben einen Überblick über die einzuhaltende Reihenfolge.

##### Die Reihenfolge beim Scannen:
1.  **Mitarbeiter**: Der Mitarbeiter scannt seinen persönlichen Barcode zu Beginn. Diese Information wird zu jedem Scannvorgang gespeichert.
2.  **Erfassungsstelle**: Die Erfassungsstelle (Bereich, Maschine, Lkw), an der der Scanner eingesetzt wird, muss dem Scanner immer aktuell bekannt sein.
3.  **Gestell (Kiste)**: Das Gestell, auf das Einheiten abgestellt werden, muss gescannt, d.h. am Scanner angemeldet werden. Ausnahme: Im Versand werden Einheiten auch direkt auf die Erfassungsstelle (Lkw) gebucht.
4.  **Einheiten**: Nachdem die Punkte 1-3 gescannt wurden, werden die Einheiten gescannt.

> **Erläuterung**: `<Text>` in spitzen Klammern bezeichnet den zu scannenden Barcode.
> **Achtung beim Barcode `<Beginn>`**: Der Barcode `<Beginn>` setzt das Gestell/Lkw BDE-seitig immer auf leer (Reset)! Befanden sich BDE-seitig noch Einheiten darauf, werden diese der Erfassungsstelle *Fehlergestell (Error-Rack)* zugewiesen.

#### Scannen von Einheiten

##### So scannen Sie eine Einheit auf ein leeres Gestell (Gestell wird BDE-seitig geleert)
1. Melden Sie ein leeres Gestell am Scanner an: `<Beginn> <Gestell>`
2. Scannen Sie das Etikett der Einheit: `<Einheit 1>`, `<Einheit 2>`, ...

##### So scannen Sie eine Einheit auf ein Gestell, auf dem bereits Einheiten stehen
`<Gestell> <Einheit 1> <Einheit 2> <Einheit ...>`

##### So scannen Sie Bruchmeldung Einheiten
`<Bruch> <Einheit 1> <Bruch> <Einheit 2> <Bruch> <Einheit ...>`

##### So scannen Sie Auslieferung Einheiten
`<Ausgeliefert> <Einheit 1> <Ausgeliefert> <Einheit 2> <Ausgeliefert> <Einheit ...>`

##### So scannen Sie Einheiten auf eine leere Erfassungsstelle: Sonderfall LKW
`<Beginn> <ErfStelle> <Einheit 1> <Einheit 2> <Einheit ...>`

##### So scannen Sie Einheiten auf eine Erfassungsstelle, die bereits Einheiten enthält
`<ErfStelle> <Einheit 1> <Einheit 2> <Einheit ...>`

#### Scannen im Versand

Dem Versand muss BDE-seitig besondere Aufmerksamkeit geschenkt werden. Hier kommen in der Regel Denso Online-Scanner zum Einsatz.

##### Grundsätzliche Vorgehensweise:
1. Scannen Sie zunächst den Name-Tag: `<Schmidt>`
2. Melden Sie die Erfassungsstelle am Scanner an: `<Versand Bereich>`
3. Scannen Sie das Gestell, auf das die Einheiten gestellt werden sollen: `<Gestell 1>`
4. Scannen Sie das Etikett der Einheit: `<Einheit 1>`, `<Einheit 2>`, ...

> **Hinweis**: Achten Sie auf die Reihenfolge des Scannens, wenn Sie Einheiten und Gestelle/Kisten in einer beliebigen Reihenfolge laden wollen bzw. müssen!

#### Erfassungsstellen scannen

Jede Erfassungsstelle (Zuschnitt, ISO-Linie, Ofen, Versand, Lkw, etc.) hat einen eigenen Barcode.

##### So scannen Sie Einheiten auf eine leere Erfassungsstelle (Sonderfall LKW)
1. Melden Sie eine neue Erfassungsstelle am Scanner an: `<Beginn> <ErfStelle>`
2. Scannen Sie das Etikett der Scheibe/Einheit.

##### So scannen Sie Einheiten auf eine Erfassungsstelle:
1. Melden Sie die Erfassungsstelle am Scanner an: `<ErfStelle>`
2. Scannen Sie das Etikett der Scheibe/Einheit: `<Einheit 1> <Einheit 2> <Einheit ...>`

##### So scannen Sie Einheiten auf verschiedene Erfassungsstellen:
`<ErfStelle 1> <Einheit 1> <Einheit 2>`
`<ErfStelle 3> <Einheit 3> <Einheit 4> <Einheit 5>`
`<ErfStelle 1> <Einheit 6>`
...

##### So scannen Sie Gestelle auf eine Erfassungsstelle:
`<ErfStelle> <Gestell 1> <Gestell 2> <Gestell ...>`

##### So scannen Sie Gestelle auf verschiedene Erfassungsstellen:
`<ErfStelle 1> <Gestell 1> <Gestell 2>`
`<ErfStelle 2> <Gestell 3>`
...

##### So scannen Sie eine Erfassungsstelle fertig:
`<Fertig> <ErfStelle>`

##### So scannen Sie die Auslieferung Lkw oder Auflieger:
`<Ausgeliefert> <ErfStelle>`

#### Erfassungsstelle LKW

##### Grundsätzliche Vorgehensweise:
1. Scannen Sie den Name-Tag: `<Schmidt>`
2. Melden Sie einen neuen Lkw am Scanner an: `<Beginn> <Lkw 1>`
3. Oder melden Sie einen teilbeladenen Lkw am Scanner an: `<Lkw 2>`
4. Scannen Sie das Etikett der Einheit.

##### Übung 1: Beladen eines leeren und eines teilbeladenen LKW
Lkw 1 (leer) und Lkw 2 (teilbeladen) sollen beladen werden.

1. Lkw 1 (ES) am Scanner anmelden: `<Beginn> <Lkw1>`
2. Einheiten direkt auf Lkw 1 buchen: `<Einheit 1> <Einheit 2> <Einheit 3>`
3. Gestelle auf Lkw 1 buchen: `<Gestell 1> <Gestell 2>`
4. Lkw 1 erneut anmelden (letztes Gestell wird abgemeldet): `<Lkw1>`
5. Einheiten direkt auf Lkw 1 buchen: `<Einheit 4> <Einheit 5>`
...
16. Beladung von Lkw 1 abschließen: `<Ausgeliefert> <Lkw1>`
... (Beladung von LKW 2 folgt analog)

> **Hinweis**: Schließen Sie das Beladen eines Lkw immer mit der Statusbuchung `<Ausgeliefert> <Lkw>` ab.

#### Gestelle bzw. Kisten scannen

Voraussetzung: Der Name des Mitarbeiters und die aktuelle Erfassungsstelle muss gescannt sein.

##### So scannen Sie eine Einheit auf ein leeres Gestell (Gestell wird BDE-seitig geleert)
1. Scannen Sie ein leeres Gestell: `<Beginn> <Gestell>`
2. Scannen Sie das Etikett der Einheit.

##### So scannen Sie ein Versandgestell fertig
`<Fertig> <Gestell 1> <Fertig> <Gestell 2> ...`

##### So scannen Sie die Auslieferung Gestelle/Versandgestelle
`<Ausgeliefert> <Gestell 1> <Ausgeliefert> <Gestell 2> ...`

##### So scannen Sie Gestelle auf den LKW
`<ErfStelle> <Gestell 1> <Gestell 2> <Gestell ...>`

#### Status scannen
Das Scannen eines Statusbarcodes setzt zahlreiche Aktivitäten in Gang. Der Status muss immer vor dem Objekt (Gestell, Einheit, etc.) gescannt werden.

##### So scannen Sie den Status Bruchmeldung Einheiten
`<Bruch> <Einheit 1> <Bruch> <Einheit 2> ...`

##### So scannen Sie den Status Auslieferung Einheiten
`<Ausgeliefert> <Einheit 1> <Ausgeliefert> <Einheit 2> ...`

##### So scannen Sie den Status Auslieferung mehrere Gestelle
`<Ausgeliefert> <Rack 1> <Ausgeliefert> <Rack 2> ...`

##### So scannen Sie den Status Auslieferung Lkw/Auflieger (und Start der Triggerzeit)
`<Ausgeliefert> <RegPoint>`

##### So melden Sie ein leeres Gestell an (wird BDE-seitig geleert)
`<Beginn> <Gestell>`

##### So melden Sie eine leere Erfassungsstelle an (Sonderfall Lkw)
`<Beginn> <ErfStelle>`

> **Bei mehrfach einscannen von `<Status>`**: Wurde mehrfach der Status hintereinander gescannt `<Status1><Status2><Objekt>`, wird der letzte gescannte Status auf das Objekt angewendet.

#### Korrigieren von Fehlbuchungen
Fehlbuchungen können grundsätzlich durch eine neue, korrekte Buchung korrigiert werden. Die zusätzliche Buchung wird in der Buchungshistory festgehalten, hat aber außer der Korrektur keine weiteren Auswirkungen.

**Beispiel**: Wurden Einheiten irrtümlich auf ein Gestell und nicht auf die Erfassungsstelle gebucht, kann dieser Fehler durch Scannen der Erfassungsstelle und anschließendem Scannen der Einheit rückgängig gemacht werden: `<ErfStelle> <Einheit 1> <Einheit 2> ...`

---

### Production Terminals

Dieser Themenblock verschafft Ihnen einen groben Überblick zu den verschiedenen Production Terminals.

**Lernziele**
- Unterschiedliche Terminals kennenlernen.
- Die Funktionsweise kennenlernen und verstehen.

**Nutzen**
Die Production Terminals helfen Ihnen, die Scheiben einer Einheit in der korrekten Reihenfolge vom Gestell der Produktion (z. B. Linie) zuzuführen.

**Definitionen**
- **Production Terminal IG**: Kommt an der ISO-Linie zum Einsatz.
- **Production Terminal TG**: Kommt an der ESG-Linie zum Einsatz.
- **Production Terminal LG**: Kommt an der VSG-Linie zum Einsatz.
- **Production Terminal Order**: Einsatzort, wo größere Mengen gebucht werden.
- **Production Terminal Manual Cutting**: Visualisiert am Handzuschnitttisch den Arbeitsplan.
- **Production Terminal Processing**: Kommt an den Bearbeitungsmaschinen zum Einsatz.
- **Production Terminal Edit**: Kommt im Versandbüro zum Einsatz.

**Merke**
- **Voraussetzung**: Ein installierter Barcode Manager (A+W Production).

#### Einführung
Bei den Production Terminals handelt es sich um Leitrechner für unterschiedliche Arbeitsstationen. Typische Einsatzorte sind:
- Zuschnitt
- ISO-Linie
- ESG-Ofen
- VSG-Linie
- Versand

Leitrechner visualisieren und steuern einzelne Prozessschritte und sind individuell konfigurierbar. Sie ermöglichen Online-Druck von Etiketten und Reports, Erfassung von Bruchscheiben und bieten eine einfache Handhabung.

**Abb. H-8 Überblick Production Terminals**
(Schematische Darstellung einer AWP-Landschaft mit verschiedenen Terminals)

**Kurze Erläuterung zu den einzelnen Production Terminals:**
- **Terminal Manual Cutting**: Visualisiert am Handzuschnitttisch den Arbeitsplan.
- **Terminal Order**: Kommt überall dort zum Einsatz, wo größere Mengen gebucht werden.
- **Terminal Processing**: Steuert Bearbeitungsmaschinen automatisch an.
- **Terminal IG-In**: Visualisiert am Einlauf der Isolierglaslinie den Arbeitsplan.
- **Terminal IG-Assembly**: Visualisiert technische Daten zwischen Waschmaschine und Rahmensetzstation.
- **Terminal IG-Out**: Visualisiert am Auslauf der Isolierglaslinie technische und versandorientierte Daten.
- **Terminal TG-In**: Anzeigesystem am Ofeneinlauf; zeigt Belegung des Ofenbettes.
- **Terminal TG-Out**: Anzeigesystem am Ofenauslauf; zeigt registrierte Scheiben.
- **Terminal Edit**: Variante im Versandbüro zum Umbuchen von Einheiten/Gruppen.
- **Terminal LG-In**: Visualisiert am Einlauf der VSG-Linie den Arbeitsplan.
- **Terminal LG-Assembly**: Visualisiert im Reinraum den Arbeitsplan.

> **Production Terminals**: Detaillierte Informationen zu den einzelnen Terminals entnehmen Sie bitte dem Handbuch *Production Terminal*.

---

### Bruchmanagement

In diesem Themenblock lernen Sie den Umgang mit zu Bruch gegangenen Scheiben.

#### Überblick

**Lernziele**
- Den Umgang mit Brüchen kennenlernen.

**Nutzen**
Es sind keine manuellen Eingaben nötig. Dadurch werden die Bruchscheiben schneller nachgeschnitten.

**Definitionen**
- **Bruchpool**: Im globalen Bruchpool finden Sie eine Übersicht der Bruchscheiben.

**Merke**
- **Bruchmeldung**: Erfolgt an jedem Production Terminal oder per Scanner.
- **Etiketten**: Der Etikettendruck erfolgt automatisch an einem zentralen Drucker.
- **Automatischer Nachschnitt**: Findet auf dem Restblatt oder durch eine Tischoptimierung im A+W Realtimeoptimizer statt.

#### Bruchbehandlung (intern)
Werden Einheiten als Bruch gemeldet, werden dadurch verschiedene interne Aktionen ausgelöst. In der Datenbank werden Informationen über die Ursprungs-Einheit sowie alle Nachläufer gespeichert. Nachläufer erhalten immer die Ursprungs-Barcode-Nummer, versehen mit einem Index.

**Tab. H-1 BDE-Bruchbehandlung**
| Barcode | Erfassungsstelle | Gestell | Bruch | Nachläuferindex | Erklärung |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 012345678 | Bohren | 15 | 0 | 0 | E1: Ursprungsscheibe |
| 012345678 001 | Bohren | 15 | 1 | 0 | E2: Bruch 1 gemeldet |
| 012345678 | - | - | 0 | 1 | E3: Nachläufer 1 erzeugt |
| 012345678 002 | Ofen | 20 | 1 | 1 | E4: Nachläufer 1 als Bruch 2 gemeldet |
| 012345678 | - | - | 0 | 2 | E5: Nachläufer 2 erzeugt |

> **Hinweis**: Beim Druck der Etiketten für die Nachläufer bzw. beim Reporting können die Werte und Flags ausgewertet und berücksichtigt werden.
> **Tipp**: In A+W Production können Filter verwendet werden. Standardfilter zeigen ggf. Einheiten mit Nachläuferindex nicht an. Zum Anzeigen dieser Einheiten deaktivieren Sie alle Filter.
> **Ansichten und Filter**: Weitere Informationen entnehmen Sie bitte dem A+W Production-Handbuch.

---

### Statistik, Reporting und Monitoring

In diesem Themenblock lernen Sie die Berichte und die unterschiedlichen Auswertungen kennen.
- "BDE-Reporting" auf Seite H-978
- "Monitoring: A+W Dashboard" auf Seite H-983
- "Statistik: A+W Discovery" auf Seite H-987

#### BDE-Reporting

Bei den hier beschriebenen Reports handelt es sich um die Standard-Barcode-Reports. Kundenindividuelle Anpassungen sind möglich.

> **Hinweis**: Allgemeingültige Reports, die Auswertungen auf eine Erfassungsstelle darstellen, zeigen in der Regel alle Einheiten an, die dieser Erfassungsstelle zugeordnet waren! Für spezifische Auswertungen (z.B. Durchsatz einer Linie) müssen angepasste Reports zur Anwendung kommen.

**Aufruf der Reports**
Alle Reports können über die A+W Production-Menü-Struktur aufgerufen werden.

**Beispiele der Standard-Barcode-Reports**

- **Abstellliste** (Listen > Abstellliste): Zeigt alle Teile an, die in einer einheitengenauen AWP-Ansicht ausgewählt werden.
- **Auftragsübersicht** (Listen > Auftragsliste): Zeigt an, wo sich die einzelnen Positionen (Kopfteile) des Auftrags befinden.
- **Auftragsstatus** (Listen > Auftragsstatus): Gibt Auskunft über den Status des Auftrags.
- **Ladeliste** (Listen > Ladeliste): Zeigt die tatsächlichen Beladungen.
- **Gestellbelegung pro Scheibe** (Listen > Gestellbelegung pro Scheibe): Zeigt für eine Gestellnummer die Belegung pro Scheibe.
- **Gestellbelegung pro Position** (Listen > Gestellbelegung pro Position): Zeigt für eine Gestellnummer die Belegung pro Position.
- **Buchungshistorie** (Listen > Buchungshistorie): Zeigt pro Auftrag, welche Buchungen an welcher Stelle stattgefunden haben.

#### Monitoring: A+W Dashboard

**Lernziele**
- Kurze Einführung in A+W Dashboard.
- Die Möglichkeiten kennenlernen.

**Nutzen**
A+W Dashboard zeigt wichtige Kennzahlen von den entscheidenden Stellen der Produktion an und sorgt damit für hohe Transparenz.

**Definitionen**
- **Ampel**: Zeigt den aktuellen Status einer Erfassungsstelle an.

**Merke**
- **Zeitraum**: Zur Auswertung wird in der Regel ein Zeitraum von max. 24 Stunden berücksichtigt.
- **Korrekte Darstellung**: Voraussetzung sind lückenlose AWP-Buchungen.
- **Anzeige**: Kann auf großen Monitoren oder mobilen Endgeräten wie Smartphones erfolgen.
- **Störungen**: Bei Störungen kann die Situation exakt kommuniziert werden.

**Überblick**
A+W Dashboard zeigt wichtige Kennzahlen der Produktion in Echtzeit an (Nutzungsgrad, Maschinenstatus, Produktivität). Das Programm ist browserbasiert und kann auf diversen Endgeräten angezeigt werden. Es dient als Online-Monitoring-Tool und Entscheidungsmittel. Die Auswertungen werden auf verschiedene Arten visualisiert:

- **A - Ampel**: Für Statusanzeigen über sehr kurze Zeiträume.
- **B - Kreis (Kuchen)**: Zeigt Anteile der Maschinenstatus über einen definierten Zeitraum (z.B. 24h).
- **C - Punktediagramm**: Zeigt Buchungen eines vergangenen Zeitraums verteilt an.
- **D - Balkendiagramm**: Stellt statistische Daten dar, die über SQL-Abfragen erhoben wurden.
- **E - Tacho**: Zeigt die aktuelle Auslastung (Stückzahlen der letzten Stunde).

> **A+W Dashboard**: Detaillierte Informationen entnehmen Sie bitte dem Handbuch A+W Dashboard.

#### Statistik: A+W Discovery

**Lernziele**
- Kurze Einführung in A+W Discovery.
- Die Möglichkeiten kennenlernen.

**Nutzen**
Mit A+W Discovery werden unternehmensübergreifende Daten zusammengeführt, aufbereitet und angezeigt.

**Definitionen**
- **Pivot Tabelle**: Spezielle Art von Tabellen, die Daten auf verschiedene Arten darstellen.
- **Fiskaljahr**: Geschäftsjahr eines Unternehmens.

**Merke**
- **A+W Discovery**: Bietet die Möglichkeit, langfristige Auswertungen von Produktionsdaten zu erstellen.
- **Auswertungen**: Können leicht über Microsoft Excel in Form von Pivot-Tabellen erstellt werden.
- **Datenbereitstellung**: Kann Daten aus ERP- (A+W Enterprise, A+W Business) und PPS-Systemen (A+W Production) bereitstellen.
- **Mandantenübergreifende Auswertungen**: Können erstellt werden.

**Überblick**
A+W Discovery ist das moderne Business Intelligence System von A+W. Es erlaubt, statistische Kennzahlen und Messgrößen aus verschiedenen Blickrichtungen zu betrachten (z.B. Deckungsbeitrag nach Standort/Monat) und daraus strategische Entscheidungen abzuleiten. Es ist möglich, produktive Kennzahlen wie Anzahl Bruchscheiben je Arbeitsstation oder Maschinenstillstandszeiten über einen definierten Zeitraum auszuwerten.

**Abb. 10 A+W Discovery**
(Beispiel-Dashboards in Excel mit Pivot-Tabellen und -Charts zu Ausschuss, produzierten Mengen, etc.)

> **A+W Discovery**: Detaillierte Informationen zu diesem Modul entnehmen Sie bitte dem Handbuch A+W Discovery.

---

# Softwarereferenz

### Übersicht Stammdaten

Im Menü Stammdaten > BDE befinden sich folgende Programmpunkte (Punkte werden durch A+W Software GmbH gepflegt, sofern nicht anders vermerkt):
- **Barcode-Optionen**
- **Barcode-Typen**
- **Erfassungsstellen-Typen**
- **Erfassungsstellen**: Sie verwalten Ihre Erfassungsstellen.
- **Gestelle**: Sie verwalten Ihre Gestelle.
- **Gestellfilter**: Sie definieren Gestellfilter.
- **Zustandstypen**
- **Zustände**: Sie verwalten die Zustände.
- **Personal**: Sie verwalten Ihr Personal.
- **Spaltenzuordnung**
- **Spalten**
- **BDE Nachbearbeitung**: Falls bei der Verarbeitung der Daten Probleme aufgetreten sind.

#### Barcode-Optionen
**Abb. H-1 Barcode-Optionen**
(Dialogfenster Barcode-Optionen)
> **Systemkritische Daten**: Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert. Bitte nehmen Sie hier keine Veränderungen vor.

#### Barcode-Typen
**Abb. H-2 Barcode-Typen**
(Dialogfenster Barcodetypen)
> **Systemkritische Daten**: Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert.

#### Erfassungsstellen-Typen
**Abb. H-3 Erfassungsstellen-Typen**
(Dialogfenster Erfassungsstellentypen)
> **Systemkritische Daten**: Dieser Bereich wird komplett durch die A+W Software GmbH angelegt und bei Bedarf geändert.

#### Erfassungsstellen

**Abb. H-4 Erfassungsstellen**
(Dialogfenster Erfassungsstellen)

In diesem Dialog legen Sie neue Erfassungsstellen an oder nehmen Änderungen vor.

**Erläuterung der Felder**
- **Erfassungsstellennr**: Nummer der Erfassungsstelle.
- **Barcode**: Barcode der Erfassungsstelle.
- **Name**: Name der Erfassungsstelle.
- **Beschreibung**: Ausführliche Beschreibung.
- **Text für Produktionslisten / Kundenlisten**: Texte für Listen.
- **Unterzeile für Barcodeetiketten**: Text unterhalb des Barcodes.
- **Erfassungsstellentyp**: Weist der ES einen Typ zu.
- **Gruppierung / Gruppierung für Arbeitsschichten**: Dient der Zusammenfassung für Auswertungen.
- **Aktueller Zustand**: Weist der ES einen aktuellen Zustand zu.
- **Restriktionen**: Aktiviert/deaktiviert die Restriktionsprüfung.
  - 0: Ausgeschaltet.
  - 1: Bezieht sich auf technische Produktionsmenge.
  - 2: Bezieht sich auf verfügbare Menge (direkt vorgelagerter Prozess abgeschlossen).
  - 3: Bezieht sich auf verfügbare Menge (alle vorgelagerten Prozesse abgeschlossen).
- **Mengenüberschreitung**: Gibt in Prozent an, um wie viel eine Startmenge überbucht werden darf.
- **Produzierte Teile anzeigen**: Steuert, ob komplett produzierte Teile im Production Terminal angezeigt werden.

