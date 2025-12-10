---
description: "DE-AWBusiness-BarcodeManagerEL"
---


# A+W Barcode Manager (EL)

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Version/Datum | Beschreibung |
| :--- | :--- |
| 1.00/03-2023 | Ersterstellung, Überführung aus docx-Dokument |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

**Anmerkungen zu diesem Dokument**
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

**Urheberrechte**
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

**Warenzeichen**
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind zu beachten.

### Kontakte
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim

- **Tel:** +49 6404 2051-0
- **Fax:** +49 6404 2051-877
- **E-Mail:** zentrale@a-w.com
- **Web:** http://www.a-w.com

## Einleitung
Die Online - Betriebsdatenerfassung mittels Barcode-Scanner erfolgt mittels eines Windows-CE basierten Scanner der Firma Datalogic (Scorpio). Das eigentliche Programm läuft dabei auf einem Terminal-Server, an den sich der Scanner via Remote-Desktop verbindet. Alle Lesungen die am Scanner vorgenommen werden, sendet der Scanner als Tastatureingabe in das jeweils aktive Datenfeld.

Damit das Programm für die BDE nach der Anmeldung des Scanners am Terminal-Server automatisch startet, ist es erforderlich eine Verknüpfung zum BDE-Programm für den Benutzer in die Autostart-Gruppe zu kopieren. Das zu verknüpfende Programm hat den Namen abcscanner.exe und befindet sich im A+W Business Programme Ordner (z.B. C:\Program Files\A+W\ALFAK 2011\Program\German). Bevor das Programm gestartet wird muss auf dem Rechner das A+W Business Startprogramm einmalig ausgeführt werden und es muss die richtige Datenbankverbindung im Login-Dialog eingegeben werden. Das BDE-Programm verbindet sich ab diesem Moment immer mit den gerade eingegebenen Informationen an die Datenbank.

Das automatische Starten des Programmes kann ab A+W Business 5.5 Update 3 durch ein Konfigurationsprogramm (A+W Business 5 Scanner Auto-Start Config) im Startmenu ConfigTools eingestellt werden. In diesem Programm kann für den aktuelle angemeldeten Benutzer das Scannerprogramm (sprachabhängig) ausgewählt werden, das beim Anmelden dieses Benutzers gestartet werden soll.

## Einstellungen

### Scanner
Die Konfiguration des Scanners kann auf einem beliebigen Arbeitsplatz durchgeführt werden. Zuerst wird die dem Scanner beiliegende Konfigurations-Software auf einem PC installiert und anschließend wird der Scanner per USB verbunden. Dann wird die Konfigurations-Software gestartet (Datalogic Configuration Utility). In dem Programm wird zunächst die Einstellung Postamble im Menü Hw Configuration > Laser > Parameters > Reader Parameters > Text Formatting vorgenommen. Hier wird einfach ein Tabulator eingegeben. Die Eingabe des Tabulators kann auf zwei Arten erfolgen. Entweder man gibt ein Tabulator in einem Editor (z.B. Notepad oder Word) ein und kopiert diesen über die Zwischenablage in das Datenfeld. Oder man drückt die Taste ALT, hält sie gedrückt währen man auf dem Nummernblock die Ziffern 0 0 9 nacheinander eingibt und die ALT Taste wieder los lässt.

Dadurch wird am Ende einer jeden Lesung ein [TAB] an das BDE-Programm gesendet um eine vollständige Lesung des Barcodes zu signalisieren.

**Abb. A-1: Vollständigkeit der Barcode-Lesung**
*(Screenshot der Datalogic Configuration Utility. Die Einstellung `Postamble` unter `Hw Configuration > Laser > Parameters > Reader Parameters > Text Formatting` ist ausgewählt. Im `Postamble` Feld ist ein Tabulator-Zeichen eingefügt, um das Ende einer Barcode-Lesung zu signalisieren.)*

Die zweite und letzte Einstellung lautet CheckEvaluation im Menü Hw Configuration > Laser > Parameters > Reader Parameters > Code39 > Standard. Diese Einstellung muss auf Enabled gesetzt werden, damit die Prüfziffern des Code39 Barcodes überprüft und nicht als gültige Daten an das Programm gesendet werden.

**Abb. A-2: Code 39 Einstellung**
*(Screenshot der Datalogic Configuration Utility. Die Einstellung `CheckEvaluation` unter `Hw Configuration > Laser > Parameters > Reader Parameters > Code39 > Standard` ist auf `Enabled` gesetzt.)*

### Erfassungsstellen in A+W Business
**Pfad:** Fertigung > Erfassungsstellen Produktion

In diesem Dialog hinterlegen Sie BDE-Typ der jeweilige Typ der Erfassungsstelle. Diese werden für den Wareneingang und die Fertigmeldung benötigt. Ist beispielsweise eine eindeutige Zuordnung von Erfassungsstelle zu BDE-Typ gemacht (in der obigen Abbildung z.B. für den Wareneingang) so ist es nicht mehr nötig die Erfassungsstelle am Scanner einzulesen, wenn man den entsprechenden Programmpunkt wählt.

