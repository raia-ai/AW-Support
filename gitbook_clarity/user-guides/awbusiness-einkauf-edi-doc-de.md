---
description: "DE_AWBusiness_Einkauf_3_4"
---


# Tutorial: Elektronischer Dokumentenaustausch

---
## Export/Import (openTRANS)

### Lernziele
- Funktionsweise des elektronischen Dokumentenaustauschs kennenlernen.
- Voreinstellungen kennenlernen und anpassen.
- Pflichtfelder in Dokumenten kennenlernen.
- Elektronische Dokumente senden und einlesen.

### Nutzen
- Mit dem elektronischen Dokumentenaustausch können Sie Dokumente Ihrer Kunden und Lieferanten einlesen, ohne die Daten einzeln erfassen zu müssen.
- Mit dem Einlesen von Daten vermindern sich Fehler bei der Erfassung.

### Merke

**Voraussetzung**
- Beim Lieferanten/Kunden und Ihnen muss die gleiche Version von A+W Business installiert sein, mindestens A+W Business 5.
- Die notwendigen Dienste müssen installiert und gestartet sein.

**Datenformat**
- Elektronische Dokumente können in den Formaten openTRANS und XML ausgetauscht werden.

**Datenimport**
- Die Daten können als Datei per E-Mail gesendet oder auf einem gemeinsamen freigegebenen Laufwerk auf einem Server gespeichert werden.

**Datenexport**
- Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird geprüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Diese Dokumente werden dann automatisch an die hinterlegte E-Mail-Adresse gesendet.

**Referenzen**
Dokumentenreferenzen werden aus folgenden Feldern gebildet:
- Im Auftragskopf Feld `Bestelltext1`
- In der Positionserfassung Feld `Kundenposition`.
Diese Felder müssen daher immer gefüllt sein.
Wenn diese Referenzen in eingelesenen Dokumenten nicht hergestellt werden können, muss die Zuordnung beim Prüfen des elektronischen Dokuments manuell nachgeholt werden.

**Teillieferungen**
- Aus einer elektronischen AB können Teillieferungen erstellt werden.

**Rundungsdifferenzen**
- Bei der Preis- und Rechnungskontrolle können Rundungsdifferenzen im Cent-Bereich akzeptiert werden, wenn in der Produktverwaltung ein Ausgleichsprodukt angelegt ist, dem diese Differenzen zugeordnet werden können.

**Sammelrechnungen**
- Bei Sammelrechnungen des Lieferanten kann ein einmal aufgeführter Zuschlag auf alle Positionen der zugehörigen Bestellungen oder Bestellpositionen verteilt werden.

**Dokumentensperre**
- Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt.

**Voreinstellungen**
- **Stammdaten:**
    - Produktdaten
    - Kunden-/Lieferantendaten
    - Statusdefinition
    - Statuszuordnung
    - Währungen
- **Firmendaten:**
    - Register Parameter
- **Stammdaten:**
    - B2B Kunde/Lieferant

### Dokumentenaustausch
Auftragsbestätigungen und Rechnungen können im openTRANS-Format exportiert und importiert werden. Dieses Format wurde für A+W Business erweitert. Es können jedoch auch Dokumente im Standard-Format und XML-Dateien eingelesen werden.
Der Datenaustausch über das openTRANS-Format setzt voraus, dass beim Lieferanten/Kunden und Ihnen die gleichen Versionen von A+W Business installiert sind, mindestens A+W Business 5. Außerdem müssen in der Schnittstellenverwaltung die Parameter beim Lieferanten/Kunden genauso festgelegt werden wie in Ihrem A+W Business.

### Dokumenten-Export
Der Export von Auftragsbestätigungen und Rechnungen wird pro Kunde/Lieferant im Modul Stammdaten > B2B konfiguriert. Dazu wird festgelegt, ob und welche Dokumente exportiert werden sollen und welcher Modus dazu verwendet wird.

*Abb. D-95: Einstellungen für den elektronischen Datenaustausch*
- **A Export-Modus:**
    - **Automatischer Versand per E-Mail:** Dazu muss im Netzwerk ein E-Mail-Server zur Verfügung stehen. Standardmäßig wird die E-Mail-Adresse aus den Stammdaten des Kunden/Lieferanten verwendet. Für Auftragsbestätigungen und für Rechnungen können aber auch abweichende E-Mail-Adressen hinterlegt werden.
    - **Ablage in einem bestimmten Verzeichnis (auf dem Server):** Diese Dateien können anschließend manuell übermittelt werden.
- **B Export-Format**
- **C Auswahl der Dokumente**
- **D Einstellungen für E-Mail-Modus**

Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird geprüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Der eigentliche Export wird über einen Dienst zyklisch im Hintergrund durchgeführt. Zur Kontrolle werden die entsprechenden Dokumente im Dialog Export angezeigt. Durch den Export werden folgende Dateien erzeugt:
- `RESPONSExxxx.awotres` für Auftragsbestätigungen.
- `DISPATCHxxxx.awotdis` für ein Liefer-Avis.
- `INVOICExxxx.awotinv` für Rechnungen.
Bei den Dateinamen wird zwischen Groß- und Kleinschreibung unterschieden.

### Dokumentenreferenzen
Die Dokumentenreferenzen auf Positionsebene werden benötigt, um Auftragspositionen automatisch ihren jeweiligen Bestellpositionen zuzuordnen (Referenzierung). Bei der manuellen Erfassung eines Auftrags werden diese Dokumentenreferenzen automatisch aus den Feldern `Bestelltext1` im Auftragskopf und `Kundenposition` in der Positionserfassung gebildet.

*Abb. D-96: Referenzen für den Datenaustausch*
- **A Kopfdaten – Dokument**
- **B Positionen – Register Position**

Außerdem muss in den Firmendaten im Register Parameter die Option `Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen` aktiviert sein.

*Abb. D-97: Firmendaten - Parameter*

### Dokumenten-Import
Auftragsbestätigungen und Rechnungen im openTRANS-Format werden über das A+W openTRANS ImportTool importiert. Es wird standardmäßig auf dem A+W Business-Client installiert.
Zum Einlesen stehen damit unterschiedliche Möglichkeiten zur Verfügung:
- Doppelklick auf die gespeicherte Datei.
- Doppelklick auf die als E-Mail-Anhang gesendete Datei.

Durch den Doppelklick werden die Daten in die Datenbank importiert und können in den Import-Dialogen von A+W Business angezeigt werden.
Wenn die Dateien auf der Festplatte abgelegt sind, so kann über das Kontextmenü die Option Anzeigen gestartet und eine generische Ansicht des Dokuments angezeigt werden.

#### XML-Dateien
XML-Dateien können nicht direkt aus dem E-Mail-Client heraus eingelesen werden. Diese Dateien müssen zunächst gespeichert werden. Danach können sie über das Kontextmenü eingelesen oder als generische Ansicht angezeigt werden.
Nachdem ein Dokument erfolgreich eingelesen wurde, steht es im jeweiligen Dialog `Elektr. Preiskontrolle` oder `Elektr. Rechnungskontrolle` zur Verfügung.

### Dokumentenkontrolle
Die Dialoge `Elektr. Preiskontrolle` und `Elektr. Rechnungskontrolle` sind identisch aufgebaut.

*Abb. D-98: Elektronische Rechnungskontrolle*
- **A Eingelesenes Dokument**
- **B Anzeige- und Filtereinstellungen**
- **C Status**
- **D Referenzierte Dokumente**

