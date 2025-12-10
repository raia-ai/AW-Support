---
description: "DE_AWBusiness_Stammdaten_9_11"
---


---
## Zum Liefertermin einlasten
Bei der automatischen Einlastung werden Aufträge standardmäßig zum Liefertermin eingelastet. Nur wenn keine Kapazitäten frei sind, wird nach einem neuen Liefertermin gesucht.
- Aufträge werden mit Lieferterminsuche eingelastet. Dies ist die Standard-Einstellung.
- Die Aufträge werden ohne Suche nach einem alternativen Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.

## Autom. Fertigmeldung berechneter Aufträge
Aufträge können automatisch fertig gemeldet werden.
- Die Aufträge werden nicht automatisch fertig gemeldet.
- Die Aufträge werden automatisch fertig gemeldet, wenn die Rechnungen bereits geschrieben wurden. Diese Einstellung ist nur sinnvoll, wenn Sie die Produktionsübergabe nach der Rechnungserstellung anstoßen.

## Produktionsübergabe (OrderXML) mit Planungsdaten
Bei der Produktionsübergabe können die Daten per OrderXML oder per Pool.asc übergeben werden.
- Die Daten sollen nicht in die OrderXML-Datei geschrieben werden.
- Die Daten der A+W Business-Kapazitätsplanung sollen auch in die OrderXML-Datei geschrieben werden.

## Schichtwechseltabelle verwenden
Für den automatischen Schichtwechsel kann eine Schichtwechseltabelle verwendet werden.

**[Einstellungen]** Öffnet den Dialog, um die Schichtenwechsel zu definieren.
⇨ Kapazitätsplanung, "Einstellungen Schichten" auf Seite H-191

## Produktgruppen ohne Statusänderung
Sie können die Erhöhung des Positionsstatus (Auftragsstatus) durch Fertigmeldungen für Produktgruppen unterdrücken. Markieren Sie dazu die gewünschten Einträge in der Liste.

## AV-Bereiche ohne Einlastung
Sie können festlegen, dass in bestimmte AV-Bereiche nicht automatisch eingelastet wird. Das bedeutet, dass Aufträge für die markierten AV-Bereiche nur manuell eingelastet werden können.

## Einstellungen der A+W Production-Kapazitätsplanungsrückmeldungen

### Aktualisierung der Zeitkosten
Aus A+W Capacity Planner können Zeitkosten zurückgemeldet werden.
- Zeitkosten werden nicht aktualisiert.
- Die Zeitkosten werden aktualisiert.

## Prüfung der Lagerverfügbarkeit
Bei der Kapazitätsplanung wird geprüft, ob die benötigten Materialien im Lager ausreichend vorrätig sind.
- Die Verfügbarkeit der Lagerartikel wird nicht geprüft.
- Die Verfügbarkeit der Lagerartikel wird geprüft. Bei Unterdeckung des Lagers wird ein Task für den Auftragserfasser eingetragen.
- In der Lagerinfo werden die Lagerartikel farblich gekennzeichnet, die nicht in ausreichender Menge zur Verfügung stehen und daher den geplanten Liefertermin gefährden.

## Barcode Rückmeldungen
Dateilose Rückmeldung von Fertigmeldungen können aus A+W Business Pro und dem A+W Barcodescanner eingelesen werden.
- Rückmeldungen werden nicht per Barcode eingelesen.
- Rückmeldungen zu den Scheiben werden per Barcode eingelesen. Diese Einstellung muss sowohl im bestellenden wie auch im liefernden Haus aktiviert werden.

Dazu müssen Barcodes in allen beteiligten Betrieben identisch sein. Der Barcode wird übergeben und in der Rückmeldung Complete Scheduling auch in den Auftrags zurückgeschrieben.

## Aktualisierung des Produktionsdatums
Wenn die Kapazitätsplanung feststellt, dass das ursprüngliche Produktionsdatum nicht eingehalten werden kann, wird ein neues Datum zurückgemeldet.
- Das Produktionsdatum im Auftrag wird nicht aktualisiert.
- Durch die Rückmeldung werden die Daten für den Produktionsstart und das Produktionsende im Auftragskopf aktualisiert. Dabei wird das früheste Datum aller im Auftrag befindlichen Produkte für den Produktionsstart übernommen. Für Produktionsende wird das späteste Datum aller im Auftrag befindlichen Positionen übernommen.

## Prüfung der Wiederbeschaffungszeit für Bestellartikel
Bei der Kapazitätsplanung wird geprüft, ob die Wiederbeschaffungszeit der benötigten Materialien ausreicht, um den Auftrag termingerecht zu produzieren.
- Die Wiederbeschaffungszeit der Lagerartikel wird nicht geprüft.
- Die Wiederbeschaffungszeit der Lagerartikel wird geprüft.

## Nicht prüfen, ob alle Positionen zurückgemeldet wurden
Bei der Rückmeldung der Einlastung im A+W Production kann im ERP Webservice geprüft werden, ob alle notwendigen Positionen zurückgemeldet wurden.
- Die Vollständigkeit der Rückmeldung wird nicht geprüft.
- Die Vollständigkeit der Rückmeldung wird geprüft. Dabei werden auch teilgelieferte Positionen berücksichtigt. Folgende Positionen werden nicht zurückgemeldet:
    - Leistungs- oder Zuschlagspositionen.
    - Positionen mit Nummer größer oder gleich 900.
    - Artikelpositionen, falls keine Artikelübergabe aktiviert ist.
Die Prüfung berücksichtigt auch teilgelieferte Positionen.

## Lieferdatum unabhängig von Einlastung änderbar
Das Lieferdatum von eingelasteten Aufträge kann standardmäßig nur auf ein früheres Datum verschoben werden, wenn der Status des Auftrags zuvor geändert wurde.
- Das Lieferdatum kann nur geändert werden, wenn der Auftragsstatus zurückgesetzt wird.
- Das Lieferdatum kann nach der Einlastung und dem Produktionsbeginn geändert werden.
    - Dabei wird nicht geprüft, ob dies in der Produktion noch möglich ist. Der Auftrag wird nicht automatisch storniert.
    - Wenn der Auftrag bereits an A+W Capacity Planner (EL) übergeben ist, wird ein Eintrag in die Auftragshistorie geschrieben.

## Richtung der Lieferterminaktualisierung
Wenn das Lieferdatum geändert werden darf, können Sie festlegen, ob automatisch ein früherer oder ein späterer Liefertermin berechnet und in den Auftrag zurückgeschrieben wird.

## A+W Production-Dokumententyp bei Kapazitätsplanungsrückmeldungen auswerten
Mit der Wahl der Option legen Sie fest, wie Dokumente von A+W Business übergeben werden sollen:
- **Angebot oder Auftrag wird gesucht:** Sowohl Aufträge als auch Angebote werden an die Produktion übergeben. Bei dieser Einstellung müssen die Nummernkreise für diese Dokumente unbedingt getrennt sein.
- **Immer als Auftrag (muss bei kapazitiver Übergabe aktiv sein):** Diese Einstellung müssen Sie wählen, wenn Sie mit der OrderXML-Übergabe und A+W Capacity Planner (EL) arbeiten.

## Firmendaten – Sonstiges
**Stammdaten > Firma > Firmendaten > Register Sonstiges**

*Abb. B-593 Firmendaten - Sonstiges*
> In diesem Register legen Sie die Einstellungen für den Import von Produkten der Lieferanten im standardisierten Austauschformat für Katalogdaten fest. Die Einstellungen werden vom BMECat-Import gelesen.
> Außerdem legen Sie die Einstellungen für Koppelung mit MS Outlook fest.
> Die automatischen Bestellungen für Dorma und der Export von Rechnungen, Lieferavis und Auftragsbestätigungen im openTrans-Format werden über den A+W Commercial Exchange Service ausgetauscht.

> **Daten- Import**
> Der Import der Daten wird über das Modul BMECat gestartet. Wenn Sie Daten von der Website von Dorma importieren wollen, müssen Sie im Register Lager/EK/EDI die URL und die Zugangsdaten eintragen.
> ⇨ "Firmendaten - Lager/EK/EDI" auf Seite B-957

### Einstellungen für BMECat Import
Sie können die folgenden Einstellungen für die Lieferanten festlegen, die ihre Produktkataloge im BMECat-Format liefern.

- **Vorlage Artikel:** Nummer des Musterartikels, nach dem die importierten Artikel aufgebaut werden.
- **Matchcode Präfix für Artikel:** Kennzeichen für den jeweiligen Lieferanten. Die Kennzeichen für die Lieferanten müssen sich voneinander unterscheiden, z. B. D. für Dorma, M. für Megla, S. für Schlechtendahl.
- **Produktnummer ab:** Produktnummer, ab der Sie Produkte importieren wollen.
- **Preis Jahrgang, Preis Schlüssel:** Preisjahrgang und -schlüssel, die für die Produkte des jeweiligen Lieferanten gelten.
- **Varianten ab Tabellennummer:** Nummer der Preistabelle für die Farben (Varianten).
- **Import von Kurzbezeichnungen, Artikel Info, Bildern:** Sie können weitere Produktdaten der jeweiligen Lieferanten importieren.
    - Die Kurzbezeichnung, Artikel-Info und/oder Bilder werden nicht importiert.
    - Die Kurzbezeichnung, Artikel-Info und/oder Bilder werden importiert.

### Outlook-Koppelung
Die Kontakte aus Outlook können mit A+W Business verknüpft werden, so dass diese Daten nicht nochmals hinterlegt werden müssen.

- **Import von Kunden, Lieferanten, Partnern:** Sie können die Microsoft-Outlook-Daten Ihrer Marktpartner importieren und so in A+W Business verfügbar machen.
    - Die Daten werden nicht importiert.
    - Die Daten können importiert werden.
- **Tausch von Name und Vorname der Markpartner, Mitarbeiter:** Sie können den Vornamen und den Nachnamen in den E-Mail-Adressen Ihrer Marktpartner oder deren Mitarbeiter beim Import der Daten tauschen, um die Darstellung anzupassen.
    - Vor- und Nachnamen werden nicht getauscht.
    - Vor- und Nachnamen werden getauscht.
- **Keine Übergabe von Marktpartnern mit fehlender Mailadresse, Telefonnummer:** Sie können den Export von Marktpartnerdaten an Outlook unterdrücken, wenn in den Daten keine E-Mail-Adressen und/oder Telefonnummern eingetragen sind.
    - Alle Daten werden exportiert.
    - Daten werden nicht exportiert, wenn E-Mail-Adressen und/oder Telefonnummern nicht vorhanden sind.
- **Alle Marktpartner übergeben (nicht nur die dem Sachbearbeiter zugeordneten):** Sie können den Export der Marktpartnerdaten davon abhängig machen, welcher Sachbearbeiter zugeordnet ist.
    - Nur die Daten werden exportiert, die dem aktuellen Sachbearbeiter zugeordnet sind.
    - Die Daten aller Marktpartner werden exportiert.

## Portugiesische Zertifizierung
**Stammdaten > Firma > Firmendaten > Register Parameter > [Parameterverwaltung]**

*Abb. B-594 Portugiesische Zertifizierung*

In diesem Dialog hinterlegen Sie die Vorgaben für die portugiesische Zertifizierung.
Im Dialog Formular-/Etikettendruck können Sie für den Druckmodus Rechnungen (Aufträge) und Gutschriften digitale Signaturen erstellen.
Beim Starten des Drucks wird mit Hilfe des privaten Schlüssels im Hintergrund die Signatur erstellt, die u. a. die Rechnungsnummer und das Rechnungsdatum enthält. Im Ausdruck werden der Zertifizierungscode und 4 Stellen der Signatur dargestellt.
Der Status der Dokumente wird umgesetzt auf Rechnung gedruckt. Danach dürfen die Rechnungen nicht mehr verändert werden.

> **Voraussetzungen**
> Für den Rechnungsdruck muss ein Sperrstatuspunkt definiert werden. Zusätzlich muss in der Rechteverwaltung das Recht zum Ändern einer Rechnung für alle Mitarbeiter entzogen werden. Mindestens ein Benutzer muss jedoch das Recht haben, in der Dokumentenverwaltung die Rechnung zu stornieren.
> Wenn das aktuelle Dokument Teil einer Sammelrechnung ist, werden alle Dokumente dieser Sammelrechnung storniert.

**Privater Schlüssel, öffentlicher Schlüssel:** Wenn Sie den Dialog zum ersten Mal öffnen, werden der private und der öffentliche Schlüssel für die digitale Rechnungssignatur erstellt.
Diese werden beim Speichern auf dem System in dem temporären Windows-Verzeichnis des aktuellen Benutzers gespeichert und in der Datenbank abgelegt.

**Zertifizierungscode:** Der Zertifizierungscode wird von der portugiesischen Regierung zugeteilt.

> **Parameter können nicht geändert werden**
> Diese drei Parameter können nach dem Speichern nicht mehr geändert werden.

### SAFT-PT Export Parameter
Alle gedruckten Rechnungen und Gutschriften können mit Bezug auf einen bestimmten Zeitraum in eine XML-Datei exportiert werden. Diese Datei kann im Modul Dokumente über den Dialog SAFT-PT Export erstellt werden.
Dabei müssen das Geschäftsjahr, das Start- und Enddatum und der Pfad zur Datei definiert werden. Anhand des eingestellten Geschäftsjahres können auch archivierte Dokumente exportieren werden.

**Audit Dateiversion, Firmenidentifizierung, Länder-Region:** In diesen Feldern tragen Sie die entsprechenden Daten ein. Diese Daten fließen mit in die Signatur ein.
Die restlichen Felder werden aus den Systemdaten gefüllt, die bei der Installation angegeben wurden.

## Mitarbeiter
**Stammdaten > Firma > Mitarbeiter**

In diesem Dialog erfassen und pflegen Sie die Daten zu Ihren Mitarbeitern.

> **Voraussetzung**
> Mitarbeiterdaten können nur vom System-Administrator angelegt bzw. geändert werden.

Im Dialog **Mitarbeiter** finden Sie folgende Register:
- Mitarbeiter - Mitarbeiter
- Mitarbeiter - Spezifikation
- Mitarbeiter - Einstellungen

### Mitarbeiter – Mitarbeiter
**Stammdaten > Firma > Mitarbeiter > Register Mitarbeiter**

*Abb. B-595 Mitarbeiter*

