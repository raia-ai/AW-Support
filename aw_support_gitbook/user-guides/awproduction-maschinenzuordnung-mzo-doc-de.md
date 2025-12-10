---
title: "DE_AWProduction_MZO_2.10"
source: "DE_AWProduction_MZO_2.10.pdf"
tags: ["A+W Production", "Maschinenzuordnung", "MZO", "Glass Manufacturing", "Window Production", "Door Production", "ERP", "Software Tutorial", "Software Reference", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A German-language user manual for the A+W Production 'Maschinenzuordnung' (MZO) module, version 2.10. This document provides both a tutorial and a software reference for assigning work operations to machines in glass, window, and door manufacturing."
long_description: "This document is the official user guide for the 'Maschinenzuordnung' (MZO - Machine Assignment) module within the A+W Production software suite, specifically for version 2.10, released in November 2018. Written in German, it serves as a comprehensive resource for users responsible for production planning and data management in the glass, window, and door manufacturing industries. The manual is divided into two main parts: a 'Tutorial' and a 'Softwarereferenz' (Software Reference). The tutorial section offers a step-by-step guide to understanding the core concepts of machine assignment, including the creation and management of physical machines, logical machines, work operations (Arbeitsgänge), and processing types. It explains how to define restrictions, conditions, and formulas to optimize production flow and capacity planning. The software reference section provides detailed descriptions of every dialog, field, and function within the MZO-Editor, serving as a quick reference guide for experienced users. The document covers key concepts like mapping the physical machine park, defining machine properties, assigning work operations to logical machines, and setting priorities to manage production bottlenecks effectively."
---

# A+W Maschinenzuordnung

**A+W Production**

A+W - Software for Glass, Windows and Doors

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Maschinenzuordnung Version / Datum | Beschreibung |
| :--- | :--- |
| 2.10 / 11-2018 | Kapitel zu Maschinentyp neu. Screenshots aktualisiert. |
| 2.02 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 2.01 / 01-2013 | Layout an CI 2013 angepasst. |
| 2.00 / 09-2012 | Neuerstellung Tutorial, Überarbeitung Softwarereferenz. |
| 1.00 / 01-2003 | Ersterstellung. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen
*   Kontakte

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbau-stufe von A+W Production.

### Urheberrechte

© 2018, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte

**A+W Software GmbH**
Am Pfahlgraben
D-35415 Pohlheim
📞 +49 6404 2051 0
📠 +49 6404 2051 877
📧 aw.zentrale@a-w.com
🌐 http://www.a-w.com

## Inhalt

*   **Vorspann**
    *   Revisionsübersicht
    *   Editorial
*   **Tutorial**
    *   **Überblick**
        *   Dokumentation
        *   Aufbau des Tutorials
        *   Darstellungskonventionen
    *   **Grundlagen**
    *   **Maschinenzuordnung**
        *   Maschinen
            *   Maschinen in der Maschinenzuordnung
            *   Maschinen anlegen und verwalten
            *   Restriktionen von Maschinen anlegen und bearbeiten
            *   Übungen zu Maschinen
        *   Logische Maschinen
            *   Logische Maschinen in der Maschinenzuordnung
            *   Logische Maschinen anlegen und verwalten
            *   Übungen zu logischen Maschinen
        *   Arbeitsgänge
            *   Arbeitsgänge in der Maschinenzuordnung
            *   Arbeitsgänge anlegen und verwalten
            *   Übungen zu Arbeitsgängen
        *   Arbeitsgangzuordnung
            *   Angepasste Arbeitsgangzuordnung
            *   Arbeitsgänge und logische Maschinen zuordnen
            *   Übungen zur Arbeitsgangzuordnung
        *   Bedingungen, Formeln, Restriktionen
            *   Bedingungen und Formeln in der Maschinenzuordnung
            *   Bedingung auswählen
            *   Formel zur Bearbeitungsdauer einer logischen Maschine auswählen
            *   Übungen zum Auswählen von Bedingungen
        *   Bearbeitungstypen und Bearbeitungsartikel
            *   Bearbeitungstypen in der Maschinenzuordnung
            *   Bearbeitungsartikel in der Maschinenzuordnung
            *   Bearbeitungstypen anlegen und verwalten
            *   Bearbeitungsartikel anlegen und verwalten
            *   Übungen zur Maschinenzuordnung
        *   Schaltflächen in der Maschinenzuordnung
*   **Softwarereferenz**
    *   **Maschinenzuordnung**
        *   MZO-Editor
            *   MZO-Editor - Maschinen
            *   MZO-Editor - Logische Maschinen
            *   MZO-Editor - Arbeitsgänge
            *   MZO-Editor - Arbeitsgangzuordnung
            *   MZO-Editor - Maschinentypen
        *   Neue Maschine
        *   Maschine
        *   Abmessungsrestriktionen
        *   SZR Restriktionen
        *   Bedingung auswählen
        *   Neue logische Maschine
        *   Logische Maschine
        *   Formel-Auswahl
        *   Neuer Arbeitsgang
        *   Arbeitsgang
        *   Neuer Maschinentyp
        *   Maschinentyp
        *   Formeln in der Maschinenzuordnung
            *   Auswahl Bedingungen
            *   Bedingungseditor (grafische Variante)
            *   Neue Bedingung
            *   Info (zur neuen Bedingung)
            *   Auswahl Menge
            *   Bedingungseditor (Text-Variante)
            *   Formel-Editor
        *   Bearbeitungen in der Maschinenzuordnung
            *   Bearbeitungstypen
            *   Bearbeitungsartikel
            *   Spalten anpassen
            *   Spaltendefinition
*   **Partindex**

## Tutorial

### Überblick

Das Tutorial zum Modul Maschinenzuordnung (MZO) beschäftigt sich mit der Zuweisung von Bearbeitungen zu Maschinen in A+W Production. Die Maschinenzuordnung weist die anstehenden Bearbeitungen den einzelnen Maschinen zu und berücksichtigt dabei Maschinenrestriktionen und Vorgaben zur Produktionssteuerung. Mit Prüfprogrammen von Maschinenherstellern kann in A+W Production geprüft werden, ob die Arbeitsgänge plausibel sind.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

**Vorausgesetzte Kenntnisse**

Das Tutorial richtet sich an Teilnehmer, die in A+W Production die Arbeitsvorbereitung verantworten und damit den optimalen Ablauf der Produktion organisieren. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Production kennen.

#### Dokumentation

Für das Modul Maschinenzuordnung stehen folgende Dokumente zur Verfügung:

*   **PDF**
    *   Vollständige Unterlagen
        *   Tutorial
        *   Softwarereferenz
        *   Index
*   **Online-Hilfe <F1>**
    *   Kontextsensitive Dialog-Hilfe

#### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

*   **Überblick**
    Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    *   Lernziele: Was soll vermittelt werden?
    *   Nutzen: Wofür können Sie dieses Wissen einsetzen?
    *   Merksätze: Welche Zusammenhänge müssen Sie sich merken?

*   **Konzepte**
    Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

*   **Übungen**
    Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Neue Maschine*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| **>** | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. **Stammdaten > MZO > MZO-Editor > Maschinen > Neu**. |
| **[]** | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten. |
| **<>** | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit **<F1>** öffnen Sie die Online-Hilfe. |

#### Lesehinweis

Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Grundlagen

Die Maschinenzuordnung stellt die Bezüge zwischen Arbeitsgängen und Maschinen dar. Auf Basis der Maschinen und der Arbeitsgänge kann die Kapazitätsplanung die Aufträge optimal einlasten.

Zum Einrichten der Stamdaten müssen folgende Fragen behandelt werden:
*   Welche Aufgabe muss durch die Bearbeitung an einer Scheibe eines Auftrags erfüllt werden: **Was** ist zu tun.
*   Welche verwendende Methode wird verwendet: **Wie** wird das gemacht.
*   Welches Arbeitsmittel wird verwendet: **Wo** wird die Bearbeitung ausgeführt.
*   Welche Rangfolge und Restriktionen müssen beachtet werden: **Warum** oder **Wann** wird in die Maschine verwendet.

[Image: Abb. D-1: Bestandteile in der Maschinenzuordnung. Ein Flussdiagramm zeigt die Verknüpfung von Maschinentyp, Maschine, logischer Maschine, Bearbeitungstyp, Bearbeitungsartikel und Arbeitsgang. Diese Komponenten werden durch Restriktionen, Eigenschaften und Formeln beeinflusst und münden in die Arbeitsgangzuordnung.]

In dieser schematischen Darstellung sehen Sie, welche Bestandteile zur Maschinenzuordnung gehören und wie sie miteinander verknüpft sind.

Maschinen werden durch einen Maschinentyp, Eigenschaften und Restriktionen definiert. Zum Beispiel ist dem Schneidtisch 8 der Maschinentyp Zuschnitt zugewiesen.

Zu den Eigenschaften von Schneidtisch 8 gehört, dass er der Kostenstelle 25 und der Erfassungsstelle 180 zugewiesen ist. Die logische Maschine zu Schneidtisch 8 heißt logischer Schneidtisch 8. Ihr ist die Formel Ist Modell zugewiesen.

#### Beschreibung der Arbeitsgänge

Mithilfe der Arbeitsgänge werden die Materialströme in der Produktion aufgeteilt und lassen sich separat behandeln. Arbeitsgänge müssen daher zuallererst betrachtet werden.

Bei der Einrichtung der Arbeitsgänge werden um folgende Fragen berücksichtigt:
*   Welche Bearbeitung können zusammengefasst werden und welche dürfen nicht zusammengefasst werden?
*   Gibt es zusätzliche Bearbeitungen die ausgeführt werden, aber nicht in der Stückliste erscheinen?
*   Gibt es ggf. verschiedene Materialströme, z. B. Serienscheiben, Badspiegel, Wohnmobilscheiben, die ganz eigene Wege durch die Produktion gehen und daher früh unterschieden werden sollen?
*   Gibt es ggf. Arbeitsgänge, die gar nicht hier gefertigt werden, z. B. Sandstrahlen am anderen Ende der Stadt?

#### Beschreibung der Maschinen

Indem die Maschinen präzise beschrieben werden, wird gewährleistet, dass zu fertigende Scheiben gültige Maschinen finden. Dabei wird zwischen physikalischen Restriktionen und logischen Maschinen mit zusätzlichen Restriktionen, Kostensätzen und Übergangszeiten unterschieden.

Zur Liste der Maschinen kommen Orte, die zwar keine Maschinen im herkömmlichen Sinne sind, die aber für die Produktion relevant sind, z. B. Lager, Wareneingang, Versandlager, Verladerampe, zusätzliche Produktionsorte.

#### Beschreibung der logischen Maschine

Logische Maschinen werden verwendet, um in der Kapazitätsplanung unterschiedliche Übergangszeiten, Kostensätze oder Bearbeitungsdauern auszudrücken. Als Leitfaden bietet sich an, eigene logische Maschinen einzurichten, wenn eine Maschine in verschiedenen Betriebsarten verwendet werden kann.

### Maschinenzuordnung

In diesem Kapitel erfahren Sie, welche Bereiche von A+W Production zur Maschinenzuordnung (MZO) gehören und wie Sie Maschinen zuordnen.

Mithilfe des MZO-Editors verwalten Sie Maschinen, logische Maschinen und Arbeitsgänge, deren Zuordnung und Eigenschaften.

Zur Maschinenzuordnung gehören folgende Kapitel:
*   "Maschinen"
*   "Logische Maschinen"
*   "Arbeitsgänge"
*   "Arbeitsgangzuordnung"
*   "Bedingungen, Formeln, Restriktionen"
*   "Bearbeitungstypen und Bearbeitungsartikel"

In den folgenden Lerneinheiten lernen Sie zunächst Maschinen, logische Maschinen, Arbeitsgänge und die Arbeitsgangzuordnung kennen. Diese Kenntnisse werden anschließend durch die Themen Bearbeitungstypen und Formelauswahl vertieft.

### Maschinen

**Lernziele**
*   Was sind Maschinen in A+W Production und speziell in der Maschinenzuordnung.
*   Wie werden Maschinen verwaltet, neu angelegt, bearbeitet oder gelöscht.
*   Wie werden Namen und Nummern sinnvoll vergeben.

**Nutzen**
*   Mit Maschinen wird der physikalische Maschinenpark abgebildet. Somit bilden Maschinen die Basis, um die Produktion zu steuern.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Maschinen** | Maschinen bilden die physikalischen Maschinen im Maschinenpark ab. Namen und Nummern werden in A+W Production systematisch vergeben. |
| **Maschinentypen** | Die Maschinentypen sind in A+W Production bereits definiert und werden Maschinen zugewiesen. Mit Maschinentypen wird definiert, um welchen Typ einer Maschine es sich handelt, zum Beispiel Zuschnitt, Rahmenbieger oder Sonstige. |
| **Verknüpfungen** | UND-/ODER-Verknüpfungen sind die Operatoren, mit denen in A+W Production Restriktionen, Bedingungen und Formeln verknüpft werden. |
| **Schnitte** | Z- und W-Schnitte sind aufwendigere Schnitte, denen ein zusätzlicher Kostenfaktor Kosten pro Z-Schnitt zugewiesen werden kann. |

> **Voraussetzung**
> Um eine Maschine in A+W Production anlegen zu können, muss der passende Maschinentyp definiert sein. Der Maschinentyp wird im Dialog *Neue Maschine* ausgewählt.
> Ist im Dialog *Neue Maschine* der entsprechende Maschinentyp nicht verfügbar, wenden Sie sich bitte an die A+W Software GmbH.

#### Maschinen in der Maschinenzuordnung

In dieser Einheit lernen Sie, wie Sie Ihren Maschinenpark in A+W Production abbilden und welche Eigenschaften den Maschinen zugeordnet werden.

[Image: Abb. D-2 MZO-Editor - Maschinen. Screenshot des MZO-Editors, der eine Liste von Maschinen mit ID, Name, Typ und Erfassungsstelle anzeigt.]

Im Register **Maschinen** sind alle physikalischen Maschinen gelistet. Das Register **Maschinen** bildet somit Ihren realen Maschinenpark ab.

Jede Maschine ist durch eine ID eindeutig identifizierbar. Zu jeder Maschine gehört eine Erfassungsstelle für die Erfassung der Betriebsdaten (BDE). Sie ordnen jeder Maschine einen Maschinentyp zu, der festlegt, um welchen technischen Typ es sich handelt, zum Beispiel Zuschnitt, CNC-Center oder Sprossenbau. Die Maschinentypen sind fest definiert und können nicht geändert werden. A+W Production legt zu jeder Maschine automatisch eine logische Maschine an.

Sie müssen also zu jeder real existierenden Maschine im Maschinenpark eine Maschine in A+W Production anlegen und die Eigenschaften definieren.

[Image: Abb. D-3 Maschinen in A+W Production. Ein Diagramm, das den Maschinenpark (links) der Abbildung in A+W Production (rechts) gegenüberstellt. Es zeigt, dass Schneidtisch 1 & 2 und CNC-Maschine 1 & 2 abgebildet sind, aber Bohrmaschine 2 aus dem realen Park in der Software fehlt.]

In diesem Beispiel ist zur Bohrmaschine 2 keine Maschine in A+W Production angelegt. Damit ist die Maschine der Software nicht bekannt und kann auch nicht angesteuert werden.

#### Maschineneigenschaften

Für jede in A+W Production angelegte Maschine müssen die folgenden Eigenschaften der Maschine festgelegt werden.
*   **Handbetrieb:** Kennzeichen für Maschinen, die nicht über automatische Ladeeinrichtungen verfügen. Dieses Kennzeichnen verhindert u.a. dass anhand der manuellen Bearbeitungsdauer gesplittet wird oder dass Positionen automatisch auf Handzuschnittstische eingelastet werden.
*   **Einzelbearbeitung:** Kennzeichen für Maschinen, deren Bearbeitungen nicht zusammengefasst werden dürfen, z. B.
    *   Bohrungen = 0: für zwei Bohrungen auf derselben Maschine werden nicht zwei Termine ermittelt.
    *   Siebdrucke oder Beschichtungen = 1: für zwei Beschichtungen werden nicht zwei verschiedene Termine ermittelt, auch wenn sie auf derselben Maschinen gemacht werden.
*   **Mindestgröße:** Mindestabmessungen für eine Scheibe, die auf der Maschine gefertigt werden kann, ohne z. B. durch die Rollen zu fallen. Wenn Sie zu kleine Scheiben auf eine größere Scheibe legen können, z. B. um sie zu bedrucken, legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den logischen Maschinen, z. B. als Siebdruck mit Trägerscheibe.
*   **Maximalgröße:** Maximale Abmessungen für eine Scheibe, die der Maschine gefertigt werden kann, weil sie die Breite der Führungsschienen, die Ofenbreite oder die Deckenhöhe überschreitet. Wenn Sie größere Scheiben fertigen können, indem Sie z. B. am Bearbeitungszentrum die Seitenwände abschrauben und Spritzschutz aufstellen, legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den logischen Maschinen, z.B: als Bearbeitungszentrum für Übergrößen.
*   **Dicken:** Dickenbereich, in dem die Maschine arbeiten kann. Anderen Dicken können nicht auf der Maschine bearbeitet werden, z. B. weil 3 mm nicht zuverlässig unterstützt werden und für 15 mm die Führungen zu schmal sind. Wenn eine 15 mm Scheibe gefertigt werden kann, indem Sie die Maschine umbauen, legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den logischen Maschinen, z. B. Schleifmaschine für Dickgläser.
*   **Modelle:** Angabe, ob die Maschine ausschließlich Rechtecke, ausschließlich Modelle oder beides fertigen kann. Berücksichtigen Sie ggf. dass Freiformen oder Rundbögen nicht gefertigt werden können, z. B. bei VSG-Zuschnitt.
*   **Gewicht:** Maximalgewicht einer Scheibe, für das die Maschine zugelassen ist. Um auszudrücken, dass die Maschine das Gewicht zwar verarbeiten kann, hierfür aber ein zweiter Mitarbeiter zum Handling bereitstehen muss, geben Sie die Restriktion bei den logischen Maschinen an, z. B. Einseiter mit zwei Personen.

> **Maschine löschen**
> Das Löschen einer Maschine kann Auswirkungen auf die Produktion haben. Vergewissern Sie sich, dass die Maschine in der Produktion nicht mehr verwendet wird, bevor Sie sie löschen.

#### Namen, IDs und Nummern vergeben

Vergeben Sie für Maschinen des gleichen Typs IDs im gleichen Hunderter-Bereich, zum Beispiel für alle Schneidtische IDs zwischen 100 und 199. Damit sind in der Liste Schneidtische sofort erkennbar. Wenn Sie keine eigenen Nummernkreise für Betriebsmittel haben, orientieren Sie sich am Nummerierungsschema der Betriebsdatenerfassung.

Vergeben Sie für Maschinen des gleichen Typs gleiche Namen und nummerieren Sie diese durch, z. B. bekommt der achte Schneidtisch im Maschinenpark den Namen Schneidtisch 8.

#### Maschinenrestriktionen

Maschinen können bauartbedingt verschiedene Restriktionen haben, z. B. können sie nur Scheiben bis zu einer bestimmten Größe bearbeiten. Die Restriktionen der einzelnen Maschinen können Sie im Dialog *Maschine* angeben.

Die verfügbaren Restriktionen im Dialog *Maschine* sind:
*   Minimale Dicke
*   Maximale Dicke
*   Modelle
*   Beschichtete Gläser
*   Strukturgläser
*   Stufen ISO
*   Abmessungen
*   SZR

Haben Sie eine Maschine, die weitere Restriktionen aufweist, müssen die Restriktionen mit zusätzlichen Bedingungen formuliert werden. Diese Bedingungen können auch Formeln enthalten. (Siehe "Bedingungen und Formeln in der Maschinenzuordnung")

Im Folgenden sind Beispiele zu den verfügbaren Restriktionen im Dialog *Maschine* aufgelistet.

**Beispiel: Restriktionen Dicke**
Sie können die Restriktion Dicke folgendermaßen einstellen:
*   Wenn die Maschine nur Scheiben ab einer Dicke von 8 mm bearbeiten kann, geben Sie die Restriktion **minimale Dicke 8 mm** ein.
*   Wenn die Maschine nur Scheiben bis zu einer Dicke von 15 mm bearbeiten kann, geben Sie die Restriktion **maximale Dicke 15 mm** ein.

**Beispiel: Restriktion Modelle**
Sie können die Restriktion *Modelle* folgendermaßen einstellen:
*   **Keine Restriktion:** die Maschine kann Modelle und Rechtecke bearbeiten, z. B. bei einem modernen Zuschnitttisch.
*   Die Maschine kann **nur Modelle** bearbeiten, z. B. um zu verhindern, dass rechteckige Scheiben zum Schleifen auf ein CNC-Center gelangen.
*   Die Maschine kann **keine Modelle**, also nur Rechtecke, bearbeiten, z. B. bei einer Schleif-Bohrstraße.

**Beispiel: Restriktion Beschichtete Gläser**
Sie können die Restriktion *Beschichtete Gläser* folgendermaßen einstellen:
*   **Keine Restriktion:** die Maschine kann beschichtete und unbeschichtete Gläser bearbeiten.
*   Die Maschine kann **nur beschichtete Gläser** bearbeiten.
*   Die Maschine kann **nur unbeschichtete Gläser** bearbeiten.

**Beispiel: Restriktion Strukturgläser**
Sie können die Restriktion *Strukturgläser* folgendermaßen einstellen:
*   **Keine Restriktion:** die Maschine kann Strukturgläser und Gläser ohne Struktur bearbeiten.
*   Die Maschine kann **nur Strukturgläser** bearbeiten.
*   Die Maschine kann **nur Gläser ohne Struktur** bearbeiten.

**Beispiel: Restriktion Stufen-ISO**
Sie können die Restriktion *Stufen-ISO* folgendermaßen einstellen:
*   **Keine Restriktion:** die Maschine kann Stufen-ISO und Normal-ISO fertigen.
*   Die Maschine kann **nur Stufen-ISO** bearbeiten.
*   Die Maschine kann **nur Normal-ISO** bearbeiten.

#### Abmessungsrestriktionen und Scheibenformat

Sie können bei einer Maschine minimale und maximale Größen der zu bearbeitenden Scheiben definieren. Orientieren Sie sich bei der Angabe der Werte an der Laufrichtung der Maschine. Die Werte Breite und Höhe dienen lediglich der Anschauung; Sie können auch Scheiben verarbeiten, deren Breite und Höhe vertauscht sind. Die Scheibe muss dann u. U. per Hand an der Maschine gedreht werden.

#### SZR-Restriktionen

Hier legen Sie fest, ob die Maschine einfaches ISO mit einem SZR oder mehrfaches ISO mit zwei SZRs fertigen kann. Für jeden SZR kann ein Mindest- und ein Maximalwert eingegeben werden.

#### UND-/ODER-Verknüpfungen

Wenn Sie die Restriktionen einer Maschine angeben, dann müssen Sie diese als logische Verknüpfungen (UND/ODER, AND/OR) angeben. Diese sind Grundverknüpfungen der booleschen Algebra, mit der sich logische Zusammenhänge zeigen lassen.
*   **UND-Verknüpfung:** Wenn zwei (oder mehr) Aussagen zutreffen, ist eine Aussage wahr.
    Beispiel: Auf einer Maschine können nur Scheiben bearbeitet werden, die breiter als 150 mm und höher als 200 mm sind. Daraus ergibt sich:
    Breite >= 150 mm UND Höhe >= 200 mm.
*   **ODER-Verknüpfung:** Wenn die eine oder die andere Aussage zutrifft, ist eine Aussage wahr.
    Beispiel: Auf einer Maschine können nur Scheiben bearbeitet werden, die breiter als 150 mm oder kürzer als 3500 mm sind. Daraus ergibt sich:
    Breite >= 150 mm ODER Länge <= 3500 mm.

#### Komponenten-ID

Die Komponenten-ID wird nur bei den Maschinentypen *Linie*, *Zuschnitt* und *Bieger* verwendet. Mit der Komponenten-ID kann zwischen Linien, Tischen oder Biegern unterschieden werden, wenn es mehrere des gleichen Typs gibt. So könnten zum Beispiel die Tische 1, 2 und 3 die Komponenten-IDs TB1, TB2 und TB3 bekommen.

Die Komponenten-ID steuert, in welchem Format die NC-Codeausgabe erfolgt.

#### Zusätzliche Bedingungen

Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaften von Maschinen unter Umständen massiv.

Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche Auswirkungen diese hat.

### Maschinen anlegen und verwalten

In dieser Lerneinheit lernen Sie, wie Sie neue Maschinen anlegen, bearbeiten oder löschen.

Wenn Sie eine Maschine anlegen, müssen Sie anschließend die Maschinendaten bearbeiten.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine Maschine an"
*   "So geben Sie die Eigenschaften einer Maschine ein"
*   "So löschen Sie eine Maschine"

> **Voraussetzung**
> Um eine neue Maschine anzulegen, muss ein passender Maschinentyp angelegt sein, z. B. *Zuschnitt*, *CNC-Center*, *Rahmenbieger*, *Sonstiges*. Der Katalog der Maschinentypen ist in A+W Production fest vorgegeben. Er steht in der Kombobox zur Verfügung, wenn Sie eine neue Maschine anlegen.

**So legen Sie eine Maschine an**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen > [Neu]**.
    [Image: Screenshot des Dialogs 'Neue Maschine' mit leeren Feldern für ID, Name, Maschinentyp und Komponenten-ID.]
2.  Geben Sie eine **ID** aus dem Nummernbereich ein, den Sie für diesen Maschinentyp vorgesehen haben, zum Beispiel **180**.
3.  Geben Sie einen **Namen** ein, der die Maschine eindeutig beschreibt, zum Beispiel **Schneidtisch 8**.
4.  Wählen Sie den zugehörigen **Maschinentyp**, zum Beispiel **Zuschnitt**.
5.  Geben Sie eine **Komponenten-ID** ein, zum Beispiel **TB8**.
    Sie müssen bei den Maschinentypen *Linien*, *Tische* oder *Bieger* eine Komponenten-ID eingeben. Damit können Sie zwischen den Maschinen unterscheiden, wenn es mehrere davon gibt.
    [Image: Abb. D-4 Beispiel für eine neue Maschine. Screenshot des Dialogs 'Neue Maschine' ausgefüllt mit ID 180, Name 'Schneidtisch 8', Maschinentyp 'Cutting (Zuschnitt)' und Komponenten-ID 'TB8'.]
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Damit haben Sie eine neue Maschine angelegt. Sie wird in der Liste der Maschinen im Dialog MZO-Editor aufgeführt.
    Um die Maschine vollständig zu beschreiben, müssen Sie die Eigenschaften und Zuordnungen festlegen.

**So geben Sie die Eigenschaften einer Maschine ein**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen**.
    [Image: Abb. D-5 MZO-Editor – Maschinen. Screenshot des MZO-Editors. Die neu erstellte Maschine 'Schneidtisch 8' mit ID 180 ist in der Liste markiert.]
2.  Markieren Sie die Maschine, die Sie bearbeiten wollen.
3.  Klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-6 Maschine. Screenshot des Dialogs 'Maschine - Schneidtisch 8', der die allgemeinen Eigenschaften der Maschine zeigt.]
4.  Ergänzen Sie die *Allgemeinen Eigenschaften* (A).
    Wenn Sie in ein Feld klicken, können Sie die Daten aus der Kombobox (B) wählen.
    Die Restriktionen im unteren Teil des Dialogs können Sie später bestimmen.
