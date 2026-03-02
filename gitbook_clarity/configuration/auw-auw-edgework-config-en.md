---
description: "AUW_Configuration_EdgeWork"
---

## Kantenbearbeitungen

## History


| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 2016.01 | DLA | Issue | 1.0 |
|  |  |  |  |


## Content


## Sonderkantekonfigurieren

Es soll eine Kantenbearbeitung für eine Sonderkante angelegt werden, z.B. eine C-Kante. Dazu muss eine neue Kantenbearbeitung in den Stammdaten der Auftragserfassung angelegt werden und eineSN-Kantenqualität Sonderkante (11-28) zugeordnet werden.

_Example AWB:__[Master Data__ Products__ Product__ Products__ Production__]_
_Die Beschreibung der Liste der Sonderkanten kann man im AWB nicht ändern. Es handelt sich dabei um Text Nummer 3866 aus der AWB Meldungsdatei (\*mes.txt), diese wird bei einem Update überschrieben._

Der richtigeBearbeitungstyp und eine entsprechende Schleifgruppe muss ausgewählt werden. Entweder in AWP über den Artikelstammdatenabgleich…
_Example__ AWB: [Master Data__ Products__Product__ Products__Alcim__]_

… oder direkt in den AWP Bearbeitungsstammdaten, bei einem anderen Auftragserfassungssystem oder ohne Stammdatenabgleich.

_Example AWP: Processing article master data_

Ab Version 5.5.3000 kanndie Einlastung in AWP eineSN-Datei automatisch über dieOrderXML erzeugen, wenn dieSN-Kantenqualität (DECO) für diese Sonderkantein derOrderXML-Datei mitgegeben wird, wasaktuell nur AWB kann.
Damit AWP dieses übergebene DECO verwendet muss der neue Schalter_[ALCIM\_SHAPE /__SNUSEORDERDECOFORAWTYPE1090]_ gesetzt werden. In diesem Fall wird die SN-Kantenqualität (Feld Extra 1) aus den AWP Bearbeitungsstammdaten nicht verwendet.

Wird keineSN-Kantenqualität für die Sonderkante übergeben, muss die Kantenqualität in den AWP Bearbeitungsstammdaten im Feld [Extra 1] gesetzt werden. In diesem Fall kann über dieOrderXML-Datei keineSN-Zeichnung erzeugt werden. Wird eineSN-Datei benötigt, kann diese über AWB oder manuell erzeugt werden.
### SN Symbol für Sonderkante definieren

Auf denSN-Zeichnungen und den zugehörigen Ausdrucken soll für die neue Sonderkante ein entsprechendes Symbol angezeigt werden.
Dies wird über die Sektion_[__Decoration__]_ in der Konfigurationsdatei_SN.INI_ gesteuert. Dort gibt es für jede Kantenqualität (DECO) einen Parametersatz. Die DECO-Nummern sind in SN um eins kleiner, DECO 12 in AWB ist in SN DECO 11.
[Decoration]
Deco11 = CC
Deco11Name = C-Edge
Deco11Shift = "1.0 mm"
Deco11EnableForDrawingViews = 1


## Unterschiedlicher Zuschlag oderunterschiedliche Maschinen

