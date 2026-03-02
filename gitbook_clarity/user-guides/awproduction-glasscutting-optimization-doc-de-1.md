---
description: "DE_AWProduction_Realtime_Optimizer_3_3"
---


# Softwarereferenz

---
## Erfassung

### Erläuterung der Felder im Bereich Chargen Bezeichnung

**Checkbox**
Wenn Sie diese Checkbox aktivieren, wird die eingegebene Chargen Nummer auf die nachfolgenden Lagerplatten der gleichen Glasart/Dicke vererbt.

**Feld**
In diesem Feld geben Sie die Chargen Bezeichnung ein.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Chargen-Editor" auf Seite J-100

---

## Optimierung

### Menü Optimierung öffnen

Im Menü **Erfassung** befinden sich folgende Programmpunkte:

- **Tischoptimierung:**
  Über diesen Menüpunkt können Sie eine Tischoptimierung erstellen.
  ⇨ Softwarereferenz, "Selektieren Sie die zu optimierenden Gläser" auf Seite J-103

- **Zurücksetzen:**
  Über diesen Menüpunkt haben Sie die Möglichkeit, Läufe zurückzusetzen.
  ⇨ Softwarereferenz, "Zurücksetzen eines Zuschnitt Laufes" auf Seite J-119

---

## Selektieren Sie die zu optimierenden Gläser

**Optimierung > Tischoptimierung**

Diesen Dialog gibt es in zwei unterschiedlichen Varianten. Welche Variante angezeigt wird, hängt davon ab, welche Einstellungen Sie für die Tischoptimierung getroffen haben:
- Standard
- Produktionstermin
⇨ Kapitel "Tischoptimierung" auf Seite J-151

### Tischoptimierung in der Variante Standard

*(Abb. J-61 Selektieren Sie die zu optimierenden Gläser - Standard)*

In diesem Dialog listet Ihnen A+W Realtime Optimizer alle Glasarten auf, für die Läufe und Eilscheiben zur Optimierung bereit stehen. Zu der gewählten Glasart werden die verfügbaren Läufe angezeigt.

#### Erläuterung der Felder im Bereich Verfügbare Glasarten

**Glasart**
Dieses Feld zeigt Ihnen die Artikelnummer der Glasart, für die Läufe verfügbar sind. Der Wert dieses Feldes kommt aus den Stammdaten.

**Dicke**
In diesem Feld wird die Dicke der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.

**Restelager**
Diese Spalte wird nur angezeigt, wenn Ihr A+W Realtime Optimizer zur Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde. In dieser Spalte steht ein Eintrag, wenn im Restelager-Magazin eine Scheibe der entsprechenden Glasart und Dicke vorhanden ist. Die angegebene Zahl ist die Länge des Restblattes in mm im Restelager-Magazin. Wenn im Restelager-Magazin mehrere Restblätter der entsprechenden Glasart und Dicke liegen, dann wird das längste Restblatt hier angezeigt.

**Bruchmenge**
Wenn für diese Glasart Bruchscheiben erfasst sind, wird in diesem Feld die Anzahl der Bruchscheiben angegeben.

**Bruchfläche**
Wenn für diese Glasart Bruchscheiben erfasst sind, wird in diesem Feld die Gesamtfläche der Bruchscheiben angegeben.

**Eilmenge**
Wenn für diese Glasart Eilscheiben erfasst sind, wird in diesem Feld die Anzahl der Eilscheiben angegeben.

**Eilfläche**
Wenn für diese Glasart Eilscheiben erfasst sind, wird in diesem Feld die Gesamtfläche der Eilscheiben angegeben.

**Glasart Bezeichnung**
In diesem Feld wird Ihnen die Klartextbezeichnung der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.

#### Erläuterung der Felder im Bereich Verfügbare Optimierungen

**Lauf**
In dieser Spalte sehen Sie die Nummer des Laufes, der Optimierungen für die gewählte Glasart enthält.

**Los**
In dieser Spalte sehen Sie die Losnummer des Laufes, der die Optimierungen für die gewählte Glasart enthält.

**Gesperrt**
In dieser Spalte sehen Sie, ob und von welcher Station das Los zur Bearbeitung oder Verwendung in einer Optimierung gesperrt ist.

**Parameter**
In dieser Spalte sehen Sie, für welchen Tisch das angezeigte Los optimiert wurde.

**Platten**
In dieser Spalte sehen Sie, wieviele Lagerplatten die Losoptimierung benötigt.

**Scheibenmenge**
In dieser Spalte sehen Sie, wieviele Scheiben die Losoptimierung beinhaltet.

**Scheibenfläche**
In dieser Spalte sehen Sie, wieviele Quadratmeter Glas die Losoptimierung beinhaltet.

**Verschnitt**
In dieser Spalte sehen Sie, wieviel Verschnitt in % bei der aktuellen Losoptimierung entstehen würde.

**Rest (mm)**
In dieser Spalte sehen Sie, wie lange das Restblatt ist, dass bei der Losoptimierung auf dem Schneidtisch übrig bleibt.

**Information**
In dieser Spalte werden Ihnen Laufbezeichnung angezeigt.

**Termin**
In dieser Spalte sehen Sie den Produktionstermin, der bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.

**Schicht**
In dieser Spalte sehen Sie die Produktionsschicht, die bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.

#### Erläuterung der Checkbox

**Erlaube Handzuschnitt**
Wenn diese Checkbox markiert ist, dann werden in der Liste Glasarten auch die Glasarten zur Optimierung angezeigt, die bei der Artikeldefinition in den Stammdaten nur für Handzuschnitt vorgesehen wurden.
- `[ ]` nur Glasarten für den automatischen Zuschnitt anzeigen
- `[x]` auch Glasarten für den Handzuschnitt anzeigen

---

### Tischoptimierung in der Variante Produktionstermin

*(Abb. J-62 Selektieren Sie die zu optimierenden Gläser - Produktionstermin)*

Dieser Dialog zeigt die Produktionstermine und ermöglicht es Ihnen, die Optimierungen nach den Produktionstermin zu filtern. Dies erleichtert die Einhaltung von Fristen und die Planung des Produktionsablaufs.

Wählen Sie zunächst einen Produktionstermin aus der Liste **Produktionsdatum**.

Im Bereich **Verfügbare Glasarten** werden Ihnen alle Glasarten angezeigt, die in Optimierungen mit dem ausgewählten Produktionsdatum enthalten sind. Wählen Sie anschließend die Glasart aus, die Sie schneiden möchten.

Im Bereich **Verfügbare Optimierungen** werden Ihnen alle Optimierungen angezeigt, die bis zum ausgewählten Produktionsdatum produziert sein sollten. Für eine bessere Übersicht sind die Optimierungen sind farbig markiert:
- **Grün:** Der Produktionstermin liegt in der Zukunft.
- **Gelb:** Der Produktionstermin ist heute.
- **Rot:** Der Produktionstermin liegt in der Vergangenheit.

Die Felder der Bereiche **Verfügbare Glasarten** und **Verfügbare Optimierungen** sind identisch mit den Feldern im Dialog Tischoptimierung in der Variante Standard und werden an dieser Stelle erläutert.
⇨ Kapitel "Tischoptimierung in der Variante Standard" auf Seite J-103

**Ergänzende Informationen**
⇨ Tutorial, "Läufe zum Zuschnitt auswählen" auf Seite J-40

---

## Tischoptimierung Lauf [Nr]

Mit diesem Dialog werden verschiedene Parameter für die Optimierung eingestellt. Der Dialog ist in folgende Register unterteilt:
- Übersicht
- Optimieren
- Restplatten und Lagerplatten
- Parameter

### Übersicht

**Optimierung > Tischoptimierung > Gläser selektieren - [Auswählen] > Übersicht**

*(Abb. J-63 Tischoptimierung - Übersicht)*

Dieser Dialog zeigt die im Dialog **Selektieren Sie die zu optimierenden Gläser** gewählten Läufe an. Wurde eine Optimierung durchgeführt, so wird deren Ergebnis angezeigt. Wenn noch keine Optimierung durchgeführt wurde, sind die Felder **Platten**, **Verschnitt** und **Rest (mm)** leer.

Nach einer durchgeführten Optimierung, kann per Doppelklick auf die Glasart das Programm **PlanEdit** gestartet werden, falls dieses an Ihrem Arbeitsplatz installiert ist. **PlanEdit** zeigt Ihnen das Brechbild der Lagerplatte grafisch an.

#### Erläuterungen der oberen Liste

**Glasart**
In diesem Feld werden Ihnen die Artikelnummern der Glasarten angezeigt, die in der gewählten Tischoptimierung enthalten sind. Der Wert dieses Feldes kommt aus den Stammdaten.

**Dicke**
In diesem Feld wird Ihnen die Dicke der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten in mm oder inch (konfigurierbar).

**Parameter**
Wenn die Optimierung durchgeführt wurde, dann sehen Sie in diesem Feld, mit welchen Optimierungsparametern die Optimierung durchgeführt wurde.

**Menge**
Der Wert dieses Feldes zeigt Ihnen die Anzahl der Scheiben.

**Fläche**
In diesem Feld sehen Sie die gesamte Fläche der optimierten Glasart in Quadratmeter.

**Platten**
Diese Feld zeigt Ihnen die Anzahl der Lagerplatten, die für die Optimierung benötigt werden (Anzeige erst nach durchgeführter Optimierung).

