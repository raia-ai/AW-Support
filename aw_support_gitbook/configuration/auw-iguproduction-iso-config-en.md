---
title: "AUW_Configuration_FlippedIGUProduction"
source: "AUW_Configuration_FlippedIGUProduction.docx"
tags: ["A+W", "IGU production", "ISO", "MZO_EXTENDED", "AUSGANGSNR", "Feinplanung", "Configuration", "Machine driver", "XL_JOBRELEASE", "German"]
version: "1.0"
last_updated: "2025-10-08"
short_description: "This document describes how to configure and operate flipped IGU (insulating glass unit) production in A+W, including planning switches, machine driver settings, and database fields. It explains reasons to flip units, how flipping is recognized and displayed at production terminals, and details two approaches—via AUSGANGSNR or the MZO_EXTENDED model—to control unit and lite orientation throughout the ISO production line."
long_description: |
  Purpose and scope
  This document provides a comprehensive configuration and operating guide for producing insulating glass units (IGUs) in a flipped orientation within the A+W environment. It explains when and why flipped production is needed—such as to protect coatings or meet downstream logistics requirements—and how these needs tie into the capabilities of the ISO line (e.g., single‑lite flippers and unit flip stations).
  
  Core configuration switches
  Two global fine‑planning switches govern how lites are placed for an IGU: [FEIN_HARPRACK / ORDERING] and [FEIN_HARPRACK / ORIENTATION]. The document outlines their operational modes and interplay, including commonly used options 6 and 7. Mode 6 allows maximum flexibility by expressing production either via MZO_EXTENDED tables or by setting POOL_TEILE.AUSGANGSNR before fine planning; mode 7 mirrors mode 6 while additionally honoring ORIENTATION.
  
  Recognition in production and standard lists
  When AUSGANGSNR is set or MZO_EXTENDED is used, A+W Production Terminals and standard ISO production lists render the cross‑section and order of assembly appropriately for flipped units. Terminals visualize the unit build (not individual lite flips); lists also mark per‑lite flips where applicable.
  
  Machine driver parameters
  To ensure correct mirroring in the sealer’s machine code, XL_JOBRELEASE.CFG must be configured with MIRRORUNIT and UseCoatingPosition. MIRRORUNIT behavior is described for values N and Y in relation to AUSGANGSNR values (e.g., 1 or 11).
  
  AUSGANGSNR value semantics
  The field POOL_TEILE.AUSGANGSNR must be set (typically via a CU function) at least on the IGU and all cutting parts prior to fine planning; values 0, 1, 10, and 11 control whether the unit build and/or individual lites are flipped.
  
  MZO_EXTENDED data model
  The MZO_EXTENDED approach models how each part enters (MZO_EINSTELLEN) and exits (MZO_ABSTELLEN) each machine, including setup edge, flipping on entry or within the machine, and multi‑part sequencing for units. Constraints and activation via [ALCIM_SETTINGS / MZO_EXTENDED] are described, along with field‑level semantics (e.g., WENDEN_IN, WENDEN_INSIDE, WENDEN_OUT, WENDEN_AFTER) that govern orientation relative to bill of materials and coating side. The document focuses examples on ISO lines, where the model is most commonly applied.
---

# Configuration flipped IGU production

## History


| Date | Author | Modification/remarks | Version |
|---|---|---|---|
| 31.03.2014 | DLA | Issue | 1.0 |
| 18.05.2016 | DLA | MZO_EXTENDED | 1.1 |
|  |  |  |  |


## Content




















## Warum ISO gewendet produzieren?

Die Erfassung von ISO Einheiten erfolgt im Normalfall immer mit Ansicht von außen. In dieser Reihenfolge wird die ISO Einheit auch produziert. Es gibt Fälle wo eine ISO Einheit nicht in der Reihenfolge der Erfassung (erst äußere Scheibe aufstellen, dann innere Scheibe) produziert werden soll:

