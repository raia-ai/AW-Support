---
title: "DE-HB-AWEnterprise_11"
source: "DE-HB-AWEnterprise_11.pdf"
tags: ["A+W Enterprise", "Verkauf", "Auftragserfassung", "Stückliste", "Sprossenerfassung", "Produktaustausch", "Preislose Erfassung", "Tutorial", "Software Referenz", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein umfassendes deutsches Handbuch für das Vertriebsmodul der A+W Enterprise Software. Es enthält einen Tutorial-Teil mit schrittweisen Anleitungen für wichtige Aufgaben wie Auftragserfassung und Stücklistenverwaltung sowie einen detaillierten Software-Referenzteil, der alle Funktionen und Dialoge systematisch beschreibt."
long_description: "Dieses Dokument dient als umfassende Anleitung für das Modul „Verkauf“ der A+W Enterprise Software. Es gliedert sich in zwei Hauptteile: ein „Tutorial“ und eine „Softwarereferenz“. Der Tutorial-Abschnitt bietet praktische, schrittweise Anleitungen zur Durchführung wesentlicher Aufgaben. Dazu gehören das Erstellen und Verwalten von Aufträgen („Aufträge“), die Bearbeitung von Auftragspositionen („Positionserfassung“), das Erstellen und Ändern von Stücklisten („Stückliste“), die Verwaltung von Sprossen („Sprossenerfassung“) und die Durchführung von Produktaustauschen. Es werden auch spezielle Funktionen wie iTOE (integrierte CAD-basierte Positionserfassung) und die Verarbeitung von Stufenglas („Stufenerfassung“) behandelt. Der Abschnitt „Softwarereferenz“ bietet eine systematische und detaillierte Beschreibung aller Funktionen, Dialoge und Felder innerhalb des Vertriebsmoduls und dient als technisches Nachschlagewerk. Es enthält detaillierte Beschreibungen von Suchfunktionen, administrativen Aufgaben und verschiedenen Datenverwaltungsmenüs. Diese Anleitung richtet sich an Benutzer von A+W Enterprise, um die Fähigkeiten der Software zu erlernen und als Referenz für spezifische Funktionen und Verfahren zu dienen."
---

# A+W Enterprise Verkauf: Tutorial

---
## Aufträge

A+W Enterprise öffnet einen Dialog für die Texteingabe.
3. Geben Sie den Text ein oder wählen Sie einen Textbaustein (den Sie als vorformulierten Text in den Stammdaten hinterlegt haben) aus der Auswahlliste aus.
4. Beenden Sie die Texteingabe mit `<Ende>`.

### So legen Sie neue Textbausteine (Floskeln) an oder ändern diese
Sie können eigene Textbausteine (Floskeln) anlegen oder vorhandene nach Ihren Wünschen ändern.

⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-1313

Starten Sie den Dialog **Kopftext** oder **Fußtext** über das `<F4>` - Menü.

1. Wenn Sie einen neuen Textbaustein in den Stammdaten anlegen möchten, betätigen Sie im Dialog **Kopftext** oder **Fußtext** `<Shift>` + `<F10>` bzw. nutzen Sie die Schaltfläche `[Floskeln neu]`.
   A+W Enterprise öffnet einen Eingabedialog.
2. Geben Sie eine neue Kennung ein und bestätigen Sie mit `<Enter>`. Die Kennung der Floskel kann sowie numerisch als auch alphanumerisch sein.
3 sobern Sie den Text für den neuen Textbaustein ein oder ändern Sie den vorhandenen Text und bestätigen Sie mit `<Enter>`.
4. Verlassen Sie den Dialog mit `<Ende>`.

### Zusatz-Dokumente im Auftrag

Sie können einem Auftrag, oder nur einzelne Positionen daraus, Dokumente zuordnen bzw. diese anhängen, z. B. eingescannte Handskizzen, CAD-Zeichnungen, Notizen, E-Mails oder Ähnliches. Diese können auch wieder entfernt werden.

> **Information zur Datenspeicherung**
> Achten Sie darauf, dass der Dateiname keine Sonder- und Leerzeichen enthält. Ansonsten wird die Datei nicht im Vorgang gespeichert.

⇨ Verkauf, "Dokumentenartenzuordnung" auf Seite D-1225

**So ordnen Sie Dokumente zu**
1. Um Dateien zuzuordnen, betätigen Sie `<Strg>` + `<K>`
	- ab Feld **Kdn-Pos** der Kopfdaten oder/und in den Fußdaten, wenn Sie einem Auftrag eine Datei zuordnen möchten.
	- in den Rumpfdaten, Register **Allgemein**, in der entsprechenden Position, wenn Sie einer einzelnen Position eine Datei zuordnen möchten.
A+W Enterprise öffnet den Dialog **Dateizuordnung**:

*(Screenshot des Dialogs "Dokumentenartenzuordnung" wird angezeigt)*

2. Öffnen Sie den (Windows) Explorer und markieren Sie die gewünschte Datei.
3. Ziehen Sie mit der Maus diese Datei auf das Ordnersymbol im Dialog **Dateizuordnung** und drücken Sie die Schaltfläche `[OK]`.
   Der Dateiname und die zugeordnete Position werden im Dialog **Dateizuordnung** angezeigt und sind in der Datenbank gespeichert.
   Wenn Sie weitere Dateien zuordnen möchten, wiederholen Sie den Vorgang.
4. Nach der Zuordnung kann sich das Symbol des Ordners ändern, je nachdem, welche Symbole für die Standardanwendungen auf Ihrem Computer verwendet werden.
5. Um eine Datei aus einem Vorgang zu entfernen, markieren Sie den entsprechenden Eintrag und drücken Sie die Schaltfläche `[Entfernen]`.
   Die Datei wird aus dem Vorgang entfernt.

### Auftragserfassung abschließen

Sobald alle Kunden- und Positionsdaten erfasst sind, kann der Auftrag abgeschlossen werden.

Durch **Speichern** verlässt der Auftrag die Erfassung und die Daten werden für andere A+W Enterprise-Komponenten (Produktion, Bestellwesen, Lager und Versand) aufbereitet und an diese übergeben.

**So speichern oder verwerfen Sie einen Auftrag**
1. Bestätigen Sie die Eingabe im Feld **Nettototal** mit `<Enter>` oder verlassen Sie den Additionsbereich mit `<Ende>`.
   Soll der Auftrag nicht abgespeichert werden, drücken Sie mehrfach die Taste `<Pos1>`, um alle Eingaben zu verwerfen.
2. Beantworten Sie die Abfrage, ob der Auftrag komplett ist, mit `[JA]`.
3. Beantworten Sie die Abfrage, ob der Auftrag zur Weiterverarbeitung freigeschaltet werden soll mit `[JA]`, um die Daten sofort an Produktion, Bestellwesen, Lager und Versand weiterzuleiten.
Wenn Sie diese Frage mit `[Nein]` beantworten, wird der Auftrag nicht freigegeben. Der Auftrag ist gespeichert und befindet sich im Freischaltepool. Sie können den Auftrag später freigeben.

### Auftragsänderung/Korrektur durchführen

Zur nachträglichen Auftragsänderung gehören alle Änderungen nach dem erstmaligen Speichern des Auftrags. Es ist empfehlungswert, alle Änderung im Auftrag durchzuführen, solange der Auftrag noch nicht in lokaler Korrektur gesperrt wird. Wenn Sie jedoch Änderungen bis zu einem gewissen Grad zulassen möchten, sprechen Sie einen A+W Mitarbeiter an, um Ihr System entsprechend zu konfigurieren.
Bitte beachten Sie, dass es Änderungen gibt, die nur in den einzelnen Positionen erfolgen und Änderungen, die auf Auftragskopf-Ebene erfolgen. Änderungen auf Kopfebene bewirken, dass die Änderungsart auf alle nicht stornierte Positionen übertragen wird, wenn die Klasse der Änderung höher ist als die eventuell vorhandene in der Position. Wird z. B. in einer Position die Menge verändert und nachträglich die Lieferadresse, so bekommen alle nicht geänderte Positionen den Status „Info an Produktion" (kpos.aendkz=4) und die eine geänderte Position dann „produktionsrelevante Änderung“ (kpos.aendkz=5).

Folgende Kapitel setzen voraus, dass die Auftragsänderungen zulässig sind:
- Verkauf, "So fügen Sie eine zusätzliche Positionen ein" auf Seite D-1009
- Verkauf, "So bearbeiten Sie die Eigenschaften einzelner Positionen" auf Seite D-1009
- Verkauf, "So ändern Sie lieferantenbezogene Daten" auf Seite D-1010
- Verkauf, "So können Sie einen Artikel in der Stückliste ändern" auf Seite D-1019

Es ist möglich, Aufträge im Modus **Korrektur** und **lokale Korrektur** zu ändern.
Nicht möglich ist eine Änderung im Modus **Globale lokal Korrektur**, **Storno** (System- oder Benutzer) und **Fakturiert**.

Bei jeder Auftragsänderung führt A+W Enterprise eine Limitprüfung sowie eine Prüfung des Deckungsbeitrags durch.
In der Regel wird der Auftragserfasser (kauf.eusr) über die Änderung informiert. Wenn Sie den E-Mail-Versand konfigurieren, bekommt der Mitarbeiter eine E-Mail.

Im Weiteren kann das System so konfiguriert werden, dass Auftragsänderungen, die durch das System vorgenommen werden, wie z. B., Liefertermin-Verschiebung, oder fehlerhafte Einlastung) nicht an den Auftragserfasser gehen, sondern an den Mitarbeiter, der die letzte Änderung am Auftrag vorgenommen hat. Dadurch wird die Informationskette übersichtlicher gestaltet.

**So ändern Sie einen bestehenden Auftrag**
1. Rufen Sie den gewünschten Auftrag auf.
	- Geben Sie die Auftragsnummer ein, wenn diese bekannt ist.
	- Oder suchen Sie den Auftrag.
	⇨ Verkauf, "Übersicht" auf Seite D-1049
2. Ändern Sie die entsprechenden Felder im Auftrag.
   Wenn beispielsweise der Liefertermin geändert wird, wird das Feld **Grund** temporär geöffnet. Geben Sie hier die Begründung für die Lieferterminverschiebung ein.
3. Verlassen Sie den Auftrag mit `<Ende>`.
4. Führen Sie gegebenenfalls eine neue Packmittelplanung durch.
   ⇨ Verkauf, "Vorgaben Packmittelplanung" auf Seite D-1295
5. Beantworten Sie den Hinweis **Soll die Änderung an Einkauf, Lager und Produktion übergeben werden?** mit `Ja` oder `Nein` und entscheiden so, ob die Änderung weitergegeben werden muss.

> **Beantworten Sie diesen Hinweis bewusst!**
> Bei allen einkaufs-, lager- und produktionsrelevanten Änderungen müssen Sie diesen Hinweis mit `[Ja]` beantworten.
>
> Beachten Sie, dass beispielsweise geänderte oder hinzugefügte Positionen im Vorgang nicht an die Produktion übergeben werden, wenn Sie diese Frage mit `[Nein]` beantworten. Der Vorgang wird dann nicht dem System übergeben und nicht in den Freischaltepool gestellt!

**So können Sie Lieferterminänderungs-Protokoll ansehen**
Mit `<Shift>` + `<F4>` können Sie zur Überprüfung den Menüpunkt **Lieferterminänderungen** öffnen. Im Dialog **Lieferterminänderungs-Protokoll** werden alle Änderungen angezeigt. Die neueste Änderung wird erst nach Abspeichern und wieder Öffnen des Vorgangs angezeigt.
⇨ Verkauf, "Lieferterminänderungs-Protokoll" auf Seite D-1232

**So kalkulieren Sie einen Auftrag erneut**
Bei geänderten Zahlungsbedienungen kann es vorkommen, dass ein bestehender Auftrag erneut kalkuliert werden muss. Diese Möglichkeit setzt voraus, dass der gewünschter Auftrag noch nicht fakturiert ist. Sollten Sie mehrere Aufträge gleichzeitig erneut zur Kostenkalkulation vorlegen wollen, nutzen Sie die Funktion im Dialog **Vorgangsänderung**:
⇨ Verkauf, "So lassen Sie einen Angebot oder einen Auftrag neue kalkulieren" auf Seite D-1057

1. Rufen Sie den gewünschten Auftrag auf.
	- Geben Sie die Auftragsnummer ein, wenn diese bekannt ist.
	- Oder suchen Sie den Auftrag.
	⇨ Verkauf, "Übersicht" auf Seite D-1049
2. Gehen Sie mit dem Cursor in eines der folgenden Felder **Erf. Datum**, **Knd-Bestnr**, **Termin**, **Route** oder **Knd-Pos**.
3. Mit `<Strg>` + `<F9>` können Sie die Neukalkulation des Vorgangs veranlassen. Sie können zwischen:
	- Keine Kalkulation
	- Verkaufspreise
	- Einkaufspreise
	- Verkaufs- und Einkaufspreise
wählen.
4. Anschließend muss der Vorgang speichernd (mit `<Ende>`) verlassen werden.

## Positionserfassung

> **Lernziele**
> - Diverse Funktionen auf der Positionsebene kennenlernen.
> - Möglichkeiten und Restriktionen der Positionserfassung beachten.
> - Handlungsschritte der Funktionen auf der Positionsebene kennenlernen.
>
> **Nutzen**
> - Die Funktionen auf der Positionsebene dienen zur schnelleren und sicheren Auftragserfassung. Auf der Positionsebene werden einzelne Produkte erfasst, die der Kunde bestellt. Die Vermeidung von Erfassungsfehlern reduzieren mögliche Fehlproduktionen.
>
> **Merke**
> - **Stückliste editieren**: Diese Funktion bietet die Möglichkeit, bei Bedarf Änderungen an der bestehenden Stückliste vorzunehmen. Sie können diese Funktion zwar direkt nach der Eingabe der Artikelnummer mit `<F5>` aufrufen, jedoch wird die Stücklistenstruktur erst nach der vollständigen Bemaßung editiert.
> - **Anhänge(1)**: In einem Vorgang auf Kopf-/Fußebene und auch auf Positionsebene können Dokumente mit `<Strg>` + `<K>` zugeordnet werden. Die Schaltfläche **Anhänge(X)** zeigt mit einer Zahl in Klammern pro Ebene an, wie viele Dokumente bereits zugeordnet sind. Mit dieser Schaltfläche kann auch die Dokumentenzuordnung gestartet werden.

Die Erfassung der einzelnen Auftragspositionen erfolgt nach dem selben Schema.
⇨ Verkauf, "Auftragspositionen" auf Seite D-1167

Die Merkmale der Erfassung unterschiedlicher Produktarten (z. B.: Basisgläser, ESG, VSG, ISO, Sprossen, Bearbeitungen Beschläge, Dienstleistungen, etc.), finden Sie in folgendem Kapitel:
⇨ Verkauf, "Positionen erfassen (nach Produktart)" auf Seite D-1013

Umfangreiche oder komplexe Themenblöcke werden in separaten Kapiteln beschrieben, z. B.:
⇨ Verkauf, "iTOE - Erfassung und Nachbearbeitung" auf Seite D-1031
⇨ Verkauf, "Produktaustausch" auf Seite D-1035

### Neue Positionen anlegen

**So erfassen Sie eine Position nach Kundenbezeichnung**
Es kann eine vom Kunden vorgegebene Positionsbezeichnung erfasst werden, wenn im Feld **Kdn-Pos** in den Kopfdaten der Eintrag **Pos.** ausgewählt wurde.
⇨ Verkauf, "Knd-Pos" auf Seite D-1138

1. Geben Sie im Feld **Ku. Pos** den neuen Positionstext ein.
   Der Text kann über die sichtbare Feldlänge hinausgehen. Es kann sich dabei um einen freien Text handeln.
2. Bestätigen Sie die Eingabe mit `<Enter>`.
   Der Cursor springt in das Feld **Artikel**.

**So erfassen Sie eine Position mit Artikelnummer**

*(Screenshot des Positionserfassungs-Dialogs)*

Hier erfassen Sie die einzelnen Artikel (Positionen) des Auftrags.
Der Cursor befindet sich im Feld **Artikel** in der Auftragserfassung. Die Bezeichnungen für Felder, die beim Betreten des Dialoges nicht vorhanden sind, werden dynamisch, je nach Eigenschaften des erfassten Artikels eingeblendet, z. B., für ein 2fach ISO-Artikel heißen die Felder **Breite/Höhe/SZR**.

1. Geben bzw. wählen Sie den Artikel wie folgt aus:
	- Geben Sie im Feld **Artikel** eine Artikelnummer ein, wenn diese bekannt ist.
	- Oder betätigen Sie die Taste `<F9>`, um die Suche über die Artikelnummer oder anderen Kriterien zu starten.
	- Oder betätigen Sie die Taste `<F8>`, um die Suche über den Matchcode zu starten.
	⇨ Verkauf, "Artikel-Suche" auf Seite D-1101
	- Wählen Sie den gewünschten Artikel mit den `<Pfeiltasten>` + `<F3>` oder mit der Maus aus.
	- Bestätigen Sie die Eingabe mit `<Enter>` oder einem Doppelklick.
	Die Positionserfassung nach bestimmten Produktgruppen entnehmen Sie folgendem Kapitel:
	⇨ Verkauf, "Positionen erfassen (nach Produktart)" auf Seite D-1013
	Betätigen Sie `<Enter>`, um den Cursor in das Feld **Menge** zu bewegen.
2. Wenn Sie in Verbindung mit SN-Auto arbeiten, folgt die Abfrage: **Möchten Sie die SN-Datei für die Position vom System generieren lassen?**
	- Wählen Sie `[JA]`, wenn A+W Enterprise eine SN-Datei im Hintergrund erzeugen soll.
	- Wählen Sie `[NEIN]`, wenn keine SN-Datei benötigt wird oder wenn Sie SN direkt in der Auftragserfassung starten möchten.
3. Geben Sie im Feld **Menge** die Stückzahl ein und entscheiden Sie, ob Sie den Produktaufbau in der Stückliste ändern möchten.
   Der Cursor springt in das Feld **Breite**.
4. Wenn Sie mit der iTOE arbeiten, beachten Sie folgende Beschreibung:
   ⇨ Verkauf, "Stufenerfassung" auf Seite D-1028
5. Geben Sie **Breite** und **Höhe** ein und bestätigen Sie jeweils mit `<Enter>`.
   Bei ISO-Gläsern muss zusätzlich das Feld **SZR** (Scheibenzwischenraum) gefüllt werden.
6. A+W Enterprise öffnet den Dialog **Bearbeitungen**, wenn Sie Produkte erfasst haben, die mit Bearbeitungen versehen sind. Alternativ können Sie an den gewünschten Artikel zusätzliche Bearbeitungen manuell anbringen:
   ⇨ Verkauf, "Komplexe Handlungsschritte im Stücklisteneditor" auf Seite D-1020
   Spezifizieren Sie die gewählten Bearbeitungen in diesem Dialog.
   Sie können den Dialog **Bearbeitungen** mit `<Strg>` + `<F8>` aus den Feldern **Breite**, **Höhe** oder **Preis/Stück** nachträglich immer wieder aufrufen.
7. Die Sprossenerfassung entnehmen Sie folgendem Kapitel:
   ⇨ Verkauf, "Sprossenerfassung" auf Seite D-1024
8. Die Stufenerfassung entnehmen Sie folgendem Kapitel:
   ⇨ Verkauf, "Stufenerfassung" auf Seite D-1028
9. Die Stücklisten-Nachbearbeitung entnehmen Sie folgendem Kapitel:
   ⇨ Verkauf, "Stückliste bearbeiten" auf Seite D-1016