**Verschnitt**
In diesem Feld sehen Sie die Glasfläche in %, die als Verschnitt anfällt (Anzeige erst nach durchgeführter Optimierung).

**Rest (mm)**
Hier sehen Sie die Breite des Restblatts in mm, das nach dem Zuschnitt noch auf dem Tisch liegt und weiterverwendet werden könnte (Anzeige erst nach durchgeführter Optimierung).

#### Erläuterungen der unteren Liste

**Lauf**
Das Feld zeigt Ihnen die Nummer der Läufe, von denen ein Los in der angezeigten Tischoptimierung enthalten ist.

**Los**
Das Feld zeigt Ihnen die Nummer des Loses, dessen Scheiben in der angezeigten Tischoptimierung enthalten sind.

**Zuschnitts-Böcke**
In diesem Feld sehen Sie die Anzahl der Zuschnittsböcke, die von der Feinplanung für die Scheiben dieses Losen eingeplant wurden.

**Sonderglaslauf**
Hier wird angegeben, ob es sich um einen Sonderglaslauf handelt. Ein Sonderglaslauf liegt dann vor, wenn die gewählte Glasart in den Stammdaten als Sonderglas definiert wurde. Mögliche Werte:
- Ja
- Nein

**Platten**
In diesem Feld sehen Sie die Anzahl an Lagerplatten, die für den Zuschnitt des Loses ermittelt wurden. Es handelt sich hierbei um das Berechnungsergebnis der **Feinplanung**, nicht der Tischoptimierung.

**Verschnitt**
Das Feld zeigt Ihnen die Glasfläche in %, die beim Zuschnitt des Loses als Verschnitt anfällt. Es handelt sich hierbei um das Berechnungsergebnis der **Feinplanung**, nicht der Tischoptimierung.

**Rest (mm)**
In diesem Feld sehen Sie die Breite des Restblatts in mm, das nach dem Zuschnitt des Loses noch auf dem Tisch liegt und weiterverwendet werden könnte. Es handelt sich hierbei um das Berechnungsergebnis der **Feinplanung**, nicht der Tischoptimierung.

**Ergänzende Informationen**
⇨ Tutorial, "Tischoptimierungen erstellen" auf Seite J-29
⇨ Tutorial, "Tischoptimierungen" auf Seite J-29

---

### Optimieren

**Optimierung > Tischoptimierung > Gläser selektieren - [Auswählen] > Optimieren**

*(Abb. J-64 Optimieren)*

In diesem Dialog nehmen Sie die Einstellungen für die Optimierung vor. Die Liste liefert Ihnen Informationen zu der gewählten Glasart.

#### Erläuterung der Felder im Bereich Optimierungsreihenfolge

**Lauf**
In diesem Feld sehen Sie, welcher Lauf bzw. welche Läufe optimiert werden sollen.

**Los**
Dieses Feld zeigt Ihnen, die Losnummer der einzelnen Läufe.

**Rang**
Dieses Feld zeigt Ihnen den Optimierungsrang. Durch Betätigen der Schaltflächen `^` oder `v` können Sie Rangfolge ändern. Gleiche Ränge werden gemischt, unterschiedliche getrennt.

**Positionen**
In diesem Feld sehen Sie, wie viele Positionen in dem Lauf enthalten sind.

**A-Böcke**
Das Feld zeigt Ihnen die Anzahl der A-Böcke, die für diesen Lauf notwendig sind.

**Fächerwagen**
Das Feld zeigt Ihnen die Anzahl der Fächerwagen, die für diesen Lauf notwendig sind.

**Scheibenmenge**
Das Feld zeigt Ihnen die Anzahl Scheiben, die in diesem Lauf enthalten sind.

**Scheibenfläche**
Das Feld zeigt Ihnen die Scheibenfläche in qm, die in diesem Lauf enthalten sind.

**Platten**
Das Feld zeigt Ihnen die Anzahl der Platten, die zum Schneiden dieses Laufes notwendig sind.

#### Erläuterung der Schaltflächen im Bereich Rangfolge

**^**
Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie z. B. einen Lauf mit dem Rang 1 gewählt und betätigen dann die Schaltfläche ^, ändert sich der Rang von 1 nach 2. Gleichzeitig ändert sich gegebenenfalls die Sortierung der Tabelle.

**v**
Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie z. B. einen Lauf mit dem Rang 2 gewählt und betätigen dann die Schaltfläche v, ändert sich der Rang von 2 nach 1. Gleichzeitig ändert sich gegebenenfalls die Sortierung der Tabelle.

**Auswählen**
Mit dieser Kombobox steuern Sie den Rang. Die Kombobox enthält soviel Ränge, wie Läufe in der Tabelle zu sehen sind. Sie können dann aus der Tabelle einen Lauf auswählen, die Kombobox öffnen und dem ausgewählten Lauf den gewünschten Rang zuweisen. Die Ränge sind fortlaufend zu vergeben, d. h. es kann kein Rang übersprungen werden. Nach Rang 1 folgt Rang 2 und danach Rang 3. Rang 2 kann nicht übersprungen werden. Haben Sie einem Lauf einen niederen Rang zugewiesen, ändert sich ebenfalls die Sortierung der Tabelle.

#### Erläuterung der Felder im Bereich Automatische Zusammenstellung

**Lose trennen**
Mit dieser Checkbox steuern Sie, ob ein Trennen der Lose gewünscht ist oder nicht. Mögliche Werte:
- `[ ]` Lose werden nicht getrennt.
- `[x]` Lose werden getrennt. Wenn Sie die Checkbox aktivieren, hat das u. U. Auswirkung auf das Feld Rang.

**Lose nach maximaler Anzahl der Zuschnittsböcke trennen**
Mit dieser Checkbox steuern Sie, ob und wenn ja wann Lose getrennt werden. Wenn Sie wünschen, dass Lose nach einer gewissen Anzahl von Zuschnittsböcken getrennt werde, müssen Sie die Checkbox aktivieren und im Feld dahinter die Menge eingeben, nach der getrennt werden soll.

**Mindestscheibenfläche für das Trennen von Losen verwenden**
Mit dieser Checkbox steuern Sie, ob und wenn ja wann Lose getrennt werden. Wenn Sie wünschen, dass Lose ab einer gewissen Scheibenfläche (in qm) getrennt werde, müssen Sie die Checkbox aktivieren und im Feld dahinter die Fläche eingeben, nach der getrennt werden soll.

> **Trennen von Losen**
> Lose können entweder nach einer maximalen Anzahl von Zuschnittsböcken oder einer Mindestscheibenfläche getrennt werden. Beide Checkboxen können zusammen nicht aktiviert werden.

#### Erläuterung der Felder im Bereich Lauf-Parameter

**XOPT-S**
Verwenden Sie in Ihrem Betrieb A-Böcke, dann muss dieser Parameter gesetzt werden. Die Optimierung berücksichtigt dann, dass die Scheiben auf A-Böcke gestellt werden und für die nachfolgende Bearbeitungen in einer bestimmten Reihenfolge stehen müssen.

**Bruchscheiben**
Wenn Sie diesen Parameter wählen, dann lassen Sie zu, dass immer dann, wenn zu der gewählten Glasart Bruchscheiben existieren, diese automatisch in die anstehende Optimierung mit einbezogen werden.

**Eilscheiben**
Wenn Sie diesen Parameter wählen, dann lassen Sie zu, dass immer dann, wenn zu der gewählten Glasart Eilaufträge existieren, diese automatisch in die anstehende Optimierung mit einbezogen werden.

**Füller nur für Lücken**
Existieren in Ihrem System Füllaufträge der gleichen Glasart und haben Sie diesen Parameter gesetzt, dann werden bei der Optimierung eventuell vorhandene Lücken in der Optimierung mit Füllaufträgen gefüllt. Das Restblatt wird nicht mit Füllaufträgen aufgefüllt. Existieren Füllaufträge zur gewählten Glasart, so werden diese im Register Füller angezeigt.

**Restelager**
Diese Checkbox wird nur angezeigt, wenn Sie über ein entsprechendes Restelager verfügen.
- `[ ]` Das Restelager wird nicht verwendet
- `[x]` Das Restelager wird verwendet

#### Erläuterung der Felder im Bereich Tisch

**Tisch**
Die Kombobox enthält alle in Ihrem Hause konfigurierten Tische. Wählen Sie aus der Kombobox den entsprechenden Tisch aus. Im darunter liegenden Bereich wird Ihnen der Name des Tisches angezeigt.

#### Erläuterung der Felder im Bereich Optimierungs-Parameter

**Optimierungsparameter**
Die Kombobox enthält die Optimierungsparameter, mit denen die Optimierung erstellt werden soll. Es stehen nur die Optimierungsparameter zur Verfügung, mit denen der ausgewählte Tisch arbeiten kann. Wählen Sie aus der Kombobox den entsprechenden Parameter aus. Im darunter liegenden Bereich wird Ihnen der Name des Parameters angezeigt.

#### Erläuterung der Schaltflächen

**Optimieren**
Mit dieser Schaltfläche starten Sie die Optimierung. Die Optimierung läuft im Hintergrund. Sobald das Ergebnis vorliegt, kann es im Register Übersicht angesehen werden. Das Optimierungsergebnis wird erst dann in die Datenbank gespeichert, wenn die Schaltfläche [Speichern] oder [Schneiden] betätigt wird.

