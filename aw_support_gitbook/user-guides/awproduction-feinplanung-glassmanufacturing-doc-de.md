---
description: "DE_AWProduction_Feinplanung_3_1"
---


# A+W Feinplanung F

---
## A+W Production
A+W - Software for Glass, Windows and Doors

## Revisionsübersicht

| Part Version / Datum | Beschreibung                                                                                |
| :------------------- | :------------------------------------------------------------------------------------------ |
| 3.00/01-2023         | Komplette Überarbeitung.                                                                    |
| 2.02/01-2017         | Produkt- und Firmennamen angepasst, Felder ergänzt.                                          |
| 2.01/07-2013         | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production.          |
| 2.00/11-2012         | Komplette Überarbeitung.                                                                    |
| 1.00/09-2007         | Ersterstellung.                                                                             |

## Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen

### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

---

## Tutorial

### Dokumentations-Hinweise

Das Tutorial zum Modul Feinplanung beschäftigt sich mit den Grundlagen des gesamten Produktionsprozesses. Angefangen vom Zuschnitt über die unterschiedlichen Produktions-Linien bis hin zu den Versandgestellen. Es baut auf den Kenntnissen der Grobplanung auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

**Themenblöcke**
Zur Schulung des Moduls Feinplanung gehören folgende Themenblöcke:
*   Gruppierungen und Sortierungen
*   Abstellplätze und -modi
*   Optimierungsmodi
*   Orgas

### Wichtige Hinweise

Diese Dokumentation ist als Unterstützung für den täglichen Arbeitsbetrieb und als Schulungsunterlage für eine begleitete Softwareschulung durch einen zertifizierten A+W Trainer zu verstehen. Sie dient nicht dem Selbststudium und kann keine 100%ig fehlerfreie Anwendung gewährleisten, da die Komplexität nicht von der Software sondern von den realen Arbeitsprozessen abhängt. Die Feinplanung definiert die gesamten Organisations- und Produktionsabläufe in Ihrer Produktion. Sie kann daher entsprechend Ihren Anforderungen sehr komplex ausfallen und wird ausschließlich in Begleitung durch einen erfahrenen A+W-Mitarbeiter erstellt und gemeinsam mit Ihnen eingerichtet. Möchten Sie Änderungen an den Einstellungen vornehmen, wenden Sie sich vorher bitte unbedingt an A+W, da es sonst zu unerwünschten Ergebnissen kommen kann!

Der Anwender muss Kenntnisse in der Anwendung von physischen Prozessabläufen in der Glasproduktion und -organisation haben.

### Produktnamen

Im Rahmen der strategischen Produktneuausrichtung wurden das Produktportfolio A+W und die Produktnamen vereinfacht. So wurde aus ALCIM beispielsweise A+W Production.

Da im Produktentwicklungszyklus sowohl die alten Produktversionen als auch die neuen Produktversionen angepasst und erweitert wurden, verwenden wir zur Vereinfachung in diesem Dokument ausschließlich die alten Produktnamen - die neuen Produktversionen werden unter den alten Namen subsummiert.

### Dokumentation

Für die Schulung zur A+W Production stehen folgende Unterlagen zur Verfügung:

|            |                                                         |
| :--------- | :------------------------------------------------------ |
| **Handout**  | Ausdruck Schulungsunterlage für die Teilnehmer         |
| **PDF**      | Vollständige Unterlagen<ul><li>Tutorial</li><li>Softwarereferenz</li><li>Index</li></ul> |
| **Online-Hilfe `<F1>`** | Kontextsensitive Dialog-Hilfe der A+W Production-Softwarereferenz. |

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

*   **Überblick**
    Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    *   Lernziele: Was soll vermittelt werden?
    *   Nutzen: Wofür können Sie dieses Wissen einsetzen?
    *   Merksätze: Welche Zusammenhänge müssen Sie sich merken?
*   **Konzepte**
    Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
*   **Übungen**
    Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
*   **Querverweisteil**
    Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen.
    Damit können Sie das neu erworbene Wissen vertiefen.

**Lesehinweis**
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen

Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht ein roter Faden durch die gesamte Dokumentation.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

*   *Kursiv*: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Gruppierung*.
*   **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B. geben Sie den Wert **0** ein.
*   **>**: Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Stammdaten > Feinplanung > Orga*.
*   **[]**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B, mit **[OK]** speichern Sie die Daten.
*   **<>**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B. mit **<F1>** öffnen Sie die Online-Hilfe.

## Überblick Feinplanung

Das für die Produktion benötigte Glas wird in der Regel aus Lagerplatten auf den Schneidtischen zugeschnitten. Häufig gibt es in einem Unternehmen mehrere automatische Schneidtische sowie mindestens einen Schneidtisch für Handzuschnitt oder aber auch für Modelle.

Die Scheiben werden nach dem Zuschnitt, in Abhängigkeit von ihrem nächsten Bearbeitungsschritt, auf Abstellplätzen (z. B. A-Böcke) abgestellt und mit dem Abstellplatz zu ihrer nächsten Bearbeitung bewegt.

Innerhalb eines Arbeitsbereiches (bspw. Zuschnitt) oder einer Prozesskette (bspw. Zuschnitt > VSG-Linie) kann die Verweil- und Bearbeitungsdauer sehr unterschiedlich sein. Dies ist unter anderem davon abhängig wie viel Platz in diesem Bereich für Gestelle zur Verfügung steht um die Gläser abzustellen, wie kompliziert die Abstelllogik ist und wie weit die Laufwege sind. Diese Fragen sind für die Feinplanung maßgeblich. Wenn z. B. hinter dem Zuschnitt wenig Platz für Gestelle ist, muss diese Situation durch eine gute Optimierung und Sequenz der Scheiben ausgeglichen werden, so dass möglichst wenige Gestelle benötigt werden und wenig umsortiert werden muss.

Für die Montage an der ISO-Linie müssen die einzelnen Scheiben der Einheit möglichst nahe beieinander stehen. Sie müssen nicht unbedingt auf einem Gestell stehen. Das bedeutet, dass, je nach Optimierung, beim Zuschnitt vor der Linie umsortiert werden muss.

> **Optimierungsergebnis**
> Die Optimierung mit dem geringsten Verschnitt kann nicht immer oberstes Ziel der A+W Production sein. Beispielsweise wenn sie dazu führt, dass sich der Sortieraufwand vor der Montage unverhältnismäßig erhöht.

Ein wichtiges Kriterium für Feinplanungsergebnisse und die Verweil- und Bearbeitungsdauer ist die Laufgröße und -zusammenstellung. Es sind verschiedene Aspekte zu berücksichtigen:

*   Ist die Anzahl der Scheiben im Lauf zu klein oder sind nur sehr große Scheiben vorhanden, dann ist der Verschnitt zu groß. Die Lagermaße können nicht effektiv geschnitten werden, es bleibt ein zu großer Rest.
*   Ist der Lauf dagegen zu groß, d. h. er enthält sehr viele Scheiben, dann ist die Produktionszeit für den Lauf sehr hoch und die Gestelle bleiben lange belegt. Gestelle können erst wieder verwendet werden, wenn die Produktion des Laufes abgeschlossen ist.

### Ablauf der A+W Production

Die Feinplanung setzt genau dort an, wo die Grobplanung endet. Das Ergebnis der Grobplanung sind die Läufe. Läufe enthalten die zu produzierenden Teile. Aufgabe der Feinplanung ist es, für die in den Läufen enthaltenen Teile die Produktionsreihenfolge zu erstellen.

Die Produktionsreihenfolge kann sich durch folgende Kriterien ergeben:
*   Durch die Vorgaben des Kunden,
*   durch die Ergebnisse einer Packmitteloptimierung (PMO) oder
*   durch fertigungstechnische Restriktionen.

Die Feinplanung läuft in verschiedenen Schritten ab. Alle dazu notwendigen Prozesse (Daten aus der Datenbank laden, etc.) werden in A+W Production im Hintergrund abgearbeitet und sind für den Benutzer nicht sichtbar. Die Schritte bauen wie folgt aufeinander auf:

