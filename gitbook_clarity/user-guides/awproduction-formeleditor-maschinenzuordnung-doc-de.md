---
description: D-AWProduction-HB_8
---

# awproduction-formeleditor-maschinenzuordnung-doc-de

## Tutorial: Der Formeleditor

***

### Vergleich

Ein Vergleich besteht aus 1-2 Formeln und einer sogenannten Vergleichsvorschrift. Dabei ist zu beachten, dass nur dann genau eine Formel verwendet werden darf, wenn die Vergleichsvorschrift _Nur Formel 1_ verwendet wird. In diesem Fall ist der Vergleich erfüllt, wenn das Ergebnis der Formel 1 eine Zahl größer Null oder ein nicht leerer String ist. Ansonsten ist der Vergleich erfüllt, wenn der Ausdruck FORMEL 1 VORSCHRIFT FORMEL 2 wahr ist.

Für die Formel 2 muss für einfache Konstanten eine Formel nicht angelegt werden. In diesem Fall aktivieren Sie die Radiotaste Wert und geben die gewünschte Konstante dort ein.

_Abb. F-2: Vergleich_

#### Beispiele

* Formel Teiletyp = Wert 1
* Formel Bin Iso Nur Formel 1
* Formel 3fache Breite < Formel Höhe
* Formel Dicke = Wert 3 mm

### Bedingung

_Abb. F-3: Bedingung mit Und-Verknüpfung_

Eine Bedingung muss erfüllt werden, damit die Zuordnung entsprechend des Formelwerkes vollzogen werden kann. Sie ist das oberste Glied innerhalb der Formelstruktur und besteht in der einfachsten Form aus einer Anzahl von Vergleichen. Die Anordnung der Vergleiche gibt an, wie die Ergebnisse der Vergleiche miteinander verknüpft werden müssen. Nebeneinander stehende Vergleiche werden durch UND verknüpft - übereinander stehende Vergleiche werden durch ODER verknüpft. Eine Bedingung ist immer dann erfüllt, wenn es möglich ist, einen horizontalen Weg von links nach rechts zu finden, der nur erfüllte Vergleiche berührt.

#### Beispiele:

**Einfachste Form**

_Abb. F-4: Schematische Darstellung einer Bedingung_

Die Bedingung _Ist ESG_ ist erfüllt, wenn die Formel _Teiletyp ESG_ mit der Eigenschaft des DB-Feldes _T\_ESG_ aus der Pool\_Teile den Wert Eins enthält (bedingt durch die Operation Nur Formel).

_Abb. F-5: Bedingungen - Erzeuger_

* **A** Formel
* **B** Vergleich
* **C** Elementarbedingung

#### Beispiele: Verknüpfung von Elementar - Bedingungen

_Abb. F-6: Schematische Darstellung einer Verknüpfung von Elementar-Bedingungen_

_Abb. F-7: Verknüpfung von Elementar-Bedingungen_

### Menge

_Abb. F-8: Mengen - Erzeuger_

Eine Menge besteht aus der Vorschrift, wie aus dem Startteil (Stückliste) die Endmenge gebildet werden soll. Dabei dürfen die folgenden Vorschriften beliebig miteinander kombiniert werden.

⇨ Softwarereferenz, "Mengen - Erzeuger" auf Seite F-708

Dabei kann Teil auch für eine Bearbeitung stehen.

_Abb. F-9: Schematische Darstellung einer Menge_

Somit ergibt sich z.B. aus der Bedingung _Ist ESG_ und der Menge _Parent_ alle End- und Zwischenprodukte, welche aus ein oder mehreren ESGs gefertigt werden.

### Zuweisung

In der einfachsten Form besteht eine Zuweisung aus einer Objekt-Eigenschaft (Property) und einer Formel. Das Ergebnis der Formel wird der Eigenschaft des Objektes zugewiesen.

#### Beispiel:

* ZUSCHLAGSDICKE = Formel 2mm
* ABSTELLBREITE = Höhe

### Elemente des Formeleditors: Stufe II

Im Formeleditor gibt es die Elemente:

* "Formel" auf Seite F-15
* "Vergleich" auf Seite F-16
* "Bedingung" auf Seite F-16
* "Menge" auf Seite F-18
* "Zuweisung" auf Seite F-18

#### Formel

Die Formel enthält nun eine Menge nebst Operationsanweisung. Ohne die Menge wirkt die Formel direkt auf zu untersuchende Objekt. Wenn eine Menge angegeben ist, so wird aus dem zu untersuchenden Objekt eine Menge gebildet, wobei das Objekt das Startobjekt der Menge ist. Die Formel wird nun für jedes Objekt der Endmenge ausgewertet und die Ergebnisse davon gemäß der Operation verknüpft. Enthält die Endmenge keine Objekte, so wird ein long-Wert -1 zurückgegeben.

**Beispiele:**

* $DICKE ; Menge Alle Basisteile; SUMME➔ Gesamtdicke
* 1 ; Menge Alle Bearbeitungen ; SUMME ➔ Anzahl aller Bearbeitungen

Erlaubte Operationen sind Summe, Mittelwert, Und-Verknüpfung, Oder-Verknüpfung, Minimum und Maximum.

_Abb. F-10: Formel_

#### Vergleich

Üblicherweise besteht ein Vergleich aus 1-2 Formel und der Vorschrift. Alternativ darf ein Vergleich auch durch eine Bedingung ausgedrückt werden (dazu aktivieren Sie die Radiotaste _Bedingungen_). In diesem Fall ist der Vergleich erfüllt, wenn die zugewiesene Bedingung erfüllt ist. Diese Art der Verknüpfung von Bedingungen ist immer dann benutzt, wenn zwei oder mehr Bedingungen auf verschiedene Mengen angewendet werden.

_Abb. F-11: Vergleich_

#### Bedingung

Zunächst kann eine Bedingung invertiert werden. D.h. die Bedingung ist erfüllt, falls das Resultat der Vergleiche nicht erfüllt ist und umgekehrt. Damit lässt sich einfach aus einer schon existierenden Bedingung die umgekehrte Bedingung erstellen. Die umgekehrte Bedingung enthält genau einen Vergleich, der die ursprüngliche Bedingung zugewiesen bekommt. Außerdem wird für die umgekehrte Bedingung die Eigenschaft invertieren ausgewählt. In der Statuszeile erscheint ein INV vor dem Namen der Bedingung.

Die Vergleiche werden normaler Weise für das zu testende Objekt ausgewertet. Will man aber z.B. überprüfen, ob eins der Unterteile des Objekt einen bestimmten Teiletyp/Bearbeitungstyp hat, so kann man dazu der Bedingung eine Menge zuweisen. Dann wird aus dem Objekt eine Menge gebildet, wobei das Objekt das Startobjekt der Menge ist. Dann wird die Bedingung für alle Teile der Endmenge ausgewertet. Nun muss man noch angeben wann die Bedingung erfüllt ist. Reicht es dazu aus, dass ein Teil der Endmenge die Bedingung erfüllt, so muss die Operation _One_ ausgewählt werden. Ist die Bedingung dagegen nur dann erfüllt, wenn alle Teile der Endmenge die Bedingung erfüllen, so ist die Operation _All_ auszuwählen. Enthält die Endmenge keine Objekte, so ist die Bedingung nicht erfüllt.

**Beispiele:**

* Formel **Teiletyp** = Wert 125; Menge **Alle Unterteile**; **One** Mit Bearbeitung vom Typ=125
* Formel **T\_ISO** Nur Formel 1; Menge **Kopfteil**; **One** (oder All) Das Kopfteil ist ein ISO

_Abb. F-12: Bedingung_

#### Menge

Die Mengendefinition enthält noch eine Bedingung. Dann werden aus der Endmenge alle Objekte entfernt, die diese Bedingung nicht erfüllen.

**Beispiel:**

* ; Anychild; Bedingung Bin Bearbeitung; -> Die Endmenge enthält nur die Bearbeitungen unter dem Startteil.

Wenn eine Bedingung verwendet wird, so dürfen auch die beiden Vorschriften _Up_ und _Addup_ verwendet werden. Diese dürfen jeweils mit keiner anderen Vorschrift kombiniert werden.

Unter Verwendung von _Up_ besteht die Endmenge genau aus einem Teil. Dabei werden vom Startteil ausgehend alle Oberteile des Startteils untersucht, ob das jeweilige Teil die Bedingung erfüllt. In der Endmenge befindet sich das letzte Teil, das die Bedingung erfüllt hat. Erfüllt ein Teil die Bedingung nicht, so wird die Iteration nach oben abgebrochen.

Unter Verwendung von _Addup_ kann die Endmenge aus mehr als einem Teil bestehen. Wie bei _Up_ wird ebenfalls vom Startobjekt nach oben iteriert und die Iteration beendet, falls ein Teil die Bedingung nicht erfüllt. Aber die Endmenge enthält alle Teile, die die Bedingung erfüllt haben.

**Beispiele:**

* ; Up; Bedingung Bin keine Bearbeitung
* ; Addup; Bedingung Bin nicht bestellt

#### Zuweisung

Auch die Zuweisung kann eine Menge enthalten. Dann wird für alle Objekte der Endmenge das jeweilige Ergebnis der Formel der jeweiligen Eigenschaft zugewiesen.

**Beispiel:**

* ZUSCHLAGDICKE = Formel 2mm ; Menge Alle Zuschnittteile

### Elemente des Formeleditors: Stufe III

#### Menge

Die Mengenbildung wird immer mit einer Startmenge aufgerufen. In den einfachen Fällen besteht die Startmenge aus genau einem Teil, dem Startteil. Im Dialog Mengen - Erzeuger kann man wie im Bedingungen - Erzeuger mehrere Elemente nebeneinander oder untereinander logisch anordnen. Die Elemente im Mengen - Erzeuger sind andere Mengen. Dabei wird aus übereinander stehenden Mengen die Vereinigungsmenge gebildet und aus nebeneinander stehenden Mengen die Schnittmenge.

Zu beachten ist dabei, dass es für diese vorgelagerte Mengenbildung ein zweites Fenster gibt. Man schaltet zwischen dem ersten und dem zweiten Fenster mittels der Schaltfläche \[+/-] um. Die Startmenge ergibt sich nun indem aus der Menge des ersten(+) Fensters alle Objekte der Menge des zweiten(-) Fensters entfernt.

**Beispiele:**

{Menge Oberteil oder selber ; Anychild + Self ; ; }

1. Fenster (Plus): Menge Oberteil oder selber
2. Fenster (Minus): leer Markiert sind Anychild und Self

Damit erhält man das Oberteil und alle Unterteile des Oberteils. Sollte kein Oberteil existieren, so befindet sich in der Endmenge das Startteil und alle seine Unterteile.

_Abb. F-13: Mengen - Erzeuger_

Damit erhält man die Endmenge mit allen Teilen, die das gleiche Oberteil haben wie das Startteil.

Soll die Iteration für Up oder Addup nicht beim Teil selber anfangen, sondern beim Oberteil, so bildet man zunächst aus dem Startteil die Startmenge via Menge Oberteil {;Parent;;} und verwendet diese in der gewünschten Menge mit der Vorschrift Up oder Addup.

Einer Mengenbildung kann man ferner noch eine Formel zuweisen. In diesem Fall wird die Formel für alle Teile der Startmenge ausgewertet und die Ergebnisse gespeichert. Aus der Endmenge werden dann alle Teile entfernt, für die das Ergebnis der Formel nicht in der Ergebnismenge der Startmenge enthalten ist.

**Beispiel:**

* ; All;; Formel Teiletyp Damit erhält man alle Teile des Teilebaums mit dem gleichen Teiletyp wie das Startteil.

### Notation Formula.dll

#### Syntax

**ASSIGNMENT**

* **Input:** Object, UserSet
* `PROPERTY = FORMULA ; SET [/USERSET]`

**FORMULA**

* **Input:** Object, UserSet
* `[formulaelements; SET ; OP [/USERSET]]`
* `OP ∈ {Summe, Mittelwert, Und, Oder, Minimum, Maximum}`
* `formulaelements = property, FORMULA ; + - * / () 0..9 @LEFT @RIGHT @MID`

**CONDITIONS**