**Ergänzende Informationen**
⇨ Tutorial, "Tischoptimierungen" auf Seite J-29

---

### Restplatten und Lagerplatten

**Optimierung > Tischoptimierung > Restplatten und Lagerplatten**

*(Abb. J-65 Restplatten und Lagerplatten)*

In diesem Dialog wählen Sie für die zuvor ausgewählte Glasart die Restplatten und die Lagerplatten aus, die Sie für die Optimierung verwenden möchten. Auf der linken Seite sehen Sie die gewählte Glasart. Die rechte Seite zeigt Ihnen die zur Glasart passende(n) Lagerplatte oder, wenn vorhanden, die passenden Restplatten. Diese sind nach Verfügbarkeit sortiert und gruppiert im Sinne der Entladereihenfolge des Gestells.

#### Erläuterung der Felder im Bereich Liste Lagerplatten (rechts)

**Breite**
Das Feld zeigt Ihnen die Breite der Lagerplatte in mm.

**Höhe**
Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm.

**XY?**
In dieser Spalte ist angegeben, in welcher Richtung die Travere gebildet wird. Mögliche Werte:
- **X:** Die Travere verläuft zwingend senkrecht zum unteren Plattenrand.
- **Y:** Die Travere verläuft zwingend parallel zum unteren Plattenrand.
- **?:** Die Optimierung kann sich wahlweise für eine der beiden Traverenrichtungen entscheiden.

**Restelagerfach**
Das Feld zeigt Ihnen, wo sich die Lagerplatte befindet. Steht in diesem Feld der Begriff **Lager**, handelt es sich bei der Platte um eine Lagerplatte. Steht in dem Feld eine Ziffer, z. B. 2, dann handelt es sich bei der Platte um eine Restlagerplatte, die sich im Restelagerfach mit der Nummer 2 befindet. Steht in dem Feld **WH** (Warehouse) befindet sich die Platte in einem vertikalen Remaster. Steht in dem Feld **RM**, befindet sich die Platte in einem (horizontalen) Remaster.

**Einlagerzeit / Menge**
Wenn es sich bei der Platte um eine Restlagerplatte handelt, können Sie in diesem Feld das Datum und die Uhrzeit der Einlagerung (in das Restelager) sehen. Steht in dem Feld eine Zahl, z. B. 7670, dann handelt es sich bei der Platte um eine Lagerplatte, von der noch 7670 Stück auf Lager sind.

#### Erläuterung der Felder im Bereich Restblatt

**Höhe/Breite**
Liegt auf dem Zuschnitttisch vom vorherigen Zuschnitt noch ein Restblatt der gleichen Glasart und Dicke, so können Sie dieses weiter verwenden. Geben Sie hier Höhe und Breite des Restblatts ein. Die Optimierung nutzt dann zuerst dieses Restblatt aus, bevor eine neue Lagerplatte verwendet wird.

> **Restblatt und Restelager-Platte nicht gleichzeitig möglich!**
> Wenn Sie bereits eine Restelager-Platte verwenden, kann kein Restblatt mehr verwendet werden. Wenn Ihr A+W Realtime Optimizer zur Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde, dann kann die Verwendung einer Restelager-Platte im Register Optimieren mit der Checkbox **Verwenden** ein- und ausgeschaltet werden.

**Ergänzende Informationen**
⇨ Tutorial, "A+W Residual Stock Manager" auf Seite J-50

---

### Parameter

**Optimierung > Tischoptimierung > Parameter**

*(Abb. J-66 Parameter)*

In diesem Dialog nehmen Sie die Parameter-Einstellungen für die Tischoptimierung vor. Die Liste zeigt Ihnen die für die Optimierung zur Verfügung stehenden Lagerplatten.

#### Erläuterung der Felder im Bereich Beschichtung

**Keine/Oben/Unten**
Falls die Lagerplatte über eine Beschichtung verfügt, geben Sie mit diesen Radiotasten an, ob sich die Beschichtung **oben** oder **unten** befindet. Hat die Lagerplatte keine Beschichtung, aktivieren Sie die Radiotaste **Keine**.

#### Erläuterung der Schaltfläche

**Anzahl**
Mit dieser Schaltfläche öffnen Sie den Dialog **Anzahl der Lagerplatten**.

#### Erläuterung der Felder im Bereich Optimierungs-Parameter

**Ränder**
Die Felder **Rand links**, **Rand rechts**, **Rand oben** und **Rand unten** zeigen Ihnen die für den entsprechenden Glasartikel erfassten Bruchränder. Die grau unterlegten Felder beziehen sich auf die aus den Glasartikel-Stammdaten gezogenen Werte. In den weiß unterlegten Feldern können Sie diesen Wert überschreiben. Es handelt sich dabei um ein temporäres Ändern der Bruchrändern für den jeweiligen Lauf.

**Autotravere**
Die Checkbox steuert, ob die angegebene maximale Traverenbreite vergrößert werden darf.
- `[x]` Die angegebene maximale Traverenbreite darf vergrößert werden.
- `[ ]` Die angegebene maximale Traverenbreite darf nicht vergrößert werden.

**Max. Travere**
Das Feld **Max. Travere** bezieht sich auf die maximale Traverenbreite des gewählten Glasartikels. Das grau unterlegte Feld bezieht sich auf den aus dem Glasartikel-Stammdaten gezogenen Wert. In dem weiß unterlegten Feld können Sie diesen Wert überschreiben. Es handelt sich dabei um ein temporäres Ändern der maximalen Traverenbreite für den jeweiligen Lauf.

**Schneidmodus**
Das Feld legt den Schneidmodus für die XOPT(S)-Optimierungen fest. Die gesetzte Radiotaste zeigt Ihnen, mit welchem Schneidmodus die Feinplanung durchlaufen wurde. Die Auswahl des richtigen Schneidmodus richtet sich nach dem Schneidtisch und den betrieblichen Anforderungen. Generell gilt, dass mit Schneidmodus 1 die besten und mit Schneidmodus 4 geringfügig schlechtere Verschnittergebnisse entstehen. Diese höheren Materialverluste lassen sich unter Umständen durch schnelleres Brechen und Abräumen (aufgrund des einfacheren Schneidmodus) kompensieren. Der Schneidmodus bestimmt die Lage der Scheiben innerhalb einer Travere zwischen zwei benachbarten Y- Schnitten. Mögliche Werte:
1. Zwischen zwei Y-Schnitten dürfen Scheiben verschiedener Breite und Höhe nebeneinander liegen. Es können also auch W - Schnitte vorkommen.
2. Zwischen zwei Y-Schnitten dürfen nur Scheiben mit unterschiedlicher Breite aber gleicher Höhe nebeneinander liegen.
3. Zwischen zwei Y-Schnitten dürfen nur Scheiben der gleichen Position nebeneinander liegen.
4. Zwischen zwei Y-Schnitten dürfen höchstens zwei Scheiben der gleichen Position nebeneinander liegen.
5. -7. Spezialmodus für einen Coopmes-Tisch. Dieser Modus ist identisch mit Modus 2-4.

#### Erläuterung der Schaltflächen

**PlanEdit**
Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung durchgeführt haben. Betätigen Sie diese Schaltfläche, öffnet sich das Programm **PlanEdit**.

**Schneiden**
Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung durchgeführt haben. Betätigen Sie diese Schaltfläche, starten Sie den Zuschnitt.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Anzahl der Lagerplatten" auf Seite J-118

---

### Anzahl der Lagerplatten

**Optimierung > Tischoptimierung > Parameter > [Anzahl]**

*(Abb. J-67 Anzahl der Lagerplatten)*

In diesem Dialog sehen Sie die Anzahl der zur Verfügung stehenden Lagerplatten für die gewählte Glasart.

---

### Zurücksetzen eines Zuschnitt Laufes

**Optimierung > Zurücksetzen**

*(Abb. J-68 Zurücksetzen eines Zuschnitt Laufes)*

Mit diesem Dialog können Sie Läufe, die bereits begonnen oder produziert wurden, wieder zurücksetzen und erneut bearbeiten. Tischoptimierungen, die bereits gespeichert wurden, können hier wieder aufgelöst werden. Läufe, die bereits produziert sind aber nicht gebucht wurden, können als produziert gebucht werden. Die Löschroutinen für alte (produzierte) Läufe übernimmt der A+CIMServer. Informationen zum Löschen von Läufen finden Sie in der zugehörigen Dokumentation.

#### Erläuterung der Liste Läufe

**Lauf**
Hier werden die Nummern der Läufe angezeigt, deren Status verändert werden kann. Die Nummern 1000 - 9999 stehen für fertig optimierte Läufe (z. B. aus A+W Production), die zum Schneiden zur Verfügung stehen. Die Nummern 15000 - 19999 (Nummernkreise konfigurierbar) sind für selbst erstellte Tischoptimierungen reserviert.

**Gesperrt**
In dieser Spalte erscheint ein Eintrag, wenn ein anderes A+W Realtime Optimizer oder ein anderer Prozess den entsprechenden Lauf in Bearbeitung hat.

**Status**
Hier wird angezeigt, in welchen Bearbeitungsstand sich die einzelnen Läufe befinden. Folgende Anzeigen sind hier möglich:

