---
description: "D-AWProduction-HB_13"
---


# A+W Realtime Optimizer Softwarereferenz

---
## Erfassung

Im Menü **Erfassung** befinden sich folgende Programmpunkte:

- **Eilscheiben:**
  Über diesen Menüpunkt können Sie Eilscheiben direkt im Realtime Optimizer erfassen.
  ⇨ Softwarereferenz, "Eilscheiben-Eingabe" auf Seite J-1146

- **Manueller Plan:**
  Über diesen Menüpunkt können Sie einen rein manuellen Plan erstellen und als Tischoptimierung in der Datenbank speichern.
  ⇨ Softwarereferenz, "Manuelle Planerstellung" auf Seite J-1151

- **Stammdaten:**
  Über diesen Menüpunkt haben Sie Zugriff auf die Stammdaten. Diese sind im Handbuch A+W Production detailliert beschrieben.

### Eilscheiben

**Erfassung > Eilscheiben**

Eilscheiben können in die Tischoptimierung mit einbezogen werden. Dieser Dialog zeigt Ihnen alle bereits erfassten Eilscheiben. Über die Kombobox für das Feld **Tisch** haben Sie die Möglichkeit, sich die Eilscheiben pro Tisch oder aber für alle Tische anzeigen zu lassen. Nähere Erläuterungen zu Eilscheiben finden Sie im Part Feinplanung.

*(Abbildung J-55 zeigt den Dialog "Eilscheiben" mit einer Tabelle, die Spalten wie Glasart, Dicke, Bock, Menge, Form Nr., Breite, Höhe, und Prio enthält. Unter der Tabelle gibt es Optionen zum Filtern nach "Alle Stationen" oder einem spezifischen "Tisch" sowie Schaltflächen zum Aktualisieren, Hinzufügen, Bearbeiten, Löschen und Bestätigen.)*

#### Erläuterung der Felder

- **Glasart**: In diesem Feld wird die Artikelnummer der Glasart angezeigt. Der Wert kommt aus dem Feld **Glasart** des Dialoges Eilscheiben-Eingabe.
- **Dicke**: In diesem Feld wird die Dicke der Glasart angezeigt. Der Wert kommt aus dem Feld **Dicke** des Dialoges Eilscheiben-Eingabe.
- **Bock**: In diesem Feld wird die Abstellplatznummer angezeigt. Der Wert kommt aus dem Feld **Bock** des Dialoges Eilscheiben-Eingabe.
- **Menge**: In diesem Feld wird die Eilscheibenmenge angezeigt. Der Wert kommt aus dem Feld **Menge** des Dialoges Eilscheiben-Eingabe.
- **Form**: Wenn es sich bei der Eilscheibe um ein Modell handelt, wird in diesem Feld die Modellnummer angezeigt. Steht in dem Feld eine 0, ist die Eilscheibe kein Modell. Der Wert kommt aus dem Feld **Form** des Dialoges Eilscheiben-Eingabe.
- **Breite**: In diesem Feld wird die Breite der Eilscheibe angezeigt. Der Wert kommt aus dem Feld **Breite** des Dialoges Eilscheiben-Eingabe.
- **Höhe**: In diesem Feld wird die Höhe der Eilscheibe angezeigt. Der Wert kommt aus dem Feld **Höhe** des Dialoges Eilscheiben-Eingabe.
- **Prio**: In diesem Feld wird die beim Erzeugen der Eilscheibe gewählte Priorität angezeigt. Die Standardpriorität ist 0.
- **Alle Stationen**: Mit dieser Checkbox steuern Sie, welche Eilscheiben angezeigt werden. Normalerweise werden nur die Eilscheiben angezeigt, die mit der eigenen Arbeitsstation angelegt worden sind um diese zu bearbeiten oder zu löschen. Damit wird verhindert, dass andere Arbeitsstation diese Datensätze verändern oder gar löschen. Wollen Sie sich jedoch darüber informieren, welche Eilscheiben es insgesamt in der Datenbank gibt, so können Sie diese Checkbox aktivieren und bekommen eine Übersicht über alle vorhandenen Eilscheiben. Eilscheiben, die von anderen Arbeitsstation erfasst wurden, werden farblich gekennzeichnet und im Info-Fenster unterhalb der Checkbox Alle Stationen angezeigt.
  - ☑ Es werden alle erfassten Eilscheiben angezeigt. Auch die, die an anderen Arbeitsstationen erfasst wurden.
  - ☐ Es werden nur die Eilscheiben angezeigt, die an der eigenen Arbeitsstation erfasst wurden.
  > **Technische Info:** Datenbankfeld: `FEIN_TEILE:STATIONID`
- **Tisch**: Die Kombobox enthält alle in Ihrem Hause angelegten Schneidtische. Somit haben Sie die Möglichkeit, Eilscheiben gezielt für einen bestimmten Schneidtisch zu erfassen. Mithilfe der Auswahl **Alle Tische** verschaffen Sie sich einen Überblick über alle erfassten Eilscheiben. Markieren Sie anschließend einen Datensatz in der Liste, erscheint im grauen Bereich unterhalb der Checkbox Alle Stationen der Tisch, auf dem Eilscheibe geschnitten werden soll.

#### Erläuterung der Schaltflächen

- **Hinzufügen**: Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog **Eilscheiben-Eingabe**.
- **Bearbeiten**: Wenn Sie diese Schaltfläche betätigen, öffnet sich für einen markierten Datensatz der Dialog **Eilscheiben-Eingabe**.
- **Löschen**: Über diese Schaltfläche löschen Sie eine zuvor markierte Eilscheibe. Es folgt eine Sicherheitsabfrage. Anschließend wird der Eintrag gelöscht.

#### Ergänzende Informationen
- ⇨ Tutorial, "Bruch, Eilscheiben und Füllaufträge" auf Seite J-1075
- ⇨ Softwarereferenz, "Form" auf Seite J-1146
- ⇨ Softwarereferenz, "Eilscheiben-Eingabe" auf Seite J-1146

### Eilscheiben-Eingabe

**Erfassung > Eilscheiben > [Hinzufügen]**

In diesem Dialog haben Sie die Möglichkeit, Eilscheiben zu erfassen. Nähere Erläuterungen zu Eilscheiben finden Sie im Part Feinplanung.

*(Abbildung J-56 zeigt den Dialog "Eilscheiben-Eingabe" mit Feldern für Glasart, Dicke, Bock, Menge, Modell-Nr., Breite und Höhe.)*

> **Technische Info:** Datenbanktabelle: `FEIN_TEILE`

#### Erläuterung der Felder

- **Glasart**: Die Kombobox listet alle in Ihrem Hause angelegten Glasarten. Wählen Sie aus der Kombobox die entsprechende Glasart aus. Die Glasarten werden in den Stammdaten angelegt.
  > **Technische Info:** Pflichtfeld, Datenbankfeld: `POOL_TEILE:GLASART`
- **Dicke**: Die Kombobox listet alle in Ihrem Hause angelegten Dicken zu der im Feld **Glasart** gewählten Glasart. Wählen Sie aus der Kombobox den entsprechenden Dicke aus. Die Dicken werden in den Stammdaten angelegt.
  > **Technische Info:** Pflichtfeld, Datenbankfeld: `POOL_TEILE:DICKE`
- **Bock**: In diesem Feld geben Sie die Abstellplatznummer ein, auf den die Eilscheibe gestellt werden soll. Die Abstellplätze werden in den Stammdaten angelegt.
  > **Technische Info:** Pflichtfeld, 4stellig, Datenbankfeld: `FEIN_TEILE:BOCK`
- **Menge**: In diesem Feld geben Sie die Menge der Eilscheiben ein.
  > **Technische Info:** Pflichtfeld, Datenbankfeld: `FEIN TEILE:MENGE`
- **Form**: Wenn es sich bei der Eilscheibe um ein Modell handelt, geben Sie in diesem Feld die vordefinierte Modell-Nr. (Modell-Katalog) ein. Haben Sie die Modell-Nr. eingegeben und verlassen das Feld, öffnet sich automatisch der Dialog **Form-Erfassung**.
  > **Technische Info:** Pflichtfeld, Datenbankfeld: `POOL_MODELL:MODELL_NR`
- **Breite**: In diesem Feld geben Sie die Breite der Eilscheibe ein. Handelt es sich bei der Eilscheibe um ein Modell, ist die Breite die, des umschreibenden Rechtecks.
  > **Technische Info:** Pflichtfeld, Datenbankfeld: `POOL_MODELL:BREITE`
- **Höhe**: In diesem Feld geben Sie die Höhe der Eilscheibe ein. Handelt es sich bei der Eilscheibe um ein Modell, ist die Höhe die, des umschreibenden Rechtecks.
  > **Technische Info:** Pflichtfeld, Datenbankfeld: `POOL_MODELL:HOEHE`

#### Erläuterung der Schaltflächen

- **Lupe**: Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog **Form-Erfassung**.

#### Ergänzende Informationen
- ⇨ Softwarereferenz, "Form-Erfassung" auf Seite J-1148
- ⇨ Feinplanung: Softwarereferenz, "Abstellplätze" auf Seite D-372
- ⇨ Tutorial, "Bruch, Eilscheiben und Füllaufträge" auf Seite J-1075

### Form-Erfassung

**Erfassung > Eilscheiben > [Hinzufügen] > [Lupe]**

*(Abbildung J-57 zeigt den Dialog "Form-Erfassung". Er ist in mehrere Bereiche unterteilt: A) Benötigte Eingaben, B) Modell-Nummern, C) Grafische Modell-Übersicht, D) Modellvorschaufenster, E) Parameterübersicht, F) Eingabefeld.)*

Dieser Dialog dient zur Erfassung von vordefinierten Modellen. Die mögliche Auswahl hängt vom Umfang des benutzten Modellkataloges ab. Die benötigten Eingaben für das gewählte Modell entnehmen Sie dem Fenster oben links (A) in dem Dialog. Ihre Eingaben werden sofort in dem Fenster rechts (D) in dem Dialog umgesetzt, das Modell proportional dargestellt. Das untere Fenster (E) dient zur Veranschaulichung der Eingabeparameter.

Die Werte vor den benötigten Eingaben für das gewählte Modell haben folgende Bedeutung:

| Wert | Erläuterung |
| :--- | :--- |
| **W** | Breite des Modells. Bei mehreren Breiten = W, W1, W2, etc. |
| **H** | Höhe des Modells. Bei mehreren Höhen = H, H1, H2, etc. |
| **T** | Trims. Bei mehreren Trims = T, T1, T2, etc. |
| **<-->** | Spiegelflag. Mögliche Werte: 0: Normal, 1: Um die Senkrechte gespiegelt. |
| **@** | Drehflag. Mögliche Werte: 90: Drehen um 90°, 180: Drehen um 180°, 270: Drehen um 270°. |

### Modell-Nummer

**Erfassung > Eilscheiben > [Hinzufügen] > [Lupe] > [Lupe]**

*(Abbildung J-58 zeigt den Dialog "Modell-Nummer" mit einer Gitteransicht verschiedener nummerierter Glasformen.)*

Wenn Sie die zur Erfassung benötigte Modell-Nummer nicht kennen, und auch keinen Modell-Katalog in gedruckter Ausgabe zur Hand haben, können Sie sich in diesem Dialog einen Überblick zu den vorhanden Modellen verschaffen. Die Nummer des Modells aus der Form-Erfassung ist mit Punkten unterlegt. Im oben abgebildeten Dialog ist das Modell-Nummer 1. Haben Sie das gewünschte Modell gefunden, klicken Sie es in der Übersicht doppelt an und es wird automatisch in die Feld-Nr. des Dialogs **Form-Erfassung** übernommen.

### Manuelle Planerstellung

**Erfassung > Manueller Plan**

*(Abbildung J-59 zeigt den Dialog "Manuelle Planerstellung". Er besteht aus drei Hauptbereichen: einer Liste von "Glasarten", einer Liste von erstellten "Plänen" und einem Bereich für "Lagerplatten" und "Restblatt".)*

In diesem Dialog haben Sie die Möglichkeit, einen rein manuellen Plan zu erstellen und als Tischoptimierung in der Datenbank zu speichern. Der manuelle Plan kann nach der Erstellung erneut editiert und geändert werden. Dies geschieht mithilfe des Moduls **PlanEdit**. Nähere Erläuterungen zu diesem Modul finden Sie in der entsprechenden Dokumentation. Es ist keine Barcodeinformation für den manuellen Plan verfügbar.

#### Erläuterung der Felder im Bereich Glasarten

- **Glasart**: In diesem Feld sehen Sie die Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Dicke**: In diesem Feld sehen Sie die Dicke der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Glasart Bezeichnung**: In diesem Feld wird Ihnen die Klartextbezeichnung der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Rand links**: Von der Optimierung nicht nutzbarer linker Rand der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Rand rechts**: Von der Optimierung nicht nutzbarer rechter Rand der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Rand oben**: Von der Optimierung nicht nutzbarer oberer Rand der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Rand unten**: Von der Optimierung nicht nutzbarer unterer Rand der Lagerplatte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

#### Erläuterung der Felder im Bereich Plan