**Abb. A-3: Erfassungsstellen Produktion**
*(Screenshot des Fensters "Erfassungsstellen Produktion" in A+W Business. Es zeigt eine Liste von Erfassungsstellen mit Details wie Barcode-ID, Bezeichnung, Statuspunkt und BDE-Typ. Die Zeile für "Wareneingang" ist hervorgehoben.)*

### Mitarbeiterverwaltung in A+W Business
In der Mitarbeiterverwaltung ist es erforderlich für diejenigen Mitarbeiter die Personalnummer einzugeben, die sich per Mitarbeiter-Barcode an dem Scanner anmelden sollen.

**Abb. A-4: Mitarbeiterverwaltung - Einstellung**
*(Screenshot des Mitarbeiter-Verwaltungsfensters in A+W Business. Das Feld "Personalbarcode" ist hervorgehoben und zeigt, wo die Barcode-Nummer für einen Mitarbeiter eingetragen wird.)*

### Interface Service
Um Fertigmeldungen per Scanner zu buchen, werden die gelesenen Fertigmeldungen in der Datenbank gepuffert und anschließend vom AIS verarbeitet. Damit der AIS die gelesenen Buchungen zuordnen kann, ist es wichtig den Instanz-Namen des AIS als „sysadm“ zu definieren.
Das ist auch der Default nach der Installation. Wenn bei einer Installation mehr als eine Instanz des AIS zum Einsatz kommt ist es wichtig diese Einstellung zu prüfen.

### Kapazitätsplanung
**Pfad:** Kapazitätsplanung > Stammdaten > Organisation > Aggregate

Soll die Verbuchung der Fertigmeldungen mit der A+W Business Kapazitätsplanung erfolgen, so ist es nötig für das jeweilige Aggregat eine eindeutige Erfassungsstelle einzutragen. Das geschieht in der Aggregat-Verwaltung unter Kapazitätsplanung > Stammdaten > Organisation > Aggregate. Die jeweils zu verwendende Arbeitsart wird dabei immer über den Barcode eingelesen.

**Abb. A-5: Aggregat-Zuordnung für Erfassungsstelle**
*(Screenshot des Fensters "Aggregate" in A+W Business. Das Feld "Erfassungsstelle" ist hervorgehoben und zeigt die Zuordnung einer Erfassungsstelle zu einem Aggregat, z.B. "1000 - Zuschnitt 1".)*

## Funktionen
Im Folgenden sind die einzelnen Dialoge der BDE aufgeführt und deren Funktionsweise erläutert:
- "Anmeldung" auf Seite A-15
- "Hauptmenü" auf Seite A-16
- "Wareneingang" auf Seite A-17
- "Produktionsmeldung" auf Seite A-18
- "Lagerbewegungen" auf Seite A-21
- "Gestelle" auf Seite A-32
- "Sonstiges" auf Seite A-37

### Anmeldung
**Scanner-Start**

Nach erfolgreicher Anmeldung eines Anwenders gelangt man direkt in das Hauptmenü. Von hier aus gelangt man in den jeweiligen Dialog um Wareneingänge, Lagerbuchungen, Gestell-Belegungen oder Fertigmeldungen durchzuführen.

**Abb. A-6: BDE - Anmeldung über Personalbarcode39 Einstellung**
*(Screenshot des Scanner-Displays mit dem Titel "Register Employee". Es zeigt ein Eingabefeld für "Staff Barcode".)*

### Hauptmenü
**Pfad:** Scanner > Hauptmenü

Über die Hauptmenü des Scanners erreichen Sie folgende Funktionen:
- "Wareneingang" auf Seite A-17
- "Produktionsmeldung" auf Seite A-18
- "Lagerbewegungen" auf Seite A-21
- "Gestelle" auf Seite A-32
- "Sonstiges" auf Seite A-37

Mit der Option [Back/ Zurück] kehren Sie zu vorherigem Dialog.

**Abb. A-7: BDE - Hauptmenü**
*(Screenshot des Scanner-Hauptmenüs mit den Optionen: Receipt of Goods, Production message, Stock Movement, Racks, Special functions, Back.)*

### Wareneingang
**Pfad:** Scanner > Hauptmenü > Wareneingang

Hier werden die Barcodes der Bestellpositionen eingelesen, für die ein Wareneingang verbucht werden soll.