*   Im ersten Schritt werden die Daten aus der Datenbank geladen.
*   Ist dies geschehen, erstellt die Feinplanung anhand der Teile und Bearbeitungen die entsprechende Stückliste.
*   Nachdem die Stückliste erstellt ist, weist die Feinplanung die Teile den zur Verfügung stehenden Orgas und Abstellplatztypen zu.
*   Anschließend erfolgen die Gruppierungen und Sortierungen innerhalb der Orga-Gruppen und auf den Abstellplätzen.
*   Im nächsten Schritt behandelt die Feinplanung das Abstellen der Scheiben auf den Abstellplätzen.
*   Dann erfolgt die Bildung der Produktionslose.
*   Im letzten Schritt beschäftigt sich die Feinplanung mit den sogenannten Sonderteilen (Restscheiben, Füllaufträge, Bruch, etc.).

Damit die für jeden Produktionsschritt gewünschte Reihenfolge auch möglich ist, müssen die Vorprodukte auf den Abstellplätzen vor diesem Produktionsschritt in einer passenden Reihenfolge stehen. Die Belegung der Abstellplätze unmittelbar nach dem jeweiligen Produktionsschritt ist das Ergebnis der Produktionsreihenfolge.

Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen der verschiedenen Einstellmöglichkeiten in der A+W Production.

(Diagramm: Dreieck mit den Ecken Ausbeute, Reihenfolge, Flexibilität)

Sie können lediglich einen Punkt auf den Linien des Dreiecks definieren. Diesen Punkt können Sie bewegen, indem Sie mithilfe der A+W Production die Produktionseinstellungen verändern.

Sie können genau an einem Eckpunkt arbeiten und die anderen beiden außer Acht lassen. Sie können sich aber auch auf einer Seite bewegen - genau in der Mitte der beiden angrenzenden Ecken, ohne Berücksichtigung des dritten Eckpunktes. Eine Produktion unter Berücksichtigung aller drei Eckpunkte gleichzeitig ist nicht möglich.

*   Sie können mit einer strikten Reihenfolge (an einem Eckpunkt) arbeiten - dies geht zu Lasten der Flexibilität und liefert ein schlechtes Ergebnis.
*   Sie können mit einer Kombination von Reihenfolge und unbedingte Ausbeute (auf einer Seite) arbeiten - sind dann aber nicht mehr flexibel.

Wir werden dieses Schema innerhalb der Dokumentation immer wieder verwenden.

**Ergänzende Informationen**
⇨ Tutorial, "Begriffe der A+W Production" auf Seite F-16

### Begriffe der A+W Production

Innerhalb der A+W Production werden folgende Begriffe verwendet:
*   Lostyp
*   Lose
    *   Verwendungslos
    *   Produktionslos
*   Böcke (Abstellplätze)
    *   Verwendungsbock
    *   Produktionsbock
*   Läufe
*   Teilebaum
*   Organisation (Orga)

#### Lostyp

Der Lostyp wird durch die Eigenschaften Bearbeitungstyp und Beschaffungsart gebildet.

*(Abb. F-1 Schematische Darstellung der Lostypen Zuschnitt und Lagerentnahme)*

#### Lose

Ein Los ist eine Anzahl an Scheiben, welche innerhalb eines Zeitraums unter den gleichen Bedingungen auf den gleichen Maschinen verwendet oder produziert werden. Ein Los enthält eine Anzahl von Scheiben eines Lostyps. In der A+W Production gibt es zwei Arten von Lostypen:

*   Verwendungslos
*   Produktionslos

**Verwendungslos**
Scheiben eines Verwendungsloses werden zur Fertigung von in Läufen befindlichen Scheiben benötigt. Alle in diesem Los enthaltenen Scheiben haben den gleichen Lostyp.

**Produktionslos**
Scheiben eines Produktionsloses werden im dazugehörigen Lauf produziert. Alle Scheiben darin haben den gleichen Lostyp. Scheiben eines Produktionsloses werden auf den gleichen Maschinen produziert. Scheiben für eine andere Maschine kommen in ein anderes Los vom gleichen Typ. Ferner können Produktionslose noch nach weiteren Kriterien getrennt werden. So wäre es zum Beispiel denkbar, die Produktion für ISO-Einheiten nach dem Scheibenzwischenraum (SZR) zu trennen. Dadurch würden mehrere Produktionslose gebildet, von denen jedes nur Scheiben für einen bestimmten Scheibenzwischenraum enthält.

**Ergänzende Informationen**
⇨ Abb. F-2 auf Seite F-18

#### Böcke (Abstellplätze)

Teile eines Laufes können nach dem Zuschnitt unterschiedlich bearbeitet werden. Dazu werden die Teile auf Böcke (Abstellplätze) für die nächste Bearbeitung gestellt. Sie gehören immer einem Verwendungslos an, d. h. es sind Scheiben, die zur Produktion benötigt werden. Deshalb müssen sie auf den Verwendungsböcken so stehen, dass für den nächsten Bearbeitungsprozess die gewünschte Produktionsreihenfolge eingehalten werden kann.

Die A+W Production unterscheidet zwischen
*   Verwendungsbock
*   Produktionsbock

**Verwendungsbock**
Teile eines Laufes können nach dem Zuschnitt unterschiedlich bearbeitet werden. Dazu werden die Teile auf einen Verwendungsbock (Abstellplatz) für die nächste Bearbeitung gestellt. Sie gehören immer einem Verwendungslos an, d. h. es sind Scheiben, die zur Produktion benötigt werden. Deshalb müssen sie auf den Verwendungsböcken so stehen, dass für den nächsten Bearbeitungsprozess die gewünschte Produktionsreihenfolge eingehalten werden kann.

*(Abb. F-2 Übersicht Produktions- und Verwendungsbock)*

**Produktionsbock**
Auf dem Produktionsbock werden Scheiben unmittelbar nach ihrer Produktion abgestellt. Sie stehen auf dem Bock in der Reihenfolge, in der sie aus der Produktion kamen. Es handelt sich dabei stets um Scheiben in einem Produktionslos. Produktionsböcke müssen in der A+W Production nicht zwingend verwendet werden, man kann die Scheiben nach der Produktion auch direkt auf einen Verwendungsbock für die nächste Bearbeitung stellen.

> **Produktions- und Verwendungsböcke**
> In der A+W Production kann für jeden Bearbeitungsschritt eine unterschiedliche Gruppierung/Sortierung verwendet werden. Es ist nicht möglich, einem Produktionsbock einfach eine andere Nummer zu geben und ihn als Verwendungsbock für den nächsten Bearbeitungsschritt zu nehmen. Wenn Scheiben direkt nach der Bearbeitung statt auf einem Produktionsbock auf einen Verwendungsbock gestellt werden, müssen sie so angeordnet werden, dass die Produktionsreihenfolge des nächsten Bearbeitungsschritts eingehalten werden kann.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite F-135

#### Läufe

Läufe enthalten eine Menge von Auftragspositionen, die gemeinsam für die Produktion frei gegeben und gemeinsam produziert werden.

**Läufe archivieren**
Läufe, die Sie nicht mehr im Produktionssystem benötigen, können archiviert werden. In der Anzeige *Läufe* können Sie über das Kontextmenü (*Lauf verwalten > Lauf archivieren*) den ausgewählten Lauf bzw. die ausgewählten Läufe auf archivierbar setzen. Archivierte Läufe erhalten dann den Laufstatus 2000.

Es gibt 2 Arten der Archivierung:
*   Manuelle Archivierung
*   Automatische Archivierung

**Manuelle Archivierung**

Die Einstellungen für die manuelle Archivierung befinden sich im Parameter-Administrator unter:
*Parameter > A+W Production > Allgemein > ALCIM Server > Automatische Laufarchivierung*

Der Eintrag für die manuelle Archivierung ist die **0**.