* **Input:** Object, UserSet
* \`conditionelements ; SET ; OP \[/N] \[/USERSET]\`\`
* `OP ∈ {NULL, One, All}`
* `conditionelements = CONDITION(S) or (conditionelements OP conditionelements) OP ∈ {Und, Oder}`

**CONDITION (Vergleich)**

* **Input:** Object, UserSet
* \`'FORMULA \[OP FORMULA] ; ; \`\`
* `OP ∈ {=,!=,>,>=,<,<=}`

**SET**

* **Input:** Set, UserSet
* `{ (setelements)[-(setelements)] ; OP ; CONDITIONS ; FORMULA [/USERSET]}`
  * **Anmerkung:** Der Teil, \`-(setelements)' wird nur verwendet, falls er nicht ,empty' ist.
* `OP ∈ {All, Master, Parent, Self; Child, Anychild, Bottom, Up, Addup}`
* `setelements = 'empty' or SET or (setelements OP setelements) OP ∈ {n, U}`

#### Funktion

**ASSIGNMENT**

Der FORMULA und dem SET werden das UserSet übergeben.

* **Ohne Set, ohne UserSet:** Für das gegebene Object wird die FORMULA ausgewertet. Das Ergebnis der FORMULA wird der PROPERTY des Objects zugewiesen.
* **Mit Set:** Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für jedes Element dieser Menge wird nun die FORMULA ausgewertet und das Ergebnis davon der PROPERTY des jeweiligen Objects zugewiesen.
* **Mit UserSet:** Für jedes Object im UserSet wird die FORMULA ausgewertet und das Ergebnis davon der PROPERTY des jeweiligen Objects zugewiesen.
* **Mit Set, mit UserSet:** Nicht erlaubt, nicht möglich.

**FORMULA**

Dem SET und allen FORMULAs in den formulaelements werden das UserSet übergeben.

* **Ohne Set, ohne UserSet:** Für das gegebene Object werden alle formulaelements ausgewertet und daraus der komplette Ausdruck berechnet. Das Ergebnis wird als MultiValue zurückgegeben.
* **Mit Set:** Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für jedes Element dieser Menge werden alle formulaelements ausgewertet und daraus der komplette Ausdruck berechnet. Die Ergebnisse werden nun gemäß der Operation ausgewertet und das so erhaltene Gesamtergebnis als MultiValue zurückgegeben.
* **Mit UserSet:** Für jedes Element des UserSet werden alle formulaelements ausgewertet und daraus der komplette Ausdruck berechnet. Die Ergebnisse werden nun gemäß der Operation ausgewertet und das so erhaltene Gesamtergebnis als MultiValue zurückgegeben.
* **Mit Set, mit UserSet:** nicht erlaubt, nicht möglich

**CONDITIONS**

Dem SET und allen CONDITION(S)s in den conditionelements werden das UserSet übergeben.

* **Ohne Set, ohne UserSet:** Für das gegebene Object werden alle conditionelements ausgewertet und daraus das komplette Ergebnis berechnet, das als BOOLEAN zurückgegeben wird.
* **Mit Set, (mit Operation != NULL):** Aus dem gegebenen Object wird mittels SET eine Menge erzeugt. Für jedes Element dieser Menge werden alle conditionelements ausgewertet und daraus der komplette BOOLEAN-Ausdruck berechnet. Wenn nun die Operation = ONE ist, so gibt CONDITIONS TRUE zurück, falls für mindestens ein Element der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Wenn aber die Operation = ALL ist, so gibt CONDITIONS TRUE zurück, falls für alle Elemente der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Andernfalls wird jeweils FALSE zurückgegeben.
* **Mit UserSet:** Für jedes Element des UserSet werden alle conditionelements ausgewertet und daraus der komplette BOOLEAN-Ausdruck berechnet. Wenn nun die Operation = ONE ist, so gibt CONDITIONS TRUE zurück, falls für mindestens ein Element der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Wenn aber die Operation = ALL ist, so gibt CONDITIONS TRUE zurück, falls für alle Elemente der komplette BOOLEAN-Ausdruck erfüllt ist, TRUE ist. Andernfalls wird jeweils FALSE zurückgegeben.
* **Mit Set, mit UserSet:** nicht erlaubt, nicht möglich

**CONDITION**

Jeder FORMULA wird das UserSet übergeben.

* **Beliebig:** Für das gegebene Object werden beide FORMULAs, falls vorhanden, ausgewertet. Sollte nur eine FORMULA vorhanden sein, so wird TRUE zurückgegeben, falls das Ergebnis der FORMULA verschieden von NULL (numerisches Resultat) ist oder aber für String-Resultate kein Leerstring ist. Ansonsten wird FALSE zurückgegeben. Sollten dagegen beide FORMULAs vorhanden sein, so werden die Ergebnisse der beiden gemäß der Operation verglichen. Sollte der Vergleich erfüllt werden, so wird TRUE zurückgegeben, ansonsten FALSE.

**SET**

Allen in den setelements enthaltenen SETs, der CONDITIONS und der FORMULA werden das UserSet übergeben.

* **Ohne FORMULA, ohne UserSet:** Für das gegebene Set werden alle setelements berechnet und daraus die vorläufige Menge A bestimmt. Für jedes Object dieser Menge A wird nun gemäß Operation eine Menge BA bestimmt und zur Menge B hinzugefügt. Aus dieser Menge B werden nun alle Objecte entfernt, die nicht die CONDITIONS erfüllen. Als Ergebnis wird Menge B als RelatedSet zurückgegeben.
* **Mit FORMULA, ohne UserSet:** Zunächst wie unter A, jedoch wird nicht Menge B zurückgegeben. Für jedes Object aus dem gegebenen Set wird die FORMULA ausgewertet. Die Ergebnisse werden in einem Array gespeichert. Danach wird für jedes Object in Menge B ebenfalls die FORMULA ausgewertet. Sollte das Ergebnis der FORMULA für ein Object aus Menge B im Array enthalten sein, so wird das jeweilige Object in Menge C eingefügt. Als Ergebnis wird Menge C als RelatedSet zurückgegeben.
* **Ohne FORMULA, mit UserSet:** Wie A, jedoch wird an Stelle der gegebenen Sets das UserSet zur Bildung der Menge A verwendet.
* **Mit FORMULA, mit UserSet:** Wie B, jedoch wird an Stelle der gegebenen Sets das UserSet zur Bildung der Menge A verwendet. Zur Bildung des Array dagegen wird weiterhin das gegebene Set verwendet.

#### Beispiel:

Es soll für eine Scheibe A und eine Menge an Scheiben die Gesamtmenge von allen Scheiben bestimmt werden, die die gleiche Tour wie Scheibe A haben: `[$MENGE ; { ; ; ; [$TOUR] /USERSET } ; SUM }`

Scheibe X soll nur am Abstellplatz hängen bleiben, falls es VSG ist und in der Menge aller Scheiben mindestens 150 VSGs enthalten sind: `'('[T_VSG;;]==[1;;];;` AND ´\[$MENGE;{;;''\[T\_VSG;;]==\[1;;]';;';/USERSET};SUM]`>=[150;;]`) ; ; \`\`

#### Ergebnisprüfung

Um die Ergebnisse des Formelwerkes zu überprüfen, gibt es die Möglichkeit, sich die entsprechende Log-Datei anzeigen zu lassen. Um die Ergebnisprüfung für die Feinplanung zu aktivieren, müssen Sie in A+W Production folgende Einstellung vornehmen: `Stammdaten > Parameter > Modul Feinplanung > Specials > ViewFormula > Wert 1 eintragen`

> **Performance** Die Anzeige der Berechnungen wirkt sich nachteilig auf die System-Performance aus!

_Abb. F-14: Log-Datei_

Die Log-Datei der Ergebnisprüfung finden Sie unter `\<AlcimRootDir>\Log\(Name der Log-Datei der Feinplanung).LOG`

### Bedingungen für Abstellplätze

Hier wird Ihnen erklärt, wie Sie im Bereich Orga Bedingungen für Abstellplätze definieren, ändern oder löschen.

#### So erstellen Sie eine Bedingung für einen Abstellplatz, die alle Scheiben mit einer Seitenlänge ab 1,20 m herausfiltert

1. Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2. Öffnen Sie das Register `Produktionsreihenfolge`.
3. Markieren Sie den Abstellplatz, für den Sie die Bedingung anlegen möchten.
4. Betätigen Sie die Schaltfläche \[Neue Bedingung]. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5. Betätigen Sie die Schaltfläche \[Neue Bedingung ...]. Es öffnet sich der Dialog `Bedingungen Erzeuger`.
6. Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Namen`. Es öffnet sich der Dialog `Name der Bedingung`. Im Feld Neue Bezeichnung steht standardmäßig Neue Bedingung. Vergeben Sie in diesem Feld einen sprechenden Namen für die Bedingung. Beispiel: Große Scheibe. Schließen Sie den Dialog über die Schaltfläche \[OK].
7. Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Info`. Es öffnet sich der Dialog `Info`. Vergeben Sie in diesem Feld eine eindeutige Beschreibung für die Bedingung. Beispiel: Dies ist eine Bedingung, die wahr ist, wenn eine Seite einer Scheibe länger als 1,20 m ist. Schließen Sie den Dialog über die Schaltfläche \[OK].
8. Öffnen Sie im Menü `Teilbedingungen` den Menüpunkt `Hinzufügen (Spalte)`. Es erscheint eine neue Teilbedingung, die Sie konfigurieren können.
9. Öffnen Sie die Kombobox (standardmäßig vorbelegt mit `nur Formel 1`) und wählen Sie `>= (größer gleich)`.
10. Aktivieren Sie die Radiotaste `Wert`. Es öffnet sich automatisch der Dialog `Eingabe Zahlenwert`. Da der neue Abstellplatz nur Scheiben über 1,20 aufnehmen soll, aktivieren wir die Radiotaste `Länge` und geben im Bereich Neuer Wert `1200 mm` ein. Schließen Sie den Dialog über die Schaltfläche \[OK]. Der Wert erscheint dann im unteren Feld der Bedingung.
11. Klicken Sie jetzt in das obere Eingabefeld der Bedingung. Es öffnet sich automatisch der Dialog `Auswahl Formeln --1--`. Hier wird definiert, auf was sicher der im 2. Eingabefeld eingetragene Wert beziehen soll.
12. Betätigen Sie die Schaltfläche \[Neue Formel ...]. Es öffnet sich der Dialog `Formel-Editor`. Im oberen linken Eingabefeld erfassen Sie einen möglichst sprechenden Namen für die Formel. Beispiel: Großes Maß. ⇨ Softwarereferenz, "Eingabefeld oben" auf Seite F-718
13. Aus dem Bereich `Vorhandene Eigenschaften` wählen Sie mit einem Doppelklick `Gross Mass`. ⇨ Softwarereferenz, "Vorhandene Eigenschaften" auf Seite F-719
14. Schließen Sie den Dialog über die Schaltfläche \[OK]. Sie befinden sich wieder im Dialog `Bedingungen-Erzeuger`. _Abb. F-15: Bedingung: Abstellplatz für Scheiben >= 1200 mm_ Schließen Sie den Dialog entweder über das Menü `Bedingungen > OK` oder durch einen Klick auf `✓`. Sie befinden sich wieder im Dialog `Auswahl-Bedingungen --1--`. Die erstellte Bedingung `Große Scheibe` steht am Ende der Liste `Vorhandene Bedingungen`.

#### So weisen Sie einem Abstellplatz eine Bedingung zu

1. Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2. Öffnen Sie das Register `Produktionsreihenfolge`.
3. Markieren Sie den Abstellplatz, dem Sie die Bedingung zuweisen möchten.
4. Betätigen Sie die Schaltfläche \[Neue Bedingung]. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5. Aus der Liste der `Vorhandenen Bedingungen` markieren Sie die Bedingung, die dem Abstellplatz zugewiesen werden soll.
6. Verlassen Sie den Dialog über die Schaltfläche \[OK].
7. Die Bedingung wurde dem im Register `Produktionsreihenfolge` markierten Abstellplatz angehängt.

#### So löschen Sie eine dem Abstellplatz zugewiesene Bedingung

1. Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2. Öffnen Sie das Register `Produktionsreihenfolge`.
3. Öffnen Sie den entsprechenden Abstellplatz durch eine Doppelklick.
4. Markieren Sie die Bedingung des Abstellplatzes, die gelöscht werden soll.
5. Betätigen Sie die Schaltfläche \[Löschen]. Die Bedingung wird sofort gelöscht.

> **Löschen** Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich etwas gelöscht haben, verlassen Sie das Register `Produktionsreihenfolge` über die Schaltfläche \[Abbrechen]. Sie werden gefragt, ob die Änderungen ignoriert werden sollen. Diese Frage beantworten Sie mit \[OK]. Der Orga-Dialog wird geschlossen. Wenn Sie ihn das nächste Mal öffnen, sind die Daten wieder vorhanden.

### Bedingungen für Orga-Gruppen

Hier wird Ihnen erklärt, wie Sie im Bereich Orga Bedingungen für Orga-Gruppen definieren, ändern oder löschen.

#### So erstellen Sie eine Bedingung für eine Orga-Gruppe, die ISO mit Sprossen für einen zweiten Fertigungsabschnitt herausfiltert

1. Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2. Öffnen Sie das Register `Produktionsreihenfolge`.
3. Markieren Sie den Orga-Gruppe, für den Sie die Bedingung anlegen möchten.
4. Betätigen Sie die Schaltfläche \[Neue Bedingung]. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`. ⇨ Softwarereferenz, "Auswahl Bedingungen" auf Seite F-694
5. Betätigen Sie die Schaltfläche \[Neue Bedingung ...]. Es öffnet sich der Dialog `Bedingungen Erzeuger`. ⇨ Softwarereferenz, "Bedingungen - Erzeuger" auf Seite F-696
6. Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Namen`. Es öffnet sich der Dialog `Name der Bedingung`. Vergeben Sie in diesem Feld einen sprechenden Namen für die Bedingung. In unserem Beispiel: `ISO Sprossen`. Schließen Sie den Dialog über die Schaltfläche \[OK]. ⇨ Softwarereferenz, "Name der Bedingung" auf Seite F-701
7. Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Info`. Es öffnet sich der Dialog `Info`. Vergeben Sie in diesem Feld eine eindeutige Beschreibung für die Bedingung. In unserem Beispiel: `Position wurde dem Fertigungsabschnitt 2 zugeordnet MZO_ROUTE_MAP.ROUTE =2`. Schließen Sie den Dialog über die Schaltfläche \[OK]. ⇨ Softwarereferenz, "Info" auf Seite F-702
8. Öffnen Sie im Menü `Teilbedingungen` den Menüpunkt `Hinzufügen (Spalte)`. Es erscheint eine neue Teilbedingung, die Sie konfigurieren können.
9. Öffnen Sie die Kombobox (standardmäßig vorbelegt mit `nur Formel 1`) und wählen Sie `== (gleich)`.
10. Aktivieren Sie die Radiotaste `Wert`. Es öffnet sich automatisch der Dialog `Eingabe Zahlenwert`. Da das ISO Sprossen ausschließlich auf dem Fertigungsabschnitt 2 produziert wird, aktivieren wir die Radiotaste `Ziffer` und geben im Bereich `Neuer Wert` 2 ein. Schließen Sie den Dialog über die Schaltfläche \[OK]. Der Wert erscheint dann im unteren Feld der Bedingung. ⇨ Softwarereferenz, "Eingabe Zahlenwert" auf Seite F-704
11. Klicken Sie jetzt in das obere Eingabefeld der Bedingung. Es öffnet sich automatisch der Dialog `Auswahl Formeln --1--`. Hier wird definiert, auf was sich der im 2. Eingabefeld eingetragene Wert beziehen soll. ⇨ Softwarereferenz, "Auswahl Formeln" auf Seite F-715
12. Betätigen Sie die Schaltfläche \[Neue Formel ...]. Es öffnet sich der Dialog `Formel-Editor`. Im oberen linken Eingabefeld erfassen Sie einen möglichst sprechenden Namen für die Formel. In unserem Beispiel: `Fertigungsabschnitt`. ⇨ Softwarereferenz, "Eingabefeld oben" auf Seite F-718
13. Aus dem Bereich `Vorhandene Eigenschaften` wählen Sie mit einem Doppelklick `Route`. Im Bereich `Formel` erscheint `$Route`. ⇨ Softwarereferenz, "Vorhandene Eigenschaften" auf Seite F-719
14. Schließen Sie den Dialog über die Schaltfläche \[OK]. Sie befinden sich wieder im Dialog `Bedingungen-Erzeuger`. _Abb. F-16: Bedingung: Fertigungsabschnitt = 2_ Schließen Sie den Dialog entweder über das Menü `Bedingungen > OK` oder durch einen Klick auf `✓`. Sie befinden sich wieder im Dialog `Auswahl-Bedingungen --1--`. Die erstellte Bedingung `ISO Sprossen` steht am Ende der Liste `Vorhandene Bedingungen`.
15. Markieren Sie die Bedingung und betätigen Sie die Schaltfläche \[Ok]. Die Bedingung wird der zuvor markierten Orga-Gruppe angehängt.