Nachdem der Barcode mit der Bestellposition gelesen wurde wird die Eingangsmenge per Tastatur eingegeben. Standardmäßig zeigt das Programm hier die komplette Menge der Bestellposition an und muss nur bei einer abweichenden Menge geändert werden. Sollte keine Änderung nötig sein, wird mit dem Barcode der nächsten Bestellposition fortgefahren. Das Programm sammelt diese Lesungen zunächst ohne eine tatsächliche Buchung durchzuführen. Das passiert erst, wenn man auf dem Scanner die ENTER-Taste getätigt, oder den Barcode einer anderen Bestellung einliest. Wird der ZURÜCK-Button oder die ESC-Taste betätigt und es sind noch nicht verbuchte Bestellpositionen im Speicher, so fragt das Programm nach, ob diese jetzt verbucht werden sollen.

Wenn es sich bei der gerade eingelesenen Bestellposition um eine Kiste handelt, so kann direkt danach ein Kisten-Identnummern-Barcode eingelesen werden und ggf. der Inhalt der Kiste geändert werden. Es wird dann automatisch nur eine Menge von 1 Stück eingetragen und diese ist auch nicht mehr änderbar. Für Kisten mit Identnummern kann ein abweichender Inhalt eingegeben werden.

Nach jeder Lesung einer Bestellposition wird in dem unteren Mengen-Feld angezeigt wie viel Artikel bestellt wurden und wie viele bereits geliefert wurden.

**Abb. A-8: BDE - Wareneingang**
*(Screenshot des Scanner-Displays für "Goods Receipt". Es zeigt Felder für "Purchase Order / Item / Ident-number", "Received", "Diff. Case Contents" und "Quantities".)*

### Produktionsmeldung
**Pfad:** Scanner > Hauptmenü > Produktionsmeldung

Die Fertig- und Bruchmeldungen befinden sich im Untermenü Produktionsmeldung, welches im Hauptmenü des Scanners die bisherige Fertigmeldung ersetzt.
- "Fertigmeldung" auf Seite A-19
- "Bruchmeldung" auf Seite A-20

**Abb. A-9: BDE - Produktionsmeldung**
*(Screenshot des Scanner-Untermenüs "Production messages" mit den Optionen "Completion report" und "Breakage report".)*

#### Fertigmeldung
**Pfad:** Scanner > Hauptmenü > Produktionsmeldung > Fertigmeldung Report

Über den Dialog der Fertigmeldung lassen sich Statusänderungen an Auftragspositionen durchführen. Alle Lesungen die hier durchgeführt werden, werden zunächst in der Datenbank gespeichert und durch den AIS als STSD-Rückmeldung verarbeitet. Statusänderungen an den Aufträgen werden daher Zeit versetzt ausgeführt. Näheres zur Konfiguration des AIS für STSD-Rückmeldungen sind dem vorherigen Kapitel zu entnehmen.

Nachdem eine Auftragsposition gelesen wurde, wird die Menge eingetragen, die fertig gemeldet werden soll. Das Programm blendet hier immer die komplette Positionsmenge vor. Zum Speichern der Fertigmeldung ist die ENTER-Taste zu drücken. Der Datensatz wird danach vom AIS verarbeitet und der Status des Auftrages ggf. angepasst. Soll pro Scannung nur ein Stück verarbeitet werden, kann die Option „Menge=1“ gewählt werden. Ist diese Option aktiviert, wird beim Scannen eines Barcodes sofort 1 Stück als fertig eingetragen. Eine zusätzliche Eingabeder Menge oder ein Bestätigen mit Enter ist damit nicht mehr nötig.

Über den Dialog Bruchmeldung lassen sich ebenfalls Statusänderungen an Aufträgen durchführen, im Gegensatz zur Fertigmeldung allerdings nur negative.

**Abb. A-10: BDE - Produktions-Rückmeldung**
*(Screenshot des Scanner-Displays für "Completion Report". Es zeigt Felder für "Order / Item / Part no.", "Report Quantity Completed" und Optionen wie "Amount = 1" und "Entry Amount".)*

#### Bruchmeldung
**Pfad:** Scanner > Hauptmenü > Produktionsmeldung > Bruchmeldung - Report

Bedienung und Verbuchung funktionieren analog zur Fertigmeldung, allerdings ist es möglich, Bruchgrund und -erfasser mit anzugeben. Diese können entweder per Druck auf die Schaltfläche auf dem Scanner oder per Barcode ausgewählt werden. Die Barcodes können in den Programmen Reklamationsgrund und -verursacher über das Formular Etiketten ausgedruckt werden.

Nach der Buchung eines Satzes werden die Informatonen zur letzten Buchung zusammengefasst auf dem Scanner angezeigt.

**Abb. A-11: BDE - Bruchmeldung**
*(Screenshot des Scanner-Displays für den Bruchmelde-Report, das dem Fertigmelde-Report sehr ähnlich ist.)*

### Lagerbewegungen
**Pfad:** Scanner > Hauptmenü > Lagerbewegung

Beim Start der Lagerbuchung wird zuerst gewählt, ob ein Zugang oder ein Abgang von Ware erfolgen soll. Zusätzlich ist das Menü für Kisten von hier erreichbar.
- "Lagerentnahme" auf Seite A-22
- "Lagerzugang" auf Seite A-23
- "Umbuchung" auf Seite A-24
- "Kisten" auf Seite A-26

