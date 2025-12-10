---
description: "DE_AWEnterprise_Einkauf"
---


# A+W Einkauf E

A+W - Software for Glass, Windows and Doors

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 5.00 / 12-2022 | Diverse Ergänzungen in der Softwarereferenz |
| 4.00 / 08-2020 | Vollständige Überarbeitung |
| 3.00 / 06-2019 | Vollständige Überarbeitung |
| 2.01 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 2.00 / 03-2014 | Vollständige Überarbeitung |
| 1.00 / 02-2007 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:

- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von **A+W Enterprise** gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

#### Urheberrechte

© 2022, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte

A+W Software GmbH
Am Pfahlgraben 4-10
35415 Pohlheim
+49 6404 2051-0
+49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

## Inhalt

- **Vorspann**
  - Revisionsübersicht (E-3)
  - Editorial (E-3)
- **Softwarereferenz** (E-9)
  - Übersicht (E-11)
  - Suchfunktionen (E-21)
  - Bestellpool (E-34)
  - Vorgangsverwaltung (E-47)
  - Texte (E-96)
  - Wareneingang (E-103)
  - Rechnungen und Gutschriften (E-128)
  - Übersichten (E-144)
- **Partindex** (E-151)
  - Index Einkauf (E-153)

## Softwarereferenz

### Übersicht

Im Modul **Einkauf** verwalten Sie die Vorgänge, die zur erfolgreichen Abwicklung des Einkaufsgeschäfts erforderlich sind, wie Bestellungen, Anfragen, Wareneingänge und Rechnungen.

Im Part Einkauf finden Sie folgende Themen:
- "Suchfunktionen" auf Seite E-21
- "Vorgangsverwaltung" auf Seite E-47
- "Bestellpool" auf Seite E-34
- "Texte" auf Seite E-96
- "Wareneingang" auf Seite E-103
- "Rechnungen und Gutschriften" auf Seite E-128
- "Übersichten" auf Seite E-144

#### Menü Einkauf

Einige der verfügbaren Menü-Einträge verzweigen in Untermenüs. Wenn diese mehr als drei Einträge umfassen, sind sie nach der folgenden Übersicht separat aufgeführt.

Die angezeigten Einträge sind von der jeweiligen Konfiguration abhängig.
- Konfiguration Bestellpool
- Konfiguration Auftragsorientierter Bestelldruck - diese Konfiguration findet keine Anwendung statt. Aus diesem Grund wird das hier nicht beschrieben.
- Konfiguration Eigene Einkaufsvorgänge

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

> **Kontext-Menüs**
> In den Kontext-Menüs (rechte Maustaste) werden zu den einzelnen Feldern der Dialoge jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen in den Kontext-Menüs können Sie auch über die beschriebenen Menüs aufrufen. In der Regel entsprechen die Menüpunkte im Kontext-Menü den angebotenen Funktionen in der Prompt-Anzeige.

Alle Dialoge und Funktionen, die den Verkauf betreffen, erreichen Sie über das Menü **Einkauf**:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Bestellungen erzeugen | ⇨ "Bestellungen erzeugen" auf Seite E-37 |
| b | Anfragen | ⇨ "Lieferanten-Anfragen" auf Seite E-50 |
| c | Bestellverwaltung | ⇨ "Bestellerfassung" auf Seite E-50 |
| d | Formular | |
| da | • Druck | ⇨ Verkauf, "Formulardruck" auf Seite D-357 |
| db | • E-Mail/Fax | ⇨ Verkauf, "E-Mail" auf Seite D-361 |
| e | Listendruck | ⇨ Verkauf, "Listendruck" auf Seite D-364 |
| f | Bestell-Freigabe | ⇨ "Bestellfreigabe" auf Seite E-98 |
| g | Lieferavis | ⇨ "Lieferavis" auf Seite E-103 |
| h | Wareneingang | ⇨ "Untermenü Wareneingang" auf Seite E-13 |
| i | Rechnungen | ⇨ "Untermenü Rechnungen" auf Seite E-13 |
| j | Gutschriften | |
| ja | • Gutschriften erfassen | ⇨ "Lieferanten-Gutschrift" auf Seite E-142 |
| jb | • Gutschriften buchen | ⇨ Verkauf, "Gutschriften buchen" auf Seite D-354 |
| k | Übersicht | ⇨ "Untermenü Übersicht" auf Seite E-14 |
| l | Recherche | ⇨ "Einkaufs-Recherche" auf Seite E-145 |

##### Konfiguration Bestellpool

Bei der Einkaufskonfiguration Bestellpool handelt sich um meist verbreiterte Einstellungen. Die Erklärungen, Beispiele und weitere Hinweise in diesem Dokument basieren sich, sofern nichts weiteres explizit erwähnt ist, auf diese Konfiguration.

##### Konfiguration Eigene Einkaufsvorgänge

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Lagerbestellung erzeugen | ⇨ "Bestellungen erzeugen" auf Seite E-37 |
| b | Anfragen erfassen und bearbeiten | ⇨ "Lieferanten-Anfragen" auf Seite E-50 |
| c | Bestellungen erfassen und bearbeiten | ⇨ "Bestellerfassung" auf Seite E-50 |
| d | Druck von Formularen verwalten | ⇨ Verkauf, "Formulardruck" auf Seite D-357 |
| e | Druck von Listen verwalten | ⇨ Verkauf, "Listendruck" auf Seite D-364 |
| f | Mehrere Bestellungen freischalten und verwalten | ⇨ "Bestellfreigabe" auf Seite E-98 |
| g | Einzelne Bestellungen freischalten und verwalten | ⇨ "Bestellfreigabe" auf Seite E-98 |
| h | Lieferbestätigungen erfassen und verwalten | ⇨ "Lieferavis" auf Seite E-103 |
| i | Wareneingang verwalten | ⇨ "Untermenü Wareneingang" auf Seite E-13 |
| j | Rechnungen erfassen und bearbeiten | ⇨ "Untermenü Rechnungen" auf Seite E-13 |
| ka | Lieferanten-Gutschriften erfassen | ⇨ "Lieferanten-Gutschrift" auf Seite E-142 |
| kb | Gutschriften buchen | ⇨ Verkauf, "Gutschriften buchen" auf Seite D-354 |
| l | Vorgangsübersichten anzeigen | ⇨ "Untermenü Übersicht" auf Seite E-14 |
| m | Vorgänge im Einkauf suchen | ⇨ "Einkaufs-Recherche" auf Seite E-145 |

##### Untermenü Wareneingang
**Einkauf > Wareneingang**

Über dieses Menü erreichen Sie die Dialoge, in denen Sie den Wareneingang verwalten.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| ha | Lieferplan | ⇨ "Lieferplan" auf Seite E-111 |
| hb | Automatischer Wareneingang | ⇨ "Wareneingang (automatisch)" auf Seite E-114 |
| hc | Manueller Wareneingang | ⇨ "Wareneingang (manuell)" auf Seite E-119 |
| hd | Gestellbezogener Wareneingang | ⇨ "Gestellbezogener Wareneingang" auf Seite E-121 |
| he | Bestellungen abschließen | ⇨ "Wareneingang" auf Seite E-103 |
| hf | Wareneingangskontrolle | ⇨ "Wareneingangskontrolle" auf Seite E-125 |
| hg | Fehlmengenkontrollpool | ⇨ "Fehlmengenkontrollpool" auf Seite E-126 |
| hh | Protokoll | ⇨ "Rechnungsprotokoll" auf Seite E-142 |

##### Untermenü Rechnungen
**Einkauf > Rechnungen**

Über dieses Menü erreichen Sie die Dialoge, in denen Sie die Einkaufsrechnungen verwalten.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| ia | Rechnungskontrolle | ⇨ "Rechnungskontrolle" auf Seite E-128 |
| ib | Automatische Rechnungen | ⇨ "Lieferanten-Rechnung (automatisch)" auf Seite E-135 |
| ic | Übertragene Rechnungen | ⇨ "Übertragene Rechnungen" auf Seite E-137 |
| id | Manuelle Rechnungen | ⇨ "Lieferanten-Rechnung (manuell)" auf Seite E-138 |
| ie | Sammelrechnungen | ⇨ "Lieferanten-Rechnung (Sammelrechnung)" auf Seite E-139 |
| if | Rechnungen buchen | ⇨ "Rechnungen buchen" auf Seite E-140 |
| ig | Bestellungen abschließen | ⇨ "Wareneingang" auf Seite E-103 |
| ih | Protokoll | ⇨ "Rechnungsprotokoll" auf Seite E-142 |

##### Untermenü Übersicht
**Einkauf > Übersicht**

Über dieses Menü erreichen Sie die Dialoge, in denen Sie sich Übersichten zu den verschiedenen Vorgängen anzeigen lassen können.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| ka | Heute geplanter Wareneingang | ⇨ "Diese Übersichten sind konfigurationsabhängig und müssen separat freigeschaltet werden. Diese Dialoge können bei Bedarf kundenindividuell gestaltet werden. Bitte kontaktieren Sie einen Service-Mitarbeiter der A+W Software GmbH." auf Seite E-145 |
| kb | Geplanter Wareneingang – verspätet | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| kc | Geplanter Wareneingang von-bis | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| kd | Geliefert - nicht berechnet | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| ke | Berechnet - nicht gebucht | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| kf | Noch nicht übertragene Best. | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| kg | Vorgangs-Recherche | ⇨ Verkauf, "Vorgangs-Recherche" auf Seite D-380 |
| kh | Bestellinformation | ⇨ "Bestellinformation" auf Seite E-144 |

#### Zusatzmenü

Das Zusatzmenü rufen Sie mit `<F4>` beim Erfassen der verschiedenen Vorgänge auf, z. B. bei einer Bestellung.
Die Einträge im Zusatzmenü werden in kontextabhängigen Ausführungen angezeigt:
- Zusatzmenü für den Kopf- und Fußbereich
- Zusatzmenü für den Positionsbereich

##### Zusatzmenü für den Kopf- und Fußbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | **Texte** | |
| aa | • Kopftext | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-252 |
| ab | • Fußtext | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-252 |
| ac | • Fremdinformationen | ⇨ Verkauf, "Fremdinformationen" auf Seite D-258 |
| b | **Adressen** | |
| ba | • Lieferadressen suchen | ⇨ Verkauf, "Adressen Suche" auf Seite D-45 |
| bb | • Neue Lieferadresse | ⇨ Verkauf, "Neue Lieferadresse" auf Seite D-136 |
| bc | • Lieferadresse löschen | Löscht die Lieferadresse aus dem Vorgang. |
| bd | • Abholadresse | ⇨ "Abholadresse" auf Seite E-92 |
| c | **Storno** | ⇨ "Bestellarten" auf Seite E-94 |
| d | **Preisangaben** | ⇨ "Untermenü Preisangaben" auf Seite E-16 |
| e | **Produktangaben** | |
| ea | • Produktaustausch | ⇨ "Bestellarten" auf Seite E-94 |
| eb | • A/Z-Regeln | ⇨ Stammdaten, "Austausch-/Zusatzregel" auf Seite J-102 |
| f | **Wiedervorlage** | ⇨ Verkauf, "Wiedervorlage" auf Seite D-398 |
| g | **Konfigurierbare Felder** | ⇨ Verkauf, "Konfigurierbare Felder" auf Seite D-144 |

##### Zusatzmenü für den Positionsbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | **Texte** | |
| aa | • Kopftext | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-252 |
| ab | • Fußtext | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-252 |
| ac | • Fremdinformationen | ⇨ Verkauf, "Fremdinformationen" auf Seite D-258 |
| ad | • Artikeltext | ⇨ Verkauf, "Artikel- und Positionstexte" auf Seite D-254 |
| ae | • Positionstext | ⇨ Verkauf, "Artikel- und Positionstexte" auf Seite D-254 |
| af | • Spezielle Texte | ⇨ "Untermenü Preisangaben" auf Seite E-16 |
| b | **Adressen** | |
| ba | • Lieferadressen suchen | ⇨ Verkauf, "Adressen Suche" auf Seite D-45 |
| bb | • Neue Lieferadresse | ⇨ Verkauf, "Neue Lieferadresse" auf Seite D-136 |
| bc | • Lieferadresse löschen | Löscht die Lieferadresse aus dem Vorgang. |
| bd | • Endkundenanschrift | ⇨ Verkauf, "Endkundenanschrift" auf Seite D-138 |
| c | **Storno** | ⇨ "Bestellarten" auf Seite E-94 |
| d | **Private Felder** | ⇨ Verkauf, "Private Felder" auf Seite D-163 |
| e | **Preisangaben** | ⇨ "Untermenü Preisangaben" auf Seite E-16 |
| f | **Produktangaben** | ⇨ "Untermenü Produktangaben" auf Seite E-17 |
| g | **Wiedervorlage** | ⇨ Verkauf, "Wiedervorlage" auf Seite D-398 |
| h | **Kommission** | |
| ha | • neue Kommission | ⇨ "Bestellpositionen - Allgemein" auf Seite E-71 |
| hb | • Kommission ändern | ⇨ "Bestellpositionen - Allgemein" auf Seite E-71 |
| i | **Lieferplan** | ⇨ Verkauf, "Lieferplan" auf Seite D-325 |
| j | **Lager** | |
| ja | • Stapel | ⇨ "Bestellpositionen - Allgemein" auf Seite E-71 |
| jb | • Lagerprognose | ⇨ Verkauf, "Bestandsprognose" auf Seite D-149 |
| k | **Konfigurierbare Felder** | ⇨ Verkauf, "Konfigurierbare Felder" auf Seite D-144 |

##### Untermenü Preisangaben
**<F4> > Preisangaben**

Über dieses Menü verwalten Sie die Preise und Konditionen für den Artikel der markierten Position.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Auftragskonditionen | ⇨ Verkauf, "Positionskonditionen" auf Seite D-279 |
| b | Auftragspreise | ⇨ "Untermenü Auftragspreise" auf Seite E-16 |
| c | Teilkalkulation | ⇨ Verkauf, "Produktionskostenkalkulation" auf Seite D-311 |
| d | Positionskonditionen (nur Positionsbereich) | ⇨ Verkauf, "Positionskonditionen" auf Seite D-279 |
| e | Konditionen holen (nur Positionsbereich) | Ermittelt den Verkaufspreis mit den Positionskonditionen und berechnet den Preis neu. |
| f | Preisberechnung (nur Positionsbereich) | Berechnet den Positionspreis neu. |
| g | Preiskontrolle (nur Positionsbereich) | ⇨ "Bestellpositionen - Allgemein" auf Seite E-71 |

##### Untermenü Auftragspreise
**<F4> > Preisangaben > Auftragspreise**

Über dieses Menü verwalten Sie die Auftragspreise.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Artikelpreise | ⇨ Verkauf, "Auftragspreise" auf Seite D-267 |
| b | Sprossenpreise | ⇨ Verkauf, "Auftragssprossenpreise" auf Seite D-269 |
| c | Austauschpreise | ⇨ Verkauf, "Auftragsaustauschpreise" auf Seite D-272 |
| d | Unterteilpreise | ⇨ Verkauf, "Auftragsunterteilpreise" auf Seite D-274 |

##### Untermenü Spezielle Texte
**<F4> > Texte > Spezielle Texte**

Über dieses Menü verwalten Sie alle speziellen Texte, die Sie dem Vorgang zuordnen können. Diese Texte sind in der Regeln kundenindividuell konfigurierbar und somit sind sie nicht der Bestandteil dieser Dokumentation.
Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

##### Untermenü Produktangaben
**<F4> > Produktangaben**

Über dieses Menü verwalten Sie die Angaben für die Produkte, z. B. Austausch- und Zusatzregeln.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Produktaustausch | ⇨ "Bestellarten" auf Seite E-94 |
| b | A/Z-Regeln | ⇨ Stammdaten, "Austausch-/Zusatzregeln" auf Seite B-215 |
| c | Warengruppe (nur Positionsbereich) | ⇨ "Bestellpositionen - Allgemein" auf Seite E-71 |
| d | Technische Werte (nur Positionsbereich) | ⇨ "Untermenü Technische Werte" auf Seite E-17 |

##### Untermenü Technische Werte
**<F4> > Produktangaben > Technische Werte**

Über dieses Menü verwalten Sie die technischen Werte.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Technische Werte anzeigen | Zeigt die technischen Werte an. |
| b | Technische Werte ändern | Wechselt zu den technischen Werten, damit sie bearbeitet werden können. Der Cursor wechselt in das Feld dB-Wert der technischen Werte im Register Positionen. |
| c | Leistungserklärung | ⇨ Verkauf, "Texte" auf Seite E-96 |
| d | Verdeckte Maßangaben anzeigen | Zeigt die verdeckten Maßangaben im Register Positionen an. |
| e | Verdeckte Maßangaben ändern | ⇨ Verkauf, "Artikel-Maßangaben" auf Seite D-148 |

#### Infomenü
**<Shift> + <F4>**

Das Infomenü wird in kontextabhängigen Ausführungen angezeigt:
- Infomenü für den Kopf- und Fußbereich
- Infomenü für den Positionsbereich

##### Infomenü für den Kopf- und Fußbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Vorgangs-Anmerkungen | ⇨ Verkauf, "Anmerkungen" auf Seite D-243 |
| b | Marktpartner-Anmerkungen | |
| c | Objekt-Anmerkungen | |
| d | Vorgangs-Recherche | ⇨ Verkauf, "Vorgangs-Recherche" auf Seite D-380 |
| e | Vorgangs-Übersicht | ⇨ Verkauf, "Übersicht" auf Seite D-145 |
| f | Marktpartner-Information | ⇨ Verkauf, "Marktpartner-Info" auf Seite D-140 |
| g | Änderungsprotokoll | ⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-171 |
| h | Lieferplan | ⇨ "Lieferplan" auf Seite E-111 |
| i | Lieferterminänderungen | ⇨ Verkauf, "Lieferterminänderungs-Protokoll" auf Seite D-173 |
| j | Heute geplanter Wareneingang | ⇨ "Diese Übersichten sind konfigurationsabhängig und müssen separat freigeschaltet werden. Diese Dialoge können bei Bedarf kundenindividuell gestaltet werden. Bitte kontaktieren Sie einen Service-Mitarbeiter der A+W Software GmbH." auf Seite E-145 |
| k | Geplanter Wareneingang – verspätet | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| l | Geplanter Wareneingang von-bis | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| m | Geliefert - nicht berechnet | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| n | Berechnet - nicht gebucht | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |
| o | Gestellverwaltung | ⇨ "Buchung Gestelle" auf Seite E-117 |
| p | Auslieferdatum | Zeigt für auftragsbezogene Bestellungen folgende Informationen aus dem Kundenauftrag an: Auftragsnummer, Liefertermin, Route. |
| r | Bestellinformation | ⇨ "Bestellinformation" auf Seite E-144 |

##### Infomenü für den Positionsbereich

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Anmerkungen | ⇨ Untermenü Anmerkungen |
| b | Vorgangs-Recherche | ⇨ Verkauf, "Vorgangs-Recherche" auf Seite D-380 |
| c | Vorgangs-Übersicht | ⇨ Verkauf, "Übersicht" auf Seite D-145 |
| d | Marktpartner-Information | ⇨ Verkauf, "Marktpartner-Info" auf Seite D-140 |
| e | Änderungsprotokoll | ⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-171 |
| f | Lieferplan | ⇨ "Lieferplan" auf Seite E-111 |
| g | Gestellverwaltung | ⇨ "Buchung Gestelle" auf Seite E-117 |
| h | Bemerkung | ⇨ "Bestellpositionen - Allgemein" auf Seite E-71 |
| i | Auslieferdatum | Zeigt für auftragsbezogene Bestellungen folgende Informationen aus dem Kundenauftrag an: Auftragsnummer, Liefertermin, Route. |
| j | Bestellinformation | ⇨ "Bestellinformation" auf Seite E-144 |

##### Untermenü Anmerkungen
**<Shift> + <F4> > Anmerkungen**

Das Infomenü Anmerkungen wird nur im Register Bestellverwaltung – Positionen angezeigt.
Im Bestellkopf öffnen Sie die vorhandenen Anmerkungen über den Infomenü <Shift> + <F4> direkt.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Vorgangs-Anmerkungen | ⇨ Verkauf, "Anmerkungen" auf Seite D-243 |
| b | Lieferanten-Anmerkungen | |
| c | Lieferanten-Artikel-Anmerkungen | |
| d | Objekt-Anmerkungen | |
| e | Objekt-Artikel-Anmerkungen | |
| f | Kunden-Anmerkungen | |
| g | Kunden-Artikel-Anmerkungen | |

#### Zusatzmenü zum Wareneingang

In den Dialogen mit automatischen Datenverarbeitung, wie Wareneingang, Lieferanten-Rechnung, Bestellungen abschließen, kann mit `<F4>` das dialogspezifische Zusatzmenü aufgerufen werden. Die angezeigten Einträge sind optional, je nach dem, in welchen Dialog das Menü aufgerufen wurde. In der folgenden Übersicht des Menüs sind immer alle Einträge aufgeführt.

> **Kontext-Menüs**
> In den Kontext-Menüs zu den einzelnen Feldern der Dialog werden jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen entsprechen den Funktionen, die Sie über die im Folgenden beschriebenen Menüs aufrufen.

