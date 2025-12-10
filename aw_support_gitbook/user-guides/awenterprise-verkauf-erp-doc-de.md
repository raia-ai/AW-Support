---
description: "DE_AWEnterprise_Verkauf_4_1"
---


# A+W Enterprise
**A+W - Software for Glass, Windows and Doors**

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 4.00 / 02-2020 | Vollständige Überarbeitung |
| 3.01 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 3.00 / 07-2013 | Vollständige Überarbeitung und Anpassung an neues CI |
| 2.30 / 01-2010 | Kleinere Korrekturen/Identifier |
| 2.20 / 01-2008 | Preisberechnung |
| 2.10 / 02-2007 | Zusammenführung Verkauf/Einkauf |
| 2.00 / 12-2006 | Änderung Register Verkauf |
| 1.00 / 02-2006 | Ersterstellung |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Enterprise gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.
Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

### Urheberrechte
© 2020, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
A+W Software GmbH
Am Pfahlgraben 4-10
35415 Pohlheim
📞 +49 6404 2051-0
📠 +49 6404 2051 877
📧 Zentrale@a-w.com
🌐 http://www.a-w.com

## Inhalt

- **Revisionsübersicht** (D-3)
- **Editorial** (D-3)
- **Softwarereferenz** (D-11)
  - **Übersicht** (D-13)
  - **Menü Verkauf** (D-14)
    - Untermenü Rechnungen (D-15)
    - Untermenü Übersicht (D-16)
  - **Zusatzmenü** (D-16)
    - Untermenü Adressen (D-18)
    - Untermenü Texte (D-18)
    - Untermenü Spezielle Texte (D-19)
    - Untermenü Preisangaben (D-19)
    - Untermenü Auftragspreise (D-20)
    - Untermenü Produktangaben (D-20)
    - Untermenü Technische Werte (D-21)
  - **Infomenü** (D-22)
    - Untermenü Anmerkungen (D-23)
  - **Suchfunktionen** (D-24)
    - **Suche Aufträge** (D-25)
      - Suche Aufträge - Vorgangs-Schlüssel (D-25)
      - Suche Aufträge - Positions-Schlüssel (D-28)
      - Suche Aufträge - Direkte Suche (D-29)
      - Suche Aufträge - Trefferliste (D-30)
      - Suche Aufträge - Lieferinfos (D-31)
      - Suche Aufträge - Verschiedenes (D-33)
      - Suche Aufträge - Mengen (D-34)
      - Suche Aufträge - Eigenschaften (D-36)
      - Suche Aufträge - Kommission (D-37)
    - **Marktpartnersuche** (D-39)
    - **Mitarbeiter/Berechtigungsgruppen** (D-43)
    - **Suche Bezugsvorgang** (D-45)
    - **Adressen Suche** (D-47)
    - **Artikel-Suche** (D-49)
      - Artikel-Suche - Kopf-, Fußbereich (D-50)
      - Artikel-Suche - Bezeichnungen (D-53)
      - Artikel-Suche - Artikelcodes (D-55)
      - Artikel-Suche - Details (D-56)
    - **Artikel-Suche nach Typen** (D-58)
    - **Produktsuche nach Elementen** (D-59)
      - Produktsuche nach Elementen - Kopf-, Fußbereich (D-60)
      - Produktsuche nach Elementen - Kundenartikel (D-62)
      - Produktsuche nach Elementen - Bezeichnungen (D-64)
      - Produktsuche nach Elementen - Techn. Werte (D-65)
    - **Objekt-Suche** (D-66)
      - Objekt-Suche - Kopf-, Fußbereich (D-67)
      - Objekt-Suche - Adresse (D-69)
      - Objekt-Suche - Identifikation (D-70)
    - **Werteingabe - Erweiterte Suche** (D-71)
    - **Werteingabe - Suche nach Kommission** (D-72)
    - **Werteingabe - Suche nach Originalnummer** (D-73)
  - **Vorgangsverwaltung** (D-75)
    - Symbolerklärung (D-76)
    - Schnellerfassung (D-79)
    - Angebotserfassung (D-80)
    - Preislose Erfassung (D-81)
    - Auftragserfassung (D-82)
      - Auftragserfassung – Kopf-, Fußbereich (D-83)
      - Auftragserfassung - Anschriften (D-90)
      - Auftragserfassung - Eigenschaften (D-93)
      - Auftragserfassung - Verschiedenes (D-99)
      - Auftragserfassung - Summen (D-104)
      - Auftragserfassung - Detailansicht Rabatte (D-108)
    - Auftragspositionen (D-113)
      - Auftragspositionen - Allgemein (D-113)
      - Auftragspositionen - Eigensch. (D-126)
      - Auftragspositionen – Preise (D-131)
      - Auftragspositionen – Status (D-134)
      - Auftragspositionen – Kosten (D-136)
    - Hauswechsel (D-137)
    - Neue Lieferadresse (D-138)
    - Endkundenanschrift (D-140)
    - Marktpartner-Info (D-142)
    - Ansprechpartner (D-144)
    - Storno (D-145)
    - Mitarbeiterzuordnung - Spezial (D-146)
    - Konfigurierbare Felder (D-146)
    - Übersicht (D-147)
    - Produktsets (Sash Master) (D-148)
    - Artikel-Maßangaben (D-150)
    - Bestandsprognose (D-151)
    - Produktaustausch (D-154)
      - Produktaustausch (D-155)
      - Produktaustausch für Positionen (D-157)
    - Reklamation (D-158)
    - Auftragsarten (D-159)
    - Artikelangaben für bemaßte Varianten (D-161)
    - Varianten- und Farben-/Dickenauswahl (D-164)
    - Private Felder (D-165)
    - Fremddaten-Import (D-166)
    - Dokumentenarten (D-168)
    - Dokumentenartenzuordnung (D-169)
    - Dateizuordnung (D-171)
    - DXF Import (D-172)
    - Änderungs-Protokoll (D-173)
    - Lieferterminänderungs-Protokoll (D-175)
    - Modellkatalog (D-176)
    - Modell-Maßangaben (D-177)
    - Zahlungsverwaltung (D-179)
    - Zahlungsplan (D-181)
    - Fehlerinformationssystem (D-183)
    - Produktionsmonitor (D-185)
  - **Technische Werte** (D-186)
    - Leistungserklärung (D-186)
    - Auftragserfassung - Technische Werte (D-187)
    - Auftragserfassung - Berechnete technische Werte (D-187)
    - Auftragserfassung - Deklarierte Leistungen (D-190)
  - **Stückliste** (D-195)
    - Stücklistendarstellung (D-195)
      - Stücklistendarstellung - Stücklistenaufbau (D-196)
      - Stücklistendarstellung – Produktaufbau (D-199)
      - Stücklistendarstellung - Produktionsskizze (D-200)
      - Stücklistendarstellung - Akt. Stücklistenebene (D-202)
      - Stücklistendarstellung - Bearbeitungsparameter (kurz) (D-207)
      - Stücklistendarstellung - Adressen (D-208)
      - Stücklistendarstellung - Alle Parameter/Skizze (D-209)
    - Kantenzuordnung (D-217)
    - Bearbeitungen zu Position (D-218)
    - Maße der einzelnen Stücklistenteile (D-219)
    - Einstand (D-221)
    - Versiegelungstiefen (D-222)
    - Stufenerfassung (relevante Teile) (D-223)
    - Stufen Abzugsmaße (D-225)
    - Sprossenerfassung (D-226)
      - Sprossenerfassung – Sprossen (D-226)
      - Sprossenerfassung - Zusatzinfo (D-229)
    - Sprossenstückliste – Sprossenartikel (D-230)
    - Sprosseneditor (D-231)
    - Bohrpunkt (D-232)
    - Lichtes Feld (D-233)
    - Sprossenabschnitte (D-233)
    - Sprossenaufteilung (D-234)
    - Packmittelplanung (D-236)
      - Vorgaben Packmittelplanung (D-236)
      - Packmittelplanung (D-242)
  - **Anmerkungen** (D-245)
    - Vorgangs-Anmerkungen (D-247)
    - Marktpartner-, Objekt-, Artikel-Anmerkungen (D-248)
    - Kunden-Artikel-, Lieferanten-Artikel-, Objekt-Artikel-Anmerkungen (D-251)
  - **Texte** (D-253)
    - Kopf- und Fußtexte (D-254)
    - Artikel- und Positionstexte (D-256)
  - **Spezielle Texte** (D-257)
    - Floskeln (D-258)
    - Fremdinformationen (D-260)
    - Kistensignatur (D-261)
  - **Preise und Konditionen** (D-263)
    - Auftragskonditionen (D-264)
    - Auftragspreise (D-269)
    - Auftragssprossenpreise (D-271)
    - Auftragsaustauschpreise (D-274)
    - Auftragsunterteilpreise (D-276)
    - Nachkalkulation (D-277)
    - Stufenpreise (D-280)
    - Positionskonditionen (D-281)
      - Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG (D-282)
      - Konditionen für PKZ-VSG, PKZ-ESG (D-286)
      - Konditionen ISO (D-288)
      - Konditionen für ISO (SCHWEIZ) (D-293)
      - Konditionen für PKZ-FARBARTIKEL (D-297)
      - Konditionen für PKZ-PREISE-ALLGEMEIN (D-298)
      - Konditionen für PKZ-GLASTÜREN (D-300)
      - Konditionen für Manuelle Preise (D-303)
      - VSG-Austausch-/Zusatzpreise (D-304)
    - Positionskonditionen - Bearbeitungspreise (VK), (EK), Detailansicht (D-307)
    - Positionskonditionen - Sprossenpreise (D-310)
    - Produktionskostenkalkulation (D-313)
      - Produktionskostenkalkulation - Übersicht (D-314)
      - Produktionskostenkalkulation - Details (D-316)
    - Preiskalkulation (D-320)
  - **Freischaltung** (D-321)
    - Auftragsfreischaltung (D-321)
    - Autorisierung (D-324)
  - **Lieferung** (D-326)
    - Lieferplan (D-327)
    - Lieferinformation - Details der Auslieferung (D-329)
    - Lieferscheine (automatisch) (D-333)
    - Lieferscheine (manuell) (D-335)
    - Lieferscheinprotokoll (D-337)
  - **Rechnungen** (D-338)
    - Rechnungen (automatisch) (D-339)
    - Positionsinfo (D-342)
    - Rechnungen (manuell) (D-344)
    - Thekenrechnung (D-345)
    - Rechnungen buchen (D-346)
    - Abschlagsrechnung (automatisch) (D-348)
    - Abschlagsrechnung (manuell) (D-350)
    - Schlussrechnung (automatisch) (D-351)
    - Schlussrechnung (manuell) (D-352)
    - Rechnungsprotokoll (D-353)
  - **Gutschriften** (D-354)
    - Gutschriften (D-354)
    - Gutschriften buchen (D-356)
  - **Formulare** (D-358)
    - Direktdruck (D-358)
    - Formulardruck (D-359)
    - E-Mail (D-363)
    - Drucken auf (D-365)
    - Listendruck (D-366)
  - **Auftragsstatus** (D-367)
    - Auftragsinformation (D-367)
      - Vorgangsinformationen – Vorgang (D-368)
      - Vorgangsinformationen - Positionen (D-369)
      - Vorgangsinformationen - Einkauf (D-370)
      - Vorgangsinformationen - Wareneingang (D-372)
      - Vorgangsinformationen – Produktion (D-373)
      - Vorgangsinformationen - Versand (D-375)
      - Vorgangsinformationen – BDE (D-376)
      - Vorgangsinformationen - Gestelle (D-378)
      - Vorgangsinformationen - Lager (D-379)
      - Vorgangsinformationen - Verbundene Produktion (D-380)
      - Vorgangsinformationen - Zwischenversand (D-381)
  - **Recherche zu Vorgängen** (D-382)
    - Vorgangs-Recherche (D-382)
      - Vorgangs-Recherche - Suchmodus (D-382)
      - Vorgangs-Recherche – Übersicht (D-386)
      - Vorgangs-Recherche - Mitarbeiter (D-388)
      - Vorgangs-Recherche – Details (D-389)
      - Vorgangs-Recherche - Vorgangsänderungs-Protokoll (D-392)
    - Positionen (D-394)
      - Positionen - Übersicht (D-394)
      - Positionen – Details (D-396)
  - **Übersichten zu Vorgängen** (D-398)
    - Auftragsanzeige (D-398)
    - Angebotsanzeige (D-399)
    - Wiedervorlage (D-400)
    - Fertigmeldung (D-401)
    - Vorgangsänderung (D-403)
    - Übersicht zu Vorgängen (D-406)
  - **Vertrieb** (D-408)