Nachdem der Lauf archiviert wurde, hat er den Status archivierbar. Ob ein Lauf tatsächlich archiviert wird oder stattdessen gelöscht werden soll, kann in der Systemkonfiguration definiert werden. Zum Archivieren eines Laufes ist eine Archivdatenbank und ein Prozess (ALCIM Server) notwendig. Dieser Prozess kann manuell gestartet werden oder ist als Automatismus im Hintergrund konfiguriert.

**■ So archivieren Sie einen Lauf**
1.  Öffnen Sie die Ansicht *Läufe*.
2.  Markieren Sie den Lauf, den Sie archivieren oder löschen möchten.
3.  Öffnen Sie das Kontext-Menü und wählen Sie *Lauf verwalten > Lauf archivieren*.
4.  Es folgt eine Sicherheits-Abfrage, ob Sie den Lauf wirklich archivieren möchten.
5.  Klicken Sie auf **[OK]** um den Lauf zu archivieren.
6.  Anschließend hat der Lauf den Status archivierbar.

**Automatische Archivierung**

Neben der manuellen Archivierung gibt es 3 weitere Archivierungsmodi, die sich auf die Laufstati produziert (700), verpackt (800) und versendet (900) beziehen. Diese Laufstati werden automatisch vom AlcimBooking gesetzt, sobald alle Kopfteile in dem Lauf die Bearbeitungen für produziert, verpackt oder versendet erhalten haben.

Die Einstellungen für die automatische Archivierung befinden sich im Parameter-Administrator unter:
*Parameter > A+W Production > Allgemein > ALCIM Server > Automatische Laufarchivierung*

Hier können Sie unterscheiden zwischen:
*   Läufe werden automatisch archiviert, wenn der Status **produziert** erreicht ist.
*   Läufe werden automatisch archiviert, wenn der Status **verpackt** erreicht ist.
*   Läufe werden automatisch archiviert, wenn der Status **versendet** erreicht ist.

> **Buchungsdisziplin**
> Die automatische Archivierung basiert auf BDE-Buchungen und ist daher von der Buchungsdisziplin abhängig. Sobald ein Kopfteil in einem Lauf nicht den entsprechenden Status erreicht, kann der Laufstatus nicht gesetzt und damit die automatische Archivierung angestoßen werden. Insofern ist darauf zu achten, dass besonders die Kopfteile vollständig gebucht werden.
> Grundsätzlich gilt: eine vollständige Archivierung eines Laufes kann erst erfolgen, wenn abhängige Läufe (enthalten gemeinsame Auftragspositionen) sich ebenfalls in diesem Satus befinden.

**Archivierungsmethode**
In diesem Bereich wählen Sie, mit welcher Archivierungsmethode gearbeitet werden soll. Es steht die alte Archivierungsmethode (die standardmäßig eingestellt ist und verwendet wird) zur Verfügung und der neuen erweiterten, der weniger restriktiv ist und es erlaubt, mehr Läufe zu archivieren und freizugeben.

Die Einstellungen für die Archivierungsmethode befinden sich im Parameter-Administrator unter:
*Parameter > A+W Production > Allgemein > ALCIM Server > Archivierungsmethode*

Hier können Sie unterscheiden zwischen:
**0: Standard-Archivierungsmethode.** Diese Methode arbeitet nur aufgrund des Status eines Laufes.
**1: Erweiterte Prüfung der Läufe.** Hier werden zusätzlich Flags der Aufträge in einem Lauf berücksichtigt, um zu prüfen, ob ein Auftrag archiviert werden kann. Diese Methode ist weniger restriktiv als die ursprüngliche Methode und erlaubt es, mehr Läufe zu archivieren und freizugeben. Der dieser Methode zugrunde liegende Parameter sagt dem AlcimServer, ab welchem Status ein Lauf als archivierungsfähig betrachtet werden soll. Der Wert der *Automatische Laufarchivierung* kann sein:
*   1=Status 700 (produziert),
*   2=Status 800 (verpackt),
*   3=Status 900 (geliefert) oder
*   0=Status 2000 (manuell als archivierbar gesetzt)

⇨ Tutorial, "Automatische Archivierung" auf Seite F-19

**Funktionsweise Standard Archivierungsmethode (0)**

Wie bereits oben erwähnt, arbeitet die Standard-Methode nur aufgrund des Status eines Laufes. Im folgenden Beispiel wird dies deutlich:
*   Lauf: 1000
*   Status: 900 (versendet)
*   Konfigurationsparameter Automatische Laufarchivierung: 3 (Läufe werden automatisch archiviert, wenn Status versendet erreicht ist)

*(Abb. F-3 Standard-Archivierungsmethode)*

Funktionsweise: Wenn der AlcimServer den Lauf 1000 (Spalte A) mit einem Status gleich oder größer als 3 (Status 900, versendet) verarbeitet, prüft er im 1. Schritt alle Aufträge des Laufes 1000 (Spalte D). Im 2. Schritt prüft er, in welchen anderen Läufen diese enthalten sind (Spalte F) und im 3. Schritt, ob die Läufe alle einen Status gleich oder größer Status 3 haben.

In Beispiel oben kann der Auftrag 2000001 nicht archiviert werden. Er enthält neben Lauf 1001 noch Lauf 1002 und dieser Lauf hat nur den Status 700 (produziert). Da dieser kleiner als "Archivierbarer Status" ist, kann auch Lauf 1000 nicht archiviert werden

**Funktionsweise Erweiterte Archivierungsmethode (1)**

Diese neue Methode wurde geschaffen, um mehr Läufe archivieren zu können.
Die Methode ermöglicht die Archivierung von Aufträgen, die als abgeschlossen betrachtet werden können, auch wenn sie in einem anderen Lauf mit einem Status niedriger als *Archivierbarer Status*, aber mit einem Status gleich oder höher als 700 (produziert) enthalten sind.

Beispiel:
*   Lauf: 1000
*   Status: 900
*   Konfigurationsparameter Automatische Laufarchivierung: 3 (Läufe werden automatisch archiviert, wenn Status versendet erreicht ist)

*(Abb. F-4 Erweiterte Archivierungsmethode (1))*

Wenn der Status des Laufes 700 oder größer ist und kleiner als *Archivierbarer Status*, dann müssen auch andere Datensätze aus `pool_teile` und `pool_auftrag` zusätzlich analysiert werden.

Ein Teil eines Auftrags 2000001 [Spalte D], der in dem Lauf 1001 [Spalte F] enthalten ist, muss nicht analysiert werden, da der Status [Spalte G] dieses Laufes gleich oder größer als *Archivierbarer Status* ist.

Aber ein anderer Teil des Auftrags 2000001 [Spalte D], der in dem Lauf 1002 [Spalte F] enthalten ist, muss analysiert werden, weil der Status [Spalte G] dieses Laufes 700 oder größer und kleiner als *Archivierbarer Status* ist.

Wie man im Vergleich zur Standardmethode sehen kann, berücksichtigt die neue Methode den Auftrag 2000001 [Spalte D] als archivierbar und somit kann der Lauf 1000 archiviert werden.

#### Teilebaum

Der Teilebaum beschreibt den Aufbau und die Produktionsschritte für ein Produkt. Das fertige Produkt (ISO) bildet dabei den Kopf des Teilebaums, seine zur Produktion benötigten Unterteile (ESG und Float) werden im Teilebaum darunter angeordnet, deren Unterteile (Float) wiederum darunter. Dies wird solange fortgesetzt, bis die Basisteile (in der Regel Float) erreicht sind. Im Teilebaum befinden sich nicht nur Teile, sondern auch deren Bearbeitungen.

*(Abb. F-5 Teilebaum)*

#### Organisation (Orga)