In beiden Dialogen werden alle Dokumente (D) einschließlich möglicher Teillieferungen angezeigt, die mit dem importierten Dokument (A) verknüpft sind. Zu jeder Bestellung wird optisch signalisiert (C), ob die Verknüpfungen zwischen Bestellung und importiertem Dokument vollständig sind. Nur vollständig referenzierte Dokumente können akzeptiert werden.
Wenn das importierte Dokument akzeptiert wurde, wird der Status der referenzierten Bestellungen entsprechend umgesetzt. Die Preis- oder Rechnungskontrolle kann dann nicht nochmals durchgeführt werden.

#### Buchungsarten
Bei der Kontrolle der importierten Dokumente werden je nach Status die Optionen `Akzeptieren`, `Teillieferung erstellen` und `Ablehnen` angeboten.
Die Buchungsart `Akzeptieren` ist nur dann freigeschaltet, wenn ein importiertes Dokument vollständig und fehlerfrei referenziert ist. Wenn nur die Bestellmengen nicht vollständig referenziert sind, das Dokument jedoch ansonsten vollständig ist, so kann über die Buchungsart automatisch eine Teillieferung erzeugt werden.

### Positionszuordnung
Sind in einem openTRANS-Dokument die Bestellreferenzen fehlerhaft oder gar nicht vorhanden, kann das System Dokumenten- und Bestellpositionen nicht automatisch miteinander verknüpfen. Diese (nicht verknüpften) Positionen werden in der Positionsübersicht gekennzeichnet und müssen manuell verknüpft werden.
In der Rechnung kann z. B. die Referenz zu einer Position fehlen oder fehlerhaft aufgeführt sein. Anhand der Produktbezeichnungen können Sie diese Referenzen im Dialog Positionen manuell zuordnen herstellen.

### Fußzuschläge/-rabatte
Fußzuschläge oder -rabatte werden im Normalfall nicht in der Bestellung erfasst. In der Auftragsbestätigung oder Rechnung sind sie jedoch aufgeführt. Um eine Rechnungskontrolle durchführen zu können, müssen diese Positionen in den Bestellungen nachträglich erfasst werden. Dazu kann die Bestellerfassung aus dem Dialog Rechnungskontrolle heraus geöffnet werden. Nachdem der Zuschlag in der Bestellung eingefügt ist, muss er in der Rechnung zugeordnet werden.
Wenn mehrere Bestellungen vom Lieferanten in einer Rechnung zusammengefasst sind, in der ein Fußzuschlag/-rabatt nur einmal aufgeführt ist, so kann diese Position auf alle verknüpften Bestellungen verteilt werden. Das Programm versucht, für die anteiligen Beträge anhand der Zuschlagsbasis sinnvolle Vorschlagswerte zu finden und bietet diese an. Diese Werte können überschrieben werden.
Außerdem können die Fußzuschläge/-rabatte anhand der Produktnummer für diesen Lieferanten automatisch zugeordnet werden. Dabei wird die Zuordnung der Produktnummer des Lieferanten zur eigenen Produktnummer gespeichert.

### Sammelrechnungen in A+W Business
Wenn in A+W Business Sammelrechnungen erstellt werden, so werden für jeden Auftrag die Fußzuschläge/-rabatte als eigene Position aufgeführt. Da eine direkte manuelle Zuordnung oft schwer ist, können in diesem Fall mehrere Dokumentenpositionen zusammengefasst und den Bestellpositionen zugeordnet werden. In der Positionsübersicht ist anschließend nur noch die zusammengefasste Dokumentenposition aufgeführt.

### Betragsdifferenzen
Üblicherweise können Sie eine Rechnung nur akzeptieren, wenn keine Differenzen auftreten. Wenn Sie bei einem Lieferanten mit Betragsdifferenzen rechnen (müssen), können Sie diese auf unterschiedliche Weise behandeln:
- Sie können die Rechnung ablehnen und den Lieferanten über die Unstimmigkeiten (telefonisch) informieren.
- Betragsdifferenzen können auch durch unterschiedliche Rundungen entstehen. Mit der Option `Betragsdifferenzen akzeptieren` können Sie die Rechnungskontrolle trotz solcher Differenzen durchführen. Die Differenz darf sich nur im Cent-Bereich bewegen. Sie sollten sich mit der Option `Hinweis auf Betragsdifferenz/Ausgleichsposition` darauf aufmerksam machen lassen.
- Die Rundungsdifferenzen im Cent-Bereich können automatisch akzeptiert werden. Dazu muss ein sogenanntes Ausgleichsprodukt angelegt sein, auf das der Differenzbetrag gebucht werden kann.
- Mit der Funktion `Prod.Nr. für Ausgleichspos.` können Sie ein Produkt auswählen, auf das Rundungsdifferenzen (im Cent-Bereich) verbucht werden sollen.

### Dienste prüfen
Folgende Dienste müssen installiert und gestartet sein:
- **A+W Business 6 Interface Service**
  - Dieser Dienst wird in aller Regel auf einem separaten Rechner installiert. Bei der Installation durch einen Service-Mitarbeiter der A+W Software GmbH muss die Funktion `Interface Service handles B2B documents` aktiviert werden.
- **AWProtocol:**
  - Diesen Dienst finden Sie unter `Systemsteuerung > Verwaltung > Dienste`.
- **ERP-WebService:**
  - Diesen Service finden Sie unter `Systemsteuerung > Computerverwaltung > Dienste und Anwendungen > Sites > Default Web Site`.

*Abb. D-99: ERP-Service prüfen*

Die Dienste werden in der Regel mit A+W Business zusammen installiert. Sie sind auf den Starttyp `Automatisch` eingestellt. Dadurch sollten sie beim Start des Rechners automatisch gestartet werden.
Wenn der Datenaustausch nicht funktioniert, sollten Sie die Dienste prüfen und ggf. manuell starten. Eine Anleitung dazu finden Sie in der Online-Hilfe des Betriebssystems.
Außerdem benötigen Sie das `A+W openTRANS ImportTool`, das vom A+W Business-Setup automatisch installiert wird.

### Statusvergabe
Der Status der Dokumente wird auch beim Im- und Export umgesetzt. Dazu müssen folgende Statuspunkte zugeordnet sein.

| Statuspunkte für Import | Statuspunkte für Export |
| :--- | :--- |
| 61 - Auftragsbestätigung nicht akzeptieren | 830 - Rechnungsexport |
| 64 - Rechnung nicht akzeptieren | 840 - Auftragsbestätigungsexport |

Beim Import wird der Status manuell umgesetzt, beim Export automatisch.
Im Part Stammdaten sind die Statuspunkte und Statuszuordnungen ausführlich beschrieben. In dieser Einheit wird daher nur auf die Besonderheiten eingegangen, die Sie für den Austausch von elektronischen Dokumenten beachten müssen.

### Voreinstellungen für Datenaustausch prüfen

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Firmendaten**
1. Wählen Sie `Stammdaten > Firma > Firmendaten` und wechseln Sie zum Register `Parameter`.
   *Abb. D-100: Firmendaten – Parameter*
2. Aktivieren Sie die Checkbox `Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen`.
3. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Die Daten werden gespeichert.
(⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-936)

### Währungseinstellungen prüfen
Für die Währungen, die in den Aufträgen und Bestellungen verwendet werden, muss das internationale Währungskennzeichen hinterlegt sein. Die Einstellungen müssen Sie prüfen, wenn Sie mit mehreren Währungen arbeiten.

**So prüfen Sie die Währungseinstellungen**
1. Wählen Sie `Stammdaten > Finanzen > Währung`.
   *Abb. D-101: Internationales Währungskennzeichen*
   - **A Wechselkurs für Umrechnung von Preisen**
   - **B Internationales Währungskennzeichen**
   (⇨ Stammdaten, "Währung" auf Seite B-909)
