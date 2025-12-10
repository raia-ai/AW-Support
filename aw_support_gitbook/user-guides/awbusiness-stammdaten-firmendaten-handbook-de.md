---
title: "D-HB-AWBusiness_12"
source: "D-HB-AWBusiness_12.pdf"
tags: ["A+W Business", "Stammdaten", "Firmendaten", "EDI", "Kapazitätsplanung", "Software-Referenz", "Konfiguration", "Archivierung", "Produktion", "Versand"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein Software-Referenzhandbuch für den Bereich 'Firmendaten' in der A+W Business Software. Es beschreibt detailliert die Konfigurationsoptionen für verschiedene Module wie Lagervorschau, Webservices, EDI-Schnittstellen, Archivierung, Kapazitätsplanung, Produktion und Druckeinstellungen."
long_description: "Dieses Dokument dient als umfassendes Referenzhandbuch für die Konfiguration der Stammdaten im Bereich 'Firma' der A+W Business Software. Es bietet eine detaillierte Anleitung zu den verschiedenen Einstellungsregistern, die für den reibungslosen Betrieb des Systems unerlässlich sind. Die behandelten Themen umfassen die Lagervorschau, die Anbindung an den Dorma Webservice, die Konfiguration von Sendebestätigungen per E-Mail und die EDI-Schnittstelle. Ein großer Teil des Dokuments widmet sich den 'Firmendaten – Archiv', wo globale und dokumentenbezogene Einstellungen für die Archivierung, Statistikübergabe und den Umgang mit Reklamationen erläutert werden. Weitere Hauptabschnitte sind 'Firmendaten – Tagesabschluss' zur Verwaltung von Datenvorhaltezeiten, 'Firmendaten – System' für grundlegende Systemparameter wie Maßsysteme und Datumsformate, 'Firmendaten – Kalkulation' zur Definition von Kosten- und Aufschlagskalkulationen, und 'Firmendaten – Druck' zur Konfiguration von Monatsrechnungen und Druckservern. Das Handbuch deckt auch die Module 'Firmendaten – Produktion' mit Einstellungen zur Produktionsübergabe und Rückmeldung sowie 'Firmendaten – Kapa-Planung' zur Steuerung der Kapazitätsplanung ab. Schließlich werden Bereiche wie 'Versand', 'Mitarbeiterverwaltung', 'Texte' und 'Formulare' behandelt, um eine vollständige Konfiguration der Unternehmensdaten zu ermöglichen. Das Dokument richtet sich an Systemadministratoren und fortgeschrittene Anwender, die für die Einrichtung und Wartung der A+W Business Software verantwortlich sind."
---

# Firma

---
## Lagervorschau

**Anzahl Werktage**
In der Lagervorschau wird die Verfügbarkeit von Produkten für einen bestimmten Zeitraum in der Zukunft angezeigt. Mit der Anzahl der Tage legen Sie fest, wie viele Werktage die Vorschau anzeigen soll. Die Anzeige rechnet vom aktuellen Datum an.

## Dorma Webservice

Die Daten in diesem Bereich müssen eingegeben werden, wenn der BMECat von der Dorma Webseite heruntergeladen werden soll. Diese Daten sind identisch mit denen für die automatischen Dorma-Bestellungen.

**Adresse**
Internet-Adresse des Dorma-Webservices.

**[Weltkugel]**
Wenn Sie die Internet-Adresse eingetragen oder geändert haben, können Sie über diese Schaltfläche prüfen, ob die Verbindung aufgebaut werden kann.

**Benutzer, Passwort**
Anmeldedaten, mit denen Sie berechtigt sind, auf den Dorma-Webservice zuzugreifen.

## Kosten in Bestellung zurückschreiben

Bei Bestellungen können sich die tatsächlichen Kosten gegenüber denen aus den Lieferantendaten geändert haben.

- Die Kosten werden nicht zurückgeschrieben. In der Bestellung werden die Kosten aus den Stammdaten unverändert angezeigt.
- Die aktuellen Kosten der bestellten Artikel werden in die Bestellung zurückgeschrieben.

**[A+W Testzugang]**
Mit dieser Schaltfläche können Sie die Zugangsdaten auf den Testzugang der A+W Software GmbH umstellen. Damit können Sie prüfen, ob die Verbindung mit diesen Daten korrekt aufgebaut werden kann.

## Dorma Sendebestätigung per E-Mail

Um sicherzugehen, dass eine Online-Bestellung abgeschickt wurde, können Sie automatisch eine Sendebestätigung erstellen lassen.

**Server**
Name des Servers, über den die Sendebestätigung gesteuert wird.

**Port**
Nummer des Ports für die Sendebestätigung.

**Absender Adresse, Empfänger Adresse, Kopie an**
E-Mail-Adressen, die standardmäßig für die Sendebestätigung verwendet werden sollen.

**Authentifizierung**
Für die Sendebestätigung kann eine Authentifizierung verwendet werden.
- Die Sendebestätigung wird nicht ohne Authentifizierung gesendet.
- Für die Sendebestätigung ist Authentifizierung erforderlich. Die Felder zur Eingabe der Anmeldedaten werden freigeschaltet.

**SSL Verschlüsselung verwenden**
Secure Sockets Layer (SSL); Verschlüsselungsprogramm zur sicheren Datenübertragung im Internet.
- Die Sendebestätigung wird nicht verschlüsselt.
- Die Sendebestätigung wird nach dem SSL-Protokoll verschlüsselt.

**Benutzer, Passwort**
Anmeldedaten, mit denen der Sender sich authentifiziert.

## EDI-Schnittstelle

Dokumente können elektronisch (als Datei) ausgetauscht und die Daten beim Import in ein anderes System sofort übernommen werden. Die nachfolgenden Einstellungen sind nur wichtig, wenn Sie mit EDI-Schnittstellen arbeiten.

**OEM/ANSI Konvertierung deaktivieren**
Die Daten werden für die Übertragung über eine Schnittstelle in ein Format konvertiert, das von allen anderen Programmen gelesen werden kann.

- Standardmäßig werden die Daten der zu transferierenden Datei automatisch im ANSI-Format konvertiert, z. B. ä in ae.
- In seltenen Fällen muss die Datenkonvertierung ausgeschaltet werden. z. B. in Verbindung mit speziellen Schnittstellen.

**Autom. Einlastung in Kapazitätsplanung deaktivieren**
Diese Einstellung betrifft das nur die A+W Business-Kapazitätsplanung. Sie wird benötigt, wenn Auftragsdaten elektronisch übermittelt werden sollen. In der Regel werden die Daten mit einem Workflow-Task übertragen.

- Standardmäßig werden die Daten der importierten Aufträge automatisch in die Kapazitätsplanung eingelastet, sofern die automatische Einlastung aktiviert ist.
- Die automatische Einlastung von importierten Aufträgen ist ausgeschaltet. Damit haben Sie die Möglichkeit, die importierten Aufträge vor der Einlastung zu prüfen.

Wenn Sie die A+W Business-Kapazitätsplanung nutzen, darf die Checkbox für das Planwertverfahren nicht aktiviert sein.
-> "Automatische Einlastung ins Planwertverfahren" auf Seite B-1078

**Architekt aus Kopfsatz für Artikelreferenz verwenden**
Beim EDI-Import kann der Name des Architekten einem bestimmten Artikel zugeordnet werden. Diese Funktion ist nur kundenspezifisch freigeschaltet.

- Beim EDI-Import wird im Kopfsatz keine Artikelreferenz verwendet.
- Beim EDI-Import wird im Kopfsatz die Artikelreferenz auf den Architekten eingetragen.

Die zum Import verwendete Architekten-Nummer wird beim Import mit in den Auftrag übertragen, um später die eCommerce-Aufträge von den restlichen Aufträgen zu unterscheiden.

## Erfassungsstellenzuordnung

**Auftrag produziert bei**
Wenn eine Position an die gewählte Erfassungsstelle gemeldet wurde, wird sie in A+W Business auf den Status produziert gesetzt. Die dazu gehörende Laufnummer wird in die Auftragsposition zurückgeschrieben.
Wenn Rückmeldungen von AWBar oder A+W Production in Dateien der folgenden Typen STSP, STSL, STSD, STSB, STSG geschrieben werden, muss eine Erfassungsstelle ausgewählt werden, die einem Statuspunkt zugewiesen ist. Wenn eine solche Erfassungsstelle nicht zugewiesen wurde, erzeugt die Rückmeldung einen Fehler.
Die Auftragsinfo zeigt diese Position im Register Produziert an. Das Produktionsdatum im Auftragskopf wird aktualisiert.
-> Statistik, "Auftragsinformation" auf Seite F-2630

**Wareneingang bei**
Angabe der Erfassungsstelle, von der der Wareneingang gemeldet wird.

**Prüfung der Bestellteile im Einkauf**
Der Wareneingang von Bestellteilen kann über eine Erfassungsstelle oder im Einkauf geprüft werden.

- Wareneingänge von Teillieferungsposition werden durch die per STSG zurückgemeldete verpackte Menge geprüft. Die gemeldeten Mengen werden bei der Erzeugung von Teillieferungen abgefragt. Die Teillieferung kann nur für die gemeldete Menge erstellt werden.
- Der Wareneingang von Bestellteilen wird im Einkauf geprüft.

## Firmendaten – Archiv

*Stammdaten > Firma > Firmendaten > Register Archiv*

*Abb. B-593 Firmendaten – Archiv*

> In diesem Register geben Sie an, wie die Archivierung von Daten und Dokumenten durchgeführt werden soll.
> -> Tutorial 1, "Datenbank" auf Seite B-440
> -> Tutorial 1, "Statistik" auf Seite B-442

### Globale Einstellungen

Die Einstellungen in diesem Bereich beziehen sich auf die automatische Archivierung, die Sie im Bereich Automatikoptionen aktivieren können.

**Archivdatenbank**
Name der A+W Business-Archivdatenbank. Üblicherweise wird das Kundenkürzel als Namen verwendet. Der Name der Archivdatenbank wird beim Einrichten des Archivs um die Jahreszahl erweitert, für die es gültig ist. Damit können Sie mehrere Archiv-Jahre gleichzeitig verwalten.

> **Neues Archiv einrichten**
> Denken Sie daran, sich rechtzeitig für das Folgejahr von der A+W Software GmbH ein neues Archiv anlegen zu lassen.

**Reklamationen in Vertreterprovisionierung verarbeiten**
Reklamationen können bei der Berechnung der Vertreterprovision berücksichtigt werden.

- Standardmäßig werden Reklamationen nicht berücksichtigt. Die Provision wird nicht reduziert.
- Die Reklamationen werden im Vertreterumsatz berücksichtigt. Die Provision des Vertreters reduziert sich im Verhältnis zu den ihn betreffenden Reklamationen jedoch nicht.

**Reklamationen ohne Mengen (St., Qm, Lfm) an Umsatzstat.**
Reklamationen können in Bezug auf die Preise und die Mengen ausgewertet werden.

- Neben den Beträgen werden auch die Mengen (Stück, Quadratmeter, Laufmeter usw.) an die Umsatzstatistik übergeben. Das kann bedeuten, dass die Mengen aus Reklamationen ohne Rechnungsstellung das Gesamtergebnis reduzieren.
- Standardmäßig wird nur der Preis an die Umsatzstatistik übergeben.

**Export Superstatistik**
Diese Option betrifft das Modul Gruppenstatistik. Die Gruppenstatistik ist für Firmengruppen konzipiert, die auf unterschiedlichen Servern mit jeweils eigenen Datenbanken arbeiten, jedoch eine statistische Gesamtauswertung aller Firmen erhalten möchten.

- Bei der Hauptfirma, in der die Gesamtauswertung erfolgt, muss diese Checkbox deaktiviert bleiben.
- Beim Mandanten, der die statistischen Daten liefert, muss diese Checkbox aktiviert sein.
- > Statistik, "Superstatistik" auf Seite F-2653

**Statistikübergabe ohne Rechnungs-/Gutschriftdruck**
Umsätze und Mengen können wahlweise vor oder nach dem Druck von Rechnungen und Gutschriften statistisch ausgewertet werden.

- Standardmäßig muss die beim Druck erzeugte Rechnungsnummer vorliegen, um die Übergabe an die Statistik auszulösen.
- Aufträge können auch ohne Rechnungs- bzw. Gutschriftendruck an die Statistik übergeben werden. Auslöser ist dann der Mindeststatus, den Sie dafür angegeben haben.
- >Tutorial 2, "Sperrstatus" auf Seite B-497

**Statistikübergabe nur nach Rechnungskontrolle**
Diese Option betrifft nur das Modul Rechnungskontrolle im Einkauf.

- Standardmäßig werden Bestellungen ohne Rechnungskontrolle an die Einkaufsstatistik übergeben.
- Bestellungen können erst dann an die Statistik übergeben werden, wenn die Rechnungskontrolle durchgeführt wurde.

**Umsatz Stücklistengläser auf Hauptprodukt übertragen**
Der Umsatz von Austauschgläsern kann getrennt oder mit dem Hauptprodukt zusammen statistisch ausgewertet werden.

- Standardmäßig fließt der Austauschzuschlag in den Umsatz der eingetauschten Komponente ein.
- Der Austauschzuschlag soll in den Umsatz des Hauptproduktes einfließen. Die Checkbox für die Auswertung Kosten wird freigeschaltet.

**Kosten Stücklistenelemente auf Hauptprodukt übertragen**
Die Kosten von Austauschgläsern können getrennt oder mit dem Hauptprodukt zusammen statistisch ausgewertet werden. Die Checkbox ist nur freigeschaltet, wenn die Checkbox für die Auswertung des Umsatzes markiert ist.

- Standardmäßig fließen die Kosten von Austauschgläsern in die Kosten der eingetauschten Komponente ein.
- Die Kosten der Austauschgläser sollen in die Kosten des Hauptproduktes einfließen.

**Statistikübergabe Kistenmenge/-Fläche auf Position buchen**
Die Fläche und Menge einer Kiste kann für die Statistik auf der Ebene der Stücklisten-Komponenten oder auf der Ebene der Positionen ausgewertet werden.

- Standardmäßig wird der Inhalt von Kisten auf der Ebene der Stücklisten-Komponenten in die Statistik gebucht.
- Der Inhalt von Kisten soll auf der Ebene der Positionen in die Statistik gebucht werden. Die Auswertungstiefe darf bei dieser Einstellung in der Statistik nur noch auf Positionen bezogen werden. Die Auswertungstiefe Position und Stückliste würde sonst die Flächen auf der Ebene der Warengruppen verfälschen, da für das Glas und die Bearbeitung die Fläche ermittelt wird.

> **Statistik-Update**
> Wenn die Einstellung Statistikübergabe Kistenmenge/-Fläche auf Position buchen gewählt wurde, muss die Statistik unbedingt über Utilities > System > Statistik Update neu erstellt werden.

**Übergabe Archiv nach Erfassungsdatum**
Dokumente werden anhand ihres Datums archiviert.

- Standardmäßig wird für die Archivierung das Rechnungsdatum herangezogen.
- Für die Archivierung wird das Erfassungsdatum des Auftrags herangezogen.

**Dokument ohne Referenzprüfung löschen**
Diese Einstellung betrifft nur Dokumente mit Referenz auf ein anderes Dokument, z. B. Bestellungen zu Aufträgen, Teillieferungen, Reklamationen.

- Standardmäßig kann ein Dokument mit Referenz nur gelöscht werden, wenn der zugehörige Auftrag archiviert und aus der Hauptdatenbank gelöscht wurde.
- Das System prüft beim Löschen eines Dokumentes nicht, ob referenzierte Dokumente vorhanden sind. Das Archivjahr wird dabei nicht durch den Auftrag bestimmt, sondern durch die Bestellung selbst.

**Dokumente nur löschen wenn bereits archiviert**
Dokumente können aus der Hauptdatenbank gelöscht werden, um diese zu entlasten.

- Das Dokument kann ohne Prüfung des Archivs gelöscht werden.
- Ein Dokument (Auftrag, Bestellung usw.) kann nur dann (manuell) gelöscht werden, wenn es vorher an das Archiv übergeben wurde. Dazu sucht das System in der Historie nach dem entsprechenden Eintrag.

**Mehrfach-Archivierung**
Ist ein Auftrag erledigt, d. h. die Rechnung an die FiBu und die Statistik übergeben, wird das zugehörige Dokument archiviert.

- Jedes Dokument kann nur einmal archiviert werden.
- Dokumente können mehrfach archiviert werden. Diese Einstellung ist nur sinnvoll, wenn ein Dokument aus dem Archiv geholt und geändert wird. In diesem Falle wird das ursprüngliche Dokument gelöscht und nur das geänderte archiviert.

**Reklamationsaufträge nur in Umsatzstatistik verbuchen**
Reklamationsaufträge können die Umsatzstatik verfälschen.

- Standardmäßig werden die Umsätze von Aufträgen und zugehörigen Reklamationsaufträgen in die Umsatzstatistik gebucht.
- Reklamationsaufträge werden nur in die Umsatzstatistik gebucht. Dazu muss ein Reklamationsgrund angegeben sein.

> **Beispiel**
> Ein Auftrag wird reklamiert. Der Sachbearbeiter erfasst dazu einen Reklamationsauftrag mit dem Dokumententyp Reklamation ohne Reklamationsgrund. Über den Reklamationsauftrag wird eine Rechnung geschrieben und er wird wie ein Standard-Auftrag in der Statistik verbucht.
>
> Wenn die Reklamation berechtigt ist, wird als drittes Dokument eine Reklamationsgutschrift (Gutschrift mit Dokumententyp Reklamation mit einem Reklamationsgrund) erstellt. Diese korrigiert die Umsatzstatistik um den reklamierten VK (Kosten und Fläche bleiben unverändert) und bucht die Reklamationsstatistik, im Gegensatz zur Standardbuchung von Reklamationen, mit positiven Beträgen.

| Dokument | VK | Kosten | Fläche |
| :--- | :--- | :--- | :--- |
| Auftrag | 100 € | 50 € | 1,0 qm |
| Reklamationsauftrag | 100 € | 50 € | 1,0 qm |
| Reklamationsgutschrift | 100 € | 50 € | 1,0 qm |

**Buchung Umsatzstatistik:**

| | VK | Kosten | Fläche |
| :--- | :--- | :--- | :--- |
| Auftrag | 100 € | 50 € | 1,0 qm |
| Reklamationsauftrag | 200 € | 100 € | 2,0 qm |
| Reklamationsgutschrift | 100 € | 100 € | 2,0 qm |

**Buchung Reklamationsstatistik:**

| | VK | Kosten | Fläche |
| :--- | :- | :- | :--- |
| Auftrag | - | - | - |
| Reklamationsauftrag | - | - | - |
| Reklamationsgutschrift | 100 € | 50 € | 1,0 qm |

**Dokumente ohne Positionen archivieren**
Dokumente können auch dann archiviert werden, wenn in ihnen keine Positionen erfasst sind.
- Die Dokumente ohne Positionen werden nicht archiviert.
- ✔ Die Dokumente ohne Positionen werden ebenfalls archiviert.

### Reklamationsstatistik für Gutschriften

**Reklamationsverursacher als Pflichteingabe**
Wird eine Reklamation erfasst, können sowohl der Reklamationsort als auch der Reklamationsverursacher eingetragen werden.

- Standardmäßig ist die Auswahl des Reklamationsverursachers optional.
- Der Reklamationsverursacher muss ausgewählt werden, damit das Dokument gespeichert werden kann.
- > Softwarereferenz, "Reklamationsverursacher" auf Seite B-689

**Default Reklamationsort**
Für statistische Auswertungen kann der Reklamationsort mit der Reklamation erfasst werden. Bei mehreren Reklamationsorten kann einer von ihnen voreingestellt werden.

- Standardmäßig ist keine Auswahl für den Reklamationsort voreingestellt.
- Sie können den am häufigsten angegebenen Reklamationsort als Voreinstellung auswählen. Dieser kann im Dokument geändert werden.

### Dokumentenbezogene Einstellungen

Die Einstellungen in diesem Bereich gelten für den jeweils ausgewählten Dokumententyp.

**Dokumententyp**
Dokumententyp, für den Sie in den nachfolgenden Feldern die Automatikoptionen einstellen möchten. Die Einstellungen können sich je nach Dokumententyp unterscheiden.
-> Verkauf, "Übergabe Archiv" auf Seite C-1974

### Automatikoptionen

Die Einstellungen der nachfolgenden Felder beziehen sich auf den Dokumententyp, den Sie im Feld Dokumententyp ausgewählt haben. Sie können für jeden Dokumententyp andere Einstellungen für die automatische Archivierung vornehmen.
In der Regel werden die Dokumente bei der (automatischen) Archivierung sowohl an die Statistik als auch ans Archiv übergeben und dann aus der Hauptdatenbank gelöscht. Standardmäßig ist für die Übergabe an die Statistik der Monat, für die Archivierung das Jahr des Rechnungsdatums ausschlaggebend.

> **Einstellungen für die Archivübergabe**
> In der Dokumentenverwaltung können Details für die automatische Archivübergabe eingestellt werden.
> Zusätzlich sind manuelle Archivübergaben in den Dokumenten möglich.
> -> Verkauf, "Übergabe Archiv" auf Seite C-1974

**Übergabe Provisionsstatistik**
Diese Checkbox betrifft das Modul Vertreterprovisionierung.
- Die Daten werden nicht an die Provisionsstatistik übergeben.
- Mit der automatischen Archivierung werden die Daten auch an die Provisionsstatistik übergeben.
Prüfen Sie bei diesen Einstellungen auch das Feld Reklamation in Vertreterprovisionierung verarbeiten im Bereich Globale Einstellungen.

**Übergabe Umsatzstatistik**
Diese Checkbox betrifft das Modul Umsatzstatistik.
- Die Daten werden nicht an die Umsatzstatistik übergeben.
- Mit der automatischen Archivierung werden die Daten auch an die Umsatzstatistik übergeben.
Prüfen Sie bei diesen Einstellungen auch das Feld Reklamation ohne Mengen im Bereich Globale Einstellungen.

**Übergabe Archiv**
Diese Checkbox betrifft das Modul Dokumentenarchivierung. Pro Jahr wird ein eigenes Archiv eingerichtet. Das System archiviert beim Jahreswechsel die Dokumente in Abhängigkeit vom Rechnungsdatum in das alte oder in das neue Archiv.
- Die Dokumente werden nicht automatisch archiviert. Jedes Dokument kann jedoch manuell an das Archiv übergeben werden.
- Die Dokumente werden automatisch archiviert. Tragen Sie zusätzlich das Jahr der Archivdatendank ein.
Bei dieser Einstellung sollten Sie auch die Checkbox Dokument löschen aktivieren.

**Dokument löschen**
Dokumente sollten regelmäßig aus der Hauptdatenbank gelöscht werden, um diese zu entlasten.
- Die Dokumente werden bei der Archivierung nicht automatisch gelöscht.
- Die Dokumente werden nach der Übergabe ans Archiv aus der Hauptdatenbank gelöscht.

> **Hauptdatenbank entlasten**
> Löschen Sie die archivierten Dokumente aus der Hauptdatenbank. Sie entlasten damit Ihre Datenbank und können deutlich schneller arbeiten. Archivierte Dokumente können jederzeit aus dem Archiv zurückgeholt werden.

**Dokument aus iQuote löschen**
Diese Checkbox erlaubt es, Dokumente aus A+W iQuote zu löschen, wenn ein Auftrag oder Angebot durch das A+W Business gelöscht wird. Dabei werden auch die zugehörigen Konfigurationseinträge aus der Datenbank entfernt. Dadurch wird die Menge der in der Datenbank gespeicherten Daten reduziert.
- Die Dokumente werden nicht gelöscht.
- Die Dokumente werden aus der Hauptdatenbank gelöscht.

### Archivierungsmodus

Die Einstellungen der nachfolgenden Felder beziehen sich auf den Dokumententyp, den Sie im Feld Dokumententyp ausgewählt haben. Sie können für jeden Dokumententyp andere Einstellungen für den Archivierungsmodus wählen. Mit der Wahl der Option legen Sie den Modus fest:

- **Mindeststatus:** Status, ab dem automatisch archiviert werden soll. Standardmäßig ist für die automatische Archivierung der Status 820-Auto. Archivierung ausgewählt.
- **Dokument älter als x Tage:** Soll die automatische Archivierung vom Datum des Dokuments abhängig sein, kann die Anzahl der Tage eingegeben werden, die nach diesem Datum verstrichen sein müssen, bevor das Dokument archiviert wird.
- **Status + Dokument älter als:** Bei diesen Einstellungen müssen beide Kriterien erfüllt sein: Der entsprechende Status muss erreicht sein und das Dokument muss das eingetragene Alter erreicht haben.

### Archivierung A+W Production

**Pfad für Meldedatei**
Verzeichnis, in dem die Meldedatei abgelegt werden soll. Sie enthält die Liste der in A+W Business archivierten Aufträge. Diese Information nutzt A+W Production, um die entsprechenden Aufträge aus seinem System zu löschen.

**AV-Bereich für Laufnummer**
Die Laufnummern werden nur für den eingetragenen AV-Bereich ausgewertet. Die Laufnummer wird aus dem entsprechenden Nummernkreis im Dialog Nummernkreise im Feld Laufnummer A+W Production Archiv gewählt.
-> "Nummernkreise - Produktion" auf Seite B-1031

**Version**
Sind für einen AV-Bereich verschiedene Versionen hinterlegt, so kann die jeweils aktuelle ausgewählt werden.

## Firmendaten – Tagesabschluss

*Stammdaten > Firma > Firmendaten > Register Tagesabschluss*

*Abb. B-594 Firmendaten - Tagesabschluss*

In diesem Register legen Sie die Fristen fest, nach denen die Daten endgültig aus der Hauptdatenbank gelöscht werden.

### Vorhaltetage

In den nachfolgenden Feldern tragen Sie ein, wie viele Tage Daten für die Statistiken und Sicherungen in der Hauptdatenbank gespeichert bleiben sollen, bis sie automatisch und endgültig gelöscht werden. Sie halten damit die Datenbank kleiner und schneller.
Gelöscht werden alle Daten, die älter sind als die eingetragene Anzahl von Tagen. Dies betrifft nicht die archivierten Daten.

**Statistik**
Wenn Sie Jahresübersichten erzeugen möchten, tragen Sie mehr als 365 Tage ein, damit Sie einen ausreichenden Spielraum für die Erstellung der Reports (Berichte) haben.
-> Statistik, "Einkaufsstatistiken" auf Seite F-2665
-> Statistik, "Umsatzstatistik Einkauf" auf Seite F-2665

**Provisionsstatistik**
Bei einem langen Zeitraum können Sie in der Statistik die Provisionen mehrerer Jahre auswerten.
-> Statistik, "Provisionsstatistik" auf Seite F-2675

**Zeitwirtschaft**
Bei einem langen Zeitraum können Sie in der Statistik die Zeitwirtschaft mehrerer Jahre auswerten.
-> Kapazitätsplanung, "Statistik" auf Seite H-3185

**EDI Sicherungsdatei**
Sicherungsdateien für die Schnittstellen sind so lange sinnvoll, bis die Datenverarbeitung in den verbundenen Programmen erfolgreich abgeschlossen ist.
-> "Schnittstellen-Dienst" auf Seite B-1175

**Historien-Einträge**
Anzahl der Tage, die eine Dokumentenhistorie gespeichert bleibt.

**Auftragsinfo**
Für Auswertungszwecke wählen Sie eine längere Speicherdauer.
-> Statistik, "Auftragsinformation" auf Seite F-2630

**Lagerlogbuch**
In der Lagerhistorie werden die Lagerein- und -abgänge, Bestellungen etc. aufgelistet. Diese Liste können Sie überschaubar halten, indem Sie Einträge nach einer angemessenen Frist löschen.
-> Lagerwirtschaft, "Lagerhistorie" auf Seite G-2884

**Gestellhistorie**
Für Auswertungszwecke wählen Sie eine längere Speicherdauer.

**Kreditlimit-Snapshots**
In einem Kreditlimit-Snapshot können Sie über einen beliebigen Zeitraum die Entwicklung von bestimmten Finanzdaten der Kunden auswerten.
-> "Kreditlimit-Analyse" auf Seite B-975

**OderXML Datensätze**
Für Auswertungszwecke wählen Sie eine längere Speicherdauer.

### Systemlogbuch

**Alter von Einträgen bei Löschung**
Anzahl der Tage, die ein Logbucheintrag im Logbuch gespeichert bleiben soll, bis er automatisch und endgültig gelöscht wird.

**Archivpfad/Name**
Verzeichnis und Namen des Logbuch-Archivs.

## Firmendaten – System

*Stammdaten > Firma > Firmendaten > Register System*

*Abb. B-595 Firmendaten – System*

In diesem Register passen Sie das Maßsystem, Produktionsvorlauftage und die Übergabe an A+W Production und die Zeitwirtschaft an.

### Maßsystem

Die Auswahl des Maßsystems muss nicht für beide Bereiche gleich sein.

**Datenbank metrisch, imperial**
Maßsystem, das standardmäßig verwendet wird. Sie können Ihre Dokumente entweder im metrischen (=cm) oder im imperialen Maßsystem (=Inch) erfassen.

**Dicke metrisch, imperial**
Wenn Sie standardmäßig in Inch erfassen, kann es jedoch notwendig sein, dass die Dicke metrisch erfasst wird.

> **Maßsystem pro Kunde wählen**
> Sie können die globale Einstellung des Maßsystems pro Kunde überschreiben. Die Maße werden dann in den Dokumenten für diesen Kunden in das andere System umgerechnet.

**Maß-Präzision = 1/**
Bei Aktivierung des imperialen Maßsystems für die Datenbank geben Sie den Wert 32, 64 oder 128 ein, je nachdem, mit welchem Faktor die Berechnungen erfolgen sollen.
Wenn Sie mit dem metrischen Maßsystem arbeiten, tragen Sie im Feld Maß-Präzision den Wert 1 ein.

**Nachkommastellen metrisch**
Anzahl der Nachkommastellen des umschriebenen Rechtecks bei Modellen, wenn das Maßsystem auf metrisch eingestellt ist.

### Formate

**Datum**
Ausgabeform des Datums:
- dd.MM.yyyy
- MM.dd.yyyy
- MM/dd/yyyy
- yyyy-MM-dd
(d = Tag (day), M = Monat, y = Jahr (year))

**Zeit**
Ausgabeform der Zeit:
- hh:mm
- hh:mm AMPM (angelsächsische 24-Stunden-Uhr)
- hhhh/mm/ss
- hhhh-mm-ss
(h = Stunde (hour), m = Minute, s = Sekunde)

**Französische Tastaturunterstützung (. nach ,)**
Auf Tastaturen mit französischem Layout ist auf dem Ziffernblock das Dezimaltrennzeichen ein Punkt. In den Ländereinstellungen des Betriebssystems ist jedoch das Komma als Dezimaltrennzeichen eingetragen.

- Das Dezimaltrennzeichen wird nach den Einstellungen des Betriebssystems angezeigt (Windows Ländereinstellungen).
- Das Dezimaltrennzeichen wird umgewandelt:
  - In Ländern, die ein Komma als Dezimaltrennzeichen verwenden, wird ein eingegebener Punkt in ein Komma umgewandelt.
  - In Ländern, die einen Punkt als Dezimaltrennzeichen verwenden, wird dieser in ein Komma umgewandelt.
Wenn die Feststelltaste aktiviert ist, wird das Dezimaltrennzeichen des Ziffernblocks auf den Punkt umgeleitet.

### Kundenversion

**Produzent, Handel**
Abhängig von dieser Einstellung werden bei der Erfassung im Dokumentenkopf unterschiedliche Felder für die Termine angezeigt. Die Berechnung der Termine wird nach den Vorgaben im Bereich Vorlauftage durchgeführt.
Diesen Optionen entsprechend sollten Sie auch die Felder Produktionsstart und Anlieferung Lieferant im Bereich Vorlauftage füllen (siehe unten).

**Kürzel**
Über das Kundenkürzel wird geprüft, welche speziellen Programmteile in dieser Installation von A+W Business aktiviert werden.

> **Kundenkürzel ändern**
> Wenn Sie das Kundenkürzel ändern, verlieren Sie den Zugriff auf die Funktionen, die speziell für Ihr Unternehmen entwickelt wurden.

**Edition**
Wenn unterschiedliche Ausgaben von A+W Business verfügbar sind, wird die zum Kundenkürzel passende Version angezeigt. In der Regel ist das aber die Standard-Edition.

### Vorlauftage

Die Felder in diesem Bereich beziehen sich auf die Felder im Bereich Kundenversion. In der Auftragserfassung können die Werte für die Vorlauftage überschrieben werden.
Im Tutorial finden Sie Beispiele für die Terminberechnung (Liefertermin Kunde, Versandtag, Produktionsstart usw.) im Auftragskopf.
-> Tutorial 1, "Lieferdauer" auf Seite B-183

**Produktionsstart**
Anzahl der Tage, die vom Versandtag im Auftragskopf standardmäßig abgezogen werden sollen, um den Termin für den Produktionsstart zu berechnen.
Diese Angabe wird benötigt, wenn Sie im Bereich Kundenversion die Option Produzent gewählt haben.
Produktionsstarttermin = Versandtag - Produktionsstart

**Produktion VSG**
Anzahl der Tage, die vom Versandtag im Auftragskopf standardmäßig abgezogen werden sollen, um den Termin für den Produktionsstart von VSG zu berechnen.
Dieses Feld wird nur angezeigt, wenn Sie als Kundenversion Produzent gewählt haben.

**Anlieferung Lieferant**
Anzahl der Tage, die vom Produktionsstart im Auftragskopf standardmäßig abgezogen werden sollen, um den Anliefertermin des Lieferanten zu berechnen.
Dieses Feld wird nur angezeigt, wenn Sie als Kundenversion Handel gewählt haben.
Anliefertermin Lieferant = Produktionsstarttermin – Anlieferung Lieferant

### Vorlauftage für Wiedervorlage

**(Dokument)**
Auswahl, ob Angebote oder Aufträge zur Wiedervorlage geprüft werden.

**(Tage)**
Anzahl der Tage, nach denen das System Sie automatisch daran erinnern soll, dass ein Auftrag oder Angebot zur Wiedervorlage bereitliegt.
Bei der Erfassung eines neuen Angebotes wird der Wiedervorlagetermin automatisch aus dem Erfassungsdatum und den eingetragenen Tagen berechnet.

### Einstellungen

**Windows-Anmeldung für A+W Business-Login benutzen**
Diese Einstellung gilt für alle Benutzer. Sie kann nicht an bestimmte Benutzer gekoppelt werden.

- A+W Business kann nur über eine eigene Anmeldung gestartet werden.
- Nach der Anmeldung in Windows kann A+W Business ohne zusätzliche Anmeldung gestartet werden (SSO: Single Sign On). Dazu müssen der Benutzername und das Passwort identisch sein.
In einer Client-/Server-Installation muss zusätzlich die Domäne angegeben werden.

**Customizing aktiv**
Diese Einstellung betrifft kundenindividuelle Zusatzentwicklungen.

- A+W Business kann in der ausgelieferten Version genutzt werden.
- Zusätzliche Formulare, Variablen oder Felder können genutzt werden. Wenn Sie diese nicht benötigen, sollten Sie die Checkbox deaktivieren, um Ihre Datenbank zu entlasten.

**Exchange Service für Workflow aktivieren**
Für die Ausführung von Workflows und die Verarbeitung von Produktionsrückmeldungen der A+W Commercial Exchange Service zur Verfügung. Er löst den A+W Business 6 Interface Service ab.

- Der A+W Commercial Exchange Service wird nicht genutzt.
- Der A+W Commercial Exchange Service wird genutzt.

**openTrans Export in Thread**
Anzahl der openTrans-Übertragungen pro Exportprozess.

### A+W CAD Designer (Shapes)

**Ansicht**
Ansicht für die SN-Datei:
- Endprodukt (Zeichnung): Dies ist die Standardeinstellung, wenn Sie mit dem SN-Editor arbeiten.
- Kantenbearbeitung (Zeichnung): Mit dieser Einstellung werden nur die Kantenbearbeitungen angezeigt.

**Farbtiefe**
Farbeinstellung für die Anzeige von SN-Dateien:
- **1 Bit:** Diese Einstellung wird für Strichzeichnungen verwendet. Die Darstellung ist monochrom.
- **4 Bit:** Mit dieser Einstellung können 16 Farben bzw. Grauwerte angezeigt werden.
- **8 Bit:** Dies ist die Standardeinstellung. Mit dieser Einstellung können bis zu 256 Farben dargestellt werden.

**Scheibenhintergrund**
Die Einstellung bezieht sich auf die Darstellung der Skizze.
- **Gefüllt:** Die Scheibe wird als farbige Fläche dargestellt.
- **Nicht gefüllt:** Nur die Umrisslinien der Scheibe werden dargestellt.

**Dekorationsgröße, Segmenttext, Maßangaben**
Größe der Darstellung einer SN-Datei in der Positionserfassung. Standardeinstellungen:
- Dekorationsgröße: 12 px
- Segmenttext: 14 px
- Maßangaben: 16 px

**Dateipfad**
Speicherort für SN-Datei. Für die Übergabe an die Produktion muss das Verzeichnis auch A+W Production bekannt sein. Lassen Sie den Pfad aus Sicherheitsgründen immer mit Doppel-Backslash beginnen und tragen Sie die gesamte Adresse (IP) ein.

**Nur Produktionsstücklistenaufgelöste Bearbeitungen**
Die Produktionsstücklistenauflösung für Bearbeitungen kann aus der SN-Datei übernommen werden. Produktionsstücklistenauflösungen aus Makros werden immer übernommen.

- Die gesamte Produktionsstücklistenauflösung wird übernommen.
- Nur die Produktionsstücklistenauflösung für Bearbeitungen wird übernommen.

**Nur bei strukturellen Änderungen**
Die SN-Dateien werden nach Änderungen neu erzeugt. Diese Funktion ist nur bei strukturellen Änderungen sinnvoll.

- Bei jeder Änderung wird eine neue SN-Datei erzeugt. Die betrifft auch Änderungen, die nicht produktionsrelevant sind.
- Nur bei strukturellen Änderungen wird eine neue SN-Datei erzeugt. z. B. wenn die Maße geändert wurden.

**Kantenbearbeitungen und Bohrungen auf Modell 99**
Kantenbearbeitungen und Bohrungen können bei freien Formen und auf importierten SN-Dateien angebracht werden.

- Bei dem Modell 99 können in der zugehörigen SN-Datei keine zusätzlichen Bearbeitungen erfasst werden.
- Die Kantenbearbeitungen und Bohrungen werden in der SN-Zeichnung gespeichert.
Diese Funktion bezieht sich nur auf die Vermaßungsart umschriebenes Rechteck und auf die Programmversion 6 von A+W CAD Designer (Shapes).
Bei einer freien Form (Modell 99) können Kantenbearbeitungen nicht selektiv angebracht werden, sondern nur an allen Kanten zusammen. Bohrungen können nur mit Bezug auf das umschriebene Rechteck bemaßt werden.
Wenn beim Import der SN Datei im A+W Business auf ein Standardmodell gewechselt wird, können Kantenbearbeitungen auf einzelnen Kanten erfasst werden, wenn eine Kantennummerierung (1, 2, 3, 4) in der SN- oder DFX-Datei vorhanden ist.

**URL für AWSOA Dienste**
Angabe des A+W SOA-Dienstes. Mit diesem Dienst können u. a. Kapazitätsübersichten aus A+W Capacity Planner (EL) eingelesen werden, um die freien und die belegten Kapazitäten einzusehen.

**Kundenlogo**
Pfad zu den Dateien der Kundenlogos. Das Kundenlogo wird im Dialog Logoposition angegeben.
-> "Logo" auf Seite B-973

**Pfad zu Produktbildern**
Pfad zum Verzeichnis mit den Produktbildern, die jeweils einem Produkt zugeordnet sind. Diese Bilder werden für den Druck auf Formularen herangezogen.
-> "Artikelskizze" auf Seite B-711

### Replikation

Bei der Replikation werden die Stammdaten von der Datenbank des Hauptsitzes in die Datenbanken der Filialen kopiert.
Die Replikation wird im Modul Utilities > Replikationsverwaltung gestartet.

**Replikationsempfänger**
Sie benötigen diese Funktion nur, wenn Sie mit mehreren Filialen mit jeweils eigenen Datenbanken arbeiten.

- Im Hauptsitz darf diese Checkbox nicht aktiviert sein.
- In den Filialen muss die Checkbox aktiviert sein. Dadurch werden alle Felder in den Stammdaten gesperrt, die über die Hauptdatenbank gepflegt werden.

**Sprache**
Im Dialog Replikation werden die Beschreibungsfelder der Tabellen und Spalten in der ausgewählten Sprache angezeigt.

### Datenbankparameter

**Isolation Level**
Der Transaktionsmodus der Datenbank kann umgestellt werden:
- **RL:** Release Lock (restriktiver Transaktionsmodus). Dies ist die Einstellung für die älteren Versionen von A+W Business.
- **RC:** Read Committed (restriktiver Transaktionsmodus). Diese Einstellung erhöht die Performance. Sie wird nach dem Neustart an allen Arbeitsplätzen übernommen.

### A+W CAD Designer (Bars)

**Lichte Feldvermaßung anzeigen**
Für die Sprossenkonstruktion können die Maße der lichten Felder angezeigt werden.
- Die Maße der lichten Felder werden nicht angezeigt.
- Die Maße der Glasflächen ohne die Sprossenbreite (lichte Felder) werden angezeigt.

**Gittermengen aus Makros addieren**
Preismengen aus A+W CAD Designer (Bars)-Makros können übernommen werden.
- Die Preismengen werden nicht übernommen.
- Die Preismengen aus A+W CAD Designer (Bars) werden übernommen und zu den vorhandenen Mengen hinzugerechnet. Wenn z. B. eine Sonne mit drei Feldern eingefügt wird, werden diese zusätzlichen Felder zur Menge der Felder hinzugerechnet.

**AWD20.INI für Konstruktionsdruck**
Die maßstäbliche Sprossenskizze kann nach der Konfiguration für CAD Designer Bars gedruckt werden.
- Die Sprossenskizze wird nach dem Standard von A+W Business gedruckt.
- Die Konfiguration für CAD Designer Bars wird verwendet, wenn im Auftrag eine vermaßte Skizze für Sprossen mit der Einstellung Sprossenzuschnittsliste ausgeben gedruckt wird.
- > Verkauf, "Vermaßte Skizze drucken" auf Seite C-1936

### Datenbank

**Transaktionen**
Die Datenbankunterstützung für SQL Server erlaubt auch Transaktionen. Damit können aufeinander folgende SQL Befehle, die Daten verändern, rückgängig gemacht werden, solange die Transaktion nicht abgeschlossen ist.
- Datenbank-Transaktionen sind möglich nur für Datenbanksystem SQL Base möglich.
- Datenbank-Transaktionen sind für SQL-Server möglich. Diese Einstellung ist wichtig für das Datenbanksystem Microsoft SQL Server.
Für das Datenbanksystem SQL Base ist die Transaktionslogik immer aktiv.

## Firmendaten - Kalkulation

*Stammdaten > Firma > Firmendaten > Register Kalkulation*

*Abb. B-596 Firmendaten - Kalkulation*

In diesem Register hinterlegen Sie die Zuschläge für die Kostenkalkulation.
-> Tutorial 2, "Kosten- und Aufschlagskalkulation" auf Seite B-615

### Kosten + Aufschlagkalkulation

Die in der Dokumentenerfassung berechneten Kosten können Sie sich in der Auftrags- und in der Positionserfassung anzeigen lassen.

#### Materialgemeinkosten

**Beschaffungsart**
Die Beschaffungsarten sind von A+W Business vorgegeben.

**% Zuschlag**
Prozentualer Zuschlag, der bei der jeweiligen Beschaffungsart berechnet werden soll.

**Lohnnebenkosten**
Prozentualen Zuschlag für die Lohnnebenkosten.

**Vertriebsgemeinkostenzuschlag**
Prozentualen Zuschlag für die Vertriebsgemeinkosten.

**Verwaltungsgemeinkostenzuschlag**
Prozentualen Zuschlag für die Verwaltungsgemeinkosten.

**Gewinnspanne**
Prozentualen Zuschlag für die Gewinnerwartung.

### Flächenkapazitäten

**Wochentag, ISO, VSG, ESG**
Diese Tabelle betrifft nur das Modul Kapazitäts-Informationssystem auf Kundenbasis.
Für die drei Hauptproduktarten (ISO, VSG, ESG) können Gesamtkapazitäten hinterlegt werden. Von diesen können Anteile für die Hauptkunden (Keykunden) reserviert werden. Diese Anteile werden in den Stammdaten des entsprechenden Kunden hinterlegt.
-> "Partnerverwaltung - Produktion" auf Seite B-915

Alle Kunden, für die keine eigenen Kapazitäten hinterlegt sind, werden in einer Gruppe zusammengefasst und mit der Restkapazität belegt. Bei der Auftragserfassung wird dann über die Funktion Kapazitätsinfo nach Kunde angezeigt, wann wie viel Kapazität für die Produktion frei ist.
-> Verkauf, "Dokument - Kopfdaten" auf Seite C-1687

### Default-Deckungsbeiträge

**Mindestbeitrag**
Prozentwert der Deckungsbeiträge, der bei Änderungen im Auftrag nicht unterschritten werden darf.

**Maximalbeitrag**
Prozentwert der Deckungsbeiträge, der bei Änderungen im Auftrag nicht überschritten werden darf.

## Firmendaten – Druck

*Stammdaten > Firma > Firmendaten > Register Druck*

*Abb. B-597 Firmendaten – Druck*

In diesem Register legen Sie die Einstellungen für den Druck von Dokumenten fest.

### Monatsrechnungen

Die Felder in diesem Bereich betreffen das Modul Monatsrechnungen.
In den Kundenstammdaten muss die Checkbox Monatsrechnung aktiviert sein.
-> "Partnerverwaltung - Finanzen" auf Seite B-904

Allen Kundenaufträgen mit dem Kennzeichen Monatsrechnung wird automatisch der Statuspunkt 73-Monatsrechnung zugewiesen.
Welchem Anwenderstatus dies in Ihrer A+W Business-Version entspricht, hängt von Ihrer eigenen Statusorganisation ab. Die gekennzeichneten Aufträge können Sie dann pro Kunde anhand dieses Status selektieren und zusammen fakturieren.
-> Tutorial 2, "Statusverwaltung" auf Seite B-492
-> Verkauf, "Monatsrechnung" auf Seite C-1287

**Druckpunkt**
Druckpunkt für den Formulardruck. Standard-Einstellung 103-Rechnungen.

**Post, Fax, Mail**
Für den Druck von Monatsrechnungen können Sie festlegen, mit welcher Versandart, die Rechnung gedruckt werden soll.
- Der Druckpunkt wird nicht verwendet.
- Der Druckpunkt wird beim Druck von Monatsrechnungen verwendet. Beim Druck wird der Status der Dokumente umgesetzt. Dazu muss der Statuspunkt auf 73-Monatsrechnung. gesetzt werden.

**Statuspunkt**
Standard-Einstellung 73-Monatsrechnung. Aufträge für Kunden mit Monatsrechnung, die versehentlich in den Rechnungslauf gelangen, werden automatisch auf den Statuspunkt 73-Monatsrechnung gesetzt.

### Skizzendruck

**Erweiterte Sprossenskizze im Formulardruck**
Skizzen können schematisch oder maßstabsgerecht gedruckt werden. Die Einstellung kann im jeweiligen Auftrag überschrieben werden.

- Standardmäßig werden die Sprossen im Druck schematisch dargestellt.
- Die Sprossenskizze kann in detaillierter Form gedruckt werden. Dazu muss in der Formularverwaltung die Skizzengröße für die Detaildarstellung erhöht werden. Die Funktion für den maßstäblichen Druck muss auch im Auftrag eingestellt werden.
  -> Tutorial 2, "Skizzendruck" auf Seite B-552
  -> "Modellskizze, Sprossenskizze" auf Seite B-1211

### Stückliste

**Maximale Anzahl**
Anzahl der Stücklisteneinträge beim Formulardruck, die an den Formulardruck übergeben werden. Legen Sie die Zahl so fest, dass die bei Ihnen vorkommenden Stücklisten tatsächlich verarbeitet werden können. Hat ein Auftrag eine tiefere Stückliste, werden alle Einträge, die die Höchstzahl überschreiten, nicht gedruckt.
Bewährt hat sich die Einstellung von 15 - 20 Einträgen. Eine höhere Anzahl verlangsamt die Verarbeitungsgeschwindigkeit von Aufträgen erheblich.

### Druckserver

Das Feld betrifft das Modul Druckserver.
-> "Druckaufträge" auf Seite B-1214

**Servername**
Tragen Sie den Namen des Servers ein, auf dem der Druck-Server installiert ist.

### Druckerliste

**Verfügbare Drucker über Windows API auslesen**
Wenn Sie mit mehreren Druckern arbeiten, können diese beim Formulardruck zur Auswahl angeboten werden. Für den Druck auf einem Server müssen Druckaufträge angelegt werden.

- Der Formulardruck wird an den Standarddrucker gesendet.
- Beim Druck kann einer der verfügbaren Drucker ausgewählt werden. Mit dieser Einstellung kann gewählt werden, ob ein Formular als PDF-Datei, als Fax oder als Hardcopy (Papier) ausgegeben wird.

### Wiederholungsdruck für Dokumentenarchivierung

**Drucker**
Auswahl des Standard-Druckers.
Wenn z. B. für das DMS System ELO (Elektronischer Leitz Ordner) automatisch ein Wiederholungsdruck gestartet werden soll, muss der ELO Drucker angegeben werden.

### DMS

**Archivpfad**
Pfad, in dem die Dokumentendateien abgelegt werden sollen. Alle Dokumente, die in A+W Business archiviert werden können, werden damit gleichzeitig mit dem Dokumenten-Management-System Saperion (DMS) archiviert.

### Primäre Formular-/Reportsuche

Mandanten können unterschiedliche Formulare für den Druck und für Reports verwenden. Dazu tragen Sie einen Pfad für die primäre Formular-/Reportsuche ein. Der Formulardruck und der Reportdruck suchen in diesem Verzeichnis nach dem Report und Formular.
Falls diese Formulare dort nicht liegen, wird auf das Standard-Installationsverzeichnis zurückgegriffen.

**Pfad**
Pfad, in dem die Formulare liegen, die der aktuelle Mandant verwendet. In diesem Pfad können auch geänderte Standard-Reports liegen. Das Feld kann leer bleiben, wenn alle Mandanten mit denselben Formularen arbeiten oder wenn nur ein Mandant angelegt ist.

### Crystal Reports ODBC

**DSN**
Name des Domain-Servers, auf dem die Applikation liegt.

**Benutzer, Passwort**
Anmeldedaten für den Zugang zu Crystal Reports.

### Formulardruck

**Formulardruck über Crystal Reports**
Die Reports können alternativ zu den internen Reportformularen auch über Crystal Reports gedruckt werden.
- Crystal Reports wird nicht verwendet.
- Die Formulare werden über Crystal Reports ausgegeben.

**Pfad**
Pfad, in dem die Formulare liegen.

**Mail**
Drucker, über den die Reports ausgegeben werden.

### Dokumentenmanagement

**Archivierungssystem aktivieren**
Wenn Sie mit einem Dokumenten-Management-System (DMS) arbeiten, können Sie die Dokumente in diesem DMS zusätzlich archivieren, z. B. in Saperion. Dazu muss die entsprechende Schnittstelle eingerichtet sein.
- Die Dokumente werden nicht an ein DMS übergeben.
- Die Dokumente werden automatisch an das angeschlossene DMS übergeben. Dazu müssen Sie für jedes Formular die Dokumentenarchivierung in der Formularverwaltung aktiviert.
Mit dieser Einstellung wird z. B. beim Druck der Rechnung automatisch erst die Rechnung verschickt und dann an das Dokumentenarchiv übergeben.
-> "Dokumentenarchivierung" auf Seite B-1204

**(Pfad)**
Angabe des Archivierungspfades.

## Firmendaten – Produktion

*Stammdaten > Firma > Firmendaten > Register Produktion*

*Abb. B-598 Firmendaten - Produktion*

In diesem Register legen Sie die Einstellungen für die Übergabe an die Produktion fest.

### Produktionsübergabe

**Profit-Center-Abrechnung aktiv**
Die Profit-Center-Abrechnung ermöglicht die Berechnung interner Leistungen zwischen unterschiedlichen Mandanten oder AV-Bereichen.
- Die Profit-Center-Abrechnung wird nicht genutzt.
- Bei der Produktionsübergabe eines Auftrags des ersten Mandanten wird automatisch eine Bestellung für den zuständigen Mandanten erzeugt.
Hierfür müssen in der Produktverwaltung für jedes Produkt pro Mandant bzw. AV-Bereich die entsprechenden Beschaffungsarten eingetragen sein.
Die Leistungen, die von dem jeweiligen Mandanten bzw. AV-Bereich erbracht wurden, werden anschließend verrechnet.
-> "Produktkennzeichen" auf Seite B-725

**[Aufträge]**
Öffnet den Dialog Einstellungen – Produktionsübergabe, um verschiedene Übergabeparameter für Aufträge einzustellen.
-> Fertigung, "Einstellungen Produktionsübergabe" auf Seite E-2470

**[Angebote]**
Öffnen den Dialog Einstellungen – Produktionsübergabe, um verschiedene Übergabeparameter für Angebote einzustellen.
-> Fertigung, "Einstellungen Produktionsübergabe" auf Seite E-2470
-> Fertigung, "Angebotsoptimierung" auf Seite E-2591

**Folgeaufträge erzeugen aktiv**
Wenn Ihre Produktionsbereiche (ISO, VSG und ESG) auf verschiedene Mandanten bzw. AV-Bereiche verteilt sind, können Sie bei internen Aufträgen automatisch Folgeaufträge für den jeweiligen Produktionsbereich erzeugen lassen.
- Für interne Aufträge wird kein Folgeauftrag erzeugt.
- Bei der Bestellübergabe werden automatisch alle internen Aufträge mit weiteren Folgeaufträgen für den jeweiligen Mandanten bzw. AV-Bereich erzeugt.
-> "Produktverwaltung - Lager/Einkauf" auf Seite B-723

**Erweiterung Werkbank (Light)**
Isolierglas und VSG kann im A+W Business komplett bestellt werden. Diese Positionen werden dann über den Einkauf an den Lieferanten übermittelt, in der Produktion werden sie als Zukaufteile (meistens nur zum Versand) betrachtet. Wenn aber ein Isolierglas aus intern zugeschnittenen Gläsern oder ein VSG laminieren bestellt werden soll, gab es in der Vergangenheit dafür keine Lösung, da die Produktion das Isolierglas als Bestellteil auch auf die Gläser übertragen hat und somit kein Zuschnitt erfolgte.
- Das Glas wird bestellt.
- Das Glas wird mit der Beschaffungsart 16 (Zuschnitt vor Bestellung) übergeben und die Gläser werden geschnitten. Nur der Zusammenbau oder das Laminieren wird zugekauft.
In der Lösung wird nicht berücksichtigt, dass die Scheiben zum Lieferanten müssen, dies muss intern manuell organisiert werden.

**Generierung von SN-Dateien (incl. EDI-Import)**
Sie können bei der Produktionsübergabe automatisch SN-Dateien erzeugen lassen.
- SN-Dateien (A+W CAD Designer) werden nicht automatisch erzeugt.
- Bei Produktionsübergabe bzw. beim EDI-Import wird für jede Position, die z. B. Einfachglas oder ESG enthält, automatisch eine SN-Datei für Rechtecke und Standardmodelle inklusive folgender Bearbeitungen erzeugt: Kantenbearbeitungen, Eckabschnitte, Eckausschnitte, Rundecken, Randausschnitte und Lochbohrungen. Dieses Verfahren ermöglicht Ihnen den Druck von maßstäblichen Skizzen auf Ihren Produktionspapieren.
Beim Erstellen einer SN-Datei wird der Anwenderstatus SN-Datei geprüft ergeben, so dass die anschließende Produktionsübergabe diesen Anwenderstatus als Mindeststatus nutzen kann.

**Importpriorisierung nach Liefertermin**
Mit dieser Option steuern Sie, ob an den OrderXML Dateinamen der Liefertermin in der Form <yyyy-MM-dd> angehängt wird. Dadurch kann der Produktionsimport Dateien mit früherem Liefertermin priorisiert einlesen. Dies ist besonders dann sinnvoll, wenn per EDI eine große Anzahl von Aufträgen ins System kommen, die den Import in die Produktion sehr lange auslasten. Somit würden frühe Lieferungen zu spät eingelastet. Bedingung hierfür ist aber, dass per EDI ein Liefertermin für die Aufträge übergeben wird.
- Der Liefertermin wird nicht an den Order XML Dateinamen angehängt.
- Der Liefertermin wird an den Order XML Dateinamen angehängt.

**Generierung Modell Nr. 0**
Sie können das Modell auswählen, das bei der automatischen Erstellung von SN-Dateien für rechteckige Scheiben eingefügt werden soll. Wenn Sie keine Angaben machen, wird das anzuhängende Modell bestimmt wie bisher.
Das Feld ist nur freigeschaltet, wenn die automatische Generierung von SN-Dateien aktiviert ist.

**Produktionsmanager**
Mit dieser Einstellung schalten Sie die Programmvariante A+W Business Pro ein.
Wenn Sie mit dem Modul Production Manager arbeiten, können bei dateiloser Rückmeldung auch Teillieferungen verbucht werden.
- Der Produktionsmanager wird nicht verwendet.
- Der Produktionsmanager ist aktiviert. Mit dieser Einstellung können Lager-Restplatten für Lauf-Optimierungen im Produktionsmanager einbezogen werden. Das Programm baut keine Verbindung zu A+W Production auf. Stattdessen steht eine Produktionsplanung im Modul Fertigung zur Verfügung.

**Dateipfad**
Pfad, in dem die Dateien abgelegt werden.

### A+W Production Anbindung

**PPS-Webservice-URL**
Adresse für den PPS-Webservice. Der PPS-Webservice wird für folgende Übertragungen benötigt:
- Produktionsfreigabe nach kapazitiver Übergabe
- Wareneingangsmeldung an A+W Production
- Stornierung

**[Weltkugel]**
Prüft, ob die Verbindung über die eingegebene URL aufgebaut werden kann.

**Storno der Produktionsübergabe über PPS-Webservice**
Bei der dateilosen Produktionsübergabe können Aufträge auf zwei unterschiedliche Arten storniert werden.
- Zur Stornierung werden Aufträge manuell mit einem Storno-Kennzeichen an die Produktion übergeben.
- Zur Stornierung werden Aufträge per PPS-Webservice an die Produktion übergeben. Die Stückzahlen der entsprechenden Auftragspositionen werden dazu im Auftrag manuell auf 0 gesetzt.

**Storno der Produktionsübergabe nur bis Status versandbereit**
Die Stornierung und damit die Herabsetzung des Status kann unterbunden werden, wenn der Auftrag schon produziert ist.
- Zur Stornierung werden Aufträge manuell mit einem Storno-Kennzeichen an die Produktion übergeben.
- Aufträge können nur bis zum Status versandbereit storniert werden. Dazu muss die Erfassungsstelle für den Status Auftrag produziert bei definiert werden.
  -> "Erfassungsstellenzuordnung" auf Seite B-1103
  In den Erfassungsstellen muss für diese Erfassungsstelle eine Statuszuordnung vorhanden sein und der zugeordnete Status definiert ob der Auftrag produziert ist, falls dieser größer oder gleich ist.

**Meldung Bestellinformationen**
Der Wareneingang von Bestellartikeln kann direkt an die Produktion weitergemeldet werden, damit die entsprechenden Aufträge mit den bestellten Artikeln produziert werden können. Je nach der Art der Produktionsübergabe können Sie folgende Einstellungen wählen:
- **Keine:** Bei dieser Einstellung wird der Wareneingang nicht an die Produktion gemeldet.
- **Durch AWPool-Übergabe:** Diese Einstellung wählen Sie, wenn Produktionsdaten in eine Datei geschrieben werden (AWPool oder OrderXML).
- **Durch PPS-Webservice:** Diese Einstellung wählen Sie, wenn Produktionsdaten dateilos übergeben werden.

### ERP-Webservice

**URL**
Adresse für ERP-Webservice. Der ERP-Webservice wird für folgende Übertragungen benötigt:
- Produktionsübergabe per OrderXML
- Planungsrückmeldungen aus A+W Capacity Planner
- Dateilose Produktionsrückmeldungen
- AWPort-Anbindung

### Stammdatenübergabe und Sprache A+W Production

Stammdaten müssen nur in A+W Business gepflegt werden und können an A+W Production übergeben werden.

**Servername**
Gläser, Bearbeitungen, Sprossen, Füllungen, Artikel, Abstandhaltern, Glasartengruppen, Glasarten, Tische, Jumbos und Jumbo-Tisch-Zuordnungen können zwischen A+W Business und A+W Production synchronisiert werden.
Tragen Sie dazu den Namen des A+W Production-Servers (DNS-Namen oder IP-Adresse) ein.
Zusätzlich müssen Sie in der Produktverwaltung angeben, welche Daten übergeben werden sollen.
-> "Produktverwaltung - A+W Production" auf Seite B-737

> **Erfassung der Stammdaten abschließen**
> Tragen Sie den Servernamen erst ein, wenn Sie die entsprechenden Stammdaten erfasst haben. Bleibt das Feld leer, können Sie z. B. Produkte erfassen, ohne dass die Daten übergeben werden.

**Abw. Produktionssprache**
Die Produktbezeichnungen und Texte können bei der OrderXML-Übergabe aus A+W Business in einer Sprache übergeben werden, die sich von der Sprache in A+W Production unterscheidet, z. B., weil sich die Sprachen von Auftragserfassung und Produktion unterscheiden. Das Feld zur Auswahl der Zielsprache ist nur freigeschaltet, wenn die Checkbox aktiviert ist.
- Die Einstellung der Sprache ist in den beiden Programmen identisch.
- Produktbezeichnungen und Texte werden aus A+W Business in einer anderen Sprache übergeben und sollen in die Zielsprache übersetzt werden. Manuell in der Auftragserfassung geänderte Texte werden nicht übersetzt.

### Online-Produktionsübersicht

Bei der Online-Produktionsübersicht kann ein Report vom PPS Webservice erzeugt werden. Diese Produktionsübersicht kann für mehrere Aufträge gleichzeitig angezeigt werden, wenn sie aus einem Nummernverwalter aufgerufen wird. Dazu geben Sie in Feld Reportparameter den Crystal Report an, der für die Produktionsübersicht verwendet werden soll.
Die Online-Produktionsübersicht bezieht die Daten direkt aus dem PPS Webservice.

**Reportparameter**
Angabe der Reportparameter in folgender Form:
Report=//awbawp60/Trans/Reports/BDE/AUW_OrderList_Status.rpt&Unterteile_anzeigen=1&Auftrag=[OrderList]
Dazu geben Sie unter Report die zu verwendende rpt-Datei an und verknüpfen die Report-Parameter mit &. Der Text [OrderList] wird vor der Übergabe an den PPS Webservice durch die entsprechenden Auftragsnummern ersetzt.

### Produktionsrückmeldung

**[Einstellungen]**
Öffnet den Dialog Produktionsrückmeldungen (Schnittstellendienst), um die Parameter für Rückmeldungen per Datei einzustellen.
-> "Schnittstellen-Dienst" auf Seite B-1175

**Dateilose Produktionsrückmeldung**
Die Rückmeldungen werden von A+W Production über den ERP-Webservice eingelagert und vom A+W Commercial Exchange Service verbucht.
- Rückmeldungen aus der Produktion werden nicht online eingelesen.
- Rückmeldungen aus der Produktion werden online eingelesen. Dazu werden keine Dateien gespeichert. Im Register Lager / EK /EDI werden die Steuerelemente zur Verwaltung der einzelnen STS-Dateien deaktiviert.
-> Fertigung, "Rückmeldungen aus der Produktion" auf Seite E-2353

**Rückmeldungen in Teillieferungen verbuchen**
Die dateilose Rückmeldung kann auch Produktionsrückmeldungen in Teillieferungen mit Teilfaktura verbuchen.
- Dateilose Rückmeldungen werden nicht in Teillieferungen verbucht.
- Dateilose Rückmeldungen werden in Teillieferungen verbucht.
Bei einer Rückmeldung für einen Auftrag werden zunächst alle Teillieferungen gesucht. Die gemeldeten Mengen werden entsprechend auf die gefundenen Dokumente verteilt. Dabei werden Rückmeldungen zuerst auf die Dokumente gebucht, deren Liefertermin am frühsten liegt. Dies bedingt, dass die Dokumente unterschiedliche Liefertermine haben sollten.
Wenn die Rückmeldung einer Erfassungsstelle für ein Dokument komplett ist, wird auf das folgende Dokument gebucht. Bruchmeldungen gelten dabei immer nur für den Originalauftrag, Übermengen für das Dokument mit dem spätesten Liefertermin. Bereits erfolgte Rückmeldungen werden beim Erstellen einer Teillieferung entsprechend der gewählten Mengen aufgeteilt. Damit ist es für die Verbuchung irrelevant, zu welchem Zeitpunkt der Produktion eine Teillieferung erstellt wird.

**Prod.freigabe Auftrag, falls Subauftrag produziert (STSP)**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden.
Zu einem Auftrag kann ein Teilauftrag erfasst sein. Wenn eine Produktionsrückmeldung einen solchen Subauftrag betrifft, kann der Status des Gesamtauftrags umgesetzt werden.
- Ein Auftrag wird nicht automatisch auf den Status zur Produktionsfreigabe gesetzt.
- Wenn die Subaufträge als produziert zurückgemeldet werden, erhöht sich der Status des Hauptauftrags automatisch auf Produktionsfreigabe.

**Laufnummer aus dem Auftragskopf übernehmen (STSP)**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden.
Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der A+W Business-Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
- Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
- Nach der Aktualisierung des Auftragskopfes erhalten alle Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für produziert ist.
-> "Erfassungsstellenzuordnung" auf Seite B-1103

**Produktionsgestellnummer in Position übernehmen (STSD)**
Das Feld ist nur freigeschaltet, wenn BDE-Rückmeldungen importiert werden.
Wenn in der BDE-Rückmeldung Gestellnummern zu Positionen enthalten sind, können diese in A+W Business der Position zugewiesen werden.
- Gestellnummern werden nicht in die Position übernommen.
- Die gemeldeten Gestellnummern werden in den Auftrag zurückgeschrieben und der jeweiligen Position zugeordnet.

**Update Produktionsübersicht durch Erfassungsstelle (STSG)**
Die STSG-Rückmeldung gibt an, welches Gestell der jeweiligen Auftragsposition zugeordnet ist und welche Mengen produziert sind. Die Gestellnummer wird auf dem Lieferschein gedruckt.
In diesem Feld wählen Sie die Erfassungsstelle aus, über die Gestellrückmeldungen den Status hochsetzen. Über die gewählte Erfassungsstelle wird die Produktionsübersicht im Dialog Übersicht Statusrückmeldung aktualisiert.
Dazu muss der Produktionsstatus ausgewählt oder über das Ordner-Symbol definiert werden.
-> Verkauf, "Übersicht Statusrückmeldung" auf Seite C-1860

**Menge > Pos. Menge zulassen (STSB, STSD, STSG, STSL, STSP)**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Wenn die produzierte Menge größer ist als die Menge der Auftragsposition, kann die produzierte Menge übernommen werden.
- Produzierte Übermengen werden nicht in den Auftrag übernommen.
- Produzierte Mengen werden in die Auftragsposition übernommen.

**Zeitwirtschaft verarbeitet STSD und STSB**
STSD- und STSB-Meldungen können über die Kapazitätsplanung (Zeitwirtschaft) verarbeitet werden.
- Die Kapazitätsplanung verarbeitet keine Daten aus den STSD- und STSB-Dateien.
- STSD- und STSB-Dateien werden von der Kapazitätsplanung verarbeitet.
Damit die Rückmeldung von A+W Production richtig verarbeitet werden können, muss im Register Lager/EK/EDI die Erfassungsstelle 700 ausgewählt werden.
-> "Erfassungsstellenzuordnung" auf Seite B-1103

**Reklamationsaufträge erstellen (STSB)**
Das Feld ist nur freigeschaltet, wenn Bruch-Rückmeldungen importiert werden.
- Reklamationsaufträge werden nicht automatisch erstellt.
- Bei einer Bruchmeldung wird automatisch ein Reklamationsauftrag erstellt. Dieser Funktion können ein Standard-Verursacher und ein Standard-Grund zugeordnet werden, die jeweils im Reklamationsauftrag überschrieben werden können.

**Verursacher**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
Sie können einen Verursacher auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird. Dieser wird unabhängig von der Einstellung in den Firmendaten > Register Archiv ausgelesen.
-> "Default Reklamationsort" auf Seite B-1108

**Grund**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
Sie können einen Reklamationsgrund auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird.

**AV-Bereich**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können dann einen AV-Bereich auswählen, aus dessen Nummernkreis die Auftragsnummer gezogen wird.

**Ziel-NV**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Nummernverwalter auswählen, in den der automatisch erstellte Reklamationsauftrag gestellt wird.

**Kostenlos**
Die Checkbox ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
- Der automatisch erstellte Reklamationsauftrag ist nicht standardmäßig kostenlos.
- Der automatisch erstellte Reklamationsauftrag ist standardmäßig kostenlos. Die Einstellung kann in dem Reklamationsauftrag überschieben werden.

## Firmendaten - Versand

*Stammdaten > Firma > Firmendaten > Register Versand*

*Abb. B-599 Firmendaten - Versand*

In diesem Register legen Sie die Einstellungen für die Gestellverwaltung und den Versand fest.

### Nummernkreise

**Gestellnummer Von, Bis**
Erste und letzte Nummer des Nummernkreises für Gestelle. Der Nummernkreis gilt jeweils für den aktuellen Mandanten.
Wenn Sie Gestelle für einen Mandanten sperren wollen, geben Sie in den beiden Feldern jeweils den Wert 0 und im Feld Aktuell den Wert 1 ein.

**Aktuell**
Das Feld gibt an, welche Nummer vom System zuletzt vergeben wurde.

**Ident.-Nummer von, aktuelle, bis**
Die Zahlen geben an, welche IDs für die Gestelle vergeben werden können und welche zuletzt vergeben wurde.

### Gestellbelegung

**Für Verpackungsart**
Verpackungsart, für die L-Gestellnummern vergeben werden dürfen. Das Feld betrifft das Modul L-Gestelle.

### Gestellverwaltung

Mit der Wahl der Option legen Sie fest, welche Gestellverwaltung Sie nutzen:
- **A+W Business:** Diese Option aktiviert die herkömmliche Gestellverwaltung von A+W Business.
- **AWRack:** Diese Option aktiviert die Gestellverwaltung von Rack Manager und schaltet die nachfolgenden Felder frei.

**Keine Rückschreibung von Abholbemerkungen**
Einer STSK-Rückmeldung kann eine Abholinformation mitgegeben werden.
- Die Abholinformation wird ins Bemerkungsfeld des Gestells geschrieben. Damit werden manuelle Einträge in diesem Feld überschrieben.
- Abholinformationen werden nicht zurückgeschrieben.

**AWRack-Webservice**
Vollständige Internet-Adresse für den Webservice Rack Manager.

**CommonBase-Mandant**
Standardmäßig ist der Wert 0 eingetragen und muss nur geändert werden, wenn Sie mit Rack Manager arbeiten.
Die eingetragenen Werte sind die Identifikationsnummern (ID) für die Schnittstelle CommonBase.

**CommonBase-Firmengruppe**
Standardmäßig ist der Wert 0 eingetragen und muss nur geändert werden, wenn Sie mit Rack Manager arbeiten.

**Default-AV-Bereich für Rechnungen**
Auswahl des AV-Bereichs, für den standardmäßig die Gestellrechnungen erzeugt werden. Bei der Rechnungserstellung in Rack Manager können Sie diese Einstellung überschreiben.

**Aktueller Mandant ist Default-Mandant für Rechnungen**
Sie können festlegen, ob der Mandant, für den Sie aktuell die Firmendaten einstellen, in Rack Manager als Standard hinterlegt sein soll.
- Der aktuelle Mandant ist nicht Default-Mandant.
- Der aktuelle Mandant wird in Rack Manager als Standard hinterlegt. Bei der Rechnungserstellung in Rack Manager können Sie diese Einstellung überschreiben.

### Frachtkosten

Wenn Sie mit den kalkulatorischen Frachtkosten arbeiten, können Sie eine Grenze angeben, ab der die Frachtkosten unwirtschaftlich werden.

**Krit. Frachtkostengrenze %**
Kritische Frachtkostengrenze in Prozent.
Wenn bei der Berechnung der angegebene Wert überschritten wird, werden die Zahlen im Dialog Kalkulatorische Frachtkosten in roter Schrift dargestellt.
-> Fertigung, "Frachtkosten" auf Seite E-2434

**Zuschläge / Frachterlöse**
Sie können angeben, welche Zuschläge die Frachterlöse bilden. Damit legen Sie auch fest, wie sich Frachterlöse für die Aufträge ergeben, die an den A+W Logistics Optimizer gesendet werden.

### Routenoptimierung

**A+W Logistic Optimizer**
Um mit der Routenoptimierung von A+W zu arbeiten, müssen Sie dieses Modul aktivieren.
- Der A+W Logistics Optimizer wird nicht verwendet.
- Der A+W Logistics Optimizer wird freigeschaltet.

**Versandtag verändern**
Update des Versanddatums nach Änderung im A+W Logistics Optimizer.
- Das Versanddatum beim Kunden wird nicht aktualisiert.
- Das Versanddatum beim Kunden wird nach der Bestätigung durch den A+W Logistics Optimizer im Auftragskopf aktualisiert.

**Anlieferung verändern**
Update des Anlieferungsdatums nach Änderung im A+W Logistics Optimizer.
- Das Anlieferungsdatum beim Kunden wird nicht aktualisiert.
- Das Anlieferungsdatum beim Kunden wird nach der Bestätigung durch den A+W Logistics Optimizer im Auftragskopf aktualisiert.

### MQTT

Die Einstellungen in diesem Bereich betreffen den Feedback Service für MQTT. Ein MQTT-basierter Broker dient als allgemeine Datenschnittstelle, an die sowohl Client-Systeme als auch Dienste der A+W Software GmbH angebunden werden. Damit der Feedback Service funktioniert, müssen alle Teilnehmer am Broker angemeldet sein. Ist ein Client offline, erhält er die Nachricht, sobald er wieder online ist. Um den Service zu aktivieren, klicken Sie auf die Checkbox Feedback Service für MQTT aktivieren. Es stehen Ihnen zwei Optionen zur Verfügung:

- **Lieferung:** Ist diese Checkbox aktiv, werden die Änderungen des Liefertermins an den Feedback Service und damit an den MQTT Broker weitergeleitet.
- **Versand:** Bei der Verarbeitung der Versanddaten geht es um die Rückmeldung von Auftragsdaten und deren Positionsmengen sowie die Information auf welches Gestell die Auftragspositionen zu stellen sind. Wenn die gemeldete Positionsmenge ungleich der Originalmenge ist, wird automatisch eine Teillieferung generiert und auf das gemeldete Gestell gesetzt. Ist die gemeldete Menge vollständig, muss dementsprechend keine Teillieferung erzeugt werden. Es wird lediglich die Auftragsposition dem Gestell zugeordnet.

Es kann jeweils nur eine dieser Optionen aktiviert werden.

> **Installation und Konfiguration**
> Die Installation und Konfiguration von diesem Service wird durch die A+W Software GmbH durchgeführt. Bei Interesse wenden Sie sich bitte an Ihren zuständigen Ansprechpartner.

## Firmendaten – Kapa-Planung

*Stammdaten > Firma > Firmendaten > Register Kapa-Planung*

*Abb. B-600 Firmendaten – Kapa-Planung*

In diesem Register legen Sie die Daten für die Planung von Kapazitäten fest.

> **Planwertverfahren**
> Wenn Sie die Kapazitätsplanung nutzen wollen, darf das Planwertverfahren nicht aktiviert sein. Deaktivieren Sie dazu im Register Parameter die Checkbox Automatische Einlastung ins Planwertverfahren.
> -> "Automatische Einlastung ins Planwertverfahren" auf Seite B-1078

### Kapazitätsplanung

**Version**
Bei der Wahl des Programms zur Kapazitätsplanung müssen Sie darauf achten, wie Sie Rückmeldungen aus der Produktion empfangen. Sie können eine der folgenden Einstellungen auswählen:
- **Keine:** Aufträge werden nicht an die Kapazitätsplanung übergeben. Mit dieser Einstellung können Sie sowohl die Rückmeldungen per Datei als auch die Online-Meldungen nutzen.
- **A+W Business Kapazitätsplanung:** Mit dieser Einstellung können Sie auch die Online-Meldungen nutzen.
- **A+W Capacity Planner:** Mit dieser Einstellung können folgende Daten ausgetauscht werden:
    - Auftragsinformationen, z. B. Tour.
    - Setzen des Auftragsstatus durch A+W Capacity Planner.
    - Setzen von Auftrags-Zeitkosten für Positionen und Stücklisten-Elemente durch A+W Capacity Planner.
    - Prüfung der Lagerverfügbarkeit durch A+W Capacity Planner.
    - Lagerreservierung durch A+W Capacity Planner.

> **Erforderliche Statuszuordnungen**
> Damit A+W Capacity Planner den Status `Eingelastet` und `Fehler beim Einlasten` in A+W Business vergeben kann, ist eine Statuszuordnung der Statuspunkte 38 und 39 nötig.

### Fehlermeldung aus autom. Kapazitätsplanung

Mit der Wahl der Option legen Sie fest, an wen Fehlermeldungen gesendet werden.

- **An Auftragserfasser:** Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat. Solche Fehlermeldungen beziehen sich in aller Regel auf Termine, die nicht eingehalten werden können, weil nicht genügend Kapazitäten zur Verfügung stehen. Dies ist die Standard-Einstellung.
- **An Mitarbeiter:** Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet. Wählen Sie diese Option, wenn nur ein einziger Mitarbeiter die Aufträge bearbeitet, die nicht problemlos eingelastet werden konnten.

### A+W Business-Kapazitätsplanung

**Schichtenzahl**
Anzahl der Schichten pro Tag. Die Schichtzeiten legen Sie im Modul Kapazitätsplanung im Dialog Kalender fest.
-> Kapazitätsplanung, "Kalender" auf Seite H-3127

**Fertigungsterminmodus**
Sie müssen festlegen, ob Sie mit offenen oder geschlossenen Kapazitäten arbeiten wollen.
- **Autom. Normalkapazität:** Die Einlastungen werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung.
- **Autom. volle Tage:** Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus. Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
- **Nur Aggregatwechsel:** Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet wird, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
- **Einlasten ohne Kontrolle:** Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist.

**Schichtfüllung bei Positionssplit**
Große Positionen können auf mehrere Aggregate, Schichten oder Tage verteilt werden. Dazu geben Sie an, zu wie viel Prozent die Schicht eines Aggregats durch das Splitting gefüllt werden darf, um Platz für andere Aufträge zu behalten.

**Aggregatabgleich**
Wenn Sie mit mehreren Maschinen arbeiten, die dieselben Arbeitsarten ausführen können, kann die Planung diese Maschinen auf unterschiedliche Weise berücksichtigen:
- **Automatisch:** Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **Semi-automatisch:** Das Programm bietet die alternativen Maschinen zur Auswahl an.
- **Manuell:** Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

**Einlastpriorität**
Die Prioritäten aus dem Auftrag können beim Einlasten berücksichtigt werden:
- **Standard:** Die Kapazitäten der benötigten Aggregate werden geprüft und die Aufträge werden entsprechend der eingetragenen Priorität eingelastet.
- **Niedrige Priorität:** Standardmäßig werden alle Aufträge mit niedriger Priorität eingelastet.
- **Geänderte Priorität in Auftrag übernehmen:** Wenn die Priorität beim Einlasten geändert wird, soll sie automatisch in den Auftrag zurückgeschrieben werden.

**Max. Verschiebung bei autom. Lieferterminbestimmung (Tage)**
Sie können festlegen, wie viele Tage in die Zukunft der Liefertermin automatisch gesucht werden darf.

**Einlastung von Bestellpositionen (Nur Hauptprodukte)**
Mit der A+W Business Kapazitätsplanung können Bestellartikel eingelastet werden.
- Bestellpositionen werden nicht eingelastet.
- Die Bestellpositionen werden eingelastet. Die Zeitkosten können bestimmt werden.

**Einlastung von Lagerpositionen (Nur Hauptprodukte)**
Mit der A+W Business Kapazitätsplanung können Lageartikel eingelastet werden. Somit können für solche Positionen die Zeitkosten bestimmt werden.
- Lagerpositionen werden nicht eingelastet.
- Die Lagerpositionen werden eingelastet. Die Zeitkosten können bestimmt werden.

**Einlastung von manuell erfassten Leistungspositionen (Nur Hauptprodukte)**
Mit der A+W Business Kapazitätsplanung können manuell erfasste Leistungspositionen eingelastet werden. Somit können für solche Positionen die Zeitkosten bestimmt werden.
- Manuell erfasste Leistungspositionen werden nicht eingelastet.
- Die manuell erfassten Leistungspositionen werden eingelastet. Die Zeitkosten können bestimmt werden.

**Historientabelle für Fertigmeldungen füllen**
In der Programmvariante A+W Business Pro können Fertigmeldungen in die Historie geschrieben werden.
- Die Fertigmeldungen werden nicht in die Historie geschrieben.
- Die Fertigmeldungen werden in die Historie geschrieben. Zusätzlich werden die durch eine Buchung implizit mit fertig gemeldeten Arbeitsgänge protokolliert. STSD-Rückmeldungen werden protokolliert, falls keine Verbuchung in die Kapazitätsplanung erfolgt. Die Historie kann im Modul Statistik ausgewertet und ausgedruckt werden.

**Autom. Liefertermin-Suche nach Tour**
Bei Engpässen kann automatisch nach einem neuen Liefertermin gesucht werden.
- Der nächstmögliche Termin wird als Liefertermin gewählt, unabhängig davon, ob es ein Tourentag ist oder nicht. Dies ist die Standard-Einstellung.
- Der neue Liefertermin wird nach den Tourentagen des Kunden gesucht. Bei der automatischen Einlastung wird der neue Liefertermin gewählt und in den Auftrag zurückgeschrieben.

**Auftrag nicht splitten**
Große Aufträge müssen in kleinere Positionen aufgeteilt werden, wenn der Arbeitsgang nicht für eine gesamte Position an einem Tag erledigt werden kann.
- Die Aufträge können bei der automatischen Einlastung gesplittet werden. Dies ist die Standard-Einstellung.
- Die Aufträge können nur manuell gesplittet werden. Bei der automatischen Einlastung großer Aufträge wird eine Meldung angezeigt, so dass Sie eingreifen können.

**Verkürzte Einlastprüfung bei gleichem Aufbau**
In einem Auftrag können Positionen mit gleichem Stücklistenaufbau enthalten sein, die sich nur durch die Maße unterscheiden.
- Bei jeder Position wird der gesamte Stücklistenaufbau geprüft.
- Bei gleichem Stücklistenaufbau wird von der Einlastung der vorigen Position ausgegangen, ohne die Stückliste neu zu prüfen. Dies ist die Standard-Einstellung.

**Zum Liefertermin einlasten**
Bei der automatischen Einlastung werden Aufträge standardmäßig zum Liefertermin eingelastet. Nur wenn keine Kapazitäten frei sind, wird nach einem neuen Liefertermin gesucht.
- Aufträge werden mit Lieferterminsuche eingelastet. Dies ist die Standard-Einstellung.
- Die Aufträge werden ohne Suche nach einem alternativen Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.

**Autom. Fertigmeldung berechneter Aufträge**
Aufträge können automatisch fertig gemeldet werden.
- Die Aufträge werden nicht automatisch fertig gemeldet.
- Die Aufträge werden automatisch fertig gemeldet, wenn die Rechnungen bereits geschrieben wurden. Diese Einstellung ist nur sinnvoll, wenn Sie die Produktionsübergabe nach der Rechnungserstellung anstoßen.

**Produktionsübergabe (OrderXML) mit Planungsdaten**
Bei der Produktionsübergabe können die Daten per OrderXML oder per Pool.asc übergeben werden.
- Die Daten sollen nicht in die OrderXML-Datei geschrieben werden.
- Die Daten der A+W Business-Kapazitätsplanung sollen auch in die OrderXML-Datei geschrieben werden.

**Schichtwechseltabelle verwenden**
Für den automatischen Schichtwechsel kann eine Schichtwechseltabelle verwendet werden.

**[Einstellungen]**
Öffnet den Dialog, um die Schichtenwechsel zu definieren.
-> Kapazitätsplanung, "Einstellungen Schichten" auf Seite H-3102

**Produktgruppen ohne Statusänderung**
Sie können die Erhöhung des Positionsstatus (Auftragsstatus) durch Fertigmeldungen für Produktgruppen unterdrücken. Markieren Sie dazu die gewünschten Einträge in der Liste.

**AV-Bereiche ohne Einlastung**
Sie können festlegen, dass in bestimmte AV-Bereiche nicht automatisch eingelastet wird. Das bedeutet, dass Aufträge für die markierten AV-Bereiche nur manuell eingelastet werden können.

### Einstellungen der A+W Production-Kapazitätsplanungsrückmeldungen

**Aktualisierung der Zeitkosten**
Aus A+W Capacity Planner können Zeitkosten zurückgemeldet werden.
- Zeitkosten werden nicht aktualisiert.
- Die Zeitkosten werden aktualisiert.

**Prüfung der Lagerverfügbarkeit**
Bei der Kapazitätsplanung wird geprüft, ob die benötigten Materialien im Lager ausreichend vorrätig sind.
- Die Verfügbarkeit der Lagerartikel wird nicht geprüft.
- Die Verfügbarkeit der Lagerartikel wird geprüft. Bei Unterdeckung des Lagers wird ein Task für den Auftragserfasser eingetragen. In der Lagerinfo werden die Lagerartikel farblich gekennzeichnet, die nicht in ausreichender Menge zur Verfügung stehen und daher den geplanten Liefertermin gefährden.

**Barcode Rückmeldungen**
Dateilose Rückmeldung von Fertigmeldungen können aus A+W Business Pro und dem A+W Barcodescanner eingelesen werden.
- Rückmeldungen werden nicht per Barcode eingelesen.
- Rückmeldungen zu den Scheiben werden per Barcode eingelesen. Diese Einstellung muss sowohl im bestellenden wie auch im liefernden Haus aktiviert werden.
Dazu müssen Barcodes in allen beteiligten Betrieben identisch sein. Der Barcode wird übergeben und in der Rückmeldung Complete Scheduling auch in den Auftrags zurückgeschrieben.

**Aktualisierung des Produktionsdatums**
Wenn die Kapazitätsplanung feststellt, dass das ursprüngliche Produktionsdatum nicht eingehalten werden kann, wird ein neues Datum zurückgemeldet.
- Das Produktionsdatum im Auftrag wird nicht aktualisiert.
- Durch die Rückmeldung werden die Daten für den Produktionsstart und das Produktionsende im Auftragskopf aktualisiert. Dabei wird das früheste Datum aller im Auftrag befindlichen Produkte für den Produktionsstart übernommen. Für Produktionsende wird das späteste Datum aller im Auftrag befindlichen Positionen übernommen.

**Prüfung der Wiederbeschaffungszeit für Bestellartikel**
Bei der Kapazitätsplanung wird geprüft, ob die Wiederbeschaffungszeit der benötigten Materialien ausreicht, um den Auftrag termingerecht zu produzieren.
- Die Wiederbeschaffungszeit der Lagerartikel wird nicht geprüft.
- Die Wiederbeschaffungszeit der Lagerartikel wird geprüft.

**Nicht prüfen, ob alle Positionen zurückgemeldet wurden**
Bei der Rückmeldung der Einlastung im A+W Production kann im ERP Webservice geprüft werden, ob alle notwendigen Positionen zurückgemeldet wurden.
- Die Vollständigkeit der Rückmeldung wird nicht geprüft.
- Die Vollständigkeit der Rückmeldung wird geprüft. Dabei werden auch teilgelieferte Positionen berücksichtigt. Folgende Positionen werden nicht zurückgemeldet:
  - Leistungs- oder Zuschlagspositionen.
  - Positionen mit Nummer größer oder gleich 900.
  - Artikelpositionen, falls keine Artikelübergabe aktiviert ist.
Die Prüfung berücksichtigt auch teilgelieferte Positionen.

**Lieferdatum unabhängig von Einlastung änderbar**
Das Lieferdatum von eingelasteten Aufträge kann standardmäßig nur auf ein früheres Datum verschoben werden, wenn der Status des Auftrags zuvor geändert wurde.
- Das Lieferdatum kann nur geändert werden, wenn der Auftragsstatus zurückgesetzt wird.
- Das Lieferdatum kann nach der Einlastung und dem Produktionsbeginn geändert werden.
  - Dabei wird nicht geprüft, ob dies in der Produktion noch möglich ist. Der Auftrag wird nicht automatisch storniert.
  - Wenn der Auftrag bereits an A+W Capacity Planner (EL) übergeben ist, wird ein Eintrag in die Auftragshistorie geschrieben.

**Richtung der Lieferterminaktualisierung**
Wenn das Lieferdatum geändert werden darf, können Sie festlegen, ob automatisch ein früherer oder ein späterer Liefertermin berechnet und in den Auftrag zurückgeschrieben wird.

### A+W Production-Dokumententyp bei Kapazitätsplanungsrückmeldungen auswerten

Mit der Wahl der Option legen Sie fest, wie Dokumente von A+W Business übergeben werden sollen:

- **Angebot oder Auftrag wird gesucht:** Sowohl Aufträge als auch Angebote werden an die Produktion übergeben. Bei dieser Einstellung müssen die Nummernkreise für diese Dokumente unbedingt getrennt sein.
- **Immer als Auftrag (muss bei kapazitiver Übergabe aktiv sein):** Diese Einstellung müssen Sie wählen, wenn Sie mit der OrderXML-Übergabe und A+W Capacity Planner (EL) arbeiten.

## Firmendaten – Sonstiges

*Stammdaten > Firma > Firmendaten > Register Sonstiges*

*Abb. B-601 Firmendaten – Sonstiges*

In diesem Register legen Sie die Einstellungen für den Import von Produkten der Lieferanten im standardisierten Austauschformat für Katalogdaten fest. Die Einstellungen werden vom BMECat-Import gelesen.

Außerdem legen Sie die Einstellungen für Koppelung mit MS Outlook fest.

Die automatischen Bestellungen für Dorma und der Export von Rechnungen, Lieferavis und Auftragsbestätigungen im open Trans-Format werden über den A+W Commercial Exchange Service ausgetauscht.

> **Daten- Import**
> Der Import der Daten wird über das Modul BMECat gestartet. Wenn Sie Daten von der Website von Dorma importieren wollen, müssen Sie im Register Lager/EK/EDI die URL und die Zugangsdaten eintragen.
> -> "Firmendaten – Lager/EK/EDI" auf Seite B-1096

### Einstellungen für BMECat Import

Sie können die folgenden Einstellungen für die Lieferanten festlegen, die ihre Produktkataloge im BMECat-Format liefern.

**Vorlage Artikel**
Nummer des Musterartikels, nach dem die importierten Artikel aufgebaut werden.

**Matchcode Präfix für Artikel**
Kennzeichen für den jeweiligen Lieferanten. Die Kennzeichen für die Lieferanten müssen sich voneinander unterscheiden, z. B. D. für Dorma, M. für Megla, S. für Schlechtendahl.

**Produktnummer ab**
Produktnummer, ab der Sie Produkte importieren wollen.

**Preis Jahrgang, Preis Schlüssel**
Preisjahrgang und -schlüssel, die für die Produkte des jeweiligen Lieferanten gelten.

**Varianten ab Tabellennummer**
Nummer der Preistabelle für die Farben (Varianten).

**Import von Kurzbezeichnungen, Artikel Info, Bildern**
Sie können weitere Produktdaten der jeweiligen Lieferanten importieren.
- Die Kurzbezeichnung, Artikel-Info und/oder Bilder werden nicht importiert.
- Die Kurzbezeichnung, Artikel-Info und/oder Bilder werden importiert.

### Duschen-Konfigurator

In diesem Bereich befinden sich die Zugangsdaten zu dem Duschen-Konfigurator. Bei Interesse wenden Sie sich bitte an Ihren zuständigen Ansprechpartner bei der A+W Software GmbH.

### Euler/Hermes API

In diesem Bereich befinden sich die Einstellungen für die Schnittstellen zu der Warenkreditversicherung Allianz Trade (Euler Hermes). Bei Interesse wenden Sie sich bitte an Ihren zuständigen Ansprechpartner bei der A+W Software GmbH.

### A+W iQuote

Für den Zugang aktivieren Sie die Checkbox **Aktivierung Login-page**, und füllen die Felder **Privater Schlüssel** und **Zulässige IP's** entsprechend aus. Wenn mehrere IP-Adressen Zugriff haben sollen, können Sie diese hintereinander, durch Semikolon getrennt, eingeben. **A+W iQuote Historie nur mit exaktem Status**

Einschränkung auf Dokumente, die genau den Status haben, der unter **Stammdaten > Auftrag > Statuspunkte** freigegeben wurde. Es wird nicht der Statuspunkt geprüft, sondern der Status, der diesem Statuspunkt zugeordnet ist.

- Es werden im A+W iQuote alle Dokumente des Kunden angezeigt und Stati, die nicht freigegeben sind, werden auf den nächst kleineren Status, der freigegeben ist, in der Anzeige verschoben.
- Es werden im A+W iQuote nur die Dokumente angezeigt, die dieser Statuszuordnungsfreigabe entsprechen.

Mit der Checkbox **Kein Prüfen der tangentialen Kantenqualität** steuern Sie, ob eine Überprüfung stattfinden soll oder nicht.

### Comarch/KSeF

In diesem Bereich befinden sich die Zugangsdaten zu Comarch und dem polnischen Krajowy System e-Faktur. Bei Interesse wenden Sie sich bitte an Ihren zuständigen Ansprechpartner bei der A+W Software GmbH.

### Portugiesische Zertifizierung

*Stammdaten > Firma > Firmendaten > Register Parameter > [Parameterverwaltung]*

*Abb. B-602 Portugiesische Zertifizierung*

In diesem Dialog hinterlegen Sie die Vorgaben für die portugiesische Zertifizierung.
Im Dialog Formular-/Etikettendruck können Sie für den Druckmodus Rechnungen (Aufträge) und Gutschriften digitale Signaturen erstellen.
Beim Starten des Drucks wird mit Hilfe des privaten Schlüssels im Hintergrund die Signatur erstellt, die u. a. die Rechnungsnummer und das Rechnungsdatum enthält. Im Ausdruck werden der Zertifizierungscode und 4 Stellen der Signatur dargestellt.

Der Status der Dokumente wird umgesetzt auf **Rechnung gedruckt**. Danach dürfen die Rechnungen nicht mehr verändert werden.

> **Voraussetzungen**
> Für den Rechnungsdruck muss ein Sperrstatuspunkt definiert werden. Zusätzlich muss in der Rechteverwaltung das Recht zum Ändern einer Rechnung für alle Mitarbeiter entzogen werden. Mindestens ein Benutzer muss jedoch das Recht haben, in der Dokumentenverwaltung die Rechnung zu stornieren.
> Wenn das aktuelle Dokument Teil einer Sammelrechnung ist, werden alle Dokumente dieser Sammelrechnung storniert.

**Privater Schlüssel, öffentlicher Schlüssel**
Wenn Sie den Dialog zum ersten Mal öffnen, werden der private und der öffentliche Schlüssel für die digitale Rechnungssignatur erstellt.
Diese werden beim Speichern auf dem System in dem temporären Windows-Verzeichnis des aktuellen Benutzers gespeichert und in der Datenbank abgelegt.

**Zertifizierungscode**
Der Zertifizierungscode wird von der portugiesischen Regierung zugeteilt.

> **Parameter können nicht geändert werden**
> Diese drei Parameter können nach dem Speichern nicht mehr geändert werden.

### SAFT-PT Export Parameter

Alle gedruckten Rechnungen und Gutschriften können mit Bezug auf einen bestimmten Zeitraum in eine XML-Datei exportiert werden. Diese Datei kann im Modul Dokumente über den Dialog SAFT-PT Export erstellt werden.
Dabei müssen das Geschäftsjahr, das Start- und Enddatum und der Pfad zur Datei definiert werden. Anhand des eingestellten Geschäftsjahres können auch archivierte Dokumente exportieren werden.

**Audit Dateiversion, Firmenidentifizierung, Länder-Region**
In diesen Feldern tragen Sie die entsprechenden Daten ein. Diese Daten fließen mit in die Signatur ein.
Die restlichen Felder werden aus den Systemdaten gefüllt, die bei der Installation angegeben wurden.

## Mitarbeiter

*Stammdaten > Firma > Mitarbeiter*

In diesem Dialog erfassen und pflegen Sie die Daten zu Ihren Mitarbeitern.

> **Voraussetzung**
> Mitarbeiterdaten können nur vom System-Administrator angelegt bzw. geändert werden.

Im Dialog Mitarbeiter finden Sie folgende Register:
- Mitarbeiter - Mitarbeiter
- Mitarbeiter - Spezifikation
- Mitarbeiter - Einstellungen

### Mitarbeiter - Mitarbeiter

*Stammdaten > Firma > Mitarbeiter > Register Mitarbeiter*

*Abb. B-603 Mitarbeiter*

In diesem Register tragen Sie neue Mitarbeiterdaten ein. Alle Felder mit blauer Beschriftung sind Pflichtfelder. Wenn Sie die Daten eines Mitarbeiters bearbeiten wollen, müssen Sie den entsprechenden Eintrag in der Tabelle markieren.

> **Datenschutz beachten**
> Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.

#### Identifikation

**Klarname**
Vollständiger Namen des Mitarbeiters. Er kann nach dem Speichern nicht geändert werden.
Dieser Name wird bei jeder Aktion des betreffenden Mitarbeiters in A+W Business mit gespeichert. Wir empfehlen, zur Eindeutigkeit den vollen Namen einzutragen.

**Loginname**
Namen, mit dem sich der Mitarbeiter in A+W Business anmeldet.

**Domäne**
Namen der Domäne, wenn A+W Business in einem Netzwerk installiert ist.

#### Anschrift

**Vor-/Nachname**
Namen des Mitarbeiters, wie er in der Personalakte geführt wird.

**Straße, Land/PLZ/Ort**
Anschrift des Mitarbeiters.

#### Kommunikation

**Durchwahl**
Nummer des hausinternen Apparates, unter der er normalerweise zu erreichen ist.

**Telefon 2 bis 4**
Weitere Telefonnummern, z. B. bei Außendienstmitarbeitern die Mobilnummer.

**Fax**
Nummer des Faxgerätes, über das der Mitarbeiter senden und empfangen kann.

**Mail**
E-Mail-Adresse des Mitarbeiters.

#### Übersicht

In der Übersicht sind alle Mitarbeiter aufgelistet, die in A+W Business angelegt sind.

### Mitarbeiter – Spezifikation

*Stammdaten > Firma > Mitarbeiter > Register Spezifikation*

*Abb. B-604 Mitarbeiter - Spezifikation*

In diesem Register legen Sie weitere Detaildaten des Mitarbeiters, z. B. Funktion, Anrede, Rechtegruppe.
Die Felder im Bereich Identifikation sind zum Register Mitarbeiter beschrieben.
-> "Mitarbeiter - Mitarbeiter" auf Seite B-1149

#### Zugangsberechtigungen

**Password**
Passwort, mit dem sich der Mitarbeiter in A+W Business anmeldet. Wenn Sie in den Firmendaten die Windows-Anmeldung aktiviert haben, ist die Anmeldung über ein A+W Business-eigenes Passwort nicht möglich. Für den Zugriff über A+W Business Connect müssen Sie auf jeden Fall ein Passwort eintragen.

**Ext. Kundennr.**
Das Feld wird mit dem Modul A+W Business Connect genutzt. Für alle internen Mitarbeiter steht der Eintrag auf 0 (<k.A.>).
Wenn einer Ihrer Kunden die Dokumentenerfassung über A+W Business Connect nutzen möchte, muss er als Mitarbeiter erfasst werden. In diesem Feld wählen Sie dann die Kundennummer seiner Firma aus, damit er nur die Dokumente seiner Firma ansehen kann.
Über die Rechteverwaltung können Sie die Zugriffsrechte weiter einschränken, z. B. für die Erfassung von Gutschriften.

**Gesperrt**
Ein Mitarbeiter kann für den Zugriff auf A+W Business gesperrt werden. Dies ist z. B. erforderlich, wenn ein Mitarbeiter aus dem Unternehmen ausscheidet. Die Mitarbeiterdaten können wegen der diversen Referenzen auf Dokumente u. Ä. nicht aus der Datenbank gelöscht werden.
- Der Mitarbeiter ist nicht gesperrt.
- Der Mitarbeiter ist gesperrt und kann nicht mehr auf A+W Business zugreifen. Er wird in Dokumenten jedoch weiterhin angezeigt.

#### Spezifikation

**Funktion**
Funktion, die der Mitarbeiter in Ihrer Firma einnimmt. Zur Wahl stehen alle Funktionen, die in den Stammdaten hinterlegt sind.
-> "Titel (Funktion)" auf Seite B-877

**Anreden**
Anreden, die in den Stammdaten hinterlegt sind.
-> "Anreden" auf Seite B-877

**Gruppe**
Die Mitarbeiter können Mitarbeitergruppen zugeordnet werden. Über Gruppen können bestimmte Rechte innerhalb von A+W Business einfacher gesteuert werden. Gruppen werden im Dialog Mitarbeitergruppen eingerichtet und verwaltet.
-> "Mitarbeitergruppen" auf Seite B-1155

**Geburtstag**
Geburtstag des Mitarbeiters.

#### Menü + A+W CAD Designer

**Sprache**
Sprache, in der die Menüs in A+W Business und A+W CAD Designer angezeigt werden. Dies betrifft nicht die Anzeige in den Dialogen oder Einträge in den Feldern.

#### Dokumente

**Dokumente auf Mandant einschränken**
Sie können einen Mitarbeiter einem Mandanten zuweisen.
- Der Mitarbeiter ist keinem Mandanten zugewiesen.
- Das Feld zur Auswahl des Mandanten ist freigeschaltet. Der Mitarbeiter ist dem ausgewählten Mandanten zugewiesen. Er kann nur für diesen Mandanten Dokumente erfassen und bearbeiten.

#### Ausgabe

**Drucker**
Drucker, der standardmäßig genutzt wird. Sie können einen anderen Drucker auswählen, wenn der Mitarbeiter seine Dokumente und Listen den Standarddrucker in der Regel nicht nutzen soll.

**Fax**
Faxgerät, das standardmäßig genutzt wird, z. B. Twinfax. Wenn Sie nicht mit der A+W Business-Faxlösung arbeiten, geben Sie den Standarddrucker an.

#### Zeiterfassung

**Personalnummer**
Personalnummer des Mitarbeiters. Sie dient nur zur Info und wird in A+W Business nicht ausgewertet.

#### Schnittstellen-Dienst

**Anwender für Schnittstellen-Dienst**
Für die Anmeldung (Login) am Schnittstellen-Dienst muss ein (virtueller) Anwender angelegt werden.

### Mitarbeiter – Einstellungen

*Stammdaten > Firma > Mitarbeiter > Register Einstellungen*

*Abb. B-605 Mitarbeiter - Einstellungen*

In diesem Register ordnen Sie dem Mitarbeiter einen Dokumententyp und/oder einen AV-Bereich zu.
-> Tutorial 1, "Mitarbeiterdaten anlegen" auf Seite B-461

Die Felder im Bereich Identifikation sind zum Register Mitarbeiter beschrieben.
-> "Mitarbeiter - Mitarbeiter" auf Seite B-1149

#### Erfassungsparameter

In der Übersicht werden die Dokumentenarten aufgeführt. Mit einem Klick in eines der Felder können Sie den gewünschten Mitarbeiter auswählen.

**Beschreibung**
In dieser Spalte stehen folgende Einträge zur Wahl:
- **Dokumentenart:** Mitarbeiter, dem der jeweilige Dokumententyp zugeordnet werden soll. -> "Dokumententyp" auf Seite B-1036
- **AV-Bereich:** Wenn Sie mit verschiedenen AV-Bereichen arbeiten, können Sie z. B. dem Mitarbeiter der Dokumentenerfassung auch einen AV-Bereich zuordnen. Wenn dieser Mitarbeiter z. B. einen Auftrag erfasst, wird der Auftrag dem AV-Bereich zugeordnet. Die Dokumentennummer wird dann aus dem dazugehörigen Nummernkreis gezogen. -> "Nummernkreise" auf Seite B-1028

**Allgemein**
Dokumententyp bzw. AV-Bereich, dem der Mitarbeiter zugeordnet ist. Wenn Sie einen Eintrag ausgewählt haben, werden die anderen Felder der Zeile gesperrt.
Sie können in den Feldern pro Dokumententyp nur dann einen Mitarbeiter auswählen, wenn Sie in Feld Allgemein der Eintrag `<deaktiviert>` ausgewählt ist.

**Aufträge, Bestellungen, Anfragen, Angebot, Gutschriften**
Dokumenttypen bzw. AV-Bereiche, die dem Mitarbeiter zugeordnet sind. Die Felder sind nur freigeschaltet, wenn in der Spalte Allgemein die Einstellung `<deaktiviert>` ausgewählt ist.

#### Einstellungen des gewählten Anwenders kopieren

**Ziel**
Mitarbeiter, auf den Sie die Benutzereinstellungen oder Tabelleneigenschaften kopieren möchten.

**[Benutzereinstellungen]**
Überträgt die Einstellungen des aktuellen Mitarbeiters auf einen anderen Mitarbeiter. Die Benutzereinstellungen beziehen sich auf alle Einstellungen im Menü Optionen der Auftragserfassung und den zuletzt genutzten Nummernverwalter im Modul Dokumente.

**[Tabelleneigenschaften]**
Überträgt die Dokumenten-Einstellungen des aktuellen Mitarbeiters auf einen anderen Mitarbeiter.

#### Benutzereinstellungen

**[Importieren...]**
Wenn Sie A+W Business auf eine Version aktualisiert haben, in der die Benutzereinstellungen nicht in einer INI-Datei gespeichert sind, können Sie die alten Einstellungen importieren.

## Mitarbeitergruppen

*Stammdaten > Firma > Mitarbeitergruppen*

*Abb. B-606 Mitarbeitergruppen*

In diesem Dialog legen Sie die Mitarbeitergruppen an, die Sie zur Vereinfachung der Rechteverwaltung einsetzen wollen.
-> "Mitarbeiterrechte" auf Seite B-1156

Standardmäßig sind vier Mitarbeitergruppen vordefiniert: Manager, Supervisor, Anwender, Geschäftsleitung. Diese Gruppen können mit weiteren Gruppen ergänzt werden. Jeder Mitarbeiter wird im Dialog Mitarbeiter einer Gruppe zugeordnet.
-> "Mitarbeiter - Mitarbeiter" auf Seite B-1149

**Gesperrt**
Eine Mitarbeitergruppe kann gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Mitarbeitergruppe kann zugewiesen werden.
- Die Mitarbeitergruppe ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie zugewiesen ist, wird sie jedoch weiterhin angezeigt.

## Mitarbeiterrechte

*Stammdaten > Firma > Mitarbeiterrechte*

**Zu Dialogbeschreibung:**
-> "Rechte kopieren" auf Seite B-1158

*Abb. B-607 Rechteverwaltung - Mitarbeiterrechte*

In diesem Dialog verwalten Sie die Zugriffsrechte der Mitarbeiter oder Mitarbeitergruppen.
Jeder Mitarbeiter erhält automatisch die Rechte der Gruppe, der er zugeordnet ist. Darüber hinaus können Sie einem Mitarbeiter weitere Rechte erteilen oder einzelne Rechte entziehen.
-> Tutorial 1, "Mitarbeiterrechte" auf Seite B-456

### Menü Profile

Über dieses Menü können Sie einzelne Rechte übergreifend zuweisen. Abhängig von der Option im Bereich Identifikation ist der Eintrag für Gruppe oder Mitarbeiter freigeschaltet. Folgende Einträge stehen jeweils zur Wahl:

- **Alle Programme ohne Rechte:** Für alle Programme werden Sätze angelegt und die Checkboxen Ausführen, Ändern, Einfügen und Löschen werden deaktiviert.
- **Alle Programme ausführbar:** Für alle Programme werden Sätze angelegt. Nur die Checkbox Ausführen wird aktiviert. Alle anderen werden deaktiviert.
- **Alle Programme mit allen Rechten:** In diesem Fall werden bei der betreffenden Gruppe alle Einträge gelöscht, das heißt kein Eintrag = alle Rechte.

### Menü Funktionen

Über dieses Menü können Sie Rechte kopieren oder löschen:
- **Rechte kopieren:** Öffnet den Dialog Recht kopieren.
  -> "Rechte kopieren" auf Seite B-1158
- **Rechte löschen:** Alle Rechteeinträge zu der Gruppe bzw. zu dem Mitarbeiter werden gelöscht.
  - Bei einer Gruppe bewirkt dies, dass sie alle Rechte erhält.
  - Bei einem Mitarbeiter bewirkt dies, dass er alle Rechte der Gruppe übernimmt.

### Menü Optionen

Über dieses Menü können Sie die Rechte einzelner Mitarbeiter oder Gruppen drucken. Wenn die Option deaktiviert ist, werden immer alle Mitarbeiter und Gruppen gedruckt.

### Identifikation, Programmauswahl

Mit der Wahl der Option legen Sie fest, ob Sie die Rechte einer Gruppe, eines Mitarbeiters oder eines Programmpunkts bearbeiten wollen.
- **Gruppe:** Das Feld zur Auswahl der Gruppe wird freigeschaltet. Wenn Sie keine Gruppe auswählen, werden in der Übersicht alle Gruppen aufgelistet.
- **Mitarbeiter:** Das Feld zur Auswahl des Mitarbeiters wird freigeschaltet. Wenn Sie keinen Mitarbeiter auswählen, werden in der Übersicht alle Mitarbeiter und Gruppen aufgelistet.
- **Programm:** Das Feld zur Auswahl des Programms wird freigeschaltet. Wenn Sie kein Programm auswählen, werden in der Übersicht alle Programme aufgelistet.

**Subrechte**
Anzeige des Unterprogramms, zu dem abweichende Rechte eingeräumt sind oder werden sollen.

> **Beispiel**
> Ein Mitarbeiter hat im Auftrag das Recht Ändern.
> Die Einkaufspreise und Rabatt/Auftrag darf er nicht verändern. Für diese Unterprogramme können Sie dieses Recht entziehen.

### Rechte

Folgende Rechte können aktiviert bzw. deaktiviert werden:
- **Ändern:** Daten dürfen bearbeitet werden.
- **Einfügen:** Neue Datensätze dürfen angelegt werden.
- **Löschen:** Datensätze dürfen gelöscht werden.
- **Ausführen/Lesen:** Der Dialog darf geöffnet werden.

> **Recht zum Ändern mit Recht zum Ausführen kombinieren**
> Soll ein Mitarbeiter das Recht zum Ändern von Daten haben, muss er unbedingt auch das Recht haben, den entsprechenden Dialog auszuführen. Ohne das Recht zum Ausführen kann er den Dialog nicht öffnen, selbst wenn er darin ändern und löschen darf.

### Übersicht

In der Übersicht sind alle vergebenen Rechte angezeigt, die den Auswahlkriterien entsprechen.

## Rechte kopieren

*Stammdaten > Firma > Mitarbeiterrechte > Menü Funktionen*

*Abb. B-608 Mitarbeiterrechte kopieren*

In diesem Dialog übertragen Sie die Rechte eines Mitarbeiters oder einer Gruppe auf einen (anderen) Mitarbeiter oder eine (andere) Gruppe.

**Quelle, Ziel**
Mit der Wahl der Option legen Sie fest, aus welcher Quelle (Datensatz) die Rechte auf welches Ziel übertragen werden sollen.

**Vorhandene Rechte des Ziels löschen**
Die Rechte des Ziels können überschrieben oder ergänzt werden.
- Die Rechte der Zielgruppe oder des Mitarbeiters werden durch die Rechte der Quelle überschrieben und ggf. durch zusätzliche Rechte ergänzt.
- Die bestehenden Rechte der Zielgruppe oder des Mitarbeiters werden gelöscht und durch die Rechte aus der Quelle ersetzt.

## Statusverwaltung pro Mitarbeitergruppe

*Stammdaten > Firma > Statusverwaltung pro Mitarbeiter(gruppe)*

*Abb. B-609 Statusverwaltung pro Mitarbeiter(gruppe)*

In diesem Dialog definieren Sie die Statusbereiche für einen der Dokumententypen Angebot, Auftrag, Gutschrift, Anfrage oder Bestellung pro Mitarbeiter oder Mitarbeitergruppe festlegen. Die Einstellungen werden bei einer manuellen Statusänderung abgefragt.
Wenn der Status des aktuellen Dokuments in einem der angegebenen Statusbereiche liegt, darf der angemeldete Mitarbeiter den Status ändern.

### Identifikation

Mit der Wahl der Option legen Sie fest, für welche Mitarbeitergruppe oder für welchen Mitarbeiter die Zuordnungen gelten soll:
- **Gruppe:** Die Einstellungen gelten für die Mitarbeiter der gewählten Mitarbeitergruppe.
- **Mitarbeiter:** Die Einstellungen gelten nur für den gewählten Mitarbeiter.

### Dokumententyp

Dokumententyp, dem die Statusbereiche zugeordnet sind.

### Statusbereich Zuordnung

**Bereiche 1, 2, 3, 4 (von - bis)**
Auswahl des Anfangs- und End-Status, in dem der Status des Dokuments manuell geändert werden kann.

### Übersicht

In der Übersicht werden alle Zuordnungen angezeigt, die den aktuellen Filtereinstellungen entsprechen.

## AV-Bereiche

*Stammdaten > Firma > AV-Bereiche*

*Abb. B-610 AV-Bereiche*

In diesem Dialog definieren Sie die AV-Bereiche und ordnen diesen die entsprechenden Geschäftsarten und Dokumententypen zu. Die Angaben werden in den Dokumenten angezeigt und können überschrieben werden.
Der AV-Bereich dient auch als Sortierkriterium in der A+W Business-Umsatzstatistik.
Den AV-Bereichen können Mitarbeiter zugeordnet werden. Außerdem können Sie zu jedem AV-Bereich eigene Nummernkreise einrichten.
-> "Nummernkreise" auf Seite B-1028
-> "Mitarbeiter - Einstellungen" auf Seite B-1153

### Übersicht

**Bezeichnung**
Namen des AV-Bereichs, z. B. Isolierglasfertigung, ESG-Fertigung.
**Geschäftsart**
Geschäftsart des AV-Bereiches, die in der Dokumentenerfassung automatisch übernommen wird.
-> "Geschäftsart" auf Seite B-1024

**Dokumententyp**
Dokumententyp des AV-Bereiches, der in der Dokumentenerfassung automatisch übernommen wird.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen.

**Gesperrt**
Ein AV-Bereich kann gesperrt werden, wenn er nicht mehr benötigt wird.
- Der AV-Bereich kann zugewiesen werden.
- Der AV-Bereich ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er zugewiesen ist, wird er jedoch weiterhin angezeigt.

**Default-Lagerort**
Abweichender Lagerort, von dem der jeweilige AV-Bereich standardmäßig die benötigten Materialien bezieht.

## AD-Bereiche

*Stammdaten > Firma > AD-Bereiche*

*Abb. B-611 Außendienst-Bereiche*

In diesem Dialog legen Sie die Außendienstmitarbeiter (Vertreter) fest. Jedem Außendienstmitarbeiter können Sie anhand von Postleitzahlen oder Vorwahlnummern ein Einsatzgebiet zuweisen.
Der AD-Bereich dient als auch Sortierkriterium in der A+W Business-Umsatzstatistik.

**Außendienst**
Außendienstmitarbeiter. Zur Auswahl werden alle Mitarbeiter angezeigt, die im Dialog Mitarbeiter angelegt sind.
-> "Mitarbeiter" auf Seite B-1149

**Bemerkungen**
Zusatzinformation, z. B. Name des Gebiets.

**Von PLZ, bis PLZ**
In diesen Feldern können Sie den Bereich nach Postleitzahlen differenzieren.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Finanzbuchhaltung oder für statistische Auswertungen.

**Vorwahlbereiche**
Vorwahlnummern der Gebiete, für die der Vertreter zuständig ist.

> **Beispiel**
> Eingaben: 400 – 440, 490 – 510, 750 – 760, 789, 865, 900 – 960
>
> Bei der Erfassung eines Auftrags wird der entsprechende Vertreter automatisch herangezogen, wenn Sie im Feld Telefon eine Telefonnummer eintragen und die Vorwahl durch ein Leerzeichen oder einen Bindestrich von der Rufnummer trennen.

**Typ**
Typ, der für das Provisionssplitting herangezogen wird:
- **<k.A.>:** Dem Mitarbeiter ist kein Typ zugeordnet.
- **Vertreter 1, Vertreter 2:** Beim Provisionssplitting wird der Prozentsatz für den ausgewählten Typ herangezogen.

## Vertreterprovision

*Stammdaten > Firma > Vertreterprovision*

*Abb. B-612 Verwaltung - Vertreterprovision*

In diesem Dialog legen Sie die Details für die Standard-Provisionssätze pro Vertreter fest. Sie können zwischen unterschiedlichen Provisionsarten wählen.
Die Provision kann im Modul Statistik ausgewertet werden.

### Menü Funktionen

In diesem Menü werden folgende Einträge angezeigt:
- **Provisionssätze kopieren:** Öffnet den Dialog Vertreter - Provisionssätze kopieren, um die Provisionssätze auf einen anderen Vertreter zu übertragen.
  -> "Vertreter - Provisionssätze kopieren" auf Seite B-1166
- **Alle Provisionssätze löschen:** Löscht alle Provisionssätze.

### Auswahl Vertreter / Warengruppe

**Jahrgang, Schlüssel**
Die Provision kann nach verschiedenen Preislisten unterschieden werden. Wenn Sie in beiden Feldern den Eintrag <k.A.> auswählen, ist der Provisionssatz allgemein gültig.

**Vertreter**
Vertreter, für den die Angaben gelten. Sie müssen für jeden Vertreter und mindestens für jede Warenhauptgruppe (WHG) einen Provisionssatz anlegen.

**Gültigkeit bis**
Datum, bis zu dem der Provisionssatz gültig ist.

**Kunde**
Der Provisionssatz kann für alle Kunden oder nur für einen einzelnen Kunden gelten:
- 0: Die Vertreterprovision gilt für alle Kunden.
- 1-9999999: Die Vertreterprovision ist auf diesen Kunden beschränkt.

**WGR**
Der Provisionssatz kann für eine Warengruppe (WHG, WOG, WGR) gelten. Sie sollten mindestens einen Satz pro WHG und pro Vertreter anlegen.

**Produkt**
Der Provisionssatz kann für alle Produkte oder nur für ein bestimmtes Produkt gelten:
- 0: Die Vertreterprovision gilt für alle Produkte.
- 1-9999999: Die Vertreterprovision ist auf dieses Produkt beschränkt.

### Provisionsart

Provision wird auf bestimmt Kennziffern vergeben, z. B. auf den Umsatz. Mit der Wahl der Option legen Sie diese Berechnungsgrundlage für die Provision fest:

- **Rabatt %:** Rabatt-Wert in Prozent. Bei dieser Einstellung bietet sich z. B. eine Staffelung an, nach der ein Vertreter mehr Provision erhält, wenn der Rabatt geringer ist.
- **Deckungsbeitrag %:** Deckungsbeitrag in Prozent (Deckungsbeitrag = Umsatz Verkauf - Eigenkosten). Bei dieser Einstellung bietet sich z. B. eine Staffelung an, nach der ein Vertreter umso mehr Provision erhält, je höher der Deckungsbeitrag ist.
- **Umsatz:** Umsatzbetrag. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.
- **Deckungsbeitrag:** Betrag des Deckungsbeitrags. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.
- **Preis/PE:** Preis pro Preiseinheit. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.

**Staffelmenge**
Menge, nach der Sie die Provision staffeln wollen.

**Beispiel**

| Menge | % Provision |
| :--- | :--- |
| 20 | 0,500 |
| 100 | 0,750 |
| 9999 | 1,250 |

Bei Auswahl der Provisionsart nach Umsatz: 13-stelliges numerisches Feld.

**Provision %**
Prozentsatz, der zur Berechnung der Provision herangezogen wird. 8-stelliges numerisches Feld.
Die Eingabe eines negativen Wertes mit bis zu 4 Nachkommastellen ist möglich. Mit einem negativen Wert würde die Provision reduziert.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung.

**Gültigkeit ab**
Datum, ab dem der Provisionssatz gültig ist.

### Übersicht

In der Übersicht werden die Felder mit den Werten angezeigt, die zur Definition des Provisionssatzes gefüllt wurden. Zusätzlich müssen Sie in den folgenden Spalten Angaben zur Berechnung der Provision machen.

## Vertreter - Provisionssätze kopieren

*Stammdaten > Firma > Vertreterprovision > Menü Funktionen > Provisionssätze kopieren*

*Abb. B-613 Provisionssätze kopieren*

In diesem Dialog übertragen Sie die Provisionssätze eines Vertreters auf einen anderen.

### Quelle, Ziel

**Vertreter**
Wenn Sie in beiden Feldern denselben Vertreter auswählen, können Sie seine bisherigen Provisionssätze kopieren und dabei mit anderen Jahrgängen, Schlüsseln und mit einem neuen Gültigkeitsdatum speichern, um anschließend die Staffelmengen und Prozentangaben zu bearbeiten.

**Jahrgang, Schlüssel**
Preislisten der Quelle und des Ziels.

**Kunde**
Kunden, auf den die Provisionssätze beschränkt sind.

**Gültigkeitsdatum, Vorgabe Gültigkeitsdatum**
Gültigkeitsdatum, ab dem die Provision in der neuen Form berechnet werden soll. Für das Ziel können Sie ein Datum in der Zukunft wählen.

**Ziel überschreiben**
Die Provisionssätze des Ziels können überschrieben oder ergänzt werden.
- Die Provisionssätze des Vertreters werden durch die Provisionssätze der Quelle überschrieben und ggf. durch zusätzliche Provisionssätze ergänzt.
- Die bestehenden Provisionssätze des Vertreters werden gelöscht und durch die Provisionssätze aus der Quelle ersetzt.

## Banken

*Stammdaten > Firma > Banken*

*Abb. B-614 Banken*

In diesem Dialog tragen Sie die firmeneigenen Bankverbindungen ein. Sie können mehrere Konten pro Mandant bei unterschiedlichen Bankverbindungen hinterlegen. Nur die Banken können angegeben werden, die im Dialog Banken hinterlegt sind.
-> "Banken" auf Seite B-1044

**Mandant**
Mandant, dessen Banken in der Übersicht angezeigt werden.

### Bankverbindung

**BLZ/BIC**
Bankleitzahl und BIC (Business Identifier Code). Über die Lupe können Sie nach der gewünschten Bank suchen.
Über den Ordner können Sie weitere Bankdaten hinterlegen oder die vorhandenen ergänzen.

**Name, Sitz**
Namen und Standort der Bank werden automatisch angezeigt.

**Konto**
Kontonummer des Mandanten.

**Hauptbank**
Wenn Sie mehrere Konten für einen Mandanten eingetragen haben, müssen Sie einen Eintrag als Hauptbank kennzeichnen.
- Die Daten des aktuell angezeigten Kontos sind nicht als Hauptbank gekennzeichnet.
- Die Daten des aktuell angezeigten Kontos sind als Hauptbank gekennzeichnet.

**IBAN**
International Bank Account Number zum angegebenen Konto.

### Banken

In der Übersicht werden alle Bankverbindungen des aktuellen Mandanten angezeigt.

## Filialen

*Stammdaten > Firma > Filialen*

*Abb. B-615 Filialen*

In diesem Dialog pflegen Sie Filialen Ihrer Mandanten. Die Daten dienen nur zur Information.

### Anschrift

**Name**
Namen der Filiale, so wie sie im Handelsregister angegeben ist oder offiziell bezeichnet wird.

**Straße**
Adresse der Filiale.

### Kommunikation

**Telefon 1-4, Fax, Mail**
Telefonnummern, Faxnummer und E-Mail-Adresse der Filiale.

### Übersicht

In der Übersicht werden alle Filialen für den jeweils ausgewählten Mandanten angezeigt.

## Buchungsperioden

*Stammdaten > Firma > Buchungsperioden*

*Abb. B-616 Buchungsperioden*

In diesem Dialog tragen Sie die Buchungsperioden ein. Die Einträge werden bei der Übergabe an Ihr FiBu-Programm geprüft.
Damit Aufträge, Bestellungen und Gutschriften zum gewünschten Zeitpunkt automatisch übergeben werden, definieren Sie unterschiedliche Buchungsperioden. Auslöser für die Übergabe ist der von Ihnen jeweils festgelegte Status.
Wenn das eingetragene Datum z. B. für Aufträge erreicht ist, kann kein Auftrag mehr in diese Buchungsperiode übergeben werden.

**Abgeschlossene Buchungsperiode**
Datum, an dem die Buchungsperiode abgeschlossen ist. Für die Prüfung der Dokumente ist immer nur das Datum relevant, das dem aktuellen Datum am nächsten ist.

**Auftrag, Gutschrift, Bestellung**
Die Buchungsperiode gilt nur für den jeweils markierten Typ.
- Die Buchungsperiode gilt nicht.
- Die Buchungsperiode gilt für diesen Dokumententyp.

## Produktzuordnung Zuschläge

*Stammdaten > Firma > Produktzuordnung Zuschläge*

*Abb. B-617 Produktzuordnung Zuschläge*

In diesem Dialog verwalten Sie Ihre Sonderrabatte und Teuerungszuschläge. Zusätzlich zu den hinterlegten Teuerungszuschlägen existieren zehn Sonderrabatte, die Sie entweder als Sonderrabatte oder Teuerungszuschläge nutzen können, z. B. Zuschläge für Transport-/Mautkosten, L-Gestelle.

> **Zuschlagsprodukt**
> Jeder Zuschlag oder Sonderrabatt, der wie ein Produkt erfasst werden soll, muss als Produkt angelegt sein.

### Zuordnung

**Mandant**
Mandant, für den die Zuschläge gelten.

**Allgemein, Kunde**
Mit der Wahl der Option legen Sie fest, ob der Zuschlag für alle Kunden oder nur für einen bestimmten gilt. Die entsprechenden Eingabefelder werden freigeschaltet.

**Zuschlag**
Zur Auswahl werden die hinterlegten Zuschläge und Sonderrabatte angeboten.
-> Tutorial 1, "Verfügbare Teuerungszuschläge/Sonderrabatte" auf Seite B-397
-> Tutorial 1, "Automatischen Zuschlag definieren" auf Seite B-399

**Produkt**
Produkt, mit dem der Zuschlag oder der Rabatt berechnet werden soll. Als Produktbezeichnung wird die Bezeichnung 1 aus der Produktverwaltung angezeigt. Diese wird auch in der Produkt- und Kundenverwaltung im Bereich Zuschläge/Rabatte anwenden angezeigt.

**Gültig von - bis**
Zeitraum, in dem der Rabatt bzw. Zuschlag gültig sein soll.

**Position im Dokument**
Mit der Positionsnummer wird die Reihenfolge angegeben, in der die Sonderrabatte bzw. Teuerungszuschläge als Position im Dokument eingefügt werden. Sie bestimmen damit auch die Berechnungsreihenfolge. Die Nummern können mehrfach vergeben werden.
- **0:** Positionsbezogene Sonderrabatte oder Teuerungszuschläge werden mit Position 0 definiert, z. B. Struktur innen-Zuschlag, Zuschlag bei Überschreitung der maximalen Fläche.
- **950-999:** Die Sonderrabatte oder Teuerungszuschläge, die auf alle vorherigen oder Teile der vorherigen Positionen wirken, werden mit einer Positionsnummer zwischen 950 und 999 definiert.
- Beim Mindermengenzuschlag werden alle Positionen mit demselben Mindermengenzuschlag (Produkt) geprüft und für alle zusammen eine Zuschlagsposition eingefügt. Als Positionsnummer muss eine Zahl eingetragen werden zwischen der Null (0), die sich auf eine einzelne Position bezieht, und 900, die am Ende des Dokuments eingefügt werden.

> **Anlieferpauschale bei Abholung**
> Damit bei der Tour Abholung die Anlieferpauschale nicht automatisch während der Dokumentenerfassung eingefügt wird, muss in der Tourenverwaltung bei dieser Tour die Checkbox `ohne Lief.Pausch.` aktiviert sein.
> -> "Touren" auf Seite B-995

### Zuschlagszuordnung

In der Übersicht werden alle Zuschläge aller Mandanten aufgeführt.
Wenn Sie einen Eintrag markieren, können Sie die Werte in den freigeschalteten Feldern überschreiben.

## Formeln

*Stammdaten > Firma > Formeln*

*Abb. B-618 Formelverwaltung*

In diesem Dialog sind alle Formeln hinterlegt, mit denen Sie bestimmte Aufgaben in A+W Business automatisieren können. Im Register Formel wird jeweils die Syntax der Formel angezeigt, die im Register Tabelle markiert ist.
Über die Auswahl im Feld Typ können Sie die Anzeige einschränken. Das bedeutet, nur bestimmte Formeln werden in der Regelerfassung der iTOE angezeigt. Dies erhöht die Übersichtlichkeit bei der Formelauswahl und erleichtert es Ihnen, die richtige Formel zu Regel hinzuzufügen. Damit wird wird verhindert, dass eine Formel ausgeführt wird und diese dann einen Fehler wirft, da sie im falschen Kontext ausgeführt wird. Alle Formeln stehen zunächst auf Standard, somit ist keine Formel mehr in den Regeln verfügbar. Hier muss im der Formelverwaltung zunächst manuell eine Typisierung erfolgen

> **Formel einfügen oder bearbeiten**
> Wenn Sie weitere Formeln benötigen oder eine Formel anpassen müssen, wenden Sie sich bitte an die A+W Software GmbH.

### Menü Optionen

Über dieses Menü können Sie die Prüfung der Formel während der Eingabe aktivieren. Fehler werden beim Speichern angezeigt.

## Schnittstellen-Dienst

*Stammdaten > Firma > Schnittstellen-Dienst*

In diesem Dialog definieren Sie die Schnittstellen, über die Daten zwischen A+W Business und anderen Programmen ausgetauscht werden sollen.

Im Dialog Schnittstellen-Dienst finden Sie folgende Register:
- Schnittstellen-Dienst - Einstellungen A+W Production-Formate
- Schnittstellen-Dienst – Einstellungen weitere Formate
- Schnittstellen-Dienst - Optionen

### Schnittstellen-Dienst – Einstellungen A+W Production-Formate

*Stammdaten > Firma > Schnittstellen-Dienst > Register Einstellungen A+W Production-Formate*

*Abb. B-619 Produktionsrückmeldungen – Einstellungen A+W Production-Formate*

In diesem Register wählen Sie die Rückmeldungen aus, die Sie von A+W Production per Datei empfangen und einlesen wollen.
Wenn STSP-, STSL-, STSD-, STSB-, STSG-Dateien für die Rückmeldungen genutzt werden, muss im Bereich Auftrag produziert bei eine Erfassungsstelle ausgewählt werden, die einem Statuspunkt zugewiesen ist. Wenn eine solche Erfassungsstelle nicht zugewiesen wurde, erzeugt die Rückmeldung einen Fehler.
Die Erfassungsstellen werden im Dialog Erfassungsstellen Produktion hinterlegt.
-> "Erfassungsstellen Produktion" auf Seite B-1004

> **Gesperrte Felder**
> Die Felder sind gesperrt, wenn im Register Einstellungen weitere Formate die Checkbox Import von Produktionsrückmeldungen aktiviert ist. Sie können dann keine Einstellungen für A+W Production-Formate festlegen.

#### Identifikation

**Einstellungen für**
Mitarbeiter, für den die Einstellungen gelten. Wenn die Einstellungen für alle Benutzer gelten sollen, wählen Sie den Eintrag Administrator. Bei dieser Einstellung muss im Bereich Auftrag produziert bei dieselbe Erfassungsstelle ausgewählt sein, wie in den Firmendaten > Register Lager / EK / EDI.

#### A+W Production-Formate

In diesem Bereich wählen Sie aus, welche Rückmeldungen aus A+W Production eingelesen werden sollen. Das Verzeichnis für die Rückmeldedatei können Sie dann im jeweils freigeschalteten Feld angeben. Dieselben Verzeichnisse müssen in A+W Production angegeben werden, damit die Dateien korrekt gespeichert werden. Die Dateien werden über den A+W Commercial Exchange Service eingelesen.

**Import von Produktionsrückmeldungen**
Die STSP-Rückmeldung erfolgt überwiegend pro Stück. Sie können für die entsprechende Erfassungsstelle einstellen, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
- Rückmeldedateien aus der Produktion werden nicht eingelesen.
- Die Rückmeldung aus der Produktion wird als STSP-Datei gesendet. Der Auftragsstatus, das Produktionsdatum und die Kopf- bzw. Positionslaufnummer werden aktualisiert.

**Prod.freigabe Auftrag, falls Subauftrag produziert**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden.
Zu einem Auftrag kann ein Teilauftrag erfasst sein. Wenn eine Produktionsrückmeldung einen solchen Subauftrag betrifft, kann der Status des Gesamtauftrags umgesetzt werden.
- Ein Auftrag wird nicht automatisch auf den Status zur Produktionsfreigabe gesetzt.
- Wenn die Subaufträge als produziert zurückgemeldet werden, erhöht sich der Status des Hauptauftrags automatisch auf Produktionsfreigabe.

**Laufnummer aus dem Auftragskopf übernehmen**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden.
Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der A+W Business-Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
- Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
- Nach der Aktualisierung des Auftragskopfes erhalten alle Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für `produziert` ist.
  -> "Erfassungsstellenzuordnung" auf Seite B-1103

**Import von Planungsrückmeldungen**
Aus der Produktion können die STSL-Daten der Grob- und Feinplanung importiert werden. Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
- Rückmeldungen aus Grob- und Feinplanung werden nicht eingelesen.
- Die Rückmeldungen aus Grob- und Feinplanung werden eingelesen. Der Auftragsstatus wird dann der angegebenen Erfassungsstelle entsprechend hoch gesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
  -> "Erfassungsstellen Produktion" auf Seite B-1004

**Import von BDE-Rückmeldungen**
Die STSD-Rückmeldung aus der Betriebsdatenerfassung (BDE) dient im A+W Business dazu, den Auftragsstatus, das Produktionsdatum und die Kopf- und/oder Positionslaufnummer zu aktualisieren.
Die Rückmeldung erfolgt überwiegend pro Stück. Sie können einstellen, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
Wenn eine Erfassungsstelle angegeben ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
- BDE-Rückmeldungen werden nicht eingelesen.
- Die BDE-Rückmeldung wird als STSD-Datei gesendet.

**Produktionsgestellnummer in Position übernehmen**
Das Feld ist nur freigeschaltet, wenn BDE-Rückmeldungen importiert werden.
Wenn in der BDE-Rückmeldung Gestellnummern zu Positionen enthalten sind, können diese in A+W Business der Position zugewiesen werden.
- Gestellnummern werden nicht in die Position übernommen.
- Die gemeldeten Gestellnummern werden in den Auftrag zurückgeschrieben und der jeweiligen Position zugeordnet.

**Import von Gestellzuordnung-Rückmeldungen**
Die STSG-Rückmeldung gibt an, welches Gestell der jeweiligen Auftragsposition zugeordnet ist und welche Mengen produziert sind. Die Gestellnummer wird auf dem Lieferschein gedruckt.
- Rückmeldungen von Gestellzuordnungen werden nicht importiert.
- Die Rückmeldung der Gestellzuordnung wird als STSG-Datei gesendet.

> **Gestell-Rückmeldung für Teillieferung**
> Bei Teillieferung besteht die Möglichkeit, die Menge der Teillieferungsposition durch die per STSG zurückgemeldete verpackte Menge bestimmen zu lassen. Dazu muss beim Kopieren des Auftrags die Option `Teillieferungsmenge > Gestellrückmeldung bei Teillieferung berücksichtigen` aktiviert werden.
> Die Menge der Teillieferungsposition ist dann mit der Gesamtmenge aus den STSG-Meldungen zur betreffenden Auftragsposition vorbelegt. Sie kann nicht mehr geändert werden.

**Update der Produktionsübersicht durch Erfassungsstelle**
Das Feld ist nur freigeschaltet, wenn Rückmeldungen von Gestellzuordnungen importiert werden.
In diesem Feld wählen Sie die Erfassungsstelle aus, über die Gestellrückmeldungen den Status hochsetzen. Über die gewählte Erfassungsstelle wird die Produktionsübersicht im Dialog Übersicht Statusrückmeldung aktualisiert.
-> Verkauf, "Übersicht Statusrückmeldung" auf Seite C-1860

**Import von Gestell-Ein-/Ausgang-Rückmeldungen**
Die STSK-Rückmeldung meldet den Status des Gestells und das jeweilige Eingangs- und Ausgangsdatum.
- Rückmeldungen zum Gestelleingang und -ausgang werden nicht importiert.
- Die Rückmeldung von Gestelleingang und -ausgang wird eingelesen. Nach einer Überprüfung, ob der Kunde und das Gestell existieren, wird die Ausgabe bzw. die Rücknahme des Gestells verbucht. Existiert das Gestell in A+W Business noch nicht, wird es mit dem Typ `<k.A.>` angelegt.

**Import von Bruch-Rückmeldungen**
Mit der STSB-Rückmeldung werden die Reklamationen und die bei der Produktion zu Bruch gegangenen Scheiben gemeldet. A+W Business kann daraus automatisch Reklamationsaufträge erstellen.
Wenn eine Erfassungsstelle angegeben ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
- Bruch-Rückmeldungen werden nicht importiert.
- Die Bruch-Rückmeldung wird als STSB-Datei gesendet.

**Reklamationsaufträge erstellen**
Das Feld ist nur freigeschaltet, wenn Bruch-Rückmeldungen importiert werden.
- Reklamationsaufträge werden nicht automatisch erstellt.
- Bei einer Bruchmeldung wird automatisch ein Reklamationsauftrag erstellt. Dieser Funktion können ein Standard-Verursacher und ein Standard-Grund zugeordnet werden, die jeweils im Reklamationsauftrag überschrieben werden können.

**Verursacher**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
Sie können einen Verursacher auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird. Dieser wird unabhängig von der Einstellung in den Firmendaten > Register Archiv ausgelesen.
-> "Default Reklamationsort" auf Seite B-1108

**Grund**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
Sie können einen Reklamationsgrund auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird.

**Kostenlos**
Die Checkbox ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
- Der automatisch erstellte Reklamationsauftrag ist nicht standardmäßig kostenlos.
- Der automatisch erstellte Reklamationsauftrag ist standardmäßig kostenlos. Die Einstellung kann in dem Reklamationsauftrag überschieben werden.

**AV-Bereich**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können dann einen AV-Bereich auswählen, aus dessen Nummernkreis die Auftragsnummer gezogen wird.

**Ziel-NV**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Nummernverwalter auswählen, in den der automatisch erstellte Reklamationsauftrag gestellt wird.

**Import von XTV-Rückmeldungen**
Mit der XTV-Rückmeldung werden die Lagermaße abgebucht, die für einen Auftrag zugeschnitten werden. Außerdem werden für Artikel mit Lagermodus kombiniert die qm-Reservierungen in den Aufträgen gelöscht.
- XTV-Rückmeldungen werden nicht importiert.
- Die Rückmeldung aus der Optimierung wird als PRODBDA*-Datei gesendet.

#### Optionen

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie Rückmeldungen importieren, zu denen weitere Angaben möglich sind.

**Menge größer Positionsmenge in STSB, STSD, STSG, STSL, STSP zulassen**
Aus der Produktion können größere Stückzahlen pro Position zurückgemeldet werden, als im Auftrag enthalten sind.
- Größere Stückzahlen pro Position werden nicht zugelassen.
- Die Meldungen können auch bei größeren Stückzahlen verarbeitet werden.

**Zeitwirtschaft verarbeitet STSD und STSB**
STSD- und STSB-Meldungen können über die Kapazitätsplanung (Zeitwirtschaft) verarbeitet werden.
- Die Kapazitätsplanung verarbeitet keine Daten aus den STSD- und STSB-Dateien.
- STSD- und STSB-Dateien werden von der Kapazitätsplanung verarbeitet.

**Erfassungsstelle STSD**
Erfassungsstelle, über die der Status umgesetzt wird, wenn die STSD-Meldung über die Kapazitätsplanung verarbeitet wird.

**Erfassungsstelle STSB**
Erfassungsstelle, über die der Status umgesetzt wird, wenn die STSB-Meldung über die Kapazitätsplanung verarbeitet wird.

#### Auftrag produziert bei

Damit ein Auftrag fertiggemeldet werden kann, müssen Sie für die Rückmeldungen eine Erfassungsstelle angeben.
Wenn die Einstellungen für alle Benutzer gelten sollen, müssen Sie dieselbe Erfassungsstelle auswählen, wie im Dialog Firmendaten.
-> "Firmendaten - Lager/EK/EDI" auf Seite B-1096

**Erfassungsstelle**
Erfassungsstelle, die bei Rückmeldungen folgende (zusätzliche) Aktionen auslösen kann:
- Im Auftrag werden das Produktionsdatum und die Laufnummer erhöht.
- Bei Produktionsaufträgen wird der Warenzugang im Lager gebucht.

### Schnittstellen-Dienst – Einstellungen weitere Formate

*Stammdaten > Firma > Schnittstellen-Dienst > Register Einstellungen weitere Formate*

*Abb. B-620 Produktionsrückmeldungen – Einstellungen weitere Formate*

In diesem Register wählen Sie die Rückmeldungen aus, die Sie aus der Betriebsdatenerfassung (BDE), von ALFERT und von der FiBu erhalten und einlesen wollen.

#### BDE- und ALFERT-Formate

> **Gesperrte Felder**
> Die Felder im Bereich BDE- und ALFERT-Formate sind gesperrt, wenn im Register Einstellungen A+W Production-Formate die Checkbox Import von Produktionsrückmeldungen aktiviert ist. Sie können dann keine Einstellungen für BDE-Formate festlegen.

**Import von Produktionsrückmeldungen**
Die Rückmeldung erfolgt überwiegend pro Stück. In A+W Business kann für die entsprechende Erfassungsstelle eingestellt werden, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
- Rückmeldedateien aus der Produktion werden nicht importiert.
- Die Rückmeldung aus der Produktion wird aus der AWB_STAT-Datei eingelesen.

**Laufnummer aus dem Auftragskopf übernehmen**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden.
- Die Laufnummer aus dem Auftragskopf kann für die Positionen übernommen werden.
- Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
- Nach der Aktualisierung des Auftragskopfes erhalten alle die Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für `produziert` ist.

**Import von Gestell-Rückmeldedateien**
Die AH_GEST.DAT-Rückmeldung meldet den Status des Gestells und das jeweilige Eingangs- und Ausgangsdatum.
- Rückmeldungen zum Gestelleingang und -ausgang werden nicht importiert.
- Rückmeldungen von Gestelleingang und -ausgang werden eingelesen.

**Import von AWPool-Dateien**
Mit der AWPool-Rückmeldung werden in A+W Business Auftragsstatus, Produktionsdatum, Kopf- und Positionslaufnummer aktualisiert. Die Zuordnung der AWPool-Status zu einem A+W Business-Status ist fest programmiert.
- AWPool-Rückmeldungen werden nicht importiert.
- AWPool-Rückmeldungen werden als POOL*.DAT-Dateien eingelesen. Das Feld `Update Produktionsdatum ab Status` wird freigeschaltet.

**Update Produktionsdatum ab Status**
Das Feld ist nur freigeschaltet, wenn AWPool-Rückmeldungen importiert werden.
- Das Produktionsdatum im Auftrag wird nicht aktualisiert.
- Das Produktionsdatum im Auftrag wird aktualisiert, wenn einer der Status eingestellt ist, die zur Wahl stehen.

#### FiBu

In diesem Bereich legen Sie die Einstellungen für die Meldung der Offenen Posten fest, die automatisiert über den A+W Commercial Exchange Service eingelesen werden.

**Import von Offen-Posten-Rückmeldungen**
Offene Posten (OP) können aus dem FiBu-Programm per Datei gemeldet werden. Dies betrifft nur die Kundenkonten.
- OP-Rückmeldungen werden nicht importiert.
- OP-Rückmeldungen werden als Datei eingelesen. Die Felder für den Ablageort, eine Sicherungs- und eine Batch-Datei werden freigeschaltet.

**Sicherungsdatei anlegen**
Das Feld ist nur freigeschaltet, wenn OP-Rückmeldungen importiert werden. Sie können dann eine zusätzliche Sicherungsdatei speichern und festlegen, wie viele Tage diese gespeichert bleibt.
- Zur OP-Rückmeldedatei wird keine Sicherungsdatei gespeichert.
- OP-Rückmeldungen sollen als Sicherung (mit Zeitstempel) zusätzlich an einem anderen Ort gespeichert werden. Die Felder zur Auswahl des Verzeichnisses und für die Vorhaltetage werden freigeschaltet.

**Vorhaltetage für Sicherungsdateien**
Das Feld wird nur freigeschaltet, wenn eine Sicherungsdatei gespeichert werden soll. Sie können eintragen, wie viele Tage diese Datei nicht überschrieben werden darf.

**Batch-Datei**
Namen der Batch-Datei, die zum Kopieren der Dateien benötigt wird.

### Schnittstellen-Dienst – Optionen

*Stammdaten > Firma > Schnittstellen-Dienst > Register Optionen*

*Abb. B-621 Produktionsrückmeldungen – Optionen*

In diesem Register legen Sie die Intervalle fest, mit denen regelmäßig nach neuen Rückmeldungen gesucht werden soll.

#### Intervall

**Standard ... Minute(n)**
Intervall für den A+W Commercial Exchange Service. Wenn Sie z. B. eine 2 eintragen, prüft der Service alle 2 Minuten, ob neue Rückmeldungen aus der Produktion vorliegen, und liest diese ein.

**OP-Rückmeldung – Minute(n)**
Intervall für die Rückmeldung der Offenen Posten (OP). Wenn Sie z. B. eine 120 eintragen, werden alle 2 Stunden neuen Rückmeldungen per Batch eingelesen.
OP-Rückmeldungen können nur importiert werden, wenn die Funktion im Register Einstellungen weitere Formate aktiviert ist.
Für die Rückmeldungen müssen Sie im Dialog Firmendaten die Checkboxen für die OP-Meldungen aktivieren.
-> "Firmendaten - FiBu" auf Seite B-1061

### Einstellungen für automatischen Mailversand

**Mailversand**
Mails eines bestimmten Absenders können automatisch an eine bestimmte Adresse gesendet werden.
- Mails nicht werden gesendet.
- Mails werden gesendet. Die Felder werden freigeschaltet.

**Server**
Name des Servers, über den der Mailversand gesteuert wird.

**Port**
Nummer des Ports für den Mailversand.

**Absender Adresse, Empfänger Adresse**
E-Mail-Adressen, die standardmäßig für verwendet werden sollen.

**Authentifizierung**
Für die Datenübertragung kann eine Authentifizierung verwendet werden.
- Die Sendebestätigung wird nicht ohne Authentifizierung gesendet.
- Für die Sendebestätigung ist Authentifizierung erforderlich. Die Felder zur Eingabe der Anmeldedaten werden freigeschaltet.

**SSL Verschlüsselung verwenden**
Secure Sockets Layer (SSL); Verschlüsselungsprogramm zur sicheren Datenübertragung im Internet.
- Die Sendebestätigung wird nicht verschlüsselt.
- Die Sendebestätigung wird nach dem SSL-Protokoll verschlüsselt.

**Benutzer, Passwort**
Anmeldedaten, mit denen der Sender sich authentifiziert.

## Customizing

*Stammdaten > Firma > Customizing*

*Abb. B-622 Customizing*

In diesem Dialog stellen Sie A+W Business und seine Funktionen auf die Bedürfnisse in Ihrem Unternehmen ein.
Sie können den Dialog nur öffnen, wenn Sie als Administrator mit den entsprechenden Rechten angemeldet sind.

> **Anpassungen einrichten**
> Mit dem Customizing greifen Sie unter Umständen tief in die Funktionen von A+W Business ein. Wenn Sie A+W Business für Ihr Unternehmen weiter anpassen wollen, setzen Sie sich bitte mit der A+W Software GmbH in Verbindung, um die Anpassungen abzustimmen.

## Datencontainer

*Stammdaten > Firma > Datencontainer*

*Abb. B-623 Customizingdaten - Datencontainer*

In diesem Dialog verwalten Sie Daten, die für das Customizing benötigt werden, mit der A+W Business-Datenbank. Die Bezeichnung der Register und der Tabellenspalten kann dabei ebenfalls konfiguriert werden.

## Texte

*Stammdaten > Texte*

In diesem Programmbereich werden die Texte und die Textkennzeichen verwaltet, die in der Dokumentenbearbeitung benötigt werden.

Im Menü Texte finden Sie folgende Einträge:
- "Textkennzeichen" auf Seite B-1188
- "Texte" auf Seite B-1189
- "Systemtexte" auf Seite B-1191
- "Mahntexte" auf Seite B-1192
- "Dateianhangs-Typen" auf Seite B-1193
- "Dateianhangs-Bemerkungen" auf Seite B-1194
- "Technische Werte" auf Seite B-1194

### Textkennzeichen

*Stammdaten > Texte > Textkennzeichen*

*Abb. B-624 Textkennzeichen*

In diesem Dialog hinterlegen Sie die Textkennzeichen. Die Textkennzeichen dienen der Zuordnung von Textblöcken zu Themenbereichen, z. B. P für Produktion, L für Lieferschein, T für allgemeine Texte. Über die Textkennzeichen können Sie steuern, welche Texte in welchen Dokumenten gedruckt werden sollen.
-> Tutorial 2, "Textarten" auf Seite B-535

**Kennzeichen**
Textkennzeichen, z. B. P für Produktionstexte, V für Terminverschiebungen.

**Bezeichnung**
Namen, z. B. Produktion für Texte, die an die Produktion übergeben werden sollen.

### Texte

*Stammdaten > Texte > Texte*

*Abb. B-625 Texte bei Mehrsprachigkeit*

In diesem Dialog erfassen Sie Standardtexte, die häufig verwendet werden, z. B. die Rahmentexte oder Texte für die Terminverschiebung. In den Texten können Platzhalter verwendet werden, die erst beim Druck eines Dokuments mit Werten gefüllt werden.
-> Tutorial 2, "Textkennzeichen und Standardtexte" auf Seite B-537
Wenn Sie mit der Mehrsprachigkeit arbeiten, müssen alle Texte auch in der jeweiligen Sprache erfasst werden. Achten Sie dabei darauf, dass die Textnummern in den Übersetzungen nicht geändert werden.
-> "Sprachen" auf Seite B-668

**Sprache**
Auswahl der Sprache, in der der Text gedruckt werden soll.

**Nummer**
Beliebige Nummer für den Text. Sie sollten die Texte pro Textkennzeichen in Nummernbereichen zusammenfassen, z. B. 1-99 für Rechnungstexte, 100 - 199 für Angebotstexte.
Wenn Sie mit dem Modul Mehrsprachigkeit arbeiten, muss zu Beginn der Erfassung der fremdsprachlichen Texte in jedem Sprachregister mindestens ein Text mit der Nummer 0 angelegt sein.

**Matchcode**
Die Eingabe des Matchcodes ist optional.

**Kennzeichen**
Über das Textkennzeichen wird der Text für den Druck zugeordnet.
Durch die Angabe des Kennzeichens L für Lieferschein können Sie z. B. Dialog Formulare steuern, ob der Text gedruckt werden soll oder nicht.

**Texttyp AWProd.**
Positionstexte werden an die Produktion übergeben, wenn das Textkennzeichen (P) für die Produktionsübergabe die Übergabe erlaubt. Für diese Texte können Sie den Texttyp (Fremdschlüssel) angeben, der in A+W Production für diese Texte genutzt wird. Ist kein Texttyp eingetragen, wird standardmäßig der Texttyp 1 übergeben.

#### Auswahl

In der Übersicht werden alle Texte angezeigt, die den Auswahlkriterien entsprechen.

#### Textbearbeitung

**Schaltflächen**
Sie können die Schriftart und -größe ändern und Hyperlinks, Bilder und Tabellen einfügen.
-> Tutorial, "Text erfassen" auf Seite C-1308

**(Eingabefeld)**
Standardtext oder Rahmentext. Bei Rahmentexten und bei bestimmten Standardtexten können Sie mit Variablen (Platzhaltern) arbeiten.
-> Tutorial 2, "Texte anlegen" auf Seite B-543

### Systemtexte

*Stammdaten > Texte > Systemtexte*

*Abb. B-626 Systemtexte*

In diesem Dialog pflegen Sie die Systemtexte. Diese Texte sind sowohl in Dialogen als auch in Formularen fest verknüpft. Sie können (sinngemäß) geändert werden, z. B. für eine andere Sprache.
-> Tutorial 2, "Systemtexte" auf Seite B-535

> **Texte nicht löschen**
> Die sinngemäße Änderung von Systemtexten ist erlaubt. Sie dürfen aber weder gelöscht noch dürfen neue hinzugefügt werden. Das Verschieben von Variablen (Platzhaltern) an eine andere Stelle im Text ist möglich.

**Sprache**
Auswahl der Sprache, in der der Text gedruckt werden soll.

**Nummer**
Anzeige der Textnummer.

**Textbearbeitung**
Sie können den Systemtext bearbeiten, z. B. in eine andere Sprache übersetzen.

#### Auswahl

In der Übersicht werden die Nummern der Systemtexte angezeigt.

### Mahntexte

*Stammdaten > Texte > Mahntexte*

*Abb. B-627 Mahntexte*

In diesem Dialog tragen Sie die Mahntexte ein, die Sie bei Mahnungen verwenden wollen. Die Texte dienen nur zur Information.
-> Verkauf, "Mahnwesen" auf Seite C-2026

**Bezeichnung**
Namen des Mahntextes.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung.

**Gesperrt**
Einen Mahntext kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
- Der Mahntext kann zugewiesen werden.
- Der Mahntext ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt und gedruckt.

### Dateianhangs-Typen

*Stammdaten > Texte > Dateianhangs-Typen*

*Abb. B-628 Typen der Dateianhänge*

In diesem Dialog tragen Sie Kennzeichen für Dateianhänge ein. Standardmäßig sind alle Anhänge mit dem Typ A (alle) gekennzeichnet und werden außer bei der Bestellübergabe immer übergeben.
Über die Kennzeichen können Sie die Übergabe von angehängten Dateien (Dokumenten, Abbildungen) steuern:
- **Produktionsübergabe:** Dateianhänge für Übergabe in OrderXML, z. B. Produktinformationen.
  -> Fertigung, "Einstellungen Produktionsübergabe - Texte/Anlagen" auf Seite E-2483
- **Dokumente kopieren:** Angebot zu Auftrag, z. B. Kalkulationsinformationen.
  -> Verkauf, "Dokumente kopieren – Texte/Anlagen" auf Seite C-1828
- **Bestellübergabe, z. B. Produktinformationen.**
  -> Verkauf, "Erweiterte Einstellungen - Allgemein" auf Seite C-1954

### Dateianhangs-Bemerkungen

*Stammdaten > Texte > Dateianhangs-Bemerkungen*

*Abb. B-629 Bemerkungen für Dateianhänge*

In diesem Dialog hinterlegen Sie Standard-Bemerkungen, die sehr oft benutzt werden. Diese Standard-Bemerkungen werden in der Auftragserfassung > Register Anlagen zur Auswahl angeboten.
-> Verkauf, "Kopfdaten - Anlagen" auf Seite C-1706

### Technische Werte

*Stammdaten > Texte > Technische Werte*

*Abb. B-630 Texte der technischen Werte für Leistungserklärungen*

In diesem Dialog hinterlegen Sie die technischen Werte für die Erzeugung von Leistungserklärungen.
Die Texte müssen für jede Sprache eingetragen werden, damit Leistungserklärung mit den entsprechende Übersetzung der Merkmale in der jeweiligen Sprache erzeugt werden können.
Diese Informationen werden nicht benötigt, wenn der Anwender bereits fertige Leistungserklärungen vorliegen.

## Formulare

*Stammdaten > Formulare*

Als Formulare werden sowohl die Ausgaben im Druck als auch auf dem Bildschirm bezeichnet. Dazu zählen neben den Dokumenten auch die Listen und Berichte (Reports).

Im Menü Formulare finden Sie folgende Einträge:
- "Formularverwaltung" auf Seite B-1195
- "Auftragsformulare" auf Seite B-1213
- "Druckaufträge" auf Seite B-1214
- "Crystal Reports" auf Seite B-1220

### Formularverwaltung

*Stammdaten > Formulare > Formularverwaltung*

In der Formularverwaltung können Sie allgemeine Einstellungen zum Formulardruck bearbeiten. Die Formulare selbst können nur von der A+W Software GmbH geändert werden.

Im Dialog Formularverwaltung finden Sie folgende Register:
- Formularverwaltung - Formular
- Formularverwaltung – Kopf-/Fußtexte
- Formularverwaltung – Texte
- Formularverwaltung - Optionen 1
- Formularverwaltung - Optionen 2
- Formularverwaltung – Skizzendruck
- Formularverwaltung – Customizing

Die Einstellungen werden für die Druckfunktionen verwendet, z. B. von Auftragsbestätigungen.
-> Verkauf, "Formular-/Etikettendruck" auf Seite C-1926

> **Anbindung an das DMS-System Algeier scanView**
> Bei dem Druckvorgang kann aus dem aktuellen Dokument eine PDF-Datei erstellt und für die DMS Archivierung an das Allgeier scanView System übertragen werden. Diese Funktionalität kann mandanten-übergreifend genutzt werden. Wenden Sie sich an die A+W Software GmbH, wenn Sie Funktionalität nutzen wollen.

### Formularverwaltung – Formular

*Stammdaten > Formulare > Formularverwaltung > Register Formular*

*Abb. B-631 Formularverwaltung - Formular*

In diesem Register legen Sie zu den einzelnen Druckpunkten fest, welche Formulare für den Druck verwendet werden. Der Druckpunkt entspricht dem Statuspunkt, der programmintern genutzt wird.
-> "Statuszuordnung" auf Seite B-1022

#### Druckpunkte

Mit der Wahl der Option legen Sie fest, ob Sie sich Kunden oder Lieferantenformulare anzeigen lassen oder ändern möchten.
- **Standard:** Die Formulare gelten allgemein.
- **Kunden, Lieferanten:** Die Formulare gelten für einen Kunden oder einen Lieferanten. Das Feld zur Auswahl des Partners wird freigeschaltet.

**Druckpunkt**
Druckpunkt, dem ein Formular zugeordnet ist. Sie können jedem Druckpunkt beliebig viele Formulare zuordnen.
Nachdem einem Formular nach der Ersterfassung ein Druckpunkt zugeordnet ist, kann dieser Druckpunkt nachträglich im Formular nicht geändert werden.
Wird z. B. eine Auftragsbestätigung mit dem Druckpunkt `100-AB Druck` gedruckt, so erhält der Auftrag automatisch den Anwenderstatus 21.

#### Formulareinstellungen

**Bezeichnung**
Ihre (firmeninterne) Bezeichnung des Formulars.

**Anzahl**
Nummer der Druckausgaben. Dabei wird jede Seite des Formulars jeweils mehrfach gedruckt. Die Anzahl der Kopien (Durchschläge) geben Sie im Register Optionen 1 an.

**Standard**
Wenn in Ihrer Firma unterschiedliche Formulare für den Druck eines Dokumentes verwendet werden, müssen Sie festlegen, welches der Formulare standardmäßig verwendet wird.
- Das Formular wird nicht standardmäßig verwendet.
- Das Formular wird standardmäßig ausgewählt, wenn Sie den entsprechenden Druck starten, z. B. eine Auftragsbestätigung für einen bestimmten Kunden.

**Sprache**
Sprache, der das markierte Formular zugeordnet ist. Dazu muss für jede Sprache je ein entsprechendes Formular angelegen sein. Diese Funktion ist nur aktiv, wenn A+W Business in der mehrsprachigen Variante installiert ist.
Jedem Kunden und allen seinen Dokumenten ist eine Sprache zugeordnet. Während des Dokumentendrucks wird das Sprachkennzeichen geprüft und für den Druck das entsprechende Formular ausgewählt. Die Texte werden in der entsprechenden Sprache gedruckt.

**Übersteuerung der Dokumentensprache**
Mit dieser Einstellung können Sie die Sprache übersteuern, die im Feld Sprache ausgewählt ist.
- Das Formular wird der gewählten Sprache entsprechend gedruckt (Standardeinstellung).
- Die gewählte Sprache wird übersteuert. Markieren Sie die Checkbox dann, wenn Sie z. B. ein Formular als Produktionspapier verwenden. In diesem Fall ist es wichtig, dass das Produktionspapier immer in Ihrer Landessprache gedruckt wird (unabhängig vom Sprachkennzeichen des Dokumentes).

#### Report

**Dateiname**
Zuordnung des Formulars zu einer Report-Datei. Ohne diese Zuordnung können die Berichte nicht erstellt werden.
Beispiele von Zuordnungen, die standardmäßig in A+W Business verwendet werden:
- Angebot = ANGEB.QRP
- Auftragsbestätigung = AUFTRAG.QRP
- Lieferschein = LIEFER.QRP
- Rechnung = RECHN.QRP
- Gutschrift = GUTSCH.QRP
- Bestellanfrage = ANFRAGE.QRP
- Bestellung = BESTELL.QRP

**Druckservice Report**
Auswahl des Druckpunkts, über den der Report erstellt wird.
Für Leistungserklärungen muss z. B. der Wert 006 – Declaration of Performance zusammen mit der zum Bericht passenden Sprache eingetragen werden. Zusätzlich kann die Übertragung an das DMS System aktiviert werden.
-> "Dokumentenarchivierung" auf Seite B-1204

**Transfer an iQuote**
Ausgegebene Formulare können auch an iQuote übergeben werden.
- Das gedruckte Formular wird nicht an iQuote übergeben.
- Das gedruckte Formular wird an iQuote übergeben.

#### Abweichender Formularstatus

**Statuspunkt**
Sie können jedem Formular einen abweichenden Statuspunkt zuordnen. Diese Zuordnung ist in der Regel nur bei einem Barverkaufsformular nötig. In diesem Fall wählen Sie den Statuspunkt Barverkauf aus.
Für den Barverkauf wird standardmäßig eine Barverkaufsrechnung gedruckt. Der Kunden zahlt bar in die Kasse. Für bar bezahlte Aufträge darf keine Rechnung gedruckt werden und die Beträge dürfen nicht an die FiBu übergeben werden.
Sollte in Ihrem System kein Statuspunkt für den Barverkauf existieren, dann legen Sie ihn bitte nur in Absprache mit der A+W Software GmbH an.

#### Leistungserklärung

**Versand per Mail**
Sie können festlegen, mit welchem Druck die Leistungserklärung gesendet werden soll.
- Beim Druck des ausgewählten Formulars wird keine Leistungserklärung gesendet.
- Beim Druck des ausgewählten Formulars wird automatisch eine Leistungserklärung per E-Mail gesendet.

#### Formulare

In der Übersicht werden alle Formulare aufgelistet, die den Auswahlkriterien entsprechen.

### Formularverwaltung – Kopf-/Fußtexte

*Stammdaten > Formulare > Formularverwaltung > Register Kopf-/Fußtext*

*Abb. B-632 Formularverwaltung – Kopf-/Fußtexte*

In diesem Register wählen Sie die Texte aus, die immer auf dem ausgewählten Formular gedruckt werden, z. B., wenn Sie auf allen Ihren Auftragsbestätigungen eine Information über Ihre nächsten Betriebsferien drucken möchten.

> **Voraussetzung**
> Der gewünschte Text muss im Dialog Texte hinterlegt sein.

Die Felder im Bereich Formulare sind zum Register Formular beschrieben.
-> "Formularverwaltung - Formular" auf Seite B-1196

#### Texte

Über die Lupe können Sie pro Kopf- und Fußtext einen der hinterlegten Text auswählen.
-> "Texte" auf Seite B-1189

**Kopftext**
Der gewählte Text wird im Formularkopf gedruckt.

**Fußtext**
Der gewählte Text wird im Formularfuß gedruckt.

### Formularverwaltung - Texte

*Stammdaten > Formulare > Formularverwaltung > Register Texte*

*Abb. B-633 Formularverwaltung - Texte*

In diesem Register tragen Sie alle Abweichungen von Standarddruck ein.
Die Felder im Bereich Druckpunkte und Formulare sind zum Register Formular beschrieben.
-> "Formularverwaltung - Formular" auf Seite B-1196

**Nicht zu druckende Textkennzeichen**
Kennzeichen der Texte, die nicht auf dem gewählten Formular gedruckt werden sollen. Auf der Auftragsbestätigung sollen z. B. keine Texte mit dem Textkennzeichen L für Lieferschein und P für Produktion gedruckt werden.
Die Einstellung betrifft immer alle Texte des gewählten Textkennzeichens. Um einzelne, ganz bestimmte Texte vom Druck auszuschließen, tragen Sie diese im Feld Variable Texte ein.
-> "Textkennzeichen" auf Seite B-1188

**Variable Texte**
Zu jedem Formular können bis zu 10 variable Texte verwaltet werden. Diese Texte werden im Formulardruck beliebig verwendet, z. B. als alternative Überschrift. Die Einstellungen können insbesondere für lieferanten- und kundenspezifische Texte verwendet werden. Die verwendeten Texte müssen in der Textverwaltung angelegt sein.