**Abb. A-12: BDE - Menü Lagerbewegung**
*(Screenshot des Scanner-Menüs "Stock Transfer" mit den Optionen: Withdrawal, Receipt, Transfer, Cases.)*

#### Lagerentnahme
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Entnahme

Der darauf folgende Dialog funktioniert für den Zugang und Abgang größten Teils identisch. Nachdem der Lagerortbarcode gelesen worden ist, kann der Lagerartikelbarcode gelesen werden und die jeweilige Menge für die Zugangs- bzw. Abgangsbuchung eingegeben werden. Durch Betätigung der ENTER-Taste wird die Buchung direkt ausgeführt.

**Abb. A-13: BDE - Lagerentnahme**
*(Screenshot des Scanner-Displays "Taken from Stock". Es zeigt Felder für "Product No. or ID" und "Qty".)*

#### Lagerzugang
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Zugang

**Abb. A-14: BDE - Lagerzugang**
*(Screenshot des Scanner-Displays "Stock receipt". Es zeigt Felder für "Product No. or ID" und "Qty".)*

#### Umbuchung
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Umbuchung

Es gibt nun unter dem Menüpunkt Lagerbewegung die Funktion Umbuchung. Wählt man diesen muss man zunächst einmal einen Lagerort – Barcode scannen.

**Abb. A-15: BDE - Lagerort wählen**
*(Screenshot des Scanner-Displays "Select Stock Location" mit einem Eingabefeld für "Stock Location Barcode".)*

Danach gelangt man in den Dialog zur Umbuchung von Lagerartikeln. Hier muss der Anwender ein Lagerartikel scannen, also eine LagerID eines Lagerartikels, woraufhin der aktuelle Bestand angezeigt wird. Nun sollte man zunächst die Menge, die umgebucht werden soll, definieren.

**Abb. A-16: BDE - Umbuchung Lagerartikel**
*(Screenshot des Scanner-Displays "Transfer". Es zeigt Felder für "Product No. or ID", "New Stock Location", "Qty." und "Last Booking" Informationen.)*

Dann kann der Anwender einen neuen Lagerort vorgeben und die Buchung ausführen. Auf dem Schirm erscheint eine Erfolgsmeldung.

**Abb. A-17: BDE - erfolgreiche Umbuchung**
*(Screenshot des Scanner-Displays "Transfer", das eine Erfolgsmeldung nach einer Umbuchung anzeigt: "Stock product with a quantity of 67 was booked to stock location <k.A.>-<k.A.>-<k.A.>.")*

### Kisten
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Kisten

Ab der A+W Business Version 12.5 steht zusätzlich noch das Untermenü Kisten zur Verfügung. Mit diesem Menü können die folgenden Funktionen aufgerufen werden:
- "Kisteninhalt ändern" auf Seite A-27
- "Auflösen von Kisten" auf Seite A-28
- "Lagerort von Kisten ändern" auf Seite A-29
- "Kiste auf Inventur setzen" auf Seite A-30
- "Warenausgang Kiste" auf Seite A-31

**Abb. A-18: BDE - Kistenlager Menü**
*(Screenshot des Scanner-Menüs "Cases" mit den Optionen: Change Content, Resolve, Change Stock Location, On Inventory List, Shipment Cases.)*

#### Kisteninhalt ändern
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Kisten > Inhalt ändern

Mit dieser Funktion kann die Blattanzahl in einer Kiste reduziert werden. Dazu wird erst ein Kistenbarcode gescannt und danach die angezeigte Menge auf den neuen Wert gesetzt. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

**Abb. A-19: BDE - Kisteninhalt ändern**
*(Screenshot des Scanner-Displays "Change Content". Es zeigt Felder für "Case" und "New Case Content".)*

#### Auflösen von Kisten
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Kisten > Auflösen

Mit dieser Funktion kann eine Kiste aufgelöst werden (d.h. die Kiste wird gelöscht und die verbleibenden Scheiben werden auf das Lager gebucht). Hierzu wird erst eine Kiste gescannt und danach kann der Inhalt noch editiert werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

**Abb. A-20: BDE - Kistenlager Menü**
*(Screenshot des Scanner-Displays "Resolve complete Case". Es zeigt Felder für "Case" und "Diff. Case Contents".)*

#### Lagerort von Kisten ändern
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Kisten > Lagerort ändern

Mit dieser Funktion kann der Lagerort einer Kiste verändert werden. Dazu wird erst eine Kiste gescannt und danach der Barcode des neuen Lagerortes. Die Buchung wird dann sofort ausgelöst.

**Abb. A-21: BDE - Kistenlager Menü**
*(Screenshot des Scanner-Displays "Rebook case". Es zeigt Felder für "Case" und "New Stock Location".)*