_Siehe hierzu auch Kapitel 4.9 der A+W Business Konfigurationsanleitung: \\\\jupiter\\Doku\_DocuWare\\ALFAK2000\\!General\\Installation\_Configuration\\__DE-CONFIG-A+W Business.pdf_
Wenn eine Scheibe komplett poliert werden soll, ist es am einfachsten, wenn alle Kanten dieser Scheibe auf der gleichen Maschine mit dem gleichen Kantenzuschlag gefertigt werden. Der Preis für die Kantenbearbeitung für jede Kante richtet sich nach den zu bearbeitenden Laufmetern. In einem solchen Fall wird eine Bearbeitung in der Stückliste benötigt, die auf allen Kanten ausgeführt wird und für die Preisberechnung wird ein Wert für jeden Laufmeter benötigt.
Leider ist dies nicht immer so einfach. Kanten sollen auf unterschiedlichen Maschinen gefertigt werden (z.B. die Modellkanten müssen auf einer CNC bearbeitet werden, was teuer ist, die geraden Kanten auf einer günstigeren Schleifmaschine). Unterschiedliche Maschine können unterschiedliche Schleifzuschläge bedeuten.Dazu kommt die Preisberechnung, Modellkanten sind teurer als gerade Kanten.
Um dies zu lösen, musste bisher in der Stückliste ein Kantenbearbeitungsartikelpro Maschine enthalten sein. Hatten beide Kantenbearbeitungen unterschiedliche Schleifzuschläge, musste es sich dabei auch um unterschiedliche Artikelnummern handeln (wegen unterschiedlicherSN-Kantenqualitäten, DECO). Beispiel: Artikel 6000 Gerade Kante poliert; Artikel 6001 Modellkante poliert. Die Preisberechnung hing an den unterschiedlichen Artikeln.
Das Problem dieser Lösung warnotwendiges technisches Wissen bei den Sachbearbeitern der Auftragserfassung. Sachbearbeiter können geschult werden, aber mit dem Einsatz voniQuotein einem Betrieb musste eine andere Lösung her. Der Endkunde, der bei einemBetrieb ein Glas überiQuote bestellt, bestellt ein Glas,das poliert ist und möchte einen Preis sehen. Ob das Glas auf unterschiedlichen Maschinen gefertigt wird, ob es unterschiedliche Kantenzuschläge bei der Fertigung gibt und ob es Zuschläge beim Preis für spezielle Kanten gibt, dasweiß derEndkunden nicht.
Um dies zu lösen, wurden A+W Business, A+W CAD Designer (Shapes) und A+WProductionmit der Version 5.5 (Build2000,AWDesk \#344692) erweitert. Füreinen Kantenbearbeitungstyp (z.B. polieren) ist nur noch ein Bearbeitungsartikel notwendig. Wird die Bearbeitung auf unterschiedlichen Maschinen gefertigt, dann wird weiterhin eine Bearbeitung pro Maschine benötigt, es kannjetztaber immerdieselbe sein, auch bei unterschiedlichen Kantenzuschlägen. Damit die richtigen Kantenzuschläge gefunden werden, haben die Bearbeitungen unterschiedliche Standard-Bearbeitungstypen: 1010 für das normale Polieren und 1090 (Sonderkante) für die abweichenden Bearbeitungen. An den A+W Bearbeitungstyp 1090 kann nun über dieOrderXML-Schnittstelle eine entsprechende SN-Kantenqualität (DECO) mitgegeben werden und so ist es nun auch möglich, bei der Einlastung in A+W Produktion eine SN-Zeichnung zu erzeugen, wenn der A+W Bearbeitungstyp 1090 in der Stückliste hängt. Bei der Berechnung der Kantenzuschläge wird die übergebene SN-Kantenqualität berücksichtigt.
### AWB -SN-Kantenqualität definieren

Für einen Kantenbearbeitungsartikel kann eineSN-Kantenqualität definiert werden.
_[Stammdaten__ Produkte__ Artikel__Artikel__ Lasche Fertigung]_
Werden dieStandard-Kantenqualitäten(z.B.8,10,11) verwendet, wird der entsprechende A+W Bearbeitungstyp dem Artikel zugeordnet. Für alle individuellen Kantenqualitäten wird der A+W Bearbeitungstyp 1090 (Sonstige Kantenbearbeitung) verwendet und die SN-Kantenqualität in dieOrderXML-Datei geschrieben.
Will man für eine Bearbeitung bei bestimmten Kanten eines Modellseinen andere SN-Kantenqualität verwenden,kann dies über den Artikel Stammdatendialog konfiguriert werden.
_[Stammdaten__ Produkte__ Artikel__ Modellkantenqualitäten]_
Für jede Bearbeitung musshierein Datensatz für jedes abweichendes Modell erfasst werden. Für jede Kante eines Modells kann eine Kantenqualität erfasst werden. Wird keine erfasst (0), wird der Standardwert aus dem Artikelstamm verwendet.
In derOrderXML-Datei wird eine Bearbeitung in mehrere Bearbeitungen gesplittet, so viele wie unterschiedliche Kantenqualitäten vorhanden sind. Ist die A+W Business Zeitwirtschaft im Einsatz, musszusätzlich dieSonderzuordnung 2 beachtet werden.
Die von A+W Business erzeugten SN-Zeichnungen und auch die SN-Ansicht bei der Auftragserfassung berücksichtigen die hier definierten Modellkantenqualitäten.
Beispiel
Es wird eine Bearbeitung 6400 Polieren auf einem Modell 1 erfasst. Die Bearbeitung poliert alle 4 Kanten. DieSN-Kantenqualität ist im Standard 11, auf der dritten Kante 12. In derOrderXML werden 2 Bearbeitungen 6400 übergeben. Eine auf den Kanten 1,2,4 und dem A+W Bearbeitungstyp 1010, und eine auf der Kante 3 mit dem A+W Bearbeitungstyp 1090 und derSN-Kantenqualität 12.
### AWB Zeitwirtschaft - Sonderzuordnung 2

Ist die A+W Business Zeitwirtschaft im Einsatz, erfolgtüber die Sonderzuordnung 2das Splitten einer Kantenbearbeitung in unterschiedliche Bearbeitungen. Die Kanten einer Bearbeitung können unterschiedlichen Arbeitsgängen zugeordnet werden.
_[Kapazitätsplanung__ Zuordnung__ Sonderzuordnung 2]_
Wird dies verwendet, dann mussdie Aufteilung der Arbeitsgänge mit den Kantenqualitäten übereinstimmen. Hat einer der Arbeitsgänge Kanten mit unterschiedlichen Kantenqualitäten, kommt es bei Erzeugung derOrderXML-Datei zu einer Meldung und es wird keineOrderXML-Datei erzeugt. Die abweichenden Modellkantenqualitäten und die Sonderzuordnung 2 müssen bei Verwendung der A+W Business Zeitwirtschaft übereinstimmen.

### AWB Preisberechnung - Modellzuschlag

Modellzuschläge für Kantenbearbeitungen können für jedes Segment definiert werden.
_[Stammdaten / Preise / Modellzuschläge]_
Der Preis-Typ „Brut-%“ bedeutet, der Zuschlag ist ein % Wert. Für jedes Segment wird der am Segment hinterlegte Zuschlag dazu gerechnet.
Der Mindestpreis bezieht sich auf den ausgerechneten Gesamtpreis.
DieMindestmenge bei Kantenbearbeitung bedeutet Mindestmenge in Laufmetern bzw. der entsprechenden Einheit der Bearbeitung. Sie bezieht sich entweder auf jede einzelne Kante oder auf alle Kanten mit dem gleichen Zuschlag, abhängig vom Parameter „Kantenmindestlänge pro Kante berechnen“[Stammdaten Firma Firmendaten Preisberechnung].
Bei der Auftragserfassung gibt es an der Kantenbearbeitung die Option „Exakte Berechnung“, diese ermittelt die Preise nach den genauen Segmentlängen. Ohne diese Option wird nach den Längen des umschriebenen Rechtecks gerechnet.
Sobald unterschiedliche Modellzuschläge vorhanden sind, wirdan der BearbeitungderStückpreis angezeigt, nicht mehr der Preis pro laufenden Meter.

### Beispiel

- Modell 1: W=500; H=500; H1=250; Schräge Kante = 559
- Mindestlänge ist 1lfm
- Kante 3 hat einZuschlag von 50 %
- Kosten prolfm betragen 9,20€

Kantenmindestlänge wird nicht pro Kante berechnet:Ohne Exakte BerechnungKanten 1 (500) + 2 (500) + 4 (500) = 1,5lfm \* 9,20€ = 13,80€
Kante 3 (500) < 1lfm = 1lfm \* 1,5 (50% Aufschlag) \* 9,20€ = 13,80€**Preis = 27,6****0****€**Kantenmindestlänge wird nicht pro Kante berechnet:ExakteBerechnung
Kanten 1 (500) + 2 (250) + 4 (500) = 1,25lfm \* 9,20€ = 11,50€
Kante 3 (559) < 1lfm = 1lfm \* 1,5 (50% Aufschlag) \* 9,20€ = 13,80€**Preis =****25****,****30€**
Kantenmindestlänge wird pro Kante berechnet: Mit oder ohne exakteBerechnung
Alle 4 Kanten < 1lfm, für jede Kante wird 1lfm verwendet und für Kante 3 noch ein Aufschlag von 50%**4,5 \* 9,20€ = 41,40€**
### AWP -Kantenzuschlagberechnen

DieSN-Kantenqualität wurde bis jetzt immer aus den A+WProduction Stammdaten der Bearbeitung gelesen undes wurdeüberprüft, ob diese Kantenqualität auf derSN-Zeichnung vorhanden ist. Sollten mehrere Kantenbearbeitungen mit derselbenSN-Kantenqualität in der Stückliste vorhanden sein, funktioniert alles, wenn derMasszuschlag (unabhängig von der zugeordneten Maschine) für alle Kantenbearbeitung gleich ist.
Jetzt haben wir aber das Problem, dass der gleiche Bearbeitungsartikel unterschiedliche SN- Kantenzuschläge in derSN-Datei hat und evtl. auch noch unterschiedliche Schleifzuschläge errechnet werden. Wird eine solche Position importiert, bleibt diese mit einem Fehler bei der Einlastung hängen.

Damit diese Position ordentlich verarbeitet werden können, muss der neue Schalter**[ALCIM\_SHAPE / SNUSEORDERDECOFORAWTYPE1090]**gesetzt werden.
## Liste derSN-Kantenqualitäten

_Nummer__ in A+W Business und A+W Production__immer__ +1_


| SN Deco | Symbol | Beschreibung | AW BearbTyp | SN Deco VSG | Symbol VSG |
| --- | --- | --- | --- | --- | --- |
| 8 | / | Säumen | 1000 | 77 | & |
| 10 | x | Feinschliff / Nachschleifen | 1005 | 75 | % |
| 11 | xx | Polieren | 1010 | 78 | %% |
| 65 | ! | Gehrung | 1015 | 76 | !! |
| 66 | FA | Facette | 1020 |  |  |
| 12-17 |  | Sonderkante | 1090 | 85-89 |  |
| 19-28 |  | Sonderkante | 1090 | 91-100 |  |
| 101-132 |  | Sonderkante | 1090 | 133-164 |  |


Wird im A+W Business eine Kantenbearbeitung an ein VSG Teil angebracht, ist auf derSN-Zeichnungdas VSG DECO angebracht und nicht das im A+W Business definierte. Dies, wenn dieSN-Zeichnung direkt von A+W Business oder bei der Einlastung in A+WProduction erzeugt wird. Bei der Bestimmung der Schleifzuschläge in A+WProduction werden die Zuschläge mit beiden DECOs geprüft.
So ist es möglich, mit einem einzigen Artikel die Kantenbearbeitungen für FLOAT und VSG zu beschreiben.
## [ALCIM\_SHAPE / SNUSEORDERDECOFORAWTYPE1090]

AWP Schalter_ [ALCIM\_SHAPE / SNUSEORDERDECOFORAWTYPE1090]:_**0**: Die SN-Kantenqualität wird aus den Artikelstammdaten (Bearbeit\_extra1) verwendet.**1**: Die SN-Kantenqualität wird aus dem Auftrag übernommen, falls das Feld <decoration\> in der Übergabedatei gefüllt war und die Kantenbearbeitung den A+W Bearbeitungstyp 1090 (Sonstige Kantenbearbeitung) hat.

Voraussetzung für diese Funktion: das ERP System gibt bei einem A+W Bearbeitungstyp 1090 eineDecoration mit, wenn nicht, bleibt alles beim Alten.
## OrderXMLSchnittstelle:<awProcessing\>

In einer Bearbeitung gibt es einen Bereich <awProcessing\>. Dieser beschreibt, welcher Bearbeitungstyp diese Bearbeitung definiert. Für den Bearbeitungstyp 1090 ist neu (5.5.3000), dass eineSN-Kantenqualität optional übergeben werden kann. Mit diesem Wert kann aus derOrderXML-Datei eineSN-Zeichnung erzeugt werden, wenn ein Bearbeitungstyp 1090 vorhanden ist.
Der DECO Wert wird in AWP ab 5.5.3000 in das Feld POOL\_BEARBEIT.BEARBEIT\_EXTRA1 geschrieben. Wird kein Wert übergeben, wird wie bisher der Wert aus BEARBEITSTAMM in das Feld geschrieben. Damit auch dieser Wert zur Berechnung verwendet wird, muss der neue Schalter_[ALCIM\_SHAPE / SNUSEORDERDECOFORAWTYPE1090]_ gesetzt werden.
<awProcessingtypeID="Polishing" id="**1010**" category="Edgework" quantity="10.25"quantityUnit="MTR"\>
<Polishing\>
<EdgeWork n="2" /\>
<EdgeWork n="4" /\>
</Polishing\>
</awProcessing\>

<awProcessingtypeID="OtherEdgework" id="**1090**" category="Edgework" quantity="3.75"quantityUnit="MTR"\>
<OtherEdgework**decoration="12"**\>
<EdgeWork n="1" /\>
</OtherEdgework\>
</awProcessing\>