5.  Bestätigen Sie mit **[OK]**.
    Damit haben Sie die Stammdaten der Maschine angegeben.
    Die Maschinen-Restriktionen lernen Sie in einer separaten Einheit kennen. (Siehe "Restriktionen von Maschinen anlegen und bearbeiten")

**So löschen Sie eine Maschine**

> **Maschinen löschen**
> Das Löschen von Maschinen in A+W Production kann Auswirkungen auf die Produktion haben. Vergewissern Sie sich, dass die Maschinen nicht verwendet werden, bevor Sie sie löschen.

1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen**.
2.  Markieren Sie die Maschine, die Sie löschen möchten.
3.  Klicken Sie auf **[Löschen]**. Eine Sicherheitsabfrage wird angezeigt.
4.  Bestätigen Sie die Sicherheitsabfrage mit **[Yes]**, wenn Sie die Maschine endgültig löschen möchten. Die Maschinendaten werden gelöscht.

### Restriktionen von Maschinen anlegen und bearbeiten

In dieser Lerneinheit lernen Sie, die Restriktionen einer Maschine festlegen.

Dazu gibt es folgende Handlungsanleitungen:
*   "So bearbeiten Sie die Restriktionen zur Dicke"
*   "So bearbeiten Sie die Restriktionen für Modelle, beschichtete Gläser, Strukturgläser und Stufen-ISO"
*   "So bearbeiten Sie Restriktionen für Abmessungen und SZR"
*   "So entfernen Sie die Restriktionen Abmessungen und SZR"