Um einen Lauf korrekt und effizient planen zu können, stehen Ihnen in A+W Production sogenannte Orgas zur Verfügung. Eine Orga ist nichts anderes als ein datentechnisches Regelwerk zur Abbildung der Produktion. In Abhängigkeit von der Struktur des Unternehmens können beliebig viele Orgas (ESG-Orga, ISO-Orga, Bearbeitungs-Orga, etc.) definiert werden. Die unterschiedlichen Orgas organisieren die Abstellplätze jeweils vor den Produktionsschritten (ISO-Linie, Ofen, etc.).

*(Abb. F-6 Schematische Darstellung der Organisation)*

## Gruppierungen und Sortierungen

In diesem Themenblock lernen Sie die unterschiedlichen Gruppierungen und Sortierungen kennen und erfahren, wie Sie damit in der A+W Production umgehen.

Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Einführung
*   Gruppierung
*   Sortierung
*   Zusatz-Sortierung
*   Demos und Übungen

### Überblick

**Lernziele**
*   Gruppierungen kennenlernen und verstehen.
*   Sortierungen kennenlernen und verstehen.
*   Zusatz-Sortierungen kennenlernen und verstehen.
*   Die Auswirkungen von Gruppierungen und Sortierungen verstehen.

**Nutzen**
Über die Gruppierungen und Sortierungen wird das Abstellen der einzelnen Scheiben in der von Ihnen gewünschten Reihenfolgen organisiert. Ohne diese Gruppierungen und/oder Sortierungen müssten die Scheiben vor dem jeweiligen nächsten Produktionsschritt immer neu sortiert werden.

**Definitionen**
*   **Gruppierung**: Erfolgt nach unterschiedlichen und eindeutigen Werten für eine Eigenschaft, z. B. nach Kundennummer, Glasdicke.
*   **Sortierung**: Erfolgt nach Eigenschaften, die einen fortlaufenden Wert innerhalb der gegebenen Gruppe annehmen.
*   **Abstellplatz**: Gestell (A-Bock, Fächerwagen, Fester Abstellplatz)
*   **Bock**: Umgangssprachlich für Abstellplatz.

> **Merke**
> **Bildung**: Gruppierungen oder Sortierungen werden durch eine beliebige Kombination aus Eigenschaften und Formeln gebildet.

### Einführung

Die Gruppierungen und Sortierungen dienen dazu, den verschiedenen Abstellplätzen die gewünschte Produktionsreihenfolge zuzuweisen. Gruppierungen können auch verwendet werden, um Scheiben vom gleichen Lostyp auf verschiedene Produktionslose zu verteilen.

A+W Production erlaubt es Ihnen, Gruppierungskriterien zu definieren und gibt Ihnen die Möglichkeit zu entscheiden, ob die Gruppierung in einer gewissen Reihenfolge (sortierte Gruppen) sein soll und ob die Inhalte der Gruppen sortiert sein sollen (Sortierung innerhalb der Gruppe). Jeder Abstellplatztyp innerhalb einer Organisation kann seine eigene Gruppierung und Sortierung haben.

Die Optimierung berechnet unter Berücksichtigung von Gruppierung und Sortierung den bestmöglichen Verschnitt. Einmal eingerichtet, kann die so ermittelte Reihenfolge für passende Scheiben einer ISO- und VSG-Einheit verwendet werden.

Jede Scheibe bzw. jede Bearbeitung hat eine Anzahl von Eigenschaften, die entweder durch die entsprechenden Felder in der Datenbank gefüllt oder berechnet werden.

*(Abb. F-7 Gruppierung und Sortierung)*

Die Grafik oben zeigt eine Gruppierung nach der Glasdicke. Innerhalb jeder Gruppe (eventuell ein Gestell pro Dicke) erfolgt die Sortierung nach der Höhe.

Gruppierung und Sortierung hängen davon ab, wie die Produktion in Ihrem Hause aufgebaut ist und abläuft. Sie werden durch eine beliebige Kombination aus Eigenschaften und Formeln gebildet. Die Einstellungen werden im Menü *Stammdaten*, in den Untermenüs *Orga, Gruppierung und Abstellplätze* vorgenommen.

**Ergänzende Informationen**
⇨ Tutorial, "Gruppierung" auf Seite F-24
⇨ Tutorial, "Sortierung" auf Seite F-25

### Gruppierung

Gruppiert wird nach unterschiedlichen und eindeutigen Werten für eine Eigenschaft wie z.B. nach *Kundennummer, Glasdicke/-farbe, Modelltyp*. Es kann nach unterschiedlichen Kriterien gruppiert werden, ohne dass innerhalb der Gruppen eine Sortierung vorhanden sein muss. Jede Gruppe enthält ausschließlich Elemente, die die Eigenschaften des Gruppierungsschlüssels enthalten. Gruppen müssen während des Laufs durch die Produktion zusammengehalten werden.

Die entsprechenden Einstellungen werden im Dialog *Gruppierung/Sortierung* gemacht:
*Stammdaten > Feinplanung > Gruppierung*

*(Abb. F-8 Gruppierung)*

**■ So legen Sie eine neue Gruppierung an**
1.  Wählen Sie im Menü *Stammdaten > Feinplanung > Gruppierung*. Der Dialog *Gruppierung/Sortierung* wird geöffnet. Das Register *Sortierung* wird automatisch geöffnet.
2.  Markieren Sie im linken Bereich den Eintrag *Gruppierungen*.
3.  Über die Checkboxen *Eigenschaft* und *Formel* bestimmen Sie, ob es sich bei der Sortierung um eine Eigenschaft oder eine Formel handelt.
4.  Wählen Sie die entsprechende Eigenschaft oder Formel aus.
5.  Betätigen Sie die Schaltfläche **[Hinzufügen]**.
6.  Der Eintrag wird der Liste auf der linken Seite am Ende hinzugefügt. Die erstellte Gruppierung kann nun für Einstellungen in den Orgas genutzt werden.

**Ergänzende Informationen**
⇨ Tutorial, "Einführung" auf Seite F-23
⇨ Softwarereferenz, "Gruppierung/Sortierung - Dialog" auf Seite F-140

### Sortierung

Sortiert werden kann nach Eigenschaften, die einen fortlaufenden Wert annehmen. Eine typische Art der Sortierung ist z. B. nach Größe. Sortiert wird innerhalb der gegebenen Gruppen. Die Sortierungen können noch bei Bedarf durch die Werte im letzten Teil des Sortierungsschlüssel verfeinert werden.

*(Abb. F-9 Gruppierung und Sortierung)*

Wie Sie an der Grafik oben erkennen können, können Sie auch eine Reihenfolge von Gruppen definieren.

> **Supergruppen**
> Die Optimierung verwendet den Begriff Supergruppe. Eine Supergruppe kann sich aus Scheiben zusammensetzen, die alle identisch bzgl. des Gruppierungsschlüssel oder des kombinierten Gruppierungs-/Sortierungsschlüssel sind.

Die Scheiben innerhalb einer Gruppe können, müssen aber nicht sortiert sein.

Die entsprechenden Einstellungen werden im Dialog *Gruppierung/Sortierung* gemacht:
*Stammdaten > Feinplanung > Gruppierung > Register Sortierung*

*(Abb. F-10 Sortierung)*

**■ So legen Sie eine neue Sortierung an**
1.  Wählen Sie im Menü *Stammdaten > Feinplanung > Gruppierung*. Der Dialog *Gruppierung/Sortierung* wird geöffnet. Wechseln Sie in das Register *Gruppierung*.
2.  Markieren Sie im linken Bereich den Eintrag *Sortierung*.
3.  Über die Checkboxen *Eigenschaft* und *Formel* bestimmen Sie, ob es sich bei der Gruppierung um eine Eigenschaft oder eine Formel handelt.
4.  Wählen Sie die entsprechende Eigenschaft oder Formel aus.
5.  Betätigen Sie die Schaltfläche **[Hinzufügen]**.
6.  Der Eintrag wird der Liste auf der linken Seite am Ende hinzugefügt.

