---
description: "DE-HB-AWCADDesignerShapes_11"
---


# A+W CAD Designer (Shapes) Überblick

---
## Konkrete Fragestellungen

### Wichtige Einschränkungen

Die TAB mit A+W Enterprise, AWBroke und A+W CAD Designer (Shapes) hat einige wichtige Einschränkungen, die in Betracht gezogen werden müssen, wenn ein Einsatz geplant wird:

*   **Herauslösen von Unterpositionen nicht möglich.**
    In der TAB existiert zu jeder A+W Enterprise-Auftragsposition genau eine SN-Datei. Diese Datei enthält die Geometrien für alle Unterpositionen der Position (soweit es sich um Gläser handelt). Ein Herauslösen einer einzelnen Unterpositions-Geometrie (z. B. für eine Unterteilbestellung) ist nicht möglich.

*   **Nicht abgebildete Glasarten:**
    Zuschnitt-VSG wird von der TAB gegenwärtig nicht abgebildet.
    Stufen-ISO wird ebenfalls nicht abgebildet.

*   **Nicht abgebildete Bearbeitungen:**
    Die TAB mit A+W Enterprise, AWBroke und A+W CAD Designer (Shapes) bildet die folgenden Bearbeitungen nicht ab:
    *   Stufen bei ISO und VSG
    *   Gehrungen mit wählbarem Gehrungswinkel
    *   Facetten mit Winkel und Einschlifftiefe
    *   Asymmetrische Fasen
    *   Rillenschliffe
    *   Oberflächenbearbeitungen (Siebdruck, Ätzung, ...)

> **Zeitaufwand**
> Die vollständige Erfassung einer Position mit CAD-Mitteln erfordert gegenüber der summarischen Erfassung von Bearbeitungen in der Stückliste einen höheren Zeitaufwand. Es fallen Berechnungszeiten im A+W CAD Designer (Shapes) und Handlingzeiten bei den Übergaben zwischen A+W Enterprise und A+W CAD Designer (Shapes) an, die die Erfassung verlangsamen. Dennoch wird eine Beschleunigung des Gesamtprozesses erreicht, weil in der Arbeitsvorbereitung keine geometrische Nacherfassung mehr erforderlich ist.

> **Nachträgliche Änderung der Stückliste vermeiden!**
> Nach der Bearbeitung mit A+W CAD Designer (Shapes) sollten Sie keine stücklistenrelevanten Informationen in A+W Enterprise mehr ändern (z. B. Glasart austauschen), da diese nicht automatisch in der SN-Datei ergänzt werden. Wenn dies dennoch erforderlich ist, dann müssen Sie A+W CAD Designer (Shapes) erneut aufrufen. So stellen Sie sicher, dass nachträglich zugefügte Informationen auch in die zugehörige SN-Datei gelangen.

### SN-Dateien via AWBroke erstellen

1.  Erfassen Sie die Daten im Auftragskopf in gewohnter Weise.
2.  Erfassen Sie die Auftragsposition.
    Beschreiben Sie die Auftragsposition möglichst vollständig. Geben Sie z. B. die Modellnummer an und tauschen Sie ggf. glasspezifische Artikel (z. B. Folien, Gläser) in der Stückliste aus, bevor Sie A+W CAD Designer (Shapes) starten.
3.  Starten Sie A+W CAD Designer (Shapes). Betätigen Sie dazu `<Strg>` + `<E>` oder klicken Sie auf die Symbolschaltfläche [ShapingNesting].
    Im Hintergrund startet AWBroke und erstellt eine SN-Datei. A+W CAD Designer (Shapes) startet und zeigt die von AWBroke erstellte Datei an. Im Dialog Globale Formdaten können Sie sich anzeigen lassen, welche Informationen aus A+W Enterprise übergeben wurden.
4.  Erfassen Sie in A+W CAD Designer (Shapes) die erforderlichen Maße, Kantenbearbeitungen, Ausschnitte, Senkbohrungen und Bohrungen.

> **Bearbeitungen als Stücklistenelement verwenden!**
> Einige Bearbeitungen verschmelzen mit der Kontur, andere bleiben als Bearbeitung erhalten. Achten Sie bei der Auswahl der Werkzeuge darauf, dass Sie die Werkzeuge verwenden, deren Bearbeitung als Stücklistenelement an A+W Enterprise zurückgegeben wird.

5.  Wählen Sie Datei > Zurück zur Auftragsbearbeitung.
    A+W CAD Designer (Shapes) schließt die Datei. AWBroke konvertiert die zugefügten und Stücklisten-tauglichen Informationen und Bearbeitungen und ergänzt die Stückliste der Auftragsposition in A+W Enterprise entsprechend.

> **A+W Enterprise wartet auf die Informationen aus CAD Designer!**
> Während Sie die Auftragsposition in A+W CAD Designer (Shapes) bearbeiten, wartet A+W Enterprise. Sie können so lange in A+W Enterprise nicht weiterarbeiten, bis Sie die Bearbeitung in A+W CAD Designer (Shapes) beendet haben. Wenn in der Kommunikation zwischen A+W Enterprise und A+W CAD Designer (Shapes) ein Fehler auftritt und ALCIB blockiert ist, dann können Sie mit der Tastenkombination `<Strg>` + `<Entf>` die Kommunikation abbrechen. Für die betroffene Position wurde dann keine SN-Datei erzeugt. Dieser Arbeitsschritt muss dann für diese Position wiederholt werden.

> **Keine CAD-relevanten Einträge in der Stückliste mehr ändern!**
> Wenn Sie jetzt die A+W Enterprise-Stückliste ändern wollen, erscheint der Hinweis, dass es sich um eine CAD-Position handelt. Wenn Sie jetzt CAD-relevante Änderungen vornehmen, dann stimmen die SN-Datei und die Auftragsposition nicht mehr überein. CAD-relevant sind Maße, Kantenbearbeitungen, Ausschnitte, Senkbohrungen und Bohrungen. Wenn Sie noch Änderungen vornehmen müssen, dann müssen Sie A+W CAD Designer (Shapes) erneut starten.

6.  Erfassen Sie ggf. weitere Positionen in A+W Enterprise.
7.  Falls Sie nachträglich CAD-relevante Einträge in der Stückliste ändern müssen, dann starten Sie A+W CAD Designer (Shapes) für die betroffene Position erneut (siehe Schritt 3).
    Die zur Auftragsposition gehörende SN-Datei wird bei der Zusammenarbeit mit A+W Production in der Produktionssteuerung wieder benötigt.

### Kopplung über SNAuto

Diese Kopplung wird auch als Hintergrund-TAB bezeichnet. Nach der Erfassung einer Position in A+W Enterprise erstellt SNAuto die zugehörige SN-Datei automatisch im Hintergrund.

In der Praxis wird das Arbeiten mit AWBroke und SNAuto kombiniert. Damit können komplizierte Produkte an wenigen ausgewählten Arbeitsplätzen über AWBroke mit A+W CAD Designer (Shapes) erstellt werden. Alle Standardprodukte können ohne Verzögerung mit SNAuto im Hintergrund an allen Arbeitsplätzen der Auftragserfassung erfasst werden.

**(Hintergrund-TAB)**

Die TAB mit A+W Enterprise und SNAuto ermöglicht das Erzeugen von SN-Dateien aus A+W Enterprise-Stücklisten. Der Auftragserfasser muss das Produkt bei der Positionserfassung in A+W Enterprise (in der Stückliste) vollständig beschreiben. Die SN-Datei wird dann anhand dieser Stückliste automatisch von SNAuto im Hintergrund erzeugt. Der Bearbeiter muss nicht darauf warten, dass SNAuto eine SN-Datei erzeugt.

Bei dieser Arbeitsweise können die Standard-Aufträge ohne Verzögerung erfasst werden.

**Abb. A-237 CAD Designer - A+W Enterprise mit SNAuto**
*   **A** Zuordnungstabelle pflegen
*   **B** Position erfassen mit Stückliste
*   **C** Automatischer Start von SNAuto
*   **D** Einlesen der Stücklisten- und Artikel-Informationen
*   **E** SN-Datei erstellen und speichern

#### Voraussetzungen

Für die TAB mit SNAuto sind lediglich normale A+W Enterprise-Arbeitsplätze erforderlich. Die Ausstattung der Arbeitsplätze richtet sich nach den aktuell gültigen Systemanforderungen für A+W Enterprise. Darüber hinaus muss ein für diesen Zweck reservierter PC mit Windows 2000 Professional, Windows 2000 Server, oder Windows XP Professional vorhanden sein, auf dem SNAuto installiert wird. Die Systemvoraussetzungen für diesen PC sind die jeweils gültigen Systemvoraussetzungen für einen SNAuto-Server (diese Systemvoraussetzungen erhalten Sie bei A+W).

Der SNAuto-Server muss Laufwerke in der UNIX-Umgebung per Samba ansprechen können. Alternativ können die Daten per ftp ausgetauscht werden.

Damit SNAuto die A+W Enterprise-Artikel in die SN-Artikelnummern umsetzen kann, wird wie bei der Zusammenarbeit mit AWBroke die Tabelle mit der Zuordnung der A+W Enterprise-Artikelnummern und die zugehörigen A+W CAD Designer (Shapes)-Artikelnummern benötigt. Diese können Sie in den A+W Enterprise-Stammdaten pflegen. Ohne diese Tabelle ist ein Betrieb der TAB nicht möglich.

#### Verfügbarkeit

Die TAB mit A+W Enterprise/SNAuto erfordert A+W CAD Designer (Shapes)-Version 4.04-00 oder eine neuere Version auf dem SNAuto-Server. Dies ist zu berücksichtigen, wenn Sie bereits A+W CAD Designer (Shapes)-Installationen haben. Ggf. ist ein Upgrade des A+W CAD Designer (Shapes) erforderlich. Empfohlen ist der Einsatz der jeweils letzten freigegebenen Version.

Die TAB mit A+W Enterprise/SNAuto ist mit der A+W Enterprise-Version 2.12 auf den A+W Enterprise-Plattformen SCO, AIX, HP-UX und Linux möglich. Andere A+W Enterprise-Versionen unterstützen diese Form der TAB nicht. Ebenso ist diese Form der TAB auf anderen UNIX-Varianten nicht verfügbar.

#### Verarbeitbare Produkttypen

Die TAB mit A+W Enterprise/SNAuto ist nur für die hier aufgelisteten Produkttypen (Gläser, Bearbeitungen, Modelle) verfügbar. Nicht aufgelistete Glasarten, Bearbeitungen oder Modelle können mit der TAB zur Zeit nicht erfasst werden.

**Glasartikel**

Die TAB mit A+W Enterprise/SNAuto kann diese Glasarten behandeln:
*   Float-Gläser, unbearbeitet (Artikel 11xxxx).
*   Float-Gläser, bearbeitetet (Artikel 15xxxx).
*   ESG-Gläser (Artikel 30xxxx und 35xxxx) mit darunter liegendem einfachen Float (Artikel 11xxxx) oder bearbeitetem Float (Artikel 15xxxx).
*   VSG aus Float oder ESG, bestehend aus den zuvor genannten Gläsern, jedoch kein Zuschnitt-VSG (Artikel 40xxxx).
*   ISO-Einheiten, bestehend aus den zuvor genannten Gläsern, jedoch kein Stufen-ISO (Artikel 50xxxx).