> **Restriktionen und Zusätzliche Bedingung gleichzeitig**
> Wenn Restriktionen aktiviert sind und gleichzeitig eine Formel ausgewählt ist, kann dies zu einem Konflikt führen. Restriktionen können sich gegenseitig aufheben.
> Für Rückfragen wenden Sie sich bitte an den Support der A+W Software GmbH.

**So bearbeiten Sie die Restriktionen zur Dicke**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen**.
    [Image: Abb. D-7 MZO-Editor – Maschinen. Screenshot des MZO-Editors, eine Maschine ist markiert.]
2.  Markieren Sie die Maschine, die Sie bearbeiten wollen.
3.  Klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-8 Restriktion - Dicke bearbeiten. Screenshot des Dialogs 'Maschine', Bereich 'Restriktionen'.]
4.  Klicken Sie doppelt auf **[...]** (B).
    [Image: Eingabefelder für minimale und maximale Dicke.]
5.  Klicken Sie auf den **[Pfeil]**, um den Wert für die minimale Dicke einzugeben.
    [Image: Detailansicht des Eingabefeldes 'minimale Dicke'.]
6.  Geben Sie den Wert der minimalen Dicke in Millimetern ein.
7.  Klicken Sie auf **[OK]**, um den Wert zu speichern. Damit haben Sie den Wert der minimalen Dicke der Maschine geändert.
8.  Wiederholen Sie die Schritte 4 bis 7, um die Restriktionen für die maximale Dicke zu bearbeiten.

**So bearbeiten Sie die Restriktionen für Modelle, beschichtete Gläser, Strukturgläser und Stufen-ISO**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen**.
2.  Markieren Sie die Maschine, die Sie bearbeiten wollen.
3.  Klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-9 Restriktion - Modelle bearbeiten. Screenshot des Dialogs 'Maschine', die Option 'Modelle: Nein' ist markiert.]
4.  Klicken Sie doppelt auf **[...]** hinter *Modelle*. Ein **[Pfeil]** wird angezeigt.
5.  Klicken Sie auf den **[Pfeil]** (B), um *Modelle* zu aktivieren.
    [Image: Abb. D-10 Restriktion Modelle - Kombinationen der Checkboxen. Zeigt die verschiedenen Checkbox-Kombinationen, um festzulegen, ob eine Maschine nur Rechtecke, nur Modelle oder beides bearbeiten kann.]
6.  Wählen Sie die gewünschte Kombination der Checkboxen, um die Restriktion festzulegen:
    *   **Keine Einschränkung (A, B)**: Die Maschine kann Rechtecke und Modelle bearbeiten.
    *   **Keine Modelle (C, D)**: Die Maschine kann nur Rechtecke bearbeiten.
    *   **Keine Rechtecke (E, F)**: Die Maschine kann nur Modelle bearbeiten.
7.  Klicken Sie auf **[OK]**, um die Restriktion für *Modelle* zu speichern.
8.  Bearbeiten Sie auf die gleiche Weise die Restriktionen für *beschichtete Gläser*, *Strukturgläser* und *Stufen-ISO*.
    [Image: Restriktionen für beschichtete Gläser, Strukturgläser und Stufen-ISO.]

**So bearbeiten Sie Restriktionen für Abmessungen und SZR**

> **Restriktionen werden unwiderruflich gelöscht**
> Abmessungsrestriktionen werden unwiderruflich und ohne Sicherheitsabfrage gelöscht, wenn Sie auf das **[X]** klicken.

1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen**.
2.  Markieren Sie die Maschine, die Sie bearbeiten wollen.
3.  Klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-11 Restriktion - Abmessungen bearbeiten. Screenshot des Dialogs 'Maschine', der Bereich 'Abmessungen' ist hervorgehoben.]
4.  Klicken Sie im Feld *Abmessungen* auf das **[Stift-Symbol]**, um den Dialog *Abmessungsrestriktionen* zu öffnen.
    [Image: Dialog 'Abmessungsrestriktionen' mit Feldern für Min/Max Breite und Höhe.]
5.  Aktivieren Sie die Checkboxen der Eingabefelder, die Sie bearbeiten möchten.
6.  Geben Sie die Werte in die Eingabefelder ein.
7.  Klicken Sie auf **[OK]**, um die Änderungen der Abmessungsrestriktionen zu speichern. Die Restriktion wird im Feld *Abmessungen* als UND-/ODER-Verknüpfungen angezeigt.
8.  Bearbeiten Sie auf die gleiche Weise die Restriktionen für den SZR.

**So entfernen Sie die Restriktionen Abmessungen und SZR**

> **Abmessungsrestriktionen löschen**
> Abmessungsrestriktionen werden unwiderruflich und ohne Sicherheitsabfrage gelöscht, wenn Sie auf das **[X]** klicken.