| Status | Bedeutung |
| :--- | :--- |
| **Freigegeben** | Es liegt eine Optimierung vor, die zum Zuschnitt freigegeben ist. Solche Läufe können in einer Tischoptimierung weiterbearbeitet werden, bevor der Zuschnitt erfolgt. |
| **Begonnen** | Die Bearbeitung des Laufes wurde begonnen. Es sind Lose aus diesem Lauf bereits beim Zuschnitt oder in einer Tischoptimierung. Auch wenn eine Tischoptimierung nicht geschnitten, sondern wieder aufgelöst wurde, wird dieser Status angezeigt. |
| **Produziert** | Der Lauf wurde produziert. |
*(Tab. J-4 Status der Läufe)*

#### Erläuterung der Schaltflächen

**Produziert**
Wenn ein freigegebener Lauf markiert ist und diese Schaltfläche gewählt wird, dann wird der Lauf als produziert markiert und steht für die Optimierung nicht mehr zur Verfügung.

**OK**
Wenn eine freigegebene Tischoptimierung (Lauf ab Nr. 15000) (konfigurierbar) markiert ist und diese Schaltfläche gewählt wird, dann wird die Tischoptimierung aufgelöst. Die enthaltenen Läufe, Bruchscheiben, Eilscheiben oder Füllscheiben stehen für neue Optimierungen wieder zur Verfügung. Vor der Ausführung dieser Funktion erfolgt eine Sicherheitsabfrage.
Wenn ein produzierter Lauf markiert ist und diese Schaltfläche gewählt wird, dann wird der Lauf zurückgesetzt und kann erneut produziert werden.

**Ergänzende Informationen**
⇨ Tutorial, "Schneidstatus zurücksetzen" auf Seite J-48

---

### Pausierende Glasarten

**Optimierung > DynOpt Einstellungen**

*(Abb. J-69 Pausierende Glasarten)*

Wird ein Lauf in das DynOpt importiert, muss sichergestellt werden, dass es genug Glasplatten dieser Glasart auf Lager gibt. Sie dürfen auf keinen Fall einen Lauf importieren, der die fehlenden Glasarten enthält.
Manchmal kommt jedoch vor, dass Sie erst während der Produktion feststellen, dass einige Glasarten nicht zur Verfügung stehen. Mit diesem Dialog haben Sie jetzt die Möglichkeit, die einzelnen Glasarten zu sperren oder aus der Produktion zu entfernen. Der Dialog zeigt Ihnen alle Glasarten, die sich in der Produktion befinden.

#### Erläuterung der einzelnen Felder

**Filter**
Mithilfe dieser Kombobox können Sie Liste der Glasarten einschränken. Folgende Werte stehen zur Verfügung:
- **Alle:** Es werden alle Glasarten angezeigt, die sich in der Produktion befinden.
- **Gesperrt:** Es werden nur gesperrte Glasarten angezeigt.
- **Dringend:** Es werden nur dringende Glasarten angezeigt. Unter dringend versteht man solche Scheiben dieser Glasart, die vor den DynOpt Ausgangslinien warten.

**Ausgang**
Diese Kombobox ist nur aktiv, wenn Sie in der Kombobox **Filter** die Einstellung **Dringend** gewählt haben. Sie haben dann die Möglichkeit, sich die dringenden Glasarten pro Ausgang anzeigen zu lassen. Hierzu müssen die Ausgänge entsprechend konfiguriert werden.

**Grund für das Pausieren**
Um eine Glasart zu sperren, markieren Sie diese und wählen aus der Kombobox den Grund aus.

**Optimierung stoppen**
Über diese Schaltfläche stoppen Sie die Optimierung. Das ist nötig, wenn Sie eine Glasart komplett aus der Produktion entfernen möchten. Dazu müssen Sie zunächst die Optimierung stoppen und dann die Glasart entfernen.

**Entfernen**
Diese Schaltfläche ist nur aktiv, wenn Sie für eine Glasart die Optimierung gestoppt haben. Anschließend können Sie die Glasart entfernen.

**Sperren**
Über diese Schaltfläche sperren Sie eine Glasart für den nächsten Optimierungsvorgang. Wählen Sie zunächst die Glasart, dann den Grund und klicken Sie dann auf [Sperren].

**Freigeben**
Über diese Schaltfläche geben Sie eine gesperrte Glasart wieder frei. Wählen Sie zunächst die Glasart und klicken Sie dann auf [Freigeben].

**Übersicht**
Mit dieser Schaltfläche öffnen Sie den Dialog **Aktuell geänderte Einstellungen** mit einer Übersicht der jeweiligen Einstellungen.

**Auflösen**
Diese Schaltfläche ist nur aktiv, wenn die Produktion aktiv ist. Dann können Sie über diese Schaltfläche eine neue DynOpt-Optimierung erzwingen.

**Übernehmen**
Über diese Schaltfläche bestätigen Sie die Aktionen. Bsp.: Sie haben eine Glasart gesperrt, dann klicken Sie auf [Übernehmen] um die Aktion abzuschließen.

---

### Aktuell geänderte Einstellungen

**Optimierung > DynOpt Einstellungen > [Übersicht]**

*(Abb. J-70 Aktuell geänderte Einstellungen - Übersicht)*

Dieser Dialog gibt Ihnen eine zusammenfassende Übersicht zu den Einstellungen der Register
- Allgemein
- Eingänge
- Ausgänge
- Puffer

---

# Zuschnitt

## Menü Zuschnitt öffnen

Im Menü **Zuschnitt** befinden sich folgende Programmpunkte:
- **Schneide Optimierung:**
  Über diesen Menüpunkt schneiden Sie einen Lauf.
  ⇨ Softwarereferenz, "Wählen Sie einen Lauf aus" auf Seite J-125
- **Bruchpool:**
  Über diesen Menüpunkt greifen Sie auf den Bruchpool zu.
  ⇨ Softwarereferenz, “Bruchpool" auf Seite J-138
- **Panorama:**
  Über diesen Menüpunkt greifen Sie auf das Panorama zu (optional)

---

## Wählen Sie einen Lauf aus

**Zuschnitt > Schneide Optimierung**

*(Abb. J-71 Wählen Sie einen Lauf aus)*

Mit diesem Dialog wählen Sie einen verfügbaren Lauf aus. Im gewählten Lauf wählen Sie eine oder alle Optimierungen aus. Diese Optimierungen werden dann zum Zuschnitt vorbereitet.

### Erläuterungen der Liste Läufe

**Lauf**
Hier werden die Nummern der Läufe angezeigt, deren Status verändert werden kann. Die Nummern 1000 - 9999 stehen für fertig optimierte Läufe (z. B. aus A+W Production), die zum Schneiden zur Verfügung stehen. Die Nummern 15000-15999 (Nummernkreise konfigurierbar) sind für selbst erstellte Tischoptimierungen reserviert. Befindet sich an dieser Stelle der Begriff **DynOpt Compact**, handelt es sich um einen DynOpt Compact Lauf.

**Status**
Hier wird angezeigt, in welchem Bearbeitungszustand sich die einzelnen Läufe befinden. Folgende Anzeigen sind möglich:

| Status | Bedeutung |
| :--- | :--- |
| **Freigegeben** | Es liegt eine Optimierung vor, die zum Zuschnitt freigegeben ist. Solche Läufe können in einer Tischoptimierung weiterbearbeitet werden, bevor der Zuschnitt erfolgt oder direkt zugeschnitten werden. |
| **Begonnen** | Die Bearbeitung des Laufes wurde begonnen. Es sind Lose aus diesem Lauf bereits beim Zuschnitt oder in einer Tischoptimierung. Auch wenn eine Tischoptimierung nicht geschnitten, sondern wieder aufgelöst wurde, wird dieser Status angezeigt. |
| **Produziert** | Der Lauf wurde produziert. |
*(Tab. J-5 Status der Läufe)*

**Information**
In dieser Spalte werden Ihnen Laufbezeichnung angezeigt.

**Termin**
In dieser Spalte sehen Sie den Produktionstermin, der bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.

**Schicht**
In dieser Spalte sehen Sie die Produktionsschicht, die bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.

> **Sortierung ändern**
> Durch einen Klick auf die Spaltenüberschriften können Sie die Listeninhalte auf- bzw. absteigend sortieren.

### Erläuterungen der Liste Optimierung

**Nr**
Losnummer der in einem Lauf enthaltenen Optimierungen.

**Status**
Hier wird angezeigt, in welchen Bearbeitungszustand sich die einzelnen Optimierungen befinden.

**Glasart**
In diesem Feld sehen Sie die Artikelnummer der Glasart, die in dieser Optimierung enthalten ist. Der Wert dieses Feldes kommt aus den Stammdaten.

**Dicke**
In diesem Feld sehen Sie die Dicke der Glasart, die in dieser Optimierung enthalten ist. Der Wert dieses Feldes kommt aus den Stammdaten.

**Glasart Bezeichnung**
In diesem Feld sehen Sie die Bezeichnung der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Parameter**
Dieses Feld zeigt Ihnen die Bezeichnung des Tisches, für den die Optimierung erzeugt wurde. Der Wert dieses Feldes kommt aus den Stammdaten.

**Platten**
In diesem Feld sehen Sie die Anzahl der benötigten Lagerplatten in dieser Optimierung.

**Verschnitt**
Das Feld zeigt Ihnen die Verschnittglasfläche in %, die bei dieser Optimierung anfällt.

**Rest (mm)**
In diesem Feld sehen Sie die Länge des Restblattes, das nach dem Zuschnitt der Optimierung übrig bleibt.

### Erläuterungen der Felder