In diesem Register tragen Sie neue Mitarbeiterdaten ein. Alle Felder mit blauer Beschriftung sind Pflichtfelder. Wenn Sie die Daten eines Mitarbeiters bearbeiten wollen, müssen Sie den entsprechenden Eintrag in der Tabelle markieren.

> **Datenschutz beachten**
> Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.

#### Identifikation
- **Klarname:** Vollständiger Namen des Mitarbeiters. Er kann nach dem Speichern nicht geändert werden. Dieser Name wird bei jeder Aktion des betreffenden Mitarbeiters in A+W Business mit gespeichert. Wir empfehlen, zur Eindeutigkeit den vollen Namen einzutragen.
- **Loginname:** Namen, mit dem sich der Mitarbeiter in A+W Business anmeldet.
- **Domäne:** Namen der Domäne, wenn A+W Business in einem Netzwerk installiert ist.

#### Anschrift
- **Vor-/Nachname:** Namen des Mitarbeiters, wie er in der Personalakte geführt wird.
- **Straße, Land/PLZ/Ort:** Anschrift des Mitarbeiters.

#### Kommunikation
- **Durchwahl:** Nummer des hausinternen Apparates, unter der er normalerweise zu erreichen ist.
- **Telefon 2 bis 4:** Weitere Telefonnummern, z. B. bei Außendienstmitarbeitern die Mobilnummer.
- **Fax:** Nummer des Faxgerätes, über das der Mitarbeiter senden und empfangen kann.
- **Mail:** E-Mail-Adresse des Mitarbeiters.

#### Übersicht
In der Übersicht sind alle Mitarbeiter aufgelistet, die in A+W Business angelegt sind.

### Mitarbeiter – Spezifikation
**Stammdaten > Firma > Mitarbeiter > Register Spezifikation**

*Abb. B-596 Mitarbeiter - Spezifikation*

In diesem Register legen Sie weitere Detaildaten des Mitarbeiters, z. B. Funktion, Anrede, Rechtegruppe.
Die Felder im Bereich Identifikation sind zum Register Mitarbeiter beschrieben.
⇨ "Mitarbeiter - Mitarbeiter" auf Seite B-1008

#### Zugangsberechtigungen
- **Password:** Passwort, mit dem sich der Mitarbeiter in A+W Business anmeldet. Wenn Sie in den Firmendaten die Windows-Anmeldung aktiviert haben, ist die Anmeldung über ein A+W Business-eigenes Passwort nicht möglich. Für den Zugriff über A+W Business Connect müssen Sie auf jeden Fall ein Passwort eintragen.
- **Ext. Kundennr.:** Das Feld wird mit dem Modul A+W Business Connect genutzt. Für alle internen Mitarbeiter steht der Eintrag auf 0 (<k.A.>). Wenn einer Ihrer Kunden die Dokumentenerfassung über A+W Business Connect nutzen möchte, muss er als Mitarbeiter erfasst werden. In diesem Feld wählen Sie dann die Kundennummer seiner Firma aus, damit er nur die Dokumente seiner Firma ansehen kann. Über die Rechteverwaltung können Sie die Zugriffrechte weiter einschränken, z. B. für die Erfassung von Gutschriften.
- **Gesperrt:** Ein Mitarbeiter kann für den Zugriff auf A+W Business gesperrt werden. Dies ist z. B. erforderlich, wenn ein Mitarbeiter aus dem Unternehmen ausscheidet. Die Mitarbeiterdaten können wegen der diversen Referenzen auf Dokumente u. Ä. nicht aus der Datenbank gelöscht werden.
    - Der Mitarbeiter ist nicht gesperrt.
    - Der Mitarbeiter ist gesperrt und kann nicht mehr auf A+W Business zugreifen. Er wird in Dokumenten jedoch weiterhin angezeigt.

#### Spezifikation
- **Funktion:** Funktion, die der Mitarbeiter in Ihrer Firma einnimmt. Zur Wahl stehen alle Funktionen, die in den Stammdaten hinterlegt sind. (⇨ "Titel (Funktion)" auf Seite B-749)
- **Anreden:** Anreden, die in den Stammdaten hinterlegt sind. (⇨ "Anreden" auf Seite B-749)
- **Gruppe:** Die Mitarbeiter können Mitarbeitergruppen zugeordnet werden. Über Gruppen können bestimmte Rechte innerhalb von A+W Business einfacher gesteuert werden. Gruppen werden im Dialog Mitarbeitergruppen eingerichtet und verwaltet. (⇨ "Mitarbeitergruppen" auf Seite B-1014)
- **Geburtstag:** Geburtstag des Mitarbeiters.

#### Menü + A+W CAD Designer
- **Sprache:** Sprache, in der die Menüs in A+W Business und A+W CAD Designer angezeigt werden. Dies betrifft nicht die Anzeige in den Dialogen oder Einträge in den Feldern.

#### Dokumente
- **Dokumente auf Mandant einschränken:** Sie können einen Mitarbeiter einem Mandanten zuweisen.
    - Der Mitarbeiter ist keinem Mandanten zugewiesen.
    - Das Feld zur Auswahl des Mandanten ist freigeschaltet. Der Mitarbeiter ist dem ausgewählten Mandanten zugewiesen. Er kann nur für diesen Mandanten Dokumente erfassen und bearbeiten.

#### Ausgabe
- **Drucker:** Drucker, der standardmäßig genutzt wird. Sie können einen anderen Drucker auswählen, wenn der Mitarbeiter seine Dokumente und Listen den Standarddrucker in der Regel nicht nutzen soll.
- **Fax:** Faxgerät, das standardmäßig genutzt wird, z. B. Twinfax. Wenn Sie nicht mit der A+W Business-Faxlösung arbeiten, geben Sie den Standarddrucker an.

#### Zeiterfassung
- **Personalnummer:** Personalnummer des Mitarbeiters. Sie dient nur zur Info und wird in A+W Business nicht ausgewertet.

#### Schnittstellen-Dienst
- **Anwender für Schnittstellen-Dienst:** Für die Anmeldung (Login) am Schnittstellen-Dienst muss ein (virtueller) Anwender angelegt werden.

### Mitarbeiter - Einstellungen
**Stammdaten > Firma > Mitarbeiter > Register Einstellungen**

*Abb. B-597 Mitarbeiter - Einstellungen*

In diesem Register ordnen Sie dem Mitarbeiter einen Dokumententyp und/oder einen AV-Bereich zu.
⇨ Tutorial 1, "Mitarbeiterdaten anlegen" auf Seite B-390

Die Felder im Bereich Identifikation sind zum Register Mitarbeiter beschrieben.
⇨ "Mitarbeiter - Mitarbeiter" auf Seite B-1008

#### Erfassungsparameter
In der Übersicht werden die Dokumentenarten aufgeführt. Mit einem Klick in eines der Felder können Sie den gewünschten Mitarbeiter auswählen.

- **Beschreibung:** In dieser Spalte stehen folgende Einträge zur Wahl:
    - **Dokumentenart:** Mitarbeiter, dem der jeweilige Dokumententyp zugeordnet werden soll. (⇨ "Dokumententyp" auf Seite B-900)
    - **AV-Bereich:** Wenn Sie mit verschiedenen AV-Bereichen arbeiten, können Sie z. B. dem Mitarbeiter der Dokumentenerfassung auch einen AV-Bereich zuordnen. Wenn dieser Mitarbeiter z. B. einen Auftrag erfasst, wird der Auftrag dem AV-Bereich zugeordnet. Die Dokumentennummer wird dann aus dem dazugehörigen Nummernkreis gezogen. (⇨ "Nummernkreise" auf Seite B-891)

- **Allgemein:** Dokumententyp bzw. AV-Bereich, dem der Mitarbeiter zugeordnet ist. Wenn Sie einen Eintrag ausgewählt haben, werden die anderen Felder der Zeile gesperrt. Sie können in den Feldern pro Dokumententyp nur dann einen Mitarbeiter auswählen, wenn Sie in Feld Allgemein der Eintrag <deaktiviert> ausgewählt ist.
- **Aufträge, Bestellungen, Anfragen, Angebot, Gutschriften:** Dokumenttypen bzw. AV-Bereiche, die dem Mitarbeiter zugeordnet sind. Die Felder sind nur freigeschaltet, wenn in der Spalte Allgemein die Einstellung <deaktiviert> ausgewählt ist.

#### Einstellungen des gewählten Anwenders kopieren
- **Ziel:** Mitarbeiter, auf den Sie die Benutzereinstellungen oder Tabelleneigenschaften kopieren möchten.
- **[Benutzereinstellungen]:** Überträgt die Einstellungen des aktuellen Mitarbeiters auf einen anderen Mitarbeiter. Die Benutzereinstellungen beziehen sich auf alle Einstellungen im Menü Optionen der Auftragserfassung und den zuletzt genutzten Nummernverwalter im Modul Dokumente.
- **[Tabelleneigenschaften]:** Überträgt die Dokumenten-Einstellungen des aktuellen Mitarbeiters auf einen anderen Mitarbeiter.

#### Benutzereinstellungen
- **[Importieren...]:** Wenn Sie A+W Business auf eine Version aktualisiert haben, in der die Benutzereinstellungen nicht in einer INI-Datei gespeichert sind, können Sie die alten Einstellungen importieren.

## Mitarbeitergruppen
**Stammdaten > Firma > Mitarbeitergruppen**

*Abb. B-598 Mitarbeitergruppen*

In diesem Dialog legen Sie die Mitarbeitergruppen an, die Sie zur Vereinfachung der Rechteverwaltung einsetzen wollen.
⇨ "Mitarbeiterrechte" auf Seite B-1015

Standardmäßig sind vier Mitarbeitergruppen vordefiniert: Manager, Supervisor, Anwender, Geschäftsleitung. Diese Gruppen können mit weiteren Gruppen ergänzt werden. Jeder Mitarbeiter wird im Dialog Mitarbeiter einer Gruppe zugeordnet.
⇨ "Mitarbeiter - Mitarbeiter" auf Seite B-1008

**Gesperrt:** Eine Mitarbeitergruppe kann gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Mitarbeitergruppe kann zugewiesen werden.
- Die Mitarbeitergruppe ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie zugewiesen ist, wird sie jedoch weiterhin angezeigt.

## Mitarbeiterrechte
**Stammdaten > Firma > Mitarbeiterrechte**

*Abb. B-599 Rechteverwaltung – Mitarbeiterrechte*

In diesem Dialog verwalten Sie die Zugriffsrechte der Mitarbeiter oder Mitarbeitergruppen.
Jeder Mitarbeiter erhält automatisch die Rechte der Gruppe, der er zugeordnet ist. Darüber hinaus können Sie einem Mitarbeiter weitere Rechte erteilen oder einzelne Rechte entziehen.
⇨ Tutorial 1, "Mitarbeiterrechte" auf Seite B-385

### Menü Profile
Über dieses Menü können Sie einzelne Rechte übergreifend zuweisen. Abhängig von der Option im Bereich Identifikation ist der Eintrag für Gruppe oder Mitarbeiter freigeschaltet. Folgende Einträge stehen jeweils zur Wahl:
- **Alle Programme ohne Rechte:** Für alle Programme werden Sätze angelegt und die Checkboxen Ausführen, Ändern, Einfügen und Löschen werden deaktiviert.
- **Alle Programme ausführbar:** Für alle Programme werden Sätze angelegt. Nur die Checkbox Ausführen wird aktiviert. Alle anderen werden deaktiviert.
- **Alle Programme mit allen Rechten:** In diesem Fall werden bei der betreffenden Gruppe alle Einträge gelöscht, das heißt kein Eintrag = alle Rechte.

### Menü Funktionen
Über dieses Menü können Sie Rechte kopieren oder löschen:
- **Rechte kopieren:** Öffnet den Dialog Recht kopieren. (⇨ "Rechte kopieren" auf Seite B-1017)
- **Rechte löschen:** Alle Rechteeinträge zu der Gruppe bzw. zu dem Mitarbeiter werden gelöscht. Bei einer Gruppe bewirkt dies, dass sie alle Rechte erhält. Bei einem Mitarbeiter bewirkt dies, dass er alle Rechte der Gruppe übernimmt.

### Menü Optionen
Über dieses Menü können Sie die Rechte einzelner Mitarbeiter oder Gruppen drucken. Wenn die Option deaktiviert ist, werden immer alle Mitarbeiter und Gruppen gedruckt.

### Identifikation, Programmauswahl
Mit der Wahl der Option legen Sie fest, ob Sie die Rechte einer Gruppe, eines Mitarbeiters oder eines Programmpunkts bearbeiten wollen.
- **Gruppe:** Das Feld zur Auswahl der Gruppe wird freigeschaltet. Wenn Sie keine Gruppe auswählen, werden in der Übersicht alle Gruppen aufgelistet.
- **Mitarbeiter:** Das Feld zur Auswahl des Mitarbeiters wird freigeschaltet. Wenn Sie keinen Mitarbeiter auswählen, werden in der Übersicht alle Mitarbeiter und Gruppen aufgelistet.
- **Programm:** Das Feld zur Auswahl des Programms wird freigeschaltet. Wenn Sie kein Programm auswählen, werden in der Übersicht alle Programme aufgelistet.

**Subrechte:** Anzeige des Unterprogramms, zu dem abweichende Rechte eingeräumt sind oder werden sollen.

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
**Stammdaten > Firma > Mitarbeiterrechte > Menü Funktionen**

*Abb. B-600 Mitarbeiterrechte kopieren*

In diesem Dialog übertragen Sie die Rechte eines Mitarbeiters oder einer Gruppe auf einen (anderen) Mitarbeiter oder eine (andere) Gruppe.

### Quelle, Ziel
Mit der Wahl der Option legen Sie fest, aus welcher Quelle (Datensatz) die Rechte auf welches Ziel übertragen werden sollen.

### Vorhandene Rechte des Ziels löschen
Die Rechte des Ziels können überschrieben oder ergänzt werden.
- Die Rechte der Zielgruppe oder des Mitarbeiters werden durch die Rechte der Quelle überschrieben und ggf. durch zusätzliche Rechte ergänzt.
- Die bestehenden Rechte der Zielgruppe oder des Mitarbeiters werden gelöscht und durch die Rechte aus der Quelle ersetzt.

## Statusverwaltung pro Mitarbeitergruppe
**Stammdaten > Firma > Statusverwaltung pro Mitarbeiter(gruppe)**