10. Das Feld **Prov** ist bereits aus den Stammdaten vorbelegt, sofern Sie mit dem Provisionsabrechnung innerhalb der A+W Enterprise - Programm arbeiten. In diesem Fall können Sie den Provisionsschlüssel mit `<F9>` ändern. Ansonsten wird das Feld übersprungen.
   ⇨ Stammdaten, "Provisionen" auf Seite B-510
11. Das Feld **B.Art** ist ebenfalls bereits aus den Stammdaten vorbelegt. Sie können die Beschaffungsart auftragsbezogen ändern. Dafür betätigen Sie die `<Leertaste>`, bis Sie den gewünschten Wert erreichen und bestätigen Sie die Auswahl mit `<Enter>`. Beachten Sie jedoch dabei, dass die Änderung der Beschaffungsart diverse andere Änderungen nach sich zieht und eventuell auch andere Angaben erforderlich macht.
   Anschließend rechnet A+W Enterprise die Werte für die Felder **ME/St** und **kg/St** sowie die Preisangaben aus und fügt diese in die Position ein.
12. Schließen Sie die Position im Feld **Preis/Stück** wie folgt ab:
	- Mit `<Enter>` oder `<F6>`, wenn Sie weitere Positionen erfassen möchten.
	- Mit `<Ende>`, um den Auftrag zu speichern und zu den Fußdaten zu wechseln.
	- Legen Sie den Artikel als festbemaßtes Kundenprodukt an, wenn Ihr Kunde öfter Artikel mit den selben Maßen bestellt.
	  ⇨ Verkauf, "Artikelangaben für bemaßte Varianten" auf Seite D-1217

Darüber hinaus fordert A+W Enterprise notwendige Schritte an entsprechender Stelle an. Dies können Bearbeitungsparameter (wie Bohrdurchmesser, Rundeckradien o. ä.) bei bearbeiteten Gläsern sein oder die gewünschte Farbe bei farbigen Artikeln.

Üblicherweise reichen für die Erfassung die Daten im Register **Allgemein** aus, da alle anderen Angaben von A+W Enterprise aus den Stammdaten entnommen werden.

### So fügen Sie eine zusätzliche Positionen ein
Sie können in einem Auftrag nachträglich neue Positionen einfügen. In der Regel werden die Positionen am Ende der bereits erfassten Positionen hinzugefügt. In seltenen Fällen können Sie neue Positionen auch zwischen bereits vorhandene Positionen einfügen. In diesem Fall muss beachten werden, dass die Positionsnummer (kpos.posnr) nicht mehr aufsteigend vergeben wird und die laufende Nummer (kpos.lfdpos, Register Allgemein > Feld Pos) erneut durchnummeriert wird. Das gleiche Nummernvergabe-Verfahren gilt auch bei stornierten Positionen.
1. Platzieren Sie den Cursor im Register **Allgemein** in der Zeile, vor der eine neue Position eingefügt werden soll.
2. Betätigen Sie die Taste `<F6>`, um eine neue Position am Ende der bereits erfassten Positionen einzufügen.
3. Betätigen Sie die Tasten `<Shift>` + `<F6>`, um eine Position zwischen bereits erfassten Positionen einzufügen.
4. Erfassen Sie die neue Position.
   ⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007

### So bearbeiten Sie die Eigenschaften einzelner Positionen
Manche Details einer erfassten Position können auftragsbezogen geändert werden. So können Sie z. B. die Artikelbezeichnung oder Kostenstelle im Register **Eigenschaften** nachträglich bearbeiteten.
⇨ Verkauf, "Auftragspositionen - Eigensch." auf Seite D-1180
1. Drücken Sie auf der Positionsebene im Register **Allgemein** `<F2>`.
   Das Register **Eigenschaften** wird angezeigt. A+W Enterprise belegt die Felder mit Daten aus dem Artikelstamm oder der vorhandenen Systemkonfiguration vor.
2. Drücken Sie `<F5>`, um die Felder im Register **Eigenschaften** zu betreten.
3. Führen Sie die Änderung durch. Beachten Sie dabei die möglichen Folgen der durchgeführten Korrektur:
	- Die geänderte **Bezeichnung** wird an die Produktion übergeben und auf die relevanten Papieren gedruckt.
	- Die geänderte **Kostenstelle** wirkt sich auf die Kostenstellen-Statistik aus.
	- Bei lagerführenden Artikeln wird die **Lagerentnahme** im Änderungsfall aus einem anderen Lager erfolgen.
	- Im Feld **CAD-Datei** können Sie eine neue S/N-/oder DXF-Datei anhängen (mit `<F9>`). Durch diese Änderung kann die Stückliste angepasst werden. Dafür müssen Sie die Frage, ob die Stückliste synchronisiert werden soll mit `Ja` beantworten.
	- Je nach Systemkonfiguration können Sie im Feld **LE-Nummer** eine neue Leistungserklärung aus den Stammdaten ermitteln (`<Strg>` + `<R>`), laut Aufbau erstellen (`<Strg>` + `<L>`), mittels Eingabe von erweiterten technischen Werten erzeugen (`<Strg>` + `<T>`) oder frei wählen (`<F9>`/`<Strg>` + `<K>`).
	- Die Änderung durch eine Systemkonfiguration-Vorbelegung **Skizzendruck-Wertes** führt zur Änderung der Formulare.
4. Mit `<Ende>` kehren Sie in das Register **Allgemein** zurück.
   Oder betätigen Sie `<F2>`, um in weitere Register zu wechseln.
   Oder wählen Sie `<Bild-runter>` - Taste, um in die nächste Position in den Register **Eigenschaften** zu gelangen.

### So ändern Sie lieferantenbezogene Daten
Sie können bei einer bestehenden Position den Lieferanten und die Lieferzeit nachträglich ändern. Wenn Sie einen Lieferanten für eine bereits erfasste Position neu eingeben, so wird die Beschaffungsart dieser Position automatisch auf Bestellung umgesetzt. Auch umgekehrt wird die Angabe des Lieferanten angefordert, sofern die Positionsbeschaffungsart auf Bestellung umgesetzt wird.
1. Nach der Artikelnummer-Angabe können Sie im Register **Allgemein** aus jedem Feld `<Shift>` + `<F12>` betätigen.
   Die Felder **Lieferant** und **Lief.zeit** werden temporär eingeblendet.
2. Geben Sie den Lieferanten ein oder wählen Sie ihn mit `<F9>` aus der Liste aus.
3. Geben Sie die Lieferzeit im Feld **Lief.zeit** ein. Über eine entsprechende Systemkonfiguration bestimmen Sie, ob diese Angabe in Tagen oder in Stunden erfolgt.
4. Beantworten Sie die nachfolgenden Fragen mit `[Ja]` oder `[Nein]`.
	- „Wollen Sie den Vorgang neu kalkulieren?"
	- Die Art der Kalkulation, die durchgeführt werden kann. Folgende Auswahl ist über die `[Leertaste]` möglich.
		- Keine Neukalkulation
		- Verkaufs- und Einkaufspreise
		- Verkaufspreise
		- Einkaufspreise
	- Wollen Sie den Lieferant für den gesamten Auftrag übernehmen?
		- Alle bisher erfassten Positionen mit Beschaffungsart **Bestellung** bekommen diesen Lieferanten, sofern Sie diese Frage mit `[Ja]` beantworten. Anschließend bekommen Sie die nächste Frage gestellt:
	- Wollen Sie den neuen Lieferanten nur in die Bestellposition übernehmen?
		- Beantworten Sie diese Frage mit `[Ja]`, wird der neue Lieferant nur in Positionen übernommen, deren Beschaffungsart=Bestellung ist.
		- Beantworten Sie diese Frage mit `[Nein]` wird der neue Lieferant in alle Positionen übernommen und die Beschaffungsart aller Position wird auf Bestellung umgestellt.
	- Wollen Sie den neuen Lieferanten nach unten vererben?
		- Der neue Lieferant wird auch in die neu erfassten Positionen übernommen.
5. Schließen Sie die Positionserfassung ab.

### So erfassen Sie in der Position ein Modell
Sie können in der Position eine Modellscheibe erfassen. Üblicherweise werden Modelle bei einem neuen Auftrag erfasst. Nachträgliche Änderung für eine bestehende Position zu einem Modell ist nur solange möglich, bis die Produktion begonnen hat. Beachten Sie, dass Modellinformationen auch die Gestellplanung beeinflusst.
1. Drücken Sie im Register **Allgemein** `<Strg>` + `<F12>`.
   Das Feld **Modell** wird temporär eingeblendet.
2. Geben Sie die Modellnummer ein.
   Oder drücken Sie im Feld **Modell** `<F9>` und wählen Sie das gewünschte Modell aus der Liste aus.
   Oder drücken Sie im Feld **Modell** `<F2>` und wählen Sie ein Modell aus dem Dialog **Modelle** aus.
   Ein Erfassungsdialog für die ausgewählte Modellnummer startet automatisch.

> **Modellkatalog**
> Mithilfe einer Systemeinstellung wird bestimmt, welcher Modellkatalog im Gesamtprogramm zur Verfügung steht. Die Standardeinstellung ist der A+W Modellkatalog. Um eventuell einen anderen Katalog zu konfigurieren, sprechen Sie bitte einen zuständigen A+W - Mitarbeiter an. Das Betreiben mehrerer Kataloge ist nicht möglich.

3. Geben Sie die Maße des Modells im Dialog **Modell-Maßangaben** ein.
4. Um ein Modell geometrisch darstellen oder auch produzieren zu können, sind diverse Einschränkungen pro Modell vorhanden. z. B., `W2 + W1 >= W`.
   Wenn Sie mit den Maßangaben die Modellrestriktion verletzt haben, wird ein Hinweis ausgegeben. Sie müssen die Angabe korrigieren, um den Dialog verlassen zu können.
5. Die Modellnummer wird in die Position übernommen. In dem Bereich der Skizzen wird eine schematische Modelldarstellung eingeblendet. Die Position enthält ein Modellsymbol.

*(Screenshots des Dialogs Modell-Maßangaben und der Auftragserfassung mit Modellsymbol)*

6. Schließen Sie die Positionserfassung ab.

## Positionen erfassen (nach Produktart)
Es gibt einige Besonderheiten bei der Erfassung mancher Produktarten. Die Positionserfassung wird von einer Reihe verschiedener Kriterien bestimmt, z. B. wie viele Parameter und welche Parameter für die Erfassung notwendig sind, oder in welchen Mengeneinheiten das Produkt verkauft bzw. produziert wird, usw. In den folgenden Kapitel erfahren Sie einige bestimmte Besonderheiten bei Positionserfassung.

### So erfassen Sie lagerführende Artikeln mit Maß- oder Farbvarianten
Die Lagerplatten eines bestimmten Glases sind in Form von Lagermaßvarianten im Artikelstamm hinterlegt. Alle zur Verfügung stehenden Maßvarianten einer bestimmten Glasart mit gleicher Glasstärke sind unter derselben Artikelnummer zusammengefasst. Die im System verfügbaren Maßvarianten sind in folgendem Kapitel beschrieben:
⇨ Stammdaten, "Maßvarianten" auf Seite B-299

Die Farbvarianten sind in den Regel ebenfalls lagerführend. Z. B. eine rote Farbe ist in Eimer mit 5 Liter, 10 Liter und 15 Liter vorhanden. Die Dialogbeschreibung finden Sie unter:
⇨ Stammdaten, "Farbvarianten" auf Seite B-296

Die Beschreibung der Größenvarianten ist ebenfalls in den Stammdaten verfügbar:
⇨ Stammdaten, "Größenvarianten" auf Seite B-302

Die Erfassung aller lagerführenden Variantenartikeln unterscheidet sich von der Glaserfassung dadurch, dass hier noch ein zusätzliches Feld für die Auswahl der Variante eingeblendet wird.
1. Starten Sie die Auftragserfassung und erfassen Sie den Auftrag bis zum Feld **Artikel** (Positionsebene).
2. Geben Sie im Feld **Artikel** eine Artikelnummer für die Lagermaße des gewünschten Gläsertyps ein.
   Oder wählen Sie einen Artikel über `<F9>` Selo aus. Es gibt keine Möglichkeit im Dialog **Artikel-Suche** nur nach Varianten (Maß-, Groß-, Farb)-Artikeln zu suchen. Eine Abhilfe könnte die Filterung nach passende Artikeltypen sein, z. B, Lagermaß-Artikeltypen.
3. Nach der Mengeneingabe öffnet sich ein Auswahldialog mit den zur Verfügung stehenden Lagermaßvarianten.

*(Screenshot des Dialogs "Variantenauswahl")*

In diesem Dialog wird der Lagerbestand für alle verfügbaren Artikelvarianten über alle Lagerräume summiert angezeigt. Negativer Bestand bedeutet, dass mehr Ausgänge als Eingänge aktuell im System gebucht sind.
Wählen Sie eine gewünschte Lagermaßvariante und bestätigen Sie die Auswahl mit `<Enter>`.
Der Lagerbestand wird jedoch nicht von Position zur Position aktualisiert. Die Abbuchungen vom Lager finden erst, wenn der Lagerbucher die Abarbeitung beendet hat.
A+W Enterprise übernimmt die Maße für die ausgewählte Variante in die Felder **Breite** und **Höhe**.
4. Setzen Sie die Positionserfassung wie gewohnt fort.

### So erfassen Sie ein Float bzw. Basisglas
Als Float bzw. Basisglas sind die Glasartikel mit Artikeltyp 100, 170 oder 180 gekennzeichnet. Erfassen Sie die Position, wie im Kapitel
⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007
beschrieben. Beachten Sie dabei nachfolgende Abweichungen:
Es gibt unterschiedliche Möglichkeiten, Basisglas (Float) zu erfassen:
- **Als Lagermaß**
  ⇨ Verkauf, "So erfassen Sie lagerführende Artikeln mit Maß- oder Farbvarianten" auf Seite D-1013
- **Als unbearbeitetes Festmaß**
	- Wählen Sie einen Artikel aus. Alternativ starten Sie die `<F9>` - Suche und filtern alle Artikel mit dem Artikeltyp=170 aus.
	- Geben Sie die Menge ein.
	- Bestimmen Sie Breite und Höhe.
- **Als bearbeitetes Festmaß**
	- Wählen Sie einen Artikel aus. Alternativ starten Sie die `<F9>` - Suche und filtern alle Artikel mit dem Artikeltyp=100 aus.
	- Fügen Sie die Bearbeitungen hinzu.
	- Geben Sie die Menge ein.
	- Erfassen Sie die Maße.

### So erfassen Sie ein ESG (Einscheiben-Sicherheits-Glas)
Erfassen Sie die Position, wie im Kapitel Tutorial, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007 beschrieben. Beachten Sie dabei nachfolgende Abweichungen.
Es gibt unterschiedliche Möglichkeiten, ESG zu erfassen:
- **Als unbearbeitetes ESG**
	- Wählen Sie einen Artikel aus.
	- Geben Sie die Menge ein.
	- Bestimmen Sie Breite und Höhe.
- **Als veredeltes (bearbeitetes) ESG**
	- Wählen Sie einen Artikel aus.
	- Fügen Sie die Bearbeitungen hinzu.
	- Geben Sie die Menge ein.
	- Erfassen Sie die Maße.

### So erfassen Sie ein VSG (Verbund-Sicherheits-Glas) erfassen
Die Erfassung von Auftragspositionen aus dem Produktbereich VSG unterscheidet sich kaum von der Basisglaserfassung. Besonderheiten können sich aus der Verwendung farbiger Folien ergeben, die in die Stückliste eingebracht werden können.

> **Achten Sie auf die Scheibeneinbauposition**
> Bei mehrscheibigen Sicherheitsgläsern werden die Scheibenoberflächen von außen nach innen durchgezählt (= Scheibeneinbauposition). Beachten Sie die Scheibeneinbauposition, wenn Sie die Stückliste anpassen.

Erfassen Sie VSG, wie unter folgendem Punkt beschrieben:
⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007

### So erfassen Sie ein ISO (Isolierglas)
Isoliergläser haben eine hohe Produktvielfalt. Die Produkte können aus den verschiedenen Glastypen (Float, ESG, VSG) und unterschiedlichen Scheibenstärken zusammengestellt werden. Grundsätzlich unterscheidet sich die Erfassung von Isoliergläsern nicht von der Erfassung anderer Produktgruppen.

Erfassen Sie Isoliergläser, wie unter folgendem Punkt beschrieben:
⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007
Sie können zusätzlich Sprossen in den ISO-Gläsern erfassen.
⇨ Verkauf, "So führen Sie die Sprossenerfassung" auf Seite D-1025

### So erfassen Sie einen Stückartikel bzw. Volumenartikel
Bei der Erfassung von Stückartikeln sind keine Maße notwendig.
Erfassen Sie Stückartikel, wie unter folgendem Punkt beschrieben:
⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007

### So erfassen Sie einen Stundenartikel (Arbeitszeit)
Bei der Erfassung von Stundenartikeln ist der Eintrag im Feld **Menge** der Multiplikator. Die Einheit wird in Stunden erfasst.
Erfassen Sie Stundenartikel, wie unter folgendem Punkt beschrieben:
⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007

### So erfassen Sie einen Farbartikel
Die Erfassung von einem Farbartikel unterscheidet sich von der Erfassung der Variantenartikeln nur in der Auswahl der Farb- statt Maßvariante.

## Stückliste bearbeiten

> **Lernziele**
> - Stücklistenkonzept kennenlernen.
> - Möglichkeit, die Stückliste kundenindividuell anzupassen.
> - Vereinfachung der Bedienung erfahren.
>
> **Nutzen**
> - Eine kundenindividuelle Anpassung des Produktaufbaus kann direkt im Auftrag vorgenommen und kalkuliert werden.
>
> **Merke**
> - **Original-Stückliste**: Produktaufbau, der in den Stammdaten festgelegt werden kann.
> - **Akt. Stückliste**: Wenn die Stückliste aus mehreren Ebenen bestehet, sehen Sie in dem ersten Register des Stücklistendialoges die Auflistung der jeweils aktuellen Ebene.
>   ⇨ Verkauf, "Register Bearbeitungsparameter (kurz)" auf Seite D-1264
> - **Bearbeitungsparameter (kurz)**: In dem zweiten Register des Stücklistendialoges sehen Sie die Darstellung wichtiger Bearbeitungsparameter, die in der Regel auch änderbar sind. Welche Parameter hier angezeigt werden, ist unter anderem von dem Bearbeitungstyp abhängig. Eine komplette Auflistung aller Parameter für die jeweilige Bearbeitung finden Sie im `[F5]`-Dialog.
>   ⇨ Verkauf, "Register Alle Parameter/Skizze" auf Seite D-1266

Um individuelle Kundenwünsche bei der Vorgangserfassung berücksichtigen zu können, wird die Originalstückliste automatisch in den Vorgang übernommen und kann anschließend auftragsspezifisch verändert werden, ohne dass Rückwirkungen auf die Originalstückliste entstehen. So können z. B. Gläser ausgetauscht, zusätzliche Bearbeitungen eingefügt, alternative Materialien gewählt werden etc. Alle Änderungen an der Stückliste beziehen sich dann auf diese Kopie. Die Originalstückliste bleibt in den Stammdaten immer erhalten.

Ob der Stücklistenbaum bei der Vorgangserfassung geändert werden darf oder nicht, kann im Artikelstamm gekennzeichnet werden und hängt zusätzlich von den individuellen Rechten des Erfassers ab. Wenn die Änderung erlaubt ist, kann in dieser Stückliste eine Baugruppe durch eine andere gleichwertige Baugruppe ersetzt oder weitere gleichwertige Baugruppen hinzugefügt werden.

Die Stücklistenstruktur einer Position wird automatisch auf die nachfolgende Position vererbt, wenn Sie die gleiche Positionsnummer eingeben. Die Stücklistennummer kann geändert werden. Sie können die Stückliste auch anzeigen und bearbeiten.
⇨ Stammdaten, "Stückliste" auf Seite B-485

