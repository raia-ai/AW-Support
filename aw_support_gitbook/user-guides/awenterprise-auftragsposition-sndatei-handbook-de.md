---
description: "DE-HB-AWEnterprise_16"
---


# A+W Enterprise Verkauf

---
## Auftragsposition

### Bearbeitung aus SN-Datei übernehmen (VK 03-006)

**Ziel der Handlung**
*   Bearbeitungen aus SN-Datei in Stückliste übernehmen.

**Voraussetzungen**
*   A+W CAD Designer (Shapes) ist installiert.
*   SN-Austauschregeln sind definiert: Menü Stammdaten > Schlüssel > Produkte > SN-Austauschregeln.
*   SN-Dateien sind verfügbar.
*   Pfad ist eingerichtet.

**Zusatzinfo**
*   Wenn keine Datei angehängt und gespeichert wird, kann der Stücklistenaufbau nur geändert werden, wenn die gesamte Handlungssequenz wiederholt wird.
    *   ⇨SN-Datei anhängen
    *   ⇨ Änderungen mit SN-Datei abgleichen

**Workflow**
1.  Menü Verkauf > Auftragserfassung > Position erfassen.
2.  Menge, Breite und Höhe eingeben.
3.  Feld Höhe: <Strg>+<E> drücken.
    Windows-Explorer wird im vordefinierten Pfad geöffnet.
4.  SN-Datei im Windows-Explorer markieren und mit [Öff-nen] bestätigen.
5.  Abfrage zur Synchronisierung der Stückliste mit [Ja] be-stätigen.
    Programm A+W CAD Designer (Shapes) wird geöffnet.
6.  In CAD Designer: Bearbeitungen prüfen und ggf. än-dern.
7.  Menü Datei: TOE Beenden wählen.
    Programm A+W CAD Designer (Shapes) wird beendet. Die AWE-Stückliste wird mit der CAD-Datei abgeglichen. Die Bearbeitungen werden übernommen. Die SN-Datei wird nicht angehängt.
8.  Mit <Tab> ins nächste Feld springen.
    Der Dialog Bearbeitungen zu Position wird angezeigt.
9.  Bearbeitungen prüfen und Dialog mit [OK] schließen.
10. Position speichern.
11. Erfassung fortsetzen oder Auftrag speichern und been-den.

### SN-Datei anhängen (VK 03-007)

**Ziel der Handlung**
*   Bearbeitungen aus SN-Datei in Stückliste übernehmen.
*   Kopie von SN-Datei anhängen.

**Voraussetzungen**
*   A+W CAD Designer (Shapes) ist installiert.
*   SN-Austauschregeln sind definiert: Menü Stammdaten > Schlüssel > Produkte > SN-Austauschregeln.
*   SN-Dateien sind verfügbar.
*   Pfad ist eingerichtet.

**Zusatzinfo**
*   Wenn in A+W Enterprise keine SN-Austauschregel für die in der SN-Datei erfasste Bearbeitung hinterlegt ist, wird ein Auswahldialog für die Zuordnung angezeigt. Diese Zuordnung gilt jeweils nur für die aktuelle Position.
*   ⇨ Änderungen mit SN-Datei abgleichen

**Workflow**
1.  Menü Verkauf > Auftragserfassung > Position erfassen.
2.  Menge, Breite und Höhe eingeben.
3.  Feld Höhe: <Strg>+<E> drücken. Windows-Explorer wird im vordefinierten Pfad geöffnet.
4.  SN-Datei im Windows-Explorer markieren und mit [Öffnen] bestätigen.
5.  Abfrage zur Synchronisierung der Stückliste mit [Ja] bestätigen. Programm A+W CAD Designer (Shapes) wird geöffnet.
6.  In CAD Designer: Bearbeitungen prüfen und ggf. ändern.
7.  Menü Datei: TOE Beenden und Datei speichern wählen. Programm A+W CAD Designer (Shapes) wird beendet. Die Bearbeitungen werden in die Stückliste der Position übernommen. Die SN-Datei wird aktualisiert.
8.  Abfragen bestätigen und Hinweise prüfen.
9.  Mit <Tab> ins nächste Feld springen. Der Dialog Bearbeitungen zu Position wird angezeigt.
10. Bearbeitungen prüfen und Dialog mit [OK] schließen.
11. Register Eingenschaften: Pfad und Name der angehängten SN-Datei prüfen. SN-Datei wird als Kopie im TOE-Verzeichnis gespeichert.
12. Position speichern.
13. Erfassung fortsetzen oder Auftrag speichern und beenden.

### Änderungen mit SN-Datei abgleichen (VK 03-008)

**Ziel der Handlung**
*   Bearbeitungen in angehängter SN-Datei ändern oder ergänzen.
*   Bearbeitungen in Stückliste ändern oder ergänzen.

**Voraussetzungen**
*   A+W CAD Designer (Shapes) ist installiert.
*   SN-Austauschregeln sind definiert: Menü Stammdaten > Schlüssel > Produkte > SN-Austauschregeln.
*   SN-Dateien sind verfügbar.
*   Pfad ist eingerichtet.
*   Arbeiten mit A+W CAD Designer (Shapes) ist bekannt.

**Zusatzinfo**
*   Vollständige Beschreibung im Handbuch A+W CAD Designer (Shapes).

**Workflow**

**Bearbeitungen in A+W CAD Designer (Shapes) ändern:**
1.  Menü Verkauf > Auftragserfassung > Position mit SN-Datei auswählen.
2.  Feld Breite: <Strg>+<E> drücken. Programm A+W CAD Designer (Shapes) wird geöffnet.
3.  In CAD Designer: Bearbeitungen ändern, z. B. Kanten-bearbeitung.
4.  Menü Datei: TOE Beenden und Datei speichern wählen. Programm A+W CAD Designer (Shapes) wird beendet. Die Bearbeitungen werden in die Stückliste der Position übernommen. Die SN-Datei wird angehängt.

**Bearbeitungen in der Stückliste ändern:**
5.  Position markieren: [Stückliste] wählen. Dialog Stücklistendarstellung wird angezeigt. A+W CAD Designer (Shapes) wird geöffnet.
6.  Bearbeitungen ändern oder hinzufügen, z. B. Durch-sprechöffnung.
    ⇨ Siehe Help Card: Bearbeitung erfassen
7.  Änderungen speichern und Dialog schließen. Die Bearbeitungen werden in die Stückliste der Position übernommen. Die SN-Datei wird aktualisiert.
8.  Position speichern.
9.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### Position in CAD erfassen (VK 03-009)

**Ziel der Handlung**
*   Geometrie und Bearbeitungen in A+W CAD Designer (Shapes) erfassen, in Position übernehmen und als SN-Datei speichern.
*   Interaktive Erfassung in A+W CAD Designer (Shapes).

**Voraussetzungen**
*   A+W CAD Designer (Shapes) ist installiert.
*   SN-Austauschregeln sind definiert: Menü Stammdaten > Schlüssel > Produkte > SN-Austauschregeln.
*   Pfad ist eingerichtet.
*   Arbeiten mit A+W CAD Designer (Shapes) ist bekannt.

**Zusatzinfo**
*   Vollständige Beschreibung im Handbuch A+W CAD Designer (Shapes).

**Workflow**
1.  Menü Verkauf > Auftragserfassung > Position mit Artikel-nummer und Menge erfassen.
2.  Feld Breite: <Strg>+<F> drücken. A+W CAD Designer (Shapes) wird geöffnet.
3.  CAD-Konstruktion der Scheibe mit Maßen und notwendigen Bearbeitungen zeichnen.
4.  Menü Datei: TOE Beenden und Datei speichern wählen. Programm A+W CAD Designer (Shapes) wird beendet. Die Stückliste wird in der Position erzeugt. SN-Datei wird im TOE-Verzeichnis gespeichert und angehängt. Änderungen sind möglich: siehe VK 03-008.
5.  Position speichern.
6.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### Stufenglas erfassen (VK 03-010)

**Ziel der Handlung**
*   Stufung in Mehrfach-Scheibe erfassen.

**Voraussetzungen**
*   Auftragserfassung ist geöffnet.
*   Artikel vom Typ Stufe ist in den Stammdaten angelegt.
*   Bei Stufe in Modell: Modell ist erfasst.

**Zusatzinfo**
*   Positive Werte für die Stufen werden von der Kantenlänge abgezogen, negative Werte hinzugerechnet.
*   Bei Stufen im VSG steht in der Produktskizze eine seitliche Ansicht zur Verfügung.

**Workflow**
1.  Register Positionen > Allgemein > Position erfassen. Beispiel: Stufung in ISO-Scheibe angeben.
2.  ISO-Artikel erfassen.
3.  Feld Breite: <Strg>+<F10> drücken. Dialog Stufenerfassung (relevante Teile) wird geöffnet.
4.  Glas für Stufe auswählen: in Feld S Stufung mit J zuweisen und <F3> und [OK] drücken. Dialog Modell-Maßangaben wird geöffnet
5.  Maße für Höhe und Breite eingeben.
6.  Maße für die Stufen pro Kante eingeben
7.  Maßangaben mit <Enter> übernehmen.
8.  Bei Mehrfach-ISO: Schritte 4 bis 7 für nächstes Glas wiederholen.
9.  Werte aus Dialog Stufenerfassung (relevante Teile) übernehmen.
10. Feld Bestellung: Stücklistendarstellung mit [Stückliste] öffnen. Dialog Stücklistendarstellung wird geöffnet.
11. Zum Register Produktionsskizze wechseln und Eingaben prüfen.
12. Ggf. Abstandhalter und weitere Details erfassen und speichern.
13. Erfassung fortsetzen oder Auftrag speichern und beenden.

### Sprossen erfassen (VK 03-011)

**Ziel der Handlung**
*   Sprossenaufbau erfassen.

**Voraussetzungen**
*   Sprossenartikel sind angelegt.
*   Auftragserfassung ist geöffnet.

**Zusatzinfo**
*   Für komplexen Sprossenaufbau Skizze aus A+W Design (Bars) anhängen.
*   ⇨ Rechnung
*   ⇨ Sprossenaufbau bearbeiten

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln.
2.  Position mit ISO-Scheibe vollständig erfassen.
3.  Feld SZR: Abstandhalter prüfen und ggf. ändern.
4.  Feld SZR: <Shift>+<F8> drücken. Dialog Sprossenerfassung wird geöffnet.
5.  Register Sprossen:
    *   Feld Sprosse: Artikelnummer für Sprosse eingeben oder auswählen.
    *   Felder wa und se: Anzahl der waagerechten und senkrechten Sprossen eingeben.
    *   Feld Symmetrie: F-Sym oder B-Sym wählen.
    *   Feld Farbe: ggf. Farbvarianten auswählen.
    *   Feld Lieferant: ggf. Lieferant auswählen.
6.  Register Zusatzinfo: ggf. Beschaffungsart ändern.
7.  Bei Mehrfach-ISO:
    *   Feld IR: Rahmen für Einbau auswählen.
    *   Angaben für den nächsten SZR (Rahmen) wiederholen.
8.  Daten mit [OK] übernehmen. Die Position wird mit dem Sprossen-Icon gekennzeichnet. Das Sprossengitter wird im Grafikbereich maßstabsgerecht angezeigt.
9.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### Sprossenaufbau bearbeiten (VK 03-012)

**Ziel der Handlung**
*   Sprossenaufbau mit dem Sprosseneditor bearbeiten.
*   Nicht symmetrischen Sprossenaufbau erfassen.

**Voraussetzungen**
*   Auftragserfassung ist geöffnet.
*   Help Card „Sprossen erfassen" ist bekannt.

**Zusatzinfo**
*   Max. 11 Sprossen werden an die Produktion übergeben.
*   Die Preise werden für max. 2 verschieden Sprossenartikel berechnet.
*   Komplexe Sprossenaufbauten, z. B. Sonnen, als Skizze aus A+W Design (Bars) anhängen.
*   ⇨ Rechnung
*   ⇨ Sprossen erfassen

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln.
2.  Position mit ISO-Scheibe vollständig erfassen.
3.  Feld SZR: <Shift>+<F8> drücken. Dialog Sprossenerfassung wird geöffnet.
4.  Anzahl der waagerechten und senkrechten Sprossen angeben.
5.  Feld Symmetrie: F-Sym+E oder B-Sym+E wählen.
6.  Sprosseneditor öffnen: [Editor].
7.  Wegfallsprosse entfernen: im Sprossenbild auf die Sprosse klicken.
8.  Änderungen verwerfen: mit [Neuaufbau] ursprünglichen Sprossenaufbau wiederherstellen.
9.  Änderungen mit [OK] übernehmen.

**Sprossenposition ändern:**
10. Lichte Felder bearbeiten: <Shift>+<F8> drücken und Wert eingeben.
11. Bohrpunkte bearbeiten:
    *   <Shift>+<F12> drücken und Wert eingeben.
    *   Tabelle öffnen: <Shift>+<F11> drücken und Werte bearbeiten.
    *   Änderungen mit <Enter> übernehmen.
12. Sprossenaufbau mit [OK] übernehmen. Sprosseneditor wird geschlossen. Die Position wird mit dem Sprossen-Icon gekennzeichnet. Der Sprossenaufbau wird im Grafikbereich angezeigt.
13. Erfassung fortsetzen oder Auftrag speichern und beenden.

### Einstand und Versiegelungstiefe (VK 03-013)

**Ziel der Handlung**
*   Einstand und Versiegelungstiefe in ISO-Scheiben erfassen.

**Voraussetzungen**
*   Das Modul ist im System konfiguriert.

**Zusatzinfo**
*   Maße für Einstand und für Versiegelungstiefe weichen in der Regel nur 1-2 mm voneinander ab.

**Workflow**
1.  Register Positionen > Allgemein > Position erfassen.
2.  Feld Preis: <F3> drücken. Dialog Maße der einzelnen Stücklistenteile wird geöffnet.
3.  Stückliste: Ebene Innenrahmen markieren und [Einstand] wählen. Dialog Einstand (Rahmenstärke) wird geöffnet.
4.  Maße an allen Kanten eintragen.
5.  Stückliste: Ebene Thiokol markieren und [Versiegelung] wählen. Dialog Versiegelungstiefe wird geöffnet.
6.  Maße an allen Kanten eintragen.
7.  Angaben mit <Enter> übernehmen.
8.  Abfragen zur Preisberechnung bestätigen.
9.  Änderung mit <Ende> speichern. Dialog Maße der einzelnen Stücklistenteile wird geschlossen. Die Position wird mit dem aktualisierten Preis angezeigt.
10. Erfassung fortsetzen oder Auftrag speichern und beenden.

### Randentschichtung erfassen (VK 03-018)

**Ziel der Handlung**
*   Randentschichtung erfassen.

**Voraussetzungen**
*   Das Modul ist im System konfiguriert.
*   Erfassung von Randentschichtung setzt voraus, dass in den Stammdaten Meta-Artikel gepflegt sind, d. h. eine Bearbeitung mit der Stückliste. Diese Meta-Artikel müssen im Auftrag erfasst werden.

**Zusatzinfo**
*   Die Randentschichtung kann nicht über die A+W-Bearbeitungstypen erfasst werden.
*   Das Gleiche gilt auch für die Bearbeitungen Abkleben, Emailestreifen, UV-Schutz u.a.

**Workflow**
1.  Register Positionen > Allgemein > Position erfassen.
2.  Feld Höhe: <F5> drücken. Dialog Stücklistendarstellung wird geöffnet.
3.  Stückliste: <F6> drücken und Meta-Artikel für Randentschichtung auswählen. Artikel wird im Register Akt. Stücklistenebene eingefügt.
4.  Artikel markieren: <F5> drücken. Dialog Tiefe des Randentschichtens wird geöffnet.
5.  Maße für die Tiefe der Entschichtung eingeben und mit [OK] speichern.
6.  Artikel und Maße mit [OK] speichern. Dialog Bearbeitungen zu Position x wird geöffnet. Die Stückliste ist den Stammdaten entsprechend vervollständigt.
7.  Angaben prüfen und ggf. Kommentare eingeben.
8.  Angaben mit [OK] speichern. Dialog Bearbeitungen zu Position x wird geschlossen. Die Bearbeitungen werden im Register Positionen angezeigt.
9.  Ggf. Abfragen zur Preisberechnung bestätigen.
10. Änderung mit <Ende> speichern. Die Position wird mit dem aktualisierten Preis angezeigt.
11. Erfassung fortsetzen oder Auftrag speichern und beenden.

### Produkt austauschen (VK 03-014)

**Ziel der Handlung**
*   Artikel in mehreren Auftragspositionen austauschen.
*   Scheibenaufbau in mehreren Auftragspositionen bearbeiten.

**Voraussetzungen**
*   Auftragserfassung ist geöffnet.
*   Mehrere Positionen mit identischer Stückliste sind erfasst.

**Zusatzinfo**
*   Bei einem Produktaustausch müssen die Bearbeitungen zur Scheibe neu erfasst werden.
*   Produktaustausch für mehrere Positionen betrifft nur Positionen mit derselben Stücklistennummer.

**Workflow**
1.  Register Positionen > Allgemein: <F4> > Produktangaben > Produktaustausch wählen. Dialog Produktaustausch wird angezeigt.
2.  Feld Typ: Stücklistennummer aus der Positionsspalte SLNr angeben.
3.  Austauschartikel angeben.
4.  Austausch mit [Start] bestätigen.
5.  Abfragen bestätigen. Die Positionen werden mit der neuen Artikelnummer und mit einer neuen Stücklistennummer angezeigt.

**Scheibenaufbau bearbeiten:**
6.  Schritt 2: Feld Austauschartikel: alte Artikelnummer angeben.
7.  Felder Wunschaufbau: einen oder mehrere Artikel ändern.
8.  Austausch mit [Start] bestätigen.
9.  Abfragen bestätigen bis Abfrage, ob Austausch für alle Positionen gelten soll.
10. Abfrage Gilt der Produktaustausch für alle Positionen... mit [Nein] bestätigen. Dialog Produktaustausch für Positionen wird angezeigt.
11. Feld Neu: alle Positionen mit N abwählen, in denen das Produkt nicht getauscht werden soll.
12. Austausch mit [Start] bestätigen. Der Dialog wird geschlossen. Die Positionen werden mit der alten Artikelnummer und mit einer neuen Stücklistennummer angezeigt.

### Artikel fixieren (VK 03-015)

**Ziel der Handlung**
*   Artikel einer Auftragsposition fixieren.
*   Fixierten Artikel in die Stammdaten übernehmen.

**Voraussetzungen**
*   Auftragserfassung ist geöffnet.
*   Auftrag und Position ist erfasst.

**Zusatzinfo**
*   Das Mitarbeiterrecht zum Zurückschreiben einer fixierten Position in die Artikelstammdaten muss erteilt sein.
*   In die Stammdaten zurückgeschriebene fixierte Artikel können den Angaben entsprechend allgemein oder kundenindividuell als Position erfasst werden.

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln.
2.  Position vollständig erfassen.
3.  Feld Preis: <Shift>+<F8> drücken.
4.  Abfrage mit [Ja] bestätigen. Die Position wird mit einem gelben Stern gekennzeichnet.
5.  Nach Bedarf weitere Positionen erfassen oder zur Fixierung markieren.

**Fixierten Artikel in die Stammdaten übernehmen:**
6.  Auftrag mit <Ende> speichern und Abfrage bestätigen. Dialog Artikelangaben für bemaßte Varianten wird für die erste fixierte Position angezeigt.
7.  Feld Artikel (neu): neue Artikelnummer eingeben.
8.  Vorbelegte Felder prüfen und ggf. abweichende Informationen eingeben, z. B.:
    *   Kunden angeben, wenn der neue Artikel ein kundenindividuelles Produkt ist.
    *   Kundenindividuelle Artikelnummer und -bezeichnung angeben.
    *   Preise angeben.
9.  Angaben mit <Ende> speichern. Die Position wird mit einem grünen Stern gekennzeichnet.
10. Ggf. Schritte 7 bis 8 für jede fixierte Position wiederholen.
11. Änderungen speichern. Der Artikel wird unter der eingegebenen Nummer im Artikelstamm gespeichert.