*Abb. B-601 Statusverwaltung pro Mitarbeiter(gruppe)*

In diesem Dialog definieren Sie die Statusbereiche für einen der Dokumententypen Angebot, Auftrag, Gutschrift, Anfrage oder Bestellung pro Mitarbeiter oder Mitarbeitergruppe festlegen. Die Einstellungen werden bei einer manuellen Statusänderung abgefragt.
Wenn der Status des aktuellen Dokuments in einem der angegebenen Statusbereiche liegt, darf der angemeldete Mitarbeiter den Status ändern.

### Identifikation
Mit der Wahl der Option legen Sie fest, für welche Mitarbeitergruppe oder für welchen Mitarbeiter die Zuordnungen gelten soll:
- **Gruppe:** Die Einstellungen gelten für die Mitarbeiter der gewählten Mitarbeitergruppe.
- **Mitarbeiter:** Die Einstellungen gelten nur für den gewählten Mitarbeiter.

### Dokumententyp
Dokumententyp, dem die Statusbereiche zugeordnet sind.

### Statusbereich Zuordnung
**Bereiche 1, 2, 3, 4 (von - bis):** Auswahl des Anfangs- und End-Status, in dem der Status des Dokuments manuell geändert werden kann.

### Übersicht
In der Übersicht werden alle Zuordnungen angezeigt, die den aktuellen Filtereinstellungen entsprechen.

## AV-Bereiche
**Stammdaten > Firma > AV-Bereiche**

*Abb. B-602 AV-Bereiche*

In diesem Dialog definieren Sie die AV-Bereiche und ordnen diesen die entsprechenden Geschäftsarten und Dokumententypen zu. Die Angaben werden in den Dokumenten angezeigt und können überschrieben werden.
Der AV-Bereich dient auch als Sortierkriterium in der A+W Business-Umsatzstatistik.
Den AV-Bereichen können Mitarbeiter zugeordnet werden. Außerdem können Sie zu jedem AV-Bereich eigene Nummernkreise einrichten.
⇨ "Nummernkreise" auf Seite B-891
⇨ "Mitarbeiter - Einstellungen" auf Seite B-1012

### Übersicht
**Bezeichnung:** Namen des AV-Bereichs, z. B. Isolierglasfertigung, ESG-Fertigung.
**Geschäftsart:** Geschäftsart des AV-Bereiches, die in der Dokumentenerfassung automatisch übernommen wird.
⇨ "Geschäftsart" auf Seite B-888
**Dokumententyp:** Dokumententyp des AV-Bereiches, der in der Dokumentenerfassung automatisch übernommen wird.
**Fremdschlüssel:** Fremdschlüssel für die Kommunikation mit anderen Programmen.
**Gesperrt:** Ein AV-Bereich kann gesperrt werden, wenn er nicht mehr benötigt wird.
- Der AV-Bereich kann zugewiesen werden.
- Der AV-Bereich ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er zugewiesen ist, wird er jedoch weiterhin angezeigt.
**Default-Lagerort:** Abweichender Lagerort, von dem der jeweilige AV-Bereich standardmäßig die benötigten Materialien bezieht.

## AD-Bereiche
**Stammdaten > Firma > AD-Bereiche**

*Abb. B-603 Außendienst-Bereiche*

In diesem Dialog legen Sie die Außendienstmitarbeiter (Vertreter) fest. Jedem Außendienstmitarbeiter können Sie anhand von Postleitzahlen oder Vorwahlnummern ein Einsatzgebiet zuweisen.
Der AD-Bereich dient als auch Sortierkriterium in der A+W Business-Umsatzstatistik.

**Außendienst:** Außendienstmitarbeiter. Zur Auswahl werden alle Mitarbeiter angezeigt, die im Dialog Mitarbeiter angelegt sind.
⇨ "Mitarbeiter" auf Seite B-1008
**Bemerkungen:** Zusatzinformation, z. B. Name des Gebiets.
**Von PLZ, bis PLZ:** In diesen Feldern können Sie den Bereich nach Postleitzahlen differenzieren.
**Fremdschlüssel:** Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Finanzbuchhaltung oder für statistische Auswertungen.
**Vorwahlbereiche:** Vorwahlnummern der Gebiete, für die der Vertreter zuständig ist.

> **Beispiel**
> Eingaben: 400 – 440, 490 – 510, 750 – 760, 789, 865, 900 – 960
> Bei der Erfassung eines Auftrags wird der entsprechende Vertreter automatisch herangezogen, wenn Sie im Feld Telefon eine Telefonnummer eintragen und die Vorwahl durch ein Leerzeichen oder einen Bindestrich von der Rufnummer trennen.

**Typ:** Typ, der für das Provisionssplitting herangezogen wird:
- **<k.A.>:** Dem Mitarbeiter ist kein Typ zugeordnet.
- **Vertreter 1, Vertreter 2:** Beim Provisionssplitting wird der Prozentsatz für den ausgewählten Typ herangezogen.

## Vertreterprovision
**Stammdaten > Firma > Vertreterprovision**

*Abb. B-604 Verwaltung - Vertreterprovision*

In diesem Dialog legen Sie die Details für die Standard-Provisionssätze pro Vertreter fest. Sie können zwischen unterschiedlichen Provisionsarten wählen.
Die Provision kann im Modul Statistik ausgewertet werden.

### Menü Funktionen
In diesem Menü werden folgende Einträge angezeigt:
- **Provisionssätze kopieren:** Öffnet den Dialog Vertreter - Provisionssätze kopieren, um die Provisionssätze auf einen anderen Vertreter zu übertragen.
  ⇨ "Vertreter - Provisionssätze kopieren" auf Seite B-1024
- **Alle Provisionssätze löschen:** Löscht alle Provisionssätze.

### Auswahl Vertreter / Warengruppe
- **Jahrgang, Schlüssel:** Die Provision kann nach verschiedenen Preislisten unterschieden werden. Wenn Sie in beiden Feldern den Eintrag <k.A.> auswählen, ist der Provisionssatz allgemein gültig.
- **Vertreter:** Vertreter, für den die Angaben gelten. Sie müssen für jeden Vertreter und mindestens für jede Warenhauptgruppe (WHG) einen Provisionssatz anlegen.
- **Gültigkeit bis:** Datum, bis zu dem der Provisionssatz gültig ist.
- **Kunde:** Der Provisionssatz kann für alle Kunden oder nur für einen einzelnen Kunden gelten:
    - 0: Die Vertreterprovision gilt für alle Kunden.
    - 1-9999999: Die Vertreterprovision ist auf diesen Kunden beschränkt.
- **WGR:** Der Provisionssatz kann für eine Warengruppe (WHG, WOG, WGR) gelten. Sie sollten mindestens einen Satz pro WHG und pro Vertreter anlegen.
- **Produkt:** Der Provisionssatz kann für alle Produkte oder nur für ein bestimmtes Produkt gelten:
    - 0: Die Vertreterprovision gilt für alle Produkte.
    - 1-9999999: Die Vertreterprovision ist auf dieses Produkt beschränkt.

### Provisionsart
Provision wird auf bestimmt Kennziffern vergeben, z. B. auf den Umsatz. Mit der Wahl der Option legen Sie diese Berechnungsgrundlage für die Provision fest:
- **Rabatt %:** Rabatt-Wert in Prozent. Bei dieser Einstellung bietet sich z. B. eine Staffelung an, nach der ein Vertreter mehr Provision erhält, wenn der Rabatt geringer ist.
- **Deckungsbeitrag %:** Deckungsbeitrag in Prozent (Deckungsbeitrag = Umsatz Verkauf - Eigenkosten). Bei dieser Einstellung bietet sich z. B. eine Staffelung an, nach der ein Vertreter umso mehr Provision erhält, je höher der Deckungsbeitrag ist.
- **Umsatz:** Umsatzbetrag. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.
- **Deckungsbeitrag:** Betrag des Deckungsbeitrags. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.
- **Preis/PE:** Preis pro Preiseinheit. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.

**Staffelmenge:** Menge, nach der Sie die Provision staffeln wollen.

> **Beispiel**
> 
> | Menge | % Provision |
> | :--- | :--- |
> | 20 | 0,500 |
> | 100 | 0,750 |
> | 9999 | 1,250 |
> 
> Bei Auswahl der Provisionsart nach Umsatz: 13-stelliges numerisches Feld.

**Provision %:** Prozentsatz, der zur Berechnung der Provision herangezogen wird. 8-stelliges numerisches Feld. Die Eingabe eines negativen Wertes mit bis zu 4 Nachkommastellen ist möglich. Mit einem negativen Wert würde die Provision reduziert.
**Fremdschlüssel:** Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung.
**Gültigkeit ab:** Datum, ab dem der Provisionssatz gültig ist.

### Übersicht
In der Übersicht werden die Felder mit den Werten angezeigt, die zur Definition des Provisionssatzes gefüllt wurden. Zusätzlich müssen Sie in den folgenden Spalten Angaben zur Berechnung der Provision machen.

## Vertreter - Provisionssätze kopieren
**Stammdaten > Firma > Vertreterprovision > Menü Funktionen > Provisionssätze kopieren**

*Abb. B-605 Provisionssätze kopieren*

In diesem Dialog übertragen Sie die Provisionssätze eines Vertreters auf einen anderen.

### Quelle, Ziel
- **Vertreter:** Wenn Sie in beiden Feldern denselben Vertreter auswählen, können Sie seine bisherigen Provisionssätze kopieren und dabei mit anderen Jahrgängen, Schlüsseln und mit einem neuen Gültigkeitsdatum speichern, um anschließend die Staffelmengen und Prozentangaben zu bearbeiten.
- **Jahrgang, Schlüssel:** Preislisten der Quelle und des Ziels.
- **Kunde:** Kunden, auf den die Provisionssätze beschränkt sind.
- **Gültigkeitsdatum, Vorgabe Gültigkeitsdatum:** Gültigkeitsdatum, ab dem die Provision in der neuen Form berechnet werden soll. Für das Ziel können Sie ein Datum in der Zukunft wählen.
- **Ziel überschreiben:** Die Provisionssätze des Ziels können überschrieben oder ergänzt werden.
    - Die Provisionssätze des Vertreters werden durch die Provisionssätze der Quelle überschrieben und ggf. durch zusätzliche Provisionssätze ergänzt.
    - Die bestehenden Provisionssätze des Vertreters werden gelöscht und durch die Provisionssätze aus der Quelle ersetzt.

## Banken
**Stammdaten > Firma > Banken**

*Abb. B-606 Banken*

In diesem Dialog tragen Sie die firmeneigenen Bankverbindungen ein. Sie können mehrere Konten pro Mandant bei unterschiedlichen Bankenverbindungen hinterlegen. Nur die Banken können angegeben werden, die im Dialog Banken hinterlegt sind.
⇨ "Banken" auf Seite B-908

**Mandant:** Mandant, dessen Banken in der Übersicht angezeigt werden.

### Bankverbindung
- **BLZ/BIC:** Bankleitzahl und BIC (Business Identifier Code). Über die Lupe können Sie nach der gewünschten Bank suchen. Über den Ordner können Sie weitere Bankdaten hinterlegen oder die vorhandenen ergänzen.
- **Name, Sitz:** Namen und Standort der Bank werden automatisch angezeigt.
- **Konto:** Kontonummer des Mandanten.
- **Hauptbank:** Wenn Sie mehrere Konten für einen Mandanten eingetragen haben, müssen Sie einen Eintrag als Hauptbank kennzeichnen.
    - Die Daten des aktuell angezeigten Kontos sind nicht als Hauptbank gekennzeichnet.
    - Die Daten des aktuell angezeigten Kontos sind als Hauptbank gekennzeichnet.
- **IBAN:** International Bank Account Number zum angegebenen Konto.

### Banken
In der Übersicht werden alle Bankverbindungen des aktuellen Mandanten angezeigt.

## Filialen
**Stammdaten > Firma > Filialen**

*Abb. B-607 Filialen*

In diesem Dialog pflegen Sie Filialen Ihrer Mandanten. Die Daten dienen nur zur Information.

### Anschrift
- **Name:** Namen der Filiale, so wie sie im Handelsregister angegeben ist oder offiziell bezeichnet wird.
- **Straße:** Adresse der Filiale.

### Kommunikation
- **Telefon 1-4, Fax, Mail:** Telefonnummern, Faxnummer und E-Mail-Adresse der Filiale.

### Übersicht
In der Übersicht werden alle Filialen für den jeweils ausgewählten Mandanten angezeigt.

## Buchungsperioden
**Stammdaten > Firma > Buchungsperioden**

*Abb. B-608 Buchungsperioden*

In diesem Dialog tragen Sie die Buchungsperioden ein. Die Einträge werden bei der Übergabe an Ihr FiBu-Programm geprüft.
Damit Aufträge, Bestellungen und Gutschriften zum gewünschten Zeitpunkt automatisch übergeben werden, definieren Sie unterschiedliche Buchungsperioden. Auslöser für die Übergabe ist der von Ihnen jeweils festgelegte Status.
Wenn das eingetragene Datum z. B. für Aufträge erreicht ist, kann kein Auftrag mehr in diese Buchungsperiode übergeben werden.

**Abgeschlossene Buchungsperiode:** Datum, an dem die Buchungsperiode abgeschlossen ist. Für die Prüfung der Dokumente ist immer nur das Datum relevant, das dem aktuellen Datum am nächsten ist.

**Auftrag, Gutschrift, Bestellung:** Die Buchungsperiode gilt nur für den jeweils markierten Typ.
- Die Buchungsperiode gilt nicht.
- Die Buchungsperiode gilt für diesen Dokumententyp.

## Produktzuordnung Zuschläge
**Stammdaten > Firma > Produktzuordnung Zuschläge**

*Abb. B-609 Produktzuordnung Zuschläge*

In diesem Dialog verwalten Sie Ihre Sonderrabatte und Teuerungszuschläge. Zusätzlich zu den hinterlegten Teuerungszuschlägen existieren zehn Sonderrabatte, die Sie entweder als Sonderrabatte oder Teuerungszuschläge nutzen können, z. B. Zuschläge für Transport-/Mautkosten, L-Gestelle.

> **Zuschlagsprodukt**
> Jeder Zuschlag oder Sonderrabatt, der wie ein Produkt erfasst werden soll, muss als Produkt angelegt sein.