##### Wareneingang – Zusatzmenü
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
| h | Gestellverwaltung (Strg+G) | Öffnet den Dialog Buchung Gestelle. ⇨ "Gestellbezogener Wareneingang" auf Seite E-121 |
| i | Bemerkung (Strg+B) | Zeigt die Spalte Bemerkung an, in der Sie zusätzliche Informationen zur Bestellung angeben können. |

### Suchfunktionen

Sie können im Modul Einkauf über unterschiedliche Kriterien nach Vorgängen, Marktpartnern, Adressen, Artikeln und Objekten suchen.

Die Suchdialoge sind für alle Vorgangsarten im Einkauf gleich aufgebaut. Die Bedienung in den Suchdialogen ist analog dem Verkauf entwickelt worden. Die Suchfunktionen werden in dieser Anleitung am Beispiel Bestellungen beschrieben. Abweichungen zu anderen Dialogen, sowie zum Verkauf sind explizit genannt.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Suche Bestellungen" auf Seite E-21
- "Suche Bestellungen – Trefferliste" auf Seite E-26

Weitere Suchdialoge sind im Einkauf und Verkauf gleich. Sie sind ausführlich zum Part Verkauf beschrieben:
- Verkauf, "Suche Bezugsvorgang" auf Seite D-43
- Verkauf, "Marktpartnersuche" auf Seite D-37
- Verkauf, "Adressen Suche" auf Seite D-45
- Verkauf, "Artikel-Suche" auf Seite D-47
- Verkauf, "Artikel-Suche nach Typen" auf Seite D-56
- Verkauf, "Produktsuche nach Elementen" auf Seite D-57
- Verkauf, "Objekt-Suche" auf Seite D-64

#### Suche Bestellungen
**Einkauf > Anfragen > <F9> > Suchkriterien eingeben > <F3>**

In diesem Dialog suchen Sie nach Bestellungen.
Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.

In diesem Dialog finden Sie im Kopfbereich folgende Register:
- "Suche Bestellungen – Vorgangs-Schlüssel" auf Seite E-21
- "Suche Bestellungen – Positions-Schlüssel" auf Seite E-24
- "Suche Bestellungen – Direkte Suche" auf Seite E-25

Die Ergebnisse der Suche werden in der Trefferliste angezeigt:
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-26

##### Suche Bestellungen – Vorgangs-Schlüssel
**Einkauf > Anfragen, Bestellverwaltung > <F9>**

*[Image: Suche Bestellungen - Vorgangs-Schlüssel (Abb. E-1)]*

In diesem Register suchen Sie Bestellungen anhand der Lieferdaten.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Vorgangs-Schlüssel**
- **Bestellungen ab**: Nummer, ab der nach Bestellungen gesucht wird. Der Feldname variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Anfragen ab. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr)
- **Lieferant**: Lieferantennummer. Wenn Sie eine Nummer angeben, wird der Lieferantenname im Klartext angezeigt. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.kunr)
- **Fremd-Nr.**: Externe Nummer des Vorgangs. Als externe Nummer kann eine Nummer oder auch ein freier Text sein. Je nach Konfiguration wird das Feld Fremd-Nr. vom System vorbelegt. Diese Daten sind zum Dialog Bestellerfassung beschrieben: ⇨ "K-Auftrag" auf Seite E-53. Enthält das Feld alphanumerische Zeichen, so ist für die Suche Groß-/Kleinschreibung zu beachten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr)
- **Bestelldatum**: Datum, an dem die Bestellung freigeschaltet wurde. (Technische Info: Datumsfeld, DB-Feld: kauf.bdat)
- **Hausnummer**: Nummer des Hauses. Standardmäßig ist die eigene Hausnummer ausgewählt. Das Feld kann nur bearbeitet werden, wenn Sie mit der internen Mandantentrennung arbeiten. (Technische Info: numerisches Feld, DB-Feld: xhaus.haus)
- **Kunde**: Kundennummer. Wenn Sie eine Nummer angeben, wird der Kundenname im Klartext angezeigt. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.orgkunr, kauf.orgname)
- **Erfassungsdatum**: Datum der Vorgangserfassung. (Technische Info: Datumsfeld, DB-Feld: kauf.edat)
- **Erfasser**: Mitarbeiternummer des Vorgangserfassers. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiter im Klartext angezeigt. (Technische Info: numerisches Feld, DB-Feld: kauf.eusr)
- **Rechnungsnummer**: Nummer der Lieferantenrechnung. (Technische Info: numerisches Feld, DB-Feld: kauf.rechnr)
- **USt-Identnr.**: Umsatzsteuer-Identifikationsnummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kaufp.steuernr)

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-26

##### Suche Bestellungen – Positions-Schlüssel
**Einkauf > Bestellverwaltung > <F9> > Register Positions-Schlüssel**

*[Image: Suche Bestellungen – Positions-Schlüssel (Abb. E-2)]*

In diesem Register suchen Sie Bestellungen anhand der Positionsdaten.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

**Positions-Schlüssel**
Sie können die Bestellungen anhand der Daten aus den Positionen suchen. Geben Sie für diese Suche die bekannte Werte ein. Folgende Felder steht zur Eingabe zur Verfügung:
- **AB Lief.**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: numerisches Feld, DB-Feld: bpos.abnr)
- **LS-Nr.**: Lieferscheinnummer des Lieferanten. (Technische Info: numerisches Feld, DB-Feld: bpos.lieferschein)
- **Bemerk**: Textfeld für eine positionsbezogene Bemerkung, die im Dialog Lieferanten-Anfragen > Register AuftragsInfo > Feld Bemerkung positionsbezogen hinterlegt wird. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.bemerkung)
- **Auftragsnr.**: Auftragsnummer bei auftragsbezogenen Bestellungen. (Technische Info: numerisches Feld, DB-Feld: bpos.vksuftrnr)
- **Anlieferdatum**: Geplantes Datum der Anlieferung, ab dem nach Bestellungen gesucht wird. (Technische Info: Datumsfeld, DB-Feld: bpos.ltplan)
- **Objekt**: Objektnummer. Wenn Sie eine Nummer angeben, wird der Objektname im Klartext angezeigt. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bpos.vkobjnr)
- **Artikel**: Artikelnummer. Wenn Sie eine Nummer angeben, wird die Artikelbezeichnung im Klartext angezeigt. (Technische Info: numerisches Feld, DB-Feld: kpos.artnr)
- **ME**: Mengeneinheit der Position, z. B. Quadratmeter. (Technische Info: numerisches Feld, DB-Feld: kpos.me)
- **Lager**: Lagernummer der Bestellung. Wenn Sie eine Nummer angeben, wird die Lagerbezeichnung im Klartext angezeigt. (Technische Info: numerisches Feld, DB-Feld: bpos.Inr)
- **Maßvariante**: Maßvariante des Artikels. (Technische Info: numerisches Feld, DB-Feld: kpos.var)

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-26

##### Suche Bestellungen – Direkte Suche
**Einkauf > Bestellverwaltung > <F9> > Register Direkte Suche**

*[Image: Suche Bestellungen – Direkte Suche (Abb. E-3)]*

In diesem Register suchen Sie Bestellungen ab einer bestimmten Bestellnummer. Mithilfe einer Systemkonfiguration ist es möglich, diesen Register als Startdialog zu konfigurieren, um so eine einfache Suche zu verwenden.
- Mit `<F2>` wechseln Sie die Register im Kopfbereich.
- Mit `<F3>` starten Sie die Suche.

- **Bestellungen ab**: Nummer, ab der nach Bestellungen gesucht wird. Die Feldbezeichnung variiert je nach Dialog, aus dem Sie die Suche öffnen, z. B. Anfragen ab. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr)

**Trefferliste**
In der Trefferliste wird das Ergebnis der Suche angezeigt. Sie ist für alle Register des Kopfbereichs gleich aufgebaut.
⇨ "Suche Bestellungen - Trefferliste" auf Seite E-26

#### Suche Bestellungen – Trefferliste
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3>**

In der Trefferliste finden Sie folgende Register:
- "Trefferliste - Allgemein" auf Seite E-27
- "Trefferliste - Mengen" auf Seite E-29
- "Trefferliste – WE-Infos" auf Seite E-30
- "Trefferliste - Artikel" auf Seite E-31
- "Trefferliste - Verschiedenes" auf Seite E-32

##### Trefferliste – Allgemein
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Allgemein**

*[Image: Trefferliste (Suche Bestellungen) – Allgemein (Abb. E-4)]*

In diesem Register werden allgemeine Informationen zu den Bestellungen angezeigt, die den Suchkriterien entsprechen. Mit `<F2>` wechseln Sie die Register in der Trefferliste.

> **Satzanzeige**
> Am rechten oberen Dialograhmen wird die Satzanzeige angeboten: z. B.: Vorgangsübersicht: 137:227.
> 137 = die Satznummer der ausgewählten Zeile in der Trefferliste
> 227 = die Anzahl der Sätzen in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben: ⇨ "Suche Bestellungen" auf Seite E-21

**Register Allgemein**
- **Haus**: Hausnummer der jeweiligen Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr)
- **Bestellnr.**: Bestellnummer. Der Spaltenname variiert je nach Vorgang, aus dem Sie die Suche öffnen. (Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr)
- **Subnr.**: Nummer des Teillieferscheins oder der Teilrechnung. (Technische Info: Anzeigefeld, DB-Feld: kauf.subnr)
- **Lieferant**: Name des Lieferanten. (Technische Info: Anzeigefeld, DB-Feld: mp.name)
- **USt-Identnr.**: Umsatzsteuer-Identifikationsnummer des Lieferanten. (Technische Info: Anzeigefeld, DB-Feld: kaufp.steuernr)
- **Rechnung**: Nummer der Lieferantenrechnung. (Technische Info: Anzeigefeld, DB-Feld: kauf.rechnr)
- **Bestellt**: Datum, an dem die Bestellung freigeschaltet wurde. (Technische Info: Anzeigefeld, DB-Feld: kauf.bdat)
- **Erfasst**: Datum der Bestellerfassung. (Technische Info: Anzeigefeld, DB-Feld: kauf.edat)
- **Erfasser**: Name des Erfassers. (Technische Info: Anzeigefeld, DB-Feld: kauf.eusr)
- **Storniert**: Angabe des Bearbeitungsstands, z. B. Stornostatus.
  - 0: Nicht stornierter Auftrag.
  - 1: Vom Benutzer stornierter Auftrag.
  - 2: Vom System stornierter Auftrag.
  - -3, -10, ..., -x: Auftrag in Hintergrundbearbeitung. (Technische Info: Anzeigefeld, DB-Feld: kauf.still)

##### Trefferliste – Mengen
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Mengen**

*[Image: Trefferliste (Suche Bestellungen) – Mengen (Abb. E-5)]*

In diesem Register werden die Positionsinformationen zu den bestellten Artikel und der Menge angezeigt, die den Suchkriterien entsprechen. Pro Artikel-Bestellposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben: ⇨ "Suche Bestellungen" auf Seite E-21

**Register Mengen**
Zusätzlich werden folgende Spalten angezeigt:
- **Pos**: Positionsnummer in der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kpos.posnr)
- **Artnr., Artikel**: Artikelnummer und Artikelbezeichnung. (Technische Info: Anzeigefelder, DB-Felder: kpos.artnr, kpos.artbez1)
- **Menge**: Bestellte Stückzahl der Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.menge)
- **Eingang**: Eingetroffene Stückzahl der Position im Wareneingang. (Technische Info: Anzeigefeld, DB-Feld: kpos.geslief)
- **Kompl.**: Ein Stern `*` zeigt an, wenn die Position komplett geliefert ist. (Technische Info: Anzeigefeld)
- **Fakt.**: Fakturierte Stückzahl der Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.gesberech)
- **F.**: Ein `F` zeigt an, wenn die Position komplett fakturiert ist. (Technische Info: Anzeigefeld)
- **Breite, Höhe**: Maße der Position in Millimeter. (Technische Info: Anzeigefelder, DB-Felder: kpos.laenge, kpos.breite)

##### Trefferliste – WE-Infos
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register WE-Infos**

*[Image: Trefferliste (Suche Bestellungen) – WE-Infos (Abb. E-6)]*

In diesem Register werden die Wareneingangs-Informationen zu den Bestellungen angezeigt, die den Suchkriterien entsprechen. Pro Bestellposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben: ⇨ "Suche Bestellungen" auf Seite E-21

**Register WE-Infos**
Zusätzlich werden folgende Spalten angezeigt:
- **Anl.Datum**: Geplantes Datum der Anlieferung, ab dem nach Bestellungen gesucht wird. (Technische Info: Anzeigefeld, DB-Feld: bpos.ltplan)
- **AB-Nr. Lief.**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: Anzeigefeld, DB-Feld: bpos.abnr)
- **Lieferschein**: Lieferscheinnummer des Lieferanten. (Technische Info: Anzeigefeld, DB-Feld: bpos.lieferschein)
- **Auftrag**: Auftragsnummer bei auftragsbezogenen Bestellungen. (Technische Info: Anzeigefeld, DB-Feld: bpos.vksuftrnr)
- **Auslieferung**: Geplantes Lieferdatum des Kundenauftrags. (Technische Info: Anzeigefeld, DB-Feld: bpos.ltplan)

##### Trefferliste - Artikel
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Artikel**

*[Image: Trefferliste (Suche Bestellungen) – Artikel (Abb. E-7)]*

In diesem Register werden Informationen zu den Artikeleigenschaften der Bestellpositionen angezeigt. Pro Bestellposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben: ⇨ "Suche Bestellungen" auf Seite E-21

**Register Artikel**
Zusätzlich werden folgende Spalten angezeigt:
- **ME**: Mengeneinheit der Position, z. B. Quadratmeter. (Technische Info: Anzeigefeld, DB-Feld: kpos.me)
- **Maßvariante**: Maßvariante des Artikels. (Technische Info: Anzeigefeld, DB-Feld: kpos.var)

##### Trefferliste – Verschiedenes
**Einkauf > Bestellverwaltung > <F9> > Suchkriterien eingeben > <F3> > Register Verschiedenes**

*[Image: Trefferliste (Suche Bestellungen) – Verschiedenes (Abb. E-8)]*

In diesem Register werden diverse Informationen zu den Bestellungen angezeigt, die den Suchkriterien entsprechen. Pro Bestellposition wird eine Zeile angezeigt. Mit `<F2>` wechseln Sie die Register in der Trefferliste.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Dialog Suche Bestellungen beschrieben: ⇨ "Suche Bestellungen" auf Seite E-21

**Register Verschiedenes**
Zusätzlich werden folgende Spalten angezeigt:
- **Lager**: Lagernummer der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: bpos.Inr)
- **Kunde**: Kundenname für auftragsbezogene Bestellungen. (Technische Info: Anzeigefeld, DB-Feld: mp.name)

### Bestellpool

Im Bestellpool werden folgende Bestellvorschläge gesammelt, die zu einer oder mehreren Bestellung/-en zusammengefasst werden:
- Auftragsbezogene Bestellvorschläge aus dem Verkauf.
- Bestellvorschläge aus dem Lager, z. B. bevor der Lagerbestand in Unterdeckung läuft. Diese Funktion muss konfiguriert sein.
- Wenn keine automatischen Bestellvorschläge durch das Lager erzeugt werden, können Sie die Lagerbestellungen über den Dialog Bestellerfassung anlegen.

Bestellungen können je nach Systemkonfiguration und festgelegten Lieferanten-Stammdaten 1:1 aus den Auftragsdaten durch den Hintergrundprozess oder manuell im Bestellpool zuerst gruppiert, anschließend erzeugt werden.

Die Bestellfreigabe erfolgt entweder automatisch oder beim Bestelldruck. Folgende Möglichkeiten sind vorhanden:
- Die Bestellung wird erstellt und automatisch freigeschaltet.
- Die Bestellung wird gedruckt und automatisch freigeschaltet.
- Die Bestellung wird über den Dialog Bestellfreischaltung manuell freigeschaltet.

Je nach Systemkonfiguration ist die Bestellfreigabe über den Menüpunkt **Bestell-Freigabe** möglich: ⇨ "Bestellfreigabe" auf Seite E-98

Eine weitere Möglichkeit besteht bei entsprechender Systemkonfiguration beim Hinterlegen einer Avise. Sofern die Bestell-Avise gespeichert wird, wird die Bestellung in den Status **Bestellt** versetzt. ⇨ "Lieferavis" auf Seite E-103

Über den Dialog **Formulardruck** oder **E-Mail** können Sie Bestellungen drucken und an den Lieferanten senden. Die Dialoge sind ausführlich zum Part Verkauf beschrieben:
- ⇨ Verkauf, "Formulardruck" auf Seite D-357
- ⇨ Verkauf, "E-Mail" auf Seite D-361

Im Änderungsprotokoll können Sie den Status einer Bestellung prüfen. Der Dialog ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-171

In diesem Abschnitt finden Sie folgende Informationen:
- "Spezielle Menüs zum Bestellpool" auf Seite E-34
- "Bestellfreigabe" auf Seite E-98
- "Bestellungen erzeugen" auf Seite E-37

#### Spezielle Menüs zum Bestellpool

Im Bestellpool können dialogspezifische Menüs aufgerufen werden.
- Mit `<F4>` öffnen Sie das Zusatzmenü zum Bestellpool.
- Mit `<Shift> + <F4>` öffnen Sie das Infomenü zum Bestellpool.

Die angezeigten Einträge sind von der jeweiligen Konfiguration abhängig. In den folgenden Übersichten der Menüs sind immer alle Einträge aufgeführt.
Folgende Zusatzmenüs stehen zur Verfügung:
- "Bestellpool – Zusatzmenü" auf Seite E-35
- "Bestellpool – Infomenü" auf Seite E-36

> **Kontext-Menüs**
> In den Kontext-Menüs zu den einzelnen Feldern der Dialog werden jeweils nur die Menüpunkte angeboten, die im Kontext sinnvoll sind. Die Funktionen sind in folgenden Kapiteln beschriebenen.

##### Bestellpool – Zusatzmenü
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > <F4>**
(Meist genutzte Konfiguration)

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Markierte Positionen zurückstellen (Shift+F12) | Deaktiviert die Checkbox Er. (Bestellung erzeugen) für die markierten Positionen. Die Positionen können wieder bearbeitet werden. |
| b | Gruppieren nach Markierungen (Strg+F8) | Gruppiert die Positionen unter einer Bestellnummer. Die Checkbox Er. (Bestellung erzeugen) muss aktiv sein. |
| c | Gruppieren nach Aufträgen (Strg+O) | Die Checkbox Er. (Bestellung erzeugen) muss aktiv sein. Positionen mit derselben Auftragsnummer und demselben Lieferanten werden die Positionen unter einer gemeinsamen Bestellung gruppiert. Für Positionen mit derselben Auftragsnummer aber verschiedenen Lieferanten werden für die Positionen pro Lieferant einzelne Bestellung angelegt. Gruppierung nach Aufträgen ist u. a. konfigurationsabhängig. Bitte kontaktieren Sie einen Service-Mitarbeiter der A+W Software GmbH |
| d | Nach Bestellungen sortieren (Strg+F12) | Sortiert die Bestellnummern absteigend. |
| e | Bestellkopftext (Strg+K) | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-252 |
| f | Bestellfußtext (Strg+F) | ⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-252 |
| g | Markieren (nach unten) (Shift+F11) | Aktiviert die Checkboxen Er. (Bestellung erzeugen), für die ausgewählte und alle nachfolgenden Positionen. |
| h | Markieren (alle) (Strg+F11) | Aktiviert die Checkbox Er. (Bestellung erzeugen) für alle Positionen. |
| i | Storno | Keine Aktion in dieser Stelle |
| j | Anfrage (Strg+E) | Markiert die Spalte An (Anfrage) der ausgewählten Position mit einem A. Wenn die Checkbox Er. (Bestellung erzeugen) der Position aktiviert ist, können Sie mit <Strg> + <F8> eine Anfrage für den Lieferanten erstellen. |
| k | Alle Anfragen (Strg+L) | Markiert die Spalte An (Anfrage) aller Positionen mit einem A. Wenn die Checkbox Er. (Bestellung erzeugen) der Position aktiviert ist, können Sie mit <Strg> + <F8> eine Anfrage für den Lieferanten erstellen. |
| l | Anfragen ab Cursorposition (Strg+G) | Markiert die Spalte An (Anfrage) mit einem A für die ausgewählte und alle nachfolgenden Positionen. Wenn die Checkbox Er. (Bestellung erzeugen) der Position aktiviert ist, können Sie mit <Strg> + <F8> eine Anfrage für den Lieferanten erstellen. |
| m | Anfragen markieren (Strg+N) | Aktiviert die Checkbox Er. (Bestellung erzeugen) für alle Positionen mit einem A in der Spalte An (Anfrage). |
| n | Noch nicht übertragene Best. | ⇨ "Übersicht zu Vorgängen" auf Seite E-145 |