- **Partindex** (D-409)
- **Index** (D-411)

# Softwarereferenz

## Übersicht
Im Modul **Verkauf** verwalten Sie die Vorgänge, die zur erfolgreichen Abwicklung des Verkaufsgeschäfts erforderlich sind. Sie erfassen z. B. Angebote, Aufträge und Gutschriften und erstellen Rechnungen.

Im Part Verkauf finden Sie folgende Themen:
- "Suchfunktionen"
- "Vorgangsverwaltung"
- "Technische Werte"
- "Stückliste"
- "Packmittelplanung"
- "Anmerkungen"
- "Texte"
- "Preise und Konditionen"
- "Freischaltung"
- "Lieferung"
- "Rechnungen"
- "Gutschriften"
- "Formulare"
- "Auftragsstatus"
- "Recherche zu Vorgängen"
- "Übersichten zu Vorgängen"
- "Vertrieb"

## Menü Verkauf
Einige der verfügbaren Menü-Einträge verzweigen in Untermenüs. Wenn diese mehr als drei Einträge umfassen, sind sie nach der folgenden Übersicht separat aufgeführt.

Die angezeigten Einträge sind von der jeweiligen Konfiguration abhängig.

Für zusätzliche Dokumentationen, die in diesem Part zum Menü Verkauf nicht enhalten sind, oder bei Fragen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

> **Kontext-Menüs**
> In den Kontext-Menüs (rechte Maustaste) werden zu den einzelnen Feldern der Dialoge jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen in den Kontext-Menüs können Sie auch über die beschriebenen Menüs aufrufen. In der Regel entsprechen die Menüpunkte im Kontext-Menü den angebotenen Funktionen in der Prompt-Anzeige.

Alle Dialoge und Funktionen, die den Verkauf betreffen, erreichen Sie über das Menü Verkauf:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Schnellerfassung | ⇨ "Schnellerfassung" |
| b | Angebotserfassung | ⇨ "Angebotserfassung" |
| c | Auftragserfassung | ⇨ "Auftragserfassung" |
| d | Preiskalkulation | ⇨ "Preiskalkulation" |
| e | Preislose Erfassung | ⇨ "Preislose Erfassung" |
| f | Lieferscheine | |
| fa | • Automatische Freigabe | ⇨ "Lieferscheine (automatisch)" |
| fb | • Manuelle Lieferscheine | ⇨ "Lieferscheine (manuell)" |
| fc | • Protokoll | ⇨ "Lieferscheinprotokoll" |
| g | Rechnungen | ⇨ "Untermenü Rechnungen" |
| h | Gutschriften | |
| ha | • Gutschriften erfassen | ⇨ "Gutschriften" |
| hb | • Gutschriften buchen | ⇨ "Gutschriften buchen" |
| i | Auftragsfreischaltung | |
| ia | • Freischaltung | ⇨ "Auftragsfreischaltung" |
| ib | • Autorisierung | ⇨ "Autorisierung" |
| j | Formulare | |
| ja | • Druck | ⇨ "Formulardruck" |
| jb | • E-Mail/Fax | ⇨ "E-Mail" |
| k | Listendruck | ⇨ "Listendruck" |
| l | Übersicht | ⇨ "Untermenü Übersicht" |
| m | Hintergrund-Kontrolle | ⇨ "Fehlerinformationssystem" |
| n | Wiedervorlagen | ⇨ "Wiedervorlage" |
| o | Fertigmeldung | ⇨ "Fertigmeldung" |
| p | Vorgangsänderung | ⇨ "Vorgangsänderung" |
| r | Vertrieb | ⇨ "Vertrieb" |