**■ So fügen Sie einer bestehenden Sortierung eine Eigenschaft hinzu**
1.  Wählen Sie in der Menü-Leiste *Stammdaten > Feinplanung > Gruppierung > Editor-Sortierung*.
2.  Aktivieren Sie die Radiotaste *Eigenschaften*.
3.  Markieren Sie im rechten Fenster die für die Sortierung gewünschte Eigenschaft.
4.  Markieren Sie im linken Fenster die Sortierung, der die Eigenschaft hinzugefügt werden soll.
5.  Betätigen Sie die Schaltfläche **[Hinzufügen]**. Die neu hinzugefügte Eigenschaft erscheint in der bereits angelegten.

**■ Einen neuen Modus für die Gruppenbildung erstellen**
Als Beispiel wird hier eine Gruppierung nach Anzahl der Scheiben pro Kunde erstellt. Das bedeutet es wird eine Gruppe pro Kunde erstellt und diese Gruppen nach der Zahl der in ihnen enthaltenen Scheiben sortiert. Zuerst produziert wird dann die Gruppe mit der größten Anzahl an Scheiben:
1.  Wählen Sie in der Menü-Leiste *Stammdaten > Feinplanung > Gruppierung*
2.  Aktivieren Sie die Radiotaste *Formel* und betätigen Sie anschließend die Schaltfläche **[Formeln ...]**. Es öffnet sich der Dialog *Auswahl Formeln --1--*
3.  Wählen Sie die Schaltfläche **[Neue Formel ...]**. Es öffnet sich der Dialog *Formel Editor*.
4.  Im Formeleditor geben Sie jetzt oben links den Namen der Gruppierung ein (für unser Beispiel: Menge der Scheiben pro Kunde).
5.  Im Bereich *Vorhandene Formeln* suchen Sie *Menge* und klicken doppelt darauf. Die Formel `#Menge#` wird in den Bereich *Formel* übernommen.
6.  Wählen Sie die Schaltfläche **[Menge]**. Es öffnet sich der Dialog *Auswahl Mengen -- 1 --*.
7.  In diesem Dialog können links oben schon gebildete Mengen (im Sinne der Mengenlehre) ausgewählt werden. Wir bilden eine neue Menge und klicken auf **[Neue Menge ...]**. Es öffnet sich der Dialog *Mengen - Erzeuger*.
8.  Wir beginnen die Mengen - Erzeugung mit einer gegebenen Menge und bekommen nach den Mengenoperationen, die wir hier durchführen, unsere gewünschte endgültige Menge. An den Formelinterpreter wird von der Feinplanung an Werten übergeben eine Position eines bestimmten Kunden, die Mengenkalkulation der Feinplanung und als weiteren Parameter alle Aufträge des aktuellen Laufs. Von uns muss nur noch die Kundennummer hinzugefügt werden. Wählen Sie *Menge > Name*. Es öffnet sich der Dialog *Name der Menge*. Sie geben im Bereich *Neue Bezeichnung* einen sprechenden Namen für die Menge an. Wählen Sie **[OK]**. Der Dialog wird geschlossen.
9.  Wählen Sie *Menge > Übergebene Menge*. Dies bewirkt, dass bei der Bildung unserer Menge nicht nur die Position, mit der wir in *Mengen - Erzeuger* gekommen sind, selbst berücksichtigt wird, sondern alle Positionen des Laufs.
10. Da die gewünschte Menge nicht alle Teile enthalten soll, sondern nur die Freigabeteile, aktivieren Sie die Checkbox *Master*. Für Erklärungen zu den anderen Möglichkeiten siehe
11. Um unserer Menge die Kundennummer als Eigenschaft hinzuzufügen, wählen Sie *Menge > Formel*. Es öffnet sich der Dialog *Auswahl Formeln --2--*. Der Bereich *Vorhandene Formeln* gibt Ihnen wieder einen Überblick zu allen bereits definierten Formeln. Sollte die Kundennummer hier noch nicht vorhanden ist, klicken Sie auf **[Neue Formel ...]**. Es öffnet sich der Dialog *Formel - Editor*. Geben Sie im Formel-Editor einen Namen für die Formel ein, wählen Sie aus dem Bereich *Vorhandene Eigenschaften KUNDENNUMMER* aus klicken diese Eigenschaft doppelt an. Die Eigenschaft erscheint dann im Bereich *Formel*. Betätigen Sie **[OK]**, um die Formel zu erstellen.
12. Schließen Sie den Dialog *Auswahl Formeln --2--* ebenfalls mit **[OK]**.
13. Im Dialog *Mengen-Erzeuger* wird jetzt unten rechts angezeigt, dass wir diese Formel bei der Bildung der neuen Menge benutzen. Bei der Bildung der gewünschten Menge benutzen wir keine Bedingung. Bedingungen werden auch über den Menüpunkt *Menge* gebildet. Der Unterschied von Formel und Bedingung bei Mengenoperationen besteht darin, dass eine Bedingung immer einen absoluten Wert enthält, während sich dieser bei der Formel auf eine bestimmte Position bezieht und so unterschiedliche Werte annehmen kann.
14. Schließen Sie jetzt alle geöffneten Dialoge mit **[OK]**, bis Sie sich wieder im Ausgangsdialog *Gruppierung/Sortierung* befinden. Dort markieren Sie die neue Formel (*Menge der Scheibe pro Kunde*) und betätigen die Schaltfläche **[Hinzufügen]**.
15. Im Dialog *Orga-Gruppen und Einstellungen – Abstellplatz* erscheint nun die erstellte Gruppierung (*Menge der Scheiben pro Kunde*) im Bereich *Bildung der Gruppen* und kann entsprechend verwendet werden.

**Ergänzende Informationen**
⇨ Tutorial, "Sortierung" auf Seite F-25
⇨ Softwarereferenz, “Gruppierung/Sortierung - Dialog" auf Seite F-140

### Zusatz-Sortierung

Die Zusatz-Sortierungen können nur auf die Sortierungen angewendet werden. Zweck der Zusatz-Sortierungen ist es, vorhandene Sortierung in Abhängigkeit des Werts des letzten Elements ergänzen zu können. Zum Beispiel könnte eine Sortierung nach Tour, Kunde und xxxxx gewünscht sein, aber für jeden Kunden soll dieses xxxxx anders aussehen können. Daher wird zunächst eine Sortierung nach Tour und Kunde angelegt und danach alle erwünschten Sortierungen erzeugt, die für das xxxxx benötigt werden. Danach kann diese Zusatz-Sortierung der Sortierung nach Tour und Kunde in Abhängigkeit der Kundennummer zugewiesen werden. Sollte für eine gegebene Kundennummer keine Zusatz-Sortierung vorhanden sein, so findet eine weitergehende Sortierung nicht statt.

**■ So erstellen Sie eine Zusatz-Sortierung**
Beispiel: Einer existierenden Sortierung nach Tour und Kunde wird eine Zusatz-Sortierung nach Auftragsnummer und Positionsnummer für den Kunden mit der Kundennummer 11 hinzugefügt.
1.  Wählen Sie in der Menü-Leiste *Stammdaten > Feinplanung > Gruppierung > Editor-Sortierung*.
2.  Aktivieren Sie die Radiotaste *Eigenschaften*.
3.  Markieren Sie im linken Fenster die Sortierung (+Auftragsnummer+Positionsnummer), für die die Zusatz-Sortierung erstellt werden soll.
4.  Markieren Sie im rechten Fenster die Eigenschaft der Zusatz-Sortierung (Kundennummer).
5.  Betätigen Sie die Schaltfläche **[Erzeuge Zusatzsortierung]**. Es öffnet sich der Dialog *Erzeugung einer Zusatz-Sortierung*.
    ⇨ Softwarereferenz, "Erzeugung einer Zusatz-Sortierung" auf Seite F-145
6.  Im Feld *Wert* geben Sie den Wert für das Sortierungselement an (in unserem Beispiel **11**).
    ⇨ Softwarereferenz, "Wert" auf Seite F-144