2. Jeder Währung muss das internationale Kennzeichen (B) zugewiesen sein. Markieren Sie die Zeile der Währung, der Sie das Kennzeichen zuweisen wollen.
3. Öffnen Sie in der Spalte `Internat. Kennzeichen` die Kombobox und wählen Sie aus der Liste das entsprechende Kennzeichen aus.
4. Prüfen Sie die jeweils eingetragenen Wechselkurse (A) und aktualisieren Sie diese ggf.
5. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Die Daten werden gespeichert.

### Statusdefinitionen prüfen
Damit die elektronischen Dokumente verarbeitet werden können, müssen die Statuspunkte 61, 64, 830, 840 definiert und zugeordnet sein. Diese Statuspunkte werden für folgende Aktionen benötigt:
- Dokumente ex- und importieren.
- Importiertes Dokument ablehnen oder akzeptieren.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So prüfen Sie die Statuspunkte" auf Seite D-163
- "So prüfen Sie die Statusverwaltung" auf Seite D-164
- "So prüfen Sie die Statuszuordnung" auf Seite D-165

**So prüfen Sie die Statuspunkte**
1. Wählen Sie `Stammdaten > Auftrag > Statuspunkte`.
   *Abb. D-102: Statuspunkte*
   (⇨ Stammdaten, "Statuspunkte" auf Seite B-886)
2. Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 vorhanden sind. Die Nummern der Statuspunkte sind in der Spalte `Kennz.` angegeben. In der Regel werden die Statuspunkte mit der Installation zusammen erstellt. Sie müssen immer manuell zugeordnet werden.
3. Wenn diese Statuspunkte nicht vollständig vorhanden sind, legen Sie die fehlenden an.
4. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Die Daten werden gespeichert. Diese Statuspunkte müssen einem entsprechenden Anwenderstatus zugeordnet sein.

**So prüfen Sie die Statusverwaltung**
1. Wählen Sie `Stammdaten > Auftrag > Statusverwaltung`.
   *Abb. D-103: Statusverwaltung*
   (⇨ Stammdaten, "Statusverwaltung" auf Seite B-885)
   Wenn die Anwenderstatus 61/64 und 830/840 nicht vollständig vorhanden sind, legen Sie die fehlenden an.
2. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Prüfen Sie als Nächstes, ob alle Zuordnungen vorhanden und vollständig sind.

**So prüfen Sie die Statuszuordnung**
1. Wählen Sie `Stammdaten > Auftrag > Statuszuordnung`.
   *Abb. D-104: Statuszuordnung*
   - **A Statuspunkt**
   - **B Dokumententyp**
   - **C Zugeordneter Anwenderstatus**
   (⇨ Stammdaten, "Statuszuordnung" auf Seite B-887)
2. Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 zugeordnet sind. Wenn Sie in der Tabelle `Statuszuordnung` einen Statuspunkt markieren, muss mindestens der Anwenderstatus (C) angezeigt werden. Wenn diese Statuspunkte nicht vollständig zugeordnet sind, holen Sie die Zuordnung nach.
3. Wählen Sie im Menü `Start > Neu`, um in den Erfassungs-Modus zu wechseln.
4. Wählen Sie in den Feldern `Statuspunkt`, `Dokumententyp` und `Anwenderstatus` die entsprechenden Einträge aus.
5. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Die Daten werden gespeichert.

### Datenexport per openTRANS einstellen
Im Modul `Stammdaten > B2B` müssen Sie festlegen, wie die Daten ausgetauscht werden sollen.

**So legen Sie die Exportart für openTRANS fest**
1. Wählen Sie `Stammdaten > B2B > Kunde > Dokumentenexport`. Der Dialog `openTRANS-Dokumentenexport` wird mit dem Register `Auswahl` angezeigt.
2. Wählen Sie im Menü `Start > Suchen`, um in die Kunden einzulesen. Die Kunden werden im Register `Tabelle` aufgelistet.
3. Markieren Sie den Kunden (C), mit dem Dokumente über das openTRANS-Format ausgetauscht werden sollen.
4. Wechseln Sie zum Register `Auswahl`.
   - Wenn die Angaben für den Kunden korrekt sind, können Sie den nächsten Kunden prüfen.
   - Wenn keine Angaben vorhanden sind, müssen Sie diese einpflegen.
   *Abb. D-105: openTRANS-Dokumentenexport*
   - **A Exportart per Datei oder per E-Mail**
   - **B Übertragungstyp**
   - **C Kundennummer**
   - **D Auswahl der Dokumentenart**
   - **E E-Mail-Adressen für unterschiedliche Dokumentenarten**
5. Wählen Sie im Feld `Typ` (B) den Eintrag `Standard (openTRANS basierend)` aus. Mit dieser Einstellung erhalten die Dokumente für diesen Kunden automatisch das Kennzeichen für den openTRANS-Austausch.
6. Wählen Sie im Feld `Exportart` (A) aus, wie die Dateien ausgetauscht werden sollen.
   - **Export in eine Datei:** Mit dieser Einstellung werden die Daten in eine Datei geschrieben. Die Felder für den Zielpfad werden freigeschaltet. Sie können ein Verzeichnis auswählen oder den Pfad manuell eintragen.
   - **Export per E-Mail:** Mit dieser Einstellung werden die Daten als Anhang einer E-Mail gesendet. Dazu müssen Sie prüfen, ob in den Stammdaten des Kunden die E-Mail-Adresse korrekt eingetragen ist. (⇨ "Partnerstammdaten prüfen" auf Seite D-168)
7. Wählen Sie aus, ob Auftragsbestätigungen und/oder Rechnungen (D) exportiert werden sollen.
8. Wenn Sie die Daten per E-Mail senden, können Sie abweichende E-Mail-Adressen (E) für Auftragsbestätigungen, Rechnungen und/oder Lieferavis eintragen.
9. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Die Daten werden gespeichert.
10. Wiederholen Sie die Schritte 3 bis 9 für alle Kunden, mit denen Sie Daten austauschen.

Um Auftragsbestätigungen und Rechnungen Ihrer Lieferanten importieren zu können, brauchen Sie keine weiteren Einstellungen festzulegen.

### Partnerstammdaten prüfen
In den Stammdaten der Lieferanten/Kunden müssen die Daten für die Kommunikation korrekt hinterlegt sein, damit Dokumente direkt aus A+W Business heraus versendet werden können.

**So prüfen Sie die Lieferanten-/Kundendaten**
1. Wählen Sie `Stammdaten > Marktpartner > Lieferant, Kunde > Lieferanten, Kunden`.
   *Abb. D-106: Partnerdaten - Adresse*
   (⇨ Stammdaten, "Partnerverwaltung" auf Seite B-759)
2. Prüfen Sie, ob die E-Mail-Adresse des Lieferanten, Kunden korrekt ist. Wenn Ihr Lieferanten oder Kunden mehrere E-Mail-Adressen haben, können Sie in den Einstellungen für den Dokumentenaustausch auch alternative E-Mail-Adressen eingeben. (⇨ "Datenexport per openTRANS einstellen" auf Seite D-166)
3. Wechseln Sie zum Register `Auftrag` und prüfen Sie, ob die externe Nummer eingetragen ist.
   *Abb. D-107: Partnerdaten – Auftrag*
   In den Kunden- und Lieferantendaten hat diese Nummer folgende Bedeutung:
   - **Lieferantendaten:** Die externe Kundennummer erhalten Sie von Ihrem Lieferanten. Sie muss auch dann eingetragen werden, wenn sie mit Ihrer internen Nummer identisch ist.
   - **Kundendaten:** In den Stammdaten zu Ihren Kunden muss in diesem Feld die Nummer stehen, die Sie bei Ihrem Kunden als Lieferant kennzeichnet.
4. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.

### Elektronisches Dokument einlesen
Elektronische Dokumente können Sie in zwei Formaten erhalten haben: als openTRANS-Datei oder als XML-Datei. Je nach den Einstellungen in Ihrem Betrieb sind diese Dateien in einem bestimmten Verzeichnis auf dem Server abgelegt oder als Anhang einer E-Mail verfügbar.