#### So weisen Sie einer Orga-Gruppe eine vorhandene Bedingung zu

1. Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2. Öffnen Sie das Register `Produktionsreihenfolge`.
3. Markieren Sie die Orga-Gruppe, der Sie die Bedingung zuweisen möchten.
4. Betätigen Sie die Schaltfläche \[Neue Bedingung]. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5. Aus der Liste der `Vorhandenen Bedingungen` markieren Sie die Bedingung, die der Orga-Gruppe zugewiesen werden soll.
6. Verlassen Sie den Dialog über die Schaltfläche \[OK].
7. Die Bedingung wurde der im Register `Produktionsreihenfolge` markierten Orga-Gruppe angehängt.

#### So löschen Sie eine der Orga-Gruppe zugewiesene Bedingung

1. Öffnen Sie den Orga-Dialog über `Stammdaten > Feinplanung > Orga`.
2. Öffnen Sie das Register `Produktionsreihenfolge`.
3. Öffnen Sie die entsprechenden Orga-Gruppe durch eine Doppelklick.
4. Markieren Sie die Bedingung der Orga-Gruppe, die gelöscht werden soll.
5. Betätigen Sie die Schaltfläche \[Löschen]. Die Bedingung wird sofort gelöscht.

> **Löschen** Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich etwas gelöscht haben, verlassen Sie das Register `Produktionsreihenfolge` über die Schaltfläche \[Abbrechen]. Sie werden gefragt, ob die Änderungen ignoriert werden sollen. Diese Frage beantworten Sie mit \[OK]. Der Orga-Dialog wird geschlossen. Wenn Sie ihn das nächste Mal öffnen, sind die Daten wieder vorhanden.

### Modus für Gruppenbildung

Dieses Beispiel dient dazu, den Orga-Gruppen und den Abstellplätzen einen weiteren wählbaren Modus zur Gruppenbildung hinzuzufügen.

#### So erstellen Sie eine Gruppierung nach Anzahl der Scheiben pro Kunde

d.h. es wird eine Gruppe pro Kunde erstellt und diese Gruppen nach der Zahl der in ihnen enthaltenen Scheiben sortiert. Zuerst produziert wird dann die Gruppe mit der größten Anzahl an Scheiben.

1. Öffnen Sie den `Gruppierung/Sortierung-Dialog` über `Stammdaten > Feinplanung > Editor-Gruppierungen`.
2. Betätigen Sie die Schaltfläche \[Formeln ...]. Es öffnet sich der Dialog `Auswahl Formeln --1--`.
3. Betätigen Sie die Schaltfläche \[Neue Formel ...]. Es öffnet sich der Dialog `Formel-Editor`.
4. Im linken oberen Eingabefeld erfassen Sie den Namen für die Formel der Gruppierung. In unserem Beispiel `Menge der Scheiben pro Kunde`.
5. Im Bereich `Vorhandene Eigenschaften` wählen Sie `Menge` mit einem Doppelklick aus. Im Bereich Formel erscheint `$MENGE`.
6. Betätigen Sie die Schaltfläche \[Menge ...]. Es öffnet sich der Dialog `Auswahl Menge --1--`.
7. Betätigen Sie die Schaltfläche \[Neue Menge ...], um eine neue Menge anzulegen. Es öffnet sich der Dialog `Mengen-Erzeuger`. Wir beginnen die Mengen-Erzeugung mit einer gegebenen Menge und bekommen nach den Mengenoperationen, die wir hier durchführen, unsere gewünschte endgültige Menge. An den Formelinterpreter wird von der Feinplanung an Werten übergeben eine Position eines bestimmten Kunden, die Mengenkalkulation der Feinplanung und als weiteren Parameter alle Aufträge des aktuellen Laufs. Von uns muss nur noch die Kundennummer hinzugefügt werden.
8. Öffnen Sie im Menü `Menge` den Menüpunkt `Namen` und geben einen neuen, möglichst sprechenden Namen für die Menge ein. In unserem Beispiel `Mengen Scheiben pro Kunde`. Verlassen Sie den Dialog mit der Schaltfläche \[Ok].
9. Aktivieren Sie im Menü `Menge` den Menüpunkt `Übergebene Menge`. Dies bewirkt, dass bei der Bildung der Menge nicht nur die Position, mit der wir in den Mengen-Erzeuger gekommen sind, selbst berücksichtigt wird, sondern alle Positionen des Laufs.
10. Da die gewünschte Menge nicht alle Teile enthalten soll, sondern nur die Freigabeteile, aktivieren Sie in der im Dialog `Mengen-Erzeuger` die Checkbox `Master`.
11. Um unserer Menge die Kundennummer als Eigenschaft hinzuzufügen, wählen Sie im Menü `Menge` den Menüpunkt `Formel` aus. Es öffnet sich der Dialog `Auswahl Formeln --2--`. Betätigen Sie die Schaltfläche \[Neue Formel ...], um die Formel für die Kundennummer anzulegen. Es öffnet sich der Dialog `Formel Editor`.
12. Geben Sie im oberen linken Eingabefeld den Namen für die Formel ein. In unserem Beispiel `Kundennummer`.
13. Wählen Sie im Bereich `Vorhandene Eigenschaften` die `Kundennummer` mit einem Doppelklick aus. Im Bereich Formel erscheint `$Kundennummer`.
14. Betätigen Sie die Schaltfläche \[Ok]. Sie kehren zurück in den Dialog `Auswahl Formeln --2--`. Die Liste enthält nun als letzten Eintrag die soeben angelegte Formel für die Kundennummer. Markieren Sie die `Kundennummer` in der Liste und betätigen Sie die Schaltfläche \[Ok]. Sie kehren zurück in den Dialog `Mengen-Erzeuger`.
15. In der Statuszeile des Mengen-Erzeuger können Sie auf der rechten Seite sehen, ob und wenn ja, welche Formel bei der Bildung der neuen Menge benutzt wird. In unserem Beispiel steht dort: `Formel: Kundennummer`.
16. Schließen Sie nun alle geöffneten Dialog mit der Schaltfläche \[Ok], bis Sie wieder im Dialog `Gruppierung/Sortierung` angekommen sind.
17. Die Formel `Menge der Scheiben pro Kunde` ist jetzt in der Liste der Formeln enthalten. Markieren Sie die Formel und betätigen Sie die Schaltfläche \[Hinzufügen]. Die Formel wird den Gruppierungen im Register `Editor-Gruppierung` hinzugefügt. Sie steht Ihnen dann in den Einstellungen für die Orga-Gruppen und den Abstellplätzen jeweils im Bereich `Bildung der Gruppen` zur Verfügung.

### Bedingungen für Fertigungsabschnitte

Hier wird Ihnen erklärt, wie Sie im Bereich MZO Bedingungen für Fertigungsabschnitte definieren, ändern oder löschen.

#### So erstellen Sie eine Bedingung für einen Fertigungsabschnitt, der alle Scheiben mit Sprossen herausfiltert