7.  Aktivieren Sie die Radiotaste *Ziffer*.
8.  Betätigen Sie die Schaltfläche **[Ok]**. Der Dialog wird geschlossen.
9.  Öffnen Sie das Register *Zusatz-Sortierungen*. Die erstellte Zusatz-Sortierung wird angezeigt (in unserem Beispiel: Schlüssel: Kundennummer, Wert: 11, Zusatzsortierung: +Auftragsnummer+Positionsnummer).

**Ergänzende Informationen:**
⇨ Tutorial, "Gruppierung" auf Seite F-24
⇨ Softwarereferenz, "Erzeugung einer Zusatz-Sortierung" auf Seite F-145

### Sonderteile

Für Sonderteile gibt es keine Gruppierung oder Sortierung, da auf einem Abstellplatz immer nur eine Position steht.
Es gibt folgende Sonderteile:
*   Füllaufträge
*   Restscheiben
*   Bruchscheiben
*   Eilscheiben

#### Füllaufträge

Füllaufträge sind Scheiben, die nicht fest einem Lauf zugeordnet sind, sondern von der Optimierung dazu verwendet werden dürfen, den Verschnitt zu verbessern. Diese Füllaufträge liegen in der Datenbank in der Tabelle `POOL_TEILE`, wo sie durch die Laufnummer 10003 spezifiziert sind. Die A+W Production verfügt über eine spezielle Anzeige für Füllaufträge, die sogenannte *Füllauftrag-Anzeige*. Die *Füllauftrag-Anzeige* wird nicht standardmäßig angezeigt, sondern muss vom Benutzer aktiviert werden.

> **Füllaufträge anzeigen**
> Damit vorhandene Füllaufträge verwendet und im Register *Spezial* des Dialogs *Feinplanung für Lauf ...* angezeigt werden können, muss im Dialog *Master-Orga* der Bereich *Verwende Füller* aktiviert und die entsprechenden Abstellplätze angegeben sein!
> Möchten Sie Änderungen an den Einstellungen vornehmen, wenden Sie sich vorher bitte unbedingt an A+W, da es sonst zu unerwünschten Ergebnissen kommen kann!

**■ So aktivieren Sie die Füllauftrag-Anzeige**
1.  Wählen Sie im Menü *Stammdaten > Konfiguration*. Es öffnet sich der Dialog *Parameter-Administrator*.
2.  Wählen Sie im Bereich *A+W Production, Allgemein* Ihre Station.
3.  Scrollen Sie auf der rechten Seite in den Bereich *Programm Menü*.
4.  Markieren Sie die darunter liegende Zeile (Menü).
5.  Klicken Sie auf die Schaltfläche **[...]** am Ende der Zeile.
6.  Es öffnet sich der Dialog *Zeichenfolgen-Editor*.
7.  Gehen Sie ans Ende der Liste und geben Sie das Wort **Filler** ein.
8.  Verlassen Sie den Dialog über die Schaltfläche **[Ok]**.
9.  Um die Änderungen wirksam zu machen, müssen Sie die A+W Production neu starten.

*(Abb. F-11 Füllauftrag-Anzeige)*

**Ergänzende Informationen**
⇨ Softwarereferenz, "Verwende Füller" auf Seite F-128
⇨ Softwarereferenz, "Register Füllaufträge" auf Seite F-171

#### Restscheiben

Im Dialog *Feinplanung* können Sie im Register *Ergebnisse* eine Position anklicken und sich durch Betätigen der Schaltfläche **[PlanEdit]** die Aufteilung der Scheiben beim Schneiden ansehen. Die Scheiben der letzen Platte können dann z.B. bei besonders hohem Verschnitt über die Schaltfläche **[Auflösen]** wieder aufgelöst werden. Das bedeutet, die Scheiben werden mit der Laufnummer 10005 in die Tabelle `FEIN_TEILE` zurückgesetzt und können später zugeschnitten werden.

Solche Restscheiben finden Sie ebenfalls im Register *Spezial* und dort im Register *Restblätter*. Hier können sie für einen späteren, passenden Lauf ausgewählt werden.

Alternativ können Scheiben auch auf den aufgelösten Restblättern im Originallauf verbleiben und dort als Handzuschnitt gefertigt werden. Dann erfolgt kein Eintrag in die Tabelle `FEIN_TEILE` mit Laufnummer 10005.

> **Restblätter anzeigen**
> Damit vorhandene Restblätter verwendet und im Register *Spezial* des Dialogs *Feinplanung für Lauf ...* angezeigt werden können, muss im Dialog *Master-Orga* der Bereich *Verwende Restblätter* aktiviert und die entsprechenden Abstellplätze angegeben sein!
>
> Möchten Sie Änderungen an den Einstellungen vornehmen, wenden Sie sich vorher bitte unbedingt an A+W, da es sonst zu unerwünschten Ergebnissen kommen kann!

*(Abb. F-12 Master-Orga, Aktivierung Restblätter)*

**Ergänzende Informationen**
⇨ Softwarereferenz, "Verwende Restblätter" auf Seite F-129
⇨ Softwarereferenz, “Register Restblätter" auf Seite F-173

#### Bruchscheiben

Gebuchte Bruchscheiben werden mit der Laufnummer 10000 in die Tabelle `FEIN_TEILE` zurückgeschrieben. Anschließend können sie in der Feinplanung einem bestimmten Lauf hinzugefügt werden. In der Regel aber werden bei eiligen Aufträgen Bruchscheiben im Handzuschnitt bearbeitet.

> **Bruchscheiben anzeigen**
> Damit vorhandene Bruchscheiben verwendet und im Register *Spezial* des Dialogs *Feinplanung für Lauf ...* angezeigt werden können, muss im Dialog *Master-Orga* der Bereich *Verwende Bruchscheiben* aktiviert und die entsprechenden Abstellplätze angegeben sein!

*(Abb. F-13 Master-Orga, Aktivierung Bruchscheiben)*

**Ergänzende Informationen**
⇨ Softwarereferenz, "Verwende Bruchscheiben" auf Seite F-129
⇨ Softwarereferenz, "Register Bruchscheiben" auf Seite F-174

#### Eilscheiben

Mit Hilfe der Eilscheiben haben Sie die Möglichkeit, zügig Scheiben selbst zu erfassen und diese der Produktion zuzuführen. Es ist hierbei nicht notwendig, dass die Scheiben über die Auftragsbearbeitung erfasst werden müssen und anschließend erst übergeben werden. Eilscheiben werden im Dialog *Eilscheiben* erfasst. Diesen Dialog erreichen Sie über *Extras > Eilscheiben*.

Eilscheiben werden mit der Laufnummer 10002 in die Tabelle `FEIN_TEILE` geschrieben.

### Demos und Übungen

In diesem Abschnitt erfahren Sie, wie Sie Gruppierungen und Sortierungen in der A+W Production anlegen.

**Trainerdemo: Gruppierungen und Sortierungen erläutern**
Es werden mögliche Gruppierungen und Sortierungen gezeigt und erläutert.
Folgender Dialog wird unter diesem Aspekt erklärt:
*   Dialog *Gruppierung/Sortierung*

**Übung 1: Eine neue Gruppierung hinzufügen**
Fügen Sie die bereits vorhandene Gruppierung *Kundennummer* hinzu.

*   **Aufgabenstellung**: Fügen Sie die bereits existierende Gruppierung mit der Eigenschaft *Kundennummer* als neue Gruppierung hinzu.
*   **Lösung**: Das Ergebnis dieser Aufgabe sieht so aus:
    *(Abb. F-14 Gruppierung)*
    Die erstellte Gruppierung kann nun für Einstellungen in den Orgas genutzt werden.

**Übung 2: Einer Gruppierung eine weitere hinzufügen**
Fügen Sie die bereits vorhandene Gruppierung *Auftragsnummer* hinzu.

*   **Aufgabenstellung**: Fügen Sie der soeben angelegten Gruppierung *Kundennummer* die Gruppierung *Auftragsnummer* hinzu.
*   **Lösung**: Das Ergebnis dieser Aufgabe sieht so aus:
    *(Abb. F-15 Weitere Gruppierung)*