Alle Änderungen an der Stückliste müssen sorgfältig durchgeführt werden. Fehlerhafte Handlungen können zu weiteren Problemen bis hin zum Programmabsturz führen.

Das Kapitel Stücklisten bearbeiten umfasst folgende Informationen:
⇨ Verkauf, "Allgemeine Arbeitsschritte in der Stückliste" auf Seite D-1018
⇨ Verkauf, "Komplexe Handlungsschritte im Stücklisteneditor" auf Seite D-1020

### Allgemeine Arbeitsschritte in der Stückliste
Die Stückliste einer Position können Sie fast in jeder Vorgangsart ansehen. Dazu müssen Sie den Stücklisteneditor der gewünschten Position starten:
⇨ Verkauf, "So markieren Sie die Stückliste für die Bearbeitung" auf Seite D-1018

Inwiefern die Stückliste jedoch bearbeitet und die Änderungen gespeichert werden können, ist von unterschiedlichen Kriterien abhängig, wie z. B. Benutzerrechte, Artikel-Stammdaten, Vorgangsart und Vorgangsstatus.

**So markieren Sie die Stückliste für die Bearbeitung**
Um den Stücklisteneditor öffnen zu können, muss der erfasste Artikel vollständig vermaßt werden. Bei der Vermaßung ermittelt das Programm automatisch relevante Parameter und schreibt diese in die Auftragsstückliste. Solange diese Vermaßung nicht abgeschlossen ist, kann der Stücklisteneditor zum Öffnen nur markiert werden. Dies ist der Fall, wenn sich der Cursor in der Auftragserfassung im Feld **Menge** der zu ändernden Position befindet:

1. Rufen Sie mit `<F3>` die Stückliste auf, um sie anzusehen.
   A+W Enterprise gibt Ihnen den Hinweis, dass die Stückliste nun für die Bearbeitung markiert ist und der Stücklisteneditor wird nach dem vollständigen Vermaßen geöffnet. Nach der Eingabe der notwendigen Parameter, wie z. B., **Breite/Höhe/SZR** öffnet das Programm die Stücklistendarstellung.
   ⇨ Verkauf, "Stücklistendarstellung" auf Seite D-1252
2. Wählen Sie den Artikel aus, den Sie ändern möchten. Klappen Sie gegebenenfalls mit `<F3>` oder per Mausklick auf den Plus-Knoten weitere Stücklistenebenen auf.
3. Betätigen Sie `<F5>`, um die Stückliste der gewünschten Stücklistenebene zur Bearbeitung zu öffnen.
   A+W Enterprise öffnet den Stücklisteneditor.

**So öffnen Sie den Stücklisteneditor oder die Stücklistendarstellung direkt**
Sie können den Stücklisteneditor in folgenden Fällen direkt öffnen:
- Mit `[F5]` aus den Feldern **SN**, **Prov** (Provision), **B.Art** (Beschaffungsart)
- Mit `[F5]` aus den Feldern **Menge**, **Breite**, **Höhe**, (**SZR**), wenn die Position schon komplett erfasst war.

Das gleich gilt für die Stücklistendarstellung, die über `[F3]` erreichbar ist.
Mit `<F2>` wechseln Sie im Stücklisteneditor jeweils in das nächste Register.
⇨ Stammdaten, "Stückliste" auf Seite B-485

**So können Sie einen Artikel in der Stückliste ändern**
Sie können noch während der Auftragserfassung, d. h., solange der Auftrag noch nicht gespeichert ist, Änderungen an den Positionen bzw. Produktaufbau vornehmen.
Änderungen in einem bereits gespeicherten Auftrag nehmen Sie in Form einer Auftragskorrektur vor.
⇨ Verkauf, "Auftragsänderung/Korrektur durchführen” auf Seite D-1003

1. Öffnen Sie die den Stücklisteneditor.
   ⇨ Verkauf, "So markieren Sie die Stückliste für die Bearbeitung" auf Seite D-1018
2. Überschreiben Sie die Artikelnummer im Feld **Artikel** mit der neuen Artikelnummer oder wählen Sie eine Artikelnummer mit `<F9>` aus. Das Programm setzt im Feld **Druck** automatisch das Kennzeichen **A** (Austausch). Dieses Kennzeichen kann Auswirkungen auf den Positionspreis haben.

> **Nur gleiche Artikelarten gegeneinander austauschen**
> Sie können Artikel nur gegen Artikel der gleichen Art austauschen.
> Beispiel: Ein Glas gegen eine Bearbeitung auszutauschen, ergibt keinen Sinn. Im Artikelstamm müssen entsprechende technische Restriktionen hinterlegt sein, damit A+W Enterprise in diesem Fall eine Warnmeldung einblendet.
> ⇨ Stammdaten, "Artikel" auf Seite B-377

3. Bestätigen Sie die neue Artikelnummer mit `<Enter>`.
   A+W Enterprise aktualisiert die Bezeichnung und alle weiteren Felder.
4. Schließen Sie den Dialog mit `<Ende>`, wenn Sie alle Änderungen vorgenommen haben und diese speichern möchten. Um die Änderungen zu verwerfen, drücken Sie `<Pos1>`.

**So können Sie einen neuen Artikel der Stückliste hinzufügen**
Sie können bei Bedarf auch neue Artikel der Stückliste hinzufügen.
1. Öffnen Sie die den Stücklisteneditor.
   ⇨ Verkauf, "So markieren Sie die Stückliste für die Bearbeitung" auf Seite D-1018
2. Navigieren zur der Stücklistenebene, in welche einen Zusatzartikel hinzugefügt werden soll.
3. Mit `[F6]` hängen Sie eine neue Zeile in diese Stücklistenebene.
4. Geben Sie im Feld **Artikel** die Nummer des neuen Artikels ein, falls Sie diese zur Hand haben. Alternativ wählen Sie die Nummer aus dem `[F9]`-Selo aus.
   Wenn mehrere vollständig erfasste Artikel (z. B. Bearbeitungen) hinzugefügt werden sollen, bietet das Programm weitere Schritte zur Vereinfachung der Eingabe an, die im nächsten Kapitel beschrieben werden.
5. Schließen Sie den Dialog mit `<Ende>`, wenn Sie alle Änderungen vorgenommen haben und diese speichern möchten. Um die Änderungen zu verwerfen, drücken Sie `<Pos1>`.

### Komplexe Handlungsschritte im Stücklisteneditor
Das A+W Enterprise bietet eine Reihe Möglichkeiten, schneller komplexe Änderung der Stückliste vorzunehmen. Bitte beachten Sie, dass einige hier beschriebenen Schritte eventuell konfigurationsabhängig sind. Sprechen Sie gegebenenfalls den zuständigen A+W - Mitarbeiter an.

**So fügen Sie zusätzlichen Artikel an der gewünschten Stelle der Stückliste ein**
Sie können neue Datensätze in die Stückliste auch an eine bestimmte Stelle einfügen. Die Reihenfolge der Artikel kann von Bedeutung sein, wenn z. B. die Bearbeitungen auf einer Produktionsmaschine nacheinander basieren.

1. Öffnen Sie den Stücklisteneditor.
   ⇨ Verkauf, "So markieren Sie die Stückliste für die Bearbeitung" auf Seite D-1018
2. Positionieren Sie den Cursor in einem Stücklisten-Satz so, dass ein neuer Artikel oberhalb dieses Datensatzes eingefügt werden kann:
   Drücken Sie `<Umschalt>` + `F6>`
   Der neue Satz wird oberhalb der Markierung hinzugefügt.
   Sie können den neuen Zusatzartikel nun erfassen.

> **Reihenfolge der Artikel in der Stückliste**
> Die Reihenfolge der Stücklistenartikeln entspricht nicht zwangsläufig dem fertigungsspezifischen Ablauf. ERP- und Produktionssysteme müssen auch aufeinander abgestimmt werden.

3. Speichern Sie die Stückliste mit `<Ende>`. Unter Umständen wird dabei eine neue Stücklistenummer vergeben.

**So kopieren Sie bereits erfasste Artikel**
Oft kommt es vor, dass in einer Stückliste mehrere nahezu identische Bearbeitungen erfasst werden müssen, die sich nur in einem Parameter unterscheiden. In solchen Fällen kann es sinnvoll sein, die betreffende Bearbeitung einmal vollständig zu erfassen, sie dann mehrfach zu kopieren und jeweils den betreffenden Parameter zu ändern.

1. Öffnen Sie den Stücklisteneditor.
   ⇨ Verkauf, "So markieren Sie die Stückliste für die Bearbeitung" auf Seite D-1018
2. Fügen Sie eine neue Bearbeitung in die Stückliste ein.
3. Bleiben Sie mit dem Cursor in dem Datensatz der Bearbeitung stehen.
4. Betätigen die Schaltflächen **Kopie** (sollten die Schaltflächen zur Stücklistenbearbeitung nicht sichtbar sein, müssen diese entsprechend konfiguriert werden).
5. Legen Sie einen neuen Datensatz an: mithilfe der Schaltfläche **Neu** oder mit `<F6>`.
6. Betätigen Sie die Schaltfläche **Einfg** (Einfügen). Die betroffene Bearbeitung wird mit allen Parametern hinzugefügt.

> **Geltungsbereich der Zwischenablage**
> Bitte beachten Sie, dass der kopierte Artikel nur solange zur Verfügung steht, wie Sie sich in dem Stücklisteneditor befinden. Verlassen Sie die Stückliste, wird die Zwischenablage geleert. Wenn Sie jedoch den kopierten Artikel in eine andere Stücklistenebene einfügen möchten, folgen Sie den Programmhinweisen und weiteren Beschreibungen:
> ⇨ Verkauf, "So kopieren Sie bereits erfasste Bearbeitungen in eine andere Stücklistenebene" auf Seite D-1022

7. Speichern Sie die Stückliste mit `<Ende>`. Unter Umständen wird dabei eine neue Stücklistenummer vergeben.

**So lassen Sie die Stücklistennummer vom System ändern**
Sie haben die Möglichkeit, einem Artikel eine neue Stücklistennummer bei gleichem Stücklistenaufbau zuzuordnen. Dies ist beispielsweise sinnvoll, wenn für diese Position Artikeltexte erneut gedruckt oder geänderte Artikeltexte gedruckt werden sollen.

1. Um die Stücklistennummer zu ändern, geben Sie im Register **Allgemein** in der betreffenden Position im Feld **SL** eine neue Stücklistennummer ein.
   Oder drücken Sie im Register **Allgemein** in der betreffenden Position im Feld **Artikel**, **SL** oder **Menge** `<Umschalt>` + `<F5>`.
   Die Stücklistennummer wird geändert.

**So weisen Sie einer neuen Position wieder die Original-Stückliste**
Wenn Sie eine weitere neue Position erfassen, können Sie dieser wieder die Original-Stückliste aus den Stammdaten zuweisen.

1. Um die Original-Stückliste zuzuweisen, drücken Sie im Register **Allgemein** in der neuen Position im Feld **Artikel** `<F5>`.
   Die Original-Stückliste wird der neuen Position zugewiesen.

> **Original-Stückliste für bereits erfasste Positionen**
> Einer bereits erfassten Position kann man die Original-Stückliste nicht mehr zuweisen, da das Feld **Artikel** nicht mehr betretbar ist.

**So kopieren Sie die komplett erfasste Bearbeitung auf ein anderes Glas**

*(Screenshot der Stücklistendarstellung mit mehreren Ebenen und Markierungen)*

Sie können eine komplett erfasste Bearbeitung auf ein anderes Glas in der Stückliste übertragen. Auf diese Art und Weise können Sie gleichzeitig mehrere Bearbeitungen in der Stückliste von einer Ebene in die Andere einfügen, um z. B. mehrere Bearbeitungen mit vielen Parametern einfacher und schneller zu erfassen.
Oft kommt es auch vor, dass man mehrere fast gleiche Bearbeitungen in einer Stückliste erfassen muss, die sich nur in einem Parameter unterscheiden. In solchen Fällen kann es hilfreich sein, die betreffende Bearbeitung einmal vollständig zu erfassen, danach mehrfach zu kopieren und anschließend den betreffenden Parameter jeweils zu ändern.
Für die beiden Anwendungsfälle bietet A+W Enterprise folgende Erfassungshilfen:

**So kopieren Sie bereits erfasste Bearbeitungen in eine andere Stücklistenebene**
1. Öffnen Sie den Stücklisteneditor.
2. Fügen Sie eine neue Bearbeitung in die Stückliste ein, erfassen Sie diese Bearbeitung vollständig.
3. Sie können mehrere Bearbeitungen zunächst vollständig erfassen, um diese dann gemeinsam in ein anderes Glas zu übertragen.
4. Wechseln Sie mit `<F2>` in das Register **Bearbeitungsparameter (kurz)**.
5. Markieren Sie die Bearbeitungen, die übertragen werden sollen, durch Aktivieren der Checkboxes **Kop** (Kopieren) bei den betreffenden Bearbeitungen (diese Funktion muss vorerst freigeschaltet werden).
6. Kopieren Sie die Bearbeitungen mithilfe der Schaltfläche `[Kopie]` oder per Tastenkombination `<Strg>` + `<B>`. Die Änderungen an Parametern, die nun vorgenommen werden, werden nicht mehr für das Übertragen vorgesehen.
   Wenn Sie die Bearbeitungen nur markieren und nicht kopieren, so werden Sie beim Wechseln der Stücklistenebenen darauf hingewiesen.
7. Wechseln Sie in die Stücklistenebene, wohin die markierten Bearbeitungen übertragen werden sollen. Dabei werden Sie gefragt, ob Sie tatsächlich die markierten Bearbeitungen in eine andere Ebene übertragen möchten. Nur, wenn Sie diese Frage mit `ja` beantworten, steht Ihnen die Zwischenablage im Ziel zur Verfügung.
8. Legen Sie dort einen neuen Datensatz an: mithilfe der Schaltfläche `[Neu]` oder mit `<F6>`. Bitte achten Sie darauf, dass die zu kopierenden Bearbeitungen der Stückliste angehängt (mit `<F6>`) und nicht eingefügt (mit `<Strg>` + `<F6>`) werden.
9. Betätigen Sie die Schaltfläche `[Einfg]` (Einfügen) oder die Tastenkombination `<Strg>` + `<O>`. Die betreffenden Bearbeitungen werden mit allen Parametern hinzugefügt.
10. Ändern Sie bei Bedarf die notwendigen Parameter.
11. Speichern Sie die Stückliste mit `<Ende>`. Unter Umständen wird dabei eine neue Stücklistenummer vergeben.
12. Wiederholen Sie die Schritte 7 bis 11, wenn Sie die markierten Bearbeitungen in weiteren Stücklistenebenen einfügen möchten.
13. Verlassen Sie speichernd den Stücklisteneditor.

## Sprossenerfassung

> **Lernziele**
> - Sprossenerfassung im Auftrag kennenlernen.
> - Möglichkeiten und Restriktionen der A+W Enterprise - Sprossenerfassung erkennen.
> - Möglichkeiten und Restriktionen der A+W CAD Designer (Bars) - Sprossenerfassung kennenzulernen.
>
> **Nutzen**
> - Sprossen sind feste Bestandteile eines Fenster bzw. einer Glasscheibe. Die Erfassung des korrekten Sprossenaufbaus ist wichtig und für die Produktion unerlässlich.
>
> **Merke**
> - **Sprosse/Sprossenstab**: Als eine Sprosse bezeichnet man einen Sprossenstab in einer Gesamtkonstruktion.
> - **Sprossengitter**: Als ein Sprossengitter bezeichnet man die Gesamtkonstruktion aller Sprossen, die in einem Rahmen verbaut wird oder auf einem Glas aufgeklebt wird.
> - **Glasteilende Sprosse**: Dieser Begriff kommt aus der Fensterbranche.

In der Regel werden Sprossen direkt in Isoliergläser eingebaut. Sprossen sind somit Bestandteil der ISO-Stückliste und nur für Isoliergläser zulässig. Eine Ausnahme bilden Klebesprossen. Diese werden jedoch in der Regel bei der Fensterfertigung mitgeliefert und eingebaut. In A+W Enterprise können Sie einfache Sprossenkonstruktionen direkt im Auftrag erfassen. Aufwendigere Konstriktionen sind so genannte Makros, z.B. Sonne, müssen in anderen Probgammen z.B. A+W CAD Designer (Bars) erfasst werden und anschließend in A+W Enterprise übertragen werden und können hier nicht mehr geändert werden. Bei Fragen zu A+W CAD Designer (Bars) haben, wenden Sie sich bitte an den zuständigen A+W Mitarbeiter.
⇨ Verkauf, "Sprossenerfassung" auf Seite D-1284

### So öffnen Sie die Sprossenerfassung
1. Erfassen Sie eine Position mit ISO-Glas.
   ⇨ "So erfassen Sie ein ISO (Isolierglas)" auf Seite D-1015
2. Rufen Sie nach der Maßeingabe mit `<Shift>` + `<F8>` die Sprossenerfassung auf oder klicken Sie mit der Maus auf die Schaltfläche `[Sprossen]`, um die Sprossenerfassung zu öffnen.

### So führen Sie die Sprossenerfassung
1. Öffnen Sie die Sprossenerfassung. Die Felder in diesem Dialog sind im folgenden Kapitel beschrieben:
   ⇨ Verkauf, "Sprossenerfassung" auf Seite D-1284
2. Geben Sie im Feld **Sprosse** eine Artikelnummer aus der Artikelgruppe 57**** ein oder wählen Sie eine Artikelnummer mit Hilfe der Suchfunktion `<F9>`, `<F8>` aus.
   Bestätigen Sie Ihre Eingabe mit `<Enter>`. Das Feld **Bezeichnung** wird von A+W Enterprise automatisch gefüllt.
3. Geben Sie die Anzahl der waagerecht sowie der senkrecht verlaufenden Sprossen ein und bestätigen Sie mit `<Enter>`.
4. Wählen Sie mit Hilfe der `<Leertaste>` eine Symmetrie und bestätigen Sie mit `<Enter>`.
5. Wenn Sie eine Sprosse gewählt haben, die in verschiedenen Farbvarianten erhältlich ist, wählen Sie in im Feld **Farbe** die Farbe aus.
6. Wählen Sie bei zu bestellenden Sprossen einen Lieferanten mit Hilfe von `<F8>`, `<F9>` aus.
7. Wählen Sie eine Beschaffungsart im Feld **B** mit `<F9>` oder mit Mausklick auf den Pfeil aus.
8. Im Feld **Rahmen** legen Sie fest, in welchen Rahmen die Sprossen eingebaut werden sollen.
   Eine Eingabe ist nur bei dreifachem ISO-Glas möglich.
9. Im Feld **Glas** legen Sie fest, auf welches Glas die Sprossen aufgeklebt werden sollen.
   Eine Eingabe ist nur bei aufgeklebten Sprossen möglich oder bei dreifachem ISO-Glas.
   Die Gesamt-Länge der Sprossen wird bei vollständiger Eingabe aller Daten von A+W Enterprise automatisch berechnet und im Feld **Lfm** angezeigt.
10. Verlassen Sie die Sprossenerfassung mit `<Ende>` oder erfassen Sie weitere Sprossen.
    Wenn Sie die **Sprossensymmetrie mit Editor** gewählt haben, öffnet jetzt der Sprosseneditor.

> **Hinweis zur Preisberechnung**
> Beachten Sie, dass die Preisberechnung maximal 2 Sprossenartikel berechnet.