**Alte Läufe**
Wenn Sie diese Checkbox markieren, dann werden auch die Läufe angezeigt, die bereits produziert wurden und sich noch im Status Produziert befinden.
- `[ ]` keine Läufe mit dem Status Produziert anzeigen.
- `[x]` nur Läufe mit dem Status Produziert anzeigen.

**Geschnittene Optimierungen ausblenden**
Wenn Sie diese Checkbox markieren, dann werden die bereits geschnittenen Optimierungen nicht angezeigt.
- `[ ]` Geschnittene Optimierungen anzeigen.
- `[x]` Geschnittenen Optimierungen nicht anzeigen.

**Reoptimierung**
Über diese Kombobox steuern Sie Neuoptimierungen. Mögliche Werte sind:
- **Nein:** Es erfolgt keine Neuoptimierung.
- **Ja:** Es erfolgt eine Neuoptimierung ohne Benutzereingriff. Wird eine Optimierung, die nicht für den konfigurierten Tisch optimiert wurde, an den Zuschnitt übergeben, so wird automatisch ohne Dialoganzeige eine Tischoptimierung erstellt und anstelle der originalen Optimierung in den Zuschnittprozess eingefügt.
- **Erweitert:** Neuoptimierung mit Anzeige der vorhandenen Optimierung der zu schneidenden Glasart. Hier können Sie der neu zu optimierenden Optimierung noch weitere Optimierungen für die Tischoptimierung hinzufügen. Die Tischoptimierung kann dann wie gewohnt erstellt werden. Nach erfolgter Optimierung kann die Optimierung verworfen oder über die Schaltfläche [Zuschnitt] an den Zuschnittprozess übergeben werden. Wird die Optimierung verworfen, haben Sie die Möglichkeit, die originale Optimierung zu schneiden oder die Optimierung zu überspringen.
- **Tischoptimierung:** Neuoptimierung mit Anzeige des Dialgos **Tischoptimierung**. Wird eine Optimierung, die nicht für den konfigurierten Tisch optimiert wurde, an den Zuschnitt übergeben, so wird der Dialog **Tischoptimierung** gestartet. Hier können die Optimierungsparameter wie z. B. Randschnitte und Schneidmodus geändert werden. Nach erfolgter Optimierung kann die Optimierung verworfen oder über die Schaltfläche [Zuschnitt] an den Zuschnittprozess übergeben werden. Wird die neue Optimierung verworfen, so haben Sie die Möglichkeit, die originale Optimierung zu schneiden oder die Optimierung zu überspringen.

Wurde die Optimierung versehentlich an den Zuschnitt übergeben, so kann der Zuschnitt beendet und die Tischoptimierung aufgelöst werden. Danach steht die originale Optimierung wieder für den Zuschnitt zur Verfügung.

**Komboboxen**
Die obere Kombobox kennzeichnet den Status der Maschine. Mögliche Werte sind:
- **Bereit:** Am Schneidtisch kann gearbeitet werden.
- **Aus:** Der Schneidtisch ist nicht arbeitsbereit (z. B. bei Pause).

Mit der darunter liegenden Kombobox können Sie entscheiden, welche Läufe angezeigt werden sollen. Mögliche Werte sind:
- **Läufe für den eigenen Tisch:** Zeigt Ihnen nur Zuschnittläufe für den eigenen Schneidtisch an.
- **Läufe für alternative Tische:** Zeigt Ihnen auch die Zuschnittläufe für alternative Schneidtische an.
- **Läufe für alle Tische:** Zeigt Ihnen Läufe für alle Schneidtische an.

**Tischauswahl**
Mithilfe der Kombobox können Sie die Anzeige einschränken. Die Kombobox enthält alle in Ihrem Hause angelegten Tische. Sie können auswählen, ob die Optimierungs-Läufe aller Tische angezeigt werden sollen, oder nur die, die für den Tisch optimiert wurden, der in Ihrer A+W Realtime Optimizer-Installation konfiguriert wurde. Ist das A+W Realtime Optimizer für eine "Tisch-9-Logik" konfiguriert, so steht auch die Auswahl **Alternative Tische** zur Verfügung.

### Erläuterung der Schaltflächen

**Optionen**
Durch Betätigen dieser Schaltfläche werden aus den Optimierungsdaten Zuschnittdaten erzeugt und an den Schneidtisch übertragen. Der Zuschnitt am angeschlossenen Schneidtisch beginnt. Die Anzeige der Schaltfläche wechselt auf STOPP.

**Sortieren**
Diese Schaltfläche ist nur aktiv, wenn für einen Lauf mehr als eine Optimierung gibt. Durch Betätigen dieser Schaltfläche starten Sie den Dialog **Optimierungs-Reihenfolge**.

**Schneiden**
Durch Betätigen dieser Schaltfläche starten Sie den Dialog **Zuschnitt-Übersicht**.

**Ergänzende Informationen**
⇨ Tutorial, "Läufe zum Zuschnitt auswählen" auf Seite J-40
⇨ Tutorial, "Tischansteuerung" auf Seite J-37

---

## Lauf [Nummer] - Lauf [Nummer]

**Zuschnitt > Schneide Optimierung > [OK]**

*(Abb. J-72 Lauf nnn - Lauf mmm)*

In diesem Dialog werden die zuvor im Dialog **Wählen Sie einen Lauf aus** gewählten Läufe und Lose angezeigt und können geschnitten werden.

### Erläuterungen der Liste Optimierungen

⇨ Softwarereferenz, "Erläuterungen der Liste Optimierung" auf Seite J-126

### Erläuterungen der Liste Muster

**Nr.**
Dieses Feld enthält die fortlaufende Nummerierung der Lagerplatten, die in dieser Optimierung verwendet werden. Die Nummern entsprechen der Zuschnittsreihenfolge.

**Breite**
In diesem Feld sehen Sie die Breite der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Höhe**
In diesem Feld sehen Sie die Höhe der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Opt. Gr.**
Hier wird angezeigt, welche Optimierungsgruppen die Lagerplatte mit Scheiben belegen. Es sind nur zwei Gruppen je Lagerplatte möglich. Eine Optimierungsgruppe kann ein Lauf oder eine Nachoptimierung sein.

**Status**
Hier wird der Status der einzelnen Lagerplatten der Optimierung angezeigt. Folgende Stati sind möglich:

| Status | Bedeutung |
| :--- | :--- |
| **Gesendet** | Der Schneidcode wurde erzeugt. |
| **Überspringen** | Für diese Lagerplatte wird kein Schneidcode erzeugt und kein Brechbild zur Verfügung gestellt. |
| **Kein Schneidcode senden** | Für diese Lagerplatte wird kein Schneidcode erzeugt aber ein Brechbild zur Verfügung gestellt. |
| **Geschnitten** | Dieser Status wird gesetzt, wenn der Schneidtisch den Schneidcode empfangen oder abgeholt hat (seriell oder über das Netzwerk). Es findet keine Überprüfung statt, ob die Platte auch tatsächlich geschnitten wurde. |
*(Tab. J-6 Status der Läufe)*

### Erläuterung der Schaltflächen

**Tisch - START**
Durch Betätigen dieser Schaltfläche werden aus den Optimierungsdaten Zuschnittdaten erzeugt und an den Schneidtisch übertragen. Der Zuschnitt am angeschlossenen Schneidtisch beginnt. Die Anzeige der Schaltfläche wechselt auf **STOPP**.

**Tisch - STOPP**
Durch Betätigen dieser Schaltfläche werden keine weiteren Zuschnittdaten an den Schneidtisch übertragen. Der Zuschnitt der aktuellen Lagerplatte am angeschlossenen Schneidtisch wird zu Ende geführt. Die Anzeige der Schaltfläche wechselt auf **START**.

**Muster - Folge**
Durch Betätigen dieser Schaltfläche wird der Dialog **Optimierungsreihenfolge** aufgerufen.

**Muster - Optionen**
Durch Betätigen dieser Schaltfläche wird der Dialog **Lauf: Nummer** aufgerufen.

**XTV - Stopp**
Mit dieser Schaltfläche wird die Kommunikation gestoppt. Das letzte Brechbild bleibt erhalten.

**XTV - <<**
Mit dieser Schaltfläche wird die Brechbildanzeige in einem angeschlossenen XTV zurückgeblättert.

**Beenden**
Mit dieser Schaltfläche wird der Dialog geschlossen. Dies ist jedoch erst dann möglich, wenn keine Schneidcodegenerierung läuft. Wenn eine Schneidcodegenerierung läuft, dann muss diese zuvor mit [STOPP] beendet werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, “Optimierungsreihenfolge" auf Seite J-131
⇨ Softwarereferenz, "Lauf: Nummer" auf Seite J-132
⇨ Tutorial, "Ergebnis der Tischoptimierung prüfen und bearbeiten" auf Seite J-31
⇨ Tutorial, "Tischoptimierungen” auf Seite J-29

---

## Optimierungsreihenfolge

**Zuschnitt > Schneide Optimierung > Optimierung wählen > [Sortieren]**

*(Abb. J-73 Optimierungssreihenfolge)*

Wenn mehrere Glasarten im gewählten Lauf zur Optimierung anstehen, dann wird in diesem Dialog die vorgesehene Reihenfolge der Glasarten angezeigt. Sollten Sie mit der Reihenfolge nicht einverstanden sein, können Sie diese mithilfe der Pfeiltasten ändern.