### Leistungserklärung zuordnen (VK 03-016)

**Ziel der Handlung**
*   Leistungserklärung prüfen und/oder zuordnen.

**Voraussetzungen**
*   ISO-Position ist vollständig erfasst.

**Zusatzinfo**
*   Alle Kopfdaten der Leistungserklärung (LE) werden auf dem Dokument gedruckt.
*   Leistungserklärung nach Produktaufbau erstellen:
    *   ⇨Technische Werte erfassen

**Workflow**

**Leistungserklärung (LE) aus Stammdaten übernehmen:**
1.  Menü Verkauf > Vorgang öffnen > Position markieren.
2.  Register Eigenschaften > Feld LE-Nummer. <Strg>+<R> drücken. Kennung der LE wird im Feld LE-Nummer angezeigt.

**Zugeordnete LE ändern:**
3.  Register Eigenschaften > Feld LE-Nummer: <Strg>+<K> drücken. Dialog Leistungserklärung wird angezeigt.
4.  Dokument suchen und auswählen.
5.  Zuordnung mit [OK] bestätigen.
6.  Daten mit <End> übernehmen. Kennung der neuen LE wird im Feld LE-Nummer angezeigt.
7.  Auftrag speichern.

### Technische Werte erfassen (VK 03-017)

**Ziel der Handlung**
*   Technische Werte erfassen.
*   Neue Leistungserklärung generieren.

**Voraussetzungen**
*   ISO-Position ist vollständig erfasst.

**Zusatzinfo**
*   Alle Kopfdaten der Leistungserklärung (LE) werden auf dem Dokument gedruckt.
*   Mindestens eine Checkbox der Leistungen muss zur Ausgabe markiert werden, um eine Leistungserklärung zu erzeugen.
*   A+W SLT-Schnittstelle für externe Berechnung muss konfiguriert sein.

**Workflow**
1.  Menü Verkauf > Vorgang öffnen > Position markieren.
2.  Register Eigenschaften > Feld LE-Nummer: <Strg>+<T> drücken. Register Berechnung technische Werte wird geöffnet.
3.  Bereich Kopfdaten der Leistungserklärung: Kopfdaten der Leistungserklärung erfassen.
4.  Register Deklarierte Leistungen: Felder für die bestätigten Leistungen füllen. Felder mit * können über die A+W SLT-Schnittstelle gefüllt werden.
5.  Checkboxen markieren für Daten, die ausgegeben werden sollen.
6.  Ggf. Ermittlung der technischen Leistungen starten: [Ext.Berechnung] oder <F3> drücken.
7.  Daten mit [OK] übernehmen.

## Preisberechnung

**Übersicht**

| Help Card | Themen |
| :--- | :--- |
| • Positionskonditionen ändern | • Positionspreis prüfen und ändern. |
| • Artikelpreise ändern | • Artikelpreise ändern. |
| • Fußrabatt, Zuschlag bearbeiten | • Rabatte und Zuschläge prüfen und/oder ändern. Auftragsspezifischen Rabatt erfassen. |
| • Produktionskosten prüfen | • Produktionskosten im Auftrag prüfen. • Produktionskosten im Angebot prüfen. |
| • Preisprotokoll für VSG | • Preisberechnung für VSG-Position prüfen. |

### Positionskonditionen ändern (VK 04-001)

**Ziel der Handlung**
*   Positionspreis prüfen und ändern.

**Voraussetzungen**
*   Preise und Konditionen sind in den Stammdaten angelegt.

**Zusatzinfo**
*   Geänderte Konditionen werden nicht in die Stammdaten der Konditionen zurückschrieben.

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln, z. B. in ISO-Position.
2.  Cursor in Feld Preis stellen.
3.  In der Symbol-Leiste auf Icon [%] klicken. Dialog Konditionen (Glasart) wird geöffnet.
4.  Matrixzuordnung oder Grundpreis ändern.
5.  Zuschläge und Rabatte eingeben.
6.  Mit [OK] übernehmen.
7.  Abfrage mit [Ja] bestätigen: Preise werden mit manuellen Änderungen neu berechnen.
8.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### Artikelpreise ändern (VK 04-002)

**Ziel der Handlung**
*   Artikelpreise ändern.

**Voraussetzungen**
*   (Keine aufgeführt)

**Zusatzinfo**
*   Auf die gleiche Weise werden alle Preise geändert, z. B. Austauschpreise, Sprossenpreise, Unterteilpreise.

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln.
2.  Position(en) erfassen.
3.  Menü <F4> > Preisangabe > Auftragspreise > Artikelpreise.
4.  Dialog Auftragspreise wird geöffnet.
5.  Kondition und Artikel auswählen, z. B. Kunde und ein Floatglas.
6.  Preis und Preistyp angeben.
7.  Änderung mit <Ende> übernehmen.
8.  Abfrage mit [Ja] bestätigen: Preise werden in allen Positionen neu berechnen, in denen der gewählte Artikel enthalten ist.
9.  Auftrag speichern und beenden.

### Fußrabatt, Zuschlag bearbeiten (VK 04-003)

**Ziel der Handlung**
*   Rabatte und Zuschläge prüfen und/oder ändern.
*   Auftragsspezifischen Rabatt erfassen.

**Voraussetzungen**
*   Rabatte sind in den Stammdaten angelegt.

**Zusatzinfo**
*   Rabattarten mit negativem Vorzeichen werden als Zuschlag aufgeschlagen.
*   Die Sequenznummer legt die Reihenfolge fest, in der die Zuschläge und Rabatte berechnet werden.

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln.
2.  Positionen erfassen und speichern.
3.  Zum Fußteil wechseln: <Ende> drücken.
4.  Feld Rabatt: <F2> drücken. Dialog für Rabatte und Zuschläge wird geöffnet.
5.  Feld Abschlag, Feld Aufschlag: Werte für Zu- und Abschlag eingeben.

**Auftragsspezifischen Rabatt erfassen:**
6.  Neue Zeile einfügen: <F6> drücken und Details festlegen:
    *   Bezeichnung.
    *   Sequenznummer.
    *   Wert und Rabattart: Plus (+) = Zuschlag, Minus (-) = Rabatt.
    *   Berechnungsart, z. B. %.
    *   Berechnungsbasis, z. B. Warengruppe = Rabatt für alle Positionen dieser Warengruppe.
7.  Checkboxen markieren:
    *   Anfang der Zeile: berechnen ja/nein.
    *   Feld Pos: rückverteilen ja/nein.
8.  Detailansicht öffnen: <F5> drücken und Daten ggf. ergänzen oder korrigieren.
9.  Änderungen mit [OK] übernehmen.
10. Rabatte speichern und mit <Ende> in den Auftrag übernehmen.
11. Auftrag speichern und beenden.
12. Abfrage zur Neuberechnung der Preise mit [Ja] bestätigen.

### Produktionskosten prüfen (VK 04-004)

**Ziel der Handlung**
*   Produktionskosten im Auftrag prüfen.
*   Produktionskosten im Angebot prüfen.

**Voraussetzungen**
*   Materialkosten sind in den Stammdaten angelegt.
*   Auftrag muss bereits an die Produktion übergeben sein.
*   Produktionsübergabe muss für Angebote konfiguriert sein.

**Zusatzinfo**
*   Die Personal- und Maschinenkosten werden ermittelt und zurückgemeldet, wenn der Auftrag erfolgreich in die Produktion eingelastet wurde.
*   Angebote werden nur vorläufig in A+W Production eingelastet und nach der Rückmeldung der Kosten aus dem Lauf gelöscht.

**Workflow**
1.  Auftrag vollständig erfassen und speichern.
2.  Abfrage zur Freigabe für die Produktion mit [Ja] beantworten. Der Auftrag wird in den Auftragspool von A+W Production gestellt.

**Nach der Einlastung in A+W Production:**
3.  Auftrag öffnen.
4.  Position auswählen: in Feld Preis <Shift>+<F10> drücken. Dialog Produktionskostenkalkulation wird geöffnet.
5.  Register Übersicht: Kalkulierte Menge und/oder Preis prüfen.

**Einzelne Kosten prüfen:**
6.  Zeile in der Übersicht markieren und zu Register Details wechseln.
7.  Ggf. Schritte 4 bis 6 für alle Positionen wiederholen.

### Preisprotokoll für VSG (VK 04-005)

**Ziel der Handlung**
*   Preisberechnung für VSG-Position prüfen.

**Voraussetzungen**
*   Das Protokoll ist noch nicht für alle Preis- und Konditionenberechnungen verfügbar.

**Zusatzinfo**
*   Preisprotokoll kann in verschiedenen Formaten gespeichert werden.

**Workflow**
1.  Zum Register Positionen > Allgemein wechseln.
2.  Feld Preis: <Shift>+<F9> drücken. Dialog Konditionen für PKZ-VSG wird geöffnet.
3.  <Strg>+<L> drücken. Das Protokoll wird in einem Texteditor geöffnet.
4.  Protokoll ggf. speichern und Texteditor schließen.
5.  Dialog Konditionen für PKZ-VSG schließen.
6.  Erfassung fortsetzen oder Auftrag beenden.

## Rechnung

**Übersicht**

| Help Card | Themen |
| :--- | :--- |
| • Rechnung manuell erstellen | • Rechnung erstellen und buchen. • Teilrechnung erstellen. |
| • Rechnungen automatisch erzeugen | • Mehrere Rechnungen erzeugen und buchen. • Sammelrechnung erzeugen. |
| • Rechnung buchen | • Rechnung buchen. |
| • Rechnung drucken | • Einzelnes Dokument drucken. • Mehrere Dokumente drucken. |
| • Elektronische Rechnung (E-Invoicing) versenden | • Einzelne Rechnungen versenden. • Mehrere Rechnungen versenden. |
| • Kunden für elektronische Rechnungen konfigurieren | • Kunden für elektronische Rechnungen konfigurieren |
| • Gutschrift erfassen | • Gutschrift erfassen. • Reklamationsangaben erfassen. |

### Rechnung manuell erstellen (VK 05-001)

**Ziel der Handlung**
*   Rechnung manuell erstellen und buchen.
*   Teilrechnung erstellen.

**Voraussetzungen**
*   Aufträge müssen freigeschaltet sein.

**Zusatzinfo**
*   Das System kann so konfiguriert sein, dass die Rechnung automatisch zusammen mit dem Lieferschein erzeugt wird.
*   ⇨ Sammelrechnung: Rechnungen automatisch erzeugen
*   ⇨ Rechnung drucken

**Workflow**
1.  Menü Verkauf > Rechnungen > Manuelle Rechnung wählen.
2.  Kunde angeben.
3.  Feld Bezug:
    *   <F9>: Auftrag suchen und auswählen.
    *   <F8> > <F9> > Eintrag Lieferschein übernehmen > <F9>: Lieferscheinsuche suchen und übernehmen.
4.  Daten aus Vorgangssuche übernehmen.
5.  Feld Termin: Zahlungsziel angeben.
6.  Weiterspringen und ggf. weitere Felder ausfüllen. Dialog Neukalkulation des Vorgangs wird geöffnet.
7.  Kalkulation auswählen, wenn Auftrag überrechnet werden soll.
8.  Mit <Enter> bestätigen. Auftrag wird ggf. neu berechnet.
9.  Änderungen mit [OK] übernehmen.

**Teilrechnung erstellen:**
10. Feld Berech: Teilmengen angeben.
11. Änderungen mit [OK] speichern.
12. Felder im Fuß prüfen, z. B. Rabatt.
13. Abfrage zur Buchung mit [Ja] bestätigen.
    *   [Ja]: Die Rechnung wird gebucht und an die FiBu übergeben.
    *   [Nein]: Rechnung wird gespeichert und muss später manuell gebucht werden.
14. Die endgültige Rechnungsnummer wird gesetzt. Hinweis zur Rechnungsnummer und weitere Abfragen nach Bedarf bestätigen.

### Rechnungen automatisch erzeugen (VK 05-002)

**Ziel der Handlung**
*   Mehrere Rechnungen erzeugen und buchen.
*   Sammelrechnung erzeugen.

**Voraussetzungen**
*   Kunde erlaubt Sammelrechnungen.
*   Aufträge müssen freigeschaltet sein.

**Zusatzinfo**
*   Das System kann so konfiguriert sein, dass die Rechnung automatisch zusammen mit dem Lieferschein erzeugt wird.
*   ⇨ Rechnung drucken

**Workflow**
1.  Menü Verkauf > Rechnungen > Automatische Freigabe wählen. Dialog Rechnungen wird geöffnet.
2.  Feld Freigabe: <Strg>+<F8> drücken. Dialog zum Import der Werte wird geöffnet.
3.  Anfangs- und Enddatum für die Belegsuche eingeben.
4.  Import mit [OK] starten. Aufträge werden eingelesen.
5.  Schritte 2 und 4 nach Bedarf wiederholen.
6.  Weiterspringen und ggf. Belegdatum ändern.
7.  Rechnungserzeugung mit <F3> auslösen.
8.  Abfragen nach Bedarf bestätigen.

**Sammelrechnung erzeugen:**
9.  Feld Freigabe: <Shift>+<F8> drücken. Dialog zur Angabe der Kundennummer wird geöffnet.
10. Kundennummer eingeben und übernehmen. Aufträge werden eingelesen.
11. Rechnungserzeugung mit <F3> auslösen.

### Rechnung buchen (VK 05-003)

**Ziel der Handlung**
*   Rechnung buchen.

**Voraussetzungen**
*   Rechnungen müssen erzeugt sein.

**Zusatzinfo**
*   Das System kann so konfiguriert sein, dass die Rechnung automatisch zusammen mit dem Lieferschein gedruckt und gebucht wird.

**Workflow**
1.  Menü Verkauf > Rechnungen > Rechnung buchen wählen.
2.  Feld Rechnung: <Strg>+<F8> drücken. Dialog zum Import der Werte wird geöffnet.
3.  Anfangs- und Enddatum für die Belegsuche eingeben.
4.  Import mit [OK] starten.
5.  Schritte 3 und 4 nach Bedarf wiederholen.
6.  Feld Bu. markieren.
7.  Buchung mit <F3> auslösen.
8.  Abfragen zur Buchung mit [Ja] bestätigen. Die Rechnungen werden gebucht und an die FiBu übergeben.

### Rechnung drucken (VK 05-004)

**Ziel der Handlung**
*   Einzelnes Dokument drucken.
*   Mehrere Dokumente drucken.

**Voraussetzungen**
*   Druckverwaltung ist eingerichtet.
*   E-Mail-Adressen der Kunden sind eingepflegt.
*   Faxnummern der Kunden sind eingepflegt.

**Zusatzinfo**
*   Automatischer Versand: Menü Verkauf > Formulare > E-Mail/Fax.
*   Auf die gleiche Weise werden alle Dokumente gedruckt, z. B. Auftragsbestätigungen, Lieferscheine, Sammelrechnungen.

**Workflow**
1.  Menü Verkauf > Formulare > Druck. Dialog Formularart wird geöffnet.
2.  Formularart wählen und mit <Ende> übernehmen, z. B. Rechnung. Dialog Formulardruck wird geöffnet.
3.  Voreinstellungen wählen und mit <Enter> übernehmen, z. B.:
    *   1 zusätzliches Exemplar.
    *   Diverse Nummern vorgeben.
4.  Feld Vorgang: mit <F9> Rechnungsnummer auswählen und übernehmen.
5.  Rechnungsnummer(n) mit [OK] bestätigen. Dialog Drucken auf wird geöffnet.
6.  Drucker auswählen und Druck der Rechnung mit <Enter> starten.

**Mehrere Rechnungen drucken:**
7.  Voreinstellungen wählen, z. B. Nummern auswählen und mit <Enter> übernehmen.
8.  Auftragsnummern eingrenzen, z. B. auf eigene Aufträge vom Vortag:
    *   Mitarbeiternummer eingeben.
    *   Erfassungsdatum eingrenzen.
    *   Ersten und letzten Vorgang auswählen.
9.  Mit <F3> Auftragsnummern des eingegrenzten Bereichs einlesen.
10. Feld Dr: zur Druckausgabe J oder N wählen.
11. Druck mit <F3> auslösen. Dialog Drucken auf wird geöffnet.
12. Drucker auswählen und Druck der Rechnungen mit <Enter> starten.

### Elektronische Rechnung (E-Invoicing) versenden (VK 05-004)

**Ziel der Handlung**
*   elektronische Rechnung versenden

**Voraussetzungen**
*   Druckverwaltung ist eingerichtet.
*   E-Mail-Adressen der Kunden sind eingepflegt.
*   Elektronische Rechnungserstellung ist für den Marktpartner ist aktiviert.
*   elektronische Rechnung wurde bei der Buchung der Rechnung erstellt.

**Zusatzinfo**
*   Automatischer Versand: Menü Verkauf > Formulare > E-Mail/Fax.
*   Auf die gleiche Weise werden alle Dokumente gedruckt, z. B. Auftragsbestätigungen, Lieferscheine, Sammelrechnungen.

**Workflow**
1.  Menü Verkauf > Formulare > Email/Fax auswählen. Dialog E-Mail wird geöffnet.
2.  Formularart Rechnung wählen und mit <Ende> übernehmen.
3.  Voreinstellungen wählen und mit <Enter> übernehmen.
4.  Feld Vorgang: mit <F9> Rechnungsnummer auswählen und übernehmen.
5.  Rechnungsnummer(n) mit Send bestätigen.

**Mehrere Rechnungen versenden:**
6.  Voreinstellungen wählen und mit <Enter> übernehmen.
7.  **Nummern auswählen:** Rechnungsnummer eingrenzen:
    *   Mitarbeiternummer eingeben.
    *   Erfassungsdatum eingrenzen.
    *   Ersten und letzten Vorgang auswählen.
8.  Mit <F3> Auftragsnummern des eingegrenzten Bereichs einlesen.
9.  Feld Dr: zur Druckausgabe J oder N wählen.
10. Feld RV: zum Versand der E-Rechnung J oder N wählen.
11. Senden mit <F3> auslösen.

### Kunden für elektronische Rechnungen konfigurieren (VK 05-005)

**Ziel der Handlung**
*   Ein Kunde soll elektronische Rechnungen erhalten.

**Voraussetzungen**
*   Der Kunde besteht bereits im System.
*   Der Formularart wurde eine Empfänger-E-Mail-Adresse zugeordnet.

**Zusatzinfo**
*   Wenn für den Auftragskunden ein FIBU-Debitor mit abweichender Marktpartnernummer hinterlegt ist, muss die gesamte beschriebene Stammdatenkonfiguration für den FIBU-Debitor erfolgen.

**Workflow**
1.  Menü Stammdaten > Marktpartner > wählen. Dialog Marktpartner wird geöffnet.
2.  Partnertyp Kunde wählen und mit <Enter> übernehmen.
3.  Kundennummer eingeben und mit <Enter> übernehmen. Die Kundendaten werden geladen.
4.  folgenden Stammdaten müssen bei dem Kunden gepflegt sein:
    *   Dialog Adresse die E-Mail-Adresse
    *   Dialog Identifikation die Ustd.-Identnr.
    *   Dialog Rechnung
        *   Feld E-Rechnung zur Erstellung XRechnung wählen
        *   Feld Leitweg-ID: Leitweg-ID vom Kunden hinterlegen.
        *   Feld Sendeart: zur Versandtart E-Rechnung+PDF oder E-Rechnung wählen.
5.  Definition mit [OK] bestätigen.

### Gutschrift erfassen (VK 05-006)

**Ziel der Handlung**
*   Gutschrift erfassen.
*   Reklamationsangaben erfassen.

**Voraussetzungen**
*   (Keine aufgeführt)

**Zusatzinfo**
*   Gutschrift kann mit Bezug zu Auftrag, Rechnung, Lieferschein oder Gutschrift erfasst werden.
*   Gutschrift kann ohne Bezug erfasst werden, z. B. aus Kulanz wegen schlechterer Qualität.
*   Gutschrift buchen: Menü Verkauf > Gutschriften > Gutschrift buchen.