### Untermenü Rechnungen
**Pfad:** `Verkauf > Rechnungen`

Über dieses Menü erreichen Sie alle Dialoge, in denen Sie die Rechnungen erstellen und verwalten.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Automatische Freigabe | ⇨ "Rechnungen (automatisch)" |
| b | Manuelle Rechnung | ⇨ "Rechnungen (manuell)" |
| c | Thekenrechnung | ⇨ "Thekenrechnung" |
| d | Rechnungen buchen | ⇨ "Rechnungen buchen" |
| e | Abschlagsrechnung | |
| ea | • Automatische Freigabe | ⇨ "Abschlagsrechnung (automatisch)" |
| eb | • Manuelle Rechnung | ⇨ "Abschlagsrechnung (manuell)" |
| f | Schlussrechnung | |
| fa | • Automatische Freigabe | ⇨ "Schlussrechnung (automatisch)" |
| fb | • Manuelle Rechnung | ⇨ "Schlussrechnung (manuell)" |
| g | Protokoll | ⇨ "Rechnungsprotokoll" |

### Untermenü Übersicht
**Pfad:** `Verkauf > Übersicht`

Über dieses Menü erreichen Sie alle Dialoge, in denen Sie sich eine Übersicht über die verschiedenen Vorgänge anzeigen lassen können.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Unberechnete Aufträge | ⇨ "Übersicht zu Vorgängen" |
| b | Ungebuchte Rechnungen | |
| c | Unvollständige Lieferungen | |
| d | Aufträge mit Fakturasperre | |
| e | Bearbeitungsstände | Das Modul wird nicht mehr genutzt. |
| f | Nummern-Ermittlung | Das Modul wird nicht mehr genutzt. |
| g | Auftragsanzeige | ⇨ "Auftragsanzeige" |
| h | Angebotsanzeige | ⇨ "Angebotsanzeige" |
| i | Auftragsinformation | ⇨ "Auftragsinformation" |
| j | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" |

## Zusatzmenü
Das Zusatzmenü rufen Sie mit `<F4>` beim Erfassen der verschiedenen Vorgänge auf, z. B. bei einem Auftrag.
Je nach Dialog und Bereich werden die Einträge im Zusatzmenü in verschiedenen Ausführungen angezeigt. Als Beispiel werden die Einträge beschrieben, die beim Aufrufen des Zusatzmenüs in der Vorgangserfassung angezeigt werden:
- Zusatzmenü für den Kopf- und Fußbereich (Vorgangserfassung)
- Zusatzmenü für die Positionsebene (Vorgangserfassung)

### Zusatzmenü für den Kopf- und Fußbereich (Vorgangserfassung)

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Texte | |
| aa | • Kopftext | ⇨ "Kopf- und Fußtexte" |
| ab | • Fußtext | ⇨ "Kopf- und Fußtexte" |
| ac | • Fremdinformationen | ⇨ "Fremdinformationen" |
| b | Adressen | ⇨ "Untermenü Adressen" |
| c | Ansprechpartner | ⇨ "Ansprechpartner" |
| d | Storno | ⇨ "Auftragspositionen" |
| e | Preisangaben | ⇨ "Untermenü Preisangaben" |
| f | Produktangaben | ⇨ "Untermenü Produktangaben" |
| g | Wiedervorlage | ⇨ "Wiedervorlage" |
| h | Übergabe an Produktion (erneut) | Den Auftrag nach dem Speichern automatisch an die Produktion übergeben. |
| i | Produktionsmonitor | ⇨ "Produktionsmonitor" |
| j | Lieferplan | ⇨ "Lieferplan" |
| k | Lieferinformation | ⇨ "Lieferinformation - Details der Auslieferung" |
| l | Zahlungsplan | ⇨ "Zahlungsplan" |
| m | Zahlungsverwaltung | ⇨ "Zahlungsverwaltung" |
| n | Konfigurierbare Felder | ⇨ "Konfigurierbare Felder" |
| o | Hauswechsel | ⇨ "Hauswechsel" |
| p | Direktdruck | ⇨ "Direktdruck" |

### Zusatzmenü für die Positionsebene (Vorgangserfassung)

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Texte | ⇨ "Untermenü Texte" |
| b | Adressen | ⇨ "Untermenü Adressen" |
| c | Storno | ⇨ "Auftragspositionen" |
| d | Private Felder | ⇨ "Private Felder" |
| e | Preisangaben | ⇨ "Untermenü Preisangaben" |
| f | Produktangaben | ⇨ "Untermenü Produktangaben" |
| g | Wiedervorlage | ⇨ "Wiedervorlage" |
| h | Kommissionen | |
| ha | • neue Kommission | In das Feld Kommis im Register Positionen wechseln, um einen Kommissionstext anzulegen oder zu bearbeiten. |
| hb | • Kommission ändern | ⇨ "Auftragspositionen - Allgemein" |
| i | Lieferplan | ⇨ "Lieferplan" |
| j | Lager | |
| ja | • Stapel (Strg+P) | Das Feld Stapel im Register Allgemein anzeigen. Die Stapelanzeige ist eine optionale Funktion und wird kundenspezifisch konfiguriert. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH. |
| jb | • Lagerprognose (Strg+G) | ⇨ "Bestandsprognose" |
| k | Zahlungsplan | ⇨ "Zahlungsplan" |
| l | Konfigurierbare Felder | ⇨ "Konfigurierbare Felder" |

### Untermenü Adressen
**Pfad:** `<F4> > Adressen`

Über dieses Menü verwalten Sie vorgangsbezogen die Adressen.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Lieferadresse suchen (Strg+L) | ⇨ "Adressen Suche" |
| b | Neue Lieferadresse (Strg+N) | ⇨ "Neue Lieferadresse" |
| c | Lieferadresse löschen | Die Lieferadresse aus dem Vorgang löschen. |
| d | Endkundenanschrift | ⇨ "Endkundenanschrift" |

### Untermenü Texte
**Pfad:** `<F4> > Texte`

Über dieses Menü verwalten Sie die Texte. Die Einträge **Artikeltext (F5)**, **Positionstext (Shift+F5)** und **Spezielle Texte** werden nur auf Positionsebene angezeigt.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Kopftext | ⇨ "Kopf- und Fußtexte" |
| b | Fußtext | ⇨ "Kopf- und Fußtexte" |
| c | Fremdinformationen | ⇨ "Fremdinformationen" |
| d | Artikeltext (F5) | ⇨ "Artikel- und Positionstexte" |
| e | Positionstext (Shift+F5) | ⇨ "Artikel- und Positionstexte" |
| f | Spezielle Texte | ⇨ "Untermenü Spezielle Texte" |

### Untermenü Spezielle Texte
**Pfad:** `<F4> > Texte > Spezielle Texte`

Über dieses Menü verwalten Sie alle speziellen Texte, die Sie dem Vorgang oder der Position zuordnen können.
Spezielle Texte ist eine optionale Funktion und wird kundenspezifisch konfiguriert. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Rahmentext | ⇨ "Spezielle Texte" |
| b | Produktkennzeichen | |
| c | Modelltexte | |
| d | Logotexte | |