1. Öffnen Sie den Dialog `Fertigungsabschnitte` über `Stammdaten > MZO > Konfiguration`.
2. Markieren Sie den Fertigungsabschnitt, für den Sie die Bedingung anlegen möchten.
3. Betätigen Sie die rechte Maustaste. Es öffnet sich das Kontext-Menü. Aus dem Kontext-Menü wählen Sie `Bedingung des Fertigungsabschnitts > Neu`.
4. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5. Betätigen Sie die Schaltfläche \[Neue Bedingung ...]. Es öffnet sich der Dialog `Bedingungen Erzeuger`.
6. Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Namen`. Es öffnet sich der Dialog `Name der Bedingung`. Vergeben Sie in diesem Feld einen sprechenden Namen für die Bedingung. In unserem Beispiel: `Bin Sprossen-ISO`. Schließen Sie den Dialog über die Schaltfläche \[OK].
7. Öffnen Sie im Menü `Bedingungen` den Menüpunkt `Info`. Es öffnet sich der Dialog `Info`. Vergeben Sie in diesem Feld eine eindeutige Beschreibung für die Bedingung. Beispiel: `Diese Bedingung ist wahr, wenn die Position ein Sprossenflag hat`. Schließen Sie den Dialog über die Schaltfläche \[OK].
8. Öffnen Sie im Menü `Teilbedingungen` den Menüpunkt `Hinzufügen (Spalte)`. Es erscheint eine neue Teilbedingung, die Sie konfigurieren können.
9. Die Kombobox ist standardmäßig vorbelegt mit `nur Formel 1`. Das bleibt in unserem Beispiel unverändert.
10. Die Radiotaste `Normal` ist standardmäßig aktiv. Es öffnet sich automatisch der Dialog `Eingabe Zahlenwert`. Das bleibt in unserem Beispiel ebenfalls unverändert.
11. Klicken Sie jetzt in das obere Eingabefeld der Bedingung. Es öffnet sich automatisch der Dialog `Auswahl Formeln --1--`.
12. Betätigen Sie die Schaltfläche \[Neue Formel ...]. Es öffnet sich der Dialog `Formel-Editor`. Im oberen linken Eingabefeld erfassen Sie einen möglichst sprechenden Namen für die Formel. In unserem Beispiel: `Sprossen`. ⇨ Softwarereferenz, "Eingabefeld oben" auf Seite F-718
13. Aus dem Bereich `Vorhandene Eigenschaften` wählen Sie mit einem Doppelklick `Pos_Sprossen_Flag`. Im Bereich Formel erscheint `$Pos_Sprossen_Flag`. ⇨ Softwarereferenz, "Vorhandene Eigenschaften" auf Seite F-719
14. Schließen Sie den Dialog über die Schaltfläche \[OK]. Sie befinden sich im Dialog `Auswahl Formeln --1--`. Die soeben angelegte Formel ist bereits markiert.
15. Schließen Sie den Dialog über die Schaltfläche \[OK]. Sie befinden sich wieder im Dialog `Bedingungen-Erzeuger`. _Abb. F-17: Bedingung: Bin ISO mit Sprosse_ Schließen Sie den Dialog entweder über das Menü `Bedingungen > OK` oder durch einen Klick auf `✓`. Sie befinden sich wieder im Dialog `Auswahl-Bedingungen --1--`. Die erstellte Bedingung `Bin Sprossen ISO` steht am Ende der Liste `Vorhandene Bedingungen`.

#### So weisen Sie einem Fertigungsabschnitt eine vorhandene Bedingung zu

1. Öffnen Sie den Dialog `Fertigungsabschnitt` über `Stammdaten > MZO > Konfiguration`.
2. Markieren Sie den Fertigungsabschnitt, dem Sie die Bedingung zuweisen möchten.
3. Betätigen Sie die rechte Maustaste. Es öffnet sich das Kontext-Menü. Aus dem Kontext-Menü wählen Sie `Bedingung des Fertigungsabschnitts > Neu`.
4. Es öffnet sich der Dialog `Auswahl Bedingungen --1--`.
5. Aus der Liste der `Vorhandenen Bedingungen` markieren Sie die Bedingung, die dem Fertigungsabschnitt zugewiesen werden soll.
6. Verlassen Sie den Dialog über die Schaltfläche \[OK].
7. Die Bedingung wurde dem markierten Fertigungsabschnitt angehängt.

#### So löschen Sie eine dem Fertigungsabschnitt zugewiesene Bedingung

1. Öffnen Sie den Dialog `Fertigungsabschnitt` über `Stammdaten > MZO > Konfiguration`.
2. Öffnen Sie den entsprechenden Fertigungsabschnitt durch einen Doppelklick.
3. Markieren Sie die Bedingung des Fertigungsabschnitts, die gelöscht werden soll.
4. Betätigen Sie die rechte Maustaste. Es öffnet sich das Kontext-Menü. Aus dem Kontext-Menü wählen Sie `Bedingung löschen`. Die Bedingung wird sofort gelöscht!

> **Löschen** Das Löschen erfolgt ohne Sicherheitsabfrage. Sollten Sie versehentlich etwas gelöscht haben, verlassen Sie den Dialog `Fertigungsabschnitte` über die Schaltfläche \[Abbrechen]. Wenn Sie ihn das nächste Mal öffnen, sind die Daten wieder vorhanden.

### Weitere Beispiele

#### So erstellen Sie eine Bedingung für ESG im ISO oder mit Bearbeitungen am Float

1. **Erster Schritt:** _Abb. F-18: Erster Schritt_ Dabei wird in Formel `Bin ESG` einfach die Eigenschaft `T_ESG` zurückgegeben.
2. **Nun die Überprüfung, ob das Teil im ISO eingebaut wird:**
   *
     1. Elementarbedingung mit Property `T_VSG`
   *
     2. Allgemeine Mengenbeschreibung für die Gegenscheibe
   *
     3. Zusammengesetzte Startmenge
   *
     4. Minus- oder Abzugsmenge _Abb. F-19: Prüfen_ Die Mengenoperation fängt mit der Startmenge an und sucht sich dann von allen Elternteilen die direkten Unterteile, subtrahiert im Anschluss sich selbst, so dass als Endmenge alle Gegenscheiben übrig bleiben.
3. **Da ein Teil nicht gleichzeitig ESG und ISO sein kann, wird die in Schritt 2 gezeigte Bedingung so nicht funktionieren. Daher ...** _Abb. F-20: Abbildung_
4. **Jetzt noch die Oder-Verknüpfung, ob eins der Unterteile eine Bearbeitung ist. Dazu wird eine weitere Bedingung erzeugt, die für alle Unterteile die Formel `Bin Bearbeitung` prüft.** _Abb. F-21: Bedingung_

#### Die Bearbeitungen direkt unter mir

1. Die Endmenge soll nur die Bearbeitungen unter dem Startteil enthalten, die nach den letzten erzeugenden Bearbeitungen unter dem Startteil erfolgen.
2. Dazu wird zunächst die Menge aller Unterteile gebildet, die keine Bearbeitungen sind.
3. Menge Erzeugende Bearbeitungen unter mir = `{ ; ANYCHILD ; Bedingung Ist keine Bearbeitung; }`
4. Mit Hilfe dieser Menge wird nun die Menge aller Teile und Bearbeitungen unterhalb des Startteils erzeugt, die man nicht haben will.
5. Menge Unerwünschte Teile/Bearbeitungen unter mir = `{ Menge Erzeugende Bearbeitungen unter mir; ANYCHILD+SELF ; ; }`
6. Die gewünschte Menge ergibt sich dann aus der Menge `Alle Unterteile` und der Menge `Unerwünschte Teile/Bearbeitungen unter mir`. `{ Menge Alle Unterteile - Menge Unerwünschte Teile/Bearbeitungen unter mir; SELF ; ; }`

### Übersicht der betroffenen Dialoge

Die Übersicht zeigt Ihnen alle Dialoge, die Sie zur vollständigen Nutzung des Formeleditors benötigen. Die Verweise führen Sie in das Kapitel Softwarereferenz des Stammdatenbereichs. Dort finden Sie detaillierte Informationen zu den Dialogen mit ihren Feldern und Schaltflächen.

#### Menü Stammdaten

| Menü-Eintrag                                                                                                                               | Dialog/Funktion                                                                                                                                                                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Der Formel-Editor ist nicht über einen Menü-Eintrag zu erreichen. Wie Sie ihn erreichen, ist bei den jeweiligen Dialogen genau beschrieben | <p>⇨ "Auswahl Bedingungen" auf Seite F-694<br>⇨ “Bedingungen - Erzeuger" auf Seite F-696<br>⇨ "Bedingung" auf Seite F-699<br>⇨ "Name der Bedingung" auf Seite F-701<br>⇨ "Info" auf Seite F-714<br>⇨ "Auswahl Formeln" auf Seite F-715<br>⇨ "Formel - Editor" auf Seite F-717<br>⇨ "Auswahl Zuweisung" auf Seite F-720<br>⇨ "Zuweisung - Editor" auf Seite F-720</p> |

_Tab. F-1: Übersicht der betroffenen Dialoge_

## Softwarereferenz: A+W Formeleditor

### Formel-Editor

Der Formel-Editor kommt in A+W Production in den folgenden Bereichen zum Einsatz:

* Organisation
* Maschinenzuordnung
* Etiketten, Skizzen, Biegertexte

Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative Wege einen Dialog aufzurufen, so sind diese ebenfalls angegeben.

#### Auswahl Bedingungen

**Aufruf über**

**Organisation**

* `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga-Gruppe markieren > [Neue Bedingung]`
* `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > [Neue Bedingung]`

**Maschinenzuordnung**

* `Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte Maustaste > Bedingung des Fertigungsabschnitts > Neu`
* `Stammdaten > MZO > Konfiguration > Bedingung des Fertigungsabschnitts markieren > rechte Maustaste > Bedingung editieren`
* `Stammdaten > MZO > Konfiguration > [Technologie] > [Neu] > [Neu]`
* `Stammdaten > MZO > Konfiguration > [Technologie] > [Ändern] > [Neu]/[Editieren]`

**Etiketten, Skizzen, Biegertexte**

* `Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration > Bedingung markieren > [Formel Editor]`

_Abb. F-22: Auswahl Bedingungen --1--_

In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte vorhandene Bedingungen ausgewählt, geändert oder neue Bedingungen angelegt werden.

**Erläuterung der Felder**

* **Vorhandene Bedingungen:** Die Tabelle listet alle im System vorhandenen Bedingungen für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte. Die Inhalte sind für die jeweiligen Bereiche unterschiedlich!
* **Keine Bedingung:** Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis, dass Nichts als selektiert gilt.
* **Beschreibung:** Das Feld enthält eine detaillierte Erläuterung zu der Bedingung. Dabei handelt es sich um den Text, den Sie im Feld Info erfassen. ⇨ Softwarereferenz, "Info" auf Seite F-702

**Erläuterung der Schaltflächen**

* **Löschen:** Betätigen Sie diese Schaltfläche, wird die zuvor markierte Bedingung gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfrage. Sollten Sie jedoch versehentlich etwas gelöscht haben, kehren Sie in den ursprünglichen Dialog (Orga-Dialog, Etikettenart-Dialog, etc.) zurück. Wenn Sie diesen dann über \[Abbrechen] schließen, werden Sie gefragt, ob die durchgeführten Änderungen ignoriert werden sollen oder nicht.
* **Neue Bedingung:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Bedingungen - Erzeuger. Sie können dann eine neue Bedingung anlegen. ⇨ Softwarereferenz, "Bedingungen - Erzeuger" auf Seite F-696
* **Editieren:** Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Bedingung der Dialog Bedingungen - Erzeuger. ⇨ Softwarereferenz, "Bedingungen - Erzeuger" auf Seite F-696

**Weitere Informationen zu Bedingungen**

* ⇨Tutorial, "Elemente des Formeleditors: Stufe I" auf Seite F-659
* ⇨Tutorial, "Elemente des Formeleditors: Stufe II" auf Seite F-665

#### Bedingungen - Erzeuger

**Aufruf über**

**Organisation**

* `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga-Gruppe markieren > [Neue Bedingung] > [Neue Bedingung ...] / [Editieren]`
* `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > [Neue Bedingung] > [Neue Bedingung ...] / [Editieren]`

**Maschinenzuordnung**

* `Stammdaten > MZO > Konfiguration > Fertigungsabschnitt markieren > rechte Maustaste > Bedingung des Fertigungsabschnitts > Neu > [Neue Bedingung ...] / [Editieren]`
* `Stammdaten > MZO > Konfiguration > Bedingung des Fertigungsabschnitts markieren > rechte Maustaste > Bedingung editieren > [Neue Bedingung ...]/[Editieren]`

**Etiketten, Skizzen, Biegertexte**

* `Stammdaten > Etiketten / Skizzen / Biegertexte > Konfiguration > Bedingung markieren > [Formel-Editor] > [Neue Bedingung ...] / [Editieren]`

_Abb. F-23: Bedingungen - Erzeuger_

Im Bedingungen - Erzeuger können Sie entweder eine zuvor markierte Bedingung ändern oder neue Bedingungen anlegen. Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die sich in den Menüs `Bedingungen` und `Teilbedingungen` befinden.

| Menü-Eintrag              | Dialog/Funktion                        |
| ------------------------- | -------------------------------------- |
| **Menü Bedingungen:**     |                                        |
| Name                      | ⇨ "Name der Bedingung" auf Seite F-701 |
| Info                      | ⇨ "Info" auf Seite F-702               |
| Menge                     | ⇨ "Auswahl Mengen" auf Seite F-706     |
| Invertieren               | ⇨ "Invertieren" auf Seite F-702        |
| Übergebene Menge          | ⇨ "Übergebene Menge" auf Seite F-703   |
| OK                        | Tab. auf Seite F-697                   |
| Abbruch                   | Tab. auf Seite F-697                   |
| **Menü Teilbedingungen:** |                                        |
| Hinzufügen (Spalte)       | Tab. auf Seite F-697                   |
| Hinzufügen (Zeile)        | Tab. auf Seite F-697                   |
| Entfernen                 | Tab. auf Seite F-697                   |

_Tab. F-2: Übersicht der Dialoge in den Menüs Bedingungen und Teilbedingungen_

**Werkzeugleiste**

| Werkzeug | Erläuterung                                                                                                                                                                                                |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ✓        | Die definierte Bedingung wird gespeichert und der Editor verlassen.                                                                                                                                        |
| X        | Die definierte Bedingung wird verworfen und der Editor verlassen.                                                                                                                                          |
| `++`     | Es öffnet sich das Bearbeitungsfenster zum Definieren der Bedingung. Bei zweimaligem Anklicken öffnen sich zwei Fenster nebeneinander, die eine Und-Verknüpfung darstellen. ⇨ "Bedingung" auf Seite F-699  |
| `‡`      | Es öffnet sich das Bearbeitungsfenster zum Definieren der Bedingung. Bei zweimaligem Anklicken öffnen sich zwei Fenster untereinander, die eine Oder-Verknüpfung darstellen. ⇨ "Bedingung" auf Seite F-699 |
| `-`      | Die selektierte Bedingung wird gelöscht.                                                                                                                                                                   |

_Tab. F-3: Werkzeugleiste im Bedingungen - Erzeuger_

**Erläuterung der Radiotasten**

* **All:** Die Bedingungen aller Teile einer Stückliste werden berücksichtigt. Bei dieser Einstellung wird z.B. auch eine Scheibe ohne Struktur einem Abstellplatz mit der Bedingung Struktur zugeordnet, wenn ihre Gegenscheibe strukturiert ist.
* **One:** Es werden nur die Eigenschaften der aktuellen Scheibe berücksichtigt.
* **Null:** Die der Bedingung zugeordnete Menge wird nicht berücksichtigt.

#### Bedingung

**Aufruf über**

* `Stammdaten > Feinplanung > Orga > ... > [Neue Bedingung] > [Neue Bedingung ...] > Menü Teilbedingungen > Hinzufügen`
* `Stammdaten > MZO > Konfiguration > ... > [Neue Bedingung ...] > Menü Teilbedingungen > Hinzufügen`
* `Stammdaten > Etiketten / Skizzen / Biegertexte > ... > [Formel-Editor] > [Neue Bedingung ...] > Menü Teilbedingungen > Hinzufügen`

_Abb. F-24: Bedingung_

* **Oberes Eingabefeld:** Klicken Sie mit der Maus in das Feld, öffnet sich der Dialog `Auswahl Formeln`. Sie können dort entweder eine bereits definierte Formel auswählen oder eine neue Formel erstellen. ⇨ Softwarereferenz, "Auswahl Formeln" auf Seite F-715
* **Mittleres Auswahlfeld:** Öffnen Sie die Kombobox und wählen Sie den gewünschten Operator aus. Mögliche Werte:
  * `nur Formel 1`
  * `== gleich`
  * `!= ungleich`
  * `< kleiner`
  * `<= kleiner gleich`
  * `> größer`
  * `>= größer gleich`
* **Unteres Eingabefeld:** Klicken Sie mit der Maus in das Feld, öffnet sich entweder der `Dialog Auswahl Formeln`, der `Dialog Eingabe Zahlenwert` oder der `Dialog Auswahl Bedingungen`. Welcher Dialog sich öffnet, hängt davon ab, welche Radiotaste (Normal, Wert, Bedingungen) aktiv ist. ⇨ Softwarereferenz, "Auswahl Formeln" auf Seite F-715 ⇨ Softwarereferenz, "Eingabe Zahlenwert" auf Seite F-704 ⇨ Softwarereferenz, "Auswahl Bedingungen" auf Seite F-694
* **Normal:** Aktivieren Sie diese Radiotaste und klicken anschließend in das untere Eingabefeld, öffnet sich der Dialog `Auswahl Formeln`.
* **Wert:** Aktivieren Sie diese Radiotaste, öffnet sich der Dialog `Eingabe Zahlenwert`.
* **Bedingungen:** Aktivieren Sie diese Radiotaste und klicken anschließend in das untere Eingabefeld, öffnet sich der Dialog `Auswahl Bedingungen --2 --`.

**Weitere Informationen zu der Bedingung**

* ⇨ "Elemente des Formeleditors: Stufe I" auf Seite F-659
* ⇨ "Elemente des Formeleditors: Stufe II" auf Seite F-665

#### Name der Bedingung

**Aufruf über**

* **Organisation:** `Stammdaten > Feinplanung > Orga > ... > [Neue Bedingung ...] > Menü Bedingungen > Name`
* **Maschinenzuordnung:** `Stammdaten > MZO > Konfiguration > ... > [Neue Bedingung ...] > Menü Bedingungen > Name`
* **Etiketten, Skizzen, Biegertexte:** `Stammdaten > Etiketten / Skizzen / Biegertexte > ... > [Formel-Editor] > [Neue Bedingung ...] > Menü Bedingungen > Name`

_Abb. F-25: Name der Bedingung_

In diesem Dialog vergeben Sie einen sprechenden Namen für die Bedingungen. Der Name wird in der Statuszeile des Dialogs `Bedingungen - Erzeuger` angezeigt.

**Erläuterung der Felder**

* **Alte Bezeichnung:** Wenn für eine Bedingung noch keine Bezeichnung vergeben wurde, steht in diesem Feld standardmäßig `neue Bedingung`. Wurde bereits eine Bezeichnung vergeben, steht diese dann dort.
* **Neue Bezeichnung:** Geben Sie in diesem Feld die Bezeichnung für die Bedingung ein. Sie kann jederzeit überschrieben werden. Die eingetragene Bezeichnung erscheint in Statuszeile des `Bedingungen - Erzeuger`.

#### Info

**Aufruf über**

* **Organisation:** `Stammdaten > Feinplanung > Orga > ... > [Neue Bedingung ...] > Menü Bedingungen > Info`
* **Maschinenzuordnung:** `Stammdaten > MZO > Konfiguration > ... > [Neue Bedingung ...] > Menü Bedingungen > Info`
* **Etiketten, Skizzen, Biegertexte:** `Stammdaten > Etiketten / Skizzen / Biegertexte > ... > [Formel-Editor] > [Neue Bedingung ...] > Menü Bedingungen > Info`

_Abb. F-26: Info zur Bedingung_

In diesem Bereich können Sie den Inhalt der Bedingung beschreiben. Der Text erscheint im Dialog `Auswahl Bedingungen` im Bereich `Beschreibung`.

**Invertieren**

Zunächst kann eine Bedingung invertiert werden. D.h. die Bedingung ist erfüllt, falls das Resultat der Vergleiche nicht erfüllt ist und umgekehrt. Damit lässt sich einfach aus einer schon existierenden Bedingung die umgekehrte Bedingung erstellen. Die umgekehrte Bedingung enthält genau einen Vergleich, der die ursprüngliche Bedingung zugewiesen bekommt. Außerdem wird für die umgekehrte Bedingung die Eigenschaft `invertieren` ausgewählt. In der Statuszeile erscheint ein `INV` vor dem Namen der Bedingung. Der Menüpunkt ist zu aktivieren bzw. zu deaktivieren.

#### Übergebene Menge

Dieser Menüpunkt ist zu aktivieren bzw. zu deaktivieren. Ist er aktiv, wird bei der Bildung der Mengen nicht nur die Position, über die der Dialog `Bedingungen - Erzeuger` geöffnet wurde, berücksichtigt, sondern alle Positionen des Laufs.

#### Eingabe Zahlenwert

**Aufruf über**

* **Organisation:** `Stammdaten > Feinplanung > Orga > ... > Radiotaste [Wert] aktivieren`
* **Maschinenzuordnung:** `Stammdaten > MZO > Konfiguration > ... > Radiotaste [Wert] aktivieren`
* **Etiketten, Skizzen, Biegertexte:** `Stammdaten > Etiketten / Skizzen / Biegertexte > ... > Radiotaste [Wert] aktivieren`

_Abb. F-27: Eingabe Zahlenwert_

Dieser Dialog dient der Eingabe von Zahlenwerten. Durch das Aktivieren der entsprechenden Radiotaste, können Sie darüber hinaus spezifizieren, ob es sich bei dem Zahlenwert um Ziffer, Dicke, Text, Länge oder SZR handelt.

**Erläuterung der Felder**

* **Alter Wert:** Wenn für eine Bedingung noch kein Wert vergeben wurde, steht in diesem Feld standardmäßig 0. Wurde bereits ein Wert vergeben, steht dieser dann dort.
* **Neuer Wert:** Geben Sie in diesem Feld den Wert für die Bedingung ein. Der Wert kann jederzeit überschrieben werden.

**Erläuterung der Radiotasten**

* **Ziffer:** Bezieht sich die Bedingung z.B. auf eine Stückzahl, aktivieren Sie diese Radiotaste und geben im Feld `Neuer Wert` den entsprechende Ziffer ein. Bsp.: Menge > 10, Glasart = 1700
* **Dicke:** Bezieht sich die Bedingung auf eine Dicke, aktivieren Sie diese Radiotaste und geben im Feld `Neuer Wert` den entsprechende Dicke in mm ein.
* **Text:** Bezieht sich die Bedingung auf einen Text, aktivieren Sie diese Radiotaste und geben im Feld `Neuer Wert` den entsprechenden Text ein.
* **Länge:** Bezieht sich die Bedingung auf eine Länge, aktivieren Sie diese Radiotaste und geben im Feld `Neuer Wert` die entsprechende Länge ein.
* **SZR:** Bezieht sich die Bedingung auf einen Scheibenzwischenraum, aktivieren Sie diese Radiotaste und geben im Feld `Neuer Wert` den entsprechende SZR ein.

#### Auswahl Mengen

**Aufruf über**

* **Organisation:** `Stammdaten > Feinplanung > Orga > ... > Teilbedingung klicken > [Neue Formel ...] > [Menge ...]`
* **Maschinenzuordnung:** `Stammdaten > MZO > Konfiguration > ... > Teilbedingung klicken > [Neue Formel ...] > [Menge ...]`
* **Etiketten, Skizzen, Biegertexte:** `Stammdaten > Etiketten / Skizzen / Biegertexte > ... > Teilbedingung klicken > [Neue Formel ...] > [Menge ...]`

_Abb. F-28: Auswahl Mengen_

In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte vorhandene Mengen ausgewählt, geändert oder neue Mengen angelegt werden.

**Erläuterung der Felder**

* **Vorhandene Mengen:** Die Tabelle listet alle im System vorhandenen Mengen für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte. Die Inhalte sind für die jeweiligen Bereiche unterschiedlich!
* **Keine Menge:** Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis, dass Nichts als selektiert gilt.
* **Beschreibung:** Das Feld enthält eine detaillierte Erläuterung zu der Menge. Dabei handelt es sich um den Text, den Sie im Feld Info erfassen. ⇨ "Info" auf Seite F-702

**Erläuterung der Schaltflächen**

* **Löschen:** Betätigen Sie diese Schaltfläche, wird die zuvor markierte Menge gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfrage.
* **Neue Menge:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Mengen - Erzeuger. Sie können dann eine neue Menge anlegen. ⇨ "Mengen - Erzeuger" auf Seite F-708
* **Editieren:** Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Menge der Dialog Mengen - Erzeuger. ⇨ "Mengen - Erzeuger" auf Seite F-708

#### Mengen - Erzeuger

**Aufruf über**

* **Organisation:** `Stammdaten > Feinplanung > Orga > ... > [Neu Menge ...] / [Editieren]`
* **Maschinenzuordnung:** `Stammdaten > MZO > Konfiguration > ... > [Neu Menge ...] / [Editieren]`
* **Etiketten, Skizzen, Biegertexte:** `Stammdaten > Etiketten / Skizzen / Biegertexte > ... > [Neu Menge ...] / [Editieren]`

_Abb. F-29: Mengen - Erzeuger_

Im Mengen - Erzeuger können Sie entweder eine zuvor markierte Menge ändern oder neue Menge anlegen. Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die sich in den Menüs Menge und Teilmengen befinden.

| Menü-Eintrag         | Dialog/Funktion                         |
| -------------------- | --------------------------------------- |
| **Menü Menge:**      |                                         |
| Name                 | ⇨ "Name der Menge" auf Seite F-712      |
| Info                 | ⇨ "Info" auf Seite F-714                |
| Bedingung            | ⇨ "Auswahl Bedingungen" auf Seite F-694 |
| Formel               | ⇨ "Auswahl Formeln" auf Seite F-715     |
| OK                   | Tab. auf Seite F-710                    |
| Abbruch              | Tab. auf Seite F-710                    |
| **Menü Teilmengen:** |                                         |
| Hinzufügen (Spalte)  | Tab. auf Seite F-710                    |
| Hinzufügen (Zeile)   | Tab. auf Seite F-710                    |
| Entfernen            | Tab. auf Seite F-710                    |
| Wechsel              | Tab. auf Seite F-710                    |

_Tab. F-4: Übersicht der Dialoge in den Menüs Menge und Teilmengen_

**Werkzeugleiste**

| Werkzeug | Erläuterung                                                                                                                                                                                            |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ✓        | Die definierte Menge wird gespeichert und der Editor verlassen.                                                                                                                                        |
| X        | Die definierte Menge wird verworfen und der Editor verlassen.                                                                                                                                          |
| `++`     | Es öffnet sich das Bearbeitungsfenster zum Definieren der Menge. Bei zweimaligem Anklicken öffnen sich zwei Fenster nebeneinander, die eine Und-Verknüpfung darstellen.                                |
| `‡`      | Es öffnet sich das Bearbeitungsfenster zum Definieren der Menge. Bei zweimaligem Anklicken öffnen sich zwei Fenster untereinander, die eine Oder-Verknüpfung darstellen. ⇨ "Bedingung" auf Seite F-699 |
| `-`      | Die selektierte Menge wird gelöscht.                                                                                                                                                                   |
| `+/-`    | Dient dem Umschalten zwischen dem ersten und dem zweiten Fenster.                                                                                                                                      |

_Tab. F-5: Werkzeugleiste im Mengen - Erzeuger_

**Erläuterung der Checkboxen**

* **All:** Alle Teile des Teilebaums, in dem das Startteil enthalten ist.
* **Master:** Das oberste Teil des Teilebaums (Kopfteil), in dem das Startteil enthalten ist.
* **Parent:** Das Teil, das sich im Teilebaum direkt über dem Startteil befindet.
* **Self:** Das Startteil.
* **Child:** Alle direkten Unterteile des Startteils.
* **Anychild:** Alle Unterteile des Startteils, auch die indirekten.
* **Bottom:** Alle Basisteile, die sich unter dem Startteil befinden.
* **Up:** Unter Verwendung von `Up` besteht die Endmenge genau aus einem Teil. Dabei werden vom Startteil ausgehend alle Oberteile des Startteils untersucht, ob das jeweilige Teil die Bedingung erfüllt. In der Endmenge befindet sich das letzte Teil, das die Bedingung erfüllt hat. Erfüllt ein Teil die Bedingung nicht, so wird die Iteration nach oben abgebrochen.
* **Addup:** Unter Verwendung von `Addup` kann die Endmenge aus mehr als einem Teil bestehen. Wie bei `Up` wird ebenfalls vom Startobjekt nach oben iteriert und die Iteration beendet, falls ein Teil die Bedingung nicht erfüllt. Aber die Endmenge enthält alle Teile, die die Bedingung erfüllt haben.

**Weitere Informationen**

* ⇨ Tutorial, "Elemente des Formeleditors: Stufe III" auf Seite F-669

#### Name der Menge

**Aufruf über**

* **Organisation, Maschinenzuordnung, Etiketten, etc.:** `... > Menü Menge > Name`

_Abb. F-30: Name der Menge_

In diesem Dialog vergeben Sie einen sprechenden Namen für die Menge. Der Name wird in der Statuszeile des Dialogs `Mengen - Erzeuger` angezeigt.

**Felder**

* **Alte Bezeichnung:** Wenn für eine Menge noch keine Bezeichnung vergeben wurde, steht in diesem Feld standardmäßig `neue Menge`. Wurde bereits eine Bezeichnung vergeben, steht diese dann dort.
* **Neue Bezeichnung:** Geben Sie in diesem Feld die Bezeichnung für die Bedingung ein. Sie kann jederzeit überschrieben werden. Die eingetragene Bezeichnung erscheint in Statuszeile des `Bedingungen - Erzeuger`.

#### Info (zur Menge)

**Aufruf über**

* **Organisation, Maschinenzuordnung, Etiketten, etc.:** `... > Menü Menge > Info`

_Abb. F-31: Info zur Menge_

In diesem Bereich können Sie den Inhalt der Bedingung beschreiben. Der Text erscheint im Dialog `Auswahl Mengen` im Bereich `Beschreibung`.

#### Auswahl Formeln

**Aufruf über**

* **Organisation, Maschinenzuordnung, Etiketten, etc.:** Klicken mit der Maus in das erste Eingabefeld der Teilbedingung.

_Abb. F-32: Auswahl Formeln_

In diesem Dialog können für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte vorhandene Formeln ausgewählt, geändert oder neue Formeln angelegt werden.

**Felder**

* **Vorhandene Formeln:** Die Tabelle listet alle im System vorhandenen Formeln für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte.
* **Keine Formel:** Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis, dass Nichts als selektiert gilt.
* **Beschreibung:** Das Feld enthält eine detaillierte Erläuterung zu der Formel. Dabei handelt es sich um den Text, den Sie im Feld Beschreibung erfassen. ⇨ "Beschreibung" auf Seite F-718

**Schaltflächen**

* **Löschen:** Betätigen Sie diese Schaltfläche, wird die zuvor markierte Formel gelöscht.
* **Neue Formel:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog `Formel - Editor`. Sie können dann eine neue Formel anlegen. ⇨ "Formel - Editor" auf Seite F-717
* **Editieren:** Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Formel der Dialog `Formel - Editor`. ⇨ "Formel - Editor" auf Seite F-717

**Weitere Informationen zu den Formeln**

* ⇨Tutorial, "Elemente des Formeleditors: Stufe I" auf Seite F-659
* ⇨Tutorial, "Elemente des Formeleditors: Stufe II" auf Seite F-665
* ⇨Tutorial, "Elemente des Formeleditors: Stufe III" auf Seite F-669

#### Formel - Editor

**Aufruf über**

* **Organisation, Maschinenzuordnung, Etiketten, etc.:** `... > [Neue Formel ...]`

_Abb. F-33: Formel - Editor_

In diesem Dialog können Sie neue Formeln erstellen. Eine Formel in ihrer einfachsten Art ist lediglich ein Feld der Datenbank. Im Bereich `Vorhandene Eigenschaften` finden Sie eine Liste der Datenbankfelder. Markieren Sie eines der Datenbankfelder, erscheint im grauen Bereich darunter die Erklärung des Feldinhaltes. Es können natürlich auch viel kompliziertere Formeln erstellt werden, mehrere Felder verknüpft, bzw. eine oder mehrere der schon vorhandenen Formeln benutzt werden.

**Felder**

* **Eingabefeld oben:** Geben Sie in diesem Feld einen möglichst sprechenden Namen für die Formel ein.
* **Beschreibung:** In diesem Feld geben Sie eine möglichst detaillierte Beschreibung zu der Formel an.
* **Formel:** In diesem Feld wird das für die Formel benötigte Datenbankfeld eingetragen. D.h. Sie suchen sich im Bereich `Vorhandene Eigenschaften` das entsprechende Datenbankfeld aus und klicken doppelt darauf. Das Datenbankfeld wird dann automatisch in den Bereich `Formel` übertragen.
* **Menge:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog `Auswahl Mengen`. Dort können Sie dann eine bereits vorhandene Menge auswählen oder eine neue Menge erstellen. ⇨ Softwarereferenz, "Auswahl Mengen" auf Seite F-706
* **Übergebene Menge (Checkbox):** Ist die Checkbox aktiv, wird bei der Bildung der Mengen nicht nur die Position, über die der Dialog `Auswahl Mengen` geöffnet wurde, berücksichtigt, sondern alle Positionen des Laufs. Nur bei aktivierter Checkbox sind die Radiotasten im Bereich `Operation` ebenfalls aktiv.

**Radiotasten im Bereich Operation**

Die Radiotasten in diesem Bereich sind nur aktiv, wenn die Checkbox `Übergebene Menge` aktiv ist. D.h. wenn der Formel eine Menge zugewiesen wurde. Dann wird zunächst für alle Teile dieser Menge die Formel ausgewertet. Die Ergebnisse der Formel werden wie folgt verarbeitet:

* **Summe (Wert):** Summe aller Ergebnisse
* **Mittelwert:** Summe/Anzahl Ergebnisse
* **Und-Verknüpfung:** Die Ergebnisse werden durch logisches Und verknüpft
*   **Oder-Verknüpfung:** Die Ergebnisse werden durch logisches Oder verknüpft

    > **Und-/Oder-Verknüpfungen** Und-/Oder-Verknüpfungen machen nur richtig Sinn, wenn Formeln als Ergebnis 0 oder 1 liefern!
* **Minimum:** Kleinstes Ergebnis
* **Maximum:** Größtes Ergebnis
* **Anzahl Resultate:** Anzahl der verschiedenen Ergebnisse

**Felder (Vorhandene Eigenschaften/Formeln)**

*   **Vorhandene Eigenschaften:** Die Tabelle listet Datenbankfelder für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte. Wird ein Feld markiert, erscheint unterhalb eine Erklärung des Feldinhaltes.

    > **Vorhandene Eigenschaften (Properties)** Objekteigenschaften (Properties) innerhalb der Orga sind aus Performance-Gründen fest verdrahtet und können nicht ohne Programmänderung erweitert werden. Objekteigenschaften (Properties) innerhalb der MZO und Etiketten können dynamisch über das Script DBInit erweitert werden.
* **Vorhandene Formeln:** Die Tabelle listet alle im System vorhandenen Formeln für die Bereiche Organisation, Maschinenzuordnung und Etiketten, Skizzen, Biegertexte.

**Weitere Informationen zum Formel-Editor**

* ⇨Tutorial, "Elemente des Formeleditors: Stufe I" auf Seite F-659
* ⇨Tutorial, "Elemente des Formeleditors: Stufe II" auf Seite F-665
* ⇨Tutorial, "Elemente des Formeleditors: Stufe III" auf Seite F-669

#### Auswahl Zuweisung

**Aufruf über**

* `Stammdaten > Feinplanung > Zuweisungen`

_Abb. F-34: Auswahl Zuweisung_

In diesem Dialog können Sie nur für den Bereich der Orga vorhandene Zuweisungen auswählen, ändern oder neue Zuweisungen anlegen.

**Felder**

* **Vorhandene Zuweisungen:** Die Tabelle listet alle im System vorhandenen Zuweisungen für den Bereich der Orga.
* **Keine Zuweisung:** Ist diese Checkbox aktiv, so liefert der Dialog als Ergebnis, dass Nichts als selektiert gilt.
* **Beschreibung:** Das Feld enthält eine detaillierte Erläuterung zu der Zuweisung. Dabei handelt es sich um den Text, den Sie im Feld Info erfassen. ⇨ Softwarereferenz, "Info" auf Seite F-702

**Schaltflächen**

* **Löschen:** Betätigen Sie diese Schaltfläche, wird die zuvor markierte Zuweisung gelöscht. Die Löschung erfolgt in diesem Dialog ohne Sicherheitsabfrage. Sollten Sie jedoch versehentlich etwas gelöscht haben schließen Sie den Dialog über \[Abbrechen]. Die Änderungen werden ignoriert.
* **Neue Zuweisung:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog `Zuweisung - Editor`. Sie können dann eine neue Bedingung anlegen. ⇨ Softwarereferenz, "Zuweisung - Editor" auf Seite F-720
* **Editieren:** Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Zuweisung der Dialog `Zuweisung - Editor`. ⇨ Softwarereferenz, "Zuweisung - Editor" auf Seite F-720

#### Zuweisung - Editor

**Aufruf über**

* `Stammdaten > Feinplanung > Zuweisungen > [Neue Zuweisung ...]`

_Abb. F-35: Zuweisung - Editor_

In diesem Dialog können Sie eine Zuweisung definieren. In der einfachsten Form besteht eine Zuweisung aus einer Objekt-Eigenschaft (Property) und einer Formel. Das Ergebnis der Formel wird der Eigenschaft des Objektes zugewiesen. Die Zuweisung kann jedoch auch eine Menge enthalten. Dann wird für alle Objekte der Endmenge das jeweilige Ergebnis der Formel der jeweiligen Eigenschaft zugewiesen.

**Felder**

* **Eingabefeld oben:** In diesem Feld vergeben Sie einen sprechenden Namen für die Zuweisung. Haben Sie den Dialog Zuweisung - Editor über die Schaltfläche \[Neue Zuweisung ...] geöffnet, steht in diesem Feld standardmäßig `neue Zuweisung`. Haben Sie den Dialog über die Schaltfläche \[Editieren] geöffnet, steht in dem Feld der Name der Zuweisung, die Sie bearbeiten möchten.
*   **Eigenschaft:** Wenn Sie die Kombobox öffnen, werden Ihnen die Datenbankfelder, die im Bereich der Feinplanung änderbar sind, angezeigt. Nachdem Sie das gewünschte Datenbankfeld ausgewählt haben, erscheint im grauen Bereich rechts neben der Kombobox die Erklärung des Feldinhaltes.

    > **Vorhandene Eigenschaften (Properties)** Objekteigenschaften (Properties) innerhalb der Feinplanung sind aus Performance-Gründen fest verdrahtet und können nicht ohne Programmänderung erweitert werden.

**Wichtige Zuweisungen:**

* **Abstellbreite:** Wird für eine eventuell verwendete Gestellbelegung verwendet. Im Normalfall ist diese Eigenschaft mit der Breite der Scheibe belegt.
* **Bewertung:** Im Normalfall mit 100 belegt. Dient innerhalb der Optimierung dazu Scheiben auf mehrere Lagerplatten zu verteilen. Je kleiner der Wert umso stärker ist diese Verschmierung. Damit kann zum Beispiel erreicht werden, dass für große Schieben nicht alle Schieben einer Einheit auf einem Lagerblatt liegen.
* **Dickendifferenz:** Für Auffüller kann hiermit eingestellt werden, um wie stark sich die Glasdicke durch das Auffüllen ändern darf.
* **Gruppennummer:** Ist per Standard mit 0 belegt. Sollten innerhalb der Feinplanung Fertigungsgruppen via dieser Gruppennummer gebildet werden, so ist diese Eigenschaft zunächst mit der geeigneten Formel zu belegen.
* **Kiste:** Ist frei verfügbar.
* **Zuschlagdicke:** Ist per Standard mit 0 mm belegt. Hiermit lässt sich erreichen, dass beim Abstellen auf A-Böcke eine größere Dicke für eine Scheibe berücksichtigt wird als dies durch ihre Glasdicke der Fall ist. Zum Beispiel wird dies verwendet für Scheiben mit Siebdruck. Um den Siebdruck zu schützen wird nach jeder Scheibe ein Stück Pappe mit einer Dicke von X mm davor gestellt. Diesen Wert weißt man hier der Zuschlagdicke zu. Damit dies nur für Scheiben mit Siebdruck erfolgt muss natürlich die Menge entsprechend gewählt sein.
* **Formel ...:** Wenn Sie diese Schaltfläche betätigen, öffnen Sie den Dialog `Auswahl Formeln`. ⇨ Softwarereferenz, "Auswahl Formeln" auf Seite F-715
* **Grau hinterlegtes Feld (Formel):** Wenn Sie über die Schaltfläche \[Formel ...] eine solche ausgewählt haben, erhalten Sie in diesem Feld den Namen der Formel angezeigt.
* **Menge ...:** Wenn Sie diese Schaltfläche betätigen, öffnen Sie den Dialog `Auswahl Mengen`. Er dient sowohl dazu für weitere Teile (nicht nur dem aktuellen Teil) die Zuweisung durchzuführen, als auch nur für bestimmte Teile die Zuweisung anwendung zu dürfen. ⇨ Softwarereferenz, "Auswahl Mengen" auf Seite F-706
* **Übergebene Menge (Checkbox):** Ist die Checkbox aktiv, wird bei der Bildung der Mengen nicht nur die Position, über die der Dialog `Auswahl Mengen` geöffnet wurde, berücksichtigt, sondern alle Positionen des Laufs.
* **Grau hinterlegtes Feld (Menge):** Wenn Sie über die Schaltfläche \[Menge ...] eine solche ausgewählt haben, erhalten Sie in diesem Feld den Namen der Menge angezeigt.

**Weitere Informationen zu der Zuweisung**

* ⇨ Tutorial, "Elemente des Formeleditors: Stufe I" auf Seite F-659
* ⇨ Tutorial, "Elemente des Formeleditors: Stufe II" auf Seite F-665

## Maschinenzuordnung

***

### _Vorspann, Editorial und Inhaltsverzeichnis des Handbuchs. Diese Metainformationen beschreiben den Aufbau, die Versionierung und die rechtlichen Hinweise des Dokuments._

## Tutorial: Maschinenzuordnung

### Überblick

Das Tutorial zum Modul Maschinenzuordnung (MZO) beschäftigt sich mit der Zuweisung von Bearbeitungen zu Maschinen in A+W Production. Die Maschinenzuordnung weist die anstehenden Bearbeitungen den einzelnen Maschinen zu und berücksichtigt dabei Maschinenrestriktionen und Vorgaben zur Produktionssteuerung. Mit Prüfprogrammen von Maschinenherstellern kann in A+W Production geprüft werden, ob die Arbeitsgänge plausibel sind.

> **Funktionen sind von den freigeschalteten Modulen abhängig** Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind. Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Production die Arbeitsvorbereitung verantworten und damit den optimalen Ablauf der Produktion organisieren. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Production kennen.

### Dokumentation

Für das Modul Maschinenzuordnung stehen folgende Dokumente zur Verfügung:

* **PDF:** Vollständige Unterlagen (Tutorial, Softwarereferenz, Index)
* **Online-Hilfe :** Kontextsensitive Dialog-Hilfe

#### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

* **Überblick:** Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  * Lernziele: Was soll vermittelt werden?
  * Nutzen: Wofür können Sie dieses Wissen einsetzen?
  * Merksätze: Welche Zusammenhänge müssen Sie sich merken?
* **Konzepte:** Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
* **Übungen:** Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.

#### Darstellungskonventionen

* _Kursiv:_ sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog _Neue Maschine_.
* **Fett:** sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
* `>`: Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. `Stammdaten > MZO > MZO-Editor > Maschinen > Neu`.
* `[]`: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit `[OK]` speichern Sie die Daten.
* `<>`: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe.

#### Lesehinweis

Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen. Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Grundlagen

Die Maschinenzuordnung stellt die Bezüge zwischen Arbeitsgängen und Maschinen dar. Auf Basis der Maschinen und der Arbeitsgänge kann die Kapazitätsplanung die Aufträge optimal einlasten.

Zum Einrichten der Stamdaten müssen folgende Fragen behandelt werden:

* Welche Aufgabe muss durch die Bearbeitung an einer Scheibe eines Auftrags erfüllt werden: **Was** ist zu tun.
* Welche verwendende Methode wird verwendet: **Wie** wird das gemacht.
* Welches Arbeitsmittel wird verwendet: **Wo** wird die Bearbeitung ausgeführt.
* Welche Rangfolge und Restriktionen müssen beachtet werden: **Warum** oder **Wann** wird in die Maschine verwendet.

_Abb. G-1: Bestandteile in der Maschinenzuordnung._ In dieser schematischen Darstellung sehen Sie, welche Bestandteile zur Maschinenzuordnung gehören und wie sie miteinander verknüpft sind.

* **Beschreibung der Arbeitsgänge:** Mithilfe der Arbeitsgänge werden die Materialströme in der Produktion aufgeteilt und lassen sich separat behandeln. Bei der Einrichtung der Arbeitsgänge werden folgende Fragen berücksichtigt:
  * Welche Bearbeitung können zusammengefasst werden und welche dürfen nicht zusammengefasst werden?
  * Gibt es zusätzliche Bearbeitungen die ausgeführt werden, aber nicht in der Stückliste erscheinen?
  * Gibt es ggf. verschiedene Materialströme, z. B. Serienscheiben, Badspiegel, Wohnmobilscheiben, die ganz eigene Wege durch die Produktion gehen und daher früh unterschieden werden sollen?
  * Gibt es ggf. Arbeitsgänge, die gar nicht hier gefertigt werden, z. B. Sandstrahlen am anderen Ende der Stadt?
* **Beschreibung der Maschinen:** In dem die Maschinen präzise beschrieben werden, wird gewährleistet, dass zu fertigende Scheiben gültige Maschinen finden. Dabei wird zwischen physikalischen Restriktionen und logischen Maschinen mit zusätzlichen Restriktionen, Kostensätzen und Übergangszeiten unterschieden. Zur Liste der Maschinen kommen Orte, die zwar keine Maschinen im herkömmlichen Sinne sind, die aber für die Produktion relevant sind, z. B. Lager, Wareneingang, Versandlager, Verladerampe, zusätzliche Produktionsorte.
* **Beschreibung der logischen Maschine:** Logische Maschinen werden verwendet, um in der Kapazitätsplanung unterschiedliche Übergangszeiten, Kostensätze oder Bearbeitungsdauern auszudrücken. Als Leitfaden bietet sich an, eigene logische Maschinen einzurichten, wenn eine Maschine in verschiedenen Betriebsarten verwendet werden kann.

### Maschinenzuordnung

In diesem Kapitel erfahren Sie, welche Bereiche von A+W Production zur Maschinenzuordnung (MZO) gehören und wie Sie Maschinen zuordnen. Mithilfe des MZO-Editors verwalten Sie Maschinen, logische Maschinen und Arbeitsgänge, deren Zuordnung und Eigenschaften.

Zur Maschinenzuordnung gehören folgende Kapitel:

* "Maschinen"
* "Logische Maschinen"
* "Arbeitsgänge"
* "Arbeitsgangzuordnung"
* "Bedingungen, Formeln, Restriktionen"
* "Bearbeitungstypen und Bearbeitungsartikel"

In den folgenden Lerneinheiten lernen Sie zunächst Maschinen, logische Maschinen, Arbeitsgänge und die Arbeitsgangzuordnung kennen. Diese Kenntnisse werden anschließend durch die Themen Bearbeitungstypen und Formelauswahl vertieft.

#### Maschinen

**Lernziele**

* Was sind Maschinen in A+W Production und speziell in der Maschinenzuordnung.
* Wie werden Maschinen verwaltet, neu angelegt, bearbeitet oder gelöscht.
* Wie werden Namen und Nummern sinnvoll vergeben.

**Nutzen**

* Mit Maschinen wird der physikalische Maschinenpark abgebildet. Somit bilden Maschinen die Basis, um die Produktion zu steuern.

**Merke**

* **Maschinen:** Maschinen bilden die physikalischen Maschinen im Maschinenpark ab. Namen und Nummern werden in A+W Production systematisch vergeben.
* **Maschinentypen:** Die Maschinentypen sind in A+W Production bereits definiert und werden Maschinen zugewiesen. Mit Maschinentypen wird definiert, um welchen Typ einer Maschine es sich handelt, zum Beispiel Zuschnitt, Rahmenbieger oder Sonstige.
* **Verknüpfungen:** UND-/ODER-Verknüpfungen sind die Operatoren, mit denen in A+W Production Restriktionen, Bedingungen und Formeln verknüpft werden.
* **Schnitte:** Z- und W-Schnitte sind aufwendigere Schnitte, denen ein zusätzlicher Kostenfaktor Kosten pro Z-Schnitt zugewiesen werden kann.

> **Voraussetzung** Um eine Maschine in A+W Production anlegen zu können, muss der passende Maschinentyp definiert sein. Der Maschinentyp wird im Dialog _Neue Maschine_ ausgewählt. Ist im Dialog _Neue Maschine_ der entsprechende Maschinentyp nicht verfügbar, wenden Sie sich bitte an die A+W Software GmbH.

**Maschinen in der Maschinenzuordnung**

In dieser Einheit lernen Sie, wie Sie Ihren Maschinenpark in A+W Production abbilden und welche Eigenschaften den Maschinen zugeordnet werden.

_Abb. G-2: MZO-Editor - Maschinen_

Im Register _Maschinen_ sind alle physikalischen Maschinen gelistet. Das Register _Maschinen_ bildet somit Ihren realen Maschinenpark ab.

Jede Maschine ist durch eine ID eindeutig identifizierbar. Zu jeder Maschine gehört eine Erfassungsstelle für die Erfassung der Betriebsdaten (BDE). Sie ordnen jeder Maschine einen Maschinentyp zu, der festlegt, um welchen technischen Typ es sich handelt, zum Beispiel Zuschnitt, CNC-Center oder Sprossenbau. Die Maschinentypen sind fest definiert und können nicht geändert werden. A+W Production legt zu jeder Maschine automatisch eine logische Maschine an.

Sie müssen also zu jeder real existierenden Maschine im Maschinenpark eine Maschine in A+W Production anlegen und die Eigenschaften definieren.

_Abb. G-3: Maschinen in A+W Production_

In diesem Beispiel ist zur Bohrmaschine 2 keine Maschine in A+W Production angelegt. Damit ist die Maschine der Software nicht bekannt und kann auch nicht angesteuert werden.

**Maschineneigenschaften**

Für jede in A+W Production angelegte Maschine müssen die folgenden Eigenschaften der Maschine festgelegt werden.

* **Handbetrieb:** Kennzeichen für Maschinen, die nicht über automatische Ladeeinrichtungen verfügen. Dieses Kennzeichnen verhindert u.a. dass anhand der manuellen Bearbeitungsdauer gesplittet wird oder dass Positionen automatisch auf Handzuschnittstische eingelastet werden.
* **Einzelbearbeitung:** Kennzeichen für Maschinen, deren Bearbeitungen nicht zusammengefasst werden dürfen, z. B.
  * Bohrungen = 0: für zwei Bohrungen auf derselben Maschine werden nicht zwei Termine ermittelt.
  * Siebdrucke oder Beschichtungen = 1: für zwei Beschichtungen werden nicht zwei verschiedene Termine ermittelt, auch wenn sie auf derselben Maschinen gemacht werden.
* **Mindestgröße:** Mindestabmessungen für eine Scheibe, die auf der Maschine gefertigt werden kann, ohne z. B. durch die Rollen zu fallen. Wenn Sie zu kleine Scheiben auf eine größere Scheibe legen können, z. B. um sie zu bedrucken, legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den logischen Maschinen, z. B. als Siebdruck mit Trägerscheibe.
* **Maximalgröße:** Maximale Abmessungen für eine Scheibe, die der Maschine gefertigt werden kann, weil sie die Breite der Führungsschienen, die Ofenbreite oder die Deckenhöhe überschreitet. Wenn Sie größere Scheiben fertigen können, indem Sie z. B. am Bearbeitungszentrum die Seitenwände abschrauben und Spritzschutz aufstellen, legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den logischen Maschinen, z.B: als Bearbeitungszentrum für Übergrößen.
* **Dicken:** Dickenbereich, in dem die Maschine arbeiten kann. Anderen Dicken können nicht auf der Maschine bearbeitet werden, z. B. weil 3 mm nicht zuverlässig unterstützt werden und für 15 mm die Führungen zu schmal sind. Wenn eine 15 mm Scheibe gefertigt werden kann, indem Sie die Maschine umbauen, legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den logischen Maschinen, z. B. Schleifmaschine für Dickgläser.
* **Modelle:** Angabe, ob die Maschine ausschließlich Rechtecke, ausschließlich Modelle oder beides fertigen kann. Berücksichtigen Sie ggf. dass Freiformen oder Rundbögen nicht gefertigt werden können, z. B. bei VSG-Zuschnitt.
* **Gewicht:** Maximalgewicht einer Scheibe, für das die Maschine zugelassen ist. Um auszudrücken, dass die Maschine das Gewicht zwar verarbeiten kann, hierfür aber ein zweiter Mitarbeiter zum Handling bereitstehen muss, geben Sie die Restriktion bei den logischen Maschinen an, z. B. Einseiter mit zwei Personen.

> **Maschine löschen** Das Löschen einer Maschine kann Auswirkungen auf die Produktion haben. Vergewissern Sie sich, dass die Maschine in der Produktion nicht mehr verwendet wird, bevor Sie sie löschen.

**Namen, IDs und Nummern vergeben**

Vergeben Sie für Maschinen des gleichen Typs IDs im gleichen Hunderter-Bereich, zum Beispiel für alle Schneidtische IDs zwischen 100 und 199. Damit sind in der Liste Schneidtische sofort erkennbar. Wenn Sie keine eigenen Nummernkreise für Betriebsmittel haben, orientieren Sie sich am Nummerierungsschema der Betriebsdatenerfassung.

Vergeben Sie für Maschinen des gleichen Typs gleiche Namen und nummerieren Sie diese durch, z. B. bekommt der achte Schneidtisch im Maschinenpark den Namen Schneidtisch 8.

**Maschinenrestriktionen**

Maschinen können bauartbedingt verschiedene Restriktionen haben, z. B. können sie nur Scheiben bis zu einer bestimmten Größe bearbeiten. Die Restriktionen der einzelnen Maschinen können Sie im Dialog `Maschine` angeben.

Die verfügbaren Restriktionen im Dialog `Maschine` sind:

* Minimale Dicke
* Maximale Dicke
* Modelle
* Beschichtete Gläser
* Strukturgläser
* Stufen ISO
* Abmessungen
* SZR

Haben Sie eine Maschine, die weitere Restriktionen aufweist, müssen die Restriktionen mit zusätzlichen Bedingungen formuliert werden. Diese Bedingungen können auch Formeln enthalten. ⇨ "Bedingungen und Formeln in der Maschinenzuordnung"

**Beispiel: Restriktionen Dicke** Sie können die Restriktion Dicke folgendermaßen einstellen:

* Wenn die Maschine nur Scheiben ab einer Dicke von 8 mm bearbeiten kann, geben Sie die Restriktion `minimale Dicke` 8 mm ein.
* Wenn die Maschine nur Scheiben bis zu einer Dicke von 15 mm bearbeiten kann, geben Sie die Restriktion `maximale Dicke` 15 mm ein.

**Beispiel: Restriktion Modelle**

* `Keine Restriktion`: die Maschine kann Modelle und Rechtecke bearbeiten, z. B. bei einem modernen Zuschnitttisch.
* `Die Maschine kann nur Modelle bearbeiten`: z. B. um zu verhindern, dass rechteckige Scheiben zum Schleifen auf ein CNC-Center gelangen.
* `Die Maschine kann keine Modelle, also nur Rechtecke, bearbeiten`: z. B. bei einer Schleif-Bohrstraße.

**Beispiel: Restriktion Beschichtete Gläser**

* `Keine Restriktion`: die Maschine kann beschichtete und unbeschichtete Gläser bearbeiten.
* `Die Maschine kann nur beschichtete Gläser bearbeiten`.
* `Die Maschine kann nur unbeschichtete Gläser bearbeiten`.

**Beispiel: Restriktion Strukturgläser**

* `Keine Restriktion`: die Maschine kann Strukturgläser und Gläser ohne Struktur bearbeiten.
* `Die Maschine kann nur Strukturgläser bearbeiten`.
* `Die Maschine kann nur Gläser ohne Struktur bearbeiten`.

**Beispiel: Restriktion Stufen-ISO**

* `Keine Restriktion`: die Maschine kann Stufen-ISO und Normal-ISO fertigen.
* `Die Maschine kann nur Stufen-ISO bearbeiten`.
* `Die Maschine kann nur Normal-ISO bearbeiten`.

**Abmessungsrestriktionen und Scheibenformat** Sie können bei einer Maschine minimale und maximale Größen der zu bearbeitenden Scheiben definieren. Orientieren Sie sich bei der Angabe der Werte an der Laufrichtung der Maschine. Die Werte Breite und Höhe dienen lediglich der Anschauung, Sie können auch Scheiben verarbeiten, deren Breite und Höhe vertauscht sind. Die Scheibe muss dann u. U. per Hand an der Maschine gedreht werden.

**SZR-Restriktionen** Hier legen Sie fest, ob die Maschine einfaches ISO mit einem SZR oder mehrfaches ISO mit zwei SZRs fertigen kann. Für jeden SZR kann ein Mindest- und ein Maximalwert eingegeben werden.

**UND-/ODER-Verknüpfungen** Wenn Sie die Restriktionen einer Maschine angeben, dann müssen Sie diese als logische Verknüpfungen (UND/ODER, AND/OR) angeben. Diese sind Grundverknüpfungen der booleschen Algebra, mit der sich logische Zusammenhänge zeigen lassen.

* **UND-Verknüpfung:** Wenn zwei (oder mehr) Aussagen zutreffen, ist eine Aussage wahr. Beispiel: Auf einer Maschine können nur Scheiben bearbeitet werden, die breiter als 150 mm und höher als 200 mm sind. Daraus ergibt sich: Breite >= 150 mm UND Höhe >= 200 mm.
* **ODER-Verknüpfung:** Wenn die eine oder die andere Aussage zutrifft, ist eine Aussage wahr. Beispiel: Auf einer Maschine können nur Scheiben bearbeitet werden, die breiter als 150 mm oder kürzer als 3500 mm sind. Daraus ergibt sich: Breite >= 150 mm ODER Länge <= 3500 mm.

**Komponenten-ID** Die Komponenten-ID wird nur bei den Maschinentypen Linie, Zuschnitt und Bieger verwendet. Mit der Komponenten-ID kann zwischen Linien, Tischen oder Biegern unterschieden werden, wenn es mehrere des gleichen Typs gibt. So könnten zum Beispiel die Tische 1, 2 und 3 die Komponenten-IDs TB1, TB2 und TB3 bekommen. Die Komponenten-ID steuert, in welchem Format die NC-Codeausgabe erfolgt.

**Zusätzliche Bedingungen** Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaften von Maschinen unter Umständen massiv. Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche Auswirkungen diese hat.

**Maschinen anlegen und verwalten**

In dieser Lerneinheit lernen Sie, wie Sie neue Maschinen anlegen, bearbeiten oder löschen. Wenn Sie eine Maschine anlegen, müssen Sie anschließend die Maschinendaten bearbeiten.

> **Voraussetzung** Um eine neue Maschine anzulegen, muss ein passender Maschinentyp angelegt sein, z. B. Zuschnitt, CNC-Center, Rahmenbieger, Sonstiges. Der Katalog der Maschinentypen ist in A+W Production fest vorgegeben. Er steht in der Kombobox zur Verfügung, wenn Sie eine neue Maschine anlegen.

**So legen Sie eine Maschine an**

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen > [Neu]`.
2. Geben Sie eine ID aus dem Nummernbereich ein, den Sie für diesen Maschinentyp vorgesehen haben, zum Beispiel `180`.
3. Geben Sie einen Namen ein, der die Maschine eindeutig beschreibt, zum Beispiel `Schneidtisch 8`.
4. Wählen Sie den zugehörigen Maschinentyp, zum Beispiel `Zuschnitt`.
5. Geben Sie eine Komponenten-ID ein, zum Beispiel `TB8`. Sie müssen bei den Maschinentypen Linien, Tische oder Bieger eine Komponenten-ID eingeben. Damit können Sie zwischen den Maschinen unterscheiden, wenn es mehrere davon gibt. _Abb. G-4: Beispiel für eine neue Maschine_
6. Klicken Sie auf `[OK]`, um die Daten zu speichern. Damit haben Sie eine neue Maschine angelegt. Sie wird in der Liste der Maschinen im Dialog MZO-Editor aufgeführt.