**Workflow**
1.  Menü Verkauf > Gutschriften > Gutschrift erfassen wählen. Dialog Gutschriften wird geöffnet.
2.  Kunde auswählen.
3.  Feld Bezug: <F9> drücken. Dialog Suche Bezugsvorgang wird geöffnet.
4.  Feld Vorgang: mit <F9> Vorgangsart auswählen, z. B. Verkaufs-Rechnung.
5.  Vorgang suchen und übernehmen.
6.  Kopfdaten der Gutschrift prüfen.
7.  Register Positionen:
    *   Feld Gutschr: Positionsmengen für Gutschrift angeben.
    *   oder
    *   Feld Preis: Preise für Gutschrift angeben.
8.  Änderungen mit [OK] bestätigen. Dialog zur Auswahl von Reklamationsart, Reklamationsort usw. wird geöffnet.
9.  Ggf. Angaben zur Reklamation auswählen.
10. Reklamationsdatum eingeben.
11. Angaben mit <Enter> bestätigen und übernehmen.
12. Abfragen bestätigen.
13. Gutschrift speichern.
14. Abfrage zur Buchung mit [Ja] bestätigen.
    *   [Ja]: Die Gutschrift wird gebucht und an die FiBu übergeben. Die endgültige Gutschriftsnummer wird gesetzt.
    *   [Nein]: Gutschrift wird gespeichert und muss später manuell gebucht werden.

## Weitere Themen

**Übersicht**

| Help Card | Themen |
| :--- | :--- |
| • Vorgang suchen | • Aufträge des aktuellen Tages suchen. • Aufträge zu einem Kunden suchen. • Aufträge zu Datum und/oder Erfasser suchen. |
| • Vorgangsänderung | • Route ändern. • Liefertermin ändern. • Stornostatus setzen oder löschen. |

### Vorgang suchen (VK 06-001)

**Ziel der Handlung**
*   Aufträge des aktuellen Tages suchen.
*   Aufträge zu einem Kunden suchen.
*   Aufträge zu Datum und/oder Erfasser suchen.

**Voraussetzungen**
*   (Keine aufgeführt)

**Zusatzinfo**
*   Auf die gleiche Weise werden alle Vorgänge gesucht.

**Workflow**

**Aufträge des aktuellen Tages suchen:**
1.  Menü Verkauf > Auftragserfassung wählen.
2.  Aufträge des aktuellen Tages suchen: <F8> drücken.
3.  Auftrag markieren und übernehmen.

**Aufträge ab einer bestimmten Auftragsnummer suchen:**
4.  Feld Auftrag: <F9> drücken. Dialog Suche Aufträge wird geöffnet.
5.  Feld Aufträge ab: Startnummer eingeben.
6.  Suche mit <F3> auslösen.

**Aufträge zu einem Kunden suchen:**
7.  Feld Auftrag: <F9> drücken. Dialog Suche Aufträge wird geöffnet.
8.  Feld Kunde: Kundennummer eingeben.
9.  Suche mit <F3> auslösen.

**Aufträge zu Datum und/oder Erfasser suchen:**
10. Feld Auftrag: <F9> drücken. Dialog Suche Aufträge wird geöffnet.
11. Register Vorgangs-Schlüssel:
    *   Feld Erfasser: Mitarbeiternummer eingeben.
    *   Feld Erfassungsdatum: Datum eingeben.
12. Suche mit <F3> auslösen.
13. Auftrag in der Trefferliste mit Doppelklick in die Auftragserfassung übernehmen.

### Vorgangsänderung (VK 06-002)

**Ziel der Handlung**
*   Route ändern.
*   Liefertermin ändern.
*   Stornostatus setzen oder löschen.

**Voraussetzungen**
*   Vorgang ist nicht gesperrt.

**Zusatzinfo**
*   Änderungen, die nicht an die nachfolgenden Prozesse weitergegeben werden, werden mit Lokale Änderung gekennzeichnet. Aufträge mit diesem Kennzeichen müssen z. B. manuell an den Versand übergeben werden.

**Workflow**
1.  Menü Verkauf > Vorgangsänderung wählen. Dialog Vorgangsänderung wird geöffnet.
2.  Feld Vorgang: Vorgangsart wählen. z. B. Auftrag.
3.  Feld Nummer: <F9> drücken. Dialog Suche Aufträge wird geöffnet.
4.  Feld Kunde: Kundennummer eingeben und Suche starten. Trefferliste wird angezeigt.
5.  Auftrag mit Doppelklick in Dialog Vorgangsänderung übernehmen.
6.  In die Felder springen und Einstellung ändern, z. B.:
    *   Feld Lokale Korrekt.: Freien Text eingeben.
    *   Feld Sto: Stornokennzeichen setzen.
    *   Feld Route: Route ändern.
    *   Feld Termin: Liefertermin ändern.
    *   Feld Frei: Änderungen freischalten.
7.  Änderungen mit <F3> speichern.

**In den Vorgang wechseln:**
8.  Vorgang mit Doppelklick zur Bearbeitung öffnen.
9.  Daten prüfen und ggf. ändern.
10. Änderungen mit [OK] speichern.

# A+W Enterprise Einkauf

## Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| 02-2022 | Diverse Ergänzungen in der Softwarereferenz |
| 08-2020 | Vollständige Überarbeitung |
| 06-2019 | Vollständige Überarbeitung |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 03-2014 | Vollständige Überarbeitung |
| 02-2007 | Ersterstellung |

Zu diesem Modul finden Sie folgende Kapitel:
*   ⇨Softwarereferenz

## Inhaltsverzeichnis

*   Übersicht
    *   Menü Einkauf
    *   Konfiguration Bestellpool
    *   Konfiguration Eigene Einkaufsvorgänge
    *   Untermenü Wareneingang
    *   Untermenü Rechnungen
    *   Untermenü Übersicht
*   Zusatzmenü
    *   Untermenü Preisangaben
    *   Untermenü Auftragspreise
    *   Untermenü Spezielle Texte
    *   Untermenü Produktangaben
    *   Untermenü Technische Werte
*   Infomenü
    *   Untermenü Anmerkungen
*   Zusatzmenü zum Wareneingang
    *   Wareneingang - Zusatzmenü
*   Suchfunktionen
    *   Suche Bestellungen
        *   Suche Bestellungen - Vorgangs-Schlüssel
        *   Suche Bestellungen - Positions-Schlüssel
        *   Suche Bestellungen - Direkte Suche
    *   Suche Bestellungen - Trefferliste
        *   Trefferliste - Allgemein
        *   Trefferliste - Mengen
        *   Trefferliste – WE-Infos
        *   Trefferliste - Artikel
        *   Trefferliste - Verschiedenes
*   Bestellpool
    *   Spezielle Menüs zum Bestellpool
        *   Bestellpool - Zusatzmenü
        *   Bestellpool - Infomenü
    *   Bestellungen erzeugen
        *   Bestellungen erzeugen - Lieferant
        *   Bestellungen erzeugen - Position
        *   Bestellungen erzeugen - Details
*   Vorgangsverwaltung
    *   Symbolerklärung
    *   Lieferanten-Anfragen
    *   Bestellerfassung
        *   Bestellerfassung – Kopf, Fuß
        *   Bestellerfassung - Anschriften
        *   Bestellerfassung - Eigenschaften
        *   Bestellerfassung - Verschiedenes
        *   Bestellerfassung – Summen
        *   Bestellerfassung - Detailansicht Rabatte
    *   Bestellpositionen
        *   Bestellpositionen – Allgemein
        *   Bestellpositionen - Eigenschaften
        *   Bestellpositionen – Preise
        *   Bestellpositionen - Auftragsinfo
        *   Bestellpositionen - Status
        *   Bestellpositionen - Bewertung
    *   Abholadresse
    *   Bestellarten
    *   Dokumentenartenzuordnung
*   Texte
    *   Auftragstexte
*   Formulardruck
*   Bestellfreigabe
    *   Bestellfreigabe - Auswahl
    *   Bestellfreigabe - Details
    *   Bestellfreigabe - Weitere Felder
*   Wareneingang
    *   Lieferavis
        *   Lieferavis - Übersicht
        *   Lieferavis - Details
    *   Bestellung - Übersicht (Lieferavis)
    *   Bestellung - Details (Lieferavis)
    *   Lieferplan
        *   Lieferplan - Details
    *   Wareneingang (automatisch)
    *   Positionsinfo
    *   Buchung Gestelle
    *   Wareneingang (manuell)
    *   Gestellbezogener Wareneingang
        *   Gestellbezogener Wareneingang
        *   Gestellbelegung
    *   Wareneingangskontrolle
    *   Fehlmengenkontrollpool
        *   Fehlmengenkontrollpool – Übersicht
        *   Fehlmengenkontrollpool – Details
    *   Wareneingangsprotokoll
*   Rechnungen und Gutschriften
    *   Rechnungskontrolle
        *   Lieferanten-Rechnung - Bestellübersicht
        *   Lieferanten-Rechnung - Detailansicht
        *   Lieferanten-Rechnung - Positionsübersicht
        *   Lieferanten-Rechnung - Rabatte
    *   Lieferanten-Rechnung (automatisch)
    *   Übertragene Rechnungen
    *   Lieferanten-Rechnung (manuell)
    *   Lieferanten-Rechnung (Sammelrechnung)
    *   Rechnungen buchen
    *   Bestellungen abschließen
    *   Rechnungsprotokoll
    *   Lieferanten-Gutschrift
*   Übersichten
    *   Bestellinformation
    *   Übersicht zu Vorgängen
    *   Einkaufs-Recherche
        *   Einkaufs-Recherche - Suchmodus
        *   Einkaufs-Recherche - Übersicht
        *   Einkaufs-Recherche - Details

## Übersicht

Im Modul Einkauf verwalten Sie die Vorgänge, die zur erfolgreichen Abwicklung des Einkaufsgeschäfts erforderlich sind, wie Bestellungen, Anfragen, Wareneingänge und Rechnungen.

Im Part Einkauf finden Sie folgende Themen:
*   "Suchfunktionen" auf Seite E-1547
*   "Vorgangsverwaltung" auf Seite E-1574
*   "Bestellpool" auf Seite E-1560
*   "Texte" auf Seite E-1624
*   "Wareneingang" auf Seite E-1632
*   "Rechnungen und Gutschriften" auf Seite E-1657
*   "Übersichten" auf Seite E-1673

### Menü Einkauf

Einige der verfügbaren Menü-Einträge verzweigen in Untermenüs. Wenn diese mehr als drei Einträge umfassen, sind sie nach der folgenden Übersicht separat aufgeführt. Die angezeigten Einträge sind von der jeweiligen Konfiguration abhängig.
*   **Konfiguration Bestellpool**
*   **Konfiguration Auftragsorientierter Bestelldruck** - diese Konfiguration findet keine Anwendung statt. Aus diesem Grund wird das hier nicht beschrieben.
*   **Konfiguration Eigene Einkaufsvorgänge**

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

> **Kontext-Menüs**
> In den Kontext-Menüs (rechte Maustaste) werden zu den einzelnen Feldern der Dialoge jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen in den Kontext-Menüs können Sie auch über die beschriebenen Menüs aufrufen. In der Regel entsprechen die Menüpunkte im Kontext-Menü den angebotenen Funktionen in der Prompt-Anzeige.

Alle Dialoge und Funktionen, die den Verkauf betreffen, erreichen Sie über das Menü Einkauf:

### Konfiguration Bestellpool

Bei der Einkaufskonfiguration Bestellpool handelt sich um meist verbreiterte Einstellungen. Die Erklärungen, Beispiele und weitere Hinweise in diesem Dokument basieren sich, sofern nichts weiteres explizit erwähnt ist, auf diese Konfiguration.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Bestellungen erzeugen | ⇨ "Bestellungen erzeugen" auf Seite E-1563 |
| b | Anfragen | ⇨ "Lieferanten-Anfragen" auf Seite E-1577 |
| c | Bestellverwaltung | ⇨ "Bestellerfassung" auf Seite E-1578 |
| d | Formular | |
| da | • Druck | Verkauf, "Formulardruck" auf Seite D-1420 |
| db | • E-Mail/Fax | Verkauf, "E-Mail" auf Seite D-1424 |
| e | Listendruck | Verkauf, "Listendruck" auf Seite D-1428 |
| f | Bestell-Freigabe | ⇨ "Bestellfreigabe" auf Seite E-1626 |
| g | Lieferavis | "Lieferavis" auf Seite E-1632 |
| h | Wareneingang | ⇨ "Untermenü Wareneingang" auf Seite E-1539 |
| i | Rechnungen | ⇨ "Untermenü Rechnungen" auf Seite E-1539 |
| j | Gutschriften | |
| ja | • Gutschriften erfassen | "Lieferanten-Gutschrift" auf Seite E-1671 |
| jb | • Gutschriften buchen | Verkauf, "Gutschriften buchen" auf Seite D-1416 |
| k | Übersicht | ⇨ "Untermenü Übersicht" auf Seite E-1540 |
| l | Recherche | "Einkaufs-Recherche" auf Seite E-1674 |

### Konfiguration Eigene Einkaufsvorgänge

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Lagerbestellung erzeugen | ⇨ "Bestellungen erzeugen" auf Seite E-1563 |
| b | Anfragen erfassen und bearbeiten | ⇨ "Lieferanten-Anfragen" auf Seite E-1577 |
| c | Bestellungen erfassen und bearbeiten | "Bestellerfassung" auf Seite E-1578 |
| d | Druck von Formularen verwalten | Verkauf, "Formulardruck" auf Seite D-1420 |
| e | Druck von Listen verwalten | Verkauf, "Listendruck" auf Seite D-1428 |
| f | Mehrere Bestellungen freischalten und verwalten | ⇨ "Bestellfreigabe" auf Seite E-1626 |
| g | Einzelne Bestellungen freischalten und verwalten | ⇨ "Bestellfreigabe" auf Seite E-1626 |
| h | Lieferbestätigungen erfassen und verwalten | "Lieferavis" auf Seite E-1632 |
| i | Wareneingang verwalten | ⇨ "Untermenü Wareneingang" auf Seite E-1539 |
| j | Rechnungen erfassen und bearbeiten | "Untermenü Rechnungen" auf Seite E-1539 |
| ka | • Lieferanten-Gutschriften erfassen | "Lieferanten-Gutschrift" auf Seite E-1671 |
| kb | • Gutschriften buchen | Verkauf, "Gutschriften buchen" auf Seite D-1416 |
| l | Vorgangsübersichten anzeigen | ⇨ "Untermenü Übersicht" auf Seite E-1540 |
| m | Vorgänge im Einkauf suchen | "Einkaufs-Recherche" auf Seite E-1674 |

### Untermenü Wareneingang
**Einkauf > Wareneingang**
Über dieses Menü erreichen Sie die Dialoge, in denen Sie den Wareneingang verwalten.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| ha | Lieferplan | ⇨ "Lieferplan" auf Seite E-1641 |
| hb | Automatischer Wareneingang | ⇨ "Wareneingang (automatisch)" auf Seite E-1644 |
| hc | Manueller Wareneingang | ⇨ "Wareneingang (manuell)" auf Seite E-1648 |
| hd | Gestellbezogener Wareneingang | ⇨ "Gestellbezogener Wareneingang" auf Seite E-1650 |
| he | Bestellungen abschließen | ⇨ "Wareneingang" auf Seite E-1632 |
| hf | Wareneingangskontrolle | ⇨ "Wareneingangskontrolle" auf Seite E-1654 |
| hg | Fehlmengenkontrollpool | ⇨ "Fehlmengenkontrollpool" auf Seite E-1655 |
| hh | Protokoll | ⇨ "Rechnungsprotokoll" auf Seite E-1671 |

### Untermenü Rechnungen
**Einkauf > Rechnungen**
Über dieses Menü erreichen Sie die Dialoge, in denen Sie die Einkaufsrechnungen verwalten.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| ia | Rechnungskontrolle | ⇨ "Rechnungskontrolle" auf Seite E-1657 |
| ib | Automatische Rechnungen | ⇨ "Lieferanten-Rechnung (automatisch)" auf Seite E-1664 |
| ic | Übertragene Rechnungen | ⇨ "Übertragene Rechnungen" auf Seite E-1666 |
| id | Manuelle Rechnungen | ⇨ "Lieferanten-Rechnung (manuell)" auf Seite E-1667 |
| ie | Sammelrechnungen | ⇨ "Lieferanten-Rechnung (Sammelrechnung)" auf Seite E-1668 |
| if | Rechnungen buchen | ⇨ "Rechnungen buchen" auf Seite E-1669 |
| ig | Bestellungen abschließen | ⇨ "Wareneingang" auf Seite E-1632 |
| ih | Protokoll | ⇨ "Rechnungsprotokoll" auf Seite E-1671 |

### Untermenü Übersicht
**Einkauf > Übersicht**
Über dieses Menü erreichen Sie die Dialoge, in denen Sie sich Übersichten zu den verschiedenen Vorgängen anzeigen lassen können.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| ka | Heute geplanter Wareneingang | ⇨ “Diese Übersichten sind konfigurationsabhängig und müssen separat freigeschaltet werden. Diese Dialoge können bei Bedarf kundenindividuell gestaltet werden. Bitte kontaktieren Sie einen Service-Mitarbeiter der A+W Software GmbH." auf Seite E-1674 |
| kb | Geplanter Wareneingang - verspätet | ⇨ “Übersicht zu Vorgängen" auf Seite E-1674 |
| kc | Geplanter Wareneingang von-bis | ⇨ "Übersicht zu Vorgängen" auf Seite E-1674 |
| kd | Geliefert - nicht berechnet | ⇨ “Übersicht zu Vorgängen" auf Seite E-1674 |
| ke | Berechnet - nicht gebucht | ⇨ “Übersicht zu Vorgängen" auf Seite E-1674 |
| kf | Noch nicht übertragene Best. | ⇨ "Übersicht zu Vorgängen" auf Seite E-1674 |
| kg | Vorgangs-Recherche | ⇨ Verkauf, "Vorgangs-Recherche" auf Seite D-1445 |
| kh | Bestellinformation | "Bestellinformation" auf Seite E-1673 |

### Zusatzmenü
Das Zusatzmenü rufen Sie mit **<F4>** beim Erfassen der verschiedenen Vorgänge auf, z. B. bei einer Bestellung.
Die Einträge im Zusatzmenü werden in kontextabhängigen Ausführungen angezeigt:
*   Zusatzmenü für den Kopf- und Fußbereich
*   Zusatzmenü für den Positionsbereich

#### Zusatzmenü für den Kopf- und Fußbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Texte | |
| a a | • Kopftext | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-1313 |
| a b | • Fußtext | Verkauf, "Kopf- und Fußtexte" auf Seite D-1313 |
| a c | • Fremdinformationen | Verkauf, "Fremdinformationen" auf Seite D-1319 |
| b | Adressen | |
| b a | • Lieferadressen suchen | Verkauf, "Adressen Suche" auf Seite D-1099 |
| b b | • Neue Lieferadresse | Verkauf, "Neue Lieferadresse" auf Seite D-1192 |
| b c | • Lieferadresse löschen | Löscht die Lieferadresse aus dem Vorgang. |
| b d | • Abholadresse | ⇨ "Abholadresse" auf Seite E-1620 |
| c | Storno | ⇨ "Bestellarten" auf Seite E-1622 |
| d | Preisangaben | ⇨ "Untermenü Preisangaben" auf Seite E-1542 |
| e | Produktangaben | |
| e a | • Produktaustausch | "Bestellarten" auf Seite E-1622 |
| e b | • A/Z-Regeln | ⇨ Stammdaten, "Austausch-/Zusatzregel" auf Seite J-102 |
| f | Wiedervorlage | ⇨ Verkauf, "Wiedervorlage” auf Seite D-1463 |
| g | Konfigurierbare Felder | ⇨ Verkauf, "Konfigurierbare Felder" auf Seite D-1201 |