**Bearbeitungen**

Die TAB mit A+W Enterprise/SNAuto kann diese Bearbeitungen behandeln:
*   Zylindrische (normale) Bohrungen
*   Senkbohrungen (oben, unten, beidseitig)
*   Gesäumte, geschliffene und polierte Kanten
*   Definierbare Sonderkanten. Diese Sonderkanten sind nicht parametrisierbar. Es stehen 15 unterschiedliche Sonderkanten zur Verfügung.

#### Modelle

Die TAB mit A+W Enterprise/SNAuto kann Rechtecke und Modelle aus einem festgelegten Modellkatalog behandeln. Der Modellkatalog kann einer der im A+W Enterprise verfügbaren Kataloge sein. Es sind nur die in einem Katalog enthaltenen Standard-Modelle möglich. Kundenspezifische Katalogerweiterungen müssen für die Zusammenarbeit mit SNAuto angepasst werden, auch wenn der Kunde diese Erweiterung im A+W Enterprise bereits besitzt.

Die TAB mit A+W Enterprise/SNAuto kann keine freien Formen (Modell 99) behandeln.

#### Wichtige Einschränkungen

Die TAB mit A+W Enterprise und SNAuto hat einige wichtige Einschränkungen, die in Betracht gezogen werden müssen, wenn ein Einsatz geplant wird.

*   **Herauslösen von Unterpositionen nicht möglich.**
    In der TAB existiert zu jeder A+W Enterprise-Auftragsposition genau eine SN-Datei. Diese Datei enthält die Geometrien für alle Unterpositionen der Position (soweit es sich um Gläser handelt). Ein Herauslösen einer einzelnen Unterpositions-Geometrien (z. B. für eine Unterteilbestellung) ist nicht möglich.

*   **Nicht abgebildete Glasarten:**
    Zuschnitt-VSG wird von der TAB gegenwärtig nicht abgebildet

*   **Nicht abgebildete Bearbeitungen**
    Die TAB mit A+W Enterprise und SNAuto bildet die folgenden Bearbeitungen nicht ab:
    *   Eckabschnitte (Fasen)
    *   Rundecken
    *   Obere, untere oder beidseitige Senkbohrungen: Im A+W Enterprise wird mit einer Umgebungsvariablen eingestellt, ob alle Senkbohrungen obere, untere oder beidseitige Senkbohrungen sind. Die jeweils anderen Varianten können nicht erfasst werden.
    *   Stufen bei ISO oder VSG
    *   Gehrungen mit wählbarem Gehrungswinkel
    *   Facetten mit Winkel und Einschlifftiefe
    *   Rillenschliffe
    *   Oberflächenbearbeitungen (Siebdruck, Ätzung, ...)

*   **Keine CAD-Eingabe**
    Die TAB mittels A+W Enterprise/SNAuto kann keine zu digitalisierenden Positionen bearbeiten. Ebenso kann die TAB mittels A+W Enterprise/SNAuto keine Positionen von CAD-Dateien (DXF, IGES) übernehmen. Auch vermaßte Zeichnungen können auf diesem Weg nicht erfasst werden.

*   **Erhöhter Zeitaufwand**
    Die vollständige Erfassung einer Position in der Stückliste erfordert gegenüber der summarischen Erfassung von Bearbeitungen einen höheren Zeitaufwand. Bearbeitungen wie Bohrungen können nicht summarisch eingegeben werden, da für jede Bohrung auch die Bohrkoordinaten eingegeben werden müssen. Die technischen Parameter der Bearbeitung (z. B. Durchmesser und Lage der Bohrung) müssen zwingend angegeben werden.

### Umgebungsvariablen für SNAuto in A+W Enterprise

Bei der Installation von SNAuto können eine Reihe von Einstellungen vorgenommen werden, die das Arbeiten mit SNAuto beeinflussen. Dies geschieht mit den Umgebungsvariablen in A+W Enterprise. Beim Freischalten des Moduls können Sie folgende Varianten wählen:

*   A+W Enterprise fragt bei jeder Position, ob zu dieser Position mit SNAuto eine SN-Datei erstellt werden soll.
*   A+W Enterprise fordert automatisch zu jeder Position über SNAuto eine SN-Datei an.

Die Einstellungen für SNAuto können von benutzerspezifisch bis installationsweit gelten. Bei Fragen zu den Umgebungsvariablen wenden Sie sich an Servicemitarbeiter von A+W.

### SN-Dateien via SNAuto erstellen

Das Arbeiten mit SNAuto ist zur schnellen Ersterfassung von Auftragspositionen mit CAD-Informationen gedacht.

1.  Erfassen Sie die Daten im Auftragskopf in gewohnter Weise.
2.  Erfassen Sie die Auftragsposition. Geben Sie die Artikelnummer ein.
3.  Nach der Eingabe der Artikelnummer fragt A+W Enterprise, ob für diese Position eine SN-Datei generiert werden soll.

> **Frage nach SN-Datei nur bei der Ersterstellung!**
> Diese Frage, ob für diese Position eine SN-Datei generiert werden soll, wird nur bei der Ersterfassung gestellt. Spätere Änderungen werden nicht automatisch in die SN-Datei übernommen. Ein erneutes Erstellen einer SN-Datei muss dann mit der Tastenkombination `<Strg>` + `<N>` angefordert werden.

4.  Bestätigen Sie die Frage mit [Ja].
5.  Öffnen Sie die Stücklistendarstellung. Betätigen Sie dazu `<F3>` im Feld Menge der Position.
    A+W Enterprise zeigt die Stückliste an.
6.  Ergänzen Sie die Stückliste um die benötigten Bearbeitungen.
7.  Kehren Sie zur Auftragsposition zurück und schließen Sie die Positionserfassung ab. A+W Enterprise zeigt den Dialog zur Erfassung der Bearbeitungsparameter an.
8.  Ergänzen Sie die Benötigten Parameter für die Bearbeitungen der Scheibe. Diese Informationen benötigt SNAuto, um eine vollständige A+W CAD Designer (Shapes)-Datei zu erstellen.
9.  Speichern Sie Ihre Eingaben.
10. Speichern Sie den Auftrag.
    Der Hintergrundprozess erkennt vorhandene CAD-Anforderungen und gibt diese an SNAuto.

> **Auftrag kann nicht weiter bearbeitet werden!**
> Solange die SN-Dateien der Auftragspositionen nicht vorliegen, wird der Auftrag nicht an die Produktion weitergegeben.

> **Fehler werden gemeldet!**
> Wenn in der Zusammenarbeit mit SNAuto ein Fehler aufgetreten ist, dann wird der A+W Enterprise-Benutzer informiert, der für solche Fehlermeldungen angegeben wurde. Dieser Benutzer wird mit der Umgebungsvariablen SNAUTO_MANR definiert.

**Ergänzende Informationen**
⇨ "Umgebungsvariablen für SNAuto in A+W Enterprise" auf Seite A-506

## Zusammenarbeit mit A+W Business

Wenn Sie mit A+W Business arbeiten, dann können Sie direkt bei der Auftragserfassung für jede Auftragsposition eine SN-Datei anlegen. Diese Arbeitsweise bezeichnet A+W Business als Technische Auftragsbearbeitung (TAB). A+W Business und A+W CAD Designer (Shapes) laufen beide auf Windows-Systemen. A+W Business kann ohne Schnittstellendateien oder Zusatzprogramme A+W CAD Designer (Shapes) fernsteuern.

**Abb. A-238 CAD Designer- Grundsätzliche Zusammenarbeit mit A+W Business**
*   **A** Produktaufbau (Stückliste) einer Position vollständig erfassen und in Hintergrund CAD Designer starten
*   **B** Vorgefertigtes Modell oder Template verwenden
*   **C** SN-Datei automatisch erstellen

Alle erforderlichen Informationen zur Fernsteuerung von A+W CAD Designer (Shapes) sind in den Stammdaten von A+W Business hinterlegt oder müssen dort ggf. ergänzt werden. Die SN-Datei wird im weiteren Arbeitsablauf für die Anzeige in der Produktion und die Maschinenansteuerung benötigt.

Im Detail stehen Ihnen bei der TAB mit A+W Business folgende Arbeitsweisen zur Verfügung:
*   Modell erfassen und SN-Datei erzeugen
*   Fertige SN-Datei an die Position anhängen
*   Template-Datei verwenden und endgültig vermaßen

### Modell erfassen und SN-Datei erzeugen

Bei der Installation von A+W Business müssen Sie angeben, mit welchem Modellkatalog Sie arbeiten wollen. Z. Zt. stehen folgende Modellkataloge zur Auswahl:
*   A+W
*   Bilco

Wenn Sie bei der Positionserfassung in die Modellerfassung wechseln, dann stellt Ihnen A+W Business den installierten Modellkatalog zur Verfügung. Sie müssen dann nur noch folgende Arbeitsschritte ausführen, um eine SN-Datei zu erzeugen:
*   Modell auswählen
*   Maße ergänzen
*   Bearbeitungen zufügen
*   Skizze kontrollieren
*   Position speichern

**Abb. A-239 SN-Datei mit A+W Business-TAB über Modell erfassen**

Wenn Sie die Position speichern, dann erzeugt A+W Business durch Fernsteuerung von A+W CAD Designer (Shapes) die SN-Datei zur erfassten Position. Tritt dabei ein Fehler auf, werden Sie darüber informiert und können eingreifen. Nur eine fehlerfreie Position können Sie abspeichern.

Das Erstellen und Ausdrucken von Skizzen (z. B. in Formularen) sind Funktionen aus A+W CAD Designer (Shapes). A+W Business bringt diese nur zur Anzeige.

### Fertige SN-Datei an die Position anhängen

Wenn Sie Positionen erfassen, die bereits vollständig und richtig vermaßt als SN-Datei vorliegen, dann können Sie diese Datei an die Position anhängen und somit die Bereitstellung einer SN-Datei für die Produktion abkürzen. Anhängen können Sie eine SN-Datei aus einem beliebigen Verzeichnis oder eine BLOCK.IND-Datei.

**Abb. A-240 SN-Datei anhängen**
*   **A** Checkbox nicht anhaken, wenn Sie eine BLOCK.IND-Datei angeben.
*   **B** Checkbox anhaken, wenn Sie eine SN-Datei angeben.
*   **C** Eingabefeld für Dateinamen
*   **D** Datei öffnen zur Auswahl der anzuhängenden Datei

Auch solche Dateien, die Sie nur anhängen, können Sie sich als Skizze anzeigen lassen.

### Template-Datei verwenden und endgültig vermaßen

Statt mit Modellen können Sie mit beliebigen SN-Dateien arbeiten, in denen Variablen enthalten sind. Solche Dateien werden als Templates bezeichnet. Damit A+W Business SN-Dateien als Template erkennt, muss der Dateiname mit T_ (T und Unterstrich) beginnen. Variablen in solchen SN-Dateien werden von A+W Business erkannt, angezeigt und können von Ihnen mit Werten belegt werden. In der A+W Business-Positionserfassung müssen Sie folgende Arbeitsschritte ausführen, um eine Template-Datei zu verwenden:

*   Modell 99 wählen
*   Template-Datei angeben
*   Variablen mit Werten belegen (Maße angeben)