**Übung 3: Eine neue Sortierung hinzufügen**
Fügen Sie die bereits vorhandene Sortierung *Positionsnummer* hinzu.

*   **Aufgabenstellung**: Fügen Sie die bereits existierende Sortierung mit der Eigenschaft *Positionsnummer* als neue Sortierung hinzu.
*   **Lösung**: Das Ergebnis dieser Aufgabe sieht so aus:
    *(Abb. F-16 Sortierung)*
    Die erstellte Sortierung kann nun für Einstellungen in den Orgas genutzt werden.

**Übung 4: Einer Sortierung eine weitere hinzufügen**
Fügen Sie die bereits vorhandene Sortierung *Positionsnummer* hinzu.

*   **Aufgabenstellung**: Fügen Sie der soeben angelegten Sortierung *Positionsnummer* die Sortierung *Gross_Mass* hinzu.
*   **Lösung**: Das Ergebnis dieser Aufgabe sieht so aus:
    *(Abb. F-17 Weitere Sortierung)*

**Ergänzende Informationen:**
⇨ Tutorial, "Gruppierung" auf Seite F-24
⇨ Tutorial, "Sortierung" auf Seite F-25
⇨ Softwarereferenz, "Gruppierung/Sortierung - Dialog" auf Seite F-140

## Abstellplätze und -modi

In diesem Themenblock lernen Sie die unterschiedlichen Abstellplätze sowie die verschiedenen Abstellmodi kennen und erfahren, wie Sie damit in der A+W Production umgehen.

Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Einführung
*   Abstellplätze
*   Logische Abstellplätze
*   Abstellregeln
*   Vordefinierte Abstellmodi für A-Böcke

### Überblick

**Lernziele**
*   Abstellplätze kennenlernen und verstehen.
*   Abstellmodi kennenlernen und verstehen.
*   Die Auswirkungen der Abstellmodi verstehen.

**Nutzen**
Wenn Sie die Funktionen der Abstellmodi verstanden haben, können Sie Ihre Produktion entsprechend organisieren. Eine gut organisierte Produktion spart Ihnen Zeit und Platz und somit Geld.

**Definitionen**
*   **Physikalischer Abstellplatz**: Gestell (A-Bock, L-Bock, Fester Abstellplatz)
*   **Logischer Abstellplatz**: Ein logischer Abstellplatz besteht aus einem oder mehreren Stapeln von Glas und definiert, wie diese Stapel zusammen gehören (bspw. um daraus ISO oder VSG zu produzieren). Abhängig ist dies vom gewählten Stapelmodus. Ein logischer Abstellplatz ist einfach ein Bereich auf einem physikalischen Abstellplatz mit Nummer, auf welchen die zusammengehörigen Glasstapel gestellt werden.

> **Merke**
> *   **Was darf auf einen Abstellplatz?**: In einen Stapel oder auf einen Fächerwagen dürfen grundsätzlich nur Teile aus einem Los.
> *   **Verschiedene Glasarten auf einen Stapel**: Das Programm trennt grundsätzlich verschiedenen Glasarten und weist sie verschiedenen Stapeln zu. Sie müssen dazu keine gesonderte Logik einrichten.
> *   **Abstellmodus: Glas**: Hier wird eine Glasart pro Abstellplatz abgestellt. Jeder Stapel bekommt eine eigene Abstellplatznummer. Im Unterschied zum Modus VABGLA werden aber nur Scheiben auf einen Stapel abgestellt, wenn auch deren jeweilige Gegenscheiben gemeinsam weggestellt werden können.
> *   **Abstellmodus: Einheit**: Hier steht jede Einheit auf einem logischen Abstellplatz.
> *   **Abstellmodus: Produktion**: Hier können verschiedene Glasarten auf einem logischen Abstellplatz kombiniert werden.
> *   **Abstellmodus: VABGLA**: Hier gibt es pro Glasart einen logischen Abstellplatz mit jeweils einem Stapel.

### Abstellplätze

Dieser Abschnitt beschäftigt sich mit den logischen Abstellplätzen sowie den entsprechenden Abstellmodi.
Es behandelt folgende Themen:
*   Logische Abstellplätze
*   Abstellregeln
*   Vordefinierte Abstellmodi für A-Böcke
*   Robot-Böcke
*   Abstellmodi für Fächerwagen
*   Abstellmodi für feste Abstellplätze

In der A+W Production haben Sie verschiedene Kriterien zur Verfügung, um Scheiben auf Abstellplätze zu stellen. Sie können komplette Gruppen abstellen, Gruppen teilen, usw.

Auf diese Weise können Sie Abstellplätze und Abstellmodi dafür nutzen, das gute Ergebnis zu behalten und zusätzlich mit einer festen Produktionsreihenfolge zu arbeiten. Auf diese Weise können Sie die Produktion frei definieren und zusätzlich den roten Punkt innerhalb des roten Kreises.

> **Abstellplätze**
> An dieser Stelle weisen wir darauf hin, dass wir ausschließlich von Abstellplätzen reden, da wir nicht wissen, ob der Kunde physikalische oder logische Gestelle verwendet. Ferner sind uns Größe und Breite der Gestelle, die beim Kunden im Einsatz, nicht bekannt.

#### Logische Abstellplätze

Ein logischer Abstellplatz besteht aus einem oder mehreren Stapeln von Glas und definiert, wie diese Stapel zusammen gehören (bspw. um daraus ISO oder VSG zu produzieren). Abhängig ist dies vom gewählten Stapelmodus. Ein logischer Abstellplatz ist einfach ein Bereich auf einem physikalischen Abstellplatz mit Nummer, auf welchen die zusammengehörigen Glasstapel gestellt werden. Das Abstellen von Scheiben auf den logischen Abstellplätzen geschieht in der für den jeweiligen Abstellplatz definierten Produktionsreihenfolge.

Aus den logischen Abstellplätzen werden physikalische Gestelle gebildet. Dies geschieht für A-Böcke und feste Abstellplätze unter Berücksichtigung der Gestellbreite, der Anzahl der Gestellseiten (1 oder 2 für L- bzw. A-Bock) und des erlaubten Maximalgewichts des Abstellplatzes.

#### Abstellregeln

*   Unterschiedliche Glasarten werden immer getrennt.
*   Die angegebene Abstelltiefe darf nicht überschritten werden. Daher ist die Frage, ob es dem System erlaubt ist, Gruppen zu trennen oder zusammen zu halten.
*   In der Regel kommen große Scheiben zu erst auf den Abstellplatz. Daher müssen diese zuerst produziert werden oder es muss vor dem Abstellen umsortiert werden. Es müssen entweder eindeutige Bedingungen definiert werden oder Sie können mit Hilfe des Formel-Editors bestimmte Einschränkungen definieren.
*   Durch die Verwendung von *Abstellmodi* können Sie bestimmen, wie das System Einheiten und Gruppen auf den physikalischen und logischen Abstellplätzen abstellt (ein physikalisches Gestell kann genügend Platz für mehrere Abstellplätze mit verschiedenen Nummern haben = logische Gestelle).

**Eine Gruppe pro Stapel**
Wählen Sie diese Einstellung,
*   kommt jede Gruppe in 1 Stapel.
*   muss eine Gruppe geteilt werden (weil das maximale Gewicht überschritten ist), wird sie in zwei Stapel geteilt - ob für den zweiten Stapel dann die gleiche oder eine neue Abstellplatznummer (logischer Abstellplatz) verwendet wird, ist abhängig vom verwendeten Stapelmodus.

**Komplette Gruppe können zusammen abgestellt werden**
Wählen Sie diese Einstellung,
*   kommen verschiedene, komplette Gruppen in einen Stapel (unter Beachtung des zulässigen Gesamtgewichtes).