1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Maschinen**.
2.  Markieren Sie die Maschine, die Sie bearbeiten wollen.
3.  Klicken Sie auf **[Bearbeiten]**. Der Dialog *Maschine* wird geöffnet.
4.  Klicken Sie im Bereich *Abmessungen*, auf **[X]**, um die Restriktion zu entfernen.
5.  Klicken Sie auf **[OK]**, um die Änderungen zu speichern.
6.  Entfernen Sie auf die gleiche Weise die SZR-Restriktionen.

### Übungen zu Maschinen

Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
*   Bilden Sie auf Papier den Maschinenpark Ihres Betriebes ab.
*   Notieren Sie, welche Maschine in welchen Maschinentyp fällt.
*   Vergeben Sie für die Maschinen systematisch IDs (Nummernkreise).
*   Notieren Sie, welche Eigenschaften für die Maschinen gelten und ob es Restriktionen gibt:
    *   Gibt es Restriktionen, wie zum Beispiel minimale Dicke, maximale Dicke oder Abmessungsrestriktionen.
    *   Kann die Maschine ISO oder 3-fach-ISO bearbeiten? Wo müssen Sie diese Eingaben vornehmen?
*   Legen Sie Maschinen als Übungsmaschinen in A+W Production an und passen Sie diese so an, dass sie Ihrem Maschinenpark entsprechen.
*   Lassen Sie die testweise erstellten Maschinen bestehen, da spätere Übungen darauf aufbauen.

**Ergänzende Informationen**
*   Softwarereferenz, "Neue Maschine"
*   Softwarereferenz, "Maschine"
*   Softwarereferenz, "Abmessungsrestriktionen"
*   Softwarereferenz, "SZR Restriktionen"

### Logische Maschinen

**Lernziele**
*   Was sind logische Maschinen in A+W Production und speziell in der Maschinenzuordnung?
*   Warum gibt es logische Maschinen?
*   Wie werden Namen und Nummern vergeben?
*   Wie werden logische Maschinen neu angelegt, bearbeitet oder gelöscht?
*   Wann können logische Maschinen gelöscht werden und wann nicht?

**Nutzen**
*   Logische Maschinen bilden eine Funktion einer Maschine ab. Kann eine Maschine Bohren und Kanten bearbeiten, werden dafür in A+W Production zwei logische Maschinen angelegt. Und damit kann im nächsten Schritt ein Arbeitsgang der Funktion einer Maschine zugeordnet werden.
*   Die A+W Production BDE (Betriebsdatenerfassung) wertet unter anderem Daten der logischen Maschinen aus, z. B. für Statistiken.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Logische Maschinen** | Logische Maschinen bilden jeweils eine Funktion einer physikalischen Maschine ab. Logische Maschinen werden zur Ablaufsteuerung in der Produktion und zur Kostenberechnung verwendet. Logische Maschinen werden zur Betriebsdatenerfassung verwendet. Sobald Sie eine Maschine anlegen, wird automatisch eine logische Maschine angelegt. Zu einer Maschine können beliebig viele logische Maschinen definiert werden. |
| **Zuordnung** | Logische Maschinen werden Arbeitsgängen zugewiesen. |

#### Logische Maschinen in der Maschinenzuordnung

Logische Maschinen bilden jeweils eine Funktion einer realen Maschine ab. Dabei werden die Eigenschaften der Maschine an die logische Maschine vererbt. Zusätzlich zu den Eigenschaften der Maschine gelten die Eigenschaften der logischen Maschine.

[Image: Abb. D-12 Logische Maschinen. Screenshot des MZO-Editors im Tab 'Logische Maschinen'. Die Liste zeigt die ID der physischen Maschine, die ID der logischen Maschine und deren Namen.]

Logische Maschinen werden benötigt für:
*   Beschreibung einzelner Maschinenfunktionen.
*   Zuordnung von Arbeitsgängen.
*   Priorisierung von Arbeitsgängen.
*   Auslastungsplanung und Umlastung.
*   Logische Maschinen trennen einzelne Funktionen von Maschinen. Damit werden für eine Maschine z. B. unterschiedliche Kostensätze oder Übergangszeiten möglich.
*   Statistische Auswertungen.

**Beispiel**
Sie haben eine CNC-Maschine, die bohren, schleifen und polieren kann. Sie definieren die Maschine als CNC-Maschine 1. Dazu erstellt A+W Production automatisch eine logische Maschine. Da die CNC-Maschine drei Funktionen besitzt, werden drei logische Maschinen definiert.
Diese definieren Sie so, dass die Stammdaten zu Bohren angelegt sind. Nun definieren Sie zur CNC-Maschine 1 zwei weitere logische Maschinen: eine mit den Stammdaten zum Schleifen und die andere mit den Stammdaten zum Polieren.

[Image: Abb. D-13 Beispiel: Drei logische Maschinen resultieren aus einem CNC-Center. Ein Diagramm zeigt, wie eine reale CNC-Maschine mit den Funktionen Bohren, Schleifen, Polieren in drei separate logische CNC-Maschinen aufgeteilt wird.]

Die Bearbeitungszeiten, die eine logische Maschine für den ihr zugewiesenen Arbeitsgang benötigt, wird als Formel in der Kapazitätsplanung definiert. Dazu steht die separate Dokumentation für den Part Kapazitätsplanung zur Verfügung.

### Logische Maschinen anlegen und verwalten

In diesem Teil des Tutorials lernen Sie, wie Sie logische Maschinen anlegen und bestehende bearbeiten oder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine logische Maschine an"
*   "So bearbeiten Sie eine logische Maschine"
*   "So löschen Sie eine logische Maschine"

> **Voraussetzung**
> Sie können logische Maschinen erst dann anlegen, wenn die zugehörige Maschine angelegt ist.

**So legen Sie eine logische Maschine an**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Logische Maschinen**.
    [Image: Abb. D-14 Logische Maschine markiert. Screenshot des MZO-Editors. Eine automatisch erstellte logische Maschine ist markiert, die als Basis für eine neue dienen wird.]
    A+W Production erstellt automatisch zu jeder Maschine eine logische Maschine. Alle weiteren logischen Maschinen können nur auf Basis der bereits bestehenden erstellt werden.
2.  Markieren Sie die logische Maschine, welche die Basis für die neue logische Maschine sein soll.
3.  Klicken Sie auf **[Neu]**.
    [Image: Dialog 'Neue logische Maschine'.]
4.  Geben Sie die **ID** und den **Namen** ein.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    [Image: Abb. D-15 Neue logische Maschine. Die neue logische Maschine 'Logischer Schneidetisch_8-2' erscheint in der Liste.]
    Damit haben Sie eine neue logische Maschine angelegt. Die neue logische Maschine wird im Register Logische Maschinen im MZO-Editor gelistet. Sie können jetzt die Eigenschaften der neuen logischen Maschine bearbeiten.

**So bearbeiten Sie eine logische Maschine**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Logische Maschinen**.
2.  Markieren Sie die logische Maschine, die Sie bearbeiten wollen.
3.  Klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-16 Logische Maschine – Eigenschaften. Screenshot des Dialogs 'Logische Maschine' mit den allgemeinen Eigenschaften.]
4.  Geben Sie die Daten für die logische Maschine ein, z. B. für einen Schneidtisch.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Damit haben Sie die Stammdaten der logischen Maschine angelegt.

**So löschen Sie eine logische Maschine**

> **Logische Maschinen löschen**
> A+W Production legt zu jeder Maschine automatisch eine logische Maschine an. Diese automatisch erstellte logische Maschine kann nicht gelöscht werden. Wird eine Maschine gelöscht, werden damit auch automatisch alle zugehörigen logischen Maschinen gelöscht.
> Wenn Sie eine logische Maschine löschen, löschen Sie die Funktion einer Maschine. Dies kann zu erheblichen Problemen im Produktionsprozess führen. Stellen Sie sicher, dass die logische Maschine und die Maschine nicht in der Fertigung verwendet wird, bevor Sie sie löschen.

1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Logische Maschinen**.
2.  Markieren Sie die logische Maschine, die Sie löschen wollen.
3.  Klicken Sie auf **[Löschen]**. Eine Sicherheitsabfrage wird angezeigt.
4.  Bestätigen Sie die Sicherheitsabfrage mit **[Yes]**, wenn Sie die logische Maschine endgültig löschen möchten. Die Daten werden gelöscht.

### Übungen zu logischen Maschinen

Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
*   Legen Sie Übungsmaschinen an, die den Maschinenpark in Ihrem Betrieb abbilden oder verwenden Sie die Übungsmaschinen aus der vorherigen Lerneinheit.
    *   Notieren Sie sich, welche Arbeitsgänge auf den jeweiligen Maschinen durchgeführt werden können, z. B. Bohren, Schleifen, Säumen.
    *   Legen Sie die entsprechenden logischen Maschinen an.
*   Ein ESG-Ofen kann vorspannen und teil-vorspannen. Würden Sie für die beiden Funktionen verschiedene logische Maschinen definieren? Nennen Sie die Vorteile und Nachteile.

**Ergänzende Informationen**
*   "Übungen zu Maschinen"
*   Softwarereferenz, "Neue logische Maschine"
*   Softwarereferenz, "Logische Maschine"

### Arbeitsgänge

**Lernziele**
*   Was sind Arbeitsgänge speziell in der Maschinenzuordnung?
*   Wie werden Arbeitsgänge verwaltet, angelegt, bearbeitet oder gelöscht?
*   Warum haben Arbeitsgänge Prioritäten und wie werden diese verändert?
*   Was haben Arbeitsgänge mit Bearbeitungstypen und Artikeln zu tun?

**Nutzen**
*   Mit einem Arbeitsgang wird eine Anforderung eine Bearbeitung auszuführen erfüllt, die aus der Stückliste kommt. Diese Anforderung kann zum Beispiel lauten *polieren* oder *schleifen*. Der Arbeitsgang definiert anhand dieser Anforderung dann die spezielle Art des Polierens oder Schleifens.
*   Die Ebene der logischen Maschine stellt die Verbindung zwischen Arbeitsgang und physikalischer Maschine her, auf welcher der Arbeitsgang ausgeführt wird.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Arbeitsgänge** | Arbeitsgänge bringen die Eigenschaften des Bearbeitungstyps, wie z. B. Zuschnitt, mit den Eigenschaften des Werkstücks zusammen. Arbeitsgänge basieren auf Bearbeitungstypen oder Artikeln. |
| **Bedingungen/Formeln** | Arbeitsgänge können auch mit Bedingungen/Formeln definiert werden. |

#### Arbeitsgänge in der Maschinenzuordnung

Ein Arbeitsgang wird durch einen hinterlegten Bearbeitungstyp, einen Bearbeitungsartikel, eine Artikelgruppe und/oder eine zusätzliche Bedingung definiert. (Siehe "Bearbeitungstypen und Bearbeitungsartikel")

[Image: Abb. D-17 Arbeitsgänge. Screenshot des MZO-Editors im Tab 'Arbeitsgänge'. Die Liste zeigt ID, Name und zusätzliche Bedingung der Arbeitsgänge.]