#### Kiste auf Inventur setzen
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Kisten > Zu Inventur Liste

Mit dieser Funktion wird eine Kiste auf die aktuelle Inventurliste gesetzt. Nachdem die Kiste gescannt wurde kann der neue Lagerort gescannt werden. Nachdem beide Scannungen durchgeführt wurden, kann die aktuelle Menge der Scheiben in der Kiste noch editiert werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

**Abb. A-22: BDE - Kisten auf Inventur setzen**
*(Screenshot des Scanner-Displays "Case On Inventory List". Es zeigt Felder für "Case", "Storage Place", und "Diff. Case Contents".)*

#### Warenausgang Kiste
**Pfad:** Scanner > Hauptmenü > Lagerbewegung > Kisten > Warenausgang Kiste

Mit dieser Funktion können Kisten mit Identnummer einer Auftragsposition zugeordnet werden. Zunächst muss ein Auftragspositions-Barcode gescannt werden. Danach wird per Scannen des Kisten-Barcodes die Blattanzahl der Kiste ermittelt. Dieser kann dementsprechend editiert werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

**Abb. A-23: BDE - Kisten Warenausgang**
*(Screenshot des Scanner-Displays "Shipment Cases". Es zeigt Felder für "Order / Item", "Case", und "Case Content".)*

### Gestelle
Damit Gestelle verarbeitet werden können, müssen die folgenden Bedingungen vorher geprüft werden:
- Gestellnummern müssen eindeutig sein. Es darf also nicht ein Gestell mit der gleichen Nummer aber unterschiedlicher Gestellart angelegt werden. Wenn die gleiche Nummer verwendet wird, sollte der Gestellnummer ein Buchstabe (Für die Gestellart) vorangestellt werden.
- Beim Verbuchen von Gestellen wird die Breite und Höhe des Gestells und das Beladungsgewicht geprüft. Diese Werte können pro Gestellart eingestellt werden.
- Die Verbuchung von Gestellen ist für den Versand entwickelt worden, d.h. es können nur Hauptpositionen einem Gestell hinzugefügt werden.
- Es können nur Gestelle beladen werden, die nicht außer Haus gebucht sind, nicht als verloren gemeldet und nicht gesperrt sind.
- Mit Punkt 5 ist sichergestellt, das beim Gestellausgang die Zuordnung des Gestells vollständig gebucht sein sollte.

#### Übersicht über Gestellmenü
**Pfad:** Scanner > Hauptmenü > Gestelle

Im Untermenü Gestelle sind folgende Funktionen verfügbar:
- "Gestelle beladen" auf Seite A-33
- "Gestelle leeren" auf Seite A-35
- "Gestelle anzeigen" auf Seite A-36

**Abb. A-24: BDE - Menü Gestelle**
*(Screenshot des Scanner-Menüs "Gestelle" mit den Optionen: Beladen, Leeren, Anzeigen.)*

#### Gestelle beladen
**Pfad:** Scanner > Hauptmenü > Gestelle > Beladen

Zum Beladen von Gestellen muss zuerst das Gestell ausgewählt werden, das beladen werden soll. Ab dem Scannen des Gestellbarcode, können dann im darauf folgenden Dialog Auftragspositionen dem Gestell hinzugefügt werden.

**Abb. A-25: BDE - Gestelle Beladen**
*(Screenshot des Scanner-Displays "Gestell wählen" mit einem Eingabefeld für "Gestellbarcode".)*

**Abb. A-26: BDE - Gestelle Beladen - Auftragspositionen**
*(Screenshot des Scanner-Displays "Gestell 4717 beladen". Es zeigt Felder für "Auftrag/Position", "Menge" und Optionen wie "Menge = 1" und "Eingabe Menge".)*

Nach der erfolgreichen Auswahl eines Gestells kann man Auftragspositionen dem Gestell hinzufügen. Hierbei werden zwei unterschiedliche Modi unterstützt, die mit den Knöpfen „Menge = 1“ und „Eingabe Menge" ausgewählt werden können. Der aktuell eingestellte Modus ist grün markiert.

Für das Hinzufügen von Auftragspositionen muss der T2 Barcode verwendet werden.

Im Modus „Eingabe Menge" wird nach dem der Positionsbarcode gescannt wurde, die noch nicht auf Gestellen abgestellte Menge im Mengenfeld des Dialoges angezeigt. Diese kann dann editiert werden, wenn eine kleinere Anzahl abgestellt werden soll. Durch ein Drücken der Enter Taste auf dem Scanner wird die Buchung gestätigt.

Im Modus „Menge = 1" wird die Verbuchung sofort nach dem Scannen des Auftragspositionsbarcodes ausgeführt. Hierbei wird immer nur 1 Stück verbucht.

Das Ergebnis der letzten Buchung wird immer im Fenster „Letzte Buchung“ angezeigt.

