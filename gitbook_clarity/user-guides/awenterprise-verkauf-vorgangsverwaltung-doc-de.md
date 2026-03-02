---
description: "DE_AWEnterprise_Verkauf_4_3"
---


# Softwarereferenz

---
## Vorgangsverwaltung

**Skonto 1, Skonto 2, Skonto 3**
Schlüssel der Skontosätze für das Zahlungsziel. Sie können bis zu 3 verschiedene Schlüssel angeben. Auf diese Weise können Sie gestaffelte Zahlungsziele definieren.
*Technische Info: numerische Felder, DB-Felder: kauf._skonto1, kauf._skonto2, kauf._skonto3*

**Merkmal**
Nummer der Form der Bezahlung, z. B. Banklastschrift, Bankabbuchung. Sie hinterlegen Merkmale in den Systemstammdaten als Zahlungsweisem. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Merkmals im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.zahlngmerk*

**Zahlungsverkehr**
Art und Weise der Bezahlung, z. B. Vorauskasse, Bankeinzug. Die Angaben zum Zahlungsverkehr sind vom System vorgegeben.
*Technische Info: Toggle-Feld, DB-Feld: kauf.skontoart*

**FIBU-Key**
Schlüssel zur Übergabe an die Finanzbuchhaltung. Die Schlüssel der Finanzbuchhaltung werden vom System eingetragen und an die Finanzbuchhaltung gesendet.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.fibukey*

**FIBU-Debitor**
Kundennummer des Marktpartners, der als Rechnungsempfänger bestimmt ist. Das Feld ist standardmäßig vorbelegt.
*Technische Info: numerisches Feld, DB-Feld: kauf.stddebnr*

**Bonus**
Vereinbarter Bonus für den Vorgang, den ein Lieferant seinem Kunden gewährt. Die Höhe des Bonus richtet sich z. B. nach dem Umsatz, der mit dem Kunden innerhalb eines festgelegten Zeitraums erzielt wird. Der Bonus wird prozentual angegeben.
*Technische Info: numerisches Feld, DB-Feld: kauf.bonusnr*

**Provision**
Vertreterprovisionssatz für den Auftrag. Die Provision wird prozentual angegeben.
*Technische Info: numerisches Feld, DB-Feld: kauf.provnr*

**Private Felder**
Die privaten Felder werden kundenspezifisch für Zusatzinformationen genutzt. Sie sind frei konfigurierbar. Die Feldbezeichnungen werden über die Umgebungsvariablen gesetzt. Die beiden oberen Zeilen sind numerische Felder, die beiden unteren Zeilen sind freie Textfelder.
*Technische Info: numerische Felder, alphanumerische Felder, DB-Felder: kauf.private_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2*

### Weitere Optionen

**Kontrolle**
Nummer des Mitarbeiters, der den Vorgang kontrolliert. Wenn das Feld gefüllt ist, werden die Vorgänge erst nach Prüfung durch den entsprechenden Mitarbeiter freigeschaltet.
*Technische Info: numerisches Feld, DB-Feld: kauf.kontrollmanr*

**Windlast**
Windlast am Einbauort. Windlast (N/m²) ist der Druck, der durch direkte Windeinwirkung auf die äußere Oberfläche eines Gebäudes ausgeübt wird. Die Windlast kann nur für Gläser mit mehreren Scheiben angegeben werden.
*Technische Info: numerisches Feld, DB-Feld: kauf.wlast*

> **Restriktionsprüfung bei Eingabe der Windlast**
> Wenn für die Windlast ein entsprechender Eintrag in den Stammdaten angelegt ist, wird die angegebene Windlast einer Restriktionsprüfung unterzogen. Das System prüft z. B., ob die Dickengruppe der gewählten Gläser für die angegebene Windlast ausreichend ist. Bei Verletzung der Restriktionsprüfung wird eine Meldung angezeigt.

**Fassadenzone**
Angabe der Fassadenzone, in der die Scheiben verbaut werden. Hohe Gebäude oder Gebäude, die an Randgebieten stehen, werden z. B. mit einer erhöhten Windlast belastet.
- 1 Rand: Für Gebäude mit erhöhter Windlast.
- 2 Zentral: Für Gebäude ohne erhöhte Windlast.
*Technische Info: numerisches Feld, DB-Feld: kauf.bereich*