Das nachfolgende Bild zeigt ein Template, bei dem die konkreten Maße ergänzt wurden:

**Abb. A-241 SN-Datei mit A+W Business-TAB über Template erfassen**

Solche Template-Dateien können Sie mit A+W CAD Designer (Shapes) erstellen und in A+W Business nutzen. Bei der Verwendung von Variablen müssen Sie darauf achten, dass alle Variablen, die nicht mit einem `_` (Unterstrich) beginnen, von A+W Business erkannt, angezeigt und mit Werten belegt werden können.

Als weiterer Automatisierungsschritt besteht die Möglichkeit, Variablen in Templates automatisch mit Werten zu belegen. Variablen, die von A+W Business automatisch gelesen und mit Werten belegt werden sollen, müssen in A+W CAD Designer (Shapes) mit einem doppelten Unterstrich `__` beginnen.

Zur Zusammenarbeit der A+W Business TAB mit A+W CAD Designer (Shapes) finden Sie nachfolgend folgende Arbeiten beschrieben:
*   ⇨ "SN-Datei über die Modellerfassung erzeugen" auf Seite A-512
*   ⇨ "Fertige SN-Datei einer Position anhängen" auf Seite A-513
*   ⇨ "SN-Datei aus Template-Datei erstellen" auf Seite A-513
*   ⇨ "Automatische Variablen anlegen" auf Seite A-514

### SN-Datei über die Modellerfassung erzeugen

1.  Erfassen Sie die Auftragskopf-Daten in gewohnter Weise.
2.  Erfassen Sie die Auftragsposition. Geben Sie dazu mindestens den Artikel ein.
3.  Wechseln Sie mit `<F9>` in die Modellerfassung und wählen Sie das gewünschte Modell aus. Das Modell können Sie mit der Modellnummer oder per Mausklick auf das entsprechende Symbol auswählen.
4.  Markieren Sie im Bereich A+W CAD Designer (Shapes) die Checkbox S+N-Datei.
5.  Klicken Sie auf die Symbolschaltfläche zum Erzeugen einer neuen SN-Datei.

> A+W Business fügt automatisch einen Dateinamen (mit Jahr, Monat und einer fortlaufenden Nummer) ein. Diese Datei wird beim Speichern der Position erstellt.

6.  Ergänzen Sie nach Bedarf Bearbeitungen im A+W Business-Autrag.
7.  Kontrollieren Sie die Skizze. Klicken Sie dazu auf das Lupen-Symbol. Jetzt ruft A+W Business im Hintergrund A+W CAD Designer (Shapes) auf und erstellt die Zeichnung. Die erstellte Zeichnung zeigt A+W Business in einem eigenen Dialog an.
8.  Speichern Sie die Auftragsposition, wenn alle Angaben korrekt sind. Jetzt erzeugt A+W Business mit A+W CAD Designer (Shapes) im Hintergrund die SN-Datei und speichert Sie im vorgegebenen Verzeichnis ab.

> **Änderungen in der Position ändern die SN-Datei**
> Wenn Sie eine Position nach dem Speichern nochmals ändern und erneut speichern, dann aktualisiert A+W Business auch die SN-Datei.

### Fertige SN-Datei einer Position anhängen

1.  Erfassen Sie die Auftragskopf-Daten in gewohnter Weise.
2.  Erfassen Sie die Auftragsposition.
3.  Wechseln Sie mit `<F9>` in die Modellerfassung und geben Sie Modell 99 ein.
4.  Entscheiden Sie, welche Art von Datei Sie anhängen wollen:
    *   Wenn Sie eine SN-Datei anhängen wollen, dann markieren Sie im Bereich A+W CAD Designer (Shapes) die Checkbox S+N-Datei.
    *   Wenn Sie eine BLOCK.IND-Datei anhängen wolle, dann markieren Sie im Bereich A+W CAD Designer (Shapes) die Checkbox S+N-Datei nicht.
5.  Klicken Sie auf die Symbolschaltfläche zum Anhängen einer Datei.

> Die Symbolschaltfläche steht Ihnen nur dann zur Verfügung, wenn Sie zuvor die Checkbox S+N-Datei markiert haben.
> A+W Business öffnet den Dialog Datei auswählen. Alternativ können Sie den Dateinamen und Pfad direkt in das Feld eingeben.
> Wenn Sie eine Datei angegeben haben, dann ermittelt A+W Business das umschreibende Rechteck und zeigt dies mit den zugehörigen Maßen an.

> **Änderungen in der Position ändern die SN-Datei nicht!**
> Wenn Sie eine Position ändern, dann hat dies keine Auswirkungen auf die SN-Datei. Wenn Sie Änderungen in der SN-Datei benötigen, dann müssen Sie diese Änderungen mit A+W CAD Designer (Shapes) durchführen.

6.  Speichern Sie die Position.

### SN-Datei aus Template-Datei erstellen

1.  Erfassen Sie die Auftragskopf-Daten in gewohnter Weise.
2.  Erfassen Sie die Auftragsposition.
3.  Wechseln Sie mit `<F9>` in die Modellerfassung und geben Sie Modell 99 ein.
4.  Markieren Sie im Bereich A+W CAD Designer (Shapes) die Checkbox S+N-Datei.
5.  Klicken Sie auf die Symbolschaltfläche zum Anhängen einer Datei.
6.  Wählen Sie eine Template-Datei aus.
    Template-Dateien beginnen immer mit T_.

> **Speichern erst nach Eingabe der Variablen möglich!**
> Wenn Sie eine Template-Datei ausgewählt haben, können Sie die Position nicht sofort speichern. Erfassen Sie zuerst die Variablen in der Modellansicht.

7.  Wechseln Sie in die Modellansicht. Klicken Sie dazu auf die Lupe. A+W Business zeigt das Modell und die zugehörige Variablenliste in einem weiteren Dialog an.
    A+W Business zeigt nur die Variablen an, die in der SN-Datei mit einem Namen bezeichnet wurden, der ohne Unterstrich (`_`) beginnt.
    Variablen, deren Namen mit zwei Unterstrichen beginnen, können von A+W Business automatisch mit Werten belegt werden. Dazu muss A+W Business entsprechend eingerichtet werden.
8.  Geben Sie für die Variablen die benötigten Werte der Auftragsposition ein.
9.  Betätigen Sie [OK]. Die Position wird mit den aktuellen Werten neu berechnet und die Zeichnung neu angezeigt.
10. Verlassen Sie die Modellansicht. Klicken Sie dazu auf [ENDE]. Im Feld mit dem Dateinamen wurde der Name der Template-Datei gegen den Namen der Datei ausgetauscht, die jetzt mit den eingegebenen Werten angelegt wurde.
11. Speichern Sie die Position.

> **Änderungen in der SN-Datei möglich!**
> Wenn Sie eine Position nach dem Speichern nochmals aufrufen und die Werte der Variablen ändern, dann aktualisiert A+W Business auch die SN-Datei.

### Automatische Variablen anlegen

In SN-Templates, die Sie aus A+W Business heraus automatisch vermaßen wollen, müssen Sie Variablen nach folgendem Schema anlegen:

`__XXXX_YY_ZZ`
(2 Unterstriche, 4 Zahlen, 1 Unterstrich, 2 Zahlen, 1 Unterstrich, 2 Zahlen)

*   **XXXX** = vierstellige Produknummer der Bearbeitung in A+W Business.
*   **YY** = wievieltes Vorkommen der Bearbeitung im zu bearbeitenden Glas.
*   **ZZ** = auszuwertendes Maß der Bearbeitung.

Gehen Sie wie folgt vor, um automatische Variablen zu verwenden:

1.  Erstellen Sie eine SN-Datei mit der gewünschten Kontur.
2.  Vermaßen Sie die Kontur mit Variablen.
    Verwenden Sie Variablennamen nach dem oben angegebenen Schema.
3.  Geben Sie in der Variablen die A+W Business-Produktnummer (XXXX) an.
4.  Geben Sie in der Variablen an, aus dem wievielten Vorkommen der angegebenen Bearbeitung (in der A+W Business-Stückliste des Glases) die Vermaßung mit einem Wert belegt werden soll (YY).
5.  Geben Sie in der Variablen an, welcher Parameter der Bearbeitung die Variable mit einem Wert belegen soll (ZZ). Die Parameter werden je nach Bearbeitungsart ausgewertet:
    *   **Bearbeitungsart Lochbohrung:**
        *   00 = X-Wert Loch 1
        *   01 = Y- Wert Loch 1
        *   02 = Durchmesser Loch 1
        *   03 = X-Wert Loch 2
        *   04 = Y- Wert Loch 2
        *   05 = Durchmesser Loch 2
        *   06 = X-Wert Loch 3
        *   07 = Y-Wert Loch 3
        *   08 = Durchmesser Loch 3
        *   09 = X-Wert Loch 4
        *   10 = Y- Wert Loch 4
        *   11 = Durchmesser Loch 4
        Hier können die Maße von 4 Löchern zugeordnet werden, weil in A+W Business mit einer Bearbeitung Bohrung vier Löcher mit identischem Durchmesser positioniert werden können.
    *   **Bearbeitungsart Randausschnitt:**
        *   00-07 = Nummer der Kante
        *   08 = Breite des Randausschnitts
        *   09 = Höhe des Randausschnitts
        *   18 = Abstand des Randausschnitts

    **Beispiel**
    Name der Variablen: `__9610_03_02`
    *   **9610** könnte z. B. die Bearbeitung *Bohrung* sein.
    *   **03** ist die dritte Bearbeitung *Bohrung* im Glas.
    *   **02** ist der Durchmesser des (ersten) Loches der dritten Bearbeitung *Bohrung*.

6.  Speichern Sie die SN-Datei und verwenden Sie diese wie andere Template-Dateien.

> **SN-Datei kann ohne Skizzenansicht erstellt werden!**
> Wenn das SN-Template außer den Modell-Ergänzungsmaßen nur automatische Variablen enthält, dann können Sie die Kontur mit A+W Business vollständig vermaßen und ohne Betreten der Skizzenansicht (in A+W Business) speichern. Enthält das Template jedoch weitere Variablen, dann müssen Sie die Variablen in der Skizzenansicht ergänzen.
>
> Ob der Name der automatischen Variable in der Skizzenansicht angezeigt werden soll, kann in der sn.ini eingestellt werden.

## Zusammenarbeit mit A+W Production

Die Kopplung von A+W CAD Designer (Shapes) an A+W Production wird hauptsächlich genutzt, um mit Hilfe von A+W CAD Designer (Shapes) den zur Produktionssteuerung benötigten Maschinencode zu erzeugen und die Ansichten zu erstellen, die an verschiedenen Bearbeitungsstationen benötigt werden.

Das folgende Schaubild zeigt einige Beispiele, wie A+W Production Funktionen von A+W CAD Designer (Shapes) nutzt:

**Abb. A-242 CAD Designer - Zusammenarbeit mit A+W Production**
*   A+W Production ruft im Hintergrund A+W CAD Designer (Shapes) auf und erzeugt den benötigten CNC- oder CAMDXF-Code.
*   Beim Import von Positionen mit angehängter SN-Datei wird ebenfalls im Hintergrund A+W CAD Designer (Shapes) gestartet und überprüft, ob die Artikel und Bearbeitungen in der SN-Datei mit der A+W Production-Stückliste übereinstimmen.

