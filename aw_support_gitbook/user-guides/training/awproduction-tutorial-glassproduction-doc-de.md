---
title: "D-AWProduction-HB_14"
source: "D-AWProduction-HB_14.pdf"
tags: ["A+W Production Terminal", "Tutorial", "Glass Production", "Manufacturing Software", "IG-Assembly", "Terminal IG-In", "Manual Cutting", "Georgian Bars", "Terminal Order", "Software Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive tutorial for the A+W Production Terminal software, a system used in glass manufacturing. It provides step-by-step instructions for various modules, including those for Insulating Glass (IG), Tempered Glass (TG), and Laminated Glass (LG) production, covering workflows from job loading to final processing."
long_description: "This user manual serves as a detailed tutorial for operators and technical staff using the A+W Production Terminal in a glass manufacturing environment. The document is structured into several major sections, each providing an overview and operational guide for a specific software module. These modules include Terminal IG (Insulating Glass), Terminal TG (Tempered Glass), Terminal LG (Laminated Glass), Manual Cutting, Georgian Bars, Order, and Processing. For each module, the tutorial covers its user interface, core functionalities, and standard operating procedures. Key topics include logging in, loading production lots (Lose), producing or processing glass units, handling exceptions like breakages (Bruch) or remakes (Nachläufer), managing machine status (e.g., ready, maintenance, pause), and working with specific unit components like spacers or foils. The manual uses screenshots, tables, and color-coded diagrams to explain complex processes, such as the assembly of IG units or the layout of glass on an oven bed. It aims to help users efficiently manage the production workflow, minimize errors, and correctly document all production steps."
---

---
## Überblick A+W Production Terminal IG

### Bereich D - Farbliche Darstellung der Einheit
In diesem Bereich wird Ihnen die zu produzierende Einheit farblich und in der richtigen Reihenfolge dargestellt. Eine detaillierte Erläuterung diesbezüglich finden Sie unter Terminal IG-Assembly.

### Bereich E - Liste der aktuellen Einheit
Dieser Bereich zeigt Ihnen die Einheit, die als nächstes zur Produktion ansteht.

**Abb. 3 Ausschnitt aktuelle Einheit**

| Typ | Nr | Bock | Auftrag | Pos | Bezeichnung | Breite | Höhe | Dicke | Etikett |
| :-- | :- | :--- | :------ | :-- | :----------------- | :----- | :--- | :---- | :-------- |
| 1 | | | 200084 | 1 | IG 4/16/Th4 A+W | 1200 | 600 | 24 | 001042960 |
| 2 | 2 | 11003 | 200084 | 1 | Float 4 mm A+W | 1200 | 600 | 4 | 001042885 |
| 3 | | 11004 | 200084 | 1 | Therm 4 mm A+W | 1200 | 600 | 4 | 001042935 |

Die obere Reihe der Tabelle (1) zeigt Ihnen die Einheit. Darunter finden Sie die zur Einheit gehörenden Scheiben in genau der Reihenfolge, wie sie zur Produktion auf die Linie gestellt werden müssen. Einheit und Scheibe sind anhand ihrer Symbole zu unterscheiden.

Folgende Symbole sind möglich:

| Symbol | Erläuterung |
| :--- | :--- |
| 🗄️ | Kennzeichnet eine Einheit. |
| 📋 | Kennzeichnet eine Scheibe. |

Bei Scheiben, die mit grüner Farbe oder roter Farbe unterlegt sind, handelt es sich grundsätzlich um sogenannte Nachläufer, d. h. das sind Scheiben, die noch einmal geschnitten werden müssen. Grüne Scheiben sind bereits nachgeschnitten, rote Scheiben müssen noch geschnitten werden.

| Typ | No | Rack | Order | Itm | Description | Width | Height | Thickne | Labe |
| :-- | :- | :--- | :---- | :-: | :----------------- | :---- | :----- | :------ | :--------- |
| 1 | 22 | | 200078 | 2 | IG 4/16/Th4 A+W | 1000 | 1200 | 24 | 001039903 |
| 2 | | 100000 | 200078 | 2 | Float 4 mm A+W | 1000 | 1200 | 4 | 001039873 |
| 3 | | 100000 | 200077 | 2 | Therm 4 mm A+W | 1000 | 1200 | 4 | 001039893 |

**Erläuterung der Tabellenüberschrift**

- **Typ**: Das Symbol kennzeichnet eine Einheit oder eine Scheibe.
- **Nr.**: Zeigt Ihnen die Produktionsnummer innerhalb eines Laufes. Steht in diesem Feld eine 1, wird diese Einheit als Erste produziert.
- **Bock**: In diesem Feld sehen Sie die Nummer des Gestells, auf dem sich die Scheibe befindet. Bei Fächerwagen wird auch die Fachnummer mit angegeben.
- **Auftrag**: Hier wird Ihnen die Auftragsnummer der Einheit angezeigt.
- **Pos.**: Hier wird Ihnen die Positionsnummer der Einheit innerhalb des Auftrags angezeigt.
- **Bezeichnung**: Hier wird Ihnen die Artikelbezeichnung der Einheit bzw. der jeweiligen Scheibe angezeigt.
- **Breite**: Hier wird die Breite der Scheibe angezeigt. Dieses Maß gibt bei Modellscheiben die breiteste Stelle an. Die Breite ist das horizontale (waagerechte) Maß der Scheibe, wenn sie so steht, wie es für die Produktion erforderlich ist. Die angegebene Zahl kann in verschiedenen mm- oder inch-Einheiten angezeigt werden (ToolTV.ini).
- **Höhe**: Hier wird die Höhe der Scheibe angezeigt. Dieses Maß gibt bei Modellscheiben die höchste Stelle an. Die Höhe ist das vertikale (senkrechte) Maß der Scheibe, wenn sie so steht, wie es für die Produktion erforderlich ist. Die angegebene Zahl kann in verschiedenen mm- oder inch-Einheiten angezeigt werden (ToolTV.ini).
- **Dicke**: Hier wird die Dicke der Scheibe angezeigt. Die angegebene Zahl kann in verschiedenen mm- oder inch-Einheiten angezeigt werden (ToolTV.ini).
- **Etikett**: Hier wird Ihnen die Etikettnummer der Einheit oder der Scheibe angezeigt.

### Bereich F - Vorschauliste
In diesem Bereich können Sie sich einen Überblick darüber verschaffen, welche Einheiten als nächstes zur Produktion anstehen.
Da die Felder dieser Liste identisch sind mit den Feldern der Liste (E), werden sie an dieser Stelle nicht noch einmal beschrieben.

### Bereich G - Infofelder
In diesem Bereich erhalten Sie Informationen zu der angemeldeten Person, der Charge sowie dem Status der Maschine.

**Abb. 4 Ausschnitt Info-Bereich**

| Info | | |
| :--- | :--- | :--- |
| **Person [F4]** M. Simek | **Charge [F1]** Charge | **Status [F3]** Bereit |

Im Feld **Person [F4]** sehen Sie den Namen der Person, die zurzeit angemeldet ist.
Im Feld **Charge [F1]** wird Ihnen die Charge angezeigt. Das Feld **Status [F3]** zeigt Ihnen den Maschinenstatus an. Folgende Werte sind möglich:
- Bereit
- Abgemeldet
- Pause
- Wartung
- Rüsten
- Störung

### Bereich H - Schaltflächen
Hier finden Sie die für den weiteren Produktionsprozess notwendigen Schaltflächen:

- **Los laden [F2]**: Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog Los laden. In diesem Dialog können Sie ein Los zur Produktion auswählen.
- **Produzieren [F5]**: Wenn Sie diese Schaltfläche betätigen, wird die Scheibe, die Sie auf die Linie gestellt haben, zur nächsten Station weiter transportiert und in den Status produziert gebucht.
- **Überspringen [F6]**: Diese Schaltfläche müssen Sie betätigen, wenn die angezeigte Scheibe nicht zur Verfügung steht. Dann überspringen Sie die Scheibe und die nächste Scheibe wird angezeigt. Es erfolgt keine Buchung.
- **Bruch [F7]**: Diese Schaltfläche müssen Sie betätigen, wenn die Scheibe, die Sie auf die Linie stellen wollen, eine Beschädigung aufweist. Dann kann sie nicht zur Produktion verwendet werden und wird als Bruch gebucht.
- **Nachläufer [F8]**: Wenn Sie diese Schaltfläche betätigen, können Sie einen Nachläufer laden. Der Dialog Nachläufer laden wird geöffnet.

### Bereich I - Laufnummer/Losnummer
In diesem Bereich wird Ihnen links die Laufnummer und rechts die Losnummer angezeigt. Im Beispiel oben handelt es sich um die Laufnummer 1010 und die Losnummer 1.

### Bereich J - Sprossenansicht
Sollte die Einheit Sprossen enthalten, werden Ihnen diese hier angezeigt.

### Bereich K - Verlinkte Dokumente
Sollte es zu dem Los verlinkte Dokumente geben, werden Ihnen diese hier angezeigt.

### Bereich L - Produktionshinweistexte
In diesem Bereich werden Ihnen mögliche Hinweistexte (z. B. welcher Abstandhalter) für die Produktion angezeigt.

> **Dialog - Erscheinungsbild**
> Die Anzeige der Spalten ist konfigurierbar, daher kann Ihre Bildschirmdarstellung von der oben gezeigten Darstellung abweichen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Los laden" auf Seite 1351
⇨ Softwarereferenz, "Bruch buchen" auf Seite 1353
⇨ Softwarereferenz, "Nachläufer laden" auf Seite 1354

### Ablauf von Arbeitsschritten
Die Vorgehensweise zum Arbeiten in **Terminal IG-In** ist:
- Starten Sie das Modul **Terminal IG-In**.
- Melden Sie sich an (<Name>).
- Laden Sie ein Los.
- Produzieren Sie die Scheibe.

Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies protokollieren. Gründe für eine Unterbrechung können sein:
- Wartung der Maschine.
- Störung der Maschine.
- Pausenzeiten.

Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung aufweisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für Mängel können sein:
- Bruch
- Kratzer
- Falsches Maß
- Riss

#### So melden Sie sich an
1. Starten Sie **Terminal IG-In**.
2. Öffnen Sie im Menü **Datei** den Menüpunkt **Ummelden** oder betätigen Sie die Funktionstaste **[F4]**. Der Dialog **ToolTV Anmeldung** wird geöffnet.
   
   **Person wechseln**
   - **Anwender**: Schmidt
   - **Station**: AUW_IG_IN
   - **[OK [F5]]**
   - **[Abbrechen [F6]]**

3. Tippen Sie in das Feld **Anwender** Ihren Namen (z. B. Schmidt).
4. Betätigen Sie die Schaltfläche **[OK]**.
5. Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Hauptfenster.

> **Namen scannen**
> Arbeiten Sie mit einem Scanner, können Sie direkt im Hauptfenster scannen und brauchen nicht den Dialog ToolTV Anmeldung öffnen.

### Ein Los laden
Wenn Sie das Modul starten, ist der Dialog leer. Um mit Ihrer Arbeit beginnen zu können, müssen Sie zunächst ein Los laden.

#### So laden Sie ein Los
1. Betätigen Sie die Schaltfläche **[Los laden]**.
2. Der Dialog **Los laden** wird geöffnet.
   
   **Dialog: Los laden**
   - Filter Lauf / Los: 1008
   - Linke Liste: Lauf 1, Los 1008, Stk 17, Text Test Awrack
   - Rechte Liste: Teile (z.B. 100000 Float 4 mm A+W)
   - Buttons: [Alle anzeigen], [Lauf entfernen], [Aktualisieren [F2]], [Laden [F5]], [Abbrechen [F6]]

3. **Terminal IG-In** merkt sich den zuletzt bearbeiteten Lauf. Um alle Läufe sehen zu können, müssen Sie deshalb den Filter löschen. Betätigen Sie die Schaltfläche **[Alle anzeigen]**.
4. Wählen Sie aus der linken Liste den Lauf, den Sie als nächstes fertigen möchten. Wenn Sie den Lauf markiert haben, sehen Sie in der rechten Liste den Inhalt.
5. Betätigen Sie die Schaltfläche **[Laden]**.
6. Der Dialog wird geschlossen und das gewählte Los wird geladen. Sie befinden sich jetzt wieder im Hauptfenster.

#### So produzieren Sie eine Scheibe
1. Stellen Sie die Scheibe vom Gestell auf die Linie und betätigen Sie die Schaltfläche **[Produzieren]**.
2. Die Scheibe wird zur nächsten Station weiter transportiert.

### Den Zustand der Maschine ändern
Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit unterbrochen werden muss. Eine solche Unterbrechung muss immer protokolliert werden.
Gründe für eine Unterbrechung können sein:
- Wartung der Maschine
- Störung der Maschine
- Pausenzeiten
- Rüstzeiten

> **Automatisches Abmelden**
> Die A+W Production Terminal Stationen können so konfiguriert werden, dass sie sich nach einer gewissen Zeit der Inaktivität automatisch abmelden.

#### So ändern Sie den Maschinenstatus
1. Wählen Sie im Menü **Maschine > Maschinenstatus**. Oder betätigen Sie die Schaltfläche **[F3]**.
2. Es öffnet sich der Dialog **Status**.
   
   **Dialog: Status**
   - Liste der Status: 1 501 Bereit, 2 502 Abgemeldet, 3 503 Pause, 4 504 Wartung, 5 505 Rüsten, 6 506 Störung
   - Buttons: [OK [F5]], [Abbrechen [F6]]

3. Wählen Sie aus der Liste den Grund aus.
4. Betätigen Sie die Schaltfläche **[OK]**.
5. Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Hauptfenster. Im Bereich **Status** wird der gewählte Status angezeigt.

> **Status auf Bereit setzen**
> Vergessen Sie nicht, nach der Arbeitsunterbrechung die Maschine wieder in den Zustand Bereit zu setzen! Sonst können Sie nicht weiterarbeiten.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Status" auf Seite 1356

### Umgang mit beschädigten Scheiben
Unter Umständen kann es vorkommen, dass Sie die vom Modul vorgeschlagene Scheibe nicht fertigen können, da sie einen Mangel aufweist. Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen. Gründe für Mängel können sein:
- Bruch
- Mangel (Qualitätssicherungsgrund)
- Kratzer
- Falsches Maß
- Falsche Glasart
- Risse

Für Bruch, Kratzer und Risse werden Nachläufer automatisch erstellt. D. h., wenn irgendwo in der Produktion ein Bruch entsteht und dieser gescannt wird, kommen die entsprechenden Scheiben automatisch in einen sogenannten Bruchpool und werden so schnell wie möglich nachgeschnitten. Bei den Fällen Falsches Maß und Falsche Glasart ist jedoch ein erneutes Schneiden nicht erwünscht. Deshalb werden bei diesen beiden Bruchgründen keine Nachläufer erzeugt.
Bei einem Mangel hat der Vorgesetzte zu entscheiden, ob dieser bleiben bzw. entfernt werden kann oder nicht. Beispiel: Es befindet sich ein Kratzer auf der Scheibe, der aber weg poliert werden kann. Aufgrund dieser Markierung können Sie Reports erstellen, die Ihnen zur Qualitätsauswertung dienen.

#### So verfahren Sie mit beschädigten Scheiben
1. Markieren Sie die entsprechende Scheibe.
2. Betätigen Sie die Schaltfläche **[Bruch]**.
3. Der Dialog **Zustand** wird geöffnet.
   
   **Dialog: Zustand**
   - Liste der Zustände: 1 11 Bruch (Bruchscheiben), 2 22 Mangel (Mangel), 3 50 Kratzer (Bruchscheiben), 4 51 Maß falsch (Bruch ohne NL), 5 52 Falsche Glasart (Bruch ohne NL), 6 250 MA-Kratzer (Mangel)
   - Buttons: [OK [F5]], [Abbrechen [F6]]

4. Wählen Sie aus der Liste den entsprechenden Grund aus.
5. Betätigen Sie die Schaltfläche **[OK]**.
6. Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Hauptfenster.

> **Automatische Nachläufer**
> Für einige Bruchtypen werden Nachläufer automatisch generiert. Dies wird bei der Konfiguration entsprechend eingestellt. Der Mitarbeiter an der Maschine muss mit diesen Modalitäten vertraut sein.

### Eine andere Produktionsnummer laden
Es kann vorkommen, dass Sie die von **Terminal IG-In** vorgeschlagene Produktionsnummer nicht fertigen können oder aber eine andere Produktionsnummer der Aktuellen vorziehen sollen. Um in der Vorschauliste nicht umständlich nach unten scrollen zu müssen, können Sie die gewünschte Produktionsnummer direkt laden.

#### So laden Sie eine Produktionsnummer
1. Wählen Sie im Menü **Datei > Springe zu ProdNr**.
2. Der Dialog **Gehe zu Produktionsnummer** wird geöffnet.
   
   **Dialog: Gehe zu Produktionsnummer**
   - **Neue Produktionsnummer**: 22
   - Buttons: [OK [F5]], [X Abbrechen [F6]]

3. Wählen Sie im Feld **Neue Produktionsnummer** über die Pfeiltasten die gewünschte Produktionsnummer aus.
4. Betätigen Sie die Schaltfläche **[OK]**.
5. Der Dialog wird geschlossen und die gewählte Produktionsnummer wird geladen. Sie befinden sich jetzt wieder im Hauptfenster.

### Einen Nachläufer laden
Befinden sich für die aktuell zu fertigende Produktionsnummer noch Nachläufer in der Produktion, können diese über den Dialog **Nachläufer einfügen** geladen oder gescannt werden.

#### So laden Sie Nachläufer
1. Betätigen Sie die Schaltfläche **[Nachläufer]**.
2. Es öffnet sich der Dialog **Einfügen**.
   
   **Dialog: Einfügen**
   - **Barcode**: 001042408
   - **Auftrag**: 1700045, **Pos**: 9, **Etikett**: 001042408
   - Buttons: [Übernehmen [F2]], [Laden [F5]], [Abbrechen [F6]]

3. Geben Sie im Feld **Barcode** die entsprechende Etikettnummer der ISO-Einheit manuell oder scannen Sie diese.
4. Betätigen Sie die Schaltfläche **[Übernehmen]**.
5. Die zugehörigen Daten werden im Feld darunter angezeigt.
6. Betätigen Sie die Schaltfläche **[Laden]**.
7. Der Dialog wird geschlossen und der Nachläufer wird geladen. Sie befinden sich jetzt wieder im Hauptfenster.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Nachläufer laden" auf Seite 1354

### Weitere Funktionen
Zu den weiteren Funktionen zählen:
- Listen (Reports)
- Log-Einträge
- Unterschiedliche Programm-Sprachen

#### Listen (Reports) generieren
Die Listen (Reports) sind im gleichnamigen Menü zu finden. Sie werden von A+W für jeden Kunden individuell erstellt und den jeweiligen Anforderungen angepasst. Wir zeigen Ihnen im Anschluss den Report einer Auftragsübersicht.

**So drucken Sie eine Auftragsübersicht**
1. Wählen Sie im Menü **Listen > Auftragsübersicht**.
2. Der Dialog **Parametereingabe für Report** wird geöffnet.
3. Geben Sie im Bereich **Geben Sie einen Wert ein** die gewünschte Auftragsnummer an.
4. Betätigen Sie die Schaltfläche **[OK]**.
5. Der Dialog wird geschlossen und der Report wird angezeigt:

**Auftrag Übersicht für 700025**
Gesamt: 3 Stück, davon 3 Endprodukte

| Pos | Barcode | Glasart | Breite | Höhe | Kg | m² | ES | Gestell | Letzte Buchung |
| :-- | :------ | :-------------------- | :--------- | :--- | :---- | :--- | :- | :------ | :--------------- |
| 1 | 001044065 (1 Stück) | A+W Float 6 mm (1 Endprodukte) | 2500 * 2500 | | 93,75 | 6,25 | | | 21.09.09 11:57 |
| 2 | 001044066 (1 Stück) | A+W Float 6 mm (1 Endprodukte) | 1000 * 1300 | | 19,50 | 1,30 | | | 21.09.09 11:57 |
| 3 | 001044067 (1 Stück) | A+W Float 6 mm (1 Endprodukte) | 1000 * 1300 | | 19,50 | 1,30 | | | 21.09.09 11:57 |

#### Log-Einträge exportieren
Sie können die Logeinträge in Form einer Text-Datei exportieren. Im Falle eines Fehlers kann es von Vorteil sein, diese Text-Datei zu Analysezwecken zu A+W zu schicken.

**So exportieren Sie Log-Einträge**
1. Wählen Sie im Menü **? > Aktuelle Log-Einträge**.
2. Der Dialog **Log-Einträge für diese Sitzung** wird geöffnet.
3. Betätigen Sie die Schaltfläche **[Exportieren]**.
4. Es öffnet sich der Dialog **Speichern unter ...**.
5. Vergeben Sie einen Namen für die Datei und wählen Sie den entsprechenden Speicherort aus.
6. Betätigen Sie die Schaltfläche **[Speichern]**.
7. Der Dialog wird geschlossen und die Datei ist gespeichert.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Logeinträge für Sitzung" auf Seite 1386

#### Programmsprache wählen
Das Modul kann in verschiedenen Sprachen betrieben werden. Die Sprache kann während der Laufzeit umgestellt werden. Ein Neustart ist nicht erforderlich.

**So wählen Sie eine andere Sprache aus**
1. Wählen Sie im Menü **? > Sprache ändern**.
2. Der Dialog **Sprache ändern** wird geöffnet.
3. Wählen Sie aus der Kombobox **Sprache** die gewünschte Sprache aus.
4. Schließen Sie den Dialog über die Schaltfläche **[OK]**. Das Modul präsentiert sich in der gewünschten Sprache.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Sprachauswahl" auf Seite 1387

### Arbeiten mit Terminal IG-Assembly

**Lernziele**
- Oberfläche von Terminal IG-Assembly kennenlernen.
- Die Funktionsweise kennenlernen und verstehen.
- Arbeitsunterbrechungen korrekt durchführen.
- Mit unvorhersehbaren Situation (z. B. fehlendes Material) umgehen lernen.
- Chargen definieren.

**Nutzen**
Terminal IG-Assembly unterstützt Sie an dieser Stelle erheblich bei Ihrer Arbeit. Es zeigt Ihnen optisch den Scheibenaufbau sowie das zu verwendende Gas und den entsprechenden Rahmen. Alle relevanten Informationen sind auf einen Blick ersichtlich und müssen nicht nachgeschlagen (Papier) werden.

**Definitionen**
- **Produktionshinweistexte**: Werden Ihnen in einem eigenen Bereich angezeigt.
- **Rahmen**: Abstandhalter, der sich zwischen den einzelnen Glasscheiben befindet.
- **Gas**: Der Scheibenzwischenraum wird mit Gas gefüllt.

**Merke**
- **Aktualisieren**: Über diese Schaltfläche aktualisieren Sie die Anzeige.
- **Farbliche Darstellung der Einheit**: Lässt Sie den Aufbau der Einheit auf einen Blick erkennen.

### Modul-Präsentation Terminal IG-Assembly
Terminal IG-Assembly befindet sich im Anschluss von Terminal IG-In. Es wird zwischen der optischer Scheibenkontrolle nach der Waschmaschine und vor der Rahmensetzstation installiert und visualisiert die technischen Daten inklusive der Rahmendaten jeder zu fertigenden Einheit. Diese ist die letzte und sinnvolle Station, an der Sie ISO-Unterteile als Bruch buchen können.

Nachdem Sie Terminal IG-Assembly gestartet haben, präsentiert sich das Modul wie folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn Sie das Modul starten, ist das Hauptfenster leer:

**Abb. 5 Terminal IG-Assembly**

*   **A**: Menüleiste
*   **B**: Produktionsnummer und Bezeichnung
*   **C**: Modellanzeige
*   **D**: Farbliche Darstellung der Einheit
*   **E**: Liste der aktuellen Einheit
*   **F**: Vorschauliste
*   **G**: Infofelder
*   **H**: Meldungsfenster und Schaltflächen
*   **I**: Laufnummer/Losnummer
*   **J**: Sprossenansicht
*   **K**: Verlinkte Dokumente
*   **L**: Produktionshinweistexte

Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Darunter finden Sie die aktuelle Produktionsnummer sowie die Bezeichnung (B). Im Bereich (C) wird Ihnen das Modell und die umschreibenden Maße der Scheibe angezeigt. In (D) finden Sie die farbliche Darstellung der zu produzierenden Einheit. Der Bereich (E) zeigt Ihnen die Liste der aktuellen Einheit. Der Bereich (F) liefert Ihnen eine Vorschau auf die nächste Einheit und im Bereich (G) befinden sich die Infofelder. Unter (H) befinden sich alle für den weiteren Produktionsprozess nötigen Schaltflächen. Der Bereich (I) zeigt Ihnen die Laufnummer und die Losnummer. Im Bereich (J) werden Ihnen vorhandene Sprossen angezeigt. Sollte es zu dem Lauf verlinkte Dokumente geben, werden Ihnen diese im Bereich (K) angezeigt. Der Bereich (L) enthält mögliche Produktionshinweistexte.

> **Anzeige der Spalten ist frei konfigurierbar**
> Die Anzeige der Spalten ist frei konfigurierbar. Daher kann die gezeigte Bildschirmdarstellung von Ihrer Darstellung abweichen.

### Detaillierte Erläuterung zu den einzelnen Bereichen
Außer dem Bereich (D) sind alle Bereiche von Terminal IG-Assembly identisch mit den Bereichen von Terminal IG-In und werden deshalb an dieser Stelle nicht noch einmal beschrieben.
⇨ Tutorial, "Detaillierte Erläuterung zu den einzelnen Bereichen" auf Seite 1236

#### Bereich D - Farbliche Darstellung der Einheit
In diesem Bereich wird Ihnen die zu produzierende Einheit farblich und in der richtigen Reihenfolge dargestellt. Im Anschluss folgt eine detaillierte Erläuterung zur Darstellung der Einheit:

*   **A**: Außenseite (Sonne)
*   **B**: Äußere Scheibe
*   **C**: Scheibenzwischenraum
*   **D**: Beschichtung
*   **E**: Innere Scheibe

**Tab. 1 Symbole und ihre Bedeutung**
Für Scheiben gibt es folgende Darstellungen:

| Symbol | Erläuterung |
| :--- | :--- |
| 