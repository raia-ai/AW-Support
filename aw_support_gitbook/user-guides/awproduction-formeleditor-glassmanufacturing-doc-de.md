---
title: "DE_AWProduction-Formeleditor"
source: "DE_AWProduction-Formeleditor.pdf"
tags: ["A+W Production", "Formeleditor", "Software Manual", "Glass Manufacturing", "Window Production", "Formula Editor", "Technical Documentation", "German", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical manual for the A+W Formula Editor, a component of the A+W Production software suite. It details the principles, operation, and software reference for creating formulas and conditions to manage production processes in the glass, window, and door manufacturing industries."
long_description: "This comprehensive user guide provides detailed instructions for the A+W Formeleditor, a powerful tool within the A+W Production software designed for the glass, window, and door manufacturing sectors. The manual is written in German and is structured into several key sections: 'Vorspann' (Preface), 'Funktionsprinzip' (Functional Principle), 'Bedienung' (Operation), 'Softwarereferenz' (Software Reference), and a 'Partindex' (Index). The 'Funktionsprinzip' section explains the core concepts and goals of the Formula Editor, breaking down its elements into three complexity levels (Stufe I, II, III). It covers the syntax for creating formulas, comparisons, conditions, and sets. The 'Bedienung' section offers practical, step-by-step examples for applying these principles, such as defining conditions for storage locations, organizational groups, and production sections. The 'Softwarereferenz' section serves as a detailed reference for all user interface dialogs, fields, and functions within the editor, explaining how to access and use each component. The document is intended for end-users of A+W Production, enabling them to customize and automate logic for tasks like machine allocation, label generation, and production flow management."
---

# A+W Formeleditor

**A+W Production**
A+W - Software for Glass, Windows and Doors

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Ersterstellung |
| :--- | :--- |
| 1.00 / 01-2004 | Ersterstellung |
| 1.01 / 07-2013 | Layout an CI 2013 angepasst. |
| 1.02 / 01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

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

### Kontakte

**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim
📞 +49 6404 2051-0
📠 +49 6404 2051-877
📧 Zentrale@a-w.com
🌐 http://www.a-w.com

## Inhalt

- **Vorspann**
    - Revisionsübersicht
    - Editorial
- **Funktionsprinzip**
    - Der Formel-Editor
    - Ziele des Formeleditors
    - Elemente des Formeleditors: Stufe I
        - Formel
        - Vergleich
        - Bedingung
        - Verknüpfung von Elementar - Bedingungen
        - Menge
        - Zuweisung
    - Elemente des Formeleditors: Stufe II
        - Formel
        - Vergleich
        - Bedingung
        - Menge
        - Zuweisung
    - Elemente des Formeleditors: Stufe III
        - Menge
    - Notation Formula.dll
        - Syntax
        - ASSIGNMENT
        - FORMULA
        - CONDITIONS
        - CONDITION (Vergleich)
        - SET
    - Funktion
        - ASSIGNMENT
        - FORMULA
        - CONDITIONS
        - CONDITION
        - SET
    - Ergebnisprüfung
    - Übersicht der betroffenen Dialoge
- **Bedienung**
    - Bedingungen für Abstellplätze
    - Bedingungen für Orga-Gruppen
    - Modus für Gruppenbildung
    - Bedingungen für Fertigungsabschnitte
    - Weitere Beispiele
- **Softwarereferenz**
    - Formel-Editor
    - Auswahl Bedingungen
    - Bedingungen - Erzeuger
    - Bedingung
    - Name der Bedingung
    - Info
    - Invertieren
    - Übergebene Menge
    - Eingabe Zahlenwert
    - Auswahl Mengen
    - Mengen - Erzeuger
    - Name der Menge
    - Info
    - Auswahl Formeln
    - Formel - Editor
    - Auswahl Zuweisung
    - Zuweisung - Editor
- **Partindex**

## Funktionsprinzip

### Der Formel-Editor

Den Formeleditor finden Sie in A+W Production in den folgenden Bereichen:
- Organisation
- Maschinenzuordnung
- Etiketten/Skizzen/Biegertexte.

Den Formeleditor gibt es in verschiedenen Stufen. Je komplexer die Formel aufgebaut ist, je höher ist die Stufe.

Die Dokumentation zum Formeleditor wurde deshalb wie folgt unterteilt:
- "Elemente des Formeleditors: Stufe I" auf Seite R-9
- "Elemente des Formeleditors: Stufe II" auf Seite R-15
- "Elemente des Formeleditors: Stufe III" auf Seite R-19

#### Ziele des Formeleditors

Im Bereich der Organisation ist das Ziel des Formeleditors das Erstellen von Bedingungen zur Trennung von beliebigen Eigenschaften eines Produktes auf die dafür vorgesehenen Abstellplätze.

Im Bereich der MZO ist es das Ziel, Bedingungen zur Lokalisierung von Maschinen in Abhängigkeit der Bearbeitung und Eigenschaften eines Produktes zu erstellen.

Das Ziel des Formeleditors im Bereich Etiketten ist das Erstellen von Bedingungen zur Auswahl des notwendigen Etikettenlayouts in Bezug auf die Produkteigenschaften.

### Elemente des Formeleditors: Stufe I

Im Formeleditor gibt es die folgenden Elemente:
- "Formel" auf Seite R-10
- "Vergleich" auf Seite R-11
- "Bedingung" auf Seite R-11
- "Menge" auf Seite R-14
- "Zuweisung" auf Seite R-15

#### Formel

In der einfachsten Form besteht eine Formel aus einem Ausdruck, in dem die erlaubten Eigenschaften der Objekte (Properties), Konstanten, andere Formeln sowie einige Operatoren vorkommen können. Die möglichen Operatoren sind die Grundrechenarten +, -, * und / nebst Klammern. Darüber hinaus gibt es noch die String-Operatoren:

- **@LEFT**: Syntax `STRING @LEFT ANZAHL = STRING`
- **@RIGHT**: Syntax `STRING @RIGHT ANZAHL = STRING`
- **@MID**: Syntax `STRING @MID INDEX = STRING`; der Index ist 0-basiert

Alle diese Operatoren dürfen nahezu beliebig gemischt werden. Die Formel wirkt genau auf ein Teil.

*Abb. R-1: Formel-Editor - Dialog zur Erstellung einer neuen Formel mit Eingabefeld, vorhandenen Eigenschaften und Formeln.*

**Beispiele:**
- `$TEILETYP`
- `$MENGE * ($DICKE+1000)`
- `($BEARB1TEXT @MID $TEILETYP) @RIGHT ($DICKE/1000)`

#### Vergleich

Ein Vergleich besteht aus 1-2 Formeln und einer sogenannten Vergleichsvorschrift. Dabei ist zu beachten, dass nur dann genau eine Formel verwendet werden darf, wenn die Vergleichsvorschrift *Nur Formel 1* verwendet wird. In diesem Fall ist der Vergleich erfüllt, wenn das Ergebnis der Formel 1 eine Zahl größer Null oder ein nicht leerer String ist. Ansonsten ist der Vergleich erfüllt, wenn der Ausdruck `FORMEL 1 VORSCHRIFT FORMEL 2` wahr ist.

Für die Formel 2 muss für einfache Konstanten eine Formel nicht angelegt werden. In diesem Fall aktivieren Sie die Radiotaste Wert und geben die gewünschte Konstante dort ein.

*Abb. R-2: Vergleich - Dialogfenster zur Definition eines Vergleichs zwischen Formeln und Werten.*

**Beispiele:**
- Formel Teiletyp = Wert 1
- Formel Bin Iso Nur Formel 1
- Formel 3fache Breite < Formel Höhe
- Formel Dicke = Wert 3 mm

#### Bedingung

Eine Bedingung muss erfüllt werden, damit die Zuordnung entsprechend des Formelwerkes vollzogen werden kann. Sie ist das oberste Glied innerhalb der Formelstruktur und besteht in der einfachsten Form aus einer Anzahl von Vergleichen. Die Anordnung der Vergleiche gibt an, wie die Ergebnisse der Vergleiche miteinander verknüpft werden müssen. Nebeneinander stehende Vergleiche werden durch UND verknüpft - übereinander stehende Vergleiche werden durch ODER verknüpft. Eine Bedingung ist immer dann erfüllt, wenn es möglich ist, einen horizontalen Weg von links nach rechts zu finden, der nur erfüllte Vergleiche berührt.

*Abb. R-3: Bedingung mit Und-Verknüpfung*

**Beispiele:**

**Einfachste Form**

*Abb. R-4: Schematische Darstellung einer Bedingung. Eine Bedingung "Ist ESG" besteht aus einem Vergleich, der prüft, ob eine Formel "Teiletyp ESG" (basierend auf der Eigenschaft "$T_ESG") einen Wert enthält ("nur Formel 1").*

Die Bedingung *Ist ESG* ist erfüllt, wenn die Formel *Teiletyp ESG* mit der Eigenschaft des DB-Feldes `T_ESG` aus der `Pool_Teile` den Wert Eins enthält (bedingt durch die Operation *Nur Formel*).

*Abb. R-5: Bedingungen - Erzeuger Dialog mit den Komponenten: A) Formel, B) Vergleich, C) Elementarbedingung.*