**So lesen Sie ein openTRANS-Dokument ein**
1. Öffnen Sie das Verzeichnis mit den gesendeten Dateien oder die E-Mail, mit der die Datei gesendet wurde. Die openTRANS-Datei hat die Dateiendung `*.awotdis`, `*.awotres` oder `*.awotinv`.
2. Starten Sie den Import mit einem Doppelklick auf die Datei. Die Daten werden eingelesen und in den Dialogen für die elektronische Preis- oder Rechnungskontrolle angezeigt.

**So lesen Sie ein XML-Dokument ein**
1. Öffnen Sie das Verzeichnis mit den gesendeten Dateien oder die E-Mail, mit der die Datei gesendet wurde.
2. Speichern Sie die XML-Datei auf Ihren Rechner.
3. Wählen Sie die Datei im Explorer aus und öffnen Sie das Kontext-Menü.
4. Wählen Sie die Option `Als openTRANS-Dokument einlesen`. Die Daten werden eingelesen und in den Dialogen für die elektronische Preis- oder Rechnungskontrolle angezeigt.

### Elektronisches Dokument prüfen
Sie können in importierten Dokumenten Ihrer Lieferanten die Preise sowohl in der Auftragsbestätigung als auch in der Rechnung prüfen. Dazu stehen zwei Dialoge zur Verfügung, die im Aufbau und den Funktionen identisch sind:
- Elektronische Preiskontrolle
- Elektronische Rechnungskontrolle

Die Handlungsschritte werden im Folgenden am Beispiel der elektronischen Rechnungskontrolle beschrieben.

**So prüfen und akzeptieren Sie eine importierte Lieferantenrechnung**
1. Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`.
   *Abb. D-108: Elektronische Rechnungskontrolle – Dokumentenimport*
   - **A Optionen für die Buchungsart**
   - **B Einschränkung der Anzeige**
   - **C Status des markierten Dokuments**
   - **D Hinweis zu Diskrepanzen**
   - **E Filterung der angezeigten Dokumente**
   - **F Referenzierte Dokumente**
2. Schränken Sie die Anzeige ein, wenn zu viele Dokumente angezeigt werden:
   - Wählen Sie für die Anzeige (B) den Eintrag `Nur offene Dokumente`.
   - Klicken Sie auf die Schaltfläche (E) und stellen Sie die gewünschten Filter ein. Im Dialog `Filtereinstellungen` können Sie mehrere Lieferanten auswählen und mit [OK] übernehmen. (⇨ Softwarereferenz, "Filtereinstellungen" auf Seite D-223)
3. Markieren Sie eine der angezeigten Rechnungen. In der Übersicht `Bestellungen/Teillieferungen` (F) werden alle Bestellungen aufgelistet, die zu dieser Rechnung gehören. Im Bereich `Dokumentenstatus` (C) können Sie sehen, ob Referenzen fehlen und/oder Differenzen in Preisen oder Mengen auftreten.
   - Wenn Sie Preisdifferenzen nicht akzeptieren wollen, wählen Sie die Option `Ablehnen` (A) und schicken Sie die Rechnung zurück. Das Dokument wird als abgelehnt gekennzeichnet und kann archiviert werden.
   - Korrigieren Sie die Differenzen wie in den folgenden Handlungsschritten erläutert wird.
   - Stellen Sie die fehlenden Referenzen her. (⇨ "So ordnen Sie Positionen in einer importierten Rechnung zu" auf Seite D-173)
4. Wechseln Sie ggf. zum Register `Positionsübersicht`, um die Differenzen der Einkaufspreise einzelner Positionen zu prüfen. Wenn Betragsdifferenzen durch unterschiedliche Rundungen aufgetreten sind, können Sie diese über `Menü Optionen > Betragsdifferenzen akzeptieren` generell zulassen. In diesem Fall können Sie eine der Buchungsarten `Ablehnen` oder `Akzeptieren` wählen.
   *Abb. D-109: Elektronische Rechnungskontrolle – Positionsübersicht*
   Sie können die Positionspreise und -mengen nicht direkt korrigieren.
5. Markieren Sie die Position, die Sie korrigieren möchten.
6. Wählen Sie im Menü `Funktionen > Bestellerfassung öffnen` und korrigieren Sie die Menge. Wenn Sie die Differenzen korrigiert und gespeichert haben und die Bestellerfassung wieder schließen, werden die neuen Werte in der elektronischen Rechnungskontrolle angezeigt. Preisdifferenzen brauchen Sie nicht manuell zu korrigieren. Es genügt, wenn Sie das Dokument trotz dieser Differenzen akzeptieren. Die Korrektur führt das Programm automatisch aus.
7. Wenn alle Fehler behoben sind, wählen Sie die Option `Akzeptieren`.
8. Wählen Sie im Menü `Start > Speichern`, um die Rechnungskontrolle abzuschließen. Die Daten werden gespeichert und der Status der Bestellung(en) wird umgesetzt. Die Rechnungskontrolle für diese Dokumente kann danach nicht nochmals durchgeführt werden.

### Teillieferung aus elektronischem Dokument erstellen
Wenn in dem eingelesenen Dokument nur ein Teil der Bestellpositionen oder bestellten Mengen aufgeführt ist, können Sie eine Teillieferung erstellen.

**So erstellen Sie eine Teillieferung zu einer importierten Lieferantenrechnung**
1. Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`. (⇨ Softwarereferenz, "Elektronische Rechnungskontrolle" auf Seite D-256)
2. Markieren Sie die Rechnung, zu der Sie eine Teillieferung erfassen möchten. Wenn der Dokumentenstatus außer Mengendifferenzen keine weiteren Fehler anzeigt, können Sie eine Teillieferung erzeugen. Nur dann ist die Option `Teillieferung erstellen` freigeschaltet. Wie Sie fehlende Referenzen herstellen, finden Sie unter: (⇨ "So ordnen Sie Positionen in einer importierten Rechnung zu" auf Seite D-173)
3. Wählen Sie die Option `Teillieferung erstellen`.
4. Wählen Sie im Menü `Start > Ausführen`, um die Teillieferung zu erzeugen. Damit wird eine Teillieferung mit der Rechnungsnummer, der gelieferten Menge und den Preisen aus dem importierten Dokument erzeugt. Der Status der Original-Bestellung wird entsprechend umgesetzt. Die Original-Bestellung kann so lange wieder zugeordnet werden, bis alle Positionen vollständig geliefert und referenziert sind.

### Positionen im elektronischen Dokument zuordnen
Wenn die Referenzen im elektronischen Dokument nicht eindeutig sind, kann die Position nicht zugeordnet werden. Diese Zuordnung können Sie bei der Prüfung des Dokuments nachholen.
Wenn eine Position in der Bestellung vollständig fehlt, z. B. ein Energiezuschlag, müssen Sie diese Position in der entsprechenden Bestellung zunächst erfassen. Sie können dazu die Bestellung aus der Preis-/Rechnungskontrolle heraus öffnen. Wenn Sie die Position erfasst und gespeichert haben, fahren Sie in der Rechnungskontrolle fort.