Um die Maschine vollständig zu beschreiben, müssen Sie die Eigenschaften und Zuordnungen festlegen.

**So geben Sie die Eigenschaften einer Maschine ein**

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen`. _Abb. G-5: MZO-Editor - Maschinen_
2. Markieren Sie die Maschine, die Sie bearbeiten wollen.
3. Klicken Sie auf `[Bearbeiten]`. _Abb. G-6: Maschine_ A. Allgemeine Eigenschaften B. Kombobox
4. Ergänzen Sie die `Allgemeinen Eigenschaften` (A). Wenn Sie in ein Feld klicken, können Sie die Daten aus der Kombobox (B) wählen. Die Restriktionen unteren Teil des Dialogs können Sie später bestimmen.
5. Bestätigen Sie mit `[OK]`. Damit haben Sie die Stammdaten der Maschine angegeben. Die Maschinen-Restriktionen lernen Sie in einer separaten Einheit kennen. ⇨ "Restriktionen von Maschinen anlegen und bearbeiten"

**So löschen Sie eine Maschine**

> **Maschinen löschen** Das Löschen von Maschinen in A+W Production kann Auswirkungen auf die Produktion haben. Vergewissern Sie sich, dass die Maschinen nicht verwendet werden, bevor Sie sie löschen.

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen`.
2. Markieren Sie die Maschine, die Sie löschen möchten.
3. Klicken Sie auf `[Löschen]`. Eine Sicherheitsabfrage wird angezeigt.
4. Bestätigen Sie die Sicherheitsabfrage mit `[Yes]`, wenn Sie die Maschine endgültig löschen möchten. Die Maschinendaten werden gelöscht.