### So starten Sie den Sprosseneditor
1. Wenn Sie eine Sprossesymmetrie mit **Editor** gewählt haben, öffnet der Sprosseneditor nach Schließen der Sprossenerfassung mit `<Ende>` automatisch.
2. Alternativ betätigen Sie `<F3>` im Dialog **Sprossenerfassung**, wenn Sie zuvor im Sprosseneditor eine Änderung bei dieser Position vorgenommen haben.
   ⇨ Verkauf, "Sprosseneditor" auf Seite D-1289

### So definieren Sie Wegfallsprosse definieren
Sie haben die Möglichkeit, einzelne Sprossenstäbe wieder zu entfernen.
1. Öffnen Sie den Sprosseneditor.
   ⇨ Verkauf, "So starten Sie den Sprosseneditor" auf Seite D-1025
2. Klicken Sie mit der Maus auf die Sprosse, die Sie entfernen möchten.
   Die Sprosse wird entfernt.

> **Sprosse wieder einblenden**
> Um die Sprosse wieder einzufügen, klicken Sie mit der Maus an die Stelle, an der sich die Sprosse zuvor befand. Die Sprosse wird wieder eingeblendet.

### So löschen Sie die Abschnitte
Sie haben die Möglichkeit, ganze Sprossenabschnitte zu entfernen.
⇨ Verkauf, "Sprossenabschnitte" auf Seite D-1292
1. Öffnen Sie den Sprosseneditor.
   ⇨ Verkauf, "So starten Sie den Sprosseneditor" auf Seite D-1025
2. Drücken Sie `<F5>`.
   A+W Enterprise markiert eine Sprosse rot.
	- Wenn Sie den Sprossenabschnitt so belassen möchten, drücken Sie `<1>`.
	- Um den Sprossenabschnitt zu löschen, drücken Sie `<2>`.
	- Um die Bearbeitung der Sprossenabschnitte zu beenden, drücken Sie `<3>`.
3. Verfahren Sie mit den übrigen Sprossen ebenso. A+W Enterprise fragt auf diese Weise alle Sprossenabschnitte nacheinander ab.
4s Schließen Sie den Sprosseneditor mit `<Ende>`.

### So verschieben Sie die Bohrpunkte
1. Öffnen Sie den Sprosseneditor.
   ⇨ Verkauf, "So starten Sie den Sprosseneditor" auf Seite D-1025
2. Klicken Sie auf einen der Randanschlusspunkte, um die Bohrpunkterfassung zu aktivieren.
   Oder betätigen Sie `<Shift>` + `<F12>`.
3. Tragen Sie die neue Position des Bohrpunktes in den Eingabedialog ein.
   Bezugspunkt für die Maßangabe ist die linke untere Ecke des Glases.
   Bestätigen Sie mit `<Enter>`.
4. Schließen Sie die Bohrpunkterfassung mit `<Ende>` oder verfahren Sie mit den übrigen Bohrpunkten ebenso.

### So ändern Sie die Größe für ein lichtes Feld
1. Öffnen Sie den Sprosseneditor.
   ⇨ Tutorial, “So starten Sie den Sprosseneditor" auf Seite D-1025
2. Klicken Sie mit der Maus in das Feld, das Sie ändern möchten.
   Oder betätigen Sie `<Strg>` + `<F8>`.
   Eine Abfrage, ob die Höhe des Feldes geändert werden soll, wird angezeigt. Beantworten Sie diese Frage mit `[nein]`, findet über den nachfolgenden Eingabedialog eine Anpassung der lichten Breite statt.
3. Tragen Sie die neue Größe des lichten Feldes in den Eingabedialog ein.
4. Schließen Sie den Sprosseneditor mit `<Ende>` oder verfahren Sie mit den übrigen lichten Feldern ebenso.

### So passen Sie die Sprossenabschnitte in der Tabelle an
⇨ Verkauf, "Sprossenabschnitte" auf Seite D-1292
1. Öffnen Sie den Sprosseneditor.
   ⇨ Verkauf, "So starten Sie den Sprosseneditor" auf Seite D-1025
2. Klicken Sie auf `[Tab]`. Oder betätigen Sie `<Shift>` + `<F11>`.
   Der Dialog **Sprossenabschnitte** öffnet sich.
3. Passen Sie die Bohrpunkte durch Eingabe eines neuen Wertes an.
4. Schließen und speichern Sie den Dialog **Sprossenabschnitte** mit `<Ende>`.

### So können Sie Änderungen im Sprosseneditor verwerfen
1. Öffnen Sie den Sprosseneditor.
   ⇨ Verkauf, "So starten Sie den Sprosseneditor" auf Seite D-1025
2. Klicken Sie `[Neu]` oder betätigen Sie `<F3>`, um die Änderungen zu verwerfen und den Sprosseneditor neu symmetrisch aufzubauen.
3. Schließen Sie den Sprosseneditor mit `<Ende>` oder nehmen Sie erneut Änderungen am Sprossenaufbau vor.

## Stufenerfassung

> **Lernziele**
> - Stufenerfassung kennenlernen.
> - Voraussetzungen der Stufenerfassung erkennen.
> - Restriktionen der Stufenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Insbesondere bei der Herstellung von Glas für den Bausektor kommt dieser Funktion eine besondere Bedeutung zu.
> - Eine Stufe an einer Glasscheibe wirkt sich auf einige nachfolgende Funktionen aus, wie z. B. Modellentartung, Versiegelungstiefe, Produktionsskizze, usw.
>
> **Merke**
> - **Stufe**: Kantenabzug an der Glasscheibe ausgehend von dem Referenzglas
> - **Referenzglas**: Im Vorfeld erfasste Konstruktionen, die billig genutzt werden.

Es ist nicht selten, dass zusammengebaute Glaseinheiten (ISO oder VSG) an den Kanten nicht bündig sind. Das kommt vor, wenn z. B. bei einer Fassade eingesetzte Gläser an der ersten Scheiben befestigt werden. Dieser Stufenabzug kann sowohl an nur einer Glaskante als auch an mehreren bzw. allen Kanten erfolgen.

Für die korrekte Erfassung benötigen Sie einen Dummyartikel mit dem Artikeltyp = 510 Stufe. Eine wichtige Voraussetzung für diesen Artikel ist, dass es sich nicht um ein Meta-Teil handelt. Eine weitere Voraussetzung beinhaltet die Berechnung der Stufenabzugsmaße. Diese Berechnung erfolgt anhand von Formeln, die in den Stammdaten hinterlegt und in der Stückliste den Glasscheiben zugeordnet sind.
⇨ Stammdaten, "Stückliste" auf Seite B-447

Eine Referenzscheibe erhält in der Stückliste eine Formel ohne den Stufenabzug. Allen anderen Scheiben in der Stückliste muss eine Formel mit Stufenabzug zugeordnet sein. Auch für Isolierglas-Rahmen werden entsprechende Formeln zugeordnet.
⇨ Stammdaten, "Zwingende Maßangaben – Maßparameter-Auswahl" auf Seite B-431

> **Beispiel**
> Formel 100 hat im Feld **Stufe** den Wert **N**.
> Formel 110 hat im Feld **Stufe** den Wert **J**.
> ⇨ Stammdaten, "Formeleditor" auf Seite B-489
> In der Stückliste für ISO wird der ersten Glasscheibe die Formel 100 zugeordnet. Dadurch wird die erste Glasscheibe als Referenzglas definiert. Allen anderen Glasscheiben wird die Formel 110 zugeordnet.

### So erfassen Sie ein gestuftes ISO im Auftrag
1. Öffnen Sie den Dialog **Auftragserfassung** und erfassen Sie den Auftragskopf, wie im folgenden Kapitel beschrieben ist:
   ⇨ Verkauf, "So erfassen Sie einen Auftrag" auf Seite D-992
2. Nach der Eingabe der **Artikelnummer** und **Menge** in der Position können Sie nun die Stufenerfassung mit `<Shift>` + `<F10>` starten:
   *(Screenshot des Dialogs "Stufenerfassung (relevante Teile)")*
3. Nach den in der Artikelstückliste hinterlegten Formeln wird ermittelt, welches Glas als **\*Referenzglas\*** dient und entsprechend markiert. Unter Umständen kann die Referenz mit `<Shift>` + `<F5>` geändert werden. Die Herstellbarkeit der Glasaufbau soll in diesem Fall geprüft werden.
4. Über die Schaltfläche `[Glasaustausch]` können Sie den Glasaufbau nach Ihren Wünschen anpassen.
5. Sie können auch eine Modellnummer für eine Glasscheibe vergeben. Wenn Sie die gesamte Produktaufbau als Modell haben wollen, geben Sie das Modell in der Position ein:
   ⇨ Verkauf, "So erfassen Sie in der Position ein Modell" auf Seite D-1011
6. Drücken Sie `[OK]`, um mit der Eingabe fortzufahren, wenn die Angaben in diesem Dialog mit der Eingabeanforderung übereinstimmen.
7. Der Dialog **Modell-Maßangaben für Referenzglas-Modell** wird nun gestartet. Geben Sie in diesem Dialog die Abmessungen des Referenzglases ein und bestätigen Sie Ihre Eingabe mit `[OK]`.
8. Der Dialog **Stufen Abzugsmaße** wird nun für jede Stufenscheibe separat gestartet:
   *(Screenshot des Dialogs "Stufen Abzugsmaße")*
9. Geben Sie in den Feldern, die sich sichtbar an den Kanten befinden, das Abzugsmaß pro Kante ein. Bitte beachten Sie, dass der Abzug parallel zur gewählten Kante erfolgt:

> **Beispiel**
> Das Abzugsmaß 100 mm wird parallel zur unteren Kante abgezogen,
> das Abzugsmaß 80 mm wird parallel zur oberen Kante abgezogen,
> das Abzugsmaß 80 mm wird parallel zur rechten Kante abgezogen:
> d. h., die Abmessung der gestuften Scheibe wird wie folgt berechnet:
> Η = 1450-100-80 = 1270 mm
> W = 1000-80 = 920 mm.

10. Bestätigen Sie die Eingabe mit `[OK]`.
    Wenn Sie mehr als eine gestufte Scheiben erfassen, erscheint dieser Dialog für jede Glasscheibe. Die Felder für die Eingabe Abzugsmaß sind mit den bereits eingegeben Werten vorbelegt. Sie können dann die Abzugsmaße ändern oder die gleiche Werteeingabe mit `[OK]` bestätigen.
11. Der Dialog zur Stufenerfassung wird geschlossen. Sie können die Position nun zu Ende erfassen.
12. Sie können die Abmessungen für den Kopfartikel, sowie für jede Glasscheibe und jeden Rahmen/VSG-Folie im Preis-Feld mit `<F3>` prüfen.

## iTOE - Erfassung und Nachbearbeitung

> **Lernziele**
> - Technische Auftragserfassung kennenlernen.
> - Möglichkeiten der technischen Auftragserfassung erkennen.
> - Restriktionen der technischen Auftragserfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Mit iTOE können Sie eine technische Zeichnung einfach und präzise erfassen. Diese Zeichnung wird anschließend in A+W Enterprise übernommen und die Stückliste synchronisiert.
>
> **Merke**
> - **iTOE**: Integrierte CAD basierende Positionserfassung. Die Nutzung setzt eine entsprechende Systemkonfiguration voraus.
> - **Template**: Im Vorfeld erfasste Konstruktionen, die billig genutzt werden.
> - **SN-Datei**: A+W CAD Designer (Shapes) - Datei

iTOE bietet die Möglichkeit spezifische Formelemente zu erfassen und technische Zeichnungen zu importieren und zu exportieren. Auf der Basis von Templates können Sie technische Auftragserfassung für komplexe Elemente durchführen, automatisch die Stückliste erzeugen und abgleichen lassen. Dabei werden auch alle notwendigen kaufmännischen Dokumente (Aufträge, Fertigungspapiere, Lieferscheine etc.) und die Maschinensteuerung unterstützt.

Folgende Erfassungsvarianten können Sie nutzen:
- **Automatische Generierung einer SN-Datei**
  ⇨ "So lassen sich die SN-Datei automatisch erzeugen" auf Seite D-1032
- **`<Strg>` + `<E>` manuelles Anhängen einer SN-Datei**
  ⇨ "So hängen Sie die SN-Datei an die Position an" auf Seite D-1032
- **`<Strg>` + `<F>` Starten der technischen Erfassung (iTOE)**
  ⇨ "So starten Sie die technische Auftragserfassung" auf Seite D-1033
- **`<Strg>` + `<B>` Starten der DXF-Import**

> **iTOE - Austauschregeln**
> Um reibungslose Kommunikation zwischen den beiden Programmen A+W Enterprise und A+W CAD Designer (Shapes) zu gewährleisten, müssen iTOE - Austauschregeln im Vorfeld sorgfältig hinterlegt werden:
> ⇨ Stammdaten, "iTOE-Austauschregeln" auf Seite B-359

### So lassen sich die SN-Datei automatisch erzeugen
1. Starten Sie die Auftragserfassung. Erfassen Sie den Auftragskopf:
   ⇨ Verkauf, "So erfassen Sie einen Auftrag" auf Seite D-992
2. Geben Sie in der Position die gewünschte Artikelnummer ein.
3. Um eine SN-Datei vom Programm generieren zu lassen, muss Ihr System entsprechend konfiguriert sein. Ist dies der Fall, erscheint direkt nach der Eingabe der Artikelnummer die Frage, ob die SN-Datei für die Position automatisch generiert werden soll. Bestätigen Sie die Frage mit `[Ja]`.
4. Checkbox **SN** wird aktiviert und kann nicht geändert werden.
5. Erfassen Sie die Position zu Ende.
6. Im Register **Eigensch.** wird im Feld **CAD Datei** die neu generierte SN-Datei der Position zugeordnet und angezeigt.
7. Anschließend haben Sie nun die Möglichkeit:
   ⇨ Verkauf, "So starten Sie die technische Auftragserfassung" auf Seite D-1033
   oder mit `<Strg>` + `<F9>` diese SN-Datei zu löschen.

### So hängen Sie die SN-Datei an die Position an
1. Starten Sie die Auftragserfassung. Erfassen Sie den Auftragskopf:
   ⇨ Verkauf, "So erfassen Sie einen Auftrag" auf Seite D-992
2. Geben Sie in der Position die gewünschte Artikelnummer und Menge ein.
3. Drücken Sie `<Strg>` + `<E>`. Das Programm wechselt sich in den Register **Eigensch.**, Feld **CAD Datei** und öffnet den Windows Dialog **Datei öffnen**:
   *(Screenshot zeigt den Datei-Öffnen-Dialog über der A+W Enterprise Oberfläche)*
4. Wählen Sie eine gewünschte Datei aus und bestätigen Sie die Auswahl mit `[OK]`.
5. Checkbox **SN** wird aktiviert und kann nicht geändert werden.
6. Erfassen Sie die Position zu Ende.
7. Im Register **Eigensch.** wird im Feld **CAD Datei** die neu generierte SN-Datei der Position zugeordnet und angezeigt.
8. Anschließend haben Sie nun die Möglichkeit:
   ⇨ Verkauf, "So starten Sie die technische Auftragserfassung" auf Seite D-1033
9. oder mit `<Strg>` + `<F9>` diese SN-Datei zu löschen.

### So starten Sie die technische Auftragserfassung
1. Für die technische Auftragserfassung werden die Stammdaten für iTOE-Austausch-/Zusatz vorausgesetzt.
   ⇨ Stammdaten, “iTOE-Austauschregeln" auf Seite B-359
2. Starten Sie den Dialog Auftragserfassung.
3. Erfassen Sie die Daten im Auftragskopf, sowie auf der Positionsebene die Felder **Artikel**, **Menge**, **Breite/Höhe/SZR** (bei ISO).
4. Starten Sie mit `<Strg>` + `<F>` die technische Auftragserfassung mit A+W CAD Designer (Shapes).
5. Die bereits erfasste Felder, sowie der Produktaufbau wird nun zur weiteren Erfassung übernommen. Bei einer entsprechenden Konfiguration kann auch die Artikelbezeichnung von Gläser und Folien (artikel.artbez1) in A+W CAD Designer (Shapes) mit übernommen werden.

> **Arbeiten mit A+W CAD Designer (Shapes)**
> Technische Erfassung in A+W CAD Designer (Shapes) können Sie aus dem Handbuch für A+W CAD Designer (Shapes) entnehmen. Bei Interesse wenden Sie sich bitte an A+W - Mitarbeiter.

6. Nach der Fertigstellung des Produktzeichnung haben Sie nun folgende Möglichkeiten:
	- **TOE beenden (`<F2>`)**
	  Sie beenden die technische Auftragserfassung und kehren zur A+W Enterprise - Auftragserfassung zurück. Die eventuelle Änderungen in A+W CAD Designer (Shapes) werden automatisch übernommen, sofern diese mit iTOE Austausch-/Zusatzregeln abgedeckt sind. Die sn-Datei wird jedoch nicht behalten. Sollten Sie weitere Bearbeitung bzw. Korrektur an der Produktaufbau vornehmen wollen, muss die technische Erfassung erneut durchgeführt werden.
	- **TOE Abbrechen (`<F3>`)**
	  Sie beenden die technische Auftragserfassung und kehren zur A+W Enterprise - Auftragserfassung zurück. Die eventuelle Änderungen in A+W CAD Designer (Shapes) werden verworfen.
	- **TOE Beenden und Datei speichern (`<F4>`)**
	  Sie beenden die technische Auftragserfassung, die sn-Datei wird gespeichert, Name der Datei wird in der Position mitgespeichert. Aufgrund der vordefinierten Austausch-/Zusatzregeln wird die Stückliste abgeglichen. Die sn-Datei kann beim Bedarf noch mal bearbeitet.
	- **TOE Beenden ohne SL-Angleich (`<F5>`)**
	  Sie beenden die technische Auftragserfassung. Die sn-Datei wird in die Position übernommen und mit gespeichert. Es findet jedoch keinen Stücklistenabgleich dabei.

### So gleich Sie die Stückliste manuell ab
Wenn der Stücklisten-Abgleich zwischen A+W CAD Designer (Shapes) und A+W Enterprise nicht durchgeführt werden konnte, wird Ihnen die Möglichkeit angeboten, die passende Artikelzuordnung selbst zu bestimmen.
1. Starten Sie den Dialog Auftragserfassung.
2. Führen Sie die iTOE-Positionserfassung durch.
   ⇨ "So starten Sie die technische Auftragserfassung" auf Seite D-1033
3. Wird für einen relevanten Stücklistenartikel aus den iTOE-Austauschregeln keine passende Zuordnung ermittelt, erscheint ein Hinweis, dass für diese CAD-Bearbeitung kein A+W Enterprise - Artikel gefunden wurde. Ein Werteeingabe-Dialog erscheint nun automatisch.
4. Sie können den gewünschten A+W Enterprise Artikel aus dem Selo auswählen und die Eingabe mit `[OK]` bestätigen.
5. Die Bearbeitung wird in die Positionsstückliste eingefügt.

### So setzen Sie das SN-Status manuell um
Nach dem Stücklistenabgleich und erfolgreicher Datenübernahme kann es erforderlich sein, die A+W Enterprise -Stückliste für eine wiederholte Datenübergabe in den A+W CAD Designer (Shapes) zu sperren. Führen Sie folgende Schritte aus:
1. Starten Sie den Dialog Auftragserfassung.
2. Führen Sie die iTOE-Positionserfassung durch.
   ⇨ "So starten Sie die technische Auftragserfassung" auf Seite D-1033
3. Positionieren Sie den Cursor im Feld **SN-Datei** auf einer Position, deren SN-Status nun geändert werden muss.
4. Betätigen `<Strg>` + `<A>`. Die Status-Änderung erfolgt erst nach der Bestätigung einer CU-Meldung (Customizing-Meldung). SN-Status=100 wird nun für diese Position gesetzt.
5. Beenden Sie nun die Positionserfassung.

## Produktaustausch