#### Zusatzmenü für den Positionsbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Texte | |
| a a | • Kopftext | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-1313 |
| a b | • Fußtext | Verkauf, "Kopf- und Fußtexte" auf Seite D-1313 |
| a c | • Fremdinformationen | Verkauf, "Fremdinformationen" auf Seite D-1319 |
| a d | • Artikeltext | Verkauf, "Artikel- und Positionstexte" auf Seite D-1315 |
| a e | • Positionstext | Verkauf, "Artikel- und Positionstexte" auf Seite D-1315 |
| a f | • Spezielle Texte | ⇨ "Untermenü Preisangaben" auf Seite E-1542 |
| b | Adressen | |
| b a | • Lieferadressen suchen | Verkauf, "Adressen Suche" auf Seite D-1099 |
| b b | • Neue Lieferadresse | Verkauf, "Neue Lieferadresse" auf Seite D-1192 |
| b c | • Lieferadresse löschen | Löscht die Lieferadresse aus dem Vorgang. |
| b d | • Endkundenanschrift | Verkauf, "Endkundenanschrift" auf Seite D-1195 |
| c | Storno | "Bestellarten" auf Seite E-1622 |
| d | Private Felder | Verkauf, "Private Felder" auf Seite D-1221 |
| e | Preisangaben | ⇨ "Untermenü Preisangaben" auf Seite E-1542 |
| f | Produktangaben | ⇨ "Untermenü Produktangaben" auf Seite E-1543 |
| g | Wiedervorlage | Verkauf, "Wiedervorlage" auf Seite D-1463 |
| h | Kommission | |
| h a | • neue Kommission | ⇨ "Bestellpositionen - Allgemein" auf Seite E-1599 |
| h b | • Kommission ändern | ⇨ "Bestellpositionen - Allgemein" auf Seite E-1599 |
| i | Lieferplan | Verkauf, "Lieferplan" auf Seite D-1386 |
| j | Lager | |
| j a | • Stapel | ⇨ "Bestellpositionen - Allgemein" auf Seite E-1599 |
| j b | • Lagerprognose | ⇨ Verkauf, "Bestandsprognose" auf Seite D-1206 |
| k | Konfigurierbare Felder | ⇨ Verkauf, "Konfigurierbare Felder" auf Seite D-1201 |

### Untermenü Preisangaben
**<F4> > Preisangaben**
Über dieses Menü verwalten Sie die Preise und Konditionen für den Artikel der markierten Position.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Auftragskonditionen | Verkauf, "Positionskonditionen" auf Seite D-1340 |
| b | Auftragspreise | ⇨ "Untermenü Auftragspreise" auf Seite E-1542 |
| c | Teilkalkulation | Verkauf, "Produktionskostenkalkulation" auf Seite D-1372 |
Die folgenden Einträge werden nur im Positionsbereich angezeigt:
| d | Positionskonditionen | Verkauf, "Positionskonditionen" auf Seite D-1340 |
| e | Konditionen holen | Ermittelt den Verkaufspreis mit den Positionskonditionen und berechnet den Preis neu. |
| f | Preisberechnung | Berechnet den Positionspreis neu. |
| g | Preiskontrolle | ⇨ "Bestellpositionen - Allgemein" auf Seite E-1599 |

#### Untermenü Auftragspreise
**<F4> > Preisangaben > Auftragspreise**
Über dieses Menü verwalten Sie die Auftragspreise.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Artikelpreise | Verkauf, "Auftragspreise" auf Seite D-1328 |
| b | Sprossenpreise | ⇨ Verkauf, "Auftragssprossenpreise" auf Seite D-1330 |
| c | Austauschpreise | Verkauf, "Auftragsaustauschpreise" auf Seite D-1333 |
| d | Unterteilpreise | ⇨ Verkauf, "Auftragsunterteilpreise" auf Seite D-1335 |

### Untermenü Spezielle Texte
**<F4> > Texte > Spezielle Texte**
Über dieses Menü verwalten Sie alle speziellen Texte, die Sie dem Vorgang zuordnen können. Diese Texte sind in der Regeln kundenindividuell konfigurierbar und somit sind sie nicht der Bestandteil dieser Dokumentation.
Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

### Untermenü Produktangaben
**<F4> > Produktangaben**
Über dieses Menü verwalten Sie die Angaben für die Produkte, z. B. Austausch- und Zusatzregeln.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Produktaustausch | "Bestellarten" auf Seite E-1622 |
| b | A/Z-Regeln | ⇨ Stammdaten, "Austausch-/Zusatzregeln" auf Seite B-304 |
Die folgenden Einträge werden nur im Positionsbereich angezeigt:
| c | Warengruppe | ⇨ "Bestellpositionen - Allgemein" auf Seite E-1599 |
| d | Technische Werte | "Untermenü Technische Werte" auf Seite E-1543 |

#### Untermenü Technische Werte
**<F4> > Produktangaben > Technische Werte**
Über dieses Menü verwalten Sie die technischen Werte.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Technische Werte anzeigen | Zeigt die technischen Werte an. |
| b | Technische Werte ändern | Wechselt zu den technischen Werten, damit sie bearbeitet werden können. Der Cursor wechselt in das Feld dB-Wert der technischen Werte im Register Positionen. ⇨ Verkauf, "Texte" auf Seite E-1624 |
| c | Leistungserklärung | Zeigt die verdeckten Maßangaben im Register Positionen an. |
| d | Verdeckte Maßangaben anzeigen | ⇨ Verkauf, "Artikel-Maßangaben" auf Seite D-1205 |
| e | Verdeckte Maßangaben ändern | |

### Infomenü
**<Shift> + <F4>**
Das Infomenü wird in kontextabhängigen Ausführungen angezeigt:
*   Infomenü für den Kopf- und Fußbereich
*   Infomenü für den Positionsbereich

#### Infomenü für den Kopf- und Fußbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Vorgangs-Anmerkungen | ⇨ Verkauf, "Anmerkungen" auf Seite D-1304 |
| b | Marktpartner-Anmerkungen | |
| c | Objekt-Anmerkungen | |
| d | Vorgangs-Recherche | ⇨ Verkauf, "Vorgangs-Recherche" auf Seite D-1445 |
| e | Vorgangs-Übersicht | ➡ Verkauf, "Übersicht" auf Seite D-1202 |
| f | Marktpartner-Information | ⇨ Verkauf, "Marktpartner-Info" auf Seite D-1197 |
| g | Änderungsprotokoll | ⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-1230 |
| h | Lieferplan | ⇨ "Lieferplan" auf Seite E-1641 |
| i | Lieferterminänderungen | ⇨ Verkauf, "Lieferterminänderungs-Protokoll" auf Seite D-1232 |
| j | Heute geplanter Wareneingang | ⇨ "Diese Übersichten sind konfigurationsabhängig und müssen separat freigeschaltet werden. Diese Dialoge können bei Bedarf kundenindividuell gestaltet werden. Bitte kontaktieren Sie einen Service-Mitarbeiter der A+W Software GmbH." auf Seite E-1674 |
| k | Geplanter Wareneingang – verspätet | ⇨ “Übersicht zu Vorgängen" auf Seite E-1674 |
| l | Geplanter Wareneingang von-bis | ⇨ "Übersicht zu Vorgängen" auf Seite E-1674 |
| m | Geliefert - nicht berechnet | ⇨ "Übersicht zu Vorgängen" auf Seite E-1674 |
| n | Berechnet - nicht gebucht | ⇨ "Übersicht zu Vorgängen" auf Seite E-1674 |
| o | Gestellverwaltung | ⇨ "Buchung Gestelle" auf Seite E-1647 |
| p | Auslieferdatum | Zeigt für auftragsbezogene Bestellungen folgende Informationen aus dem Kundenauftrag an: Auftragsnummer, Liefertermin, Route |
| r | Bestellinformation | ⇨ "Bestellinformation" auf Seite E-1673 |

#### Infomenü für den Positionsbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Anmerkungen | Untermenü Anmerkungen |
| b | Vorgangs-Recherche | ⇨ Verkauf, "Vorgangs-Recherche" auf Seite D-1445 |
| c | Vorgangs-Übersicht | Verkauf, "Übersicht" auf Seite D-1202 |
| d | Marktpartner-Information | ⇨ Verkauf, "Marktpartner-Info" auf Seite D-1197 |
| e | Änderungsprotokoll | ⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-1230 |
| f | Lieferplan | ⇨ "Lieferplan" auf Seite E-1641 |
| g | Gestellverwaltung | ⇨ "Buchung Gestelle" auf Seite E-1647 |
| h | Bemerkung | ⇨ "Bestellpositionen - Allgemein" auf Seite E-1599 |
| i | Auslieferdatum | Zeigt für auftragsbezogene Bestellungen folgende Informationen aus dem Kundenauftrag an: Auftragsnummer, Liefertermin, Route |
| j | Bestellinformation | ⇨ "Bestellinformation" auf Seite E-1673 |

#### Untermenü Anmerkungen
**<Shift> + <F4> > Anmerkungen**
Das Infomenü Anmerkungen wird nur im Register Bestellverwaltung – Positionen angezeigt.
Im Bestellkopf öffnen Sie die vorhandenen Anmerkungen über den Infomenü <Shift> + <F4> direkt.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Vorgangs-Anmerkungen | ⇨ Verkauf, "Anmerkungen" auf Seite D-1304 |
| b | Lieferanten-Anmerkungen | |
| c | Lieferanten-Artikel-Anmerkungen | |
| d | Objekt-Anmerkungen | |
| e | Objekt-Artikel-Anmerkungen | |
| f | Kunden-Anmerkungen | |
| g | Kunden-Artikel-Anmerkungen | |

### Zusatzmenü zum Wareneingang
In den Dialogen mit automatischen Datenverarbeitung, wie Wareneingang, Lieferanten-Rechnung, Bestellungen abschließen, kann mit **<F4>** das dialogspezifische Zusatzmenü aufgerufen werden. Die angezeigten Einträge sind optional, je nach dem, in welchen Dialog das Menü aufgerufen wurde. In der folgenden Übersicht des Menüs sind immer alle Einträge aufgeführt.

> **Kontext-Menüs**
> In den Kontext-Menüs zu den einzelnen Feldern der Dialog werden jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen entsprechen den Funktionen, die Sie über die im Folgenden beschriebenen Menüs aufrufen.

#### Wareneingang – Zusatzmenü
**Einkauf > Wareneingang > Automatischer Wareneingang > <F4>**

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Markieren (nach unten) (Shift+F9) | Aktiviert die Checkboxen Er. (Erzeugen), für die ausgewählte und alle nachfolgenden Bestellungen. |
| b | Markieren (alle) (Strg+F9) | Aktiviert die Checkbox Er. (Erzeugen) für alle Bestellungen. |
| c | Werte importieren (Strg+F8) | Öffnet einen Dialog zur Angabe eines Zeitraums und importiert alle nicht gebuchten Bestellungen mit einem Liefertermin innerhalb des gewählten Zeitraums. In der Trefferliste werden auch zukünftige Lieferungen angezeigt. |
| d | Lieferantenbewertung (Strg+N) | Dieses Menüpunktes wird zur Zeit nicht unterstützt. |
| e | Wareneingangskontrolle (Shift+F10) | Nach der erfolgreichen Kontrolle des Wareneingangs, kann durch den Aufruf dieses Menüpunktes bzw. der Tastenkombination die Checkbox Ko gesetzt werden. |
| f | Kontrollstatus ab akt. Satz (Shift+F11) | Aktiviert die Checkboxen Ko. (Kontrolle), für die ausgewählte und alle nachfolgenden Bestellungen. |
| g | Kontrollstatus alle Sätze (Strg+F11) | Aktiviert die Checkbox Ko. (Kontrolle) für alle Bestellungen. |
| h | Gestellverwaltung (Strg+G) | Öffnet den Dialog Buchung Gestelle. ⇨ "Gestellbezogener Wareneingang" auf Seite E-1650 |
| i | Bemerkung (Strg+B) | Zeigt die Spalte Bemerkung an, in der Sie zusätzliche Informationen zur Bestellung angeben können. |

## Suchfunktionen

Sie können im Modul Einkauf über unterschiedliche Kriterien nach Vorgängen, Marktpartnern, Adressen, Artikeln und Objekten suchen.

Die Suchdialoge sind für alle Vorgangsarten im Einkauf gleich aufgebaut. Die Bedienung in den Suchdialogen ist analog dem Verkauf entwickelt worden. Die Suchfunktionen werden in dieser Anleitung am Beispiel Bestellungen beschrieben. Abweichungen zu anderen Dialogen, sowie zum Verkauf sind explizit genannt.

In diesem Abschnitt sind folgende Dialoge erklärt:
*   "Suche Bestellungen" auf Seite E-1547
*   "Suche Bestellungen - Trefferliste" auf Seite E-1552

Weitere Suchdialoge sind im Einkauf und Verkauf gleich. Sie sind ausführlich zum Part Verkauf beschrieben:
*   Verkauf, "Suche Bezugsvorgang" auf Seite D-1097
*   Verkauf, "Marktpartnersuche" auf Seite D-1091
*   ⇨ Verkauf, "Adressen Suche" auf Seite D-1099
*   Verkauf, "Artikel-Suche" auf Seite D-1101
*   ⇨ Verkauf, "Artikel-Suche nach Typen" auf Seite D-1110
*   Verkauf, "Produktsuche nach Elementen" auf Seite D-1111
*   ⇨ Verkauf, "Objekt-Suche" auf Seite D-1118

### Suche Bestellungen
**Einkauf > Anfragen > <F9> > Suchkriterien eingeben > <F3>**
In diesem Dialog suchen Sie nach Bestellungen.

Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt.
*   Mit **<F2>** wechseln Sie die Register im Kopfbereich.
*   Mit **<F3>** starten Sie die Suche.
*   Mit **<F2>** wechseln Sie die Register in der Trefferliste.

In diesem Dialog finden Sie im Kopfbereich folgende Register:
*   "Suche Bestellungen - Vorgangs-Schlüssel" auf Seite E-1548
*   "Suche Bestellungen – Positions-Schlüssel" auf Seite E-1550
*   "Suche Bestellungen - Direkte Suche" auf Seite E-1551

Die Ergebnisse der Suche werden in der Trefferliste angezeigt:
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-1552

#### Suche Bestellungen – Vorgangs-Schlüssel
**Einkauf > Anfragen, Bestellverwaltung > <F9>**
In diesem Register suchen Sie Bestellungen anhand der Lieferdaten.
*   Mit **<F2>** wechseln Sie die Register im Kopfbereich.
*   Mit **<F3>** starten Sie die Suche.

**Vorgangs-Schlüssel**

*   **Bestellungen ab**: Nummer, ab der nach Bestellungen gesucht wird. Der Feldname variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Anfragen ab.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr
*   **Lieferant**: Lieferantennummer. Wenn Sie eine Nummer angeben, wird der Lieferantenname im Klartext angezeigt.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.kunr
*   **Fremd-Nr.**: Externe Nummer des Vorgangs. Als externe Nummer kann eine Nummer oder auch ein freier Text sein. Je nach Konfiguration wird das Feld Fremd-Nr. vom System vorbelegt. Diese Daten sind zum Dialog Bestellerfassung beschrieben: ⇨ "K-Auftrag" auf Seite E-1581. Enthält das Feld alphanumerische Zeichen, so ist für die Suche Groß-/Kleinschreibung zu beachten. Über eine Umgebungsvariable können Sie die Suche jedoch bei nach alphanumerischen Zeichen unabhängig von Groß-/Kleinschreibung aktivieren.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr
*   **Bestelldatum**: Datum, an dem die Bestellung freigeschaltet wurde.
    *   Technische Info: Datumsfeld, DB-Feld: kauf.bdat
*   **Hausnummer**: Nummer des Hauses. Standardmäßig ist die eigene Hausnummer ausgewählt. Das Feld kann nur bearbeitet werden, wenn Sie mit der internen Mandantentrennung arbeiten.
    *   Technische Info: numerisches Feld, DB-Feld: xhaus.haus
*   **Kunde**: Kundennummer. Wenn Sie eine Nummer angeben, wird der Kundenname im Klartext angezeigt.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.orgkunr, kauf.orgname
*   **Erfassungsdatum**: Datum der Vorgangserfassung.
    *   Technische Info: Datumsfeld, DB-Feld: kauf.edat
*   **Erfasser**: Mitarbeiternummer des Vorgangserfassers. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiter im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.eusr
*   **Rechnungsnummer**: Nummer der Lieferantenrechnung.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.rechnr
*   **USt-Identnr.**: Umsatzsteuer-Identifikationsnummer des Lieferanten.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kaufp.steuernr

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-1552

#### Suche Bestellungen – Positions-Schlüssel
**Einkauf > Bestellverwaltung > <F9> > Register Positions-Schlüssel**
In diesem Register suchen Sie Bestellungen anhand der Positionsdaten.
*   Mit **<F2>** wechseln Sie die Register im Kopfbereich.
*   Mit **<F3>** starten Sie die Suche.

**Positions-Schlüssel**
Sie können die Bestellungen anhand der Daten aus den Positionen suchen. Geben Sie für diese Suche die bekannte Werte ein. Folgende Felder steht zur Eingabe zur Verfügung:

*   **AB Lief.**: Nummer der Auftragsbestätigung vom Lieferanten.
    *   Technische Info: numerisches Feld, DB-Feld: bpos.abnr
*   **LS-Nr.**: Lieferscheinnummer des Lieferanten.
    *   Technische Info: numerisches Feld, DB-Feld: bpos.lieferschein
*   **Bemerk**: Textfeld für eine positionsbezogene Bemerkung, die im Dialog Lieferanten-Anfragen > Register AuftragsInfo > Feld Bemerkung positionsbezogen hinterlegt wird.
    *   Technische Info: alphanumerisches Feld, DB-Feld: bpos.bemerkung
*   **Auftragsnr.**: Auftragsnummer bei auftragsbezogenen Bestellungen.
    *   Technische Info: numerisches Feld, DB-Feld: bpos.vksuftrnr
*   **Anlieferdatum**: Geplantes Datum der Anlieferung, ab dem nach Bestellungen gesucht wird.
    *   Technische Info: Datumsfeld, DB-Feld: bpos.ltplan
*   **Objekt**: Objektnummer. Wenn Sie eine Nummer angeben, wird der Objektname im Klartext angezeigt.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bpos.vkobjnr
*   **Artikel**: Artikelnummer. Wenn Sie eine Nummer angeben, wird die Artikelbezeichnung im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kpos.artnr
*   **ME**: Mengeneinheit der Position, z. B. Quadratmeter.
    *   Technische Info: numerisches Feld, DB-Feld: kpos.me
*   **Lager**: Lagernummer der Bestellung. Wenn Sie eine Nummer angeben, wird die Lagerbezeichnung im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: bpos.lnr
*   **Maßvariante**: Maßvariante des Artikels.
    *   Technische Info: numerisches Feld, DB-Feld: kpos.var

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-1552

#### Suche Bestellungen – Direkte Suche
**Einkauf > Bestellverwaltung > <F9> > Register Direkte Suche**
In diesem Register suchen Sie Bestellungen ab einer bestimmten Bestellnummer. Mithilfe einer Systemkonfiguration ist es möglich, diesen Register als Startdialog zu konfigurieren, um so eine einfache Suche zu verwenden.
*   Mit **<F2>** wechseln Sie die Register im Kopfbereich.
*   Mit **<F3>** starten Sie die Suche.

*   **Bestellungen ab**: Nummer, ab der nach Bestellungen gesucht wird. Die Feldbezeichnung variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Anfragen ab.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-1552

### Suche Bestellungen - Trefferliste
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3>**
In der Trefferliste finden Sie folgende Register:
*   "Trefferliste - Allgemein" auf Seite E-1553
*   "Trefferliste - Mengen" auf Seite E-1555
*   "Trefferliste - WE-Infos" auf Seite E-1556
*   "Trefferliste - Artikel" auf Seite E-1557
*   "Trefferliste - Verschiedenes" auf Seite E-1558

#### Trefferliste – Allgemein
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Allgemein**
In diesem Register werden allgemeine Informationen zu den Bestellungen angezeigt, die den Suchkriterien entsprechen.
Mit **<F2>** wechseln Sie die Register in der Trefferliste.