### Untermenü Preisangaben
**Pfad:** `<F4> > Preisangaben`

Über dieses Menü verwalten Sie die Preise und Konditionen für einen Vorgang oder einzelne Positionen.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Auftragskonditionen | ⇨ "Positionskonditionen" |
| b | Auftragspreise | ⇨ "Untermenü Auftragspreise" |
| c | Teilkalkulation | ⇨ "Produktionskostenkalkulation" |

Die folgenden Einträge werden nur zu den Vorgangspositionen angezeigt:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| d | + | ⇨ "Positionskonditionen" |
| e | Konditionen holen | Den Verkaufspreis mit den Positionskonditionen ermitteln und den Preis neu berechnen. |
| f | Preisberechnung | Den Positionspreis neu berechnen. |
| g | Preiskontrolle | Die Felder zur Preiskontrolle im Register Allgemein anzeigen. |

### Untermenü Auftragspreise
**Pfad:** `<F4> > Preisangaben > Auftragspreise`

Über dieses Menü verwalten Sie die Auftragspreise für einzelne Positionen.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Artikelpreise | ⇨ "Auftragspreise" |
| b | Sprossenpreise | ⇨ "Auftragssprossenpreise" |
| c | Austauschpreise | ⇨ "Auftragsaustauschpreise" |
| d | Unterteilpreise | ⇨ "Auftragsunterteilpreise" |

### Untermenü Produktangaben
**Pfad:** `<F4> > Produktangaben`

Über dieses Menü verwalten Sie die Angaben für die Produkte, z. B. Austausch- und Zusatzregeln.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Produktaustausch | ⇨ "Produktaustausch" |
| b | A/Z-Regeln | ⇨ Stammdaten, "Austausch-/Zusatzregel" |

Die folgenden Einträge werden nur auf Positionsebene angezeigt:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| c | Warengruppe | Die Warengruppe bearbeiten. Der Cursor wechselt in das Feld `Warengrp`. |
| d | Technische Werte | ⇨ "Untermenü Technische Werte" |

### Untermenü Technische Werte
**Pfad:** `<F4> > Produktangaben > Technische Werte`

Über dieses Menü verwalten Sie die technischen Werte.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Technische Werte anzeigen | Die technischen Werte anzeigen. ⇨ "Register Positionen (linker Bereich)" |
| b | Technische Werte ändern | Die technischen Werte bearbeiten. Der Cursor wechselt in das Feld dB-Wert der technischen Werte im Register Positionen. ⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" |
| c | Leistungserklärung | ⇨ "Leistungserklärung" |
| d | Verdeckte Maßangaben anzeigen | Die verdeckten Maßangaben im Register Positionen anzeigen. ⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" |
| e | Verdeckte Maßangaben ändern | ⇨ "Artikel-Maßangaben" |

## Infomenü
**Tastenkombination:** `<Shift> + <F4>`

Je nach Dialog und Bereich werden die Einträge im Infomenü in verschiedenen Ausführungen angezeigt. Als Beispiel werden die Einträge beschrieben, die beim Aufrufen des Infomenüs in der Vorgangserfassung angezeigt werden:
- Infomenü für den Kopf- und Fußbereich (Vorgangserfassung)
- Infomenü für die Positionsebene (Vorgangserfassung)

### Infomenü für den Kopf- und Fußbereich (Vorgangserfassung)

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Vorgangs-Anmerkungen | ⇨ "Anmerkungen" |
| b | Marktpartner-Anmerkungen | |
| c | Objekt-Anmerkungen | |
| d | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" |
| e | Vorgangs-Übersicht | ⇨ "Übersicht" |
| f | Marktpartner-Information | ⇨ "Marktpartner-Info" |
| g | Änderungsprotokoll | ⇨ "Änderungs-Protokoll" |
| h | Lieferterminänderungen | ⇨ "Lieferterminänderungs-Protokoll" |
| i | Auftragsinformation | ⇨ "Auftragsinformation" |
| k | Kistensignatur | ⇨ "Kistensignatur" |
| l | Dokumentenarten | ⇨ "DXF Import" |
| m | Dokumentenübersicht | ⇨ "Dokumentenartenzuordnung" |

### Infomenü für die Positionsebene (Vorgangserfassung)

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Anmerkungen | ⇨ "Untermenü Anmerkungen" |
| b | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" |
| c | Vorgangs-Übersicht | ⇨ "Übersicht" |
| d | Marktpartner-Information | ⇨ "Marktpartner-Info" |
| e | Änderungsprotokoll | ⇨ "Änderungs-Protokoll" |
| f | Lieferterminänderungen | ⇨ "Lieferterminänderungs-Protokoll" |
| g | Auftragsinformation | ⇨ "Auftragsinformation" |
| h | Kistensignatur | ⇨ "Kistensignatur" |
| i | Dokumentenübersicht | ⇨ "Dokumentenartenzuordnung" |

### Untermenü Anmerkungen
**Pfad:** `<Shift> + <F4> > Anmerkungen`

Über dieses Menü verwalten Sie alle internen Informationen zu Vorgängen, Marktpartnern oder Objekten.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Vorgangs-Anmerkungen | ⇨ "Anmerkungen" |
| b | Artikel-Anmerkungen | |
| c | Kunden-Anmerkungen | |
| d | Kunden-Artikel-Anmerkungen | |
| e | Objekt-Anmerkungen | |
| f | Objekt-Artikel-Anmerkungen | |
| g | Lieferanten-Anmerkungen | |
| h | Lieferanten-Artikel-Anmerkungen | |

## Suchfunktionen
Sie können im Modul **Verkauf** über unterschiedliche Kriterien nach Vorgängen, Marktpartnern, Adressen und Artikeln suchen.
Die Suchdialoge sind für alle Vorgangsarten im Verkauf gleich aufgebaut. Sie werden in diesem Kapitel am Beispiel **Auftrag** beschrieben. Abweichungen werden explizit beschrieben.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Suche Aufträge"
- "Suche Aufträge – Trefferliste"
- "Marktpartnersuche"
- "Mitarbeiter/Berechtigungsgruppen"
- "Suche Bezugsvorgang"
- "Adressen Suche"
- "Artikel-Suche"
- "Artikel-Suche nach Typen"
- "Produktsuche nach Elementen"
- "Objekt-Suche"
- "Werteingabe - Erweiterte Suche"

## Suche Aufträge
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9>`

In diesem Dialog suchen Sie nach Aufträgen. Im Kopfbereich geben Sie die Suchkriterien an. Mit jedem Kriterium, das Sie angeben, können Sie die Treffermenge reduzieren.

In diesem Dialog finden Sie im Kopfbereich folgende Register:
- "Suche Aufträge – Vorgangs-Schlüssel”
- "Suche Aufträge - Positions-Schlüssel"
- "Suche Aufträge – Direkte Suche"

Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.
⇨ "Suche Aufträge - Trefferliste"

### Suche Aufträge – Vorgangs-Schlüssel
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9>`

*Abb. D-1: Suche Aufträge - Vorgangs-Schlüssel*

In diesem Register suchen Sie Aufträge anhand von Auftragsdaten. Es ist konfigurierbar, in welchem Suchkriterienfeld Sie sich für die Eingabe zuerst befinden, wenn sie den Dialog öffnen. Konfigurierbar als erste Eingabefelder im Register **Vorgangs-Schlüssel** sind die Felder **Aufträge ab, Kunde, Objekt, Rechnungsnummer, Liefertermin, Bestelldatum, USt-Ident-Nr., Erfasser, Erfassungsdatum und Währung**.