Um das Gestell zu wechseln, kann der Zurück Knopf getätigt werden und dann ein anderes Gestell ausgewählt werden.

#### Gestelle leeren
**Pfad:** Scanner > Hauptmenü > Gestelle > Leeren

Mit diesem Dialog kann ein Gestell als leer gemeldet werden. Dabei werden alle Zuordnungen der vorher auf dem Gestell abgestellten Auftragspositionen gelöscht.

> **Keine Sicherungsabfrage**
> Beim Leeren eines Gestells erfolgt keine Bestätigungsabfrage!

**Abb. A-27: BDE - Gestelle Leeren**
*(Screenshot des Scanner-Displays "Gestell leeren" mit einem Feld für "Gestell" und einem Anzeigebereich für "Letzte Buchung".)*

#### Gestelle anzeigen
**Pfad:** Scanner > Hauptmenü > Gestelle > Anzeigen

Mit diesem Dialog kann die aktuelle Zuordnung von Auftragspositionen auf einem Gestell angezeigt werden. Wird ein Gestellbarcode gescannt, werden im Belegungsfenster die Auftragspositionen mit der jeweils abgestellten Menge angezeigt. Zusätzlich wird noch die Kundennummer mit ausgegeben. Die Liste enthält jeweils sechs Einträge. Mit dem Vor und Zurück Knopf kann diese geblättert werden.

**Abb. A-28: BDE - Gestelle anzeigen**
*(Screenshot des Scanner-Displays "Gestellbelegung für Gestell 123". Es zeigt eine Tabelle mit den Spalten "Auftrag", "Pos.", "Menge", "Kunde".)*

### Sonstiges
**Pfad:** Scanner > Hauptmenü > Sonstiges

Über den Menüpunkt Sonstiges erreicht man die Dialoge für die Auftragspositionsinfo, die Anmeldeinfo und den Dialog zum Wechseln des Mitarbeiters:
- "Auftragsinformation" auf Seite A-37
- "Anmeldeinformation" auf Seite A-38
- "Mitarbeiterwechsel" auf Seite A-38

#### Auftragsinformation
**Pfad:** Scanner > Hauptmenü > Sonstiges > Auftragsinformation

Die Auftragspositionsinfo zeigt nach der Lesung eines Auftragspositions-Barcodes die Bezeichnung der Position, deren Abmessung, die Stückzahl, die gelieferte Menge den Preis pro Preiseinheit und das Lieferdatum an.

**Abb. A-29: BDE - Auftragsinformation**
*(Screenshot des Scanner-Displays "Order Item Info". Nach dem Scannen eines Barcodes werden Details wie Description, Dim., Qty., Delivered, Price, und Delivery angezeigt.)*

#### Anmeldeinformation
**Pfad:** Scanner > Hauptmenü > Sonstiges > Anmeldeinformation

Der Dialog für die Anmeldeinformationen zeigt den aktuell angemeldeten Benutzer, die Datenbank, das Datenbanksystem (Microsoft SQL Server oder Unify SQL Base), die Erfassungsstelle, das Aggregat und die Arbeitsart an.

**Abb. A-30: BDE - Sonstiges**
*(Screenshot des Scanner-Displays "Registration Information", das Details zum angemeldeten Benutzer, Server, Datenbank etc. anzeigt.)*

#### Mitarbeiterwechsel
**Pfad:** Scanner > Hauptmenü > Sonstiges > Mitarbeiterwechsel

Der Dialog zum Mitarbeiterwechsel ist im folgenden Abschnitt beschrieben:
- "Anmeldung" auf Seite A-15

Nach der Lesung eines gültigen Mitarbeiterbarcodes wird der aktuelle Mitarbeiter abgemeldet und der neue Mitarbeiter angemeldet.

**Abb. A-31: BDE - Anmelden**
*(Screenshot des Scanner-Displays "Register Employee" mit einem Eingabefeld für "Staff Barcode", verwendet für den Mitarbeiterwechsel.)*

## Barcodes
Für die einzelnen Dialoge und Funktionen sind bestimmte Barcodes erforderlich. Bei den Barcodes handelt es sich um Code39 Barcodes mit Prüfziffer und einem Stern als Anfangs- und Ende-Zeichen.