**So ordnen Sie Positionen in einer importierten Rechnung zu**
1. Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`. Der Dialog (elektronische) Rechnungskontrolle wird geöffnet und die importierten Rechnungen werden angezeigt. (⇨ Softwarereferenz, “Elektronische Rechnungskontrolle" auf Seite D-256)
2. Markieren Sie die Rechnung, deren Positionen Sie zuordnen möchten.
3. Wechseln Sie zum Register `Positionsübersicht`. Sie können eine Position in der Bestellung nachträglich erfassen, indem Sie über das `Menü Funktionen > Bestellerfassung öffnen` zum Dokument wechseln. Wenn Sie die Position erfasst und gespeichert haben, fahren Sie in der Rechnungskontrolle mit Schritt 4 fort.
   *Abb. D-110: Elektronische Rechnungskontrolle – Positionsübersicht*
4. Markieren Sie die Position, die nicht zugeordnet werden konnte, und wählen Sie im `Menü Funktionen > Positionen manuell zuordnen`.
   *Abb. D-111: Elektronische Rechnungskontrolle – Positionen zuordnen*
   - **A Position aus der Rechnung**
   - **B Zuordnung des Fußzuschlags für die aktuelle Sitzung beibehalten**
   - **C Zuordnung des Fußzuschlags für alle künftigen Importe speichern**
   - **D Position in der Bestellung**
   (⇨ Softwarereferenz, "Positionen manuell zuordnen" auf Seite D-221)
5. Markieren Sie in der linken und der rechten Übersicht jeweils die Positionen (A, D), die Sie einander zuordnen möchten.
6. Klicken Sie auf [OK], um die Zuordnung zu speichern.
7. Wiederholen Sie den Vorgang, bis alle Positionen zugeordnet sind. Wenn Sie Fußzuschläge/-rabatte zugeordnet haben, können Sie über die beiden Checkboxen (B, C) festlegen, ob die Zuordnung für diese Rechnung und/oder diesen Lieferanten beibehalten werden soll. Wie Sie einen Fußzuschlag/-rabatt auf mehrere Bestellungen verteilen, finden Sie unter: (⇨ "Zuschläge/Rabatte manuell zuordnen" auf Seite D-175)
8. Klicken Sie auf [Ende], wenn alle Zuordnungen korrekt sind. Im Dialog `Elektr. Rechnungskontrolle` sind alle Buchungsarten freigeschaltet.
9. Wählen Sie die gewünschte Buchungsart, z. B. `Akzeptieren`.
10. Wählen Sie im Menü `Start > Ausführen`, um die Aktion zu starten.
11. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert und der Status der Bestellung(en) wird umgesetzt.

### Zuschläge/Rabatte manuell zuordnen
Wenn in einer Rechnung zu mehreren Bestellungen nur ein Fußzuschlag/-rabatt aufgeführt ist, können Sie diesen manuell auf die einzelnen Bestellungen und/oder Bestellpositionen verteilen. Der Zuschlag/Rabatt wird dann anteilig berechnet und in die Bestellungen zurückgeschrieben.

**So verteilen Sie den Fußzuschlag/-rabatt auf Bestellungen**
1. Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`. Der Dialog `Elektr. Rechnungskontrolle` wird geöffnet und die importierten Rechnungen werden angezeigt.
2. Markieren Sie die Rechnung, aus der Sie den Fußzuschlag/-rabatt verteilen möchten. (⇨ Softwarereferenz, "Fußzuschläge/-rabatte verteilen" auf Seite D-222) In der Übersicht `Bestellungen/Teillieferungen` werden alle referenzierten Dokumente angezeigt.
3. Wählen Sie im Menü `Funktionen > Fußzuschläge/-rabatte auf Bestellungen verteilen`.
4. Halten Sie die Taste `<Strg>` gedrückt und markieren Sie alle Position, auf die der Zuschlag/Rabatt verteilt werden soll.
5. Klicken Sie auf [OK], um die Verteilung zu speichern. Die Daten werden in die betreffenden Bestellungen zurückgeschrieben. Die Einkaufspreise in den Bestellungen werden aktualisiert.
6. Schließen Sie den Dialog mit [Ende] und fahren Sie mit der Rechnungskontrolle fort. (⇨ "So prüfen und akzeptieren Sie eine importierte Lieferantenrechnung" auf Seite D-170)

### Ergänzende Informationen
- ⇨ Softwarereferenz, "Elektronische Preiskontrolle" auf Seite D-213
- ⇨ Softwarereferenz, "Elektronische Rechnungskontrolle" auf Seite D-256
- ⇨ Softwarereferenz, "Positionen manuell zuordnen" auf Seite D-221
- ⇨ Stammdaten, "Geschäftsabläufe abbilden" auf Seite B-420
- ⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-936

---

## Datenexport/-import (EDI)

### Lernziele
- Funktion der Fremdschnittstelle kennenlernen.
- Voreinstellungen für den Datenaustausch per EDI-Schnittstelle kennenlernen.

### Nutzen
- Durch den Datenaustausch über EDI-Schnittstellen müssen Dokumente nicht manuell erfasst werden.

### Merke

**EDI**
- EDI = Electronic Data Interchange, Elektronischer Datenaustausch per ASCII-Datei

**Schnittstellen**
- Die Schnittstellen müssen für Kunden und Lieferanten eingerichtet werden.

**Voreinstellungen**
- **Firmendaten:**
    - Register Lager/EK/EDI
- **B2B:**
    - Kunde, Lieferant

### Datenaustausch im ASC-Format
Über eine EDI-Schnittstelle können Angebote, Aufträge, Bestellungen und Gutschriften ausgetauscht werden. Dabei werden die Daten in eine ASC-Datei (ascii) geschrieben. Den Pfad für diese Datei legen Sie für jeden Kunden und jeden Lieferanten fest.
Standardmäßig werden die Daten der zu transferierenden Datei automatisch im ANSI-Format konvertiert, z. B. `ä` in `ae`.

#### Firmendaten prüfen
In den Firmendaten müssen Sie im Register `Lager/EK/EDI` die Voreinstellungen prüfen, die sich auf die Konvertierung beziehen.

*Abb. D-112: Firmendaten - Register Lager/EK/EDI*
> **EDI-Schnittstelle**
> - OEM/ANSI Konvertierung deaktivieren
> - Automatische Einlastung in Kapazitätsplanung deaktivieren
> - Architekt aus Kopfsatz für Artikelreferenzen verwenden

In der Regel sollte die OEM/ANSI-Konvertierung nur deaktiviert werden, wenn die verwendete Schnittstelle dies explizit fordert.

### Einstellungen prüfen
Wenn Sie mit Ihren Lieferanten/Kunden Aufträge und Bestellungen im ASC-Format austauschen, müssen Sie die Parameter für jeden einzelnen Lieferanten/Kunden einstellen.

**So prüfen Sie die Einstellungen für den Datenexport per EDI**
1. Wählen Sie `Stammdaten > B2B > Lieferant > Lieferant`. Für den Datenimport per EDI wählen Sie `Stammdaten > B2B > Kunde > Kunde`. Die nachfolgenden Handlungsschritte gelten analog.
2. Wählen Sie im Menü `Start > Suchen`, um in die Suche zu starten. Die Trefferliste wird im Register `Tabelle` angezeigt.
3. Markieren Sie den Lieferanten, an den Bestellungen über die EDI-Schnittstelle gesendet werden sollen.
4. Wechseln Sie zum Register `Auswahl`.
   *Abb. D-113: Schnittstellenverwaltung*
   - **A Typ der Schnittstelle**
   - **B Angaben für die Zieldatei**
   - **C Angaben für die Protokolldatei**
   - **D Pfad für die Sicherungsdatei**
5. Geben Sie die Verzeichnisse und Dateinamen (B) für die Export- und die Sicherungsdatei an (D).
6. Wählen Sie die Schnittstellenversion (A) aus, mit der Ihr System arbeitet. Wenn Sie Auftragsbestätigungen und Rechnungen ebenfalls elektronisch austauschen (openTRANS-Format), müssen Sie die Version wählen, mit der Sie die Daten bisher übertragen haben. Die Version wird bei der Installation von A+W Business festgelegt.
   *Abb. D-114: Einstellungen für EDI-Dokumentenexport*
7. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.
8. Wechseln Sie zum Register `Parameter`.
   *Abb. D-115: Parameter für den EDI-Austausch*
9. Markieren Sie die Checkboxen für Export:
   - **Zwangsreferenzierung (A):** Wenn eine Position ohne Referenz auf ein (externes) Produkt gesendet wird, kann diese Position ignoriert werden. In diesem Fall wird eine Fehlermeldung im Logbuch eingetragen. Wenn die Checkbox nicht markiert ist, wird die Produktnummer aus den Stammdaten in die Schnittstellendatei geschrieben. Das ist z. B. dann sinnvoll, wenn das sendende und das empfangende System die gleichen Produktstammdaten benutzen. In dem Fall ist es nicht nötig, Daten in die Referenztabellen einzutragen.
   - **Locking aktiv und Maximale Lock-Zeit (B):** Mit dieser Einstellung verhindern Sie, dass für den eingegebenen Zeitraum nur ein Programm auf dieselbe Schnittstellendatei zugreifen kann.
   - **Import von Kundenaufträgen (C):** Wenn Sie die Daten für Kunden einrichten, können Sie zusätzlich Einstellungen für den Import festlegen.
10. Wiederholen Sie die Schritte für alle Lieferanten, mit denen Sie Daten per EDI austauschen.
11. Wechseln Sie zu `Stammdaten > B2B > Kunde > Kunde` und wiederholen Sie die Schritte für alle Kunden, mit denen Sie Daten per EDI austauschen.

### Bestellung exportieren
Wenn Sie Bestellungen exportieren, werden die Daten in eine ASC-Datei geschrieben. Diese wird im festgelegten Verzeichnis abgelegt. Die Datei wird danach über die EDI-Schnittstelle zum Lieferanten übertragen.

**So exportieren Sie eine Bestellung**
1. Wählen Sie `Dokumente > Bestellungen > Export`. Der Dialog `Export` wird geöffnet und die Bestellungen im aktuellen Nummernverwalter werden angezeigt.
   *Abb. D-116: Export von Bestellungen*
2. Wählen Sie im Menü `Start > Ausführen`, um den Export zu starten. Der Export wird gestartet. Eine Verlaufsmeldung zeigt an, welche Bestellung aktuell übertragen wird.
3. Wechseln Sie zum Register `Pool`, um den Status des Exports zu prüfen. Sie können die Anzeige mit [Abfragen] aktualisieren.

#### Ergänzende Informationen
- ⇨ Verkauf, "Import von Dokumenten" auf Seite C-377
- ⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1032

---

# Softwarereferenz

## A+W Business

### Übersicht
In der Dokumentenverwaltung können Sie alle Dokumente erfassen und bearbeiten, die im Rahmen des Einkaufs benötigt werden, z. B. Anfragen zu Lieferungen und Bestellungen. Außerdem können Sie Wareneingänge erfassen, Liefertermine prüfen und korrigieren und die Lieferanten-Rechnungen kontrollieren.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
- Anfrage (Menü)
- Bestellung (Menü)
- Auftragsbestätigung
- Wareneingang
- Rechnung
- Basisglasverrechnung

Folgende Dialoge sind für alle Dokumentenarten gleich und sind daher nur einmal im Part Verkauf erklärt:
- FiBu-Übergabe
- Übergabe Archiv
- Suche

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass viele Übersichten und Funktionen zum Thema Einkauf in A+W Business aus unterschiedlichen Dialogen heraus gestartet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.
> Dialoge, die auch für den Verkauf benötigt werden, sind ausführlich im Part Verkauf beschrieben.

**Dialogbeschreibungen im Part Verkauf**
- ⇨ Softwarereferenz, “Dokumentenverwaltung" auf Seite C-409
- ⇨ Softwarereferenz, “Übersichten und Referenzen zu Kopfdaten" auf Seite C-522
- ⇨ Softwarereferenz, "Positionsdaten" auf Seite C-440
- ⇨ Softwarereferenz, "Übersichten und Referenzen zu Positionen" auf Seite C-582
- ⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-629
- ⇨ Softwarereferenz, "Druck" auf Seite C-637
- ⇨ Softwarereferenz, "Übergabe Archiv" auf Seite C-686

### Anfrage (Menü)
`Dokumente > Anfrage`

Über das Menü `Anfrage` erreichen Sie folgende Programmpunkte:
- **NV Anfrage:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Nummernverwalter" auf Seite C-629)
- **Anfrage:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Dokumentenverwaltung" auf Seite C-409; Verkauf, "Positionsdaten" auf Seite C-440)
- **Druck Anfrage:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Druck" auf Seite C-637)
- **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Journal" auf Seite C-725)
- **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Übergabe Archiv" auf Seite C-686)
- **Suche:** Die Suche ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Dokument suchen" auf Seite C-523)

### Anfrage (Dokumentenverwaltung)
`Dokumente > Anfrage > Anfrage`

*Abb. D-117: Dokumentenverwaltung – Anfrage*

In diesem Dialog erfassen und bearbeiten Sie Anfragen an Ihren Lieferanten. Anfragen können entweder manuell erfasst werden oder sie werden bei der Bestellübergabe erzeugt, wenn im Bestellpool die Option `Sofort anfragen` gewählt ist.
- ⇨ Tutorial, "Anfrage" auf Seite D-110
- ⇨ Verkauf, "Bestellübergabe - Bestellnummern" auf Seite C-657

Die Felder im Dialog `Dokumentenverwaltung` und in der `Positionserfassung` sind für alle Dokumententypen gleich. Sie sind ausführlich zu den Aufträgen erklärt:
- ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-417
- ⇨ Verkauf, "Dokument - Positionen" auf Seite C-451

### Bestellung (Menü)
`Dokumente > Bestellung`

Über das Menü `Bestellung` erreichen Sie folgende Programmpunkte:
- **NV Bestellung:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. (⇨ Verkauf, "Nummernverwalter" auf Seite C-629)
- **Bestellung:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. (⇨ Verkauf, "Dokumentenverwaltung" auf Seite C-409; Verkauf, "Positionsdaten" auf Seite C-440)
- **Teillieferung:** Die Erstellung von Teillieferungen ist für alle Dokumentenarten gleich. (⇨ Verkauf, "Teillieferungen" auf Seite C-616)
- **Nachbestellung:** In diesem Dialog können Sie Bestellteile, die als Bruch gemeldet sind, nachbestellen, reklamieren, verrechnen oder die Auftragsmenge reduzieren. (⇨ "Nachbestellung" auf Seite D-191)
- **Druck Bestellung:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. (⇨ Verkauf, "Druck" auf Seite C-637)
- **Export (EDI):** In diesem Dialog exportieren Sie Bestellungen über die EDI-Schnittstelle. (⇨ "Export (EDI)" auf Seite D-193)
- **Journal:** Der Journaldruck ist für alle Dokumente gleich. (⇨ Verkauf, "Journal" auf Seite C-725)
- **AB Lieferant:** In diesem Dialog erfassen und prüfen Sie die Auftragsbestätigungen (AB) Ihrer Lieferanten. (⇨ "AB-Lieferant" auf Seite D-197)
- **Auftragsbestätigung:**
    - **Preiskontrolle:** Prüfen und korrigieren Sie Preise in Auftragsbestätigungen. (⇨ "Auftragsbestätigung" auf Seite D-204)
    - **Elektr. Preiskontrolle:** Prüfen Sie Preise und Referenzen in elektronisch übermittelten ABs. (⇨ "Auftragsbestätigung" auf Seite D-204)
- **Mahnung:** Erfassen Sie Mahnungen für ausstehende Lieferungen. (⇨ "Mahnung" auf Seite D-225)
- **Wareneingang:**
    - **Wareneingang:** Erfassen Sie Wareneingänge zu Bestellungen. (⇨ "Wareneingang" auf Seite D-227)
    - **Eingangskontrolle:** Prüfen Sie die Vollständigkeit der Wareneingänge. (⇨ "Eingangskontrolle" auf Seite D-241)