Sie können zusätzliche Suchkriterien im Register **Positions-Schlüssel** angeben. Konfigurierbar als erste Eingabefelder im Register **Positions-Schlüssel** sind die Felder **Artikel, Mengeneinheit und Maßvariante**.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Vorgangs-Schlüssel**
- **Aufträge ab**: Nummer, ab der nach Aufträgen gesucht wird. Die Suche wird auf alle Aufträge beschränkt, deren Nummer gleich oder größer der angegebenen Auftragsnummer ist. Der Feldname variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Angebote ab. *Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr*
- **Kunde**: Kundennummer. Die Suche wird auf alle Aufträge von diesem Kunden beschränkt. Wenn Sie eine Nummer angeben, wird der Kundenname im Klartext angezeigt. *Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kauf.kunr, kauf.orgname*
- **Hausnummer**: Mandantennummer. Standardmäßig ist die Nummer des eigenen Hauses vorbelegt. Die Suche wird auf alle Aufträge aus diesem Haus beschränkt. Das Feld kann nur bearbeitet werden, wenn Sie mit der internen Mandantentrennung arbeiten. *Technische Info: numerisches Feld, DB-Feld: kauf.hausnr*
- **Objekt**: Objektnummer, für die Aufträge gesucht werden. Die Suche wird auf alle Aufträge mit diesem Objekt beschränkt. Der Objektname wird nach Eingabe der Nummer im Klartext angezeigt. *Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kauf.objnr, kauf.orgname*
- **Fremdnummer**: Auftragsnummer, die vom Kunden vorgegeben wird. Die Suche wird auf alle Aufträge mit dieser Fremdnummer beschränkt. *Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr*
- **Org. Vorgang**: Original-Vorgangsnummer bei übertragenen Vorgängen. Die Suche wird auf alle Aufträge mit diesem Referenzvorgang beschränkt. *Technische Info: numerisches Feld, DB-Feld: kauf._orgauftrnr*
- **Rechnungsnummer**: Die Suche wird auf alle Aufträge beschränkt, zu denen diese Rechnung erstellt wurde. *Technische Info: numerisches Feld, DB-Feld: kauf.rechnr*
- **Liefertermin**: Gewünschter Liefertermin des Auftrags. Die Suche wird auf alle Aufträge mit diesem Liefertermin beschränkt. Der Liefertermin kann als Datum oder Kalenderwoche angegeben sein. In der Trefferliste wird der geplante Liefertermin angezeigt. *Technische Info: Datumsfeld, DB-Feld: kauf.ltplan*
- **Bestelldatum**: Bestelldatum des Auftrags. Die Suche wird auf alle Aufträge mit diesem Bestelldatum beschränkt. *Technische Info: Datumsfeld, DB-Feld: kauf.bdat*
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Kunden. Die Suche wird auf alle Aufträge mit dieser Identifikationsnummer beschränkt. *Technische Info: alphanumerisches Feld, DB-Feld: kaufp.steuernr*
- **Erfasser**: Mitarbeiternummer des Sachbearbeiters, der die Aufträge erfasst hat. Die Suche wird auf alle Aufträge von diesem Erfasser beschränkt. *Technische Info: numerisches Feld, DB-Feld: kauf.eusr*
- **Erfassungsdatum**: Datum der Auftragserfassung. Die Suche wird auf alle Aufträge mit diesem Erfassungsdatum beschränkt. *Technische Info: Datumsfeld, DB-Feld: kauf.edat*
- **Währung**: Währung, die dem Auftrag zugeordnet ist. Die Suche wird auf alle Aufträge mit dieser Währung beschränkt. *Technische Info: numerisches Feld, DB-Feld: kauf.waehrung*

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut:
⇨ "Suche Aufträge - Trefferliste"

**Fußbereich**
- **Neue Suche**: Löscht alle Suchkriterien für eine neue Suche. Alternativ können Sie mit `<Strg> + <F7>` die Suchkriterien löschen.
- **Suchen**: Startet die Suche mit den angegebenen Kriterien. Alternativ können Sie die Suche mit `<F3>` starten.

### Suche Aufträge – Positions-Schlüssel
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Register Positions-Schlüssel`

*Abb. D-2: Suche Aufträge - Positions-Schlüssel*

In diesem Register suchen Sie Aufträge anhand der Positionsdaten. Sie können zusätzliche Suchkriterien in den Registern **Vorgangs-Schlüssel** und **Direkte Suche** angeben.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Positions-Schlüssel**
- **Artikel**: Artikelnummer. Die Suche wird auf alle Aufträge beschränkt, die diesen Artikel als Positionsartikel beinhalten. Wenn Sie eine Nummer angeben, wird die Artikelbezeichnung im Klartext angezeigt. Die Stücklisten der Positionen werden nicht geprüft. *Technische Info: numerisches Feld, DB-Feld: kpos.artnr*
- **Kundenprodukt**: Referenznummer für kundenspezifische Produkte aus den Stammdaten. Die Suche wird auf alle Aufträge mit Artikeln dieser kundenspezifischen Nummer beschränkt. *Technische Info: alphanumerisches Feld, DB-Feld: kpos.kuposnr*
- **Breite, Höhe**: Breite und Höhe der Position in Millimeter. Die Suche wird auf alle Aufträge mit Artikeln dieser Maße beschränkt. *Technische Info: numerische Felder, DB-Felder: kpos.laenge, kpos.breite*
- **Kommission**: Kommissionstext. Die Suche wird auf alle Aufträge beschränkt, die den angegebenen Kommissionstext enthalten. *Technische Info: alphanumerisches Feld, DB-Feld: komm.kommtxt*
- **Mengeneinheit**: Mengeneinheit der Position, z. B. Quadratmeter. Die Suche wird auf alle Aufträge mit dieser Mengeneinheit beschränkt. *Technische Info: numerisches Feld, DB-Feld: kpos.me*
- **Maßvariante**: Maßvariante des Artikels. Die Suche wird auf alle Aufträge mit diesen Variantenartikeln beschränkt. *Technische Info: numerisches Feld, DB-Feld: kpos.var*

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut:
⇨ "Suche Aufträge - Trefferliste"

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

### Suche Aufträge – Direkte Suche
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Register Direkte Suche`

*Abb. D-3: Suche Aufträge - Direkte Suche*

In diesem Register suchen Sie Aufträge ab einer bestimmten Auftragsnummer. Sie können zusätzliche Suchkriterien in den Registern **Vorgangs-Schlüssel** und **Positions-Schlüssel** angeben.
Wenn die Suchfunktion auf die direkte Suche nach Auftragsnummern beschränkt werden soll, dann kann der Dialog so konfiguriert werden, dass die Register **Vorgangs-Schlüssel** und **Positions-Schlüssel** deaktiviert sind. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Direkte Suche**
- **Aufträge ab**: Startnummer, ab der aufsteigend nach Aufträgen gesucht wird. Die Suche wird auf alle Aufträge beschränkt, deren Nummern gleich oder größer der angegebenen Auftragsnummer ist. Der Feldname variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Angebote ab. *Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr*

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

### Suche Aufträge – Trefferliste
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Suchkriterien eingeben > <F3>`

In der Trefferliste finden Sie folgende Register:
- "Suche Aufträge - Lieferinfos"
- "Suche Aufträge - Verschiedenes"
- "Suche Aufträge – Mengen"
- "Suche Aufträge - Eigenschaften"
- "Suche Aufträge – Kommission"

### Suche Aufträge – Lieferinfos
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Suchkriterien eingeben > <F3>`

*Abb. D-4: Suche Aufträge – Lieferinfos*

In diesem Register werden die Lieferinformationen und weitere Details zu den Aufträgen angezeigt, die den Suchkriterien entsprechen.
Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Aufträge beschrieben.