### Zuordnung
- **Mandant:** Mandant, für den die Zuschläge gelten.
- **Allgemein, Kunde:** Mit der Wahl der Option legen Sie fest, ob der Zuschlag für alle Kunden oder nur für einen bestimmten gilt. Die entsprechenden Eingabefelder werden freigeschaltet.
- **Zuschlag:** Zur Auswahl werden die hinterlegten Zuschläge und Sonderrabatte angeboten.
  ⇨ Tutorial 1, "Verfügbare Teuerungszuschläge/Sonderrabatte" auf Seite B-327
  ⇨ Tutorial 1, "Automatischen Zuschlag definieren" auf Seite B-329
- **Produkt:** Produkt, mit dem der Zuschlag oder der Rabatt berechnet werden soll. Als Produktbezeichnung wird die Bezeichnung 1 aus der Produktverwaltung angezeigt. Diese wird auch in der Produkt- und Kundenverwaltung im Bereich Zuschläge/Rabatte anwenden angezeigt.
- **Gültig von - bis:** Zeitraum, in dem der Rabatt bzw. Zuschlag gültig sein soll.
- **Position im Dokument:** Mit der Positionsnummer wird die Reihenfolge angegeben, in der die Sonderrabatte bzw. Teuerungszuschläge als Position im Dokument eingefügt werden. Sie bestimmen damit auch die Berechnungsreihenfolge. Die Nummern können mehrfach vergeben werden.
    - **0:** Positionsbezogene Sonderrabatte oder Teuerungszuschläge werden mit Position 0 definiert, z. B. Struktur innen-Zuschlag, Zuschlag bei Überschreitung der maximalen Fläche.
    - **950-999:** Die Sonderrabatte oder Teuerungszuschläge, die auf alle vorherigen oder Teile der vorherigen Positionen wirken, werden mit einer Positionsnummer zwischen 950 und 999 definiert.
    - Beim Mindermengenzuschlag werden alle Positionen mit demselben Mindermengenzuschlag (Produkt) geprüft und für alle zusammen eine Zuschlagsposition eingefügt. Als Positionsnummer muss eine Zahl eingetragen werden zwischen der Null (0), die sich auf eine einzelne Position bezieht, und 900, die am Ende des Dokuments eingefügt werden.

> **Anlieferpauschale bei Abholung**
> Damit bei der Tour Abholung die Anlieferpauschale nicht automatisch während der Dokumentenerfassung eingefügt wird, muss in der Tourenverwaltung bei dieser Tour die Checkbox ohne Lief.Pausch. aktiviert sein.
> ⇨ "Touren" auf Seite B-862

### Zuschlagszuordnung
In der Übersicht werden alle Zuschläge aller Mandanten aufgeführt.
Wenn Sie einen Eintrag markieren, können Sie die Werte in den freigeschalteten Feldern überschreiben.

## Formeln
**Stammdaten > Firma > Formeln**

*Abb. B-610 Formelverwaltung*

In diesem Dialog sind alle Formeln hinterlegt, mit denen Sie bestimmte Aufgaben in A+W Business automatisieren können. Im Register **Formel** wird jeweils die Syntax der Formel angezeigt, die im Register **Tabelle** markiert ist.

> **Formel einfügen oder bearbeiten**
> Wenn Sie weitere Formeln benötigen oder eine Formel anpassen müssen, wenden Sie sich bitte an die A+W Software GmbH.

### Menü Optionen
Über dieses Menü können Sie die Prüfung der Formel während der Eingabe aktivieren. Fehler werden beim Speichern angezeigt.

## Schnittstellen-Dienst
**Stammdaten > Firma > Schnittstellen-Dienst**

In diesem Dialog definieren Sie die Schnittstellen, über die Daten zwischen A+W Business und anderen Programmen ausgetauscht werden sollen.

Im Dialog Schnittstellen-Dienst finden Sie folgende Register:
- Schnittstellen-Dienst - Einstellungen A+W Production-Formate
- Schnittstellen-Dienst – Einstellungen weitere Formate
- Schnittstellen-Dienst - Optionen

### Schnittstellen-Dienst – Einstellungen A+W Production-Formate
**Stammdaten > Firma > Schnittstellen-Dienst > Register Einstellungen A+W Production-Formate**

*Abb. B-611 Produktionsrückmeldungen – Einstellungen A+W Production-Formate*

In diesem Register wählen Sie die Rückmeldungen aus, die Sie von A+W Production per Datei empfangen und einlesen wollen.
Wenn STSP-, STSL-, STSD-, STSB-, STSG-Dateien für die Rückmeldungen genutzt werden, muss im Bereich Auftrag produziert bei eine Erfassungsstelle ausgewählt werden, die einem Statuspunkt zugewiesen ist. Wenn eine solche Erfassungsstelle nicht zugewiesen wurde, erzeugt die Rückmeldung einen Fehler.

Die Erfassungsstellen werden im Dialog Erfassungsstellen Produktion hinterlegt.
⇨ "Erfassungsstellen Produktion" auf Seite B-870

> **Gesperrte Felder**
> Die Felder sind gesperrt, wenn im Register Einstellungen weitere Formate die Checkbox Import von Produktionsrückmeldungen aktiviert ist. Sie können dann keine Einstellungen für A+W Production-Formate festlegen.

#### Identifikation
**Einstellungen für:** Mitarbeiter, für den die Einstellungen gelten. Wenn die Einstellungen für alle Benutzer gelten sollen, wählen Sie den Eintrag Administrator. Bei dieser Einstellung muss im Bereich Auftrag produziert bei dieselbe Erfassungsstelle ausgewählt sein, wie in den Firmendaten > Register Lager / EK / EDI.

#### A+W Production-Formate
In diesem Bereich wählen Sie aus, welche Rückmeldungen aus A+W Production eingelesen werden sollen. Das Verzeichnis für die Rückmeldedatei können Sie dann im jeweils freigeschalteten Feld angeben. Dieselben Verzeichnisse müssen in A+W Production angegeben werden, damit die Dateien korrekt gespeichert werden. Die Dateien werden über den A+W Commercial Exchange Service eingelesen.

- **Import von Produktionsrückmeldungen:** Die STSP-Rückmeldung erfolgt überwiegend pro Stück. Sie können für die entsprechende Erfassungsstelle einstellen, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
    - Rückmeldedateien aus der Produktion werden nicht eingelesen.
    - Die Rückmeldung aus der Produktion wird als STSP-Datei gesendet. Der Auftragsstatus, das Produktionsdatum und die Kopf- bzw. Positionslaufnummer werden aktualisiert.

- **Prod.freigabe Auftrag, falls Subauftrag produziert:** Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Zu einem Auftrag kann ein Teilauftrag erfasst sein. Wenn eine Produktionsrückmeldung einen solchen Subauftrag betrifft, kann der Status des Gesamtauftrags umgesetzt werden.
    - Ein Auftrag wird nicht automatisch auf den Status zur Produktionsfreigabe gesetzt.
    - Wenn die Subaufträge als produziert zurückgemeldet werden, erhöht sich der Status des Hauptauftrags automatisch auf Produktionsfreigabe.
- **Laufnummer aus dem Auftragskopf übernehmen:** Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der A+W Business-Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
    - Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
    - Nach der Aktualisierung des Auftragskopfes erhalten alle Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für *produziert* ist.
      ⇨ "Erfassungsstellenzuordnung" auf Seite B-964

- **Import von Planungsrückmeldungen:** Aus der Produktion können die STSL-Daten der Grob- und Feinplanung importiert werden. Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
    - Rückmeldungen aus Grob- und Feinplanung werden nicht eingelesen.
    - Die Rückmeldungen aus Grob- und Feinplanung werden eingelesen. Der Auftragsstatus wird dann der angegebenen Erfassungsstelle entsprechend hoch gesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
      ⇨ "Erfassungsstellen Produktion" auf Seite B-870

- **Import von BDE-Rückmeldungen:** Die STSD-Rückmeldung aus der Betriebsdatenerfassung (BDE) dient im A+W Business dazu, den Auftragsstatus, das Produktionsdatum und die Kopf- und/oder Positionslaufnummer zu aktualisieren. Die Rückmeldung erfolgt überwiegend pro Stück. Sie können einstellen, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
    - BDE-Rückmeldungen werden nicht eingelesen.
    - Die BDE-Rückmeldung wird als STSD-Datei gesendet.

- **Produktionsgestellnummer in Position übernehmen:** Das Feld ist nur freigeschaltet, wenn BDE-Rückmeldungen importiert werden. Wenn in der BDE-Rückmeldung Gestellnummern zu Positionen enthalten sind, können diese in A+W Business der Position zugewiesen werden.
    - Gestellnummern werden nicht in die Position übernommen.
    - Die gemeldeten Gestellnummern werden in den Auftrag zurückgeschrieben und der jeweiligen Position zugeordnet.

- **Import von Gestellzuordnung-Rückmeldungen:** Die STSG-Rückmeldung gibt an, welches Gestell der jeweiligen Auftragsposition zugeordnet ist und welche Mengen produziert sind. Die Gestellnummer wird auf dem Lieferschein gedruckt.
    - Rückmeldungen von Gestellzuordnungen werden nicht importiert.
    - Die Rückmeldung der Gestellzuordnung wird als STSG-Datei gesendet.
    - **Gestell-Rückmeldung für Teillieferung:** Bei Teillieferung besteht die Möglichkeit, die Menge der Teillieferungsposition durch die per STSG zurückgemeldete verpackte Menge bestimmen zu lassen. Dazu muss beim Kopieren des Auftrags die Option Teillieferungsmenge > Gestellrückmeldung bei Teillieferung berücksichtigen aktiviert werden. Die Menge der Teillieferungsposition ist dann mit der Gesamtmenge aus den STSG-Meldungen zur betreffenden Auftragsposition vorbelegt. Sie kann nicht mehr geändert werden.

- **Update der Produktionsübersicht durch Erfassungsstelle:** Das Feld ist nur freigeschaltet, wenn Rückmeldungen von Gestellzuordnungen importiert werden. In diesem Feld wählen Sie die Erfassungsstelle aus, über die Gestellrückmeldungen den Status hochsetzen. Über die gewählte Erfassungsstelle wird die Produktionsübersicht im Dialog Übersicht Statusrückmeldung aktualisiert.
  ⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-576

- **Import von Gestell-Ein-/Ausgang-Rückmeldungen:** Die STSK-Rückmeldung meldet den Status des Gestells und das jeweilige Eingangs- und Ausgangsdatum.
    - Rückmeldungen zum Gestelleingang und -ausgang werden nicht importiert.
    - Die Rückmeldung von Gestelleingang und -ausgang wird eingelesen. Nach einer Überprüfung, ob der Kunde und das Gestell existieren, wird die Ausgabe bzw. die Rücknahme des Gestells verbucht. Existiert das Gestell in A+W Business noch nicht, wird es mit dem Typ <k.A.> angelegt.

- **Import von Bruch-Rückmeldungen:** Mit der STSB-Rückmeldung werden die Reklamationen und die bei der Produktion zu Bruch gegangenen Scheiben gemeldet. A+W Business kann daraus automatisch Reklamationsaufträge erstellen.
    - Bruch-Rückmeldungen werden nicht importiert.
    - Die Bruch-Rückmeldung wird als STSB-Datei gesendet.

- **Reklamationsaufträge erstellen:** Das Feld ist nur freigeschaltet, wenn Bruch-Rückmeldungen importiert werden.
    - Reklamationsaufträge werden nicht automatisch erstellt.
    - Bei einer Bruchmeldung wird automatisch ein Reklamationsauftrag erstellt. Dieser Funktion können ein Standard-Verursacher und ein Standard-Grund zugeordnet werden, die jeweils im Reklamationsauftrag überschrieben werden können.

- **Verursacher:** Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Verursacher auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird. (⇨ "Default Reklamationsort" auf Seite B-969)
- **Grund:** Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Reklamationsgrund auswählen.
- **Kostenlos:** Die Checkbox ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
    - Der automatisch erstellte Reklamationsauftrag ist nicht standardmäßig kostenlos.
    - Der automatisch erstellte Reklamationsauftrag ist standardmäßig kostenlos. Die Einstellung kann in dem Reklamationsauftrag überschieben werden.
- **AV-Bereich:** Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können dann einen AV-Bereich auswählen, aus dessen Nummernkreis die Auftragsnummer gezogen wird.
- **Ziel-NV:** Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Nummernverwalter auswählen, in den der automatisch erstellte Reklamationsauftrag gestellt wird.

- **Import von XTV-Rückmeldungen:** Mit der XTV-Rückmeldung werden die Lagermaße abgebucht, die für einen Auftrag zugeschnitten werden. Außerdem werden für Artikel mit Lagermodus kombiniert die qm-Reservierungen in den Aufträgen gelöscht.
    - XTV-Rückmeldungen werden nicht importiert.
    - Die Rückmeldung aus der Optimierung wird als PRODBDA*-Datei gesendet.

#### Optionen
Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie Rückmeldungen importieren, zu denen weitere Angaben möglich sind.

- **Menge größer Positionsmenge in STSB, STSD, STSG, STSL, STSP zulassen:** Aus der Produktion können größere Stückzahlen pro Position zurückgemeldet werden, als im Auftrag enthalten sind.
    - Größere Stückzahlen pro Position werden nicht zugelassen.
    - Die Meldungen können auch bei größeren Stückzahlen verarbeitet werden.
- **Zeitwirtschaft verarbeitet STSD und STSB:** STSD- und STSB-Meldungen können über die Kapazitätsplanung (Zeitwirtschaft) verarbeitet werden.
    - Die Kapazitätsplanung verarbeitet keine Daten aus den STSD- und STSB-Dateien.
    - STSD- und STSB-Dateien werden von der Kapazitätsplanung verarbeitet.
- **Erfassungsstelle STSD:** Erfassungsstelle, über die der Status umgesetzt wird, wenn die STSD-Meldung über die Kapazitätsplanung verarbeitet wird.
- **Erfassungsstelle STSB:** Erfassungsstelle, über die der Status umgesetzt wird, wenn die STSB-Meldung über die Kapazitätsplanung verarbeitet wird.