### Felder

**Status**
In diesem Feld sehen Sie den Status der Optimierung.

**Glasart**
In diesem Feld sehen Sie die Artikelnummer der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Dicke**
In diesem Feld sehen Sie die Dicke der Glasart in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Glasart Bezeichnung**
In diesem Feld sehen Sie die Bezeichnung der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Parameter**
In diesem Feld sehen Sie, auf welchem Schneidtisch die Optimierung geschnitten werden soll.

**Platten**
In diesem Feld sehen Sie, wie viele Lagerplatten die Optimierung benötigt.

**Verschnitt**
In diesem Feld sehen Sie den Verschnitt der Optimierung.

**Rest**
In diesem Feld sehen Sie den Plattenrest.

---

## Lauf: Nummer

**Zuschnitt > Schneide Optimierung > Optimierung auswählen > [Optionen]**

*(Abb. J-74 Restblattbehandlung)*

In diesem Dialog wird u. a. angegeben, was mit den Bruchscheiben und Restblättern jeder Glasart in der ausgewählten Optimierung geschehen kann oder soll.

### Erläuterung der Liste Optimierungen

**Los**
In diesem Feld sehen Sie die Losnummer der angezeigten Glasart in der Optimierung.

**Glasart**
In diesem Feld sehen Sie die Artikelnummer der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Dicke**
In diesem Feld sehen Sie die Dicke der Glasart in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Glasart Bezeichnung**
In diesem Feld sehen Sie die Bezeichnung der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Parameter**
In diesem Feld sehen Sie, für welchen Zuschnitttisch die Optimierung durchgeführt wurde.

**Platten**
Diese Feld zeigt Ihnen die Anzahl der Platten, die für den Zuschnitt dieses Loses benötigt wird.

**Verschnitt**
Das Feld zeigt Ihnen die Verschnittglasfläche in %, die bei dieser Optimierung anfällt.

**Rest (mm)**
In diesem Feld sehen Sie die Länge des Restblattes, das nach dem Zuschnitt der Optimierung übrig bleibt.

### Erläuterung der Liste Platten

**Nr.**
In diesem Feld sehen Sie die Nummer der Lagerplatte, die für die in der Liste **Optimierungen** markierte Optimierung benötigt wird.

**Breite**
In diesem Feld sehen Sie die Breite der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Höhe**
In diesem Feld sehen Sie die Höhe der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Opt. Gr.**
In diesem Feld sehen Sie, welche Optimierungsgruppen die Lagerplatte mit Scheiben belegen. Es sind nur zwei Gruppen je Lagerplatte möglich. Eine Optimierungsgruppe kann ein Lauf oder eine Nachoptimierung sein.

**Schneidstatus**
In diesem Feld wird Ihnen der Schneidstatus der einzelnen Lagerplatten der Optimierung angezeigt. Folgende Stati sind möglich:

| Status | Bedeutung |
| :--- | :--- |
| **Gesendet** | Der Schneidcode wurde erzeugt. |
| **Überspringen** | Für diese Lagerplatte wird kein Schneidcode erzeugt und kein Brechbild zur Verfügung gestellt. |
| **Kein Schneidcode senden** | Für diese Lagerplatte wird kein Schneidcode erzeugt aber ein Brechbild zur Verfügung gestellt. |
| **Geschnitten** | Dieser Status wird gesetzt, wenn der Schneidtisch den Schneidcode empfangen oder abgeholt hat (seriell oder über das Netzwerk). Es findet keine Überprüfung statt, ob die Platte auch tatsächlich geschnitten wurde. |
*(Tab. J-7 Schneidstatus der Läufe)*

### Erläuterung der Felder im Bereich Bruchscheibenoptimierung

**Optimiere Bruchscheiben**
Hier stellen Sie ein, wie A+W Realtime Optimizer mit Bruchscheiben umgehen soll, die an den Zuschnitt übergeben werden. Folgende Einstellungen sind möglich:
- **Nein:** Es erfolgt keine Nachoptimierung.
- **Trennen:** Die neu erstellte Nachoptimierung wird am Ende der vorhandenen Optimierung angefügt. Dadurch entsteht zwangsläufig ein Traverenschnitt zwischen der vorhandenen Optimierung und dem neu erstellten Teil.
- **Mischen:** Das letzte Lagerblatt wird komplett neu optimiert. Das führt in den meisten Fällen zu einer Verschnittverbesserung.

**Schneide Bruchscheiben nach Restblattlänge**
Mit dieser Checkbox wird festgelegt, ob die Bruchscheiben auch auf ein neues Restblatt optimiert werden sollen, wenn das bisherige Restblatt dafür nicht ausreicht. Wenn diese Checkbox markiert ist, dann ist der Eintrag im nachfolgenden Feld von Bedeutung.
- `[ ]` Keine neue Lagerplatte für den Zuschnitt von Bruchscheiben beginnen.
- `[x]` Eine neue Lagerplatte für den Zuschnitt beginnen, wenn das neu entstandene Restblatt kleiner ist als die im nachfolgendem Feld Länge angegebene neue Restblattlänge.

**Schneide Restblatt unter einer Länge von**
Dieses Feld ist nur aktiv, wenn die vorherige Checkbox markiert wurde. Geben Sie hier an, wie groß das neu entstandene Restblatt höchstens sein darf. Wenn die Nachoptimierung ein größeres Restblatt erzeugt, wird kein neues Restblatt begonnen. Die Bruchscheiben werden im Bruchpool gesammelt.

### Erläuterung der Felder im Bereich Restblattverwaltung

**Verlinken**
Hier stellen Sie ein, wie A+W Realtime Optimizer mit Restblätter umgehen soll. Folgende Einstellungen sind möglich:
- **Nein:** Es erfolgt keine Verlinkung.
- **Trennen:** Die neu erstellte Nachoptimierung wird am Ende der vorhandenen Optimierung angefügt. Dadurch entsteht zwangsläufig ein Traverenschnitt zwischen der vorhandenen Optimierung und dem neu erstellten Teil.
- **Mischen:** Die Scheiben werden auf dem Restblatt aufgelöst und mit der zu optimierenden Menge neu optimiert.

**Restblatt vor dem Schneiden bearbeiten**
Wenn diese Checkbox markiert ist, erfolgt eine Abfrage, ob PlanEdit gestartet werden soll.

### Erläuterung der Felder im Bereich Schnelloptimierung

**Schnelloptimierung**
- **Standard:** In diesem Modus können Sie während des Zuschnittprozesses die Muster einer Glasart, für die noch kein Schneidcode übertragen wurde, auflösen und neu optimieren. Der Sinn ist, dass bei Optimierungen mit vielen Mustern die Bruchscheiben nicht erst auf das letzte Blatt optimiert werden. Die Bruchscheiben kommen in der neuen Optimierung am Anfang (ohne weiteren Benutzereingriff).
- **Erweitert:** In diesem Modus sind weitere Benutzereingaben nötig. Es wird automatisch das Glasauswahlmenü für die Tischoptimierung geöffnet. Dort ist aber nur die Glasart der aufgelösten Optimierung zu sehen. Hier können Sie noch weitere Optimierungen hinzufügen. Anschließend öffnet sich der Dialog Tischoptimierung. Dort können z. B. Ränder geändert werden. Wenn fertig optimiert ist, kann die Optimierung über die Schaltfläche [Schneiden] direkt wieder an den Zuschnittprozess übergeben werden.

**Nachladen**
Über diese Einstellung können Sie einen weiteren Lauf laden. Folgende Einstellungen sind möglich:
- **Manuell:** Das Nachladen erfolgt manuell.
- **Anforderung:** Es wird eine Meldung angezeigt, sobald im A+W Realtime Optimizer eine konfigurierbare Anzahl noch nicht geschnittener Muster unterschritten wird. Sie können dann das Nachladen ablehnen oder im Lauf-auswahlmenü einen neuen Lauf laden.
- **Automatisch:** Das Nachladen erfolgt automatisch.

### Erläuterung der Felder im Bereich Etikettendruck

**Aktiv**
Über diese Checkbox können Sie den Etikettendruck aktivieren bzw. deaktivieren.
- `[ ]` Der Etikettendruck ist deaktiviert.
- `[x]` Der Etikettendruck ist aktiviert. Sie können Etiketten direkt drucken.

### Erläuterung der Schaltflächen

**PlanEdit**
Wenn Sie diese Schaltfläche wählen und das Modul PlanEdit bei Ihnen installiert ist, dann startet PlanEdit und zeigt die Optimierung grafisch an.

**Schneiden**
Wenn Sie diese Schaltfläche wählen, startet die Zuschnitt-Übersicht.

### Erläuterung des Kontextmenüs

Durch Klicken mit der rechten Maustaste auf eine Platte mit dem Status **Geschnitten** kann der Status **Geschnitten** gelöscht und die Platte erneut geschnitten werden.

Durch Klicken mit der rechten Maustaste auf eine Platte ohne Status kann der Status **Kein Schneidcode senden** oder **Überspringen** für die gewählte Platte gesetzt werden.

**Ergänzende Informationen**
⇨ Tutorial, "A+W Pattern Viewer" auf Seite J-59
⇨ Tutorial, “A+W Residual Stock Manager" auf Seite J-50

---

## Auswahl der zu verlinkenden Optimierung

**Zuschnitt > Schneide Optimierung > Lauf auswählen > [OK] > Dialog Aktiver Lauf: xxx wird geöffnet > Optimierung auswählen > [Start]**