Ist zu einem Arbeitsgang ein Bearbeitungstyp, z. B. *Zuschnitt*, hinterlegt, ist damit festgelegt, um welche technische Form der Bearbeitung es sich bei dem Arbeitsgang handelt. Nutzen Sie vorrangig den Standard-Bearbeitungstypen-katalog der A+W Software GmbH, um Arbeitsgänge zu definieren.

Legen Sie nur eigene Bearbeitungstypen an, wenn es keine passenden vordefinierten Bearbeitungstypen gibt. Separate Arbeitsgänge legen Sie an, wenn Sie Aussagen über Ihre Produktion treffen können, z. B.:
*   Siebdruck in dunklen Farben fassen Sie an einem bestimmten Wochentag zusammen, weil Sie dann das Lösemittel entsorgen (Mögliche Kampagnenplanung).
*   Die dicken Scheiben werden auf Maschine 1 geschliffen. Die dünnen Scheiben auf Maschine 2, aber sie dienen gegenseitig als Ausweichmaschine (Wahl des Bestbetriebsmittels).
*   Serienscheiben dürfen nur auf der automatischen Bohrstraße gebohrt werden. Wenn die ausfällt, müssen Sie den Liefertermin verschieben.

Der Arbeitsgang *Pseudo-Bearbeitung* steht für Bearbeitungen in der Stückliste, die informativen Charakter haben, z. B. *Nicht stempeln*, *Handschuhe benutzen*, *Toleranz beachten*. Damit für diese Bearbeitungen keine Terminfindung durchgeführt wird, werden sie auf eine Maschine *Dummy für informative Bearbeitungen* eingelastet, die keine BDE-Erfassungsstelle hat und damit auch keinen Schichtplan.

#### Bearbeitungsartikel am Arbeitsgang

Wenn Sie zu einem Arbeitsgang einen Bearbeitungsartikel hinterlegen, z. B. *Modellzuschnitt für VSG*, können Sie noch vor der eigentlichen Maschinenzuordnung die Behandlung der VSG-Modelle von den anderen Gläsern trennen.

[Image: Abb. D-18 Arbeitsgang - Artikel. Screenshot des Dialogs 'Arbeitsgang', der die Restriktionen basierend auf A+W Typen, Typen oder Artikeln zeigt.]

Sie können den Arbeitsgang noch genauer spezifizieren, indem Sie zusätzlich eine Restriktion aus dem Feld *Artikel* wählen. Der **Artikeltyp (A)** ist von der A+W Software GmbH vordefiniert. Er enthält Basis-Artikel, z. B. ESG, VSG oder Sprossen.

Wenn Sie z. B. den Bearbeitungstyp *Zuschnitt* und zusätzlich den Artikel *VSG* auswählen, legen Sie einen Arbeitsgang an, mit dem der Zuschnitt von VSG durchgeführt wird.

Mit der **Artikelgruppe (B)** können Sie aus Produktionsartikelgruppen wählen, die Sie selbst definiert haben. Wählen Sie z. B. zum Bearbeitungstyp *Zuschnitt* die Artikelgruppe *Ganzglastüren*. Damit haben Sie einen Arbeitsgang angelegt, mit dem der Zuschnitt von Ganzglastüren durchgeführt wird.

Wählen Sie einen **Artikel (C)**, um einen Arbeitsgang an einem speziellen Artikel festzumachen. Wenn Sie z. B. zu einem Arbeitsgang den Bearbeitungstyp *Zuschnitt* und den Artikel *Float 6 mm* angeben, legen Sie einen Arbeitsgang an, mit dem der Zuschnitt von 6 mm-Float durchgeführt wird.

> **Bearbeitungstypen**
> Zu Bearbeitungstypen gibt es eine separate Lerneinheit.

[Image: Abb. D-19 Beispiele für unterschiedlich definierte Arbeitsgänge. Ein Diagramm, das drei verschiedene Arbeitsgänge zeigt: einen allgemeinen 'Zuschnitt', einen spezifischen 'Zuschnitt von VSG' (basierend auf dem VSG-Katalog) und einen noch spezifischeren 'Zuschnitt von Float 6 mm' (basierend auf dem Artikel Float 6 mm).]

#### Arbeitsgang exakt definieren

Durch Verwenden der Optionen im Dialog *Arbeitsgang* im Feld *Artikel* definieren Sie Arbeitsgänge exakt.

**Beispiel 1:**
Der Zuschnitt von VSG kann nur an Schneidetischen erfolgen, die zwei Schneidköpfe haben, oder andere Techniken einsetzen, wie z. B. Waterjet.
Für den Zuschnitt von Float besteht bereits der Arbeitsgang *Zuschnitt*.
Definieren Sie nun einen neuen Arbeitsgang zum Schneiden von VSG. Wählen Sie dazu den Bearbeitungstyp *Zuschnitt* und den Glastyp *VSG*.
Damit definieren Sie einen Arbeitsgang, der die Problematik beim Schneiden von VSG berücksichtigt und dem nur logische Maschinen zugeordnet werden dürfen, die diese Bearbeitung durchführen können.

**Beispiel 2 - Option Artikelgruppe:**
Sie haben Artikel, die nur selten produziert werden.
Bilden Sie in diesem Fall eine Artikelgruppe mit den seltenen Artikeln und starten Sie eine Kampagne. Da die Kampagnen-Planung auf einem Arbeitsgang basiert, wählen Sie für diese Kampagne die Artikelgruppe mit den seltenen Artikeln.
So können Sie exakt vorausplanen, wann und wie die seltenen Artikel gefertigt werden.
Kampagnen sind ausführlich im Part Kapazitätsplanung beschrieben.

#### Nicht zugeordnete Arbeitsgänge

Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logische Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logische Maschine zu. Ist die zugehörige logische Maschine noch nicht definiert, sollte temporär die logische Maschine *Dummy* zugeordnet werden.

#### Priorität von Arbeitsgängen

Die Arbeitsgänge können in der Liste nach oben oder unten verschoben werden. Die Liste wird bei der Arbeitsgangzuordnung von oben nach unten abgearbeitet. Sobald alle einem Arbeitsgang zugeordneten Bedingungen zutreffen, wird dieser Arbeitsgang zugeordnet. Deshalb ist es notwendig, spezialisierten Arbeitsgängen immer eine höhere Priorität zuzuweisen, als unspezialisierten Arbeitsgängen.

#### Mehrere Arbeitsgänge an einer Scheibe

Sie haben den Auftrag eine Glastür zu produzieren. Dazu werden die Arbeitsgänge *Rechteckschleifen*, *Bohren* und *Ausschnitte* benötigt.

Anstatt das Rechteckschleifen auf der kostengünstigen Rechteckschleifmaschine auszuführen, lassen Sie alle drei Arbeitsgänge auf dem CNC-Center durchführen. Damit ist der einzelne Arbeitsgang Rechteckschleifen zwar teurer, aber Sie sparen Aufwand, indem alle drei Arbeitsgänge direkt hintereinander auf einer Maschine durchgeführt werden.

Dazu haben Sie den Arbeitsgang *Rechteckschleifen auf CNC-Center* definiert, dem Sie die logische Maschine *CNC-Center Rechteckschleifen* mit hoher Priorität zugeordnet haben.
Um Engpässe zu vermeiden, ist dem Arbeitsgang *Rechteckschleifen auf CNC-Center* auch die logische Maschine *Rechteckschleifmaschine* zugeordnet, mit niedriger Priorität.

Würden Sie die Glastür auf günstigeren Maschinen fertigen, sähe der Produktionsablauf so aus:
*   Schleifen auf der Rechteckschleifmaschine.
*   Anschließend Bohren auf der automatischen Bohrmaschine.
*   Abschließend Fertigen der Ausschnitte auf dem CNC-Center.
*   Dazu kommen 2 x Handling, 2 x Waschen und die Rüstzeit für das CNC-Center.

Es kann also günstiger sein, die Glastür komplett auf dem CNC-Center zu fertigen.

#### Zusätzliche Bedingungen in Arbeitsgängen

Arbeitsgänge sind nicht ausschließlich an Bearbeitungen gebunden. Sie können auch zusätzliche Bedingungen enthalten. Eine Bedingung kann zum Beispiel lauten: *Dieser Arbeitsgang wird auf dem CNC-Center durchgeführt*. So können Sie bei der Definition des Arbeitsgangs vorgeben, welche Maschinen vorrangig verwendet werden.

Eine zusätzliche Bedingung kann auch die Stückliste abfragen. Wird eine entsprechende Bedingung an einem Arbeitsgang hinterlegt, kann damit der Laufweg der Scheibe durch die Produktion gesteuert werden. Die Bedingung könnte beispielsweise lauten: *Stehen in der Stückliste der Scheibe die Bearbeitungen Schleifen, Bohren und Ausschneiden, dann fertige die Scheibe komplett auf dem CNC-Center*.

[Image: Abb. D-20 Beispiel: Eine zusätzliche Bedingung im Arbeitsgang fragt die Stückliste ab. Das Diagramm zeigt, dass ein Arbeitsgang 'Glastür' mit einer Bedingung ('Schleifen + Bohren + Ausschneiden') direkt dem CNC-Center zugeordnet wird.]

[Image: Abb. D-21 Beispiel: Arbeitsgangzuordnung auf Basis eines Bearbeitungsartikels. Das Diagramm zeigt, dass der Bearbeitungsartikel 'Glastür' einen Arbeitsgang 'Glastür' auslöst, der wiederum an das CNC-Center gebunden ist.]

**Beispiel: Engpass durch zusätzliche Bedingung**
Zum Arbeitsgang *Glastür* ist die Bedingung hinterlegt, dass Glastüren auf dem CNC-Center gefertigt werden. Die Bedingung kann sich entweder auf die Stückliste oder einen Bearbeitungsartikel beziehen.
Wenn zum Auftrag mit Glastüren ein weiterer Auftrag, zum Beispiel mit Modellen, kommt, entsteht auf dem CNC-Center ein Engpass.
**Lösung:** Sie ändern die Priorität der logischen Maschine CNC-Center, sodass das CNC-Center nicht mehr die erste Wahl für Glastüren ist. Dadurch werden die Glastüren nicht auf dem CNC-Center gefertigt, sondern in einzelnen Arbeitsschritten auf der Rechteckschleifmaschine, der automatischen Bohrmaschine und der Ausschneidemaschine.
Das erhöht zwar den Handling-Aufwand bei den Glastüren, ermöglicht aber, die Modelle gleichzeitig auf dem CNC-Center zu fertigen.
Ist der Engpass vorüber, müssen die ursprünglichen Prioritäten der logischen Maschinen wieder hergestellt werden.

Sie können Arbeitsgänge auch auf Basis eines Bearbeitungsartikels definieren, was zum Beispiel dann sinnvoll ist, wenn Sie eine Bearbeitung künstlich in die Stückliste einfügen wollen.

**Beispiel: Arbeitsgang basierend auf Bearbeitungsartikel**
Ein ESG wurde beschichtet und muss ab diesem Zeitpunkt mit Handschuhen angefasst werden.
Definieren Sie für diesen Fall den Bearbeitungsartikel *Handschuhe tragen!* und wählen Sie diesen als Grundlage für den Arbeitsgang. In der Arbeitsgangzuordnung ordnen Sie den Arbeitsgang der logischen Maschine *Dummy* zu.
Damit haben Sie einen Arbeitsgang eingeführt, der auf keiner Maschine läuft, aber in der Produktion als handhabe *beschichtete ESG mit Handschuhen* existiert.