#### Auftrag produziert bei
Damit ein Auftrag fertiggemeldet werden kann, müssen Sie für die Rückmeldungen eine Erfassungsstelle angeben. Wenn die Einstellungen für alle Benutzer gelten sollen, müssen Sie dieselbe Erfassungsstelle auswählen, wie im Dialog Firmendaten.
⇨ "Firmendaten - Lager/EK/EDI" auf Seite B-957

**Erfassungsstelle:** Erfassungsstelle, die bei Rückmeldungen folgende (zusätzliche) Aktionen auslösen kann:
- Im Auftrag werden das Produktionsdatum und die Laufnummer erhöht.
- Bei Produktionsaufträgen wird der Warenzugang im Lager gebucht.

### Schnittstellen-Dienst – Einstellungen weitere Formate
**Stammdaten > Firma > Schnittstellen-Dienst > Register Einstellungen weitere Formate**

*Abb. B-612 Produktionsrückmeldungen – Einstellungen weitere Formate*

In diesem Register wählen Sie die Rückmeldungen aus, die Sie aus der Betriebsdatenerfassung (BDE), von ALFERT und von der FiBu erhalten und einlesen wollen.

#### BDE- und ALFERT-Formate
> **Gesperrte Felder**
> Die Felder im Bereich BDE- und ALFERT-Formate sind gesperrt, wenn im Register Einstellungen A+W Production-Formate die Checkbox Import von Produktionsrückmeldungen aktiviert ist. Sie können dann keine Einstellungen für BDE-Formate festlegen.

- **Import von Produktionsrückmeldungen:** Die Rückmeldung erfolgt überwiegend pro Stück. In A+W Business kann für die entsprechende Erfassungsstelle eingestellt werden, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
    - Rückmeldedateien aus der Produktion werden nicht importiert.
    - Die Rückmeldung aus der Produktion wird aus der AWB_STAT-Datei eingelesen.
- **Laufnummer aus dem Auftragskopf übernehmen:** Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Die Laufnummer aus dem Auftragskopf kann für die Positionen übernommen werden.
    - Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
    - Nach der Aktualisierung des Auftragskopfes erhalten alle die Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für *produziert* ist.
- **Import von Gestell-Rückmeldedateien:** Die AH_GEST.DAT-Rückmeldung meldet den Status des Gestells und das jeweilige Eingangs- und Ausgangsdatum.
    - Rückmeldungen zum Gestelleingang und -ausgang werden nicht importiert.
    - Rückmeldungen von Gestelleingang und -ausgang werden eingelesen.
- **Import von AWPool-Dateien:** Mit der AWPool-Rückmeldung werden in A+W Business Auftragsstatus, Produktionsdatum, Kopf- und Positionslaufnummer aktualisiert. Die Zuordnung der AWPool-Status zu einem A+W Business-Status ist fest programmiert.
    - AWPool-Rückmeldungen werden nicht importiert.
    - AWPool-Rückmeldungen werden als POOL*.DAT-Dateien eingelesen. Das Feld Update Produktionsdatum ab Status wird freigeschaltet.
- **Update Produktionsdatum ab Status:** Das Feld ist nur freigeschaltet, wenn AWPool-Rückmeldungen importiert werden.
    - Das Produktionsdatum im Auftrag wird nicht aktualisiert.
    - Das Produktionsdatum im Auftrag wird aktualisiert, wenn einer der Status eingestellt ist, die zur Wahl stehen.

#### FiBu
In diesem Bereich legen Sie die Einstellungen für die Meldung der Offenen Posten fest, die automatisiert über den A+W Commercial Exchange Service eingelesen werden.
- **Import von Offen-Posten-Rückmeldungen:** Offene Posten (OP) können aus dem FiBu-Programm per Datei gemeldet werden. Dies betrifft nur die Kundenkonten.
    - OP-Rückmeldungen werden nicht importiert.
    - OP-Rückmeldungen werden als Datei eingelesen. Die Felder für den Ablageort, eine Sicherungs- und eine Batch-Datei werden freigeschaltet.
- **Sicherungsdatei anlegen:** Das Feld ist nur freigeschaltet, wenn OP-Rückmeldungen importiert werden. Sie können dann eine zusätzliche Sicherungsdatei speichern und festlegen, wie viele Tage diese gespeichert bleibt.
    - Zur OP-Rückmeldedatei wird keine Sicherungsdatei gespeichert.
    - OP-Rückmeldungen sollen als Sicherung (mit Zeitstempel) zusätzlich an einem anderen Ort gespeichert werden. Die Felder zur Auswahl des Verzeichnisses und für die Vorhaltetage werden freigeschaltet.
- **Vorhaltetage für Sicherungsdateien:** Das Feld wird nur freigeschaltet, wenn eine Sicherungsdatei gespeichert werden soll. Sie können eintragen, wie viele Tage diese Datei nicht überschrieben werden darf.
- **Batch-Datei:** Namen der Batch-Datei, die zum Kopieren der Dateien benötigt wird.

### Schnittstellen-Dienst – Optionen
**Stammdaten > Firma > Schnittstellen-Dienst > Register Optionen**

*Abb. B-613 Produktionsrückmeldungen – Optionen*

In diesem Register legen Sie die Intervalle fest, mit denen regelmäßig nach neuen Rückmeldungen gesucht werden soll.

#### Intervall
- **Standard - Minute(n):** Intervall für den A+W Commercial Exchange Service. Wenn Sie z. B. eine 2 eintragen, prüft der Service alle 2 Minuten, ob neue Rückmeldungen aus der Produktion vorliegen, und liest diese ein.
- **OP-Rückmeldung – Minute(n):** Intervall für die Rückmeldung der Offenen Posten (OP). Wenn Sie z. B. eine 120 eintragen, werden alle 2 Stunden neuen Rückmeldungen per Batch eingelesen. OP-Rückmeldungen können nur importiert werden, wenn die Funktion im Register Einstellungen weitere Formate aktiviert ist. Für die Rückmeldungen müssen Sie im Dialog Firmendaten die Checkboxen für die OP-Meldungen aktivieren. (⇨ "Firmendaten - FiBu" auf Seite B-924)

#### Einstellungen für automatischen Mailversand
- **Mailversand:** Mails eines bestimmten Absenders können automatisch an eine bestimmte Adresse gesendet werden.
    - Mails nicht werden gesendet.
    - Mails werden gesendet. Die Felder werden freigeschaltet.
- **Server:** Name des Servers, über den der Mailversand gesteuert wird.
- **Port:** Nummer des Ports für den Mailversand.
- **Absender Adresse, Empfänger Adresse:** E-Mail-Adressen, die standardmäßig für verwendet werden sollen.
- **Authentifizierung:** Für die Datenübertragung kann eine Authentifizierung verwendet werden.
    - Die Sendebestätigung wird nicht ohne Authentifizierung gesendet.
    - Für die Sendebestätigung ist Authentifizierung erforderlich. Die Felder zur Eingabe der Anmeldedaten werden freigeschaltet.
- **SSL Verschlüsselung verwenden:** Secure Sockets Layer (SSL); Verschlüsselungsprogramm zur sicheren Datenübertragung im Internet.
    - Die Sendebestätigung wird nicht verschlüsselt.
    - Die Sendebestätigung wird nach dem SSL-Protokoll verschlüsselt.
- **Benutzer, Passwort:** Anmeldedaten, mit denen der Sender sich authentifiziert.

## Customizing
**Stammdaten > Firma > Customizing**

*Abb. B-614 Customizing*

In diesem Dialog stellen Sie A+W Business und seine Funktionen auf die Bedürfnisse in Ihrem Unternehmen ein.
Sie können den Dialog nur öffnen, wenn Sie als Administrator mit den entsprechenden Rechten angemeldet sind.

> **Anpassungen einrichten**
> Mit dem Customizing greifen Sie unter Umständen tief in die Funktionen von A+W Business ein. Wenn Sie A+W Business für Ihr Unternehmen weiter anpassen wollen, setzen Sie sich bitte mit der A+W Software GmbH in Verbindung, um die Anpassungen abzustimmen.

## Datencontainer
**Stammdaten > Firma > Datencontainer**

*Abb. B-615 Customizingdaten – Datencontainer*

In diesem Dialog verwalten Sie Daten, die für das Customizing benötigt werden, mit der A+W Business-Datenbank. Die Bezeichnung der Register und der Tabellenspalten kann dabei ebenfalls konfiguriert werden.

## Texte
**Stammdaten > Texte**

In diesem Programmbereich werden die Texte und die Textkennzeichen verwaltet, die in der Dokumentenbearbeitung benötigt werden.

Im Menü Texte finden Sie folgende Einträge:
- "Textkennzeichen" auf Seite B-1044
- "Texte" auf Seite B-1045
- "Systemtexte" auf Seite B-1046
- "Mahntexte" auf Seite B-1047
- "Dateianhangs-Typen" auf Seite B-1048
- "Dateianhangs-Bemerkungen" auf Seite B-1049
- "Technische Werte" auf Seite B-1049

### Textkennzeichen
**Stammdaten > Texte > Textkennzeichen**

*Abb. B-616 Textkennzeichen*

In diesem Dialog hinterlegen Sie die Textkennzeichen. Die Textkennzeichen dienen der Zuordnung von Textblöcken zu Themenbereichen, z. B. P für Produktion, L für Lieferschein, T für allgemeine Texte. Über die Textkennzeichen können Sie steuern, welche Texte in welchen Dokumenten gedruckt werden sollen.
⇨ Tutorial 2, "Textarten" auf Seite B-462

- **Kennzeichen:** Textkennzeichen, z. B. P für Produktionstexte, V für Terminverschiebungen.
- **Bezeichnung:** Namen, z. B. Produktion für Texte, die an die Produktion übergeben werden sollen.

### Texte
**Stammdaten > Texte > Texte**

*Abb. B-617 Texte bei Mehrsprachigkeit*

In diesem Dialog erfassen Sie Standardtexte, die häufig verwendet werden, z. B. die Rahmentexte oder Texte für die Terminverschiebung. In den Texten können Platzhalter verwendet werden, die erst beim Druck eines Dokuments mit Werten gefüllt werden.
⇨ Tutorial 2, "Textkennzeichen und Standardtexte" auf Seite B-464

Wenn Sie mit der Mehrsprachigkeit arbeiten, müssen alle Texte auch in der jeweiligen Sprache erfasst werden. Achten Sie dabei darauf, dass die Textnummern in den Übersetzungen nicht geändert werden.
⇨ "Sprachen" auf Seite B-556

- **Sprache:** Auswahl der Sprache, in der der Text gedruckt werden soll.
- **Nummer:** Beliebige Nummer für den Text. Sie sollten die Texte pro Textkennzeichen in Nummernbereichen zusammenfassen, z. B. 1-99 für Rechnungstexte, 100-199 für Angebotstexte. Wenn Sie mit dem Modul Mehrsprachigkeit arbeiten, muss zu Beginn der Erfassung der fremdsprachlichen Texte in jedem Sprachregister mindestens ein Text mit der Nummer 0 angelegt sein.
- **Matchcode:** Die Eingabe des Matchcodes ist optional.
- **Kennzeichen:** Über das Textkennzeichen wird der Text für den Druck zugeordnet. Durch die Angabe des Kennzeichens L für Lieferschein können Sie z. B. Dialog Formulare steuern, ob der Text gedruckt werden soll oder nicht.
- **Texttyp AWProd.:** Positionstexte werden an die Produktion übergeben, wenn das Textkennzeichen (P) für die Produktionsübergabe die Übergabe erlaubt. Für diese Texte können Sie den Texttyp (Fremdschlüssel) angeben, der in A+W Production für diese Texte genutzt wird. Ist kein Texttyp eingetragen, wird standardmäßig der Texttyp 1 übergeben.

#### Auswahl
In der Übersicht werden alle Texte angezeigt, die den Auswahlkriterien entsprechen.

#### Textbearbeitung
- **Schaltflächen:** Sie können die Schriftart und -größe ändern und Hyperlinks, Bilder und Tabellen einfügen.
  ⇨ Tutorial, "Text erfassen" auf Seite C-54
- **(Eingabefeld):** Standardtext oder Rahmentext. Bei Rahmentexten und bei bestimmten Standardtexten können Sie mit Variablen (Platzhaltern) arbeiten.
  ⇨ Tutorial 2, "Texte anlegen" auf Seite B-470

### Systemtexte
**Stammdaten > Texte > Systemtexte**

*Abb. B-618 Systemtexte*

In diesem Dialog pflegen Sie die Systemtexte. Diese Texte sind sowohl in Dialogen als auch in Formularen fest verknüpft. Sie können (sinngemäß) geändert werden, z. B. für eine andere Sprache.
⇨ Tutorial 2, "Systemtexte" auf Seite B-462

> **Texte nicht löschen**
> Die sinngemäße Änderung von Systemtexten ist erlaubt. Sie dürfen aber weder gelöscht noch dürfen neue hinzugefügt werden. Das Verschieben von Variablen (Platzhaltern) an eine andere Stelle im Text ist möglich.

- **Sprache:** Auswahl der Sprache, in der der Text gedruckt werden soll.
- **Nummer:** Anzeige der Textnummer.
- **Textbearbeitung:** Sie können den Systemtext bearbeiten, z. B. in eine andere Sprache übersetzen.

#### Auswahl
In der Übersicht werden die Nummern der Systemtexte angezeigt.

### Mahntexte
**Stammdaten > Texte > Mahntexte**

*Abb. B-619 Mahntexte*

In diesem Dialog tragen Sie die Mahntexte ein, die Sie bei Mahnungen verwenden wollen. Die Texte dienen nur zur Information.
⇨ Verkauf, "Mahnwesen" auf Seite C-733

- **Bezeichnung:** Namen des Mahntextes.
- **Fremdschlüssel:** Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung.
- **Gesperrt:** Einen Mahntext kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
    - Der Mahntext kann zugewiesen werden.
    - Der Mahntext ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt und gedruckt.

### Dateianhangs-Typen
**Stammdaten > Texte > Dateianhangs-Typen**

*Abb. B-620 Typen der Dateianhänge*

In diesem Dialog tragen Sie Kennzeichen für Dateianhänge ein. Standardmäßig sind alle Anhänge mit dem Typ A (alle) gekennzeichnet und werden außer bei der Bestellübergabe immer übergeben.
Über die Kennzeichen können Sie die Übergabe von angehängten Dateien (Dokumenten, Abbildungen) steuern:
- **Produktionsübergabe:** Dateianhänge für Übergabe in OrderXML, z. B. Produktinformationen.
  ⇨ Fertigung, "Einstellungen Produktionsübergabe - Texte/Anlagen" auf Seite E-187