**Satzanzeige für die Vorgangsübersicht**
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Vorgangsübersicht: Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der Treffer`.

**Register Lieferinfos**
- **Haus**: Mandantennummer (Hausnummer). *Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr*
- **Auftrag**: Auftragsnummer. Der Spaltenname und die Nummer variieren je nach Vorgang, aus dem Sie die Suche öffnen, z. B. Angebot und Angebotsnummer bei der Angebots-Suche. *Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr*
- **Subnr.**: Nummer des Teillieferscheins oder der Teilrechnung. *Technische Info: Anzeigefeld, DB-Feld: kauf.subnr*
- **Lieferdatum**: Geplanter Liefertermin. *Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan*
- **Kunde**: Kundenname. *Technische Info: Anzeigefeld, DB-Feld: kauf.orgkunr*
- **Objekt**: Objektnummer bei Aufträgen, denen ein Objekt zugeordnet ist. *Technische Info: Anzeigefeld, DB-Feld: kauf.objnr*
- **Rechnung**: Rechnungsnummer bei fakturierten Aufträgen. *Technische Info: Anzeigefeld, DB-Feld: kauf.rechnr*
- **Org. Vorgang**: Original-Vorgangsnummer bei übertragenen Vorgängen. *Technische Info: Anzeigefeld, DB-Feld: kauf._orgauftrnr*
- **Storniert**: Angabe des Bearbeitungsstands, z. B. Stornostatus.
    - `0`: Nicht stornierter Auftrag.
    - `1`: Vom Benutzer stornierter Auftrag.
    - `2`: Vom System stornierter Auftrag.
    - `-3, -10, ..., -x`: Auftrag in Hintergrundbearbeitung.
    *Technische Info: Anzeigefeld, DB-Feld: kauf.still*

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

### Suche Aufträge – Verschiedenes
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Suchkriterien eingeben > <F3> > Register Verschiedenes`

*Abb. D-5: Suche Aufträge - Verschiedenes*

In diesem Register werden diverse Informationen zu den Aufträgen angezeigt, die den Suchkriterien entsprechen.
Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Aufträge beschrieben.

**Satzanzeige**
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Vorgangsübersicht: Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der Treffer`.

**Register Verschiedenes**
Die Spalten sind zum Register Lieferinfos beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **Erfassung**: Datum der Auftragserfassung. *Technische Info: Anzeigefeld, DB-Feld: kauf.edat*
- **Erfasser**: Name des Sachbearbeiters, der die Aufträge erfasst hat. *Technische Info: Anzeigefeld, DB-Feld: kauf.eusr*
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Kunden. *Technische Info: Anzeigefeld, DB-Feld: kaufp.steuernr*
- **Referenz**: Vorgangsnummer, auf die bei der Vorgangserfassung Bezug genommen wurde. *Technische Info: Anzeigefeld, DB-Feld: kauf.referenz*

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

### Suche Aufträge – Mengen
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Suchkriterien eingeben > <F3> > Register Mengen`

*Abb. D-6: Suche Aufträge – Mengen*

In diesem Register werden die Positionsinformationen zu den Aufträgen angezeigt, die den Suchkriterien entsprechen. Pro Auftragsposition wird eine Zeile angezeigt.
Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Aufträge beschrieben.

**Satzanzeige für die Positionsübersicht**
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Positionsübersicht: Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der Treffer`.

**Register Mengen**
Die Spalten sind zum Register **Lieferinfos** beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **Pos**: Positionsnummer im Auftrag. *Technische Info: numerisches Feld, DB-Feld: kpos.posnr*
- **Artnr, Artikel**: Artikelnummer und Artikelbezeichnung des Kopfartikels. *Technische Info: numerisches Feld, alphanumerisches Feld, DB-Felder: kpos.artnr, kpos.artbez1*
- **Menge**: Positionsmenge. *Technische Info: numerisches Feld, DB-Feld: kpos.menge*
- **Gelief.**: Bereits gelieferte Positionsmenge. *Technische Info: numerisches Feld, DB-Feld: kpos.gelief*
- **Kompl.**: Ein Stern `*` zeigt an, wenn die Position komplett geliefert ist. *Technische Info: Anzeigefeld*
- **Fakt.**: Fakturierte Positionsmenge. *Technische Info: numerisches Feld, DB-Feld: kpos.gesberech*
- **Kompl.**: Ein `F` zeigt an, wenn die Position komplett fakturiert ist. *Technische Info: Anzeigefeld*

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

### Suche Aufträge – Eigenschaften
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Suchkriterien eingeben > <F3> > Register Eigenschaften`

*Abb. D-7: Suche Aufträge - Eigenschaften*

In diesem Register werden zusätzliche Positionsinformationen aus Aufträgen angezeigt. Pro Auftragsposition wird eine Zeile angezeigt.
Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Aufträge beschrieben.

**Satzanzeige für die Positionsübersicht**
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Positionsübersicht: Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der Treffer`.

**Register Eigenschaften**
Die Spalten sind zu den Registern Lieferinfos und Mengen beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **ΜΕ**: Mengeneinheit der Position, z. B. Quadratmeter. *Technische Info: Anzeigefeld, DB-Feld: kpos.me*
- **qm**: Glasfläche des Artikels pro Stück in Quadratmeter. *Technische Info: Anzeigefeld, DB-Feld: kpos.qm*
- **lfm**: Längenangabe für den Artikels pro Stück in Umlaufenden Meter. *Technische Info: Anzeigefeld, DB-Feld: kpos.umlfdm*
- **Gewicht**: Gewicht der Position in Kilogramm. *Technische Info: Anzeigefeld, DB-Feld: kpos.gewicht*
- **Breite, Höhe**: Maße des Artikels in Millimeter. *Technische Info: Anzeigefelder, DB-Feld: kpos.laenge, kpos.breite*
- **Maßvariante**: Maßvariante des Artikels. *Technische Info: Anzeigefeld, DB-Feld: kpos.var*

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

### Suche Aufträge – Kommission
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <F9> > Suchkriterien eingeben > <F3> > Register Kommission`

*Abb. D-8: Suche Aufträge – Kommission*

In diesem Register werden Informationen zu Kommissionen der Aufträge angezeigt, die den Suchkriterien entsprechen. Pro Auftragsposition wird eine Zeile angezeigt.
Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Aufträge beschrieben.