> **Arbeitsgang basierend auf Bearbeitungsartikel nur in Einzelfällen**
> Arbeitsgänge auf der Basis von Bearbeitungsartikeln bilden eine Ausnahme, da Sie für die Aufnahme neuer Bearbeitungsartikel die Arbeitsgangzuordnung ergänzen und pflegen müssen. Die Definition von Arbeitsgängen basierend auf Bearbeitungsartikeln ist nur in Einzelfällen, wie in oben genanntem Beispiel, sinnvoll.

### Arbeitsgänge anlegen und verwalten

In dieser Lerneinheit legen Sie neue Arbeitsgänge an, bearbeiten und löschen diese aus der Liste.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie einen Arbeitsgang an"
*   "So bearbeiten Sie die Restriktionen zu einem Arbeitsgang"
*   "So löschen Sie einen Arbeitsgang"

> **IDs für Arbeitsgänge**
> Geben Sie einem Arbeitsgang immer die zugrundeliegende ID der Bearbeitung und/oder des Artikels multipliziert mit 10.
> **Beispiel:** Dem Arbeitsgang liegt die Bearbeitung *Säumen* mit der ID 1000 aus dem Standard-Bearbeitungskatalog zugrunde. Geben Sie in diesem Fall dem neuen Arbeitsgang die ID 10000.
> Mit diesem System lassen sich Bearbeitungen, Artikel und Arbeitsgänge auseinanderhalten, aber die Zugehörigkeit ist leicht erkennbar.

**So legen Sie einen Arbeitsgang an**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Arbeitsgänge > [Neu]**. Der Dialog *Neuer Arbeitsgang* wird geöffnet.
2.  Geben Sie die Daten ein.
    [Image: Abb. D-22 Neuer Arbeitsgang. Screenshot des Dialogs 'Neuer Arbeitsgang'.]
3.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Der Dialog *Arbeitsgang* wird geöffnet, um die Restriktionen zu bearbeiten.

> **Arbeitsgänge in roter Schrift**
> Ein Arbeitsgang wird im MZO-Editor in roter Schrift angezeigt, wenn ihm noch keine logische Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logische Maschine zu. Ist die zugehörige logische Maschine noch nicht definiert, kann temporär die logische Maschine *Dummy* zugeordnet werden.

**So bearbeiten Sie die Restriktionen zu einem Arbeitsgang**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Arbeitsgänge**.
2.  Markieren Sie den Arbeitsgang, den Sie bearbeiten möchten.
3.  Klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-23 Arbeitsgang – Restriktionen bearbeiten. Screenshot des Dialogs 'Arbeitsgang'.]
4.  Wählen Sie die Optionen und die entsprechenden Typen oder Artikel, um den Arbeitsgang zu definieren. Damit haben Sie den Arbeitsgang bearbeitet.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.

**So löschen Sie einen Arbeitsgang**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Arbeitsgänge**.
2.  Markieren Sie den Arbeitsgang, den Sie löschen möchten. Ein Arbeitsgang wird im MZO-Editor in roter Schrift angezeigt, wenn ihm noch keine logische Maschine zugeordnet ist.
3.  Klicken Sie auf **[Löschen]**. Eine Sicherheitsabfrage wird geöffnet.
4.  Klicken Sie auf **[Yes]**, um den Arbeitsgang endgültig zu löschen. Die Daten werden gelöscht.

### Übungen zu Arbeitsgängen

Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
*   Legen Sie Übungsmaschinen und logische Übungsmaschinen an, die den Maschinenpark in Ihrem Betrieb abbilden oder verwenden Sie die Übungsmaschinen aus den vorigen Übungen.
    *   Definieren Sie einen Übungsarbeitsgang *Polieren*, der auf dem Standard-Bearbeitungskatalog basiert.
    *   Definieren Sie einen Übungsarbeitsgang *handhabe beschichtete ESG mit Handschuhen*. Der Arbeitsgang soll auf einem Bearbeitungsartikel basieren.
    *   Definieren Sie einen Übungsarbeitsgang *VSG-Zuschnitt*, der auf dem Standard-Bearbeitungskatalog basiert und den Sie mit einem Artikel genauer definieren.
*   Bilden Sie den Maschinenpark Ihres Betriebes auf Papier ab und listen Sie die daraus resultierenden logischen Maschinen auf. Betrachten Sie die aktuelle Auftragssituation, welche Arbeitsgänge sind in dieser Situation anzulegen?

**Ergänzende Informationen**
*   Softwarereferenz, "Neuer Arbeitsgang"
*   Softwarereferenz, "Arbeitsgang"

### Arbeitsgangzuordnung

**Lernziele**
*   Was ist die Arbeitsgangzuordnung?
*   Wie werden Arbeitsgänge zugeordnet?
*   Wie werden Zuordnungen wieder aufgelöst?
*   Wie wird die Priorität von logischen Maschinen geändert?
*   Warum haben logische Maschinen eine Priorität?

**Nutzen**
*   Mit der Arbeitsgangzuordnung ordnen Sie logische Maschinen den Arbeitsgängen zu. Durch eine geschickte Zuordnung optimieren Sie die Kosten der Produktion.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Arbeitsgangzuordnung** | Die Arbeitsgangzuordnung verbindet logische Maschinen mit Arbeitsgängen. |
| **Prioritäten** | Mit der Arbeitsgangzuordnung werden Prioritäten der logischen Maschinen festgelegt. Damit legen Sie fest, dass der jeweilige Arbeitsgang auf der optimalen Maschine und möglichst kostengünstig durchgeführt wird. |
| **Arbeitsgangzuordnung** | Mit der Arbeitsgangzuordnung hat der Anwender die Möglichkeit in den Produktionsprozess einzugreifen. |

#### Angepasste Arbeitsgangzuordnung

Sie ordnen logische Maschinen den jeweiligen Arbeitsgängen zu. Unter jedem Arbeitsgang kann die Reihenfolge, und damit die Priorität der logischen Maschinen, festgelegt werden. Somit legen Sie Prioritäten der Maschinen im Produktionsprozess fest.

Bei Maschinen, die mehrere Funktionen durchführen können, wie z. B. ein CNC-Center, entsteht die Tendenz, dass mehr Arbeitsgänge auflaufen als bei spezialisierten Maschinen, die z. B. nur eine Funktion durchführen können. Resultat ist, dass mehr Arbeitsgänge am teuren CNC-Center durchgeführt werden und dadurch ein Engpass entsteht.

Das können Sie durch Priorisierung in der Arbeitsgangzuordnung und dem Definieren angepasster Arbeitsgänge verhindern.

Sie legen Arbeitsgänge an, die die einzelnen Anwendungen exakt abbilden und ordnen diese Arbeitsgänge den dazu passenden logischen Maschinen zu. So können Sie sicherstellen, dass die Arbeitsgänge an den jeweils kostengünstigsten Maschinen durchgeführt werden.

#### Bedingung in einem Arbeitsgang

Arbeitsgänge können auch zusätzliche Bedingungen enthalten. So können Sie schon bei der Definition des Arbeitsgangs vorgeben, welche Maschinen vorrangig verwendet werden.

Eine zusätzliche Bedingung kann auch die Stückliste abfragen. Die Bedingung könnte beispielsweise lauten: *Stehen in der Stückliste der Scheibe die Bearbeitungen Schleifen, Bohren und Ausschneiden, dann fertige die Scheibe komplett auf dem CNC-Center.*

Wird eine entsprechende Bedingung an einem Arbeitsgang hinterlegt, kann damit der Laufweg der Scheibe durch die Produktion gesteuert werden.

> **Arbeitsgänge immer zuordnen**
> Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logische Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logische Maschine zu. Ist die zugehörige logische Maschine noch nicht definiert, sollte temporär die logische Maschine *Dummy* zugeordnet werden.

[Image: Abb. D-24 & D-25 sind Duplikate von D-20 & D-21 und werden hier nicht wiederholt.]

[Image: Abb. D-26 Beispiel: angepasste Arbeitsgangzuordnung. Screenshot des MZO-Editors. Der Arbeitsgang 'Rechteckschleifen' (10051) ist neu definiert und wird der logischen Maschine der Rechteckschleifmaschine (B) und der logischen Maschine für Modellschleifen am CNC (C) zugeordnet.]

**Beispiel: angepasste Arbeitsgangzuordnung**
Sie haben in Ihrer Produktion eine Rechteckschleifmaschine und ein CNC-Center. Mit beiden kann die Bearbeitung *Schleifen* durchgeführt werden.
*   In der Liste der Arbeitsgänge ist ein Arbeitsgang *Rechteckschleifen* definiert, dem alle rechteckigen Scheiben zugeführt werden. In der Arbeitsgangzuordnung ist dem Arbeitsgang *Rechteckschleifen* die Rechteckschleifmaschine zugeordnet. Diese hat höchste Priorität.
*   In der Liste der Arbeitsgänge ist ein Arbeitsgang *Modellschleifen* definiert, dem alle Modelle zugeführt werden. In der Arbeitsgangzuordnung ist dem Arbeitsgang *Modellschleifen* das CNC-Center zugeordnet.
*   Das CNC-Center ist auch dem Arbeitsgang *Rechteckschleifen* zugeordnet, jedoch mit geringerer Priorität.

Mit diesen Einstellungen wird das Schleifen von rechteckigen Scheiben auf der kostengünstigen Rechteckschleifmaschine durchgeführt. Sollte ein Engpass entstehen, werden die Rechtecke auch auf dem CNC-Center geschliffen.

[Image: Abb. D-27 & D-28: Beispiel mehrerer Arbeitsgänge an einer Scheibe. Screenshots, die zeigen, wie der Arbeitsgang 'Rechteckschleifen auf CNC' (10053) definiert und den entsprechenden logischen Maschinen mit unterschiedlichen Prioritäten zugeordnet wird, um Engpässe zu managen.]

In diesem Beispiel sehen Sie, dass dem Arbeitsgang *Rechteckschleifen auf CNC-Center* die logische Maschine *CNC-Center Rechteckschleifen* mit höchster Priorität zugeordnet ist. Zudem wurde die logische Maschine *Rechteckschleifmaschine* mit geringerer Priorität zugeordnet, um Engpässe zu vermeiden. Dem Beispiel zu mehreren Arbeitsgängen an einer Scheibe entsprechend ist es die kostengünstigere Variante, die Glastür komplett auf dem CNC-Center zu fertigen.

### Arbeitsgänge und logische Maschinen zuordnen

In dieser Lerneinheit ordnen Sie logische Maschinen den Arbeitsgängen zu, trennen Arbeitsgänge und logische Maschinen und ändern Prioritäten von logischen Maschinen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So ordnen Sie eine logische Maschine einem Arbeitsgang zu"
*   "So trennen Sie logische Maschinen von Arbeitsgängen"
*   "So ändern Sie die Priorität einer logischen Maschine"

**So ordnen Sie eine logische Maschine einem Arbeitsgang zu**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung**.
2.  Markieren Sie den Arbeitsgang und die logische Maschine, die Sie einander zuordnen wollen.
    [Image: Abb. D-29 Arbeitsgang und logische Maschine markiert. Ein Arbeitsgang und eine nicht zugeordnete Maschine sind markiert.]