- **Dokumente kopieren:** Angebot zu Auftrag, z. B. Kalkulationsinformationen.
  ⇨ Verkauf, "Dokumente kopieren - Texte/Anlagen" auf Seite C-547
- **Bestellübergabe, z. B. Produktinformationen.**
  ⇨ Verkauf, "Erweiterte Einstellungen - Allgemein" auf Seite C-666

### Dateianhangs-Bemerkungen
**Stammdaten > Texte > Dateianhangs-Bemerkungen**

*Abb. B-621 Bemerkungen für Dateianhänge*

In diesem Dialog hinterlegen Sie Standard-Bemerkungen, die sehr oft benutzt werden. Diese Standard-Bemerkungen werden in der Auftragserfassung > Register Anlagen zur Auswahl angeboten.
⇨ Verkauf, "Kopfdaten - Anlagen" auf Seite C-435

### Technische Werte
**Stammdaten > Texte > Technische Werte**

*Abb. B-622 Texte der technischen Werte für Leistungserklärungen*

In diesem Dialog hinterlegen Sie die technischen Werte für die Erzeugung von Leistungserklärungen.
Die Texte müssen für jede Sprache eingetragen werden, damit Leistungserklärung mit den entsprechende Übersetzung der Merkmale in der jeweiligen Sprache erzeugt werden können.
Diese Informationen werden nicht benötigt, wenn der Anwender bereits fertige Leistungserklärungen vorliegen.

## Formulare
**Stammdaten > Formulare**

Als Formulare werden sowohl die Ausgaben im Druck als auch auf dem Bildschirm bezeichnet. Dazu zählen neben den Dokumenten auch die Listen und Berichte (Reports).

Im Menü **Formulare** finden Sie folgende Einträge:
- "Formularverwaltung" auf Seite B-1050
- "Auftragsformulare" auf Seite B-1066
- "Druckaufträge" auf Seite B-1067
- "Crystal Reports" auf Seite B-1073

### Formularverwaltung
**Stammdaten > Formulare > Formularverwaltung**

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
⇨ Verkauf, "Formular-/Etikettendruck" auf Seite C-640

> **Anbindung an das DMS-System Algeier scanView**
> Bei dem Druckvorgang kann aus dem aktuellen Dokument eine PDF-Datei erstellt und für die DMS Archivierung an das Allgeier scanView System übertragen werden. Diese Funktionalität kann mandanten-übergreifend genutzt werden. Wenden Sie sich an die A+W Software GmbH, wenn Sie Funktionalität nutzen wollen.

#### Formularverwaltung - Formular
**Stammdaten > Formulare > Formularverwaltung > Register Formular**

*Abb. B-623 Formularverwaltung – Formular*

In diesem Register legen Sie zu den einzelnen Druckpunkten fest, welche Formulare für den Druck verwendet werden. Der Druckpunkt entspricht dem Statuspunkt, der programmintern genutzt wird.
⇨ "Statuszuordnung" auf Seite B-887

##### Druckpunkte
Mit der Wahl der Option legen Sie fest, ob Sie sich Kunden oder Lieferantenformulare anzeigen lassen oder ändern möchten.
- **Standard:** Die Formulare gelten allgemein.
- **Kunden, Lieferanten:** Die Formulare gelten für einen Kunden oder einen Lieferanten. Das Feld zur Auswahl des Partners wird freigeschaltet.

**Druckpunkt:** Druckpunkt, dem ein Formular zugeordnet ist. Sie können jedem Druckpunkt beliebig viele Formulare zuordnen. Nachdem einem Formular nach der Ersterfassung ein Druckpunkt zugeordnet ist, kann dieser Druckpunkt nachträglich im Formular nicht geändert werden. Wird z. B. eine Auftragsbestätigung mit dem Druckpunkt 100-AB Druck gedruckt, so erhält der Auftrag automatisch den Anwenderstatus 21.

##### Formulareinstellungen
- **Bezeichnung:** Ihre (firmeninterne) Bezeichnung des Formulars.
- **Anzahl:** Nummer der Druckausgaben. Dabei wird jede Seite des Formulars jeweils mehrfach gedruckt. Die Anzahl der Kopien (Durchschläge) geben Sie im Register Optionen 1 an.
- **Standard:** Wenn in Ihrer Firma unterschiedliche Formulare für den Druck eines Dokumentes verwendet werden, müssen Sie festlegen, welches der Formulare standardmäßig verwendet wird.
    - Das Formular wird nicht standardmäßig verwendet.
    - Das Formular wird standardmäßig ausgewählt, wenn Sie den entsprechenden Druck starten, z. B. eine Auftragsbestätigung für einen bestimmten Kunden.
- **Sprache:** Sprache, der das markierte Formular zugeordnet ist. Dazu muss für jede Sprache je ein entsprechendes Formular angelegen sein. Diese Funktion ist nur aktiv, wenn A+W Business in der mehrsprachigen Variante installiert ist.
- **Übersteuerung der Dokumentensprache:** Mit dieser Einstellung können Sie die Sprache übersteuern, die im Feld Sprache ausgewählt ist.
    - Das Formular wird der gewählten Sprache entsprechend gedruckt (Standardeinstellung).
    - Die gewählte Sprache wird übersteuert. Markieren Sie die Checkbox dann, wenn Sie z. B. ein Formular als Produktionspapier verwenden. In diesem Fall ist es wichtig, dass das Produktionspapier immer in Ihrer Landessprache gedruckt wird (unabhängig vom Sprachkennzeichen des Dokumentes).

##### Report
- **Dateiname:** Zuordnung des Formulars zu einer Report-Datei. Ohne diese Zuordnung können die Berichte nicht erstellt werden. Beispiele von Zuordnungen, die standardmäßig in A+W Business verwendet werden:
    - Angebot = ANGEB.QRP
    - Auftragsbestätigung = AUFTRAG.QRP
    - Lieferschein = LIEFER.QRP
    - Rechnung = RECHN.QRP
    - Gutschrift = GUTSCH.QRP
    - Bestellanfrage = ANFRAGE.QRP
    - Bestellung = BESTELL.QRP
- **Druckservice Report:** Auswahl des Druckpunkts, über den der Report erstellt wird. Für Leistungserklärungen muss z. B. der Wert 006 – Declaration of Performance zusammen mit der zum Bericht passenden Sprache eingetragen werden. Zusätzlich kann die Übertragung an das DMS System aktiviert werden.
  ⇨ "Dokumentenarchivierung" auf Seite B-1059
- **Transfer an iQuote:** Ausgegebene Formulare können auch an iQuote übergeben werden.
    - Das gedruckte Formular wird nicht an iQuote übergeben.
    - Das gedruckte Formular wird an iQuote übergeben.

##### Abweichender Formularstatus
- **Statuspunkt:** Sie können jedem Formular einen abweichenden Statuspunkt zuordnen. Diese Zuordnung ist in der Regel nur bei einem Barverkaufsformular nötig. In diesem Fall wählen Sie den Statuspunkt Barverkauf aus.

##### Leistungserklärung
- **Versand per Mail:** Sie können festlegen, mit welchem Druck die Leistungserklärung gesendet werden soll.
    - Beim Druck des ausgewählten Formulars wird keine Leistungserklärung gesendet.
    - Beim Druck des ausgewählten Formulars wird automatisch eine Leistungserklärung per E-Mail gesendet.

##### Formulare
In der Übersicht werden alle Formulare aufgelistet, die den Auswahlkriterien entsprechen.

#### Formularverwaltung – Kopf-/Fußtexte
**Stammdaten > Formulare > Formularverwaltung > Register Kopf-/Fußtext**

*Abb. B-624 Formularverwaltung – Kopf-/Fußtexte*

In diesem Register wählen Sie die Texte aus, die immer auf dem ausgewählten Formular gedruckt werden, z. B., wenn Sie auf allen Ihren Auftragsbestätigungen eine Information über Ihre nächsten Betriebsferien drucken möchten.

> **Voraussetzung**
> Der gewünschte Text muss im Dialog Texte hinterlegt sein.

- **Texte:** Über die Lupe können Sie pro Kopf- und Fußtext einen der hinterlegten Text auswählen. (⇨ "Texte" auf Seite B-1045)
- **Kopftext:** Der gewählte Text wird im Formularkopf gedruckt.
- **Fußtext:** Der gewählte Text wird im Formularfuß gedruckt.

#### Formularverwaltung - Texte
**Stammdaten > Formulare > Formularverwaltung > Register Texte**

*Abb. B-625 Formularverwaltung – Texte*

In diesem Register tragen Sie alle Abweichungen von Standarddruck ein.

- **Nicht zu druckende Textkennzeichen:** Kennzeichen der Texte, die nicht auf dem gewählten Formular gedruckt werden sollen. Auf der Auftragsbestätigung sollen z. B. keine Texte mit dem Textkennzeichen L für Lieferschein und P für Produktion gedruckt werden. (⇨ "Textkennzeichen" auf Seite B-1044)
- **Variable Texte:** Zu jedem Formular können bis zu 10 variable Texte verwaltet werden. Diese Texte werden im Formulardruck beliebig verwendet, z. B. als alternative Überschrift. Die verwendeten Texte müssen in der Textverwaltung angelegt sein.

> **Beispiel**
> Für den Druck von Aufträgen wird nur ein Formular verwendet. Als variable Texte sind die Texte Auftragsbestätigung (1) und Lieferschein (2) eingetragen.
> Wenn der Druck der Auftragsbestätigung gestartet wird, wird automatisch der variable Text 1 ausgewählt und gedruckt. Beim Druck des Lieferscheins wird der Text 2 gedruckt.

#### Formularverwaltung – Optionen 1
**Stammdaten > Formulare > Formularverwaltung > Register Optionen 1**

*Abb. B-626 Formularverwaltung - Optionen 1*

In diesem Register legen Sie fest, wie die Angaben zu den Auftragspositionen gedruckt werden.

##### Kopfwechsel
Mit der Wahl der Option legen Sie den Druck der Produktbezeichnungen fest:
- **Standard:** Bezeichnung 1 und 2
- **Kurzbezeichnung:** Kurzinfo
- **ISO-Aufbau:** Glasbezeichnungen aus Stückliste
- **Immer:** Der Positionskopf wird immer ausgegeben
  ⇨ "Produktverwaltung" auf Seite B-590

##### Mit Modellskizze (siehe Register Skizzendruck)
Sie können pro Formular festlegen, ob eine Modellskizze gedruckt werden soll. Die Größe und Position der Skizze legen Sie im Register Skizzendruck fest.
- Auf dem gewählten Formular wird keine Modellskizze gedruckt.
- Zu jeder Modellposition kann eine Modellskizze gedruckt werden. Die Skizze wird nur dann gedruckt, wenn im Auftrag oder in den Stammdaten des Produktes die entsprechenden Checkboxen markiert sind.
  ⇨ Tutorial 2, "Skizzendruck" auf Seite B-479
  ⇨ "Modellskizze, Sprossenskizze" auf Seite B-600
  ⇨ "Modellskizze, Sprossenskizze" auf Seite B-1064

##### SZR in Bezeichnung
In der Bezeichnung des Produktes kann der Abstandhalter (SZR) mit aufgeführt werden.
- Die Bezeichnung des Abstandhalters wird nicht gedruckt.
- Die Bezeichnung des Abstandhalters wird der Produktbezeichnung hinzugefügt.

##### Modellparameter drucken in
Mit der Wahl der Option legen Sie die Einheit für die Angabe der Modellmaße fest.
- **mm/Inch:** Die Maße werden in Millimeter angegeben.
- **cm/Inch:** Die Maße werden in Zentimeter angegeben.
Die Angabe in Inch wird über die Firmendaten gesteuert: ⇨ "Maßsystem" auf Seite B-974. Die Größe der Skizze wird im Register Skizzendruck festgelegt: ⇨ "Formularverwaltung - Skizzendruck" auf Seite B-1063.

##### Preisdruck
Sie können pro Formular festlegen, ob die Preise der Auftragspositionen gedruckt werden sollen:
- **0 - Standard:** Die Einstellung aus dem Auftrag wird für den Druck übernommen.
- **1 - Preise immer drucken:** Die Preise werden immer gedruckt, unabhängig davon, was im Auftrag angegeben ist.
- **2- Preise immer drucken (Summenmodus):** Die Einstellung aus dem Auftrag wird für den Druck ausgelesen.
  ⇨ Verkauf, "Darstellung der Preise im Druck" auf Seite C-200
  ⇨ Verkauf, "Formularverwaltung" auf Seite C-201

##### Stücklistendruck
Mit der Wahl der Option legen Sie fest, wie die Stückliste gedruckt werden soll:
- **Standard-Druck:** Die Produktbezeichnungen 1, 2 und 3 aus den Produktstammdaten werden gedruckt.
- **Stückliste immer drucken:** Die Stückliste wird immer gedruckt, unabhängig vom Druckkennzeichen in den Produktstammdaten.
- **Entsprechend Druck-Kennz.:** Für den Druck wird das Druckkennzeichen jeder Stücklisten-Komponente abgefragt.
- **Produktionsrel. Stücklisten:** Nur die produktionsrelevante Stückliste wird gedruckt.
  ⇨ "Formularverwaltung - Skizzendruck" auf Seite B-1063

##### Positionen
- **Auf verschiedene Formulare:** Angabe, ob Auftragspositionen auf unterschiedliche Formulare gedruckt werden sollen.
    - Alle Auftragspositionen werden auf dasselbe Formular gedruckt (Standardeinstellung).
    - Die Auftragspositionen können auf unterschiedliche Formulare gedruckt werden.

##### Dokumentenarchivierung
- **Aktiv:** Angabe, ob beim Druck automatisch eine Archivdatei für ein Dokumenten-Management-System (DMS) erstellt wird.
    - Beim Druck des Formulars wird keine Archivdatei erstellt.
    - Beim Druck des Formulars wird automatisch eine Archivdatei erstellt.
      ⇨ "Dokumentenmanagement" auf Seite B-986
      ⇨ "Wiederholungsdruck für Dokumentenarchivierung" auf Seite B-985
- **PDF-Template:** Für den AWSOA Reporting Service kann der Template-Name für PDF-Dateien gespeichert werden.