##### Bestellpool – Infomenü
**Einkauf > Bestellungen erzeugen > Abteilung angeben> <F3> > <Shift> + <F4>**

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Auftragstexte darstellen (Strg+F10) | ⇨ "Auftragstexte" auf Seite E-96 |
| b | Einkaufsinfo | In der ausgewählten, zu bestellenden Auftragsposition wird ein Extra-Feld Einkaufsinfo eingeblendet. Sofern solche Information im dazugehörigen Auftrag erfasst wurde, wird dieser Text in dem Feld angezeigt. Eine Neuerfassung der Einkaufsinformation im Bestellpool ist nicht möglich. |
| c | Lieferanten-Anmerkungen | ⇨ Verkauf, "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-246 |
| d | Lieferanten-Artikel-Anmerkungen | ⇨ Verkauf, "Kunden-Artikel-, Lieferanten-Artikel-, Objekt-Artikel-Anmerkungen" auf Seite D-249 |
| e | Artikel-Anmerkungen | ⇨ Verkauf, "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-246 |
| f | Reklamationsinformationen | Zeigt die Reklamationsinformationen für die ausgewählte Position aus dem Auftrag an. ⇨ "Bestellungen erzeugen" auf Seite E-37 |

#### Bestellungen erzeugen
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3>**
**Einkauf > Lagerbestellungen erzeugen**

In diesem Dialog können Sie Bestellvorschläge in Bestellungen umwandeln. Je nach Konfiguration des Programms und des gewünschten Ergebnis können Sie aus jeweils einen Bestellvorschlag die Bestellung erzeugen, oder mehrere Bestellungen unter einer Bestellnummer gruppieren.

Bestellvorschläge können auch automatisch erzeugt werden, wenn:
- der Lieferant für die bestellte Ware aus dem Auftrag in den Stammdaten als Direktlieferant markiert ist.
- wenn eine Lagerware-Unterdeckung vorliegt. Die Funktion zur automatischen Bestellungen aus dem Lager muss konfiguriert sein. Wenn Bestellvorschläge durch das Lager nicht automatisch erstellt werden können, müssen Sie die Lagerbestellungen über den Dialog Bestellerfassung anlegen. ⇨ "Bestellerfassung" auf Seite E-50

In diesem Dialog finden Sie folgende Register:
- "Bestellungen erzeugen – Lieferant" auf Seite E-37
- "Bestellungen erzeugen - Position" auf Seite E-41
- "Bestellungen erzeugen - Details" auf Seite E-43

##### Bestellungen erzeugen – Lieferant
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > Register Lieferant**

*[Image: Bestellung erzeugen - Lieferant (Abb. E-9)]*

In dem Bestellpool werden alle Bestellvorschläge gesammelt. Beim Arbeiten mit mehreren Einkaufsabteilungen oder/und Häuser können Sie den Auswahldialog konfigurieren, um den Datenbestand zu minimieren und entsprechend zu verteilen. Nach Auswahl des Hauses und/oder Abteilung werden die Bestellvorschläge im Dialog **Bestellung erzeugen** aufgelistet.

In diesem Register werden die Lieferanteninformationen zu den Bestellungsvorschlägen angezeigt.

Im Dialog **Bestellfreigabe** können Sie die Bestellungen freischalten. ⇨ "Bestellfreigabe" auf Seite E-98

**Auswahldialog**
- **Haus**: Auswahl der Nummer des Mandanten. Dieses Feld ist nur bei internen Mandantentrennung betretbar. (Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr)
- **Abteilung**: Abteilungsnummer. Mit `<F9>` können Sie nach einer Nummer suchen. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.abtnr)
- **Zusätzliche Bestellungen**: Bestellnummer. Mit `<F9>` können Sie nach einer Nummer suchen. Mit `<Enter>` können Sie eine weitere Bestellnummer angeben, die in einer neuen Zeile hinzugefügt wird. Sie können die Bestellnummern über die Schaltfläche **Zusätzliche Bestellungen** auf- oder absteigend sortieren. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr (kauf.vorgang=2))

Mit `<F3>` bestätigen Sie die Auswahl.

**Bestellung erzeugen**
Um die Bestellungen zu erzeugen, müssen folgende Schritte gemacht werden:
1. In dem Feld **Er.** markieren Sie die Bestellvorschläge, für die Sie eine Bestellung erzeugen wollen. Je nach Systemkonfiguration können bei Markierung einer der Bestellposition aus dem Auftrag auch alle weitere Bestellpositionen aus dem selben Auftrag mitmarkiert werden. Die Option Auftragspositionen zusammenhalten kann auch beim Markierung-Löschen angewendet werden.
2. Mit `<Strg> + <F8>` gruppieren Sie die Bestellvorschläge und erzeugen Bestellungen. Wenn Sie mehrere Positionen markieren, kann für die Positionen eine oder mehrere Bestellungen erzeugt werden. Die Gruppierung erfolgt entweder nach Markierung, Lieferantenwechsel, oder Aufträge. Die Art die Gruppierung kann über die Systemkonfiguration festgelegt werden.
3. Mit `<Ende>` lösen Sie die Bestellerzeugung aus und speichern die erstellten Bestellungen. Die Bestellungen können im Dialog Bestellverwaltung korrigiert und im Dialog Bestellfreigabe freigegeben werden.

**Gruppierung löschen**
Sie können die gruppierte Position mit bereits vergebenden Bestellnummer wieder zurücksetzen um die Position im Bestellpool zu lassen. Dafür markieren Sie die betroffene Position und entfernen diese einen auftragsbezogenen Bestellvorschlag entfernen, indem Sie die Bestellposition auswählen und über `<F4> > Markierte Positionen zurückstellen` die Bestellnummer für diese Bestellposition löschen.

**Register Lieferant**
- **Haus**: Nummer des Hauses. (Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr)
- **Best. Nr.**: Bestellnummer, unter der Bestellungen gruppiert werden können. Bestellnummern werden über die Auswahl der Spalte Er. vorläufig erstellt oder über die Auswahl der Spalte S storniert. Ihre Auswahl können Sie mit `<Ende>` oder [OK] bestätigen. (Technische Info: numerisches Feld, DB-Feld: bestpool.baufnr)
- **Er.**: Angabe, ob für die Position eine Bestellung erzeugt werden soll. Sie können mehrere Einträge markieren und in einer Bestellung gruppieren.
  - ☑ Die Position im Bestellpool ist für die Bestellungerzeugung markiert.
  - ☐ Für diese Position erfolgt keine Bestellungerzeugung.
  Mit `<Strg> + <F8>` gruppieren Sie die markierte Position für die Bestellerzeugung. Wenn Sie mehrere Positionen gleichzeitig markieren, wird je nach Systemkonfiguration eine oder mehrere Bestellungen erzeugt. (Technische Info: Checkbox)
- **Auftrag**: Auftragsnummer bei Bestellvorschlägen, die auftragsbezogen ermittelt werden. (Technische Info: numerisches Feld, DB-Feld: bestpool.orgauftrnr)
- **Artikel**: Artikelnummer, die bestellt werden soll. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: bestpool.artnr)
- **Bezeichnung**: Bezeichnung des Artikels aus der Bestellposition. (Technische Info: alphanumerisches Feld, DB-Feld: bestpool.artbez1)
- **S**: Anzeige, ob die zu bestellende Artikel bereits storniert wurde, z. B. zwischenzeitlich eine Auftragskorrektur vorgenommen wurde. Das Flag wird vom System gesetzt und kann hier nicht geändert werden.
  - ☑ Die Bestellposition wurde storniert und kann nicht mehr erzeugt werden.
  - ☐ Die Bestellposition ist nicht storniert und kann weiter bearbeitet werden.
  (Technische Info: Checkbox, DB-Feld: bestpool.still)
- **Lieferant**: Lieferantennummer für den Artikel. Standardmäßig wird die Nummer des Standardlieferanten für den Artikel aus den Stammdaten angezeigt. Wenn dem Artikel im Kundenauftrag ein abweichender Lieferant zugewiesen wurde, wird die Nummer dieses Lieferanten angezeigt.
  - Mit `<F10>` öffnen Sie die Marktpartnersuche zur Auswahl eines anderen Lieferanten.
  - Mit `<F5>` öffnen Sie den Dialog Adressen zur Auswahl einer anderen Adresse.
  - Mit `<Strg>+<O>` können Sie den neuen Lieferanten als Standardlieferanten für den gewählten Artikel in den Stammdaten hinterlegen.
  (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: bestpool.linr)
- **Menge**: Artikelmenge der bestellten Position. Bei Lagerbestellungen wird die Bestellmenge aus den Lager-Stammdaten herangezogen. Sie können die Bestellmenge ändern. (Technische Info: numerisches Feld, DB-Feld: bestpool.menge)
- **Bestellt zum**: Voraussichtlicher Liefertermin der Bestellung. Der Liefertermin wird aus den Stammdaten berechnet. Sie können das Datum ändern. (Technische Info: Datumsfeld, DB-Feld: bestpool.solldat)
- **Txt.**: Texte. Angabe, ob zu der Bestellposition Texte erfasst sind.
  - A: Für die Position sind Artikeltexte hinterlegt.
  - B: Für die Position sind Artikel- und Positionstexte hinterlegt.
  - P: Für die Position sind Positionstexte hinterlegt.
  Mit `<Shift> + <F4> > Auftragstexte darstellen` können Sie sich die hinterlegten Informationen anzeigen lassen. ⇨ "Auftragstexte" auf Seite E-96 (Technische Info: numerisches Feld, DB-Feld: bestpool.arttxtnr und bestpool.poskotxtnr)
- **Ei.**: Einkaufsinformation. Anzeige, ob für die Bestellposition eine Fremdinformation im Kundenauftrag hinterlegt ist. Wenn eine Einkaufsinformation hinterlegt ist, wird in dem Feld ein `/` angezeigt. Mit `<Shift> + <F4> > Einkaufsinfo` werden die hinterlegten Informationen angezeigt. (Technische Info: Anzeigefeld)
- **Re.**: Reklamation. Anzeige, ob die Bestellung wegen einer Kundenreklamation angelegt wurde.
  - ☑ Die Position wird wegen einer Kundenreklamation neu bestellt.
  - ☐ Die Position ist nicht Teil eines Reklamationsauftrags.
  (Technische Info: Checkbox)
- **An.**: Anfrage. Angabe, ob eine Anfrage an den Lieferanten erstellt wird. Wenn eine Lieferantenanfrage erstellt wird, wird in dem Feld ein `A` angezeigt. Über das Zusatzmenü können Sie angeben, für welche Bestellpositionen eine Lieferantenanfrage erstellt werden soll. (Technische Info: Anzeigefeld)
- **In.**: Infoanzeige. Das Feld wird zurzeit nicht genutzt. (Technische Info: Anzeigefeld)
- **NB**: Nachbestellung. Anzeige, ob eine zu Bruch gegangenen Position nachbestellt werden muss. (Technische Info: Anzeigefeld)

**Fußbereich**
- **Lieferant**: Name des Lieferanten der gewählten Position. (Technische Info: Anzeigefeld)
- **Gruppieren**: Gruppiert aus der markierten Bestellvorschlägen eine oder mehrere Bestellung/-en.
- **Auslösen**: Löst die jeweilige Funktion aus, d. h. die gruppierte Bestellvorschläge werden zu den Bestellungen umgewandelt und im System unter den vorgegeben Nummer gespeichert. Die Schaltfläche wird nur angezeigt, wenn die Gruppierung bereits erfolgte.

##### Bestellungen erzeugen – Position
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > Register Position**

*[Image: Bestellung erzeugen - Position (Abb. E-10)]*

In diesem Register werden die Positionsinformationen zu den zu bestellenden Artikeln angezeigt.

**Register Position**
Die Felder sind zum Dialog **Bestellung erzeugen** beschrieben: ⇨ "Bestellungen erzeugen – Lieferant" auf Seite E-37
Zusätzlich werden folgende Felder angezeigt:
- **Pos**: Positionsnummer bei Bestellpositionen aus Kundenaufträgen. (Technische Info: numerisches Feld, DB-Feld: bestpool.orglfdpos)
- **Lager**: Lagernummer für die Bestellung bei Lagerartikeln. Sie können die Lagernummer ändern. (Technische Info: numerisches Feld, DB-Feld: bestpool.Inr)
- **Breite, Höhe**: Maße der Position in Millimeter. Sie können die Maßangaben ändern. Wenn in der Bestellposition ein Variantenartikel erfasst ist, können Sie mit `<F9>` eine andere Maßvariante wählen oder den Variantenbezug entfernen und frei gewählte Maße angeben. (Technische Info: numerische Felder, DB-Felder: bestpool.laenge, bestpool.breite)
- **St**: Angabe, ob Artikel in der Bestellposition kein Positionsartikel, sondern eine Unterteil aus einer Stückliste ist. Wenn der Artikel ein Stücklistenunterteil ist, wird ein Stern `*` in dem Feld angezeigt. (Technische Info: numerisches Feld, DB-Feld: bestpool.orgIfdpos)

**Fußbereich**
Die Felder und Schaltflächen im Fußbereich sind zum Register **Bestellung erzeugen – Lieferant** beschrieben: ⇨ "Bestellungen erzeugen – Lieferant" auf Seite E-37

##### Bestellungen erzeugen – Details
**Einkauf > Bestellungen erzeugen > Abteilung angeben > <F3> > Register Details**

*[Image: Bestellungen erzeugen – Details (Abb. E-11)]*

In diesem Register werden die detaillierte Information zu den zu bestellenden Artikeln angezeigt. Sie können Positionsdaten beim Bedarf ergänzen.

**Register Details**
- **Haus**: Hausnummer, für welches die Bestellungen ausgelöst werden. (Technische Info: Anzeigefeld, DB-Feld: bestpool.hausnr)
- **Bestellung**: Bestellnummer und Positionsnummer in der Bestellung. (Technische Info: Anzeigefelder, DB-Felder: bestpool.baufnr, bestpool.orglfdpos)
- **Auftrag**: Auftragsnummer, Positionsnummer und Tupelnummer für die bestellte Auftrags-Unterteile, für die der Bestellvorschlag entsteht. (Technische Info: Anzeigefelder, DB-Felder: bestpool.orgauftrnr, bestpool.orglfdpos, bestpool.orgtnr)
- **Kunde**: Nummer und Name des Kunden bei Bestellpositionen aus Kundenaufträgen. (Technische Info: Anzeigefelder, DB-Felder: bestpool.kunr, mp.name)
- **Erfasser**: Name des Auftragserfasser bei Bestellpositionen aus Kundenaufträgen. (Technische Info: Anzeigefeld, DB-Feld: kauf.eusr)
- **Objekt**: Nummer und Bezeichnung des Objekts bei Bestellpositionen aus Kundenaufträgen. (Technische Info: Anzeigefelder, DB-Felder: bestpool.objnr, mp.name)
- **Einkaufsinfo**: Fremdinformation zum Einkauf bei Bestellpositionen aus Kundenaufträgen. Das Feld wird nur dann eingeblendet, wenn eine Einkaufinfo in dem Auftrag hinterlegt wurde. (Technische Info: Anzeigefelder, DB-Felder: kauf.exbez1)
- **(ohne Bezeichnung)**: Nummer für diverse Adresse, falls diese als Lieferadresse erfasst wurde. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bestpool.divadrnr)
- **Lager**: Nummer und Bezeichnung des Lagers bei Lagerartikeln. Sie können das Lager ändern. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bestpool.Inr)
- **Artikel**: Nummer und Bezeichnung des Artikels. (Technische Info: Pflichtfeld, numerisches Feld, Anzeigefeld, DB-Felder: bestpool.artnr, bestpool.artbez1)
- **Modell**: Modellnummer bei Bestellpositionen mit Scheibenmodell. (Technische Info: Anzeigefeld, DB-Feld: bestpool.modnr)
- **Lieferant**: Nummer und Name des Lieferanten. Sie können den Lieferanten ändern.
  - Mit `<F9>` können Sie den Lieferanten aus den Lieferanten wählen, die für den Artikel in den Stammdaten hinterlegt sind.
  - Mit `<F10>` öffnen Sie den Dialog Marktpartnersuche zur freien Auswahl eines anderen Lieferanten.
  - Mit `<Strg> + <O>` hinterlegen Sie den gewählten Marktpartner als Standardlieferant für den aktuellen Artikel in die Stammdaten.
  - Mit `<F5>` können Sie die Lieferadresse ändern. Standardmäßig ist die Hauptlieferadresse des Lieferanten gewählt. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bestpool.linr, mp.name)
- **Fax.**: Faxnummer des Lieferanten aus den Stammdaten. (Technische Info: Anzeigefeld, DB-Feld: bestpool.faxnr)
- **Bestellnr.**: Lieferantenseitige Nummer und Bezeichnung des Artikels, wenn für den Artikel in den Stammdaten eine lieferantenspezifische Artikelnummer hinterlegt ist. (Technische Info: alphanumerisches Feld, Anzeigefeld, DB-Felder: bestpool.exartnr, bestpool.exartbez)
- **Menge**: Bestellmenge der bestellten Position in den im Stammdaten hinterlegten Mengeneinheit des Artikels. Sie können die Bestellmenge ändern. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: bestpool.menge)
- **ME**: Mengeneinheit. Bei Längen-, Zeit- und Stückartikeln wird in diesem Feld die jeweilige Maßeinheit angezeigt, z. B. Meter, Liter. (Technische Info: Anzeigefeld, DB-Feld: bestpool.me)
- **Breite, Höhe**: Maße der Position in den im Stammdaten hinterlegten Mengeneinheit des Artikels. Sie können die Maßangaben ändern. (Technische Info: numerische Felder, DB-Felder: bestpool.laenge, bestpool.breite)
- **SZR**: Breite des Scheibenzwischenraums in entsprechenden Maßeinheiten. Sie können den Scheibenzwischenraum ändern. Der Scheibenzwischenraum wird nur angezeigt, wenn in der Bestellposition ein ISO-Artikel erfasst ist. (Technische Info: numerisches Feld, DB-Feld: bestpool.szr)
- **Variante**: Variantenummer und Variantenbezeichnung des Artikels. Sie können die Variante ändern. Wenn Sie eine andere Maßvariante wählen, werden die Felder **Breite** und **Höhe** automatisch angepasst. (Technische Info: alphanumerisches Feld, numerisches Feld, DB-Felder: bestpool.bitnr, bestpool.varart)
- **Kundenanfahrt**: Auslieferungstermin an den Kunden. (Technische Info: Anzeigefeld, DB-Feld: bestpool.liefdat)
- **Bestellt zum**: Voraussichtlicher Liefertermin der Bestellung. Der Liefertermin wird aus den Stammdaten berechnet. Sie können das Datum ändern. (Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: bestpool.solldat)
- **Bestellt am**: Datum der Bestellerfassung. (Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: bestpool.bestdat)
- **Eigenwähr.**: Stückpreis und Positionspreis in Eigenwährung, z. B. Euro. (Technische Info: Anzeigefelder, DB-Felder: bestpool.nstpreis, bestpool.npospreis)
- **Fremdwähr.**: Stückpreis und Positionspreis in Fremdwährung, z. B. Dollar. (Technische Info: Anzeigefelder, DB-Felder: bestpool.fnstpreis, bestpool.fnstpreis)
- **Währung, Kurs**: Nummer und Name der Währung und Währungskurs, z. B. Kurs bei Umrechnung von Euro in Dollar. (Technische Info: Anzeigefelder, DB-Felder: bestpool.waehrung, waehrung.kurzbez, bestpool.kurs)
- **Kostenstelle**: Bezeichnung der Kostenstelle für statistische Auswertungen bei Bestellpositionen aus Kundenaufträgen. (Technische Info: Anzeigefeld, DB-Feld: bestpool.kostenst)
- **Lieferart**: Gewünschte Art der Lieferung:
  - Abholung: Der Kunde holt die Ware selbst ab.
  - Streckengeschäft: Die Ware wird vom beauftragten Produktionsbetrieb direkt an den Endkunden ausgeliefert.
  - keine Auswahl: Die Ware wird über die Route geliefert, die in dem Kundenauftrag erfasst ist. (Technische Info: Toggle-Feld, DB-Feld: bestpool.geschart)
- **Bruchort**: Nummer und Bezeichnung des Bruchortes, an dem der Glasbruch entstanden ist. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bestpool.bruchort)
- **Bruchgrund**: Nummer und Bezeichnung des Bruchgrundes. Die Nummer muss nur angegeben werden, wenn eine Position wegen Glasbruchs neu bestellt werden muss. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bestpool.bruch)
- **Summen**: Summe des Positionswerts für Gewicht in Kilogramm, Fläche in Quadratmeter und Länge in Laufmeter. (Technische Info: Anzeigefelder)
- **Position**: Die Anzeige Position gibt an, dass angezeigte Summen pro Position gelten. (Technische Info: Anzeigefeld)

**Fußbereich**
Die Schaltflächen im Fußbereich sind zum Register **Bestellung erzeugen – Lieferant** beschrieben: ⇨ "Bestellungen erzeugen - Lieferant" auf Seite E-37

### Vorgangsverwaltung

Zu den Vorgängen, die Sie im Bereich **Einkauf** bearbeiten, gehören Lieferanten-Anfragen, Bestellungen, Wareneingänge, Lieferanten-Rechnungen und Gutschriften. Die Dialogen sind vorwiegend gleich zum Bereich **Verkauf** aufgebaut und benutzbar.