> **Satzanzeige**
> Am rechten oberen Dialograhmen wird die Satzanzeige angeboten: z. B.: Vorgangsübersicht: 137:227.
> 137 = die Satznummer der ausgewählten Zeile in der Trefferliste
> 227 = die Anzahl der Sätzen in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben:
⇨ "Suche Bestellungen" auf Seite E-1547

**Register Allgemein**
*   **Haus:** Hausnummer der jeweiligen Bestellung.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
*   **Bestellnr.:** Bestellnummer. Der Spaltenname variiert je nach Vorgang, aus dem Sie die Suche öffnen.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
*   **Subnr.:** Nummer des Teillieferscheins oder der Teilrechnung.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.subnr
*   **Lieferant:** Name des Lieferanten.
    *   Technische Info: Anzeigefeld, DB-Feld: mp.name
*   **USt-Identnr.:** Umsatzsteuer-Identifikationsnummer des Lieferanten.
    *   Technische Info: Anzeigefeld, DB-Feld: kaufp.steuernr
*   **Rechnung:** Nummer der Lieferantenrechnung.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.rechnr
*   **Bestellt:** Datum, an dem die Bestellung freigeschaltet wurde.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.bdat
*   **Erfasst:** Datum der Bestellerfassung.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.edat
*   **Erfasser:** Name des Erfassers.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.eusr
*   **Storniert:** Angabe des Bearbeitungsstands, z. B. Stornostatus.
    *   0: Nicht stornierter Auftrag.
    *   1: Vom Benutzer stornierter Auftrag.
    *   2: Vom System stornierter Auftrag.
    *   -3, -10, -x: Auftrag in Hintergrundbearbeitung.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.still

#### Trefferliste – Mengen
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Mengen**
In diesem Register werden die Positionsinformationen zu den bestellten Artikel und der Menge angezeigt, die den Suchkriterien entsprechen. Pro Artikel-Bestellposition wird eine Zeile angezeigt.
Mit **<F2>** wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben:
⇨ "Suche Bestellungen" auf Seite E-1547

**Register Mengen**
Die Spalten sind zum Register Allgemein beschrieben:
⇨ "Register Allgemein" auf Seite E-1553
Zusätzlich werden folgende Spalten angezeigt:
*   **Pos:** Positionsnummer in der Bestellung.
    *   Technische Info: Anzeigefeld, DB-Feld: kpos.posnr
*   **Artnr., Artikel:** Artikelnummer und Artikelbezeichnung.
    *   Technische Info: Anzeigefelder, DB-Felder: kpos.artnr, kpos.artbez1
*   **Menge:** Bestellte Stückzahl der Position.
    *   Technische Info: Anzeigefeld, DB-Feld: kpos.menge
*   **Eingang:** Eingetroffene Stückzahl der Position im Wareneingang.
    *   Technische Info: Anzeigefeld, DB-Feld: kpos.geslief
*   **Kompl.:** Ein Stern * zeigt an, wenn die Position komplett geliefert ist.
    *   Technische Info: Anzeigefeld
*   **Fakt.:** Fakturierte Stückzahl der Position.
    *   Technische Info: Anzeigefeld, DB-Feld: kpos.gesberech
*   **F:** Ein F zeigt an, wenn die Position komplett fakturiert ist.
    *   Technische Info: Anzeigefeld
*   **Breite, Höhe:** Maße der Position in Millimeter.
    *   Technische Info: Anzeigefelder, DB-Felder: kpos.laenge, kpos.breite

#### Trefferliste – WE-Infos
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register WE-Infos**
In diesem Register werden die Wareneingangs-Informationen zu den Bestellungen angezeigt, die den Suchkriterien entsprechen. Pro Bestellposition wird eine Zeile angezeigt.
Mit **<F2>** wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben:
⇨ "Suche Bestellungen" auf Seite E-1547

**Register WE-Infos**
Die Spalten sind zu den Registern Allgemein und Mengen beschrieben:
⇨ "Trefferliste - Allgemein" auf Seite E-1553
⇨ "Trefferliste - Mengen" auf Seite E-1555
Zusätzlich werden folgende Spalten angezeigt:
*   **Anl.Datum:** Geplantes Datum der Anlieferung, ab dem nach Bestellungen gesucht wird.
    *   Technische Info: Anzeigefeld, DB-Feld: bpos.ltplan
*   **AB-Nr. Lief.:** Nummer der Auftragsbestätigung vom Lieferanten.
    *   Technische Info: Anzeigefeld, DB-Feld: bpos.abnr
*   **Lieferschein:** Lieferscheinnummer des Lieferanten.
    *   Technische Info: Anzeigefeld, DB-Feld: bpos.lieferschein
*   **Auftrag:** Auftragsnummer bei auftragsbezogenen Bestellungen.
    *   Technische Info: Anzeigefeld, DB-Feld: bpos.vksuftrnr
*   **Auslieferung:** Geplantes Lieferdatum des Kundenauftrags.
    *   Technische Info: Anzeigefeld, DB-Feld: bpos.ltplan

#### Trefferliste – Artikel
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Artikel**
In diesem Register werden Informationen zu den Artikeleigenschaften der Bestellpositionen angezeigt. Pro Bestellposition wird eine Zeile angezeigt.
Mit **<F2>** wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben:
⇨ "Suche Bestellungen" auf Seite E-1547

**Register Artikel**
Die Spalten sind zu den Registern Allgemein und Mengen beschrieben:
⇨ "Trefferliste - Allgemein" auf Seite E-1553
⇨ "Trefferliste - Mengen" auf Seite E-1555
Zusätzlich werden folgende Spalten angezeigt:
*   **ME:** Mengeneinheit der Position, z. B. Quadratmeter.
    *   Technische Info: Anzeigefeld, DB-Feld: kpos.me
*   **Maßvariante:** Maßvariante des Artikels.
    *   Technische Info: Anzeigefeld, DB-Feld: kpos.var

#### Trefferliste – Verschiedenes
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Verschiedenes**
In diesem Register werden diverse Informationen zu den Bestellungen angezeigt, die den Suchkriterien entsprechen. Pro Bestellposition wird eine Zeile angezeigt.
Mit **<F2>** wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben:
⇨ "Suche Bestellungen" auf Seite E-1547

**Register Verschiedenes**
Die Spalten sind zu den Registern Mengen und Artikel beschrieben:
⇨ "Trefferliste - Mengen" auf Seite E-1555
⇨ "Trefferliste - Artikel" auf Seite E-1557
Zusätzlich werden folgende Spalten angezeigt:
*   **Lager:** Lagernummer der Bestellung.
    *   Technische Info: Anzeigefeld, DB-Feld: bpos.lnr
*   **Kunde:** Kundenname für auftragsbezogene Bestellungen.
    *   Technische Info: Anzeigefeld, DB-Feld: mp.name

## Bestellpool
Im Bestellpool werden folgende Bestellvorschläge gesammelt, die zu einer oder mehreren Bestellung/-en zusammengefasst werden:
*   Auftragsbezogene Bestellvorschläge aus dem Verkauf.
*   Bestellvorschläge aus dem Lager, z. B. bevor der Lagerbestand in Unterdeckung läuft. Diese Funktion muss konfiguriert sein. Wenn keine automatischen Bestellvorschläge durch das Lager erzeugt werden, können Sie die Lagerbestellungen über den Dialog Bestellerfassung anlegen.

Bestellungen können je nach Systemkonfiguration und festgelegten Lieferanten-Stammdaten 1:1 aus den Auftragsdaten durch den Hintergrundprozess oder manuell im Bestellpool zuerst gruppiert, anschließend erzeugt werden.

Die Bestellfreigabe erfolgt entweder automatisch oder beim Bestelldruck. Folgende Möglichkeiten sind vorhanden:
*   Die Bestellung wird erstellt und automatisch freigeschaltet.
*   Die Bestellung wird gedruckt und automatisch freigeschaltet.
*   Die Bestellung wird über den Dialog Bestellfreischaltung manuell freigeschaltet.

Je nach Systemkonfiguration ist die Bestellfreigabe über den Menüpunkt Bestell-Freigabe möglich:
⇨ "Bestellfreigabe" auf Seite E-1626

Eine weitere Möglichkeit besteht bei entsprechender Systemkonfiguration beim Hinterlegen einer Avise. Sofern die Bestell-Avise gespeichert wird, wird die Bestellung in den Status Bestellt versetzt.
"Lieferavis" auf Seite E-1632

Über den Dialog Formulardruck oder E-Mail können Sie Bestellungen drucken und an den Lieferanten senden. Die Dialoge sind ausführlich zum Part Verkauf beschrieben:
*   Verkauf, "Formulardruck" auf Seite D-1420
*   Verkauf, "E-Mail" auf Seite D-1424

Im Änderungsprotokoll können Sie den Status einer Bestellung prüfen. Der Dialog ist ausführlich zum Part Verkauf beschrieben:
⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-1230

In diesem Abschnitt finden Sie folgende Informationen:
*   "Spezielle Menüs zum Bestellpool" auf Seite E-1561
*   "Bestellfreigabe" auf Seite E-1626
*   "Bestellungen erzeugen" auf Seite E-1563

### Spezielle Menüs zum Bestellpool
Im Bestellpool können dialogspezifische Menüs aufgerufen werden.
*   Mit **<F4>** öffnen Sie das Zusatzmenü zum Bestellpool.
*   Mit **<Shift> + <F4>** öffnen Sie das Infomenü zum Bestellpool.

Die angezeigten Einträge sind von der jeweiligen Konfiguration abhängig. In den folgenden Übersichten der Menüs sind immer alle Einträge aufgeführt.
Folgende Zusatzmenüs stehen zur Verfügung:
*   "Bestellpool - Zusatzmenü" auf Seite E-1561
*   "Bestellpool - Infomenü" auf Seite E-1562

> **Kontext-Menüs**
> In den Kontext-Menüs zu den einzelnen Feldern der Dialog werden jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen sind in folgenden Kapiteln beschriebenen.

#### Bestellpool – Zusatzmenü
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > <F4>**
Meist genutzte Konfiguration

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Markierte Positionen zurückstellen (Shift+F12) | Deaktiviert die Checkbox Er. (Bestellung erzeugen) für die markierten Positionen. Die Positionen können wieder bearbeitet werden. |
| b | Gruppieren nach Markierungen (Strg+F8) | Gruppiert die Positionen unter einer Bestellnummer. Die Checkbox Er. (Bestellung erzeugen) muss aktiv sein. |
| c | Gruppieren nach Aufträgen (Strg+O) | Die Checkbox Er. (Bestellung erzeugen) muss aktiv sein. Positionen mit derselben Auftragsnummer und demselben Lieferanten werden unter einer gemeinsamen Bestellung gruppiert. Für Positionen mit derselben Auftragsnummer aber verschiedenen Lieferanten werden für die Positionen pro Lieferant einzelne Bestellung angelegt. Gruppierung nach Aufträgen ist u. a. konfigurationsabhängig. Bitte kontaktieren Sie einen Service-Mitarbeiter der A+W Software GmbH. |
| d | Nach Bestellungen sortieren (Strg+F12) | Sortiert die Bestellnummern absteigend. |
| e | Bestellkopftext (Strg+K) | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-1313 |
| f | Bestellfußtext (Strg+F) | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-1313 |
| g | Markieren (nach unten) (Shift+F11) | Aktiviert die Checkboxen Er. (Bestellung erzeugen), für die ausgewählte und alle nachfolgenden Positionen. |
| h | Markieren (alle) (Strg+F11) | Aktiviert die Checkbox Er. (Bestellung erzeugen) für alle Positionen. |
| i | Storno | Keine Aktion in dieser Stelle |
| j | Anfrage (Strg+E) | Markiert die Spalte An (Anfrage) der ausgewählten Position mit einem A. Wenn die Checkbox Er. (Bestellung erzeugen) der Position aktiviert ist, können Sie mit <Strg> + <F8> eine Anfrage für den Lieferanten erstellen. |
| k | Alle Anfragen (Strg+L) | Markiert die Spalte An (Anfrage) aller Positionen mit einem A. Wenn die Checkbox Er. (Bestellung erzeugen) der Position aktiviert ist, können Sie mit <Strg> + <F8> eine Anfrage für den Lieferanten erstellen. |
| l | Anfragen ab Cursorposition (Strg+G) | Markiert die Spalte An (Anfrage) mit einem A für die ausgewählte und alle nachfolgenden Positionen. Wenn die Checkbox Er. (Bestellung erzeugen) der Position aktiviert ist, können Sie mit <Strg> + <F8> eine Anfrage für den Lieferanten erstellen. |
| m | Anfragen markieren (Strg+N) | Aktiviert die Checkbox Er. (Bestellung erzeugen) für alle Positionen mit einem A in der Spalte An (Anfrage). |
| n | Noch nicht übertragene Best. | ⇨ "Übersicht zu Vorgängen" auf Seite E-1674 |

#### Bestellpool – Infomenü
**Einkauf > Bestellungen erzeugen > Abteilung angeben> <F3> > <Shift> + <F4>**

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Auftragstexte darstellen (Strg+F10) | ⇨ "Auftragstexte" auf Seite E-1624 |
| b | Einkaufsinfo | In der ausgewählten, zu bestellenden Auftragsposition wird ein Extra-Feld Einkaufsinfo eingeblendet. Sofern solche Information im dazugehörigen Auftrag erfasst wurde, wird dieser Text in dem Feld angezeigt. Eine Neuerfassung der Einkaufsinformation im Bestellpool ist nicht möglich. |
| c | Lieferanten-Anmerkungen | Verkauf, "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-1307 |
| d | Lieferanten-Artikel-Anmerkungen | ⇨ Verkauf, "Marktpartner-Artikel-Anmerkungen" auf Seite D-1310 |
| e | Artikel-Anmerkungen | ⇨ Verkauf, "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-1307 |
| f | Reklamationsinformationen | Zeigt die Reklamationsinformationen für die ausgewählte Position aus dem Auftrag an. ⇨ "Bestellungen erzeugen" auf Seite E-1563 |

### Bestellungen erzeugen
**Einkauf > Bestellungen erzeugen > Abteilung angeben> <F3>**
**Einkauf > Lagerbestellungen erzeugen**
In diesem Dialog können Sie Bestellvorschläge in Bestellungen umwandeln. Je nach Konfiguration des Programms und des gewünschten Ergebnis können Sie aus jeweils einen Bestellvorschlag die Bestellung erzeugen, oder mehrere Bestellungen unter einer Bestellnummer gruppieren.

Bestellvorschläge können auch automatisch erzeugt werden, wenn:
*   der Lieferant für die bestellte Ware aus dem Auftrag in den Stammdaten als Direktlieferant markiert ist.
*   wenn eine Lagerware-Unterdeckung vorliegt. Die Funktion zur automatischen Bestellungen aus dem Lager muss konfiguriert sein. Wenn Bestellvorschläge durch das Lager nicht automatisch erstellt werden können, müssen Sie die Lagerbestellungen über den Dialog Bestellerfassung anlegen.
    ⇨ "Bestellerfassung" auf Seite E-1578

In diesem Dialog finden Sie folgende Register:
*   "Bestellungen erzeugen – Lieferant" auf Seite E-1564
*   "Bestellungen erzeugen – Position" auf Seite E-1568
*   "Bestellungen erzeugen – Details" auf Seite E-1569

#### Bestellungen erzeugen – Lieferant
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > Register Lieferant**
In dem Bestellpool werden alle Bestellvorschläge gesammelt. Beim Arbeiten mit mehreren Einkaufsabteilungen oder/und Häuser können Sie den Auswahldialog konfigurieren, um den Datenbestand zu minimieren und entsprechend zu verteilen. Nach Auswahl des Hauses und/oder Abteilung werden die Bestellvorschläge im Dialog Bestellung erzeugen aufgelistet.

In diesem Register werden die Lieferanteninformationen zu den Bestellungsvorschlägen angezeigt.
Im Dialog Bestellfreigabe können Sie die Bestellungen freischalten.
⇨ "Bestellfreigabe" auf Seite E-1626

**Auswahldialog**
*   **Haus**: Auswahl der Nummer des Mandanten. Dieses Feld ist nur bei internen Mandantentrennung betretbar.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
*   **Abteilung**: Abteilungsnummer. Mit **<F9>** können Sie nach einer Nummer suchen.
    *   Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.abtnr
*   **Zusätzliche Bestellungen**: Bestellnummer. Mit **<F9>** können Sie nach einer Nummer suchen. Mit **<Enter>** können Sie eine weitere Bestellnummer angeben, die in einer neuen Zeile hinzugefügt wird. Sie können die Bestellnummern über die Schaltfläche Zusätzliche Bestellungen auf- oder absteigend sortieren.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr (kauf.vorgang=2)
Mit **<F3>** bestätigen Sie die Auswahl.

**Bestellung erzeugen**
Um die Bestellungen zu erzeugen, müssen folgende Schritte gemacht werden:
*   In dem Feld **Er.** markieren Sie die Bestellvorschläge, für die Sie eine Bestellung erzeugen wollen. Je nach Systemkonfiguration können bei Markierung einer der Bestellposition aus dem Auftrag auch alle weitere Bestellpositionen aus dem selben Auftrag mitmarkiert werden. Die Option *Auftragspositionen zusammenhalten* kann auch beim Markierung-Löschen angewendet werden. Wenn eine verlängerte Werkbank-Bestellung aus dem Bestell-Pool erzeugt werden soll, so werden alle zusammengehörige Bestandteile für eine Auftragsposition und das Datum am Block markiert und so zusammengehalten.
*   Mit **<Strg> + <F8>** gruppieren Sie die Bestellvorschläge und erzeugen Bestellungen. Wenn Sie mehrere Positionen markieren, kann für die Positionen eine oder mehrere Bestellungen erzeugt werden. Die Gruppierung erfolgt entweder nach Markierung, Lieferantenwechsel, oder Aufträge. Die Art die Gruppierung kann über die Systemkonfiguration festgelegt werden.
*   Mit **<Ende>** lösen Sie die Bestellerzeugung aus und speichern die erstellten Bestellungen. Die Bestellungen können im Dialog Bestellverwaltung korrigiert und im Dialog Bestellfreigabe freigegeben werden.

**Gruppierung löschen**
Sie können die gruppierte Position mit bereits vergebenden Bestellnummer wieder zurücksetzen um die Position im Bestellpool zu lassen. Dafür markieren Sie die betroffene Position und entfernen diese einen auftragsbezogenen Bestellvorschlag entfernen, indem Sie die Bestellposition auswählen und über **<F4> > Markierte Positionen zurückstellen** die Bestellnummer für diese Bestellposition löschen.

**Register Lieferant**
*   **Haus**: Nummer des Hauses.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
*   **Best. Nr.**: Bestellnummer, unter der Bestellungen gruppiert werden können. Bestellnummern werden über die Auswahl der Spalte **Er.** vorläufig erstellt oder über die Auswahl der Spalte **S** storniert. Ihre Auswahl können Sie mit **<Ende>** oder **[OK]** bestätigen.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.baufnr
*   **Er.**: Angabe, ob für die Position eine Bestellung erzeugt werden soll. Sie können mehrere Einträge markieren und in einer Bestellung gruppieren.
    *   `☑` Die Position im Bestellpool ist für die Bestellungerzeugung markiert.
    *   `☐` Für diese Position erfolgt keine Bestellungerzeugung.
    *   Mit **<Strg> + <F8>** gruppieren Sie die markierte Position für die Bestellerzeugung. Wenn Sie mehrere Positionen gleichzeitig markieren, wird je nach Systemkonfiguration eine oder mehrere Bestellungen erzeugt.
    *   Technische Info: Checkbox
*   **Auftrag**: Auftragsnummer bei Bestellvorschlägen, die auftragsbezogen ermittelt werden.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.orgauftrnr
*   **Artikel**: Artikelnummer, die bestellt werden soll.
    *   Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: bestpool.artnr
*   **Bezeichnung**: Bezeichnung des Artikels aus der Bestellposition.
    *   Technische Info: alphanumerisches Feld, DB-Feld: bestpool.artbez1