##### Durchschläge
- **Drucker schließen pro Dokument:** Angabe ob der Drucker nach jedem Dokument geschlossen wird.
    - Der Drucker wird nach dem Druck des Formulars nicht geschlossen.
    - Der Drucker wird nach jeder Ausgabe des Formulars geschlossen.
- **Anzahl:** Anzahl der Druckausgaben (Kopien). Die Einstellung 0 bedeutet ein Exemplar.

#### Formularverwaltung – Optionen 2
**Stammdaten > Formulare > Formularverwaltung > Register Optionen 2**

*Abb. B-627 Formularverwaltung - Optionen 2*

In diesem Register wählen Sie weitere Vorgaben für den Druck auf den Formularen aus.

##### Weitere Optionen
- **Kundendaten lesen (Bank):** Die Bankverbindung kann auf dem gewählten Formular gedruckt werden.
  - Die Bankverbindungen werden nicht auf dem Formular gedruckt.
  - Die Bankverbindungen werden auf dem Formular gedruckt.
  ⇨ "PLZ/Postfach" auf Seite B-762
- **Referenzen drucken:** Die Referenzen können auf dem gewählten Formular gedruckt werden.
  - Die Referenzen werden nicht gedruckt.
  - Die Referenzen werden gedruckt.
- **Preise explizit drucken:** Die impliziten Preise der Stücklisten-Komponenten können gedruckt werden.
  - Die Preise der Stücklisten-Komponenten werden nicht explizit gedruckt.
  - Auf dem Formular werden auch die Stücklistenpreise gedruckt.
  ⇨ "Stücklistendruck" auf Seite B-1058
- **Gestelldaten drucken:** Die Angaben zu den Packmitteln auf dem gewählten Formular gedruckt werden.
  - Die Angaben zu den Packmitteln werden nicht auf dem Formular gedruckt.
  - Die bei der Kommissionierung dem Auftrag zugeordneten Packmittel werden auf dem Formular gedruckt.
- **Kundenindividuelle Artikel drucken:** Die kundenindividuellen Artikel können auf dem gewählten Formular gedruckt werden.
  - Kundenindividuelle Artikel werden nicht auf dem Formular gedruckt.
  - Die im Auftrag enthaltenen kundenindividuellen Artikel werden mit auf das gewählte Formular gedruckt.
- **Gestaffelte Zahlungsziele drucken:** Gestaffelte Zahlungsziele und die zugehörigen Beträge können gedruckt werden.
  - Die gestaffelten Zahlungsziele werden nicht auf dem Formular gedruckt.
  - Die gestaffelten Zahlungsziele werden auf dem Formular gedruckt.
  ⇨ Verkauf: Tutorial, "Fälligkeitsberechnung" auf Seite C-209
- **Auswärtige Gestelle drucken:** Angaben zu ausgeliehenen Gestellen können gedruckt werden.
  - Die Angaben zu ausgeliehenen Gestellen werden nicht auf das Formular gedruckt.
  - Die Angaben zu ausgeliehenen Gestellen werden auf das Formular gedruckt.
- **Kommission in jeder Position drucken:** Ein Kommissionstext kann pro Auftragsposition eingegeben und gedruckt werden.
  - Der Kommissionstext wird nur für die erste Position gedruckt.
  - Für jede Position wird der Kommissionstext gedruckt.
  ⇨ Verkauf, "Kommission" auf Seite C-456
- **Produkttexte nicht wiederholen:** Bei mehreren Positionen mit demselben Produkt kann der Druck des Produkttextes gesteuert werden.
  - Der Produkttext wird immer gedruckt.
  - Wiederholt sich der Produkttext, wird er nur für die erste Position der Gruppe gedruckt.
- **Zeitwirtschaftsdaten drucken:** Aggregate (Maschinen) zur Anfertigung können gedruckt werden (nur für Gläser).
  - Daten zur Kapazitätsplanung werden nicht gedruckt.
  - Wenn für eine Position Daten zur Kapazitätsplanung vorhanden sind, werden diese gedruckt.
- **Klassifikator-Abfrage:** Zusätzliche Kundeninformationen aus den Klassifikatoren können gedruckt werden.
  - Die Klassifikatoren werden nicht abgefragt.
  - Die Klassifikatoren werden auf dem Formular gedruckt.
  ⇨ "Partnerverwaltung - Klassifikatoren" auf Seite B-773
- **Vorherige Rechnungswerte lesen:** Die Daten der Rechnungen können geprüft werden, bevor das Dokument gedruckt wird.
- **Produktdaten lesen:** Sie können festlegen, ob die Produktdaten vor dem Druck neu eingelesen werden.
  - Die Produktdaten werden nicht neu eingelesen.
  - Die Produktdaten werden vor dem Druck neu eingelesen.

#### Formularverwaltung – Skizzendruck
**Stammdaten > Formulare > Formularverwaltung > Skizzendruck**

*Abb. B-628 Formularverwaltung - Skizzendruck*

In diesem Register legen Sie fest, wie groß eine Modellskizze und der zugehörige Text gedruckt werden.

> **Voraussetzung**
> Sie benötigen für den Skizzendruck Shaping & Nesting für A+W Business. Die Einträge werden nur berücksichtigt, wenn im Register Optionen 1 die Checkbox mit Modellskizze aktiviert ist.

##### Modellskizze, Sprossenskizze
- **Druckmodus (Einschränkung):** Auswahl zur Einschränkung des Skizzendrucks:
  - **Kein Druck:** Auf dem gewählten Formular wird keine Skizze gedruckt.
  - **Modell (maßstäblich), Sprosse (maßstäblich):** Maßstabsgetreue Skizzen werden gedruckt.
  - **Modell (schematisch), Sprosse (schematisch):** Standardskizzen werden gedruckt.
- **Breite x Höhe der Skizze:** Max. Breite und Höhe der maßstabsgetreuen Skizze.
  ⇨ "Skizzendruck" auf Seite B-984
- **Maßangaben:** Textgröße bei Sprossen. Der Standardwert ist x 1,00.

##### Textgröße der Modellskizzen
- **Maßangaben:** Textgröße der Maße. Standardwert ist 12 px (Pixel).
- **Segmenttext:** Textgröße der Segmenttexte. Standardwert ist 12 px.
- **Decotexte:** Textgröße in Formen. Standardwert ist 6 px.

#### Formularverwaltung – Customizing
**Stammdaten > Formulare > Formularverwaltung > Register Customizing**

*Abb. B-629 Formularverwaltung - Customizing*

In diesem Register legen Sie fest, an welcher Position auf dem gewählten Formular ein bestimmter Abschnitt beginnt. Dafür müssen die entsprechenden Formeln hinterlegt sein.
⇨ "Formeln" auf Seite B-1031

> **Formel für den Formulardruck**
> Wenn Sie Formeln benötigen oder eine Formel anpassen müssen, wenden Sie sich bitte an die A+W Software GmbH.

### Auftragsformulare
**Stammdaten > Formulare > Auftragsformulare**

*Abb. B-630 Formularverwaltung für den Direktdruck*

In diesem Dialog ordnen Sie Formulare für den Direktdruck zu. Diese Zuordnungen werden im Dialog Dokumentenverwaltung in der Gruppe Druck > Direktdruck aufgelistet.
⇨ Verkauf, "Menü Start" auf Seite C-409

#### Einstellungen
- **Bezeichnung:** Namen, mit dem der Direktdruck in der Dokumentenverwaltung angezeigt wird.
- **Dokumententyp:** Zuordnungen des Direktdrucks zum Dokumententyp. Möglich für:
  - Angebot
  - Auftrag (inkl. AB, Lieferschein, Rechnung etc.)
  - Bestellanfrage
  - Bestellung
  - Gutschrift
- **Druckpunkt:** Druckpunkt, der durch den Druck vergeben wird und den Anwenderstatus des Dokuments setzt.
  ⇨ "Statusverwaltung" auf Seite B-885
- **Drucker:** In der Regel wird der Direktdruck einem Systemdrucker zugeordnet.
- **Formular:** Formular für den Direktdruck.
- **Rückfrage vor Druck:** Der Direktdruck kann wahlweise sofort oder nach einer Abfrage gestartet werden.
  - Der Formulardruck wird sofort und ohne weitere Abfrage gestartet.
  - Nach der Auswahl werden Sie gefragt, ob Sie das Formular drucken möchten (Ja/Nein).

### Druckaufträge
**Stammdaten > Formulare > Druckaufträge**

*Abb. B-631 Druckaufträge*

In diesem Dialog verwalten Sie die Druckaufträge. Sie können über die Definition von Druckaufträgen mehrere Druckläufe hintereinanderschalten, die automatisch auf dem Printserver ausgeführt werden, z. B. Drucken der Auftragsbestätigungen für interne Zwecke.

> **Druckläufe auf dem Printserver anlegen**
> Wenn Sie keinen lokalen Drucker verwenden, erfassen Sie die Druckläufe am besten direkt auf dem Server, da in der Kombobox Drucker nur die auf dem Rechner installierten Drucker angezeigt werden.

#### Druckauftrag
Alle Einstellungen in diesem Bereich gelten jeweils nur für den ausgewählten Druckauftrag.
- **Bezeichnung:** Namen des Druckauftrags, z. B. AB Druck 2-fach.
- **Dokumententyp:** Dokumententyp, für den der Druckauftrag eingerichtet ist.

#### Nummernkreis
- **Nummer aus AV-Bereich Dokument:** Wenn Sie mit Mandanten und/oder AV-Bereichen arbeiten, können Sie festlegen, dass die Dokumenten-Nummer aus zugeordneten Nummernkreisen genommen wird.
  - Mit dieser Einstellung müssen Sie Mandanten und AV-Bereich auswählen.
  - Es wird der Mandant und AV-Bereich aus dem Dokument genommen.
- **Mandant:** Mandant, aus dessen Nummernkreis die Nummer genommen wird.
- **Bereich:** AV-Bereich, aus dessen Nummernkreis die Nummer genommen wird.

#### Formularauswahl
Zu einem Druckauftrag können ein oder mehrere Druckläufe definiert werden. Auf dem Printserver werden diese in der angezeigten Reihenfolge abgearbeitet.

> **Reihenfolge gemäß Statusvergabe**
> Achten Sie bei der Formularzuordnung auf die Reihenfolge im Hinblick auf die Statusvergabe: Nach jedem Drucklauf wird der Status des Dokuments aktualisiert.

- **Formular:** Wählen Sie das Formular aus.
- **Drucker:** Wählen Sie das Gerät aus (z.B. Drucker, Fax).
- **Übersicht:** Zeigt alle Druckläufe des gewählten Druckauftrags an.
- **[Hinzufügen]:** Fügt ein weiteres Formular hinzu.
- **[Entfernen]:** Entfernt ein markiertes Formular.

#### Druckmodus
Wird für Etikettenformulare freigeschaltet.
- **Pro Einheit:** Pro Stück wird ein Etikett gedruckt.
- **Pro Position:** Pro Position wird ein Etikett gedruckt.
- **Pro Auftrag:** Pro Auftrag wird ein Etikett gedruckt.
- **Nach Dokumenteneinstellung:** Die Einstellungen aus dem Dokument werden übernommen.

#### Sonderdruck
- **Wiederholungsdruck:** Aktiv, wenn ein Formular für den Wiederholungsdruck (WH) gewählt wurde.
- **Dokumentenarchivierung:** Dokumente können zusätzlich in einem DMS (z.B. Saperion) archiviert werden.
  - Die Dokumente werden nicht an ein DMS übergeben.
  - Die Dokumente werden automatisch an das angeschlossene DMS übergeben.
    ⇨ "Schnittstellen-Dienst" auf Seite B-1032

#### Sammelausdruck
Rechnungen können als Sammeldruck ausgegeben werden.
- In diesem Druckauftrag werden keine Sammelrechnungen gedruckt.
- Die Dokumente eines Kunden werden beim Druck zusammengefasst. Kriterien:
  - **Immer:** Überschreibt die Einstellung aus den Stammdaten.
  - **Pro Bestelltext 1:** Alle Dokumente werden nach Bestelltext 1 gefiltert und zusammengefasst.
  - **Pro Lieferadresse:** Alle Dokumente mit derselben Lieferanschrift werden zusammengefasst.
  - **Standard:** Alle Dokumente mit demselben Kunden/Lieferanten werden zusammengefasst, wenn das Kennzeichen gesetzt ist.
    ⇨ "Partnerverwaltung - Finanzen" auf Seite B-774
    ⇨ Verkauf: Tutorial, “Sammelrechnungsdruck" auf Seite C-33

#### Einschränkung Betrag
Sie können festlegen, ob der Betrag vor dem Druck abgefragt wird.
- **Alle Dokumente:** Werden gedruckt, Betrag wird nicht geprüft.
- **Betrag ungleich 0:** Dokumente ohne Betrag oder mit Betrag = 0 werden übersprungen.
- **Betrag größer 0:** Nur Dokumente mit Auftragssumme > 0 werden verarbeitet.

- **Nur Postversand:** Der Druckauftrag gilt nur für Dokumente, die per Post versendet werden.
- **Faxversand:** Dokumente werden automatisch als Fax versendet.
- **Faxversand an Vertreter:** Dokumente werden per Fax an den Vertreter gesendet.
- **Mail:** Das gewählte Formular kann als E-Mail gesendet werden.
  - **an Kunde:** Dokument geht an die E-Mail-Adresse des Kunden.
  - **an Vertreter:** Dokument geht an die E-Mail-Adresse des Vertreters.
    ⇨ "Dokumentenversand" auf Seite B-765
    ⇨ "Mitarbeiter" auf Seite B-1008

- **Archivjahr abfragen:** Legt fest, ob das im Formulardruck eingestellte Archivjahr berücksichtigt wird.
- **Druckdatum abfragen:** Legt fest, ob das manuell eingegebene Druckdatum berücksichtigt wird.
- **Nicht optimierte Gläser:** Nur für Etikettenformulare. Legt fest, ob für nicht optimierte Gläser Etiketten gedruckt werden.

### Crystal Reports
**Stammdaten > Formulare > Crystal Reports**

*Abb. B-632 Verfügbare Reports*