> **Lernziele**
> - Produktaustausch in der Auftragserfassung kennenlernen.
> - Die Möglichkeit des schnellen Produktaustausches in einem bestehenden Auftrag nutzen.
> - Restriktionen der Funktion zum Produktaustausch beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Mit der Funktion Produkttausch können Sie auf einfache Weise mehrere Stücklisten in einem bereits erfassten Auftrag auf einmal ändern. Die geänderten Produktstrukturen können nur für diesen Auftrag gelten oder wahlweise in die Stammdaten zurückgeschrieben werden.
>
> **Merke**
> - **Produktaustausch**: Unter Produktaustausch versteht man einen Tausch einer kompletten Positionsartikel, sowie auch eine Änderung der Produktaufbau in einem bereits erfassten Auftrag.
> - **Originalaufbau**: Stücklistenbaum eines Positionsartikels aus den Stammdaten.
> - **Wunschaufbau**: Neue bzw. geänderte Stückliste eines Positionsartikels.

Auf der Positionsebene in der Auftragserfassung können Sie einen Produktaustausch vornehmen. So ist es möglich, schnell und einfach diverse Produkte bzw., den Produktaufbau gleichzeitig für mehrere Position durchzuführen. In diesem Kapitel werden einige Anwenderfälle beschrieben:
⇨ "So führen Sie einen Produktaustausch aus" auf Seite D-1036
⇨ "So führen Sie einen Austausch von zweifach-ISO zum dreifach-ISO" auf Seite D-1037

### So führen Sie einen Produktaustausch aus
*(Screenshot des "Produktaustausch" Dialogs mit Markierungen A, B, C, D)*
**A**: Nummer der Stückliste/ Kundenposition - Typ
**B**: Aktuelle Produktaufbau in der Position
**C**: Original Produktaufbau aus den Stammdaten
**D**: Gewünschte Produktaufbau nach dem Produtkaustausch

1. Starten Sie den Dialog **Auftragserfassung**.
2. Wählen Sie oder geben Sie ein die Auftragsnummer, inder Sie die Änderungen vornehmen wollen.

> **Auftragsstatus**
> Beachten Sie, dass die Änderung der Stückliste zu der produktionsrelevanten Änderungen gehören. So können die Änderungen an der Stückliste nur vorgenommen werden, solange der Auftrag nicht weiter an System zur Bearbeitung freigegeben ist.

3. Starten Sie den Dialog **Produktaustausch** aus dem `<F4>` > **Produktangaben**.
4. Geben Sie im Dialog **Produktaustausch** unter (A), Feld **Alte Stückliste/Typ** die Stückliste-Nummer oder den Typ der Kundenposition ein.
5. Der aktuelle Produktaufbau wird im Dialog **Produktaustausch** unter (B) angezeigt.
6. Geben Sie im Feld **Austauschartikel** die gewünschte Artikelnummer, bzw. wählen Sie die Nummer über Artikelselo mit `<F9>` aus.
   ⇨ Verkauf, "Artikel-Suche" auf Seite D-1101
7. Unter (C) und (D) im Dialog wird nun Originalaufbau dargestellt.
8. Die Felder für **Wunschaufbau** können Sie ändern, z.B.:
	- Für die 1. Scheibe ein anders Glas auswählen,
	- Für 2. Scheibe eine andere Einbauposition eingeben
	- im Feld **Zusatzartikel** eine zusätzliche Bearbeitung hinzufügen.
9. Anschließend haben Sie folgende Option zur Auswahl:
	- mit `<Original>` lassen Sie die Wunschaufbau erneut aus den Stammdaten darstellen.
	- mit `<F3>` oder `<Start>` führen Sie die Aktion aus.
	- mit `<Weiter>` erfassen Sie den Produktaustausch für weitere Stücklistennummer/Typ.
	- mit `<Abbrechen>` verlassen Sie den Dialog **Produktaustausch**, ohne Änderungen vorgenommen zu haben.

### So führen Sie einen Austausch von zweifach-ISO zum dreifach-ISO
*(Screenshot des "Produktaustausch für Positionen" Dialogs)*
**A**: Anzeige, welche Artikeln getauscht werden
**B**: SZR-Felder, die geändert werden können

1. Führen Sie die Schritte 1 bis 8 aus.
2. Anschließend führen Sie den Austausch aus: mit `<Start>`, oder mir `<F3>`.
3. Das Programm erkennt automatisch, dass beim Austausch noch die Eingabe für **SZR2** fehlt und startet den Dialog **Produktaustausch für Position**.
4. In diesem Dialog, Bereich (B) können Sie für jede Position, in der ein Produktaustausch erkannt wird, eine bestehende SZR zu ändern, bzw. eine neue SZR2 vergeben.
5. Führen Sie anschließend die Aktion mit `<Start>` aus.

> **Zwingende Maßangaben beachten**
> Ob die SZR2 eingegeben bzw. geändert werden kann, hängt von zwingenden Maßangaben für den gewählten Artikel bzw. dessen Artikeltyp ab. Nur wenn die Erfassung für den Maßparamer SZR2 zugelassen ist, können Sie die Änderung im Auftrag vornehmen.
> ⇨ Stammdaten, "Zwingende Maßangaben – Maßparameter-Auswahl" auf Seite B-431
> ⇨ Stammdaten, "Zwingende Maßangaben – Ansicht 1" auf Seite B-432

## Preislose Erfassung

### Preiskalkulation
*(Schematischer Aufbau einer einfachen ISO-Scheibe)*

Die Preiskalkulation ermöglicht eine schnelle Kalkulation der Einkaufs- und Verkaufspreise, ohne dass dabei ein Abspeichern der Berechnung erfolgt.
⇨ Softwarereferenz, "Preiskalkulation" auf Seite D-1379

### Preislose Erfassung
Kundenaufträge können mit der preislosen Erfassung beschleunigt aufgenommen werden. Der Vorteil der preislosen Erfassung liegt darin, dass der Kunde die Auftragserfassung verfolgen kann, in die Preisberechnung aber keinen Einblick erhält. Die Preisberechnung unter Berücksichtigung der aktuellen Preise und Konditionen erfolgt erst nach der eigentlichen Auftragserfassung im Hintergrund. Preisänderungen sind anschließend problemlos möglich.
⇨ Softwarereferenz, "Preislose Erfassung" auf Seite D-1133

Sie haben die Möglichkeit, eine kundenindividuelle Abfrage von Preisen durchzuführen, ohne dass ein Vorgang (Angebot, Auftrag) angelegt und abgespeichert wird.
Die Erfassung der Felder erfolgt auf gleiche Weise wie bei der Auftragserfassung, mit dem Unterschied, dass bei der Preiskalkulation nicht alle Felder der Kopfdaten ausgefüllt werden müssen.
Bedienung, "Angebots- und Auftragserfassung" auf Seite D-33
Softwarereferenz, "Preiskalkulation" auf Seite D-68

**Preiskalkulation durchführen**
1. Öffnen Sie im Menü **Verkauf > Preiskalkulation**.
   ALCIB zeigt den ausgewählten Dialog an.
2. Wählen Sie den Kunden folgendermaßen aus:
   - Geben Sie die Kundennummer ein, wenn diese bekannt ist.
   - Oder betätigen Sie die Taste `<F9>` für eine Suche nach der Kundennummer oder `<F8>` für eine Matchcode-Suche.
   Der Dialog **Marktpartner-Suche** öffnet sich.
3. Mit `<F2>` öffnen Sie die erweiterte Suche.
4. Geben Sie die Suchkriterien ein.
5. Mit `<F3>` starten Sie die Suche.
   Software, "Suche durchführen" auf Seite A-60
   Softwarereferenz, "Kunde" auf Seite D-73
6. Ordnen Sie den aktuellen Vorgang einem Objekt zu (optional), um objektspezifische Sondervereinbarungen für diesen Vorgang zu berücksichtigen.
   Betätigen Sie `<F9>` im Feld **Objekt**. Wählen Sie in der Liste das gewünschte Objekt aus.
   Softwarereferenz, "Objekt" auf Seite C-77
7. Erfassen Sie die Positionen und Produkte.
   Bedienung, "Positionen und Produkte anlegen" auf Seite D-39
8. Schließen Sie den Vorgang ab.
   Bedienung, "Auftragserfassung abschließen" auf Seite D-56

Sie haben die Möglichkeit, Vorgänge (Angebot, Auftrag) zu erfassen, ohne dass die Preisberechnung zum Zeitpunkt der Erfassung sichtbar ist. Der Vorteil der preislosen Erfassung liegt darin, dass der Kunde die Auftragserfassung verfolgen kann, in die Preisberechnung aber keinen Einblick erhält. Die Preise werden nach dem Abspeichern durch A+W Enterprise vervollständigt und erscheinen dann auf dem Ausdruck. Die Erfassung unterscheidet sich nicht von der Auftragserfassung.

Wie Sie die einzelnen Felder erfassen, erfahren Sie in den folgenden Abschnitten:
⇨ Softwarereferenz, "Preislose Erfassung" auf Seite D-1133

## Lieferscheine

> **Lernziele**
> - A+W Enterprise-Sprossenerfassung kennenlernen.
> - Bedienung im Sprosseneditor beherrschen.
> - Tipps und Tricks der Sprossenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **Symmetrie**: Aufbauart einer Sprossenkonstruktion. Wird dabei ein Gitternetz gleichmäßig aufgebaut, so spricht mal vom .feldsymmetrischen Sprossen.
> - **Bohrpunkt**: Befestigungspunkte der Sprossenkonstruktion an Iso-Rahmen.
> - **Lichtes Feld**: Abstand zwischen zwei waagerechten und zwei senkrechten Sprossenkanten.

Bei jeder Auslieferung eines Auftrags wird ein Lieferschein ausgestellt. Dieser dient zum einen als Nachweis für den Kunden, zum anderen als Auskunft über den jeweiligen Status der Auftragsabwicklung. Es können Komplett- oder Teillieferscheine erstellt werden. Teillieferscheine werden ausgestellt, wenn die Lieferung nicht komplett, sondern in mehreren Teilen erfolgt. Sie können wählen, ob eine automatische Freigabe oder eine manuelle Ausstellung der Lieferscheine erfolgen soll.
⇨ Softwarereferenz, "Lieferung" auf Seite D-1385

## Rechnungen

> **Lernziele**
> - A+W Enterprise-Sprossenerfassung kennenlernen.
> - Bedienung im Sprosseneditor beherrschen.
> - Tipps und Tricks der Sprossenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **Symmetrie**: Aufbauart einer Sprossenkonstruktion. Wird dabei ein Gitternetz gleichmäßig aufgebaut, so spricht mal vom .feldsymmetrischen Sprossen.
> - **Bohrpunkt**: Befestigungspunkte der Sprossenkonstruktion an Iso-Rahmen.
> - **Lichtes Feld**: Abstand zwischen zwei waagerechten und zwei senkrechten Sprossenkanten.

Die Rechnungsstellung richtet sich nach den Lieferungs- und Zahlungsbedingungen, die im Auftrag vereinbart wurden. Sie können nach Lieferung der Ware Teil- oder Sammelrechnungen erstellen. Ein fakturierter Vorgang ist prinzipiell nicht mehr korrigierbar. Sollen dennoch preisliche Änderungen vorgenommen werden, so ist dies nur noch über die Ausstellung einer Gutschrift oder durch eine Nachbelastung möglich.

Die Vergabe von Rechnungsnummer wird vom Systemautomatisch vorgenommen. Bei der manuellen Rechnungserfassung wird zuerst eine interne Nummer vergeben und erst, wenn die Rechnung fertig erfasst ist, wird diese Rechnung unter endgültiger Nummer gespeichert. So wird eine lückenlose Nummerierung gewährleistet.

In äußerst seltenen Fällen (z.B.: Programmabbruch direkt nachdem die finale Rechnungsnummer vergeben wurde) kann es dazu kommen, dass bei der Vergabe von Rechnungsnummern Lücken entstehen. Da diese Lücken Probleme im Controlling bereiten können, gibt es eine Möglichkeit, diese Nummern wiederzuverwenden. Diese Logik bedarf eine spezielle Systemkonfiguration und darf nur in Absprache mit A+W aktiviert werden. Wenden Sie sich bei Interesse an einen Mitarbeiter der A+W Software GmbH an.

Sie haben außerdem die Möglichkeit, Abschlags- oder Schlussrechnungen mit einem vorher erstellten Zahlungsplan zu stellen und zwischen der automatischen Freigabe und der manuellen Rechnung zu wählen.

## Gutschriften

> **Lernziele**
> - A+W Enterprise-Sprossenerfassung kennenlernen.
> - Bedienung im Sprosseneditor beherrschen.
> - Tipps und Tricks der Sprossenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **Symmetrie**: Aufbauart einer Sprossenkonstruktion. Wird dabei ein Gitternetz gleichmäßig aufgebaut, so spricht mal vom .feldsymmetrischen Sprossen.
> - **Bohrpunkt**: Befestigungspunkte der Sprossenkonstruktion an Iso-Rahmen.
> - **Lichtes Feld**: Abstand zwischen zwei waagerechten und zwei senkrechten Sprossenkanten.

Bei Auftragsstornierungen, Transportschäden oder Mängelrügen seitens des Kunden können Sie komplette Gutschriften oder Teil-Gutschriften für einen Auftrag anfertigen und sofort buchen. Möglich ist auch eine Gutschrift über eine Pauschalsumme, wenn Sie auf die betreffende Rechnung Bezug nehmen, damit die Gutschrift buchhalterisch erfasst werden kann.

## Auftragsfreischaltung

> **Lernziele**
> - A+W Enterprise-Sprossenerfassung kennenlernen.
> - Bedienung im Sprosseneditor beherrschen.
> - Tipps und Tricks der Sprossenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **Symmetrie**: Aufbauart einer Sprossenkonstruktion. Wird dabei ein Gitternetz gleichmäßig aufgebaut, so spricht mal vom .feldsymmetrischen Sprossen.
> - **Bohrpunkt**: Befestigungspunkte der Sprossenkonstruktion an Iso-Rahmen.
> - **Lichtes Feld**: Abstand zwischen zwei waagerechten und zwei senkrechten Sprossenkanten.

Sie können Aufträge, die im Rahmen der Auftragserfassung nicht freigeschaltet wurden, nachträglich freischalten.
Mit der Freischaltung verlässt der Auftrag die Erfassungsebene und die Daten werden für andere A+W Enterprise-Komponenten (Produktion, Bestellwesen, Lager und Versand) aufbereitet und an diese übergeben.
Der Auftrag ist noch so lange änderbar, bis mit der Produktion begonnen bzw. eine Bestellung an den Lieferanten ausgelöst oder ein Lieferschein erzeugt wurde. Änderungen müssen erneut zur Weiterverarbeitung freigeschaltet werden.
⇨ Softwarereferenz, "Freischaltung" auf Seite D-1380

### Auftrag freischalten
1. Wählen Sie im Menü **Verkauf > Auftragsfreischaltung > Freischaltung**.
2. Wählen Sie mit `<F9>`, `<F8>` die Abteilung aus, in welcher der Vorgang erfasst wurde.
   Oder betätigen Sie `<Enter>`, um alle nicht freigeschalteten Vorgänge anzeigen zu lassen.
   Die Liste **Auftragsfreischaltung** mit allen noch nicht freigegebenen Aufträgen wird angezeigt.
3. Wählen Sie mit den `<Pfeiltasten>` den Vorgang aus, den Sie freischalten möchten.
4. Verändern Sie in der Spalte **frei** den Status.
5. Lösen Sie die Freischaltung mit `<F3>` aus.

Alle notwendigen Beschaffungsstellen (Lager, Einkauf, Produktion) werden mit der Auftragsfreischaltung über den Auftrag informiert und lösen ihrerseits die erforderlichen Beschaffungsmaßnahmen aus. Darüber hinaus wird der Auftrag mit der Freischaltung auch dem Versandsteuerungssystem gemeldet, um die erforderlichen Transportkapazitäten vorzuplanen.
⇨ Softwarereferenz, "Freischaltung" auf Seite D-1380

## Druck

> **Lernziele**
> - Formulardruck-Dialog kennenlernen.
> - Voraussetzungen für den Druck und E-Mail-Versand beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **VODR**: Der Zutritt zu dem Dialog Fomulardruck wird durch EDV-Modul-Kürzel VOKA gesteuert.
> - **VOEM**: Der Zutritt zu dem Dialog E-Mailversand wird durch EDV-Modul-Kürzel VOKA gesteuert

Mit dem Menüpunkt **Formulare** können Sie vorhandene Vorgänge wie Angebote, Aufträge, Auftragsbestätigungen usw. ausdrucken oder per E-Mail versenden. Falls Sie noch die Fax-Funktion nutzen, wird diese ebenfalls über diesen Menüpunkt erreicht.
Seit der Version 2008 bietet A+W Enterprise alle Druckfunktionen sowie die REPGO-Umgebung (Unix/Linux) als auch die Crystal Reports-Anbindung. Beide Möglichkeiten müssen vollständig konfiguriert werden.

> **Voraussetzungen**
> - Formulararten sind eingerichtet
> - Drucker (auch PDF- und E-Mail-Druck) sind eingerichtet.
> - E-Mail-Adressen der Kunden sind eingepflegt.
> - Faxnummern der Kunden sind eingepflegt.

### So arbeiten Sie im Dialog Formulare:
*(Screenshots der Dialoge Formularart und Formulardruck)*

1. Menü **Verkauf > Formulare > Druck**.
   Dialog **Formularart** wird geöffnet.
2. Formularart wählen und mit `<Ende>` übernehmen, z. B. **Rechnung**.
   Dialog **Formulardruck** wird geöffnet.
3. Voreinstellungen wählen und mit `<Enter>` übernehmen, z. B.:
	- 1 zusätzliches Exemplar.
	- Diverse Nummern vorgeben.
4. Feld **Vorgang**: mit `<F9>` Rechnungsnummer auswählen und übernehmen.
5. Rechnungsnummer(n) mit `[OK]` bestätigen.
   Dialog **Drucken auf** wird geöffnet.
6. Drucker auswählen und Druck der Rechnung mit `<Enter>` starten.

**Mehrere Rechnungen drucken:**
7. Voreinstellungen wählen, z. B. **Nummern auswählen** und mit `<Enter>` übernehmen.
8. Auftragsnummern eingrenzen, z. B. auf eigene Aufträge vom Vortag:
	- Mitarbeiternummer eingeben.
	- Erfassungsdatum eingrenzen.
	- Ersten und letzten Vorgang auswählen.
9. Mit `<F3>` Auftragsnummern des eingegrenzten Bereichs einlesen.
10. Feld **Dr**: zur Druckausgabe **J** oder **N** wählen.
11. Druck mit `<F3>` auslösen.
    Dialog **Drucken auf** wird geöffnet.
    Drucker auswählen und Druck der Rechnungen mit `<Enter>` starten.
⇨ Softwarereferenz, "Formulardruck" auf Seite D-1420

## Listendruck

> **Lernziele**
> - A+W Enterprise-Sprossenerfassung kennenlernen.
> - Bedienung im Sprosseneditor beherrschen.
> - Tipps und Tricks der Sprossenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **Symmetrie**: Aufbauart einer Sprossenkonstruktion. Wird dabei ein Gitternetz gleichmäßig aufgebaut, so spricht mal vom .feldsymmetrischen Sprossen.
> - **Bohrpunkt**: Befestigungspunkte der Sprossenkonstruktion an Iso-Rahmen.
> - **Lichtes Feld**: Abstand zwischen zwei waagerechten und zwei senkrechten Sprossenkanten.

Eine Auflistung verschiedener Stamm- und Bewegungsdaten ist über den Menüpunkt **Listendruck** erhältlich. Der Menüpunkt bietet eine sinnvolle Auswahl von auszudruckenden Listen, z. B. die Artikel- oder Kundenstammdaten, der Auftragsein- oder Rechnungsausgang, die Provisionsabrechnung oder die zur Verfügung stehenden Sprossenarten.