- Die ISO Einheit hat eine Beschichtung auf der ersten Scheibe zum SZR, und um Beschädigungen der Schicht zur verhindern, soll die Scheibe nicht mit der Schicht zur Linie aufgelegt werden. In diesem Fall produziert man die ISO Einheit komplett gewendet, die ISO Einheit wird umgedreht und die Einzelscheiben gewendet. Zuerst wird somit die zweite Scheibe aufgelegt, dann die erste mit Schicht weg von der ISO Linie.

- Die ISO Einheiten sollen gewendet von der Linie kommen, da dies z.B. für den Versand benötigt wird und man die fertige ISO Einheit nicht manuell wenden möchte.

Es gibt viele Gründe, die auch mit der Beschaffenheit der ISO Linie zusammenhängen:

- Hat die ISO Linie einen Einzelscheibenwender?

- Hat die ISO Linie eine Wendestation für fertige Einheiten?

- Wie werden die Scheiben auf die ISO Linie gestellt? Manuell oder über automatische Einzüge direkt von der Schneidanlage?

## Wie werden ISO Einheiten gewendet?

Es gibt zwei globale Schalter der Feinplanung, die das Abstellen der Scheiben einer ISO Einheit beeinflussen.

**[FEIN_HARPRACK / ORDERING]**

0 	 No matter or MZO_EXTENDED?
1 	 Coated lite to front
2 	 Coated lite to back
3 	 Coated lite to front. In case of exchange the lites will be mirrored, too.
4 	 Coated lite to back. In case of exchange the lites will be mirrored, too.
5 	 Special solution W+M
6 	 AUSGANGSNR or MZO_EXTENDED
7 	 Special solution Glasid


**[FEIN_HARPRACK / ORIENTATION]**

Dieser Schalter wirkt sich bei den [FEIN_HARPRACK / ORDERING] Modi 1-4,7 aus

0 	 No matter
1 	 Coated layer to front
2 	 Coated layer to back
3 	 Coated layer shows to inside
4 	 Coated layer shows tom outside

Soll eine Einzelscheibe gewendet werden, dann setzt die Feinplanung das Feld FEIN_TEILE.MIRROR. Ist das Feld nicht gleich dem Feld FEIN_TEILE.CUTMIRROR, muss die Scheibe vor dem aufstellen auf die ISO Linie erneut gewendet werden.

### [FEIN_HARPRACK / ORDERING] = 6

Eine häufig verwendete Konfiguration ist [FEIN_HARPRACK / ORDERING] = 6, da man hier alle Freiheiten hat. Diese Option bietet zwei mögliche Wege, um das Wenden in der ISO Produktion auszudrücken. Der erste ist die Verwendung des **MZO_EXTENDED** Modus, hier wird die Art der Produktion Scheibengenau in den Tabellen MZO_EINSTELLEN und MZO_ABSTELLEN beschrieben.  Um diese Tabellen mit den richtigen Werten zu füllen, ist eine komplexe CU Funktion nötig. Der zweite Weg läuft über das Feld **POOL_TEILE.AUSGANGSNR**, was vor der Feinplanung über eine CU Funktion gesetzt werden muss. Der Weg über die AUSGANGSNR ist der am meisten verwendetet Weg. Unsere Standardlisten reagieren auf diese Werte.

### [FEIN_HARPRACK / ORDERING] = 7

Dieser Modus entspricht dem Modus 6, aber es wird zusätzlich der Schalter [FEIN_HARPRACK / ORIENTATION] berücksichtigt.

## Wie wird das Wenden in der Produktion erkannt?

Wird AUSGANGNR gesetzt oder der MZO_EXTENDED Modus genutzt, wird dies an den A+W Production Terminals an der ISO Linie dargestellt. Diese wenden den Aufbau der ISO Einheit in der Liste und in der Querschnittsskizze, nur den Aufbau nicht die Einzelscheibe. Das ISO, ob gewendet oder nicht, wird vom Aufbau als Endprodukt dargestellt.