Zu der Vorgangsverwaltung gehören folgende Kapiteln:
- "Symbolerklärung" auf Seite E-47
- "Lieferanten-Anfragen" auf Seite E-50
- "Bestellerfassung" auf Seite E-50
- "Bestellungen erzeugen" auf Seite E-37
- "Wareneingang (manuell)" auf Seite E-119
- "Lieferanten-Rechnung (manuell)" auf Seite E-138
- "Lieferanten-Gutschrift" auf Seite E-142

#### Symbolerklärung

In diesem Abschnitt werden die Kennzeichen für den Dialogmodus, den Positionsstatus und das Positionskennzeichen beschrieben.

##### Dialogmodus
Der Dialogmodus wird in der Titelzeile des Dialogs angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| `+` | Dialog mit Kreuzchen | In diesem Modus können Sie neue Datensätze anlegen. |
| 📝 | Dialog mit Stift | In diesem Modus können Sie einen Vorgang bearbeiten. |
| ⚠️ | Gelbes Dreieck mit Ausrufezeichen | In diesem Modus können Sie den Vorgang nicht bearbeiten. |
| 🔍 | Suche | In diesem Modus können Sie nach Vorgängen suchen. |

##### Positionsstatus und Positionszeichen
Der Positionsstatus wird im Register **Positionen** vor der Spalte **Pos** angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| 🟢 (grün) | Die Position kann frei geändert werden, da die Bestellung noch nicht freigegeben ist. |
| 🟡 (gelb) | Die Position oder Unterteile der Position sind bestellt und die Bestellung ist gedruckt worden. |
| 🔴 (rot) | Die Position ist in der Bestellung freigegeben. Sie kann nicht mehr geändert werden. |
| 🔴/🔴🔵 (rot/rotblau) | Die Position ist teilweise geliefert. |
| 🔴🔵 (rot/blau) | Die Position ist komplett geliefert. |
| 🔴🔵/🔵 (rotblau/blau) | Die Position ist teilfakturiert. |
| 🔵 (blau) | Die Position ist komplett fakturiert. |

Das Positionskennzeichen wird vor der Spalte Pos angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| ⭐ (Gelber Stern) | Die Produktbemaßung sowie zusätzliche Bearbeitungen des Artikels sind für den ausgewählten Lieferanten hinterlegt. Nach dem Speichern des lieferantenindividuellen Artikels wird ein grüner Stern angezeigt. ⇨ Verkauf, Help Cards, "Artikel fixieren" auf Seite D-29 |
| ⭐ (Grüner Stern) | Der Artikel ist lieferantenindividuell definiert und kann nur für den jeweiligen Lieferanten erfasst werden. In einem lieferantenindividuellen Artikel können Sie den Stücklistenaufbau mit zusätzlichen Bearbeitungen, Artikeln, Maßänderungen und weiteren lieferantenspezifischen Wünschen speichern. ⇨ Verkauf, "Artikelangaben für bemaßte Varianten" auf Seite D-159 |
| 🔳 (Scheibenmodell) | Die Position ist mit Modell erfasst. ⇨ Verkauf, "Modell-Maßangaben" auf Seite D-175 |
| 🪟 (Fenster mit Sprossen) | Die Position ist mit Sprossen erfasst. ⇨ Verkauf, "Sprossenerfassung" auf Seite D-224 |

##### Statusanzeige in Textform
Der Status in Textform wird in der Dialogzeile oder im Register **Allgemein** über der Spalte **B.Art** angezeigt, wenn sich der Positionsstatus ändert.

| Status in Textform | Bedeutung |
| :--- | :--- |
| **Lagerabgang** | Für die Position wurde ein Lagerabgang gebucht. |
| **Teil-Bestellt** | Für die Position existiert eine Teilbestellung, z. B. für einen Artikel aus der Stückliste. |
| **Storno** | Die Bestellung ist storniert. |
| **Fakturiert** | Die Bestellung ist fakturiert und kann nicht geändert werden. Rechts neben der Anzeige Fakturiert steht die Nummer der Lieferantenrechnung. |
| **Versandplanung liegt vor** | Die Bestellung ist im Versand verplant. Kaufmännische Änderungen, wie z. B. Preisänderungen, sind unter Umständen noch möglich. |
| **Globalkorrektur** | Änderung in der Bestellung werden nicht mehr an die Datenbank übergeben. Kaufmännische Änderungen, wie z. B. Preisänderungen, sind unter Umständen noch möglich. |
| **Lokalkorrektur** | Änderungen in der Position werden in der Bestellerfassung nicht mehr an das System übergeben, soweit sie die Bestellung betreffen, z. B. Maßänderungen. Kaufmännische Änderungen, wie z. B. Preisänderungen, sind unter Umständen noch möglich. |

#### Lieferanten-Anfragen
**Einkauf > Anfragen**

*[Image: Lieferanten-Anfragen (Abb. E-12)]*

In diesem Dialog erstellen und bearbeiten Sie Anfragen an Lieferanten. Wenn Sie in der Anfrage einen Liefertermin eintragen, können Sie einen Wiedervorlage-Termin anlegen, um die Anfrage nachzuverfolgen. Wenn der Wiedervorlage-Termin erreicht ist, wird beim Programmstart eine Meldung angezeigt.
Die Wiedervorlage ist ausführlich im Part Verkauf beschrieben: ⇨ Verkauf, "Wiedervorlage" auf Seite D-398

Jede Anfrage kann in eine Bestellung umgewandelt werden. Der Dialog ist wie der Dialog **Bestellerfassung** aufgebaut. Abweichungen werden explizit zum Dialog **Bestellerfassung** beschrieben: ⇨ "Bestellerfassung" auf Seite E-50

#### Bestellerfassung
**Einkauf > Bestellverwaltung**

In diesem Dialog erfassen und bearbeiten Sie Bestellungen. Für die reguläre Erzeugung von Bestellungen verwenden Sie in der Regel den Dialog **Bestellungen erzeugen**. Anschließend können Sie im Dialog **Bestellverwaltung** die erzeugte Bestellungen ansehen ggf. ändern. ⇨ "Bestellungen erzeugen" auf Seite E-37

In diesem Dialog finden Sie im Kopfbereich folgende Register:
- "Bestellerfassung – Kopf, Fuß" auf Seite E-51
- "Bestellerfassung - Anschriften" auf Seite E-57
- "Bestellerfassung - Eigenschaften" auf Seite E-59
- "Bestellerfassung – Verschiedenes" auf Seite E-64

Im Register **Positionen** finden Sie folgende Register:
- "Bestellpositionen - Allgemein" auf Seite E-71
- "Bestellpositionen - Eigenschaften" auf Seite E-80
- "Bestellpositionen - Preise" auf Seite E-83
- "Bestellpositionen – AuftragsInfo” auf Seite E-87
- "Bestellpositionen – Status" auf Seite E-88
- "Bestellpositionen – Bewertung" auf Seite E-91

##### Bestellerfassung – Kopf, Fuß
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen**

*[Image: Bestellerfassung - Register Positionen (Abb. E-13)]*

In diesem Dialog geben Sie die Lieferantendaten an und erfassen die Bestellpositionen. Wenn Sie Positionen erfassen, genügt es in der Regel, die Daten im Register **Allgemein** zu erfassen.

- Mit `<Enter>` wechseln Sie in das nächste Feld, mit `<Bild hoch>` wechseln Sie zur ersten Position, mit `<Bild runter>` zur letzten Position.
- Mit `<Ende>` wechseln Sie in den Fußbereich und schließen die Bestellverwaltung ab.
- Mit `<F2>` wechseln Sie aus dem Feld **Objekt** in die Register **Anschriften**, **Eigenschaften** oder **Verschiedenes**.

**Kopfbereich**
- Mit `<Strg> + <F12>` wechseln Sie aus den Feldern **Eingang**, **Rechnungstyp** oder **Objekt** in den Dialog **Bestellart**. ⇨ "Bestellarten" auf Seite E-94
- Mit `<F2>` wechseln Sie aus den Felder **Eingang**, **Rechnungstyp** oder **Objekt** in den Positionsbereich.

> **Bestellungen auflisten**
> Wenn Sie den Dialog Bestellerfassung öffnen, können Sie mit `<F5>` ins Feld **K-Auftrag** wechseln und durch die Auftragsnummer-Eingabe nach dazugehörigen Bestellungen suchen. Alternativ können Sie mithilfe `<F9>` alle vorhandene Bestellungen auflisten und anschließend auswählen.

- **Bestell.**: Bestellnummer. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr (kauf.vorgang=2))
- **Lieferant**: Lieferantennummer. Wenn Sie eine Nummer angeben, werden Name und Ort des Lieferanten im Klartext angezeigt. (Technische Info: Pflichtfeld, numerisches Feld, Anzeigefelder, DB-Feld: kauf.kunr, kauf.orgname)
- **Grund**: Begründung für eine Terminänderung. Das Feld **Grund** wird nur angezeigt, wenn Sie den Liefertermin in einer früher erfassten Bestellung ändern. (Technische Info: alphanumerisches Feld, DB-Feld: kaufltedit.text)
- **Bezug**: Vorgangsnummer, auf die Bezug genommen wird.
  - **Vorgangsart für den Bezug vorauswählen**: Je nach Systemkonfiguration ist es möglich, eine der Vorgangsarten als Vorauswahl für die Bezugserfassung festzulegen. Mit `<F9>` öffnen Sie einen Auswahldialog mit allen Vorgangsarten.
- **Vorgang mit Bezug erfassen**:
  - Mit `<F9>` öffnen Sie den Dialog **Suche Bezugsvorgang**, um einen Bezugsvorgang zu den angegebenen Kriterien auszuwählen. ⇨ Verkauf, "Suche Bezugsvorgang" auf Seite D-43 (Technische Info: numerisches Feld, DB-Feld: kauf.referenz)
  > **Bezugnahme auf Auftrag**
  > Wenn Sie in der Bestellung Bezug auf einen Auftrag nehmen, dann werden alle Auftragspositionen in die Bestellerfassung geladen. Gegebenenfalls müssen Positionen im Register **Allgemein** gelöscht oder angepasst werden.
- **Haus**: Hausnummer, in dem die Bestellung erfasst wird. (Technische Info: numerische Felder, DB-Felder: kauf.company, kauf.hausnr)
- **Erf. Datum**: Erfassungsdatum. Standardmäßig ist das Feld mit dem aktuellen Datum vorbelegt. (Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat)
- **K-Auftrag**: Kunden-Auftragsnummer aus dem Verkauf bei auftragsbezogenen Bestellungen. Je nach Konfiguration können alternative Daten angezeigt werden (Knd-Bestnr., Lagerbestellung, Externes Nummernsystem). (Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr)
- **Termin**: Gewünschter Liefertermin der Bestellung. Im ersten Feld können Sie die Kalenderwoche eingeben. Im zweiten Feld können Sie das Datum im Format TT.MM.JJJJ eingeben. (Technische Info: Pflichtfeld, numerisches Feld, Datumsfeld, DB-Felder: kauf.kwideal, kauf.Itideal)
- **Route**: Routennummer. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.routenr)
- **Anlief. Datum**: Anzeige des geplanten Anlieferdatums. (Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan)
- **Lief-Pos**: Angabe zu Lieferantenpositionen in der Bestellung (ja/nein). (Technische Info: Toggle-Feld, DB-Feld: kauf.kndposkz)
- **Term. Art**: Information über die Terminierungsart, die auf den Auftrag gedruckt wird (Abruf, eilt, mögl, verbl, ohne, Auto, folgt). (Technische Info: Toggle-Feld, DB-Feld: kauf.abrufkz)
- **Eingang**: Wird nicht verwendet. (Technische Info: Toggle-Feld, DB-Feld: kauf.eingang)
- **Rechnungstyp**: Angabe, für welche Leistungen die Rechnung erstellt wird (Gesamt, Glas, Dienstltg). (Technische Info: Toggle-Feld, DB-Feld: kauf.rechart)
- **Objekt**: Objektnummer. Ein Objekt ist dem Marktpartner zugeordnet. Mit `<F9>` öffnen Sie die Objekt-Suche. ⇨ Verkauf, "Objekt-Suche" auf Seite D-64 (Technische Info: numerisches Feld, DB-Feld: kauf.objnr)

**Positionsbereich**
In diesem Bereich werden Informationen zur markierten Position oder Spalte angezeigt. ⇨ "Bestellpositionen" auf Seite E-70

**Fußbereich**
- **Sender**: Anzeige der Haus- und der Referenznummer. (Technische Info: Anzeigefelder, DB-Felder: kauf.hausnr)
- **ST, kg, qm**: Anzeige der Gesamtsumme der Bestellwerte für Anzahl in Stück, Gewicht in Kilogramm und Fläche in Quadratmeter. (Technische Info: Anzeigefelder, DB-Felder: kauf.gesst, kauf.gesm2, kauf.gesgewicht)
- **Gesamt**: Anzeige des Gesamtpreises aller Positionen abzüglich der Positionsrabatte. ⇨ "Bestellpositionen – Preise" auf Seite E-83 (Technische Info: Anzeigefeld, DB-Feld: kauf.gesnetto)
- **Rabatt**: Auf den Gesamtbetrag gewährter Rabatt in Prozent. (Technische Info: numerisches Feld, DB-Feld: kauf.gesfaktor)
- **Nettototal**: Summe aller Positionspreise, inkl. Rabatte und Zuschläge. ⇨ "Bestellerfassung - Summen" auf Seite E-68 (Technische Info: numerisches Feld, DB-Feld: kauf.nettototal)
- **+MwSt ()**: Anzeige der Mehrwertsteuer. (Technische Info: Anzeigefeld, DB-Feld: kauf.mwstbetrag)
- **Brutto**: Anzeige des Brutto-Gesamtbetrags. (Technische Info: Anzeigefeld, DB-Feld: kauf.gesbrutto)
- **D-Beitrag**: Anzeige des Deckungsbeitrags (Bruttogewinn). (Technische Info: Anzeigefeld, DB-Feld: kauf.dbdm)

##### Bestellerfassung – Anschriften
**Einkauf > Bestellverwaltung > Bestellung öffnen > Feld Eingang, Rechnungstyp > <F2> > Register Anschriften**

*[Image: Bestellerfassung – Anschriften (Abb. E-14)]*

In diesem Register bearbeiten Sie die Lieferanten- und Lieferanschrift. Standardmäßig wird im Bereich **Lieferanschrift** die Lieferanschrift aus den Lieferantenstammdaten herangezogen.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Lieferantenanschrift**
- **Name, Vorname**: Name und Vorname des Lieferanten. (Technische Info: alphanumerische Felder, DB-Felder: kauf.orgname, kauf.orgvorname)
- **Anrede**: Nummer der Anrede. (Technische Info: numerisches Feld, DB-Feld: kauf.organrede)
- **Z. Hd.**: Name der Person, an die die Bestellung ausgehändigt werden soll. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgzhd)
- **Zusatz**: Zusatztext der Anschrift. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgbranche)
- **Straße**: Straßenname und Hausnummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgstr)
- **PLZ, Fach**: Postleitzahl und Nummer des Postfachs. (Technische Info: alphanumerische Felder, DB-Felder: kauf.orgpfplz, kauf.orgpostfach)
- **PF Ort**: Ortsname des Postfachs von Lieferanten außerhalb Europas. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgpfort)
- **PLZ, Ort**: Postleitzahl und Ortsname der Lieferantenanschrift. (Technische Info: alphanumerische Felder, DB-Felder: kauf.orgplz, kauf.orgort)
- **KFZ Land**: Kraftfahrzeug-Kennzeichen des Ziel-Landes. (Technische Info: alphanumerische Felder, DB-Felder: kauf.orgkfzcode, kauf.orgland)
- **Tel**: Telefonnummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgtel)
- **Fax**: Faxnummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.faxnr)
- **Sprache**: Nummer der Landessprache des Lieferanten. (Technische Info: numerisches Feld, DB-Feld: kauf.sprkz)
- **Kennz.**: Nummer des Steuerkennzeichens. (Technische Info: numerisches Feld, DB-Feld: kauf.kukz)

**Lieferanschrift**
Sie können eine abweichende Lieferanschrift eingeben, z. B. bei einer Direktanlieferung die Adresse einer Baustelle.
- Mit `<Strg> + <N>` legen Sie eine neue Lieferanschrift für den Lieferanten an.
- Mit `<Strg> + <L>` wählen Sie eine hinterlegte Lieferanschrift des Lieferanten aus.
- **Region**: Versandregion. (Technische Info: Anzeigefeld)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

##### Bestellerfassung – Eigenschaften
**Einkauf > Bestellverwaltung > Bestellung öffnen > ab dem Feld Eingang> <F2> > Register Eigenschaften**

*[Image: Bestellerfassung – Eigenschaften (Abb. E-15)]*

In diesem Register bearbeiten Sie die Angaben zur Mitarbeiterzuordnung, den Versandinformationen und den Rechnungs- und Druckoptionen.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Mitarbeiterzuordnung**
- **Bestellt bei**: Mitarbeiternummer des Lieferanten. Mit `<F5>` öffnen Sie den Dialog **Ansprechpartner**. ⇨ Verkauf, "Ansprechpartner" auf Seite D-142 (Technische Info: numerisches Feld, DB-Feld: kauf.busr)
- **Bestelldatum**: Datum der Bestellerfassung. (Technische Info: Datumsfeld, DB-Feld: kauf.bdat)
- **Erfasser**: Anzeige der Nummer und des Namens des Erfassers. (Technische Info: Anzeigefelder, DB-Feld: kauf.esuer)
- **Sachbearbeiter**: Nummer des Sachbearbeiters. (Technische Info: numerisches Feld, DB-Feld: kauf.abvertr)
- **Außendienst**: Name des Außendienst-Mitarbeiters. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.vertr)
- **Vertr. (Erlös)**: Vertreter-Erlös. Nummer des Vertreters, an den die Provision ausgezahlt wird. (Technische Info: numerisches Feld, DB-Feld: kauf.vertrerloe)

**Versandinformationen**
- **Max. Abladung**: Maximales Gewicht, das der Lieferant mit seinem technischen Gerät abladen kann. (Technische Info: numerisches Feld, DB-Feld: kauf.gmaxgew)
- **Zustellung**: Vermerk über die gewünschte Art der Zustellung (Abholung, Streckengeschäft, keine Auswahl). (Technische Info: Toggle-Feld, DB-Feld: kauf.geschart)
- **Direktauslief.**: Angabe, ob der Lieferant direkt von den Produktionsstätten beliefert wird. Das Kennzeichen wird im Bereich Einkauf nicht verwendet. (Technische Info: Toggle-Feld, DB-Feld: kauf.drkliefkz)
- **Lieferart**: Nummer der Lieferart, z. B. frei Haus. (Technische Info: numerisches Feld, DB-Feld: kauf.lieferart)
- **Versandart**: Nummer der Versandart, z. B. LKW. (Technische Info: numerisches Feld, DB-Feld: kauf.versandart)
- **Verpackungsart**: Nummer der Verpackungsart, z. B. Kiste. (Technische Info: numerisches Feld, DB-Feld: kauf.verpackart)
- **Gest.-Beladung**: Gestell-Beladung. Sie wählen aus, nach welchen Kriterien die Ware auf den Gestellen sortiert wird. (Technische Info: Toggle-Feld, DB-Feld: kauf.gbelad)
- **Ausgangszoll**: Nummer der Ausgangszollstelle für die Lieferpapiere. (Technische Info: numerisches Feld, DB-Feld: kauf.azsnr)
- **Bestimmungszoll**: Nummer der Zollstelle des Empfängerlandes. (Technische Info: numerisches Feld, DB-Feld: kauf.bzsnr)
- **Fahrtdauer, Entfernung**: Voraussichtliche Fahrzeit und Anzeige der Fahrstrecke. (Technische Info: numerische Felder, DB-Felder: kauf.anfahrt)

**Rechnungs- und Druckoptionen**
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.steuernr)
- **FA-Steuer-Nr.**: Finanzamt-Steuer-Nummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.finstnr)
- **Kostenstelle**: Bezeichnung der Kostenstelle für statistische Auswertungen.
  > **Festlegen der Kostenstelle für die gesamte Bestellung**
  > Wenn Sie eine Kostenstelle angeben, werden bestellbezogen die positionsgenauen Kostenstellen aus den Stammdaten überschrieben.
- **Rechnungsart**: Art der Rechnung (Einzelrechnung, Sammelrechnung). (Technische Info: Toggle-Feld, DB-Feld: kauf.rechungsart)
- **Teilfaktura**: Angabe, ob Teilabrechnungen nach einer Teillieferung erstellt werden (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.teilfakkz)
- **Eilbestellung**: Die aktuelle Bestellung kann bevorzugt und mit höherer Priorität freigegeben werden (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.schnell)
- **Bruttopreise drucken**: Die Bruttopreise können auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.preisdrkz)
- **Kundenfaktor drucken**: Der kundenspezifische Faktor kann auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.rabdrkz)
- **Artikeltexte drucken**: Die Artikeltexte können auf den marktpartnerseitigen Dokumenten gedruckt werden (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.atxtdrukz)
- **Modelle drucken**: Die Modellskizze der Positionen kann im Anhang der marktpartnerseitigen Dokumente gedruckt werden (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.moddrkz)
- **Positionspreise unterdrücken**: Die Positionspreise werden standardmäßig auf den marktpartnerseitigen Dokumenten gedruckt (J/N). (Technische Info: Toggle-Feld, DB-Feld: kauf.posdrkz)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung – Kopf, Fuß" auf Seite E-51