- **Rechnung:**
    - **Rechnungskontrolle:** Prüfen und korrigieren Sie Lieferantenrechnungen. (⇨ "Rechnungskontrolle - Bestellungen" auf Seite D-248)
    - **Elektr. Rechnungskontrolle:** Prüfen Sie Preise und Referenzen in elektronischen Rechnungen. (⇨ "Elektronische Rechnungskontrolle" auf Seite D-256)
- **FiBu-Übergabe:** Die FiBu-Übergabe wird am Beispiel Auftrag erklärt. (⇨ Verkauf, "FiBu-Übergabe" auf Seite C-679)
- **Übergabe Archiv:** Die Archivübergabe wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Übergabe Archiv" auf Seite C-686)
- **Suche:** Die Suche wird ausführlich zu den Aufträgen erklärt. (⇨ Verkauf, "Dokument suchen" auf Seite C-523)
- **Basisglasverrechnung:** Hier werden interne Verrechnungen von Profit Centern verwaltet (kundenspezifisch freigeschaltet).

### Bestellung (Dokumentenverwaltung)
`Dokumente > Bestellung > Bestellung`

*Abb. D-118: Dokumentenverwaltung - Bestellung*

In diesem Dialog erfassen und bearbeiten Sie Bestellungen. (⇨ Tutorial, "Manuelle Bestellung" auf Seite D-79)
Der Dialog `Dokumentenverwaltung` und die zugehörigen Menüs sind für alle Dokumentenarten gleich. Er wird am Beispiel Auftrag beschrieben.
- ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-417
- ⇨ Verkauf, "Dokument - Positionen" auf Seite C-451

> **Bestellung erfassen**
> Die Bestellungen erfassen Sie auf die gleiche Weise wie einen Auftrag. Achten Sie dabei darauf, dass Sie den richtigen Dokumententyp auswählen:
> - **Lagerbestellung:** Mit dieser Einstellung bestellen Sie Lagerprodukte. Mit dem Wareneingang werden die gelieferten Positionen automatisch auf Lager verbucht. In dieser Bestellung müssen Sie den Lagerartikel über die Lagersuche `<F3>` auswählen. Der Typ `Lagerbestellung` wird im Feld `Typ` angezeigt.
> - **<k.A>:** Mit dieser Einstellung bestellen Sie alle Produkte, die nicht über das Lager verbucht werden. (⇨ Verkauf, "Typ" auf Seite C-422; Tutorial, "Unabhängige Bestellung erfassen" auf Seite D-81)

Wenn Sie eine Lagerbestellung mit Produkten erfassen, die nicht als Lagerartikel geführt werden, kann der Wareneingang für diese Produkte nicht automatisch ins Lager verbucht werden. Eine entsprechende Meldung weist Sie beim Erfassen der Bestellung darauf hin.

> **Positionen ohne Lagerkennzeichen**
> Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Firmendaten die entsprechende Option aktivieren. (⇨ Stammdaten, "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." auf Seite B-959)

### Nachbestellung
`Dokumente > Bestellung > Nachbestellung`

*Abb. D-119: Nachbestellung*

In diesem Dialog verwalten Sie Aufträge mit Bestellteilen, die aus der Produktion als Bruch gemeldet sind. Sie können die Bestellteile nachbestellen, reklamieren, verrechnen oder die Auftragsmenge reduzieren.

#### Selektion
- **Auftrag von, bis:** Einschränkung der Suche auf einen Auftrag oder eine Folge von Aufträgen.
- **Liefertermin von, bis:** Einschränkung der Suche auf einen bestimmten Liefertermin oder eine Reihe von Lieferterminen.

#### Dokumente
In der Übersicht werden alle Aufträge mit Bruchscheiben angezeigt, die den Suchkriterien entsprechen.
- **Auftrag:** Auftragsnummer.
- **Auftragsposition:** Positionsnummer aus dem Auftrag.
- **Lieferdatum:** Lieferdatum aus dem Auftragskopf.
- **Bestellung:** Bestellnummer.
- **Bestellposition:** Positionsnummer aus der Bestellung.
- **Lieferant:** Name des Lieferanten aus der Bestellung.
- **Produkt:** Nummer und Bezeichnung des Produkts.
- **Auftragsmenge:** Menge aus dem Auftrag.
- **Bestellmenge:** Menge, die bestellt ist.
- **Bruchmenge:** Menge, die als Bruch gemeldet ist.
- **Rückmeldedatum:** Datum der Bruchmeldung.
- **Aktion:** Auswahl der Aktion:
    - **Nachbestellung:** Die Bestellung wird erstellt und in den ausgewählten Nummernverwalter gestellt.
    - **Reklamation:** Für die Bestellteile wird eine Reklamation erstellt. Wenn diese Option gewählt wird, können Reklamationsgrund und -verursacher angegeben werden.
    - **wertmäßige Buchung:** Die Bestellung wird mit einer negativen Positionsmenge erstellt. Damit wird die Bruchmenge ausgebucht und der Wert der Bruchmenge mit dem Wert des Auftrags verrechnet.
    - **Auftragsmenge reduzieren:** Der Ursprungsauftrag wird um die Bruchmenge reduziert. Damit wird eine Nachbestellung ausgeschlossen.
- **Reklamationsgrund:** Wird nur angegeben, wenn als Aktion `Reklamation` gewählt ist.
- **Reklamationsverursacher:** Wird nur angegeben, wenn als Aktion `Reklamation` gewählt ist.
- **Bemerkung:** Sie können eine Bemerkung eintragen, z. B. Absprachen.
- **Etikett:** Nummer des Etiketts aus der Produktion. Die Nummer kann nicht geändert werden.

#### Ziel
- **Nummernverwalter:** Nummernverwalter, in den die Nachbestellungen gestellt werden sollen.

### Export (EDI)
`Dokumente > Bestellung > Export`

In diesem Dialog können Sie Bestellungen exportieren, um Sie über die EDI-Schnittstelle an den betreffenden Lieferanten zu übertragen.
- ⇨ Tutorial, "Datenexport/-import (EDI)" auf Seite D-177

> **Voraussetzung**
> Die Parameter für die Schnittstelle müssen für jeden einzelnen Lieferanten/Kunden festgelegt werden, mit dem Dokumente über die Fremdschnittstelle ausgetauscht werden sollen. Diese Parameter werden im Menü `Stammdaten > B2B` eingestellt.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite D-194
- "Export - Export" auf Seite D-195
- "Export - Pool" auf Seite D-196

#### Menü Funktionen
`Dokumente > Bestellung > Export > Menü Funktionen`
Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog `Export` zu schließen.

**Gruppe Bearbeiten**
- **Kopieren:** Öffnet den Dialog `Nummernverwalter kopieren`. (⇨ Verkauf, "Nummernverwalter kopieren" auf Seite C-634)
- **Statusänderung:** Öffnet den Dialog `Statusänderung`. (⇨ Verkauf, "Statusänderung" auf Seite C-554)

**Gruppe Dokument**
- **Dokument anzeigen:** Öffnet den Dialog `Dokumentenansicht`. (⇨ Verkauf, "Reklamationen" auf Seite C-591)
- **Historie:** Öffnet eine Übersicht über Statusänderungen. (⇨ Verkauf, "Historie" auf Seite C-552)
- **Dokumentendaten:** Öffnet den Dialog `Dokumentendaten`. (⇨ Verkauf, "Dokumentendaten" auf Seite C-738)
- **Dokumentenerfassung:** Öffnet den Dialog `Dokumentenverwaltung`. (⇨ Verkauf, "Dokumentenverwaltung" auf Seite C-409)