Auch die Standard ISO Produktionsliste reagiert auf die AUSGANGSNR und zeigt entsprechend den Aufbau an, auch hier immer den Querschnitt einer ISO Einheit. Soll Eine Scheibe zusätzlich gewendet eingestellt werden, wird dies auf der ISO Produktionsliste markiert.

### Maschinentreiber

Damit die Scheiben auch im Maschinencode des Versieglers entsprechend gewendet geschrieben werden, müssen zwei Schalter in der XL_JOBRELEASE.CFG richtig gesetzt werden.

- [GENERAL]MIRRORUNIT =Y/N (DEFAULT = N)

- [GENERAL]UseCoatingPosition = Y/N (DEFAULT = N)

Wenn AUSGANGSNR = 1 oder 11, dann wird der Schalter MIRRORUNIT aktiv:

- N = Scheiben werden umsortiert und dabei die Beschichtungslage mitgezogen

- Y = Scheiben werden umsortiert, gespiegelt und dabei die Beschichtungslage mitgezogen

## Konfiguration POOL_TEILE.AUSGANGSNR

Das Datenbankfeld **POOL_TEILE.AUSGANGSNR** muss vor der Feinplanung gesetzt werden (z.B. über eine CU Funktion). Folgende Werte kann das Feld haben:

0 	 ISO Aufbau so wie erfasst
1 	 ISO Aufbau und Einzelscheiben werden zur Erfassung gewendet
10 	 ISO Aufbau bleibt,  Einzelscheiben werden gewendet
11 	 ISO Aufbau wird gewendet,  Einzelscheiben nicht

Der Wert muss mindestens auf dem ISO Teil und auf allen Zuschnittsteilen gesetzt werden. Auf den Zuschnittsteilen wird er für XOPTON benötigt.

## Konfiguration MZO_EXTENDED

Diese Funktion bietet die Möglichkeit den Fluss von Scheiben durch die ganze Produktion zu beschreiben. Für alle Maschinen (ausgewählte und Alternativen) wird beschrieben wie eine Scheibe auf die Maschine eingestellt wird und wie sie aus der Maschine raus kommt.

Es gibt Grenzen dieses Modells, z.B. wenn das Einstellen auf 2 Maschinen gleichen Typs unterschiedlich ist, was Auswirkungen auf die Maschinen der Vorprozesse hat. Bei einer Umlastung auf die eine oder andere Maschine müssten die Vorprozesse neu berechnet werden, was nur bis zur Feinplanung möglich ist. Eine weitere Einschränkung ist, dass die Datenstruktur Positionsgenau ist. Ist PMO im Einsatz, kann Einheitengenau unterschiedlich abgestellt werden.

Über den Schalter _[ALCIM_SETTINGS / MZO_EXTENDED]_ wird diese Funktion aktiviert.


0 = MZO_EXTENDED wird nicht verwendet (Standard)

1 = MZO_EXTENDED ist aktiv, die Daten für Tabellen MZO_EINSTELLEN und MZO_ABSTELLEN müssen über die SP _cu_mzo_extended_ erzeugt werden

2 = MZO_EXTENDED ist aktiv, die Daten für Tabellen MZO_EINSTELLEN und MZO_ABSTELLEN werden für alle Maschinen initialisiert und müssen über die SP _cu_mzo_extended_ entsprechend angepasst werden


Aktuell wird diese Funktion nur verwendet, um eine ISO Linie anzusteuern, aus diesem Grund beziehen sich folgende Beispiele auf eine ISO Produktion.

### Datenstruktur

Die Daten werden in den Tabellen MZO_EINSTELLEN und MZO_ABSTELLEN beschrieben. Es gibt somit  Datensätze pro Teil und Maschine in beiden Tabellen mit folgenden Feldern:

| AUFTNR | Auftragsnummer (POOL_BEARBEIT.AUFTNR) |
|---|---|
| POS | Position (POOL_BEARBEIT.POS) |
| U_POS | Unterposition (POOL_BEARBEIT.U_POS) |
| TEILE_NR | Nummer des auf der Maschine zu produzierende Teils (POOL_BEARBEIT.TEILE_NR) |
| BEARB_NR | Bearbeitungsnummer (POOL_BEARBEIT.BEARB_NR) |
| ID_PHYS | Nummer der Maschine, für jede mögliche Maschine gibt es entsprechende Datensätze |