## Übersicht-Funktionen im Verkauf

> **Lernziele**
> - A+W Enterprise-Sprossenerfassung kennenlernen.
> - Bedienung im Sprosseneditor beherrschen.
> - Tipps und Tricks der Sprossenerfassung beachten.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Sprossen in einem Auftrag einfach erfassen und die freie Sprossenkonstruktion erstellen.
>
> **Merke**
> - **Symmetrie**: Aufbauart einer Sprossenkonstruktion. Wird dabei ein Gitternetz gleichmäßig aufgebaut, so spricht mal vom .feldsymmetrischen Sprossen.
> - **Bohrpunkt**: Befestigungspunkte der Sprossenkonstruktion an Iso-Rahmen.
> - **Lichtes Feld**: Abstand zwischen zwei waagerechten und zwei senkrechten Sprossenkanten.

Im Menüpunkt **Übersicht** finden Sie folgende Untermenüpunkte:
- **Übersicht**
- **Auftragsinformation**

### Übersicht
Der Menüpunkt **Übersicht** erlaubt das Anzeigen der erfassten Vorgänge nach verschiedenen Gesichtspunkten. Sie haben die Möglichkeit, unberechnete Aufträge, Aufträge mit Fakturasperre und ungebuchte Rechnungen anzeigen zu lassen.
Des Weiteren können Sie Informationen über den Status von Aufträgen, unvollständigen Lieferungen sowie Auftragsinformationen abrufen.
⇨ Softwarereferenz, "Recherche zu Vorgängen" auf Seite D-1445

### Auftragsinformation
Die Auftragsinformationen geben Ihnen Auskünfte zu den Status der einzelnen Auftragspositionen. Sie haben die Möglichkeit, sobald ein Dialog geöffnet wurde, mit `<F2>` in den verschiedenen Status zu blättern.

**Auftragsinformationen anzeigen**
1. Rufen Sie die Auftragsinformationen folgendermaßen auf:
	- im Menü **Verkauf > Übersicht > Auftragsinformation**
	  ⇨ Verkauf: Softwarereferenz, "Auftragsinformation" auf Seite D-1429
	- oder in den Kopfdaten oder Rumpfdaten mit `<Shift>` + `<F10>` **Auftragsinformation**
	  ⇨ Verkauf: Softwarereferenz, "Auftragspositionen - Status" auf Seite D-1188
2. Wählen Sie den entsprechenden Untermenüpunkt (Status) aus der Liste aus.
3s Wenn Sie das Menü **Auftragsinformation** nicht aus dem Auftrag heraus aufgerufen haben, geben Sie die Vorgangsnummer im Dialog **Vorgangs-Status** ein oder suchen Sie den Vorgang.
   ⇨ Tutorial, "Übersicht" auf Seite D-1049

## Hintergrund-Kontrollen
Der Menüpunkt **Kontrollen** gliedert sich in die Untermenüpunkte **Erfassungs-** und **Hintergrundkontrolle**.
Die **Erfassungskontrolle** präsentiert die bestehenden Aufträge in textueller Form. Dabei werden vor allem die preisrelevanten Daten der jeweiligen Positionen detailliert dargestellt.
Die **Hintergrundkontrolle** beinhaltet ein Fehlerinformationssystem, das alle Aufträge listet, bei denen Bearbeitungsfehler durch Hintergrundprozesse aufgetreten sind. Zur Korrektur können Sie den betreffenden Auftrag direkt aufrufen und nachbearbeiten.
⇨ Softwarereferenz, "Recherche zu Vorgängen" auf Seite D-1445

## Wiedervorlagen

> **Lernziele**
> - Unterschied zwischen vorgangsbezogener und freier Wiedervorlage kennenlernen.
> - Möglichkeit der Wiedervorlage-Funktion kennenlernen.
> - Nutzen der Funktion erkennen.
>
> **Nutzen**
> - Die Wiedervorlage-Funktion dient zur Erinnerung für Bearbeitung der Vorgängen, die nach bestimmten Kriterien definiert werden kann.
>
> **Merke**
> - **SYWV**: Der Zutritt zu dem Dialog Wiedervorlagemodus wird durch EDV-Modul-Kürzel SYWV gesteuert.

Terminlich orientierte Bearbeitungsvermerke werden in der Wiedervorlage abgelegt. Bei der Wiedervorlage besteht die Möglichkeit, den Text der Wiedervorlage direkt nach der Systemanmeldung am Monitor anzuzeigen oder im virtuellen Briefkasten der jeweiligen Mitarbeiter abzulegen.
Der Dialog Wiedervorlage ist ausführlich im folgenden Kapitel beschrieben:
⇨ Verkauf, "Wiedervorlage" auf Seite D-1463

Bei der freien Wiedervorlage entfällt die Bindung an einen Vorgang.
Bei der Vorgangsbezogenen Wiedervorlage für Angebote gilt der eingetragene Liefertermin als Vorlage-Datum. Diese Variante muss jedoch explizit konfiguriert werden.

Terminlich orientierte Bearbeitungsvermerke werden in der Wiedervorlage abgelegt. Dabei sind die **vorgangsbezogene** und die **freie Wiedervorlage** zu unterscheiden.
Die vorgangsbezogene Vorlage erfolgt im Rahmen der Vorgangserfassung, z. B. beim Anlegen eines Auftrages oder bei Ausstellung einer Rechnung.
Freie Wiedervorlagen dienen der Erinnerung an einen frei wählbaren Sachverhalt, der nicht in Bezug zu einem kaufmännischen Vorgang steht.
Sowohl bei der freien, als auch bei der vorgangsbezogenen Wiedervorlage können Sie den Text der Wiedervorlage direkt beim Einloggen am Monitor anzeigen lassen oder im virtuellen Briefkasten des jeweiligen Mitarbeiters ablegen.
⇨ Verkauf: Softwarereferenz, "Wiedervorlage" auf Seite D-1463

### Aktivierung der Wiedervorlage
1. Öffnen Sie den Dialog **Wiedervorlagemodus** (System > Vorgangsverwaltung > Wiedervorlagemodus).
   A+W Enterprise zeigt den Dialog **Wiedervorlage** an.
2. Wählen Sie im Feld **Vorgang** die Vorgangsart, für die das Wiedervorlagemodus gelten soll.
3. Bestimmen Sie im Feld **Modus**, wie es mit der Wiedervorlage umgegangen werden soll. Folgende Möglichkeiten stehen Ihnen zur Verfügung:
	- **keine Vorlage**: für die ausgewählte Vorgangsart wird keine automatische Wiedervorlage angelegt
	- **zwingende Vorlage**: beim Speichern der hier ausgewählten Vorgangsart wird automatisch der Wiedervorlage-Dialog geöffnet. der Wiedervorlage-Dialog kann nur mit vollständigen Angaben speichernd verlassen werden.
	  ⇨ "Vorgangsbezogene Wiedervorlage anlegen" auf Seite D-1052
	- **autom. Vorlage nach**: bei diesem Modus geben Sie im Folgefeld (Tage) Anzahl der Tagen, nach deren Ablauf die Wiedervorlage automatisch angelegt wird.
	- **autom. Löschen nach**: bei diesem Modus geben Sie im Folgefeld (Tage) Anzahl der Tagen, nach deren Ablauf die Wiedervorlage automatisch gelöscht wird.

### Vorgangsbezogene Wiedervorlage anlegen
1. Öffnen Sie ein Dialog zur Vorgangserfassung, z. B. Auftragserfassung.
2. Über `<F4>` auf jeder Vorgangsebene (Kopf, Rumpf, Fuß) starten Sie den Dialog **Wiedervorlage**.
3. Füllen Sie die Felder im Dialog **Wiedervorlage** aus.
   ⇨ "Dialog Wiedervorlage ausfüllen" auf Seite D-1052

### Freie Wiedervorlage anlegen
1. Öffnen Sie im Menü **Verkauf > Wiedervorlagen**.
   A+W Enterprise zeigt den Dialog **Wiedervorlage** an.
2. Füllen Sie die Felder im Dialog **Wiedervorlage** aus.
   ⇨ "Dialog Wiedervorlage ausfüllen" auf Seite D-1052
3. Füllen Sie die Felder im Dialog **Wiedervorlage** aus.

### Dialog Wiedervorlage ausfüllen
1. Wählen Sie ein Datum für die Wiedervorlage im Feld **Vorl-Datum** aus.
   Wenn der Wiedervorlage-Termin erreicht ist, bekommt der gewählte Mitarbeiter eine Nachricht als Texteinblendung am Bildschirm oder per E-Mail, sofern Sie weitere Felder entsprechend ausfüllen.
2. Wählen Sie die Vorlageart aus, der die Wiedervorlage erhalten soll. Folgende Möglichkeiten stehen Ihnen zur Verfügung:
	- **Mitteilung in Meldesystem**: bei diesem Modus geben Sie im Folgefeld (Mitarbeiter) die Mitarbeiternummer, an dem die Wiedervorlage E-Mail versendet wird. Die Nachrichten werden dem Anwender über das Nachrichtensystem übermittelt. Mit `<Strg>` + `<F4>` rufen Sie die Nachrichten im Systemmenü ab. Falls eine E-Mail-Adresse in den Mitarbeiter-Stammdaten hinterlegt wurde, wird dem Nachrichtenempfänger eine externe E-Mail zugesendet.
	- **Aktive Wiedervorlage**: bei diesem Modus geben Sie im Folgefeld (Mitarbeiter) die Mitarbeiternummer denjenigen, der die Wiedervorlage (auf dem Bildschirm beim Start des Programms) aktiv bekommt.
	- **direktes Löschen des Vorgangs**: bei diesem Modus geben Sie im Folgefeld (Anmerkung) einen Hinweis, warum der Vorgang gelöscht wird. Diese Option ist nur bei Kundenangeboten und Lieferantenanfragen zulässig. Nach Ablauf der Frist (Am Vorl-Datum) wird der entsprechende Vorgang stillgelegt und der Wiedervorlage-Text als Storno-Grund eingetragen.
3. Tragen Sie die Mitarbeiternummer, der die Wiedervorlage erhält, ein. Standardmäßig ist der Vorgangserfasser bzw. A+W Enterprise - Anwender voreingestellt.
4. Notieren Sie den Wiedervorlage-Text.
5. Um weitere Wiedervorlage-Termine für diesen Vorgang (vorgangsbezogenes Dialogausfüllen) oder eine weitere freie Wiedervorlage anzulegen, drücken Sie die beiden Textfelder mit `<Enter>` durch oder betätigen die Taste `<F6>`, um direkt eine weitere Wiedervorlage anzulegen.
   Es werden neue Zeilen eingeblendet.
   Sie können auf diese Art und Weise beliebig viele Wiedervorlagen hinterlegen.
6. Mit `<F7>` löschen Sie die nicht mehr benötigte Wiedervorlage.
7. Speichern Sie den Dialog mit `<ENDE>`.

## Modifikations-Funktionen im Verkauf

In der folgenden Tabelle haben Sie einen kurzen Überblick über weitere Funktionen im Bereich Verkauf.

| Funktion | Beschreibung |
| :--- | :--- |
| **Fertigmeldung** | Mit Hilfe von Fertigmeldungen erfolgt die Mitteilung des aktuellen Produktionsstatus an A+W Enterprise. Fertigmeldungen beziehen sich auf eine Mengeneinheit. So kann eine Fertigmeldung auch über teilgelieferte Mengen einer Position erfolgen. Die manuelle Fertigmeldung entspricht nicht dem üblichen Vorgehen und ist nur für kleine Handelsbetriebe sinnvoll nutzbar. Fertigmeldungen sollten aus Produktion oder Einkauf übermittelt werden. ⇨ Softwarereferenz, "Fertigmeldung" auf Seite D-1464. |
| **Vorgangsänderung** | Funktion zur Änderung von bestimmten Auftragsdaten, ohne den Vorgang zu betreten. ⇨ "Vorgangsänderung" auf Seite D-1055 |
| **Vertrieb** | Vertriebsmitarbeiter können ihre Besuchsberichte, Besuchsstatistiken und Provisionsabrechnungen über A+W Enterprise verwalten, bearbeiten und erzeugen. Hierüber hinaus werden Budgets, die das gesamte Unternehmen betreffen, genauso unterstützt wie eine umfassende Objektbudgetierung. So können beispielsweise Verteilungsmatrizen, Verteilungsvektoren, Budgetierung und Soll-Ist-Vergleiche für das Unternehmen erstellt werden. Die Objektbudgetierung umfasst eine Vielzahl von Anwendungsmöglichkeiten, von der Verwaltung von Objektkonten und Objektlisten, Montagekosten bis hin zur Lohnabrechnung. Für weitere Informationen zu diesem Bereich kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH. |

## Vorgangsänderung

> **Lernziele**
> - Dialogbedienung kennenlernen.
> - Roten- bzw. Liefertermin-Änderung durchführen.
> - Voraussetzungen und Einschränkungen der Funktion erkennen.
>
> **Nutzen**
> - Schnelle und einfache Änderung eines oder mehreren Auftrag/-e durchführen.
> - Gleichzeitige Änderung mehrere Angebote, Aufträge und Lieferscheine vornehmen.
>
> **Merke**
> - **VOKA**: Der Zutritt zu dem Dialog Vorgangsänderung wird durch Auftragserfassung-EDV-Modul-Kürzel VOKA gesteuert.

In dem Dialog **Vorgangsänderung** können Sie einige Vorgangsdaten ändern, ohne dafür den Vorgang in der entsprechenden Dialog laden zu müssen. Für folgende Vorgangsarten können Sie auf diese Art und Weise Änderungen vornehmen:
- Angebot
- Auftrag
- Lieferschein

Ein weiterer Vorteil an dieser Funktion: Sie können für mehrere Vorgängen die Änderungen gleichzeitig vornehmen. Änderbar sind z. B., der geplante Liefertermin, die Route, Stornostatus sowie die Mandantennummer.
Die Änderungen an Aufträgen werden erneut an das Produktionssystem und die Versandsteuerung übergeben, sofern der Auftrag bereits schon einmal freigegeben wurde. Wurde der Auftrag bislang noch nicht an den Versand übergeben oder steht er noch im Freigabepool, so werden die relevanten Felder nicht betretbar.
Die Änderungen an Angeboten werden nur dann an das Produktionssystem übergeben, wenn das System dafür konfiguriert ist.
Die Änderungen an Lieferscheinen sind nur solange möglich, bis das Lieferschein noch offen ist und nicht als komplett geliefert gilt.
Änderungen, die nicht an die nachfolgenden Prozesse weitergegeben werden, werden mit **Lokale Änderung** gekennzeichnet. Aufträge mit diesem Kennzeichen müssen z. B. manuell an den Versand übergeben werden.

Folgende Einschränkungen sind zu beachten:
- Bei Callcenter Aufträge, die bei Nutzung der Mehrmandantenlogik in A+W iQuote - Enterprise erfasst sind, kann keine Hausänderung über diese Funktion vorgenommen werden.

### So führen Sie die Vorgangsänderung schnell durch
*(Screenshot des "Vorgangsänderung" Dialogs)*

1. Menü **Verkauf > Vorgangsänderung** wählen.
   Dialog **Vorgangsänderung** wird geöffnet.
2. Feld **Vorgang**: Vorgangsart wählen. z. B. Auftrag.
3. Feld **Nummer**: `<F9>` drücken.
   Dialog **Suche Aufträge** wird geöffnet.
4. Feld **Kunde**: Kundennummer eingeben und Suche starten.
   Trefferliste wird angezeigt.
5. Auftrag mit Doppelklick in Dialog **Vorgangsänderung** übernehmen.
6. In die Felder springen und Einstellung ändern, z. B.:
	- Feld **Lokale Korrekt.**: Freien Text eingeben.
	- Feld **Sto**: Stornokennzeichen setzen.
	- Feld **Route**: Route ändern.
	- Feld **Termin**: Liefertermin ändern.
	- Feld **Frei**: Änderungen freischalten.
7. Änderungen mit `<F3>` ausführen.
   Zum Überprüfen können Sie mit `<Shift>` + `<F5>` in den aktuellen Vorgang wechseln:
8. Vorgang mit Doppelklick zur Bearbeitung öffnen.
9. Daten prüfen und ggf. ändern.
   Änderungen mit `[OK]` speichern.
10. Sie kehren zum Dialog **Vorgangsänderung** und können so weitere Änderungen durchführen.

### So können Sie bestimmte Kosten schnell anpassen
Da die Zuschläge wegen steigenden Energiekosten heute sehr oft angepasst werden müssen, gibt es auch eine Möglichkeit diese in den bestehende Vorgängen zu aktualisieren. Sie können einen passenden Skripte selbst oder mit Hilfe des A+W Service-Mitarbeiter erstellen, um diese Vorgänge vor den Hintergrundprozess `intauf` mit (still=-26) zu stellen. Diese `intauf`-Art wird die über die Umgebungsvariable `RABATTMETHODEN_UPDATE` definierte Methoden aktualisieren und den Auftrag neu berechnet.
Diese Aktualisierung können Sie auch im Dialog **Vorgangsänderung** ansteuern.

1. Starten Sie den Dialog **Vorgangsänderung**.
2. Wählen Sie ein oder mehrere Aufträge aus.
3. Wechseln Sie mit `<F2>` in die 3. Registerkarte **Kalkulation**.
4. Wählen Sie im Feld **Rabatte** die Art der Änderung aus. Dabei werden die gewählte Aufträge mit einer entsprechenden `inatauf`-Art dem Hintergrundprozess erneut vorgelegt. Folgende Möglichkeiten stehen Ihnen zur Auswahl an:
	- Vorhanden Rabatte aktualisieren (intauf-26)
	- Einfügen der neue Rabattmetoden (intauf -28)
	- Alle Rabatte neu ziehen und den Auftrag neu aufsummieren
5. Führen Sie die Aktion mit `<F3>` aus.
   Diese Funktionalität steht nur für nicht fakturierte Aufträge, Angebote oder Lieferscheine zu Verfügung.

### So lassen Sie einen Angebot oder einen Auftrag neue kalkulieren
1. Starten Sie den Dialog **Vorgangsänderung**.
2. Wählen Sie ein oder mehrere Aufträge aus.
3. Wechseln Sie mit `<F2>` in die 3. Registerkarte **Kalkulation**.
4. Wählen Sie im Feld **Kalkulation** die Art der Änderung aus, die entsprechend an den Hintergrundprozess übergeben wird. Folgende Möglichkeiten stehen Ihnen zur Auswahl an:
	- VK - Nur Verkaufspreise neue kalkulieren lassen
	- EK - Nur Einkaufspreise neue kalkulieren lassen
	- VK+EK - den Auftrag komplett neue kalkulieren lassen
5. Führen Sie die Aktion mit `<F3>` aus.
   Diese Funktionalität steht ebenfalls nur für nicht fakturierte Aufträge, Angebote oder Lieferscheine zu Verfügung.

---
# A+W Enterprise Verkauf: Softwarereferenz

## Übersicht
Im Modul **Verkauf** verwalten Sie die Vorgänge, die zur erfolgreichen Abwicklung des Verkaufsgeschäfts erforderlich sind. Sie erfassen z. B. Angebote, Aufträge und Gutschriften und erstellen Rechnungen.