3.  Klicken Sie auf den **Pfeil nach links**, um die logische Maschine dem Arbeitsgang zuzuordnen. Die logische Maschine ist nun dem Arbeitsgang zugeordnet und wird unter dem Arbeitsgang grau hinterlegt angezeigt.
    [Image: Abb. D-30 Arbeitsgang und logische Maschine zugeordnet. Die Maschine erscheint nun unter dem Arbeitsgang.]
4.  Klicken Sie auf **[Übernehmen]**, um die Daten zu speichern. Die Zuordnung wird gespeichert.

**So trennen Sie logische Maschinen von Arbeitsgängen**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung**.
2.  Klicken Sie auf **[+]** des Arbeitsgangs. Die Ansicht klappt auf und die logischen Maschinen werden angezeigt.
3.  Markieren Sie die logische Maschine, die getrennt werden soll.
    [Image: Abb. D-31 Arbeitsgang und logische Maschine trennen. Eine zugeordnete Maschine ist markiert.]
4.  Klicken Sie auf den **Pfeil nach rechts**, um die logische Maschine vom Arbeitsgang zu trennen.
5.  Klicken Sie auf **[Übernehmen]**, um die Änderungen zu speichern.

> **Logische Maschine noch in Verwendung**
> Wenn eine Zuordnung entfernt werden soll, die noch in Verwendung ist, wird sie automatisch deaktiviert. Deaktivierte Zuordnungen werden in kursiver Schrift und mit einem entsprechenden Symbol dargestellt.
> Bitte beachten: falls eine deaktivierte logische Maschine in einem bestehenden Auftrag für einen Arbeitsgang eine Alternative darstellt, wird diese Alternative bei der Umlastung nach wie vor angeboten. Erst bei einer Wiederholung der MZO für diesen Auftrag wird die Deaktivierung berücksichtigt.

**So ändern Sie die Priorität einer logischen Maschine**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung**.
2.  Klicken Sie auf **[+]** eines Arbeitsgangs, um die zugeordneten logischen Maschinen anzuzeigen.
3.  Markieren Sie die logische Maschine, deren Priorität Sie ändern wollen.
4.  Klicken Sie auf den **Pfeil nach oben oder den Pfeil nach unten**, um die Priorität hoch oder runter zu setzen.
    [Image: Abb. D-32 Priorität logischer Maschinen ändern. Zeigt die Pfeiltasten zur Änderung der Reihenfolge.]
5.  Klicken Sie auf **[Übernehmen]**, um die Änderungen zu speichern. Die Änderung der Priorität wird gespeichert.

### Übungen zur Arbeitsgangzuordnung

Festigen Sie Ihr neu erworbenes Wissen mit nachfolgenden Übungen.
*   Legen Sie testweise Übungsmaschinen, logische Übungsmaschinen und Übungsarbeitsgänge an.
    *   Ordnen Sie die testweise erstellten logischen Maschinen und Arbeitsgänge einander zu.
    *   Spielen Sie verschiedene Szenarien durch und vergeben Sie Prioritäten, um Arbeitsgänge auf der günstigsten Maschine durchzuführen, oder um mehrere Arbeitsgänge auf einem CNC-Center durchzuführen.
*   Betrachten Sie die gegenwärtige Situation Ihres Maschinenparks und der angelegten Maschinen, logischen Maschinen und Arbeitsgänge. Notieren Sie sich, welche Arbeitsgangzuordnung bei den momentanen Aufträgen sinnvoll ist und welche Prioritäten Sie vergeben müssen, um ein optimales Ergebnis zu erzielen.

**Ergänzende Informationen**
*   Softwarereferenz, "Neuer Arbeitsgang"
*   Softwarereferenz, "Arbeitsgang"

### Bedingungen, Formeln, Restriktionen

**Lernziele**
*   Wo werden Formeln und Bedingungen eingesetzt?
*   Wie werden Formeln und Bedingungen ausgewählt?
*   Warum ist von Formeln und Bedingungen die Rede und wo liegt der Unterschied?

**Nutzen**
*   Mit Formeln und Restriktionen werden Maschinen, logische Maschinen und Arbeitsgänge genauer definiert.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Formeln** | Formeln kommen bei Maschinen, logischen Maschinen und Arbeitsgängen zum Einsatz. Formeln sind bereits vordefiniert oder können mit dem grafischen Formeleditor oder mit dem Text-Formeleditor definiert werden. Formeln werden verwendet, um Restriktionen von Maschinen, logischen Maschinen und Arbeitsgängen exakter zu definieren. Formeln sind Restriktionen oder Bedingungen, die in der Datenbanksprache SQL ausgedrückt werden können. |
| **Formeleditor** | Der Formeleditor ist ein Werkzeug, das es dem Anwender ermöglicht, Restriktionen selbst zu formulieren. |

#### Bedingungen und Formeln in der Maschinenzuordnung

In dieser Lerneinheit erfahren Sie, wie Sie Formeln/Bedingungen auswählen.

In der Maschinenzuordnung können Formeln und Bedingungen zu Maschinen, logischen Maschinen und Arbeitsgängen hinzugefügt werden. Im Zusammenhang mit Formeln ist oftmals auch die Rede von Restriktionen und Bedingungen. In A+W Production besteht zwischen Formeln, Restriktionen und Bedingungen folgender Zusammenhang:
*   Maschinen, logische Maschinen und Arbeitsgänge haben bestimmte Eigenschaften, die oftmals restriktiv sind. So können zum Beispiel Schneidtische nur Scheiben bis zu einer bestimmten Größe bearbeiten. Für einen Teil der gängigen Restriktionen gibt es zum Beispiel im Dialog *Maschine* vordefinierte Felder. Die Werte, die Sie dort festlegen, werden in den Stammdaten als Formel hinterlegt.
*   Darüber hinaus gibt es jeweils im Feld *Zusätzliche Bedingung* die Möglichkeit, selbst definierte Formeln zu hinterlegen. Sie haben damit einen höheren Freiheitsgrad, um Sachverhalte abzubilden, die genau auf Ihre Produktion zutreffen.

> **Anlegen von Formeln**
> Bei Fragen zur Erstellung und Änderung von Formeln wenden Sie sich bitte an den Support der A+W Software GmbH. Zum Anlegen und Verwalten von Formeln besteht ein separates Tutorial.

### Bedingung auswählen

Sie können eine Bedingung in den Eigenschaften der Maschinen, logischen Maschinen oder Arbeitsgängen auswählen. Die Formeln für eine Bedingung bearbeiten Sie im Formel-Editor.

**So wählen Sie eine Bedingung aus**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Logische Maschinen**. (Die Beschreibung gilt analog auch für Maschinen und Arbeitsgänge.)
2.  Markieren Sie die Logische Maschine und klicken Sie auf **[Bearbeiten]**.
3.  Klicken Sie im Bereich *Zusätzliche Bedingung* die **[Lupe]**, um eine Bedingung auszuwählen.
    [Image: Abb. D-33 Bedingung auswählen. Screenshot des Dialogs 'Bedingung auswählen' mit einer Liste von Bedingungen.]
4.  Markieren Sie die Bedingung, die Sie übernehmen wollen. Wenn zu der Bedingung eine Formel angelegt ist, wird der Inhalt im Feld *Text* angezeigt.
5.  Klicken Sie auf **[OK]**, um die Bedingung zu übernehmen. Die Bezeichnung wird im Bereich *Zusätzliche Bedingung* angezeigt.
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Um die Formel zu bearbeiten, müssen Sie in den Formel-Editor wechseln.

### Formel zur Bearbeitungsdauer einer logischen Maschine auswählen

Sie können eine Formel zur Bearbeitungsdauer direkt in den Eigenschaften der logischen Maschinen auswählen. Die Formeln für eine Bedingung bearbeiten Sie im Formel-Editor.

Alternativ dazu können Sie die Bearbeitungsdauer einer logischen Maschine kann auch in der A+W Production Kapazitätsplanung erstellen oder bearbeiten.

**So wählen Sie eine Formel für die Bearbeitungsdauer aus**
1.  Wählen Sie **Stammdaten > MZO > MZO-Editor > Logische Maschinen**.
2.  Markieren Sie die Logische Maschine und klicken Sie auf **[Bearbeiten]**.
    [Image: Abb. D-34 Logische Maschine. Screenshot des Dialogs 'Logische Maschine', das Feld 'Bearbeitungsdauer' ist hervorgehoben.]
3.  Klicken Sie auf **[...]** (B).
    [Image: Abb. D-35 Formel-Auswahl. Screenshot des Dialogs 'Formel-Auswahl' mit einer Liste verfügbarer Formeln.]
4.  Wählen Sie im Dialog *Formel-Auswahl* eine Formel aus.
5.  Klicken Sie auf **[OK]**, um die Formel in die Eigenschaften der Logische Maschine zu übernehmen. Die Formel wird in der Zeile *Bearbeitungsdauer* angezeigt.
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Sie können die Formel bearbeiten, indem Sie auf **[Editieren]** klicken. Zu den Formeln finden Sie eine ausführliche Beschreibung in der Dokumentation zum Part Formeln.

### Übungen zum Auswählen von Bedingungen

Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
*   Notieren Sie sich, in welchen Dialogen in der Maschinenzuordnung Sie Bedingungen auswählen können.
*   Bilden Sie auf Papier den Maschinenpark Ihres Betriebes ab, mit den dazu gehörigen Maschinen, logischen Maschinen und Arbeitsgängen. Oder verwenden Sie bereits bestehende Notizen.
    *   Welche Bedingungen sind in Ihrem Maschinenpark und bei der aktuellen Auftragssituation sinnvoll?
    *   Welche Auswirkungen hätten die Bedingungen auf die jeweils anderen Bereiche der Maschinenzuordnung?

**Ergänzende Informationen**
*   Softwarereferenz, "Bedingung auswählen"
*   Softwarereferenz, "Auswahl Bedingungen"

### Bearbeitungstypen und Bearbeitungsartikel

**Lernziele**
*   Was sind Bearbeitungstypen in A+W Production und speziell in der Maschinenzuordnung?
*   Wie werden Bearbeitungstypen angelegt, bearbeitet oder gelöscht?
*   Wann können Bearbeitungstypen nicht gelöscht werden?
*   Was sind Bearbeitungsartikel in A+W Production und speziell in der Maschinenzuordnung?
*   Wie werden Bearbeitungsartikel angelegt, bearbeitet oder gelöscht?

**Nutzen**
*   Arbeitsgänge können auf Basis von Bearbeitungstypen oder Bearbeitungsartikeln definiert werden.
*   Ist einem Arbeitsgang ein Bearbeitungstyp hinterlegt, beschreibt dieser, um welche technische Form einer Bearbeitung es sich handelt, zum Beispiel *Zuschnitt*.
*   Ist ein Bearbeitungsartikel hinterlegt, beschreibt dieser, um welche technische Form der Bearbeitung es sich handelt, jedoch konkreter als beim Bearbeitungstyp. So wird mit einem Bearbeitungsartikel ein Arbeitsgang z. B. als *Facetten-Schleifen* definiert.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Bearbeitungstypen** | Bearbeitungstypen beschreiben, um welche technische Form einer Bearbeitung es sich handelt. Bearbeitungstypen sind vom Anwender definierte Bearbeitungen. Demgegenüber gibt es noch den vordefinierten Katalog der A+W Software GmbH. |
| **Bearbeitungsartikel** | Bearbeitungsartikel definieren konkreter als ein Bearbeitungstyp, um welche technische Form der Bearbeitung es sich handelt. |