*(Abb. J-75 Auswahl der zu verlinkenden Optimierung)*

Die Liste **Verfügbare Optimierungen** enthält alle Läufe, in denen Optimierungen für die gewählte Glasart und Dicke enthalten sind. Im Kopf des Dialoges wird Ihnen der ausgewählte Lauf, das Los und die Glasart angezeigt. Wählen Sie aus der Tabelle den Lauf aus, den Sie verlinken möchten und betätigen Sie anschließend [Verwenden].

### Erläuterung der Felder im Bereich Auswahl-Parameter und Restblatt

**Alle Tische**
Mit dieser Checkbox steuern Sie, welche Optimierungen angezeigt werden. Ist die Checkbox aktiv, werden hier auch Optimierungen angezeigt, die für andere Tische bestimmt sind.

**Erlaube Handzuschnitt**
Wenn diese Checkbox markiert ist, dann werden in der Liste **Verfügbare Optimierungen** auch die Glasarten angezeigt, die bei der Artikeldefinition in den Stammdaten nur für Handzuschnitt vorgesehen wurden.

**Restblatt**
In diesem Feld sehen Sie, wie lange das Restblatt ist, dass bei der gewählten Optimierung (Dialog Aktiver Lauf: xxx) übrig bleibt.

---

## Optimierungsergebnis

**Zuschnitt > Schneide Optimierung > Lauf auswählen > [OK] > Dialog Aktiver Lauf: xxx wird geöffnet > Optimierung auswählen > [Start] > Lauf auswählen > [Verlinken]**

*(Abb. J-76 Optimierungsergebnis)*

Dieser Dialog zeigt Ihnen das Optimierungsergebnis nach dem Verlinken. Er ist in zwei Bereiche unterteilt. Im Bereich **Neue Optimierung nach dem Verlinken** sehen Sie das Ergebnis nach dem Verlinken. Der Bereich **Original-Optimierung** zeigt Ihnen das Ergebnis vor dem Verlinken bzw. ohne ein Verlinken.

In dem grauen Bereich oberhalb der Schaltflächen sehen Sie, was und wie viel zusätzlich optimiert wurde.

### Erläuterung der Schaltflächen

**Wiederholen**
Wenn Sie diese Schaltfläche betätigen, kehren Sie zurück zur Auswahl der Linkoptimierung, wo Sie einen Lauf auswählen können.
⇨ Softwarereferenz, "Auswahl der zu verlinkenden Optimierung" auf Seite J-136

**Verlinken**
Wenn Sie diese Schaltfläche betätigen, bestätigen Sie das Ergebnis und die Optimierung wird geschnitten.

---

## Bruchpool

**Zuschnitt > Bruchpool**

*(Abb. J-77 Bruchpool)*

Dieser Dialog zeigt alle Scheiben an, die als Bruch gemeldet oder erfasst wurden. Scheiben aus dem Bruchpool können bei passender Glasart und Dicke bei Tischoptimierungen und in der Nachoptimierung erneut optimiert werden.

### Erläuterung der Liste Bruchscheiben

**Glasart**
In diesem Feld sehen Sie die Artikelnummer der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Bezeichnung**
In diesem Feld sehen Sie die Bezeichnung der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Dicke**
In diesem Feld sehen Sie die Dicke der Glasart in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Breite**
In diesem Feld sehen Sie die Breite der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Höhe**
In diesem Feld sehen Sie die Höhe der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

**Lauf**
In diesem Feld sehen Sie die Laufnummer, zu der die Scheibe ursprünglich gehörte.

**Dynopt**
Mit diesem Feld haben Sie die Möglichkeit, für einzelne Bruchscheiben ein DynOpt-Flag zu setzen, sodass diese vom DynOpt reoptimiert werden können. Wählen Sie dazu den bzw. die entsprechenden Scheiben aus und klicken Sie anschließend auf die Schaltfläche DynOpt. Es können nur Scheiben ausgewählt werden, für die keine Sperrstation eingetragen ist.

**Kunde**
In diesem Feld ist der Name des Kunden angegeben, zu dem die Bruchscheibe gehört.

**Auftrag**
In diesem Feld ist die Nummer des Auftrags angegeben, zu dem die Bruchscheibe gehört.

**Pos**
In diesem Feld ist die Positionsnummer des Auftrags angegeben, zu dem die Bruchscheibe gehört.

**Menge**
In diesem Feld sehen Sie die Anzahl der Scheiben.

**FormNr.**
Wenn es sich bei der Bruchscheibe um ein Modell handelt, dann wird Ihnen in diesem Feld die Modellnummer angezeigt.

**Bock**
In diesem Feld sehen Sie die Nummer des Abstellplatzes (Bock oder Fächerwagen), auf dem die Scheibe hätte stehen sollen, wenn sie nicht zu Bruch gegangen wäre.

**Etikett-Nr.**
In diesem Feld sehen Sie die Etikett-Nummer der Bruchscheibe.

**Los**
Dieses Feld wird nur programm-intern verwendet und hat keine Aussagekraft.

### Erläuterung der Schaltflächen

**Aktualisieren**
Wenn während der Arbeit mit diesem Dialog weitere Bruchscheiben gemeldet werden (z. B. via A+W Production Terminal XTV), dann werden diese erst dann angezeigt, wenn die Anzeige im Dialog mit dieser Schaltfläche aktualisiert wird.

**Löschen**
Mit dem Betätigen dieser Schaltfläche wird die markierte Bruchscheibe aus dem Bruchpool gelöscht. Es können auch mehrere Scheiben gleichzeitig markiert und gelöscht werden. Arbeiten Sie mit einer BDE, haben Sie die Möglichkeit, die Scheiben zu buchen.

**Modell-Info**
Mit dieser Schaltfläche wird die Modellscheibenanzeige von A+W Production gestartet.

**Drucken**
Mit dieser Schaltfläche wird ein Ausdruck gestartet, in dem alle Bruchscheiben des Bruchpools aufgelistet werden. Diese Schaltfläche steht nur dann zur Verfügung, wenn dies im System konfiguriert wurde.

**Hinzufügen**
Mit dieser Schaltfläche wird der Dialog Brucherfassung aufgerufen.

### Erläuterung der Kombobox

Mithilfe der Kombobox können Sie auswählen, zu welchem Tisch der Bruch, den Sie hinzufügen möchten, gebucht werden soll.

Öffnen Sie den Bruchpool zum ersten Mal, ist als Standard der Tisch ausgewählt, an dem der A+W Realtime Optimizer hängt.

**Ergänzende Informationen**
⇨ Tutorial, "Bruch, Eilscheiben und Füllaufträge" auf Seite J-21
⇨ Softwarereferenz, “Form-Erfassung" auf Seite J-94
⇨ Softwarereferenz, "Brucherfassung" auf Seite J-141

---

## Brucherfassung

**Zuschnitt > Bruchpool > [Hinzufügen]**

*(Abb. J-78 Brucherfassung)*

Mit diesem Dialog können Sie Scheiben erfassen, die zu Bruch gegangen sind und nochmals in eine Optimierung aufgenommen werden sollen.

### Erläuterung der Felder

**Auftrag**
In diesem Feld erfassen Sie die Auftragsnummer, zu der die Bruchscheibe gehört.

**Position**
In diesem Feld geben Sie Positionsnummer des Auftrags ein, zu dem die Bruchscheibe gehört.

**Bruchgrund**
Wählen Sie aus der Kombobox den Bruchgrund der Scheiben. Bruchgründe, die hier ausgewählt werden können, müssen in den Stammdaten definiert worden sein.

### Erläuterung der Liste Teile

**AuftNr**
In diesem Feld sehen Sie die Auftragsnummer, zu der die Bruchscheibe gehört.

**TeileNr**
In diesem Feld sehen Sie die Teilenummer der Scheibe.

**Bezeichnung**
In diesem Feld sehen Sie die Bezeichnung der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.

**Breite**
In diesem Feld sehen Sie die Breite der Glasart in mm oder inch (konfigurierbar).

**Höhe**
In diesem Feld sehen Sie die Höhe der Glasart in mm oder inch (konfigurierbar).

### Suchfelder

**Zuschnitt > Bruchpool > [Hinzufügen] > <Strg> + <F12>**

*(Abb. J-79 Suchfelder)*

Im Dialog **Brucherfassung** können bis zu drei frei konfigurierbare Suchfelder hinzugefügt werden. Es handelt sich dabei um die Felder **Searchfield1**, **Searchfield2** und **Searchfield3**. Die Felder werden über die Formadministration hinzugefügt:
- **Control with action:** Entry can freely be defined
- **Selected part:** Searchfield1, ...
- **Action:** Kombobox Searchfield1, ...

Sollten Sie sich nicht mit dieser Technologie auskennen, wenden Sie sich bitte an einen A+W-Mitarbeiter.

**Ergänzende Informationen**
⇨ Tutorial, "Bruch, Eilscheiben und Füllaufträge" auf Seite J-21

---

## Modell-Erfassung

**Zuschnitt > Bruchpool > [Modell-Info]**

*(Abb. J-80 Form-Erfassung)*

Die Felder und Schaltflächen diesen Dialoges sind identisch mit den Feldern und Schaltflächen des Dialoges **Form-Erfassung** im Bereich der Eilscheiben. Der Dialog wird an dieser Stelle erläutert.
A. Benötigten Eingaben pro Modell
B. Modell-Nummern
C. Grafische Modell-Übersicht
D. Modellvorschaufenster
E. Parameterübersicht
F. Eingabefeld