- **Lauf**: In diesem Feld sehen Sie die Nummer des Laufes, in dem der manuell zugefügte Plan geschnitten wird.
- **Gesperrt**: In dieser Spalte sehen Sie, ob und von welcher Station der Lauf zur Bearbeitung oder Verwendung in einer Optimierung gesperrt ist.
- **Glasart**: In diesem Feld sehen Sie für welche Glasart Sie einen manuellen Plan hinzugefügt haben.
- **Dicke**: In diesem Feld sehen Sie, welche Dicke die Glasart hat, die Sie dem manuellen Plan hinzugefügt haben.
- **Glasart Bezeichnung**: In diesem Feld wird Ihnen die Klartextbezeichnung der Glasart, die Sie dem manuellen Plan hinzugefügt haben.
- **Tisch**: In diesem Feld sehen Sie, auf welchem Tisch der manuell hinzugefügte Plan geschnitten wird.
- **Scheibenmenge**: In diesem Feld sehen Sie die Anzahl der Scheiben, die der manuell hinzugefügte Plan enthält.
- **Scheibenfläche**: In diesem Feld sehen Sie die Fläche der Scheiben in qm, die der manuell hinzugefügte Plan enthält.
- **Platten**: In diesem Feld sehen Sie die Anzahl der Platten, die der manuell hinzugefügte Plan in Anspruch nimmt.
- **Verschnitt**: In dieser Spalte sehen Sie, wieviel Verschnitt in % bei dem manuell hinzugefügten Plan entstehen würde.
- **Restblatt**: In dieser Spalte sehen Sie, wie lange das Restblatt ist, dass bei dem manuell hinzugefügten Plan übrig bleibt.

#### Erläuterung der Felder im Bereich Lagerplatten

- **Breite**: Das Feld zeigt Ihnen die Breite der Lagerplatte in mm oder inch (konfigurierbar).
- **Höhe**: Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm oder inch (konfigurierbar).
- **XY?**: In dieser Spalte ist angegeben, in welcher Richtung die Travere gebildet wird. Mögliche Werte:
  - **X**: Die Travere verläuft zwingend senkrecht zum unteren Plattenrand.
  - **Y**: Die Travere verläuft zwingend parallel zum unteren Plattenrand.
  - **?**: Die Optimierung kann sich wahlweise für eine der beiden Traverenrichtungen entscheiden.
- **Menge**: Der Wert dieses Feldes zeigt Ihnen die Anzahl der zur Verfügung stehenden Lagerplatten.

#### Erläuterung der Felder im Bereich Restblatt

- **Breite**: Falls ein Restblatt der entsprechenden Glasart/Dicke-Kombination vorhanden ist, kann das Restblatt an dieser Stelle verwendet werden. Geben Sie hier die Breite des Restblattes in mm an.
- **Höhe**: Falls ein Restblatt der entsprechenden Glasart/Dicke-Kombination vorhanden ist, kann das Restblatt an dieser Stelle verwendet werden. Geben Sie hier die Höhe des Restblattes in mm an.

#### Erläuterung der Felder und Schaltfläche im unteren Bereich

- **Feld ohne Namen**: In diesem Feld sehen Sie die Nummer des Laufes, in dem der manuell zugefügte Plan geschnitten wird.
- **Tisch**: In diesem Feld wird Ihnen der Tisch angezeigt, auf dem der manuell zugefügte Plan geschnitten wird.
- **Neu**: Über diese Schaltfläche starten Sie das Modul **PlanEdit**. Nähere Informationen zu diesem Modul finden Sie in der entsprechenden Dokumentation.
- **Editieren**: Diese Schaltfläche ist erst aktiv, wenn Sie einen manuellen Plan hinzugefügt haben. Anschließend haben Sie die Möglichkeit, über diese Schaltfläche den hinzugefügten Plan erneut zu bearbeiten.
- **Schneiden**: Über diese Schaltfläche starten Sie den Zuschnitt.

#### Ergänzende Informationen
- ⇨ Softwarereferenz, "Parameter" auf Seite J-1169

### Chargen-Editor

**Erfassung > Erfassung [F3]**

*(Abbildung J-60 zeigt den Dialog "Chargen-Editor". Er enthält eine Liste von Lagerplatten mit Details wie Glasart, Dicke, Breite, Höhe und Chargen-Bezeichnung. Unten gibt es ein Eingabefeld für die "Chargen-Bezeichnung" und eine Checkbox.)*

In diesem Dialog haben Sie die Möglichkeit, eine Chargen-Nummer einzugeben.

#### Erläuterung der Felder im Bereich Lagerplatten

- **Glasart**: In diesem Feld sehen Sie die Glasart. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Dicke**: In diesem Feld sehen Sie die Dicke der Glasart. Der Wert dieses Feldes kommt aus den Stammdaten in mm oder inch (konfigurierbar).
- **Breite**: Das Feld zeigt Ihnen die Breite der Lagerplatte in mm oder inch (konfigurierbar).
- **Höhe**: Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm oder inch (konfigurierbar).
- **Chargen Bezeichnung**: In diesem Feld wird Ihnen die eingegebene Chargen Bezeichnung angezeigt.
- **Glasart Bezeichnung**: In diesem Feld wird Ihnen die Klartextbezeichnung der Glasart angezeigt.

#### Erläuterung der Felder im Bereich Chargen Bezeichnung

- **Checkbox**: Wenn Sie diese Checkbox aktivieren, wird die eingegebene Chargen Nummer auf die nachfolgenden Lagerplatten der gleichen Glasart/Dicke vererbt.
- **Feld**: In diesem Feld geben Sie die Chargen Bezeichnung ein.

#### Ergänzende Informationen
- ⇨ Softwarereferenz, "Chargen-Editor" auf Seite J-1154

## Optimierung

Im Menü **Optimierung** befinden sich folgende Programmpunkte:

- **Tischoptimierung:**
  Über diesen Menüpunkt können Sie eine Tischoptimierung erstellen.
  ⇨ Softwarereferenz, "Selektieren Sie die zu optimierenden Gläser" auf Seite J-1157

- **Zurücksetzen:**
  Über diesen Menüpunkt haben Sie die Möglichkeit, Läufe zurückzusetzen.
  ⇨ Softwarereferenz, "Zurücksetzen eines Zuschnitt Laufes" auf Seite J-1173

### Selektieren Sie die zu optimierenden Gläser

**Optimierung > Tischoptimierung**

Diesen Dialog gibt es in zwei unterschiedlichen Varianten. Welche Variante angezeigt wird, hängt davon ab, welche Einstellungen Sie für die Tischoptimierung getroffen haben:
- Standard
- Produktionstermin
⇨ Kapitel "Tischoptimierung" auf Seite J-1203

#### Tischoptimierung in der Variante Standard

*(Abbildung J-61 zeigt den Dialog "Selektieren Sie die zu optimierenden Gläser" in der Standard-Variante. Der Dialog ist zweigeteilt: Oben eine Liste "Verfügbare Glasarten", unten eine Liste "Verfügbare Optimierungen".)*

In diesem Dialog listet Ihnen A+W Realtime Optimizer alle Glasarten auf, für die Läufe und Eilscheiben zur Optimierung bereit stehen. Zu der gewählten Glasart werden die verfügbaren Läufe angezeigt.

##### Erläuterung der Felder im Bereich Verfügbare Glasarten

- **Glasart**: Dieses Feld zeigt Ihnen die Artikelnummer der Glasart, für die Läufe verfügbar sind. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Dicke**: In diesem Feld wird die Dicke der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Restelager**: Diese Spalte wird nur angezeigt, wenn Ihr A+W Realtime Optimizer zur Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde. In dieser Spalte steht ein Eintrag, wenn im Restelager-Magazin eine Scheibe der entsprechenden Glasart und Dicke vorhanden ist. Die angegebene Zahl ist die Länge des Restblattes in mm im Restelager-Magazin. Wenn im Restelager-Magazin mehrere Restblätter der entsprechenden Glasart und Dicke liegen, dann wird das längste Restblatt hier angezeigt.
- **Bruchmenge**: Wenn für diese Glasart Bruchscheiben erfasst sind, wird in diesem Feld die Anzahl der Bruchscheiben angegeben.
- **Bruchfläche**: Wenn für diese Glasart Bruchscheiben erfasst sind, wird in diesem Feld die Gesamtfläche der Bruchscheiben angegeben.
- **Eilmenge**: Wenn für diese Glasart Eilscheiben erfasst sind, wird in diesem Feld die Anzahl der Eilscheiben angegeben.
- **Eilfläche**: Wenn für diese Glasart Eilscheiben erfasst sind, wird in diesem Feld die Gesamtfläche der Eilscheiben angegeben.
- **Glasart Bezeichnung**: In diesem Feld wird Ihnen die Klartextbezeichnung der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.

##### Erläuterung der Felder im Bereich Verfügbare Optimierungen

- **Lauf**: In dieser Spalte sehen Sie die Nummer des Laufes, der Optimierungen für die gewählte Glasart enthält.
- **Los**: In dieser Spalte sehen Sie die Losnummer des Laufes, der die Optimierungen für die gewählte Glasart enthält.
- **Gesperrt**: In dieser Spalte sehen Sie, ob und von welcher Station das Los zur Bearbeitung oder Verwendung in einer Optimierung gesperrt ist.
- **Parameter**: In dieser Spalte sehen Sie, für welchen Tisch das angezeigte Los optimiert wurde.
- **Platten**: In dieser Spalte sehen Sie, wieviele Lagerplatten die Losoptimierung benötigt.
- **Scheibenmenge**: In dieser Spalte sehen Sie, wieviele Scheiben die Losoptimierung beinhaltet.
- **Scheibenfläche**: In dieser Spalte sehen Sie, wieviele Quadratmeter Glas die Losoptimierung beinhaltet.
- **Verschnitt**: In dieser Spalte sehen Sie, wieviel Verschnitt in % bei der aktuellen Losoptimierung entstehen würde.
- **Rest (mm)**: In dieser Spalte sehen Sie, wie lange das Restblatt ist, dass bei der Losoptimierung auf dem Schneidtisch übrig bleibt.
- **Information**: In dieser Spalte werden Ihnen Laufbezeichnung angezeigt.
- **Termin**: In dieser Spalte sehen Sie den Produktionstermin, der bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.
- **Schicht**: In dieser Spalte sehen Sie die Produktionsschicht, die bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.

##### Erläuterung der Checkbox

- **Erlaube Handzuschnitt**: Wenn diese Checkbox markiert ist, dann werden in der Liste Glasarten auch die Glasarten zur Optimierung angezeigt, die bei der Artikeldefinition in den Stammdaten nur für Handzuschnitt vorgesehen wurden.
  - ☐ nur Glasarten für den automatischen Zuschnitt anzeigen
  - ☑ auch Glasarten für den Handzuschnitt anzeigen

#### Tischoptimierung in der Variante Produktionstermin

*(Abbildung J-62 zeigt den Dialog "Selektieren Sie die zu optimierenden Gläser" in der Variante Produktionstermin. Links befindet sich eine Liste von "Produktionsdatum". Die Hauptbereiche sind "Verfügbare Glasarten" und "Verfügbare Optimierungen".)*

Dieser Dialog zeigt die Produktionstermine und ermöglicht es Ihnen, die Optimierungen nach den Produktionstermin zu filtern. Dies erleichtert die Einhaltung von Fristen und die Planung des Produktionsablaufs.

Wählen Sie zunächst einen Produktionstermin aus der Liste **Produktionsdatum**.

Im Bereich **Verfügbare Glasarten** werden Ihnen alle Glasarten angezeigt, die in Optimierungen mit dem ausgewählten Produktionsdatum enthalten sind. Wählen Sie anschließend die Glasart aus, die Sie schneiden möchten.

Im Bereich **Verfügbare Optimierungen** werden Ihnen alle Optimierungen angezeigt, die bis zum ausgewählten Produktionsdatum produziert sein sollten. Für eine bessere Übersicht sind die Optimierungen farbig markiert:
- **Grün:** Der Produktionstermin liegt in der Zukunft.
- **Gelb:** Der Produktionstermin ist heute.
- **Rot:** Der Produktionstermin liegt in der Vergangenheit.

Die Felder der Bereiche **Verfügbare Glasarten** und **Verfügbare Optimierungen** sind identisch mit den Feldern im Dialog **Tischoptimierung in der Variante Standard** und werden an dieser Stelle erläutert.
⇨ Kapitel "Tischoptimierung in der Variante Standard" auf Seite J-1157

##### Ergänzende Informationen
- ⇨ Tutorial, "Läufe zum Zuschnitt auswählen" auf Seite J-1094

### Tischoptimierung Lauf [Nr]

Mit diesem Dialog werden verschiedene Parameter für die Optimierung eingestellt. Der Dialog ist in folgende Register unterteilt:
- Übersicht
- Optimieren
- Restplatten und Lagerplatten
- Parameter

#### Übersicht

**Optimierung > Tischoptimierung > Gläser selektieren - [Auswählen] > Übersicht**

*(Abbildung J-63 zeigt den Dialog "Tischoptimierung Lauf" mit dem Reiter "Übersicht". Er zeigt zwei Listen: die obere mit den zu optimierenden Glasarten und die untere mit den zugehörigen Läufen/Losen.)*