*   **S**: Anzeige, ob die zu bestellende Artikel bereits storniert wurde, z. B. zwischenzeitlich eine Auftragskorrektur vorgenommen wurde. Das Flag wird vom System gesetzt und kann hier nicht geändert werden.
    *   `☑` Die Bestellposition wurde storniert und kann nicht mehr erzeugt werden.
    *   `☐` Die Bestellposition ist nicht storniert und kann weiter bearbeitet werden.
    *   Technische Info: Checkbox, DB-Feld: bestpool.still
*   **Lieferant**: Lieferantennummer für den Artikel. Standardmäßig wird die Nummer des Standardlieferanten für den Artikel aus den Stammdaten angezeigt. Wenn dem Artikel im Kundenauftrag ein abweichender Lieferant zugewiesen wurde, wird die Nummer dieses Lieferanten angezeigt.
    *   Mit **<F10>** öffnen Sie die Marktpartnersuche zur Auswahl eines anderen Lieferanten.
        *   Verkauf, "Marktpartnersuche" auf Seite D-1091
    *   Mit **<F5>** öffnen Sie den Dialog Adressen zur Auswahl einer anderen Adresse.
    *   Mit **<Strg>+<O>** können Sie den neuen Lieferanten als Standardlieferanten für den gewählten Artikel in den Stammdaten hinterlegen.
    *   Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: bestpool.linr
*   **Menge**: Artikelmenge der bestellten Position. Je nach zugeordneter Mengeneinheit des Artikels wird die Menge in dieser Mengeneinheit angezeigt. Bei Lagerbestellungen wird die Bestellmenge aus den Lager-Stammdaten herangezogen. Sie können die Bestellmenge ändern.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.menge
*   **Bestellt zum**: Voraussichtlicher Liefertermin der Bestellung. Der Liefertermin wird aus den Stammdaten berechnet. Sie können das Datum ändern.
    *   Technische Info: Datumsfeld, DB-Feld: bestpool.solldat
*   **Txt.**: Texte. Angabe, ob zu der Bestellposition Texte erfasst sind.
    *   A: Für die Position sind Artikeltexte hinterlegt.
    *   B: Für die Position sind Artikel- und Positionstexte hinterlegt.
    *   P: Für die Position sind Positionstexte hinterlegt.
    *   Mit **<Shift> + <F4> > Auftragstexte darstellen** können Sie sich die hinterlegten Informationen anzeigen lassen.
        ⇨ "Auftragstexte" auf Seite E-1624
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.arttxtnr und bestpool.poskotxtnr
*   **Ei.**: Einkaufsinformation. Anzeige, ob für die Bestellposition eine Fremdinformation im Kundenauftrag hinterlegt ist. Wenn eine Einkaufsinformation hinterlegt ist, wird in dem Feld ein / angezeigt.
    *   Mit **<Shift> + <F4> > Einkaufsinfo** werden die hinterlegten Informationen angezeigt.
    *   Technische Info: Anzeigefeld
*   **Re.**: Reklamation. Anzeige, ob die Bestellung wegen einer Kundenreklamation angelegt wurde.
    *   `☑` Die Position wird wegen einer Kundenreklamation neu bestellt.
    *   `☐` Die Position ist nicht Teil eines Reklamationsauftrags.
    *   Technische Info: Checkbox
*   **An.**: Anfrage. Angabe, ob eine Anfrage an den Lieferanten erstellt wird. Wenn eine Lieferantenanfrage erstellt wird, wird in dem Feld ein A angezeigt. Über das Zusatzmenü können Sie angeben, für welche Bestellpositionen eine Lieferantenanfrage erstellt werden soll.
    *   Technische Info: Anzeigefeld
*   **In.**: Infoanzeige. Das Feld wird zurzeit nicht genutzt.
    *   Technische Info: Anzeigefeld
*   **NB**: Nachbestellung. Anzeige, ob eine zu Bruch gegangenen Position nachbestellt werden muss.
    *   Technische Info: Anzeigefeld

**Fußbereich**
*   **Lieferant**: Name des Lieferanten der gewählten Position.
    *   Technische Info: Anzeigefeld
*   **[Gruppieren]**: Diese Schaltfläche gruppiert aus der markierten Bestellvorschlägen eine oder mehrere Bestellung/-en.
*   **[Auslösen]**: Löst die jeweilige Funktion aus, d. h. die gruppierte Bestellvorschläge werden zu den Bestellungen umgewandelt und im System unter den vorgegeben Nummer gespeichert. Die Schaltfläche wird nur angezeigt, wenn die Gruppierung bereits erfolgte.

#### Bestellungen erzeugen – Position
**Einkauf > Bestellungen erzeugen > Abteilung angeben> <F3> > Register Position**
In diesem Register werden die Positionsinformationen zu den zu bestellenden Artikeln angezeigt.

**Register Position**
Die Felder sind zum Dialog Bestellung erzeugen beschrieben:
⇨ "Bestellungen erzeugen - Lieferant" auf Seite E-1564
Zusätzlich werden folgende Felder angezeigt:
*   **Pos**: Positionsnummer bei Bestellpositionen aus Kundenaufträgen.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.orglfdpos
*   **Lager**: Lagernummer für die Bestellung bei Lagerartikeln. Sie können die Lagernummer ändern.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.lnr
*   **Breite, Höhe**: Maße der Position in Millimeter. Sie können die Maßangaben ändern. Wenn in der Bestellposition ein Variantenartikel erfasst ist, können Sie mit **<F9>** eine andere Maßvariante wählen oder den Variantenbezug entfernen und frei gewählte Maße angeben.
    *   Technische Info: numerische Felder, DB-Felder: bestpool.laenge, bestpool.breite
*   **St**: Angabe, ob Artikel in der Bestellposition kein Positionsartikel, sondern eine Unterteil aus einer Stückliste ist. Wenn der Artikel ein Stücklistenunterteil ist, wird ein Stern * in dem Feld angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.orglfdpos

**Fußbereich**
Die Felder und Schaltflächen im Fußbereich sind zum Register Bestellung erzeugen - Lieferant beschrieben:
⇨ "Bestellungen erzeugen - Lieferant" auf Seite E-1564

#### Bestellungen erzeugen – Details
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > Register Details**
In diesem Register werden die detaillierte Information zu den zu bestellenden Artikeln angezeigt. Sie können Positionsdaten beim Bedarf ergänzen.

**Register Details**
*   **Haus**: Hausnummer, für welches die Bestellungen ausgelöst werden.
    *   Technische Info: Anzeigefeld, DB-Feld: bestpool.hausnr
*   **Bestellung**: Bestellnummer und Positionsnummer in der Bestellung.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.baufnr, bestpool.orglfdpos
*   **Auftrag**: Auftragsnummer, Positionsnummer und Tupelnummer für die bestellte Auftrags-Unterteile, für die der Bestellvorschlag entsteht.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.orgauftrnr, bestpool.orglfdpos, bestpool.orgtnr
*   **Kunde**: Nummer und Name des Kunden bei Bestellpositionen aus Kundenaufträgen.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.kunr, mp.name
*   **Erfasser**: Name des Auftragserfasser bei Bestellpositionen aus Kundenaufträgen.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.eusr
*   **Objekt**: Nummer und Bezeichnung des Objekts bei Bestellpositionen aus Kundenaufträgen.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.objnr, mp.name
*   **Einkaufsinfo**: Fremdinformation zum Einkauf bei Bestellpositionen aus Kundenaufträgen. Das Feld wird nur dann eingeblendet, wenn eine Einkaufinfo in dem Auftrag hinterlegt wurde.
    *   Technische Info: Anzeigefelder, DB-Felder: kauf.exbez1
*   **(ohne Bezeichnung)**: Nummer für diverse Adresse, falls diese als Lieferadresse erfasst wurde.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bestpool.divadrnr
*   **Lager**: Nummer und Bezeichnung des Lagers bei Lagerartikeln. Sie können das Lager ändern.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bestpool.lnr
*   **Artikel**: Nummer und Bezeichnung des Artikels.
    *   Technische Info: Pflichtfeld, numerisches Feld, Anzeigefeld, DB-Felder: bestpool.artnr, bestpool.artbez1
*   **Modell**: Modellnummer bei Bestellpositionen mit Scheibenmodell.
    *   Technische Info: Anzeigefeld, DB-Feld: bestpool.modnr
*   **Lieferant**: Nummer und Name des Lieferanten. Sie können den Lieferanten ändern.
    *   Mit **<F9>** können Sie den Lieferanten aus den Lieferanten wählen, die für den Artikel in den Stammdaten hinterlegt sind.
    *   Mit **<F10>** öffnen Sie den Dialog Marktpartnersuche zur freien Auswahl eines anderen Lieferanten.
    *   Mit **<Strg> + <O>** hinterlegen Sie den gewählten Marktpartner als Standardlieferant für den aktuellen Artikel in die Stammdaten.
    *   Mit **<F5>** können Sie die Lieferadresse ändern. Standardmäßig ist die Hauptlieferadresse des Lieferanten gewählt.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bestpool.linr, mp.name
*   **Fax**: Faxnummer des Lieferanten aus den Stammdaten.
    *   Technische Info: Anzeigefeld, DB-Feld: bestpool.faxnr
*   **Bestellnr**: Lieferantenseitige Nummer und Bezeichnung des Artikels, wenn für den Artikel in den Stammdaten eine lieferantenspezifische Artikelnummer hinterlegt ist.
    *   Technische Info: alphanumerisches Feld, Anzeigefeld, DB-Felder: bestpool.exartnr, bestpool.exartbez
*   **Menge**: Bestellmenge der bestellten Position in den im Stammdaten hinterlegten Mengeneinheit des Artikels. Sie können die Bestellmenge ändern.
    *   Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: bestpool.menge
*   **ME**: Mengeneinheit. Bei Längen-, Zeit- und Stückartikeln wird in diesem Feld die jeweilige Maßeinheit angezeigt, z. B. Meter, Liter.
    *   Technische Info: Anzeigefeld, DB-Feld: bestpool.me
*   **Breite, Höhe**: Maße der Position in den im Stammdaten hinterlegten Mengeneinheit des Artikels. Sie können die Maßangaben ändern. Wenn in der Bestellposition ein Variantenartikel erfasst ist, können Sie mit **<F9>** eine andere Maßvariante wählen oder den Variantenbezug entfernen und frei gewählte Maße angeben. Bei Bestellvorschlägen aus dem Lager werden hier die Maßangaben der Bestellvariante herangezogen. Bei fehlenden Eingaben wird diese Information beim Betreten der betroffenen Position zwingend benötigt.
    *   Technische Info: numerische Felder, DB-Felder: bestpool.laenge, bestpool.breite
*   **SZR**: Breite des Scheibenzwischenraums in entsprechenden Maßeinheiten. Sie können den Scheibenzwischenraum ändern. Der Scheibenzwischenraum wird nur angezeigt, wenn in der Bestellposition ein ISO-Artikel erfasst ist.
    *   Technische Info: numerisches Feld, DB-Feld: bestpool.szr
*   **Variante**: Variantenummer und Variantenbezeichnung des Artikels. Sie können die Variante ändern. Wenn Sie eine andere Maßvariante wählen, werden die Felder **Breite** und **Höhe** automatisch angepasst.
    *   Technische Info: alphanumerisches Feld, numerisches Feld, DB-Felder: bestpool.bitnr, bestpool.varart
*   **Kundenanfahrt**: Auslieferungstermin an den Kunden.
    *   Technische Info: Anzeigefeld, DB-Feld: bestpool.liefdat
*   **Bestellt zum**: Voraussichtlicher Liefertermin der Bestellung. Der Liefertermin wird aus den Stammdaten berechnet. Sie können das Datum ändern.
    *   Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: bestpool.solldat
*   **Bestellt am**: Datum der Bestellerfassung.
    *   Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: bestpool.bestdat
*   **Eigenwähr.**: Stückpreis und Positionspreis in Eigenwährung, z. B. Euro.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.nstpreis, bestpool.npospreis
*   **Fremdwähr.**: Stückpreis und Positionspreis in Fremdwährung, z. B. Dollar.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.fnstpreis, bestpool.fnstpreis
*   **Währung, Kurs**: Nummer und Name der Währung und Währungskurs, z. B. Kurs bei Umrechnung von Euro in Dollar.
    *   Technische Info: Anzeigefelder, DB-Felder: bestpool.waehrung, waehrung.kurzbez, bestpool.kurs
*   **Kostenstelle**: Bezeichnung der Kostenstelle für statistische Auswertungen bei Bestellpositionen aus Kundenaufträgen.
    *   Technische Info: Anzeigefeld, DB-Feld: bestpool.kostenst
*   **Lieferart**: Gewünschte Art der Lieferung:
    *   **Abholung:** Der Kunde holt die Ware selbst ab.
    *   **Streckengeschäft:** Die Ware wird vom beauftragten Produktionsbetrieb direkt an den Endkunden ausgeliefert.
    *   **keine Auswahl:** Die Ware wird über die Route geliefert, die in dem Kundenauftrag erfasst ist.
    *   Technische Info: Toggle-Feld, DB-Feld: bestpool.geschart
*   **Bruchort**: Nummer und Bezeichnung des Bruchortes, an dem der Glasbruch entstanden ist. Die Nummer kann angegeben werden, wenn eine Position wegen Glasbruchs neu bestellt werden muss. In den Regeln wird der Bruchort aus der Produktion übermittelt und in dieses Feld übernommen. Beim Bedarf können Sie den Bruchort in A+W Enterprise ändern. Die Bruchort-Bezeichnung wird im Folgefeld im Klartext angezeigt. Die Bruchorten werden in der Datenbank-Tabelle xbruchort gespeichert. Die Werte werden aus der Produktion automatisch übernommen. Für diese Tabelle existiert kein Pflegedialog in A+W Enterprise.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bestpool.bruchort
*   **Bruchgrund**: Nummer und Bezeichnung des Bruchgrundes. Die Nummer muss nur angegeben werden, wenn eine Position wegen Glasbruchs neu bestellt werden muss. Sie können den Bruchgrund ändern. Wenn Sie eine Nummer angeben, wird der Bruchgrund im Klartext angezeigt.
    *   Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bestpool.bruch

**Summen**
Summe des Positionswerts für Gewicht in Kilogramm, Fläche in Quadratmeter und Länge in Laufmeter.
*   Technische Info: Anzeigefelder

**Position**
Die Anzeige Position gibt an, dass angezeigte Summen pro Position gelten.
*   Technische Info: Anzeigefeld

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Bestellung erzeugen – Lieferant beschrieben:
⇨ "Bestellungen erzeugen - Lieferant" auf Seite E-1564

## Vorgangsverwaltung

Zu den Vorgängen, die Sie im Bereich Einkauf bearbeiten, gehören Lieferanten-Anfragen, Bestellungen, Wareneingänge, Lieferanten-Rechnungen und Gutschriften. Die Dialogen sind vorwiegend gleich zum Bereich Verkauf aufgebaut und benutzbar.
Zu der Vorgangsverwaltung gehören folgende Kapiteln:
*   "Symbolerklärung" auf Seite E-1574
*   "Lieferanten-Anfragen" auf Seite E-1577
*   "Bestellerfassung" auf Seite E-1578
*   "Bestellpositionen" auf Seite E-1598
*   "Abholadresse" auf Seite E-1620
*   "Bestellarten" auf Seite E-1622
*   "Dokumentenartenzuordnung" auf Seite E-1623

### Symbolerklärung

In diesem Abschnitt werden die Kennzeichen für den Dialogmodus, den Positionsstatus und das Positionskennzeichen beschrieben.

**Dialogmodus**
Der Dialogmodus wird in der Titelzeile des Dialogs angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| `+` | Dialog mit Kreuzchen | In diesem Modus können Sie neue Datensätze anlegen. |
| `✎` | Dialog mit Stift | In diesem Modus können Sie einen Vorgang bearbeiten. |
| `⚠` | Gelbes Dreieck mit Ausrufezeichen | In diesem Modus können Sie den Vorgang nicht bearbeiten. |
| `🔍` | Suche | In diesem Modus können Sie nach Vorgängen suchen. |

**Positionsstatus und Positionszeichen**
Der Positionsstatus wird im Register Positionen vor der Spalte Pos angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| 🟢 | grün | Die Position kann frei geändert werden, da die Bestellung noch nicht freigegeben ist. |
| 🟡 | gelb | Die Position oder Unterteile der Position sind bestellt und die Bestellung ist gedruckt worden. |
| 🔴 | rot | Die Position ist in der Bestellung freigegeben. Sie kann nicht mehr geändert werden. |
| 🔴/🔴🔵 | rot/rotblau | Die Position ist teilweise geliefert. |
| 🔴/🔵 | rot/blau | Die Position ist komplett geliefert. |
| 🔴🔵/🔵 | rotblau/blau | Die Position ist teilfakturiert. |
| 🔵 | blau | Die Position ist komplett fakturiert. |

Das Positionskennzeichen wird vor der Spalte Pos angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| ⭐ (Gelber Stern) | Gelber Stern | Die Produktbemaßung sowie zusätzliche Bearbeitungen des Artikels sind für den ausgewählten Lieferanten hinterlegt. Nach dem Speichern des lieferantenindividuellen Artikels wird ein grüner Stern angezeigt. ⇨ Verkauf: Help Cards, "Artikel fixieren" auf Seite D-29 |
| ⭐ (Grüner Stern) | Grüner Stern | Der Artikel ist lieferantenindividuell definiert und kann nur für den jeweiligen Lieferanten erfasst werden. In einem lieferantenindividuellen Artikel können Sie den Stücklistenaufbau mit zusätzlichen Bearbeitungen, Artikeln, Maßänderungen und weiteren lieferantenspezifischen Wünschen speichern. ⇨ Verkauf, "Artikelangaben für bemaßte Varianten" auf Seite D-1217 |
|  মডেল | Scheibenmodell | Die Position ist mit Modell erfasst. ⇨ Verkauf, "Modell-Maßangaben" auf Seite D-1234 |
| 🪟 | Fenster mit Sprossen | Die Position ist mit Sprossen erfasst. ⇨ Verkauf, "Sprossenerfassung" auf Seite D-1284 |

**Statusanzeige in Textform**
Der Status in Textform wird in der Dialogzeile oder im Register Allgemein über der Spalte B.Art angezeigt, wenn sich der Positionsstatus ändert. Folgende Statusanzeigen sind möglich:

| Status in Textform | Bedeutung |
| :--- | :--- |
| Lagerabgang | Für die Position wurde ein Lagerabgang gebucht. |
| Teil-Bestellt | Für die Position existiert eine Teilbestellung, z. B. für einen Artikel aus der Stückliste. |
| Storno | Die Bestellung ist storniert. |
| Fakturiert | Die Bestellung ist fakturiert und kann nicht geändert werden. Rechts neben der Anzeige Fakturiert steht die Nummer der Lieferantenrechnung. |
| Versandplanung liegt vor | Die Bestellung ist im Versand verplant. Kaufmännische Änderungen, wie z. B. Preisänderungen, sind unter Umständen noch möglich. |
| Globalkorrektur | Änderung in der Bestellung werden nicht mehr an die Datenbank übergeben. Kaufmännische Änderungen, wie z. B. Preisänderungen, sind unter Umständen noch möglich. |
| Lokalkorrektur | Änderungen in der Position werden in der Bestellerfassung nicht mehr an das System übergeben, soweit sie die Bestellung betreffen, z. B. Maßänderungen. Kaufmännische Änderungen, wie z. B. Preisänderungen, sind unter Umständen noch möglich. |

### Lieferanten-Anfragen
**Einkauf > Anfragen**
In diesem Dialog erstellen und bearbeiten Sie Anfragen an Lieferanten.
Wenn Sie in der Anfrage einen Liefertermin eintragen, können Sie einen Wiedervorlage-Termin anlegen, um die Anfrage nachzuverfolgen. Wenn der Wiedervorlage-Termin erreicht ist, wird beim Programmstart eine Meldung angezeigt.
Die Wiedervorlage ist ausführlich im Part Verkauf beschrieben:
⇨ Verkauf, "Wiedervorlage" auf Seite D-1463
Jede Anfrage kann in eine Bestellung umgewandelt werden.
Der Dialog ist wie der Dialog Bestellerfassung aufgebaut. Abweichungen werden explizit zum Dialog Bestellerfassung beschrieben:
⇨ "Bestellerfassung" auf Seite E-1578