### Über CNC-Dateien

CNC ist ein Standard Export-/Import-Format zur Ansteuerung von CNC-Maschinen. A+W CAD Designer (Shapes) kann in dieses Format exportieren. Einige CNC-Maschinen verstehen mehr CNC-Befehle, als im Standard festgelegt sind. Daher stellt A+W CAD Designer (Shapes) mehrere Möglichkeiten zur Verfügung, wie Sie CNC-Code erstellen können:

*   Standard-CNC-Code können Sie über Datei > Exportieren > CNC erstellen.
*   Wenn Sie maschinenspezifische CNC-Codes erstellen wollen, dann müssen Sie zuvor den entsprechenden Treiber installieren. Wenn Sie den Treiber installiert haben, dann erstellt A+W CAD Designer (Shapes) über das Menü Maschine > Übergabe an ... den maschinenspezifischen CNC-Code.

> **Maschinenspezifische Treiber sind erforderlich!**
> Informationen über die verfügbaren Treiber und die entsprechende Konfiguration von A+W CAD Designer (Shapes) erhalten Sie auf Anfrage bei A+W.

Bei der Einrichtung von Maschinentreibern wird festgelegt, aus welcher Ansicht die Geometrie exportiert werden soll. Somit können Sie sicherstellen, dass die Schleifmaschine aus der Ansicht Schleifen, die Bohrmaschine aus der Ansicht Bohren mit Daten versorgt wird.

### Über DXF-Dateien

DXF ist ein Standard Export-/Import-Format, das den Austausch von CAD-Dateien zwischen verschiedenen Anwendungsprogrammen ermöglicht. In DXF-Dateien sind die grafisch-geometrischen Daten der Zeichnungsobjekte in einem international verwendeten Code gespeichert. Diese Informationen sind für jedes CAD-Programm lesbar.

A+W CAD Designer (Shapes) ist wegen seiner CAM-Komponenten darauf angewiesen, Konturenzusammenhänge zu erkennen und zu verwalten. Im Gegensatz zum konventionellen CAD sind dabei Segmentzusammengehörigkeiten von Bedeutung. Für A+W CAD Designer (Shapes) reicht es nicht aus, nur eine Kollektion von individuellen Segmenten zu verwalten, sondern diese Segmente müssen eine zusammenhängende Kontur bilden.

#### Standard DXF

Das DXF-Format enthält geometrische Daten, d. h., es definiert Parameter wie Kontur und Anzahl der gezeichneten Elemente, Größe, Farbe, Linienstärke, Positionen von Bohrlöchern, etc. Solche DXF-Dateien kann A+W CAD Designer (Shapes) lesen und weiterverarbeiten und umgekehrt Konturen in diesem Format abspeichern.

In DXF-Dateien sind keine Informationen zu maschinenseitigen Prozessen, die zur Herstellung des gezeichneten Elements nötig sind, enthalten. Dazu zählen z. B. der Schneidweg, die Brechreihenfolge und weitere Informationen, die im A+W CAD Designer (Shapes) bereits erfasst und vorgegeben werden können.

Damit DXF-Daten aus anderen CAD-Programmen ohne viel Nacharbeit in A+W CAD Designer (Shapes) richtig gelesen werden können, müssen Sie einige Anforderungen einhalten. Z. B. wird zwischen zwei aneinander angrenzenden Scheiben im allgemeinen nur eine Linie gezeichnet, obwohl hier für A+W CAD Designer (Shapes) zwei Segmente für die Begrenzung der Scheiben erforderlich sind. Häufig liegen die Endpunkte von aneinander angrenzenden Segmenten nicht exakt aufeinander. A+W CAD Designer (Shapes) arbeitet in solchen Fällen mit so genannten Fangbereichen. Liegen Segmentenden im selben Fangbereich, so kann A+W CAD Designer (Shapes) diese automatisch verbinden.

Folgende Richtlinien sollten Sie beim Erstellen von Dateien in einem CAD-Programm beachten, wenn Sie die Daten in A+W CAD Designer (Shapes) weiterbearbeiten wollen:

*   Die einzulesende Kontur soll vollständig und allein in einem DXF-Layer liegen. Sollen von einer DXF-Datei mehrere Konturen eingelesen werden, so sollte jede Kontur in einem eigenen Layer liegt. Beschriftungen, Vermaßungen, Legenden, etc. sollten in getrennten Layern liegen.
*   Die einzulesende Kontur muss geschlossen sein. Offene Konturen müssen Sie in A+W CAD Designer (Shapes) nachbearbeiten.
*   Die einzulesende Kontur soll aus ARC-, LINE- und CIRCLE-Entities bestehen. A+W CAD Designer (Shapes) kann in begrenztem Maß POLYLINE-Entities einlesen, diese sollten Sie aber vermeiden. A+W CAD Designer (Shapes) wandelt SOLID- und TRACE-Entities vor der Übernahme in mehrere LINE-Entities um, so dass diese Entities gelesen werden können. CIRCLE-Entities sollen Sie nur verwenden, um die Lage von Bohrlöchern anzuzeigen.
*   Der DXF-Header wird nicht interpretiert. Die DXF-Dateien werden kleiner, wenn Sie den Header weglassen. Für den Import nach A+W CAD Designer (Shapes) sind nur die SECTION ENTITIES erforderlich. Aus dieser Eigenschaft folgt, dass ARC-Entities nicht im Uhrzeigersinn definiert werden können, da diese Einstellung durch die Variable $ANGDIR in SECTION HEADER bestimmt wird.
*   INSERT-Entities werden nicht expandiert. Daraus folgt, dass die Kontur komplett in SECTION ENTITIES definiert werden muss und nicht aus Blocks zusammengebaut werden kann.
*   Die Begrenzungspunkte aneinander angrenzender Segmente einer Kontur sollen aufeinander liegen.
*   Müssen mehrere Konturen in ein Layer gelegt werden, so sollten Sie Verzweigungspunkte vermeiden. Anderenfalls kann es dazu kommen, dass die falschen Segmente zu Konturen verbunden werden.

Grundsätzlich gilt die Empfehlung, dass der Lieferant der DXF-Datei seine Datei mit den oben genannten Richtlinien auf den Import ins A+W CAD Designer (Shapes) zuschneiden sollte.

### CAMDXF

Für den Bediener einer CNC-Maschine beginnt die Arbeit normalerweise mit dem Vorliegen einer DXF-Datei. Der Maschinenführer muss dann jedes für eine Bearbeitung notwendige Detail der DXF-Datei in einen vordefinierten Bearbeitungsprozess umsetzen. Er muss die zu benutzenden Werkzeuge und sämtliche Bearbeitungsparameter definieren. Auf diese Weise wurde bisher das Bearbeitungs- (CAM)-Programm erstellt und zur Ausführung an die Maschine übergeben.

A+W CAD Designer (Shapes) stellt mit dem Datenformat CAMDXF ein erweitertes DXF zur Verfügung. In diesem Format sind die Informationen zur Maschinenansteuerung bereits enthalten. Das Format CAMDXF bietet folgende Vorteile:

*   Das das Steuern der Maschinen mit den Bearbeitungsdaten wird schneller, eleganter und sicherer.
*   Neben den geometrischen Daten enthält CAMDXF auch die Maschineninformationen für mehrere Maschinen in der Bearbeitungskette.
*   Das Format kann für die Ansteuerung von Maschinen der Hersteller Z. Bavelloni, Intermac und Forvet verwendet werden.
*   Die in den CAMDXF-Dateien enthaltenen Informationen werden ohne eine aufwändige Maschinenprogrammierung von den Bearbeitungsmaschinen direkt eingelesen.
*   Die CAMDXF-Dateien enthalten sämtliche Details wie die nötigen Werkzeuge und Einstellungen, die Referenzpunkte für die Saugerpositionierung etc.
*   CAMDXF ist so aufgebaut, dass es von allen Maschinenherstellern unterstützt werden kann.

Mit CAMDXF wird das CAD/CAM Programm an der Maschine nicht ersetzt. Dieses Programm wird weiterhin gebraucht, um die CAMDXF Dateien zu verarbeiten.

Die CAMDXF Datei kann bereits in A+W CAD Designer (Shapes) erstellt und direkt an die Arbeitsvorbereitung bzw. in das DV-System des Produzenten geschickt werden. Aufwändige Schulungs- und Trainingsmaßnahmen für die Maschinenführer entfallen. Die Durchlaufzeiten werden verkürzt und potenzielle Fehlerquellen entfallen.

Damit Sie dieses Format mit A+W CAD Designer (Shapes) schreiben können, müssen Sie zuvor den entsprechenden Maschinentreiber installieren. Die Export-Funktion steht Ihnen dann im Menü Maschine zur Verfügung.

Einen CAMDXF-Export können Sie ab der A+W CAD Designer (Shapes)-Version 5.02 und nur aus der Ansicht Kantenbearbeitung heraus durchführen.

### Über CAMXML-Dateien

CAMXML ist ein xml-basiertes format.
Häufig werden Teile eines Produktes (z. B. ESG in ISO oder ESG in VSG) zugekauft. In A+W CAD Designer (Shapes) liegt der vollständige Produktaufbau vor, der jedoch aus unterschiedlichen Gründen nicht zum Zulieferer gegeben werden kann oder darf.

Mit der Funktion CAMXML bietet Ihnen A+W CAD Designer (Shapes) die Möglichkeit, Daten einzelner Stücklistenteile zu exportieren. So exportierte Teile sind vollständig beschrieben und können vom Empfänger als neues Produkt in eine andere A+W CAD Designer (Shapes)-Installation importiert werden. Diese Funktion steht ab der A+W CAD Designer (Shapes)-Version 5.02 zur Verfügung.

### Datenexport

Daten von Konturen und Bearbeitungen, die in A+W CAD Designer (Shapes) definiert wurden, können in viele Datenformate exportiert werden. Dazu stehen Ihnen folgende Wege zur Verfügung:
*   Daten in ein Standardformat exportieren
*   Daten in ein maschinenspezifisches Format exportieren
*   Teil einer Stückliste exportieren

Eine Kurzbeschreibung der Datenformate finden Sie unter:
*   ⇨ Softwarereferenz, "Datei speichern unter (exportieren)" auf Seite A-175
*   ⇨ "Über CNC-Dateien" auf Seite A-516
*   ⇨ "Über DXF-Dateien" auf Seite A-517
*   ⇨ "Über CAMXML-Dateien" auf Seite A-519

#### Daten in ein Standardformat exportieren

1.  Speichern Sie den Bearbeitungsstand der SN-Datei, die Sie exportieren wollen. Vergeben Sie dazu, falls erforderlich, einen geeigneten Dateinamen.
2.  Wechseln Sie in die Ansicht, deren Darstellung Sie exportieren wollen.
3.  Öffnen Sie das Menü Datei > Exportieren. A+W CAD Designer (Shapes) zeigt mehrere mögliche Standard-Exportformate an.
4.  Wählen Sie das Format, in dem Sie Ihre Daten speichern wollen. A+W CAD Designer (Shapes) zeigt den Dialog Speichern unter an.
5.  Wählen Sie den gewünschten Speicherort und geben Sie den gewünschten Dateinamen an.
6.  Bestätigen Sie Ihre Eingaben mit `<OK>`. A+W CAD Designer (Shapes) speichert die Daten im angegebenen Format mit der zugehörigen Dateiendung ab.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Datei speichern unter (exportieren)" auf Seite A-175