##### Bestellerfassung – Verschiedenes
**Einkauf > Bestellverwaltung > Bestellung öffnen > ab dem Feld Eingang> <F2> > Register Verschiedenes**

*[Image: Bestellerfassung - Register Verschiedenes (Abb. E-16)]*

In diesem Register werden Reklamationsinformationen, private Felder, weitere technische Informationen und die Zahlungsoptionen angezeigt.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Reklamationsinformation**
- **Art**: Nummer der Reklamationsart. (Technische Info: numerisches Feld, DB-Feld: kauf.reklamart)
- **Ort**: Nummer des Reklamationsorts. (Technische Info: numerisches Feld, DB-Feld: kauf.reklamort)
- **Typ**: Nummer des Reklamationstyps. (Technische Info: numerisches Feld, DB-Feld: kauf.reklamspec)
- **Datum**: Reklamationsdatum im Format TT.MM.JJJJ. (Technische Info: Datumsfeld, DB-Feld: kauf.reklamdat)

**Zahlungsoptionen**
- **Währung, Kurs**: Nummer und Name der Währung und Währungskurs. (Technische Info: Pflichtfeld, numerische Felder, DB-Felder: kauf.waehrung, kauf.kurs)
- **Kalkulation in**: Legt fest, ob Preise in Eigenwährung oder Fremdwährung berechnet werden. (Technische Info: Toggle-Feld, DB-Feld: kauf.waehrprs)
- **Ausdruck in**: Nummer für den Ausdruck in der kalkulierten Währung oder der Fremdwährung.
  > Die Felder **Kalkulation in** und **Ausdruck in** sind nur zugänglich, wenn das Währungs-Modul lizenziert ist.
- **Zahlziel**: Zahlungsziel in Tagen. (Technische Info: numerisches Feld, DB-Feld: kauf.zahlziel)
- **Valuta**: Frist zur Wertstellung in Tagen. (Technische Info: numerisches Feld, DB-Feld: kauf.valuta)
- **Skonto1, Skonto2, Skonto3**: Schlüssel der Skontosätze für das Zahlungsziel. (Technische Info: numerische Felder, DB-Felder: kauf.skonto1, kauf.skonto2, kauf.skonto3)
- **Merkmal**: Nummer der Form der Bezahlung, z. B. Banklastschrift. (Technische Info: numerisches Feld, DB-Feld: kauf.zahlngmerk)
- **Zahlungsverkehr**: Art und Weise der Bezahlung, z. B. Vorauskasse. (Technische Info: Toggle-Feld, DB-Feld: kauf.skontoart)
- **FIBU-Key**: Schlüssel zur Übergabe an die Finanzbuchhaltung. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.fibukey)
- **FIBU-Debitor**: Lleferantennummer des Marktpartners, der als Rechnungsempfänger bestimmt ist. (Technische Info: numerisches Feld, DB-Feld: kauf.stddebnr)

**Private Felder**
Die privaten Felder werden kundenspezifisch für Zusatzinformationen genutzt. Sie sind frei konfigurierbar. (Technische Info: numerische Felder, alphanumerische Felder, DB-Felder: kauf.private_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2)

**Weitere Optionen**
- **Kontrolle**: Nummer des Mitarbeiters, der den Vorgang kontrolliert. (Technische Info: numerisches Feld, DB-Feld: kauf.kontrollmanr)
- **Windlast**: Windlast am Einbauort (N/m²).
  > **Restriktionsprüfung bei Eingabe der Windlast**
  > Wenn für die Windlast ein entsprechender Eintrag in den Stammdaten angelegt ist, wird die angegebene Windlast einer Restriktionsprüfung unterzogen.
- **Fassadenzone**: Angabe der Fassadenzone, in der die Scheiben verbaut werden (1 Rand, 2 Zentral). (Technische Info: numerisches Feld, DB-Feld: kauf.bereich)
- **Min ISO Ges-Stärke, Max ISO Ges-Stärke**: Minimale und maximale Glasstärke des gesamten ISO-Artikels in Millimeter. (Technische Info: numerische Felder, DB-Felder: kauf.minszr, kauf.maxszr)
- **Falzmaß**: Korrekturmaß in Millimeter. (Technische Info: numerisches Feld, DB-Feld: kauf.falzmass)
- **Angeb. Status**: Status des Angebots (offen, gewonnen, verloren, verjährt). (Technische Info: Toggle-Feld, DB-Feld: kauf.angbstatus)
- **Textformeln**: Nummer und Bezeichnung der Produktkennzeichnung. (Technische Info: numerisches Feld, DB-Feld: kauf.artkennfrm)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

##### Bestellerfassung – Summen
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein > Preisfeld> <Ende> > Feld Nettototal > <F2>**

*[Image: Bestellerfassung (Summen) (Abb. E-17)]*

In diesem Dialog definieren Sie Rabatte, Ab- und Aufschläge für die gesamte Bestellung und bearbeiten verschiedene Zahlungsoptionen. Rabatte werden mit den Lieferanten vereinbart.
Der Dialog ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Auftragserfassung - Summen" auf Seite D-102

##### Bestellerfassung – Detailansicht Rabatte
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein > Preisfeld > <Ende> > Feld Nettototal > <F2> > <F5> > <F5>**

*[Image: Detailansicht Rabatte (Abb. E-18)]*

In diesem Dialog geben Sie Details zum ausgewählten Rabatt an.
Der Dialog ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Auftragserfassung - Detailansicht Rabatte" auf Seite D-106

### Bestellpositionen
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein**

Im Register **Positionen** finden Sie folgende Register:
- "Bestellpositionen - Allgemein" auf Seite E-71
- "Bestellpositionen - Eigenschaften" auf Seite E-80
- "Bestellpositionen – Preise" auf Seite E-83
- "Bestellpositionen – AuftragsInfo” auf Seite E-87
- "Bestellpositionen - Status" auf Seite E-88
- "Bestellpositionen – Bewertung" auf Seite E-91

Auf der Positionsebene können Sie Modelle, Bearbeitungen, Stufungen und Sprossen neuerfassen bzw. diese Information in den erzeugten Bestellungen ansehen und ändern. Sie können auch die Einkaufspreise zu den Positionen einsehen und anpassen.
Die Dialoge sind ausführlich zum Part Verkauf beschrieben.
- ⇨ Verkauf, "Sprossenerfassung" auf Seite D-224
- ⇨ Verkauf, "Stufenerfassung (relevante Teile)" auf Seite D-221
- ⇨ Verkauf, "Stücklistendarstellung" auf Seite D-193
- ⇨ Verkauf, "Modell-Maßangaben" auf Seite D-175
- ⇨ Verkauf, "Preise und Konditionen" auf Seite D-261

#### Bestellpositionen – Allgemein
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein**

*[Image: Bestellpositionen – Allgemein (Abb. E-19)]*

In diesem Register erfassen und bearbeiten Sie die Positionen einer Bestellung. Sie können die Artikel auswählen, die Maße, Menge und Beschaffungsart bestimmen und den Artikeln Bearbeitungen zuordnen.

Bei einer Statusänderung wird auf der Höhe des Registers ein entsprechender Hinweis zum Status der Bestellung angezeigt. Vor dem Feld **Pos** werden der Positionsstatus als Ampel und ggf. das Positionskennzeichen angezeigt. ⇨ "Symbolerklärung" auf Seite E-47

Auftragsbezogene Bestellungen und Lagerbestellungen werden in der Regel über den Dialog **Bestellungen erzeugen** angelegt und können in der Bestellverwaltung beim Bedarf bearbeitet werden. ⇨ "Bestellungen erzeugen" auf Seite E-37

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Register Positionen (linker Bereich)**
Im Infobereich werden verschiedene Informationen zur markierten Position angezeigt.
⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" auf Seite E-74

*[Image: Register Positionen (Infobereich links) (Abb. E-20)]*

- **Kommis**: Kommissionstext für den Druck. Das Feld ist nur betretbar, wenn für den Artikel in den Stammdaten entsprechendes Flag gesetzt ist.
  - Mit `<F4> > Kommissionen > neue Kommission` oder `Kommission ändern` legen Sie über das Zusatzmenü einen neuen Kommissionstext an.
  - Mit `<Shift> + <F11>` wechseln Sie aus der Positionsebene in die Texterfassung der Kommission.
  > **Kommissionstext vererben**
  > Wenn Sie einer Position mit `<Shift> + <F11>` einen Kommissionstext zuordnen, kann der Kommissionstext für alle folgenden Positionen übernommen werden.
- **LE**: Leistungserklärung. Bezeichnung der Leistungserklärung, die dem Artikel zugeordnet ist. (Technische Info: Anzeigefeld, DB-Feld: kposp.lbrefnr)
- **(CAD-Kennzeichen)**: Kennzeichen, ob der Position eine CAD-Datei zugeordnet ist.
- **(Kostenstelle)**: Bezeichnung der Kostenstelle, die der Position zugeordnet ist.
- **(Sprossenkennzeichen)**: Kennzeichen, ob in der Position Sprossen erfasst sind (S, E).
- **(Kopfartikel, Artikel)**: Bezeichnung des Kopfartikels. Bei Mehrfachgläsern werden neben dem Kopfartikel die Bezeichnungen der einzelnen Gläser angezeigt.
- **(Austausch-, Zusatzartikel, Anzahl1/Anzahl2)**: Bezeichnung der Austausch- und Zusatzartikel und Anzahl der Artikel in der Stückliste.
- **(Sprossenaustausch-, Sprossenzusatzartikel, Anzahl1/Anzahl2)**: Bezeichnung der Sprossenaustausch- und/oder Sprossenzusatzartikel und Anzahl der Sprossen in der Stückliste.

**Register Positionen (Info-Bereich – Grafik, Technische Werte)**
Im rechten Bereich im Register **Positionen** werden, abhängig von der Systemkonfiguration und den Einstellungen, eine der folgenden Informationen angezeigt:
- Beschaffung, Warengruppe und Modell
- Technische Werte
- Verdeckte Maßangaben

*[Image: Register Positionen (Infobereich rechts) (Abb. E-21)]*

- **Kunde**: Kundenname. (Technische Info: Anzeigefeld, DB-Feld: mp.name, kauf.kunr)
- **Warengrp**: Warengruppennummer der Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.wgrp)
- **Modell**: Modellnummer. Mit `<F9>` öffnen Sie eine Auswahl an Modellbezeichnungen. (Technische Info: Anzeigefeld, DB-Feld: kpos.modnr)

**Technische Werte**
Mit `<F4> > Produktangaben > Technische Werte` können Sie im Zusatzmenü einen der folgenden Einträge auswählen:
- **Technische Werte anzeigen**: Zeigt die technischen Werte der gewählten Position an.
- **Technische Werte ändern**: Wechselt in die Eingabefelder für die technischen Werte.

- **Position**: Positionsnummer der gewählten Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.posnr)
- **Artikelcode**: Artikelnummer der gewählten Position. (Technische Info: Anzeigefeld, DB-Feld: ktechw.artnrgen)
- **Ges-Stärke**: Glasstärke für den gesamten Artikel der Position. (Technische Info: numerisches Feld, DB-Feld: ktechw.dicke)
- **Windlast**: Windlast am Einbauort (N/m²). (Technische Info: numerisches Feld, DB-Feld: ktechw.wlast)
- **Bereich**: Angabe der Fassadenzone (Rand, zentral). (Technische Info: Toggle-Feld, DB-Feld: ktechw.bereich)
- **Ug-WertDIN**: Wärmedurchgangskoeffizient nach DIN-Norm (W/m²K). (Technische Info: numerisches Feld, DB-Feld: ktechw.kwert)
- **Ug-Wert**: Wärmedurchgangskoeffizient. (Technische Info: numerisches Feld, DB-Feld: ktechw.kbazwert)
- **Transmiss.**: Lichtdurchlässigkeit für den direkt durchgelassenen Strahlungsanteil. (Technische Info: numerisches Feld, DB-Feld: ktechw.trwert)
- **g-Wert**: Energiedurchlasskoeffizient (Gesamtdurchlassgrad). (Technische Info: numerisches Feld, DB-Feld: ktechw.gwert)
- **dB-Wert**: Schalldämmungs-Wert der Position in Dezibel. (Technische Info: numerisches Feld, DB-Feld: ktew.dbwert)

**Verdeckte Maßangaben**
Mit `<F4> > Produktangaben > Technische Werte` können Sie im Zusatzmenü einen der folgenden Einträge auswählen:
- **Verdeckte Maßangaben anzeigen**: Zeigt die verdeckten Maßangaben der gewählten Position an.
- **Verdeckte Maßangaben ändern**: Öffnet den Dialog Artikel-Maßangaben. ⇨ Verkauf, "Artikel-Maßangaben" auf Seite D-148

**Grafische Darstellung der Position**
- **Schematischer Aufbau**: Zeigt den Scheibenaufbau im Querschnitt an.
- **Aufsicht**: Zeigt das Scheibenmodell und/oder den Sprossenaufbau der Scheibe in der Aufsicht an.

**Register Allgemein**
- **Pos**: Positionsnummer. (Technische Info: numerisches Feld, DB-Feld: kpos.Ifdpos)
- **Li. Pos**: Lieferantenposition. (Technische Info: numerisches Feld, DB-Feld: kpos.kuposnr)
- **Artikel**: Artikelnummer. Sie können im Feld Artikel eine kunden- oder lieferantenindividuelle Artikelnummer angeben. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.artnr)
  > **Originale oder neue Stückliste zuweisen**
  > Sie können dem Artikel die originale Stückliste oder eine neue Stückliste zuweisen. Mit `<F5>` im Feld Artikel übernehmen Sie die originale Stückliste. Mit `<Shift> + <F5>` im Feld Artikel wird dem Artikel eine neue Stückliste zugeordnet.
- **SLNr**: Stücklistennummer des Artikels. (Technische Info: numerisches Feld, DB-Feld: kpos.poskonr)
- **Menge**: Einheiten der Position. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.menge)
- **Breite, Höhe, SZR**: Breite, Höhe und Scheibenzwischenraum in für den Artikel hinterlegten Maßeinheiten. (Technische Info: Pflichtfelder, numerische Felder, DB-Felder: kpos.laenge, kpos.breite, kpos.szr)
- **(Spalten ohne Bezeichnung)**: Maßangabe für Längen-, Zeit- und Stückartikel. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.laenge)
- **SN**: Die Checkbox zeigt an, ob eine SN-Datei der Position zugewiesen ist.
- **Prov**: Provision bei aktiver Vertreter-Provisionierung. (Technische Info: numerisches Feld, DB-Feld: kpos.provnr)
- **B.Art**: Die Beschaffungsart bestimmt, wie ein Artikel beschafft wird. (Technische Info: Toggle-Feld, DB-Feld: kpos.beschaffart)
- **kg/St, ME/St**: Mengeneinheit in Kilogramm pro Stück, Mengeneinheit in Quadratmetern pro Stück. (Technische Info: Anzeigefeld, DB-Feld: kpos.gewme)
- **Preis(-feld)**: Nettopreis der Position.
  - Mit `<F4> > Preisangaben > Preiskontrolle` zeigen Sie weitere Spalten im Register an:
    - **aVK**: Vorab-Verkaufs-Preiskennzeichen aus dem übertragenen Haus.
    - **PKZ**: Vorab-Preiskennzeichen aus dem übertragenen Haus.
    - **nVK**: Neu ermitteltes Verkaufs-Preiskennzeichen.
    - **aVF**: Vorab-Verkaufs-Faktor aus dem übertragenen Haus.
    - **Faktor**: Vorab-Faktor in Prozent aus dem übertragenen Haus.
    - **nVF**: Neu ermittelter Verkaufs-Faktor.
    - **aVK-Pr.**: Vorab-Verkaufs-Preis aus dem übertragenen Haus.
    - **nVK-Pr.**: Neu ermittelter Verkaufs-Preis.
- **Stapel**: Stapel-ID des Artikels, der aus dem Stapellager bezogen wird.
- **Bemerkung**: Eine Information zur Position eintragen.

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

#### Bestellpositionen – Eigenschaften
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Eigenschaften**

*[Image: Bestellposition – Eigenschaften (Abb. E-22)]*

In diesem Register können Sie die Eigenschaften der aktuellen Position bearbeiten, z. B. Lagerzuordnung, Verpackart.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Register Eigenschaften**
- **Bezeichnung**: Bezeichnung des Kopfartikels. (Technische Info: alphanumerisches Feld, DB-Feld: kpos.artbez1)
- **Kostenstelle**: Bezeichnung der Kostenstelle. (Technische Info: alphanumerisches Feld, DB-Feld: kpos.kostenst)
- **LE-Nummer**: Nummer der Leistungserklärung. ⇨ Verkauf, "Auftragserfassung - Berechnete technische Werte" auf Seite D-185 (Technische Info: alphanumerisches Feld, DB-Feld: kpos.lbrefnr)
- **Lager**: Nummer des Lagers. (Technische Info: numerisches Feld, DB-Feld: kpos.Inr)
- **Stapel**: Nummer des Stapellagers. (Technische Info: numerisches Feld, DB-Feld: kpos.sfill1)
- **Kiste**: Nummer des Kistenlagers. (Technische Info: numerisches Feld, DB-Feld: bpos.kistennr)
- **Fach**: Bezeichnung des Fachlagers. (Technische Info: numerisches Feld, DB-Feld: bpos.fach)
- **CE-Kennz**: CE-Kennzeichen. (Technische Info: alphanumerisches Feld, DB-Feld: kpos.steuerzu)
- **Konto**: Bezeichnung des Buchungskontos der Kostenstelle. (Technische Info: alphanumerisches Feld, DB-Feld: kposp.mankonto)
- **Bruchgrund**: Nummer des Bruchgrundes. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bpos.bruch)
- **Bruchort**: Nummer und Bezeichnung des Bruchortes. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bpos.bruchort)
- **Skizzendruck**: Art der Skizze, z. B. SNLive. (Technische Info: Auswahlfeld, DB-Feld: ipos.imagedrkz)
- **kg/ME, kg/Stück, kg/Pos, kg/Glas**: Gewicht der Position. (Technische Info: numerische Felder)
- **Physik ME/St**: Physikalische Menge in Mengeneinheit pro Stück. (Technische Info: numerisches Feld, DB-Feld: kpos.phymestk)
- **Berech ME/St**: Berechnete Menge in Mengeneinheit pro Stück. (Technische Info: numerisches Feld, DB-Feld: kpos.qm)
- **Verpackart**: Nummer der Verpackungsart. (Technische Info: numerisches Feld, DB-Feld: kpos.verpackart)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

#### Bestellpositionen – Preise
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Preise**

*[Image: Bestellposition – Preise (Abb. E-23)]*

In diesem Register werden die Einkaufs-Preise zu der aktuellen Position angezeigt.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Register Preise**
- **ME-Preis**: Preis pro Mengeneinheit. (Technische Info: Anzeigefeld, DB-Feld: kpos.ekbmepreis)
- **Stück-Brutto**: Brutto-Stückpreis. (Technische Info: Anzeigefeld, DB-Feld: kpos.bmstpreis)
- **Faktor**: Faktor für den Preiszuschlag in Prozent. (Technische Info: Anzeigefeld, DB-Feld: kpos.ekfaktor)
- **Stück-Netto**: Netto-Stückpreis. (Technische Info: Anzeigefeld, DB-Feld: kpos.eknstpreis)
- **Stück-Verglas**: Stückpreis für Verglasungs- oder Montagearbeiten. (Technische Info: Anzeigefeld, DB-Feld: kpos.ekverglas)
- **Gesamtpreis**: Netto-Gesamt-Preis der Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.vorrabatt)
- **Abzg**: Abzüglich. Individuell vereinbarter Rabatt der Position. (Technische Info: numerische Felder, DB-Felder: kpos.rabatt, kpos.nachlass)
- **Positionspr.**: Positionspreis. (Technische Info: numerisches Feld, DB-Feld: kpos.npospreis)
- **Steuersätze**: ID des Mehrwertsteuersatzes der Position. (Technische Info: Auswahlfeld, DB-Feld: kpos.steuerzu)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

#### Bestellpositionen – Auftragsinfo
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register AuftragsInfo**

*[Image: Bestellposition – AuftragsInfo (Abb. E-24)]*