Dieser Dialog zeigt die im Dialog **Selektieren Sie die zu optimierenden Gläser** gewählten Läufe an. Wurde eine Optimierung durchgeführt, so wird deren Ergebnis angezeigt. Wenn noch keine Optimierung durchgeführt wurde, sind die Felder **Platten**, **Verschnitt** und **Rest (mm)** leer.

Nach einer durchgeführten Optimierung, kann per Doppelklick auf die Glasart das Programm **PlanEdit** gestartet werden, falls dieses an Ihrem Arbeitsplatz installiert ist. **PlanEdit** zeigt Ihnen das Brechbild der Lagerplatte grafisch an.

##### Erläuterungen der oberen Liste

- **Glasart**: In diesem Feld werden Ihnen die Artikelnummern der Glasarten angezeigt, die in der gewählten Tischoptimierung enthalten sind. Der Wert dieses Feldes kommt aus den Stammdaten.
- **Dicke**: In diesem Feld wird Ihnen die Dicke der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten in mm oder inch (konfigurierbar).
- **Parameter**: Wenn die Optimierung durchgeführt wurde, dann sehen Sie in diesem Feld, mit welchen Optimierungsparametern die Optimierung durchgeführt wurde.
- **Menge**: Der Wert dieses Feldes zeigt Ihnen die Anzahl der Scheiben.
- **Fläche**: In diesem Feld sehen Sie die gesamte Fläche der optimierten Glasart in Quadratmeter.
- **Platten**: Diese Feld zeigt Ihnen die Anzahl der Lagerplatten, die für die Optimierung benötigt werden (Anzeige erst nach durchgeführter Optimierung).
- **Verschnitt**: In diesem Feld sehen Sie die Glasfläche in %, die als Verschnitt anfällt (Anzeige erst nach durchgeführter Optimierung).
- **Rest (mm)**: Hier sehen Sie die Breite des Restblatts in mm, das nach dem Zuschnitt noch auf dem Tisch liegt und weiterverwendet werden könnte (Anzeige erst nach durchgeführter Optimierung).

##### Erläuterungen der unteren Liste

- **Lauf**: Das Feld zeigt Ihnen die Nummer der Läufe, von denen ein Los in der angezeigten Tischoptimierung enthalten ist.
- **Los**: Das Feld zeigt Ihnen die Nummer des Loses, dessen Scheiben in der angezeigten Tischoptimierung enthalten sind.
- **Zuschnitts-Böcke**: In diesem Feld sehen Sie die Anzahl der Zuschnittsböcke, die von der Feinplanung für die Scheiben dieses Losen eingeplant wurden.
- **Sonderglaslauf**: Hier wird angegeben, ob es sich um einen Sonderglaslauf handelt. Ein Sonderglaslauf liegt dann vor, wenn die gewählte Glasart in den Stammdaten als Sonderglas definiert wurde. Mögliche Werte:
  - Ja
  - Nein
- **Platten**: In diesem Feld sehen Sie die Anzahl an Lagerplatten, die für den Zuschnitt des Loses ermittelt wurden. Es handelt sich hierbei um das Berechnungsergebnis der Feinplanung, nicht der Tischoptimierung.
- **Verschnitt**: Das Feld zeigt Ihnen die Glasfläche in %, die beim Zuschnitt des Loses als Verschnitt anfällt. Es handelt sich hierbei um das Berechnungsergebnis der Feinplanung, nicht der Tischoptimierung.
- **Rest (mm)**: In diesem Feld sehen Sie die Breite des Restblatts in mm, das nach dem Zuschnitt des Loses noch auf dem Tisch liegt und weiterverwendet werden könnte. Es handelt sich hierbei um das Berechnungsergebnis der Feinplanung, nicht der Tischoptimierung.

##### Ergänzende Informationen
- ⇨ Tutorial, "Tischoptimierungen erstellen" auf Seite J-1083
- ⇨ Tutorial, "Tischoptimierungen" auf Seite J-1083

#### Optimieren

**Optimierung > Tischoptimierung > Gläser selektieren - [Auswählen] > Optimieren**

*(Abbildung J-64 zeigt den Reiter "Optimieren" des "Tischoptimierung" Dialogs. Er enthält Bereiche für "Optimierungsreihenfolge", "Lauf-Parameter", "Rangfolge", "Automatische Zusammenstellung", "Tisch" und "Optimierungs-Parameter".)*

In diesem Dialog nehmen Sie die Einstellungen für die Optimierung vor. Die Liste liefert Ihnen Informationen zu der gewählten Glasart.

##### Erläuterung der Felder im Bereich Optimierungsreihenfolge

- **Lauf**: In diesem Feld sehen Sie, welcher Lauf bzw. welche Läufe optimiert werden sollen.
- **Los**: Dieses Feld zeigt Ihnen, die Losnummer der einzelnen Läufe.
- **Rang**: Dieses Feld zeigt Ihnen den Optimierungsrang. Durch Betätigen der Schaltflächen **^** oder **v** können Sie Rangfolge ändern. Gleiche Ränge werden gemischt, unterschiedliche getrennt.
- **Positionen**: In diesem Feld sehen Sie, wie viele Positionen in dem Lauf enthalten sind.
- **A-Böcke**: Das Feld zeigt Ihnen die Anzahl der A-Böcke, die für diesen Lauf notwendig sind.
- **Fächerwagen**: Das Feld zeigt Ihnen die Anzahl der Fächerwagen, die für diesen Lauf notwendig sind.
- **Scheibenmenge**: Das Feld zeigt Ihnen die Anzahl Scheiben, die in diesem Lauf enthalten sind.
- **Scheibenfläche**: Das Feld zeigt Ihnen die Scheibenfläche in qm, die in diesem Lauf enthalten sind.
- **Platten**: Das Feld zeigt Ihnen die Anzahl der Platten, die zum Schneiden dieses Laufes notwendig sind.

##### Erläuterung der Schaltflächen im Bereich Rangfolge

- **A (Pfeil nach oben)**: Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie z. B. einen Lauf mit dem Rang 1 gewählt und betätigen dann die Schaltfläche A, ändert sich der Rang von 1 nach 2. Gleichzeitig ändert sich gegebenenfalls die Sortierung der Tabelle.
- **V (Pfeil nach unten)**: Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie z. B. einen Lauf mit dem Rang 1 gewählt und betätigen dann die Schaltfläche V, ändert sich der Rang von 2 nach 1. Gleichzeitig ändert sich gegebenenfalls die Sortierung der Tabelle.
- **Auswählen**: Mit dieser Kombobox steuern Sie den Rang. Die Kombobox enthält soviel Ränge, wie Läufe in der Tabelle zu sehen sind. Sie können dann aus der Tabelle einen Lauf auswählen, die Kombobox öffnen und dem ausgewählten Lauf den gewünschten Rang zuweisen. Die Ränge sind fortlaufend zu vergeben, d. h. es kann kein Rang übersprungen werden.

##### Erläuterung der Felder im Bereich Automatische Zusammenstellung

- **Lose trennen**: Mit dieser Checkbox steuern Sie, ob ein Trennen der Lose gewünscht ist oder nicht. Mögliche Werte:
  - ☐ Lose werden nicht getrennt.
  - ☑ Lose werden getrennt. Wenn Sie die Checkbox aktivieren, hat das u. U. Auswirkung auf das Feld **Rang**.
- **Lose nach maximaler Anzahl der Zuschnittsböcke trennen**: Mit dieser Checkbox steuern Sie, ob und wenn ja wann Lose getrennt werden. Wenn Sie wünschen, dass Lose nach einer gewissen Anzahl von Zuschnittsböcken getrennt werde, müssen Sie die Checkbox aktivieren und im Feld dahinter die Menge eingeben, nach der getrennt werden soll.
- **Mindestscheibenfläche für das Trennen von Losen verwenden**: Mit dieser Checkbox steuern Sie, ob und wenn ja wann Lose getrennt werden. Wenn Sie wünschen, dass Lose ab einer gewissen Scheibenfläche (in qm) getrennt werde, müssen Sie die Checkbox aktivieren und im Feld dahinter die Fläche eingeben, nach der getrennt werden soll.

> **Trennen von Losen**
> Lose können entweder nach einer maximalen Anzahl von Zuschnittsböcken oder einer Mindestscheibenfläche getrennt werden. Beide Checkboxen können zusammen nicht aktiviert werden.

##### Erläuterung der Felder im Bereich Lauf-Parameter

- **XOPT-S**: Verwenden Sie in Ihrem Betrieb A-Böcke, dann muss dieser Parameter gesetzt werden. Die Optimierung berücksichtigt dann, dass die Scheiben auf A-Böcke gestellt werden und für die nachfolgende Bearbeitungen in einer bestimmten Reihenfolge stehen müssen.
- **Bruchscheiben**: Wenn Sie diesen Parameter wählen, dann lassen Sie zu, dass immer dann, wenn zu der gewählten Glasart Bruchscheiben existieren, diese automatisch in die anstehende Optimierung mit einbezogen werden.
- **Eilscheiben**: Wenn Sie diesen Parameter wählen, dann lassen Sie zu, dass immer dann, wenn zu der gewählten Glasart Eilaufträge existieren, diese automatisch in die anstehende Optimierung mit einbezogen werden.
- **Füller nur für Lücken**: Existieren in Ihrem System Füllaufträge der gleichen Glasart und haben Sie diesen Parameter gesetzt, dann werden bei der Optimierung eventuell vorhandene Lücken in der Optimierung mit Füllaufträgen gefüllt. Das Restblatt wird nicht mit Füllaufträgen aufgefüllt. Existieren Füllaufträge zur gewählten Glasart, so werden diese im Register Füller angezeigt.
- **Restelager**: Diese Checkbox wird nur angezeigt, wenn Sie über ein entsprechendes Restelager verfügen.
  - ☐ Das Restelager wird nicht verwendet
  - ☑ Das Restelager wird verwendet

##### Erläuterung der Felder im Bereich Tisch

- **Tisch**: Die Kombobox enthält alle in Ihrem Hause konfigurierten Tische. Wählen Sie aus der Kombobox den entsprechenden Tisch aus. Im darunter liegenden Bereich wird Ihnen der Name des Tisches angezeigt.

##### Erläuterung der Felder im Bereich Optimierungs-Parameter

- **Optimierungsparameter**: Die Kombobox enthält die Optimierungsparameter, mit denen die Optimierung erstellt werden soll. Es stehen nur die Optimierungsparameter zur Verfügung, mit denen der ausgewählte Tisch arbeiten kann. Wählen Sie aus der Kombobox den entsprechenden Parameter aus. Im darunter liegenden Bereich wird Ihnen der Name des Parameters angezeigt.

##### Erläuterung der Schaltflächen

- **Optimieren**: Mit dieser Schaltfläche starten Sie die Optimierung. Die Optimierung läuft im Hintergrund. Sobald das Ergebnis vorliegt, kann es im Register **Übersicht** angesehen werden. Das Optimierungsergebnis wird erst dann in die Datenbank gespeichert, wenn die Schaltfläche [Speichern] oder [Schneiden] betätigt wird.

##### Ergänzende Informationen
- ⇨ Tutorial, "Tischoptimierungen" auf Seite J-1083

#### Restplatten und Lagerplatten

**Optimierung > Tischoptimierung > Restplatten und Lagerplatten**

*(Abbildung J-65 zeigt den Reiter "Restplatten und Lagerplatten". Links werden die Glasartdetails angezeigt. Rechts eine Liste der verfügbaren Lager- und Restplatten für diese Glasart.)*

In diesem Dialog wählen Sie für die zuvor ausgewählte Glasart die Restplatten und die Lagerplatten aus, die Sie für die Optimierung verwenden möchten. Auf der linken Seite sehen Sie die gewählte Glasart. Die rechte Seite zeigt Ihnen die zur Glasart passende(n) Lagerplatte oder, wenn vorhanden, die passenden Restplatten. Diese sind nach Verfügbarkeit sortiert und gruppiert im Sinne der Entladereihenfolge des Gestells.

##### Erläuterung der Felder im Bereich Liste Lagerplatten (rechts)

- **Breite**: Das Feld zeigt Ihnen die Breite der Lagerplatte in mm.
- **Höhe**: Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm.
- **XY?**: In dieser Spalte ist angegeben, in welcher Richtung die Travere gebildet wird. Mögliche Werte:
  - **X**: Die Travere verläuft zwingend senkrecht zum unteren Plattenrand.
  - **Y**: Die Travere verläuft zwingend parallel zum unteren Plattenrand.
  - **?**: Die Optimierung kann sich wahlweise für eine der beiden Traverenrichtungen entscheiden.