**Ergänzende Informationen**
⇨ Softwarereferenz, "Form-Erfassung" auf Seite J-94

---

## A+W DynOpt - Editor

**Zuschnitt > DynOpt Compact ...**

*(Abb. J-81 Editor)*

Der Editor zeigt Ihnen auf der linken Seite im Bereich **Freigegebene Läufe** alle Feinplanungs-Läufe, die mit DynOpt Compact verarbeitet werden können.

### Erläuterung der Felder im Bereich Freigegebene Läufe

**Lauf**
In diesem Feld sehen Sie die Laufnummer der Feinplanung.

**Text**
In diesem Feld sehen Sie den Namen der Laufnummer.
Der Bereich **Importierte Läufe** zeigt Ihnen die Läufe, die bereits optimiert oder importiert wurden. Durch das Aufklappen der Baumstruktur können Sie sich nähere Informationen zu dem jeweiligen Lauf anzeigen lassen. Die Baumstruktur zeigt Ihnen in der ersten Ebene die Laufnummer, in der zweiten Ebene die Abstellplatznummer und in der dritten Ebene den Status, die Anzahl der Scheiben und die Art des Abstellplatzes. Klicken Sie mit der Maus die zweite Ebene (Abstellplatznummer) der Baumstruktur an, zeigt Ihnen die Liste **Importierte Scheiben** Detailinformationen zu jeder einzelnen Scheibe.

### Erläuterung der Schaltflächen

**>**
Mit dieser Schaltfläche verschieben Sie einen markierten Lauf aus dem Bereich **Freigegebene Läufe** in den Bereich **Importierte Läufe**.

**<**
Mit dieser Schaltfläche verschieben Sie einen markierten Lauf aus dem Bereich **Importierte Läufe** wieder zurück in den Bereich **Freigegebene Läufe**.

**^**
Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie im Bereich **Freigegebene Läufe** einen Lauf gewählt und betätigen dann die Schaltfläche ^, rückt der Lauf in der Liste eine Stelle weiter noch oben.

**v**
Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie im Bereich **Freigegebene Läufe** einen Lauf gewählt und betätigen dann die Schaltfläche v, rückt der Lauf in der Liste eine Stelle weiter noch unten.

### Erläuterung der Felder im Bereich Importierte Scheiben

**Lauf**
In diesem Feld sehen Sie die Laufnummer der Feinplanung.

**Sequenzlauf**
In diesem Feld wird der Sequenzlauf des Gestells angezeigt. Es handelt sich hierbei um eine laufende Nummer der importierten Gestelle innerhalb des Laufes.

**Laufende Nr.**
In diesem Feld wird in aufsteigender Reihenfolge die laufende Nummer innerhalb des Laufes angezeigt.

**Fach Nr.**
Wenn es sich bei dem Abstellplatz um einen Fächerwagen handelt, wird in diesem Feld die Fachnummer angezeigt. Bei A-Böcken steht hier 0.

**Glasart**
In diesem Feld wird die Artikelnummer der Glasart angezeigt.

**Dicke**
In diesem Feld wird die Dicke der Scheibe in mm oder inch (konfigurierbar) angezeigt.

**Breite**
In diesem Feld wird die Breite der Scheibe in mm oder inch (konfigurierbar) angezeigt.

**Höhe**
In diesem Feld wird die Höhe der Scheibe in mm oder inch (konfigurierbar) angezeigt.

**Auftrag**
In diesem Feld wird die Auftragsnummer angezeigt.

**Pos**
In diesem Feld wird die Positionsnummer des Auftrags angezeigt.

**Status**
In diesem Feld wird der Status angezeigt. Nähere Erläuterungen finden Sie weiter unten.

**DynOpt Compact Lauf**
In diesem Feld sehen Sie die Laufnummer der DynOpt Compact Optimierung.

**DynOpt Compact Los**
In diesem Feld sehen Sie die Losnummer der DynOpt Compact Optimierung.

**DynOpt Compact Muster**
In diesem Feld wird die Nummer des Musters angezeigt, auf dem die einzelne Scheibe liegt.

Markieren Sie im linken Bereich einen Lauf, finden Sie entsprechende Detail-Informationen bezüglich der einzelnen Scheiben dazu im linken Fenster.

Im unteren Bereich des Dialogs wird Ihnen eine Zeitleiste angezeigt. Jedes farbige Rechteck kennzeichnet den Zustand eines entsprechenden Abstellplatzes.

Folgende Farben sind möglich:

| Farbe (Symbol) | Erläuterung |
| :--- | :--- |
| 🟦 (Blau) | Alle Scheiben des Gestells wurden geschnitten. |
| 🟦 (Blau) | Alle Scheiben des Gestells wurden optimiert. |
| 🟨 (Gelb) | Scheiben des Gestells wurden teilweise optimiert. |
| 🟩 (Grün) | Das Gestell wurde noch nicht optimiert. |
*(Tab. J-8 Erläuterung der Symbole)*

Die Zahlen unter dem farbigen Rechteck zeigen Ihnen die Lauf- und Abstellplatznummer. Beispiel: 1187/9951 bedeutet, Laufnummer 1187 und die Abstellplatznummer 9951.

### Erläuterung der Felder

**Status**
Die Kombobox enthält die für DynOpt Compact relevanten Stati. Mögliche Werte:
- **0:** Unbearbeitet
- **100:** Komplette Abstellplätze, die jedoch nur teilweise optimiert wurden.
- **200:** Optimiert.
- **300:** Geschnitten.
- **500:** Sollten während der Optimierung Fehler aufgetreten sein, bekommen diese Scheiben den Status 500. Darüber hinaus werden Sie im rechten Bereich des Editors in einem roten Balken dargestellt.

**Zeitleisten-Darstellung**
Mit der Zeitleisten-Darstellung bestimmen Sie die Art der Ansicht. Sie können sich den Editor für den Zuschnitt und für die Optimierung darstellen lassen.

### Erläuterung der Schaltflächen

**Aktualisieren**
Mithilfe dieser Schaltfläche aktualisieren Sie den Editor.

> **Bilden von DynOpt Compact-Läufen**
> Sie können DynOpt Compact-Läufe aus dem Editor heraus bilden, aber auch aus dem Zuschnitt heraus. Im Editor können Sie einen oder mehrere Läufe markieren und über das Kontext-Menü die Funktion **DynOpt Compact-Lauf erzeugen** wählen. Im Zuschnitt können Sie das immer nur für einen Lauf tun.

**Ergänzende Informationen**
⇨ Tutorial, “A+W DynOpt Compact" auf Seite J-81

---

# Einstellungen

## Menü Einstellungen öffnen

Im Menü **Einstellungen** befindet sich folgender Programmpunkt:
- **Tische**
  Über diesen Menüpunkt greifen Sie auf die konfigurierten Tische zu.
  ⇨ Softwarereferenz, "Einstellungen" auf Seite J-149
- **Tischoptimierung**
  Über diesen Menüpunkt greifen Sie auf die Tischoptimierung zu.
  ⇨ Softwarereferenz, “Tischoptimierung" auf Seite J-151

---

## Einstellungen > Tische

*(Abb. J-82 Tische)*

Dieser Dialog steht Ihnen für alle konfigurierten Tische zur Verfügung.
Er bietet die Möglichkeit, zur Laufzeit Einstellungen zu ändern, die sonst nur über die Konfigurationsdatei (xopton.cfg) angepasst werden können. Somit muss der A+W Realtime Optimizer nicht beendet und anschließend neu gestartet werden.

### Erläuterung der Felder im Bereich Restplattenlager

**Aktiv**
Die Checkbox steuert, ob das Restplattenlager verwendet wird oder nicht.
- `[x]` Das Restplattenlager wird verwendet.
- `[ ]` Das Restplattenlager wird nicht verwendet.

**Platten einlagern**
Die Checkbox steuert, ob Restplatten in das Restplattenlager gefahren werden oder nicht.
- `[x]` Restplatten werden in das Restplattenlager gefahren.
- `[ ]` Restplatten werden nicht in das Restplattenlager gefahren.

**Platten verwenden**
Die Checkbox steuert, ob die Optimierung die Restplatten aus dem Restplattenlager verwendet oder nicht.
- `[x]` Restplatten aus dem Restplattenlager werden verwendet.
- `[ ]` Restplatten aus dem Restplattenlager werden nicht verwendet.

**Mindesteinlagerungslänge**
In diesem Feld geben Sie die Mindestlänge in mm ein, ab der ein Rest eingelagert wird.

### Erläuterung der Felder im Bereich Zuschnitt

**Aktiv**
Die Checkbox steuert den Etikettendruck während des Zuschnitts.
- `[x]` Etiketten werden während des Zuschnitts gedruckt.
- `[ ]` Etiketten werden nicht gedruckt.

**Restblatt editieren**
In diesem Feld geben Sie die Mindestlänge eines Restblatts in mm ein, damit während des Zuschnitts mit PlanEdit editiert werden kann.

### Erläuterung der Schaltflächen

**Übernehmen**
Wenn Sie diese Schaltfläche betätigen, werden die Änderungen übernommen.

**Verwerfen**
Wenn Sie diese Schaltfläche betätigen, werden die Änderungen verworfen.