**Restriktionen von Maschinen anlegen und bearbeiten**

In dieser Lerneinheit lernen Sie, die Restriktionen einer Maschine festlegen.

> **Restriktionen und Zusätzliche Bedingung gleichzeitig** Wenn Restriktionen aktiviert sind und gleichzeitig eine Formel ausgewählt ist, kann dies zu einem Konflikt führen. Restriktionen können sich gegenseitig aufheben. Für Rückfragen wenden Sie sich bitte an den Support der A+W Software GmbH.

**So bearbeiten Sie die Restriktionen zur Dicke**

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen`. _Abb. G-7: MZO-Editor - Maschinen_
2. Markieren Sie die Maschine, die Sie bearbeiten wollen.
3. Klicken Sie auf `[Bearbeiten]`. _Abb. G-8: Restriktion - Dicke bearbeiten_ A. Aktivieren der Restriktion B. Eingabefeld öffnen.
4. Klicken Sie doppelt auf `[...]` (B).
5. Klicken Sie auf den `[Pfeil]`, um den Wert für die minimale Dicke einzugeben.
6. Geben Sie den Wert der minimalen Dicke in Millimetern ein.
7. Klicken Sie auf `[OK]`, um den Wert zu speichern. Damit haben Sie den Wert der minimalen Dicke der Maschine geändert.
8. Wiederholen Sie die Schritte 4 bis 7, um die Restriktionen für die maximale Dicke zu bearbeiten.

**So bearbeiten Sie die Restriktionen für Modelle, beschichtete Gläser, Strukturgläser und Stufen-ISO**

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen`.
2. Markieren Sie die Maschine, die Sie bearbeiten wollen.
3. Klicken Sie auf `[Bearbeiten]`. _Abb. G-9: Restriktion - Modelle bearbeiten_ A. Aktivieren der Restriktion Modelle B. Weitere Checkbox öffnen.
4. Klicken Sie doppelt auf `[...]` hinter `Modelle`. Ein `[Pfeil]` wird angezeigt.
5. Klicken Sie auf den `[Pfeil]` (B), um Modelle zu aktivieren. _Abb. G-10: Restriktion Modelle - Kombinationen der Checkboxen_
   * A und B: Keine Restriktion. Die Maschine kann Rechtecke und Modelle bearbeiten.
   * C und D: Die Maschine kann nur Rechtecke bearbeiten.
   * E und F: Die Maschine kann nur Modelle bearbeiten.