- **Restelagerfach**: Das Feld zeigt Ihnen, wo sich die Lagerplatte befindet. Steht in diesem Feld der Begriff Lager, handelt es sich bei der Platte um eine Lagerplatte. Steht in dem Feld eine Ziffer, z. B. 2, dann handelt es sich bei der Platte um eine Restlagerplatte, die sich im Restelagerfach mit der Nummer 2 befindet. Steht in dem Feld WH (Warehouse) befindet sich die Platte in einem vertikalen Remaster. Steht in dem Feld RM, befindet sich die Platte in einem (horizontalen) Remaster.
- **Einlagerzeit / Menge**: Wenn es sich bei der Platte um eine Restlagerplatte handelt, können Sie in diesem Feld das Datum und die Uhrzeit der Einlagerung (in das Restelager) sehen. Steht in dem Feld eine Zahl, z. B. 7670, dann handelt es sich bei der Platte um eine Lagerplatte, von der noch 7670 Stück auf Lager sind.

##### Erläuterung der Felder im Bereich Restblatt

- **Höhe/Breite**: Liegt auf dem Zuschnitttisch vom vorherigen Zuschnitt noch ein Restblatt der gleichen Glasart und Dicke, so können Sie dieses weiter verwenden. Geben Sie hier Höhe und Breite des Restblatts ein. Die Optimierung nutzt dann zuerst dieses Restblatt aus, bevor eine neue Lagerplatte verwendet wird.
> **Restblatt und Restelager-Platte nicht gleichzeitig möglich!**
> Wenn Sie bereits eine Restelager-Platte verwenden, kann kein Restblatt mehr verwendet werden. Wenn Ihr A+W Realtime Optimizer zur Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde, dann kann die Verwendung einer Restelager-Platte im Register Optimieren mit der Checkbox Verwenden ein- und ausgeschaltet werden.

##### Ergänzende Informationen
- ⇨ Tutorial, “A+W Residual Stock Manager" auf Seite J-1104

#### Parameter

**Optimierung > Tischoptimierung > Parameter**

*(Abbildung J-66 zeigt den Reiter "Parameter". Links eine Liste der Lagerplatten. Rechts Bereiche für "Beschichtung" und "Optimierungs-Parameter" wie Ränder, Travere und Schneidmodus.)*

In diesem Dialog nehmen Sie die Parameter-Einstellungen für die Tischoptimierung vor. Die Liste zeigt Ihnen die für die Optimierung zur Verfügung stehenden Lagerplatten.

##### Erläuterung der Felder im Bereich Beschichtung

- **Keine/Oben/Unten**: Falls die Lagerplatte über eine Beschichtung verfügt, geben Sie mit diesen Radiotasten an, ob sich die Beschichtung **oben** oder **unten** befindet. Hat die Lagerplatte keine Beschichtung, aktivieren Sie die Radiotaste **Keine**.

##### Erläuterung der Schaltfläche

- **Anzahl**: Mit dieser Schaltfläche öffnen Sie den Dialog **Anzahl der Lagerplatten**.

##### Erläuterung der Felder im Bereich Optimierungs-Parameter

- **Ränder**: Die Felder **Rand links**, **Rand rechts**, **Rand oben** und **Rand unten** zeigen Ihnen die für den entsprechenden Glasartikel erfassten Bruchränder. Die grau unterlegten Felder beziehen sich auf die aus den Glasartikel-Stammdaten gezogenen Werte. In den weiß unterlegten Feldern können Sie diesen Wert überschreiben. Es handelt sich dabei um ein temporäres Ändern der Bruchrändern für den jeweiligen Lauf.
- **Autotravere**: Die Checkbox steuert, ob die angegebene maximale Traverenbreite vergrößert werden darf.
  - ☑ Die angegebene maximale Traverenbreite darf vergrößert werden.
  - ☐ Die angegebene maximale Traverenbreite darf nicht vergrößert werden.
- **Max. Travere**: Das Feld **Max. Travere** bezieht sich auf die maximale Traverenbreite des gewählten Glasartikels. Das grau unterlegte Feld bezieht sich auf den aus dem Glasartikel-Stammdaten gezogenen Wert. In dem weiß unterlegten Feld können Sie diesen Wert überschreiben. Es handelt sich dabei um ein temporäres Ändern der maximalen Traverenbreite für den jeweiligen Lauf.
- **Schneidmodus**: Das Feld legt den Schneidmodus für die XOPT(S)-Optimierungen fest. Die gesetzte Radiotaste zeigt Ihnen, mit welchem Schneidmodus die Feinplanung durchlaufen wurde. Die Auswahl des richtigen Schneidmodus richtet sich nach dem Schneidtisch und den betrieblichen Anforderungen. Generell gilt, dass mit Schneidmodus 1 die besten und mit Schneidmodus 4 geringfügig schlechtere Verschnittergebnisse entstehen. Diese höheren Materialverluste lassen sich unter Umständen durch schnelleres Brechen und Abräumen kompensieren. Der Schneidmodus bestimmt die Lage der Scheiben innerhalb einer Travere zwischen zwei benachbarten Y-Schnitten. Mögliche Werte:
  - **1**: Zwischen zwei Y-Schnitten dürfen Scheiben verschiedener Breite und Höhe nebeneinander liegen. Es können also auch W - Schnitte vorkommen.
  - **2**: Zwischen zwei Y-Schnitten dürfen nur Scheiben mit unterschiedlicher Breite aber gleicher Höhe nebeneinander liegen.
  - **3**: Zwischen zwei Y-Schnitten dürfen nur Scheiben der gleichen Position nebeneinander liegen.
  - **4**: Zwischen zwei Y-Schnitten dürfen höchstens zwei Scheiben der gleichen Position nebeneinander liegen.
  - **5-7**: Spezialmodus für einen Coopmes-Tisch. Dieser Modus ist identisch mit Modus 2-4.

##### Erläuterung der Schaltflächen

- **PlanEdit**: Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung durchgeführt haben. Betätigen Sie diese Schaltfläche, öffnet sich das Programm **PlanEdit**.
- **Schneiden**: Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung durchgeführt haben. Betätigen Sie diese Schaltfläche, starten Sie den Zuschnitt.

##### Ergänzende Informationen
- ⇨ Softwarereferenz, "Anzahl der Lagerplatten" auf Seite J-1172

#### Anzahl der Lagerplatten

**Optimierung > Tischoptimierung > Parameter > [Anzahl]**

*(Abbildung J-67 zeigt den Dialog "Anzahl der Lagerplatten" mit einem Feld zur Eingabe der Anzahl und den Schaltflächen "Verwenden" und "Abbrechen".)*

In diesem Dialog sehen Sie die Anzahl der zur Verfügung stehenden Lagerplatten für die gewählte Glasart.

### Zurücksetzen eines Zuschnitt Laufes

**Optimierung > Zurücksetzen**

*(Abbildung J-68 zeigt den Dialog "Zurücksetzen eines Zuschnitt-Laufes" mit einer Liste von Läufen und deren Status (z.B. Freigegeben, Begonnen, Produziert).)*

Mit diesem Dialog können Sie Läufe, die bereits begonnen oder produziert wurden, wieder zurücksetzen und erneut bearbeiten. Tischoptimierungen, die bereits gespeichert wurden, können hier wieder aufgelöst werden. Läufe, die bereits produziert sind aber nicht gebucht wurden, können als produziert gebucht werden. Die Löschroutinen für alte (produzierte) Läufe übernimmt der ALCIMServer. Informationen zum Löschen von Läufen finden Sie in der zugehörigen Dokumentation.

#### Erläuterung der Liste Läufe

- **Lauf**: Hier werden die Nummern der Läufe angezeigt, deren Status verändert werden kann. Die Nummern 1000 - 9999 stehen für fertig optimierte Läufe (z. B. aus A+W Production), die zum Schneiden zur Verfügung stehen. Die Nummern 15000 - 19999 (Nummernkreise konfigurierbar) sind für selbst erstellte Tischoptimierungen reserviert.
- **Gesperrt**: In dieser Spalte erscheint ein Eintrag, wenn ein anderes A+W Realtime Optimizer oder ein anderer Prozess den entsprechenden Lauf in Bearbeitung hat.
- **Status**: Hier wird angezeigt, in welchen Bearbeitungsstand sich die einzelnen Läufe befinden.

| Status | Bedeutung |
| :--- | :--- |
| **Freigegeben** | Es liegt eine Optimierung vor, die zum Zuschnitt freigegeben ist. Solche Läufe können in einer Tischoptimierung weiterbearbeitet werden, bevor der Zuschnitt erfolgt. |
| **Begonnen** | Die Bearbeitung des Laufes wurde begonnen. Es sind Lose aus diesem Lauf bereits beim Zuschnitt oder in einer Tischoptimierung. Auch wenn eine Tischoptimierung nicht geschnitten, sondern wieder aufgelöst wurde, wird dieser Status angezeigt. |
| **Produziert** | Der Lauf wurde produziert. |

#### Erläuterung der Schaltflächen

- **Produziert**: Wenn ein freigegebener Lauf markiert ist und diese Schaltfläche gewählt wird, dann wird der Lauf als produziert markiert und steht für die Optimierung nicht mehr zur Verfügung.
- **OK**: Wenn eine freigegebene Tischoptimierung (Lauf ab Nr. 15000) (konfigurierbar) markiert ist und diese Schaltfläche gewählt wird, dann wird die Tischoptimierung aufgelöst. Die enthaltenen Läufe, Bruchscheiben, Eilscheiben oder Füllscheiben stehen für neue Optimierungen wieder zur Verfügung. Vor der Ausführung dieser Funktion erfolgt eine Sicherheitsabfrage. Wenn ein produzierter Lauf markiert ist und diese Schaltfläche gewählt wird, dann wird der Lauf zurückgesetzt und kann erneut produziert werden.

#### Ergänzende Informationen
- ⇨ Tutorial, "Schneidstatus zurücksetzen" auf Seite J-1102

### Pausierende Glasarten

**Optimierung > DynOpt Einstellungen**

*(Abbildung J-69 zeigt den Dialog "DynOpt Einstellungen" mit dem Reiter "Pausierende Glasarten". Er enthält eine Liste von Glasarten mit ihrem Status und Schaltflächen, um sie zu sperren, freizugeben etc.)*

Wird ein Lauf in das DynOpt importiert, muss sichergestellt werden, dass es genug Glasplatten dieser Glasart auf Lager gibt. Sie dürfen auf keinen Fall einen Lauf importieren, der die fehlenden Glasarten enthält. Manchmal kommt jedoch vor, dass Sie erst während der Produktion feststellen, dass einige Glasarten nicht zur Verfügung stehen. Mit diesem Dialog haben Sie jetzt die Möglichkeit, die einzelnen Glasarten zu sperren oder aus der Produktion zu entfernen. Der Dialog zeigt Ihnen alle Glasarten, die sich in der Produktion befinden.

#### Erläuterung der einzelnen Felder

- **Filter**: Mithilfe dieser Kombobox können Sie Liste der Glasarten einschränken. Folgende Werte stehen zur Verfügung:
  - **Alle**: Es werden alle Glasarten angezeigt, die sich in der Produktion befinden.
  - **Gesperrt**: Es werden nur gesperrte Glasarten angezeigt.
  - **Dringend**: Es werden nur dringende Glasarten angezeigt. Unter dringend versteht man solche Scheiben dieser Glasart, die vor den DynOpt Ausgangslinien warten.
- **Ausgang**: Diese Kombobox ist nur aktiv, wenn Sie in der Kombobox Filter die Einstellung Dringend gewählt haben. Sie haben dann die Möglichkeit, sich die dringenden Glasarten pro Ausgang anzeigen zu lassen. Hierzu müssen die Ausgänge entsprechend konfiguriert werden.
- **Grund für das Pausieren**: Um eine Glasart zu sperren, markieren Sie diese und wählen aus der Kombobox den Grund aus.

#### Schaltflächen

- **Optimierung stoppen**: Über diese Schaltfläche stoppen Sie die Optimierung. Das ist nötig, wenn Sie eine Glasart komplett aus der Produktion entfernen möchten. Dazu müssen Sie zunächst die Optimierung stoppen und dann die Glasart entfernen.
- **Entfernen**: Diese Schaltfläche ist nur aktiv, wenn Sie für eine Glasart die Optimierung gestoppt haben. Anschließend können Sie die Glasart entfernen.
- **Sperren**: Über diese Schaltfläche sperren Sie eine Glasart für den nächsten Optimierungsvorgang. Wählen Sie zunächst die Glasart, dann den Grund und klicken Sie dann auf [Sperren].
- **Freigeben**: Über diese Schaltfläche geben Sie eine gesperrte Glasart wieder frei. Wählen Sie zunächst die Glasart und klicken Sie dann auf [Freigeben].
- **Übersicht**: Mit dieser Schaltfläche öffnen Sie den Dialog **Aktuell geänderte Einstellungen** mit einer Übersicht der jeweiligen Einstellungen.
- **Auflösen**: Diese Schaltfläche ist nur aktiv, wenn die Produktion aktiv ist. Dann können Sie über diese Schaltfläche eine neue DynOpt-Optimierung erzwingen.
- **Übernehmen**: Über diese Schaltfläche bestätigen Sie die Aktionen. Bsp.: Sie haben eine Glasart gesperrt, dann klicken Sie auf [Übernehmen] um die Aktion abzuschließen.

### Aktuell geänderte Einstellungen

**Optimierung > DynOpt Einstellungen > [Übersicht]**