Im Part Verkauf finden Sie folgende Themen:
- "Suchfunktionen" auf Seite D-1076
- "Vorgangsverwaltung" auf Seite D-1127
- "Technische Werte" auf Seite D-1243
- "Stückliste" auf Seite D-1252
- "Packmittelplanung" auf Seite D-1295
- "Anmerkungen" auf Seite D-1304
- "Texte" auf Seite D-1312
- "Preise und Konditionen" auf Seite D-1322
- "Freischaltung" auf Seite D-1380
- "Lieferung" auf Seite D-1385
- "Rechnungen" auf Seite D-1397
- "Gutschriften" auf Seite D-1414
- "Formulare" auf Seite D-1419
- "Auftragsstatus" auf Seite D-1429
- "Recherche zu Vorgängen" auf Seite D-1445
- "Übersichten zu Vorgängen" auf Seite D-1461
- "Vertrieb" auf Seite D-1473

---

*Die folgenden Seiten D-1066 bis D-1075 sind eine detaillierte Referenz der Menüstruktur und werden hier als Listen und Tabellen dargestellt.*

## Menüstruktur Referenz

### Menü Verkauf (D-1066)
Einige der verfügbaren Menü-Einträge verzweigen in Untermenüs. Wenn diese mehr als drei Einträge umfassen, sind sie nach der folgenden Übersicht separat aufgeführt. Die angezeigten Einträge sind von der jeweiligen Konfiguration abhängig.

> **Kontext-Menüs**
> In den Kontext-Menüs (rechte Maustaste) werden zu den einzelnen Feldern der Dialoge jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen in den Kontext-Menüs können Sie auch über die beschriebenen Menüs aufrufen. In der Regel entsprechen die Menüpunkte im Kontext-Menü den angebotenen Funktionen in der Prompt-Anzeige.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Schnellerfassung | ⇨ "Schnellerfassung" auf Seite D-1131 |
| `b` | Angebotserfassung | ⇨ "Angebotserfassung" auf Seite D-1132 |
| `c` | Auftragserfassung | ⇨ "Auftragserfassung" auf Seite D-1134 |
| `d` | Preiskalkulation | ⇨ "Preiskalkulation" auf Seite D-1379 |
| `e` | Preislose Erfassung | ⇨ "Preislose Erfassung" auf Seite D-1133 |
| `f` | Lieferscheine | |
| `fa` | • Automatische Freigabe | ⇨ "Lieferscheine (automatisch)" auf Seite D-1392 |
| `fb` | • Manuelle Lieferscheine | ⇨ "Lieferscheine (manuell)" auf Seite D-1394 |
| `fc` | • Protokoll | ⇨ "Lieferscheinprotokoll" auf Seite D-1396 |
| `g` | Rechnungen | ⇨ "Untermenü Rechnungen" auf Seite D-1067 |
| `h` | Gutschriften | |
| `ha` | • Gutschriften erfassen | ⇨ "Gutschriften" auf Seite D-1414 |
| `hb` | • Gutschriften buchen | ⇨ "Gutschriften buchen" auf Seite D-1416 |
| `i` | Auftragsfreischaltung | |
| `ia` | • Freischaltung | ⇨ "Auftragsfreischaltung" auf Seite D-1380 |
| `ib` | • Autorisierung | ⇨ "Autorisierung" auf Seite D-1383 |
| `j` | Formulare | |
| `ja` | • Druck | ⇨ "Formulardruck" auf Seite D-1420 |
| `jb` | • E-Mail/Fax | ⇨ "E-Mail" auf Seite D-1424 |
| `k` | Listendruck | ⇨ "Listendruck" auf Seite D-1428 |
| `l` | Übersicht | ⇨ "Untermenü Übersicht" auf Seite D-1068 |
| `m` | Hintergrund-Kontrolle | ⇨ "Fehlerinformationssystem" auf Seite D-1240 |
| `n` | Wiedervorlagen | ⇨ "Wiedervorlage" auf Seite D-1463 |
| `o` | Fertigmeldung | ⇨ "Fertigmeldung" auf Seite D-1464 |
| `p` | Vorgangsänderung | ⇨ "Vorgangsänderung" auf Seite D-1466 |
| `r` | Vertrieb | ⇨ "Vertrieb" auf Seite D-1473 |

### Untermenü Rechnungen (D-1067)
Verkauf > Rechnungen
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Automatische Freigabe | ⇨ "Rechnungen (automatisch)" auf Seite D-1398 |
| `b` | Manuelle Rechnung | ⇨ "Rechnungen (manuell)" auf Seite D-1403 |
| `c` | Thekenrechnung | ⇨ "Thekenrechnung" auf Seite D-1404 |
| `d` | Rechnungen buchen | ⇨ "Rechnungen buchen" auf Seite D-1405 |
| `e` | Abschlagsrechnung | |
| `ea` | • Automatische Freigabe | ⇨ "Abschlagsrechnung (automatisch)" auf Seite D-1408 |
| `eb` | • Manuelle Rechnung | ⇨ "Abschlagsrechnung (manuell)" auf Seite D-1410 |
| `f` | Schlussrechnung | |
| `fa` | • Automatische Freigabe | ⇨ "Schlussrechnung (automatisch)" auf Seite D-1411 |
| `fb` | • Manuelle Rechnung | ⇨ "Schlussrechnung (manuell)" auf Seite D-1412 |
| `g` | Protokoll | ⇨ "Rechnungsprotokoll" auf Seite D-1413 |

### Untermenü Übersicht (D-1068)
Verkauf > Übersicht
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Unberechnete Aufträge | ⇨ "Übersicht zu Vorgängen" auf Seite D-1471 |
| `b` | Ungebuchte Rechnungen | |
| `c` | Unvollständige Lieferungen | |
| `d` | Aufträge mit Fakturasperre | |
| `e` | Bearbeitungsstände | Das Modul wird nicht mehr genutzt. |
| `f` | Nummern-Ermittlung | Das Modul wird nicht mehr genutzt. |
| `g` | Auftragsanzeige | ⇨ "Auftragsanzeige" auf Seite D-1461 |
| `h` | Angebotsanzeige | ⇨ "Angebotsanzeige" auf Seite D-1462 |
| `i` | Auftragsinformation | ⇨ "Auftragsinformation" auf Seite D-1429 |
| `j` | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" auf Seite D-1445 |

### Zusatzmenü (`<F4>`) (D-1068)
Das Zusatzmenü rufen Sie mit `<F4>` beim Erfassen der verschiedenen Vorgänge auf. Je nach Dialog und Bereich werden die Einträge in verschiedenen Ausführungen angezeigt.

#### Zusatzmenü für den Kopf- und Fußbereich (Vorgangserfassung) (D-1068)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Texte | |
| `aa` | • Kopftext | ⇨ "Kopf- und Fußtexte" auf Seite D-1313 |
| `ab` | • Fußtext | ⇨ "Kopf- und Fußtexte" auf Seite D-1313 |
| `ac` | • Fremdinformationen | ⇨ "Fremdinformationen" auf Seite D-1319 |
| `b` | Adressen | ⇨ "Untermenü Adressen" auf Seite D-1070 |
| `c` | Ansprechpartner | ⇨ "Ansprechpartner" auf Seite D-1199 |
| `d` | Storno | ⇨ "Auftragspositionen" auf Seite D-1167 |
| `e` | Preisangaben | ⇨ "Untermenü Preisangaben" auf Seite D-1071 |
| `f` | Produktangaben | ⇨ "Untermenü Produktangaben" auf Seite D-1072 |
| `g` | Wiedervorlage | ⇨ "Wiedervorlage" auf Seite D-1463 |
| `h` | Übergabe an Produktion (erneut) | Den Auftrag nach dem Speichern automatisch an die Produktion übergeben. |
| `i` | Produktionsmonitor | ⇨ "Produktionsmonitor" auf Seite D-1242 |
| `j` | Lieferplan | ⇨ "Lieferplan" auf Seite D-1386 |
| `k` | Lieferinformation | ⇨ "Lieferinformation - Details der Auslieferung" auf Seite D-1388 |
| `l` | Zahlungsplan | ⇨ "Zahlungsplan" auf Seite D-1238 |
| `m` | Zahlungsverwaltung | ⇨ "Zahlungsverwaltung" auf Seite D-1236 |
| `n` | Konfigurierbare Felder | ⇨ "Konfigurierbare Felder" auf Seite D-1201 |
| `o` | Hauswechsel | ⇨ "Hauswechsel" auf Seite D-1192 |
| `p` | Direktdruck | ⇨ "Direktdruck" auf Seite D-1419 |

#### Zusatzmenü für die Positionsebene (Vorgangserfassung) (D-1069)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Texte | ⇨ "Untermenü Texte" auf Seite D-1070 |
| `b` | Adressen | ⇨ "Untermenü Adressen" auf Seite D-1070 |
| `c` | Storno | ⇨ "Auftragspositionen" auf Seite D-1167 |
| `d` | Private Felder | ⇨ "Private Felder" auf Seite D-1221 |
| `e` | Preisangaben | ⇨ "Untermenü Preisangaben" auf Seite D-1071 |
| `f` | Produktangaben | ⇨ "Untermenü Produktangaben" auf Seite D-1072 |
| `g` | Wiedervorlage | ⇨ "Wiedervorlage" auf Seite D-1463 |
| `h` | Kommissionen | |
| `ha` | • neue Kommission | in das Feld Kommis im Register Positionen wechseln, um einen Kommissionstext anzulegen oder zu bearbeiten |
| `hb` | • Kommission ändern | ⇨ "Auftragspositionen - Allgemein" auf Seite D-1167 |
| `i` | Lieferplan | ⇨ "Lieferplan" auf Seite D-1386 |
| `j` | Lager | |
| `ja` | • Stapel (Strg+P) | Das Feld Stapel im Register Allgemein anzeigen. (optionale, kundenspezifische Funktion) |
| `jb` | • Lagerprognose (Strg+G) | ⇨ "Bestandsprognose" auf Seite D-1206 |
| `k` | Zahlungsplan | ⇨ "Zahlungsplan" auf Seite D-1238 |
| `l` | Konfigurierbare Felder | ⇨ "Konfigurierbare Felder" auf Seite D-1201 |

#### Untermenü Adressen (`<F4>` > Adressen) (D-1070)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Lieferadresse suchen (Strg+L) | ⇨ "Adressen Suche" auf Seite D-1099 |
| `b` | Neue Lieferadresse (Strg+N) | ⇨ "Neue Lieferadresse" auf Seite D-1192 |
| `c` | Lieferadresse löschen | Die Lieferadresse aus dem Vorgang löschen. |
| `d` | Endkundenanschrift | ⇨ "Endkundenanschrift" auf Seite D-1195 |

#### Untermenü Texte (`<F4>` > Texte) (D-1070)
(Einträge Artikeltext (F5), Positionstext (Shift+F5) und Spezielle Texte werden nur auf Positionsebene angezeigt)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Kopftext | ⇨ "Kopf- und Fußtexte" auf Seite D-1313 |
| `b` | Fußtext | ⇨ "Kopf- und Fußtexte" auf Seite D-1313 |
| `c` | Fremdinformationen | ⇨ "Fremdinformationen" auf Seite D-1319 |
| `d` | Artikeltext (F5) | ⇨ "Artikel- und Positionstexte" auf Seite D-1315 |
| `e` | Positionstext (Shift+F5) | ⇨ "Artikel- und Positionstexte" auf Seite D-1315 |
| `f` | Spezielle Texte | ⇨ "Untermenü Spezielle Texte" auf Seite D-1071 |

#### Untermenü Spezielle Texte (`<F4>` > Texte > Spezielle Texte) (D-1071)
(optionale, kundenspezifisch konfigurierte Funktion)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Rahmentext | ⇨ "Spezielle Texte" auf Seite D-1316 |
| `b` | Produktkennzeichen | |
| `c` | Modelltexte | |
| `d` | Logotexte | |

#### Untermenü Preisangaben (`<F4>` > Preisangaben) (D-1071)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Auftragskonditionen | ⇨ "Positionskonditionen" auf Seite D-1340 |
| `b` | Auftragspreise | ⇨ "Untermenü Auftragspreise" auf Seite D-1072 |
| `c` | Teilkalkulation | ⇨ "Produktionskostenkalkulation" auf Seite D-1372 |
| `d` | Neue Kalkulation | |
| `e` | Rabatte neu ermitteln | |
| `d + e` | Konditionen holen | (Nur Position) ⇨ "Positionskonditionen" auf Seite D-1340 |
| `f` | Preisberechnung | (Nur Position) Den Verkaufspreis mit den Positionskonditionen ermitteln und den Preis neu berechnen. |
| `g` | Preiskontrolle | (Nur Position) Die Felder zur Preiskontrolle im Register Allgemein anzeigen. |

#### Untermenü Auftragspreise (`<F4>` > Preisangaben > Auftragspreise) (D-1072)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Artikelpreise | ⇨ "Auftragspreise" auf Seite D-1328 |
| `b` | Sprossenpreise | ⇨ "Auftragssprossenpreise" auf Seite D-1330 |
| `c` | Austauschpreise | ⇨ "Auftragsaustauschpreise" auf Seite D-1333 |
| `d` | Unterteilpreise | ⇨ "Auftragsunterteilpreise" auf Seite D-1335 |

#### Untermenü Produktangaben (`<F4>` > Produktangaben) (D-1072)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Produktaustausch | ⇨ "Produktaustausch" auf Seite D-1209 |
| `b` | A/Z-Regeln | ⇨ Stammdaten |
| `c` | Warengruppe (nur Position) | Die Warengruppe bearbeiten. Der Cursor wechselt in das Feld Warengrp. |
| `d` | Technische Werte (nur Position) | ⇨ "Untermenü Technische Werte" auf Seite D-1073 |

#### Untermenü Technische Werte (`<F4>` > Produktangaben > Technische Werte) (D-1073)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Technische Werte anzeigen | ⇨ "Register Positionen (linker Bereich)" auf Seite D-1168 |
| `b` | Technische Werte ändern | ⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" auf Seite D-1170 |
| `c` | Leistungserklärung | ⇨ "Leistungserklärung" auf Seite D-1243 |
| `d` | Verdeckte Maßangaben anzeigen | ⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" auf Seite D-1170 |
| `e` | Verdeckte Maßangaben ändern | ⇨ “Artikel-Maßangaben" auf Seite D-1205 |

### Infomenü (`<Shift>` + `<F4>`) (D-1074)
Je nach Dialog und Bereich werden die Einträge im Infomenü in verschiedenen Ausführungen angezeigt.

#### Infomenü für den Kopf- und Fußbereich (Vorgangserfassung)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Vorgangs-Anmerkungen | ⇨ "Anmerkungen" auf Seite D-1304 |
| `b` | Marktpartner-Anmerkungen | |
| `c` | Objekt-Anmerkungen | |
| `d` | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" auf Seite D-1445 |
| `e` | Vorgangs-Übersicht | ⇨ "Übersicht" auf Seite D-1202 |
| `f` | Marktpartner-Information | ⇨ "Marktpartner-Info" auf Seite D-1197 |
| `g` | Änderungsprotokoll | ⇨ "Änderungs-Protokoll" auf Seite D-1230 |
| `h` | Lieferterminänderungen | ⇨ "Lieferterminänderungs-Protokoll" auf Seite D-1232 |
| `i` | Auftragsinformation | ⇨ "Auftragsinformation" auf Seite D-1429 |
| `k` | Kistensignatur | ⇨ "Kistensignatur" auf Seite D-1320 |
| `l` | Dokumentenarten | ⇨ "DXF Import" auf Seite D-1229 |
| `m` | Dokumentenübersicht | ⇨ "Dokumentenartenzuordnung" auf Seite D-1225 |

#### Infomenü für die Positionsebene (Vorgangserfassung)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Anmerkungen | ⇨ "Untermenü Anmerkungen" auf Seite D-1075 |
| `b` | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" auf Seite D-1445 |
| `c` | Vorgangs-Übersicht | ⇨ "Übersicht" auf Seite D-1202 |
| `d` | Marktpartner-Information | ⇨ "Marktpartner-Info" auf Seite D-1197 |
| `e` | Änderungsprotokoll | ⇨ "Änderungs-Protokoll" auf Seite D-1230 |
| `f` | Lieferterminänderungen | ⇨ "Lieferterminänderungs-Protokoll" auf Seite D-1232 |
| `g` | Auftragsinformation | ⇨ "Auftragsinformation" auf Seite D-1429 |
| `h` | Kistensignatur | ⇨ "Kistensignatur" auf Seite D-1320 |
| `i` | Dokumentenübersicht | ⇨ "Dokumentenartenzuordnung" auf Seite D-1225 |

#### Untermenü Anmerkungen (`<Shift>` + `<F4>` > Anmerkungen) (D-1075)
| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| `a` | Vorgangs-Anmerkungen | ⇨ "Anmerkungen" auf Seite D-1304 |
| `b` | Artikel-Anmerkungen | |
| `c` | Kunden-Anmerkungen | |
| `d` | Kunden-Artikel-Anmerkungen | |
| `e` | Objekt-Anmerkungen | |
| `f` | Objekt-Artikel-Anmerkungen | |
| `g` | Lieferanten-Anmerkungen | |
| `h` | Lieferanten-Artikel-Anmerkungen | |

## Suchfunktionen
Sie können im Modul **Verkauf** über unterschiedliche Kriterien nach Vorgängen, Marktpartnern, Adressen und Artikeln suchen. Die Suchdialoge sind für alle Vorgangsarten im Verkauf gleich aufgebaut. Sie werden in diesem Kapitel am Beispiel **Auftrag** beschrieben. Abweichungen werden explizit beschrieben.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Suche Aufträge" auf Seite D-1077
- "Suche Aufträge - Trefferliste" auf Seite D-1082
- "Marktpartnersuche" auf Seite D-1091
- "Mitarbeiter/Berechtigungsgruppen" auf Seite D-1095
- "Suche Bezugsvorgang" auf Seite D-1097
- "Adressen Suche" auf Seite D-1099
- "Artikel-Suche" auf Seite D-1101
- "Artikel-Suche nach Typen" auf Seite D-1110
- "Produktsuche nach Elementen" auf Seite D-1111
- "Objekt-Suche" auf Seite D-1118
- "Werteingabe - Erweiterte Suche" auf Seite D-1123