**Gruppe Dokumentenkopie**
- **Dokumente kopieren:** Öffnet den Dialog `Dokumente kopieren`. (⇨ Verkauf, "Dokumente kopieren" auf Seite C-532)
- **Teillieferung:** Öffnet den Dialog `Dokumente kopieren` für eine Teillieferung. (⇨ Verkauf, "Dokumente kopieren" auf Seite C-532)

#### Export - Export
`Dokumente > Bestellung > Export > Register Export`

*Abb. D-120: Export - Export*

In diesem Register exportieren Sie die Bestellungen. Die Daten werden in eine ASC-Datei geschrieben und im festgelegten Verzeichnis abgelegt. Die Datei wird danach über die EDI-Schnittstelle zum Lieferanten übertragen. Die Einstellungen für den Export werden pro Lieferant im Modul `Stammdaten > B2B` festgelegt. (⇨ Tutorial, "Datenexport/-import (EDI)" auf Seite D-177)

**Selektion nach**
- **Mitarbeiter:** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter:** Auswahl des Nummernverwalters, auf den der Dialog `Export` zugreifen soll.
- **[Logbuch]:** Schaltfläche zum Öffnen des Systemlogbuchs.

**Dokumente**
Liste aller Dokumente, die im gewählten Nummernverwalter stehen und an den Lieferanten gesendet werden sollen.
- **Nummer:** Nummer des Dokuments.
- **Nummer Kunde/Lief.:** Nummer des Kunden oder Lieferanten.
- **Kunde/Lieferant:** Name des Kunden oder Lieferanten.
- **Status:** Status des Dokuments.
- **Datum Erfassung:** Datum, an dem das Dokument erfasst wurde.
- **Datum Lieferung:** Lieferdatum.
- **Datum AB:** Datum der Auftragsbestätigung.
- **Sperr-KZ:** Kennzeichen, ob das Dokument gesperrt ist. Wird bei Bestellungen selten gesetzt.

#### Export – Pool
`Dokumente > Bestellung > Export > Register Pool`

*Abb. D-121: Export – Pool*

In diesem Register können Sie die aufgelisteten Bestellungen elektronisch über die EDI-Schnittstelle übergeben.

**Übertragungs-Pool**
In der Übersicht werden alle Bestellungen aufgelistet, die elektronisch übergeben werden sollen.
- **[Löschen]:** Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Sie können dann einen Eintrag aus dem Übertragungspool löschen.
- **[Aktivieren]:** Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Wenn ein Fehler festgestellt wurde, können Sie die Daten korrigieren und erneut zur Übertragung übergeben.
- **[Abfragen]:** Mit dieser Schaltfläche aktualisieren Sie die Anzeige, um den Übertragungsstatus zu prüfen.

### AB-Lieferant
`Dokumente > Bestellung > AB Lieferant`

In diesem Dialog können Sie die Auftragsbestätigung erfassen, die Ihr Lieferant zu einer Bestellung gesendet hat. Außerdem können Sie den zugehörigen Wareneingang erfassen und/oder die Termine für Bestellungen und Lieferungen prüfen und ggf. korrigieren.

#### Menü Optionen
`Dokumente > Bestellung > AB Lieferant > Menü Optionen`
Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen.
- **Lagerbuchungsdatum = Lieferdatum:** Als Buchungsdatum wird automatisch das Lieferdatum aus der Bestellung übernommen.
- **AB-Nummer prüfen:** Eine Meldung wird angezeigt, wenn die Nummer der Auftragsbestätigung nicht eingegeben ist.
- **Identnummernvergabe:** Diese Einstellung wird für den Wareneingang von Kisten und Lagerplatten benötigt.
    - **Manuell:** Sie müssen die ID manuell vergeben. Die Checkbox `Identnummer(n) vergeben` im Bereich `Optionen` wird freigeschaltet. (⇨ "Optionen" auf Seite D-199)
    - **Automatisch:** Die ID wird automatisch vergeben. Dazu kann eine Vorgabe festgelegt werden.
    - **Einstellungen:** Öffnet den Dialog `Einstellungen`, in dem Sie die Vorgabe für die automatische Vergabe von IDs festlegen. (⇨ "Einstellungen (ID)" auf Seite D-240)

#### AB-Lieferant – Dokumente
`Dokumente > Bestellung > AB Lieferant > Register Dokumente`

*Abb. D-122: AB-Lieferant – Dokumente*

In diesem Register können Sie eine Auftragsbestätigung des Lieferanten und/oder den zugehörigen Wareneingang erfassen. Außerdem können Sie die Termine für Bestellungen und Lieferungen prüfen und ggf. korrigieren. Alle Daten gelten für alle Positionen in der Bestellübersicht. Für einzelne Positionen wechseln Sie zum Register `Positionen`.
- ⇨ Tutorial, "Lieferanten-AB" auf Seite D-87

**Dokumente**
- **Bestellnummer:** Auswahl einer Bestellung.
- **Auftragsnummer:** Auswahl eines Kundenauftrags, aus dem eine Bestellung erzeugt wurde.

**Optionen**
- **Auftrags-NV füllen:** Der zugehörige (Kunden-) Auftrag kann automatisch in einen anderen Nummernverwalter gestellt werden.
- **Bestell-NV füllen:** Die zugehörige Bestellung kann automatisch in einen anderen Nummernverwalter gestellt werden.
- **Wareneingang buchen:** Erfassen Sie den kompletten Wareneingang, wenn die Ware zusammen mit der AB geliefert wurde.
    > **Wareneingang teilweise erfassen:** Den vollständigen Wareneingang für einzelne Positionen können Sie im Register `Positionen` erfassen. Für den teilweisen Wareneingang einer Position müssen Sie zum Dialog `Wareneingang` wechseln. (⇨ "Wareneingang (Dialog)" auf Seite D-227)
- **Identnummer(n) vergeben:** Die Checkbox wird über die Einstellung zur Identnummernvergabe aktiviert. IDs werden in der Regel für Kisten vergeben.

**Bestelldaten**
- **Lieferant:** Name des Lieferanten aus der Bestellung oder dem Kundenauftrag.
- **Status:** Status des ausgewählten Dokuments.
- **Gesamtstückzahl:** Stückzahl aller Positionen insgesamt im ausgewählten Dokument.
- **Bestätigter Anliefertermin:** Termin der Lieferung durch den Lieferanten. Das Datum ist aus der Bestellung übernommen und kann geändert werden. Ein geänderter Termin wird zurückgeschrieben. (⇨ "AB-Lieferant - Liefertermine ändern" auf Seite D-203)
- **Teilliefertermin:** Liefertermin, der in der Auftragsbestätigung gemeldet wird.
- **AB-Nummer:** Nummer der Auftragsbestätigung des Lieferanten. Diese Nummer wird in alle angezeigten Positionen eingetragen.

**Auftragsdaten**
Dieser Bereich wird nur angezeigt, wenn ein Auftrag oder eine Bestellung zu einem Auftrag ausgewählt ist.
- **Kunde:** Name des Kunden, für den die Bestellung erzeugt wurde.
- **Status:** Status des Kundenauftrags.
- **Gesamtstückzahl:** Stückzahl aller Positionen im Kundenauftrag.
- **Anliefertermin bei Kunden:** Termin der Anlieferung beim Kunden. Kann geändert und zurückgeschrieben werden. (⇨ Verkauf, "Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-565; Tutorial, "Liefertermine ändern und Kunden benachrichtigen" auf Seite D-102)
- **Geplant:** Ursprünglich geplanter Anliefertermin beim Kunden.
- **Versandtag:** Termin, an dem die Lieferung an den Kunden gesendet wird.
- **Tour:** Auswahl der Tour, mit der die Lieferung an den Kunden geht.