*(Abbildung J-70 zeigt den Dialog "Aktuell geänderte Einstellungen - Übersicht", der eine Zusammenfassung der Einstellungen für Allgemein, Eingänge, Ausgänge und Puffer anzeigt.)*

Dieser Dialog gibt Ihnen eine zusammenfassende Übersicht zu den Einstellungen der Register:
- Allgemein
- Eingänge
- Ausgänge
- Puffer

## Zuschnitt

Im Menü **Zuschnitt** befinden sich folgende Programmpunkte:

- **Schneide Optimierung:**
  Über diesen Menüpunkt schneiden Sie einen Lauf.
  ⇨ Softwarereferenz, "Wählen Sie einen Lauf aus" auf Seite J-1179
- **Bruchpool:**
  Über diesen Menüpunkt greifen Sie auf den Bruchpool zu.
  ⇨ Softwarereferenz, "Bruchpool" auf Seite J-1192
- **Panorama:**
  Über diesen Menüpunkt greifen Sie auf das Panorama zu (optional)

### Wählen Sie einen Lauf aus

**Zuschnitt > Schneide Optimierung**

*(Abbildung J-71 zeigt den Dialog "Wählen Sie einen Lauf aus", der eine obere Liste mit "Läufen" und eine untere Liste mit "Optimierungen" für den ausgewählten Lauf enthält.)*

Mit diesem Dialog wählen Sie einen verfügbaren Lauf aus. Im gewählten Lauf wählen Sie eine oder alle Optimierungen aus. Diese Optimierungen werden dann zum Zuschnitt vorbereitet.

#### Erläuterungen der Liste Läufe

- **Lauf**: Hier werden die Nummern der Läufe angezeigt, deren Status verändert werden kann. Die Nummern 1000 - 9999 stehen für fertig optimierte Läufe (z. B. aus A+W Production), die zum Schneiden zur Verfügung stehen. Die Nummern 15000 - 15999 (Nummernkreise konfigurierbar) sind für selbst erstellte Tischoptimierungen reserviert. Befindet sich an dieser Stelle der Begriff **DynOpt Compact**, handelt es sich um einen DynOpt Compact Lauf.
- **Status**: Hier wird angezeigt, in welchem Bearbeitungszustand sich die einzelnen Läufe befinden.

| Status | Bedeutung |
| :--- | :--- |
| **Freigegeben** | Es liegt eine Optimierung vor, die zum Zuschnitt freigegeben ist. Solche Läufe können in einer Tischoptimierung weiterbearbeitet werden, bevor der Zuschnitt erfolgt oder direkt zugeschnitten werden. |
| **Begonnen** | Die Bearbeitung des Laufes wurde begonnen. Es sind Lose aus diesem Lauf bereits beim Zuschnitt oder in einer Tischoptimierung. |
| **Produziert** | Der Lauf wurde produziert. |

- **Information**: In dieser Spalte werden Ihnen Laufbezeichnung angezeigt.
- **Termin**: In dieser Spalte sehen Sie den Produktionstermin, der bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.
- **Schicht**: In dieser Spalte sehen Sie die Produktionsschicht, die bei der Lauferstellung durch die Kapazitätsplanung ermittelt wurde.

> **Sortierung ändern**
> Durch einen Klick auf die Spaltenüberschriften können Sie die Listeninhalte auf- bzw. absteigend sortieren.

#### Erläuterungen der Liste Optimierung

- **Nr**: Losnummer der in einem Lauf enthaltenen Optimierungen.
- **Status**: Hier wird angezeigt, in welchen Bearbeitungszustand sich die einzelnen Optimierungen befinden.
- **Glasart**: In diesem Feld sehen Sie die Artikelnummer der Glasart, die in dieser Optimierung enthalten ist.
- **Dicke**: In diesem Feld sehen Sie die Dicke der Glasart, die in dieser Optimierung enthalten ist.
- **Glasart Bezeichnung**: In diesem Feld sehen Sie die Bezeichnung der Glasart.
- **Parameter**: Dieses Feld zeigt Ihnen die Bezeichnung des Tisches, für den die Optimierung erzeugt wurde.
- **Platten**: In diesem Feld sehen Sie die Anzahl der benötigten Lagerplatten in dieser Optimierung.
- **Verschnitt**: Das Feld zeigt Ihnen die Verschnittglasfläche in %, die bei dieser Optimierung anfällt.
- **Rest (mm)**: In diesem Feld sehen Sie die Länge des Restblattes, das nach dem Zuschnitt der Optimierung übrig bleibt.

#### Erläuterungen der Felder

- **Alte Läufe**: Wenn Sie diese Checkbox markieren, dann werden auch die Läufe angezeigt, die bereits produziert wurden und sich noch im Status Produziert befinden.
- **Geschnittene Optimierungen ausblenden**: Wenn Sie diese Checkbox markieren, dann werden die bereits geschnittenen Optimierungen nicht angezeigt.
- **Reoptimierung**: Über diese Kombobox steuern Sie Neuoptimierungen. Mögliche Werte sind:
  - **Nein**: Es erfolgt keine Neuoptimierung.
  - **Ja**: Es erfolgt eine Neuoptimierung ohne Benutzereingriff.
  - **Erweitert**: Neuoptimierung mit Anzeige der vorhandenen Optimierung der zu schneidenden Glasart. Hier können Sie der neu zu optimierenden Optimierung noch weitere Optimierungen für die Tischoptimierung hinzufügen.
  - **Tischoptimierung**: Neuoptimierung mit Anzeige des Dialgos Tischoptimierung. Hier können die Optimierungsparameter geändert werden.
- **Komboboxen (Maschinenstatus & Laufanzeige)**:
  - Die obere Kombobox kennzeichnet den Status der Maschine (**Bereit**, **Aus**).
  - Die untere Kombobox filtert die angezeigten Läufe (**Läufe für den eigenen Tisch**, **Läufe für alternative Tische**, **Läufe für alle Tische**).
- **Tischauswahl**: Mithilfe der Kombobox können Sie die Anzeige einschränken (alle Tische oder spezifische Tische).

#### Erläuterung der Schaltflächen

- **Optionen**: Durch Betätigen dieser Schaltfläche werden aus den Optimierungsdaten Zuschnittdaten erzeugt und an den Schneidtisch übertragen. Der Zuschnitt beginnt. Die Anzeige wechselt auf **STOPP**.
- **Sortieren**: Diese Schaltfläche ist nur aktiv, wenn für einen Lauf mehr als eine Optimierung gibt. Startet den Dialog **Optimierungs-Reihenfolge**.
- **Schneiden**: Durch Betätigen dieser Schaltfläche starten Sie den Dialog **Zuschnitt-Übersicht**.

#### Ergänzende Informationen
- ⇨ Tutorial, "Läufe zum Zuschnitt auswählen" auf Seite J-1094
- ⇨ Tutorial, "Tischansteuerung" auf Seite J-1091

### Lauf [Nummer] - Lauf [Nummer] (Zuschnitt-Übersicht)

**Zuschnitt > Schneide Optimierung > [OK]**

*(Abbildung J-72 zeigt den Dialog "Aktiver Lauf", der die ausgewählten Optimierungen und die dazugehörigen Muster (Lagerplatten) für den Zuschnitt anzeigt.)*

In diesem Dialog werden die zuvor im Dialog **Wählen Sie einen Lauf aus** gewählten Läufe und Lose angezeigt und können geschnitten werden.

#### Erläuterungen der Liste Optimierungen
⇨ Softwarereferenz, "Erläuterungen der Liste Optimierung" auf Seite J-1179

#### Erläuterungen der Liste Muster

- **Nr.**: Fortlaufende Nummerierung der Lagerplatten in der Zuschnittsreihenfolge.
- **Breite**: Breite der Lagerplatte in mm.
- **Höhe**: Höhe der Lagerplatte in mm.
- **Opt. Gr.**: Zeigt an, welche Optimierungsgruppen die Lagerplatte belegen. Nur zwei Gruppen je Lagerplatte möglich (Lauf oder Nachoptimierung).
- **Status**: Status der einzelnen Lagerplatten der Optimierung.

| Status | Bedeutung |
| :--- | :--- |
| **Gesendet** | Der Schneidcode wurde erzeugt. |
| **Überspringen** | Für diese Lagerplatte wird kein Schneidcode erzeugt und kein Brechbild zur Verfügung gestellt. |
| **Kein Schneidcode senden** | Für diese Lagerplatte wird kein Schneidcode erzeugt aber ein Brechbild zur Verfügung gestellt. |
| **Geschnitten** | Status wird gesetzt, wenn der Schneidtisch den Schneidcode empfangen hat. |

#### Erläuterung der Schaltflächen

- **Tisch - START**: Startet die Übertragung der Zuschnittdaten an den Schneidtisch. Die Anzeige wechselt auf **STOPP**.
- **Tisch - STOPP**: Beendet die Übertragung. Der aktuelle Zuschnitt wird zu Ende geführt. Die Anzeige wechselt auf **START**.
- **Muster - Folge**: Ruft den Dialog **Optimierungsreihenfolge** auf.
- **Muster - Optionen**: Ruft den Dialog **Lauf: Nummer** auf.
- **XTV - Stopp**: Stoppt die Kommunikation. Das letzte Brechbild bleibt erhalten.
- **XTV - <<**: Blättert in der Brechbildanzeige eines angeschlossenen XTV zurück.
- **Beenden**: Schließt den Dialog. Dies ist nur möglich, wenn keine Schneidcodegenerierung läuft.

#### Ergänzende Informationen
- ⇨ Softwarereferenz, "Optimierungsreihenfolge" auf Seite J-1185
- ⇨ Softwarereferenz, "Lauf: Nummer" auf Seite J-1186
- ⇨ Tutorial, "Ergebnis der Tischoptimierung prüfen und bearbeiten" auf Seite J-1085
- ⇨ Tutorial, “Tischoptimierungen" auf Seite J-1083

### Optimierungsreihenfolge

**Zuschnitt > Schneide Optimierung > Optimierung wählen > [Sortieren]**

*(Abbildung J-73 zeigt den Dialog "Optimierungsreihenfolge" mit einer Liste der zu optimierenden Glasarten. Die Reihenfolge kann mit Pfeiltasten geändert werden.)*

Wenn mehrere Glasarten im gewählten Lauf zur Optimierung anstehen, wird in diesem Dialog die vorgesehene Reihenfolge der Glasarten angezeigt. Sie können diese mithilfe der Pfeiltasten ändern.

#### Felder

- **Status**: Status der Optimierung.
- **Glasart**: Artikelnummer der Glasart.
- **Dicke**: Dicke der Glasart in mm.
- **Glasart Bezeichnung**: Bezeichnung der Glasart.
- **Parameter**: Auf welchem Schneidtisch die Optimierung geschnitten werden soll.
- **Platten**: Wie viele Lagerplatten die Optimierung benötigt.
- **Verschnitt**: Verschnitt der Optimierung.
- **Rest**: Plattenrest.

### Lauf: Nummer (Optionen / Restblattbehandlung)

**Zuschnitt > Schneide Optimierung > Optimierung auswählen > [Optionen]**

*(Abbildung J-74 zeigt den Dialog "Lauf: Nummer" mit Optionen zur "Bruchscheibenoptimierung", "Restblattverwaltung", "Nachladen" und "Etikettendruck".)*

In diesem Dialog wird u. a. angegeben, was mit den Bruchscheiben und Restblättern jeder Glasart in der ausgewählten Optimierung geschehen kann oder soll.

#### Erläuterung der Liste Optimierungen
- **Los**: Losnummer der angezeigten Glasart.
- **Glasart**: Artikelnummer der Glasart.
- **Dicke**: Dicke der Glasart in mm.
- **Glasart Bezeichnung**: Bezeichnung der Glasart.
- **Parameter**: Zuschnitttisch der Optimierung.
- **Platten**: Anzahl der Platten für den Zuschnitt.
- **Verschnitt**: Verschnittglasfläche in %.
- **Rest (mm)**: Länge des Restblattes.

#### Erläuterung der Liste Platten
- **Nr.**: Nummer der Lagerplatte.
- **Breite**: Breite der Lagerplatte in mm.
- **Höhe**: Höhe der Lagerplatte in mm.
- **Opt. Gr.**: Optimierungsgruppen auf der Lagerplatte (Lauf oder Nachoptimierung).
- **Schneidstatus**:

| Status | Bedeutung |
| :--- | :--- |
| **Gesendet** | Der Schneidcode wurde erzeugt. |
| **Überspringen** | Kein Schneidcode/Brechbild wird erzeugt. |
| **Kein Schneidcode senden** | Kein Schneidcode, aber ein Brechbild wird erzeugt. |
| **Geschnitten** | Schneidcode wurde vom Tisch empfangen/abgeholt. |

#### Erläuterung der Felder im Bereich Bruchscheibenoptimierung

- **Optimiere Bruchscheiben**: Hier stellen Sie ein, wie mit Bruchscheiben umgegangen werden soll:
  - **Nein**: Keine Nachoptimierung.
  - **Trennen**: Die Nachoptimierung wird am Ende der vorhandenen Optimierung angefügt.
  - **Mischen**: Das letzte Lagerblatt wird komplett neu optimiert, um den Verschnitt zu verbessern.