#### Tabelle MZO_EINSTELLEN

Tabelle MZO_EINSTELLEN beschreibt wie Teile auf eine Maschine eingestellt werden: die Aufstellkante, ob eine Scheibe gewendet eingestellt wird und ob eine Scheibe in der Maschine gewendet wird. Werden mehrere Teile einer Einheit in die Maschine eingestellt, wird die Reihenfolge der Teile beschrieben, wie es bei einer ISO Einheit der Fall ist.

| TEILE_NR_UNTERTEIL | Nummer des Unterteils was auf der Maschine zur Einheit zusammengebaut wird |
|---|---|
| REIHENFOLGE | Sequenz wie Unterteile auf die Maschine eingestellt werden |
| KANTE_IN | Kante auf der das Teil eingestellt wird |
| WENDEN_IN | Ausrichtung Schicht oder Struktur der Scheibe beim Einstellen in die Maschine:<br>0 – zeigt von Maschine weg<br>1 –zeigt zur Maschine hin |
| WENDEN_INSIDE | Behandlung Scheibe auf der Maschine (z.B. durch automatischer Wender):<br>0 – Scheibe bleibt wie eingestellt<br>1 – Scheibe wird gewendet |


_**WENDEN_IN **__**bezieht sich nicht auf die Stückliste sondern wo Schicht oder Struktur beim Einstellen liegt**__**. **__**WENDEN_INSIDE bezieht sich auf WENDEN_IN.**_

#### Tabelle MZO_ABSTELLEN

Die Tabelle beschreibt wie eine Einheit aus der Maschine kommt und dahinter abgestellt wird.

| KANTE_OUT | Aufstellkante auf der die Einheit aus der Maschine kommt |
|---|---|
| WENDEN_OUT | Einheit kommt aus der Maschine:<br>0 – wie Stückliste, erste Scheibe zeigt von Maschine weg<br>1 – gewendete Stückliste, erste Scheibe zeigt zur Maschine hin |
| KANTE_AFTER | Aufstellkante auf der die Einheit abgestellt wird |
| WENDEN_AFTER | Einheit wird hinter Maschine abgestellt:<br>0 – wie Stückliste, erste Scheibe zeigt von Maschine weg<br>1 – gewendete Stückliste, erste Scheibe zeigt zur Maschine hin |


_**WENDEN_OUT und WENDEN_AFTER beziehen sich auf Stückliste des Auftrags.**_ Liegt bei einer ISO Produktion die erste Scheibe der ISO Einheit (nach Stückliste) vorne (weg von der Linie), dann hat WENDEN_OUT den Wert 0, sonst 1.

Wenn WENDEN_OUT = WENDEN_AFTER, dann muss beim Abstellen der Einheit von der Maschine diese nicht gewendet werden. Sind die Werte ungleich, muss gewendet abgestellt werden.

Wie nach einer ISO Linie abgestellt werden soll, kann über das Feld POOL_POS.FACE bereits bei der Auftragserfassung bestimmt werden.

| POOL_POS.FACE | Beschreibung | Bedingung |
|---|---|---|
| 1 | Erste Scheibe der ISO Einheit zeigt zum Gestell | WENDEN_AFTER = 1 |
| 2 | Erste Scheibe der ISO Einheit zeigt weg vom Gestell | WENDEN_AFTER = 0 |
| 3 | Egal wie ISO Einheit auf Gestell gepackt wird | WENDEN_AFTER = WENDEN_OUT |


Auf welche Kante eine ISO Einheit abgestellt werden muss, kann bei Verwendung der PMO nicht alleine aus KANTE_OUT abgelesen werden, da für jede Einheit einer Position dies unterschiedlich sein könnte. In diesem Fall muss die Information aus der PMO_ITEMS ermittelt werden.

### Werte ermitteln

