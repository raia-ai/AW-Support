---
title: "DE_AWBusiness_Stammdaten_9_10"
source: "DE_AWBusiness_Stammdaten_9_10.pdf"
tags: ["A+W Business", "Stammdaten", "Master Data", "ERP", "Software Reference", "Finanzen", "Auftrag", "Firmendaten", "Kalkulation", "Produktion"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein Auszug aus dem Softwarereferenzhandbuch für A+W Business und beschreibt die Einrichtung von Stammdaten für die Module Auftrag, Finanzen und Firma. Es behandelt die Konfiguration von Dokumententypen, Kategorien, Steuern, Zahlungsbedingungen, Währungen und firmenspezifischen Parametern."
long_description: "Dieser Auszug aus dem A+W Business Softwarereferenzhandbuch bietet eine detaillierte Anleitung zur Konfiguration der Stammdaten. Der Inhalt ist in drei Hauptbereiche gegliedert: Auftrag, Finanzen und Firma. Im Bereich 'Auftrag' werden die verschiedenen Dokumententypen wie interner Auftrag, Kundenmaterial oder Reklamation definiert. Zudem wird die Einrichtung von Kategorien für statistische Auswertungen und die Festlegung von Gründen für Lieferterminverschiebungen erläutert. Der Abschnitt 'Finanzen' behandelt alle finanzrelevanten Stammdaten, einschließlich der Definition von Steuersätzen, Zahlungsbedingungen, Bonitätsstufen, Bankdaten, Währungen, Erlöskonten, Kostenarten und Kostenstellen. Es wird detailliert auf die Anbindung an Finanzbuchhaltungssysteme (FiBu) eingegangen. Der umfangreichste Teil 'Firma' beschreibt die globalen Einstellungen für das Unternehmen (Mandanten). Dies umfasst die Konfiguration der Firmendaten (Adresse, Mail-Server), steuerliche Einstellungen, FiBu-Schnittstellen, Dokumenten- und Preisberechnungsparameter, Lager-, Einkaufs- und EDI-Einstellungen, Archivierungsregeln, Produktions- und Versandeinstellungen sowie Parameter für die Kapazitätsplanung. Das Dokument dient als technisches Nachschlagewerk für Administratoren und Projektierer zur korrekten Einrichtung und Wartung des A+W Business Systems."
---

# Softwarereferenz

---
## Auftrag

- **Interner Auftrag:**
  Dieser Dokumententyp wird während der Bestellübergabe bei Einsatz des Moduls **Interne Aufträge** (mehrstufige Produktion) gesetzt.
  ⇨ Verkauf, "Bestellübergabe" auf Seite C-654

- **Kundenmaterial:**
  Dieser Dokumententyp muss manuell gesetzt werden. Dadurch werden alle Positionen automatisch auf die Beschaffungsart **Kundeneigenes Glas** gesetzt.

- **Lagerbestellung:**
  Dieser Dokumententyp wird automatisch bei der Generierung einer Lager-bestellung gesetzt. Dieses Kennzeichen kann aber auch manuell in einem Bestellauftrag gesetzt werden.
  ⇨ Verkauf, "Bestellübergabe" auf Seite C-654
  ⇨ Lagerwirtschaft, "Lagerbestellung" auf Seite G-220

- **Produktionsauftrag:**
  Dieser Dokumententyp wird verwendet, um den eigenen Lagerbestand aufzufüllen.
  ⇨ Fertigung, "Produktionsaufträge" auf Seite E-130

- **Rahmenauftrag:**
  Dieser Dokumententyp wird bei der Erstellung von Rahmenaufträgen verwendet.
  ⇨ "Objekte (Kunde, Lieferant)" auf Seite B-822

- **Reklamation:**
  Der Dokumententyp wird bei der Erfassung von Reklamationen gesetzt.

- **Serienauftrag:**
  Dieser Dokumententyp wird bei der Erstellung von Serienaufträgen verwendet.

- **Teillieferung:**
  Dieser Dokumententyp wird automatisch bei der Erstellung von Teilliefer-aufträgen gesetzt.

- **Versandauftrag:**
  Zurzeit nicht genutzt.

- **Wertmäßige Buchung:**
  Dieser Dokumententyp wird bei der Erfassung von Gutschriften verwendet. Mengenwerte wie Stück, Quadratmeter und Laufmeter werden dadurch nicht an die Statistik übergeben.
  ⇨ Verkauf, "Gutschrift (Dokumentenverwaltung)" auf Seite C-724

**Gesperrt**
Ein Dokumententyp kann für die Verwendung gesperrt werden, wenn er nicht mehr benötigt wird.
- Der Dokumententyp kann zugewiesen werden.
- Der Dokumententyp ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

> **Dokumententyp sperren**
> Die Sperrung eines Dokumententyps hat massive Auswirkungen auf die Auftragserfassung. Wenn Sie einen Dokumententyp sperren wollen, wenden Sie sich an die A+W Software GmbH. Sie vermeiden damit ungewollte Beeinträchtigungen der Arbeit mit A+W Business.

## Kategorien
*Stammdaten > Auftrag > Kategorien*

*Abb. B-565 Kategorien*

| Bezeichnung | Fremdschlüssel | Dokumententyp | Default-Kategorie | Gesperrt |
| :--- | :--- | :--- | :--- | :--- |
| Keine Rückmeldung | <k.A.> | Angebot | ☐ | ☐ |
| wg. Falschlieferung | 12 | Gutschrift | ☑ | ☐ |
| zu teuer | <k.A.> | Anfrage | ☐ | ☐ |
| Sonderangebot | A | Bestellung | ☐ | ☐ |
| Entscheidung auf Termin | A | Angebot | ☐ | ☐ |
| Test | <k.A.> | Auftrag | ☐ | ☐ |

In diesem Dialog richten Sie Kategorien ein, die bei der statistischen Auswertung von Dokumenten als Kriterium eingesetzt werden.

**Bezeichnung:** Namen der Kategorie.

**Fremdschlüssel:** Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.

**Dokumententyp:** Dokumententyp, bei dem die Kategorie gesetzt werden kann.

**Default-Kategorie:** Eine Kategorie kann standardmäßig im Dokument vergeben werden.
- Die Kategorie wird in dem entsprechenden Dokumententyp nicht standardmäßig zugewiesen.
- Die Kategorie wird standardmäßig bei der Erfassung des Dokuments zugewiesen. Sie kann im Dokument überschrieben werden.

**Gesperrt:** Eine Kategorie kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Kategorie kann zugewiesen werden.
- Die Kategorie ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

## Gründe Lieferterminverschiebung
*Stammdaten > Auftrag > Kategorien*

*Abb. B-566 Gründe für Lieferterminverschiebung*

| Bezeichnung | Gesperrt |
| :--- | :--- |
| Kundenwunsch | ☐ |

In diesem Dialog hinterlegen Sie Gründe für die Verschiebung eines Liefertermins.

Gründe für Lieferterminverschiebungen können in der Dokumentenerfassung, den Dokumentendaten, der Tourenliste und in der Kommissionierung eingetragen werden.

Der Grund muss zwingend eingetragen werden, wenn in den Stammdaten die Einstellung **Lieferterminverschiebung** aktiviert ist.
⇨ "Lieferterminverschiebung" auf Seite B-932

## Finanzen
*Stammdaten > Finanzen*

In diesem Programmbereich legen Sie die Daten fest, die für die Berechnung von Auftragspositionen und die Weiterleitung der Beträge an die Buchhaltung benötigt werden.

Im Menü Finanzen finden Sie folgende Einträge:
- "Steuer" auf Seite B-904
- "Zahlungsbedingungen" auf Seite B-906
- "Bonität" auf Seite B-907
- "Banken" auf Seite B-908
- "Währung" auf Seite B-909
- "Erlöskonten" auf Seite B-910
- "Kostenart" auf Seite B-913
- "Kostenstellen" auf Seite B-914
- "Zahlungswege" auf Seite B-915
- "Brasilianische Steuer" auf Seite B-916

### Steuer
*Stammdaten > Finanzen > Steuer*

*Abb. B-567 Steuer*

| Schlüssel | Steuersatz | Bemerkung | Erl. kto. Deb. | Erl.kto. Kred. | Fremdschlüssel | Gesperrt |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 19,0000 | 19 % Inland | 8201 | 9201 | 0 | ☐ |
| 2 | 7,5000 | 7,5% Inland erm. | 8202 | 9202 | 1 | ☐ |
| 3 | 1,6500 | 1,65% PIS tax | | | | ☐ |
| 4 | 7,6000 | 7,6% CONFIX tax | | | | ☐ |
| 5 | 5,0000 | 5% IPI tax | | | | ☐ |
| 6 | 10,0000 | 10% IPI tax | | | | ☐ |
| 7 | 15,0000 | 15% IPI tax | | | | ☐ |
| 8 | 0,0000 | 0% ICMS tax | | | | ☐ |
| 9 | 7,0000 | 7% ICMS tax | | | | ☐ |
| 10 | 12,0000 | 12% ICMS tax | | | | ☐ |
| 11 | 18,0000 | 18% ICMS tax | | | | ☐ |
| 12 | 12,0000 | 12% ISS service tax | | | | ☐ |
| 13 | 13,0000 | 13% ISS service tax | | | | ☐ |

In diesem Dialog legen Sie die (Mehrwert-)Steuersätze fest. In der Partnerverwaltung und in der Produktverwaltung weisen Sie den Partnern (Kunden) und den Produkten die jeweils gültigen Steuersätze zu.

In den Dokumenten kann diese Zuweisung überschrieben werden.
⇨ "Produktverwaltung - Preis/Zuschlag" auf Seite B-602
⇨ "Partnerverwaltung - Finanzen" auf Seite B-774

**Schlüssel:** Eindeutige Nummer (Identifikationsnummer).

**Steuersatz:** Prozentwert, der bei der Steuer berechnet werden soll. Bis zu 4 Nachkommastellen sind möglich.

**Bemerkung:** Bezeichnung des Steuersatzes, z. B. 19 % Inland.

**Erl.kto.Deb., Erl.kto.Kred.:** Nummern der Erlöskonten für Debitoren und Kreditoren, die in der Finanzbuchhaltung (FiBu) geführt werden. Die Steuerbeträge werden dann nicht auf die Erlöskonten der Warengruppe gebucht, sondern auf die hier hinterlegten Konten.
Wenn das Feld leer bleibt, wird der Steuerbetrag standardmäßig auf das Erlöskonto der zugehörigen Warengruppe gebucht.
⇨ Softwarereferenz, "Erlöskonten" auf Seite B-910

**Fremdschlüssel:** Der Fremdschlüssel wird an das Programm zur Finanzbuchhaltung übergeben. Der Eintrag ist von dem FiBu-Programm abhängig. Lesen Sie dazu die Benutzerdokumentation zu dem von Ihnen eingesetzten FiBu-Programm.

**Gesperrt:** Eine Steuer kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Steuer kann zugewiesen werden.
- Die Steuer ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Zahlungsbedingungen
*Stammdaten > Finanzen > Zahlungsbedingungen*

*Abb. B-568 Zahlungsbedingungen*

| Bezeichnung | Satz 1 | Tage 1 | Satz 2 | Tage 2 | Satz 3 | Tage 3 | Zahl.-ziel 1 | Zahl.-ziel 2 | Zahl.-ziel 3 | Zahl.-ziel 4 | Zahl.-ziel 5 | Mahn-tage | Fremd-schlüssel | Gesperrt |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 3% Skonto | 3,00 | 10 | | | | | 60 | 90 | 120 | 150 | 180 | 5 | | ☐ |
| 2% Skonto | 2,00 | 14 | 0,00 | 30 | | | | | | | | 33 | | ☐ |
| 14 Tage ohne Abzug | | | 0,00 | 14 | | | | | | | | 17 | | ☐ |
| 30 Tage ohne Abzug | | | 0,00 | 30 | | | | | | | | 30 | | ☐ |
| 7 Tage ohne Abzug | | | 0,00 | 7 | | | | | | | | 10 | | ☐ |
| 3% 7T,2% 10 T,1% 14 T, 30 Ta... | 3,00 | 7 | 2,00 | 10 | 1,00 | 14 | 30 | | | | | 0 | | ☐ |

In diesem Dialog tragen Sie die für Sie gängigen Zahlungsbedingungen ein, z. B. innerhalb von 10 Tage 2% Skonto.

Die Zahlungsbedingung weisen Sie den Kunden in der Kundenverwaltung im Register Finanzen zu. Im Auftragskopf werden die Zahlungsbedingungen aus den Kundendaten eingelesen und können überschrieben werden.
⇨ "Partnerverwaltung - Finanzen" auf Seite B-774

**Bezeichnung:** Namen der Zahlungsbedingung. Sie können bis zu 40 alphanumerische Zeichen verwenden. Diese Bezeichnung kann auf den Rechnungsformularen gedruckt werden.

**Satz 1, 2, 3:** Wert in Prozent, der zur Berechnung des abzugsfähigen Skonto-Betrags herangezogen wird. Der Skontosatz kann konstant oder zeitlich gestaffelt sein.

**Tage 1, 2, 3:** Anzahl der Tage, in denen der Skonto-Betrag abgezogen werden darf.

**Zahlungsziel 1-5:** Zeitraum, innerhalb dessen eine offene Rechnung beglichen werden soll.
Zur Berechnung des Zahlungsziels werden im Auftrag unterschiedliche Felder aus den Kundenstammdaten herangezogen.
⇨ "Fälligkeitsberechnung" auf Seite B-775

**Mahntage:** Anzahl der Tage, die ab dem Datum der Rechnungsstellung abgewartet werden, bevor eine Mahnung erstellt wird. Dieser Wert wird an Ihr Programm zur Finanzbuchhaltung (FiBu) übergeben.

**Fremdschlüssel:** Der Fremdschlüssel kann für die Kommunikation mit FiBu-Programmen verwendet werden.

**Gesperrt:** Eine Zahlungsbedingung kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Zahlungsbedingung kann zugewiesen werden.
- Die Zahlungsbedingung ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Bonität
*Stammdaten > Finanzen > Bonität*

*Abb. B-569 Bonität*

| Bezeichnung | Fremdschlüssel | Gesperrt |
| :--- | :--- | :--- |
| sehr gut | | ☐ |
| gut | | ☐ |
| durchschnittlich | | ☐ |
| keine | | ☐ |

In diesem Dialog tragen Sie die Stufen zur Klassifizierung der Bonität Ihrer Kunden ein, z. B. sehr gut, gut, schlecht.
Die Bonität weisen Sie den Kunden in der Kundenverwaltung im Register Finanzen zu.
⇨ "Partnerverwaltung - Finanzen" auf Seite B-774

**Bezeichnung:** Name der Bonität.

**Fremdschlüssel:** Der Fremdschlüssel kann für die Kommunikation mit einem FiBu-Programm verwendet werden.

**Gesperrt:** Eine Bonität kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Bonität kann zugewiesen werden.
- Die Bonität ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie einem Partner zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Banken
*Stammdaten > Finanzen > Banken*

*Abb. B-570 Banken*

| Name | Kurzbez. | BLZ | BIC | Land | PLZ | Sitz | Straße | Fremdschlüssel |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| SPK Wetzlar | | 515 500 15 | | DE | | Wetzlar | | |
| Volksbank Gießen | VoBaGi | 519 919 00 | | DE | | Linden | | |
| Berliner Bank | BB | 501 718 12 | | DE | | Berlin | | |
| Deutsche Bank | DeuBa | 500 100 00 | | DE | | Frankfurt | | |
| Spardabank Köln | | 588 745 87 | | DE | | Köln | | |
| Hanseatenbank | | 522 202 00 | | DE | | Hamburg | | |
| Hypothekenbank | | 585 155 15 | | DE | | München | | |
| Berliner Bank | | 501 718 13 | | DE | | Potsdam | | |
| Dresdner Bank | DreBa | 535 999 11 | | DE | | Dresden | | |
| Raiffeisenbank Mainz | | 595 654 92 | | DE | | Mainz | | |
| Schwabenbank | | 574 100 35 | | DE | | Stuttgart | | |
| Saarl. Bank | | 540 410 25 | | DE | | Saarbrücken | | |
| Postscheckamt Frankf... | | 519 555 00 | | DE | | Gießen | | |
| Nordhessische Volksb... | | 555 715 75 | | DE | | Kassel | | |
| Deutsche Bank AG Ba... | | 476 700 23 | | DE | | Bad Salzuflen | | |

In diesem Dialog tragen Sie die Daten der Banken Ihrer Geschäftspartner ein.
Die Bank weisen Sie den Partnern in der Partnerverwaltung im Register Finanzen zu. In der Partnerverwaltung können Sie die IBAN errechnen lassen, wenn mindestens folgende Daten für die Bank hinterlegt sind: Länderkennzeichen, BLZ und Kontonummer.
⇨ "Partnerverwaltung - Finanzen" auf Seite B-774

**Name:** Bankname.

**Kurzbez.:** Kurzbezeichnung, mit der die Bank in den Dialogen angezeigt wird.

**BLZ:** Bankleitzahl der Bank.

**BIC:** Bank Identifier Code. (SWIFT-)Code der Bank, der im internationalen Zahlungsverkehr genutzt wird.

**Land:** Kennzeichen des Landes, an dem die Bank ihren Sitz hat.

> **IBAN errechnen**
> In der Partnerverwaltung können Sie die IBAN errechnen lassen. Dazu ist es nötig, dass Sie bei den Einträgen der Bank die BLZ, BIC und das Länderkennzeichen angegeben haben.

**PLZ, Sitz, Straße:** Adressdaten der Bank.

**Fremdschlüssel:** Der Fremdschlüssel kann für die Kommunikation mit einem FiBu-Programm verwendet werden.

### Währung
*Stammdaten > Finanzen > Währung*

*Abb. B-571 Währungen*

| Erfassung in Landeswährung | Eigen-währung / Euro | Währungskurs / Faktor | Fremd-währung | Triangu-lation | Nkst. | Datum | Internat. Kennzeichen | Fremd-schl. | Gesperrt | Fremd-schl. 2 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Euro | ☑ | 0 | <k.A.> | | 2 | | DEM | Κ.Α. | | |
| Euro | ☑ | 1,95583 | DM | ☐ | 2 | 05.01.1999 | DEM | | ☐ | |
| Euro | ☑ | 1,1751 | US $ | ☐ | 2 | 15.11.2005 | USD | | ☐ | |
| Euro | ☑ | 1,662456 | SFR | ☐ | 2 | 05.01.1999 | SFR | | ☐ | |
| Euro | ☑ | 7 | FF | ☐ | 2 | 04.01.1999 | FF | | ☐ | |
| Euro | ☑ | 14 | OS | ☐ | 2 | 05.01.1999 | ÖS | | ☐ | |
| Euro | ☑ | 0,667329 | Brit.£ | ☐ | 2 | 04.01.1999 | BP | | | |
| Euro | ☑ | 970 | It. Lira | ☐ | 2 | 05.01.1999 | ITL | | ☐ | |
| Euro | ☑ | 1 | Euro | ☐ | 2 | 05.01.1999 | EUR | EURO | ☐ | |
| Euro | ☑ | 0,787564 | Ir.£ | ☐ | 2 | 05.01.1999 | IRP | | ☐ | |
| Euro | ☑ | 40,3399 | BF | ☐ | 2 | 05.01.1999 | BFR | | ☐ | |
| Euro | ☑ | 2,20371 | NGL | ☐ | 2 | 05.01.1999 | NGL | | ☐ | |
| Euro | ☑ | 166,386 | Pts. | ☐ | 2 | 05.01.1999 | PTS | | ☐ | |
| Euro | ☑ | 5,94573 | Finm. | ☐ | 2 | 04.01.1999 | FINM | | ☐ | |
| Euro | ☑ | 40,3399 | LF | ☐ | 2 | 06.01.1999 | LF | | ☐ | |
| Euro | ☑ | 200,842 | PEsc | ☐ | 2 | 06.01.1999 | PESC | | ☐ | |
| Euro | ☑ | 10,25 | BMI | | | 21.12.2011 | | | ☐ | |

In diesem Dialog hinterlegen Sie alle Währungen, die Sie für die Dokumentenerfassung benötigen. Die Währungen werden nur benötigt, wenn Sie mit dem Modul **Fremdwährung/Euro** arbeiten.

Die Währung wird einem Geschäftspartner in der Partnerverwaltung zugewiesen. Sie kann im Dokument überschrieben werden.
⇨ "Partnerverwaltung - Saldo" auf Seite B-779

**Erfassung in Landeswährung, Fremdwährung, Euro:** Das Anzeigefeld wird aus dem Eintrag in den Firmendaten gefüllt.
⇨ "Firmendaten - Steuer" auf Seite B-921

Die Beschreibung der nachfolgenden Felder bezieht sich auf die Einstellung **Default ist Landeswährung**.

**Eigenwährung:** Landeswährung.

**Euro:** Der Euro-Umrechnungskurs wird aus den Firmendaten gefüllt.

**Währungskurs/Faktor:** Währungskurs in Bezug auf die Eigenwährung.

**Fremdwährung:** Fremdwährung, in die umgerechnet werden soll.

**Triangulation:** Die Checkbox muss nur aktiviert werden, wenn die Berechnungen auf die Währung Euro umgestellt werden.
Der Euro bildet die Basis für Währungskalkulationen. Ein Wert in einer anderen Währung wird erst in Euro und dann zu seinem Gegenwert, beispielsweise in amerikanischen Dollar, umgerechnet. Diese Dreiecksmethode wird als Triangulation bezeichnet.
- Die Triangulation wird nicht zur Berechnung herangezogen.
- Die Triangulation wird eingesetzt, wenn eine dritte Währung benutzt wird.

**Nkst.:** Anzahl der möglichen Nachkommastellen der Fremdwährung.

**Datum:** Zeitpunkt, ab dem die Währung oder der Wechselkurs gültig ist.

**Fremdschl., Fremdschl. 2:** Die Fremdschlüssel können für die Kommunikation mit einem FiBu-Programm verwendet werden.

**Gesperrt:** Eine Währung kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Währung kann zugewiesen werden.
- Die Währung ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Erlöskonten
*Stammdaten > Finanzen > Erlöskonten*

*Abb. B-572 Erlöskonten*

**Identifikation**
- **Warengruppe:** 9** Kunstst., Vers. Beschl.
- **Produkt:**
- **Bemerkung:**

**Erlöskonten/Kostenstelle**
- **Rechnung:**
  - **Debitor:** 80900
  - **Kreditor:** 90900
- **Gutschrift:**
  - **Debitor:** 70900
  - **Kreditor:** 71900
- **Kostenstelle:**

**Zusatz**
- **ICMS:** 1 19% Inland
- **PIS:** 3 1,65% PIS tax
- **CONFIS:** 0
- **IPI:** 0
- **ISS:** 0
- **Fremdschlüssel:**
- **Geschäftsart:** Handelsgeschäft

**Übersicht**
| Bezeichnung | WGR | ICMS | PIS | CONFIS | IPI | ISS | Geschäftsart | Bemerkung ICMS | Bemerkung PIS | ... | Erlöskonto Debitor | Erlöskonto Kreditor |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 9** Kunstst., Vers., Beschl.... | | 2 | 4 | 0 | 0 | 0 | <K.A.> | 7,5% Inlan... | 7,6% C... | ... | 80900 | 90900 |
| 9** Kunstst., Vers. Beschl.... | | 1 | 3 | 0 | 0 | 0 | Handelsge... | 19% Inland | 1,65% | ... | 80900 | 90900 |
| 9** Kunstst., Vers., Beschl.... | | 1 | 4 | 0 | 0 | 0 | Streckenge... | 19% Inland | 7,6% C... | ... | 80900 | 90900 |
| 1** Isolierglas | | 0 | 0 | 0 | 0 | 0 | <K.A.> | | | ... | 80100 | 90100 |
| 1** Isolierglas | | 0 | 0 | 0 | 0 | 1 | <K.A.> | 19% In... | | ... | 80100 | 90100 |
| 1** Isolierglas | | 1 | | | | | <K.A.> | 19% In... | | ... | 80100 | 90100 |

In diesem Dialog hinterlegen Sie Ihre FiBu-Erlöskonten. Diese Erlöskonten werden von A+W Business bebucht.

**Menü Funktionen**
Über das Menü Funktionen können Sie Erlöskonten einer Geschäftsart in eine andere Geschäftsart kopieren bzw. bestehende Sätze überschreiben.
⇨ "Erlöskonten kopieren" auf Seite B-912

**Identifikation**
Für jede Kombination von Warengruppe und MwSt.-Kennzeichen richten Sie ein Erlöskonto ein, um so auch die Geschäfte mit Ihren ausländischen Kunden Mehraufwand zu verbuchen. Damit die Produktumsätze auf das richtige Konto gebucht werden, ordnen Sie den Warengruppen die Erlöskonten zu.

Außerdem können Sie auch für einzelne Produkte Erlöskonten einrichten. Dazu muss in den Firmendaten die Checkbox Erlöskonten pro Produkt markiert sein.
⇨ "Firmendaten - FiBu" auf Seite B-924

Wenn für eine Kombination aus Warengruppe und Mehrwertsteuer kein Konto eingerichtet ist, wird ein Dialog geöffnet, in dem Sie die gewünschte Kontonummer eintragen können.

> **Kopierfunktion nutzen**
> Sie können die notwendigen Erlöskonten über die Kopierfunktion einrichten. Damit erleichtern Sie sich die Arbeit.

**Steuer 1 bis 5:** Wenn Sie in Ihrem System mit mehreren Steuersätzen arbeiten, müssen Sie jeden Steuersatz zumindest einer Warenhauptgruppe zuweisen. Der zugehörige Steuersatz wird automatisch angezeigt.
⇨ "Steuer" auf Seite B-904

**Geschäftsart:** Geschäftsart, für die Sie das Erlöskonto einrichten.
Wenn Sie den Geschäftsarten keine unterschiedlichen Steuersätze zugewiesen haben, dann übernehmen Sie den Standardeintrag `<k.A.>`.
⇨ "Geschäftsart" auf Seite B-888

**Erlöskonten/Kostenstelle**
Debitor = Kunde, Kreditor = Lieferant

**Debitor, Kreditor:** Nummern der jeweiligen Erlöskonten.
- **Rechnung:** Nummern der Erlöskonten für die Rechnungen der Kundenaufträge bzw. Lieferantenbestellungen.
- **Gutschrift:** Nummern der Erlöskonten für Gutschriften auf Kundenaufträge bzw. Lieferantenbestellungen.
- **Kostenstelle:** Nummern der Kostenstelle des jeweiligen Debitors oder Kreditors aus Ihrem FiBu-Programm. Die Kostenstelle sind im Dialog Kostenstellen hinterlegt.

Wenn im Dialog Steuer kein anderes Erlöskonto für den Steuersatz eingetragen ist, wird auch die Mehrwertsteuer wird auf dieses Erlöskonto gebucht.

**Zusatz**

**Bemerkung:** Anmerkung zum Erlöskonto.

**Fremdschlüssel:** Der Fremdschlüssel kann für die Kommunikation mit einem FiBu-Programm verwendet werden.

**Übersicht**
In der Übersicht werden alle Erlöskonten aufgelistet, die für Warengruppen oder Produkte hinterlegt sind.

### Erlöskonten kopieren
*Stammdaten > Finanzen > Erlöskonten > Menü Funktionen > Erlöskonten kopieren*

*Abb. B-573 Erlöskonten kopieren*

In diesem Dialog übertragen Sie die Erlöskonten der Steuersätze und/oder Geschäftsarten auf andere Steuersätze oder Geschäftsarten.

**Von**
- **Steuer 1 – 5:** Steuer-Erlöskonten, die kopiert werden sollen.
- **Geschäftsart:** Geschäftsart, für die die Erlöskonten eingerichtet sind.

**Nach**
- **Steuer 1 – 5:** Steuer-Erlöskonten, auf die die Konten übertragen werden sollen.
- **Geschäftsart:** Geschäftsart, für die die Erlöskonten eingerichtet sind.

**Bereits vorhandene Datensätze überschreiben:** Standardmäßig werden vorhandene Datensätze nicht überschrieben.
- Vorhandene Datensätze werden nicht überschrieben. Wenn ein Datensatz vorhanden ist, wird eine entsprechende Meldung ausgegeben. Der Kopiervorgang wird abgebrochen.
- Vorhandene Datensätze werden mit den neuen Daten ohne Abfrage überschrieben.

### Kostenart
*Stammdaten > Finanzen > Kostenart*

*Abb. B-574 Kostenart*

| Bezeichnung | Fremdschlüssel | Gesperrt |
| :--- | :--- | :--- |
| 0234- Bürobedarf | 0234 | ☐ |
| 0357 Grundstoffe | 0357 | ☐ |
| 0378-Verbrauchsstoffe | 0378 | ☐ |

In diesem Dialog hinterlegen Sie Kostenarten. Diese Kostenarten dienen zur Auswertung in externen Programmen. z. B. über Excel.
Sie können Ihren Produkten eine Kostenart zuordnen. Diese wird in die Dokumente übernommen und kann dort überschrieben werden.
⇨ "Produktverwaltung - Preis/Zuschlag" auf Seite B-602

**Bezeichnung:** Namen der Kostenart.

**Fremdschlüssel:** Der Fremdschlüssel kann für die Kommunikation mit einem FiBu-Programm verwendet werden.

**Gesperrt:** Eine Kostenart kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Kostenart kann zugewiesen werden.
- Die Kostenart ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Kostenstellen
*Stammdaten > Finanzen > Kostenstellen*

*Abb. B-575 Kostenstellen*

| Bezeichnung | Fremdschlüssel | Gesperrt |
| :--- | :--- | :--- |
| 0001 Schleiferei | 0001 | ☐ |
| 0002 Zuschnitt | 0002 | ☐ |
| 0003-ISO Produktion | 0003 | ☐ |
| 0004 - Vertrieb | 0004 | ☐ |

In diesem Dialog hinterlegen Sie Kostenstellen. Diese Kostenstellen dienen zur Auswertung in externen Programmen, z. B. über Excel.
Sie können Ihren Produkten eine Kostenstelle zuordnen. Diese wird in die Dokumente übernommen und kann dort überschrieben werden.
⇨ "Produktverwaltung - Preis/Zuschlag" auf Seite B-602

**Bezeichnung:** Namen der Kostenstelle.

**Fremdschlüssel:** Der Fremdschlüssel kann für die Kommunikation mit einem FiBu-Programm verwendet werden.

**Gesperrt:** Eine Kostenstelle kann für die Verwendung gesperrt werden, wenn sie nicht mehr benötigt wird.
- Die Kostenstelle kann zugewiesen werden.
- Die Kostenstelle ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Zahlungswege
*Stammdaten > Finanzen > Zahlungswege*

*Abb. B-576 Zahlungswege*

| Bezeichnung | Fremdschlüssel | Fremdschlüssel 2 | Gesperrt |
| :--- | :--- | :--- | :--- |
| ÜBERWEISUNG | 01 | | ☐ |
| BAR | 02 | | ☐ |
| SCHECK | 03 | | ☐ |
| WECHSEL | 05 | | ☐ |
| RECHNUNG | 20 | | ☐ |

In diesem Dialog hinterlegen Sie die Zahlungsformen, die von Ihrer Firma akzeptiert werden, z. B. Scheck, Überweisung, bar. Sie dienen nur zur Information.
In der Partnerverwaltung können Sie dem Partner einen Zahlungsweg zuweisen.
⇨ "Partnerverwaltung - Finanzen" auf Seite B-774

**Bezeichnung:** Namen des Zahlungswegs.

**Fremdschlüssel, Fremdschlüssel 2:** Die Fremdschlüssel können für die Kommunikation mit einem FiBu-Programm verwendet werden.

**Gesperrt:** Ein Zahlungsweg kann für die Verwendung gesperrt werden, wenn er nicht mehr benötigt wird.
- Der Zahlungsweg kann zugewiesen werden.
- Der Zahlungsweg ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er zugewiesen ist, wird er jedoch weiterhin angezeigt.

### Brasilianische Steuer
*Stammdaten > Finanzen > Brasilianische Steuer*

In diesen Dialogen richten Sie die Steuersätze für die brasilianische Steuerberechnung ein. Dazu stehen folgende Dialoge zur Verfügung:
- TIPI Verwaltung
- ICMS-Modus
- CFOP-Code
- CST-Code
- Steuerzuordnung
- Geschäftsarten Workflow
- ICMS Reduktion
- Produkttypen

Die Dialoge sind nur freigeschaltet, wenn Sie in den Firmendaten die brasilianische Steuer aktiviert haben.

## Firma
*Stammdaten > Firma*

In diesem Programmbereich legen Sie Daten für Ihr Unternehmen an.
Im Menü **Firma** finden Sie folgende Einträge:
- "Firmendaten" auf Seite B-918
- "Portugiesische Zertifizierung" auf Seite B-1006
- "Mitarbeiter" auf Seite B-1008
- "Mitarbeitergruppen" auf Seite B-1014
- "Mitarbeiterrechte" auf Seite B-1015
- "Rechte kopieren" auf Seite B-1017
- "Statusverwaltung pro Mitarbeitergruppe" auf Seite B-1018
- "AV-Bereiche" auf Seite B-1019
- "AD-Bereiche" auf Seite B-1020
- "Vertreterprovision" auf Seite B-1022
- "Vertreter - Provisionssätze kopieren" auf Seite B-1024
- "Banken" auf Seite B-1025
- "Filialen" auf Seite B-1027
- "Buchungsperioden" auf Seite B-1028
- "Produktzuordnung Zuschläge" auf Seite B-1029
- "Formeln" auf Seite B-1031
- "Schnittstellen-Dienst" auf Seite B-1032
- "Customizing" auf Seite B-1042
- "Datencontainer" auf Seite B-1043

### Firmendaten
*Stammdaten > Firma > Firmendaten*

In diesem Dialog legen Sie die Grundeinstellungen fest, die als Standardvorgaben (Default) in die Dokumentenerfassung übernommen werden.
Bei Öffnen des Dialoges **Firmendaten** wird das Register **Mandant** angezeigt.
Mit dem Modul **Mandantenfähigkeit** können Sie mehrere Mandanten anlegen. Wenn Sie mit mehreren Mandanten arbeiten, wählen Sie den gewünschten Mandanten über das Register Tabelle aus. Die nachfolgend beschriebenen Register müssen für jeden Mandanten gesondert bearbeitet werden.
Mit den Navigationsschaltflächen können Sie von jedem Register aus in der Liste der Mandanten blättern, um sich die zugehörigen Daten anzeigen zu lassen.

Im Dialog **Firmendaten** finden Sie folgende Register:
- Firmendaten - Mandant
- Firmendaten - Steuer
- Firmendaten – FiBu
- Firmendaten - Dokumente
- Firmendaten - Parameter
- Firmendaten – Preisberechnung
- Firmendaten – Lager/EK/EDI
- Firmendaten – Archiv
- Firmendaten – Tagesabschluss
- Firmendaten – System
- Firmendaten - Kalkulation
- Firmendaten – Druck
- Firmendaten - Produktion
- Firmendaten - Versand
- Firmendaten – Kapa-Planung
- Firmendaten – Sonstiges

#### Firmendaten - Mandant
*Stammdaten > Firma > Firmendaten > Register Mandant*

*Abb. B-577 Firmendaten - Mandant*

In diesem Register legen Sie die Mandanten Ihres Unternehmens an und tragen die Adresse und Daten zur Kommunikation ein.
⇨ Tutorial 1, "Finanzbuchhaltung (FiBu)" auf Seite B-369
⇨ Tutorial 1, "Mitarbeiterverwaltung" auf Seite B-382

**Anschrift**
- **Nummer:** Mandanten-Nummer. Sie kann frei gewählt werden.
- **Firmennummer:** Firmennummer des Mandanten. Sie wird z. B. für die Gruppenstatistik und beim Im- und Export von Bestellungen und Aufträgen verwendet.
- **Matchcode:** Matchcode für den Mandanten (Pflichtfeld).
- **Name, Straße, Land/PLZ/Ort, Provinz:** Adressdaten, wie sie im Handelsregister angegeben sind.

**Kommunikation**
- **Telefon 1-4, Fax:** Kommunikationsnummern.
- **Mail:** E-Mail-Adresse, von der aus die eingehenden Sendungen an die jeweiligen Ansprechpartner weitergeleitet werden.

**Allgemeine Einstellungen zum Mailversand**
- **Server:** Name des Servers, über den der Mailversand gesteuert wird.
- **Port:** Nummer des Ports für den Mailversand.
- **Absender Adresse, Empfänger Adresse, Kopie an:** E-Mail-Adressen, die standardmäßig für verwendet werden sollen.
- **[E-Mail]:** Sendet eine Test-Mail, um die Einstellungen zu prüfen.
- **Authentifizierung:** Für die Datenübertragung kann eine Authentifizierung verwendet werden.
  - Die Sendebestätigung wird ohne Authentifizierung gesendet.
  - Für die Sendebestätigung ist Authentifizierung erforderlich. Die Felder zur Eingabe der Anmeldedaten werden freigeschaltet.
- **SSL Verschlüsselung verwenden:** Secure Sockets Layer (SSL); Verschlüsselungsprogramm zur sicheren Datenübertragung im Internet.
  - Die Sendebestätigung wird nicht verschlüsselt.
  - Die Sendebestätigung wird nach dem SSL-Protokoll verschlüsselt.
- **Benutzer, Passwort:** Anmeldedaten, mit denen der Sender sich authentifiziert.

#### Firmendaten - Steuer
*Stammdaten > Firma > Firmendaten > Register Steuer*

*Abb. B-578 Firmendaten - Steuer*

In diesem Register geben Sie die Daten des zuständigen Finanzamts ein und geben die Einstellungen zur Währung an.

**Finanzamt / Steuer**
- **Name, Straße, PLZ/Ort:** Adresse des Finanzamtes.
- **BLZ, Kontonummer:** Bankleitzahl und Kontonummer, auf die Sie die Steuern einzahlen.
- **Steuernummer, Betriebsnummer:** Ihre Steuer- und Betriebsnummer.
- **Ust-ID:** Steuernummer für die Umsatzsteuer-Vorauszahlungen.

**Währungseinstellungen**
Sie können wählen, in welcher Währung Sie standardmäßig in der Dokumentenerfassung arbeiten.
⇨ Tutorial 2, "Währungen" auf Seite B-457
⇨ "Währung" auf Seite B-909
⇨ "Firmendaten - Preisberechnung" auf Seite B-946

> **Arbeiten mit drei Währungen**
> Wenn Sie mit drei verschiedenen Währungen arbeiten, müssen Sie zusätzlich zur Währung auch bestimmen, ob die Währung aus dem Stammdatenpreisen berücksichtigt werden soll.
> ⇨ "Berücksichtigung der Währung der Stammdatenpreise" auf Seite B-953

- **Eigenwährung:** Ihre Landeswährung. Die Angabe bezieht sich auf die Einstellung im Bereich Währungsanzeige in Auftragserfassung.
  ⇨ "Währungsanzeige in Auftragserfassung" auf Seite B-923
- **Euro-Kurs:** Offizieller Euro-Umrechnungskurs in Bezug auf Ihre Landeswährung. Wenn als Landeswährung der Euro genutzt wird, tragen Sie den Wert 1 ein.
- **Defaultwährung:** Mit der Wahl der Option legen Sie fest, in welcher Währung Dokumente erfasst werden:
  - **Keine Währung:** Mit dieser Einstellung können Sie Aufträge nur in Ihrer Landeswährung erfassen, d. h., dass Sie in der Dokumentenerfassung keine Möglichkeit haben, von der Landes- zu einer Fremdwährung zu wechseln.
  - **Landeswährung:** Mit dieser Einstellung können Sie Aufträge in Landeswährung erfassen und können dabei in die Fremdwährung umschalten. Die Preisberechnung basiert dann auf den Preislisten in Eigenwährung und den hinterlegten Wechselkursen.
    ⇨ Verkauf, "Kopfdaten - Konditionen" auf Seite C-429
  - **Fremdwährung:** Mit dieser Einstellung können Sie Aufträge in Fremdwährung erfassen und dabei in die Landeswährung umschalten. Die Preisberechnung basiert dann auf den Preislisten in Fremdwährung. Wechselkurse werden in diesem Fall nicht hinterlegt.

> **Keine Wechselkurse bei Preisen in Fremdwährung**
> Wenn die Preise in Fremdwährung hinterlegt sind, dürfen keine Wechselkurse gepflegt werden.
> Standardmäßig werden die Preise automatisch in Euro umgerechnet. Ein zusätzlich hinterlegter Wechselkurs würde die Preise zweimal umrechnen.

**Währungsanzeige in Auftragserfassung**
Mit der Wahl der Option legen Sie fest, welche Währung in der Dokumentenverwaltung angezeigt wird:
- **Keine:** Bei dieser Einstellung wird in der Auftragserfassung automatisch die Währung verwendet, die im Feld **Eigenwährung** eingestellt wurde. Wenn Ihr Land nicht zu den Euro-Ländern gehört, muss die Option **Keine** aktiviert sein.
- **Euro:** Wählen Sie diese Einstellung, wenn Ihr Land nicht auf den Euro umgestellt hat, die Preislisten aber in Euro hinterlegt sind. Wenn Sie zudem im Feld **Eigenwährung** Ihre Landeswährung eingestellt haben, können Sie im Auftrag die Preise in Euro erfassen und in Ihrer Währung anzeigen lassen, z. B. in SFR.
- **Altwährung:** Wenn Sie auf den Euro umgestellt haben, so müssen Sie im Feld **Eigenwährung** der Eintrag **Euro** auswählen und der Optionsschalter **Altwährung** aktivieren. Zusätzlich wählen Sie Ihre alte Eigenwährung aus.

**Zugangsdaten Umsatzsteuerberechnung Avalara WebService**
A+W Business kann alle relevanten Informationen eines Dokumentes an den Avalara WebService übergeben und erhält die Steuersätze, die Steuerbasisbeträge und die berechnete Steuer zurück.
Für die korrekte Steuerberechnung müssen sogenannte Steuercodes zu jeder Warengruppe eingetragen werden.
⇨ "WGR" auf Seite B-567

Sie festlegen, wie sich das System am Avalara Webservice anmelden soll. Mit der Wahl der Option werden die entsprechenden Eingabefelder freigeschaltet:
- Benutzername / Passwort
- Kontonummer / Lizenzschlüssel

> **Übergabe einrichten**
> Der Aufruf des Avalara WebServices wird über ein Customizing für die Steuerberechnung durchgeführt. Dazu ist eine Formel in der Customizing-Verwaltung dem Programmpunkt 52-Steuerberechnung zuzuordnen. Wenden Sie sich an Ihren Projektierer bei der A+W Software GmbH, wenn Sie diese Funktionalität nutzen wollen.

#### Firmendaten – FiBu
*Stammdaten > Firma > Firmendaten > Register FiBu*

*Abb. B-579 Firmendaten – FiBu*

In diesem Register geben Sie an, mit welchem Programm zur Finanzbuchhaltung (FiBu) Sie arbeiten.
Die Angaben sind abhängig vom jeweiligen FiBu-Programm. Die erforderlichen Daten werden bei der Installation durch die A+W Software GmbH eingegeben.
Nach Auswahl einer Schnittstelle werden folgende Informationen zur Konfiguration der Schnittstelle angezeigt:
- Unterstützte Dokumentenarten, z. B. Auftrag, Gutschrift, Bestellung.
- Anzahl und Name der Schnittstellendatei für Dokumente und Kunden-Stammdaten.
- Anzahl und Name der Schnittstellendatei für den OP-Import.
- Benötigte Fremdschlüssel, z. B. Steuer, Zahlungsbedingung, Währung.
- Weitere notwendige Einstellungen, z. B. Buchungskreis, FiBu-Mandant.
⇨ Tutorial 1, "Finanzbuchhaltung (FiBu)" auf Seite B-369

**Finanzbuchhaltung**
- **Export:** Über die ausgewählte Schnittstelle werden Rechnungen und Stammdaten exportiert.
- **Import:** Über die ausgewählte Schnittstelle werden offene Posten importiert.
  ⇨ Tutorial 1, "Kreditlimit-Analyse" auf Seite B-94
- **Konto / Fremdschlüssel:** Nummer des Kontos oder Fremdschlüssels, über die die Daten identifiziert werden.
- **FiBu-Mandant:** FiBu-Nummer des Mandanten, für den diese Einstellungen gelten.
- **Buchungskreis:** Wenn Sie im eingesetzten FiBu-Programm Buchungskreise für Ihre Mandanten definiert haben, können Sie die FiBu der einzelnen Mandanten gesondert pflegen. Dazu legen Sie in A+W Business die entsprechenden Buchungskreise an. Falls Sie mit verschiedenen Buchungskreisen arbeiten, tragen Sie den Buchungskreis ein, der für diesen Mandanten gilt.

**Pfad und Dateiname**
Die Einstellungen in diesem Bereich werden bei der Installation eingerichtet und müssen in der Regel nicht geändert werden.
- **Export Dokumente:** Pfad und Namen der Datei, in die Bewegungsdaten exportiert werden. Beachten Sie das Beispiel für die Schreibweise.
- **Export Markpartner:** Pfad und Namen der Datei, in die Kunden- und Lieferantenstammdaten exportiert werden. Beachten Sie das Beispiel für die Schreibweise.
- **Batchfile:** Pfad und Namen der Stapeldatei (Batch), die nach der Übergabe gestartet werden soll. Wenn Sie eine Datei eingetragen haben, die nicht ausgeführt werden kann, wird eine Fehlermeldung angezeigt.
- **Import OP-Rückmeldung:** Pfad und Name der OP-Datei, die vom Batchfile verarbeitet wird.

**Optionen**
Die Angaben in diesem Bereich sind abhängig von dem Programm zur Finanzbuchhaltung, mit dem A+W Business über die Schnittstelle kommuniziert. Die erforderlichen Daten werden bei der Installation durch die A+W Software GmbH eingegeben.

- **Standardausgabe erstellen:** Die Exportdatei für die FiBu wird der Schnittstelle entsprechend erstellt. Daneben besteht die Möglichkeit, eine Standardausgabe erzeugen zu lassen.
  - Nur die FiBu-spezifische Exportdatei wird erstellt.
  - Neben der FiBu-spezifischen Exportdatei wird eine Datei im AWStandard2-Format erstellt.

- **Kostenrechnung aktiv:** Für die Übergabe können Kostenrechnungssätze geschrieben werden. Dazu muss das FiBu-Programm die Kostenrechnung unterstützen. Neben der Kosten- und Aufschlagskalkulation in A+W Business können für Ihre FiBu auch Kostenrechnungssätze geschrieben werden, anhand derer Sie Ihre Kalkulation prüfen und überarbeiten können.
  - Kostenrechnungssätze werden nicht geschrieben.
  - Wenn Ihre FiBu die Kostenrechnung unterstützt, werden spezifische Kostenrechnungssätze geschrieben.
    ⇨ Tutorial 2, "Kosten- und Aufschlagskalkulation" auf Seite B-541

- **Update OP-Saldo nach Übergabe:** In der Auftragserfassung kann das Kreditlimit eines Kunden angezeigt werden. Damit der Saldo aktualisiert wird, müssen die offenen Posten zurückgemeldet und in A+W Business aktualisiert werden.
  - Die Übergabe der Rechnung an die FiBu bewirkt kein Update des Kundenkontos.
  - Der Saldo des Kundenkontos wird um den Rechnungsbetrag erhöht, sobald die Rechnung an die FiBu übergeben wurde.

- **Einzel-OP-Rückmeldung:** Die offenen Posten können einzeln oder kumuliert pro Kunde zurückgemeldet werden.
  - Standardmäßig werden offene Posten kumuliert zurückgemeldet.
  - Offene Posten werden pro Rechnung zurückgemeldet.

- **Erlöskonten pro Produkt:** Die Erlöskonten können für Produkte und WGR eingerichtet und bebucht werden.
  - Erlöskonten werden nur für WGR bebucht.
  - Erköskonten können für Produkte und WGR bebucht werden.
    ⇨ "Erlöskonten" auf Seite B-910

> **Voraussetzungen**
> Für die folgenden drei Funktionen muss einer der Mandanten als FiBu-Hauptmandant gekennzeichnet sein. Zusätzlich müssen die Funktionen bei allen Mandanten aktiviert werden.

- **Kunden zusätzlich im FiBu-Hauptmandanten anlegen/aktualisieren:** Nur Syska-FiBu. Wenn Kunden eines Mandanten an die FiBu übergeben werden, kann festgelegt werden, ob diese Kunden als Kunden des Hauptmandanten angelegt werden.
  - Die Kunden des aktuellen Mandanten werden in der FiBu nicht als Kunden des Hauptmandanten angelegt.
  - Die Kunden eines Mandanten, der nicht der FiBu-Hauptmandant ist, werden als Kunden desjenigen Mandanten angelegt oder aktualisiert, der dem FiBu-Mandanten des Kunden entspricht.

- **Dateien im Unicode-Format lesen und schreiben:** Die Einstellung ist abhängig von dem System, mit dem die Daten ausgetauscht werden.
  - Die Dateien werden in dem Code gelesen und geschrieben, in dem sie angelegt wurden.
  - Die Dateien werden im Unicode gelesen und geschrieben.

- **Neue Kundennummer gegen FiBu prüfen:** Nur Syska-FiBu. Beim Anlegen neuer Kundendaten kann geprüft werden, ob die gewählte Kundennummer in der FiBu bereits vorhanden ist.
  - Die Nummer des neuen Kunden wird nicht geprüft.
  - Beim Abgleich der Stammdaten in der Syska-FiBu wird geprüft, ob die Nummer des neuen Kunden bereits vorhanden ist. Wenn die Kundennummer existiert, wird eine Fehlermeldung angezeigt. Sie müssen für den neuen Kunden dann eine andere Kundennummer eintragen.

- **FiBu-Hauptmandant:** Nur Syska-FiBu. Wenn Sie mit mehreren Mandanten arbeiten, muss einer von ihnen der FiBu als Hauptmandant angezeigt werden.
  - Der Mandant, dessen Einstellungen Sie aktuell bearbeiten, ist nicht Hauptmandant für die FiBu.
  - Der aktuelle Mandant ist in der FiBu der Hauptmandant.

- **Kundenkonto statt Kundenummer übergeben:** Standardmäßig wird die Kundennummer als Kontonummer herangezogen. Statt der Kundennummer kann in den Stammdaten eines Kunden jedoch auch die Debitorennummer eingetragen werden.
  - Die Kundennummer wird an die FiBu übergeben.
  - Die Kontonummer wird an die FiBu übergeben. Diese Kontonummer muss in den Kundendaten eingetragen sein. Diese Einstellung übersteuert die Einstellung in den Kundenstammdaten.
    ⇨ "Hauptkto." auf Seite B-777

**FiBu-Datenbank**
Diese Felder müssen nur gefüllt werden, wenn Sie mit einer SQL-FiBu arbeiten, in die direkt exportiert werden kann.
- **Server:** Name des Servers, auf dem die FiBu-Datenbank liegt.
- **Datenbankname:** Name der FiBu-Datenbank.
- **Login:** Benutzername, mit dem sich A+W Business an der FiBu-Datenbank anmeldet.
- **Passwort:** Passwort, mit dem sich A+W Business an der FiBu-Datenbank anmeldet.

**Optionen für Offene Posten Rückmeldung**
- **Sicherungsdatei anlegen, Pfad:** Das Feld ist nur freigeschaltet, wenn OP-Rückmeldungen importiert werden. Sie können dann eine zusätzliche Sicherungsdatei speichern und festlegen, wie viele Tage diese gespeichert bleibt.
  - Zur OP-Rückmeldedatei wird keine Sicherungsdatei gespeichert.
  - OP-Rückmeldungen sollen als Sicherung (mit Zeitstempel) zusätzlich an einem anderen Ort gespeichert werden. Die Felder zur Auswahl des Verzeichnisses und für die Vorhaltetage werden freigeschaltet.

- **Vorhaltetage für Sicherungsdateien:** Das Feld wird nur freigeschaltet, wenn eine Sicherungsdatei gespeichert werden soll. Sie können eintragen, wie viele Tage diese Datei nicht überschrieben werden darf.

#### Firmendaten – Dokumente
*Stammdaten > Firma > Firmendaten > Register Dokumente*

*Abb. B-580 Firmendaten - Dokumente*

In diesem Register legen Optionen für die Datenausgabe der Dokumente fest.

**Auswahl Modell-Katalog**
- **Modell-Katalog:** Standardmäßig arbeitet A+W Business mit dem Modell-Katalog der A+W Software GmbH. Sie können für Ihre unterschiedlichen Mandaten unterschiedliche Kataloge auswählen.
  ⇨ Verkauf, "Modelle" auf Seite C-71

**Sperrkennzeichen**
Sperrkennzeichen setzen Sie ein, um Dokumente aus bestimmten Abläufen in der automatischen Verarbeitung auszuschließen.
⇨ Tutorial 2, "Sperrkennzeichen" auf Seite B-426

> **Voraussetzung**
> Sperrkennzeichen müssen im Dialog Sperrkennzeichen angelegt sein, damit sie in den Feldern ausgewählt werden können.
> ⇨ "Sperrkennzeichen" auf Seite B-898

- **Reklamation:** Sperrkennzeichen für Reklamationen. Es kann in den einzelnen Dokumenten überschrieben werden.
- **Teillieferung:** Sperrkennzeichen für Teillieferungen. Es kann im einzelnen Dokument überschrieben werden.
> **Einstellung für Kunden aktivieren**
> Soll ein Kunde Teillieferung ohne Teilfakturierung erhalten können, so definieren Sie dies in den Kundenstammdaten mit den Checkboxen **Teillieferung** und **Teilfakturierung**.
> ⇨ "Partnerverwaltung - Auftrag" auf Seite B-764

**Fax / Mail - Optionen**
> **Voraussetzung**
> In der Partnerverwaltung müssen eine Fax-Nummer und eine E-Mail-Adresse hinterlegt und der Fax- und E-Mail-Versand aktiviert sein.
> ⇨ "Partnerverwaltung - Auftrag" auf Seite B-764

- **Faxversand pro Dokument:** Dokumente können per Fax versendet werden.
  - Die Dokumente werden gesammelt an die Marktpartner gesendet.
  - Standardmäßig werden die Dokumente einzeln an die Marktpartner gesendet. Um Engpässe beim Faxversand zu vermeiden, sollten Sie diese Einstellung beibehalten.

- **Mailversand pro Dokument:** Dokumente können per E-Mail in verschiedenen Formaten versendet werden.
  - Die Dokumente werden gesammelt per E-Mail an die Marktpartner verschickt.
  - Die Dokumente werden einzeln per E-Mail an die Marktpartner verschickt. Um Engpässe beim Mailversand zu vermeiden, sollten Sie diese Standardeinstellung beibehalten.
  Bedenken Sie beim RTF-Versand, dass die Modellskizzen und andere Grafiken nicht korrekt dargestellt werden können.

**Zwingende Modellvermaßung**
> **Berechnungsfehler vermeiden**
> Wenn Sie die Berücksichtigung von Kantenbearbeitung nach exakten Laufmetern im Register Parameter aktiviert haben, sollten Sie die Zwingende Modellvermaßung bei allen Dokumenten aktivieren, um Preisberechnungsfehler zu vermeiden.
> ⇨ "Kantenbearbeitung mit exakten Lfm berechnen" auf Seite B-936

- **Angebot, Auftrag, Bestellung:** Zu Modellen werden in den Dokumenten Maße angegeben werden. Die Angaben von Maßen sollten für den Auftrag und die Bestellung zwingend sein, im Angebot kann ggf. darauf verzichtet werden.
  - Bei der Erfassung des Dokuments müssen für Modelle keine Maße angegeben werden. Während des Kopierens von Angebot nach Auftrag werden die Vermaßungen überprüft und Sie werden gegebenenfalls aufgefordert, die fehlenden Maße einzugeben.
  - In den Dokumenten (Angebot, Auftrag, Bestellung) müssen die Maße eingegeben werden. Für Auftrag und Bestellung sollten Sie die standardmäßige Aktivierung der Checkboxen beibehalten (notwendig für die Produktion).

**Mischkalkulationsfaktoren**
Wenn Sie mit Mischkalkulationen arbeiten, können Sie die Faktoren hinterlegen, mit denen die Preise berechnet werden.
⇨ Tutorial 2, "Mischkalkulation" auf Seite B-535
⇨ "Positionen - Zusatz" auf Seite C-504
- **2-fach-ISO:** Die Faktoren für 2-fach-ISO sind frei wählbar, z. B. 0,5 / 0,5.
- **3-fach-ISO:** Die Faktoren für 3-fach-ISO sind frei wählbar, z. B. 0,5 / 0,8 / 0,5.

**Nummernvergabe pro Seite bei**
- **Lieferscheindruck, Rechnungsdruck:** In bestimmten Ländern ist zwingend vorgeschrieben, jeder Seite eines Lieferscheins und einer Rechnung eine eigene Nummer zuzuweisen.
  - Standardmäßig erhalten der Lieferschein bzw. die Rechnung eine Nummer pro Dokument.
  - Jede Seite des Lieferscheins bzw. der Rechnung erhält beim Druck eine eigene Nummer.

**Gutschrift-Rechnungsnummer**
Die Nummernkreise werden für jede Dokumentenart getrennt eingerichtet.
- **Nummer Gutschrift = Nummer Dokument:** Standardmäßig sind Gutschriften eigenständige Dokumente mit einem eigenständigen Nummernkreis.
  - Für den Druck der Gutschriften wird eine Nummer aus dem Nummernkreis der Rechnungen eingesetzt.
  - Beim Druck der Gutschrift wird eine Nummer aus dem Nummernkreis der Gutschriften eingesetzt.
    ⇨ Tutorial 2, "Nummernkreise festlegen" auf Seite B-438
    ⇨ "Nummernkreise" auf Seite B-891

**Lieferterminverschiebung**
Sie können für eine Lieferterminverschiebungen von Aufträgen zwingend eine Begründung vorschreiben. Die Eingabe eines Grundes wird in folgenden Fällen gefordert:
- Auftragserfassung, sofern der Auftrag nicht neu erfasst wird
- Dokumentendaten
- Tourenliste
- Kommissionierung

In der manuellen Anmerkung der Auftragshistorie sind das alte und neue Lieferdatum und der eingegebene Grund ersichtlich. Wenn mehr als ein Auftrag geändert wird, muss der Änderungsgrund pro Auftrag eingegeben werden. Das Feld wird mit dem vorher eingegeben Wert gefüllt und kann als Grund übernommen werden.

Wenn der Auftrag durch das Produktionssystem bei der Einlastung verschoben wird, ist automatisch mit der Grund **Lieferterminbestimmung mit A+W Production** eingetragen. Wenn die Lieferterminverschiebung durch eine Umlastung im Produktionssystem erfolgt, wird der dort eingegebene Kommentar als Text verwendet.

- **Eintrag in Historie mit Kommentar ab Status:** Bei einer manuellen Verschiebung des Liefertermins kann die Angabe eines Grundes zwingend vorgeschrieben werden.
  - Die Verschiebung des Liefertermins muss nicht in der Historie begründet werden.
  - In der Historie wird ein Eintrag erstellt, wenn der Liefertermin ab dem eingestellten Status verschoben wurde. Die Eingabe des Grundes ist zwingend notwendig und kann nicht abgebrochen werden. Die Einstellung gilt für folgende Programmbereiche: Bestellübergabe, Dokumentendaten, AB-Lieferant, Wareneingang und in der Kommissionierung.
  Das Feld für die Auswahl des Status wird freigeschaltet.

**Modelle drehen**
- **Modelle in Bearbeitungsdialog drehbar:** Modelle mit Modellnummern kleiner 137 können im Bearbeitungsdialog gedreht werden. Ausgeschlossen sind dabei die Modell-Nummern 0, 24, 98, 99, 60, 61 und 81.
  - Die Modell können nicht gedreht werden.
  - Die Modelle können gedreht werden: Dabei stehen als Drehwinkel 90, 180 oder 270 Grad zur Verfügung. Der Ausdruck gibt die gedrehte Form wieder.

**GGA Datenquelle**
Das Feld betrifft das Modul AWDoor.

**ODBC DSN:** Namen der Datenbankverbindung, die unter Windows konfiguriert wurde.

**Mindestpreisunterschreitung**
- **Passwort:** Passwort, wenn Sie die zufällige Unterschreitung von Mindestpreisen verhindern wollen. Es wird abgefragt, sobald in der Auftragserfassung der hinterlegte Mindestpreis unterschritten wird. Über die Weitergabe des Passworts können Sie steuern, welche Mitarbeiter befugt sind, solche individuellen Preise zu vereinbaren.

**Objektverwaltung**
- **Aktive Objektverwaltung:** Für die Arbeit mit der Objektverwaltung stehen unterschiedliche Einstellungen zur Verfügung:
  - Keine
  - Abrechnungsverwaltung (kundenspezifische Einstellung)
  - Abrechnungsverwaltung mit zugeordneten Aufträgen
  - Erweiterte Objektverwaltung
  - Standard-Objektverwaltung
  - Standard-Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen
  Die Unterschiede der Einstellungen sind ausführlich im Tutorial beschrieben.
  ⇨ Tutorial 1, "Objekte" auf Seite B-123
  ⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-495

**Produktkennzeichnung**
Für die CEKAL-Klassifizierung oder Gütetexte können Sie den jeweils zutreffenden Modus einstellen. Eine gültige Lizenz ist für die jeweilige Methode erforderlich. Falls keine Produktkennzeichnung aktiviert ist, wird bei der Auswahl des jeweiligen Dialoges ein Hinweis angezeigt.

- **Aktive Kennzeichnung:** Produktkennzeichen:
  - **Keine:** Mit dieser Auswahl wird die Produktkennzeichnung nicht geprüft.
  - **CEKAL-Klassifizierung:** Mit dieser Auswahl werden die Rahmentexte nach der CEKAL-Klassifizierung gesetzt.
  - **Gütekennzeichen:** Mit dieser Auswahl werden die Restriktionen aus dem Dialog **Gütetext** berücksichtigt.
    ⇨ "Gütetext" auf Seite B-582

**Dateianhänge**
Dateien können in der Partner- und in der Dokumentenverwaltung angehängt werden.
- **Pfad:** Pfad, in dem die Dateianhänge abgelegt werden sollen. Im Ablageverzeichnis wird automatisch ein Ordner pro Kunde oder Auftrag erstellt, in dem die Anhänge gespeichert werden. Beachten Sie, dass das Ablageverzeichnis auf einem zentralen Rechner zur Verfügung steht, auf den Ihre Mitarbeiter Zugriff haben.

**Leistungserklärung**
- **Versand von Leistungserklärungen:** Sie können festlegen, ob Leistungserklärungen gesendet werden sollen.
  - Leistungserklärungen werden nicht automatisch erstellt und gesendet.
  - Leistungserklärungen werden für die zugewiesenen Partner und Produkte gesendet. Das Feld für die Auswahl der Standard-Leistungserklärung wird freigeschaltet.

- **Standard-Leistungserklärung:** Sie können eine Leistungserklärung (LE) angeben, die standardmäßig gesendet werden soll, wenn im Auftrag keine spezifische LE zugeordnet ist.
- **[Ordner]:** Öffnet den Dialog **Leistungserklärung Verwaltung**, in dem Sie die Leistungserklärung (LE) registrieren können.
  ⇨ "Leistungserklärung Verwaltung" auf Seite B-584
- **[Lupe]:** Öffnet den Dialog **Leistungserklärung Suche**, in dem Sie die Standard-Leistungserklärung auswählen können.
- **Größenbeschränkung beim Mailversand ... MB:** Für den Versand der Leistungserklärungen können Sie eine Höchstgrenze in MegaByte angeben. Bei Dokumenten, die diesen Wert übersteigen, wird die E-Mail in mehrere Teile gesplittet.

- **A+W SLT-Schnittstelle verwenden:** Für die Datenübertragen in Modul B2B kann eine A+W-eigene Schnittstelle installiert werden.
  - Die A+W SLT-Schnittstelle wird nicht verwendet.
  - Die A+W SLT-Schnittstelle wird verwendet. Mit dieser Einstellung können Sie angeben, wo die Schnittstellendatei abgelegt ist, wenn ein abweichender Installationspfad verwendet wurde.

- **Abweichender Installationspfad:** Angabe, ob ein abweichender Installationspfad für die Schnittstellendatei A+WSLT.exe verwendet wurde. Das Feld ist nur freigeschaltet, wenn die A+W SLT-Schnittstelle aktiviert ist.
  - Die Schnittstellendatei ist im Standard-Installationspfad installiert.
  - Die Schnittstellendatei ist in einem abweichenden Installationspfad installiert. Dazu müssen Sie den Pfad angeben.
- **(Pfad):** Angabe des Installationsverzeichnisses für die Schnittstellendatei A+WSLT.exe.

**CEKAL-Parameter**
Diese Einstellungen werden nur in Frankreich verwendet.
- **Default-Text:** Diese Felder betreffen das Modul CEKAL. Für die Zuordnung eines allgemeinen Standard-CEKAL-Textes existieren zwei Möglichkeiten:
  - Entweder tragen Sie den Standardtext hier ein. Dieser wird dann immer automatisch bei der Positionserfassung für jede Position gebildet.
  - Oder Sie lassen im Dialog Textzuordnung die Felder leer und ordnen diesen den Standardtext zu. Dieser wird nur dann gebildet, falls keine anderen CEKAL-Definitionen gefunden werden.
    ⇨ "CEKAL" auf Seite B-1075
- **Center Nr.:** Firmennummer im Rahmen der CEKAL-Zertifizierung. Die Nummer kann sich von der Firmennummer im Register Mandant unterscheiden.

#### Firmendaten – Parameter
*Stammdaten > Firma > Firmendaten > Register Parameter*

*Abb. B-581 Firmendaten - Parameter*

In diesem Register legen Sie Optionen für die Dokumente fest. Änderungen in diesem Register setzen die Standardberechnung in A+W Business außer Kraft.

**Parameter für Dokumenterfassung**
- **Kantenbearbeitung mit exakten Lfm berechnen:** Je nach den Gepflogenheiten des Landes können Kantenbearbeitungen generell gerundet berechnet werden.
  - Die Kantenbearbeitung wird mit gerundeten Laufmetern berechnet.
  - Die Kantenbearbeitung wird mit den exakten Laufmetern berechnet.
    ⇨ "Rundung" auf Seite B-881
    ⇨ "Zwingende Modellvermaßung" auf Seite B-931
- **Logo-Erfassung:** Soll ein Logo gedruckt werden, muss in den Stammdaten pro Kunden für die Modelle und Rechteckscheiben die Logoposition angeben werden.
  - Standardmäßig wird das Logo in der Stückliste hinzugefügt.
  - Das Logo wird automatisch auf dem Glas (ESG) angebracht. Diese Einstellung kann pro Kunde überschrieben werden.
    ⇨ "Logoposition" auf Seite B-842

- **Tatsächliche Warengruppen für Stücklistensuche:** Das Logo kann in den Stammdaten bei einem Hauptprodukt oder bei einer Warengruppe hinterlegt sein. Die automatische Suche nach einem Logo kann bei Positionen mit einer Stückliste sowohl über das Hauptprodukt als auch über die WGR gestartet werden. Die Checkbox ist nur freigeschaltet, wenn die Logo-Erfassung aktiviert ist.
  - Standardmäßig wird das Logo über das Hauptprodukt gesucht.
  - Für alle Stücklistenelemente der ersten Ebene wird das Logo über die jeweilige Warengruppe des Stücklistenelements gesucht. Mit dieser Einstellung wird das Logo z. B. bei einem VSG unabhängig davon gesucht, ob es eigenständig als Hauptposition erfasst wird, oder ob es in die Stückliste eines Isolierglases eingetauscht wird.

- **Teillieferungsposition nicht löschen:** Aufträge können als Teillieferungen mit und ohne Teilfakturierung ausgeführt werden. Die Einstellung kann zusätzlich pro Kunde festgelegt werden.
  - Standardmäßig werden die Positionen einer Teillieferung aus dem Originalauftrag gelöscht, nachdem diese Positionen vollständig geliefert wurden.
  - Bei Teillieferung mit Teilfakturierung werden die gelieferten Positionen nicht aus dem Originalauftrag gelöscht. Die vollständig gelieferten Positionen werden auf 0 gesetzt.
    ⇨ "Partnerverwaltung - Auftrag" auf Seite B-764

- **Teillieferungsdatum von Originalauftrag übernehmen:** Im Lieferschein kann das Datum des Auftrages bei Teillieferungen aktualisiert werden.
  - Standardmäßig wird das Teillieferungsdatum bei jeder Erstellung einer Teillieferung eingetragen.
  - Das Lieferdatum des Originalauftrages wird in den Teillieferauftrag übernommen.

- **Status erhöhen, wenn Kreditlimit überschritten:** Das Kreditlimit für einen Kunden wird in der Auftragserfassung geprüft, sobald der Auftrag gespeichert wird.
  - Wird bei der Auftragserfassung das Kreditlimit überschritten, können folgende Aktionen ausgelöst werden:
    - Es wird lediglich eine Meldung angezeigt, der Auftrag kann jedoch vollständig erfasst werden.
    - Die Erfassung des Auftrags ist nicht möglich.
    Diese Entscheidung legen Sie in den Stammdaten jedes Kunden fest.
    ⇨ "Kreditlimit" auf Seite B-779
  - Während der Auftragserfassung wird automatisch der Statuspunkt des Auftrags auf 700 Kreditlimit überschritten gesetzt, wenn das Kreditlimit überschritten wird. Solche Aufträge können über den Nummernverwalter selektiert werden. Danach muss entschieden werden, ob der Auftrag für die Produktion freigegeben werden kann, oder ob er für die weitere Bearbeitung gesperrt bleibt.
    ⇨ Tutorial 1, "Kreditlimit für Kunden" auf Seite B-90
> **Anwenderstatus zuordnen**
> Zum Statuspunkt 700 muss ein entsprechender Anwenderstatus existieren, der im Dialog Statuszuordnung zugeordnet wird. Haben Sie den Status eines Auftrags, der automatisch auf den Statuspunkt 700 gesetzt wurde, manuell runtergesetzt, so wird er danach nicht mehr automatisch verändert.
> ⇨ Tutorial 2, "Statusverwaltung" auf Seite B-419
> ⇨ "Statuszuordnung" auf Seite B-887

- **Abweichende Beschaffungsart pro Mandant/AV-Bereich aktivieren:** Wenn Sie mit Mandanten arbeiten, kann die Beschaffungsart der Produkte pro Mandant eingestellt werden.
  - Die Beschaffungsart wird übergreifend für alle Mandanten eingestellt.
  - Die Beschaffungsart kann pro Mandant eingestellt werden. Dazu muss in den Produktstammdaten das abweichende Produktkennzeichen pro Produkt und Mandant festgelegt werden.
    **Beispiel:** Die Firma hat die AV-Bereiche ESG und ISO. Der AV-Bereich ISO bestellt ein ESG beim AV-Bereich ESG, z. B. ein ESG 6 mm. Dieses Produkt ESG 6 mm hat im AV-Bereich ESG die Beschaffungsart Produktion und im AV-Bereich ISO die Beschaffungsart Bestellung.
    ⇨ "Produktkennzeichen" auf Seite B-610

- **Produktkennzeichensuche aktivieren:** In der Produktverwaltung wird einem Produkt eine Beschaffungsart zugeordnet. Zusätzlich können im Dialog **Produktkennzeichen Verwaltung** einem Produkt pro Mandant und AV-Bereich andere Beschaffungsarten zugeordnet werden.
  - Wenn Sie nicht mit unterschiedlichen Beschaffungsarten pro Produkt arbeiten, sollten Sie die Checkbox deaktivieren. Sie entlasten damit das System.
  - Das Programm prüft, ob einem Produkt unterschiedliche Beschaffungsarten zugeordnet sind. Das Produkt wird dem AV-Bereich entsprechend produziert oder bestellt.
    ⇨ "Produktverwaltung - Lager/Einkauf" auf Seite B-608
    ⇨ "Produktkennzeichen Verwaltung" auf Seite B-632

- **Interaktive Vertreterprovisionierung:** Standardmäßig wird die Vertreterprovision bei der Übergabe der Dokumente an das Archiv ermittelt. Dazu muss im Register Archiv die Checkbox **Übergabe Provisionsstatistik** aktiviert sein. Bei der Auftragserfassung kann die Vertreterprovision pro Position eingegeben bzw. geändert werden.
  - In der Auftragserfassung wird der Provisionssatz nicht angezeigt. Erst bei der Übergabe an die Provisionsstatistik werden die Provisionssätze aus den Stammdaten zur Berechnung der Provision herangezogen.
  - In der Auftragserfassung wird der Provisionssatz angezeigt. Sie müssen die Aufträge zusätzlich über den Dialog **Übergabe Archiv** an die Provisionsstatistik übergeben, damit die Provision errechnet wird.
    ⇨ "Automatikoptionen" auf Seite B-969
    ⇨ "Vertreterprovision" auf Seite B-1022
    ⇨ Verkauf, "Übergabe Archiv" auf Seite C-686

- **Rückschreibung von manuell geänderten Werten in referenzierendes Dokument:** Wird in einer referenzierten Bestellung der Lieferantenpreis geändert, kann dieser Preis in den Auftrag zurückgeschrieben werden.
  - Standardmäßig werden geänderte Werte nicht in das referenzierende Dokument zurückgeschrieben.
  - Die geänderten Werte sollen in das referenzierende Dokument übernommen werden.
  - **Referenzierendes Dokument:** Angabe, wie die geänderten Werte übernommen werden sollen.
    - **Ja, Nein:** Der geänderte Wert wird nur zurückgeschrieben, wenn die zusätzlich angezeigte Abfrage mit [Ja] bestätigt wurde.
    - **Immer:** Der geänderte Wert wird ohne Abfrage immer zurückgeschrieben.
    - **Niemals:** Der geänderte Wert wird nicht zurückgeschrieben. Eine Abfrage wird dazu nicht angezeigt.

- **Stücklistenvererbung von Varianten:** Wenn eine Stücklisten-Komponente auf der obersten oder auf einer mittleren Stücklistenebene durch eine Variante ausgetauscht wird, können automatisch die Varianten der zugehörigen Komponenten ausgetauscht werden.
  - Die Änderung einer Stücklisten-Komponente wird nicht an die darunterliegenden Komponenten weitergereicht.
  - Wird in der Positionserfassung bei einem Produkt mit Stücklisten-Komponenten z. B. dessen Farbe geändert, so ändert sich automatisch die Farbe aller darunterliegenden Stücklisten-Komponenten.
    ⇨ "Produktvarianten" auf Seite B-643

- **Rechteckeckausschnitte als Breite x Höhe erfassen:** Die Kennzeichnung für Eckausschnitte kann umgekehrt werden.
  - Die Maße werden umlaufend erfasst nach dem Schema A-B-A-B.
  - Randausschnitte werden nach dem Standardschema erfasst, d. h., dass A immer der Wert für Breite, B immer der Wert für Höhe ist.
  
  