- **Schneide Bruchscheiben nach Restblattlänge**: Legt fest, ob Bruchscheiben auf ein neues Restblatt optimiert werden, wenn das bisherige nicht ausreicht.
  - ☐ Keine neue Lagerplatte für den Zuschnitt von Bruchscheiben beginnen.
  - ☑ Eine neue Lagerplatte beginnen, wenn das neu entstandene Restblatt kleiner ist als die im nachfolgenden Feld angegebene Länge.
- **Schneide Restblatt unter einer Länge von**: Gibt die maximale Größe des neu entstandenen Restblatts an. Größere Restblätter führen dazu, dass die Bruchscheiben im Bruchpool gesammelt werden.

#### Erläuterung der Felder im Bereich Restblattverwaltung

- **Verlinken**: Legt fest, wie mit Restblättern umgegangen wird.
  - **Nein**: Keine Verlinkung.
  - **Trennen**: Neue Nachoptimierung wird am Ende angefügt.
  - **Mischen**: Scheiben werden auf dem Restblatt aufgelöst und neu optimiert.
- **Restblatt vor dem Schneiden bearbeiten**: Wenn markiert, erfolgt eine Abfrage, ob PlanEdit gestartet werden soll.

#### Erläuterung der Felder im Bereich Schnelloptimierung

- **Schnelloptimierung**:
  - **Standard**: Ermöglicht das Auflösen und Neuoptimieren von Mustern während des Zuschnitts, um Bruchscheiben früher zu integrieren.
  - **Erweitert**: Erfordert Benutzereingaben; öffnet das Glasauswahlmenü, um weitere Optimierungen hinzuzufügen.
- **Nachladen**: Steuert das Laden weiterer Läufe.
  - **Manuell**: Nachladen erfolgt manuell.
  - **Anforderung**: Eine Meldung erscheint, wenn die Anzahl ungeschnittener Muster einen Schwellenwert unterschreitet.
  - **Automatisch**: Das Nachladen erfolgt automatisch.

#### Erläuterung der Felder im Bereich Etikettendruck

- **Aktiv**: Aktiviert oder deaktiviert den Etikettendruck.

#### Erläuterung der Schaltflächen

- **PlanEdit**: Startet das Modul PlanEdit, um die Optimierung grafisch darzustellen.
- **Schneiden**: Startet die Zuschnitt-Übersicht.

#### Erläuterung des Kontextmenüs
- Rechtsklick auf eine Platte mit Status **Geschnitten**: Der Status kann gelöscht und die Platte erneut geschnitten werden.
- Rechtsklick auf eine Platte ohne Status: Der Status kann auf **Kein Schneidcode senden** oder **Überspringen** gesetzt werden.

#### Ergänzende Informationen
- ⇨ Tutorial, “A+W Pattern Viewer" auf Seite J-1113
- ⇨ Tutorial, “A+W Residual Stock Manager" auf Seite J-1104

### Auswahl der zu verlinkenden Optimierung

**Zuschnitt > Schneide Optimierung > Lauf auswählen > [OK] > Dialog Aktiver Lauf: xxx wird geöffnet > Optimierung auswählen > [Start]**

*(Abbildung J-75 zeigt den Dialog "Auswahl der zu verlinkenden Optimierung" mit einer Liste "Verfügbare Optimierungen".)*

Die Liste **Verfügbare Optimierungen** enthält alle Läufe, in denen Optimierungen für die gewählte Glasart und Dicke enthalten sind. Wählen Sie aus der Tabelle den Lauf aus, den Sie verlinken möchten und betätigen Sie anschließend [Verwenden].

#### Erläuterung der Felder im Bereich Auswahl-Parameter und Restblatt

- **Alle Tische**: Wenn aktiv, werden auch Optimierungen für andere Tische angezeigt.
- **Erlaube Handzuschnitt**: Wenn aktiv, werden auch Glasarten angezeigt, die nur für Handzuschnitt vorgesehen sind.
- **Restblatt**: Zeigt an, wie lange das Restblatt ist, das bei der gewählten Optimierung übrig bleibt.

### Optimierungsergebnis

**Zuschnitt > Schneide Optimierung > Lauf auswählen > [OK] > ... > [Verlinken]**

*(Abbildung J-76 zeigt den Dialog "Optimierungsergebnis" mit einem Vergleich der "Neuen Optimierung nach dem Verlinken" und der "Original-Optimierung".)*

Dieser Dialog zeigt Ihnen das Optimierungsergebnis nach dem Verlinken. Er ist in zwei Bereiche unterteilt: **Neue Optimierung nach dem Verlinken** und **Original-Optimierung**. In dem grauen Bereich oberhalb der Schaltflächen sehen Sie, was und wie viel zusätzlich optimiert wurde.

#### Erläuterung der Schaltflächen

- **Wiederholen**: Kehrt zur Auswahl der Linkoptimierung zurück.
- **Verlinken**: Bestätigt das Ergebnis und die Optimierung wird geschnitten.

### Bruchpool

**Zuschnitt > Bruchpool**

*(Abbildung J-77 zeigt den Dialog "Bruchpool" mit einer Liste von Bruchscheiben und einer Detailansicht einer ausgewählten Scheibe, inklusive grafischer Darstellung.)*

Dieser Dialog zeigt alle Scheiben an, die als Bruch gemeldet oder erfasst wurden. Scheiben aus dem Bruchpool können bei passender Glasart und Dicke bei Tischoptimierungen und in der Nachoptimierung erneut optimiert werden.

#### Erläuterung der Liste Bruchscheiben

- **Glasart**: Artikelnummer der Glasart.
- **Bezeichnung**: Bezeichnung der Glasart.
- **Dicke**: Dicke der Glasart in mm.
- **Breite**: Breite der Lagerplatte in mm.
- **Höhe**: Höhe der Lagerplatte in mm.
- **Lauf**: Ursprüngliche Laufnummer der Scheibe.
- **Dynopt**: DynOpt-Flag, das anzeigt, ob die Scheibe vom DynOpt reoptimiert werden kann.
- **Kunde**: Name des Kunden.
- **Auftrag**: Nummer des Auftrags.
- **Pos**: Positionsnummer des Auftrags.
- **Menge**: Anzahl der Scheiben.
- **FormNr.**: Modellnummer, falls es sich um ein Modell handelt.
- **Bock**: Abstellplatznummer (Bock oder Fächerwagen).
- **Etikett-Nr.**: Etikett-Nummer der Bruchscheibe.
- **Los**: Programm-interne Verwendung.

#### Erläuterung der Schaltflächen

- **Aktualisieren**: Aktualisiert die Anzeige, wenn neue Bruchscheiben gemeldet wurden.
- **Löschen**: Löscht die markierte Bruchscheibe aus dem Bruchpool.
- **Modell-Info...**: Startet die Modellscheibenanzeige von A+W Production.
- **Drucken**: Startet einen Ausdruck aller Bruchscheiben (wenn konfiguriert).
- **Hinzufügen**: Ruft den Dialog **Brucherfassung** auf.

#### Erläuterung der Kombobox
Mithilfe der Kombobox können Sie auswählen, zu welchem Tisch der Bruch, den Sie hinzufügen möchten, gebucht werden soll.

#### Ergänzende Informationen
- ⇨ Tutorial, "Bruch, Eilscheiben und Füllaufträge" auf Seite J-1075
- ⇨ Softwarereferenz, “Form-Erfassung" auf Seite J-1148
- ⇨ Softwarereferenz, "Brucherfassung" auf Seite J-1194

### Brucherfassung

**Zuschnitt > Bruchpool > [Hinzufügen]**

*(Abbildung J-78 zeigt den Dialog "Brucherfassung" mit Feldern zur Eingabe von Auftragsdaten und einer Liste der Teile.)*

Mit diesem Dialog können Sie Scheiben erfassen, die zu Bruch gegangen sind und nochmals in eine Optimierung aufgenommen werden sollen.

#### Erläuterung der Felder

- **Auftrag**: Auftragsnummer, zu der die Bruchscheibe gehört.
- **Position**: Positionsnummer des Auftrags.
- **Bruchgrund**: Wählen Sie den Bruchgrund aus der Kombobox. Bruchgründe müssen in den Stammdaten definiert werden.

#### Erläuterung der Liste Teile

- **AuftNr**: Auftragsnummer der Bruchscheibe.
- **TeileNr**: Teilenummer der Scheibe.
- **Bezeichnung**: Bezeichnung der Glasart.
- **Breite**: Breite der Glasart in mm oder inch (konfigurierbar).
- **Höhe**: Höhe der Glasart in mm oder inch (konfigurierbar).

#### Suchfelder

**Zuschnitt > Bruchpool > [Hinzufügen] > <Strg> + <F12>**

Im Dialog **Brucherfassung** können bis zu drei frei konfigurierbare Suchfelder hinzugefügt werden (Searchfield1, Searchfield2, Searchfield3). Die Felder werden über die Formadministration hinzugefügt.

### Modell-Erfassung (im Bruchpool)

**Zuschnitt > Bruchpool > [Modell-Info]**

*(Abbildung J-80 zeigt den Dialog "Form-Erfassung", der identisch mit dem auf Seite J-1148 ist.)*

Die Felder und Schaltflächen diesen Dialoges sind identisch mit den Feldern und Schaltflächen des Dialoges **Form-Erfassung** im Bereich der Eilscheiben. Der Dialog wird an dieser Stelle erläutert.

#### Ergänzende Informationen
- ⇨ Softwarereferenz, "Form-Erfassung" auf Seite J-1148

### A+W DynOpt - Editor

**Zuschnitt > DynOpt Compact ...**

*(Abbildung J-81 zeigt den "XOPT-ON Plus Editor" (A+W DynOpt - Editor) mit Bereichen für "Freigegebene Läufe", "Importierte Läufe" und "Importierte Scheiben" sowie eine "Timeline".)*

Der Editor zeigt Ihnen auf der linken Seite im Bereich **Freigegebene Läufe** alle Feinplanungs-Läufe, die mit DynOpt Compact verarbeitet werden können.

#### Erläuterung der Felder im Bereich Freigegebene Läufe

- **Lauf**: Laufnummer der Feinplanung.
- **Text**: Name der Laufnummer.

Der Bereich **Importierte Läufe** zeigt Ihnen die Läufe, die bereits optimiert oder importiert wurden. Durch das Aufklappen der Baumstruktur können Sie sich nähere Informationen zu dem jeweiligen Lauf anzeigen lassen. Die Baumstruktur zeigt Ihnen:
- **Erste Ebene**: Laufnummer
- **Zweite Ebene**: Abstellplatznummer
- **Dritte Ebene**: Status, Anzahl der Scheiben und Art des Abstellplatzes.

#### Erläuterung der Schaltflächen

- **>**: Verschiebt einen markierten Lauf von **Freigegebene Läufe** nach **Importierte Läufe**.
- **<**: Verschiebt einen markierten Lauf zurück von **Importierte Läufe** zu **Freigegebene Läufe**.
- **^**: Rückt einen markierten Lauf in der Liste **Freigegebene Läufe** eine Stelle nach oben (ändert die Rangfolge).
- **v**: Rückt einen markierten Lauf in der Liste eine Stelle nach unten.

#### Erläuterung der Felder im Bereich Importierte Scheiben

- **Lauf**: Laufnummer der Feinplanung.
- **Sequenzlauf**: Sequenzlauf des Gestells.
- **Laufende Nr.**: Laufende Nummer innerhalb des Laufes.
- **Fach Nr.**: Fachnummer bei Fächerwagen (bei A-Böcken: 0).
- **Glasart**: Artikelnummer der Glasart.
- **Dicke**: Dicke der Scheibe (mm oder inch).
- **Breite**: Breite der Scheibe (mm oder inch).
- **Höhe**: Höhe der Scheibe (mm oder inch).
- **Auftrag**: Auftragsnummer.
- **Pos**: Positionsnummer des Auftrags.
- **Status**: Status der Scheibe.
- **DynOpt Compact Lauf**: Laufnummer der DynOpt Compact Optimierung.
- **DynOpt Compact Los**: Losnummer der DynOpt Compact Optimierung.
- **DynOpt Compact Muster**: Musternummer, auf dem die Scheibe liegt.

Im unteren Bereich des Dialogs wird Ihnen eine **Zeitleiste** angezeigt. Jedes farbige Rechteck kennzeichnet den Zustand eines entsprechenden Abstellplatzes.

| Farbe | Erläuterung |
| :--- | :--- |
| Hellblau | Alle Scheiben des Gestells wurden geschnitten. |
| Blau | Alle Scheiben des Gestells wurden optimiert. |
| Gelb | Scheiben des Gestells wurden teilweise optimiert. |
| Grün | Das Gestell wurde noch nicht optimiert. |

Die Zahlen unter dem farbigen Rechteck zeigen Ihnen die Lauf- und Abstellplatznummer (z.B. 1187/9951).

#### Erläuterung der Felder