**Verknüpfung von Elementar - Bedingungen**

*Abb. R-6: Schematische Darstellung einer Verknüpfung von Elementar-Bedingungen. Zeigt, wie Formeln und Vergleiche mittels Oder- und Und-Verknüpfungen zu einer komplexen Bedingung "Freie Form mit Bearbeitung" kombiniert werden.*

*Abb. R-7: Verknüpfung von Elementar-Bedingungen im Dialogfenster.*

#### Menge

*Abb. R-8: Mengen - Erzeuger Dialogfenster mit Optionen zur Mengenauswahl.*

Eine Menge besteht aus der Vorschrift, wie aus dem Startteil (Stückliste) die Endmenge gebildet werden soll. Dabei dürfen die folgenden Vorschriften beliebig miteinander kombiniert werden.
⇨ Softwarereferenz, "Mengen - Erzeuger" auf Seite R-58

Dabei kann Teil auch für eine Bearbeitung stehen.

*Abb. R-9: Schematische Darstellung einer Menge. Baumstruktur, die von einem ISO-Teil ausgeht und über Bedingungen (z.B. "Ist ESG") und Bearbeitungen zu verschiedenen End- und Zwischenprodukten führt.*

Somit ergibt sich z.B. aus der Bedingung *Ist ESG* und der Menge *Parent* alle End- und Zwischenprodukte, welche aus ein oder mehreren ESGs gefertigt werden.

#### Zuweisung

In der einfachsten Form besteht eine Zuweisung aus einer Objekt-Eigenschaft (Property) und einer Formel. Das Ergebnis der Formel wird der Eigenschaft des Objektes zugewiesen.

**Beispiel:**
- `ZUSCHLAGSDICKE = Formel 2mm`
- `ABSTELLBREITE = Höhe`

### Elemente des Formeleditors: Stufe II

Im Formeleditor gibt es die Elemente:
- "Formel"
- "Vergleich"
- "Bedingung"
- "Menge"
- "Zuweisung"

#### Formel

Die Formel enthält nun eine Menge nebst Operationsanweisung. Ohne die Menge wirkt die Formel direkt auf zu untersuchende Objekt. Wenn eine Menge angegeben ist, so wird aus dem zu untersuchenden Objekt eine Menge gebildet, wobei das Objekt das Startobjekt der Menge ist. Die Formel wird nun für jedes Objekt der Endmenge ausgewertet und die Ergebnisse davon gemäß der Operation verknüpft. Enthält die Endmenge keine Objekte, so wird ein long-Wert -1 zurückgegeben.

*Abb. R-10: Formel-Dialog mit Optionen für Menge und Operationen (Summe, Mittelwert, etc.).*

**Beispiele:**
- `$DICKE ; Menge Alle Basisteile; SUMME➔ Gesamtdicke`
- `1; Menge Alle Bearbeitungen ; SUMME → Anzahl aller Bearbeitungen`

Erlaubte Operationen sind Summe, Mittelwert, Und-Verknüpfung, Oder-Verknüpfung, Minimum und Maximum.

#### Vergleich

Üblicherweise besteht ein Vergleich aus 1-2 Formel und der Vorschrift. Alternativ darf ein Vergleich auch durch eine Bedingung ausgedrückt werden (dazu aktivieren Sie die Radiotaste *Bedingungen*). In diesem Fall ist der Vergleich erfüllt, wenn die zugewiesene Bedingung erfüllt ist. Diese Art der Verknüpfung von Bedingungen ist immer dann benutzt, wenn zwei oder mehr Bedingungen auf verschiedene Mengen angewendet werden.

*Abb. R-11: Vergleich-Dialog, der eine Bedingung "irgend ein Oberteil, das ISO ist" zeigt.*

#### Bedingung

Zunächst kann eine Bedingung invertiert werden. D.h. die Bedingung ist erfüllt, falls das Resultat der Vergleiche nicht erfüllt ist und umgekehrt. Damit lässt sich einfach aus einer schon existierenden Bedingung die umgekehrte Bedingung erstellen. Die umgekehrte Bedingung enthält genau einen Vergleich, der die ursprüngliche Bedingung zugewiesen bekommt. Außerdem wird für die umgekehrte Bedingung die Eigenschaft *invertieren* ausgewählt. In der Statuszeile erscheint ein *INV* vor dem Namen der Bedingung.

Die Vergleiche werden normaler Weise für das zu testende Objekt ausgewertet. Will man aber z.B. überprüfen, ob eins der Unterteile des Objekt einen bestimmten Teiletyp/Bearbeitungstyp hat, so kann man dazu der Bedingung eine Menge zuweisen. Dann wird aus dem Objekt eine Menge gebildet, wobei das Objekt das Startobjekt der Menge ist. Dann wird die Bedingung für alle Teile der Endmenge ausgewertet. Nun muss man noch angeben wann die Bedingung erfüllt ist. Reicht es dazu aus, dass ein Teil der Endmenge die Bedingung erfüllt, so muss die Operation *One* ausgewählt werden. Ist die Bedingung dagegen nur dann erfüllt, wenn alle Teile der Endmenge die Bedingung erfüllen, so ist die Operation *All* auszuwählen. Enthält die Endmenge keine Objekte, so ist die Bedingung nicht erfüllt.

**Beispiele:**
- Formel `Teiletyp` = Wert 125 ; Menge `Alle Unterteile`; One
- Mit Bearbeitung vom Typ=125
- Formel `T_ISO` Nur Formel 1; Menge `Kopfteil`; One (oder All)
- Das Kopfteil ist ein ISO

*Abb. R-12: Bedingung-Dialog mit der Option "Mit Menge".*

#### Menge

Die Mengendefinition enthält noch eine Bedingung. Dann werden aus der Endmenge alle Objekte entfernt, die diese Bedingung nicht erfüllen.

**Beispiel:**
- `; Anychild; Bedingung Bin Bearbeitung;`
- > Die Endmenge enthält nur die Bearbeitungen unter dem Startteil.

Wenn eine Bedingung verwendet wird, so dürfen auch die beiden Vorschriften `Up` und `Addup` verwendet werden. Diese dürfen jeweils mit keiner anderen Vorschrift kombiniert werden.

Unter Verwendung von `Up` besteht die Endmenge genau aus einem Teil. Dabei werden vom Startteil ausgehend alle Oberteile des Startteils untersucht, ob das jeweilige Teil die Bedingung erfüllt. In der Endmenge befindet sich das letzte Teil, das die Bedingung erfüllt hat. Erfüllt ein Teil die Bedingung nicht, so wird die Iteration nach oben abgebrochen.

Unter Verwendung von `Addup` kann die Endmenge aus mehr als einem Teil bestehen. Wie bei `Up` wird ebenfalls vom Startobjekt nach oben iteriert und die Iteration beendet, falls ein Teil die Bedingung nicht erfüllt. Aber die Endmenge enthält alle Teile, die die Bedingung erfüllt haben.

**Beispiele:**
- `; Up; Bedingung Bin keine Bearbeitung`
- `; Addup; Bedingung Bin nicht bestellt`

#### Zuweisung

Auch die Zuweisung kann eine Menge enthalten. Dann wird für alle Objekte der Endmenge das jeweilige Ergebnis der Formel der jeweiligen Eigenschaft zugewiesen.

**Beispiel:**
`ZUSCHLAGDICKE = Formel 2mm; Menge Alle Zuschnittteile`

### Elemente des Formeleditors: Stufe III

#### Menge

Die Mengenbildung wird immer mit einer Startmenge aufgerufen. In den einfachen Fällen besteht die Startmenge aus genau einem Teil, dem Startteil. Im Dialog *Mengen - Erzeuger* kann man wie im *Bedingungen - Erzeuger* mehrere Elemente nebeneinander oder untereinander logisch anordnen. Die Elemente im *Mengen - Erzeuger* sind andere Mengen. Dabei wird aus übereinander stehenden Mengen die Vereinigungsmenge gebildet und aus nebeneinander stehenden Mengen die Schnittmenge.