6. Wählen Sie die gewünschte Kombination der Checkboxen, um die Restriktion festzulegen:
   * Keine Einschränkung (A, B)
   * Keine Modelle (C, D)
   * Keine Rechtecke (E, F)
7. Klicken Sie auf `[OK]`, um die Restriktion für Modelle zu speichern. Damit haben Sie die Restriktion Modelle für die Maschine bearbeitet.
8. Bearbeiten Sie auf die gleiche Weise die Restriktionen für beschichtete Gläser, Strukturgläser und Stufen-ISO.

**So bearbeiten Sie Restriktionen für Abmessungen und SZR**

> **Restriktionen werden unwiderruflich gelöscht** Abmessungsrestriktionen werden unwiderruflich und ohne Sicherheitsabfrage gelöscht, wenn Sie auf das `[Kreuz]` klicken.

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen`.
2. Markieren Sie die Maschine, die Sie bearbeiten wollen.
3. Klicken Sie auf `[Bearbeiten]`. _Abb. G-11: Restriktion - Abmessungen bearbeiten_
4. Klicken Sie im Feld `Abmessungen` auf das `[Stift-Symbol]`, um den Dialog `Abmessungsrestriktionen` zu öffnen.
5. Aktivieren Sie die Checkboxen der Eingabefelder, die Sie bearbeiten möchten.
6. Geben Sie die Werte in die Eingabefelder ein.
7. Klicken Sie auf `[OK]`, um die Änderungen der Abmessungsrestriktionen zu speichern. Die Restriktion wird im Feld `Abmessungen` als UND-/ODER-Verknüpfungen angezeigt.
8. Bearbeiten Sie auf die gleiche Weise die Restriktionen für den SZR.

**So entfernen Sie die Restriktionen Abmessungen und SZR**

> **Abmessungsrestriktionen löschen** Abmessungsrestriktionen werden unwiderruflich und ohne Sicherheitsabfrage gelöscht, wenn Sie auf das `[Kreuz]` klicken.

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Maschinen`.
2. Markieren Sie die Maschine, die Sie bearbeiten wollen.
3. Klicken Sie auf `[Bearbeiten]`. Der Dialog `Maschine` wird geöffnet.
4. Klicken Sie im Bereich `Abmessungen`, auf `[X]`, um Restriktion zu entfernen. Damit haben Sie die Restriktionen `Abmessungen` für die Maschine gelöscht.
5. Klicken Sie auf `[OK]`, um die Änderungen zu speichern.
6. Entfernen Sie auf die gleiche Weise die SZR-Restriktionen.