### Bestellerfassung
**Einkauf > Bestellverwaltung**
In diesem Dialog erfassen und bearbeiten Sie Bestellungen.
Für die reguläre Erzeugung von Bestellungen verwenden Sie in der Regel den Dialog Bestellungen erzeugen. Anschließend können Sie im Dialog Bestellverwaltung die erzeugte Bestellungen ansehen ggf. ändern.
⇨ "Bestellungen erzeugen" auf Seite E-1563

In diesem Dialog finden Sie im Kopfbereich folgende Register:
*   "Bestellerfassung – Kopf, Fuß" auf Seite E-1578
*   "Bestellerfassung - Anschriften" auf Seite E-1585
*   "Bestellerfassung - Eigenschaften" auf Seite E-1587
*   "Bestellerfassung - Verschiedenes" auf Seite E-1592

Im Register Positionen finden Sie folgende Register:
*   "Bestellpositionen - Allgemein" auf Seite E-1599
*   "Bestellpositionen – Eigenschaften" auf Seite E-1608
*   "Bestellpositionen – Preise" auf Seite E-1612
*   "Bestellpositionen - AuftragsInfo" auf Seite E-1615
*   "Bestellpositionen - Status" auf Seite E-1617
*   "Bestellpositionen – Bewertung" auf Seite E-1619

#### Bestellerfassung – Kopf, Fuß
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen**
In diesem Dialog geben Sie die Lieferantendaten an und erfassen die Bestellpositionen. Wenn Sie Positionen erfassen, genügt es in der Regel, die Daten im Register Allgemein zu erfassen.
*   Mit **<Enter>** wechseln Sie in das nächste Feld, mit **<Bild hoch>** wechseln Sie zur ersten Position, mit **<Bild runter>** zur letzten Position.
*   Mit **<Ende>** wechseln Sie in den Fußbereich und schließen die Bestellverwaltung ab.
*   Mit **<F2>** wechseln Sie aus dem Feld Objekt in die Register Anschriften, Eigenschaften oder Verschiedenes.

**Kopfbereich**
*   Mit **<Strg> + <F12>** wechseln Sie aus den Feldern Eingang, Rechnungstyp oder Objekt in den Dialog Bestellart.
    *   "Bestellarten" auf Seite E-1622
*   Mit **<F2>** wechseln Sie aus den Felder Eingang, Rechnungstyp oder Objekt in den Positionsbereich.

> **Bestellungen auflisten**
> Wenn Sie den Dialog Bestellerfassung öffnen, können Sie mit **<F5>** ins Feld K-Auftrag wechseln und durch die Auftragsnummer-Eingabe nach dazugehörigen Bestellungen suchen. Alternativ können Sie mithilfe **<F9>** alle vorhandene Bestellungen auflisten und anschließend auswählen.

*   **Bestell.**: Bestellnummer.
    *   Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr (kauf.vorgang=2)
*   **Lieferant**: Lieferantennummer. Wenn Sie eine Nummer angeben, werden Name und Ort des Lieferanten im Klartext angezeigt.
    *   Technische Info: Pflichtfeld, numerisches Feld, Anzeigefelder, DB-Feld: kauf.kunr, kauf.orgname
*   **Grund**: Begründung für eine Terminänderung. Das Feld Grund wird nur angezeigt, wenn Sie den Liefertermin in einer früher erfassten Bestellung ändern.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kaufltedit.text
*   **Bezug**: Vorgangsnummer, auf die Bezug genommen wird.

**Vorgangsart für den Bezug auswählen**
Je nach Systemkonfiguration ist es möglich, eine der Vorgangsarten als Vorauswahl für die Bezugserfassung festzulegen:
*   Mit **<F8>** wird im Feld **Bezug** die als Standard konfigurierte Vorgangsart im Feld angezeigt.
*   Mit **<F9>** öffnen Sie einen Auswahldialog mit allen Vorgangsarten, auf die Bezug genommen werden kann. Mit den Pfeiltasten können Sie eine Vorgangsart wählen.
*   Mit **<Enter>** bestätigen Sie die Auswahl.
*   Im Feld **Bezug** wird die Nummer des aktuellen Marktpartners angezeigt.
*   Wenn Sie den aktuellen Marktpartner als Vorauswahl festlegen möchten, dann bestätigen Sie mit **<Enter>**.
*   Wenn Sie einen anderen Marktpartner als Vorauswahl festlegen möchten, dann öffnen Sie mit **<F9>** den Dialog Marktpartnersuche, um einen Marktpartner auszuwählen. Alternativ können Sie die Marktpartnernummer direkt im Feld angeben. Mit **<Enter>** bestätigen Sie die Auswahl.
*   Das Feld **Bezug** ist leer. Wenn Sie jetzt den Dialog Suche Bezugsvorgang öffnen, dann sind die Vorgangsart und der Marktpartner, den Sie festgelegt haben, als Suchkriterien vorausgewählt.

**Vorgang mit Bezug erfassen**
*   Mit **<F9>** öffnen Sie den Dialog Suche Bezugsvorgang, um einen Bezugsvorgang zu den angegebenen Kriterien auszuwählen. Alternativ können Sie die Vorgangsnummer direkt im Feld angeben.
*   Mit **<Enter>** bestätigen Sie die Auswahl. Sie können alle Daten des Bezugsvorgangs oder nur die Kopfdaten des Bezugsvorgangs übernehmen. Sie können alle Daten des Bezugsvorgangs oder nur die Kopfdaten des Bezugsvorgangs übernehmen. Diese Entscheidung wird über die Bestätigung entsprechenden Ja/Nein-Meldung durchgeführt.
*   Mit **<F9>** öffnen Sie den Dialog Suche Bezugsvorgang. Der Dialog ist ausführlich zum Part Verkauf beschrieben:
    *   Verkauf, "Suche Bezugsvorgang" auf Seite D-1097
*   Technische Info: numerisches Feld, DB-Feld: kauf.referenz

> **Bezugnahme auf Auftrag**
> Wenn Sie in der Bestellung Bezug auf einen Auftrag nehmen, dann werden alle Auftragspositionen in die Bestellerfassung geladen. Gegebenenfalls müssen Positionen im Register Allgemein gelöscht oder angepasst werden.

*   **Haus**: Hausnummer, in dem die Bestellung erfasst wird. Wenn Sie mit interner Mandantentrennung arbeiten, wird das Feld Haus freigeschaltet. Wenn Sie zusätzlich mit der Haus-Firmenzuordnung arbeiten, wird im ersten Feld die Firmennummer, zu der das Haus zugeordnet ist, aus den Systemstammdaten herangezogen.
    *   Technische Info: numerische Felder, DB-Felder: kauf.company, kauf.hausnr
*   **Erf. Datum**: Erfassungsdatum. Standardmäßig ist das Feld mit dem aktuellen Datum vorbelegt. Der Eintrag kann überschrieben werden.
    *   Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat
*   **K-Auftrag**: Kunden-Auftragsnummer aus dem Verkauf bei auftragsbezogenen Bestellungen. Je nach Konfiguration können alternative Daten angezeigt werden:
    *   **Knd-Bestnr.:** Externe Kunden-Bestellnummer. Für Aufträge aus einem anderen Haus steht in diesem Feld die Auftragsnummer des sendenden Hauses.
    *   Bei interner DFÜ zwischen zwei Häusern können folgende Daten auch in Kombination angezeigt werden:
        *   Bestellnummer vom sendenden Haus.
        *   Auftragsnummer.
        *   Kunden-Bestellnummer.
    *   **Lagerbestellung:** Anzeige, dass eine Lagerbestellung ausgeführt wird.
    *   **Sammelbestellung:** Anzeige, dass auftragsbezogene Bestellpositionen zu einer Sammelbestellung zusammengefasst wurden. Sammelbestellungen können vom Lieferanten als Teillieferungen erfolgen.
    *   Externes Nummernsystem, z. B. lieferantenseitige Angebotsnummer.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr
*   **Termin**: Gewünschter Liefertermin der Bestellung. Im ersten Feld können Sie die Kalenderwoche eingeben. Im zweiten Feld können Sie das Datum im Format TT.MM.JJJJ eingeben.
    *   Technische Info: Pflichtfeld, numerisches Feld, Datumsfeld, DB-Felder: kauf.kwideal, kauf.ltideal
*   **Route**: Routennummer. In der Routenauswahl sind die Fahrtwege sowie die jeweiligen Routentage aufgelistet. Sie können in den Kundenstammdaten eine Hauptroute und drei alternative Routen hinterlegen. Wenn die Via-Plant-Funktion konfiguriert ist, wählen Sie mit **<F5>** das Haus, über das die Auslieferung organisiert werden soll.
    *   Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.routenr
*   **Anlief. Datum**: Anzeige des geplanten Anlieferdatums.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan
*   **Lief-Pos**: Angabe zu Lieferantenpositionen in der Bestellung.
    *   **ja:** Die Positionen können mit lieferantenseitigen Artikelnummern erfasst werden. Wenn Sie lieferantenseitige Artikelnummern den Artikeln in Ihren Stammdaten zugeordnet haben, können Sie über Ihre Stammdaten Artikel auswählen. In der Bestellung werden die lieferantenseitigen Artikelnummern an den Lieferanten übermittelt. Für die Positionserfassung über lieferantenbezogenen Artikeldaten wird im Register Allgemein das Feld Li. Pos aktiviert.
    *   **nein:** Die eigenen Artikelnummern werden erfasst.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.kndposkz
*   **Term. Art**: Information über die Terminierungsart, die auf den Auftrag gedruckt wird.
    *   **Abruf:** Termin auf Abruf.
    *   **eilt:** schnellstmöglich.
    *   **mögl:** möglichst zum Termin.
    *   **verbl:** Termin ist verbindlich.
    *   **ohne:** ohne Terminart.
    *   **Auto:** zurzeit nicht genutzt.
    *   **folgt:** Termin folgt.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.abrufkz
*   **Eingang**: Wird nicht verwendet.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.eingang
*   **Rechnungstyp**: Angabe, für welche Leistungen die Rechnung erstellt wird. In der Regel werden die Gläser und Montageleistungen gemeinsam berechnet. Auf Wunsch können Sie einzelne Rechnungen erstellen.
    *   **Gesamt:** Die Rechnung wird für die komplette Bestellung erstellt, d. h. für Material und Montageleistungen.
    *   **Glas:** Die Rechnung wird nur für das Material der Bestellung erstellt.
    *   **Dienstltg:** Die Rechnung wird nur für die Montageleistung der Bestellung erstellt.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.rechart
*   **Objekt**: Objektnummer. Ein Objekt ist dem Marktpartner zugeordnet und kann z. B. eine Baustelle, die direkt vom Lieferanten beliefert wird, sein und eine andere Lieferadresse haben. Mit dem Objekt können Sie besondere Konditionen verknüpfen, die nur für dieses Objekt gelten, z. B. Rabatte oder Zahlungsoptionen. Sie haben die Möglichkeit objektbezogen abzurechnen.
    *   Mit **<F9>** öffnen Sie die Objekt-Suche. Die Objektsuche ist ausführlich zum Part Verkauf beschrieben:
        ⇨ Verkauf, "Objekt-Suche" auf Seite D-1118
    *   Technische Info: numerisches Feld, DB-Feld: kauf.objnr

**Positionsbereich**
In diesem Bereich werden Informationen zur markierten Position oder Spalte angezeigt. Das Register und die Unterregister sind separat beschrieben:
⇨ "Bestellpositionen" auf Seite E-1598

**Fußbereich**
Im Fußbereich werden die Gesamtbestellwerte für die einzelnen Maßeinheiten und die Gesamtbeträge der Positionen angezeigt. Sie können einen allgemeinen Rabatt gewähren und den Betrag im Feld Nettototal überschreiben, z. B. wenn Sie mit dem Lieferanten eine entsprechende Vereinbarung getroffen haben.
Mit **<F2>** öffnen Sie den Dialog Bestellerfassung für die Berechnung von Rabatten und des Nettototalbetrags.
⇨ "Bestellerfassung - Summen" auf Seite E-1596

*   **Sender**: Anzeige der Haus- und der Referenznummer. Die Referenznummer kann die Angebotsnummer sein oder bei DFÜ-Aufträgen die Auftrags- oder Bestellnummer.
    *   Technische Info: Anzeigefelder, DB-Felder: kauf.hausnr
*   **ST, kg, qm**: Anzeige der Gesamtsumme der Bestellwerte für Anzahl in Stück, Gewicht in Kilogramm und Fläche in Quadratmeter.
    *   Technische Info: Anzeigefelder, DB-Felder: kauf.gesst, kauf.gesm2, kauf.gesgewicht.
*   **Gesamt**: Anzeige des Gesamtpreises aller Positionen abzüglich der Positionsrabatte aus dem Feld Abzg/ im Register Preise. Der Gesamtpreis einer Position ergibt sich aus Positionspreis x Positionsmenge.
    ⇨ "Bestellpositionen – Preise" auf Seite E-1612
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.gesnetto
*   **Rabatt**: Auf den Gesamtbetrag gewährter Rabatt in Prozent. Bei gewährtem Rabatt wird der Betrag im Feld Nettototal angepasst.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.gesfaktor
*   **Nettototal**: Summe aller Positionspreise, inkl. Rabatte und Zuschläge. Eine Bearbeitung des Betrags ist möglich. Die Differenz wird vom System berechnet und im Feld Allg. Abschlag oder Allg. Aufschlag im Berechnungsdialog angezeigt.
    ⇨ "Bestellerfassung - Summen" auf Seite E-1596
    *   Technische Info: numerisches Feld, DB-Feld: kauf.nettototal
*   **+MwSt ()**: Anzeige der Mehrwertsteuer. Im Feld steht der Mehrwertsteuerbetrag, der auf den Nettobetrag aufgeschlagen wird. In den Klammern wird der geltende Mehrwertsteuersatz in Prozent angezeigt.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.mwstbetrag
*   **Brutto**: Anzeige des Brutto-Gesamtbetrags. Der Betrag wird aus dem Nettobetrag zuzüglich der Mehrwertsteuer berechnet.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.gesbrutto
*   **D-Beitrag**: Anzeige des Deckungsbeitrags (Bruttogewinn), den ein Produkt zur Deckung der Fixkosten und zur Erzielung eines Nettogewinns beiträgt. Berücksichtigt werden alle Rabatte und Aufschläge.
    *   Technische Info: Anzeigefeld, DB-Feld: kauf.dbdm

#### Bestellerfassung – Anschriften
**Einkauf > Bestellverwaltung > Bestellung öffnen > Feld Eingang, Rechnungstyp > <F2> > Register Anschriften**
In diesem Register bearbeiten Sie die Lieferanten- und Lieferanschrift. Standardmäßig wird im Bereich Lieferanschrift die Lieferanschrift aus den Lieferantenstammdaten herangezogen. Sie können die Ermittlung der Lieferanschrift kundenspezifisch konfigurieren. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-1578

**Lieferantenanschrift**
*   **Name, Vorname**: Name und Vorname des Lieferanten.
    *   Technische Info: alphanumerische Felder, DB-Felder: kauf.orgname, kauf.orgvorname
*   **Anrede**: Nummer der Anrede. Wenn Sie eine Nummer auswählen, wird die Anrede im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.organrede
*   **Z. Hd.**: Zu Händen. Name der Person, an die die Bestellung ausgehändigt werden soll.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgzhd
*   **Zusatz**: Zusatztext der Anschrift.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgbranche
*   **Straße**: Straßenname und Hausnummer des Lieferanten.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgstr
*   **PLZ, Fach**: Postleitzahl und Nummer des Postfachs.
    *   Technische Info: alphanumerische Felder, DB-Felder: kauf.orgpfplz, kauf.orgpostfach
*   **PF Ort**: Ortsname des Postfachs von Lieferanten außerhalb Europas.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgpfort
*   **PLZ, Ort**: Postleitzahl und Ortsname der Lieferantenanschrift.
    *   Technische Info: alphanumerische Felder, DB-Felder: kauf.orgplz, kauf.orgort
*   **KFZ Land**: Kraftfahrzeug-Kennzeichen des Ziel-Landes. Wenn Sie ein KFZ-Kennzeichen auswählen, wird der Landesname im Klartext angezeigt.
    *   Technische Info: alphanumerische Felder, DB-Felder: kauf.orgkfzcode, kauf.orgland
*   **Tel**: Telefonnummer des Lieferanten.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgtel
*   **Fax**: Faxnummer des Lieferanten.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.faxnr
*   **Sprache**: Nummer der Landessprache des Lieferanten, in der die Dokumente gedruckt werden. Wenn Sie eine Nummer auswählen, wird die Sprache im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.sprkz
*   **Kennz.**: Nummer des Steuerkennzeichens. Das Steuerkennzeichen ist der Steuerschlüssel, mit dem die Mehrwertsteuer berechnet wird. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Steuerkennzeichens im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.kukz

**Lieferanschrift**
Sie können eine abweichende Lieferanschrift eingeben, z. B. bei einer Direktanlieferung die Adresse einer Baustelle.
*   Mit **<Strg> + <N>** legen Sie eine neue Lieferanschrift für den Lieferanten an.
*   Mit **<Strg> + <L>** wählen Sie eine hinterlegte Lieferanschrift des Lieferanten aus.
Die Felder sind zum Bereich Lieferantenanschrift beschrieben:
⇨ "Lieferantenanschrift" auf Seite E-1585
Zusätzlich ist folgendes Feld beschrieben:
*   **Region**: Versandregion. Die Versandregion ist in den Stammdaten hinterlegt und wird über die PLZ ermittelt. Sie ist nur für Aufträge relevant.
    *   Technische Info: Anzeigefeld

**Fußbereich**
Die Felder im Fußbereich können nur im Register Positionen betreten werden. Sie sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-1578

#### Bestellerfassung – Eigenschaften
**Einkauf > Bestellverwaltung > Bestellung öffnen > ab dem Feld Eingang> <F2> > Register Eigenschaften**
In diesem Register bearbeiten Sie die Angaben zur Mitarbeiterzuordnung, den Versandinformationen und den Rechnungs- und Druckoptionen.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-1578

**Mitarbeiterzuordnung**
*   **Bestellt bei**: Mitarbeiternummer des Lieferanten. Wenn Sie eine Nummer auswählen, wird der Name des Mitarbeiters im Klartext angezeigt. Mit **<F5>** öffnen Sie den Dialog Ansprechpartner, in dem Sie einen Ansprechpartner wählen oder neu anlegen können. Der Dialog Ansprechpartner ist ausführlich zum Part Verkauf beschrieben:
    ⇨ Verkauf, "Ansprechpartner" auf Seite D-1199
    *   Technische Info: numerisches Feld, DB-Feld: kauf.busr
*   **Bestelldatum**: Datum der Bestellerfassung.
    *   Technische Info: Datumsfeld, DB-Feld: kauf.bdat
*   **Erfasser**: Anzeige der Nummer und des Namens des Erfassers.
    *   Technische Info: Anzeigefelder, DB-Feld: kauf.esuer
*   **Sachbearbeiter**: Nummer des Sachbearbeiters. Wenn Sie eine Nummer auswählen, wird der Name des Sachbearbeiters im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.abvertr
*   **Außendienst**: Name des Außendienst-Mitarbeiters.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.vertr
*   **Vertr. (Erlös)**: Vertreter-Erlös. Nummer des Vertreters, an den die Provision ausgezahlt wird. Wenn Sie eine Nummer auswählen, wird der Name des Vertreters im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.vertrerloe

**Versandinformationen**
*   **Max. Abladung**: Maximales Gewicht, das der Lieferant mit seinem technischen Gerät abladen kann.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.gmaxgew
*   **Zustellung**: Vermerk über die gewünschte Art der Zustellung. Die Art der Zustellung wird im Bereich Einkauf in der Regeln nicht verwendet.
    *   **Abholung:** Die Ware wird bei Bestellung selbst abgeholt.
    *   **Streckengeschäft:** Die Ware wird vom beauftragten Produktionsbetrieb direkt zu den Endlieferanten ausgeliefert.
    *   **keine Auswahl:** Die Ware wird über die Route eingeliefert, die im Kopfbereich erfasst ist.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.geschart