#### Daten in ein maschinenspezifisches Format exportieren

Zur Ansteuerung von CNC-Maschinen kann A+W CAD Designer (Shapes) den passenden Steuercode ausgeben.

> **Maschinenspezifische Formate nur nach Einrichtung möglich!**
> Damit Sie maschinenspezifischen Code erzeugen können, müssen Sie zuerst den entsprechenden Maschinentreiber installieren und A+W CAD Designer (Shapes) entsprechend konfigurieren. Unterstützung erhalten Sie auf Anfrage bei A+W.

1.  Speichern Sie den Bearbeitungsstand der SN-Datei, die Sie exportieren wollen. Vergeben Sie dazu, falls erforderlich, einen geeigneten Dateinamen.
2.  Öffnen Sie das Menü Datei. A+W CAD Designer (Shapes) zeigt alle eingerichteten Maschinen an, für die Sie Daten exportieren können.
3.  Wählen Sie die Maschine aus, für die Sie Daten erzeugen wollen. A+W CAD Designer (Shapes) zeigt Ihnen weitere Optionen an.
4.  Wählen Sie das Datenformat (z. B. NC-Code), um den Datenexport aufzurufen. A+W CAD Designer (Shapes) speichert die Daten an der Stelle, die bei der Einrichtung des Maschinentreibers angegeben wurde.
5.  Bestätigen Sie Ihre Eingaben mit [OK]. A+W CAD Designer (Shapes) speichert die Daten im angegebenen Format mit der zugehörigen Dateiendung ab.
    A+W CAD Designer (Shapes) exportiert die Daten aus der Ansicht, die zur gewählten Maschine konfiguriert wurde.

#### Teil einer Stückliste exportieren

A+W CAD Designer (Shapes) stellt als Datenaustauschformat CAMXML zur Verfügung. Damit können Sie vollständige SN-Dateien aber auch nur Teile eines mehrstufigen Aufbaus speichern und z. B. an einen Zulieferer weitergeben.

1.  Speichern Sie den Bearbeitungsstand der SN-Datei, die Sie exportieren wollen. Vergeben Sie dazu, falls erforderlich, einen geeigneten Dateinamen.
2.  Wechseln Sie in die Ansicht Kantenbearbeitung. Nur aus dieser Ansicht ist ein Export in das Format CAMXML möglich. Wenn Sie aus einer anderen Ansicht heraus diese Funktion starten, dann wechselt A+W CAD Designer (Shapes) intern in diese Ansicht.
3.  Klicken Sie auf die Stufe, aus der Sie ein Teil exportieren wollen. Wenn Sie Stufe 0 wählen, wird der gesamte Produktaufbau exportiert.
4.  Klicken Sie auf ein Segment der Kontur, die Sie exportieren wollen. A+W CAD Designer (Shapes) wird das markierte Teil mit allen darunter liegenden zugehörigen Stufen exportieren.
5.  Wählen Sie im Menü Datei > Exportieren > CAMXML. A+W CAD Designer (Shapes) zeigt den Dialog Speichern unter an
6.  Wählen Sie den gewünschten Speicherort und geben Sie den gewünschten Dateinamen an.
7.  Bestätigen Sie Ihre Eingaben mit [OK]. A+W CAD Designer (Shapes) speichert die ausgewählte Teilform in der angegebenen Datei mit der Endung .xml ab. Die gespeicherte Datei kann mit jeder A+W CAD Designer (Shapes)-Version ab 5.02 geöffnet und als normale SN-Datei weiterverarbeitet werden. Wenn Sie prüfen wollen, welche Informationen in der CAMXML-Datei enthalten sind, dann öffnen Sie die Datei mit A+W CAD Designer (Shapes).

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Datei speichern unter (exportieren)" auf Seite A-175

## Darstellung der Zeichnung ändern

Im Menü Ansicht können Sie einstellen, wie A+W CAD Designer (Shapes) die Zeichnung und Vermaßung in den verschiedenen Ansichten anzeigen soll. Diese Einstellungen verändern die Darstellung der Zeichnung, deren Hintergrund oder die Maßdarstellung. Grundeinstellungen, die sich während eines Programmlaufs nicht ändern, werden in der Konfigurationsdatei sn.ini fest eingestellt.

Mit folgenden Funktionen können Sie die Darstellung der Zeichnung am Bildschirm verändern:
*   Maßeinheit auswählen
*   Anzeige erweitern

Darüber hinaus finden Sie eine Segmenterfassung für Experten, die nachfolgend näher erklärt wird.

### Maßeinheit auswählen

Sie können mit Millimetern (mm) oder mit Inch (inch) arbeiten. Beim Arbeiten mit Inch können Sie zwischen der dezimalen Form oder in der Schreibweise als Bruch wählen.

1.  Öffnen Sie das Menü Ansicht.
2.  Klicken Sie im Untermenü Einstellungen auf den Eintrag Maße. Maße bietet beim Anklicken folgende Optionen:
    *   Maßeingabe in mm
    *   Maßeingabe in Zoll (Brüche)
    *   Maßeingabe in Zoll (dezimal)
    *   gemischte Maßausgabe

Die oberen drei Optionen legen fest, in welcher Maßeinheit Zahlenwerte eingegeben werden: Millimeter, Zoll in Bruchzahldarstellung oder Zoll in dezimaler Schreibweise. Je nach Wahl der Maßeingabeoptionen ändert sich auch die Maßeinheit des Lineals am Rande der Zeichenfläche.

Wenn Sie bei der Maßeingabe nur eine Zahl (ohne mm oder ") eingeben, dann wird die Maßeinheit der Zahl durch die hier eingegebene Optionen festgelegt. Alternativ können Sie bei der Eingabe direkt die gewünschte Maßeinheit angeben (etwa 12 mm oder 25" 1/32). Die eingegebenen Werte werden dann in die eingestellte Einheit umgerechnet. Durch Anklicken von gemischte Maßausgabe werden alle Werte in ihrer ursprünglichen Maßeinheit angezeigt.

> **Eine Maßeinheit festlegen!**
> Aus Gründen der Übersichtlichkeit sollten Sie sich vor Beginn der Vermaßung auf eine Maßeinheit festlegen. Es ist jedoch möglich, verschiedene Teile einer Zeichnung in verschiedenen Maßeinheiten zu vermaßen. In diesem Fall sollten Sie gemischte Maßausgabe aktivieren, denn diese Funktion bewirkt eine Maßanzeige mit Einheiten (bei deaktivierter Funktion werden alle Maßangaben in der Zeichnung einheitenlos angezeigt).

3.  Wählen Sie eine der angezeigten Maßeingabeoptionen. Diese ist jetzt aktiv. A+W CAD Designer (Shapes) schließt das Menü. Die gewählte Option ist beim nächsten Öffnen des Menüs mit einem Haken versehen.

### Anzeige erweitern

Zusätzlich zur Zeichnung in verschiedenen Ansichten können Sie sich folgende Elemente zusätzlich anzeigen lassen:
*   "Kritische Stellen anzeigen" auf Seite A-524
*   "Messpunkte anzeigen" auf Seite A-525
*   "Kritische Stellen anzeigen" auf Seite A-524

#### Kritische Stellen anzeigen

Mit diesen Einstellungen können Sie (zu) spitze Winkel zwischen den Segmenten, (zu) kurze Segmente und (zu) kleine Innenradien einer Kontur anzeigen lassen. Es ist jeweils die durch einen Haken markierte Einstellung gültig.

1.  Öffnen Sie das Menü Ansicht.
2.  Klicken Sie im Untermenü Einstellungen auf den Eintrag Kritische Stellen anzeigen. Kritische Stellen anzeigen bietet beim Anklicken folgende Optionen:
    *   Markiere kritische Segmente in Geometrie und Revision.
        Kritische Segmente werden nur in den Ansichten Geometrie und Revision angezeigt.
    *   Markiere kritische Segmente in jeder Ansicht.
        Kritische Segmente werden in jeder Ansicht angezeigt.
    *   Kritische Segmente nicht markieren.
        Kritische Segmente werden nicht angezeigt.
3.  Wählen Sie eine der angezeigten Optionen. Diese ist jetzt aktiv. A+W CAD Designer (Shapes) schließt das Menü. Die gewählte Option ist beim nächsten Öffnen des Menüs mit einem Haken versehen.

Ab wann ein Winkel zu spitz, ein Segment oder ein Radius zu klein ist, wird mit der Datei sn.ini gesteuert. Im Abschnitt User dieser Datei befinden sich 4 Einträge, mit denen Sie das Anzeigen der kritischen Segmenten steuern können:

*   **MarkInsideRadiusBelow**
    Dieser Parameter gibt an, bis zu welchem Radius Bogensegmente als kritisch zu markieren sind (das ganze Segment wird dann in einer besonderen Farbe gezeichnet).
*   **MarkOutsideAngleAbove**
    Dieser Parameter gibt an, ab welchem Wert der äußere Übergangswinkel (Knick nach außen) zwischen Segmenten als kritisch zu markieren ist. Die Markierung erfolgt durch einen kleinen Pfeil, der auf den entsprechenden Punkt zeigt.
*   **MarkInsideAngleAbove**
    Dieser Parameter gibt an, ab welchem Wert der innere Übergangswinkel (Knick nach außen) zwischen Segmenten als kritisch zu markieren ist. Die Markierung erfolgt durch einen kleinen Pfeil, der auf den entsprechenden Punkt zeigt.
*   **MarkShortSegmentBelow**
    Dieser Parameter gibt an bis zu welcher maximalen Länge Segment als kurze Segmente zu markieren sind (das ganze Segment wird in einer anderen Farbe gezeichnet).

#### Messpunkte anzeigen

Durch diese Einstellung können Sie das Anzeigen von Messpunkten auf bestimmte Ansichten beschränken. Die Eingabe von Messpunkte ist in der Ansicht Punkte ist durch die Benutzung eines entsprechenden Digitalisierwerkzeugs möglich.

Die Punkte dienen als Referenzpunkte zur ursprünglichen Kontur. Eine nachträgliche Änderung der Lage eines Referenzpunktes ist nicht empfehlenswert. Ein Entfernen von Messpunkten ist in jeder Ansicht, in der sie sichtbar sind, möglich.

1.  Öffnen Sie das Menü Ansicht.
2.  Klicken Sie im Untermenü Einstellungen auf den Eintrag Messpunkte anzeigen. Messpunkte anzeigen bietet beim Anklicken folgende Optionen:
    *   **Zeige Messpunkte nur in Ansicht Punkte:**
        Messpunkte werden nur in der Ansicht Punkte angezeigt.
    *   **Zeige Messpunkte in einigen Ansichten:**
        Messpunkte werden in den Ansichten Punkte, Geometrie und Revision angezeigt. Die letzte Ansicht, in der noch Messpunkte angezeigt werden, kann in der Konfigurationsdatei sn.ini eingestellt werden ([View] LastViewToDrawCheckpoints=, Standardwert ist Revision).
    *   **Zeige Messpunkte in allen Ansichten:**
        Messpunkte werden in allen Ansichten angezeigt.

#### Gitter anzeigen