### Suche Aufträge
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9>`

In diesem Dialog suchen Sie nach Aufträgen. Im Kopfbereich geben Sie die Suchkriterien an. Mit jedem Kriterium, das Sie angeben, können Sie die Treffermenge reduzieren.

In diesem Dialog finden Sie im Kopfbereich folgende Register:
- "Suche Aufträge - Vorgangs-Schlüssel" auf Seite D-1077
- "Suche Aufträge - Positions-Schlüssel" auf Seite D-1080
- "Suche Aufträge - Direkte Suche" auf Seite D-1081

Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.
⇨ "Suche Aufträge - Trefferliste" auf Seite D-1082

#### Suche Aufträge – Vorgangs-Schlüssel
*(Screenshot des "Suche Aufträge" Dialogs, Register "Vorgangs-Schlüssel")*

In diesem Register suchen Sie Aufträge anhand von Auftragsdaten. Es ist konfigurierbar, in welchem Suchkriterienfeld Sie sich für die Eingabe zuerst befinden, wenn sie den Dialog öffnen. Konfigurierbar als erste Eingabefelder im Register **Vorgangs-Schlüssel** sind die Felder **Aufträge ab, Kunde, Objekt, Rechnungsnummer, Liefertermin, Bestelldatum, USt-Ident-Nr., Erfasser, Erfassungsdatum** und **Währung**.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Felder im Vorgangs-Schlüssel**
- **Aufträge ab**: Nummer, ab der nach Aufträgen gesucht wird. Die Suche wird auf alle Aufträge beschränkt, deren Nummer gleich oder größer der angegebenen Auftragsnummer ist. Der Feldname variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. **Angebote ab**.
  *Technische Info: numerisches Feld, DB-Feld: `kauf.auftrnr`*
- **Kunde**: Kundennummer. Die Suche wird auf alle Aufträge von diesem Kunden beschränkt. Wenn Sie eine Nummer angeben, wird der Kundenname im Klartext angezeigt.
  *Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: `kauf.kunr`, `kauf.orgname`*
- **Hausnummer**: Mandantennummer. Standardmäßig ist die Nummer des eigenen Hauses vorbelegt. Die Suche wird auf alle Aufträge aus diesem Haus beschränkt. Das Feld kann nur bearbeitet werden, wenn Sie mit der internen Mandantentrennung arbeiten.
  *Technische Info: numerisches Feld, DB-Feld: `kauf.hausnr`*
- **Objekt**: Objektnummer, für die Aufträge gesucht werden. Die Suche wird auf alle Aufträge mit diesem Objekt beschränkt. Der Objektname wird nach Eingabe der Nummer im Klartext angezeigt.
  *Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: `kauf.objnr`, `kauf.orgname`*
- **Fremdnummer**: Auftragsnummer, die vom Kunden vorgegeben wird. Die Suche wird auf alle Aufträge mit dieser Fremdnummer beschränkt. Durch eine Konfiguration kann die Suche nach Fremdnummern in der Vorgangssuche so umgestellt, dass sie ohne Berücksichtigung von Groß- und Kleinschreibung erfolgt.
  *Technische Info: alphanumerisches Feld, DB-Feld: `kauf.exaufnr`*
- **Org. Vorgang**: Original-Vorgangsnummer bei übertragenen Vorgängen. Die Suche wird auf alle Aufträge mit diesem Referenzvorgang beschränkt.
  *Technische Info: numerisches Feld, DB-Feld: `kauf._orgauftrnr`*
- **Rechnungsnummer**: Die Suche wird auf alle Aufträge beschränkt, zu denen diese Rechnung erstellt wurde.
  *Technische Info: numerisches Feld, DB-Feld: `kauf.rechnr`*
- **Liefertermin**: Gewünschter Liefertermin des Auftrags. Die Suche wird auf alle Aufträge mit diesem Liefertermin beschränkt. Der Liefertermin kann als Datum oder Kalenderwoche angegeben sein. In der Trefferliste wird der geplante Liefertermin angezeigt.
  *Technische Info: Datumsfeld, DB-Feld: `kauf.ltplan`*
- **Bestelldatum**: Bestelldatum des Auftrags. Die Suche wird auf alle Aufträge mit diesem Bestelldatum beschränkt.
  *Technische Info: Datumsfeld, DB-Feld: `kauf.bdat`*
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Kunden. Die Suche wird auf alle Aufträge mit dieser Identifikationsnummer beschränkt.
  *Technische Info: alphanumerisches Feld, DB-Feld: `kaufp.steuernr`*
- **Erfasser**: Mitarbeiternummer des Sachbearbeiters, der die Aufträge erfasst hat. Die Suche wird auf alle Aufträge von diesem Erfasser beschränkt.
  *Technische Info: numerisches Feld, DB-Feld: `kauf.eusr`*
- **Erfassungsdatum**: Datum der Auftragserfassung. Die Suche wird auf alle Aufträge mit diesem Erfassungsdatum beschränkt.
  *Technische Info: Datumsfeld, DB-Feld: `kauf.edat`*
- **Währung**: Währung, die dem Auftrag zugeordnet ist. Die Suche wird auf alle Aufträge mit dieser Währung beschränkt.
  *Technische Info: numerisches Feld, DB-Feld: `kauf.waehrung`*

**Fußbereich**
- `Neue Suche`: Löscht alle Suchkriterien für eine neue Suche. Alternativ können Sie mit `<Strg>` + `<F7>` die Suchkriterien löschen.
- `Suchen`: Startet die Suche mit den angegebenen Kriterien. Alternativ können Sie die Suche mit `<F3>` starten.

#### Suche Aufträge – Positions-Schlüssel
*(Screenshot des "Suche Aufträge" Dialogs, Register "Positions-Schlüssel")*

In diesem Register suchen Sie Aufträge anhand der Positionsdaten. Sie können zusätzliche Suchkriterien in den Registern **Vorgangs-Schlüssel** und **Direkte Suche** angeben.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Felder im Positions-Schlüssel**
- **Artikel**: Artikelnummer. Die Suche wird auf alle Aufträge beschränkt, die diesen Artikel als Positionsartikel beinhalten. Wenn Sie eine Nummer angeben, wird die Artikelbezeichnung im Klartext angezeigt. Die Stücklisten der Positionen werden nicht geprüft.
  *Technische Info: numerisches Feld, DB-Feld: `kpos.artnr`*
- **Kundenprodukt**: Referenznummer für kundenspezifische Produkte aus den Stammdaten. Die Suche wird auf alle Aufträge mit Artikeln dieser kundenspezifischen Nummer beschränkt.
  *Technische Info: alphanumerisches Feld, DB-Feld: `kpos.kuposnr`*
- **Breite, Höhe**: Breite und Höhe der Position in Millimeter. Die Suche wird auf alle Aufträge mit Artikeln dieser Maße beschränkt.
  *Technische Info: numerische Felder, DB-Felder: `kpos.laenge`, `kpos.breite`*
- **Kommission**: Kommissionstext. Die Suche wird auf alle Aufträge beschränkt, die den angegebenen Kommissionstext enthalten.
  *Technische Info: alphanumerisches Feld, DB-Feld: `komm.kommtxt`*
- **Mengeneinheit**: Mengeneinheit der Position, z. B. Quadratmeter. Die Suche wird auf alle Aufträge mit dieser Mengeneinheit beschränkt.
  *Technische Info: numerisches Feld, DB-Feld: `kpos.me`*
- **Maßvariante**: Maßvariante des Artikels. Die Suche wird auf alle Aufträge mit diesen Variantenartikeln beschränkt.
  *Technische Info: numerisches Feld, DB-Feld: `kpos.var`*

#### Suche Aufträge – Direkte Suche
*(Screenshot des "Suche Aufträge" Dialogs, Register "Direkte Suche")*

In diesem Register suchen Sie Aufträge ab einer bestimmten Auftragsnummer. Sie können zusätzliche Suchkriterien in den Registern **Vorgangs-Schlüssel** und **Positions-Schlüssel** angeben.
Wenn die Suchfunktion auf die direkte Suche nach Auftragsnummern beschränkt werden soll, dann kann der Dialog so konfiguriert werden, dass die Register **Vorgangs-Schlüssel** und **Positions-Schlüssel** deaktiviert sind.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Feld in Direkte Suche**
- **Aufträge ab**: Startnummer, ab der aufsteigend nach Aufträgen gesucht wird. Die Suche wird auf alle Aufträge beschränkt, deren Nummern gleich oder größer der angegebenen Auftragsnummer ist.
  *Technische Info: numerisches Feld, DB-Feld: `kauf.auftrnr`*

#### Suche Aufträge – Trefferliste
Nach dem Starten der Suche (`<F3>`) werden die Ergebnisse in der Trefferliste angezeigt. In der Trefferliste finden Sie folgende Register:
- "Suche Aufträge - Lieferinfos" auf Seite D-1083
- "Suche Aufträge – Verschiedenes" auf Seite D-1085
- "Suche Aufträge – Mengen" auf Seite D-1086
- "Suche Aufträge – Eigenschaften" auf Seite D-1088
- "Suche Aufträge - Kommission" auf Seite D-1089

#### Register: Lieferinfos
*(Screenshot des "Suche Aufträge" Dialogs, Trefferliste mit Register "Lieferinfos")*

In diesem Register werden die Lieferinformationen und weitere Details zu den Aufträgen angezeigt, die den Suchkriterien entsprechen. Mit `<F2>` wechseln Sie die Register in der Trefferliste.

- **Kopfbereich**: Die Felder im Kopfbereich sind zum Dialog Suche Aufträge beschrieben: ⇨ "Suche Aufträge" auf Seite D-1077
- **Satzanzeige für die Vorgangsübersicht**: Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Vorgangsübersicht: Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der Treffer`.

**Spalten in Lieferinfos**
- **Haus**: Mandantennummer (Hausnummer).
- **Auftrag**: Auftragsnummer. Der Spaltenname und die Nummer variieren je nach Vorgang, aus dem Sie die Suche öffnen.
- **Subnr.**: Nummer des Teillieferscheins oder der Teilrechnung.
- **Lieferdatum**: Geplanter Liefertermin.
- **Kunde**: Kundenname.
- **Objekt**: Objektnummer bei Aufträgen, denen ein Objekt zugeordnet ist.
- **Rechnung**: Rechnungsnummer bei fakturierten Aufträgen.
- **Org. Vorgang**: Original-Vorgangsnummer bei übertragenen Vorgängen.
- **Storniert**: Angabe des Bearbeitungsstands, z. B. Stornostatus.
  - `0`: Nicht stornierter Auftrag.
  - `1`: Vom Benutzer stornierter Auftrag.
  - `2`: Vom System stornierter Auftrag.
  - `-3, -10, ..., -x`: Auftrag in Hintergrundbearbeitung.

#### Register: Verschiedenes
*(Screenshot des "Suche Aufträge" Dialogs, Trefferliste mit Register "Verschiedenes")*

In diesem Register werden diverse Informationen zu den Aufträgen angezeigt. Mit `<F2>` wechseln Sie die Register. Die Spalten **Haus, Auftrag, Subnr** sind beim Register Lieferinfos beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **Erfassung**: Datum der Auftragserfassung.
- **Erfasser**: Name des Sachbearbeiters.
- **Rechnung**: Rechnungsnummer.
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Kunden.
- **Referenz**: Vorgangsnummer, auf die bei der Vorgangserfassung Bezug genommen wurde.
- **Storniert**: Status der Stornierung.

#### Register: Mengen
*(Screenshot des "Suche Aufträge" Dialogs, Trefferliste mit Register "Mengen")*

In diesem Register werden die Positionsinformationen zu den Aufträgen angezeigt. Pro Auftragsposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register. Die Spalten **Haus, Auftrag, Subnr, Storniert** sind beim Register Lieferinfos beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **Pos**: Positionsnummer im Auftrag.
- **Artnr, Artikel**: Artikelnummer und Artikelbezeichnung des Kopfartikels.
- **Menge**: Positionsmenge.
- **Gelief.**: Bereits gelieferte Positionsmenge.
- **Kompl.***: Ein Stern `*` zeigt an, wenn die Position komplett geliefert ist.
- **Fakt.**: Fakturierte Positionsmenge.
- **Kompl.** `F`: Ein `F` zeigt an, wenn die Position komplett fakturiert ist.

#### Register: Eigenschaften
*(Screenshot des "Suche Aufträge" Dialogs, Trefferliste mit Register "Eigenschaften")*

In diesem Register werden zusätzliche Positionsinformationen aus Aufträgen angezeigt. Pro Auftragsposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register. Die Spalten **Haus, Auftrag, Subnr, Pos, Artnr** sind bei den Registern Lieferinfos und Mengen beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **ME**: Mengeneinheit der Position, z. B. Quadratmeter.
- **qm**: Glasfläche des Artikels pro Stück in Quadratmeter.
- **lfm**: Längenangabe für den Artikels pro Stück in Umlaufenden Meter.
- **Gewicht**: Gewicht der Position in Kilogramm.
- **Breite, Höhe**: Maße des Artikels in Millimeter.
- **Maßvariante**: Maßvariante des Artikels.

#### Register: Kommission
*(Screenshot des "Suche Aufträge" Dialogs, Trefferliste mit Register "Kommission")*

In diesem Register werden Informationen zu Kommissionen der Aufträge angezeigt. Pro Auftragsposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register. Die Spalten sind bei den Registern Lieferinfos und Mengen beschrieben. Zusätzlich wird folgende Spalte angezeigt:
- **Kommission**: Kommissionstext.

### Marktpartnersuche
**Pfad:** `Verkauf > Auftragserfassung > Feld Kunde > <F9>`

In diesem Dialog suchen Sie nach Marktpartnern. Die Suchkriterien geben Sie im Kopfbereich an. Wenn Sie die Marktpartnersuche öffnen, werden Ihnen alle Marktpartner in der Trefferliste angezeigt, die in den Stammdaten hinterlegt und nicht stillgelegt sind. Bei interner Mandantentrennung werden nur die Marktpartner aufgelistet, die dem Haus zugeordnet sind. Über die Filterkriterien können Sie die Trefferliste beschränken.

Es ist konfigurierbar, in welchem Suchkriterienfeld Sie sich für die Eingabe zuerst befinden, wenn sie den Dialog öffnen. Konfigurierbar als erste Eingabefelder sind die Felder **Ab Nummer, Matchcode, Name, Vorname, Land, PLZ** und **Ort**.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

In der Trefferliste werden die Adressen und Informationen zur Identifikation der Marktpartner angezeigt:
- "Register Adresse" auf Seite D-1093
- "Register Identifikation" auf Seite D-1094

**Voreinstellung des Marktpartnertypen**
Je nachdem über welchen Menüpfad Sie den Dialog öffnen, ist der Marktpartnertyp, nach dem gesucht wird, bereits voreingestellt, z. B. Kunde oder Lieferant. Die Trefferliste wird dann entsprechend vorgefiltert. Die Auswahl des Marktpartnertypen ist nur bei der Suche in den Stammdaten möglich.

**Suchfelder**
- **Ab Nummer**: Startnummer, ab der aufsteigend nach Marktpartnern gesucht wird.
- **Matchcode**: Alphanumerischer Matchcode des Marktpartners.
- **Typ**: Anzeige des Marktpartnertyps.
- **Name, Vorname**: Name und Vorname des Marktpartners.
- **Straße**: Straßenname und Hausnummer.
- **Haus**: Mandantennummer (Hausnummer) bei interner Mandantentrennung.
- **Land**: Internationales Länderkennzeichen.
- **PLZ, Ort**: Postleitzahl und Ortsname.
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer.
- **Art**: Marktpartnerstatus. In der Vorgangserfassung werden nur aktive Marktpartner angezeigt.

**Satzanzeige für die Marktpartnerübersicht**
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der angezeigten Treffer in der Liste (Gesamtzahl der Treffer)`.

> **Die Anzeige von Treffern wird satzweise geladen**
> Wenn eine große Menge an Treffern angezeigt werden muss, dann kann das System dafür unter Umständen viel Zeit brauchen. Damit die Trefferliste schnell angezeigt werden kann, wird sie satzweise geladen. Die Satzgröße wird in den Systemeinstellungen konfiguriert. Die Treffer werden in numerischer Reihenfolge geladen, z. B. die numerisch ersten 100 Treffer. Weitere Treffer können mit der Schaltfläche `[Weitere Daten]` geladen werden.

**Register Adresse**
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Nummer**: Marktpartnernummer.
- **Zusatz**: Ergänzende Anmerkung, z. B. ein Adresszusatz.

**Register Identifikation**
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Nummer**: Marktpartnernummer.
- **Still**: Anzeige, ob der Marktpartner stillgelegt ist. (`J`: stillgelegt, `N`: aktiv).
- **Typ**: Typ des Marktpartners, z. B. Kunde, Lieferant.
- **Firma**: Nummer der Firma des Marktpartners bei interner Mandantentrennung.

**Erläuterung der Schaltflächen im Fußbereich**
- `[OK]`: Übernimmt den markierten Marktpartner.
- `[Abbrechen]`: Bricht den Vorgang ab.
- `[<]` und `[>]`: Wechseln zum ersten oder letzten Eintrag.
- `[<<]` und `[>>]`: Zeigen die vorherige oder nächste Seite an.
- `[Refresh]`: Aktualisiert die Suche mit korrigierten/zusätzlichen Suchkriterien.
- `[Weitere Daten]`: Zeigt weitere Treffer an.
- `[Neue Suche]`: Löscht alle Suchkriterien für eine neue Suche (`<Strg>` + `<R>`).

### Mitarbeiter/Berechtigungsgruppen
**Pfad:** `Verkauf > Auftragserfassung > Register Eigenschaften > Feld Sachbearbeiter > <F9>`

In diesem Dialog suchen Sie nach Mitarbeitern. Die Suchkriterien geben Sie im Kopfbereich an. Wenn Sie die Mitarbeitersuche öffnen, werden Ihnen alle Mitarbeiter in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.
- Mit `<F3>` starten Sie die Suche.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.
- "Trefferliste" auf Seite D-1096

**Suchfelder**
- **Ab Nummer**: Startnummer, ab der aufsteigend nach Mitarbeitern gesucht wird.
- **Typ**: Anzeige des Mitarbeitertyps. Ist in den Mitarbeiterstammdaten hinterlegt.
- **Name, Vorname**: Name und Vorname des Mitarbeiters.
- **Abteilung**: Nummer und Bezeichnung der Abteilung.
- **Login**: Benutzername des Mitarbeiters zur Anmeldung bei A+W Enterprise.

**Trefferliste**
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich wird folgende Spalte angezeigt:
- **Nummer**: Mitarbeiternummer.

Der Fußbereich ist ausführlich zur Marktpartnersuche beschrieben: ⇨ "Marktpartnersuche" auf Seite D-1091

### Suche Bezugsvorgang
**Pfad:** `Verkauf > Auftragserfassung > Feld Bezug > <F9>`

In diesem Dialog suchen Sie nach Vorgängen, auf die Sie in der Vorgangserfassung Bezug nehmen können. Die Ergebnisse der Suche werden in der Trefferliste angezeigt.
Der Dialog ist wie der Dialog **Suche Aufträge** aufgebaut: ⇨ "Suche Aufträge" auf Seite D-1077

**Register Vorgangs-Schlüssel**
Die meisten Felder sind zum Register Vorgangs-Schlüssel zur Auftragssuche beschrieben. Zusätzlich werden folgende Felder angezeigt:
- **Vorgang**: Vorgangsart (Angebot, Auftrag, Lieferantenanfrage, Bestellung).
  *Standard-Voreinstellung der Vorgangsart*: Die Vorgangsart ist benutzerindividuell voreingestellt, z. B. Angebot.
- **Vorgangsnummer**: Nummer und Subnummer des Bezugsvorgangs.
- **Geplant**: Geplantes Lieferdatum des Bezugsvorgangs im Format TT.MM.JJJJ.

**Register Positions-Schlüssel, Direkte Suche, Trefferliste, Fußbereich**
Diese sind analog zur Auftragssuche beschrieben.

### Adressen Suche
**Pfad:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Adressen > Lieferadresse suchen`

In diesem Dialog suchen Sie nach Adressen des Marktpartners. Die Suchkriterien geben Sie im Kopfbereich an. Wenn Sie die Adressen-Suche öffnen, werden Ihnen alle Adressen des Marktpartners in der Trefferliste angezeigt.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.
- "Register Adresse, Register Kontaktdaten" auf Seite D-1100

**Suchfelder**
- **Name**: Kundenname.
- **Strasse**: Straßenname und Hausnummer.
- **PLZ, Ort**: Postleitzahl und Ortsname.
- **Land**: Ländername des Lieferziels.
- **Adressencode**: Code der gespeicherten Adresse.
- **Tel, E-Mail**: Telefonnummer, E-Mail-Adresse.
- **Incl. Schnellerfassung**: Angabe, ob Adressen aus der Schnellerfassung aufgelistet werden.
  - ☑ Die Adressen aus der Schnellerfassung werden in der Trefferliste angezeigt.
  - ☐ Aus der Schnellerfassung werden keine Adressen in der Trefferliste angezeigt.
  ⇨ "Schnellerfassung" auf Seite D-1131

**Hauptlieferadresse**
Die Hauptlieferadresse des Marktpartners wird rechts, über den Registern, angezeigt. Wenn dem Marktpartner keine Hauptlieferadresse zugewiesen ist, wird keine Hauptadresse angezeigt.

**Register Adresse, Register Kontaktdaten**
Die Spalten auf Positionsebene entsprechen den Feldern im Kopfbereich. Zusätzlich wird folgende Spalte angezeigt:
- **Vorname**: Vorname des Kunden.