In diesem Register werden die referenzierten Auftragsinformationen zur aktuellen Position angezeigt.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Register Auftragsinfo**
- **Kund.Auftrag, Pos.**: Auftrags- und Positionsnummer bei auftragsbezogenen Bestellungen. (Technische Info: numerische Felder, DB-Felder: bpos.vkauftrnr, bpos.vklfdpos)
- **Knd-Objekt**: Objektnummer des Kundenauftrags. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: bpos.vkobjnr)
- **Orig. Tupel**: Teilenummer der Stücklistenposition aus dem Kundenauftrag. (Technische Info: numerisches Feld, DB-Feld: bpos.orgtnr)
- **Bemerkung**: Zusätzliche Information zur Position. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.bemerkung)
- **Anlieferdatum**: Gewünschter Liefertermin der Position. (Technische Info: Datumsfeld, DB-Feld: bpos.Itideal)
- **Geplant**: Geplanter Liefertermin der Position. (Technische Info: Datumsfeld, DB-Feld: bpos.Itplan)
- **Avisiert**: Lieferantenseitig bestätigter Liefertermin der Position. (Technische Info: Datumsfeld, DB-Feld: bpos.ltavis)
- **Avisierte Menge**: Lieferantenseitig bestätigte Stückzahl der Lieferposition. (Technische Info: Datumsfeld, DB-Feld: bpos.avismenge)
- **AB-Nr. Lief.**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: numerisches Feld, DB-Feld: bpos.abnr)
- **Art.Nr. Lief.**: Lieferantenseitige Artikelnummer. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.exartnr)
- **LS-Nr.**: Lieferschein-Nummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.lieferschein)
- **Bestellbez.**: Lieferantenspezifische Artikelbezeichnung. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.bestellbez)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

#### Bestellpositionen – Status
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Status**

*[Image: Bestellposition – Status (Abb. E-25)]*

In diesem Register wird der Status der Positionen angezeigt, z. B. Anzahl der gelieferten und fakturierten Artikel.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Register Status**
- **Fertig**: Anzeige der gefertigten Einheiten pro Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.gesfert)
- **Verpackt**: Anzeige der verpackten und zum Transport vorbereiteten Einheiten pro Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.gespack)
- **Gelief.**: Anzeige der ausgelieferten Einheiten pro Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.geslief)
- **Berech**: Anzeige der fakturierten Einheiten pro Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.gesberech)
- **Storno**: Anzeige der stornierten Einheiten pro Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.gesstorno)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

#### Bestellpositionen – Bewertung
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Bewertung**

*[Image: Bestellposition – Bewertung (Abb. E-26)]*

In diesem Register lassen Sie sich Details zur Lieferung anzeigen, z. B. wie zuverlässig der Lieferant liefert. Die Bewertungskriterien hinterlegen Sie in den Lieferanten-Stammdaten.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

**Register Bewertung**
- **Termin**: Bewertung der Termintreue des Lieferanten für die Position. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.wtermin)
- **Preise**: Bewertung der Preisgestaltung des Lieferanten für die Position. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.wpreis)
- **Qualität**: Bewertung der Qualität der gelieferten Position. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.wqual)
- **Menge**: Bewertung der gelieferten Menge der Position. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.wmenge)
- **Spezial**: Bewertung des Lieferanten und Abwicklungsvorgangs. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.wspec)

**Fußbereich**
Die Felder im Fußbereich sind zum Register **Bestellerfassung – Kopf, Fuß** beschrieben: ⇨ "Bestellerfassung - Kopf, Fuß" auf Seite E-51

### Abholadresse
**Einkauf > Bestellverwaltung > Bestellung öffnen > Feld Erf.Datum > <F4> > Adressen > Abholadresse**

*[Image: Abholadresse (Abb. E-27)]*

In diesem Dialog erfassen Sie eine Abholadresse. Wenn Sie die Ware selbst abholen möchten, können Sie hier die Abholadresse hinterlegen.
- **Name, Vorname**: Nachname und Vorname des Kunden. (Technische Info: Pflichtfelder, alphanumerische Felder, DB-Felder: adr.adrname, adr.adrvname)
- **Anrede**: Nummer der Anrede des Kunden. (Technische Info: numerisches Feld, DB-Feld: adr.anrede)
- **z. Hd.**: Name des Ansprechpartners. (Technische Info: alphanumerisches Feld, DB-Feld: adr.zhd)
- **Zusatz**: Zusätzliche Information zur Adresse. (Technische Info: alphanumerisches Feld, DB-Feld: adr.branche)
- **Straße**: Straßenname und Hausnummer der Abholadresse. (Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: adr.str)
- **Postfach**: Postleitzahl und Nummer des Postfachs. (Technische Info: alphanumerische Felder, DB-Felder: adr.pfplz, adr.postfach)
- **PF Ort**: Postfachkürzel der Abholadresse bei Kunden außerhalb Europas. (Technische Info: alphanumerisches Feld, DB-Feld: adr.pfort)
- **PLZ**: Postleitzahl der Abholadresse. (Technische Info: alphanumerisches Feld, DB-Feld: adr.plz)
- **Ort**: Ortsname der Abholadresse. (Technische Info: alphanumerisches Feld, DB-Feld: adr.ort)
- **KFZ Land**: Internationales Kraftfahrzeugkennzeichen des Empfängerlandes. (Technische Info: alphanumerisches Feld, DB-Feld: adr.kfzcode)
- **Entfernung**: Entfernung bis zum Lieferanten in Kilometer. (Technische Info: numerisches Feld, DB-Feld: adr.kilometer)
- **Fahrtzeit**: Fahrtzeit bis zum Lieferanten in Tagen. (Technische Info: numerisches Feld, DB-Feld: adr.fahrtzeit)
- **Handlingszeit**: Zeit zum Beladen und Entladen der Lieferung. (Technische Info: numerisches Feld, DB-Feld: adr.handlingszeit)
- **Ankunftszeit**: Gewünschte Ankunftszeit zum Lieferant im Format hh:mm. (Technische Info: alphanumerisches Feld, DB-Feld: adr.ankunftszeit)
- **Anlieferstelle**: Genauere Beschreibung der Anlieferstelle, z. B. Tor A. (Technische Info: alphanumerisches Feld, DB-Feld: adr.anlieferstelle)
- **Faxnummer**: Faxnummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: adr.fax)
- **Route**: Nummer der Fahrtroute. (Technische Info: numerisches Feld, DB-Feld: adr.routenr)
- **Ladefolge**: Nummer der gewünschten Ladeposition. (Technische Info: numerisches Feld, DB-Feld: adr.routeposnr)
- **Bemerkung**: Textfelder für zusätzliche Informationen. (Technische Info: alphanumerische Felder, DB-Felder: adr.text1, adr.text2, adr.text3)

### Bestellarten
**Einkauf > Bestellverwaltung > Bestellung öffnen > Feld Objekt > <Strg> + <F12>**

*[Image: Bestellarten (Abb. E-28)]*

In diesem Dialog legen Sie die Art der Bestellung fest. Standardmäßig hat jede Bestellung die Bestellart **normal**.
- **Normale Bestellung**: Voreingestellter Standard der Bestellerfassung.
- **Interne Bestellung**: Interne Bestellung zwischen den eigenen Häusern.
- **Kostenlose Bestellung**: Bestellung mit dem Rechnungsbetrag gleich Null. ⇨ Verkauf, "Reklamation" auf Seite D-156
- **Speditionsbestellung**: Diese Bestellart wird nicht mehr unterstützt.

### Dokumentenartenzuordnung
**Einkauf > Bestellverwaltung > Bestellung öffnen > Feld Lief-Pos > <Strg> + <K>**
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein > Feld Preis > <Strg> + <K>**

*[Image: Dokumentenartenzuordnung (Abb. E-29)]*

In diesem Dialog ordnen Sie einem Vorgang oder einzelnen Positionen Dateien zu.
Der Dialog ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Dokumentenartenzuordnung" auf Seite D-167

> **Dokumentenzuordnung aus dem Auftrag**
> In der Auftragserfassung können die zugeordneten Dokumente sowie auf der Kopfebene als auch auf der Positionsebene zur Übernahme für die erzeugten Bestellung markiert werden. Dazu wird im Auftrag das Checkbox **Best.** aktiviert werden. Dabei wird das zugeordnete Dokument in die neue Bestellung kopiert.

### Texte

Mit Texten hinterlegen Sie zusätzliche Informationen zu Vorgängen. Die Texte können auf verschiedenen Formularen ausgedruckt werden. Die Menüpunkte sind ausführlich zum Part Verkauf beschrieben:
- Verkauf, "Anmerkungen" auf Seite D-243
- Verkauf, "Kopf- und Fußtexte" auf Seite D-252
- Verkauf, "Artikel- und Positionstexte" auf Seite D-254
- Verkauf, "Spezielle Texte" auf Seite D-255
- Verkauf, "Floskeln" auf Seite D-256
- Verkauf, "Fremdinformationen" auf Seite D-258

#### Auftragstexte
**Einkauf > Bestellungen erzeugen > Abteilung auswählen > <F3> > <Shift> + <F4> > Auftragstexte darstellen**

*[Image: Auftragstexte (Abb. E-30)]*

In diesem Dialog werden die Auftragstexte zu den Bestellartikeln angezeigt. Artikeltexte sind mit dem Buchstaben A gekennzeichnet, Positionstexte mit dem Buchstaben P.
Im Dialog **Bestellungen erzeugen** wird in der Spalte **Txt** angezeigt, ob Texte zu der Bestellposition erfasst wurden. ⇨ "Bestellungen erzeugen - Lieferant" auf Seite E-37

Alternativ zum Infomenü können Sie die Auftragstexte mit `<Strg> + <F10>` aus dem Dialog **Bestellungen erzeugen** aufrufen.

### Formulardruck

Über den Dialog **Formulardruck** oder **E-Mail** können Sie Bestellungen drucken und an den Lieferanten versenden. Die Dialoge sind ausführlich zum Part Verkauf beschrieben:
- ⇨ Verkauf, "Formulardruck" auf Seite D-357
- ⇨ Verkauf, "E-Mail" auf Seite D-361

### Bestellfreigabe
**Einkauf > Bestell-Freigabe**

In diesem Dialog können Sie Bestellungen freischalten, bzw. sperren oder stornieren. Je nach Systemkonfiguration können die Bestellungen auch direkt nach der Bestellerzeugung bzw. Bestellerfassung freigegeben werden.
Im Änderungsprotokoll können Sie den Status einer Bestellung prüfen. ⇨ Verkauf, "Änderungs-Protokoll" auf Seite D-171

In diesem Dialog finden Sie folgende Ansichten:
- "Bestellfreigabe - Auswahl" auf Seite E-98
- "Bestellfreigabe - Details" auf Seite E-99
- "Bestellfreigabe – Weitere Felder" auf Seite E-101

#### Bestellfreigabe – Auswahl
**Einkauf > Bestell-Freigabe**

*[Image: Bestellfreigabe – Auswahl (Abb. E-31)]*

In dieser Ansicht wählen Sie die Bestellung aus, die Sie bearbeiten wollen.
- Mit `<F5>` wechseln Sie zur Ansicht **Bestellfreigabe – Details**.
- Mit `<F3>` lösen Sie die gewählte Funktion zur Bestellung aus.

**Kopfbereich**
- **Bestellnr.**: Bestellnummer. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr)
- **Aktuell**: Aktueller Status der Bestellung (freigegeben, erzeugt, storniert). (Technische Info: Anzeigefeld, DB-Feld: kaufstat.status)
- **Aktion**: Auswahl der Funktion, die Sie auslösen wollen.
  - **freigeben**: Die Bestellung wird freigegeben.
  - **stornieren**: Die Bestellung wird storniert und die Positionen werden zurück in den Bestellpool gestellt.
  - **zurücksetzen**: Die Bestellung wird storniert. Sie können nur Bestellungen zurücksetzen, die den Status `freigegeben` haben.
- **Anlieferdatum**: Geplanter Liefertermin der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan)
- **Lieferant**: Nummer und Name des Lieferanten. (Technische Info: Anzeigefelder, DB-Felder: kauf.kunr, mp.name)
- **Stornoinfo**: Bemerkung zum Storno. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.exbez2)

**Fußbereich**
- **Auslösen**: Löst die gewählte Funktion aus.
- **Details**: Wechselt zur Ansicht **Bestellfreigabe – Details**.
- **Beenden**: Schließt den Dialog.

#### Bestellfreigabe – Details
**Einkauf > Bestell-Freigabe > Bestellung auswählen > <F5>**

*[Image: Bestellfreigabe – Details (Abb. E-32)]*

In dieser Ansicht werden die Positionsdetails zur gewählten Bestellung angezeigt.
Mit `<F2>` wechseln Sie zur Ansicht **Bestellfreigabe – Weitere Felder**.

**Kopfbereich**
Der Kopfbereich ist zur Ansicht **Bestellfreigabe – Auswahl** beschrieben.

**Positionsübersicht**
- **Pos**: Positionsnummer. (Technische Info: numerisches Feld, DB-Feld: kpos.lfdpos)
- **Artikel**: Artikelbezeichnung. (Technische Info: Anzeigefeld, DB-Feld: kpos.artbez1)
- **Bestellt**: Stückzahl der bestellten Position. (Technische Info: numerisches Feld, DB-Feld: kpos.menge)
- **Breite, Höhe**: Maße der Position in Millimeter. (Technische Info: numerische Felder, DB-Feld: kpos.laenge, kpos.breite)
- **Auftrag**: Auftragsnummer bei Bestellpositionen aus Kundenaufträgen. (Technische Info: numerisches Feld, DB-Feld: bpos.vkauftrnr)
- **Auslieferung**: Geplanter Liefertermin des Kundenauftrags. (Technische Info: Datumsfeld, DB-Feld: kpos.ltplan)

**Fußbereich**
- **OK**: Schließt die aktuelle Ansicht und wechselt zur Ansicht **Bestellfreigabe – Auswahl**.
- **Abbrechen**: Schließt die aktuelle Ansicht und wechselt zur Ansicht **Bestellfreigabe – Auswahl**.

#### Bestellfreigabe – Weitere Felder
**Einkauf > Bestell-Freigabe > Bestellung auswählen > <F5> > <F2>**

*[Image: Bestellfreigabe – Weitere Felder (Abb. E-33)]*

In diesem Dialog werden weitere Informationen zur ausgewählten Bestellposition angezeigt.
- Mit `<F2>` wechseln Sie zur Ansicht **Bestellfreigabe – Details**.
- Mit `<Bild hoch>` und `<Bild runter>` wechseln Sie zur vorherigen bzw. nächsten Position.

**Kopfbereich**
Der Kopfbereich ist zur Ansicht **Bestellfreigabe – Auswahl** beschrieben.

**Bestelldetails**
- **Artikel**: Nummer und Bezeichnung des Artikels. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kpos.artnr, kpos.artbez1)
- **Menge**: Stückzahl der bestellten Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.menge)
- **Avisiert**: Lieferantenseitig bestätigte Stückzahl zum Liefertermin. (Technische Info: Anzeigefeld, DB-Feld: bpos.avismenge)
- **Maßvar.**: Maßvariante der bestellten Position bei variantenführigen Artikeln. (Technische Info: Anzeigefeld, DB-Feld: kpos.var)
- **Lfm**: Laufmeter der Bestellposition. (Technische Info: Anzeigefeld, DB-Feld: kpos.umlfdm)
- **Qm**: Glasfläche der Bestellposition in Quadratmeter. (Technische Info: Anzeigefeld, DB-Feld: kpos.qm)
- **SZR**: Scheibenzwischenraum in Millimeter. (Technische Info: Anzeigefeld, DB-Feld: kpos.szr)
- **AB-Nr. Lief.**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: numerisches Feld, DB-Feld: bpos.abnr)
- **Position**: Positionsnummer aus dem Auftrag. (Technische Info: numerisches Feld, DB-Feld: bpos.vklfdpos)
- **Kunde**: Kundenname bei Bestellpositionen aus Kundenaufträgen. (Technische Info: Anzeigefeld, DB-Feld: kauf.kunr, mp.name)
- **Lager**: Nummer und Bezeichnung des Lagers bei Lagerartikeln. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bpos.Inr)
- **Objekt**: Nummer und Bezeichnung des Objekts. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bpos.vkobjnr, mp.name)
- **Stückpreis**: Stückpreis der Bestellposition. (Technische Info: numerisches Feld, DB-Feld: kpos.nstpreis)
- **Pos. Preis**: Gesamtpreis der Bestellposition. (Technische Info: numerisches Feld, DB-Feld: kpos.npospreis)

**Fußbereich**
- **OK / Abbrechen**: Schließt den Dialog **Bestellfreigabe**. Änderungen werden nicht gespeichert.

### Wareneingang

Für Lieferungen können Sie sich den Lieferplan zur Bestellung und die Lieferbestätigung des Lieferanten anzeigen lassen. Sie können Teilwareneingänge und Wareneingänge avisieren und verbuchen und so einen termingerechten Wareneingang überprüfen.
Außerdem können Sie die Bestellungen abschließen, die im System nicht mehr verfolgt werden sollen.

In diesem Abschnitt finden Sie folgende Informationen:
- "Lieferavis" auf Seite E-103
- "Lieferplan" auf Seite E-111
- "Wareneingang (automatisch)" auf Seite E-114
- "Positionsinfo" auf Seite E-117
- "Buchung Gestelle" auf Seite E-117
- "Wareneingang (manuell)" auf Seite E-119
- "Gestellbezogener Wareneingang" auf Seite E-121
- "Bestellungen abschließen" auf Seite E-141
- "Wareneingangskontrolle" auf Seite E-125
- "Fehlmengenkontrollpool" auf Seite E-126
- "Wareneingangsprotokoll" auf Seite E-127

#### Lieferavis
**Einkauf > Lieferavis**

In diesem Dialog verwalten Sie die Lieferbestätigungen der Lieferanten.
In diesem Dialog finden Sie folgende Register und Ansichten:
- "Lieferavis - Übersicht" auf Seite E-104
- "Lieferavis - Details" auf Seite E-106
- "Bestellung - Übersicht (Lieferavis)" auf Seite E-108
- "Bestellung - Details (Lieferavis)" auf Seite E-109

##### Lieferavis – Übersicht
**Einkauf > Lieferavis > Register Übersicht**

*[Image: Lieferavis - Register Übersicht (Abb. E-34)]*

In diesem Register erfassen Sie die Ankündigungen der Wareneingänge.
- Mit `<F2>` wechseln Sie zum Register **Lieferavis – Details**.
- Mit `<F5>` im Feld **AB-Nr. Lieferant** im Rumpfbereich öffnen Sie den Dialog **Bestellung**.

**Kopfbereich**
- **AB-Nr. Lieferant**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.abnr)
- **Anlieferdatum**: Geplanter Anliefertermin. (Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: bpos.ltplan)
- **Haus**: Hausnummer aus der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr)
- **Lieferant**: Lieferantennummer. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.kunr)

**Rumpfbereich**
- **Bestellung**: Bestellnummer. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr)
- **AB-Nr. Lieferant**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.abnr)
- **Bestellt zum**: Datum, an dem die Bestellung eintreffen soll. (Technische Info: Datumsfeld, DB-Feld: kauf.ltplan)
- **Nummer**: Lieferantennummer aus der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.kunr)
- **Lieferant**: Name des Lieferanten. (Technische Info: Anzeigefeld, DB-Feld: mp.name)
- **Menge**: Stückzahl der Position, die angeliefert wird. (Technische Info: Anzeigefeld, DB-Feld: bpos.avismenge)

##### Lieferavis – Details
**Einkauf > Lieferavis > Register Details**

*[Image: Lieferavis - Register Details (Abb. E-35)]*

In diesem Register lassen Sie sich die Details der Bestellung anzeigen. Änderungen können Sie anhand der Lieferantenbestätigung eintragen.
- Mit `<F2>` wechseln Sie zum Register **Lieferavis – Übersicht**.
- Mit `<F5>` im Feld **AB-Nr. Lieferant** öffnen Sie den Dialog **Bestellung**.
- Mit `<Strg> + <L>` kann die Lieferadresse überprüft werden.

**Kopfbereich**
Die Felder im Kopfbereich sind zum Register **Lieferavis – Übersicht** beschrieben.

**Bestellinformationen**
- **Bestellnr.**: Bestellnummer. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr)
- **AB-Nr. Lief.**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.abnr)
- **Lieferant**: Nummer und Name des Lieferanten. (Technische Info: Anzeigefelder, DB-Felder: kauf.kunr)
- **Straße, PLZ, Ort**: Anschrift des Lieferanten.
- **MwSt-Kennz.**: Nummer, Bezeichnung und Prozentsatz des Mehrwertsteuer-Kennzeichens. (Technische Info: Anzeigefelder, DB-Felder: kauf.kukz)
- **Liefertermin**: Tatsächlicher Liefertermin der Bestellung. (Technische Info: Datumsfeld, DB-Feld: kauf.ltplan)
- **alt**: Alter, geplanter Liefertermin der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: bpos.Itplan)
- **Tour**: Nummer und Bezeichnung der Lieferroute. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.routenr)
- **Nettobetrag**: Summe aller Positionspreise der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.nettototal)
- **MwSt-Betrag**: Mehrwertsteuer-Betrag der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.mwstbetrag)
- **Bruttobetrag**: Brutto-Betrag der Bestellung. (Technische Info: Anzeigefeld, DB-Feld:kauf.gesbrutto)

**Auftragsinformationen**
- **Auftragsnr.**: Auftragsnummer bei auftragsbezogenen Bestellungen. (Technische Info: Anzeigefeld, DB-Feld:kauf.auftrnr)
- **Kundenname**: Name des Kunden aus dem Kundenauftrag. (Technische Info: Anzeigefeld, DB-Feld:kauf.kunr)
- **Liefertermin**: Geplanter Liefertermin des Kundenauftrags. (Technische Info: Anzeigefeld, DB-Feld:kauf.ltplan)
- **Tour**: Nummer und Name der Lieferroute zum Kunden. (Technische Info: Anzeigefelder, DB-Felder: kauf.routenr)