| Bezeichnung | Präfix | Nutzdaten | Beispiel |
| :--- | :--- | :--- | :--- |
| Personalbarcode | PE | Die Personalnummer aus der Mitarbeiterverwaltung | `*PE000000199F*` |
| Erfassungsstellenbarcode ohne Arbeitsart für Wareneingang | ES | Die ID der Erfassungsstelle | `*ES00000000166*` |
| Erfassungsstellenbarcode mit Arbeitsart für Fertigmeldung | EA | Die ID der Erfassungsstelle und die ID der Arbeitsart getrennt mit Bindestrich | `*EA0000000015-101P*` |
| Auftragsbarcode für Fertigmeldung und Scheiben-Gestell-Zuordnung | T2 | Auftragsnummer + Positionsnummer (3stellig) + Teilenummer (3stellig) | `*T200000243001001%*` |
| Auftragsbarcode für Auftragsinfo | D2 oder T2 | Auftragsnummer + Positionsnummer (3stellig) + Teilenummer (3stellig) (Nur T2) | `*D200000243002Q*` oder `*T200000243002001Q*` |
| Bestellbarcode für Wareneingang | D5 | Bestellnummer + Positionsnummer (3stellig) | `*D50000070650001.*` |
| Kistenbarcode für Lagerabgang und Wareneingang | BO | Identnummer einer Kiste. Achtung Identnummer darf keine führende Null enthalten! | `*BOBC00002H*` |
| Lagerortbarcode für Lagerbuchung | LA | Die ID des Lagerortes | `*LA0000000001W*` oder `*L0000000001W*` |
| Lagerartikel Barcode für Lagerbuchung | LP | Die LagerID des Lagerartikels | `*LP0000000164E*` |
| Gestellnummer | GE | Die Gestellnummer | `*GE9099E*` |
| Reklamationsgrund | BR | Die Nummer des Reklamationsgrundes | `*BR1$*` |
| Reklamationsverursacher | BC | Die Nummer des Reklamationsverursachers | `*BC2P*` |

### Ausdrucken von Barcodes
In den folgenden Programmen im A+W Business wurde eine Barcode-Druckfunktionalität für die Online - Betriebsdatenerfassung (mittels Barcode-Scanner) implementiert:
- Mitarbeiterverwaltung (Stammdaten > Firma > Mitarbeiter)
- Erfassungsstellen Produktion (z.B. Stammdaten > Fertigung > Sonstige > Erfassungsstellen Produktion)
- Vorgabezeiten (Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten)
- Druckprogramm (z. B. Dokumente > Auftrag > Druck Auftrag)
- Lagerdefinition (Stammdaten > Lager > Lagerdefinition)
- Lagerverwaltung (Lagerwirtschaft > Lagerverwaltung)
- Gestelle (Fertigung > Gestellverwaltung > Gestelle)
- Reklamationsgrund (Stammdaten > Produkte > Allgemein > Reklamationsgrund)
- Reklamationsverursacher (Stammdaten > Produkte > Allgemein > Reklamationsverursacher)

Die Barcodes werden, wenn die Nutzdaten nicht die mögliche Datenlänge überschreiten, mit Nullen (0) aufgefüllt (Ausnahme Gestellbarcodes). Des Weiteren erhalten alle Barcodes eine abschließende Prüfziffer. In der Mitarbeiterverwaltung (1) wurde zudem eine allgemeine Druckfunktionalität eingebaut. Die Barcodes enthalten die Personalnummer (hier 199) des Mitarbeiters (Beispiel: PE000000199F). Der Erfassungsstellenbarcode (2) wird aus der ID der Erfassungsstelle gebildet (Beispiel: ES00000000166). In dem Programm Vorgabezeiten (3) hat der Anwender jetzt die Möglichkeit einen Erfassungsstellenbarcode mit Arbeitsart für die Fertigmeldung in der Online - BDE zu drucken. Dieser setzt sich aus der ID der Erfassungsstelle und der ID der Arbeitsart getrennt mit Bindestrich zusammen (Beispiel: EA0000000015-101P). Das Druckprogramm für den Formulardruck (4) kann ab sofort auch einen Auftragsbarcode (Auftragsinfo in Online - BDE) oder einen Bestellbarcode (Wareneingang in Online - BDE) drucken. Dieser Barcode beinhaltet die Dokumentennummer, die 3-stellige Positionsnummer und eine 3 stellige Teilenummer (immer 000, da hier nur Hauptpositionen ausgegeben werden) (Beispiel Auftrag: T200000243002000Q - Beispiel Bestellung: D50000070650001.). Für die Lagerbuchung in der BDE muss entsprechend der Lagerort gescannt werden. Hierfür wurde zum einen der Barcode-Druck in dem Lagerdefinition-Dialog (5) überarbeitet und zum anderen die Online - BDE erweitert. Die Online - BDE kann ab sofort solche Lagerortbarcodes mit einem L-Präfix verarbeiten. Der Barcode beinhaltet die ID des Lagerortes (Beispiel: *L0000000001W*). Abschließend sind für die Lagerbuchung Barcodes der Lagerartikel (5) notwendig. In der Lagerverwaltung können nun die entsprechenden Barcodes, die die ID des Lagerartikels enthalten, gedruckt werden (Beispiel: LP0000000164E). Für Gestelle kann in der Gestellverwaltung (7) eine Liste von Gestellen selektiert werden und dann für diese der Barcode ausgedruckt werden (Funktionen > Gestellbarcodes drucken). Da Gestelle alphanummerisch sind, werden diese nicht mit führenden Nullen aufgefüllt.