**Übungen zu Maschinen**

Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.

* Bilden Sie auf Papier den Maschinenpark Ihres Betriebes ab.
* Notieren Sie, welche Maschine in welchen Maschinentyp fällt.
* Vergeben Sie für die Maschinen systematisch IDs (Nummernkreise).
* Notieren Sie, welche Eigenschaften für die Maschinen gelten und ob es Restriktionen gibt:
  * Gibt es Restriktionen, wie zum Beispiel minimale Dicke, maximale Dicke oder Abmessungsrestriktionen.
  * Kann die Maschine ISO oder 3-fach-ISO bearbeiten? Wo müssen Sie diese Eingaben vornehmen?
* Legen Sie Maschinen als Übungsmaschinen in A+W Production an und passen Sie diese so an, dass sie Ihrem Maschinenpark entsprechen.
* Lassen Sie die testweise erstellten Maschinen bestehen, da spätere Übungen darauf aufbauen.

**Ergänzende Informationen**

* ⇨ Softwarereferenz, "Neue Maschine"
* ⇨ Softwarereferenz, "Maschine"
* ⇨ Softwarereferenz, "Abmessungsrestriktionen"
* ⇨ Softwarereferenz, "SZR Restriktionen"

#### Logische Maschinen

**Lernziele**

* Was sind logische Maschinen in A+W Production und speziell in der Maschinenzuordnung?
* Warum gibt es logische Maschinen?
* Wie werden Namen und Nummern vergeben?
* Wie werden logische Maschinen neu angelegt, bearbeitet oder gelöscht?
* Wann können logische Maschinen gelöscht werden und wann nicht?

**Nutzen**

* Logische Maschinen bilden eine Funktion einer Maschine ab. Kann eine Maschine Bohren und Kanten bearbeiten, werden dafür in A+W Production zwei logische Maschinen angelegt. Und damit kann im nächsten Schritt ein Arbeitsgang der Funktion einer Maschine zugeordnet werden.
* Die A+W Production BDE (Betriebsdatenerfassung) wertet unter anderem Daten der logischen Maschinen aus, z. B. für Statistiken.

**Merke**

* **Logische Maschinen:** Logische Maschinen bilden jeweils eine Funktion einer physikalischen Maschine ab. Sie werden zur Ablaufsteuerung in der Produktion und zur Kostenberechnung verwendet. Logische Maschinen werden zur Betriebsdatenerfassung verwendet. Sobald Sie eine Maschine anlegen, wird automatisch eine logische Maschine angelegt. Zu einer Maschine können beliebig viele logische Maschinen definiert werden.
* **Zuordnung:** Logische Maschinen werden Arbeitsgängen zugewiesen.

**Logische Maschinen in der Maschinenzuordnung**

Logische Maschinen bilden jeweils eine Funktion einer realen Maschine ab. Dabei werden die Eigenschaften der Maschine an die logische Maschine vererbt. Zusätzlich zu den Eigenschaften der Maschine gelten die Eigenschaften der logischen Maschine.

_Abb. G-12: Logische Maschinen_

Logische Maschinen werden benötigt für:

* Beschreibung einzelner Maschinenfunktionen.
* Zuordnung von Arbeitsgängen.
* Priorisierung von Arbeitsgängen.
* Auslastungsplanung und Umlastung.
* Logische Maschinen trennen einzelne Funktionen von Maschinen. Damit werden für eine Maschine z. B. unterschiedliche Kostensätze oder Übergangszeiten möglich.
* Statistische Auswertungen.

**Beispiel** Sie haben eine CNC-Maschine, die bohren, schleifen und polieren kann. Sie definieren die Maschine als CNC-Maschine 1. Dazu erstellt A+W Production automatisch eine logische Maschine. Da die CNC-Maschine drei Funktionen besitzt, werden drei logische Maschinen definiert. Diese definieren Sie so, dass die Stammdaten zu Bohren angelegt sind. Nun definieren Sie zur CNC-Maschine 1 zwei weitere logische Maschinen: eine mit den Stammdaten zum Schleifen und die andere mit den Stammdaten zum Polieren.

_Abb. G-13: Beispiel: Drei logische Maschinen resultieren aus einem CNC-Center_

Die Bearbeitungszeiten, die eine logische Maschine für den ihr zugewiesenen Arbeitsgang benötigt, wird als Formel in der Kapazitätsplanung definiert. Dazu steht die separate Dokumentation für den Part Kapazitätsplanung zur Verfügung.

**Logische Maschinen anlegen und verwalten**

In diesem Teil des Tutorials lernen Sie, wie Sie logische Maschinen anlegen und bestehende bearbeiten oder löschen.

> **Voraussetzung** Sie können logische Maschinen erst dann anlegen, wenn die zugehörige Maschine angelegt ist.

**So legen Sie eine logische Maschine an**

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Logische Maschinen`. _Abb. G-14: Logische Maschine markiert_ A+W Production erstellt automatisch zu jeder Maschine eine logische Maschine. Alle weiteren logischen Maschinen können nur auf Basis der bereits bestehenden erstellt werden.
2. Markieren Sie die logische Maschine, welche die Basis für die neue logische Maschine sein soll.
3. Klicken Sie auf `[Neu]`.
4. Geben Sie die ID und den Namen ein.
5. Klicken Sie auf `[OK]`, um die Daten zu speichern. _Abb. G-15: Neue logische Maschine_ Damit haben Sie eine neue logische Maschine angelegt. Die neue logische Maschine wird im Register `Logische Maschinen` im MZO-Editor gelistet. Sie können jetzt die Eigenschaften der neuen logischen Maschine bearbeiten.

**So bearbeiten Sie eine logische Maschine**

1. Wählen Sie `Stammdaten > MZO > MZO-Editor > Logische Maschinen`. Das Register `Logische Maschinen` wird angezeigt.
2. Markieren Sie die logische Maschine, die Sie bearbeiten wollen.
3. Klicken Sie auf `[Bearbeiten]`. _Abb. G-16: Logische Maschine - Eigenschaften_
4. Geben Sie die Daten für die logische Maschine ein, z. B. für einen Schneidtisch.
5. Klicken Sie auf `[OK]`, um die Daten zu speichern. Damit haben Sie die Stammdaten der logischen Maschine angelegt.
