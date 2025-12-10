---
title: "AUW_Configuration_Combine_Strips_for_optimization"
source: "AUW_Configuration_Combine_Strips_for_optimization.docx"
tags: ["AUW", "configuration", "combine strips", "optimization", "manufacturing", "process", "setup", "guide", "best practices"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "CombineStripsforOptimization History Content Hintergrund Die Kanten kleinerRechteck-Scheiben können oft nicht maschinell bearbeitet werden. Durch ein Zusammenlegen der kleinen Scheiben zu einer größeren Rechteckscheibe können zumindest einige der Bearbeitungen maschinell durchgeführt werden. Die Außenkanten werden bearbeitet, danach wird die Scheibe in Streifen geschnitten und die Innenkanten können bearbeitet werden."
long_description: "CombineStripsforOptimization History Content Hintergrund Die Kanten kleinerRechteck-Scheiben können oft nicht maschinell bearbeitet werden. Durch ein Zusammenlegen der kleinen Scheiben zu einer größeren Rechteckscheibe können zumindest einige der Bearbeitungen maschinell durchgeführt werden. Die Außenkanten werden bearbeitet, danach wird die Scheibe in Streifen geschnitten und die Innenkanten können bearbeitet werden. Mit dieser Funktion werden Scheiben zu einer einzigen großen Scheibe zusammengefasst. Das Schneiden in kleine Scheiben muss später erfolgen. Die Anforderung, dass Zwischenschnitte auch gleich geschnitten werden, aber erst nach dem polieren, z.B. hinter einemDoppelseiter, gebrochen werden, wird durch diese Funktion nicht unterstützt. Voraussetzung Es wird in Tabelle POOL_TEILE ein freies SONDERTEXT Feld (SONDERTEXT1, SONDERTEXT2, SONDERTEXT3. SONDERTEXT4 oder SONDERTEXT5) benötigt um das Zusammenlegen der Scheibe zu beschreiben. Für die Optimierung wird im Modellkatalog die**666.FRM**benötigt, auf diese bezieht sich die zusammengelegte Scheibe (FRM Datei wird im UnterverzeichnisC:\Program Files (x86)\A+W\Techsoft\Shapes\SpecialShapes\ mit ausgeliefert). DieseFunktion arbeitet mit dem A+W Modellkatalog und nur mit Rechtecken.Wenn auch Rechtecke eine SN Zeichnung haben, muss der Schalter[ALCIM_SHAPE / SNCUTASSTANDARDFRM] auf 1 gesetzt sein (indiesem Zusammenhang unabhängig von dieser Funktion evtl. auch [ALCIM_SHAPE / SNUPDATESTEP] setzen). Aktivieren der Funktion Die Funktion wird in der Feinplanung über den versteckten Schalter [FEIN_SPECIALS /TOGETHER666] aktiviert. Der Wert im Feld [TEXT] ist die Nummer der Spalte SONDERTEXT aus der Tabelle POOL_TEILE: 1,2,3,4 oder 5.Sobald das FeldamZuschnittsteilmit einem entsprechenden Wert gefüllt ist, wird die Funktion verwendet."
---
CombineStripsforOptimization

History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 2015.10.07 | DLA | Issue | 1.0 |
|  |  |  |  |

Content

## Hintergrund

Die Kanten kleinerRechteck-Scheiben können oft nicht maschinell bearbeitet werden.

Durch ein Zusammenlegen der kleinen Scheiben zu einer größeren Rechteckscheibe können zumindest einige der Bearbeitungen maschinell durchgeführt werden.

Die Außenkanten werden bearbeitet, danach wird die Scheibe in Streifen geschnitten und die Innenkanten können bearbeitet werden.

Mit dieser Funktion werden Scheiben zu einer einzigen großen Scheibe zusammengefasst. Das Schneiden in kleine Scheiben muss später erfolgen. Die Anforderung, dass Zwischenschnitte auch gleich geschnitten werden, aber erst nach dem polieren, z.B. hinter einemDoppelseiter, gebrochen werden, wird durch diese Funktion nicht unterstützt.

## Voraussetzung

Es wird in Tabelle POOL_TEILE ein freies SONDERTEXT Feld (SONDERTEXT1, SONDERTEXT2, SONDERTEXT3. SONDERTEXT4 oder SONDERTEXT5) benötigt um das Zusammenlegen der Scheibe zu beschreiben.

Für die Optimierung wird im Modellkatalog die**666.FRM**benötigt, auf diese bezieht sich die zusammengelegte Scheibe (FRM Datei wird im UnterverzeichnisC:\Program Files (x86)\A+W\Techsoft\Shapes\SpecialShapes\ mit ausgeliefert).

DieseFunktion arbeitet mit dem A+W Modellkatalog und nur mit Rechtecken.Wenn auch Rechtecke eine SN Zeichnung haben, muss der Schalter[ALCIM_SHAPE / SNCUTASSTANDARDFRM] auf 1 gesetzt sein (indiesem Zusammenhang unabhängig von dieser Funktion evtl. auch [ALCIM_SHAPE / SNUPDATESTEP] setzen).

## Aktivieren der Funktion

Die Funktion wird in der Feinplanung über den versteckten Schalter [FEIN_SPECIALS /TOGETHER666] aktiviert. Der Wert im Feld [TEXT] ist die Nummer der Spalte SONDERTEXT aus der Tabelle POOL_TEILE: 1,2,3,4 oder 5.Sobald das FeldamZuschnittsteilmit einem entsprechenden Wert gefüllt ist, wird die Funktion verwendet.

INSERTINTOparameter(lastmodstation,lastmodzeit,bereich,eintrag,nummer,typ,text)VALUES('AW----',CURRENT_TIMESTAMP,'FEIN_SPECIALS','TOGETHER666',0,0,'5');

## RegelzumZusammenlegen

Über einemit dem Kunden zu erarbeitendenCU Funktion wird definiert wie die Scheiben einer Position zusammengelegt werden sollen.Das Ergebnis muss im SONDERTETEXT Feld gespeichert werden und muss folgenden Aufbau haben:

**A_x_B**oder**A_x_B_x_C_x_D_x_E**

A = Anzahlder Stapel (Scheiben auf kurze Kante (Breite) gestapelt)

B =Anzahl der Scheiben in einem Stapel (Scheiben auf lange Kante (Höhe) gestapelt)

C = Höhe der Zwischenstückeim Stapelin mm[Gesamthöhe der Zwischenstücke = (B-1)*C ]

D = Höhe des Ergänzungsstücksdes Stapelsin mm

E = Gesamthöhe des Stapelsin mm[wenn E>0, so C=0 und D=0]

Die Gesamthöhe der großen Scheibe ist also entweder gegeben durch E (falls E>0) oder (falls E=0) durch: [Kurze Kante] * B + (B-1)*C + D

Die Gesamtbreite der großen Scheibe ist immer gegeben durch:

[Lange Kante] * A

Beispielvon 2 Stapeln, jeder Stapel enthält 4 Scheiben mit definierten Zwischenstück und Endstück: 2_x_4_x_1_x_1_x_0

## Beispiele

Die folgenden Beispiele sind mit einerPositionmit der Größe 1350x250 und derMenge 22durchgeführt worden.

**1_x_5**

Scheiben mit je 5 Streifen, Insgesamt 25 Streifen(3 zu viel).

**1_x_5_x_1_x_1_x_0******

Scheiben mit je 5 Streifen, Insgesamt 25 Streifen(3 zu viel). 1mm zwischen den Streifen und 1 mm am Ende ergibt eine Breite von 1255.

**1_x_5_x_0_x_0****_x_****1260**

Scheiben mit je 5 Streifen, Insgesamt 25 Streifen und einer Gesamthöhe von Fest 1260.

**1_x_5_x_0_x_0****_x_****1100**

Scheiben mit je 5 Streifen, Insgesamt 25 Streifen (3 zu viel) und einer Gesamthöhe von Fest 1100, hier wäre der einzelne Streifen zu klein. Es gibt keine Logikprüfung, die Konfiguration muss richtig sein!

**2****_x_****1**

2 Scheiben auf der kurzen Kante gestapelt ergibt eine Breite von 2700, Höhe bleibt bei 250.

**2****_x_5_x_1_x_1_x_0**

Scheibenmit je 10 Streifen (2 Pakete mit je 5 Streifen übereinander), insgesamt 30 Streifen (8 zu viel). 1mm zwischen den Streifen und 1 mm am Ende ergibt eine Breite von 1255. Höhe 2x1350 = 2700