*   **Direktauslief.**: Angabe, ob der Lieferant direkt von den Produktionsstätten beliefert wird oder ob die Ware ins Handelshaus geliefert wird. Das Kennzeichen wird im Bereich Einkauf nicht verwendet.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.drkliefkz
*   **Lieferart**: Nummer der Lieferart, z. B. frei Haus. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Lieferart im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.lieferart
*   **Versandart**: Nummer der Versandart, z. B. LKW. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Versandart im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.versandart
*   **Verpackungsart**: Nummer der Verpackungsart, z. B. Kiste. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Verpackart im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.verpackart
*   **Gest.-Beladung**: Gestell-Beladung. Sie wählen aus, nach welchen Kriterien die Ware auf den Gestellen sortiert wird:
    *   **Pos:** nach Positionen.
    *   **Größe:** nach Größe.
    *   **SZR+Gr:** nach Scheibenzwischenraum und Größe.
    *   **Pos(frei):** Positionen zusammengehalten aber frei organisiert.
    *   **HM Glas Farb Dick:** nach Hardmaß, Glasmaß, Farbe und Dicke.
    *   **HM Gl.maß Farbe:** nach Hardmaß, Glasmaß und Farbe.
    *   **HM Gl.maß - Dicke:** nach Hardmaß, Glasmaß und Dicke.
    *   **HM - Farbe Dicke:** nach Hardmaß, Farbe und Dicke.
    *   **HM Glasmaß**: nach Hardmaß und Glasmaß.
    *   **HM - Farbe**: nach Hardmaß und Farbe.
    *   **HM - - Dicke:** nach Hardmaß und Dicke.
    *   **HM - - -**: nach Hardmaß.
    *   **Kommission:** nach Kommissionstext.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.gbelad
*   **Ausgangszoll**: Nummer der Ausgangszollstelle für die Lieferpapiere. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Zollstelle im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.azsnr
*   **Bestimmungszoll**: Nummer der Zollstelle des Empfängerlandes. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Zollstelle im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.bzsnr
*   **Fahrtdauer, Entfernung**: Voraussichtliche Fahrzeit und Anzeige der Fahrstrecke. Je nach Konfiguration wird die Fahrzeit in Stunden oder Tagen angegeben. Sie kann sich auf den Liefertermin auswirken. Die Fahrstrecke wird aus dem Feld Entfernung der Lieferadresse herangezogen.
    *   Technische Info: numerische Felder, DB-Felder: kauf.anfahrt

**Rechnungs- und Druckoptionen**
*   **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Lieferanten.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.steuernr
*   **FA-Steuer-Nr.**: Finanzamt-Steuer-Nummer des Lieferanten.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.finstnr
*   **Kostenstelle**: Bezeichnung der Kostenstelle für statistische Auswertungen.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.kostenst

> **Festlegen der Kostenstelle für die gesamte Bestellung**
> Wenn Sie eine Kostenstelle angeben, werden bestellbezogen die positionsgenauen Kostenstellen aus den Stammdaten überschrieben.

*   **Rechnungsart**: Art der Rechnung:
    *   **Einzelrechnung:** Rechnungsempfänger bekommt für jeden Bestellung eine separate Rechnung zugestellt.
    *   **Sammelrechnung:** Der Rechnungsempfänger bekommt mehrere Bestellungen zusammengefasst in einer Rechnung zugestellt. Sie können auswählen, in welchen Intervallen eine Sammelrechnung ausgestellt wird:
        *   wöchentlich
        *   14-tägig
        *   monatlich
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.rechungsart

> **Hinweis zur Sammelrechnungserstellung**
> Das Einverständnis des Rechnungsempfängers zur Sammelrechnung sowie die Festlegung des Sammelrechnungslimits ist in den Marktpartner-Stammdaten hinterlegt.

*   **Teilfaktura**: Angabe, ob Teilabrechnungen nach einer Teillieferung erstellt werden:
    *   **J:** Die Teilabrechnungen zulassen.
    *   **N:** Keine Teilabrechnungen zulassen.
    *   Wenn Sie als Rechnungsart Sammelrechnung wählen und Teilabrechnungen zulassen, werden nach jeder Teillieferung die ausgelieferten Artikel mit der nächsten Sammelrechnung fakturiert.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.teilfakkz
*   **Eilbestellung**: Die aktuelle Bestellung kann bevorzugt und mit höherer Priorität freigegeben werden.
    *   **J:** Die Bestellung mit höherer Priorität freigeben.
    *   **N:** Keine höhere Priorität für die Bestellung vergeben.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.schnellBestellung ist ein Eilauftrag.
*   **Bruttopreise drucken**: Die Bruttopreise können auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden.
    *   **J:** Die Bruttopreise ausweisen und drucken.
    *   N: Keine Bruttopreise ausweisen und drucken.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.preisdrkz
*   **Kundenfaktor drucken**: Der kundenspezifische Faktor kann auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden.
    *   **J:** Den Kundenfaktor ausweisen und drucken.
    *   **N:** Keinen Kundenfaktor ausweisen und drucken.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.rabdrkz
*   **Artikeltexte drucken**: Die Artikeltexte können auf den marktpartnerseitigen Dokumenten gedruckt werden.
    *   **J:** Die Artikeltexte drucken.
    *   **N:** Keine Artikeltexte drucken.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.atxtdrukz
*   **Modelle drucken**: Die Modellskizze der Positionen kann im Anhang der marktpartnerseitigen Dokumente gedruckt werden.
    *   **J:** Die Modellskizze drucken.
    *   **N:** Keine Modellskizze drucken.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.moddrkz
*   **Positionspreise unterdrücken**: Die Positionspreise werden standardmäßig auf den marktpartnerseitigen Dokumenten gedruckt. Sie können die Auflistung der Positionspreise unterdrücken, z. B. wenn mit dem Lieferanten ein Fixpreis für die gesamte Bestellung vereinbart wurde.
    *   **J:** Keine Positionspreise drucken.
    *   **N:** Die Positionspreise drucken.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.posdrkz

**Fußbereich**
Die Felder im Fußbereich können nur im Register Positionen betreten werden. Sie sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung – Kopf, Fuß" auf Seite E-1578

#### Bestellerfassung – Verschiedenes
**Einkauf > Bestellverwaltung > Bestellung öffnen > ab dem Feld Eingang> <F2> > Register Verschiedenes**
In diesem Register werden Reklamationsinformationen, private Felder, weitere technische Informationen und die Zahlungsoptionen angezeigt.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-1578

**Reklamationsinformation**
Mit den Daten können Sie eine Reklamationsstatistik führen. Die Art, der Ort und der Typ der Reklamation müssen in den Stammdaten angelegt sein.
*   **Art**: Nummer der Reklamationsart. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Reklamationsart im Klartext angezeigt, z. B. Glasbruch.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.reklamart
*   **Ort**: Nummer des Reklamationsorts. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Reklamationsorts im Klartext angezeigt, z. B. Entladung.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.reklamort
*   **Typ**: Nummer des Reklamationstyps. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Reklamationstyps im Klartext angezeigt, z. B. falsche Farbe.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.reklamspec
*   **Datum**: Reklamationsdatum im Format TT.MM.JJJJ.
    *   Technische Info: Datumsfeld, DB-Feld: kauf.reklamdat

**Zahlungsoptionen**
Die vom Lieferanten übermittelten Zahlungsoptionen können Sie für die Bestellung einsehen und bei Bedarf bearbeiten. Die Zahlungsoptionen werden aus den Stammdaten ermittelt.
*   **Währung Kurs**: Nummer und Name der Währung und Währungskurs. Der Preis wird kundenbezogen in der angegebenen Währung berechnet. Wenn Sie eine Nummer auswählen, werden Währungsname und Währungskurs im Klartext angezeigt. Das Feld Kurs ist gesperrt, wenn die Eigenwährung gewählt ist.
    *   Technische Info: Pflichtfeld, numerische Felder, DB-Felder: kauf.waehrung, kauf.kurs
*   **Kalkulation in**: Das Feld ist nur freigeschaltet, wenn im Feld Währung nicht die Eigenwährung gewählt ist. Sie können festlegen, ob die Preise in der Eigenwährung oder in der Fremdwährung des Marktpartners berechnet werden:
    *   **Eigenwährung:** Die Preise werden in der Eigenwährung von A+W Enterprise berechnet.
    *   **Fremdwährung:** Die Preise werden in der Währung berechnet, die dem Marktpartner im Feld Währung zugewiesen ist.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.waehrprs
*   **Ausdruck in**: Nummer für den Ausdruck der marktpartnerspezifischen Unterlagen in der kalkulierten Währung oder der Fremdwährung. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Druckoption im Klartext angezeigt. Für den Druck muss der entsprechende Report hinterlegt sein.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.waehrdru

> **Die Felder Kalkulation in und Ausdruck in**
> Die Felder Kalkulation in und Ausdruck in sind nur zugänglich, wenn das Währungs-Modul lizenziert ist.

*   **Zahlziel**: Zahlungsziel in Tagen, das mit dem Marktpartner vereinbart wurde.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.zahlziel
*   **Valuta**: Frist zur Wertstellung in Tagen.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.valuta
*   **Skonto1, Skonto2, Skonto3**: Schlüssel der Skontosätze für das Zahlungsziel. Sie können bis zu 3 verschiedene Schlüssel angeben. Auf diese Weise können Sie gestaffelte Zahlungsziele definieren.
    *   Technische Info: numerische Felder, DB-Felder: kauf.skonto1, kauf.skonto2, kauf.skonto3
*   **Merkmal**: Nummer der Form der Bezahlung, z. B. Banklastschrift, Bankabbuchung. Sie hinterlegen Merkmale in den Systemstammdaten als Zahlungsweisem. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Merkmals im Klartext angezeigt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.zahlngmerk
*   **Zahlungsverkehr**: Art und Weise der Bezahlung, z. B. Vorauskasse, Bankeinzug. Die Angaben zum Zahlungsverkehr sind vom System vorgegeben.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.skontoart
*   **FIBU-Key**: Schlüssel zur Übergabe an die Finanzbuchhaltung. Die Schlüssel der Finanzbuchhaltung werden vom System eingetragen und an die Finanzbuchhaltung gesendet.
    *   Technische Info: alphanumerisches Feld, DB-Feld: kauf.fibukey
*   **FIBU-Debitor**: Lleferantennummer des Marktpartners, der als Rechnungsempfänger bestimmt ist. Das Feld ist standardmäßig vorbelegt.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.stddebnr

**Private Felder**
Die privaten Felder werden kundenspezifisch für Zusatzinformationen genutzt. Sie sind frei konfigurierbar. Die Feldbezeichnungen werden über die Umgebungsvariablen gesetzt. Die beiden oberen Zeilen sind numerische Felder, die beiden unteren Zeilen sind freie Textfelder.
*   Technische Info: numerische Felder, alphanumerische Felder, DB-Felder: kauf.private_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2

**Weitere Optionen**
*   **Kontrolle**: Nummer des Mitarbeiters, der den Vorgang kontrolliert. Wenn das Feld gefüllt ist, werden die Vorgänge erst nach Prüfung durch den entsprechenden Mitarbeiter freigeschaltet.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.kontrollmanr
*   **Windlast**: Windlast am Einbauort. Windlast (N/m²) ist der Druck, der durch direkte Windeinwirkung auf die äußere Oberfläche eines Gebäudes ausgeübt wird. Das System führt mit diesem Wert eine Plausibilitätsprüfung durch, um zu prüfen, ob die Dickengruppe der gewählten Gläser für die angegebene Windlast ausreichend ist. Die Windlast kann nur für Gläser mit mehreren Scheiben angegeben werden.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.wlast

> **Restriktionsprüfung bei Eingabe der Windlast**
> Wenn für die Windlast ein entsprechender Eintrag in den Stammdaten angelegt ist, wird die angegebene Windlast einer Restriktionsprüfung unterzogen. Bei Verletzung der Restriktionsprüfung wird ein Hinweis angezeigt.

*   **Fassadenzone**: Angabe der Fassadenzone, in der die Scheiben verbaut werden. Hohe Gebäude oder Gebäude, die an Randgebieten stehen, werden z. B. mit einer erhöhten Windlast belastet.
    *   **1 Rand:** Für Gebäude mit erhöhter Windlast.
    *   **2 Zentral:** Für Gebäude ohne erhöhte Windlast.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.bereich
*   **Min ISO Ges-Stärke, Max ISO Ges-Stärke**: Minimale und maximale Glasstärke des gesamten ISO-Artikels in Millimeter. Die Glasstärke ist abhängig von der gewählten Fassadenzone und der Windlast.
    *   Technische Info: numerische Felder, DB-Felder: kauf.minszr, kauf.maxszr
*   **Falzmaß**: Korrekturmaß in Millimeter. Das Falzmaß wird auf die Breite und Höhe der Positionen aufgeschlagen. Z. B. werden für ein Glas mit den Maßen 1050 mm x 1250 mm und einem Falzmaß von 2 mm in der Datenbank die Maße 1052 mm x 1252 mm hinterlegt. Der Wert wird an die Produktion übergeben. Wenn Sie mit A+W Production arbeiten, wird dieser Wert in der Regel ignoriert und das Falzmaß aus A+W Production herangezogen.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.falzmass
*   **Angeb. Status**: Status des Angebots. Dieses Feld wird nur bei Angeboten angezeigt. Bei Bezugnahme wird der Feldinhalt übernommen.
    *   **offen:** Das Angebot wurde noch nicht bestätigt.
    *   **gewonnen:** Das Angebot wurde bestätigt.
    *   **verloren:** Das Angebot wurde abgelehnt.
    *   **verjährt:** Das Angebot ist nicht mehr gültig.
    *   Technische Info: Toggle-Feld, DB-Feld: kauf.angbstatus
*   **Textformeln**: Nummer und Bezeichnung der Produktkennzeichnung, z. B. Rahmentext. Die Textformeln müssen in den Stammdaten angelegt sein.
    *   Technische Info: numerisches Feld, DB-Feld: kauf.artkennfrm

**Fußbereich**
Die Felder im Fußbereich können nur im Register Positionen betreten werden. Sie sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung – Kopf, Fuß" auf Seite E-1578

#### Bestellerfassung – Summen
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein > Preisfeld> <Ende> > Feld Nettototal > <F2>**
In diesem Dialog definieren Sie Rabatte, Ab- und Aufschläge für die gesamte Bestellung und bearbeiten verschiedene Zahlungsoptionen.
Rabatte werden mit den Lieferanten vereinbart. In den Stammdaten können Sie einen allgemeingültigen Rabatt hinterlegen und jedem Lieferanten einen lieferantenspezifischen Rabatt zuweisen. Für eine Bestellung mit ausgewähltem Lieferanten wird immer zuerst der lieferantenspezifische Rabatt verrechnet. Wenn für den Lieferanten kein Rabatt hinterlegt ist, wird der allgemeine Rabatt verwendet.
Der Dialog ist ausführlich zum Part Verkauf beschrieben:
⇨ Verkauf, "Auftragserfassung - Summen" auf Seite D-1157

#### Bestellerfassung - Detailansicht Rabatte
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein > Preisfeld > <Ende> > Feld Nettototal > <F2> > <F5> > <F5>**
In diesem Dialog geben Sie Details zum ausgewählten Rabatt an.
Der Dialog ist ausführlich zum Part Verkauf beschrieben:
⇨ Verkauf, "Auftragserfassung - Detailansicht Rabatte" auf Seite D-1162

### Bestellpositionen
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein**
Im Register Positionen finden Sie folgende Register:
*   "Bestellpositionen – Allgemein" auf Seite E-1599
*   "Bestellpositionen - Eigenschaften" auf Seite E-1608
*   "Bestellpositionen – Preise" auf Seite E-1612
*   "Bestellpositionen - AuftragsInfo" auf Seite E-1615
*   "Bestellpositionen - Status" auf Seite E-1617
*   "Bestellpositionen – Bewertung" auf Seite E-1619

Auf der Positionsebene können Sie Modelle, Bearbeitungen, Stufungen und Sprossen neuerfassen bzw. diese Information in den erzeugten Bestellungen ansehen und ändern. Sie können auch die Einkaufspreise zu den Positionen einsehen und anpassen.

Die Dialoge sind ausführlich zum Part Verkauf beschrieben.
*   ⇨ Verkauf, "Sprossenerfassung" auf Seite D-1284
*   ⇨ Verkauf, "Stufenerfassung (relevante Teile)" auf Seite D-1281
*   ⇨ Verkauf, "Stücklistendarstellung" auf Seite D-1252
*   ⇨ Verkauf, "Modell-Maßangaben" auf Seite D-1234
*   ⇨ Verkauf, "Preise und Konditionen" auf Seite D-1322

#### Bestellpositionen – Allgemein
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein**
In diesem Register erfassen und bearbeiten Sie die Positionen einer Bestellung. Sie können die Artikel auswählen, die Maße, Menge und Beschaffungsart bestimmen und den Artikeln Bearbeitungen zuordnen.
Bei einer Statusänderung wird auf der Höhe des Registers ein entsprechender Hinweis zum Status der Bestellung angezeigt. Vor dem Feld Pos werden der Positionsstatus als Ampel und ggf. das Positionskennzeichen angezeigt.
⇨ "Symbolerklärung" auf Seite E-1574
Auftragsbezogene Bestellungen und Lagerbestellungen werden in der Regel über den Dialog Bestellungen erzeugen angelegt und können in der Bestellverwaltung beim Bedarf bearbeitet werden.
⇨ "Bestellungen erzeugen" auf Seite E-1563

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register Bestellerfassung – Kopf, Fuß beschrieben:
⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-1578

**Register Positionen (linker Bereich)**
Im Infobereich werden verschiedene Informationen zur markierten Position angezeigt. Die technischen Werte können bearbeitet werden.
⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" auf Seite E-1602

*   **Kommis**: Kommissionstext für den Druck. Das Feld ist nur betretbar, wenn für den Artikel in den Stammdaten entsprechendes Flag gesetzt ist. Sie können für die erste Position den Kommissionstext direkt eingeben. Wenn Sie eine neue Position erfassen, wird automatisch der Kommissionstext der vorangehenden Position übernommen. Alternativ haben Sie folgende Möglichkeiten:
    *   Mit **<F4> > Kommissionen > neue Kommission** oder **Kommission ändern** legen Sie über das Zusatzmenü einen neuen Kommissionstext an oder bearbeiten einen bestehenden Kommissionstext für die gesamte Bestellung.
    *   Mit **<Shift> + <F11>** wechseln Sie aus der Positionsebene in die Texterfassung der Kommission, um einen Kommissionstext für die ausgewählte Position anzulegen.
    *   Mit **<Enter>** wechseln Sie aus dem Feld Kommis in das Register Allgemein, das sich im Positionsbereich befindet, um die Positionserfassung fortzusetzen.
    *   Technische Info: alphanumerisches Feld, DB-Feld: komm.kommtxt

> **Kommissionstext vererben**
> Wenn Sie einer Position mit **<Shift> + <F11>** einen Kommissionstext zuordnen, kann der Kommissionstext für alle folgenden Positionen übernommen werden. Dazu müssen Sie die Abfrage, ob die Kommission nach unten vererbt werden soll, mit [Ja] bestätigen. Wenn Sie [Nein] klicken, wird der Kommissionstext nur für die aktuelle Position übernommen. Die Abfrage wird nur angezeigt, wenn nach der aktuellen Position weitere Positionen erfasst sind. Die Erfassung der Kommissionstexte im Bereich Einkauf ist jedoch unüblich. In der Regeln werden die Kommissionstexte bei auftragsbezogenen Bestellungen aus dem Verkauf übernommen.

*   **LE**: Leistungserklärung. Bezeichnung der Leistungserklärung, die dem Artikel zugeordnet ist. Das Feld wird nur angezeigt, wenn dem aktuellen Artikel eine Leistungserklärung zugeordnet ist.
    *   Technische Info: Anzeigefeld, DB-Feld: kposp.lbrefnr
