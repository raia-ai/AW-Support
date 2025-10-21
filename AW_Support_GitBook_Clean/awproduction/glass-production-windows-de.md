---
title: "D-AWProduction-HB_15"
source: "D-AWProduction-HB_15.pdf"
tags: ["A+W Production Terminal", "Software Manual", "Technical Documentation", "Glass Production", "Window Manufacturing", "Terminal Edit", "Terminal IG", "Softwarereferenz", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive user manual for the A+W Production Terminal software, covering both a tutorial overview and an in-depth software reference. It details the functionalities of various modules like Terminal Edit, Terminal IG, Manual Cutting, and others, explaining procedures for data handling, user login, and operational workflows in a glass and window production environment."
long_description: "This document serves as a detailed guide and software reference for the A+W Production Terminal, a system designed for managing and monitoring production processes in the glass, window, and door manufacturing industry. The manual is divided into two main parts: a Tutorial and a Softwarereferenz (Software Reference). The Tutorial section provides a step-by-step guide on using the A+W Production Terminal Edit module, covering the workflow from logging in, loading source data (from stations or racks), to transferring data between source and target areas. The Softwarereferenz section offers an exhaustive description of all modules and their functions, including Terminal IG (for insulating glass lines), Terminal Manual Cutting, Terminal Georgian Bars, Terminal Order, Terminal Processing, and Terminal TG (for tempering furnaces). It explains the user interface elements like buttons, combo boxes, and menus, and provides a complete list of keyboard shortcuts. Detailed explanations are given for core processes such as registering breakages (Bruch buchen), loading remakes (Nachläufer laden), changing machine statuses, and managing orders. The document also covers administrative functions like report generation, log file exportation, and language selection. It is intended for operators, supervisors, and technical staff who use the A+W Production Terminal to manage daily production tasks."
---

# Tutorial

## Überblick A+W Production Terminal Edit

### Bereich J - Schaltflächen zum Verschieben der Daten
Mit diesen Schaltflächen können Sie die Daten aus dem Quellbereich in den Zielbereich verschieben oder auch umgekehrt.

### Bereich L - Schaltflächen
Die Schaltfläche Aktualisieren [F2] dient dem Auffrischen der Anzeige.
Über die Schaltfläche [Reset] leeren Sie die Anzeige.
Betätigen Sie die Schaltfläche Übernehmen [F5], werden die Daten von der Quelle auf das Ziel gebucht.

## Ablauf von Arbeitsschritten
Die Vorgehensweise zum Arbeiten in Terminal Edit ist:
- Starten Sie das Modul Terminal Edit.
- Melden Sie sich an (<Name>).
- Laden Sie die Quelldaten.
- Bei Erfassungsstellen wählen Sie das Gestell aus.
- Wählen Sie den Zielbereich aus.
- Buchen Sie die Daten vom Quellbereich auf den Zielbereich.

### Anmelden an der Arbeitsstation
Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich. Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
- Tutorial, "So melden Sie sich an" auf Seite 1240

### So laden Sie eine Erfassungsstelle
1. Öffnen Sie im Feld Erf.-Stelle die Kombobox und wählen Sie die entsprechende Erfassungsstelle aus. Alternativ dazu können Sie auch die erste Ziffer der Erfassungsstelle tippen. Es werden anschließend alle Erfassungsstellen angezeigt, die mit dieser Ziffer beginnen.
2. Wählen Sie die entsprechende Erfassungsstelle aus.
3. Betätigen Sie die Schaltfläche [Hinzufügen].
4. Die Daten werden geladen.

### So laden Sie ein Gestell
1. Öffnen Sie im Feld Gestell die Kombobox und wählen Sie das entsprechende Gestell aus. Alternativ dazu können Sie auch die erste Ziffer des Gestells tippen. Es werden anschließend alle Gestelle angezeigt, die mit dieser Ziffer beginnen.
2. Wählen Sie das entsprechende Gestell aus.
3. Betätigen Sie die Schaltfläche [Hinzufügen].
4. Die Daten werden geladen.

### So laden Sie einen Auftrag, einen Lauf oder ein Etikett
1. Entscheiden Sie, ob Sie eine Auftragsnummer, eine Laufnummer oder eine Etikettnummer laden wollen und wählen Sie in der Kombobox den entsprechenden Eintrag Auftrag, Lauf oder Etikett.
2. Geben Sie im Feld darunter die entsprechende Nummer ein.
3. Betätigen Sie die Schaltfläche [Hinzufügen].
4. Die Daten werden geladen.

### So buchen Sie einen LKW außer Haus
1. Öffnen Sie im Bereich Quelle die Kombobox Erf.-Stelle oder ES-Typ. Wählen Sie den Eintrag LKW.
2. Betätigen Sie die Schaltfläche [Hinzufügen]. Die Daten werden geladen.
3. Öffnen Sie im Bereich Ziel die Kombobox Zustand. Wählen Sie den Eintrag Ausgeliefert.
4. Betätigen Sie die Schaltfläche [Hinzufügen]. Die Daten werden geladen.
5. Wählen Sie im Bereich Quelle aus der Liste den LKW aus, den Sie umbuchen möchten. Sie können auch alle LKWs auswählen und mit einem Klick umbuchen.
6. Betätigen Sie die Schaltfläche zum Verschieben.
7. Die Daten werden vom Quell- in den Zielbereich verschoben.
8. Betätigen Sie die Schaltfläche [Übernehmen]. Die Daten werden gebucht.

> **Daten versehentlich oder falsch gebucht**
> Sollten Sie Daten versehentlich gebucht haben, können Sie auf die oben beschriebene Art und Weise die Daten aus dem Zielbereich wieder in den Quellbereich verschieben.

### So passen Sie den Tabellenkopf im Bereich der Quelldaten an
Das Erscheinungsbild von Terminal Edit wird bei der Installation konfiguriert. Sollten Sie im Laufe der Zeit feststellen, dass Sie gerne zusätzliche Felder angezeigt bekommen möchten, oder auch vorhandene Felder überflüssig geworden sind, gehen Sie wie folgt vor.
1. Wählen Sie die Erf.-Stelle oder das Gestell aus.
2. Betätigen Sie die Schaltfläche [Hinzufügen]. Die Daten werden geladen.
3. Der Dialog Auftrag laden wird geöffnet.
4. Wählen Sie den gewünschten Auftrag aus.
5. Betätigen Sie die Schaltfläche [Laden].
6. Der Dialog wird geschlossen und der gewählte Auftrag wird geladen. Sie befinden sich jetzt wieder im Hauptfenster.

### Weitere Funktionen
Zu den weiteren Funktionen zählen:
- Listen (Reports)
- Log-Einträge
- Unterschiedliche Programm-Sprachen

Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal beschrieben.

**Ergänzende Informationen**
- Tutorial, "Listen (Reports) generieren" auf Seite 1247
- Tutorial, "Log-Einträge exportieren" auf Seite 1247
- Tutorial, "Programmsprache wählen" auf Seite 1248
- Softwarereferenz, "Logeinträge für Sitzung" auf Seite 1386

# Softwarereferenz

## Bedienung der Module
Die Module starten Sie entweder über einen Desktop-Shortcut, oder über den entsprechenden Eintrag im Menü Start > Programme (unter Windows).
Im Anschluss finden Sie Erläuterungen zu den in der Dokumentation verwendeten Begriffe und wie Sie das Programm beenden.
- Softwarebegriffe
- Programm beenden

### Softwarebegriffe
In diesem Abschnitt wird Ihnen der allgemeine Umgang mit den Menüs und den Dialogen vorgestellt.
Nachfolgend erhalten Sie Informationen zu:
- Schaltflächen
- Optionsschalter
- Kombobox
- Menüleiste/Menüpunkt
- Tastaturbefehle

### Schaltflächen
**Beispiel:** Bruch [F7]

### Optionsschalter
**Beispiel:** Scheiben: Alle / Verfügbare
In einem Rahmen mit Optionsschaltern kann immer nur eine Option angewählt werden! In der Abbildung oben ist die Option Senkrecht angewählt. Klicken Sie z. B. nun die Option Waagerecht an, wird automatisch die Option Senkrecht abgewählt.

### Kombobox
**Beispiel:**
- Sprache
- German (Germany)
- English (United States)
- French (France)
- German (Germany)

Wenn Sie in einer Kombobox auf den Pfeil rechts klicken, öffnet sich eine Auswahlliste. Wählen Sie aus dieser Liste den gewünschten Eintrag durch Anklicken aus. Ihre Auswahl wird in der Anzeige dargestellt.

### Menüleiste/Menüpunkt
Auch Pull-Down-Menü-Leiste genannt. Wenn Sie z. B. eine Fassadenanlage erstellen möchten, klicken Sie mit der Maus auf den Menüeintrag Makros, das entsprechende Pull-Down- Menü öffnet sich (siehe Abbildung oben) und hier auf den Menüeintrag Fassadenanlage.
**Beispielmenü:**
- Datei
- Listen
- Maschine
- Extras
- Ummelden [F4]
- Springe zu ProdNr [F11]
- Vorschau-Dialog [F12]
- Charge [F1]
- Beenden

### Tastaturbefehle
Tastaturbefehle sind Tasten oder Tastenkombinationen, mit denen ein Befehl aufgerufen bzw. eine Funktion ausgeführt wird. Tastaturbefehle helfen dem geübten Benutzer schnell zum gewünschten Ergebnis zu gelangen. Nachfolgend erhalten Sie einen Überblick über die wichtigsten Tastaturbefehle und Funktionstasten:

| Tastaturbefehl | Erläuterung |
| :--- | :--- |
| **[F1]** | Mit dieser Funktionstaste erfassen Sie eine Charge. Der Dialog Manuelle Eingabe wird geöffnet. |
| **[F2]** | Wenn Sie diese Funktionstaste betätigen, können Sie ein neues Los laden. Der Dialog Lade Los wird geöffnet. |
| **[F3]** | Mit dieser Funktionstaste bringen Sie die Maschine in einen anderen Zustand. Der Dialog Status wird geöffnet. |
| **[F4]** | Mit dieser Funktionstaste melden Sie eine Person an der Maschine an. Der Dialog ToolTV Anmeldung wird geöffnet. Sie können mit dieser Taste auch zwischen mehreren Schirmen umschalten. |
| **[F5]** | Wenn Sie diese Funktionstaste betätigen, wird die aktuelle Einheit in den Status produziert gebucht. |
| **[F6]** | Wenn Sie diese Funktionstaste betätigen, wird die aktuelle Einheit übersprungen und die nächsten Einheit zur Produktion angezeigt. Es erfolgt keine Buchung. |
| **[F7]** | Wenn Sie diese Funktionstaste betätigen, wird die aktuelle Scheibe zu Bruch gebucht. Der Dialog Zustand wird geöffnet. |
| **[F8]** | Wenn Sie diese Funktionstaste betätigen, können Sie einen Nachläufer laden. Der Dialog Nachläufer laden wird geöffnet. |
| **[F11]** | Mit dieser Funktionstaste können Sie eine andere Produktionsnummer laden. Der Dialog Gehe zu Produktionsnummer wird geöffnet. |
| **[F12]** | Mit dieser Funktionstaste starten Sie die Vorschau. Der Dialog Vorschau wird geöffnet. |

**Aktive bzw. inaktive Schaltflächen**
In den verschiedenen Programmdialogen finden Sie aktive und inaktive Schaltflächen vor. Die Schaltflächen werden abhängig von den Eingaben aktiv oder inaktiv!

### Programm beenden
Es bestehen verschiedene Möglichkeiten das Programm zu beenden.
- Mausklick auf die Schaltfläche [Schließen] in der rechten oberen Programm-Fensterecke beendet das Programm.
- Über das Menü Datei > Beenden.

> **Hinweis zum Beenden**
> Wurden Daten geändert bzw. neue Daten erfasst, die noch nicht gesichert wurden, erscheint ein entsprechender Hinweis. Wählen Sie [Ja] um den Dialog Datei speichern unter zu aktivieren. Sie können hier die Datei bzw. Ihre Änderungen speichern. Anschließend wird das Programm beendet. Wählen Sie [Nein] um das Programm ohne Speichern der Datei bzw. der Änderungen zu beenden. Wählen Sie [Abbrechen] um den Vorgang Beenden abzubrechen und mit dem Programm weiter zu arbeiten.

## Übersicht allgemein
In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
- Terminal IG
- Terminal Manual Cutting
- Terminal Order
- Terminal Processing
- Terminal TG
- Reports
- Die Hilfe verwenden

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass Dialoge und Funktionen auf verschiedenen Wegen geöffnet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.

## Übersicht Terminal IG
Terminal IG kommt an der Isolierglas-Linie zum Einsatz und zeigt Ihnen alle verfügbaren Lose inklusive produktionsunterstützender Informationen.

Die Module Terminal IG-In, Terminal IG-Assembly und Terminal IG-Out haben die gleichen Menüs:
- Menü Datei
- Menü Listen
- Menü Maschine
- Menü Extras (für A+W-Mitarbeiter)
- Menü ?

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
- **Menü Datei, Menü-Eintrag Ummelden:**
  Mit diesen Menüpunkt melden Sie sich am Terminal an.
  - Softwarereferenz, "Registrierung" auf Seite 299
- **Menü Datei, Menü-Eintrag Springe zu ProdNr. [F11]:**
  Mit diesem Menüpunkt können Sie direkt zu einer anderen Produktionsnummer springen.
  - Softwarereferenz, "Gehe zu Produktionsnummer" auf Seite 300
- **Menü Datei, Menü-Eintrag Vorschau-Dialog [F12]:**
  Mit diesem Menüpunkt öffnen Sie die Dialog Vorschau.
  - Softwarereferenz, "Vorschau" auf Seite 301
- **Menü Datei, Menü-Eintrag Charge [F1]:**
  Wählen Sie diesen Menüpunkt um Chargen zuzuweisen.
  - Softwarereferenz, "Charge" auf Seite 303
- **Menü Listen, Menü-Eintrag Auftragsübersicht:**
  Mit diesen Menüpunkt drucken Sie den Report Auftragsübersicht.
  - Softwarereferenz, "Parametereingabe für Report" auf Seite 340
- **Menü Maschine, Menü-Eintrag Maschinenstatus Dialog [F3]:**
  Wählen Sie diesen Menüpunkt um Arbeitsunterbrechungen zu buchen.
  - Softwarereferenz, "Status" auf Seite 310
- **Benutzer Hilfe:**
  Über diesen Menüpunkt starten Sie die Kurzbeschreibungen.
- **Aktuelle Logeinträge:**
  Über diesen Menüpunkt starten Sie die Log-Datei. Diese Datei enthält die Log-Einträge für die jeweilige Sitzung.
  - Softwarereferenz, "Logeinträge für Sitzung" auf Seite 342
- **Sprache ändern:**
  Über diesen Menüpunkt können Sie die Modulsprache ändern. Es öffnet sich der Dialog Sprache ändern.
  - Softwarereferenz, "Sprachauswahl" auf Seite 343
- **Informationen:**
  Über diesen Menüpunkt können Sie sich weitere Informationen zu den Modulen anzeigen lassen. Es öffnet sich der Dialog Version Infos.
  - Softwarereferenz, "Über Production Terminal" auf Seite 344

### Registrierung
**Pfad:** Datei > Ummelden oder über die Funktionstaste F4

**Abbildung 24: Anmelden**
*Screenshot des Dialogs "Person wechseln" mit Feldern für Anwender und Station sowie den Schaltflächen OK und Abbrechen.*

Dieser Dialog hat zwei Funktionen. Er erscheint automatisch, wenn Sie das Programm starten. Dann geben Sie im Feld Anwender Ihren Namen ein. Das entsprechende Terminal-Modul wird gestartet. Wenn bereits ein Terminal-Modul läuft, können Sie mit diesem Dialog dann einen anderen Benutzer anmelden (z. B. Wechsel eines Mitarbeiters).

> **Namen scannen**
> Wenn Sie mit einem Scanner arbeiten, können Sie direkt im Hauptfenster unter Person Ihren Namen scannen und brauchen nicht den Dialog ToolTV Registrierung öffnen.

#### Erläuterung der Felder
- **Anwender:** Wählen Sie aus der Kombobox den entsprechenden Anwender aus.
  *Technische Info: Pflichtfeld, Auswahl*
- **ToolTV:** Wählen Sie aus der Kombobox den Leitrechner aus, an dem Sie sich anmelden möchten.
  *Technische Info: Pflichtfeld, Auswahl*

#### Erläuterung der Schaltflächen
- **OK:** Haben Sie in den Feldern Anwender und ToolTV die gewünschten Auswahlen getroffen, wird durch das Betätigen der Schaltfläche [OK] der entsprechende Leitrechner geöffnet. In diesem Beispiel wird Terminal IG-In geöffnet.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen.

**Ergänzende Informationen**
- Tutorial, "So melden Sie sich an" auf Seite 1240

### Gehe zu Produktionsnummer
**Pfad:** Datei > Springe zu ProdNr. oder über die Funktionstaste F11

**Abbildung 25: Gehe zu Produktionsnummer**
*Screenshot des Dialogs "Gehe zu Produktionsnummer" mit einem Eingabefeld für "Neue Produktionsnummer" und den Schaltflächen OK und Abbrechen.*

Mit diesem Dialog können Sie eine andere Produktionsnummer laden. Die Produktionsnummer bestimmt die Reihenfolge der zu produzierenden Einheiten. So können Sie z. B. direkt von der Produktionsnummer 3 auf die Produktionsnummer 15 springen ohne mehrfach die Schaltfläche [Überspringen] betätigen zu müssen. Das kann der Fall sein, wenn noch Nachläufer unterwegs sind.

#### Erläuterung der Felder
- **Produktionsnummer:** Wählen Sie über die Pfeiltasten die Produktionsnummer aus, die als nächstes produziert werden soll.

#### Erläuterung der Schaltflächen
- **OK:** Wenn Sie diese Schaltfläche betätigen, wird die gewählte Produktionsnummer übernommen.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen. Die gewählte Produktionsnummer wird nicht übernommen.

**Ergänzende Informationen**
- Tutorial, "Eine andere Produktionsnummer laden" auf Seite 1245

### Vorschau
**Pfad:** Datei > Vorschau-Dialog oder über die Funktionstaste F12

**Abbildung 26: Vorschau**
*Screenshot des "Vorschau"-Dialogs, der eine Liste von Losen und deren Details für eine bestimmte Erfassungsstelle anzeigt.*

Dieser Dialog zeigt Ihnen die Arbeitsmenge für die jeweilige Erfassungsstelle und den heutigen Tag. Über die Radiotasten haben Sie die Möglichkeit, die Anzeige einzuschränken.

#### Erläuterung der Felder
- **Erfassungsstelle:** In diesem Feld wird Ihnen die Erfassungsstelle angezeigt, auf die sich die Vorschau bezieht.
- **Alle:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben angezeigt.
- **Verfügbare:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Scheiben angezeigt, die zurzeit verfügbar sind.
- **Geplante:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben angezeigt, die geplant sind.
- **Mögliche:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Scheiben angezeigt, deren Bearbeitung möglich ist.

#### Erläuterung der Schaltflächen
- **Schließen:** Wenn Sie diese Schaltfläche oder die Funktionstaste [F5] betätigen, wird der Dialog geschlossen.

### Charge
**Pfad:** Datei > Charge oder über die Funktionstaste F1

**Abbildung 27: Charge**
*Screenshot des Dialogs "Manuelle Eingabe" zur Eingabe einer Chargennummer.*

Mit diesem Dialog können Sie Chargen zuweisen. Chargen dienen der Qualitätssicherung und -überwachung. Für Terminal IG-Assembly wäre z. B. an der Visitierstation ein Butyl-Fass eine denkbare Charge.

#### Erläuterung der Felder
- **Charge:** Geben Sie in diesem Feld die gewünschte Chargen-Bezeichnung ein. Alphanumerische Werte sind möglich.

#### Erläuterung der Schaltflächen
- **OK:** Wenn Sie diese Schaltfläche betätigen, wird die eingegebene Charge übernommen.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen. Die eingegebene Charge wird nicht übernommen.

**Ergänzende Informationen**
- Tutorial, "So definieren Sie Chargen" auf Seite 1253

### Los laden
**Pfad:** ToolTV IG-In > [Los laden] oder über die Funktionstaste F2

**Abbildung 28: Los laden**
*Screenshot des "Los laden"-Dialogs, der eine Liste anstehender Läufe und der dazugehörigen Lose anzeigt.*

In diesem Dialog werden Ihnen die zur Bearbeitung anstehenden Läufe inklusive aller enthaltenen Lose angezeigt. Der Dialog ist in zwei Fenster unterteilt. Im linken Fenster befindet sich die Übersicht aller anstehenden Läufe. Wählen Sie einen Lauf aus, sehen Sie im rechten Fenster, welche Einheiten zu diesem Lauf gehören und auf welcher Gestell-Nummer sie sich befinden. Sollten Sie nicht alle aufgeführten Gestell-Nummern für den Lauf im Zugriff haben, können Sie auch nur die vorhandenen Gestell-Nummern laden.

> **Filter löschen**
> Terminal IG-In merkt sich den zuletzt bearbeiteten Lauf. Um alle Läufe sehen zu können, müssen Sie deshalb den Filter löschen. Zum Löschen des Filters betätigen Sie die Schaltfläche [Alle anzeigen]. Sie erhalten dann die vollständige Laufliste.

#### Erläuterung der Felder
- **Lauf:** In dieser Spalte werden alle Läufe angezeigt, die zur Produktion an der angemeldeten Maschine anstehen.
- **Los:** In dieser Spalte wird die Losnummer der im Lauf enthaltenen Lose angezeigt.
- **Stk:** In dieser Spalte sehen Sie, wie viele Einheiten zu produzieren sind. Eine Einheit besteht aus mindestens zwei Scheiben.
- **Text:** In dieser Spalte wird Ihnen die Glasbezeichnung angezeigt. Die Glasbezeichnung kommt aus den Stammdaten.
- **Sperre:** Sollten Scheiben eines Laufes bereits von einer anderen Maschine bearbeitet werden, sehen Sie in dieser Spalte den Namen der Maschine. Diese Scheiben sind dann zur Bearbeitung an Ihrer Maschine gesperrt.
- **Gestell:** In dieser Spalte sehen Sie, auf welchem logischen Gestell (Gestell-Nummer) sich die Scheiben befinden.
- **Glasart:** In dieser Spalte wird Ihnen die Glasbezeichnung angezeigt.
- **Teile:** In dieser Spalte wird Ihnen die Anzahl der Scheiben angezeigt.

#### Erläuterung der Schaltflächen
- **Alle anzeigen:** Wenn Sie diese Schaltfläche betätigen, löschen Sie den Filter zur Anzeige der Läufe. Es werden dann alle anstehenden Läufe angezeigt.
- **Lauf entfernen:** Diese Schaltfläche entfernt alte, überflüssige Läufe, die nicht mehr produziert werden müssen.
- **Aktualisieren:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog aktualisiert.
- **Laden:** Wenn Sie diese Schaltfläche betätigen, wird der gewählte Lauf geladen.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen. Es wird kein Lauf geladen.

**Ergänzende Informationen**
- Tutorial, "Ein Los laden" auf Seite 1241

### Bruch buchen
**Pfad:** ToolTV IG-In > Einheit markieren > [Bruch] oder über die Funktionstaste F7

**Abbildung 29: Bruch buchen**
*Screenshot des "Zustand"-Dialogs, der eine Liste von Bruchgründen wie "Bruch", "Mangel", "Kratzer" anzeigt.*

Mit diesem Dialog wird die markierte Scheibe auf Bruch gesetzt. Wenn mit automatischen Nachläufern gearbeitet wird, dann werden für alle Teile der Einheit entsprechende Nachläufer angestoßen.

#### Erläuterung der Felder
- **Einheit:** Barcodenummer der Einheit, für die Bruch gemeldet werden soll.
- **Bruchgründe:** Liste der auswählbaren Bruchgründe. Die verfügbaren Bruchgründe müssen bei der Konfiguration des Systems definiert werden. Mögliche Gründe können sein:
  - Bruch
  - Mangel
  - Kratzer
  - Maß falsch
  - Falsche Glasart
  - MA-Kratzer
  - Teilebruch

> **Automatische Nachläufer**
> Für einige Bruchtypen werden Nachläufer automatisch generiert. Dies wird bei der Konfiguration entsprechend eingestellt. Der Mitarbeiter an der Maschine muss mit diesen Modalitäten vertraut sein.

#### Erläuterung der Schaltflächen
- **OK:** Wenn Sie diese Schaltfläche betätigen, wird der gewählte Bruchgrund übernommen.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen. Der zugewiesene Bruchgrund wird nicht übernommen.

**Ergänzende Informationen**
- Tutorial, "Umgang mit beschädigten Scheiben" auf Seite 1244
- Tutorial, "So verfahren Sie mit beschädigten Scheiben" auf Seite 1244

### Nachläufer laden
**Pfad:** ToolTV IG-In > [Nachläufer] oder über die Funktionstaste F8

**Abbildung 30: Nachläufer laden**
*Screenshot des "Einfügen"-Dialogs zur Eingabe einer Etikettnummer für einen Nachläufer.*

In diesem Dialog können Sie Nachläufer laden. Geben Sie zunächst die Etikettnummer manuell oder via Scanner ein. Sie können auch mehrere Etikettnummern hinter einander eingeben.

#### Erläuterung der Felder
- **Barcode:** In diesem Feld geben Sie die Etikettnummer des Nachläufers ein oder scannen ein Etikett.
- **Übernehmen [F2]:** Nachdem Sie die Etikettnummer eingegeben oder gescannt haben, betätigen Sie diese Schaltfläche. Die entsprechenden Daten werden im Feld darunter angezeigt.
- **Auftrag:** In diesem Feld sehen Sie die Auftragsnummer für den Nachläufer.
- **Pos:** In diesem Feld sehen Sie die Positionsnummer für den Nachläufer.
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.

#### Erläuterung der Schaltflächen
- **Laden:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen und der gewählte Nachläufer wird geladen.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen. Der Nachläufer wird nicht geladen.

**Ergänzende Informationen**
- Tutorial, "So laden Sie Nachläufer" auf Seite 1246
- Tutorial, "Einen Nachläufer laden" auf Seite 1246

### Status
**Pfad:** Maschine > Maschinenstatus

**Abbildung 31: Status**
*Screenshot des "Status"-Dialogs, der eine Liste von Maschinenzuständen wie "Bereit", "Abgemeldet", "Pause", "Wartung", "Rüsten", "Störung" anzeigt.*

Die Grundlage für aussagekräftige Auswertungen der Maschinendaten ist eine korrekte Zustandserfassung dieser Maschinen. Tritt an der Maschine ein Fehler auf, fehlt Personal, müssen Wartungsarbeiten durchgeführt oder kann der Produktivbetrieb wieder aufgenommen werden, so muss dieser neue Zustand jeweils dokumentiert werden.

#### Erläuterung der Felder
- **Nr:** In diesem Feld werden Ihnen die Zustandsnummer angezeigt. Die möglichen Zustände müssen konfiguriert werden.
- **Name:** In diesem Feld werden Ihnen die Zustandsnamen angezeigt. Die möglichen Zustände müssen konfiguriert werden.

**Ergänzende Informationen**
- Tutorial, "So ändern Sie den Maschinenstatus" auf Seite 1242

### Nachläufer-Verwaltung
**Pfad:** Extras > Nachläufer-Verwaltung

**Abbildung 32: Nachläufer-Verwaltung**
*Screenshot des "Nachläufer-Verwaltung"-Dialogs. Dieser zeigt eine Übersichtstabelle mit Nachläuferpositionen und eine Detailansicht mit der zugehörigen Stückliste.*

In diesem Dialog werden Ihnen die Nachläuferpositionen angezeigt, für die noch entschieden werden muss, wie sie wieder in die Produktion eingesteuert werden sollen und welche Teile ggf. wiederzuverwenden sind. Für eine solche Nachläuferposition wurde eine Zustandsbuchung vom Typ Teilebruch erzeugt.

#### Erläuterung der Felder im Bereich Übersicht
- **BT:** In diesem Feld wird Ihnen angezeigt, ob es sich bei dem Teil um ein Bestellteil handelt. In diesem Fall erscheint in dem Feld ein blauer Punkt.
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Auftrag:** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
- **Pos.:** In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.
- **PPos.:** In diesem Feld wird Ihnen die Produktionspositionsnummer angezeigt.
- **Teil:** In diesem Feld wird Ihnen die Teilenummer angezeigt.
- **Bezeichnung:** In diesem Feld wird Ihnen die Teilebezeichnung angezeigt.
- **Name:** In diesem Feld wird Ihnen der Bruchgrund angezeigt.
- **Buchungszeit:** In diesem Feld wird Ihnen angezeigt, wann die Buchung stattgefunden hat.
- **Erfassungsstelle:** In diesem Feld wird Ihnen die Erfassungsstelle angezeigt, an der der Bruch entstanden ist.
- **Info:** In diesem Feld wird Ihnen der Info-Text angezeigt, der erfasst wurde.
- **Mitarbeiter:** In diesem Feld wird Ihnen der Mitarbeiter angezeigt, der den Bruch gebucht hat.

#### Erläuterung der Schaltflächen (Übersicht)
- **Umbuchen:** Wenn Sie diese Schaltfläche betätigen, können Sie der Scheibe einen anderen Bruchgrund zuweisen und eine zusätzliche Information erfassen.
- **Wiederverwendung:** Wenn Sie diese Schaltfläche betätigen, kann das komplette Teil noch weiter verwendet werden. D. h., das Teil erhält die Beschaffungsart Wiederverwenden und verschwindet aus der Anzeige.
- **AV-Nachläufer:** Wenn Sie diese Schaltfläche betätigen, wird für das Teil eine komplett neue Produktionsposition im Auftragspool mit den ursprünglichen Beschaffungsarten erzeugt. Die alte Produktionsposition wird mengenmäßig entsprechend reduziert, sodass die Gesamtmenge der Auftragsposition wieder stimmt.
- **Direkte Nachfertigung:** Wenn Sie diese Schaltfläche betätigen, wird für das Teil eine direkte Nachfertigung ausgelöst. D. h. es wird für das Teil ein Eintrag im Bruchpool (globales Bruchmanagement) erzeugt, so dass die Scheibe automatisch nachgeschnitten werden kann.

#### Erläuterung der Kombobox
- **Filter:** Über diese Kombobox haben Sie die Möglichkeit, die angezeigten Daten nach einzelnen Zuständen in der Nachläufer-Verwaltung zu filtern.

#### Erläuterung der Felder im Bereich Details
Selektieren Sie im Bereich Übersicht eine Scheibe, wird Ihnen hier die gesamte Stückliste unterhalb der Position angezeigt. Dadurch können Sie auch für die zugehörigen Teile eine Entscheidung treffen, wie mit ihnen zu verfahren ist.
- **Bearbeitet:** In diesem Feld wird Ihnen angezeigt, ob es sich bei dem Teil um ein Bestellteil handelt. In diesem Fall erscheint in dem Feld ein blauer Punkt.
- **BT:** In diesem Feld wird Ihnen angezeigt, ob es sich bei dem Teil um ein Bestellteil handelt. In diesem Fall erscheint in dem Feld ein blauer Punkt.
- **Beschaffungsart:** In diesem Feld wird Ihnen die Beschaffungsart angezeigt.
- **AV-Nachläufer:** Wenn diese Checkbox aktiviert ist, wird eine neue Produktionsposition im Auftragspool erzeugt.
- **ES:** In diesem Feld wird Ihnen die Erfassungsstelle angezeigt, auf die die Scheibe gebucht werden soll.
- **Gestell:** In diesem Feld wird Ihnen der Name des Gestells angezeigt, auf den die Scheibe gebucht werden soll.
- **Name:** In diesem Feld wird Ihnen der Bruchgrund angezeigt.
- **Fehlerort:** In diesem Feld wird Ihnen der Fehlerort angezeigt, wenn dieser ausgewählt wurde.
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Teil:** In diesem Feld wird Ihnen die Teilenummer angezeigt.
- **Bezeichnung:** In diesem Feld wird Ihnen die Teilebezeichnung angezeigt.
- **Lauf:** In diesem Feld wird Ihnen die Laufnummer angezeigt.
- **Prod.-Termin:** In diesem Feld wird Ihnen der Produktionstermin angezeigt.

#### Erläuterung der Schaltflächen (Details)
- **Aktualisieren:** Wenn Sie diese Schaltfläche betätigen, wird der Bildschirm aufgefrischt. Es ist auch möglich, in den Parametern eine Zeit einzustellen, nach der der Bildschirm automatisch aufgefrischt wird.
- **Bearbeiten:** Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog Bearbeiten, für das Stücklistenelement, das Sie im Bereich Details ausgewählt haben.
- **Zurück:** Wenn Sie diese Schaltfläche betätigen, wird die zuletzt durchgeführte Aktion rückgängig gemacht.
- **Alles zurück:** Wenn Sie diese Schaltfläche betätigen, werden alle Aktionen, die Sie an dem Teil vorgenommen haben, rückgängig gemacht.
- **Speichern:** Wenn Sie diese Schaltfläche betätigen, wird die eigentliche Buchung gemäß den vorgenommenen Einstellungen ausgeführt. D. h., so lange, wie Sie diese Schaltfläche noch nicht gedrückt haben, wurde nichts in die Datenbank geschrieben und Sie können noch Aktionen rückgängig machen.
- **Schließen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog beendet.

**Ergänzende Informationen**
- Softwarereferenz, "Nachläufer-Verwaltung - Bearbeiten" auf Seite 1360
- Tutorial, "Nachläufer-Verwaltung" auf Seite 1260

### Nachläufer-Verwaltung - Bearbeiten
**Pfad:** Extras > Nachläufer-Verwaltung > [Bearbeiten]

**Abbildung 33: Nachläufer-Verwaltung - Bearbeiten**
*Screenshot des "Bearbeiten"-Dialogs für ein Nachläufer-Teil. Hier können Beschaffungsart, Erfassungsstelle, Gestell und Fehlergrund detailliert eingestellt werden.*

In diesem Dialog können Sie die genauen Einstellungen für jedes einzelne Teil vornehmen.

#### Erläuterung der Felder
- **Beschaffungsart:** In diesem Feld können Sie über die Kombobox die Beschaffungsart des gewählten Teils ändern. Sie können zwischen der ursprünglichen Beschaffungsart und Beschaffungsart Wiederverwendung wählen. Wählen Sie Wiederverwendung, dann werden die darunter liegenden Felder Erfassungsstelle und Gestell zur Bearbeitung freigegeben.
- **Erfassungsstelle:** Wenn das Teil wieder verwendet werden kann, wählen Sie hier den Ort, wo Sie das Teil bis zur Wiederverwendung abstellen. Diese Information kann in den Production Terminals angezeigt werden.
- **Gestell:** Wenn das Teil wieder verwendet werden kann, können Sie hier zusätzlich zur Erfassungsstelle noch das Gestell angeben, auf dem das wieder verwendbare Teil steht. Diese Information wird z. B. bei der Nachproduktion des gesamten ISOs am A+W Production Terminal IG-In anstelle der logischen Gestellnummer angezeigt.
- **Fehlergrund:** Wenn das Teil nicht wieder verwendet werden kann und die Beschaffungsart Produktion gewählt wurde, dann können Sie hier den wirklichen Bruchgrund auswählen. Dieser kann dann später für statistische Auswertungen genutzt werden.
- **Fehlerort:** Zusätzlich zum Bruchgrund können Sie hier noch einen Fehlerort angeben. Dieser ist, unabhängig von der Erfassungsstelle, an der der Bruch passiert ist, wählbar.
- **AV-Nachläufer:** Wenn Sie diese Checkbox aktivieren, wird eine neue Produktionsposition im Auftragspool erzeugt.

#### Erläuterung der Felder im Bereich Bearbeitungen
In diesem Bereich werden alle Bearbeitungen angezeigt, die an der betroffenen Scheibe schon gebucht wurden.
- **Wiederholen:** Durch setzen der Haken in dieser Spalte, werden die Bearbeitungen so zurückgesetzt, dass man sie erneut buchen kann.
- **Artikel:** In diesem Feld wird Ihnen die Artikelnummer angezeigt.
- **BearbNr:** In diesem Feld wird Ihnen die Bearbeitungsnummer angezeigt.
- **Bearbeitung:** In diesem Feld wird Ihnen der Name der Bearbeitung angezeigt.

#### Erläuterung der Felder im Bereich Mögliche Teile
In diesem Bereich werden Ihnen alle Teile angezeigt, die für das ausgewählte Teil in Frage kommen. D. h., Sie müssen aus dieser Liste eine Etikettnummer auswählen, die mit dem Nachläufer als Gegenscheibe zusammen laufen soll. Idealerweise verwendet man hier eine Etikettnummer, die sich noch nicht in der Produktion befindet. Ist dies nicht möglich, muss die ausgewählte Etikettnummer aus der Produktion entfernt werden, damit eine versehentliche Verwendung dieser Etikettnummer vermieden wird. Die Zuweisung einer Etikettnummer ist nur erforderlich, wenn die Teile nicht vorher schon zusammengebaut waren, in diesem Fall sind bereits eindeutige Etikettnummern zugewiesen.
- **Auswählen:** Durch setzen der Haken in dieser Spalte, werden genau diese Bearbeitungen in den Tabellen so zurückgesetzt, dass man sie erneut buchen kann.
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Erfassungsstelle:** In diesem Feld wird Ihnen die Erfassungsstelle angezeigt.
- **Gestell:** In diesem Feld wird Ihnen der Gestellname angezeigt.
- **Lauf:** In diesem Feld wird Ihnen die Laufnummer angezeigt.
- **Letzte Buchung:** In diesem Feld wird Ihnen angezeigt, wann die letzte Buchung durchgeführt wurde.
- **Status:** In diesem Feld wird Ihnen der Status angezeigt.
- **Bezeichnung:** In diesem Feld wird Ihnen die Artikelbezeichnung angezeigt.

**Ergänzende Informationen**
- Softwarereferenz, "Nachläufer-Verwaltung" auf Seite 1357
- Tutorial, "Nachläufer-Verwaltung" auf Seite 1260

## Übersicht Terminal Manual Cutting
Terminal Manual Cutting zeigt Ihnen alle freigegebenen Läufe bzw. Lose für einen bestimmten Zuschnitttisch. Bei dem Zuschnitttisch handelt es sich in der Regel um einen Handzuschnitttisch. Sofern Sie keinen Maschinencode am Tisch erzeugen müssen, kann das Terminal Manual Cutting auch an einem anderen Tisch installiert sein.
Die Menüs von Terminal Manual Cutting sind identisch mit den Menüs von Terminal IG-In und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

### Freigabe
**Pfad:** JobTV Handzuschnitt > Lauf markieren > Schaltfläche [Freigabe]

**Abbildung 34: Freigabe**
*Screenshot des "Freigabe"-Dialogs, der eine Liste von zu schneidenden Scheiben, eine Modellskizze und Buchungsschaltflächen anzeigt.*

Dieser Dialog zeigt Ihnen die Scheiben an, die Sie zuvor im Terminal Manual Cutting ausgewählt haben. Sie können alle Scheiben auf einmal buchen oder aber einzelnen Scheiben. Wenn der Dialog geöffnet wird, sind standardmäßig alle Scheiben selektiert. Um eine einzelne Scheibe zu buchen, markieren Sie diese in der Tabelle.

#### Erläuterung der Felder im Bereich A (Auswahl)
- **Lauf:** In diesem Feld wird Ihnen die Laufnummer angezeigt.
- **Los:** In diesem Feld wird Ihnen die Losnummer angezeigt.
- **Glasart:** In diesem Feld wird Ihnen die Glasart angezeigt.
- **Barcode:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Bock:** In diesem Feld wird Ihnen die Gestellnummer angezeigt.
- **Fach:** In diesem Feld wird Ihnen die Fachnummer angezeigt.
- **Pr.-Nr.:** In diesem Feld wird Ihnen die Produktionsnummer angezeigt.
- **Modell:** In diesem Feld wird Ihnen die Modellnummer angezeigt.
- **ZS-Breite:** In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.
- **ZS-Höhe:** In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.
- **Auftrag:** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
- **Pos.:** In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

#### Erläuterung der Felder im Bereich B (Modellanzeige)
In diesem Bereich befindet sich die Modellanzeige.

#### Erläuterung der Felder im Bereich C (Modell-Skizze)
In diesem Bereich sehen Sie die Modellskizze. Die Tabelle daneben zeigt Ihnen die entsprechenden Werte. Folgende Werte sind möglich:
- W = Breite
- H = Höhe
- T1, T2, ... = Bruchrand
- <-> = Spiegelkennzeichen
- @ = Drehkennzeichen

#### Erläuterung der Felder im Bereich D (Selektiert von Gesamt)
In diesem Bereich sehen Sie, wie viele Scheiben Sie in der Tabelle markiert haben und die Gesamtstückzahl. Bsp.: 1/64 bedeutet, dass 64 Scheiben in der Tabelle angezeigt werden und Sie 1 Scheibe davon markiert haben.

#### Erläuterung der Felder im Bereich E (Gestell)
In diesem Bereich befinden sich die Daten zum Gestell. Sie können die Gestellnummer eingeben oder aber scannen. Wenn das Gestell leer ist, aktivieren Sie die Checkbox Beginn.

#### Erläuterung der Schaltflächen
- **Produzieren:** Wenn Sie diese Schaltfläche betätigen, wird die markierte Scheibe gebucht.
- **Eti Druck:** Wenn Sie diese Schaltfläche betätigen, wird für die markierte Scheibe ein Etikett gedruckt.
- **Bruch:** Wenn Sie diese Schaltfläche betätigen, wird die markierte Scheibe als Bruch gebucht.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal Manual Cutting" auf Seite 1266
- Tutorial, "So buchen Sie die ausgewählte(n) Scheibe(n)" auf Seite 1275

### Bruchpool
**Pfad:** JobTV Handzuschnitt > Schaltfläche [Bruchpool]

**Abbildung 35: Bruchpool**
*Screenshot des "Bruchpool"-Dialogs, der eine Liste von als Bruch gemeldeten Scheiben enthält, die nachgeschnitten werden müssen.*

Mit diesem Instrument haben Sie die Möglichkeit, auf zu Bruch gegangene Scheiben schnell reagieren zu können. Wird irgendwo in der Produktion eine Scheibe als Bruch gescannt, öffnet sich der Dialog Bruchpool automatisch. Die zu Bruch gegangene Scheibe ist dann im Bruchpool enthalten und kann sofort nachgeschnitten werden (ohne über die Hauttische zu laufen).

#### Erläuterung der Felder im Bereich A (Auswahl)
- **Artikel:** In diesem Feld wird Ihnen die Artikelnummer angezeigt.
- **Bezeichnung:** In diesem Feld wird Ihnen die Glasart angezeigt.
- **Glasart:** In diesem Feld wird Ihnen die Glasart angezeigt.
- **Dicke:** In diesem Feld wird Ihnen die Dicke der Scheibe angezeigt.
- **Breite:** In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.
- **Höhe:** In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.
- **Lauf:** In diesem Feld wird Ihnen die Laufnummer angezeigt.
- **Kunde:** In diesem Feld wird Ihnen der Kundenname angezeigt.
- **Auftrag:** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
- **Pos.:** In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Modell:** In diesem Feld wird Ihnen die Modellnummer angezeigt.
- **Bock:** In diesem Feld wird Ihnen die Gestellnummer angezeigt.
- **Liefertermin:** In diesem Feld wird Ihnen der Liefertermin angezeigt.

#### Erläuterung der Schaltflächen
- **Aktualisieren:** Wenn Sie diese Schaltfläche betätigen, wird die Anzeige aktualisiert.
- **Hinzufügen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog Brucherfassung geöffnet.
- **Löschen:** Wenn Sie diese Schaltfläche betätigen, wird die markierte Scheibe gelöscht.
- **Drucken/Drucken2:** Diese Schaltflächen werden vor Ort angepasst und dienen dem Drucken von Etiketten oder Reports.
- **BDE buchen:** Wenn Sie diese Schaltfläche betätigen, wird die markierte Scheibe gebucht.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen.

> **Automatische Aktualisierung**
> Der Bruchpoool aktualisiert sich automatisch alle x Sekunden. Dieser Wert ist einstellbar.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal Manual Cutting" auf Seite 1266
- Tutorial, “So buchen Sie die ausgewählte(n) Scheibe(n)" auf Seite 1275

### Brucherfassung
**Pfad:** JobTV Handzuschnitt > Schaltfläche [Bruchpool] > Schaltfläche [Hinzufügen]

**Abbildung 36: Brucherfassung**
*Screenshot des "Brucherfassung"-Dialogs zur manuellen Erfassung einer Bruchscheibe mit Kunden-, Auftrags- und Teiledetails.*

Mit dem Dialog Brucherfassung besteht die Möglichkeit, Brüche manuell dem Bruchpool hinzuzufügen.

#### Erläuterung der Felder im Bereich Kunde
- **Auftrag:** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
- **Position:** In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

#### Erläuterung der Felder im Bereich Teile
- **Auftrag:** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
- **Pos:** In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.
- **Teilenummer:** In diesem Feld wird Ihnen die Teilenummer angezeigt.
- **Glasart:** In diesem Feld wird Ihnen die Glasart angezeigt.
- **Breite:** In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.
- **Höhe:** In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.

#### Erläuterung der Felder im Bereich Bruchgrund
Wählen Sie aus der Kombobox den entsprechenden Bruchgrund aus.

#### Erläuterung der Felder im Bereich Barcodes
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **ES:** In diesem Feld wird Ihnen die Erfassungsstelle angezeigt.
- **Gestell:** In diesem Feld wird Ihnen die Gestellnummer angezeigt.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal Manual Cutting" auf Seite 1266
- Tutorial, "So fügen Sie einen Bruch manuell hinzu" auf Seite 1275

## Übersicht Terminal Georgian Bars
Terminal Georgian Bars zeigt Ihnen alle freigegebenen Läufe bzw. Lose für den Sprossenbau.
Die Menüs von Terminal Georgian Bars sind identisch mit den Menüs von Terminal IG-In und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

### Sprossen-Freigabe
**Pfad:** Terminal Georgian Bars > Lauf markieren > Schaltfläche [Freigabe]

**Abbildung 37: Sprossen-Freigabe**
*Screenshot des "Sprossen-Freigabe"-Dialogs, der eine Liste von Sprossen, ein Sprossenbild und Buchungsschaltflächen anzeigt.*

Dieser Dialog zeigt Ihnen die Sprossen an, die Sie zuvor im Terminal Georgian Bars ausgewählt haben. Sie können alle Sprossen auf einmal buchen oder aber einzelne Sprossen. Wenn der Dialog geöffnet wird, sind standardmäßig alle Sprossen selektiert. Um eine einzelne Sprossen zu buchen, markieren Sie diese in der Tabelle.

#### Erläuterung der Felder im Bereich A (Auswahl)
- **Lauf:** In diesem Feld wird Ihnen die Laufnummer angezeigt.
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Bezeichnung:** In diesem Feld wird Ihnen die Sprossenbezeichnung angezeigt.
- **Auftrag:** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
- **Pos.:** In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.
- **PPos.:** In diesem Feld wird Ihnen die Produktionspositionsnummer angezeigt.
- **Termin:** In diesem Feld wird Ihnen die Produktionstermin angezeigt.
- **Modell:** In diesem Feld wird Ihnen die Modellnummer angezeigt.
- **Breite:** In diesem Feld wird Ihnen die Breite des Modells (umschreibendes Rechteck) angezeigt.
- **Höhe:** In diesem Feld wird Ihnen die Höhe des Modells (umschreibendes Rechteck) angezeigt.

#### Erläuterung der Felder im Bereich B (Gestell)
In diesem Bereich befinden sich die Daten zum Gestell. Sie können die Gestellnummer eingeben oder aber scannen. Wenn das Gestell leer ist, aktivieren Sie die Checkbox Beginn.

#### Erläuterung der Felder im Bereich C (Selektiert von Gesamt)
In diesem Bereich sehen Sie, wie viele Sprossen Sie in der Tabelle markiert haben und die Gesamtstückzahl. Bsp.: 1/9 bedeutet, dass 9 Sprossen in der Tabelle angezeigt werden und Sie 1 Sprosse davon markiert haben.

#### Erläuterung der Felder im Bereich D (Sprossenbild)
In diesem Bereich befindet sich die Anzeige des Sprossenbildes.

#### Erläuterung der Schaltflächen
- **Produzieren:** Wenn Sie diese Schaltfläche betätigen, wird die markierte Sprosse gebucht.
- **Drucken:** Wenn Sie diese Schaltfläche betätigen, können Sie das Sprossenbild auf einem lokalen Drucker ausdrucken.
- **Bruch:** Wenn Sie diese Schaltfläche betätigen, wird die markierte Sprosse als Bruch gebucht.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal Georgian Bars" auf Seite 1278
- Tutorial, "So buchen Sie die ausgewählte(n) Sprosse(n)" auf Seite 1284

## Übersicht Terminal Order
Mit Terminal Order haben Sie die Möglichkeit größere Mengen zu verbuchen. Bearbeitungen, die mit der jeweiligen Erfassungsstelle verknüpft sind, werden dabei mit gebucht.
Die Menüs von Terminal Order sind identisch mit den Menüs von Terminal IG und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

## Übersicht Terminal Processing
Terminal Processing ist ein Leitrechner, der an Bearbeitungsmaschinen zum Einsatz kommt. Terminal Processing gibt Ihnen detaillierte Auskunft über die durchzuführenden Bearbeitungen inklusive maßstabgetreuer Produktionszeichnungen.
Die Menüs von Terminal Processing sind identisch mit den Menüs von Terminal IG und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

### Manuelle Eingabe
**Pfad:** Extras > Barcode

**Abbildung 38: Manuelle Eingabe**
*Screenshot des "Manuelle Eingabe"-Dialogs zur Eingabe einer Barcode/Etikett-Nummer.*

Mit diesem Dialog haben Sie die Möglichkeit, eine weitere Scheibe zu laden. Geben Sie im Feld Barcode die gewünschte Etikett-Nummer ein oder scannen Sie den Barcode. Anschließend betätigen Sie die Schaltfläche [OK].
Der Dialog wird geschlossen. Sie sind jetzt wieder im Hauptfenster. Die geladene Scheibe wird am Ende der Übersicht angezeigt.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal Processing" auf Seite 1295
- Tutorial, "So scannen Sie ein Etikett" auf Seite 1300

## Übersicht Terminal TG
Terminal TG kommt an ESG-Öfen zum Einsatz und unterstützt Sie dort bei der Be- und Entladung der Ofenbetten.
Die Module Terminal TG-In und Terminal TG-Out haben die gleichen Menüs wie Terminal IG und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

### Manuelle Eingabe
**Pfad:** ToolTV TG-In > Extras > Barcode

**Abbildung 39: Manuelle Eingabe**
*Screenshot des "Manuelle Eingabe"-Dialogs zur Eingabe einer Barcode/Etikett-Nummer.*

Mit diesem Dialog haben Sie die Möglichkeit, eine weitere Scheibe zu laden. Geben Sie im Feld Barcode die entsprechende Etikett-Nummer ein und betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen und die Etikett-Nummer wird geladen.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal TG-In" auf Seite 1305
- Tutorial, "So scannen Sie ein Etikett" auf Seite 1309

### Offene Bearbeitungen
**Pfad:** ToolTV TG-In > Etikettnummer laden

**Abbildung 40: Offene Bearbeitungen**
*Screenshot des "Offene Bearbeitungen"-Dialogs. Er listet Bearbeitungsschritte auf, die für eine Scheibe noch nicht abgeschlossen sind, bevor sie gehärtet wird.*

Dieser Dialog erscheint automatisch, wenn es vor dem Härten noch offene Bearbeitungen gibt. Dann werden Ihnen diese offenen Bearbeitungen angezeigt und Sie können entscheiden, wie mit der Scheibe weiter verfahren werden soll.

#### Erläuterung der Felder
- **Etikett:** In diesem Feld wird Ihnen die Etikettnummer angezeigt.
- **Auftrag/Pos.:** In diesem Feld wird Ihnen die Auftrags- sowie die Positionsnummer angezeigt.

#### Erläuterung der Tabelle
- **Fertig:** In diesem Feld sehen Sie, welche Bearbeitungen noch offen sind. Mögliche Werte:
  - Rotes X: Die Bearbeitung ist noch offen.
  - Grüner Haken: Die Bearbeitung ist gemacht.
- **Termin:** In diesem Feld sehen Sie, wann die Bearbeitung durchgeführt wird.
- **Bearbeitung:** In diesem Feld wird Ihnen die Bearbeitung angezeigt.

#### Erläuterung der Schaltflächen
- **Trotzdem laden:** Diese Schaltfläche müssen Sie verwenden, wenn die Bearbeitung durchgeführt wurde, jedoch nicht gebucht wurde. Der Dialog wird geschlossen. Sie befinden sich jetzt wieder im Hauptfenster. Die geladene Scheibe wird in der Übersicht angezeigt.
- **Schließen:** Diese Schaltfläche müssen Sie verwenden, wenn die Bearbeitung wirklich fehlt. Dann wird der Dialog geschlossen, die Scheibe muss noch bearbeitet werden.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal TG-In" auf Seite 1305
- Tutorial, "Arbeiten mit Terminal TG-Out" auf Seite 1313
- Tutorial, "So verfahren Sie mit offenen Bearbeitungen" auf Seite 1309

## Übersicht Terminal LG
Terminal LG kommt an der VSG-Linie zum Einsatz und zeigt Ihnen alle verfügbaren Lose inklusive produktionsunterstützender Informationen.
Die Module Terminal LG-In und Terminal LG-Assembly haben die gleichen Menüs wie Terminal IG und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
- **Menü Datei, Menü-Eintrag Auftrag laden:**
  Mit diesen Menüpunkt laden Sie einen speziellen Auftrag.
  - Softwarereferenz, "Registrierung" auf Seite 299

### Auftrag laden
**Pfad:** Terminal LG-In > Datei > Auftrag laden

**Abbildung 41: Auftrag laden**
*Screenshot des "Auftrag laden"-Dialogs, der eine Liste von Auftragspositionen und deren Details anzeigt.*

Mit diesem Dialog haben Sie die Möglichkeit, einen bestimmten Auftrag zu laden. Über die Radiotasten haben Sie die Möglichkeit, die Anzeige einzuschränken.

#### Erläuterung der Felder
- **Alle:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben angezeigt.
- **Verfügbare:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Scheiben angezeigt, die zurzeit verfügbar sind.
- **Geplante:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben angezeigt, die geplant sind.
- **Mögliche:** Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Scheiben angezeigt, deren Bearbeitung möglich ist.
- **Auftrag:** In diesem Feld wird Ihnen die Auftrags-Nummer angezeigt.
- **Pos:** In diesem Feld wird Ihnen die Positions-Nummer angezeigt.
- **Teil:** In diesem Feld wird Ihnen die Teile-Nummer angezeigt.
- **Bezeichnung:** In diesem Feld wird Ihnen die Teile-Bezeichnung angezeigt.
- **Lauf:** In diesem Feld wird Ihnen die Lauf-Nummer angezeigt.
- **Menge:** In diesem Feld wird Ihnen die zu produzierende Menge angezeigt.

Die Tabelle darunter enthält detaillierte Informationen zu dem Auftrag, den Sie oben ausgewählt haben.

#### Erläuterung der Schaltflächen
- **Laden:** Wenn Sie diese Schaltfläche oder die Funktionstaste [F5] betätigen, wird die Auswahl übernommen.
- **Abbrechen:** Wenn Sie diese Schaltfläche oder die Funktionstaste [F6] betätigen, wird der Dialog geschlossen.

**Ergänzende Informationen**
- Tutorial, "Arbeiten mit Terminal LG-In" auf Seite 1320
- Tutorial, "Arbeiten mit Terminal LG-Assembly" auf Seite 1326

### Gehe zu Produktionsnummer
**Pfad:** Datei > Springe zu ProdNr. oder über die Funktionstaste F11

**Abbildung 42: Gehe zu Produktionsnummer**
*Screenshot des Dialogs "Gehe zu Produktionsnummer" mit einem Eingabefeld für "Neue Produktionsnummer".*

Mit diesem Dialog können Sie eine andere Produktionsnummer laden. Die Produktionsnummer bestimmt die Reihenfolge der zu produzierenden Einheiten. So können Sie z. B. direkt von der Produktionsnummer 3 auf die Produktionsnummer 15 springen ohne mehrfach die Schaltfläche [Überspringen] betätigen zu müssen.

#### Erläuterung der Felder
- **Produktionsnummer:** Wählen Sie über die Pfeiltasten die Produktionsnummer aus, die als nächstes produziert werden soll.

#### Erläuterung der Schaltflächen
- **OK:** Wenn Sie diese Schaltfläche betätigen, wird die gewählte Produktionsnummer übernommen.
- **Abbrechen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen. Die gewählte Produktionsnummer wird nicht übernommen.

**Ergänzende Informationen**
- Tutorial, "Eine andere Produktionsnummer laden" auf Seite 1245

## Übersicht Terminal Edit
Terminal Edit bietet die Möglichkeit, fehlende oder falsche Buchungen zu korrigieren und größere Mengen auf einmal zu buchen.
Das Modul hat die gleichen Menüs wie Terminal IG und werden an dieser Stelle nicht noch einmal beschrieben.
- "Terminal IG" auf Seite L-1346

## Reports
Menü Listen öffnen
Im Menü Listen befindet sich die auf Kundenwunsch erstellten Reports. In unserem Beispiel finden Sie dort den Menüpunkt:
- **Auftragsübersicht:**
  Über diesen Menüpunkt starten Sie den Report für die Auftragsübersicht.
  - Softwarereferenz, "Parametereingabe für Report" auf Seite 1384

### Parametereingabe für Report
**Pfad:** Listen > Auftragsübersicht

**Abbildung 43: Parametereingabe für Report**
*Screenshot des "Parametereingabe für Report"-Dialogs, der zur Eingabe einer Auftragsnummer auffordert.*

Der Dialog oben zeigt die Parametereingabe für eine Auftragsübersicht. In Terminal gibt es viele unterschiedliche Listen (Reports). Sie werden von A+W für jeden Kunden individuell erstellt und den jeweiligen Anforderungen angepasst.

**Abbildung 44: Beispielreport Auftragsübersicht**
*Beispiel eines Auftragsübersicht-Reports für einen bestimmten Auftrag, mit Positionsdetails, Glasart, Maßen und Buchungszeiten.*

**Ergänzende Informationen**
- Tutorial, "Listen (Reports) generieren" auf Seite 1247
- Tutorial, "So drucken Sie eine Auftragsübersicht" auf Seite 1247

## Die Hilfe verwenden
Menü ? öffnen
Im Menü ? befinden sich folgende Menüpunkte:
- **Benutzer-Hilfe:**
  Über diesen Menüpunkt starten Sie die Kurzbeschreibungen.
- **Aktuelle Logeinträge:**
  Über diesen Menüpunkt starten Sie die Log-Datei. Diese Datei enthält die Log-Einträge für die jeweilige Sitzung.
  - Softwarereferenz, "Logeinträge für Sitzung" auf Seite 1386
- **Sprache ändern:**
  Über diesen Menüpunkt können Sie die Modulsprache ändern. Es öffnet sich der Dialog Sprache ändern.
  - Softwarereferenz, “Sprachauswahl" auf Seite 1387
- **Informationen:**
  Über diesen Menüpunkt erhalten Sie weitere Informationen zum jeweiligen Modul.
  - Softwarereferenz, “Über Production Terminal" auf Seite 1388

### Logeinträge für Sitzung
**Pfad:** ? > Aktuelle Logeinträge

**Abbildung 45: Logeinträge**
*Screenshot des Dialogs "Log Einträge für diese Sitzung", der eine detaillierte Liste von Systemereignissen, Debug-Informationen und Fehlern anzeigt.*

In diesem Dialog werden Ihnen Details zu der jeweiligen Sitzung angezeigt. Sie können die Logeinträge in Form einer Text-Datei exportieren. Im Falle eines Fehlers kann es von Vorteil sein, diese Text-Datei zu Analysezwecken zu A+W zu schicken.

#### Erläuterung der Schaltflächen
- **Aktualisieren:** Wenn Sie diese Schaltfläche betätigen, aktualisieren Sie die Anzeige.
- **Exportieren:** Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog Speichern unter .... Sie können die Logeinträge dann als Text-Datei speichern.
- **Schließen:** Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen.

**Ergänzende Informationen**
- Tutorial, “So exportieren Sie Log-Einträge" auf Seite 1247

### Sprachauswahl
**Pfad:** ? > Sprache ändern

**Abbildung 46: Sprache ändern**
*Screenshot des "Sprache ändern"-Dialogs mit Komboboxen für die Auswahl der Haupt- und Ersatzsprache.*

In diesem Dialog wählen Sie die Sprache für das jeweilige Terminal aus. Nachdem Sie den Dialog mit der Schaltfläche [OK] verlassen haben, stellt Terminal die Sprache um.

#### Erläuterung der Felder
- **Sprache:** Wählen Sie aus der Kombobox die gewünschte Sprache aus und betätigen Sie die Schaltfläche [OK]. Die Sprache wird automatisch umgestellt. Es ist kein Neustart erforderlich.
- **Ersatz-Sprache:** Wählen Sie aus der Kombobox die gewünschte Ersatz-Sprache aus. Die Ersatz-Sprache kommt dann zum Einsatz, wenn z. B. die Übersetzung für einen Eintrag fehlt.

**Ergänzende Informationen**
- Tutorial, "So wählen Sie eine andere Sprache aus" auf Seite 1248

### Über Production Terminal
**Pfad:** ? > Information

**Abbildung 47: Über ToolTV**
*Screenshot des "ToolTV Version Infos"-Dialogs, der detaillierte Informationen über die Anwendungsversion, Dateiversion, Webservices und Datenbankverbindung anzeigt.*

In diesem Dialog erhalten Sie weitere Informationen zu den einzelnen Modulen, z. B. Version und Release-Stand.

# A+W Production Index

### Symbols
- 'Zuweisung
  - Stufe II F-668

### A
- A+W Continuous Cutting J-1127
  - Übersicht geplanter Läufe J-1127
- A+W Pattern Viewer J-1113
- A+W Residual Stock Manager J-1104
- Abgelaufene Reservierungen E-601
- Abgelaufene Reservierungen löschen E-473
- Abhängige Bearbeitung
  - Erzeugung D-381
  - Lostyp D-381
  - Name D-381
  - Register D-381
  - Typ D-381
- Abladereihenfolge (Terminal TG-In) L-1315
- Ablauf von Arbeitsschritten
  - Terminal Edit L-1337
  - Terminal IG-Assembly L-1253
  - Terminal IG-Out L-1259
  - Terminal LG-Assembly L-1329
  - Terminal LG-In L-1323
  - Terminal Manual Cutting L-1274, L-1283
  - Terminal Order L-1291
  - Terminal Processing L-1300
  - Terminal TG-In L-1309
  - Terminal TG-Out L-1317
- Abmessungsrestriktionen G-742, G-820
- A-Böcke
  - Gruppierung und Sortierung D-322
  - Nummernkreise D-323
  - Optimierung D-323
  - Produktionsreihenfolge D-321
  - Standard-Produktionsorganisation D-321
- A-Böcke SZR
  - Nummernkreise D-315
  - Optimierung D-315
- A-Böcke Versand
  - Größenklassen D-327
  - Gruppierung und Sortierung D-328
  - Nummernkreise D-329
  - Produktionsreihenfolge D-328
  - Standard-Produktionsorganisation D-327
- Abstand v. Achsen
  - Fächerwagen D-375
- Absteigend
  - Gruppierung D-367
- Abstellbreite
  - A-Bock D-372
  - FAP D-374, D-375
- Abstellmodus D-363
  - Einstellungen-Abstellplatz D-363
  - Orga D-357
- Abstellmodus Gruppen
  - Einstellungen-Abstellplatz D-361
- Abstellplatz
  - Abstand v. Achsen D-375
  - Abstellbreite (A-Bock) D-372
  - Abstellbreite (FAP) D-374, D-375
  - Abstelltiefe (A-Bock) D-372
  - Abstelltiefe (FAP) D-375
  - Abweichung Schwerpunkt v. Mitte D-375
  - Anzahl D-373
  - Anzahl der Stellen für ... D-374
  - Anzahl Fachnummer D-373
  - Dialog D-372
  - ID für Stack-Opti D-373
  - L-Bock D-372
  - Leergewicht (Fächerwagen) D-374
  - Max. Abstellplätze/Bock D-372
  - Max. Anzahl Fächerwagen D-373, D-374
  - Maximale Nutzlast (Fächerwagen) D-374
  - Maximales Gewicht (A-Bock) D-373
  - Maximales Gewicht (FAP) D-375
  - Robot D-373
  - Sortjet D-373, D-374
  - Start=0 D-374
  - Überprüfung Anzahl (Fächerwagen) D-373, D-374
  - Überprüfung Anzahl (FAP) D-375
  - Zwei Fächer/Nummer D-374
- Abstellplatz-Typ
  - Einstellungen-Abstellplatz (Register Verwendung) D-363
- Abstelltiefe
  - A-Bock D-372
  - Abstellplatz (FAP) D-375
- Addup
- Mengen Erzeuger F-711
- Aktion für Stücklistenkonfiguration E-582
- All
  - Bedinungen-Erzeuger F-698
  - Mengen Erzeuger F-710
- Alte Bezeichnung
  - Name der Bedingung F-701
  - Name der Menge F-713
- Alter Wert
  - Eingabe Zahlenwert F-704, F-705
- Alternativmaschinen E-431
- Andere Produktionsnummer laden L-1245
- Ändern der minimalen Anzahl A-Böcke
  - Dialog D-412
- Änderung der Beschaffungsart C-157
- Änderung verplanter Aufträge E-593
- Anfang
  - Prüfreihenfolge D-352
- Anmelden
  - Terminal IG-In L-1240
- Ansichten C-104
  - Arbeiten mit der Liste C-111
  - Filter konfigurieren C-117
  - konfigurierbare Bestandteile C-105
  - konfigurieren C-107
  - Register konfigurieren C-107
  - Spalte definieren C-114
  - Spalten konfigurieren C-109
  - Summenzeile definieren C-114
  - Summenzeile konfigurieren C-112
  - Übungen C-121
  - Weißer Screen C-120
- Ansteuern
  - Tisch J-1183
- Anychild
  - Mengen Erzeuger F-710
- Anzahl
  - Abstellplatz D-373
  - Detail-Ansicht 1-986
  - Fachnummer, Dialog Abstellplatz D-373
- Anzahl der Stellen für ...
  - Abstellplatz D-374
- Anzahl Resultate
  - Formel Editor F-719
- Anzeige
  - Bruchscheiben J-1192
- Anzeigen
  - Eilscheibe J-1144
  - Kontext-Menü bei markiertem Eintrag 1-1036
- Arbeit
  - fortsetzen J-1099
  - unterbrechen J-1099
- Arbeitsfreie Tage
  - anlegen E-484
  - bearbeiten E-485
  - löschen E-486
- Arbeitsgang A-41, G-763, G-764, G-811
  - anlegen G-770, G-826
  - basierend auf Bearbeitungsartikel G-769
  - bearbeiten G-771, G-828
  - erstellen G-770, G-826
  - exakt definieren G-766
  - löschen G-772
  - mehrere Arbeitsgänge G-767
  - nicht zugeordnet G-767
  - Priorität G-767
  - verwalten G-770
  - zusätzliche Bedingung G-768
- Arbeitsgangzuordnung G-774, G-812
  - angepasste A-42, G-775
  - logische Maschine und Arbeitsgang trennen G-782
  - logische Maschine und Arbeitsgang zuordnen G-780
  - Prioriät ändern G-783
  - zusätzliche Bedingung G-775
- Arbeitsplan C-211
  - Exportieren E-445
- Arbeitsschicht
  - Anpassungen E-435
  - Engpass E-439
  - Maschine E-440
  - reservieren E-438
  - sperren E-437
  - verlängern, verkürzen E-438
  - zusätzlich einrichten E-435
- Arbeitsschichten E-434, E-561
  - Darstellung E-443
- Arbeitsschichten erzeugen E-490
- Arbeitsvorbereitung C-101
- Arbeitsweise
  - Datenübernahne J-1069
  - Tischansteuerung J-1091
- Übersicht J-1067, J-1073, J-1081, J-1092
- Artikelnummer für fehlende Bearbeitung
  - Bearbeitung D-380
- Asynchrone Verarbeitung E-591
- Auffang-Abstellplatz D-362
  - Einstellungen-Abstellplatz D-362
- Auffüllbedingung
  - Master-Orga D-355
- Aufgefüllte Fächerwagen
  - Gruppierung und Sortierung D-337
  - Nummernkreise D-338
  - Optimierung D-338
  - Produktionsreihenfolge D-337
  - Standard-Produktionsorganisation D-337
- Auflösen
  - Tischoptimierung J-1086
- Aufsteigend
  - Gruppierung D-367
- Auftrag
  - auswählen (Produktionsmonitor) E-569
  - einlasten E-447
  - Einlastung nachbearbeiten E-453
  - Reservierung E-467
  - Umlastung E-448
- Auftrag zu Positionen hinzufügen C-184
- Aufträge C-122, C-147
  - fehlerhafte Angaben C-124
  - Kapazitätsplanung C-124
- Auftrags-Nr.
  - Detail-Ansicht 1-986
- Auftragsübersicht C-150
- Ausschalten
  - Import J-1072
- Auswahl Bedingungen
  - Beschreibung F-695
  - Dialog F-694
  - Editieren F-695
  - Keine Bedingung F-695
  - Löschen F-695
  - Neue Bedingung F-695
  - Vorhandene Bedingungen F-695
- Auswahl Formeln
  - Beschreibung F-716
  - Dialog F-715
  - Editieren F-716
  - Keine Formel F-716
  - Löschen F-716
  - Neue Formel F-716
  - Vorhandene Formeln F-716
- Auswahl Mengen
  - Beschreibung F-707
  - Dialog F-706
  - Editieren F-707
  - Keine Menge F-707
  - Löschen F-707
  - Neue Menge F-707
  - Vorhandene Menge F-707
- Auswahl Zuweisung
  - Beschreibung F-720
  - Dialog F-720
  - Editieren F-720
  - Keine Zuweisung F-720
  - Löschen F-720
  - Neue Zuweisung F-720
  - Vorhandene Zuweisung F-720
- Auswählen
  - Bruchscheibe J-1084
  - Eilscheibe J-1084
  - Glasart J-1157
  - Job J-1136, J-1137
  - Lagerplatte J-1166
  - Lauf J-1083, J-1094, J-1179
  - Optimierung J-1157, J-1179
- Automatische Umlastung E-429

### B
- BDE C-203
- BDE-Buchungen
  - lückenlose Buchung H-929
- Bearbeiten
  - Restblatt J-1186
- Bearbeitung
  - Artikelnummer für fehlende Bearbeitung D-380
  - auflösen E-478
  - Beschaffungsart D-380
  - ergänzen E-477
  - erzeugen E-477
  - Lostyp D-380
  - Name D-379
  - Typ D-379
  - Umlastung E-449
- Bearbeitungen C-191
  - Positionen splitten E-594
  - Register D-379
  - umlasten E-450
  - Vorgabezeiten ändern C-194
- Bearbeitungsartikel G-791
  - anlegen G-798
- bearbeiten G-800
- erstellen G-798
- in der MZO A-43, G-793
- löschen G-801
- verwalten G-798
- Zuordnung zu Bearbeitungstyp auflösen G-801
- Bearbeitungsdauer siehe Vorgabezeiten
- Bearbeitungserzeugung E-476, E-610
  - Bearbeitung entfernen E-478
  - Bedingung hinzufügen E-612
  - Reihenfolge E-611
  - Sequenz E-611
- Bearbeitungsketten E-429
- Bearbeitungstypen G-791, G-840, G-841
  - anlegen G-795
  - bearbeiten G-796
  - erstellen G-795
  - in der MZO A-43, G-792
  - löschen G-797
  - verwalten G-795
- Bedingung
  - Bedingungen F-700
  - Bedinungen-Erzeuger F-699
  - Invertieren F-702
  - Mittleres Auswahlfeld F-699
  - Normal F-700
  - Oberes Eingabefeld F-699
  - Stufe I F-661
  - Stufe II F-666
  - Übergebene Menge F-703
  - Unteres Eingabefeld F-700
  - Wert F-700
- Bedingung auswählen G-787, G-822
- Bedingungen
  - Bedingung F-700
- Bedingungen und Formeln G-785, G-832
  - Bearbeitungsdauer G-788, G-826
  - in der MZO G-786
- Bedingungen-Erzeuger
  - All F-698
  - Bedingung F-699
  - Dialog F-696
  - Menü F-696
  - Null F-698
  - One F-698
  - Werkzeugleiste F-697
- Bedingungseditor
  - grafische Variante G-834
  - Text-Variante G-838
- Begriffe in der Grobplanung C-102
- Benutzerdefinierte Tabellenelemente E-626
- Berechnungsreihenfolge E-618
- Vorgabezeitformel E-524
- Beschädigte Scheiben L-1244
- Beschaffungsart
  - Bearbeitung D-380
- Beschaffungsart ändern C-157
- Beschichtete Gläser G-741
- Beschreibung
  - Auswahl Bedingungen F-695
  - Auswahl Formeln F-716
  - Auswahl Mengen F-707
  - Auswahl Zuweisung F-720
  - Formel Editor F-718
- Bestellteile C-165
- Bestellteile-Topf C-165
- Betriebsdatenerfassung C-203
- Bildung der Gruppen
  - Einstellungen-Abstellplatz D-361
  - Orga-Gruppen D-359
- Bottom
  - Mengen Erzeuger F-710
- Breite
  - Gestell hinzufügen I-1051
- Breite Zuschlag
  - Kiste hinzufügen I-1053
- Bruch
  - erfassen J-1194
- Bruchscheibe
  - auswählen J-1084
  - erfassen J-1077
  - löschen J-1078, J-1079
  - optimieren J-1084
  - Pool J-1192

### C
- Chefauftrag E-584
- Child
  - Mengen Erzeuger F-710
- Cluster-Ansicht J-1197

### D
- Datenerfassung
  - Bruchscheiben J-1075
  - Eilscheiben J-1075
  - Füllaufträge J-1075
- Datenübernahme
- Stand alone-System J-1205
- Datenübernahne
  - A+W Production J-1070
  - Arbeitsweise J-1069
  - Stand alone-System J-1071
- Datenverarbeitung
  - Tischoptimierung J-1083
- Defect Optimizer J-1134
- Denso-Scanner H-891
- Detail-Ansicht
  - Anzahl 1-986
  - Auftrags-Nr. 1-986
  - Fläche 1-986
  - Gestell# 1-983
  - Gestellbezeichnung 1-986
  - Gestell-ID 1-986
  - Gewicht 1-986
  - Größe. I-986, I-987
  - PM-Gruppe 1-986
  - Positions-Nr. 1-986
  - Produktions-Linie 1-987
  - Reihe 1-986
  - Seite 1-983
  - Stapel 1-983
  - Typ 1-986
  - Vert. Stapel 1-986
- Details C-199
- Dialog
  - Auswahl Bedingungen F-694
  - Auswahl Formeln F-715
  - Auswahl Mengen F-706
  - Auswahl Zuweisung F-720
  - Bedinungen-Erzeuger F-696
  - Eingabe Zahlenwert F-704
  - Formel Editor F-717
  - Info F-702, F-714
  - Mengen Erzeuger F-708
  - Name der Bedingung F-701
  - Name der Menge F-712
  - Zuweisung Editor F-720
- Direkte Objekte H-864
- Dokumente
  - verknüpfen C-219
- Dokumentenverknüpfungen C-219
- Drucken
  - Auftragsübersicht L-1247
- DynOpt Einstellung D-359

### E
- Editieren
  - Auswahl Bedingungen F-695
  - Auswahl Formeln F-716
  - Auswahl Mengen F-707
  - Auswahl Zuweisung F-720
- Editor-Gruppierungen
  - Register D-367
- Editor-Sortierung
  - Register D-369
- Eigene Filter (Produktionsmonitor) E-570
- Eigenschaft
  - Gruppierung D-368
  - Zuweisung Editor F-721
- Eigenschaften Formelobjekt E-629
- Eigenschaften von Register C-214
- Eilscheibe
  - anzeigen J-1144
  - auswählen J-1084
  - erfassen J-1076, J-1146
  - löschen J-1077
  - optimieren J-1084
- Einabefeld oben
  - Zuweisung Editor F-720
- Eingabe Zahlenwert
  - Alter Wert F-704, F-705
  - Dialog F-704
  - Länge F-705
  - Neuer Wert F-704
  - SZR F-705
  - Text F-705
  - Ziffer F-705
- Eingabefeld oben
  - Formel Editor F-718
- Eingabehilfe für Vektoren E-622
- Einheiten scannen H-897
- Einlastung E-560, E-580
  - Änderung verplanter Aufträge E-593
  - Asynchrone Verarbeitung E-591
  - Aufträge einlasten E-447
  - Bearbeitungserzeugung E-476
  - Fehler E-452, E-588
  - Fehlerhafte Aufträge E-591
  - nachbearbeiten E-453
  - Nachbearbeitung Einlastung E-588
  - Positionssplit E-594
  - Stücklistenkonfiguration E-581
- Einlastungsregeln E-426
- Einschalten
  - Import J-1071
- Einstellungen
  - Produktionsreihenfolge D-351
  - Tische J-1202
  - Tischoptimireung J-1203
- Einstellungen-Abstellplatz
  - Abstellmodus D-363
  - Abstellmodus Gruppen D-361
  - Abstellplatz-Typ (Register Verwendung) D-363
  - Auffang-Abstellplatz D-362
  - Bildung der Gruppen D-361
  - Dialog D-361
  - Max. Anzahl Gruppen (Register Verwendung) D-362
  - Name D-361
  - Optimierungsverhalten D-362
  - Register Verwendung, Von/Bis D-362
  - Sortierung in den Gruppen D-361
- Einzeltermin (Kampagne) E-598
- Einzeltermine in Kampagne anlegen E-460
- Elemente hinzufügen (Vorgabezeit) E-620
- Ende
  - Bruch, Master-Orga D-356
  - Füller, Master-Orga D-355
  - Prüfreihenfolge D-352
  - Restblatt, Master-Orga D-356
- Engpass
  - Arbeitsschicht E-439
  - Maschine E-441
- Entschichtungsflächen C-220
- Erfassen
  - Bruchscheibe J-1077, J-1194
  - Eilscheibe J-1076, J-1146
- Erfassungsstelle
  - Aktueller Zustand H-943
  - Barcode H-942
  - Bearbeitungsrückmeldung H-945
  - Beschreibung H-942
  - Betriebsmittel für Auftragserfassung H-945
  - Einheitenrückmeldung H-945
  - Erfassungsstellentyp H-943
  - Gestellbelegung melden H-945
  - Gestellrückmeldung H-945
  - Gruppierung H-943
  - Gruppierung für Schichten H-943
  - LKW H-873
  - Mengenüberschreitung H-943
  - Name H-942
  - Nummer H-942
  - Produktionsrückmeldung H-945
  - Produzierte Teile H-944
  - Restriktionen H-943
  - Text für Kundenlisten H-942
  - Text für Produktionslisten H-942
  - Unterzeile für Etiketten H-943
- Erfassunsstellen
  - Verwalten H-871
- ERP-System A-11
- Erstellen
  - Tischoptimierung J-1084, J-1136
- Erzeuge Zusatz-Sortierung
  - Dialog D-371
  - Sortierung D-369
  - Wert D-371
  - Wert nicht prüfen D-371
- Erzeugen
  - Schneidcode J-1183
- Erzeugung
  - Abhängige Bearbeitung D-381
- Expertenmodus
  - Überblick H-921
- Export/Import
  - Positionsansicht C-189
- Exportieren
  - Arbeitsplan E-445
  - Log-Einträge L-1247

### F
- Fächerwagen ohne Auffüllen
  - Gruppierung und Sortierung D-333
  - Nummernkreise D-334
  - Optimierung D-333
  - Produktionsreihenfolge D-332
  - Standard-Produktionsorganisation D-332
- Faktoren E-621
- Faktoren (Vorgabezeitformel) E-521
- Farbliche Darstellung der Einheit L-1251
- Fehler
  - Einlastung E-452
- Fehlergestell H-868
- Fehlerhafte Aufträge E-591
- Fehlermeldung J-1072, J-1206
- Feinplanung für Lauf ...
  - Dialog D-382
  - Register Auswahl Lagermaß D-412
  - Register Bockbelegung D-386
  - Register Bruchscheiben D-398
  - Register Eilscheiben D-400
  - Register Ergebnisse D-391
  - Register Freie
- Optimierung D-403
- Register Füllaufträge D-395
- Register Glasarten D-383
- Register Glasdicken D-401
- Register Optionen D-410
- Register Orga D-406
- Register Orga-Optionen D-408
- Register Restblätter D-397
- Register Spezial D-393
- Register Teilmengen D-404
- Register Zusammenlegen D-393
- Felddefinition C-187
- Fertigungsgruppen D-354
  - Master-Orga D-354
- Feste Elemente (Vorgabezeitformel) E-521
- Filter
  - bearbeiten C-216
  - definieren C-217
- Filter konfigurieren C-117
- Filter-Definition C-217
- Filterfunktion
  - Pool-Anzeige I-1034
- Fläche
  - Detail-Ansicht I-986
- Formel
  - Formel Editor F-718
  - Gruppierung D-368
  - Stufe I F-660
  - Stufe II F-665
  - Zuweisung Editor F-721
- Formel auswählen E-624, G-787, G-822
- Formel Editor
  - Anzahl Resultate F-719
  - Beschreibung F-718
  - Dialog F-717
  - Eingabefeld oben F-718
  - Formel F-718
  - Maximum F-718
  - Menge F-718
  - Minimum F-718
  - Mittelwert F-718
  - Oder-Verknüpfung F-718
  - Summe F-718
  - Übergebene Menge F-718
  - Und-Verknüpfung F-718
  - Vorhandene Eigenschaften F-719
  - Vorhandene Formeln F-719
- Formelauswertung E-631
- Formel-Editor
  - grafische Variante G-834
  - Text-Variante G-838
- Formeln und Bedingungen G-785, G-832
  - Bearbeitungsdauer G-788, G-826
  - in der MZO G-786
- Formelobjekt E-627
- Form-Erfassung J-1148
- Fortsetzen
  - Zuschnitt J-1099
- Freier Editier-Modus I-991
- Füllauftrag
  - verwenden J-1086
- Füllaufträge C-153

### G
- Gesamtes Ofenbett buchen (Terminal TG-Out) L-1317
- Gestell hinzufügen
  - Breite I-1051
  - Höhe I-1051
  - Tiefe I-1051
- Gestell#
  - Detail-Ansicht I-983
- Gestellbezeichnung
  - Detail-Ansicht I-986
- Gestellbezeichnung ändern
  - PackView I-1050, I-1051, I-1053
- Gestelle H-875
  - Aktuelle ES H-948
  - Aktueller Zustand H-948
  - Basis ES H-948
  - BC-Startwert H-946
  - Endwert H-946
  - Fachnummer von ... bis H-947
  - Filtern H-875
  - Gestellart H-946
  - Gestelltyp H-947
  - Kundenname H-948
  - Kundennummer H-948
  - Letzte ES H-948
  - Letzter Zustand H-948
  - Lieferort H-949
  - Mehrere Gestelle anlegen H-946
  - Präfix H-946
  - Startwert H-946
  - Temporäres Gestell H-948
  - Tournummer H-949
- Gestellfilter
  - Betriebseigene Gestelle H-950
  - Erfassungsstelle H-950
  - Erfassungsstellentyp H-950
- Gestellart H-950
- Gestellname von bis H-950
- Gestelltyp H-950
- Gestell-ID
  - Detail-Ansicht I-986
- Gewicht
  - Detail-Ansicht I-986
- Glasart
  - auswählen J-1157
- Glasarten C-196
- Globale Einstellungen
  - Funktionsprinzip D-307
- Grobplanung
  - Begriffe C-102
- Größe.
  - Detail-Ansicht I-986, I-987
- Größenklasse A-Böcke Versand D-327
- Grundgedanke
  - Schneidcodegenerierung J-1065
  - Zuschnittsoptimierung J-1065
- Gruppenbildung
  - Voreinstellungen D-365
- Gruppierung
  - Absteigend D-367
  - Aufsteigend D-367
  - Eigenschaft D-368
  - Formel D-368
  - Lostyp D-377
- Gruppierung und Sortierung
  - A-Böcke D-322
  - A-Böcke Versand D-328
  - Aufgefüllte Fächerwagen D-337
  - Fächerwagen ohne Auffüllen D-333

### H
- Hilfethemen
  - Online-Hilfe A-84
- Hoch
  - Prüfreihenfolge D-352
  - Reihenfolge der Maschinen D-413
- Höhe
  - Gestell hinzufügen I-1051
- Höhe Zuschlag
  - Kiste hinzufügen I-1053

### I
- ID für Stack-Opti
  - Fächerwagen D-373
- Import
- ausschalten J-1072
- Daten J-1205
- einschalten J-1071
- Importieren
  - Lauf J-1071
- Index
  - Online-Hilfe A-86
- Indirekte Objekte H-864
- Info
  - Dialog F-702, F-714
- Infofelder L-1238
- Invertieren
  - Bedingung F-702

### J
- Job
  - auswählen J-1136, J-1137
  - schneiden J-1183

### K
- Kalender
  - arbeitsfreie Tage anlegen E-484
  - arbeitsfreie Tage bearbeiten E-485
  - arbeitsfreie Tage löschen E-486
- Kampagne
  - anlegen E-458
  - bearbeiten E-464
  - deaktivieren E-465
  - Einzeltermin anlegen E-460
  - löschen E-465
  - Termin löschen E-464
  - wöchentlichen Termin anlegen E-462
- Kampagnen E-597
  - Einzeltermine E-598
  - Einzeltermine, Wöchentliche Termine E-456
  - Kampagnentage E-598
  - Terminfindung E-458
  - Wöchentliche Termine E-600
- Kampagnentage E-598
- Kapazität reservieren E-467
- Kapazitätsplanung C-102
- Kein Teilen von...bei Bockbelegung von mehr als... Prozent
  - Orga D-357
- Keine Bedingung
  - Auswahl Bedingungen F-695
- Keine Formel
  - Auswahl Formeln F-716
- Keine Menge
- Auswahl Mengen F-707
- Keine Zuweisung
  - Auswahl Zuweisung F-720
- Kiste hinzufügen
  - Breite Zuschlag I-1053
  - Höhe Zuschlag I-1053
  - Tiefe Zuschlag I-1053
- Kisten H-876
- Komponenten-ID G-743
- Kontextmenüs C-221
- Korrekte Daten H-929
- Kosten E-646
  - anlegen E-502
  - bearbeiten E-503
  - löschen E-504
- Kostenkalkulation E-646
  - Definition E-501
- Kunde für Reservierung auswählen E-606
- Kurzbeschreibung Standard-Produktionsorganisation D-313

### L
- Lagerplatte
  - auswählen J-1085, J-1166
- Länge
  - Eingabe Zahlenwert F-705
- Lastverteilung E-649
  - bearbeiten E-554
  - Definition E-551
  - einrichten E-552
  - löschen E-555
- Lauf
  - auswählen J-1083, J-1179
  - zurücksetzen J-1173
  - zuschneiden J-1094
- Lauf auswählen (Produktionsmonitor) E-569
- Laufbezeichnung ändern C-176
- Lauf-Bildung C-173
- Läufe C-131, C-170
  - auflösen C-137
  - Auftrag hinzufügen C-136
  - Bezeichnung ändern C-176
  - bilden C-134, C-173
  - Laufstrategien C-133
  - Sonderglas-Lauf C-175
  - Verlinken J-1090
  - verwalten C-137
- Läufe auflösen C-137
- Läufe bilden C-134
- Läufe verwalten C-137
- Laufnummer/Losnummer
  - Terminal IG L-1239
- Laufstrategien C-133
- L-Bock
  - Dialog Abstellplatz D-372
- Leergewicht Fächerwagen D-374
- Leistungsmerkmale J-1066
- Leitstand J-1091
- Liste C-111
- Liste aktuelle Einheit
  - Terminal IG-In L-1237
- Logische Maschine G-755, G-756, G-810
  - anlegen G-758, G-823
  - bearbeiten G-760, G-824
  - Bearbeitungsdauer G-826, G-839
  - erstellen G-758, G-823
  - Formel-Auswahl G-826, G-839
  - Kosten anlegen E-502
  - löschen G-761
  - Schichtgruppe E-643
  - verwalten G-758
  - Vorgabezeit E-519
- Logische Maschine siehe auch Maschine
- Los
  - Reihenfolge J-1097
- Los laden
  - Terminal IG-In L-1241
- Löschen
  - Auswahl Bedingungen F-695
  - Auswahl Formeln F-716
  - Auswahl Mengen F-707
  - Auswahl Zuweisung F-720
  - Bruchscheibe J-1078, J-1079
  - Eilscheibe J-1077
- Lose C-207
- Lostyp
  - Abhängige Bearbeitung D-381
  - Bearbeitung D-380
  - Gruppierung D-377
  - Name D-377
  - Name/Typ/Beschaffungsart D-377
  - Nummer D-377
  - Produktionsreihenfolge D-377
  - Sortierung invertieren D-378
  - Technologietyp D-377
  - Verhalten in der Feinplanung D-378
- Lostypen
  - Register D-376

### M
- Marken D-233
- Marktentest
  - Testmarke D-233
- Maschine A-40, G-737, G-738, G-809
  - Abmessungsrestriktionen G-742, G-752, G-753, G-820
  - anlegen G-744, G-814
  - Anzeigeart einstellen E-444
  - Arbeitsschicht E-440
  - bearbeiten G-745, G-748, G-815
  - beschichtete Gläser G-741, G-750
  - Eigenschaften bearbeiten G-745
  - Engpass E-441
  - erstellen G-744, G-814
  - Komponenten-ID G-743
  - Kosten anlegen E-502
  - Kosten bearbeiten E-503
  - Kosten löschen E-504
  - löschen G-747
  - maximale Dicke G-748
  - maximale dicke G-741
  - minimale Dicke G-741
  - minimale dicke G-748
  - Modelle G-741, G-750
  - Namen und Nummern G-740
  - Restriktionen G-741
  - Scheibenformat G-742
  - Strukturgläser G-742, G-750
  - Stufen-ISO G-742, G-750
  - SZR-Restriktionen G-742, G-752, G-753, G-821
  - Umlastung E-448
  - UND-/ODER-Verknüpfungen G-742
  - verwalten G-744
  - X-, Y-, Z-,W-Schnitte G-817
  - zusätzliche Bedingung G-743
- Maschine siehe auch Logische Maschine
- Maschinen
  - Anzeige im Produktionsmonitor E-565
  - im Produktionsmonitor anzeigen E-442
- Maschinengruppe
  - anlegen E-546
  - bearbeiten E-548
  - löschen E-549
- Maschinengruppen E-647
  - Definition E-545
- Maschinenrestriktionen G-741
  - bearbeiten G-748
- Maschinenschichten E-561
- Maschinentyp
  - anlegen G-830
  - bearbeiten G-831
- Maschinentypen G-813
- Maschinenumlastung E-587
- Maschinenwege
  - Alternativmaschinen E-431
  - Bearbeitungsketten E-429
- Maschinenzuordnung G-736
  - Arbeitsgang G-763
  - Arbeitsgangzuordnung G-774
  - Bestandteile G-734
  - logische Maschine G-755
  - Maschine A-40, G-737, G-738
  - Schaltflächen G-803
- Maschinenzustand L-1242
- Master
  - Mengen Erzeuger F-710
- Master-Orga
  - Auffüllbedingung D-355
  - Dialog D-353
  - Ende Bruch D-356
  - Ende Füller D-355
  - Ende Restblatt D-356
  - Fertigungsgruppen D-354
  - Mindestmenge D-354
  - Name D-353
  - Pseudoserien D-354
  - Quasi Teile D-355
  - Register D-348
  - Schnell-Orga D-353
  - Script D-354
  - Start Bruch D-356
  - Start Füller D-355
  - Start Restblatt D-356
  - Verwende Bruchscheiben D-356
  - Verwende Eilscheiben D-356
  - Verwende Füller D-355
  - Verwende Restblätter D-355
  - XOPT zusammen abstellen D-353
- Matrix für Übergangszeiten E-513
- Max
  - Anzahl Fächerwagen, Dialog Abstellplatz D-373, D-374
  - Anzahl Gruppen (Register Verwendung), Dialog Einstellungen-Abstellplatz D-362
- Max. Abstellplätze/Bock
  - Abstellplätze D-372
- Maximale Dicke G-741
- Maximale Nutzlast
  - Fächerwagen D-374
- Maximales Gewicht
  - A-Bock D-373
  - FAP D-375
- Maximum
  - Formel Editor F-718
- Menge
  - Formel Editor F-718
  - Stufe I F-664
  - Stufe II F-668
  - Stufe III F-669
  - Zuweisung Editor F-721
- Mengen Erzeuger
  - Addup F-711
  - All F-710
  - Anychild F-710
  - Bottom F-710
  - Child F-710
  - Dialog F-708
  - Master F-710
  - Menü F-709
  - Parent F-710
  - Self F-710
  - Up F-710
  - Werkzeugleiste F-710
- Menü
  - Bedinungen-Erzeuger F-696
  - Mengen Erzeuger F-709
- Software J-1141
- Menüleiste L-1236
- Mindestmenge
  - Master-Orga D-354
- Minimale Dicke G-741
- Minimum
  - Formel Editor F-718
- Mittelwert
  - Formel Editor F-718
- Mittleres Auswahlfeld
  - Bedingung F-699
- Modellanzeige L-1236
- Modelle G-741
- Modellscheibe J-1196
- Modul
  - Funktion H-857
- Module
  - angeschlossene J-1103
  - Defect Optimizer J-1134
  - PlanEditor J-1126
- MZO G-736
  - Bestandteile G-734
- MZO-Editor
- Arbeitsgänge G-811
- Arbeitsgangzuordnung G-812
- Logische Maschinen G-810
- Maschinen G-809
- Maschinentypen G-813

### N
- Nachbearbeitung Einlastung E-588
- Änderung verplanter Aufträge E-593
- Fehlerhafte Aufträge E-591
- Nachläufer laden
  - Terminal IG-In L-1246
- Name
  - Abhängige Bearbeitung D-381
  - Bearbeitung D-379
  - Einstellungen-Abstellplatz D-361
  - Lostyp D-377
  - Master-Orga D-353
  - Orga-Gruppen D-359
- Name der Bedingung
  - Alte Bezeichnung F-701
  - Dialog F-701
  - Neue Bezeichnung F-701
- Name der Menge
  - Alte Bezeichnung F-713
  - Dialog F-712
  - Neue Bezeichnung F-713
- Name der Orga-Form
  - Orga D-357
- Name/Typ/Beschaffungsart
  - Lostyp D-377
- Neu
  - Produktionsreihenfolge D-350
  - Schaltflächen A-80
- Neue Bedingung
  - Auswahl Bedingungen F-695
  - Produktionsreihenfolge D-350
- Neue Bezeichnung
  - Name der Bedingung F-701
  - Name der Menge F-713
- Neue Formel
  - Auswahl Formeln F-716
- Neue logische Maschine G-823
- Neue Maschine G-744, G-814
- Neue Menge
  - Auswahl Mengen F-707
- Neue Zuweisung
  - Auswahl Zuweisung F-720
- Neuen Filter erstellen (Produktionsmonitor) E-571
- Neuer Arbeitsgang G-826
- Neuer Maschinentyp G-830
- Neuer Wert
  - Eingabe Zahlenwert F-704
- Normal
  - Bedingung F-700
- Null
  - Bedinungen-Erzeuger F-698
- Nummer
  - Lostyp D-377
- Nummernkreise
  - A-Böcke D-323
  - A-Böcke SZR D-315
  - A-Böcke Versand D-329
  - Aufgefüllte Fächerwagen D-338
  - Fächerwagen ohne Auffüllen D-334

### O
- Oberes Eingabefeld
  - Bedingung F-699
- Oberläche L-1235
- Objekt auswählen (Reservierung) E-608
- Oder-Verknüpfung
  - Formel Editor F-718
- Offene Bearbeitung Terminal TG-In L-1309
- Offline-Scanner H-892
- OK
  - Schaltflächen A-80
- One
  - Bedinungen-Erzeuger F-698
- Online-Hilfe
  - Hilfethemen A-84
  - Index A-86
  - Inhalt A-85
  - Suchen A-87
- Online-Scanner H-891
- Optimieren
  - Bruchscheibe J-1084
  - Eilscheibe J-1084
  - Glasart wählen J-1157
  - Restelagerplatte J-1112
  - Tischoptimierung J-1164
- Optimierung
  - A-Böcke D-323
  - A-Böcke SZR D-315
  - Aktuell geänderte Einstellungen J-1177
  - Aufgefüllte Fächerwagen D-338
  - auswählen J-1179
  - Fächerwagen ohne Auffüllen D-333
  - importieren J-1071
  - Lagerplatte wählen. J-1085
  - Pausierende Glasarten J-1175
  - prüfen J-1097
  - schneiden J-1097
- Optimierungsverhalten
  - Einstellungen-Abstellplatz D-362
- Orga
  - Abstellmodus D-357
  - Dialog D-348, D-357
  - Funktionsprinzip D-247
  - Kein Teilen von...bei Bockbelegung von mehr als...Prozent D-357
  - Name der Orga-Form D-357
  - Produktion D-357
  - Typ D-357
  - Voreinstellungen D-365
- Orga-Gruppen
  - Bildung der Gruppen D-359
  - Dialog D-359
  - Name D-359
  - Sortierung der Gruppen D-359
  - Sortierung in den Gruppen D-359

### P
- Packmittelgruppe I-1031
- Packmittelgruppen
  - Beschreibung I-1031
  - Packmittelgruppe I-1031
  - Packmittelhauptgruppe I-1030
  - Packmittelregel I-1031
  - Positionen von einer Optimierung ausschließen I-1031
  - Produktionslinien zusammenpacken I-1031
- Packmittelhauptgruppe I-1030
- Packmittelregel I-1031
- PackView
  - Automatische Sicherung I-1040
  - Datei öffnen I-1040
  - Datei schließen I-1040
  - Drucken I-1041
  - Drucker Setup I-1041
  - Druck-Vorschau I-1041
  - Gestellbezeichnung ändern I-1050, I-1051, I-1053
  - Menü I-1040, I-1055
  - Programm Beenden I-1041
  - Symbol-Schaltflächen I-1045
- Parent
- Mengen Erzeuger F-710
- Pausierende Glasarten J-1175
- Personal H-954
- PlanEditor J-1126
- Platte
  - erneut schneiden J-1102
  - nicht schneiden J-1095
- PM-Gruppe
  - Detail-Ansicht I-986
- Pool C-122
- Pool-Anzeige
  - Filterfunktion I-1034
  - Schaltfläche zur Schnellanwahl I-1034
  - Summenzeile I-1034
- Positionen C-138, C-181
  - Auftrag hinzufügen C-184
  - Felddefinition C-187
  - Import/Export Ansicht C-189
  - splitten C-140, C-185
- Positionen splitten E-594
- Positions-Nr.
  - Detail-Ansicht I-986
- Positionssplit C-185
- Produktion
  - Orga D-357
- Produktionshinweistexte Terminal IG L-1239
- Produktions-Linie
  - Detail-Ansicht I-987
- Produktionsmonitor E-434, E-561
  - angezeigte Maschinen E-565
  - Anpassungen E-435
  - Anzeige einstellen E-443
  - Arbeitsschichten erzeugen E-490
  - Auftrag auswählen (Produktionsmonitor) E-569
  - Darstellung der Schichten E-566
  - Detailansicht E-435
  - Eigene Filter E-570
  - Einstellungen E-566
  - Lauf auswählen E-569
  - Maschine E-572
  - Maschinen anzeigen E-442
  - nach Auftrag filtern E-569
  - nach Lauf filtern E-569
  - neuen Filter erstellen E-571
  - Schichteigenschaften E-574
  - Schichten anpassen E-573
- Produktionsreihenfolge
  - A-Böcke D-321
  - A-Böcke Versand D-328
  - Aufgefüllte Fächerwagen D-337
  - Einstellungen D-351
  - Fächerwagen ohne Auffüllen D-332
  - Lostyp D-377
  - Neu D-350
  - Neue Bedingung D-350
  - Register D-350
- Produktionsstatus
  - zurücksetzen J-1102
- Produktionstermine
  - Bewertung E-431
- Produktportfolio A-11
- Programmsprache ändern L-1248
- Prüfreihenfolge
  - Anfang D-352
  - Ende D-352
  - Funktionsprinzip D-304
  - Hoch D-352
  - Register D-351
  - Runter D-352
- Pseudoserien D-354
  - Master-Orga D-354

### Q
- Quasi Teile
  - Master-Orga D-355

### R
- Rechtsklick C-221
- Regeln
  - .Bezeichnung der .RUL-Datei I-1025
  - RUL-Datei I-1025
  - RUL-Datei laden I-1025
  - Beschreibung der .RUL-Datei I-1025
  - Terminfindung E-428
  - Terminoptimierung E-427
- Register
  - Eigenschaften C-214
- Register konfigurieren C-107
- Reihe
  - Detail-Ansicht I-986
- Reihenfolge
  - Los J-1097
  - Zuschnitt J-1097, J-1185
- Reihenfolge der Maschinen
  - Dialog D-413
  - Hoch D-413
  - Runter D-413
- Reservierung
  - abgelaufen E-468
- abgelaufene Reservierung löschen E-473
- abgelaufene Reservierungen E-601
- anlegen E-469
- Auftrag E-467
- bearbeiten E-471
- Kapazitäten E-467
- Konfiguration E-466
- Kunde auswählen E-606
- löschen E-472
- Objekt auswählen E-608
- pro Maschine E-604
- pro Schicht E-604
- Reservierung für Maschine E-606
- Reservierungen E-603
- pro Kunde E-604
- tageweise, wochenweise E-604
- Reservierungsaufträge C-161
- Reservierungsaufträge-Topf C-161
- Restblatt
  - anzeigen J-1097
  - bearbeiten J-1186
  - verwenden J-1085
- Restelagerplatte
  - optimieren J-1112
- Robot
  - Abstellplatz D-373
  - Funktionsprinzip D-275
- Runter
  - Prüfreihenfolge D-352
  - Reihenfolge der Maschinen D-413

### S
- Scannen
  - Einheiten H-897
- Scanner
  - Konfiguration H-892
- Schaltflächen A-78
  - Neu A-80
  - OK A-80
  - Schließen A-81
  - Speichern A-81
  - Suchen A-81
- Schaltflächen allgemein
  - Bruch L-1239
  - Produzieren L-1239
- Schaltflächen in der MZO G-803
- Schaltflächen Terminal IG
  - Überspringen L-1239
- Schaltflächen Terminal IG-In
- Los Laden L-1239
- Schaltflächen Terminal TG-Out L-1315
- Schaltflächen ToolTV IG-In
  - Nachläufer L-1239
- Scheibe
  - erfassen J-1076
- Scheibe produzieren
  - Terminal IG-In L-1241
- Scheibenformat G-742
- Schicht
  - Sonderfall für Wechsel E-510
- Schichteigenschaften E-574
- Schichten E-636
  - Logische Maschine E-643
  - Schichtgruppe E-495, E-641
  - Schichtkalender E-637
  - Schichtplan E-489, E-637
  - Schichtregel E-493, E-639
  - Übergangszeit E-632
- Schichten anpassen E-573
- Schichtgruppe E-641
  - bearbeiten E-498
  - erstellen E-495
  - löschen E-499
- Schichtkalender E-637
- Schichtplan E-637
  - bearbeiten E-489
  - erstellen E-488
  - löschen E-490
- Schichtpläne E-482
- Schichtregel E-639
  - bearbeiten E-493
  - erstellen E-491
  - löschen E-494
- Schichtreservierungen E-604
- Schichtwechsel Sonderfall E-510
- Schließen
  - Schaltflächen A-81
- Schlüssel
  - Zusatz-Sortierung D-370
- Schneidcode
  - erzeugen J-1183
  - nicht erstellen J-1095
- Schneiden
  - Job J-1183
- Schnell-Orga
  - Master-Orga D-353
- Schwellenwert (Vorgabezeitformel) E-528
- Script
  - Master-Orga D-354
- Seite
- Detail-Ansicht I-983
- Self
  - Mengen Erzeuger F-710
- Sequenz (Bearbeitungserzeugung) E-611
- Serielle Scanner H-892
- Software
  - Menü J-1141
  - Übersicht J-1141
- Softwarebegriffe A-77
- Sonderglas-Lauf bilden C-175
- Sortierung
  - Erzeuge Zusatz-Sortierung D-369
  - Sortierung auf Abstellplatz Voreinstellungen D-365
- Sortierung der Gruppen
  - Orga-Gruppen D-359
- Sortierung in den Gruppen
  - Einstellungen-Abstellplatz D-361
  - Orga-Gruppen D-359
- Sortierung invertieren
  - Lostyp D-378
- Sortjet
  - Fächerwagen D-373, D-374
- Spalte definieren C-114
- Spalten
  - Definition C-215
- Spalten konfigurieren C-109
- Spaltendefinition C-215
- Speichern
  - Schaltflächen A-81
- Sprossenansicht Terminal IG L-1239
- Stammdaten J-1071
  - Kapazitätsplanung E-426
  - Maschinenzuordnung E-426
  - Schutz, Datensicherung E-480
- Stand alone-System
  - Datenimport J-1205
- Standard-Produktionsorganisation
  - A-Böcke D-321
  - A-Böcke Versand D-327
  - Fächerwagen ohne Auffüllen D-332
  - Kurzbeschreibung D-313
- Standard-Produktionsorganisationen
  - Aufgefüllte Fächerwagen D-337
- Standard-Report
  - Abstellliste H-923
  - Auftragsstatus H-924
  - Auftragsübersicht H-923
  - Buchungshistorie H-926
  - Gestellbelegung pro Position H-926
  - Gestellbelegung pro Scheibe H-925
  - Ladeliste H-924
- Stapel
  - Detail-Ansicht I-983
- Start
  - =0, Abstellplatz D-374
  - Bruch, Master-Orga D-356
  - Füller, Master-Orga D-355
  - Restblatt, Master-Orga D-356
- Starten
  - Zuschnitt J-1183
- Status setzen C-102
- Statusbarcode
  - Scannen H-909
- Strukturgläser G-742
- Stückliste
  - Teileketten E-428
- Stücklistenkonfiguration E-581
- Stufen-ISO G-742
- Suchen
  - Online-Hilfe A-87
  - Schaltflächen A-81
- Summe
  - Formel Editor F-718
- Summenzeile
  - Pool-Anzeige I-1034
  - Summenzeile definieren C-114
  - Summenzeile konfigurieren C-112
- Symbol-Schaltfläche
  - Pool-Anzeige I-975
- Symbol-Schaltflächen
  - PackView I-1045
  - Übersicht J-1142
- Systemkritische Daten
  - Barcode-Optionen H-939
  - Barcode-Typen H-940
  - Erfassungsstellen-Typen H-941
  - Spalten H-957
  - Spaltenzuordnung H-956
  - Zustandstypen H-951
- SZR
  - Eingabe Zahlenwert F-705
- SZR-Restriktionen G-742, G-821

### T
- Tabelle (Vorgabezeitformel) E-522
- Technologietyp
  - Lostyp D-377
- Terminal Edit
- Arbeitsschritte L-1337
- Terminal IG
  - Laufnummer/Losnummer L-1239
  - Produktionshinweistexte L-1239
  - Produktionsnummer/Bezeichnung L-1236
  - Sprossenansicht L-1239
- Terminal IG-In L-1235
  - Andere Produktionsnummer laden L-1245
  - Anmelden L-1240
  - Arbeitsschritte L-1240
  - Liste der aktuellen Einheit L-1237
  - Los laden L-1241
  - Nachläufer laden L-1246
  - Oberfläche L-1235
  - Scheibe produzieren L-1241
  - Vorschauliste L-1238
- Terminal IG-Out
  - Arbeitsschritte L-1259
- Terminal LG-Assembly
  - Arbeitsschritte L-1329
- Terminal LG-In
  - Arbeitsschritte L-1323
- Terminal Order
  - Arbeitsschritte L-1291
- Terminal Processing
  - Arbeitsschritte L-1300
- Terminal TG-In
  - Arbeitsschritte L-1309
  - Liste Abladereihenfolge L-1315
  - Offene Bearbeitung L-1309
- Terminal TG-Out
  - Arbeitsschritte L-1317
  - Gesamtes Ofenbett buchen L-1317
- Termine
  - Kampagne anlegen E-460, E-462
  - Kampagnen E-456
  - Terminfindung E-428
  - Kampagnen E-458
  - Maschinenwege E-429
  - Produktionstermine E-431
  - Stückliste E-428
  - Übergangszeiten E-507
- Terminoptimierung
  - Regeln E-427
- Text
  - Eingabe Zahlenwert F-705
- Tiefe
  - Gestell hinzufügen I-1051
- Tiefe Zuschlag
  - Kiste hinzufügen I-1053
- Tisch
  - ansteuern J-1183
- Tische
  - Einstellungen J-1202
- Tischoptimierung J-1083
  - Anzahl Lagerplatten J-1172
  - auflösen J-1086
  - Einstellungen J-1203
  - Ergebnis prüfen J-1085
  - erstellen J-1084, J-1136
  - Lagerplatte J-1166
  - Parameter J-1164, J-1169
  - Übersicht J-1161
- Tischoptimierungen
  - verlinken J-1088
- Topfbezeichnung ändern C-168
- Topf-Bildung C-167
- Töpfe C-125, C-159
  - auflösen C-130
  - Aufträge hinzufügen C-128
  - Bestellteile C-165
  - Bezeichnung ändern C-168
  - bilden C-167
  - erstellen C-127
  - Reservierungsaufträge C-161
- Töpfe auflösen C-130
- Töpfe erstellen C-127
- Topic A-84
- Typ
  - Abhängige Bearbeitung D-381
  - Bearbeitung D-379
  - Detail-Ansicht I-986
  - Orga D-357

### U
- Überblick
  - Expertenmodus H-921
- Übergang
  - in Stunden oder Schichten E-507
  - Schichten E-508
  - Stunden E-509
- Übergangszeit
  - anlegen E-514
  - bearbeiten E-516
  - löschen E-516
  - Schichten E-508
  - Sonderfall E-510
  - Stunden E-509
  - Typ E-512
- Übergangszeiten E-505, E-632
  - Definition E-511
  - Matrix E-513
- Schichten E-632
- Terminfindung E-507
- Übergebene Menge
  - Bedingung F-703
  - Formel Editor F-718
  - Zuweisung Editor F-722
- Übergreifende Dialoge C-210
- Übermengen-Editor C-156
- Überprüfung Anzahl
  - Fächerwagen D-373, D-374
  - FAP D-375
- Übersicht
  - Arbeitsweise J-1067, J-1073, J-1081, J-1092
  - Software J-1141
  - Symbol-Schaltflächen J-1142
  - Tischoptimierung J-1161
- Übersichtsdialoge C-104
- Überspringen
  - Zuschnitt J-1095
- Übungen
  - Ansichten C-121
- Umgang mit
  - beschädigten Scheiben L-1244
  - Maschinenzuständen L-1242
- Umlastung E-583
  - Auftrag E-448
  - Bearbeitung E-449
  - Chefauftrag E-583
  - Maschine E-448
  - Maschinenumlastung E-587
  - Termin sperren E-583
  - Wareneingang E-584
- UND-/ODER-Verknüpfungen G-742
- Und-Verknüpfung
  - Formel Editor F-718
- Unterbrechen
  - Zuschnitt J-1099
- Unteres Eingabefeld
  - Bedingung F-700
- Up
  - Mengen Erzeuger F-710
- Urheberrechte L-1222

### V
- Vektoren E-621
- Eingabehilfe E-523
- in Vorgabezeitformel anwenden E-534
- Vektoren (Vorgabezeitformel) E-522
- Verarbeitungsreihenfolge
  - Voreinstellungen D-365
- Vergleich
  - Stufe I F-661
  - Stufe II F-666
- Verhalten in der Feinplanung
  - Lostyp D-378
- Verlauf der Formelauswertung E-631
- Verlinken J-1090
  - Tischoptimierungen J-1088
- Verlinkte Dokumente L-1239
- Versand H-899
- Vert. Stapel
  - Detail-Ansicht I-986
- Verweildauer siehe Übergangszeiten
- Verwende
  - Bruchscheiben, Dialog Master-Orga D-356
  - Eilscheiben, Dialog Master-Orga D-356
  - Füller, Master-Orga D-355
  - Restblätter, Dialog Master-Orga D-355
- Verwenden
  - Füllauftrag J-1086
  - Restblatt J-1085
- Von/Bis
  - Register Verwendung, Dialog Einstellungen-Abstellplatz D-362
- Vorausgesetzte Kenntnisse A-8, H-857, L-1226
- Voreinstellung
  - Dialog D-365
  - Gruppenbildung D-365
  - Orga D-365
  - Sortierung auf Abstellplatz D-365
  - Verarbeitungsreihenfolge D-365
- Vorgabezeiten E-614
  - Definition E-519
- Vorgabezeiten ändern C-194
- Vorgabezeitformel E-520, E-616
  - Bedingung für Modell E-528
  - Bedingung für Rundbogen E-527
  - Bedingung für Schwellenwert E-528
  - Beispiel E-526
  - Benutzerdefinierte Tabellenelemente E-626
  - Berechnung testen E-538
  - Berechnungsreihenfolge E-524, E-618
  - definieren E-531
- Eigenschaften Formelobjekt E-629
- Eingabehilfe Vektoren E-523, E-622
- Elemente hinzufügen E-620
- Faktoren E-521, E-621
- Feste Elemente E-521
- Formel E-630
- Formel anzeigen E-630
- Formel auswählen E-624
- Formel kopieren E-630
- Formeleditor E-525
- Formelobjekt E-627
- Formelstruktur E-520
- Grenzwert für Tabelle E-626
- löschen E-536
- Syntax kopieren E-542
- Tabelle E-522, E-621
- testen E-537
- Vektor erstellen E-534
- Vektoren E-522, E-621
- Verlauf der Formelauswertung E-631
- Zeitformel testen E-537
- Zeitformelelement erfassen E-624
- Zeitformel-Objekt E-529
- Zeitformeltest E-627
- Zeitzuschläge E-523
- Vorgang suchen C-141
- Vorhandene Bedingungen
  - Auswahl Bedingungen F-695
- Vorhandene Eigenschaften
  - Formel Editor F-719
- Vorhandene Formeln
  - Auswahl Formeln F-716
  - Formel Editor F-719
- Vorhandene Menge
  - Auswahl Mengen F-707
- Vorhandene Zuweisung
  - Auswahl Zuweisung F-720
- Vorschauliste L-1238

### W
- Warenzeichen L-1222
- Weißer Screen C-120
- Werkzeugleiste
  - Bedinungen-Erzeuger F-697
  - Mengen Erzeuger F-710
- Wert
  - Bedingung F-700
  - Erzeuge Zusatz-Sortierung D-371
- Zusatz-Sortierung D-370
- Wert nicht prüfen
  - Erzeuge Zusatz-Sortierung D-371
- Werte I-1027
  - .VAL-Datei I-1027
  - .VAL-Datei laden I-1027
  - Beschreibung der .VAL-Datei I-1029
  - Bezeichnung der .VAL-Datei I-1029
  - Maximalwert der .VAL-Datei I-1029
  - Mindestwert der .VAL-Datei I-1029
  - Nummer des Packmittelparameters I-1028
- Wiederholen
  - Lauf J-1094
  - Zuschnitt J-1102, J-1173
- Wöchentliche Termine (Kampagne) E-600

### X
- XOPT zusammen abstellen
  - Master-Orga D-353
- XOPT-ON Plus
  - Allgemein J-1135
  - Cluster-Ansicht J-1197
  - Import J-1135
  - Optimierung J-1135

### Z
- Zeitformel testen E-537
- Zeitformelelement E-624
- Zeitformel-Objekt E-529
- Zeitformeltest E-537, E-627
- Eigenschaften Formelobjekt E-629
- Formelobjekt E-627
- Ziffer
  - Eingabe Zahlenwert F-705
- Zurücksetzen
  - Status J-1102, J-1173
- Zusätzliche Bedingung G-743
  - auswählen G-822
- Zusatz-Sortierung
  - Register D-370
  - Schlüssel D-370
  - Wert D-370
  - Zusatz-Sortierung D-370