**Gruppen werden geteilt**
Wählen Sie diese Einstellung,
*   wenn das Teilen von Gruppen erlaubt ist (beim Erreichendes maximalen Gesamtgewichtes) und die Gruppe zu einer anderen Gruppe gestellt werden kann.
*   um ein Umsortieren von Gruppen zu vermeiden, die Reihenfolge der Gruppen wird automatisch eingehalten (XOPTS 6.2).

### Vordefinierte Abstellmodi für A-Böcke

Auf A-Böcken kann nach vier verschiedenen Verfahren abgestellt werden:
*   Abstellmodus Glas
*   Abstellmodus Einheit
*   Abstellmodus Produktion
*   Abstellmodus VABGLA

> **Trennung von Glasarten**
> Das Programm trennt immer die Glasarten. Das gilt sowohl für das Abstellen der Glasarten als auch für die Optimierung.

#### Abstellmodus Glas

Im Abstellmodus Glas wird eine Glasart pro Abstellplatz gestellt. Dabei bekommt jeder Stapel (Gruppe 3 und 4) eine eigene Abstellplatznummer (1000, 2000, 3000). Sie werden mehr Abstellplätze und Abstellplatznummern benötigen als bei anderen Abstellmodi.

**Abstellen kompletter Gruppen**
Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Und die zugehörige Gruppe des anderen Abstellplatzes kommt ebenfalls auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Beide Abstellplätze (1000 und 2000) gelten als voll. Auf die beiden neuen Abstellplätze können weitere Stapel (Gruppen) Glas gestapelt werden - solange, bis auch hier wiederum das Maximum der Beladung erreicht ist.

**Abstellen geteilter Gruppen**
Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die restlichen Scheiben (über der max. Beladung) gehen jeweils auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Und die betreffenden Scheiben der zugehörigen Gruppe des anderen Abstellplatzes gehen ebenfalls auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Beide Abstellplätze (1000 und 2000) gelten als voll. Auf die beiden neuen Abstellplätze können weitere Stapel (Gruppen) Glas gestapelt werden - solange, bis auch hier wiederum das Maximum der Beladung erreicht ist.

#### Abstellmodus Einheit

Im Abstellmodus *Einheit* steht jede Einheit (bspw. Gläser für ISO oder VSG) auf einem logischen Abstellplatz.
*   Jede Glasart befindet sich auf einem anderen Stapel.
*   Jede Einheit bekommt ihre eigene Abstellplatznummer.
*   Sobald ein Stapel das Maximum erreicht, ist die ganze Abstellplatznummer voll.
*   Sie benötigen weniger physikalische Gestelle als im Abstellmodus *Glas*.
*   Da Einheiten immer zusammengehalten werden, ist die Produktion einfach.

**Abstellen kompletter Gruppen**
Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe auf einen neuen Abstellplatz mit einer neuen Abstellplatznummer. Und die zugehörige Gruppe des anderen Stapels kommt ebenfalls auf diesen neuen (logischen) Abstellplatz (Gruppe 4 ist über dem Limit, also gehen Gruppe 4 und 3 auf einen neuen Abstellplatz: 1002). Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen beladen werden, bis auch hier die maximale Beladung erreicht wird.

**Abstellen geteilter Gruppen**
Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die Scheiben dieser Gruppe, die über der max. Beladung sind, und die zugehörigen Scheiben der anderen Gruppe gehen auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. (Gruppe 4 ist über dem Limit; die letzte Scheibe von Gruppe 4 und die letzte Scheibe der Gruppe 3 gehen auf einen neuen Abstellplatz: 1002). Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen beladen werden, bis auch hier die maximale Beladung erreicht wird.

#### Abstellmodus Produktion

Im Abstellmodus *Produktion* können verschiedene Glasarten auf einem logischen Abstellplatz in mehreren Stapeln kombiniert abgestellt werden. Es ist möglich, verschiedene Kombinationen von Produkten, welche gefertigt werden sollen, abzustellen.
*   Jede Glasart befindet sich in einem anderen Stapel.
*   Unterschiedliche Glasarten werden zusammen auf einem logischen (oder physikalischen) Abstellplatz gestellt.
*   Sobald ein Stapel das Maximum erreicht, ist die ganze Abstellplatznummer "voll".
*   Zusammengehörige Gruppen müssen definiert und beibehalten werden.
*   Sie benötigen weniger physikalische Gestelle.
*   Sie benötigen zusätzliche Hilfs- und Kontrollmechanismen wie bspw. Produktionspapiere oder Anzeigesysteme um die Kontrolle zu behalten.

**Abstellen kompletter Gruppen**
Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe und die zugehörige Gruppe des anderen Stapel auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer (Gruppe 3 ist über dem Limit, also gehen Gruppe 3 und 4 auf einen neuen Abstellplatz: 1002). Auf diesem neuen Abstellplatz können Sie neue Glasarten und neue Gruppen abstellen. Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen beladen werden, bis auch hier die maximale Beladung erreicht wird.

**Abstellen geteilter Gruppen**
Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die Scheiben dieser Gruppe, die über der max. Beladung sind, und die betreffenden Scheiben der entsprechenden Gruppe innerhalb des anderen Abstellplatzes gehen zusammen auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. (Gruppe 3 ist über dem Limit, also geht die letzte Scheibe der Gruppe 3 und die letzte Scheibe der Gruppe 4 auf einen neuen Abstellplatz: 1002). Auf diesem neuen Abstellplatz können Sie neue Glasarten und neue Gruppen abstellen. Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen beladen werden, bis auch hier die maximale Beladung erreicht wird.

#### Abstellmodus VABGLA

Im Abstellmodus VABGLA gibt es pro Glasart einen logischen Abstellplatz mit jeweils einem Stapel. Es ist möglich, verschieden Kombinationen von Produkten, welche gefertigt werden sollen, abzustellen.
*   Jede Glasart befindet sich auf einem separaten Abstellplatz.
*   Jede Glasart (Stapel) bekommt ihre eigene Abstellplatznummer.
*   Das Abstellen und Produzieren ist sehr komplex.
*   Zusammengehörige Gruppen müssen definiert und beibehalten werden.

**Abstellen kompletter Gruppen**
Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Die zugehörige Gruppe (Einheit) auf einem anderen Gestell wird nicht bewegt.

**Abstellen geteilter Gruppen**
Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die Scheiben dieser Gruppe, die über der max. Beladung sind, gehen auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Die zugehörige Gruppe (Einheit) auf einem anderen Gestell wird nicht bewegt und auch nicht geteilt.

### Robot-Böcke

Bei den A-Böcken besteht die Möglichkeit, diese als sogenannte Robot-Böcke zu kennzeichnen. Ein Robot-Bock ist ein A-Bock, der mittels eines Roboters angesteuert wird. Robot-Böcke haben die folgenden Eigenschaften:
*   Unendliche Abstellplatztiefe (>20 Meter) und
*   Maximale Anzahl Gruppen auf Abstellplatz = 1.

Auf einem solchen Abstellplatz landen also nur Scheiben mit gleichen Eigenschaften gemäß der Gruppierungsvorschrift.

### Abstellmodi für Fächerwagen

Auf Fächerwagen gibt es zwei verschiedene Verfahren:
*   **Zusammen**: Dabei werden Scheibe und Gegenscheibe(n) immer zusammen auf einen Fächerwagen gestellt (in unterschiedliche Fächer).
*   **Glas**: Dabei werden die Scheiben immer getrennt weggestellt (unterschiedliche Fächerwagen).

Diese Modi gelten natürlich nur auf den Verwendungsböcken, da für den jeweiligen Produktionsschritt die Gegenscheibe des zu produzierenden Teils nicht berücksichtigt wird. Sollte es eine Gegenscheibe geben, so kommt diese erst auf den Verwendungsböcken des nachfolgenden Produktionsschritt ins Spiel.

### Abstellmodi für feste Abstellplätze

Für feste Abstellplätze gibt es keine Abstellmodi. Sie dienen als sogenannte Zwischenlager hinter dem Zuschnitt. Es wird so lange auf diesen Abstellplätzen abgestellt, bis er voll ist. Dann muss für die Produktion umsortiert werden.