**Satzanzeige für die Positionsübersicht**
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Positionsübersicht: Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der Treffer`.

**Register Kommission**
Die Spalten sind zu den Registern **Lieferinfos** und **Mengen** beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **Kommission**: Kommissionstext. *Technische Info: Anzeigefeld, DB-Feld: komm.kommtxt*

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register Vorgangs-Schlüssel beschrieben.

## Marktpartnersuche
**Pfad:** `Verkauf > Auftragserfassung > Feld Kunde > <F9>`

*Abb. D-9: Marktpartnersuche*

In diesem Dialog suchen Sie nach Marktpartnern. Die Suchkriterien geben Sie im Kopfbereich an. Wenn Sie die Marktpartnersuche öffnen, werden Ihnen alle Marktpartner in der Trefferliste angezeigt, die in den Stammdaten hinterlegt und nicht stillgelegt sind. Bei interner Mandantentrennung werden nur die Marktpartner aufgelistet, die dem Haus zugeordnet sind. Über die Filterkriterien können Sie die Trefferliste beschränken.

Es ist konfigurierbar, in welchem Suchkriterienfeld Sie sich für die Eingabe zuerst befinden, wenn sie den Dialog öffnen. Konfigurierbar als erste Eingabefelder sind die Felder **Ab Nummer, Matchcode, Name, Vorname, Land, PLZ und Ort**.

Sie können die Marktpartnersuche über verschiedene Menüpfade aufrufen. Der Dialog ist immer gleich aufgebaut.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

In der Trefferliste werden die Adressen und Informationen zur Identifikation der Marktpartner angezeigt:
- "Register Adresse"
- "Register Identifikation"

> **Voreinstellung des Marktpartnertypen**
> Je nachdem über welchen Menüpfad Sie den Dialog öffnen, ist der Marktpartnertyp, nach dem gesucht wird, bereits voreingestellt, z. B. Kunde oder Lieferant. Die Trefferliste wird dann entsprechend vorgefiltert. Die Auswahl des Marktpartnertypen ist nur bei der Suche in den Stammdaten möglich.

### Suchfelder
- **Ab Nummer**: Startnummer, ab der aufsteigend nach Marktpartnern gesucht wird. Die Marktpartner, deren Nummer kleiner als die angegebene Nummer ist, werden aus der Trefferliste ausgeschlossen. *Technische Info: numerisches Feld, DB-Feld: mp.mpnr*
- **Matchcode**: Alphanumerischer Matchcode des Marktpartners. Die Marktpartner, deren Matchcode nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: mp.mc*
- **Typ**: Anzeige des Marktpartnertyps. Der Typ ist in den Marktpartnerstammdaten hinterlegt. Das Feld wird automatisch vom System vorbelegt. *Technische Info: Anzeigefeld, DB-Feld: mp.kuliflag*
- **Name, Vorname**: Name und Vorname des Marktpartners. Die Marktpartner, deren Namen nicht die angegebenen Daten enthalten, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: mp.name, mp.vname*
- **Straße**: Straßenname und Hausnummer des Marktpartners. Die Marktpartner, deren Straße und Hausnummer nicht die angegebenen Daten enthalten, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: mp.strasse*
- **Haus**: Mandantennummer (Hausnummer) bei interner Mandantentrennung. Die Marktpartner, die nicht dem angegebenen Haus zugeordnet sind, werden aus der Trefferliste ausgeschlossen. *Technische Info: numerisches Feld, DB-Feld: mpmdzu.hnr*
- **Land**: Internationales Länderkennzeichen des Marktpartners. Die Marktpartner, deren Länderkennzeichen nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: mp.land*
- **PLZ, Ort**: Postleitzahl und Ortsname der Anschrift des Marktpartners. Die Marktpartner, deren Postleitzahl und Ort nicht die angegebenen Daten enthalten, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: mp.plz, mp.ort*
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Marktpartners. Die Marktpartner, deren Identifikationsnummer nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: mp.steuernr*
- **Art**: Marktpartnerstatus. In der Vorgangserfassung werden nur aktive Marktpartner angezeigt. Das Feld kann nicht bearbeitet werden. *Technische Info: Anzeigefeld, DB-Feld: mp.still*

### Satzanzeige für die Marktpartnerübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Anzeige bedeutet `Nr. des aktuell markierten Treffers in der Liste: Gesamtzahl der angezeigten Treffer in der Liste (Gesamtzahl der Treffer)`.

> **Die Anzeige von Treffern wird satzweise geladen**
> Wenn eine große Menge an Treffern angezeigt werden muss, dann kann das System dafür unter Umständen viel Zeit brauchen. Damit die Trefferliste schnell angezeigt werden kann, wird sie satzweise geladen. Die Satzgröße wird in den Systemeinstellungen konfiguriert. Die Treffer werden in numerischer Reihenfolge geladen, z. B. die numerisch ersten 100 Treffer. Weitere Treffer können mit der Schaltfläche [Weitere Daten] geladen werden.
>
> **Beispiel**
> In der Satzanzeige wird `11:100 (1256)` angezeigt.
> `11` steht für die Nummer des markierten Treffers in der Trefferliste.
> `100` steht für die Anzahl der Treffer, die aktuell in der Trefferliste angezeigt werden.
> `1256` steht für die Anzahl aller Treffer.

### Register Adresse
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Nummer**: Marktpartnernummer. *Technische Info: Anzeigefeld, DB-Feld: mp.mpnr*
- **Zusatz**: Ergänzende Anmerkung, z. B. ein Adresszusatz. *Technische Info: Anzeigefeld, DB-Feld: mp.branche*

### Register Identifikation
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Nummer**: Marktpartnernummer. *Technische Info: Anzeigefeld, DB-Feld: mp.mpnr*
- **Still**: Anzeige, ob der Marktpartner stillgelegt ist.
    - `J`: Marktpartner ist stillgelegt.
    - `N`: Marktpartner ist aktiv.
    In der Vorgangserfassung werden nur aktive Marktpartner angezeigt. *Technische Info: Anzeigefeld, DB-Feld: mp.still*
- **Typ**: Typ des Marktpartners, z. B. Kunde, Lieferant. *Technische Info: Anzeigefeld, DB-Feld: mp.kuliflag*
- **Firma**: Nummer der Firma des Marktpartners bei interner Mandantentrennung. Die Firmennummer wird aus den Systemstammdaten herangezogen. *Technische Info: Anzeigefeld, DB-Feld: xcompany.compid*

### Fußbereich
Mit den Schaltflächen im Fußbereich navigieren Sie in der Trefferliste, zeigen weitere Treffer an und aktualisieren die Trefferliste.
- **`<` | `<<` | `>>` | `>`**: Mit `[<]` und `[>]` wechseln Sie zum ersten oder letzten Eintrag in der Trefferliste. Mit `[<<]` und `[>>]` zeigen Sie die vorherige oder nächste Seite der Trefferliste an.
- **Refresh**: Aktualisiert die Einträge in den Suchfeldern. Korrigierte oder zusätzliche Einträge in den Suchfeldern werden dadurch bei der Suche berücksichtigt. Die Schaltfläche ist nur im Bereich **Suchfelder** freigeschaltet.
- **Weitere Daten**: Zeigt in der Trefferliste weitere Einträge an, die den Suchkriterien entsprechen. Wenn keine weiteren Treffer mehr angezeigt werden können, ist die Schaltfläche gesperrt.
- **Neue Suche**: Löscht alle Suchkriterien für eine neue Suche. Alternativ können Sie die Suchkriterien mit `<Strg> + <R>` löschen und eine neue Suche starten.

## Mitarbeiter/Berechtigungsgruppen
**Pfad:** `Verkauf > Auftragserfassung > Register Eigenschaften > Feld Sachbearbeiter > <F9>`

*Abb. D-10: Mitarbeiter/Berechtigungsgruppen*

In diesem Dialog suchen Sie nach Mitarbeitern. Die Suchkriterien geben Sie im Kopfbereich an. Wenn Sie die Mitarbeitersuche öffnen, werden Ihnen alle Mitarbeiter in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.

Sie können die Mitarbeitersuche über verschiedene Menüpfade aufrufen. Der Dialog ist immer gleich aufgebaut.
- Mit `<F3>` starten Sie die Suche.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

In der Trefferliste werden die Mitarbeiter angezeigt, die den Suchkriterien entsprechen.

### Suchfelder
- **Ab Nummer**: Startnummer, ab der aufsteigend nach Mitarbeitern gesucht wird. Die Mitarbeiter, deren Nummer kleiner als die angegebene Nummer ist, werden aus der Trefferliste ausgeschlossen. *Technische Info: numerisches Feld, DB-Feld: mitarb.manr*
- **Typ**: Anzeige des Mitarbeitertyps. Der Typ ist in den Mitarbeiterstammdaten hinterlegt. Das Feld wird automatisch vom System vorbelegt. *Technische Info: Anzeigefeld, DB-Feld: mitarb.matyp*
- **Name, Vorname**: Name und Vorname des Mitarbeiters. Die Mitarbeiter, deren Namen nicht die angegebenen Daten enthalten, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: mitarb.maname, mitarb.vname*
- **Abteilung**: Nummer und Bezeichnung der Abteilung. Wenn Sie eine Nummer angeben, wird die Bezeichnung der Abteilung im zweiten Feld angezeigt. *Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: mitabr.abtnr, abteilung.bez*
- **Login**: Benutzername des Mitarbeiters zur Anmeldung bei A+W Enterprise. *Technische Info: alphanumerisches Feld, DB-Feld: mitarb.loginname*

### Satzanzeige für die Mitarbeiterübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Satzanzeige ist zum Dialog **Marktpartnersuche** beschrieben.

### Trefferliste
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich wird folgende Spalte angezeigt:
- **Nummer**: Mitarbeiternummer. *Technische Info: Anzeigefeld, DB-Feld: mitarb.manr*

### Fußbereich
Mit den Schaltflächen im Fußbereich navigieren Sie in der Trefferliste, zeigen weitere Treffer an und aktualisieren die Trefferliste. Die Felder und Schaltflächen im Fußbereich sind ausführlich zur Marktpartnersuche beschrieben.

## Suche Bezugsvorgang
**Pfad:** `Verkauf > Auftragserfassung > Feld Bezug > <F9>`

*Abb. D-11: Suche Bezugsvorgang*

In diesem Dialog suchen Sie nach Vorgängen, auf die Sie in der Vorgangserfassung Bezug nehmen können.
Im Kopfbereich geben Sie die Suchkriterien an. Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.

Der Dialog ist wie der Dialog **Suche Aufträge** aufgebaut.

### Register Vorgangs-Schlüssel
Die meisten Felder sind zum Register **Vorgangs-Schlüssel** zur Auftragssuche beschrieben. Zusätzlich werden folgende Felder angezeigt:
- **Vorgang**: Vorgangsart. Die Suche wird auf alle Vorgänge dieser Art beschränkt.
    - Angebot
    - Auftrag
    - Lieferantenanfrage
    - Bestellung
    *Technische Info: Auswahl-Feld, DB-Feld: kauf.vorgang*

> **Standard-Voreinstellung der Vorgangsart**
> Die Vorgangsart ist benutzerindividuell voreingestellt, z. B. Angebot. Die Voreinstellung konfigurieren Sie in den Systemeinstellungen.

- **Vorgangsnummer**: Nummer und Subnummer des Bezugsvorgangs. Die Suche wird auf alle Vorgänge mit dieser Nummer und/oder Subnummer beschränkt. *Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.auftrnr, kauf.subnr*
- **Geplant**: Geplantes Lieferdatum des Bezugsvorgangs im Format TT.MM.JJJJ. Die Suche wird auf alle Vorgänge mit diesem Lieferdatum beschränkt. *Technische Info: Datumsfeld, DB-Feld: kauf.ltplan*

### Register Positions-Schlüssel
Die Felder sind zum Register **Positions-Schlüssel** zur Auftragssuche beschrieben.

### Register Direkte Suche
- **Aufträge ab**: Startnummer, ab der aufsteigend nach Aufträgen gesucht wird. Die Suche wird auf alle Aufträge mit Nummern gleich oder größer dieser Auftragsnummer beschränkt. Der Feldname variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Angebote ab. *Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr*

### Trefferliste
Die Register in der Trefferliste sind ausführlich zur Auftragssuche beschrieben.

### Fußbereich
Die Schaltflächen im Fußbereich sind in der Auftragssuche zum Register **Vorgangs-Schlüssel** beschrieben.

## Adressen Suche
**Pfad:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Adressen > Lieferadresse suchen`