##### Bestellung – Übersicht (Lieferavis)
**Einkauf > Lieferavis > ... > Feld AB-Nr.Lieferant > <F5>**

*[Image: Bestellung - Übersicht (Lieferavis) (Abb. E-36)]*

In diesem Register können Sie die positionsgenaue Lieferavis bearbeiten, z. B. die angekündigte Liefermenge ändern.
Mit `<F2>` wechseln Sie zum Register **Bestellung – Details (Lieferavis)**.

**Übersicht**
- **Pos**: Positionsnummer. (Technische Info: Anzeigefeld, DB-Feld:kpos.Ifdpos)
- **Artikel**: Artikelnummer der Position. (Technische Info: numerisches Feld, DB-Feld: kpos.artnr)
- **Bestellt**: Stückzahl der bestellten Position. (Technische Info: numerisches Feld, DB-Feld: kpos.menge)
- **AB-Nr. Lief.**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: numerisches Feld, DB-Feld: bpos.abnr)
- **Avisiert**: Lieferantenseitig bestätigte Stückzahl der Lieferung. (Technische Info: numerische Felder, DB-Felder: bpos.avismenge)
- **Stückpreis**: Netto-Stück-Preis der Position. (Technische Info: numerisches Feld, DB-Feld: kpos.nstpreis)
- **Pos. Preis**: Netto-Gesamt-Preis der Position. (Technische Info: numerisches Feld, DB-Feld: kpos.npospreis)
- **Faktur.**: Faktura-Kennzeichen der Position. (Technische Info: Anzeigefeld, DB-Feld: kpos.fakturakz)

##### Bestellung - Details (Lieferavis)
**Einkauf > Lieferavis > ... > Feld AB-Nr.Lieferant > <F5> > Register Details**

*[Image: Bestellung (Lieferavis) – Register Details (Abb. E-37)]*

In diesem Register können Sie die Details für die vom Lieferanten angekündigte Lieferung eingeben.
Mit `<F2>` wechseln Sie zum Register **Bestellung – Übersicht (Lieferavis)**.

- **Artikel**: Nummer und Bezeichnung des Artikels. (Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kpos.artnr, kpos.artbez1)
- **Bemerkung**: Zusätzliche Information zur Position. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.bemerkung)
- **Kostenstelle**: Bezeichnung der Kostenstelle. (Technische Info: numerisches Feld, DB-Feld: kpos.kostenst)
- **Konto**: Bezeichnung des Buchungskontos. (Technische Info: alphanumerisches Feld, DB-Feld: kpos.konto)
- **Modell**: Modellnummer bei Bestellpositionen. (Technische Info: Anzeigefeld, DB-Feld: kpos.modnr)
- **Bestellt**: Stückzahl der bestellten Position. (Technische Info: numerisches Feld, DB-Feld: kpos.menge)
- **Geliefert**: Anzahl der gelieferten Positionen. (Technische Info: Anzeigefeld, DB-Feld: kpos.geliefert)
- **Breite, Höhe**: Maße der Position in Millimeter. (Technische Info: Anzeigefelder, DB-Felder: kpos.laenge, kpos.breite)
  > **Eindimensionale Mengen-Eingabe**
  > Bei einer Systemkonfiguration kann im Wareneingang bei Artikel mit Mengeneinheiten (1,6,7,8,10) auch eine Teilmenge bezogen auf diese Mengeneinheit gemeldet werden. Das Feld `kpos.laenge` ist entsprechend änderbar.
- **SZR**: Scheibenzwischenraum in Millimeter. (Technische Info: Anzeigefeld, DB-Feld: kpos.szr)
- **qm Stück**: Fläche in Quadratmeter pro Stück. (Technische Info: numerisches Feld, DB-Feld: kpos.qm)
- **AB-Nr. Lieferant**: Nummer der Auftragsbestätigung vom Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.abnr)
- **Anlieferdatum**: Tatsächlicher Liefertermin der Bestellposition. (Technische Info: Datumsfeld, DB-Feld: bpos.ltavis)
- **Avisiert**: Lieferantenseitig bestätigte Stückzahl der Lieferung. (Technische Info: numerische Felder, DB-Felder: bpos.avismenge)
- **alt**: Alter, geplanter Liefertermin der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: bpos.ltplan)
- **Auftrag**: Auftragsnummer bei auftragsbezogenen Bestellungen. (Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr)
- **Position**: Nummer der Position bei auftragsbezogenen Bestellungen. (Technische Info: Anzeigefeld, DB-Feld: kpos.Ifdpos)
- **Bruchgrund**: Anzeige der Nummer und die dazugehörige Bruchgrund-Bezeichnung. (Technische Info: Anzeigefeld, DB-Feld: bpos.bruch)
- **Lieferdatum**: Termin der Anlieferung beim Kunden.
- **Knd-Objekt**: Objektnummer und -bezeichnung des Kundenauftrags. (Technische Info: Anzeigefelder, DB-Felder: bpos.vkobjnr.)
- **Lagernummer**: Nummer und Bezeichnung des Lagers. (Technische Info: Anzeigefelder, DB-Felder: bpos.Inr)
- **Art.Nr. Lief.**: Lieferantenseitige Artikelnummer. (Technische Info: numerisches Feld, alphanumerisches Feld, DB-Felder: bpos.exartnr, bpos.bestellbez)
- **ME-Preis**: Preis pro Mengeneinheit. (Technische Info: numerisches Feld, DB-Feld: kpos.bmepreis)
- **Stück-Netto**: Netto-Stückpreis. (Technische Info: numerisches Feld, DB-Feld: kpos.nstpreis)
- **Pos. Preis**: Netto-EK-Preis pro Stück. (Technische Info: numerisches Feld, DB-Feld: kpos.npospreis)

#### Lieferplan
**Einkauf > Wareneingang > Lieferplan**

*[Image: Lieferplan - Register Übersicht (Abb. E-38)]*

In diesem Dialog können Sie die geplante Lieferungen verplanen.
- Mit `<F2>` wechseln Sie zum Register **Lieferplan – Details**.
- Mit `<Strg> + <G>` wechseln Sie zum Dialog **Buchung Gestelle**.
- Mit `<OK>` speichern Sie den Lieferplan.

- **Haus**: Hausnummer. (Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr)
- **Bestellung**: Angabe der Bestellnummer. (Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr, kauf.vorgang=2)
- **Lieferant**: Anzeige der Lieferantennamen. (Technische Info: Anzeigefeld, DB-Feld: kauf.kunr, mp.name)

**Übersicht**
- **Pos**: Positionsnummer. (Technische Info: Anzeigefeld, DB-Feld: liefplan.lfdpos)
- **Lief.**: Nummer der Lieferung. (Technische Info: Anzeigefeld, DB-Feld: liefplan.subnr)
- **Anlieferdatum**: Lieferdatum der geplanten Ware. (Technische Info: Anzeigefeld, DB-Feld: liefplan.ltplan)
- **Artikel**: Artikelbezeichnung.
- **AB-Nr. Lief**: Auftragsbestätigung des Lieferanten. (Technische Info: numerisches Feld, DB-Feld: liefplan.abnr)
- **Gesamt**: Gesamt-Menge der bestellten Position. (Technische Info: Anzeigefeld, DB-Feld: liefplan.geslief)
- **Gelief.**: Bereits gelieferte Menge. (Technische Info: Anzeigefeld, DB-Feld: liefplan.geliefert)
- **Verpackt**: Bereits verpackte Menge. (Technische Info: Anzeigefeld, DB-Feld: liefplan.gespack)
- **Geplant**: Geplante Menge für diese (Teil-)Lieferung. (Technische Info: Anzeigefeld, DB-Feld: liefplan.zuliefern)

##### Lieferplan - Details
**Einkauf > Wareneingang > Lieferplan > Bestellung auswählen > <F2>**

*[Image: Lieferplan - Register Details (Abb. E-39)]*

In diesem Register werden die detaillierte Information zur ausgewählten Bestellposition angezeigt.
- Mit `<F2>` wechseln Sie zum Register **Lieferplan – Übersicht**.

**Details**
- **Lager**: Lagernummer des Standardlagers. (Technische Info: Anzeigefeld, DB-Feld: liefplan.Inr)
- **Stapel**: Lagernummer des Stapellagers. (Technische Info: Anzeigefeld, DB-Feld: liefplan.stapel, liefplan.stapelbez)
- **Kiste**: Kistennummer des Kistenlagers. (Technische Info: Anzeigefeld, DB-Feld: liefplan.kistenr)
- **Fach**: Fachbezeichnung des Fachlagers. (Technische Info: Anzeigefeld, DB-Feld: liefplan.fach)

#### Wareneingang (automatisch)
**Einkauf > Wareneingang > Automatischer Wareneingang**

*[Image: Wareneingang (automatisch) (Abb. E-40)]*

In diesem Dialog können Sie die eingetroffenen Lieferungen als Wareneingang buchen.
- Mit `<Werteimport>` laden die im System vorhandenen Bestellungen in den Dialog hoch.
- Mit `<F9>` wählen Sie einzeln die nicht gebuchten Bestellungen aus.
- Mit `<F8>` wählen Sie die nicht gebuchten Bestellungen, zu denen ein Lieferplan existiert, aus.
- Mit `<Strg> + <L>` wechseln Sie in die Spalte **Lieferschein**.
- Mit `<F5>` öffnen Sie den Dialog **Positionsinfo**.
- Mit `<F3>` buchen Sie die davor markierte Bestellung als Wareneingang.

**Bestellungen**
- **Bestellung**: Bestellnummer. (Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr)
- **1. Spalte ohne Namen (Subnummer)**: Subnummer aus dem Lieferplan.
- **2. Spalte ohne Namen (Lieferplan)**: Anzeige, ob ein Lieferplan zu der Bestellung existiert.
- **Haus**: Hausnummer der Bestellung. (Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr)
- **Eingang**: Anzeige, ob zu der Bestellung bereits ein Wareneingang eingetroffen ist.
- **Rechnung**: Nummer der Lieferantenrechnung. (Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr)
- **Fremdnummer**: Auftragsnummer aus dem Verkauf. (Technische Info: Anzeigefeld, DB-Feld: kauf.exaufnr)
- **Datum**: Erfassungsdatum der Bestellung. (Technische Info: Datumsfeld, DB-Feld: kauf.bdat)
- **Lieferschein**: Textfeld für die Lieferscheinbezeichnung. (Technische Info: alphanumerisches Feld, DB-Feld: bpos.lieferschein)
- **Ko.**: Kontrolle. Checkbox, ob die Bestellung im Wareneingang auf Vollständigkeit kontrolliert werden soll.
- **Er.**: Erzeugen. Angabe, ob die Bestellung im Wareneingang gebucht werden soll.

**Fußbereich**
- **Positionen**: Öffnet den Dialog **Positionsinfo**.
- **Werteimport**: Importiert alle nicht gebuchten Bestellungen.
- **Erzeugen**: Bucht alle markierten Bestellungen im Wareneingang.
- **Abbrechen**: Schließt den Dialog.

#### Positionsinfo
**Einkauf > Wareneingang > Automatischer Wareneingang > Bestellung suchen > <F5>**
**Einkauf > Wareneingang > Bestellungen abschließen> Bestellung suchen > <F5>**

*[Image: Positionsübersichten (Abb. E-41)]*

In diesem Dialog lassen Sie sich die Positionsübersicht zu einer Bestellung anzeigen. Mit `<F2>` wechseln Sie das Register.
Die Register zur **Positionsinfo** ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Positionsinfo" auf Seite D-340

#### Buchung Gestelle
**Einkauf > Automatischer Wareneingang > Bestellung auswählen> <F4> > Gestellverwaltung**

*[Image: Buchung Gestelle (Abb. E-42)]*

In diesem Dialog können Sie die Scheiben einer Bestellung pro Position auf die Gestelle zuordnen.

**Kopfbereich**
- **Vorgang**: Bestellnummer, für die das Gestell gebucht wird. (Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr, bcbock.auftrnr)

**Rumpfbereich**
- **Pos**: Nummer der Position auf dem angelieferten Gestell. (Technische Info: Anzeigefeld, DB-Feld: bcbock.bposnr)
- **Anzahl**: Anzahl der Scheiben aus der Position. (Technische Info: Anzeigefeld, DB-Feld: bcbock.anzahl)
- **Gestell, Bezeichnung**: Nummer und Bezeichnung des Gestelltyps. (Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: bcbock.gnr, gest.exgnr)
- Mit `<F2>` zeigen Sie zusätzlich folgende Spalten an:
  - **Verschieben**: Gestellnummer, von dem die Gläser verschoben werden.
  - **Anzahl**: Stückzahl der Gläser, die auf das Zielgestell gebucht werden.
  - **Zielgestell**: Gestellnummer des Zielgestells.

#### Wareneingang (manuell)
**Einkauf > Wareneingang > Manueller Wareneingang > Bestellung suchen**

*[Image: Wareneingang (manuell) (Abb. E-43)]*

In diesem Dialog bearbeiten und buchen Sie die Lieferungen und Teillieferungen, die im Wareneingang eingetroffenen sind.
Mit `[Ende]` speichern Sie Ihre Eingaben und buchen den (Teil-)Wareneingang.

> **Bestellungen bei Teillieferung abschließen**
> Wenn Sie Teilwareneingang buchen, werden Sie gefragt, ob noch weitere Wareneingänge folgen. Mit [Ja] wird nur der Teil-Wareneingang erstellt und gebucht. Mit [Nein] wird der Teil-Wareneingang erstellt und gebucht und die Bestellung wird abgeschlossen.

Der Dialog ist wie der Dialog **Bestellerfassung** aufgebaut: ⇨ "Bestellerfassung" auf Seite E-50

**Kopfbereich**
- **Bestell.**: Bestellnummer und Teillieferungsnummer. (Technische Info: Pflichtfeld, numerische Felder, DB-Felder: kauf.auftrnr, kauf.subnr)
- **LS-Nr.**: Lieferschein-Nummer des Lieferanten. (Technische Info: alphanumerisches Feld, DB-Feld: kauf.lieferschein)
- **Kontrolle**: Anzeige, ob die Bestellung im Wareneingang auf Vollständigkeit kontrolliert werden soll. (Technische Info: Toggle-Feld, DB-Feld: kauf.kontrolle)

**Register Allgemein**
- **Bestellt**: Bestellte Positionsmenge. (Technische Info: numerisches Feld, DB-Feld: kpos.menge)
- **Ber. erhalten**: Bereits eingetroffene Positionsmenge.
- **Erhalten**: Bereits gelieferte Positionsmenge. (Technische Info: numerisches Feld, DB-Feld: kpos.geliefert)
- **Avisiert**: Lieferantenseitig bestätigte Positionsmenge. (Technische Info: numerisches Feld, DB-Feld: bpos.avismenge)

#### Gestellbezogener Wareneingang
**Einkauf > Wareneingang > Gestellbezogener Wareneingang**

In diesem Dialog erfassen und bearbeiten Sie Wareneingänge anhand der Gestelle.
- "Gestellbezogener Wareneingang" auf Seite E-121
- "Gestellbelegung" auf Seite E-123

##### Gestellbezogener Wareneingang
**Einkauf > Wareneingang > Gestellbezogener Wareneingang**

*[Image: Gestellbezogener Wareneingang (Abb. E-44)]*

In diesem Dialog werden gestellbezogene Wareneingänge gebucht.
- Mit `<F6>` öffnen Sie den Dialog **Gestellbelegung** und können eine neue Gestellbelegung durchführen.
- Mit `<F5>` öffnen Sie den Dialog **Gestellbelegung** und können den markierten Wareneingang bearbeiten.

**Übersicht**
- **Gestell**: Gestellnummer. (Technische Info: Anzeigefeld, DB-Feld: waeingestkopf.exgnr)
- **LieferID**: Manuell erfasstes Kennzeichen einer Lieferung. (Technische Info: Anzeigefeld, DB-Feld: waeingestkopf.lieferid)
- **Lagerplatz**: Nummer und Bezeichnung des Lagerplatzes. (Technische Info: Anzeigefeld, DB-Feld: waeingestkopf.lagerplatz)
- **LKW**: KFZ-Kennzeichen des LKWs. (Technische Info: Anzeigefeld, DB-Feld: waeingestkopf.lkwkennzeichen)
- **Lieferant**: Nummer und Name des Lieferanten. (Technische Info: Anzeigefeld, DB-Feld: kauf.kunr, mp.name)
- **Menge**: Die Gesamtmenge aller auf dem Gestell befindlichen Scheiben. (Technische Info: Anzeigefeld, DB-Feld: waeingestpos.menge)
- **Anl.Datum, Zeit**: Datum und Uhrzeit der Lieferung. (Technische Info: Anzeigefeld, DB-Feld: waeingestkopf.datum. waeingstkopf.zeit)
- **Bu.**: Angabe, ob das Gestell im Wareneingang gebucht werden soll.

**Fußbereich**
- **Neu**: Öffnet den Dialog **Gestellbelegung**.
- **Korrektur**: Öffnet den Dialog **Gestellbelegung** für das ausgewählte Gestell.
- **Löschen**: Löscht das ausgewählte Gestell.
- **Buchen**: Bucht die markierten Gestelle.
- **OK**: Bucht die markierten Gestelle und schließt den Dialog.
- **Abbrechen**: Schließt den Dialog ohne zu buchen.

##### Gestellbelegung
**Einkauf > Wareneingang > Gestellbezogener Wareneingang > [Neu], [Korrektur]**

*[Image: Gestellbelegung (Abb. E-45)]*

In dieser Ansicht erfassen und bearbeiten Sie die Gestellbelegung für den Wareneingang.

**Kopfbereich**
- **Gestell (Nr./Bezeichnung)**: Gestellnummer und Gestellbezeichnung. (Technische Info: Pflichtfeld, numerisches und alphanummerisches Felder, DB-Feld: waeingestkopf.gestellnr, waeingestkopf.exgnr)
- **LieferID**: Manuell erfasstes Kennzeichen einer Lieferung. (Technische Info: Anzeigefeld, DB-Feld: waeingestkopf.lieferid)
- **Lagerplatz**: Nummer und Bezeichnung der Lagerstelle. (Technische Info: Pflichtfeld, numerisches Feld, alphanumerisches Feld, DB-Felder: waeingestkopf.lagerplatz)
- **LKW-Kennzeichen**: KFZ-Kennzeichen des LKWs. (Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: waeingestkopf.lkwkennzeichen)
- **Gesamtmenge**: Gesamtstückzahl auf allen Gestellen der Lieferung. (Technische Info: Anzeigefeld, DB-Feld: waeingestpos.menge)
- **Datum**: Datum der Lieferung im Format TT.MM.JJJJ. (Technische Info: Datumsfeld, DB-Feld: waeingestkopf.datum)
- **Zeit**: Uhrzeit der Lieferung im Format hh:mm. (Technische Info: alphanumerisches Feld, DB-Feld: waeingstkopf.zeit)

**Rumpfbereich**
- **Bestellung**: Bestellnummer. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: waeingestpos.auftrnr)
- **Posnr.**: Positionsnummer in der Bestellung. (Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: waeingestpos.posnr)
- **Lieferant**: Nummer und Name des Lieferanten.
- **Lieferschein**: Lieferscheinbezeichnung.
- **Gesamt**: Gesamtstückzahl der gewählten Position.
- **Ber.erh.**: Bereits gelieferte Stückzahl.
- **Menge**: Aktuell gelieferte Stückzahl.
- **Fehlmenge**: Differenz zwischen bestellter und gelieferter Menge.
- **Seite**: Gestellseite (0=keine, 1=links, 2=rechts).
- **Sequenz**: Die Reihenfolge, in der die Position auf dem Gestell steht.

#### Wareneingangskontrolle
**Einkauf > Wareneingang > Wareneingangskontrolle**

*[Image: Wareneingangskontrolle (Abb. E-46)]*

In diesem Dialog werden automatisch Wareneingänge und Einkaufsrechnungen auf Basis zu Grunde liegenden Bestellung und einer empfangenen Rechnung erzeugt.
Diese kostenpflichtige Funktion muss explizit konfiguriert werden. Bei Fragen bitte kontaktieren Sie einen Mitarbeiter der A+W Software GmbH.

#### Fehlmengenkontrollpool
**Einkauf > Wareneingang > Fehlmengenkontrollpool**

In diesem Dialog wird eine Auflistung aller Positionen dargestellt, bei denen die Menge korrigiert wurde. Diese kostenpflichtige Funktion muss explizit konfiguriert werden.

##### Fehlmengenkontrollpool – Übersicht
**Einkauf > Wareneingang > Fehlmengenkontrollpool > Register Übersicht**

*[Image: Fehlmengenkontrollpool – Übersicht (Abb. E-47)]*

In diesem Register ist die Auflistung aller Positionen dargestellt, bei denen die Menge korrigiert wurde. Die Daten werden per openTrans-Schnittstelle übertragen.
Die Funktionsbeschreibung ist nicht der Bestandteil des Handbuches und muss beim Bedarf angefordert werden.

##### Fehlmengenkontrollpool – Details
**Einkauf > Wareneingang > Fehlmengenkontrollpool > Register Details**