Mit dieser Funktion können Sie Gitterpunkte in die Zeichenebene einblenden. Je nach Vergrößerung der Anzeige werden Gitterpunkte je Millimeter, Zentimeter, Dezimeter oder Meter angezeigt.

1.  Öffnen Sie das Menü Ansicht.
2.  Klicken Sie im Untermenü Einstellungen auf den Eintrag Gitter anzeigen. Die Gitteranzeige ist jetzt aktiv. A+W CAD Designer (Shapes) schließt das Menü. Die gewählte Option ist beim nächsten Öffnen des Menüs mit einem Haken versehen. Um das Gitter wieder abzuschalten, wählen Sie diesen Punkt erneut aus.

#### Hintergrundbild (Deckkraft)

Mit dieser Funktion können Sie die Sichtbarkeit und die Deckkraft des Hintergrundbildes einstellen.

1.  Öffnen Sie das Menü Ansicht.
2.  Klicken Sie im Untermenü Einstellungen auf den Eintrag Hintergrundbild und anschließend auf Deckkraft.
3.  Wählen Sie die gewünschte Deckkraft aus.

### Segmenterfassung für Experten

Mit dieser Funktion können Sie das Wertefenster bei der Segmenteingabe verändern (Handeingabe von Geraden- und Bogensegment).
*   ⇨Tutorial, "Wertefenster (D)" auf Seite A-25

#### Segmente erfassen

1.  Aktivieren Sie Segmenterfassung für Experten. Markieren Sie dazu im Menü Ansicht > Einstellungen den Eintrag Segmenterfassung für Experten. A+W CAD Designer (Shapes) zeigt einen Haken vor dem Eintrag, wenn die Funktion aktiv ist.
2.  Erfassen Sie Segmente durch die Angabe von relativen Abständen, Längen, Winkeln usw. Löschen Sie dazu die Eingabefelder für nicht bekannte Größen (es darf kein Leerzeichen enthalten sein). Gehen Sie wie folgt vor:
    *   **Geradensegmente (Typ 1):**
        Lassen Sie die Felder für X2 und Y2 leer und geben Sie für dx und dy den relativen Abstand zum Startpunkt des Segments ein. Sie können aber auch X2 angeben, Y2 leer lassen und dy vorgeben. A+W CAD Designer (Shapes) errechnet dann die Strecke, deren Endpunkt die X-Koordinate X2 und die Y-Koordinate Y1+dy hat.
    *   **Längen und Winkeln:**
        Auch bei der Eingabe von Längen und Winkeln können Sie Angaben kombinieren. Wenn Sie z. B. dx und dis angeben, dann bestimmt A+W CAD Designer (Shapes) den Endpunkt im horizontalen Abstand dx vom Anfangspunkt, wobei die Länge des konstruierten Segmentes dis ist.
        Bei der Eingabe von Winkeln können Sie mit `<1` den Winkel zum vorhergehenden Segment oder mit `_` den Winkel zur horizontalen Achse angeben, jeweils in Grad und in mathematisch positiver Orientierung (im Uhrzeigersinn ist negativ, gegen den Uhrzeigersinn ist positiv).
    *   **Bögen:**
        Sinngemäß gelten die vorherigen Hinweise auch für die Eingabe von Bögen. Dabei wird wie zuvor beschrieben zunächst der Endpunkt des Bogens bestimmt. Dann können Sie wahlweise den Radius r, die Bogenhöhe h oder die Bogenlänge l angeben, um den Bogen endgültig zu beschreiben.
3.  Bestätigen Sie Ihre Eingaben mit [OK].

# Help Cards

## Informationen zu den Helpcards

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W CAD Designer (Shapes) 2014. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

### In diesem Kapitel finden Sie folgende Informationen:

*   ⇨ Informationen zu den Helpcards
*   ⇨ Geometrien erstellen
*   ⇨ Bearbeitungen
*   ⇨ Form mit Wölbung u. Randausschnitt

| Thema | Seite |
| :--- | :--- |
| Informationen zu den Helpcards | A-529 |
| **Geometrien erstellen** | **A-530** |
| Rechteck mit abgeschnittener Ecke | A-531 |
| Pfeil erstellen | A-532 |
| Abgewandeltes Parallelogramm | A-533 |
| Rechteck schräge Kante runde Ecke | A-534 |
| Form erstellen, vermaßen u. speichern | A-535 |
| Trapez erstellen und speichern | A-536 |
| Form erstellen und spiegeln | A-537 |
| Form erstellen und spiegeln | A-538 |
| **Bearbeitungen** | **A-539** |
| Form m. fehlender Ecke u. Ausschnitt | A-540 |
| Form m. runder Ecke u. Ausschnitt | A-541 |
| Rechteck mit Bogen | A-542 |
| Form mit Wölbung u. Randausschnitt | A-543 |
| **Makros und Templates** | **A-544** |
| Symmetrisches Marko erstellen | A-545 |
| Unsymmetrisches Makro erstellen | A-546 |
| Template erstellen | A-547 |
| Makro in Template einfügen | A-548 |
| Parametrisches Makro | A-549 |

## Geometrien erstellen

| Help Card | Themen |
| :--- | :--- |
| Rechteck mit abgeschnittener Ecke | Rechteck mit abgeschnittener Ecke erstellen und vermaßen. |
| Pfeil erstellen | Die Form eines Pfleils erstellen und vermaßen |
| Abgewandeltes Parallelogramm | Die Form eines abgewandelten Parallelogramms erstellen und vermaßen. |
| Rechteck schräge Kante runde Ecke | Die Form eines Rechtecks mit einer schrägen Kante und einer Runden Ecke erstellen und vermaßen. |
| Form erstellen, vermaßen u. speichern | Ein Rechteck mit Bogen oben erstellen, vermaßen und speichern. |
| Trapez erstellen und speichern | Ein Trapez erstellen, vermaßen und speichern. |
| Form erstellen und spiegeln | Form zur Hälfte erstellen und spiegeln. |
| Form erstellen und spiegeln | Form zur Hälfte erstellen und spiegeln. |

### Shp 01-001: Rechteck mit abgeschnittener Ecke

#### Ziel der Handlung

Rechteck mit abgeschnittener Ecke erstellen und vermaßen.

#### Voraussetzungen

(Keine)

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die Form in der Ansicht **Skizze**.
2.  Vermaßen Sie die Geraden.
3.  Definieren Sie die rechten Winkel. In der Ecke erscheint das Symbol ⦛.
4.  Für die Eckabschnitte wählen Sie das Werkzeug zum Vermaßen des Abstandes zwischen einem Punkt und einer Strecke.
5.  Über die Funktion **Neu zeichnen** (Ansicht > Neu zeichnen oder über `<Strg>+<D>`) prüft A+W CAD Designer (Shapes) ob die Form berechnet werden kann oder nicht.

### Shp 01-002: Pfeil erstellen

#### Ziel der Handlung

Die Form eines Pfeils erstellen und vermaßen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die Form in der Ansicht **Skizze**.
2.  Vermaßen Sie die einzelnen Geraden.
3.  Definieren Sie die rechten Winkel.
4.  Wählen Sie das Werkzeug zum Vermaßen des Innenwinkels zwischen zwei Segmenten.
5.  Lassen Sie A+W CAD Designer (Shapes) die Form neu berechnen.

### Shp 01-003: Abgewandeltes Parallelogramm

#### Ziel der Handlung

Die Form eines abgewandelten Parallelogramms erstellen und vermaßen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die Form in der Ansicht **Skizze**.
2.  Vermaßen Sie die einzelnen Geraden.
3.  Wählen Sie das Werkzeug zum Vermaßen des Abstands zwischen zwei Punkten parallel zu einer Strecke.
    *   Markieren Sie den linken Punkt der oberen Gerade. Dieser wird in roter Farbe dargestellt. Markieren Sie den unteren Punkt der linken Schräge. Dieser wird in grüner Farbe dargestellt. Markieren Sie die untere Gerade. Diese wird in grauer Farbe dargestellt. Es öffnet sich das Wertefenster. Geben Sie im Wertefenster unter `P=` die Länge von **2099** ein. Betätigen Sie die Schaltfläche [OK].
4.  Zum Vermaßen der rechten Schräge wählen Sie das Werkzeug zum Vermaßen des Abstands zwischen einem Punkt und einer Strecke.
5.  Wählen Sie das Werkzeug zum Vermaßen des Innenwinkels zwischen zwei Segmenten.
6.  Lassen Sie A+W CAD Designer (Shapes) die Form neu berechnen.

### Shp 01-004: Rechteck schräge Kante runde Ecke

#### Ziel der Handlung

Die Form eines Rechtecks mit einer schrägen Kante und einer Runden Ecke erstellen und vermaßen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die Form in der Ansicht **Skizze**.
2.  Vermaßen Sie die einzelnen Geraden.
3.  Vermaßen Sie die Schräge.
4.  Wählen Sie das Werkzeug um den Radius eines Bogens zu vermaßen.
    *   Markieren Sie den Bogen. Es öffnet sich das Wertefenster. Geben Sie im Wertefenster unter `R=` den Radius von **200** ein. Betätigen Sie die Schaltfläche [OK].
5.  Wählen Sie das Werkzeug um die Bogensegmente glatt anzuschließen.
    *   Markieren Sie den Bogen. Dieser färbt sich rot. Markieren Sie die linke Gerade. Diese färbt sich grün. Betätigen Sie die Schaltfläche [OK]. Das Segment wird glatt angeschlossen. Wiederholen Sie den Vorgang mit der oberen Gerade.
6.  Wählen Sie das Werkzeug um zwischen zwei geraden Segmenten einen rechten Winkel festzulegen (auf beiden Seiten).
7.  Lassen Sie A+W CAD Designer (Shapes) die Form neu berechnen.

### Shp 01-005: Form erstellen, vermaßen u. speichern

#### Ziel der Handlung

Ein Rechteck mit Bogen oben erstellen, vermaßen und speichern.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die Form mit Gerade und Bogen.
2.  Vermaßen Sie den Abstand der Geraden und des Bogens.
3.  Schließen Sie alle Bogensegmente glatt an.
4.  Vermaßen Sie die beiden senkrechten Segmente zueinander.
5.  Wechseln Sie in die Ansicht **Endprodukt**, um das Ergebnis zu überprüfen.
6.  Wählen Sie im Menü **Datei** den Menüpunkt **Speichern unter...**. Es öffnet sich der Dialog **Globale Formdaten**.
7.  Füllen Sie die Felder **Name** und **Text** aus.
8.  Schließen Sie den Dialog mit der Schaltfläche [OK]. Es öffnet sich der Dialog **Speichern unter...**
9.  Geben Sie einen Dateinamen ein und betätigen Sie die Schaltfläche [Speichern].

### Shp 01-006: Trapez erstellen und speichern

#### Ziel der Handlung

Ein Trapez erstellen, vermaßen und speichern.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Form erstellen, vermaßen u. speichern studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie ein Trapez.
2.  Vermaßen Sie die Form entsprechend der Aufgabenstellung.
3.  Schließen Sie alle Bogensegmente glatt an.
4.  Speichern Sie die Form als Datei.

### Shp 01-007: Form erstellen und spiegeln

#### Ziel der Handlung