Tabellen MZO_EINSTELLEN und MZO_ABSTELLEN können im Modus 2 bereist mit Datensätzen initialisiert werden, aber all Felder die das Verhalten beschreiben stehen auf 0 oder -1. Die Reihenfolge beim Einstellen entspricht der Stückliste. Will man diese Funktion nutzen, muss man die Datensätze mit Leben füllen und das wird über die SP MZO_EXTENDED gemacht, die man nach Kundenanforderung entsprechend entwickeln muss.

### Feinplanung

Wird dieser Modus verwendet, werden die Felder MIRROR und PRODMIRROR in den Tabellen FEIN_UNIT und FEIN_TEILE bei einer ISO Produktion entsprechend der Werte aus MZO_EINSTELLEN und MZO_ABSTELLEN gesetzt. Die Feinplanung schaut dabei auf die Werte für die ISO Linie (ID_PHYS). Zulässige Werte in den Feldern sind 0 und 1.

**ISO Teil **
MIRROR 	= WENDEN_OUT
PRODMIRROR 	= WENDEN_AFTER

**Einzelscheibe**
MIRROR 	= WENDEN_IN 		 wenn Schicht/Struktur im Zuschnitt oben liegt
MIRROR	<> WENDEN_IN		 wenn Schicht/Struktur im Zuschnitt unten liegt
PRODMIRROR	= MIRROR		 wenn WENDEN_IN = WENDEN_INSIDE
PRODMIRROR	<> MIRROR		 wenn WENDEN_IN <> WENDEN_INSIDE

### Beispiele

#### ISO Einheit ohne Wenden produzieren

**POOL_TEILE**

| AUFTNR | POS | TEILE_NR | TTYP | ARTBEZ | BESCHICHT_POS | STRUKTUR_POS |
|---|---|---|---|---|---|---|
| 600001 | 1 | 0 | 7 | ISO | 0 | 0 |
| 600001 | 1 | 1000000 | 1 | FLOAT | 0 | 0 |
| 600001 | 1 | 2000000 | 12 | SPACER | 0 | 0 |
| 600001 | 1 | 3000000 | 1 | FL COAT | 1 | 0 |


MZO_EINSTELLEN

| AUFTNR | POS | TEILE_NR | ID_PHYS | UNTERTEIL | REIHENFOLGE | WENDEN_IN | WENDEN_INSIDE |
|---|---|---|---|---|---|---|---|
| 600001 | 1 | 0 | 1610 | 1000000 | 1 | 0 | 0 |
| 600001 | 1 | 0 | 1610 | 2000000 | 2 | 0 | 0 |
| 600001 | 1 | 0 | 1610 | 3000000 | 3 | 0 | 0 |


**MZO_ABSTELLEN**

| AUFTNR | POS | TEILE_NR | ID_PHYS | WENDEN_OUT | WENDEN_AFTER |
|---|---|---|---|---|---|
| 600001 | 1 | 0 | 1610 | 0 | 0 |

ISO Einheit kommt mit gewendeten Aufbau aus der Linie (Gegenscheibe zeigt von Linie weg), soll aber wie erfasst abgestellt werden.

**Stückliste**

**Einstellen**
1. Scheibe Teil 1000000				2. Scheibe Teil 2000000

**Produktion**
1.  Scheibe ansaugen		Rahmen auf 2. Scheibe		Produktion

**Abstellen**
ISO Einheit 			abstellen auf Gestell wie erfasst, erste Scheibe zeigt vom Gestell weg

#### ISO Einheit gewendet produzieren

**POOL_TEILE**

| AUFTNR | POS | TEILE_NR | TTYP | ARTBEZ | BESCHICHT_POS | STRUKTUR_POS |
|---|---|---|---|---|---|---|
| 600001 | 2 | 0 | 7 | ISO | 0 | 0 |
| 600001 | 2 | 1000000 | 1 | FL PATT | 0 | 2 |
| 600001 | 2 | 2000000 | 12 | SPACER | 0 | 0 |
| 600001 | 2 | 3000000 | 1 | FL COAT | 1 | 0 |