Zu beachten ist dabei, dass es für diese vorgelagerte Mengenbildung ein zweites Fenster gibt. Man schaltet zwischen dem ersten und dem zweiten Fenster mittels der Schaltfläche [+/-] um. Die Startmenge ergibt sich nun indem aus der Menge des ersten(+) Fensters alle Objekte der Menge des zweiten(-) Fensters entfernt.

**Beispiele:**
`{Menge Oberteil oder selber; Anychild + Self ; ; }`
1.  **Fenster (Plus):** Menge Oberteil oder selber
2.  **Fenster (Minus):** leer
Markiert sind `Anychild` und `Self`.

Damit erhält man das Oberteil und alle Unterteile des Oberteils. Sollte kein Oberteil existieren, so befindet sich in der Endmenge das Startteil und alle seine Unterteile.

*Abb. R-13: Mengen - Erzeuger Dialog. Zeigt eine Plus-Menge "Elternteil" und die Möglichkeit, eine Minus-Menge zu definieren.*

Damit erhält man die Endmenge mit allen Teilen, die das gleiche Oberteil haben wie das Startteil.

Soll die Iteration für `Up` oder `Addup` nicht beim Teil selber anfangen, sondern beim Oberteil, so bildet man zunächst aus dem Startteil die Startmenge via Menge Oberteil `{;Parent;;}` und verwendet diese in der gewünschten Menge mit der Vorschrift `Up` oder `Addup`.

Einer Mengenbildung kann man ferner noch eine Formel zuweisen. In diesem Fall wird die Formel für alle Teile der Startmenge ausgewertet und die Ergebnisse gespeichert. Aus der Endmenge werden dann alle Teile entfernt, für die das Ergebnis der Formel nicht in der Ergebnismenge der Startmenge enthalten ist.

**Beispiel:**
`; All; ; Formel Teiletyp`
Damit erhält man alle Teile des Teilebaums mit dem gleichen Teiletyp wie das Startteil.

### Notation Formula.dll

#### Syntax

**ASSIGNMENT**
Input: Object, UserSet
`PROPERTY = FORMULA ; SET [/USERSET]`

**FORMULA**
Input: Object, UserSet
`[formulaelements ; SET ; OP [/USERSET]]`
`OP ∈ {Summe, Mittelwert, Und, Oder, Minimum, Maximum}`
`formulaelements = property, FORMULA ; + - * / () 0..9 @LEFT @RIGHT @MID`

**CONDITIONS**
Input: Object, UserSet
``conditionelements; SET ; OP [/N] [/USERSET]```
`OP ∈ {NULL, One, All}`
`conditionelements = CONDITION(S)`
or
`(conditionelements OP conditionelements) OP ∈ {Und, Oder}`

**CONDITION (Vergleich)**
Input: Object, UserSet
``'FORMULA [OP FORMULA] ; ; ```
`OP ∈ {=,!=,>,>=,<,<=}`

**SET**
Input; Set, UserSet
`{ (setelements)[-(setelements)] ; OP ; CONDITIONS ; FORMULA [/USERSET] }`
Anmerkung: Der Teil `'-(setelements)'` wird nur verwendet, falls er nicht `'empty'` ist.
`OP ∈ {All, Master,Parent, Self;Child,Anychild,Bottom, Up, Addup}`
`setelements = 'empty'`
or
`SET`
or
`(setelements OP setelements) OP ∈ {∩, ∪}`

#### Funktion

**ASSIGNMENT**
Der FORMULA und dem SET werden das UserSet übergeben.
- **Ohne Set, ohne UserSet:** Für das gegebene Object wird die FORMULA ausgewertet. Das Ergebnis der FORMULA wird der PROPERTY des Objects zugewiesen.
- **Mit Set:** Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für jedes Element dieser Menge wird nun die FORMULA ausgewertet und das Ergebnis davon der PROPERTY des jeweiligen Objects zugewiesen.
- **Mit UserSet:** Für jedes Object im UserSet wird die FORMULA ausgewertet und das Ergebnis davon der PROPERTY des jeweiligen Objects zugewiesen.
- **Mit Set, mit UserSet:** Nicht erlaubt, nicht möglich.

**FORMULA**
Dem SET und allen FORMULAS in den formulaelements werden das UserSet übergeben.
- **Ohne Set, ohne UserSet:** Für das gegebene Object werden alle formulaelements ausgewertet und daraus der komplette Ausdruck berechnet. Das Ergebnis wird als MultiValue zurückgegeben.
- **Mit Set:** Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für jedes Element dieser Menge werden alle formulaelements ausgewertet und daraus der komplette Ausdruck berechnet. Die Ergebnisse werden nun gemäß der Operation ausgewertet und das so erhaltene Gesamtergebnis als MultiValue zurückgegeben.
- **Mit UserSet:** Für jedes Element des UserSet werden alle formulaelements ausgewertet und daraus der komplette Ausdruck berechnet. Die Ergebnisse werden nun gemäß der Operation ausgewertet und das so erhaltene Gesamtergebnis als MultiValue zurückgegeben.
- **Mit Set, mit UserSet:** nicht erlaubt, nicht möglich

**CONDITIONS**
Dem SET und allen CONDITION(S)s in den conditionelements werden das UserSet übergeben.
- **Ohne Set, ohne UserSet:** Für das gegebene Object werden alle conditionelements ausgewertet und daraus das komplette Ergebnis berechnet, das als BOOLEAN zurückgegeben wird.
- **Mit Set, (mit Operation != NULL):** Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für jedes Element dieser Menge werden alle conditionelements ausgewertet und daraus der komplette BOOLEAN-Ausdruck berechnet. Wenn nun die Operation = ONE ist, so gibt CONDITIONS TRUE zurück, falls für mindestens ein Element der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Wenn aber die Operation = ALL ist, so gibt CONDITIONS TRUE zurück, falls für alle Elemente der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Andernfalls wird jeweils FALSE zurückgegeben.
- **Mit UserSet:** Für jedes Element des UserSet werden alle conditionelements ausgewertet und daraus der komplette BOOLEAN-Ausdruck berechnet. Wenn nun die Operation = ONE ist, so gibt CONDITIONS TRUE zurück, falls für mindestens ein Element der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Wenn aber die Operation = ALL ist, so gibt CONDITIONS TRUE zurück, falls für alle Elemente der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Andernfalls wird jeweils FALSE zurückgegeben.
- **Mit Set, mit UserSet:** nicht erlaubt, nicht möglich

**CONDITION**
Jeder FORMULA wird das UserSet übergeben.
- **Beliebig:** Für das gegebene Object werden beide FORMULAs, falls vorhanden, ausgewertet.
Sollte nur eine FORMULA vorhanden sein, so wird TRUE zurückgegeben, falls das Ergebnis der FORMULA verschieden von NULL (numerisches Resultat) ist oder aber für String-Resultate kein Leerstring ist. Ansonsten wird FALSE zurückgegeben. Sollten dagegen beide FORMULAs vorhanden sein, so werden die Ergebnisse der beiden gemäß der Operation verglichen. Sollte der Vergleich erfüllt werden, so wird TRUE zurückgegeben, ansonsten FALSE.

**SET**
Allen in den setelements enthaltenen SETs, der CONDITIONS und der FORMULA werden das UserSet übergeben.
- **Ohne FORMULA, ohne UserSet:** Für das gegebene Set werden alle setelements berechnet und daraus die vorläufige Menge A bestimmt. Für jedes Object dieser Menge A wird nun gemäß Operation eine Menge BA bestimmt und zur Menge B hinzugefügt. Aus dieser Menge B werden nun alle Objecte entfernt, die nicht die CONDITIONS erfüllen. Als Ergebnis wird Menge B als RelatedSet zurückgegeben.
- **Mit FORMULA, ohne UserSet:** Zunächst wie unter A, jedoch wird nicht Menge B zurückgegeben. Für jedes Object aus dem gegebenen Set wird die FORMULA ausgewertet. Die Ergebnisse werden in einem Array gespeichert. Danach wird für jedes Object in Menge B ebenfalls die FORMULA ausgewertet. Sollte das Ergebnis der FORMULA für ein Object aus Menge B im Array enthalten sein, so wird das jeweilige Object in Menge C eingefügt. Als Ergebnis wird Menge C als RelatedSet zurückgegeben.
- **Ohne FORMULA, mit UserSet:** Wie A, jedoch wird an Stelle der gegebenen Sets das UserSet zur Bildung der Menge A verwendet.
- **Mit FORMULA, mit UserSet:** Wie B, jedoch wird an Stelle der gegebenen Sets das UserSet zur Bildung der Menge A verwendet. Zur Bildung des Array dagegen wird weiterhin das gegebene Set verwendet.

**Beispiel:**
Es soll für eine Scheibe A und eine Menge an Scheiben die Gesamtmenge von allen Scheiben bestimmt werden, die die gleiche Tour wie Scheibe A haben:
`[$MENGE ; { ; ; ; [$TOUR] /USERSET } ; SUM }`