*[Image: Fehlmengenkontrollpool – Details (Abb. E-48)]*

In diesem Register erhalten Sie Details-Informationen zu der ausgewählten Position.
Die Funktionsbeschreibung ist nicht Bestandteil des Handbuches und muss bei Bedarf angefordert werden.

#### Wareneingangsprotokoll
**Einkauf > Wareneingang > Protokoll**

*[Image: Wareneingangsprotokoll (Abb. E-49)]*

In diesem Dialog lassen Sie sich ein Protokoll über das Erzeugen und Buchen von Wareneingänge des aktuellen Tages anzeigen. Alle Vorgänge zum Wareneingang sind mit der Angabe des Datums und der Zeit protokolliert.

### Rechnungen und Gutschriften

Zu Bestellungen werden Rechnungen im Programm erfasst und gebucht. Je nach Konfiguration wird die interne Rechnung vom Programm an die Finanzbuchhaltung (FIBU) automatisch gesendet.

In diesem Abschnitt finden Sie folgende Informationen:
- "Rechnungskontrolle" auf Seite E-128
- "Lieferanten-Rechnung (automatisch)" auf Seite E-135
- "Lieferanten-Rechnung (manuell)" auf Seite E-138
- "Lieferanten-Rechnung (Sammelrechnung)” auf Seite E-139
- "Übertragene Rechnungen" auf Seite E-137
- "Rechnungen buchen" auf Seite E-140
- "Bestellungen abschließen" auf Seite E-141
- "Rechnungsprotokoll" auf Seite E-142
- "Lieferanten-Gutschrift" auf Seite E-142

Der Dialog **Gutschriften buchen** ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Gutschriften buchen" auf Seite D-354

#### Rechnungskontrolle
**Einkauf > Rechnungen > Rechnungskontrolle**

In diesem Dialog können Sie die Lieferanten-Rechnungen erfassen, kontrollieren, eine interne Rechnung erstellen und buchen. Die Nutzung der Rechnungskontrolle im Einkauf benötigt eine Konfiguration seitens A+W Software GmbH.

Für diesen Dialog gibt es folgende Ansichten:
- "Lieferanten-Rechnung – Bestellübersicht" auf Seite E-129
- "Lieferanten-Rechnung – Detailansicht" auf Seite E-132
- "Lieferanten-Rechnung – Positionsübersicht" auf Seite E-133
- "Lieferanten-Rechnung - Rabatte" auf Seite E-134

##### Lieferanten-Rechnung – Bestellübersicht
**Einkauf > Rechnungen > Rechnungskontrolle**

*[Image: Lieferanten-Rechnung – Bestellübersicht (Abb. E-50)]*

In diesem Dialog geben Sie die Bestellungsdaten zur Kontrolle ein. Anschließend können Sie zu der kontrollierten Bestellung die Lieferanten-Rechnung erzeugen und buchen.
- Mit `<F2>` wechseln Sie im Rumpfbereich in die Detailansicht.
- Mit `<F5>` im Feld **Nettobetrag** wechseln Sie in die Positions-Detailübersicht.
- Mit `<Strg> + <A>` wechseln Sie in die Rabattübersicht.
- Mit `<Enter>` wechseln Sie aus dem Rumpfbereich in den Fußbereich.

**Kopfbereich**
- **Belegnummer**: Interne Belegnummer der Lieferanten-Rechnung. (Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: kauf.exauftrnr)
- **Intern (Rechnung/Gutschrift)**: Angabe, ob eine Rechnung oder eine Gutschrift bereits erzeugt wurde.
- **Belegdatum**: Datum, an dem die Lieferanten-Rechnung erfasst wird. (Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat)
- **Buchungsdatum**: Datum, an dem die Lieferanten-Rechnung gebucht wird. (Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.bdat)
- **Haus**: Hausnummer. (Technische Info: numerisches Feld, DB-Feld: kauf.hausnr)
- **Lieferant**: Lieferantennummer. (Technische Info: numerisches Feld, DB-Feld: kauf.kunr)

**Bestellübersicht**
- **Bestellnr.**: Bestellnummer in der Lieferanten-Rechnung. (Technische Info:Pflichtfeld, alphanumerisches Feld, DB-Feld: kauf.auftrnr)
- **Bezugsvorgang**: Bezugsvorgang, für den die interne Rechnung erzeugt und gebucht wird (Wareneingang, Bestellung). (Technische Info: Toggle-Feld, DB-Feld: kaufp.refvorgang)
- **Subnr.**: Subnummer für Teillieferungen. (Technische Info: numerisches Feld, DB-Feld: kaufp.refsubnr)
- **Nettobetrag**: Nettobetrag der Lieferanten-Rechnung aus der Bestellung. (Technische Info: numerisches Feld, DB-Feld: kauf.nettototal)
- **Fremdnummer**: Fremdnummer, die im Dialog Wareneingang erfasst wurde. (Technische Info: numerisches Feld, DB-Feld: kauf.exaufnr)
- **Lieferschein**: Lieferanten-AB-Nr., die im Dialog Lieferavis erfasst wurde. (Technische Info: numerisches Feld, DB-Feld: kauf.lieferschein)

**Fußbereich**
- **Endbetrag netto**: Gesamt-Nettobetrag der Lieferanten-Rechnung. (Technische Info: numerisches Feld, DB-Feld: kauf.nettototal)
- **MwSt-Betrag**: Mehrwertsteuer-Betrag der Bestellungen. (Technische Info: numerische Felder)
- **Endbetrag brutto**: Gesamt-Bruttobetrag der Bestellungen. (Technische Info: numerisches Feld, DB-Feld: kauf.gesbrutto)
- **Stk. gesamt**: Gesamtstückzahl der Artikel.
- **Qm gesamt**: Gesamtfläche der Artikel.
- **Lfm gesamt**: Gesamtlänge der Artikel.

##### Lieferanten-Rechnung – Detailansicht
**Einkauf > Rechnungen > Rechnungskontrolle > Bestellung suchen > <F2>**

*[Image: Lieferanten-Rechnung – Detailansicht (Abb. E-51)]*

In diesen Ansichten werden die Lieferantendaten und Lieferdetails zur gewählten Bestellung angezeigt.

##### Lieferanten-Rechnung – Positionsübersicht
**Einkauf > Rechnungen > Rechnungskontrolle > Feld Nettobetrag > <F5>**

*[Image: Lieferanten-Rechnung – Positionsübersicht (Abb. E-52)]*

In diesen Ansichten werden die Positionsdetails zu der gewählten Bestellung angezeigt. Mit `<F2>` wechseln Sie zwischen den Registern.

##### Lieferanten-Rechnung – Rabatte
**Einkauf > Rechnungen > Rechnungskontrolle > Feld Nettobetrag > <Strg> + <A>**

*[Image: Lieferanten-Rechnung – Rabatte (Abb. E-53)]*

#### Lieferanten-Rechnung (automatisch)
**Einkauf > Rechnungen > Automatische Rechnungen**

*[Image: Lieferanten-Rechnung (automatisch) (Abb. E-54)]*

In diesem Dialog erstellen Sie die Rechnungen für Komplettlieferungen. Die Teillieferungen buchen Sie im Dialog **Lieferanten-Rechnung (manuell)**. Wenn zu einer Bestellung bereits ein Lieferplan existiert ist und ein Teil der Lieferung auf dem aktuellen Tag liegt, kann auch in diesem Dialog die Teilrechnung für diese Lieferung erzeugt und gebucht werden.

**Rumpfbereich**
- **Bestellung**: Bestellnummer.
- **Subnr**: Subnummer für Lieferungen.
- **Lieferplan**: Angabe ob der Lieferplan existiert.
- **Eingang**: Lieferung ist als Wareneingang bereits gebucht.
- **Rechnung**: Nummer der Lieferantenrechnung.
- **Belegdatum**: Datum, an dem der Lieferant die Rechnung erstellt hat.
- **Buch.datum**: Datum, an dem die Rechnung gebucht wurde.
- **Er.**: Auswahl, um die Buchung der Position zu erzeugen.

**Fußbereich**
Name des Lieferanten und Rechnungsbetrag der Lieferung.

#### Lieferanten-Rechnung (manuell)
**Einkauf > Rechnungen > Manuelle Rechnungen**

*[Image: Lieferanten-Rechnung (manuell) (Abb. E-56)]*

In diesem Dialog können Sie die Rechnungen bearbeiten und manuell buchen. Die Felder, Spalten und Register sind zum Dialog **Bestellerfassung** beschrieben: ⇨ "Bestellerfassung" auf Seite E-50

**Kopfbereich**
- **Rech-Nr.**: Rechnungsnummer der Lieferanten-Rechnung.

**Register Allgemein**
- **Berech.**: Stückzahl der Position, die mit der Rechnung fakturiert wird.

**Fußbereich**
- **Fakturasaldo**: Rechnungssumme inkl. Mehrwertsteuer.

#### Lieferanten-Rechnung (Sammelrechnung)
**Einkauf > Rechnungen > Sammelrechnungen**

*[Image: Lieferanten-Rechnung (Sammelrechnung) (Abb. E-57)]*

In diesem Dialog können Sie die Lieferantenrechnungen erstellen und buchen.
Um Sammelrechnung zu erstellen, müssen die entsprechenden Bestellungen bestimmte Voraussetzungen erfüllen:
- Der Lieferant akzeptiert die Teillieferungen.
- Die Bestellungen müssen im Feld **Rechnungsart** die Option **Sammelrechnung** eingestellt haben. ⇨ "Bestellpositionen – Eigenschaften" auf Seite E-80
- Die Bestellungen müssen im Wareneingang gebucht sein. ⇨ "Wareneingang (automatisch)" auf Seite E-114
Die Felder und der Fußbereich sind zum Dialog **Lieferanten-Rechnung** beschrieben: ⇨ "Lieferanten-Rechnung (automatisch)" auf Seite E-135

#### Rechnungen buchen
**Einkauf > Rechnungen > Rechnungen buchen**

*[Image: Rechnungen buchen (Abb. E-58)]*

In diesem Dialog können Sie bereits erzeugte aber noch nicht gebuchte Rechnungen nachträglich buchen.
- ⇨ "Rechnungskontrolle" auf Seite E-128
- ⇨ "Lieferanten-Rechnung (automatisch)" auf Seite E-135
- ⇨ "Lieferanten-Rechnung (manuell)" auf Seite E-138
- ⇨ "Lieferanten-Rechnung (Sammelrechnung)" auf Seite E-139
Die Felder sind im Part Verkauf beschrieben: ⇨ Verkauf, "Rechnungen buchen" auf Seite D-344

#### Bestellungen abschließen
**Einkauf > Wareneingang > Bestellungen abschließen**
**Einkauf > Rechnungen > Bestellungen abschließen**

*[Image: Bestellungen abschließen (Abb. E-59)]*

In diesem Dialog können Sie offene Bestellungen manuell abschließen. Mit `<F3>` schließen Sie manuell Bestellungen ab.

> **Bestellungen regulär abschließen**
> Bestellungen schließen Sie regulär ab, nachdem Sie die Bestellungen vom Lieferanten erhalten haben. Mit den beiden Dialogen **Wareneingang** und **Lieferanten-Rechnung** müssen Sie die Bestellungen buchen, damit das Programm die Bestellungen regulär abschließt.

Die Spalten sind an folgender Stelle beschrieben: ⇨ "Wareneingang (automatisch)" auf Seite E-114

#### Rechnungsprotokoll
**Einkauf > Rechnungen > Protokoll**

*[Image: Rechnungsprotokoll (Abb. E-60)]*

In diesem Dialog wird das Rechnungsprotokoll angezeigt. Alle Vorgänge zu den Rechnungen sind mit der Angabe des Datums und der Zeit vermerkt.

#### Lieferanten-Gutschrift
**Einkauf > Gutschriften > Gutschriften erfassen**

*[Image: Lieferanten-Gutschrift (Abb. E-61)]*

In diesem Dialog können Sie die vom Lieferanten übermittelten Gutschriften erfassen und buchen. Die Dialogregister und Felder sind zum Dialog **Bestellerfassung** beschrieben: ⇨ "Bestellerfassung" auf Seite E-50

**Kopfbereich**
- **Gutschr.**: Vorläufige Nummer der Gutschrift.
- **Bezug**: Vorgangsnummer, auf die Bezug genommen wird.

**Rumpfbereich**
- **Gutschr.**: Positionsmenge in der Artikelmengeneinheit, die für die Gutschrift verrechnet werden.

### Übersichten

Um den Bestand an Bestellvorgängen zu prüfen, stehen diverse Übersichten zur Verfügung.
- "Bestellinformation" auf Seite E-144
- "Übersicht zu Vorgängen" auf Seite E-145
- "Einkaufs-Recherche" auf Seite E-145

#### Bestellinformation
**Einkauf > Übersicht > Bestellinformation > Bestellung öffnen**
**Einkauf > Bestellverwaltung > Bestellung öffnen > Register Positionen > Register Allgemein > Spalte Menge > <Shift> + <F10>**

*[Image: Bestellinformation (Abb. E-62)]*

Zu allen Bestellungen können Sie sich die Vorgangs-Informationen anzeigen lassen, z. B. wann der Wareneingang gebucht wurde.
Der Dialog ist ausführlich zum Part Verkauf beschrieben: ⇨ Verkauf, "Auftragsinformation" auf Seite D-365

#### Übersicht zu Vorgängen
**Einkauf > Übersicht > Heute geplanter Wareneingang, Geplanter Wareneingang - verspätet, etc.**

*[Image: Beispiel für einen Übersicht-Dialog: Geplanter Wareneingang von-bis (Abb. E-63)]*

In diesen Dialogen werden die Übersichten zu folgenden Vorgängen angezeigt:
- Heute geplanter Wareneingang
- Geplanter Wareneingang – verspätet
- Geplanter Wareneingang von-bis
- Geliefert - nicht berechnet
- Berechnet – nicht gebucht
- Noch nicht übertragene Bestellungen

Diese Übersichten sind konfigurationsabhängig und müssen separat freigeschaltet werden.

#### Einkaufs-Recherche
**Einkauf > Recherche**

In diesem Dialog suchen Sie nach Vorgängen. Die Ergebnisse werden in einer Trefferliste angezeigt.
- "Einkaufs-Recherche - Suchmodus" auf Seite E-146
- "Einkaufs-Recherche - Übersicht" auf Seite E-147
- "Einkaufs-Recherche - Details" auf Seite E-149

##### Einkaufs-Recherche – Suchmodus
**Einkauf > Recherche**

*[Image: Einkaufs-Recherche - Suchmodus (Abb. E-64)]*

In diesem Dialog geben Sie die Kriterien für die Suche nach Vorgängen ein. Mit `<F3>` starten Sie die Suche.
- **Haus (Auftrag)**: Haus-/Mandantennummer der Aufträge.
- **Auftrag**: Auftragsnummer.
- **Kunde**: Kundennummer.
- **Kundenanfahrt**: Datum der Fahrt zum Kunden bei Direktanlieferung.
- **Objektnummer**: Nummer des Objekts, für das die Ware bestellt wurde.
- **Lieferant**: Lieferantennummer.
- **Haus (Bestellung)**: Haus-/Mandantennummer der Bestellungen.
- **Bestellung**: Bestellnummer.
- **Bestellt zum**: Datum, an dem die Bestellung eintreffen soll.
- **Artikel**: Artikelnummer.
- **Komplett**: Kennziffer für die Filterung nach dem Eingangsstatus (0=alle, 1=teilgeliefert, 2=komplett geliefert).
- **Storno**: Kennziffer für die Filterung nach dem Stornostatus (0=alle, 1=nicht storniert, 2=storniert).
- **AB-Nr. Lieferant**: Nummer der Auftragsbestätigung vom Lieferanten.
- **Lager**: Nummer der Lager, für das die Bestellung erfasst wurde.
- **Erfassungsdatum**: Datum der Bestellerfassung.
- **Erfasser**: Mitarbeiter, der die Bestellung erfasst hat.
- **Bemerkung**: Text der positionsbezogene Bemerkung.
- **Fremdnummer**: Auftragsnummer aus dem Verkauf.
- **Kostenstelle**: Kostenstelle, auf die die Bestellung erfasst wurde.
- **Breite, Höhe**: Maße der Position in Millimeter.

##### Einkaufs-Recherche – Übersicht
**Einkauf > Recherche > Filterkriterien eingeben > <F3>**

*[Image: Einkaufs-Recherche – Übersicht (Abb. E-65)]*

In diesem Dialog wird das Ergebnis der Suche angezeigt. Mit `<F5>` wechseln Sie in die Detailansicht.
Folgende Spalten werden angezeigt:
- **Anl. Datum**: Datum der Anlieferung.
- **Lieferant**: Lieferantennummer.
- **Bestellung**: Bestellnummer.
- **Pos**: Positionsnummer.
- **Artikel**: Artikelnummer.
- **Auftrag**: Auftragsnummer.
- **Kunde**: Kundennummer.
- **Kundenanf.**: Datum der geplanten Anlieferung des Auftrags.
- **Anzeigefelder für den Status**:
  - Leeres Feld = es liegt kein Status vor.
  - S = Storniert.
  - Stern * = Komplett geliefert.
  - F = Komplett fakturiert.

##### Einkaufs-Recherche – Details
**Einkauf > Recherche > Filterkriterien eingeben > <F3> > Eintrag markieren > <F5>**

*[Image: Einkaufs-Recherche – Details (Abb. E-66)]*

In diesem Dialog lassen Sie sich Details zu einer Position der Trefferliste anzeigen. Mit `<F2>` wechseln Sie zurück zur Trefferliste.
Die Felder sind zum Suchmodus und zur Trefferliste beschrieben.
Zusätzlich werden folgende Felder angezeigt:
- **Bruchgrund**: Bruchgrund im Klartext.
- **Erfassung**: Erfassungsdatum der auftragsbezogenen Bestellung.
- **Erfasser**: Mitarbeitername des Auftragserfassers.
- **Kunde**: Kundenname und Standort des Kunden.
- **Tour**: Nummer und Bezeichnung der Lieferroute.

## Partindex

### Index Einkauf

**A**
- **Anfrage**
  - Lieferant E-50
  - Suche E-21
- **Anschrift**
  - Bestellerfassung E-57
- **Auftrag**
  - Lieferadresse bearbeiten E-58
  - Reklamationsinformation E-64
  - Teilfaktura E-62
  - Versandinformation E-60
- **Auftragsinformationen**
  - Bestellerfassung E-87

**B**
- **Bestellart** E-94
  - Rechnung E-94
- **Bestellerfassung**
  - Anschrift E-57
  - Auftragsinformationen E-87
  - Bewertung E-91
  - Eigenschaften E-59, E-80
  - Modus E-47
  - Position E-71
  - Preise E-83
  - Reklamationsinformation E-64
  - Status E-47, E-88
  - Verschiedenes E-64
  - Zahlungsoption E-64
- **Bestellung**
  - Bestellart E-94
  - Lieferant, erzeugen für E-37
  - Position, erzeugen zur E-41
  - Position, Details zur E-43
  - Suche E-21
- **Bewertung**
  - Bestellerfassung E-91

**D**
- **Details**
  - Bestellung zur Position E-43
- **Dokumentenart**
  - Zuordnung E-95

**E**
- **Eigenschaften**
  - Bestellerfassung E-59, E-80
- **Einkauf**
  - Übersicht E-11
- **Erzeugen**
  - Bestellung für Lieferant E-37
  - Bestellung zur Position E-41

**F**
- **Formulardruck**
  - Formulardruck E-97

**K**
- **Kommission** E-72

**L**
- **Lieferadresse**
  - bearbeiten E-58
- **Lieferant**
  - Anfrage E-50
  - Bestellung erzeugen für E-37

**M**
- **Modus**
  - Bestellerfassung E-47

**P**
- **Position**
  - Auftrag, im E-55
  - Bestellerfassung E-71
  - Bestellung erzeugen zur E-41
  - Bestellung, Details zur E-43
- **Preise**
  - Bestellerfassung E-83

**R**
- **Recherche**
  - Einkauf, Details zum E-149
  - Einkauf, Übersicht zum E-147
- **Rechnung**
  - Bestellart E-94
  - Reklamationsinformation
    - Auftrag E-64
    - Bestellerfassung E-64

**S**
- **Status**
  - Bestellerfassung E-47, E-88
- **Summen**
  - Anfrage E-21
- **Suche**
  - Anfragen E-21
  - Bestellung E-21
  - Einkauf, Details zum E-149
  - Einkauf, Übersicht zum E-147
  - Einkauf, Vorgang zum E-146

**T**
- **Teilfaktura**
  - Auftrag E-62

**U**
- **Übersicht**
  - Einkauf E-11
  - Vorgänge E-145

**V**
- **Versandinformation**
  - Auftrag E-60
- **Verschiedenes**
  - Bestellerfassung E-64
- **Vorgang**
  - Details zum Einkauf E-149
  - Einkauf, Suche zum E-146
  - Einkauf, Übersicht zum E-147
- **Vorgänge**
  - Übersicht E-145

**Z**
- **Zahlungsoption**
  - Bestellerfassung E-64
- **Zuordnung**
  - Dokumentenart E-95