**MZO_EINSTELLEN**

| AUFTNR | POS | TEILE_NR | ID_PHYS | UNTERTEIL | REIHENFOLGE | WENDEN_IN | WENDEN_INSIDE |
|---|---|---|---|---|---|---|---|
| 600001 | 2 | 0 | 1610 | 1000000 | 3 | 0 | 0 |
| 600001 | 2 | 0 | 1610 | 2000000 | 2 | 0 | 0 |
| 600001 | 2 | 0 | 1610 | 3000000 | 1 | 0 | 1 |

Gegenscheibe wird zuerst aufgestellt und soll in der Linie gewendet werden, evtl. durch eine automatische Wendestation.

**MZO_ABSTELLEN**

| AUFTNR | POS | TEILE_NR | ID_PHYS | WENDEN_OUT | WENDEN_AFTER |
|---|---|---|---|---|---|
| 600001 | 2 | 0 | 1610 | 1 | 0 |

ISO Einheit kommt mit gewendeten Aufbau aus der Linie (Gegenscheibe zeigt von Linie weg), soll aber wie erfasst abgestellt werden.

**Stückliste**

**Einstellen**
1. Scheibe Teil 3000000				2. Scheibe Teil 1000000

**Produktion**
1.  Scheibe wenden und ansaugen 	Rahmen auf 2. Scheibe		Produktion

**Abstellen**
ISO Einheit gewendet produziert 	Abstellen auf Gestell wenden

## Maschinenansteuerung

Die Reihenfolge der Scheiben im Versieglercode entspricht der Stückliste, es sei denn die Scheiben sollen gewendet eingestellt werden. Wird POOL_TEILE.AUSGANGSNR verwendet, wird der Aufbau bei den Werten 1 und 11 gedreht. Bei MZO_EXTENDED aus dem Feld MZO_EINSTELLEN.REIHENFOLGE.


Die Ansteuerung einer Wendestation wurde bis jetzt nur für LISEC realisiert. Hier wird bei der Treiberausgabe für jede Scheibe die SP **cu_jr_turnunit** aufgerufen, diese ermittelt ob die Scheibe gewendet werden soll.

Übergabeparameter: AUFTNR, POS, U_POS, TEILE_NR, ID_PHYS

Soll gewendet werden wird ein entsprechender Bearbeitungssatz (<BEA>) in die LISEC Datei geschrieben:

```
<REL>|02.40|                                        
<BTH>|712001    |712001
<ORD>|204294    |3         |23VSP1                                  |23VSP1                          . . . |09/11/2009|16/12/2009|0000000000
<POS>|00001|     A01|2001|00001|02384|04944|3-0  |13 |3-0  |   |     |063|00|00|00|1|0|00000|0
<BEA> 001 0 0                                          07 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 00000 00000 00000 00000 00000
<GL1>|00001|3.1 Clear                               |0|00008|0| A01      |0
<GL2>|00001|3.1 Clear                               |0|00008|0| A02      |0
<FR1>|00001|13.0 Super Spacer                       |04|00|00032|00012|          
<TXT>|

```
Wird MZO_EXTENDED verwendet, muss die SP den Wert aus MZO_EINSTELLEN.WENDEN_INSIDE einfach weiter geben. Hier ein SP Beispiel:

```
CREATE PROCEDURE cu_jr_turnunit (sp_auftnr INTEGER, sp_pos INTEGER, sp_u_pos INTEGER, sp_teile_nr INTEGER, sp_id_phys INTEGER)
  DEFINE sp_wenden_inside INTEGER;
  LET sp_wenden_inside = 0;
  SELECT wenden_inside INTO sp_wenden_inside FROM mzo_einstellen WHERE auftnr = sp_auftnr AND pos = sp_pos AND u_pos = sp_u_pos and teile_nr_unterteil = sp_teile_nr AND id_phys = sp_id_phys;
  RETURN sp_wenden_inside;
END PROCEDURE;
```