Hinweis: Alle Barcodes werden in die Report-Variable F_IDENT_C39 des jeweiligen Formulars/Reports geschrieben.

### Buchungshistorie
Es ist jetzt möglich, sich die getätigten Fertig- und Bruchmeldungen protokollieren zu lassen. Um die Funktionalität zu aktivieren, muss in den Firmenstammdaten auf Register 15.Kapazitätsplanung der Schalter ‚Historientabelle für Fertigmeldungen füllen' aktiviert werden.

Wurde der Schalter aktiviert, werden die verarbeiteten Meldungen in der Tabelle FS_BOOK_HISTORY protokolliert. Ist die Verbuchung in die A+W Business Kapazitätsplanung aktiv, so werden die Meldungen auch bei Verbuchung in selbige protokolliert. Das gilt auch für Meldungen, die per Dialog im A+W Business getätigt werden. Ansonsten werden die Buchungen in die PD_AWBAR protokolliert.

Dabei werden folgende Daten gespeichert:
- Auftragsnummer
- Positionsnummer
- Stücklistenelement
- Zeitpunkt der Scannung
- Mitarbeiter
- Erfassungsstelle
- Arbeitsart (Nur bei Buchung in Kapazitätsplanung, ansonsten 0)
- Bruchgrund (Nur bei Bruchmeldungen)
- Bruchverursacher (Nur bei Bruchmeldungen)
- Verbuchte Menge
- Ursprung (BDE, manuell, implizit)

Außerdem gibt es einen Dialog zur Auswertung der Buchungshistorie (Statistik > Buchugshistorie). Man kann dort per QBE Modus die anzuzeigenden Sätze filtern, so dass man hier genaue Statistiken z. B. pro Mitarbeiter erstellen kann.

**Abb. A-32: Buchungshistorie**
*(Screenshot des Fensters "Buchungshistorie" in A+W Business. Es zeigt Filteroptionen (Datum, Mitarbeiter, etc.) und eine Ergebnisliste der Buchungen mit Details wie Auftrag, Zeit, Mitarbeiter und Menge.)*

Beim Druck kann man sich die angezeigten Sätze dann noch zusätzlich nach zwei dynamischen Kriterien gruppieren lassen, die ebenfalls im Dialog eingestellt werden.

## Index

**A**
- **Aggregate**
  - Kapazitätsplanung: A-14
- **Anmeldung**: A-15

**B**
- **BDE**
  - Anmeldeinformation: A-38
  - Anmeldung: A-15
  - Auftragsinformation: A-37
  - Ausdrucken von Barcodes: A-39, A-40
  - Barcodes: A-39
  - Funktionen: A-15
  - Gestelle: A-32
  - Gestellfunktionen: A-33, A-35, A-36
  - Gestellmenü: A-32
  - Hauptmenü: A-16
  - Lagerbewegungen: A-21
  - Mitarbeiterwechsel: A-38
  - Produktionsmeldung: A-18
  - Sonstige Funktionen: A-37
- **Bruchmeldung**: A-20
- **Buchungshistorie**: A-41

**E**
- **Einstellungen**
  - Scanner: A-10
- **Erfassungsstellen**
  - A+W Business Stammdaten: A-12

**F**
- **Fertigmeldung**: A-19
- **Funktionen**
  - Überblick: A-15

**G**
- **Gestelle**: A-32
  - Anzeigen: A-36
  - Beladen: A-33
  - Leeren: A-35
  - Menüübersicht: A-32

**I**
- **Interface Service**: A-13

**K**
- **Kistenbuchungen**:
  - Inventurliste: A-30
  - Kiste auflösen: A-28
  - Kisteninhalt ändern: A-27
  - Kistenlagerort ändern: A-29
  - Kistenwarenausgang: A-31
- **Kistenverwaltung**: A-26

**L**
- **Lagerbewegungen**: A-21
  - Kiste auf Inventurliste setzen: A-30
  - Kiste auflösen: A-28
  - Kistenbuchungen: A-26
  - Kisteninhalt ändern: A-27
  - Kistenort ändern: A-29
  - Kistenwarenausgang: A-31
  - Lagerentnahme: A-22
  - Lagerumbuchungen: A-24
  - Lagerzugang: A-23
- **Lagerentnahme**: A-22
- **Lagerumbuchung**: A-24
- **Lagerzugang**: A-23

**M**
- **Menü**: A-16
- **Mitarbeiter**
  - A+W Business: A-12, A-13
- **Mitarbeiterwechsel**: A-15

**P**
- **Produktionsmeldung**: A-18
  - Bruchmeldung: A-20
  - Fertigmeldung: A-19

**S**
- **Scanner**
  - Einstellungen: A-10
  - Hauptmenü: A-16
  - Wareneingang: A-17
- **Sonstiges**: A-37

**U**
- **Ummelden**: A-38

**W**
- **Wareneingang**: A-17