In diesem Dialog hinterlegen Sie Hyperlinks zu Crystal Reports *.RPT-Dateien. Zusätzlich können Sie für jeden Report eine Beschreibung eingeben und eine Datenquelle und Mitarbeiter bzw. Mitarbeitergruppen zuordnen. Der Ausdruck der Crystal Reports wird in einem gesonderten Modul erzeugt, das über das A+W Business-Startmenü erreichbar ist.

#### Zuordnung
**Stammdaten > Formulare > Crystal Reports > Report markieren > Kontextmenü (rechte Maustaste) > Mitarbeiter, Gruppe zuordnen**

*Abb. B-633 Zuordnung*

In diesem Dialog ordnen Sie einem Report einen Mitarbeiter oder eine Mitarbeitergruppe zu.

## CEKAL
**Stammdaten > CEKAL**

In Frankreich wird mit dem Zertifikat CEKAL gearbeitet. Isoliergläser, die mit diesem Zertifikat gekennzeichnet sind, müssen definierten Qualitätskriterien entsprechen. Diese Kriterien legen Sie in den Dialogen dieses Menüs fest.

> **Voraussetzungen**
> Die Dialoge zur CEKAL-Zertifizierung sind nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen CEKAL-Klassifizierung ausgewählt ist.
> ⇨ "Produktkennzeichnung" auf Seite B-934

Im Menü CEKAL finden Sie folgende Einträge:
- "Klassen" auf Seite B-1076
- "Zuordnung" auf Seite B-1077
- "Ergebnisse" auf Seite B-1078
- "Textzuordnung" auf Seite B-1079
- "Restriktionen" auf Seite B-1081
- "Produkttexte" auf Seite B-1082

### Klassen
**Stammdaten > CEKAL > Klassen**

*Abb. B-634 CEKAL Klassen*

In diesem Dialog legen Sie Variablen (Platzhalter) für die verschiedenen CEKAL-Klassen an. Sie werden in der Dokumentenerfassung automatisch durch die Texte ersetzt, die aus den CEKAL-Regeln resultieren.

- **Nr.:** Nummer der Klasse.
- **Bezeichnung:** Name der Klasse.
- **Platzhalter:** Selbst definierter Platzhalter (Variable) für die Klasse.
  ⇨ Tutorial 2, "Verfügbare Variablen (Platzhalter)" auf Seite B-525
- **Ebene:** Stücklistenebene, bis zu der die CEKAL-Prüfung durchgeführt werden soll.
  - 0: Prüfung auf Hauptproduktebene
  - 1: Prüfung auf der ersten Stücklistenebene
- **Fremdschlüssel:** Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.

### Zuordnung
**Stammdaten > CEKAL > Zuordnung**

*Abb. B-635 CEKAL-Zuordnung*

In diesem Dialog ordnen Sie jedem einzelnen Glasprodukt, das in eine ISO-Einheit eingebaut wird, eine Klasse zu und tragen den dazugehörigen Wert ein.
- **Produkt:** Produkt, dem eine Klasse zugeordnet ist.
- **Klasse:** Zugeordnete Klasse.
- **Ebene:** Strukturseite, für die die Zuordnung gilt.
- **Wert:** CEKAL-Wert des Produkts.
- **Bemerkung:** Bemerkung zur weiteren Information.

### Ergebnisse
**Stammdaten > CEKAL > Ergebnisse**

*Abb. B-636 CEKAL Ergebnisse*

In diesem Dialog können Sie die CEKAL-Werte, die Sie im Dialog Zuordnung den unterschiedlichen Produkten zugeordnet haben, miteinander kombinieren. Aus diesen Kombinationen resultieren die verschiedenen CEKAL-Ergebnisse.

#### Zuordnung
- **Klasse:** Klasse, für die das Ergebnis angelegt ist.
- **Ergebnis:** Bezeichnung für das Ergebnis.
- **Bemerkung:** Bemerkung zur Zuordnung.

#### Elemente
- **Elemente 1 - 10:** Pro CEKAL-Ergebnis können Sie maximal 10 unterschiedliche CEKAL-Werte zuordnen.

### Textzuordnung
**Stammdaten > CEKAL > Textzuordnung**

*Abb. B-637 CEKAL Textzuordnung*

In diesem Dialog geben Sie an, welche Texte bei welchen Ergebnissen gedruckt werden sollen.

#### Klassen
- **Klasse 1 bis 10:** Ergebnis, zu dem ein Text ausgegeben werden soll.

#### Bieger
- **Nummer:** Textnummer, die an den Bieger übergeben werden soll.

#### Texte
- **Allgemein:** Dieser Text wird auf den Formularen gedruckt (bis zu 80 Zeichen).
- **Etikett:** Dieser Text wird auf den Etiketten gedruckt.
- **Produktion:** Dieser Text wird auf den Produktionspapieren gedruckt.
- **Bieger:** Dieser Text kann an den Rahmenbieger übergeben werden.

### Restriktionen
**Stammdaten > CEKAL > Restriktionen**

*Abb. B-638 CEKAL Restriktionen*

In diesem Dialog hinterlegen Sie die Restriktionen, die bei der CEKAL-Prüfung berücksichtigt werden. Bei Über- oder Unterschreitung der Werte erfolgt keine CEKAL-Klassifizierung.

#### Restriktionswerte
- **Nummer:** Die Nummern sind vom System vorgegeben.
- **Parameter 1 bis 4:** Werte für die einzelnen Parameter der Restriktion.
- **Bemerkung:** Anzeige der vorgegebenen Texte zur Restriktion.

#### Texte
- **Allgemein:** Dieser Text wird auf den Formularen gedruckt (bis zu 80 Zeichen).
- **Etikett:** Dieser Text wird auf den Etiketten gedruckt.
- **Produktion:** Dieser Text wird auf den Produktionspapieren gedruckt.
- **Bieger:** Dieser Text kann an den Rahmenbieger übergeben werden.

### Produkttexte
**Stammdaten > CEKAL > Produkttexte**

*Abb. B-639 CEKAL-Produkttexte*

In diesem Dialog hinterlegen Sie für spezielle Produkte CEKAL-Texte, die sich auf eine bestimmte Strukturebene beziehen. Wenn ein solches Produkt Bestandteil einer Isolierglaseinheit ist, hat dieser CEKAL-Text absolute Priorität vor den anderen CEKAL-Texten.

#### Produktauswahl
- **Produkt:** Produkt, dem ein spezieller Produkttext zugeordnet ist.
- **Ebene:** Strukturebene, für die der Text gilt.
- **Bemerkung:** Kurze Beschreibung, die den Text erläutert.

#### Texte
- **Allgemein, Etikett, Produktion, Bieger:** Siehe vorherige Abschnitte.

## CE-Kennzeichen
**Stammdaten > CE-Kennzeichen**

Isoliergläser, die mit diesem Zertifikat gekennzeichnet sind, müssen fest definierten Qualitätskriterien entsprechen. Der CPIP-Code (Characteristic Performance Identification Paper) wird nur in Frankreich benötigt.

Im Menü CE-Kennzeichen finden Sie folgende Einträge:
- "CPIP-Code" auf Seite B-1084
- "Maßrestriktionen" auf Seite B-1085
- "ISO-Suchdaten" auf Seite B-1086
- "Restriktionen" auf Seite B-1081
- "Einstellungen" auf Seite B-1087

### CPIP-Code
**Stammdaten > CE-Kennzeichen > CPIP-Code**

*Abb. B-640 CE-Kennzeichen - CPIP-Code*

In diesem Dialog legen Sie Details zu einem CPIP-Code fest, z. B. die Gültigkeit, ob er zertifiziert wurde und ob er einer CE-Norm entspricht.
Die Standards und Regeln zur CPIP-Bildung können im Dialog Einstellungen eingelesen werden.
⇨ "Einstellungen" auf Seite B-1087

### Maßrestriktionen
**Stammdaten > CE-Kennzeichen > Maßrestriktionen**

*Abb. B-641 CE-Kennzeichen - Maßrestriktionen*

In diesem Dialog hinterlegen Sie die Maßrestriktionen für CPIP-Codes. Während der Auftragserfassung wird geprüft, ob CE relevante Maßrestriktionen überschritten sind.

### ISO-Suchdaten
**Stammdaten > CE-Kennzeichen > ISO-Suchdaten**

*Abb. B-642 ISO-Suchdaten*

In diesem Dialog pflegen Sie die Daten für den CPIP-Code für Isoliergläser. Diese Daten steuern das Verhalten der Auftragserfassung.

### Einstellungen
**Stammdaten > CE-Kennzeichen > Einstellungen**

*Abb. B-643 CE-Kennzeichen – Einstellungen*

In diesem Dialog importieren Sie die Dateien mit den erforderlichen CPIP-Codes und weiteren Definitionen.

#### Standardwerte für ISO-Suchfunktion
Hier werden die Standard-Werte für Nicht-Glas-Komponenten gepflegt.

#### Datei-Update CPIP-Code
Hier können Datenbank-Tabellen über Schnittstellendateien gefüllt werden.

## B2B
**Stammdaten > B2B**

In diesem Programmbereich sind Schnittstellen-Daten für den Datenaustausch hinterlegt.

Im Menü **B2B** finden Sie folgende Einträge:
- "Produkte (Kunde, Lieferant)" auf Seite B-1088
- "Kopieren von Fremdartikeln" auf Seite B-1095
- "SZR (Kunde, Lieferant)" auf Seite B-1096
- "Gas (Kunde, Lieferant)" auf Seite B-1097
- "Touren (Kunde, Lieferant)" auf Seite B-1098
- "Kunde, Lieferant" auf Seite B-1099
- "Dokumentenexport" auf Seite B-1105
- "SN-Datei-Regeln" auf Seite B-1107
- "Artikelimport" auf Seite B-1108
- "Preisimport" auf Seite B-1110

### Produkte (Kunde, Lieferant)
**Stammdaten > B2B > Kunde, Lieferant > Produkt**

Aufträge können über EDI importiert und Bestellungen können exportiert werden. Für Kunden und Lieferanten werden die Produktdaten für diesen Datenaustausch getrennt gepflegt.

#### Menü Funktionen
- **Dorma-Referenz erstellen:** Bezüge zu den Dorma-Artikeln erstellen. Nur für Lieferanten freigeschaltet.
- **Artikel kopieren:** Öffnet den Dialog Kopieren von Fremdartikeln.
  ⇨ "Kopieren von Fremdartikeln" auf Seite B-1095

#### Produkte – Stückliste
**Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Stückliste**

*Abb. B-644 Produkte – Stückliste*

In diesem Register ordnen Sie die eigenen Glas-Produkte den Produkten des Marktpartners zu.

- **Fremdartikel:** Partner, Gültigkeitsdatum, Artikelnummer und Bezeichnung des Marktpartners.
- **Identifikation:** Artikel/MCode, Bezeichnung, Maße, Farbe und Preis des eigenen Produkts.
- **Stücklistenartikel:** Details der markierten Komponente aus der Stückliste.
- **Stückliste:** Übersicht der Stückliste des ausgewählten Produkts.

#### Produkte – Parameter
**Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Parameter**

*Abb. B-645 Produkte - Parameter*

In diesem Register geben Sie an, ob bei der Rechnungskontrolle die korrespondierende Produktnummer automatisch gesucht und eingetragen wird.

#### Produkte – Tabelle
**Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Tabelle**

*Abb. B-646 Produkte - Tabelle*

In diesem Register werden alle zugeordneten Produkte aufgelistet.

#### Produkte – Modelle/Bearbeitungen
**Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Modelle/Bearbeitungen**

*Abb. B-647 Produkte - Modelle/Bearbeitungen*

In diesem Register legen Sie die Parameter für Modelle und Bearbeitungen fest.
⇨ "Produktverwaltung - Modelle/Bearbeitungen" auf Seite B-613

#### Produkte – Sprossen
**Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Sprossen**

*Abb. B-648 Produkte - Sprossen*

In diesem Register legen Sie die Parameter für Sprossen(-Konstruktionen) fest.
⇨ "Produktverwaltung - Sprossen" auf Seite B-627

### Kopieren von Fremdartikeln
**Stammdaten > B2B > Kunde, Lieferant > Produkt > Menü Funktionen > Artikel kopieren**

*Abb. B-649 B2B - Kopieren von Fremdartikeln*

In diesem Dialog können Sie die Daten eines Partners kopieren und auf einen anderen Partner übertragen.

### SZR (Kunde, Lieferant)
**Stammdaten > B2B > Kunde, Lieferant > SZR**

*Abb. B-650 B2B - Abstandhalter (SZR)*

In diesem Dialog ordnen Sie die eigenen SZR-Produkte den Produkten des Marktpartners zu. Die Dialoge für Kunden und Lieferanten sind identisch aufgebaut.

### Gas (Kunde, Lieferant)
**Stammdaten > B2B > Kunde, Lieferant > Gas**

*Abb. B-651 B2B-Gas*

In diesem Dialog ordnen Sie die eigenen Gas-Produkte den Produkten des Marktpartners zu.

### Touren (Kunde, Lieferant)
**Stammdaten > B2B > Kunde, Lieferant > Touren**

*Abb. B-652 B2B - Touren*

In diesem Dialog ordnen Sie die eigenen Touren den Touren des Marktpartners zu.

### Kunde, Lieferant (EDI)
**Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant**

Für Kunden und Lieferanten werden die Einstellungen für den Datenaustausch per EDI getrennt gepflegt.

#### Kunde, Lieferant – Auswahl
**Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant > Register Auswahl**

*Abb. B-653 B2B - Partnerauswahl*

In diesem Register legen Sie die Einstellungen für die EDI-Schnittstelle pro Marktpartner fest.

- **Partner:** Nummer des Marktpartners.
- **Filialnummer:** Nummer der Filiale des Marktpartners.
- **Abweichender Partner für Artikelreferenzierung:** Nummer des Marktpartners, auf dessen Artikel verwiesen wird.
- **Schnittstelle Typ:** Schnittstellenversion.
- **Laufnummer der Zieldatei:** Nummernkreis für die Laufnummern der Übergabe.
- **Pfadangaben:** Quellpfad, Quelldatei, Protokollpfad, Sicherungspfad.
- **Eine Datei pro Dokument (nur Lieferanten):**
  - Alle Bestellungen eines Lieferanten werden in eine Datei geschrieben.
  - Beim Export wird eine Datei pro Bestellung erzeugt.
- **Command-Skript:** Hier kann ein Skript eingetragen werden, um EDI-Dateien zu modifizieren und zu kopieren.