#### Bearbeitungstypen in der Maschinenzuordnung

Mit einem Bearbeitungstyp wird beschrieben, um welche technische Form der Bearbeitung es sich handelt. So wird zum Beispiel definiert, ob es sich um *Zuschnitt*, *Montage*, *Säumen*, *Schleifen* oder *Verpacken* handelt.

Arbeitsgänge werden auf Basis von Bearbeitungstypen definiert. Der Arbeitsgang bringt dabei die Eigenschaften des Werkstücks mit den Eigenschaften des Bearbeitungstyps zusammen.

[Image: Abb. D-36 Bearbeitungstyp als Basis eines Arbeitsgangs. Ein Diagramm, das zeigt, wie verschiedene Bearbeitungstypen (Säumen, Zuschnitt, Schleifen, Polieren) als Basis für einen neuen Arbeitsgang dienen können.]

Bearbeitungstypen sind von der A+W Software GmbH vordefiniert, können aber auch selbst definiert werden.

[Image: Abb. D-37 Bearbeitungstypen. Screenshot des Dialogs 'Bearbeitungstypen' mit einer Liste von Typen und deren Eigenschaften.]

#### Bearbeitungsartikel in der Maschinenzuordnung

Bearbeitungsartikel referenzieren auf Bearbeitungstypen. Mit Bearbeitungsartikeln können Sie Bearbeitungstypen genauer beschreiben. Sie können zum Beispiel zum Bearbeitungstyp *Schleifen* die Bearbeitungsartikel *Facetten-Schleifen*, *Gehrungs-Schleifen*, *Kerben-Schleifen*, *Rodieren* und *Rundeck-Schleifen* anlegen und so den jeweiligen technischen Vorgang genauer definieren.

Da die Bearbeitungsartikel auf den jeweiligen Bearbeitungstyp referenzieren, können Sie Änderungen zentral vornehmen. Ändern Sie z. B. beim Bearbeitungstyp *Schleifen* die Einstellung *Zählen von Bearbeitungen*, ändert sich diese Einstellung auch bei allen zugehörigen Bearbeitungsartikeln.

[Image: Abb. D-38 Bearbeitungsartikel als Basis eines Arbeitsgangs. Ein Diagramm zeigt, wie verschiedene Bearbeitungsartikel (Gehrung-, Facetten-, Kerben-Schleifen) als Basis für einen neuen Arbeitsgang 'Facetten-Schleifen' dienen.]

In diesem Beispiel sehen Sie, wie Arbeitsgänge auf Basis von Bearbeitungsartikeln definiert werden können. Der Arbeitsgang bringt dabei die Eigenschaften des Werkstücks mit den Eigenschaften des Bearbeitungsartikels zusammen.

Bearbeitungsartikel können Sie selbst definieren.

[Image: Abb. D-39 Bearbeitungsartikel. Screenshot des Dialogs 'Bearbeitungsartikel' mit einer langen Liste von Artikeln und deren zugehörigen Bearbeitungstypen.]

### Bearbeitungstypen anlegen und verwalten

In dieser Lerneinheit erfahren Sie, wie Sie Bearbeitungstypen anlegen, bearbeiten oder löschen.

*   "So legen Sie einen Bearbeitungstyp an"
*   "So bearbeiten Sie einen Bearbeitungstyp"
*   "So löschen Sie einen Bearbeitungstyp"

> **Standard-Katalog von Bearbeitungstypen**
> In A+W Production gibt es einen Standard-Katalog von Bearbeitungstypen. Diese tragen vierstellige Nummern und dürfen vom Anwender nicht verändert oder gelöscht werden.
> Sie können weitere Bearbeitungstypen definieren. Es wird empfohlen, dabei die jeweils passenden Bearbeitungstypen aus dem Standard-Katalog als Basis zu verwenden.

**So legen Sie einen Bearbeitungstyp an**
1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungstypen**.
    [Image: Abb. D-40 Bearbeitungstyp anlegen. Screenshot, der zeigt, wie ein neuer Bearbeitungstyp auf Basis eines bestehenden angelegt wird.]
2.  Markieren Sie den Bearbeitungstyp (A), der dem neuen Bearbeitungstyp als Basis dienen soll.
3.  Klicken Sie auf **[Neu]** (B). Die Eingabefelder (C) werden freigeschaltet.
4.  Geben Sie die Daten ein.
5.  Klicken Sie auf **[Speichern]**, um den neuen Bearbeitungstyp zu speichern.

**So bearbeiten Sie einen Bearbeitungstyp**
1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungstypen**.
2.  Markieren Sie den Bearbeitungstyp, den Sie bearbeiten möchten (A).
    [Image: Abb. D-41 Bearbeitungstyp bearbeiten. Screenshot, der zeigt, wie ein bestehender Bearbeitungstyp zur Bearbeitung ausgewählt wird.]
3.  Klicken Sie auf **[Ändern]** (B). Die Eingabefelder des Bearbeitungstyps werden freigeschaltet und können bearbeitet werden (C).
4.  Geben Sie die Daten ein.
5.  Klicken Sie auf **[Speichern]**, um die Änderungen zu speichern.

**So löschen Sie einen Bearbeitungstyp**

> **Voraussetzung**
> Bearbeitungstypen können nicht gelöscht werden, wenn sie einem Bearbeitungsartikel zugeordnet sind. In diesem Fall erscheint eine Fehlermeldung. Lösen Sie vor dem Löschen von Bearbeitungstypen die Zuordnung auf.

1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungstypen**.
2.  Markieren Sie den Bearbeitungstyp, den Sie löschen möchten.
3.  Klicken Sie auf **[Löschen]**. Es erscheint eine Sicherheitsabfrage.
4.  Klicken Sie auf **[Yes]**, um den Bearbeitungstyp zu löschen.

### Bearbeitungsartikel anlegen und verwalten

In dieser Lerneinheit erfahren Sie, wie Sie Bearbeitungsartikel anlegen, bearbeiten oder löschen und wie Sie die Zuordnung eines Bearbeitungstyps zu einem Bearbeitungsartikel auflösen.

*   "So legen Sie einen Bearbeitungsartikel an"
*   "So bearbeiten Sie einen Bearbeitungsartikel"
*   "So lösen Sie die Zuordnung eines Bearbeitungstyps zu einem Bearbeitungsartikel auf"
*   "So löschen Sie einen Bearbeitungsartikel"

**So legen Sie einen Bearbeitungsartikel an**
1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungsartikel**.
    [Image: Abb. D-42 Bearbeitungsartikel anlegen. Screenshot, der zeigt, wie ein neuer Bearbeitungsartikel auf Basis eines bestehenden angelegt wird.]
2.  Markieren Sie den Bearbeitungsartikel (A), der dem neuen Bearbeitungsartikel als Basis dienen soll.
3.  Klicken Sie auf **[Neu]** (B). Die Eingabefelder (C) werden freigeschaltet und können bearbeitet werden.
4.  Geben Sie die Daten ein.
5.  Klicken Sie auf **[Speichern]**, um den neuen Bearbeitungsartikel zu speichern.

**So bearbeiten Sie einen Bearbeitungsartikel**
1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungsartikel**.
2.  Markieren Sie den Bearbeitungsartikel (A), den Sie bearbeiten möchten.
3.  Klicken Sie auf **[Ändern]** (B). Die Eingabefelder (C) werden freigeschaltet und können bearbeitet werden.
    [Image: Abb. D-43 Bearbeitungsartikel anlegen. (Anmerkung: Bildtitel scheint falsch, zeigt Bearbeitung). Screenshot, der zeigt, wie ein bestehender Bearbeitungsartikel bearbeitet wird.]
4.  Geben Sie die Daten ein.
5.  Klicken Sie auf **[Speichern]**, um die Änderungen zu speichern.

**So lösen Sie die Zuordnung eines Bearbeitungstyps zu einem Bearbeitungsartikel auf**
1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungsartikel**.
2.  Markieren Sie den Bearbeitungsartikel, dem Sie einen anderen Bearbeitungstyp zuordnen möchten.
3.  Klicken Sie auf **[Ändern]**. Die Eingabefelder werden freigeschaltet.
4.  Wählen Sie in der Kombobox *Bearbeitungstyp* einen anderen Bearbeitungstyp.
5.  Klicken Sie auf **[Speichern]**, um den Bearbeitungsartikel zu speichern.

**So löschen Sie einen Bearbeitungsartikel**
1.  Wählen Sie **Stammdaten > Bearbeitungen > Bearbeitungsartikel**.
2.  Markieren Sie den Bearbeitungsartikel, den Sie löschen möchten.
3.  Klicken Sie **[Löschen]**. Es erscheint eine Sicherheitsabfrage.
4.  Klicken Sie auf **[Yes]**, um den Bearbeitungsartikel zu löschen.

### Übungen zur Maschinenzuordnung

Festigen Sie mit den folgenden Übungen Ihr neu erworbenes Wissen.
Legen Sie folgende Stammdaten an:
*   Definieren Sie eine Übungsmaschine **Bohren**. Geben Sie der Bohrmaschine folgende Restriktionen:
    *   Die Bohrmaschine kann nur Scheiben ab einer Dicke von 10 mm und bis zu einer Dicke von 20 mm bearbeiten.
    *   Die Maschine kann keine Modelle bearbeiten.
    *   Die Maschine kann unstrukturierte und strukturierte Scheiben bearbeiten.
*   Definieren Sie eine Übungsmaschine **Linie**. Geben Sie der Linie folgende Restriktionen:
    *   Die Maschine kann Stufen-ISO und Normal-ISO bearbeiten.
    *   Die minimalen Scheibenabmessungen betragen 200 x 300 mm.
    *   Die maximalen Scheibenabmessungen betragen 2500 x 4000 mm.
    *   Die Maschine kann 3-fach-ISO ohne maßliche Restriktion bearbeiten.
    *   Fügen Sie eine zusätzliche Bedingung ein. Welche Auswirkungen kann eine zusätzliche Bedingung auf die Maschine haben?
*   Definieren Sie eine Übungsmaschine **CNC-Center**.
    *   Zum CNC-Center soll es zwei logische Maschinen für die Bearbeitungen *Bohren* und *Polieren* geben.
*   Definieren Sie einen Übungs-Schneidtisch, bei dem die Scheiben im Hochformat auf der Maschine stehen.
*   Definieren Sie einen Übungsarbeitsgang **Bohren**.
    *   Weisen Sie dem Arbeitsgang die Bohrmaschine und das CNC-Center zu. Die Bohrmaschine soll dabei höchste Priorität haben.
*   Definieren Sie einen Übungsarbeitsgang **Bohren auf CNC-Center**, dem Sie das CNC-Center mit höchster Priorität zuweisen. Die Bohrmaschine weisen Sie dem Arbeitsgang mit geringer Priorität für Engpässe zu.
*   Definieren Sie einen Übungsarbeitsgang, der auf einem Bearbeitungsartikel basiert.
*   Definieren Sie einen eigenen Übungsbearbeitungstyp **Bohren**.
*   Ändern Sie die Arbeitsgänge aus der Übung so, dass diese auf Ihrem eigenen Übungsbearbeitungstyp *Bohren* basieren.

### Schaltflächen in der Maschinenzuordnung

| Schaltfläche | Bedeutung |
| :--- | :--- |
| 