- **Status**: Die Kombobox enthält die für DynOpt Compact relevanten Stati:
  - **0**: Unbearbeitet
  - **100**: Komplette Abstellplätze, die jedoch nur teilweise optimiert wurden.
  - **200**: Optimiert.
  - **300**: Geschnitten.
  - **500**: Fehler während der Optimierung.
- **Zeitleisten-Darstellung**: Bestimmt die Art der Ansicht (Zuschnitt oder Optimierung).

#### Erläuterung der Schaltflächen

- **Aktualisieren**: Aktualisiert den Editor.
> **Bilden von DynOpt Compact-Läufen**
> Sie können DynOpt Compact-Läufe aus dem Editor heraus bilden, aber auch aus dem Zuschnitt heraus. Im Editor können Sie einen oder mehrere Läufe markieren und über das Kontext-Menü die Funktion DynOpt Compact-Lauf erzeugen wählen. Im Zuschnitt können Sie das immer nur für einen Lauf tun.

#### Ergänzende Informationen
- ⇨ Tutorial, “A+W DynOpt Compact" auf Seite J-1135

## Einstellungen

Im Menü **Einstellungen** befindet sich folgender Programmpunkt:

- **Tische**:
  Über diesen Menüpunkt greifen Sie auf die konfigurierten Tische zu.
  ⇨ Softwarereferenz, "Einstellungen" auf Seite J-1202
- **Tischoptimierung**:
  Über diesen Menüpunkt greifen Sie auf die Tischoptimierung zu.
  ⇨ Softwarereferenz, “Tischoptimierung" auf Seite J-1203

### Einstellungen > Tische

*(Abbildung J-82 zeigt den Einstellungsdialog für einen Tisch mit Bereichen für "Restplattenlager" und "Zuschnitt".)*

Dieser Dialog steht Ihnen für alle konfigurierten Tische zur Verfügung. Er bietet die Möglichkeit, zur Laufzeit Einstellungen zu ändern, die sonst nur über die Konfigurationsdatei (xopton.cfg) angepasst werden können.

#### Erläuterung der Felder im Bereich Restplattenlager

- **Aktiv**: Steuert, ob das Restplattenlager verwendet wird.
- **Platten einlagern**: Steuert, ob Restplatten in das Restplattenlager gefahren werden.
- **Platten verwenden**: Steuert, ob die Optimierung Restplatten aus dem Restplattenlager verwendet.
- **Mindesteinlagerungslänge**: Mindestlänge in mm, ab der ein Rest eingelagert wird.

#### Erläuterung der Felder im Bereich Zuschnitt

- **Aktiv**: Steuert den Etikettendruck während des Zuschnitts.
- **Restblatt editieren**: Mindestlänge eines Restblatts in mm, damit während des Zuschnitts mit PlanEdit editiert werden kann.

#### Erläuterung der Schaltflächen

- **Übernehmen**: Die Änderungen werden übernommen.
- **Verwerfen**: Die Änderungen werden verworfen.

### Tischoptimierung

**Einstellungen > Tischoptimierung**

*(Abbildung J-83 zeigt einen einfachen Dialog "Einstellungen Tischoptimierung" mit einer Kombobox "Ansicht".)*

Mit diesem Dialog steuern Sie, ob bei der Auswahl der Tischoptimierung das Produktionsdatum mit angezeigt wird oder nicht. Die Kombobox enthält folgende Modi:
- **Standard**: Tischoptimierung ohne Produktionsdatum. (⇨ Seite J-1157)
- **Produktionsdatum**: Tischoptimierung mit Produktionsdatum. (⇨ Seite J-1159)

## Ansicht

Im Menü **Ansicht** befinden sich folgende Programmpunkte:
- **Import starten und beenden** (nur bei A+W Realtime Optimizer Stand alone): Startet und beendet den Import.
  ⇨ Softwarereferenz, "Import" auf Seite J-1205
- **Fehlermeldungen**: Greift auf die Fehlermeldungen zu.
  ⇨ Softwarereferenz, “Fehlermeldungen" auf Seite J-1206
- **Statusleiste**: Blendet die Statusleiste ein oder aus.

### Import

**Ansicht > Import**

*(Abbildung J-84 zeigt den "Import"-Dialog, der ein Log-Fenster mit dem Status von Datei-Importen anzeigt.)*

Mit diesem Dialog wird das Arbeitsverzeichnis für Importdateien überwacht und der Status des Imports angezeigt. Fehlerfrei importierte Läufe stehen im Dialog **Wählen Sie einen Lauf aus** zur weiteren Bearbeitung bereit.

#### Erläuterung der Schaltflächen

- **Start**: Überwacht das Arbeitsverzeichnis und importiert neue Dateien automatisch. Die Schaltfläche wechselt zu **Stopp**.
- **Stopp**: Beendet die Importfunktion. Die Schaltfläche wechselt zu **Start**.

#### Ergänzende Informationen
- ⇨ Tutorial, "Optimierungen importieren" auf Seite J-1071

### Fehlermeldungen

**Ansicht > Fehlermeldungen**

*(Abbildung J-85 zeigt den Dialog "Fehlermeldungen" mit Bereichen für "Es ist folgender Fehler aufgetreten" und "Bisherige Fehler".)*

In diesem Dialog wird ein aktuell vorliegender Fehler und alle bisherigen Fehler (seit dem letzten Programmstart) angezeigt.

- **Es ist folgender Fehler aufgetreten**: Zeigt einen neu aufgetretenen Fehler an.
- **Bisherige Fehler**: Zeigt alle bisher aufgetretenen Fehler an.
- **Fehlerdatei** (Schaltfläche): Speichert den Inhalt dieses Dialogs in einer Fehlerdatei.

## A+W Residual Stock Manager

Mit dem A+W Residual Stock Manager können Sie Restplatten ohne maschinelle Unterstützung speichern und bearbeiten. Hierfür gibt es eine Weboberfläche (A+W Planning Web), die über einen Browser von überall geöffnet werden kann. Die eingelagerten Restplatten stehen anschließend automatisch im A+W Realtime Optimizer zur weiteren Verarbeitung zur Verfügung.

### A+W Planning Web

In diesem Modul nehmen Sie die Konfiguration für den A+W Residual Stock Manager vor.

> **A+W Planning Web-Konfiguration**
> Die Standard-Konfiguration wird bei der Installation durch A+W-Mitarbeiter vorgenommen. Wir erläutern in dieser Dokumentation, wie Sie Lager, Abstellplätze und Gestelle im A+W Planning Web anlegen.

#### Lager

**A+W Planning Web > Lager > Stammdaten**

*(Abbildung J-86 zeigt die Stammdaten-Seite für "Lager" mit einer Liste bestehender Lager und Optionen zum Bearbeiten, Hinzufügen und Löschen.)*

In diesem Bereich werden Ihnen alle in Ihrem Hause angelegten Lager angezeigt. Sie können bestehende Lager ändern, neue Lager hinzufügen oder bestehende Lager löschen.

##### Erläuterung der Felder

- **ID**: Eindeutiger numerischer Schlüssel.
- **Bezeichnung**: Eindeutiger Name für Ihr Lager.

##### Erläuterung der Schaltflächen

- **Bearbeiten**: Öffnet das Register **Abstellplatz**, wo alle Abstellplätze für das Lager angezeigt werden.
- **Speichern**: Speichert alle vorgenommenen Änderungen.
- **Hinzufügen**: Fügt ein weiteres Lager hinzu.
- **Löschen**: Löscht das gewählte Lager (ohne Sicherheitsabfrage).
- **Aktualisieren**: Aktualisiert die Anzeige.
- **[< Lager]**: Kehrt zur Übersicht der einzelnen Lager zurück.

##### Ergänzende Informationen
- ⇨ Tutorial, "Lager" auf Seite J-1106

#### Abstellplatzinformationen

**A+W Planning Web > Lager > Stammdaten > Schaltfläche [Bearbeiten]**

*(Abbildung J-87 zeigt die Übersicht der Abstellplätze für ein ausgewähltes Lager.)*

In diesem Dialog werden Ihnen alle Abstellplätze angezeigt, die für das entsprechende Lager angelegt sind.

##### Erläuterung der Felder

- **Oben links**: Zeigt an, wo Sie sich gerade befinden (z.B. Stammdaten > Übersicht der Abstellplätze).
- **ID**: Eindeutiger numerischer Schlüssel für den Abstellplatz.
- **Bezeichnung**: Eindeutiger Name zur Identifizierung des Abstellplatzes.
- **Lagertyp**: Gibt den Typ des Abstellplatzes an (z.B. Lagerplatz, Lagereingang).
- **Zuordnungsstatus**: Gibt an, ob der Abstellplatz verwendet werden kann oder gesperrt ist.

##### Erläuterung der Schaltfläche

- **Lager**: Kehrt zurück zur Übersicht der einzelnen Lager.
- **Speichern**: Speichert Änderungen.
- **Hinzufügen**: Fügt einen neuen Abstellplatz hinzu.
- **Löschen**: Löscht den gewählten Abstellplatz.
- **Aktualisieren**: Aktualisiert die Anzeige.

##### Ergänzende Informationen
- ⇨ Tutorial, "Abstellplätze" auf Seite J-1107

#### Gestelle

**A+W Planning Web > Lager > Stammdaten > Abstellplatz > Schaltfläche [Bearbeiten]**

*(Abbildung J-88 zeigt die Übersicht der Gestelle für einen ausgewählten Abstellplatz.)*

In diesem Dialog werden Ihnen alle Gestelle angezeigt, die für den entsprechenden Abstellplatz angelegt sind. Scheiben können ausschließlich auf Gestellen verbucht werden.

##### Erläuterung der Felder

- **ID**: Eindeutiger numerischer Schlüssel für das Gestell.
- **Bezeichnung**: Eindeutiger Name zur Identifizierung des Gestells.
- **Zuordnungsstatus**: Gibt an, ob das Gestell verwendet werden kann oder gesperrt ist.
- **Eigenschaften**: Zeigt die Gestellart an (z.B. Fächerwagen, A-Bock).

##### Erläuterung der Schaltfläche
- **Abstellplatz**: Kehrt zurück zur Übersicht der einzelnen Abstellplätze.
- Weitere Schaltflächen (Speichern, Hinzufügen, Löschen, Aktualisieren) funktionieren wie oben beschrieben.

##### Ergänzende Informationen
- ⇨ Softwarereferenz, "Gestelle" auf Seite J-1211

#### Gestelleigenschaften

**A+W Planning Web > Lager > Stammdaten > Schaltfläche [Gestelleigenschaften]**

*(Abbildung J-89 zeigt eine Tabelle mit den Eigenschaften verschiedener Gestelltypen, wie Zugangsart, Maße, Gewicht etc.)*

In diesem Bereich werden Ihnen die Eigenschaften der unterschiedlichen Gestelltypen angezeigt. Sie können Änderungen vornehmen, aber auch neue Gestelle anlegen.

##### Erläuterung der Felder

- **Bezeichnung**: Eindeutiger Name für einen Gestelltyp.
- **Zugangsart**: Beschreibt, wie Glas auf- oder abgestapelt wird:
  - **Frei**: Wahlfreier Zugriff (z. B. Fächerwagen).
  - **First in, First out (FiFo)**: Nur das zuerst eingelagerte Glas kann entnommen werden.
  - **Last in, First out (LiFo)**: Nur das zuletzt eingelagerte Glas kann entnommen werden (z. B. A-Bock).
- **Maximalgewicht**: Maximalgewicht in kg.
- **Maximale Höhe/Breite/Tiefe**: Maximale Abmessungen.
- **Minimale Höhe/Breite**: Minimale Abmessungen.
- **Maximalanzahl der Stapel/Fächer**: Maximale Anzahl an Stapeln oder Fächern. Bei -1 ist die Anzahl unbegrenzt.
- **Segmenttyp**: Art des Gestelltyps:
  - **HarpRack**: Fächerwagen
  - **LRack**: L-Gestell
> **A-Gestell**
> Zur Konfiguration eines A-Bocks müssen zwei L-Gestelle angelegt werden!

##### Erläuterung der Schaltfläche
- Die Schaltflächen (Speichern, Hinzufügen, Löschen, Aktualisieren) funktionieren wie oben beschrieben.

##### Ergänzende Informationen
- ⇨ Softwarereferenz, "Gestelleigenschaften" auf Seite J-1213

### Glasübersicht

**A+W Planning Web > Lager > Übersicht**

*(Abbildung J-90 zeigt die "Glasübersicht", eine tabellarische Ansicht aller eingelagerten Restblätter mit Details und Filteroptionen in den Spaltenköpfen.)*

In diesem Bereich werden Ihnen alle Restblätter angezeigt, die eingelagert wurden. Die Daten können in der Ansicht editiert werden. Über die Filterfunktionen in den Überschriften des Tabellenkopfes können Sie die Ergebnisse der Anzeige einschränken.

#### Erläuterung der Felder