Scheibe X soll nur am Abstellplatz hängen bleiben, falls es VSG ist und in der Menge aller Scheiben mindestens 150 VSGs enthalten sind:
`'('[T_VSG;;]==[1;;];;` AND `[$MENGE;{;;''[T_VSG;;]==[1;;]';;';/USERSET};SUM]`>=[150;;]`) ; ; ``

#### Ergebnisprüfung

Um die Ergebnisse des Formelwerkes zu überprüfen, gibt es die Möglichkeit, sich die entsprechende Log-Datei anzeigen zu lassen. Um die Ergebnisprüfung für die Feinplanung zu aktivieren, müssen Sie in A+W Production folgende Einstellung vornehmen:
`Stammdaten > Parameter > Modul Feinplanung > Specials > ViewFormula > Wert 1 eintragen`

> **Performance**
> Die Anzeige der Berechnungen wirkt sich nachteilig auf die System-Performance aus!

*Abb. R-14: Log-Datei - Beispielhafter Auszug aus einer Log-Datei zur Prüfung von Formelergebnissen.*

Die Log-Datei der Ergebnisprüfung finden Sie unter:
`\<AlcimRootDir>\Log\(Name der Log-Datei der Feinplanung).LOG`

#### Übersicht der betroffenen Dialoge

Die Übersicht zeigt Ihnen alle Dialoge, die Sie zur vollständigen Nutzung des Formeleditors benötigen. Die Verweise führen Sie in das Kapitel Softwarereferenz des Stammdatenbereichs. Dort finden Sie detaillierte Informationen zu den Dialogen mit ihren Feldern und Schaltflächen.

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| Der Formel-Editor ist nicht über einen Menü-Eintrag zu erreichen. Wie Sie ihn erreichen, ist bei den jeweiligen Dialogen genau beschrieben. | ⇨ "Auswahl Bedingungen" auf Seite R-46<br>⇨ “Bedingungen - Erzeuger” auf Seite R-48<br>⇨ "Bedingung" auf Seite R-50<br>⇨ "Name der Bedingung" auf Seite R-52<br>⇨ "Info" auf Seite R-62<br>⇨ "Auswahl Formeln" auf Seite R-63<br>⇨ "Formel - Editor" auf Seite R-65<br>⇨ "Auswahl Zuweisung" auf Seite R-68<br>⇨ "Zuweisung - Editor" auf Seite R-69 |

*Tab. R-1: Übersicht der betroffenen Dialoge*

## Bedienung

### Bedingungen für Abstellplätze

Hier wird Ihnen erklärt, wie Sie im Bereich Orga Bedingungen für Abstellplätze definieren, ändern oder löschen.

**■ So erstellen Sie eine Bedingung für einen Abstellplatz, die alle Scheiben mit einer Seitenlänge ab 1,20 m herausfiltert**

1.  Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2.  Öffnen Sie das Register `Produktionsreihenfolge`.
3.  Markieren Sie den Abstellplatz, für den Sie die Bedingung anlegen möchten.
4.  Betätigen Sie die Schaltfläche `[Neue Bedingung]`. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5.  Betätigen Sie die Schaltfläche `[Neue Bedingung ...]`. Es öffnet sich der Dialog `Bedingungen Erzeuger`.
6.  Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Namen`. Es öffnet sich der Dialog `Name der Bedingung`. Vergeben Sie einen sprechenden Namen für die Bedingung. Beispiel: `Große Scheibe`. Schließen Sie den Dialog über `[OK]`.
7.  Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Info`. Vergeben Sie eine eindeutige Beschreibung. Beispiel: `Dies ist eine Bedingung, die wahr ist, wenn eine Seite einer Scheibe länger als 1,20 m ist.` Schließen Sie den Dialog über `[OK]`.
8.  Öffnen Sie im Menü `Teilbedingungen` den Menüpunkt `Hinzufügen (Spalte)`. Es erscheint eine neue Teilbedingung.
9.  Öffnen Sie die Kombobox und wählen Sie `>=` (größer gleich).
10. Aktivieren Sie die Radiotaste `Wert`. Es öffnet sich der Dialog `Eingabe Zahlenwert`. Aktivieren Sie die Radiotaste `Länge` und geben im Bereich `Neuer Wert` 1200 mm ein. Schließen Sie den Dialog über `[OK]`.
11. Klicken Sie in das obere Eingabefeld der Bedingung. Es öffnet sich der Dialog `Auswahl Formeln --1--`.
12. Betätigen Sie `[Neue Formel ...]`. Es öffnet sich der `Formel-Editor`. Erfassen Sie einen sprechenden Namen. Beispiel: `Großes Maß`.
13. Aus dem Bereich `Vorhandene Eigenschaften` wählen Sie mit einem Doppelklick `Gross Mass`.
14. Schließen Sie den Dialog über `[OK]`. Sie befinden sich wieder im Dialog `Bedingungen-Erzeuger`.

*Abb. R-15: Bedingung: Abstellplatz für Scheiben >= 1200 mm*

Schließen Sie den Dialog. Sie befinden sich wieder im Dialog `Auswahl-Bedingungen --1--`. Die erstellte Bedingung `Große Scheibe` steht am Ende der Liste `Vorhandene Bedingungen`.

**■ So weisen Sie einem Abstellplatz eine Bedingung zu**

1.  Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2.  Öffnen Sie das Register `Produktionsreihenfolge`.
3.  Markieren Sie den Abstellplatz, dem Sie die Bedingung zuweisen möchten.
4.  Betätigen Sie `[Neue Bedingung]`. Es öffnet sich `Auswahl Bedingungen --1--`.
5.  Aus der Liste der `Vorhandenen Bedingungen` markieren Sie die Bedingung.
6.  Verlassen Sie den Dialog über `[OK]`.
7.  Die Bedingung wurde dem markierten Abstellplatz angehängt.

**■ So löschen Sie eine dem Abstellplatz zugewiesene Bedingung**

1.  Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2.  Öffnen Sie das Register `Produktionsreihenfolge`.
3.  Öffnen Sie den entsprechenden Abstellplatz durch einen Doppelklick.
4.  Markieren Sie die Bedingung des Abstellplatzes, die gelöscht werden soll.
5.  Betätigen Sie die Schaltfläche `[Löschen]`. Die Bedingung wird sofort gelöscht.

> **Löschen**
> Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich etwas gelöscht haben, verlassen Sie das Register `Produktionsreihenfolge` über `[Abbrechen]`. Beantworten Sie die Frage, ob die Änderungen ignoriert werden sollen, mit `[OK]`. Der Orga-Dialog wird geschlossen. Beim nächsten Öffnen sind die Daten wieder vorhanden.

### Bedingungen für Orga-Gruppen

Hier wird Ihnen erklärt, wie Sie im Bereich Orga Bedingungen für Orga-Gruppen definieren, ändern oder löschen.

**■ So erstellen Sie eine Bedingung für eine Orga-Gruppe, die ISO mit Sprossen für einen zweiten Fertigungsabschnitt herausfiltert**

1.  Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2.  Öffnen Sie das Register `Produktionsreihenfolge`.
3.  Markieren Sie die Orga-Gruppe, für die Sie die Bedingung anlegen möchten.
4.  Betätigen Sie `[Neue Bedingung]`. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5.  Betätigen Sie `[Neue Bedingung ...]`. Es öffnet sich der Dialog `Bedingungen Erzeuger`.
6.  Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Namen`. Vergeben Sie einen sprechenden Namen. Beispiel: `ISO Sprossen`.
7.  Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Info`. Vergeben Sie eine eindeutige Beschreibung. Beispiel: `Position wurde dem Fertigungsabschnitt 2 zugeordnet MZO_ROUTE_MAP.ROUTE =2`.
8.  Öffnen Sie im Menü `Teilbedingungen` den Menüpunkt `Hinzufügen (Spalte)`.
9.  Öffnen Sie die Kombobox und wählen Sie `==` (gleich).
10. Aktivieren Sie die Radiotaste `Wert`. Im Dialog `Eingabe Zahlenwert` aktivieren Sie die Radiotaste `Ziffer` und geben im Bereich `Neuer Wert` `2` ein.
11. Klicken Sie in das obere Eingabefeld der Bedingung. Es öffnet sich der Dialog `Auswahl Formeln --1--`.
12. Betätigen Sie `[Neue Formel ...]`. Im `Formel-Editor` erfassen Sie einen sprechenden Namen. Beispiel: `Fertigungsabschnitt`.
13. Aus dem Bereich `Vorhandene Eigenschaften` wählen Sie mit einem Doppelklick `Route`. Im Bereich `Formel` erscheint `$Route`.
14. Schließen Sie den Dialog über `[OK]`.

*Abb. R-16: Bedingung: Fertigungsabschnitt = 2*

Schließen Sie den Dialog. Die erstellte Bedingung `ISO Sprossen` steht am Ende der Liste `Vorhandene Bedingungen`.
15. Markieren Sie die Bedingung und betätigen Sie `[OK]`. Die Bedingung wird der Orga-Gruppe angehängt.

**■ So weisen Sie einer Orga-Gruppe eine vorhandene Bedingung zu**

1.  Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2.  Öffnen Sie das Register `Produktionsreihenfolge`.
3.  Markieren Sie die Orga-Gruppe.
4.  Betätigen Sie `[Neue Bedingung]`.
5.  Aus der Liste der `Vorhandenen Bedingungen` markieren Sie die gewünschte Bedingung.
6.  Verlassen Sie den Dialog über `[OK]`.
7.  Die Bedingung wurde der Orga-Gruppe angehängt.

**■ So löschen Sie eine der Orga-Gruppe zugewiesene Bedingung**

1.  Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2.  Öffnen Sie das Register `Produktionsreihenfolge`.
3.  Öffnen Sie die Orga-Gruppe durch einen Doppelklick.
4.  Markieren Sie die Bedingung, die gelöscht werden soll.
5.  Betätigen Sie `[Löschen]`.

> **Löschen**
> Das Löschen erfolgt ohne Sicherheitsabfrage. Um ein versehentliches Löschen rückgängig zu machen, verlassen Sie den Dialog über `[Abbrechen]`.

### Modus für Gruppenbildung

Dieses Beispiel dient dazu, den Orga-Gruppen und den Abstellplätzen einen weiteren wählbaren Modus zur Gruppenbildung hinzuzufügen.

**■ So erstellen Sie eine Gruppierung nach Anzahl der Scheiben pro Kunde**
d.h. es wird eine Gruppe pro Kunde erstellt und diese Gruppen nach der Zahl der in ihnen enthaltenen Scheiben sortiert. Zuerst produziert wird dann die Gruppe mit der größten Anzahl an Scheiben.

1.  Öffnen Sie den `Gruppierung/Sortierung-Dialog` über `Stammdaten > Feinplanung > Editor-Gruppierungen`.
2.  Betätigen Sie die Schaltfläche `[Formeln ...]`. Es öffnet sich der Dialog `Auswahl Formeln --1--`.
3.  Betätigen Sie die Schaltfläche `[Neue Formel ...]`. Es öffnet sich der `Formel-Editor`.
4.  Im linken oberen Eingabefeld erfassen Sie den Namen für die Formel. Beispiel: `Menge der Scheiben pro Kunde`.
5.  Im Bereich `Vorhandene Eigenschaften` wählen Sie `Menge` mit einem Doppelklick. Im Bereich Formel erscheint `$MENGE`.
6.  Betätigen Sie die Schaltfläche `[Menge ...]`. Es öffnet sich der Dialog `Auswahl Menge --1--`.
7.  Betätigen Sie `[Neue Menge ...]`. Es öffnet sich der `Mengen-Erzeuger`.
8.  Öffnen Sie im Menü `Menge` den Menüpunkt `Namen` und geben einen Namen ein. Beispiel: `Mengen Scheiben pro Kunde`.
9.  Aktivieren Sie im Menü `Menge` den Menüpunkt `Übergebene Menge`. Dies bewirkt, dass alle Positionen des Laufs berücksichtigt werden.
10. Da die gewünschte Menge nur die Freigabeteile enthalten soll, aktivieren Sie die Checkbox `Master`.
11. Um die Kundennummer hinzuzufügen, wählen Sie im Menü `Menge` den Menüpunkt `Formel`. Es öffnet sich `Auswahl Formeln --2--`. Betätigen Sie `[Neue Formel ...]`.
12. Geben Sie im `Formel Editor` den Namen für die Formel ein. Beispiel: `Kundennummer`.
13. Wählen Sie `Kundennummer` aus `Vorhandene Eigenschaften`. Im Bereich Formel erscheint `$Kundennummer`.
14. Betätigen Sie `[OK]`. Im Dialog `Auswahl Formeln --2--` markieren Sie `Kundennummer` und betätigen `[OK]`.
15. In der Statuszeile des `Mengen-Erzeuger` sehen Sie, welche Formel benutzt wird: `Formel: Kundennummer`.
16. Schließen Sie alle Dialoge mit `[OK]`, bis Sie wieder im Dialog `Gruppierung/Sortierung` sind.
17. Die Formel `Menge der Scheiben pro Kunde` ist nun in der Liste der Formeln. Markieren Sie die Formel und betätigen Sie `[Hinzufügen]`. Sie steht dann in den Einstellungen für Orga-Gruppen und Abstellplätze zur Verfügung.

### Bedingungen für Fertigungsabschnitte

Hier wird Ihnen erklärt, wie Sie im Bereich MZO Bedingungen für Fertigungsabschnitte definieren, ändern oder löschen.

**■ So erstellen Sie eine Bedingung für einen Fertigungsabschnitt, der alle Scheiben mit Sprossen herausfiltert**

1.  Öffnen Sie den Dialog `Fertigungsabschnitte` über `Stammdaten > MZO > Konfiguration`.
2.  Markieren Sie den Fertigungsabschnitt.
3.  Betätigen Sie die rechte Maustaste und wählen Sie `Bedingung des Fertigungsabschnitts > Neu`.
4.  Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5.  Betätigen Sie `[Neue Bedingung ...]`. Es öffnet sich der `Bedingungen Erzeuger`.
6.  Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Namen`. Vergeben Sie einen Namen. Beispiel: `Bin Sprossen-ISO`.
7.  Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Info`. Vergeben Sie eine Beschreibung. Beispiel: `Diese Bedingung ist wahr, wenn die Position ein Sprossenflag hat`.
8.  Öffnen Sie im Menü `Teilbedingungen` den Menüpunkt `Hinzufügen (Spalte)`.
9.  Die Kombobox bleibt auf `nur Formel 1`.
10. Die Radiotaste `Normal` bleibt aktiv.
11. Klicken Sie in das obere Eingabefeld. Es öffnet sich `Auswahl Formeln --1--`.
12. Betätigen Sie `[Neue Formel ...]`. Im `Formel-Editor` erfassen Sie einen Namen. Beispiel: `Sprossen`.
13. Aus dem Bereich `Vorhandene Eigenschaften` wählen Sie `Pos_Sprossen_Flag` mit einem Doppelklick.
14. Schließen Sie den Dialog mit `[OK]`.
15. Schließen Sie den `Bedingungen-Erzeuger` mit `[OK]`.

*Abb. R-17: Bedingung: Bin ISO mit Sprosse*

Die erstellte Bedingung `Bin Sprossen ISO` steht am Ende der Liste `Vorhandene Bedingungen`.

**■ So weisen Sie einem Fertigungsabschnitt eine vorhandene Bedingung zu**

1.  Öffnen Sie den Dialog `Fertigungsabschnitt` über `Stammdaten > MZO > Konfiguration`.
2.  Markieren Sie den Fertigungsabschnitt.
3.  Betätigen Sie die rechte Maustaste und wählen Sie `Bedingung des Fertigungsabschnitts > Neu`.
4.  Es öffnet sich `Auswahl Bedingungen --1--`.
5.  Aus der Liste der `Vorhandenen Bedingungen` markieren Sie die gewünschte Bedingung.
6.  Verlassen Sie den Dialog über `[OK]`.
7.  Die Bedingung wurde dem Fertigungsabschnitt angehängt.

**■ So löschen Sie eine dem Fertigungsabschnitt zugewiesene Bedingung**

1.  Öffnen Sie den Dialog `Fertigungsabschnitt` über `Stammdaten > MZO > Konfiguration`.
2.  Öffnen Sie den Fertigungsabschnitt durch einen Doppelklick.
3.  Markieren Sie die Bedingung, die gelöscht werden soll.
4.  Betätigen Sie die rechte Maustaste und wählen Sie `Bedingung löschen`.

> **Löschen**
> Das Löschen erfolgt ohne Sicherheitsabfrage. Um ein versehentliches Löschen rückgängig zu machen, verlassen Sie den Dialog `Fertigungsabschnitte` über `[Abbrechen]`.

### Weitere Beispiele

**■ So erstellen Sie eine Bedingung für ESG im ISO oder mit Bearbeitungen am Float**

1.  **Erster Schritt:** Erstellen einer einfachen Bedingung `Bin ESG`, die die Eigenschaft `T_ESG` zurückgibt.
    *Abb. R-18: Erster Schritt - Bedingung `Bin ESG`*

2.  **Überprüfung, ob das Teil im ISO eingebaut wird:** Dies erfordert eine zusammengesetzte Mengenbeschreibung, um die "Gegenscheibe" zu identifizieren.
    *   1. Elementarbedingung: `Teiletyp VSG` mit `Property T_VSG`.
    *   2. Allgemeine Mengenbeschreibung: Erzeugt eine Menge für die Gegenscheibe.
    *   3. Zusammengesetzte Startmenge: `Alle direkten Unterteile der Eltern`. Die Operation sucht von der Startmenge alle Elternteile, deren Unterteile, und subtrahiert das Startteil selbst, sodass nur die Gegenscheiben übrig bleiben.
    *   4. Minus- oder Abzugsmenge: `Ich allein`.
    *Abb. R-19: Prüfen - Dialoge zur Definition der Mengenoperation.*

3.  Da ein Teil nicht gleichzeitig ESG und ISO sein kann, wird die Bedingung angepasst. Es wird eine ODER-Verknüpfung erstellt: `Bin ESG` ODER `Kopfteil ist ISO`.
    *Abb. R-20: Abbildung der ODER-Verknüpfung.*

4.  Jetzt die Oder-Verknüpfung, ob eins der Unterteile eine Bearbeitung ist. Dazu wird eine weitere Bedingung `Bin Bearbeitung` für alle Unterteile geprüft.
    *Abb. R-21: Bedingung mit ODER-Verknüpfung für `Kopfteil ist ISO` und `unter mir sind Bearbeitungen`.*

**■ Die Bearbeitungen direkt unter mir**

1.  Die Endmenge soll nur die Bearbeitungen unter dem Startteil enthalten, die nach den letzten erzeugenden Bearbeitungen unter dem Startteil erfolgen.
2.  Dazu wird zunächst die Menge aller Unterteile gebildet, die keine Bearbeitungen sind.
3.  **Menge Erzeugende Bearbeitungen unter mir** = `{ ; ANYCHILD ; Bedingung Ist keine Bearbeitung; }`
4.  Mit Hilfe dieser Menge wird nun die Menge aller Teile und Bearbeitungen unterhalb des Startteils erzeugt, die man nicht haben will.
5.  **Menge Unerwünschte Teile/Bearbeitungen unter mir** = `{ Menge Erzeugende Bearbeitungen unter mir ; ANYCHILD+SELF ; ; }`
6.  Die gewünschte Menge ergibt sich dann aus der Menge **Alle Unterteile** und der Menge **Unerwünschte Teile/Bearbeitungen unter mir**:
    `{ Menge Alle Unterteile - Menge Unerwünschte Teile/Bearbeitungen unter mir; SELF ; ; }`

## Softwarereferenz

### Formel-Editor

Der Formel-Editor kommt in A+W Production in den folgenden Bereichen zum Einsatz:
- Organisation
- Maschinenzuordnung
- Etiketten, Skizzen, Biegertexte

Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative Wege einen Dialog aufzurufen, so sind diese ebenfalls angegeben.

### Auswahl Bedingungen

**Aufruf über**

-   **Organisation**
    -   `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga-Gruppe markieren > [Neue Bedingung]`
    -   `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > [Neue Bedingung]`

-   **Maschinenzuordnung**
    -   `Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte Maustaste > Bedingung des Fertigungsabschnitts > Neu`
    -   `Stammdaten > MZO > Konfiguration > Bedingung des Fertigungsabschnitts markieren > rechte Maustaste > Bedingung editieren`
    -   `Stammdaten > MZO > Konfiguration > [Technologie] > [Neu] > [Neu]`
    -   `Stammdaten > MZO > Konfiguration > [Technologie] > [Ändern] > [Neu]/[Editieren]`

-   **Etiketten, Skizzen, Biegertexte**
    -   `Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration ... > Bedingung markieren > [Formel Editor]`

*Abb. R-22: Auswahl Bedingungen --1-- Dialogfenster*

In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte vorhandene Bedingungen ausgewählt, geändert oder neue Bedingungen angelegt werden.

**Erläuterung der Felder**

-   **Vorhandene Bedingungen**: Die Tabelle listet alle im System vorhandenen Bedingungen für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte. Die Inhalte sind für die jeweiligen Bereiche unterschiedlich!
-   **Keine Bedingung**: Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis, dass Nichts als selektiert gilt.
-   **Beschreibung**: Das Feld enthält eine detaillierte Erläuterung zu der Bedingung. Dabei handelt es sich um den Text, den Sie im Feld `Info` erfassen.

**Erläuterung der Schaltflächen**

-   **Löschen**: Betätigen Sie diese Schaltfläche, wird die zuvor markierte Bedingung gelöscht (ohne Sicherheitsabfrage).
-   **Neue Bedingung**: Betätigen Sie diese Schaltfläche, öffnet sich der Dialog `Bedingungen - Erzeuger`. Sie können dann eine neue Bedingung anlegen.
-   **Editieren**: Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Bedingung der Dialog `Bedingungen - Erzeuger`.

### Bedingungen - Erzeuger

**Aufruf über**
Dieser Dialog wird aufgerufen, wenn im Dialog "Auswahl Bedingungen" die Schaltfläche `[Neue Bedingung ...]` oder `[Editieren]` betätigt wird.

*Abb. R-23: Bedingungen - Erzeuger Dialogfenster*

Im `Bedingungen - Erzeuger` können Sie entweder eine zuvor markierte Bedingung ändern oder neue Bedingungen anlegen.

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| **Menü Bedingungen:** | |
| Name | ⇨ "Name der Bedingung" |
| Info | ⇨ "Info" |
| Menge | ⇨ "Auswahl Mengen" |
| Invertieren | ⇨ "Invertieren" |
| Übergebene Menge | ⇨ “Übergebene Menge" |
| OK | Speichert und schließt |
| Abbruch | Verwirft und schließt |
| **Menü Teilbedingungen:** | |
| Hinzufügen (Spalte) | Fügt eine UND-Bedingung hinzu |
| Hinzufügen (Zeile) | Fügt eine ODER-Bedingung hinzu |
| Entfernen | Entfernt die Auswahl |

**Werkzeugleiste**

| Werkzeug | Erläuterung |
| :--- | :--- |
| ✓ (OK) | Die definierte Bedingung wird gespeichert und der Editor verlassen. |
| X (Abbruch) | Die definierte Bedingung wird verworfen und der Editor verlassen. |
| ++ (Spalte) | Es öffnet sich das Bearbeitungsfenster zum Definieren einer UND-Verknüpfung. |
| ‡ (Zeile) | Es öffnet sich das Bearbeitungsfenster zum Definieren einer ODER-Verknüpfung. |
| - (Entfernen) | Die selektierte Bedingung wird gelöscht. |

**Erläuterung der Radiotasten**

-   **All**: Die Bedingungen aller Teile einer Stückliste werden berücksichtigt.
-   **One**: Es werden nur die Eigenschaften der aktuellen Scheibe berücksichtigt.
-   **Null**: Die der Bedingung zugeordnete Menge wird nicht berücksichtigt.

### Bedingung

**Aufruf über**
Der Dialog wird über das Menü `Teilbedingungen > Hinzufügen` im `Bedingungen - Erzeuger` aufgerufen.

*Abb. R-24: Bedingung Dialogfenster*

**Felder**

-   **Oberes Eingabefeld**: Klicken öffnet den Dialog `Auswahl Formeln`.
-   **Mittleres Auswahlfeld**: Kombobox zur Auswahl des Operators (`nur Formel 1`, `==`, `!=`, `<`, etc.).
-   **Unteres Eingabefeld**: Klicken öffnet `Auswahl Formeln`, `Eingabe Zahlenwert` oder `Auswahl Bedingungen`, abhängig von der Radiotaste.
-   **Normal (Radiotaste)**: Aktiviert die Auswahl einer Formel im unteren Feld.
-   **Wert (Radiotaste)**: Aktiviert die Eingabe eines Zahlenwertes.
-   **Bedingungen (Radiotaste)**: Aktiviert die Auswahl einer weiteren Bedingung.

### Name der Bedingung

**Aufruf über**
`Bedingungen - Erzeuger > Menü Bedingungen > Name`

*Abb. R-25: Name der Bedingung Dialogfenster*

In diesem Dialog vergeben Sie einen sprechenden Namen für die Bedingungen. Der Name wird in der Statuszeile des Dialogs `Bedingungen - Erzeuger` angezeigt.

-   **Alte Bezeichnung**: Zeigt den bisherigen Namen oder `neue Bedingung`.
-   **Neue Bezeichnung**: Eingabefeld für den neuen Namen der Bedingung.

### Info

**Aufruf über**
`Bedingungen - Erzeuger > Menü Bedingungen > Info`

*Abb. R-26: Info zur Bedingung Dialogfenster*

In diesem Bereich können Sie den Inhalt der Bedingung beschreiben. Der Text erscheint im Dialog `Auswahl Bedingungen` im Bereich `Beschreibung`.

### Invertieren

Zunächst kann eine Bedingung invertiert werden. D.h. die Bedingung ist erfüllt, falls das Resultat der Vergleiche nicht erfüllt ist und umgekehrt. Die umgekehrte Bedingung enthält genau einen Vergleich, der die ursprüngliche Bedingung zugewiesen bekommt. In der Statuszeile erscheint ein `INV` vor dem Namen der Bedingung. Der Menüpunkt ist zu aktivieren bzw. zu deaktivieren.

### Übergebene Menge

Dieser Menüpunkt ist zu aktivieren bzw. zu deaktivieren. Ist er aktiv, wird bei der Bildung der Mengen nicht nur die Position, über die der Dialog `Bedingungen - Erzeuger` geöffnet wurde, berücksichtigt, sondern alle Positionen des Laufs.

### Eingabe Zahlenwert

**Aufruf über**
Dieser Dialog wird aufgerufen, wenn im `Bedingung`-Dialog die Radiotaste `[Wert]` aktiviert und in das untere Eingabefeld geklickt wird.

*Abb. R-27: Eingabe Zahlenwert Dialogfenster*

Dieser Dialog dient der Eingabe von Zahlenwerten. Durch das Aktivieren der entsprechenden Radiotaste, können Sie darüber hinaus spezifizieren, ob es sich bei dem Zahlenwert um `Ziffer`, `Dicke`, `Text`, `Länge` oder `SZR` handelt.

**Felder**
-   **Alter Wert**: Zeigt den bisherigen Wert. Standard ist 0.
-   **Neuer Wert**: Eingabefeld für den neuen Wert.

**Radiotasten**
-   **Ziffer**: Für Stückzahlen. Bsp: `Menge > 10`.
-   **Dicke**: Für Dickenangaben in mm.
-   **Text**: Für Textwerte.
-   **Länge**: Für Längenangaben.
-   **SZR**: Für den Scheibenzwischenraum.

### Auswahl Mengen

**Aufruf über**
Dieser Dialog wird aufgerufen, wenn im `Formel-Editor` die Schaltfläche `[Menge ...]` betätigt wird und dort eine neue Menge erstellt oder editiert wird.

*Abb. R-28: Auswahl Mengen Dialogfenster*

In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte vorhandene Mengen ausgewählt, geändert oder neue Mengen angelegt werden.

**Erläuterung der Felder**
-   **Vorhandene Mengen**: Listet alle im System vorhandenen Mengen auf.
-   **Keine Menge**: Ist diese Checkbox aktiv, wird "Nichts" selektiert.
-   **Beschreibung**: Detaillierte Erläuterung zur markierten Menge.

**Erläuterung der Schaltflächen**
-   **Löschen**: Löscht die markierte Menge.
-   **Neue Menge**: Öffnet den `Mengen - Erzeuger` zum Anlegen einer neuen Menge.
-   **Editieren**: Öffnet den `Mengen - Erzeuger` zum Bearbeiten der markierten Menge.

### Mengen - Erzeuger

**Aufruf über**
Dieser Dialog wird über die Schaltflächen `[Neue Menge ...]` oder `[Editieren]` im Dialog `Auswahl Mengen` aufgerufen.

*Abb. R-29: Mengen - Erzeuger Dialogfenster*

Im `Mengen - Erzeuger` können Sie eine zuvor markierte Menge ändern oder neue Menge anlegen.

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| **Menü Menge:** | |
| Name | ⇨ "Name der Menge" |
| Info | ⇨ "Info" |
| Bedingung | ⇨ "Auswahl Bedingungen" |
| Formel | ⇨ "Auswahl Formeln" |
| OK / Abbruch | Speichert/Verwirft und schließt |
| **Menü Teilmengen:** | |
| Hinzufügen (Spalte/Zeile) | Fügt eine UND/ODER Teilmenge hinzu |
| Entfernen | Entfernt die Auswahl |
| Wechsel | Schaltet zwischen Plus- und Minus-Fenster um |

**Werkzeugleiste im Mengen - Erzeuger**
-   ✓ (OK): Speichert und schließt.
-   X (Abbruch): Verwirft und schließt.
-   ++ (Spalte): Fügt UND-Teilmenge hinzu.
-   ‡ (Zeile): Fügt ODER-Teilmenge hinzu.
-   - (Entfernen): Löscht Auswahl.
-   +/- (Wechsel): Schaltet zwischen erstem und zweitem Fenster um.

**Erläuterung der Checkboxen**
-   **All**: Alle Teile des Teilebaums.
-   **Master**: Das oberste Teil des Teilebaums (Kopfteil).
-   **Parent**: Das Teil direkt über dem Startteil.
-   **Self**: Das Startteil.
-   **Child**: Alle direkten Unterteile des Startteils.
-   **Anychild**: Alle Unterteile (direkt und indirekt).
-   **Bottom**: Alle Basisteile unter dem Startteil.
-   **Up**: Iteriert vom Startteil nach oben. Die Endmenge ist das letzte Teil, das eine Bedingung erfüllt.
-   **Addup**: Wie `Up`, aber die Endmenge enthält alle Teile auf dem Weg nach oben, die die Bedingung erfüllen.

### Name der Menge

**Aufruf über**
`Mengen - Erzeuger > Menü Menge > Name`

*Abb. R-30: Name der Menge Dialogfenster*

In diesem Dialog vergeben Sie einen sprechenden Namen für die Menge, der in der Statuszeile des `Mengen - Erzeuger` angezeigt wird.

### Info (zur Menge)

**Aufruf über**
`Mengen - Erzeuger > Menü Menge > Info`

*Abb. R-31: Info zur Menge Dialogfenster*

In diesem Bereich können Sie den Inhalt der Menge beschreiben. Der Text erscheint im Dialog `Auswahl Mengen` im Bereich `Beschreibung`.

### Auswahl Formeln

**Aufruf über**
Dieser Dialog wird aufgerufen, wenn in einem `Bedingung`-Dialog oder `Zuweisung`-Dialog in ein Formelfeld geklickt wird.

*Abb. R-32: Auswahl Formeln Dialogfenster*

In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte vorhandene Formeln ausgewählt, geändert oder neue Formeln angelegt werden.

**Felder**
-   **Vorhandene Formeln**: Listet alle im System vorhandenen Formeln.
-   **Keine Formel**: Ist diese Checkbox aktiv, wird "Nichts" selektiert.
-   **Beschreibung**: Zeigt eine Erläuterung zur markierten Formel.

**Schaltflächen**
-   **Löschen**: Löscht die markierte Formel.
-   **Neue Formel**: Öffnet den `Formel - Editor` zum Anlegen einer neuen Formel.
-   **Editieren**: Öffnet den `Formel - Editor` zum Bearbeiten der markierten Formel.

### Formel - Editor

**Aufruf über**
Dieser Dialog wird über die Schaltflächen `[Neue Formel ...]` oder `[Editieren]` im Dialog `Auswahl Formeln` aufgerufen.

*Abb. R-33: Formel - Editor Dialogfenster*

In diesem Dialog können Sie neue Formeln erstellen.

**Felder**
-   **Eingabefeld oben**: Geben Sie einen sprechenden Namen für die Formel ein.
-   **Beschreibung**: Geben Sie eine detaillierte Beschreibung an.
-   **Formel**: Hier wird das Datenbankfeld eingetragen, typischerweise durch Doppelklick aus der Liste `Vorhandene Eigenschaften`.
-   **Menge (Schaltfläche)**: Öffnet den Dialog `Auswahl Mengen`.

**Radiotasten im Bereich Operation**
(Nur aktiv, wenn eine Menge zugewiesen wurde)
-   **Summe (Wert)**: Summe aller Ergebnisse.
-   **Mittelwert**: Summe/Anzahl Ergebnisse.
-   **Und-Verknüpfung**: Logisches UND der Ergebnisse (sinnvoll für 0/1-Ergebnisse).
-   **Oder-Verknüpfung**: Logisches ODER der Ergebnisse.
-   **Minimum**: Kleinstes Ergebnis.
-   **Maximum**: Größtes Ergebnis.
-   **Anzahl Resultate**: Anzahl der verschiedenen Ergebnisse.

**Weitere Felder**
-   **Übergebene Menge Checkbox**: Berücksichtigt alle Positionen des Laufs, nicht nur die aktuelle.
-   **Vorhandene Eigenschaften**: Listet verfügbare Datenbankfelder (Properties).
-   **Vorhandene Formeln**: Listet alle bereits definierten Formeln auf.

### Auswahl Zuweisung

**Aufruf über**
`Stammdaten > Feinplanung > Zuweisungen`

*Abb. R-34: Auswahl Zuweisung Dialogfenster*

In diesem Dialog können Sie nur für den Bereich der Orga vorhandene Zuweisungen auswählen, ändern oder neue Zuweisungen anlegen.

**Felder**
-   **Vorhandene Zuweisungen**: Listet alle im System vorhandenen Zuweisungen für Orga.
-   **Keine Zuweisung**: Ist diese Checkbox aktiv, wird "Nichts" selektiert.
-   **Beschreibung**: Zeigt eine Erläuterung zur markierten Zuweisung.

**Schaltflächen**
-   **Löschen**: Löscht die markierte Zuweisung.
-   **Neue Zuweisung**: Öffnet den `Zuweisung - Editor`.
-   **Editieren**: Öffnet den `Zuweisung - Editor` für die markierte Zuweisung.

### Zuweisung - Editor

**Aufruf über**
`Stammdaten > Feinplanung > Zuweisungen > [Neue Zuweisung ...]`

*Abb. R-35: Zuweisung - Editor Dialogfenster*

In diesem Dialog können Sie eine Zuweisung definieren. Eine Zuweisung besteht aus einer Objekt-Eigenschaft (Property) und einer Formel.

**Felder**
-   **Eingabefeld oben**: Name der Zuweisung.
-   **Eigenschaft**: Kombobox zur Auswahl der zu ändernden Eigenschaft (Datenbankfeld).
-   **Formel... (Schaltfläche)**: Öffnet `Auswahl Formeln`.
-   **Grau hinterlegtes Feld (Formel)**: Zeigt den Namen der ausgewählten Formel.
-   **Menge... (Schaltfläche)**: Öffnet `Auswahl Mengen`.
-   **Übergebene Menge (Checkbox)**: Berücksichtigt alle Positionen des Laufs.
-   **Grau hinterlegtes Feld (Menge)**: Zeigt den Namen der ausgewählten Menge.

**Wichtige Zuweisungen:**
-   **Abstellbreite**: Wird für eine eventuell verwendete Gestellbelegung verwendet. Normalerweise mit der Breite der Scheibe belegt.
-   **Bewertung**: Normalerweise mit 100 belegt. Dient der Optimierung, um Scheiben auf mehrere Lagerplatten zu verteilen. Ein kleinerer Wert führt zu stärkerer "Verschmierung".
-   **Dickendifferenz**: Für Auffüller, um die Änderung der Glasdicke zu steuern.
-   **Gruppennummer**: Standardmäßig 0. Wird zur Bildung von Fertigungsgruppen in der Feinplanung verwendet.
-   **Zuschlagdicke**: Standardmäßig 0 mm. Erlaubt, eine größere Dicke für die Gestellbelegung zu berücksichtigen, z.B. für Pappe bei Scheiben mit Siebdruck.

## Partindex

### Symbols
-   'Zuweisung (Stufe II): R-18

### A
-   Addup (Mengen Erzeuger): R-61
-   All (Bedingungen-Erzeuger): R-50
-   All (Mengen Erzeuger): R-60
-   Alte Bezeichnung (Name der Bedingung): R-52
-   Alte Bezeichnung (Name der Menge): R-62
-   Alter Wert (Eingabe Zahlenwert): R-55
-   Anychild (Mengen Erzeuger): R-60
-   Anzahl Resultate (Formel Editor): R-67
-   Auswahl Bedingungen: R-46
-   Auswahl Formeln: R-63
-   Auswahl Mengen: R-56
-   Auswahl Zuweisung: R-68

### B
-   Bedingung: R-11, R-16, R-51
-   Bedingungen-Erzeuger: R-48
-   Beschreibung (Auswahl Bedingungen): R-47
-   Beschreibung (Auswahl Formeln): R-64
-   Beschreibung (Auswahl Mengen): R-57
-   Beschreibung (Auswahl Zuweisung): R-68
-   Beschreibung (Formel Editor): R-66
-   Bottom (Mengen Erzeuger): R-60

### C
-   Child (Mengen Erzeuger): R-60

### D
-   Dialog (Auswahl Bedingungen): R-46
-   Dialog (Auswahl Formeln): R-63
-   Dialog (Auswahl Mengen): R-56
-   Dialog (Auswahl Zuweisung): R-68
-   Dialog (Bedingungen-Erzeuger): R-48
-   Dialog (Eingabe Zahlenwert): R-54
-   Dialog (Formel Editor): R-65

### E
-   Editieren (Auswahl Bedingungen): R-47
-   Editieren (Auswahl Formeln): R-65
-   Editieren (Auswahl Mengen): R-57
-   Editieren (Auswahl Zuweisung): R-68
-   Eigenschaft (Zuweisung Editor): R-69
-   Eingabefeld oben (Zuweisung Editor): R-69
-   Eingabe Zahlenwert: R-54
-   Eingabefeld oben (Formel Editor): R-66

### F
-   Formel (Stufe I): R-10
-   Formel (Stufe II): R-15
-   Formel (Zuweisung Editor): R-70
-   Formel Editor: R-65

### I
-   Info: R-53, R-62
-   Invertieren (Bedingung): R-53

### K
-   Keine Bedingung (Auswahl Bedingungen): R-47
-   Keine Formel (Auswahl Formeln): R-64
-   Keine Menge (Auswahl Mengen): R-57
-   Keine Zuweisung (Auswahl Zuweisung): R-68

### L
-   Länge (Eingabe Zahlenwert): R-55
-   Löschen (Auswahl Bedingungen): R-47
-   Löschen (Auswahl Formeln): R-64
-   Löschen (Auswahl Mengen): R-57
-   Löschen (Auswahl Zuweisung): R-68

### M
-   Master (Mengen Erzeuger): R-60
-   Maximum (Formel Editor): R-67
-   Menge (Stufe I): R-14
-   Menge (Stufe II): R-18
-   Menge (Stufe III): R-19
-   Menge (Formel Editor): R-66
-   Menge (Zuweisung Editor): R-70
-   Mengen Erzeuger: R-58
-   Menü (Bedingungen-Erzeuger): R-49
-   Menü (Mengen Erzeuger): R-59
-   Minimum (Formel Editor): R-67
-   Mittelwert (Formel Editor): R-67
-   Mittleres Auswahlfeld (Bedingung): R-51

### N
-   Name der Bedingung: R-52
-   Name der Menge: R-61
-   Neue Bedingung (Auswahl Bedingungen): R-47
-   Neue Bezeichnung (Name der Bedingung): R-52
-   Neue Bezeichnung (Name der Menge): R-62
-   Neue Formel (Auswahl Formeln): R-64
-   Neue Menge (Auswahl Mengen): R-57
-   Neue Zuweisung (Auswahl Zuweisung): R-68
-   Neuer Wert (Eingabe Zahlenwert): R-55
-   Normal (Bedingung): R-51
-   Null (Bedingungen-Erzeuger): R-50

### O
-   Oberes Eingabefeld (Bedingung): R-51
-   Oder-Verknüpfung (Formel Editor): R-67
-   One (Bedingungen-Erzeuger): R-50

### P
-   Parent (Mengen Erzeuger): R-60

### S
-   Self (Mengen Erzeuger): R-60
-   Summe (Formel Editor): R-67
-   SZR (Eingabe Zahlenwert): R-55

### T
-   Text (Eingabe Zahlenwert): R-55

### U
-   Übergebene Menge (Bedingung): R-54
-   Übergebene Menge (Formel Editor): R-67
-   Übergebene Menge (Zuweisung Editor): R-70
-   Und-Verknüpfung (Formel Editor): R-67
-   Unteres Eingabefeld (Bedingung): R-51
-   Up (Mengen Erzeuger): R-60

### V
-   Vergleich (Stufe I): R-11
-   Vergleich (Stufe II): R-16
-   Vorhandene Bedingungen (Auswahl Bedingungen): R-47
-   Vorhandene Eigenschaften (Formel Editor): R-67
-   Vorhandene Formeln (Auswahl Formeln): R-64
-   Vorhandene Formeln (Formel Editor): R-67
-   Vorhandene Menge (Auswahl Mengen): R-57
-   Vorhandene Zuweisung (Auswahl Zuweisung): R-68

### W
-   Werkzeugleiste (Bedingungen-Erzeuger): R-49
-   Werkzeugleiste (Mengen Erzeuger): R-60
-   Wert (Bedingung): R-51

### Z
-   Ziffer (Eingabe Zahlenwert): R-55
-   Zuweisung (Stufe I): R-15
-   Zuweisung Editor: R-69