*Abb. D-12: Adressen Suche*

In diesem Dialog suchen Sie nach Adressen des Marktpartners. Die Suchkriterien geben Sie im Kopfbereich an. Wenn Sie die Adressen-Suche öffnen, werden Ihnen alle Adressen des Marktpartners in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

In der Trefferliste werden die Lieferadressen und weitere Kontaktdaten des Marktpartners angezeigt.

### Suchfelder
- **Name**: Kundenname. Die Adressen von Kunden, deren Name nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: adr.adrname*
- **Strasse**: Straßenname und Hausnummer der Lieferadresse. Die Adressen, deren Straßenname und Hausnummer nicht die angegebenen Daten enthalten, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: adr.str*
- **PLZ**: Postleitzahl der Lieferadresse. Die Adressen, deren Postleitzahl nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: adr.plz, adr.ort*
- **Ort**: Ortsname der Lieferadresse. Die Adressen, deren Ort nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: adr.plz, adr.ort*
- **Land**: Ländername des Lieferziels. Die Adressen aus Ländern, die nicht die angegebenen Daten enthalten, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: adr.land*
- **Adressencode**: Code der gespeicherten Adresse. Die Adressen, deren Adresscode nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: adr.text1*
- **Tel**: Telefonnummerdes Kunden. Die Adressen, deren Telefonnummer nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: adr.telefon, adr.email*
- **E-Mail**: E-Mail-Adresse des Kunden. Die Adressen, deren E-Mail-Adresse nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerische Felder, DB-Felder: adr.telefon, adr.email*
- **Incl. Schnellerfassung**: Angabe, ob Adressen aufgelistet werden, die über die Schnellerfassung gespeichert sind.
    - ☑ Die Adressen aus der Schnellerfassung werden in der Trefferliste angezeigt.
    - ☐ Aus der Schnellerfassung werden keine Adressen in der Trefferliste angezeigt.
    ⇨ "Schnellerfassung"
    *Technische Info: Checkbox*

### Hauptlieferadresse
Die Hauptlieferadresse des Marktpartners wird rechts, über den Registern, angezeigt.
Wenn dem Marktpartner keine Hauptlieferadresse zugewiesen ist, wird keine Hauptadresse angezeigt.

### Register Adresse, Register Kontaktdaten
Die Spalten auf Positionsebene entsprechen den Feldern im Kopfbereich. Zusätzlich wird folgende Spalte angezeigt:
- **Vorname**: Vorname des Kunden. *Technische Info: Anzeigefeld, DB-Feld: adr.adrvname*

### Fußbereich
- **Details**: Öffnet einen Dialog mit den Details zur markierten Lieferadresse. Alternativ können Sie den Dialog mit `<F5>` öffnen. Die Schaltfläche ist nur freigeschaltet, wenn eine Adresse in der Trefferliste markiert ist.
- **Neue Suche**: Löscht alle Suchkriterien für eine neue Suche.

## Artikel-Suche
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9>`

In diesem Dialog suchen Sie nach Artikeln, die Sie für die Erfassung eines Auftrags benötigen. Sie können die Artikel-Suche über verschiedene Menüpfade aufrufen. Der Dialog ist immer gleich aufgebaut.

Die Treffer der Suche werden in den Registern angezeigt. Wenn Sie die Artikel-Suche öffnen, werden Ihnen alle Artikel in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.

Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.

In diesem Dialog finden Sie folgendes Register:
- "Artikel-Suche - Kopf-, Fußbereich"
- "Artikel-Suche - Bezeichnungen"
- "Artikel-Suche - Artikelcodes"
- "Artikel-Suche - Details"

Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.

### Artikel-Suche – Kopf-, Fußbereich
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9>`

*Abb. D-13: Artikel-Suche – Kopf-, Fußbereich*

In diesem Dialog suchen Sie Artikel anhand von verschiedenen Suchkriterien. Wenn Sie die Artikel-Suche öffnen, werden Ihnen alle Artikel in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.

**Kopfbereich**
Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt.
Mit `<F3>` starten Sie die Suche.

- **Ab Nummer**: Startnummer, ab der aufsteigend nach Artikeln gesucht wird. Die Artikel, deren Nummer kleiner als die angegebene Artikelnummer ist, werden aus der Trefferliste ausgeschlossen. *Technische Info: numerisches Feld, DB-Feld: artikel.artnr*
- **Matchcode**: Alphanumerischer Matchcode des Artikels. Die Artikel, deren Matchcode nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen. *Technische Info: alphanumerisches Feld, DB-Feld: artikel.artmc*
