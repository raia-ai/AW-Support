---
title: "D-AWBusiness-HB_16"
source: "D-AWBusiness-HB_16.pdf"
tags: ["A+W Business", "ERP", "Verkauf", "Bestellung", "Angebot", "Gutschrift", "Datenübergabe", "Archivierung", "FiBu", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a German-language tutorial for the A+W Business sales module, covering the creation and management of credit notes, purchase orders, offers, and the process of data transfer to other systems."
long_description: "This comprehensive tutorial serves as a user guide for the 'A+W Business Verkauf' (Sales) module of the A+W Business ERP software. The document is structured into several learning blocks, each focusing on a key aspect of the sales process. It begins with exercises on creating credit notes for incorrectly recorded order items. The main sections cover 'Bestellung' (Orders), detailing how to handle order items that require purchasing parts, including order handovers to the purchasing department, managing the order pool, and handling internal orders. The 'Dokumentendaten' (Document Data) section explains how to collectively manage and modify data for multiple documents, such as delivery dates. The 'Angebote' (Offers) part of the tutorial explains how to create and manage offers, including alternative positions and entire alternative offers, and how to track them using a follow-up system. 'Datenübergabe' (Data Transfer) describes the process of transferring financial data to accounting systems (FiBu), exporting data for statistical analysis, and archiving old documents. Finally, 'Zusatzfunktionen' (Additional Functions) covers topics like importing documents via EDI, generating inventory lists, and using the system journal. The document includes step-by-step instructions, screenshots, learning objectives, and practical exercises."
---

# Tutorial: Dokumente kopieren

---
## Übungen

### Gutschrift erfassen
Öffnen Sie einen Auftrag, zu dem Sie bereits einen Lieferschein erstellt haben.
- Erfassen Sie zur Position 1 eine Gutschrift, da diese falsch erfasst wurde.

### Ergänzende Informationen
⇨ Stammdaten, "Nummernkreise" auf Seite B-903
⇨ Stammdaten, "Nummer Gutschrift = Nummer Dokument" auf Seite B-944

---

## Tutorial: Bestellung

### Bestellung
In diesem Themenblock lernen Sie, wie Sie Auftragspositionen weiter bearbeiten, in denen Bestellungen enthalten sind.

Dazu gehören folgende Lerneinheiten:
- "Bestellübergabe" auf Seite C-303
- "Bestellungen" auf Seite C-320
- "Dokumentendaten" auf Seite C-325

---

## Bestellübergabe

### Lernziele
- Auftragspositionen mit Bestellungen in den Bestellpool stellen.
- Bestellung im Bestellpool prüfen.
- Lieferant und Liefertermin ändern.
- Bestellung an den Einkauf übergeben.

### Nutzen
- Sie können in einem Auftrag auch Positionen erfassen, zu denen Teile dazugekauft werden müssen. Sie brauchen diese Zukäufe nicht neu zu erfassen, sondern übergeben die entsprechenden Auftragspositionen an den Einkauf.
- Sie erkennen die Umsetzung des Status einer Auftragsposition durch eine Rückmeldung aus dem Wareneingang. Sie wissen, wie Sie den Auftrag dann weiter bearbeiten müssen.

### Merke

**Beschaffungsart**
Die Beschaffungsart eines Produktes ist in den Produktstammdaten hinterlegt. Sie kann für jede einzelne Auftragsposition überschrieben werden.
Über dieses Kennzeichen erkennt A+W Business die Bestellposition und leitet automatisch die Bestellung ein.

**Bestellübergabe**
Die Übergabe einer Bestellung muss manuell angestoßen werden. Aus dem Bestellpool werden nur die Auftragspositionen mit einem Bestellkennzeichen an den Einkauf übergeben.
Wenn in einem Auftrag mehrere Positionen mit Bestellkennzeichen erfasst wurden, wird für jeden Lieferanten eine eigene Bestellung erzeugt.

**Preisvergleich**
Vor der Übergabe der Bestellung können Sie die Preise der Lieferanten vergleichen, die das Produkt liefern können. Dazu muss die Lieferantenkartei gepflegt werden.

**Terminänderung**
Wird im Bestellpool das Anlieferdatum beim Kunden geändert, wird diese Änderung auch in den referenzierten Auftrag übernommen.

**Voreinstellungen**
Stammdaten:
- Nummernkreise
- Lieferantenkartei

Firmendaten:
- Register Produktion (Profit-Center-Abrechnung)
- Register Lager/EK/EDI (Abstandhalter mitbestellen)

---

### Bestellposition im Auftrag
Bestellungen zu Auftragspositionen können direkt aus den Aufträgen heraus erzeugt werden. Dazu muss mindestens eine Stücklisten-Komponente oder die gesamte Position als Bestellung gekennzeichnet sein.

Bestellungen werden nicht automatisch an den Einkauf übergeben. Sind Bestellartikel in einem Auftrag enthalten, können Sie sich dies durch eine Meldung anzeigen lassen, wenn Sie die Positionserfassung schließen.