Die neben stehende Form zur Hälfte erstellen und dann spiegeln.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die linke Hälfte der Form mit Gerade und Bogen.
2.  Die untere Gerade vermaßen Sie mit dem Wert **75**.
3.  Den Bogen vermaßen Sie mit dem Wert **75**.
4.  Schließen Sie die Bogensegmente glatt an.
5.  Wählen Sie das Werkzeug zum Vermaßen zweier Segmente parallel zueinander.
    *   Markieren Sie die obere Gerade. Diese färbt sich rot. Markieren Sie die untere Gerade. Diese färbt sich grün. Betätigen Sie die Schaltfläche [OK]. Unterhalb der oberen Geraden erscheint das Symbol **=**.
6.  Vermaßen Sie die beiden senkrechten Segmente zueinander.
7.  Wechseln Sie in die Ansicht **Geometrie**.
8.  Wählen Sie das Werkzeug zum Verdoppeln einer Kontur durch Spiegeln an einem Segment.
    *   Markieren Sie die senkrechte Gerade, an der gespiegelt werden soll. Diese färbt sich rot.
9.  Betätigen Sie die Schaltfläche [OK]. Die Kontur wird gespiegelt.

### Shp 01-008: Form erstellen und spiegeln

#### Ziel der Handlung

Die neben stehende Form zur Hälfte erstellen und dann spiegeln.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.
*   HelpCard Form erstellen und spiegeln studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die linke Hälfte der Form mit Geraden und 3 Bögen.
2.  Die untere Gerade vermaßen Sie mit dem Wert **18**.
3.  Die untere Gerade vermaßen Sie mit dem Wert **30**.
4.  Die obere Gerade vermaßen Sie mit dem Wert **6**.
5.  Die drei Bögen vermaßen Sie mit dem Wert **75**.
6.  Vermaßen Sie den Rest gemäß den neben stehenden Werten.
7.  Setzen Sie drei rechte Winkel.
8.  Schließen Sie die beiden Bogensegmente glatt an.
9.  Wechseln Sie in die Ansicht **Geometrie**.
10. Wählen Sie das Werkzeug zum Verdoppeln einer Kontur durch Spiegeln an einem Segment.
    *   Markieren Sie die senkrechte Gerade, an der gespiegelt werden soll. Diese färbt sich rot.
11. Betätigen Sie die Schaltfläche [OK]. Die Kontur wird gespiegelt.

## Bearbeitungen

| Help Card | Themen |
| :--- | :--- |
| Form m. fehlender Ecke u. Ausschnitt | Ein Rechteck mit abgeschnittener Ecke und Ausschnitt erstellen. |
| Form m. runder Ecke u. Ausschnitt | Ein Rechteck mit abgerundeten Ecken und Randausschnitt erstellen. |
| Rechteck mit Bogen | Ein Rechteck mit einem oben liegenden Bogen erstellen. |
| Form mit Wölbung u. Randausschnitt | Eine Form mit einer Wölbung und zwei Randausschnitten erstellen. |

### Shp 02-001: Form m. fehlender Ecke u. Ausschnitt

#### Ziel der Handlung

Ein Rechteck mit abgeschnittener Ecke und Ausschnitt erstellen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren und vermaßen Sie ein Rechteck mit einer schrägen Ecke.
2.  Wechseln Sie in die Ansicht **Innenkonturen**. Öffnen Sie im Menü **Datei** den Menüpunkt **Einfügen**. Wählen Sie die Datei der Übung **Shp 01-005** aus, die Sie gespeichert haben. Betätigen Sie die Schaltfläche [Öffnen]. Die Form wird platziert.
3.  Wählen Sie das Werkzeug zum Positionieren von Ausschnitten. Markieren Sie in der eingefügten Form die untere waagerechte Gerade in der Nähe des Segment-Endpunktes (rot mit kleinem Pfeil in Richtung Ende). Markieren Sie jetzt in dem skizzierten Rechteck den oberen Bereich der rechten Geraden (grün). Geben Sie im Wertefenster unter `D2=` den Abstand von **200** ein. Betätigen Sie die Schaltfläche [OK]. Unter `D1` bleibt der Wert 0 stehen, da D1 der parallele Abstand zur Ausschnittunterkante ist und diese aufeinander liegen sollen. Die eingefügte Datei wird in Form eines Innen-Ausschnitts platziert.
4.  Wählen Sie das Werkzeug zum Erfassen eines Bohrloches mit Vermaßung. Markieren Sie die linke Gerade (rot). Markieren Sie die untere Gerade (grün). Geben Sie im Wertefenster unter `D1=` den Abstand von **852** ein, unter `D2=` den Abstand von **102** und unter `o=` den Durchmesser von **34** ein. Betätigen Sie die Schaltfläche [OK]. Das Bohrloch wird platziert.
5.  Für das nächste Bohrloch markieren Sie wieder die linke Gerade (rot). Markieren Sie die untere Gerade (grün). Geben Sie im Wertefenster unter `D1=` den Abstand von **552** ein, unter `D2=` den Abstand von **102** und unter `o=` den Durchmesser von **34** ein. Betätigen Sie die Schaltfläche [OK]. Das Bohrloch wird platziert.
6.  Wählen Sie das Werkzeug zum Erfassen eines Bohrloches durch Handeingabe. Platzieren Sie das Bohrloch an der gewünschten Stelle.
7.  Wählen Sie das Werkzeug zum Vermaßen. Vermaßen Sie das Bohrloch.
8.  Wählen Sie das Werkzeug zum Vermaßen zweier Punkte parallel zu einer Strecke. Markieren Sie das linke Bohrloch (rot). Markieren Sie das mittlere Bohrloch (grün). Markieren Sie die untere Gerade (grau) und geben Sie im Wertefenster unter `D=150` ein. Markieren Sie den linken Punkt der Schräge und dann die obere waagerechte Gerade und geben Sie im Wertefenster unter `D=450` ein.
9.  Überprüfen Sie das Ergebnis.

### Shp 02-002: Form m. runder Ecke u. Ausschnitt

#### Ziel der Handlung

Ein Rechteck mit abgerundeten Ecken und Randausschnitt erstellen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren und vermaßen Sie ein Fünfeck.
2.  Wechseln Sie in die Ansicht **Geometrie**. Runden Sie die beiden Eckpunkte mit den Radien von je **75** ab.
3.  Wechseln Sie in die Ansicht **Skizze**. Öffnen Sie im Menü **Datei** den Menüpunkt **Einfügen**. Wählen Sie die Datei der Übung **Shp 01-006** aus, die Sie gespeichert haben. Betätigen Sie die Schaltfläche [Öffnen]. Die Form wird platziert.
4.  Wechseln Sie in die Ansicht **Geometrie**. Vermaßen Sie in der soeben platzierten Form die beiden oberen Bögen mit den Radien von je **25**.
5.  Wechseln Sie in die Ansicht **Innenkonturen**.
6.  Wählen Sie das Werkzeug zum Positionieren von Ausschnitten. Markieren Sie in der eingefügten Form die untere waagerechte Gerade in der Nähe des Segment-Startpunktes (rot mit kleinem Pfeil in Richtung Start).
    *   Markieren Sie jetzt in dem skizzierten Fünfeck die untere Geraden in der Nähe des Segment-Startpunktes (grün mit kleinem Pfeil in Richtung Start). Geben Sie im Wertefenster unter D1 und D2 die entsprechenden Abstände ein. Unter R1 und R2 können Sie gleich die Radien von 25 eingeben, damit die Ecken gerundet werden. Betätigen Sie die Schaltfläche [OK]. Die Form wird als Innenkontur platziert.
7.  Wechseln Sie in die Ansicht **Geometrie**. Wählen Sie das Werkzeug zum Abschneiden einer Ecke mit verschiedenen Abständen. Markieren Sie den Startpunkt und nehmen Sie die entsprechenden Eingaben vor. Wiederholen Sie den Vorgang mit unteren rechten Ecke.
8.  Wählen Sie das Werkzeug zum Runden von Ecken. Vermaßen Sie die noch fehlenden Bögen.
9.  Überprüfen Sie das Ergebnis.

### Shp 02-003: Rechteck mit Bogen

#### Ziel der Handlung

Ein Rechteck mit einem oben liegenden Bogen erstellen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren Sie die Hälfte der Form.
2.  Vermaßen Sie die Form.
3.  Wechseln Sie in die Ansicht **Geometrie**.
4.  Verdoppeln Sie die Form.
5.  Wechseln Sie in die Ansicht **Innenkonturen**.
6.  Überprüfen Sie das Ergebnis.
7.  Speichern Sie die Form.

### Shp 02-004: Form mit Wölbung u. Randausschnitt

#### Ziel der Handlung

Eine Form mit einer Wölbung und zwei Randausschnitten erstellen.

#### Voraussetzungen

*   HelpCard Rechteck mit abgeschnittener Ecke studiert.
*   HelpCard Pfeil erstellen studiert.
*   HelpCard Abgewandeltes Parallelogramm studiert.
*   HelpCard Rechteck schräge Kante runde Ecke studiert.

#### Zusatzinfo

Zur Erstellung und Vermaßung der gezeigten Form sind folgende Werkzeuge nötig.

#### Workflow

1.  Skizzieren und vermaßen Sie die Form.
2.  Öffnen Sie im Menü **Datei** den Menüpunkt **Einfügen**. Wählen Sie die Datei der Übung **Shp 02-003** aus, die Sie gespeichert haben. Betätigen Sie die Schaltfläche [Öffnen]. Die Form wird platziert.
3.  Wechseln Sie in die Ansicht **Innenkonturen**. Wählen Sie das Werkzeug zum Positionieren von Ausschnitten. Vergrößern Sie eventuell die Ansicht.
4.  Markieren Sie in der eingefügten Form die untere waagerechte Gerade in der Nähe des Segment-Startpunktes (rot mit kleinem Pfeil in Richtung Start).
5.  Markieren Sie jetzt in der skizzierten Form die rechte Geraden in der Nähe des Segment-Startpunktes (grün mit einem Pfeil in Richtung Start). Es öffnet sich das Wertefenster. Geben Sie unter D1 den Wert **0** und D2 den Wert **205** ein. R1 und R2 bleiben leer. Betätigen Sie die Schaltfläche [OK]. Die Form wird als Innenkontur platziert.
6.  Öffnen Sie im Menü **Datei** den Menüpunkt **Einfügen**. Wählen Sie die Datei der Übung **Shp 02-003** aus, die Sie gespeichert haben. Betätigen Sie die Schaltfläche [Öffnen]. Die Form wird platziert.
7.  Wechseln Sie in die Ansicht **Innenkonturen**. Wiederholen Sie die Schritte 3, 4 und 5. Achten Sie auf die korrekten Maße.
8.  Überprüfen Sie das Ergebnis.

## Makros und Templates

| Help Card | Themen |
| :--- | :--- |
| Symmetrisches Marko erstellen | Makro Symmetrischer Randausschnitt erstellen und speichern. |
| Unsymmetrisches Makro erstellen | Makro Unsymmetrischer Randausschnitt erstellen und speichern. |
| Template erstellen | Template Tür erstellen und speichern. |
| Makro in Template einfügen | Symmetrisches Makro einfügen. |
| Parametrisches Makro | Parametrisches Makro erstellen. |

### Shp 03-001: Symmetrisches Marko erstellen

#### Ziel der Handlung