- **Typ**: Glastyp (Restblatt, Lagerblatt, Scheibe). Filterbar.
- **Abstellplatzinformationen**: Informationen zum Abstellplatz der Glasscheibe. Filterbar.
- **Glastyp**: Glastyp der eingelagerten Glasscheibe. Filterbar.
- **Etikettennr.**: Etikettnummer für eingelagerte Scheiben. Filterbar.
- **Breite**: Breite der Glasscheibe. Filterbar nach Wert und Eigenschaft (größer, kleiner, gleich).
- **Höhe**: Höhe der Glasscheibe. Filterbar nach Wert und Eigenschaft.
- **Info**: Zusätzliche Information. Filterbar nach Wert und Eigenschaft (gleich, beinhaltet, Startwert).
- **Zuordnungsstatus**: Status des Abstellplatzes. Filterbar.
- **Datum**: Datum der Einlagerung. Filterbar.

#### Erläuterung der Schaltflächen

- **Neuen Datensatz hinzufügen**: Öffnet einen Dialog, um Daten für einen neuen Datensatz einzugeben.
- **Verwendbare Restblätter hervorheben**: Hebt alle verwendbaren Restblätter in der Tabelle hervor, unter Berücksichtigung der Zugangsart des Gestells.
- **Bearbeiten**: Gibt den Datensatz zur Bearbeitung frei.
- **Löschen**: Löscht den Datensatz.
- **Drucken**: Löst den Etikettendruck aus.

#### Ergänzende Informationen
- ⇨ Softwarereferenz, "Glasübersicht" auf Seite J-1215

### Neuen Datensatz hinzufügen/bearbeiten

**A+W Planning Web > Lager > Übersicht > [Neuen Datensatz hinzufügen] / [Editieren]**

*(Abbildung J-91 zeigt den Dialog zum Hinzufügen/Bearbeiten eines Datensatzes mit Komboboxen und Eingabefeldern für Lager, Abstellplatz, Gestell, Glastyp, Maße etc.)*

In diesem Dialog können Sie bestehende Datensätze editieren oder neue Datensätze anlegen.

#### Erläuterung der Felder

- **Lager**: Wählen Sie das entsprechende Lager aus.
- **Abstellplatzinformationen**: Wählen Sie den entsprechenden Abstellplatz aus.
- **Gestell**: Wählen Sie das entsprechende Gestell aus.
- **Gruppe**: Wählen Sie die entsprechende Gruppe aus.
- **Glastyp**: Wählen Sie den entsprechenden Glastyp aus.
- **Breite/Höhe**: Geben Sie die entsprechenden Abmessungen ein.
- **Info**: Geben Sie einen zusätzlichen Text als Information ein.
- **Zuordnungsstatus**: Wählen Sie den entsprechenden Zuordnungsstatus aus.
- **Datum**: Wählen Sie aus dem Kalender das Datum aus, an dem das Restblatt eingelagert wurde.

#### Ergänzende Informationen
- ⇨ Tutorial, "Übersicht" auf Seite J-1110

---

# A+W Production Terminal

## Vorspann

In diesem Teil der Dokumentation finden Sie die editorischen Notizen.

### Revisionsübersicht

| Version / Datum | Beschreibung |
| :--- | :--- |
| 1.50 / 01-2023 | Diverse Ergänzungen |
| 1.30 / 01-2016 | Nachläufer-Verwaltung ergänzt |
| 1.20 / 09-2014 | Terminal Georgian Bars ergänzt |
| 1.10 / 04-2013 | Terminal LG und Edit ergänzt |
| 1.00 / 01-2012 | Ersterstellung |

### Editorial

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender des Production Terminal (Terminal) gedacht.
Diese Dokumentation und die darin beschriebene Software werden nur in Lizenz vergeben und dürfen nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Dieses Dokument beschreibt die volle Ausbaustufe des Production Terminal.

#### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, noch mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

---

## Tutorial

### Überblick

Die Schulung zu den A+W Production Terminal-Modulen ist für Mitarbeiter konzipiert, die in der Produktion an den entsprechenden Erfassungsstellen arbeiten.
Wir vermitteln dem Mitarbeiter, wie er mit Hilfe unserer Software seine Arbeitsabläufe effizienter und einfacher ausführen kann und wie er auf Störungen usw. eingeht.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- Production Terminal Systeme
- Überblick A+W Production Terminal IG
- Überblick A+W Production Terminal Manual Cutting
- Überblick A+W Production Terminal Order
- Überblick A+W Production Terminal Processing
- Überblick A+W Production Terminal TG

#### Vorausgesetzte Kenntnisse
EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei der Anwendung der entsprechenden Module vorausgesetzt. Der Mitarbeiter muss wissen, wie die physischen Arbeitsabläufe und Prozessschritte an der entsprechenden Arbeitsstation aussehen und auszuführen sind.

### Dokumentation

Für die Schulung stehen folgende Unterlagen zur Verfügung:

- **Handout**: Ausdruck Schulungsunterlage für die Teilnehmer
- **PDF**: Vollständige Unterlagen (Tutorial, Softwarereferenz)
- **Online-Hilfe <F1>**: Kontextsensitive Dialog-Hilfe der Softwarereferenz

#### Aufbau des Tutorials
- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über Lernziele, Nutzen und Merksätze.
- **Konzepte**: Begriffe der jeweiligen Lerneinheit werden erläutert.
- **Lesehinweis**: Der Inhalt baut auf vorherigen Einheiten auf. Es ist sinnvoll, keine Einheiten zu überspringen.

### Darstellungskonventionen

- *Kursiv*: Zeichenfolgen, die sich auf Elemente der Software beziehen, z. B. der Dialog *Muster senkrecht/waagerecht*.
- **Fett**: Zeichenfolgen, die Sie über die Tastatur eingeben, z. B. geben Sie den Wert **0** ein.
- **>**: Der Brotkrumenpfad, der den Weg zum Öffnen eines Dialogs kennzeichnet, z. B. *Datei > Importieren > Übergabedatei*.
- **[]**: Bezeichnen Schaltflächen im Dialog, z. B. mit [OK] speichern Sie die Daten.
- **<>**: Bezeichnen Tasten oder Tastenkombinationen, z. B. mit <F1> öffnen Sie die Online-Hilfe.

### Production Terminal Systeme

Die A+W Production Terminals sind Softwaremodule des Produktionssteuerungssystems A+W Production, mit denen Prozessschritte im Produktionsablauf gesteuert, erfasst, modifiziert, kontrolliert und umgelenkt werden können. Sie visualisieren und steuern einzelne Prozessschritte, sind individuell konfigurierbar und ermöglichen den Online-Druck von Etiketten und Reports sowie die Erfassung von Bruchscheiben.

*(Abbildung 1 zeigt eine schematische Darstellung einer A+W Production Terminal-Landschaft mit verschiedenen Terminals wie Terminal Manual Cutting, Terminal Processing, Terminal IG-In/Out/Assembly, Terminal LG-In/Out, etc.)*

Da an jedem Arbeitsplatz in der Produktion andere Informationen erforderlich sind, gibt es für verschiedene Prozesse und Arbeitsabläufe entsprechend konfigurierte Standard-Schirme.

#### Kurze Erläuterung zu den einzelnen Terminals:

- **Terminal Manual Cutting**: Visualisiert am Handzuschnitttisch den Arbeitsplan.
- **Terminal Order**: Kommt überall dort zum Einsatz, wo größere Mengen gebucht werden.
- **Terminal Processing**: Steuert Bearbeitungsmaschinen an und gibt detaillierte Auskunft über Bearbeitungen.
- **Terminal IG-In**: Visualisiert am Einlauf der Isolierglaslinie den Arbeitsplan.
- **Terminal IG-Assembly**: Wird zwischen Scheibenkontrolle und Rahmensetzstation installiert und visualisiert technische Daten inkl. Rahmendaten.
- **Terminal IG-Out**: Visualisiert am Auslauf der Isolierglaslinie technische und versandorientierte Daten.
- **Terminal TG-In**: Anzeigesystem am Ofeneinlauf. Zeigt Belegung des Ofenbettes.
- **Terminal TG-Out**: Anzeigesystem am Ofenauslauf. Zeigt alle registrierten Scheiben an.
- **Terminal Edit**: Variante des Leitrechners, i.d.R. im Versandbüro, um Einheiten, Scheiben oder Gruppen umzubuchen.
- **Terminal LG-In**: Visualisiert am Einlauf der VSG-Linie den Arbeitsplan.
- **Terminal LG-Assembly**: Visualisiert im Reinraum den Arbeitsplan, sobald eine Scheibe am Terminal LG-In gebucht wurde.

#### Ziele der Leitrechner-Technologie

- Geplante Jobs/Lose auf Arbeitsplätze verteilen.
- Arbeiter mit relevanten Informationen (Form, Maß, Bearbeitung) grafisch unterstützen.
- Durchgeführte Arbeiten buchen.
- Abweichungen erfassen.
- Soll- und Ist-Arbeitsweise abgleichen.
- Produktionsfortschritt anzeigen.
- Nachläufer (wegen Bruch) automatisch generieren.
- Produktionsablauf manuell nachoptimieren.
- Gesammelte Daten für Auswertungen nutzen.

> **Performance Zähler**
> In den Leitrechnern können zusätzliche Felder eingeblendet werden, welche die produzierte Menge, Fläche und Laufmeter für eine bestimmte Zeit an einer Erfassungsstelle anzeigen.

#### Bedienung der Leitrechner

Um schnell und effektiv zu arbeiten, werden Barcodes an relevanten Stellen eingesetzt. Mit Barcode-Scannern können Produktionsfaktoren, Prozesse oder Zustände identifiziert werden, z.B.:
- Scheiben (Einzelne oder Gruppen)
- Gestelle
- Mitarbeiter
- Bearbeitungen
- Brüche

### Überblick A+W Production Terminal IG

In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit dem A+W Production Terminal IG (Terminal IG) kennen. Der Themenblock beinhaltet folgende Schulungseinheiten:
- Arbeiten mit Terminal IG-In
- Arbeiten mit Terminal IG-Assembly
- Arbeiten mit Terminal IG-Out

### Arbeiten mit Terminal IG-In

#### Lernziele
- Die Oberfläche von *Terminal IG-In* kennenlernen.
- Die Funktionsweise kennenlernen und verstehen.
- Arbeitsunterbrechungen korrekt durchführen.
- Mit unvorhersehbaren Situation (z. B. fehlendes Material) umgehen lernen.

#### Nutzen
Terminal IG-In hilft Ihnen, die Scheiben einer Einheit in der korrekten Reihenfolge vom Gestell auf die Linie zu stellen.

#### Definitionen
- **Barcode**: Optoelektronisch lesbare Schrift aus Strichen und Lücken.
- **Lauf**: Eine Menge von Positionen, die gemeinsam verplant und produziert werden.
- **Los**: Eine Menge von Teilen, deren Bearbeitungen gleichzeitig auf derselben Maschine gefertigt werden.
- **Nachläufer**: Eine Scheibe, die aufgrund von Bruch oder Mangel erneut geschnitten wurde.
- **Charge**: Eine Gütermenge mit gleichen Eigenschaften.
- **Bruch**: Eine mangelhafte Scheibe, die nicht verwendet werden kann.
- **Produktionsnummer**: Definiert/visualisiert die Produktionsreihenfolge innerhalb eines Laufes.
- **Scannen**: Das Lesen einer oder mehrerer Barcodes.
- **Buchen**: Das Schreiben und Speichern von Daten in die Datenbank.

#### Merke
- Arbeitsunterbrechungen müssen immer protokolliert werden.
- Bruchgründe müssen immer dokumentiert werden.

### Modul-Präsentation Terminal IG-In

*(Abbildung 2 zeigt die Benutzeroberfläche des "Production Terminal IG-In" mit Daten. Bereiche sind mit Buchstaben A bis L markiert.)*

- **A**: Menüleiste
- **B**: Produktionsnummer mit Bezeichnung
- **C**: Modellanzeige
- **D**: Farbliche Darstellung der Einheit
- **E**: Liste der aktuellen Einheit
- **F**: Vorschauliste
- **G**: Infofelder
- **H**: Schaltflächen
- **I**: Laufnummer/Losnummer
- **J**: Sprossenansicht
- **K**: Verlinkte Dokumente
- **L**: Produktionshinweistexte

Im oberen Bereich befindet sich die Menüleiste (A), darunter die aktuelle Produktionsnummer und Bezeichnung (B). Bereich (C) zeigt das Modell und die Maße. (D) ist die farbliche Darstellung der Einheit. (E) ist die Liste der aktuellen Einheit. (F) ist eine Vorschau auf die nächste Einheit, (G) die Infofelder, und (H) die Schaltflächen.

#### Detaillierte Erläuterung zu den einzelnen Bereichen

> **Anzeige der Spalten ist frei konfigurierbar**
> Die Anzeige der Spalten ist frei konfigurierbar. Daher kann die gezeigte Bildschirmdarstellung von Ihrer Darstellung abweichen.

##### Bereich A - Menüleiste
Die Menüleiste beinhaltet die für den Anwender wichtigsten Funktionen.

##### Bereich B - Produktionsnummer und Bezeichnung
Zeigt die aktuelle Produktionsnummer und die Artikelbezeichnung der Einheit.
`22 IG 4/16/Th4 A+W`

##### Bereich C - Modellanzeige
Zeigt das Modell mit den Abmessungen an.
`1000 X 1200`