**Min/Max ISO Ges-Stärke**
Minimale und maximale Glasstärke des gesamten ISO-Artikels in Millimeter. Die Glasstärke ist abhängig von der gewählten Fassadenzone und der Windlast.
*Technische Info: numerische Felder, DB-Felder: kauf.minszr, kauf.maxszr*

**Falzmaß**
Korrekturmaß in Millimeter. Das Falzmaß wird auf die Breite und Höhe der Positionen aufgeschlagen. Z. B. werden für ein Glas mit den Maßen 1050 mm x 1250 mm und einem Falzmaß von 2 mm in der Datenbank die Maße 1052 mm x 1252 mm hinterlegt. Der Wert wird an die Produktion übergeben. Wenn Sie mit A+W Production arbeiten, wird dieser Wert in der Regel ignoriert und das Falzmaß aus A+W Production herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kauf.falzmass*

**Textformeln**
Nummer und Bezeichnung der Produktkennzeichnung, z. B. Rahmentext. Die Textformeln müssen in den Stammdaten angelegt sein.
*Technische Info: numerisches Feld, DB-Feld: kauf.artkennfrm*

**Angeb. Status**
Status des Angebots. Dieses Feld wird nur bei Angeboten angezeigt. Bei Bezugnahme wird der Feldinhalt übernommen.
- **offen:** Das Angebot wurde noch nicht bestätigt.
- **gewonnen:** Das Angebot wurde bestätigt.
- **verloren:** Das Angebot wurde abgelehnt.
- **verjährt:** Das Angebot ist nicht mehr gültig.
*Technische Info: Toggle-Feld, DB-Feld: kauf.angbstatus*

### Details der Auslieferung
Diese Felder werden vorbelegt, wenn die Via-Plant-Funktion konfiguriert ist. Mit der Via-Plant-Funktion können Auslieferungen zum Kunden über ein weiteres Haus organisiert werden. Dazu muss auch die interne Mandantentrennung aktiv sein.

**Ankunft in via Haus**
Datum, an dem die Lieferung voraussichtlich im Haus ankommt, über das die Lieferung versendet wird.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ankunftvia*

**via Haus**
Mandantennummer des Hauses, über das die Lieferung versendet wird. Dieses Ziel-Haus können Sie im Kopfbereich im Feld Route mit `<F5>` festlegen.
*Technische Info: Anzeigefeld, DB-Feld: kauf.vsvia*

**Fahrtdauer**
Voraussichtliche Fahrzeit zum Ziel-Haus. Die Fahrtdauer wirkt sich auf den Liefertermin aus.
*Technische Info: Anzeigefeld, DB-Feld: kauf.anfahrt*

**Handlingsz.**
Handlings-Zeit, um die Lieferung im Ziel-Haus auf- oder abzuladen.
*Technische Info: Anzeigefeld, DB-Feld: kauf.handlingvia*

**Geplant in via**
Datum der geplanten Auslieferung im Ziel-Haus. Das Datum gibt an, an welchem Tag die Lieferung das Ziel-Haus voraussichtlich verlässt.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ltplanvia*

**Route**
Nummer der Route. Auslieferungsroute zum Kunden hin. Die Route unterscheidet sich von der Route im Start-Haus.
*Technische Info: Anzeigefeld, DB-Feld: kauf.endroutenr*

**Ankunftstag bei Kunden**
Datum, an dem die Lieferung beim Kunden ankommt.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ankunft*

**Fahrtdauer**
Voraussichtliche Fahrzeit vom Ziel-Haus zum Kunden. Die Fahrtdauer wirkt sich auf den Liefertermin aus.
*Technische Info: Anzeigefeld, DB-Feld: kauf.anfahrtvia*

**Wareneingangstermin**
Datum, an dem die Lieferung am Wareneingang eintrifft. Das Datum wird im Format TT.MM.JJJJ angegeben.
*Technische Info: Datumsfeld, DB-Feld: kauf.ptermin1*

### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83

Die Felder können nur betreten werden, wenn Sie die Positionserfassung abgeschlossen haben. Mit `<Ende>` wechseln Sie aus der Positionsebene in den Fußbereich.

## Auftragserfassung – Summen
Verkauf > Auftragserfassung > Auftragsfuß > Feld Rabatt, Nettototal > <F2>