Makro Symmetrischer Randausschnitt erstellen und speichern.

#### Voraussetzungen

*   Sie wissen, wie eine Form gezeichnet und vermaßt wird.
*   Sie wissen, wie Bearbeitungen platziert und vermaßt werden.

#### Workflow

1.  Zeichnen und vermaßen der Form in der Ansicht **Skizze**.
2.  Zwei Bohrlöcher in der Ansicht **Innenkonturen** mit entsprechenden Werten platzieren.
3.  Form gruppieren: Beide Bohrlöcher markieren und ein Segment der Form. Über **Transformieren > Gruppieren** die Form gruppieren. Um die Gruppierung sichtbar zu machen, im Wertefenster unter `<=`, `>=`, `^=` und `v=` jeweils **10 mm** eintragen. Ein umschreibendes Rechteck wird platziert. Der Pfeil, der an der unteren Seite des umschreibenden Rechtecks zu sehen ist, kennzeichnet den Referenzpunkt und die Referenzseite.
4.  Den Referenzpunkt verlegen, so dass er sich mittig auf einer Seite befindet und nicht an einer Ecke. Dazu das Werkzeug **Segment halbieren** auswählen, die linke Seite des Gruppierungsrechtecks anklicken und [OK] drücken. Danach ist das Segment in zwei gleich lange Teile zerlegt. Den Vorgang für die rechte Seite wiederholen.
5.  Anschließend beide Punkte durch eine Hilfslinie (Werkzeug: **Neue Hilfslinie**) miteinander verbinden.
6.  Das Werkzeug **Referenzsegment setzen** aktivieren und an der linken Seite des Gruppierungsrechtecks die obere Hälfte des Segments nahe dem Halbierungspunkt anklicken. Das Segment färbt sich rot und hat einen Pfeil in Richtung Halbierungspunkt. Klicken Sie [OK], wird das neue Referenzsegment platziert.
7.  Im nächsten Schritt das Gruppierungsrechteck wieder der Form anpassen. Dazu eine beliebige Linie des Gruppierungsrechtecks markieren und im Wertefenster die Werte `<=`, `>=`, `^=` und `v=` von 10 mm auf **0 mm** ändern. Der Referenzpunkt und das Referenzsegment dienen der späteren Erfassung und Vermaßung im ERP-System.
8.  Die Datei speichern unter **Datei > Speichern unter ...**. Es öffnet sich der Dialog **Globale Formdaten**. Bitte keine Umlaute und keine Leerzeichen verwenden.

### Shp 03-002: Unsymmetrisches Makro erstellen

#### Ziel der Handlung

Makro Unsymmetrischer Randausschnitt erstellen und speichern.

#### Voraussetzungen

*   Sie wissen, wie eine Form gezeichnet und vermaßt wird.
*   Sie wissen, wie Bearbeitungen platziert und vermaßt werden.

#### Workflow

1.  Zeichnen und vermaßen der Form in der Ansicht **Skizze**.
2.  Zwei Bohrlöcher in der Ansicht **Innenkonturen** mit entsprechenden Werten platzieren.
3.  Form gruppieren: Bohrloch markieren und ein Segment der Form. Über **Transformieren > Gruppieren** die Form gruppieren. Um die Gruppierung sichtbar zu machen, im Wertefenster unter `<=`, `>=`, `^=` und `v=` jeweils **10 mm** eintragen. Ein umschreibendes Rechteck wird platziert. Der Pfeil, der an der unteren Seite des umschreibenden Rechtecks zu sehen ist, kennzeichnet den Referenzpunkt und die Referenzseite.
4.  Den Referenzpunkt verlegen, so dass er sich unten rechts in der Ecke befindet. Dazu das Werkzeug **Referenzsegment setzen** aktivieren und die rechte untere Ecke des Gruppierungsrechtecks anklicken. Das Segment färbt sich rot und hat einen Pfeil in Richtung Eckpunkt. Klicken Sie [OK], wird das neue Referenzsegment platziert.
5.  Im nächsten Schritt das Gruppierungsrechteck wieder der Form anpassen. Dazu eine beliebige Linie des Gruppierungsrechtecks markieren und im Wertefenster die Werte `<=`, `>=`, `^=` und `v=` von 10 mm auf **0 mm** ändern. Der Referenzpunkt und das Referenzsegment dienen der späteren Erfassung und Vermaßung im ERP-System.
6.  Die Datei speichern unter **Datei > Speichern unter ...**. Es öffnet sich der Dialog **Globale Formdaten**. Bitte keine Umlaute und keine Leerzeichen verwenden.

### Shp 03-003: Template erstellen

#### Ziel der Handlung

Template Tür erstellen und speichern.

#### Voraussetzungen

*   Sie wissen, wie eine Form gezeichnet und vermaßt wird.
*   Sie wissen, wie Bearbeitungen platziert und vermaßt werden.

#### Workflow

1.  Zeichnen und vermaßen der Form in der Ansicht **Skizze**.
2.  Zwei Bohrlöcher (für Randaufhängung) in der Ansicht **Innenkonturen** mit folgenden Werten platzieren:
    *   Abstand von der oberen und unteren Kante: BohrlochHoehe=150
    *   Abstand von der linken Kante: 100
3.  Ein Bohrloch (für Türgriff) mit folgenden Werten platzieren:
    *   Abstand von der rechten Kante: 100
    *   Abstand von der unteren Kante: TuergriffHoehe=1000
4.  In der Ansicht **Kantenbearbeitung** alle Kanten säumen.
5.  In der Ansicht **Schneiden (einzeln)** alle Bruchränder entfernen, da diese im Produktionsplanungs-System in den Stammdaten hinterlegt sind. Dazu die gestrichelte Linie anklicken, im Wertefenster das Symbol der geschlossenen Faust anklicken. Die Faust öffnet sich zu einer Hand. Dann können die Werte im Bereich `<=`, `>=`, `^=` und `v=` auf **0** gesetzt werden.
6.  Die Datei speichern unter **Datei > Speichern unter ...**. Es öffnet sich der Dialog **Globale Formdaten**. Namen für Template-Dateien müssen mit **T_** beginnen (bspw. T_Tuer). Bitte keine Umlaute und keine Leerzeichen verwenden. Die Datei im Ordner **Templates** speichern, sonst wird sie als solche nicht erkannt!

### Shp 03-004: Makro in Template einfügen

#### Ziel der Handlung

Symmetrisches Makro einfügen.

#### Voraussetzungen

*   Sie wissen, wie eine Form gezeichnet und vermaßt wird.
*   Makro Symmetrischer Randausschnitt ist vorhanden.

#### Workflow

1.  Zeichnen und vermaßen der Form in der Ansicht **Skizze**.
2.  Das Makro **Symmetrischer Randausschnitt** zweimal für die Türaufhängungen platzieren (**Datei > Einfügen**). Einmal für die obere Türaufhängung und einmal für die Untere.
3.  In die Ansicht **Innenkonturen** wechseln, um die Randausschnitte zu platzieren. Ein Segment des Randausschnittes markieren, über **Transformieren > Verschieben** den einen Randausschnitt oben links und den anderen Randausschnitt unten links positionieren. In Bezug auf die anschließende Vermaßung ist es ratsam, die Randausschnitte links **außerhalb** der Form zu platzieren und nicht **innerhalb**, wo sie eigentlich hingehören!
4.  Zum Platzieren der Randausschnitte wird das Werkzeug **Ausschnitt in Form einfügen** aktiviert. Platzieren Sie erst den unteren Randausschnitt, indem Sie das Referenzsegment des Randausschnitts anklicken (Pfeil färbt sich rot) und den linken Rand der Tür im unteren Bereich (Pfeil färbt sich grün). Im Wertefenster geben Sie für **D1** (horizontal) den Wert **0** und für **D2** (vertikal) den Wert **100** ein. Wiederholen Sie diese Vorgehensweise für den oberen Randausschnitt.
5.  Platzieren Sie noch ein Bohrloch für den Türgriff.
6.  Säumen Sie alle Kanten.
7.  Entfernen Sie die Bruchränder.
8.  Die Datei speichern unter **Datei > Speichern unter ...**. Es öffnet sich der Dialog **Globale Formdaten**. Namen für Template-Dateien müssen mit **T_** beginnen (bspw. T_TuerRandausschnitt). Bitte keine Umlaute und keine Leerzeichen verwenden. Die Datei im Ordner **Templates** speichern, sonst wird sie als solche nicht erkannt!

### Shp 03-005: Parametrisches Makro

#### Ziel der Handlung

Parametrisches Makro erstellen.

#### Voraussetzungen

*   A+W CAD Designer (Shapes) (Shapes) ab Version 5.5.
*   Sie wissen, wie man eine Form gruppiert und den Referenzpunkt verlegt.

#### Zusatzinfo

*   Interne Variablen beginnen mit einem Unterstrich, z. B. **_D** und dienen der Berechnung der Form.
*   Restriktionen beginnen mit **_TEST** und dienen dazu, Einschränkungen zu beschreiben.

#### Workflow

1.  Zeichnen der Form in der Ansicht **Skizze**.
2.  Die Vermaßung ist wie folgt:
    *   Höhe: H=100, Breite: B=50, Sehne: H=100 und Bogenhöhe: B/2
3.  Zwei Bohrlöcher in der Ansicht **Innenkonturen** mit folgenden Werten platzieren.
    *   Durchmesser: R=20
4.  Um sicherzustellen, dass der Bohrlochrand immer auf Höhe des Sehnenrandes liegt, wird für diesen Wert eine Variable erfasst. Öffnen Sie im Menü **Bearbeiten** den Eintrag **Variablen editieren**. Der Dialog **Variablen bearbeiten** wird geöffnet. Für diese Form befinden sich bereits drei Einträge im Dialog (H, B und R). Klicken Sie auf **[Neu]**, gehen Sie in die nächste freie Zeile und geben Sie im Bereich Namen **_D** ein. Im Bereich Ausdruck geben Sie **B/2+R/2** ein. Der Bereich Wert wird automatisch gefüllt, nachdem Sie auf [Übernehmen] geklickt haben. Für unser Beispiel bedeutet das:
    *   Bogenhöhe = 50, B/2 = 25
    *   Radius = 20, R/2 = 10
    *   25 + 10 = 35.
    Aktivieren Sie das Werkzeug **Paralleler Abstand** und geben Sie bei `P=` **_D** ein. Wiederholen Sie die Prozedur für das zweite Bohrloch.
5.  Darüber hinaus wollen wir sicherstellen, dass die Höhe immer zweimal die Breite ist. Die entsprechende Beschreibung ist: Höhe minus zweimal die Breite ist gleich Null. Um dies abzubilden lautet die Formel: **H-2*B**. Klicken Sie erneut auf [Neu]. Da es sich hierbei um eine Restriktion handelt, geben Sie im Bereich Namen **_TEST** ein und im Bereich Ausdruck **H-2*B**. Da H=100 ist und B=50, ist der Eintrag im Feld Wert 0. Schließen Sie den Dialog.
6.  Gruppieren Sie die Form. Der Wert **fix** darf nicht aktiv sein!
7.  Verlegen Sie den Referenzpunkt wie in der Grafik zu sehen ist.
8.  Das Gruppierungsrechteck wieder der Form anpassen.
9.  Die Datei speichern.
