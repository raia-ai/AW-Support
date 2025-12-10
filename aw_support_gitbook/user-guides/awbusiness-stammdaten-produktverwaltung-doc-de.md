---
title: "DE_AWBusiness_Stammdaten_9_7"
source: "DE_AWBusiness_Stammdaten_9_7.pdf"
tags: ["A+W Business", "Stammdaten", "Produktverwaltung", "Preiskalkulation", "Lagerverwaltung", "ERP", "Software-Referenz", "technische Dokumentation", "Glasindustrie"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical software reference guide for A+W Business, focusing on master data management within the Product Management module. It covers topics such as creating and configuring products, countersinks, pricing, surcharges, inventory parameters, and production data."
long_description: "This document is a comprehensive software reference manual for the \"A+W Business\" ERP system, specifically detailing the \"Stammdaten\" (Master Data) section of the \"Produktverwaltung\" (Product Management) module. It provides step-by-step instructions and explanations for configuring various product attributes. Key areas covered include: defining countersinks with specific parameters; managing prices and surcharges, including tax settings, discounts, and rounding rules; setting up inventory and purchasing parameters, such as procurement types, stock management, and CE/CPIP data for compliance; configuring models and processing steps, including parameters, restrictions, and pricing for different shapes and machining; managing bill of materials (BOM) for complex products like insulated glass units (IGUs); assigning texts and language-specific descriptions; and integrating with A+W Production for manufacturing control. The manual is intended for system administrators and power users responsible for setting up and maintaining the product master data, which is fundamental for sales, purchasing, and production processes within the A+W Business software."
---

# Produktverwaltung

---
## Senkbohrung

Sie können mehrere Senkbohrungen mit unterschiedlichen Werten anlegen, z. B. als Standard-Einstellungen für verschiedene Glasarten oder als Bearbeitungsprodukt.

### Typ
Der Typ gibt an, ob die Senkbohrung innen und/oder außen liegt.

### Winkel
Winkel der Senkung. Er wird senkrecht zur Glasebene angegeben. Ein Winkel von 0° entspricht der geraden Schnittkante.

*[Abb. B-374 Senkbohrung (beidseitig) - Diagramm zeigt eine beidseitige Senkbohrung mit den Bezeichnungen A (Schnittkante), B (Durchmesser) und C (Einsenktiefe).]*

- **A** Schnittkante
- **B** Durchmesser
- **C** Einsenktiefe

### Erfassungsart
Die Erfassungsart gibt an, welche Größe im Auftrag für die Senkbohrung angegeben werden muss.

---

## Produktverwaltung – Preis/Zuschlag

**Stammdaten > Produkte > Artikel > Artikel > Register Preis/Zuschlag**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register Preis/Zuschlag]*

In diesem Register ordnen Sie die Zuschläge zu, die automatisch zu dem Produkt berechnet werden sollen.

Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben:
- "Produktverwaltung - Produkt" auf Seite B-591

### Zuschläge/Rabatte anwenden
In diesem Feld sind die automatischen Zuschläge aufgelistet.
- **☐** Der Zuschlag wird nicht berechnet.
- **☑** Der Zuschlag wird berechnet.
- Tutorial 1, "Funktion der automatischen Zuschläge" auf Seite B-325
- "Produktzuordnung Zuschläge" auf Seite B-1029

### Steuer
Standardmäßig wird jedem Produkt das Steuerkennzeichen 1 zugeordnet. Sie können ein anderes auswählen. In einigen Ländern können auch mehrere Steuersätze zugeordnet werden, z. B. in Nord-Amerika.
Wenn Sie keine Steuer aktiviert haben, wird für das Produkt keine Steuer berechnet, z. B. für das Produkt Anzahlung.
Die Steuersätze selbst werden im Dialog **Steuer** gepflegt.
- "Steuer" auf Seite B-904

### Kostenrechnung

**Kostenart, Kostenstelle**
Für die Kostenrechnung können Sie jedem Produkt eine Kostenart und eine Kostenstelle zuweisen. Die Daten können über externe Berichte ausgewertet werden.
Die Einstellungen können in der Auftragserfassung überschrieben werden.
- "Kostenart" auf Seite B-913
- "Kostenstellen" auf Seite B-914

### Preis-Parameter

**Preisdarstellung**
Der Preis eines Produktes kann im Formular unterschiedlich ausgewiesen werden:
- **Implizit**: Der Netto-Preis der Hauptposition beinhaltet alle Preise der Stücklisten-Komponenten, also auch die Modell- und Austauschzuschläge und die Bearbeitungen.
- **Explizit**: Die Preise der Stücklisten-Komponenten werden einzeln ausgewiesen.
- **Implizit in Preis pro ME**: Die Preise der Stücklisten-Komponenten werden umgerechnet auf die Preiseinheit des Hauptproduktes. Dieser Gesamtpreis der Preiseinheit wird im Dokument ausgewiesen, aber nur dann, wenn alle Stücklisten-Komponenten einer Position die gleiche Darstellungsart zugewiesen wurde.

**Übernahme Hauptpos.**
Wenn das Produkt in eine Stückliste übernommen wird, kann sich die Berechnung und Darstellung der Preise und Rabatte nach den Angaben richten, die zum Produkt der Hauptposition hinterlegt sind. Folgende Einstellungen sind möglich:
- **Keine Übernahme**: Die Preiseinstellungen werden nicht aus der Hauptposition übernommen.
- **Rabatt + Preisschlüssel**: Rabatt und Preisschlüssel sollen aus der Hauptposition übernommen werden.
- **Rabatt**: Nur der Rabatt soll aus der Hauptposition übernommen werden.
- **Preisschlüssel**: Nur der Preisschlüssel soll aus der Hauptposition übernommen werden.
- **Keine Übernahme (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto sollen die Einstellungen aus der Hauptposition nicht übernommen werden.
- **Rabatt + Preisschlüssel (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto sollen der Rabatt und der Preisschlüssel übernommen werden.
- **Rabatt (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto soll nur der Rabatt übernommen werden.
- **Preisschlüssel (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto soll nur der Preisschlüssel aus der Hauptposition soll übernommen werden.
- **Rabatt + Preisschlüssel (auch falls Rabatt vorh.)**: Rabatt und Preisschlüssel aus der Hauptposition sollen auch dann übernommen werden, wenn im Stücklisten-Produkt ein Rabatt angegeben ist, z. B. beim Austausch eines Glases.
- **Rabatt (auch falls Rabatt vorh.)**: Der Rabatt aus der Hauptposition soll auch dann übernommen werden, wenn im Stücklisten-Produkt ein Rabatt angegeben ist, z. B. beim Austausch eines Glases.
- **Preisschlüssel (auch falls Rabatt vorh.)**: Der Preisschlüssel aus der Hauptposition soll auch dann übernommen werden, wenn im Stücklisten-Produkt ein Rabatt angegeben ist, z. B. beim Austausch eines Glases.

Zur Übernahme von Rabatten siehe auch:
- "Rabattverwaltung - Austauschrabatte" auf Seite B-810

> **Einstellungen zur Preisfindung in den Firmendaten**
> Im Dialog Firmendaten > Register Preisberechnung werden übergreifende Einstellungen festgelegt, die die Einstellungen in den Produktstammdaten z. T. überschreiben können.

**Preistabelle VK / EK**
Nummern der Preistabellen, die zur Berechnung des Verkaufspreises und des Einkaufspreises herangezogen werden.
Die Produkte und die dazugehörigen Preise werden getrennt angelegt. In der Regel sind Produktnummer und Nummer der Preistabelle gleich. Eine Unterscheidung ist nur dann sinnvoll, wenn viele unterschiedliche Produkte denselben Preis haben.
- Tutorial 1, "Preistabellen" auf Seite B-230

**[Preistabelle]**
Öffnet den Dialog zur Bearbeitung der Preise.
- "Preise" auf Seite B-714

**Grundprodukt**
Nummer der Preistabelle, die als Berechnungsgrundlage dient, wenn BEIDE Gläser in einem ISO ausgetauscht werden. Wenn eine Preistabelle angegeben ist, wird in der Auftragserfassung automatisch eine Meldung angezeigt, die abfragt, ob tatsächlich auf die Grundtabelle zurückgegriffen werden soll.
Wird kein Glas oder nur ein Glas ausgetauscht, so wird auf den Eintrag im Feld Preistabelle zurückgegriffen.

**Tab. Austauschzuschl.**
Nummer der Tabelle für Austauschzuschläge. Jeder Isolierglastabelle kann ein anderer Austauschzuschlag zugeordnet werden.
- Tutorial 1, "Funktion des Austauschzuschlags" auf Seite B-288
- "Austauschzuschläge" auf Seite B-668

**Mindermengenzuschl.**
Nummer des Mindermengenzuschlags.
Bei Gläsern kann ein Zuschlag angegeben werden, der immer dann erhoben wird, wenn im Auftrag eine bestimmte Menge (Fläche) unterschritten wird. Der Mindermengenzuschlag muss als Produktzuordnung Zuschlag angelegt sein.
- Tutorial 1, "Funktion der automatischen Zuschläge" auf Seite B-325
- "Produktzuordnung Zuschläge" auf Seite B-1029

**Sonstiger Zuschlag**
Sonstige Zuschläge können aus unterschiedlichen Gründen erhoben werden, z. B. ein Zuschlag für eine Kantenlänge größer 3760 mm, da diese Länge schwerer zu bearbeiten ist.
- Tutorial 1, "Funktion der Sonstigen Zuschläge" auf Seite B-306
- "Sonstige Zuschläge" auf Seite B-666

**Zuschlagsart**
Zuschlagsarten geben an, auf welcher Basis der jeweilige Zuschlag berechnet werden soll:
- **akt. Bearbeitung:** Für die markierte Komponente in der Stückliste.
- **alle vorherigen Bearbeitungen:** Für alle Bearbeitungen, die vor der markierten Komponente in der Stückliste aufgeführt werden.
- **alle vorherigen Positionen:** Für alle Komponenten, die vor der markierten Komponente in der Stückliste aufgeführt werden.
- **Basisposition:** Für die oberste Position (Produkt) in der Stückliste, der ebenfalls ein Zuschlag zugewiesen sein kann.
- **Basisposition ohne sonstige Zuschläge:** Für die oberste Position in der Stückliste, ohne den Zuschlag, der dem Produkt zugewiesen sein kann.
- **Basisposition + Bearbeitungen:** Für die oberste Position in der Stückliste und die zugehörigen Bearbeitungen.
- **Basisposition + Modell:** Für die oberste Position in der Stückliste und das zugehörige Modell.
- **Basispreis:** Für den Preis der obersten Position in der Stückliste.
- **Vater + dessen Gläser:** Für die oberste Position einer Baugruppe (Vater) und der Gläser dieser Baugruppe.
- **Vater + dessen vorh. Bearbeitung:** Für die oberste Position einer Baugruppe (Vater) und die Bearbeitung, die an diese Komponente angehängt ist.
- **vorher. Stckl. m. gl. Vater:** (Vorherige Stückliste mit gleichem Vater). Alle Komponenten der Baugruppe.
- **vorherige Bearbeitung:** Alle Bearbeitungen, die vor der Komponente aufgeführt sind, zu der der Zuschlag festgelegt wurde.

Alle Zuschlagsarten können sowohl additiv als auch nicht additiv berechnet werden. Die Alternative nicht additiv bezieht sich nur auf prozentuale Zuschläge. Der Einstellung entsprechend wird ein Wert gebildet, der als Grundlage zur Berechnung des prozentualen Zuschlages dient.
- Tutorial 1, "Berechnungen nach Zuschlagsarten" auf Seite B-311

**Maßrundung Breite / Höhe**
In Deutschland basiert die Preisberechnung auf einer 30er-Rundung. Dies bedeutet, dass zur Berechnung der nächste durch 30 teilbare Wert für die Kantenlänge zugrunde gelegt wird. In Frankreich wird mit einer 10er-Rundung gerechnet.
> **Beispiel**
> Rundung 30:
> Bei einem Glas von 1000 x 1000 mm wird die Fläche 1,04 (= 1020 x 1020) berechnet.

**Fläche max.**
Höchstmaß für die Fläche, für die der reguläre Preis berechnet wird. Der Wert wird bei der Positionserfassung geprüft. Bei Überschreitung wird der angegebene Sonstige Zuschlag (Übergrößenzuschlag) berechnet. Der Wert für die Fläche und für das Seitenverhältnis (im nachfolgenden Feld) sollte sich an den entsprechenden Werten im Register **Produkt** orientieren.
- "Fläche / Seitenverhältnis max." auf Seite B-594

**Seitenverhältnis max.**
Höchstmaß für das Seitenverhältnis. Der Wert wird im Verhältnis von 1: x angegeben. 1: 6 bedeutet, dass bei einer Breite von 600 mm die Höhe höchstens 3600 mm betragen darf. Bei Überschreitung wird der angegebene Sonstige Zuschlag berechnet.

**Mittlerer Verschnitt**
Dieser Wert wird bei der Berechnung des EK-Preises für Glas, für Gas (Verlust) und bei der Berechnung der reservierten Lagermenge, berücksichtigt.

> **Beispiel: Verschnitt = 5 %, EK = 8,00 €/qm**
>
> | Scheibe: 1000 x 1000 mm | EK: 8,00 € |
> | :--- | :--- |
> | Scheibe: 1000 x 1000 mm<br>Verschnitt: 0,05 qm | Berechnete Fläche: 1,05 qm<br>EK: 8,40 € |
- Lagerwirtschaft, "Einkaufspreis und Durchschnitts-EK" auf Seite G-52

**Bearbeitungsindex**
Der Bearbeitungsindex bewertet den Aufwand und die Schwierigkeit bei der Bearbeitung des Produkts. Das Feld ist nur bei Glasprodukten freigeschaltet.
Für den Preis kann der Bearbeitungsindex als Grenztyp eingegeben werden.
- Tutorial 1, "Grenztypen für Staffelungen" auf Seite B-250

**Preisrelevant VK, EK**
Das Produkt kann bei der Berechnung des Preises für den Verkauf und/oder den Einkauf berücksichtigt werden. Bei Produkten mit einer Stückliste bezieht sich diese Checkbox auf die Hauptposition.
- **☐** Das Produkt wird im Auftrag nicht bei der Preisberechnung des VK und/oder des EK berücksichtigt. Diese Einstellung können Sie verwenden, wenn das Produkt als Stücklisten-Komponente verwendet werden soll und der Preis dann über das Hauptprodukt ermittelt wird, z. B. Folie im VSG.
- **☑** Für die Preisberechnung wird auf die zugehörige Preistabelle für VK und/oder EK zurückgegriffen.
Für Gläser in ISO-Einheiten, die im Auftrag ausgetauscht werden, hat diese Angabe keine Bedeutung, da die Preise dann nach den hinterlegten Austauschpreisen berechnet werden.
- Tutorial 1, "Kennzeichen zur Preisberechnung" auf Seite B-168

**Rabattfähig, Skontofähig**
Angabe, ob im Auftrag ein Rabatt oder Skonto zur Preisberechnung zugelassen ist. Beide Einstellungen können im Auftrag überschrieben werden.
- **☐** Für die Preisberechnung wird im Auftrag kein Rabatt berücksichtig, bzw. kann ein Skonto eingeräumt werden. Selbst wenn für eine Warengruppe ein Rabatt angelegt wurde, ist es an dieser Stelle möglich, ihn nicht zu gewähren. Dasselbe gilt für die Skontofähigkeit.
- **☑** Rabatt und/oder Skonto sind im Auftrag möglich.

---

## Produktverwaltung - Lager/Einkauf

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register Lager/Einkauf]*

In diesem Register legen Sie die Parameter für den Einkauf und die Lagerführung des Produktes fest.

Die Felder in den Bereichen **Artikel** und **Eigenschaften** sind zum Register **Produkt** beschrieben.
- "Produktverwaltung - Produkt" auf Seite B-591

### CPIP-Daten
Die Felder in diesem Bereich werden nur angezeigt, wenn in den Firmendaten die CPIP-Bildung aktiviert ist. Damit die Daten korrekt eingegeben und geprüft werden können, müssen bei der Installation und Konfiguration von A+W Business die entsprechenden Dateien importiert worden sein.
- "CPIP-Bildung" auf Seite B-953

#### CE-relevant
Die CPIP-Daten können unabhängig vom CE-Kennzeichen gekennzeichnet werden.
- **☐** Der CPIP-Code hat für die CE-Kennzeichnung keine Bedeutung.
- **☑** Der CPIP-Code ist Bestandteil der CE-Kennzeichnung.

#### Zertifizierung
Zertifizierung, die für das Produkt zutrifft. Die Zertifizierungen müssen in den Stammdaten zur CE-Kennzeichnung hinterlegt sein. Folgende Werte stehen zur Wahl:
- **Selbsterklärt:**
  - **Alle Produkttypen:** Der CPIP-Code kann gebildet werden, die CE-relevanten Komponenten dürfen nicht gelöscht werden.
  - **Einfachglas, VSG:** Durch Tauschen oder Hinzufügen CE-relevanter Komponenten wird der CPIP-Code entfernt.
  - **ISO:** Nach einem Austausch von CE-relevanten Komponenten wird die Suche nach dem CPIP-Code neu gestartet. Wenn die getauschten Komponenten nicht durch die ISO-CPIP-Suche abgefragt werden, wird der CPIP-Code entfernt.
- **Zertifiziert, Zertifiziert mit Maßrestriktion:**
  - **Alle Produkttypen:** Der CPIP-Code muss gebildet werden, die CE-relevanten Komponenten dürfen nicht gelöscht werden.
  - **Einfachglas, VSG:** Tauschen oder Hinzufügen CE-relevanter Komponenten ist nicht zulässig.
  - **ISO:** Wenn kein CPIP-Code gefunden wurde, können die Eingaben nicht gespeichert werden.
- "CE-Kennzeichen" auf Seite B-1084

#### Typ
Auswahl des Produkttyps.

#### CPIP-Code
CPIP-Code für das Produkt. Während der Eingabe wird der Code entsprechend der Einstellung im Feld **Zertifizierung** geprüft.
- "CPIP-Code" auf Seite B-1084

### SAP Produkt Identifikation

**Materialtyp**
Nummer des Materialtyps, der in SAP für dieses Produkt angegeben ist.

**Produktcode**
Produktnummer, die in SAP für dieses Produkt angegeben ist.

**Statistikcode**
Nummer der Auswertung, die in SAP für dieses Produkt verwendet wird.

### Parameter Bestellung

**Maximale Breite, Maximale Höhe Bestellung**
Die Werte geben die Höchstmaße der Glasplatte für den Einkauf an.
Wenn diese Werte im Auftrag überschritten werden, kann die Position weder in Eigenfertigung erzeugt noch bei einem externen Lieferanten bestellt werden.
Die Höchstmaße für die Lagerführung können unter diesen Werten liegen. Diese Maße werden im Bereich **Parameter Lagerführung** angegeben.

### Produktkennzeichen

**Beschaffungsart**
Die Beschaffungsart legt fest, wie das Produkt für den Auftrag beschafft wird:
- **Produktion:** Die Auftragsposition wird selbst produziert. Wenn ein Hauptartikel mit dieser Beschaffungsart gekennzeichnet ist, können dessen Stücklisten-Komponenten als Lagerartikel oder als Bestellartikel definiert werden.
  - Tutorial 1, "Beschaffungsart" auf Seite B-171
- **Zuschnitt:** Das Glas für die Auftragsposition wird aus Lagerplatten zugeschnitten. Die Daten werden an die Produktion übergeben.
- **Lagerentnahme:** Das Produkt wird als Lagerartikel mit seinen genauen Abmessungen oder als Stückartikel im Lager geführt. Bei der Auftragserfassung wird die erfasste Menge reserviert.
- **Bearbeitung:** Die Bearbeitungen für eine Auftragsposition werden an die Produktion übergeben.
- **Kundeneigenes Glas:** Das Produkt wird vom Kunden angeliefert und für die Produktion seiner Aufträge verwendet.
- **Bestellung:** Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste zu beachten. Besteht z. B. ein VSG aus einem Float, einer Folie und einem ESG und ist nur das ESG als Bestellung gekennzeichnet, so wird nur das ESG beim Lieferanten bestellt. Das VSG wird in Eigenfertigung produziert.
- **Bestellung (komplett):** Das Produkt wird inklusive aller Bearbeitungen, die im Auftrag in der Stückliste erfasst wurden, bestellt. Besteht z. B. ein VSG aus einem Float 5 mm, einer Folie und einem ESG 5 mm, so wird das VSG als Ganzes bestellt. Beachten Sie hierzu die Abgrenzung zum Kennzeichen Bestellung.
- **Lagerzugang durch Produktion:** Das Produkt soll nur in Produktionsaufträgen verwendet werden, um das Lager zu füllen. Die produzierten Positionen werden dem Lager zugebucht.
  - Tutorial, "Produktionsaufträge" auf Seite E-130

**Lagerbuchungsart**
Die Lagerbuchungsart legt fest, wie ein Produkt als Lagerartikel in der Lagerverwaltung geführt wird:
- **Maßabhängig:** Wählen Sie diese Einstellung, wenn Lagermaße als Stückartikel geführt werden sollen. Die Einstellung ist nur für Glas sinnvoll. Die Mengeneinheit im Register **Produkt** setzen Sie trotzdem auf qm, damit die Fläche berechnet wird.
- **Nicht maßabhängig:** Wählen Sie diese Einstellung, für alle Lagerartikel, die in ihrer eigentlichen Mengeneinheit geführt werden sollen, z. B. Stückartikel, Beschläge. Wählen Sie diese Einstellung auch für Gläser, die in qm geführt werden sollen.
- **Kombiniert:** Wählen Sie diese Einstellung, wenn Sie mit Rückmeldungen aus der Produktion arbeiten. Die Einstellung ist nur für Glas sinnvoll. Vergessen Sie nicht, dass Sie dazu ein Dummy-Lagermaß ohne Maße anlegen müssen.
  - Tutorial, "Wie soll das Lager geführt werden" auf Seite G-17
Die Einstellung **ohne** wird in diesem Zusammenhang nicht benutzt.

**Automatischer Zuschnitt**
Dieses Kennzeichen wird an A+W Production übergeben.
- **☐** A+W Production fügt die Scheibe der Liste der Sonderzuschnitte zu. Diese Scheibe wird dann nicht von der Maschine, sondern von Hand zugeschnitten.
- **☑** A+W Production leitet die Scheiben an die Schneidmaschine weiter und optimiert gleichzeitig den Zuschnitt.

**Keine Verfügbarkeitsprüfung**
Für jedes Produkt kann im Dialog **Lagerinfo** geprüft werden, ob der aktuelle Bestand für die anstehenden Aufträge ausreicht. Wenn Sie die Verfügbarkeitsprüfung auf die Produkte beschränken, für die im Lager tatsächlich Bestände gepflegt werden, erhöhen Sie die Performance des Systems.
- **☐** Für das Produkt wird eine Verfügbarkeitsprüfung durchgeführt.
- **☑** Die Verfügbarkeit wird für das Produkt nicht geprüft. Das Produkt wird im Dialog Lagerinfo nicht angezeigt. Diese Einstellung ist dann sinnvoll, wenn Sie ein Produkt zwar im Lager haben, aber nicht als Lagerartikel führen.

**Technische Artikelnummer**
Pro Glasart-Dicke-Kombination kann bei der Beschaffungsart **Zuschnitt** eine alphanumerische technische Artikelnummer angegeben werden. Diese Nummer wird in der Regel von A+W Production vorgegeben.

**Abweichende Produktkennzeichen**
Öffnet den Dialog **Produktkennzeichen Verwaltung**, um ein anderes Produktkennzeichen auszuwählen, z. B. aus einem anderen AV-Bereich.
- "Produktkennzeichen Verwaltung" auf Seite B-632

### Parameter Lagerführung

**Maximale Breite, Maximale Höhe Lager**
Höchstmaße für die Lagerplatten, die im Lager geführt werden können. Alle Auftragspositionen innerhalb der festgelegten Maße können aus dem Lagerbestand gefertigt werden.
Zwischen den Parametern für die Bestellung und denjenigen für die Lagerführung muss unterschieden werden. Auftragspositionen, deren Maße zwischen denen der Lagerführung und denen der Bestellung liegen, können bei einem Lieferanten bestellt werden. Überschreiten die Maße jedoch die Parameter **Bestellung**, so kann der betreffende Artikel weder gefertigt noch bei einem Lieferanten bestellt werden.

### Produktkennzeichnung

**CE Kennzeichnung**
Sie können ein CE-Kennzeichen für das Produkt (mit seinem Standard-Aufbau) eintragen.
Das CE-Kennzeichen wird in den Auftrag übernommen und kann in den Formularen gedruckt werden. Bei der Produktionsübergabe kann es an A+W Production übergeben werden.

> **CE-Kennzeichnung bei mitgeliefertem Glas**
> Bei der Bestellung von Lohnhärten wird die CE-Kennzeichnung für das Glas aus den Stammdaten ausgelesen. Der Besteller muss die CE-Kennzeichnung des Basisglases an seinen Lieferanten (Lohnhärter) weitergeben. Nur so kann dieser die CE-Konformität ebenfalls bescheinigen.

---

## Produktverwaltung - Modelle/Bearbeitungen

**Stammdaten > Produkte > Artikel > Artikel > Register Modelle/Bearbeitungen**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register Modelle/Bearbeitungen]*

In diesem Register legen Sie die Daten für die Modelle und Bearbeitungen fest, die im Verkauf einer Scheibe zugeordnet werden.

> **Produktart und Produktgruppe für Modelle**
> A+W Business unterscheidet Standardmodelle und das Modell für Stufen-Isolierglas. Dementsprechend müssen Sie auch die Produktgruppe definieren und die Modell-Nummer.
> Standardmodelle verwenden die Modell-Nr. 1 – 99, das Modell für Stufen-Isolierglas hat die Nummer 999.

Eine ausführliche Beschreibung der Daten, die Sie in diesem Register erfassen können, finden Sie im Part Verkauf:
- Verkauf, "Positionen - Bearbeitungen" auf Seite C-468
- Verkauf, "Positionen - Stufung" auf Seite C-487
- Verkauf, "Positionen – Gebogenes Glas" auf Seite C-488
- Verkauf, "Positionen - Bleiverglasungen" auf Seite C-490
- Verkauf, "Positionen – Modell-Template" auf Seite C-491

### Stückliste
Bearbeitungen können an einzelnen Komponenten der Stückliste ausgeführt werden. Angaben zum Modell betreffen immer das Hauptprodukt.
In der Ansicht wird das Modell schematisch angezeigt. Die Legende bezeichnet die Felder, in denen die Maße eingegeben werden.

### Bearbeitungen
**Schaltflächen**
Mit den Schaltflächen wählen Sie eine Produktgruppe aus, z. B. Modelle, Bearbeitungen, gebogenes Glas oder Bleiverglasung. Wenn der Produktgruppe verschiedene Produkte zugewiesen sind, können Sie das gewünschte Produkt im Dialog **Auswahl** markieren und übernehmen.

**Artikel**
Produktnummer und Bezeichnung aus den Stammdaten.

**Formel**
Auswahl und Anzeige der Formel für den Bearbeitungstext.

### Modell
**Symbole**
Über diese Schaltflächen können Sie ein Modell auswählen.

**Artikel**
Die Produktnummer des Modells wird aus den Stammdaten übernommen.

**Modell**
Die Modellnummer wird aus den Stammdaten übernommen.

**Bezeichnung**
Die Bezeichnung des Modells wird aus den Stammdaten übernommen.

### Parameter
**W, H**
Zu jedem Modell werden nur die Felder freigeschaltet, die zur Produktion des Modells notwendig sind. Die Bezeichnungen für die Kanten werden in der Ansicht gezeigt.

**Restriktionen**
In diesem Bereich finden Sie Angaben zu den Restriktionen. Beispiel: H1>0 bedeutet, dass die Kante H1 nicht 0 sein darf.

**S+N Datei**
Wenn Sie häufiger ein bestimmtes Modell mit identischen Maßen erfassen, können Sie es als S+N-Datei speichern. In späteren Aufträgen können Sie diese Datei über die Schaltfläche [Ordner] dann auswählen und der Auftragsposition zuordnen, ohne die Details neu eingeben zu müssen.
Wenn Sie das Modell 99 ausgewählt haben, können Sie auch ein S+N-Template laden und zuordnen.

### Skizzendruck
Sie können auswählen, wie das Modell im Druck wiedergegeben werden soll:
- **Kein Druck:** Die Skizze wird nicht auf den Formularen gedruckt.
- **Modell (maßstäblich):** Bei dieser Einstellung werden maßstabsgetreue Modellskizzen gedruckt.
- **Modell (schematisch):** Bei dieser Einstellung werden die Standardskizzen gedruckt. Sie geben lediglich das Schema des Modells wieder.

### Preise
**Jahrgang/Schlüssel**
Preisjahrgang und -schlüssel für den Modellzuschlag werden aus den Stammdaten übernommen. Sie können geändert werden.

**Preis/PE**
Preis und Preiseinheit für den Modellzuschlag aus den Stammdaten. Sie können geändert werden.

**Rabatt**
Rabatt für den Modellzuschlag aus den Stammdaten. Er kann geändert werden.

**Netto**
Der Nettobetrag für den Modellzuschlag wird automatisch angezeigt.

---

## Produktverwaltung – Stückliste

**Stammdaten > Produkte > Artikel > Artikel > Register Stückliste**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register Stückliste]*

In diesem Register wird die Stückliste ISO- oder VSG-Scheiben abgebildet. Zusätzlich werden Informationen zu den Stücklisten-Komponenten angegeben.
- Tutorial 1, "Stücklistenaufbau bearbeiten" auf Seite B-185
- Tutorial 1, "Produktionsstücklistenauflösung festlegen" auf Seite B-189

### Stückliste
In der Übersicht werden alle Stücklisten-Komponenten aufgeführt. Die Ebene gibt wieder, an welches Produkt die Komponente angehängt wurde. Wenn Sie eine Komponente markieren, werden deren Details in den zugehörigen Feldern angezeigt. Für die oberste Ebene (Hauptprodukt) bleiben die Felder leer.

### Produktionsstücklistenauflösung
In der Übersicht werden alle Bearbeitungen angezeigt, die am Produkt ausgeführt werden können. Mit der Markierung der Checkboxen legen Sie fest, ob die Bearbeitung am Hauptprodukt oder an der Stückliste-Komponente ausgeführt wird. Wenn zu den Stücklisten-Komponenten keine Checkboxen markiert sind, werden die Bearbeitungen am Hauptprodukt ausgeführt.

> **Beispiel**
> In einem VSG haben Sie die Bearbeitungen für Kanten an den Stücklisten-Komponenten aktiviert. Die Kanten werden also vor dem Verbund bearbeitet. Wenn zusätzlich ein Logo angebracht werden soll, so wird dies am Hauptprodukt ausgeführt, also an der VSG-Scheibe.

Die Zuweisung kann in der Auftragserfassung überschrieben werden.
Siehe dazu auch die Einstellungen für die Übernahme bei Austauschgläsern in den Firmendaten.
- "Prod.-Stkl.-Auflösung bei Austausch beibehalten" auf Seite B-942

### Stücklistenartikel
Die Felder in diesem Bereich werden freigeschaltet, wenn in der Übersicht zur Stückliste eine Komponente markiert ist. Die Felder bleiben gesperrt, wenn Sie die oberste Ebene (Hauptprodukt) markieren.

**Artikelnummer, Bezeichnung**
Jede Komponente einer Stückliste ist als Produkt mit einer eigenen Produktnummer und Bezeichnung angelegt.

**Menge/Breite/Höhe**
Die Menge bezieht sich auf Artikel, z. B. 3 Beschläge mitliefern.
In den Feldern Breite und Höhe steht standardmäßig eine Null. Sie können die Maße z. B. bei Standard-Türen (ESG) angeben. Diese Maße können im Auftrag überschrieben werden.

**Abw. WGR, WGR-Statistik**
Die Warengruppe einer Stücklisten-Komponente kann von der der Hauptposition abweichen. Sie können dann z. B. eine Kombinationswarengruppe auswählen, um Komponenten gemeinsam auszuwerten.
- Tutorial 1, "Kombi-WGR" auf Seite B-143

**Strukturebene, Strukturverlauf, Beschichtungsseite**
Die Angaben gelten jeweils für die markierte Stücklisten-Komponente. Diese Felder sind zum Register **Fertigung** beschrieben.
- "Produktverwaltung – Fertigung" auf Seite B-596

**Lieferant, Name**
Die Stücklisten-Komponente wird standardmäßig bei dem eingetragenen Lieferanten bestellt. Die Einstellung kann im Auftrag, in der Position und im Bestellpool geändert werden.
- "Lieferantenkartei" auf Seite B-855
- Einkauf, "Bestellungen" auf Seite D-43

**Beschaffungsart**
Die Angabe gilt für die markierte Stücklisten-Komponente. Die Beschaffungsart ist zum Register **Lager/Einkauf** beschrieben.
- "Produktverwaltung - Lager/Einkauf" auf Seite B-608

**Preisrelevant VK, Preisrelevant EK**
Die Angaben gelten jeweils für die markierte Stücklisten-Komponente. Diese beiden Checkboxen sind zum Register **Preis/Zuschlag** beschrieben.
- "Produktverwaltung – Preis/Zuschlag" auf Seite B-602

**Wird gedruckt**
Sie können für jede Komponente festlegen, ob sie im Formulardruck in der Stückliste aufgeführt werden soll.
- **☐** Die Komponente wird nicht in der Stückliste auf dem Formular gedruckt.
- **☑** Die Komponente wird in der Stückliste auf dem Formular gedruckt.
- Tutorial 2, "Formularverwaltung" auf Seite B-473

**Gruppe für Stücklistenaustausch**
Auswahl der gültigen Austauschgruppe. Mit der Auswahl legen Sie fest, dass nur die Produkte eingebaut werden können, die der angegeben Austauschgruppe zugeordnet sind.
Wenn keine Austauschgruppe angegeben ist, können alle Produkte ausgetauscht werden.
- "Austauschzuordnung" auf Seite B-586

---

## Produktverwaltung – Texte

**Stammdaten > Produkte > Artikel > Artikel > Register Texte**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register Texte]*

In diesem Register ordnen Sie einen Text zu, der im Auftrag angezeigt werden kann. Ein Rahmentext kann an die Produktion übergeben werden.
- Tutorial 2, "Textarten" auf Seite B-462
- "Texte" auf Seite B-1045

Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben.
- "Produktverwaltung - Produkt" auf Seite B-591

### Standardtexte
Der zugewiesene Standardtext muss ein produktbezogener Text sein. Dieser wird auf dem Formular nur im Positionsbereich im Zusammenhang mit dem betreffenden Produkt gedruckt.
In der Positionserfassung wird im Zeilenkopf der Positionsanzeige ein Symbol für einen zugeordneten Text angezeigt.
Über das Textkennzeichen wird gesteuert, in welchen Dokumenten/Formularen der Text gedruckt wird.
- Tutorial 2, "Textkennzeichen und Standardtexte" auf Seite B-464
- "Textkennzeichen" auf Seite B-1044

### Rahmentext
Rahmentexte werden in die Abstandhalter (SZR, Rahmen) der Isolierglasscheiben gedruckt. Der Text muss in Dialog **Texte** angelegt sein.
- Tutorial 2, "Rahmentexte" auf Seite B-463
- "Texte" auf Seite B-1045
Es ist möglich, für jede ISO-Einheit einen speziellen Rahmentext zu hinterlegen. Die Textnummer kann frei vergeben werden.

---

## Produktverwaltung – Sprachen

**Stammdaten > Produkte > Artikel > Artikel > Register Sprachen**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register Sprachen]*

In diesem Register tragen Sie für jedes Produkt die entsprechende fremdsprachliche Bezeichnung ein, wenn Sie mit dem Modul **Mehrsprachigkeit** arbeiten. Die entsprechende Bezeichnung wird über das Sprachkennzeichen des Kunden ausgewählt und im Formular gedruckt.
- "Partnerverwaltung - Adresse" auf Seite B-760

---

## Produktverwaltung – A+W Production

**Stammdaten > Produkte > Artikel > Artikel > Register A+W Production**

*[Screenshot: Artikel | 736/IG Sun4/12/4 A+W - Register A+W Production]*

In diesem Register definieren Sie die Stammdaten, die an die Produktion übergeben werden können. Dieses Register ist nur freigeschaltet, wenn Sie mit A+W Production arbeiten und in den Firmendaten die zugehörige Verbindung eingerichtet haben. Über den Stammdatenabgleich werden die Daten aus diesem Register an A+W Production übertragen.

> **A+W Production-Daten ändern**
> Die Stammdaten werden bei der Installation von A+W Business eingerichtet und an A+W Production übertragen. Setzten Sie sich mit Ihrem Service-Mitarbeiter der A+W Software GmbH in Verbindung, wenn Sie nachträglich Werte ändern müssen.

Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben.
- "Produktverwaltung - Produkt" auf Seite B-591

### A+W Production Glasparameter

**Glasart**
Das aktuelle Glasprodukt ist einer Glasart zugeordnet. Über den Ordner öffnen Sie den Dialog **Glasarten**, in dem Sie Glasarten anlegen können.
- "Glasarten" auf Seite B-635

**Schleifgruppe**
Beim Schleifen und Bearbeiten ist ein Maßzuschlag für die Kanten notwendig, damit die Scheibe auf das Nennmaß bearbeitet werden kann. Diese Schleifzuschläge sind von vier Faktoren abhängig:
- Glasart
- Maschine
- Bearbeitungsart
- Glasdicke
Um nicht für jede einzelne Glasart, Maschine und Bearbeitung einen eigenen Zuschlag erfassen zu müssen, werden diese Kriterien in A+W Production in Gruppen zusammengefasst. Es stehen folgende Gruppen zur Verfügung:
- Standard
- Artikelschleifgruppen
- Maschinenschleifgruppen
- Bearbeitungsschleifgruppen

**Übergangszeit**
Bei einigen Produkten muss zwischen dem Übergang von einem Produktionsbereich zum nächsten oder zum nachfolgenden Arbeitsgang eine Ruhezeit eingehalten werden, z. B. nach dem Härten. Die Zeit wird in ganzen Tagen angegeben. Dieser Wert wird von den Werten der eingesetzten Kapazitätsplanung überschrieben.

**[Glasart-Jumbos-Tische]**
Öffnet den Dialog **Glasart-Jumbos-Tische**. Die Schaltfläche ist nur bei Einfachglas freigeschaltet, das zugeschnitten wird.
- "Glasart-Jumbos-Tische" auf Seite B-873

**Max. Traverenbreite**
Eingabe in mm. Die Breite der zu bildenden Traveren wird begrenzt. Der Wert ist abhängig von der Breite der Lagerplatte. Bei automatischen Brechanlagen gelten die Vorschriften des Herstellers.
Die Begrenzung ist zum einen notwendig, um das manuelle Brechen handlich zu machen, zum anderen können automatische Brechanlagen Traveren nur bis zu einer bestimmten Breite auf der dynamischen Brechstation verarbeiten.

**Min. Abst. X-Z Schnitte**
Mindestabstand zwischen X-Z-Schnitten. Ein Z-Schnitt verläuft zwischen zwei Y-Schnitten parallel zum X-Schnitt. Der Minimalabstand richtet sich in erster Linie nach der Glasdicke und ist für das manuelle Brechen notwendig.

**Reihenf. Opti.**
Reihenfolge, in der die Feinplanung die Optimierungen durchläuft. Je nach Einstellungen der Stammdaten auf- oder absteigend. Glasarten mit hohem Rang werden zuerst optimiert. Üblicherweise bekommen teure Glasarten einen hohen Rang.

**Min. Fläche automatische Opti.**
Fläche, ab der die Optimierung eingesetzt werden soll. Dieser Wert kann durch die Feinplanung überschrieben werden.

### Lage am Zuschnittstisch

**Strukturlage**
Lage der Struktur beim Zuschnitt. Diese Angabe ist wichtig, wenn das strukturierte Glas nur auf einer Seite geschnitten werden kann.

**Beschichtungslage**
Die Beschichtung muss in aller Regel oben liegen, um Beschädigungen durch die weitertransportierenden Rollen beim Zuschnitt zu vermeiden.

### Maschinenzentrum
Die Felder in diesem Bereich werden nicht ausgelesen, da die Zuordnung zu den Maschinen von A+W Production gesteuert wird.
- **Nummer / logisch**: Zurzeit nicht genutzt.
- **Dauer in Sekunden**: Zurzeit nicht genutzt.

### Bruchränder
Der Bruchrand gibt an, wie viel Rand auf der Platte mindestens vorhanden sein muss, damit die zugeschnittene Scheibe (ab)gebrochen werden kann.

**Modell**
Bruchrandwert für Modelle. Dieser Wert ist abhängig von der Glasdicke und der Form des Modells.

**Links, Rechts, Oben, Unten**
Bruchränder für Rechteckscheiben. Die Werte sind abhängig von der Glasdicke.

### A+W Production Bearbeitungsparameter
Die Felder dieser Gruppe sind nur bei Bearbeitungen freigeschaltet.

**Bearb.maße enthalten**
Insbesondere bei gestuften Scheiben muss beachtet werden, ob Bearbeitungsmaße enthalten sind, damit die Berechnung von weiteren Bearbeitungsmaßen zu korrekten Ergebnissen führt.

**Zuschnittsmaß korrigieren**
Zurzeit nicht genutzt.

**Explizite Planung**
Das Produkt kann explizit verplant werden. Wenn eine Bearbeitung als explizit gekennzeichnet ist, wird das zugehörige Produkt (Glas) als so genanntes Freigabeteil gekennzeichnet. In A+W Production können Freigabeteile aus der Stückliste gelöst und explizit verplant werden. In einer ISO-Einheit sind also die Scheiben Freigabeteile, an denen die Bearbeitung ausgeführt wird.

**Interne Bearbeitung**
Interne Bearbeitungen erzeugen ein neues (A+W Production-)Teil, z. B. Zuschnitt, Härten.

**Bearbeitung zukaufen**
Eine Bearbeitung kann zugekauft werden, wenn sie nicht im Betrieb durchgeführt werden kann. Dies muss bei der Produktionsplanung berücksichtigt werden, weil dabei der Produktionsprozess unterbrochen wird.

**Bearbeitungstyp**
Bearbeitungen werden in verschiedene Bearbeitungstypen zusammengefasst, z. B. Zuschnitt, Säumen, Polieren. Sie wählen den Bearbeitungstyp aus, zu dem die aktuelle Bearbeitung gehört.
Für den Stufungsartikel (Produktart Modell, Produktgruppe Stufung) muss der Bearbeitungstyp 99999 - Pseudobearbeitung ausgewählt werden.

**Schichtlage**
Einige Bearbeitungen können bei beschichteten Gläsern nur auf einer Seite ausgeführt werden. Dazu geben Sie an, wo die Schichtseite liegt.

**Plantext**
Der Plantext für Gläser wird in A+W Production angezeigt. Plantexte können auch mehrfach nach Priorität (Prio 1 ist hoch, 10 ist niedrig) übernommen werden.

**Planpriorität**
Priorität für die Übernahme des Plantextes.

**Sequenz**
Reihenfolge der Bearbeitung. Die Ziffer entscheidet, wann die Bearbeitung ausgeführt wird. Zuschneiden hat dabei die Ziffer 1, denn das ist immer der erste Arbeitsschritt bei einem Glas.

**Zuschlagsgruppe**
Zur Bearbeitung gehörende Maßzuschlagsgruppe für Kantenbearbeitungen. Die Zuschlagsgruppen werden in A+W Production angelegt und verwaltet.

**Zulässiger Teiletyp**
Zurzeit nicht genutzt.

---

## Produktverwaltung – Anlagen/Klassifikatoren

**Stammdaten > Produkte > Artikel > Artikel > Register Anlagen/Klassifikatoren**

*[Screenshot: Artikel 736/IG Sun4/12/4 A+W - Register Anlagen/Klassifikatoren]*

In diesem Register binden Sie externe Dateien ein, um weitere Informationen zum Produkt zur Verfügung zu stellen. Außerdem können Sie Klassifikatoren bearbeiten.
Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben.
- "Produktverwaltung - Produkt" auf Seite B-591

In der Produktsuche und in der Auftragssuche kann nach den Klassifikatoren gesucht werden.
Die Klassifikatoren werden immer auf der Ebene des Hauptprodukts angelegt. Sie werden bei der Erfassung mit in die Stücklistenelemente übernommen.

> **Beispiel**
> Wenn für das Float 104 der Klassifikator Geeignet für ISO mit dem Wert Ja eingetragen ist, übernehmen alle Produkte, die in der Stückliste das Produkt 104 enthalten, diesen Klassifikator, wenn im Auftrag eine entsprechende Position erfasst wird.
- "Partnerverwaltung - Klassifikatoren" auf Seite B-773
- Tutorial 1, "Klassifikator anlegen" auf Seite B-74

### Klassifikatoren
In der Übersicht werden alle Klassifikatoren angezeigt, die für das Produkt vergeben werden können.
- **A (alphanumerisch):** Um einen Wert einzutragen, öffnen Sie den Dialog **Klassifikatoren Wertzuordnung** mit einem Doppelklick in das Feld Wert.
  - "Klassifikatoren Wertzuordnung" auf Seite B-799
- **N (numerisch):** Den Wert können Sie direkt in das Feld Wert schreiben.
- **D (Datum):** Den Wert können Sie direkt in das Feld Wert schreiben.

### Dateianhang
In dieses Feld ziehen Sie die externe Datei, die Sie im Windows-Explorer markiert haben. Damit wird eine Verknüpfung hergestellt.
Die verknüpften Dateien dürfen nicht in einen anderen Ordner verschoben werden.

**Bemerkung**
In dieser Spalte können Sie eine Bemerkung zur verknüpften Datei eintragen oder auswählen, z. B. über den Inhalt.

### Leistungserklärung
Sie können dem Produkt eine Leistungserklärung zuweisen, die als Standard (Default) gesendet werden soll. Im Auftrag können Sie diese Leistungserklärung an der Position manuell überschreiben, z. B. nach einem Glasaustausch.

**Nummer**
Nummer der Leistungserklärung.

**Leistungserklärung erforderlich**
Für bestimmte Produkte kann eine Leistungserklärung erforderlich sein.
- **☐** Die Leistungserklärung muss nicht gesendet werden.
- **☑** Die Leistungserklärung muss gesendet werden.

---

## Produktverwaltung – Sprossen

**Stammdaten > Produkte > Artikel > Artikel > Register Sprossen**

*[Screenshot: Artikel 150134/CLIMAPLUS - Sprossenkonstruktion im ISO-Produkt]*

In diesem Register erfassen Sie eine Sprossenkonstruktion. Das gewählte Sprossenschema wird als Grafik angezeigt, sobald Sie in den Bereichen **Waagerechte, Senkrechte Sprossen** eine Sprosse ausgewählt haben.
Eine ausführliche Beschreibung der Daten, die Sie in diesem Register erfassen können, finden Sie im Part Verkauf:
- Verkauf, "Positionen - Sprossen" auf Seite C-493

---

## Technische Parameter

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen > Gruppe Technische Parameter > Technische Parameter allgemein, Technische Parameter Isolierglas**

*[Screenshot: Technische Parameter 150134 - CLIMAPLUS]*

In diesem Dialog tragen Sie die technischen Werte für Glas-Produkte ein.

### Abweichender Glasaufbau
- **1. Glas, 2. Glas, 3. Glas**: Bei einfachen Glas-Produkten bleiben diese Felder leer. Bei ISO-Produkten werden die jeweiligen Gläser eingetragen.
- **SZR, Gas**: Technische Werte pro ISO-Tabelle und SZR.
- **Bezeichnung**: Namen des Glasaufbaus.

### Technische Werte
Die nachfolgenden Feldbezeichnungen können Sie im Dialog **Systemtexte** an die Anforderungen in Ihrem Unternehmen anpassen (Systemtexte Nr. 111 - 118). Die Bezeichnungen gelten in den technischen Parametern in der Produktverwaltung und in der Produktsuche.
- "Systemtexte" auf Seite B-1046

**Ug-Wert in W/qm**
Wärmedurchgangskoeffizient (Systemtext 110). Der Ug-Wert ist die zentrale Maßeinheit beim Ermitteln des Wärmeverlusts eines Bauteils. Die Maßeinheit ist W/m² K. Je kleiner der Ug-Wert desto größer ist die Wärmedämmung.

**Ug-Wert nach DIN 4108-4**
Wärmedurchlasswiderstand

**Lichtdurchlässigkeit in %**
Lichtdurchlässigkeit. Die Lichtdurchlässigkeit drückt den direkt durchgelassenen sichtbaren Strahlungsanteil im Bereich der Wellenlänge von 280 bis 380 nm bezogen auf die Hellempfindlichkeit des menschlichen Auges aus. Die Bezugsgröße 100 % ist eine unverglaste Maueröffnung.

**g-Wert in %**
Gesamtenergiedurchlassgrad %. Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen infolge langwelliger Strahlung und Konvektion. Der g-Wert ist die sekundäre Kenngröße nach dem k-Wert.

**b-Faktor**
Mittlerer Durchlassfaktor. Er stellt den mittleren Durchlassfaktor der Sonnenenergie dar, bezogen auf den Gesamtenergiedurchlassgrad einer 4-mm-Scheibe. Er ist für die Kühllastberechnung eines Gebäudes notwendig.

**Schalldämmmaß in dB**
Das Schalldämmmaß ist die kennzeichnende Wirkung beim Schallschutz.

**Dickentoleranz in mm**
Die Dicke kann bei Isolierglas um wenige Millimeter differieren. Geben Sie den entsprechenden Wert für diese Toleranz mm an.

**Größentoleranz mm (<200 cm), (>=200 cm)**
Die Größe kann bei Isolierglas um wenige Zentimeter differieren. Geben Sie den entsprechenden Wert für die Toleranz in cm an.

**(Kombobox)**
Sie können einen Aufschlag auf den Ug-Wert aktivieren, wenn in der ISO-Scheibe Sprossen eingebaut werden. Zur Auswahl stehen folgende Einstellungen:
- **Keine Sprossen im SZR:** Auf den Ug-Wert wird kein Aufschlag berechnet.
- **Sprossen im SZR, einfach (+0.1):** Bei einem einfachen ISO mit Sprossen wird der Ug-Wert um 0,1 erhöht.
- **Sprossen im SZR, mehrfach (+0.2):** Bei mehrfachem ISO mit Sprossen wird der Ug-Wert um 0,2 erhöht.
Der Ug-Wert wird in der Auftragserfassung automatisch an die Sprossenanzahl angepasst.

---

## Technische Parameter kopieren

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen > Gruppe Technische Parameter > Technische Parameter kopieren**

*[Screenshot: Technische Parameter kopieren]*

In diesem Dialog kopieren Sie die technischen Werte und übertragen diese auf ein anderes Produkt.

### Optionen
Mit der Wahl der Option legen Sie fest, wie bereits vorhandene Parameter im Ziel-Produkt behandelt werden:
- **Vorhandene Parameter im Ziel updaten:** Wenn im Ziel-Produkt bereits Parameter vorhanden sind, werden diese überschrieben. Zusätzliche Parameter aus dem Quell-Produkt werden übernommen.
- **Alle Parameter im Ziel zuvor löschen:** Die Parameter im Ziel-Produkt werden gelöscht. Danach werden die Parameter aus dem Quell-Produkt eingetragen.

---

## Produktänderung

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen > Selektierte Produkte ändern**

*[Screenshot: Produktänderung - Zuordnung der automatischen Zuschläge ändern]*

In diesem Dialog ändern Sie die Zuordnung der automatischen Zuschläge. Die Zuordnungen gelten immer für alle Produkte, die im Register **Tabelle** angezeigt werden.

### Zuschläge/Rabatte
In diesem Bereich werden die Zuschläge und (Sonder-)Rabatte angezeigt, die im Dialog **Produktzuordnung Zuschläge** angelegt sind.
- "Produktzuordnung Zuschläge" auf Seite B-1029

Mit der Wahl der Option legen Sie fest, was mit den markierten Zuschlägen/Rabatten gemacht werden soll:
- **Setzen:** Die markierten Zuschläge oder Rabatte werden in den allen Produkten aktiviert, die in der Produktverwaltung ausgewählt sind.
- **Löschen:** Die markierten Zuschläge oder Rabatte werden in den allen Produkten deaktiviert, die in der Produktverwaltung ausgewählt sind.

---

## Produktkennzeichen Verwaltung

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf [Abweichende Produktkennzeichen]**

In diesem Dialog definieren Sie abweichende Beschaffungsarten, wenn Sie mit internen Aufträgen und Verrechnungen arbeiten. Dazu müssen die entsprechenden Mandanten und/oder AV-Bereiche angelegt sein.
- "Firmendaten - Mandant" auf Seite B-919
- "AV-Bereiche" auf Seite B-1019

In diesem Dialog finden Sie folgende Register:
- Produktkennzeichen Verwaltung – Editieren
- Produktkennzeichen Verwaltung - Kopieren

### Produktkennzeichen Verwaltung - Editieren

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf [Abweichende Produktkennzeichen] > Editieren**

*[Screenshot: Produktkennzeichen Verwaltung – Editieren]*

In diesem Register können Sie die Produktkennzeichen anlegen und bearbeiten.

#### Produkt
In dieser Gruppe werden die Produktnummer und die Bezeichnungen des aktuellen Produkts angezeigt.

#### Bereich, Kennzeichen
Sie können die Beschaffungsart für unterschiedliche Mandanten und/oder AV-Bereiche festlegen.

> **Beispiel**
> Die AV-Bereiche ISO, VSG und ESG arbeiten untereinander mit internen Aufträgen. Alle AV-Bereiche benutzen dieselbe Datenbank mit denselben Stammdaten usw.
> Im AV-Bereich ISO wird ein Kundenauftrag erfasst, in dem ein VSG mit ESG, ein SZR und ein Float die Komponenten einer ISO-Einheit bilden.
> - Für den AV-Bereich ISO ist das ISO Produktion, das VSG eine Bestellung, das Float aber Zuschnitt.
> - Für den AV-Bereich VSG ist das VSG Produktion, das ESG eine Bestellung, das Float ebenfalls Zuschnitt.
> - Für den AV-Bereich ESG ist das ESG Produktion, das Float ebenfalls Zuschnitt.
> Die unterschiedlichen Beschaffungsarten für VSG und ESG müssen daher als abweichende Produktkennzeichen definiert werden.

**Mandant**
Mandant, für den die abweichenden Kennzeichen gelten.

**AV-Bereich**
AV-Bereich, für den die abweichenden Kennzeichen gelten.

**Beschaffungsart**
Abweichende Beschaffungsart für den eingestellten Mandanten oder AV-Bereich.

**Lagerbuchungsart**
Abweichende Lagerbuchungsart für den eingestellten Mandanten oder AV-Bereich.

**Gültig in**
Mit der Wahl der Option legen Sie fest, wo die Einstellungen gelten sollen:
- **Sonstige:** Die Zuordnung beschränkt sich nicht auf die eine der beiden anderen Optionen.
- **Auftragserfassung:** Die Einstellungen gelten für die Auftragserfassung. Siehe dazu das Beispiel.
- **Profitcenter:** Die Suche nach dem Kennzeichen beschränkt sich auf einen Mandanten oder einen AV-Bereich. Dazu muss in den Firmendaten > Register Produktion die Profit-Center-Abrechnung aktiviert sein.
- **Suche über alles:** Die Option ist nur im Auswahl-Modus freigeschaltet. Die Suche wird mit dieser Option nicht weiter eingeschränkt.

#### Übersicht
In der Übersicht werden alle Produkte angezeigt, für die abweichende Kennzeichen angegeben sind.

### Produktkennzeichen Verwaltung – Kopieren

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf [Abweichende Produktkennzeichen] > Kopieren**

*[Screenshot: Produktkennzeichen Verwaltung – Kopieren]*

In diesem Register kopieren Sie die Einstellungen eines Produktes zu einer Warengruppe und/oder zu einer Folge von Produkten.

#### Quelle
In diesem Bereich werden die Daten des ausgewählten Produkts angezeigt. Die Felder sind zum Register **Editieren** beschrieben.
- "Produktkennzeichen Verwaltung - Editieren" auf Seite B-632

#### Ziel
In diesem Bereich geben Sie an, worauf das Produktkennzeichen übertragen werden soll. Sie müssen mindestens eine Warengruppe oder eine Produktart angeben.

**Warengruppe**
Sie können eine WGR, WHG oder WOG auswählen.

**Produktart, Produktgruppe**
Wenn Sie eine Produktart ausgewählt haben, können Sie zusätzlich eine Produktgruppe angeben.

**Produkt von, bis**
Sie können ein einzelnes Produkt auswählen, indem Sie in beiden Feldern dieselbe Produktnummer angeben. Wenn Sie unterschiedliche Produktnummern angeben, wird das Produktkennzeichen auf alle Produkte zwischen der ersten und der zweiten Nummer übertragen.

**Mandat**
Mandant, auf dessen Produkte das abweichende Kennzeichen übertragen werden soll.

**AV-Bereich**
AV-Bereich, auf dessen Produkte das abweichende Kennzeichen übertragen werden soll.
Zusätzlich können Sie die Zuordnung zu wählen:
- **Sonstige:** Die Zuordnung beschränkt sich nicht auf die eine der beiden anderen Optionen.
- **Auftragserfassung:** Die Einstellungen gelten für die Auftragserfassung.
- **Profitcenter:** Die Einstellungen gelten für einen Mandanten oder einen AV-Bereich. Dazu muss in den Firmendaten > Register Produktion die Profit-Center-Abrechnung aktiviert sein.

---

## Glasarten

**Stammdaten > Produkte > Artikel > Artikel > Register A+W Production > Ordner [Glasart]**

*[Screenshot: Glasarten Dialog]*

In diesem Dialog tragen Sie alle relevanten Daten zur aktuellen Glasart ein. Die Glasarten können in folgenden Dialogen zugeordnet werden:
- **Produktverwaltung:** Wenn Sie einem Glasprodukt eine Glasart zuordnen, werden die Felder **Produktart** und **Produktgruppe** deaktiviert und können nicht mehr verändert werden.
  - "Produktverwaltung - A+W Production" auf Seite B-621
- **Glasart-Jumbo-Tische:** Jeder Glasart kann ein Schneidetisch zugeordnet werden, damit die Schnitte korrekt ausgeführt werden. Einem VSG muss z. B. der Tisch zugeordnet werden, der diese Glasart schneiden kann.
  - "Glasart-Jumbos-Tische" auf Seite B-873

### Werte
- **Glasart**: Nummer der Glasart. In der Regel entspricht die Glasartnummer der A+W Business-Artikelnummer.
- **Bezeichnung**: Name der Glasart.
- **Produktgruppe**: Produktgruppe und Produktart, zu der die Glasart gehört.
- **Glasartgruppe**: Glasartgruppe, zu der die Glasart gehört.
- **Struktur**: Strukturverlauf der Glasart.
- **Beschichtung**: Beschichtungsart der Glasart.

### Tabelle
In der Übersicht werden alle definierten Glasarten (aus A+W Enterprise) aufgelistet.

---

# Artikel

**Stammdaten > Produkte > Artikel**

In A+W Business können Sie Ihre firmeneigenen Produkte definieren und Daten für die Produktion hinterlegen.

Im Menü **Artikel** finden Sie zusätzlich zur Produktverwaltung folgende Einträge:
- "Lagermaße" auf Seite B-637
- "Maßzuschlag" auf Seite B-641
- "Produktvarianten" auf Seite B-643
- "EK-Kalkulation" auf Seite B-647
- "Abstandhalterrestriktionen" auf Seite B-649
- "Template Editor" auf Seite B-651
- "ISO-Aufbau" auf Seite B-652
- "Bearbeitungsrestriktionen" auf Seite B-654
- "Motive" auf Seite B-655
- "Modellkantenqualitäten" auf Seite B-656
- "Beschlagszuordnung" auf Seite B-657
- "iTOE Regeln" auf Seite B-659

## Lagermaße

**Stammdaten > Produkte > Artikel > Lagermaße**

Sie können für die Preisfindung die Lagermaße anlegen. Diese Lagermaße sind unabhängig von den Lagerartikeln, die in der Lagerverwaltung gepflegt werden.

In diesem Kapitel finden Sie folgende Informationen:
- Menü Funktionen
- Lagermaße - Produkt
- Lagermaße - Tabelle

### Menü Funktionen
Über dieses Menü können Sie den Dialog **Lagerverwaltung** öffnen, um das ausgewählte Produkt auch als Lagermaß (Lagerartikel) für die Lagerverwaltung anzulegen.
- Lagerwirtschaft, "Lagerverwaltung" auf Seite G-185

### Lagermaße – Produkt

**Stammdaten > Produkte > Artikel > Lagermaße > Register Produkt**

*[Screenshot: Produktverwaltung Lagermaße – Produkte]*

In diesem Register legen Sie die Lagermaße für die Preisfindung an. Sie können hier auch Lagermaße anlegen, die im Lager selbst nicht geführt werden. Sie können jedem Lagermaß einen Preisschlüssel VK und EK sowie eine Warengruppe zuordnen.

> **Lagerverwaltung**
> Die Lagermaße für die Lagerverwaltung werden im Dialog **Lagerverwaltung** (Modul Lagerwirtschaft) angelegt. Eine ausführliche Beschreibung der Lagermaße finden Sie im Part Lagerwirtschaft:
> - Lagerwirtschaft, "Lagermaße" auf Seite G-42
> - Lagerwirtschaft, "Lagerverwaltung" auf Seite G-68

#### Artikel
In dieser Gruppe werden die Artikelnummer (Produktnummer) und die Bezeichnung zum aktuellen Produkt angezeigt.

#### Einheiten / Restriktionen
**Inh./Breite/Höhe**
Für Kisten geben Sie die Anzahl der Blätter an. Breite und Höhe tragen Sie in mm ein.

**WGR, WGR-Statistik**
Jedem Lagermaß bzw. jeder Kiste können unterschiedliche Warengruppen zugeordnet werden.
- Tutorial 1, "Warengruppen" auf Seite B-142

#### Preis
**Preisschl. VK, Preisschl. EK**
Zur Auswahl werden alle Preisschlüssel für den Verkauf (VK) und den Einkauf (EK) angeboten, die in den Stammdaten für Preise hinterlegt sind.
Für Kisten sollte ein eigener Preisschlüssel angelegt sein.

**EK Suche Lager**
Ein Produkt kann in die Ermittlung des durchschnittlichen Einkaufspreises einbezogen werden.
- **☐** Bei der Ermittlung des Durchschnittspreises wird das Produkt nicht berücksichtigt.
- **☑** Bei der Ermittlung des Durchschnittspreises wird das Produkt mitberücksichtigt.
- Lagerwirtschaft, "Einkaufspreis und Durchschnitts-EK" auf Seite G-52

#### Bezeichnung
**Bezeichnung, Kurzbezeichnung**
Name und Kurzbezeichnung zur (besseren) Unterscheidung vom Bandmaß. Die Bezeichnungen werden in der Auftragserfassung angezeigt, z. B. `Kiste Float 4 LM`. Dies wird als Produktname im Formular gedruckt.

#### Kennzeichen
**Beschaffungsart**
Die Beschaffungsart legt fest, wie das Produkt für den Auftrag beschafft wird.
- **Produktion:** Das Lagermaß wird produziert. Wenn ein Hauptartikel mit dieser Beschaffungsart gekennzeichnet ist, können dessen Stücklisten-Komponenten als Lagerartikel oder als Bestellartikel definiert werden.
  - Tutorial 1, "Beschaffungsart" auf Seite B-171
- **Zuschnitt:** Das Glas wird aus Lagerplatten zugeschnitten.
- **Lagerentnahme:** Das Produkt wird als Lagerartikel mit seinen genauen Abmessungen oder als Stückartikel im Lager geführt.
- **Bearbeitung:** Die Bearbeitungen für eine Auftragsposition werden an die Produktion übergeben.
- **Kundeneigenes Glas:** Das Produkt wird vom Kunden angeliefert und für die Produktion seiner Aufträge verwendet.
- **Bestellung:** Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste zu beachten.
- **Bestellung (komplett):** Das Produkt wird inklusive aller Bearbeitungen bestellt.
- **Lagerzugang durch Produktion:** Das Produkt soll nur in Produktionsaufträgen verwendet werden, um das Lager zu füllen. Die produzierten Positionen werden dem Lager zugebucht.
  - Tutorial, "Produktionsaufträge" auf Seite E-130

Die Beschaffungsarten sind ausführlich zu den Produktstammdaten erklärt.
- "Produktverwaltung - Lager/Einkauf" auf Seite B-608

#### Fremdschlüssel Statistik
**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

#### Verfügbare Lagermaße
In der Übersicht werden alle Lagermaße zur aktuellen Produktnummer angezeigt. Diese Lagermaße werden zur Preisfindung herangezogen.

### Lagermaße – Tabelle

**Stammdaten > Produkte > Artikel > Lagermaße > Register Tabelle**

*[Screenshot: Produktverwaltung Lagermaße – Tabelle]*

In diesem Register werden alle Produkte angezeigt, die den Suchkriterien im Auswahlmodus entsprechen. Die Beschreibungen der Felder gelten für beide Register. Die Felder sind ausführlich zum Register **Produkt** beschrieben.
- "Lagermaße – Produkt" auf Seite B-638

## Maßzuschlag

**Stammdaten > Produkte > Artikel > Maßzuschlag**

Sie können Tabellen für maßabhängige Zuschläge anlegen und pro Tabelle verschiedene Zuschlagsstufen angeben.

Im Dialog **Maßzuschlag** finden Sie folgende Register:
- Maßzuschlag – Maßzuschläge
- Maßzuschlag - Tabelle

### Maßzuschlag – Maßzuschläge

**Stammdaten > Produkte > Artikel > Maßzuschlag > Register Maßzuschläge**

*[Screenshot: Produktverwaltung Maßzugaben/Maßabzüge – Maßzuschläge]*

In diesem Register legen Sie die Stufen für maßabhängige Zu- und Abschläge an.

Mit der Wahl der Option legen Sie fest, wie die Tabelle ausgewertet werden soll.
- **Zugabentabelle:** Eine Maßzugabe gleicht den Materialverlust aus, der bei einer Bearbeitung entsteht. Diese Zugabe wird beim Zuschnitt berücksichtigt.
- **Abzugstabelle:** Ein Maßabzug wird z. B. bei Bilderrahmen gebraucht.

> **Beispiel**
> Durch Polieren aller vier Kanten reduziert sich ein Float von 1000 x 1000 mm auf die Maße 998 x 998 mm.
> Als Maßzuschlag müssen 2 mm zugegeben werden. Dieser Wert wird der zugeordneten Tabelle entnommen, wobei die Dicke des Glases berücksichtigt wird.

Die Maßzuschläge werden in der Produktverwaltung bei den Produkten der Produktart Bearbeitung zugewiesen (nicht bei den Gläsern).
- "Produktverwaltung - Fertigung" auf Seite B-596

#### Tabelle (Übersicht)

**Bis Dicke**
Pro Tabelle können Sie stufenweise angeben, bis zu welcher Dicke ein bestimmter Wert zugegeben werden soll.

**Wert**
Der Wert gibt den Zuschlag in mm an, der bei der entsprechenden Dicke zu- oder abgerechnet werden muss.

### Maßzuschlag – Tabelle

**Stammdaten > Produkte > Artikel > Maßzuschlag > Register Tabelle**

*[Screenshot: Produktverwaltung Maßzugaben/Maßabzüge – Tabelle]*

In diesem Register legen Sie neue Tabellen für maßabhängige Zu- oder Abschläge an.

---

## Produktvarianten

**Stammdaten > Produkte > Artikel > Produktvarianten**

Sie können Produktvarianten zu den Produkten anlegen, z. B. zu Abstandhaltern, Sprossen, Stückartikeln. Gläsern werden keine Farben zugeordnet. Die verschiedenen Glasfarben werden über unterschiedliche Produkte abgebildet.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite B-643
- "Produktvarianten - Varianten" auf Seite B-643
- "Produktvarianten - Tabelle" auf Seite B-645

### Menü Funktionen
Über dieses Menü öffnen Sie den Dialog **Varianten kopieren**, in dem Sie die Produktvarianten eines Produktes auf ein anderes Produkt übertragen.
- "Varianten kopieren" auf Seite B-646

### Produktvarianten – Varianten

**Stammdaten > Produkte > Artikel > Produktvarianten > Register Varianten**

*[Screenshot: Produktvarianten - Varianten]*

In diesem Register legen Sie zu den Produkten aus der Produktverwaltung verschiedene Varianten an, z. B. andere Farben, unterschiedliche Polierungen oder Mattierungen usw. Jeder Produktvariante können Sie eine Preistabelle zuweisen.
- Tutorial 1, "Produktvariante anlegen" auf Seite B-207

#### Produkt
- **Nummer**: Produktnummer oder Spanne von Produktnummern, für die die Farbe gilt.
- **EAN**: Der EAN-Code wird nur angezeigt, wenn ein einzelnes Produkt markiert ist.
- **Bezeichnung**: Anzeige von Name und Beschreibung des Produkts.
- **Produktart, Produktgruppe**: Anzeige der Produktart und der Produktgruppe, die dem Produkt zugewiesen sind.
  - "Produktverwaltung - Produkt" auf Seite B-591

#### Variante
- **Nr./Variante**: Nummer und Bezeichnung der Variante aus dem Dialog **Varianten**.
  - "Varianten" auf Seite B-572
- **Preistabelle**: Sie können pro Produkt und Variante unterschiedliche Preistabellen angeben.
  - "Preise" auf Seite B-714
- **Gewicht**: Spezifisches Gewicht der Variante, wenn sich das Gewicht der Variante von dem des Produktes unterscheidet. In der Regel spielt das Gewicht für die Produkte mit Varianten keine Rolle und steht daher standardmäßig auf null.
- **Default**: Wenn eine bestimmte Produktvariante häufig verlangt wird, kann sie in der Auftragserfassung standardmäßig zuerst angezeigt werden.
  - **☐** Die Produktvariante wird nicht standardmäßig zuerst angezeigt.
  - **☑** Die Produktvariante wird automatisch zur Erfassung vorgeschlagen. Der Vorschlag kann in der Auftragserfassung überschrieben werden.
- **Gesperrt**: Eine Variante kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
  - **☐** Die Variante kann zugewiesen werden.
  - **☑** Die Variante ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.
  - Tutorial 1, "Sperren" auf Seite B-34
- **WGR, WGR-Statistik**: Jeder Produktvariante können unterschiedliche Warengruppen zugeordnet werden.
  - Tutorial 1, "Warengruppen" auf Seite B-142

#### Kennzeichen, Beschaffungsart
Die Beschaffungsart der Produktvariante kann sich von derjenigen des Produkts unterscheiden.
- Tutorial 1, "Beschaffungsart" auf Seite B-171

#### Abstandhalterkennzeichen
Bei Produkten der Produktgruppe **Abstandhalter** können Sie weitere Kennzeichen festlegen. Das Abstandhalterkennzeichen aus den Varianten übersteuert das Kennzeichen aus den Produktstammdaten.
- **Frei**: Zurzeit nicht genutzt.
- **Farbe**: Die Farbe wird von A+W Production vorgegeben.

#### Verfügbare Produktvarianten
In der Übersicht werden pro Produkt alle Varianten mit den zugeordneten Preistabellen aufgelistet.

### Produktvarianten – Tabelle

**Stammdaten > Produkte > Artikel > Produktvarianten > Register Tabelle**

*[Screenshot: Produktvarianten - Tabelle]*

In diesem Register werden alle Produktvarianten angezeigt, die den Suchkriterien im Auswahlmodus entsprechen.
Die Felder sind zum Register **Varianten** beschrieben.
- "Produktvarianten - Varianten" auf Seite B-643

---

## Varianten kopieren

**Stammdaten > Produkte > Artikel > Produktvarianten > Menü Funktionen > Varianten kopieren**

*[Screenshot: Produktvarianten kopieren]*

In diesem Dialog übertragen Sie die Varianten eines Produktes auf ein anderes Produkt.

### Quelle, Ziel
In diesen Feldern geben Sie an, aus welchem Produkt die Varianten kopiert und auf welches diese übertragen werden sollen.

### Vorhandene Einträge überschreiben
Wenn zu dem Ziel-Produkt bereits Varianten angelegt sind, müssen Sie entscheiden, ob Sie diese behalten oder überschreiben wollen.
- **☐** Die vorhandenen Varianten werden beibehalten und durch die neuen Varianten aus dem Quell-Produkt ergänzt. Gleiche Variantennummern werden nicht überschrieben.
- **☑** Die Varianten im Ziel-Produkt werden mit den Varianten aus dem Quell-Produkt überschrieben. Zusätzliche Varianten werden hinzugefügt. Vorhandene Varianten werden nicht gelöscht.

---

## EK-Kalkulation

**Stammdaten > Produkte > Artikel > EK-Kalkulation**

*[Screenshot: EK-Kalkulationsvorgaben – Stückliste]*

In diesem Dialog hinterlegen Sie Vorgaben für Kalkulation der Eigenkosten für Isolierglas (ISO). Pro Abstandhalter (SZR) legen Sie den durchschnittlichen Verbrauch von Butyl, Thiokol, etc. fest.
Im Register **Stückliste** geben Sie die Werte für die EK-Kalkulation an.

### SZR - Artikel
- **Artikel/MCode, Bezeichnung**: Nummer, Matchcode und Bezeichnung des Abstandhalters, zu dem die Eigenkalkulation durchgeführt wird.
- **Rückschnitt (einfach)**: Rückschnitt für den Abstandhalter.
- **Entspannte Menge für Gas**: Entspannte Menge für das Schallschutzgas lt. Herstellerangaben.

### Stücklistenprodukt
In diesem Bereich werden die Details zu den Produkten angezeigt, die mit dem SZR zusammen verbraucht werden.
- **Produkt**: Nummer des Produktes.
- **Bezeichnung, Mengeneinheit**: Anzeige der Bezeichnung und der Mengeneinheit, z. B. für Butyl.
- **Verbrauch pro - Bezugseinheit**: Menge und Einheit, auf die sich die verbrauchte Menge bezieht.

> **Beispiel**
> Mengeneinheit (Butyl): kg
> Verbrauch: 0,0055
> Bezugseinheit: Lfm
> Berechnung: Pro Meter Abstandhalter werden 0,0055 kg Butyl verbraucht.
- Tutorial 2, "Komplexbeispiel: Kalkulation ISO" auf Seite B-547

### Stückliste
In der Übersicht sind alle Produkte aufgeführt, die als Komponenten zu einem Abstandhalter hinzugefügt wurden. Daten werden nur angezeigt, wenn im Bereich **Tabelle** ein Abstandhalter markiert ist.

### Tabelle (Übersicht)
Übersicht über alle Produkte, die den Suchkriterien im Auswahlmodus entsprechen, bzw. für die ein bestimmter Verbrauch an Butyl, Trockenmittel, Randverbund usw. hinterlegt wurde.

---

## Abstandhalterrestriktionen

**Stammdaten > Produkte > Artikel > Abstandhalterrestriktionen**

*[Screenshot: Abstandhalterrestriktionen]*

In diesem Dialog hinterlegen Sie die Einschränkungen (Restriktionen) für bestimmte Abstandhalter. Bei TPS-Isolierglas (Thermo Plastic Spacer) können nicht alle Aufbauten ausgeführt werden, die für das herkömmliche ISO-Glas verwendet werden.
Wenn bei der Erfassung eines Auftrags die Restriktionen verletzt werden, muss auf ein anderes Produkt ausgewichen werden.

### Identifikation
- **Produktgruppe**: In der Regel sind die Abstandhalterrestriktionen für TPS-ISO notwendig. Es können jedoch auch andere Produktgruppen ausgewählt werden.
- **Passwort**: Wenn ein Passwort hinterlegt ist, kann die Restriktion im Auftrag überschrieben werden. In diesem Fall wird das Passwort bei der Erfassung des Auftrags abgefragt. Ist kein Passwort hinterlegt, wird im Auftrag automatisch auf den Ausweichartikel zugegriffen, der in der Gruppe **Bei Verletzung des Gültigkeitsbereichs ausweichen auf** angegeben ist.
- **Regel**: Die hinterlegten Regeln sind mit Variablen definiert, deren Werte aus den Feldern für Parameter gezogen werden. Dabei gilt [N1], [N2] und [N3] für die Parameter 1 bis 3. Die Regeln sind fest hinterlegt. Wenn Sie zusätzliche Regeln brauchen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

### Gültigkeitsbereich
- **Parameter 1 - 3**: Felder für die Werte, die über Variablen in die Regel eingefügt werden. Die Felder werden entsprechend der ausgewählten Regel freigeschaltet. Wenn eine Regel ohne Variablen ausgewählt wurde, sind keine Felder freigeschaltet, z. B. bei Regel 3114 - Bei Modellen darf keine Sprosse vorhanden sein. Bei bestimmten Regeln steht für Parameter 1 eine Kombobox zur Verfügung, aus der die entsprechende Einschränkung ausgewählt werden kann.

### Bei Verletzung des Gültigkeitsbereichs ausweichen auf
Wenn die gesetzten Parameter verletzt werden, kann auf ein Ausweichprodukt zugegriffen werden.
- **Produktgruppe**: Auswahlliste der Produktgruppe, auf die ausgewichen werden kann, wenn die Restriktion verletzt wird.
- **Variante**: Zusätzlich zur Produktgruppe kann auch eine Variante für den Ausweichartikel festgelegt werden.

### Restriktionen
Übersicht über die definierten Restriktionen mit den hinterlegten Parametern.

---

## Template Editor

**Stammdaten > Produkte > Artikel > Template Editor**

*[Screenshot: Template Editor]*

In diesem Dialog können Sie ein Template für die Modellerfassung auswählen. Mit dem Editor können Sie Vorlagen von A+W CAD Designer (Shapes) bearbeiten oder neue Vorlagen für die Bearbeitung erstellen.

### Verzeichnis
Sie können die Templates (Vorlagen) in verschiedenen Verzeichnissen verwalten. Das jeweils zuletzt genutzte wird automatisch angezeigt.

### Templates
Die Templates werden angezeigt, die im ausgewählten Verzeichnis gespeichert sind.

> **Handbuch für A+W CAD Designer**
> Für die Arbeiten mit A+W CAD Designer stehen eine separate Online-Hilfe und ein separates Handbuch zur Verfügung.

---

## ISO-Aufbau

**Stammdaten > Produkte > Artikel > ISO-Aufbau**

*[Screenshot: ISO Aufbau]*

In diesem Dialog hinterlegen Sie Schlüsselnummern für einen eindeutigen Aufbau von ISO-Scheiben.
Die Nummern können in den Rahmentext gedruckt werden. Anhand dieser Schlüsselnummer kann der Aufbau einer fertig produzierten ISO-Einheit unabhängig vom zugehörigen Auftrag ermittelt werden.
Der Dialog ist nur freigeschaltet, wenn in den **Firmendaten > Register Dokumente** die Funktion **Gütekennzeichen** aktiviert ist.
- "Produktkennzeichnung" auf Seite B-934

### Schlüsselnummer
Schlüsselnummer, die für den entsprechenden ISO-Aufbau vergeben werden soll.

### Glasaufbau
- **1. Glas, 2. Glas, 3. Glas**: Produktnummern der Gläser, aus denen das 2-fach bzw. 3-fach Isolierglas zusammengesetzt ist.
- **SZR Dicke**: Breite des Abstandhalters.
- **Gas**: Gastyp, wenn der Scheibenzwischenraum des Isolierglases mit Gas gefüllt ist.

> **Feldbezeichnungen anpassen**
> Die nachfolgenden Feldbezeichnungen können Sie im Dialog **Systemtexte** an die Anforderungen in Ihrem Unternehmen anpassen (Systemtexte Nr. 111 - 118).
> - "Systemtexte" auf Seite B-1046

- **Ug-Wert in W/m²**: Wärmedurchgangskoeffizient. Der Ug-Wert ist die zentrale Maßeinheit beim Ermitteln des Wärmeverlustes eines Bauteils. Die Maßeinheit ist W/m² K. Je kleiner der Ug-Wert desto größer ist die Wärmedämmung.
- **g-Wert in %**: Gesamtenergiedurchlassgrad in %. Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen infolge langwelliger Strahlung und Konvektion. Der g-Wert ist die sekundäre Kenngröße nach dem k-Wert.
- **b-Faktor**: Mittlerer Durchlassfaktor. Er stellt den mittleren Durchlassfaktor der Sonnenenergie dar, bezogen auf den Gesamtenergiedurchlassgrad einer 4-mm-Scheibe. Die ist für die Kühllastberechnung eines Gebäudes notwendig.

### Tabelle (Übersicht)
Übersicht über alle Datensätze für ISO-Aufbauten. Wenn Sie einen Datensatz markieren, werden die Felder im Bereich **Glasaufbau** gefüllt.

---

## Bearbeitungsrestriktionen

**Stammdaten > Produkte > Artikel > Bearbeitungsrestriktionen**

*[Screenshot: Bearbeitungsrestriktionen]*

In diesem Dialog legen Sie die Regeln fest, die für Bearbeitungen bei bestimmten Produktgruppen gelten sollen.
Wenn bei der Erfassung eines Auftrags die Restriktionen verletzt werden, wird eine Meldung ausgegeben, auf die der Mitarbeiter in geeigneter Weise reagieren muss.

### Zuweisung
- **Produktgruppe**: In der Regel gelten Restriktionen für Bearbeitungen von ESG- oder VSG-Scheiben. Es können jedoch auch andere Produktgruppen ausgewählt werden.
- **Glasdicke**: Glasdicke, für die die Restriktion gilt. Wenn für eine Produktgruppe abhängig von der Glasdicke unterschiedliche Restriktionen gelten, müssen Sie für jede Glasdicke eine entsprechende Regel hinterlegen.
- **Regel**: Die hinterlegten Regeln sind mit Variablen definiert, deren Werte aus den Feldern für Parameter gezogen werden. Dabei gilt [p1], [p2] bis [p5] für die Parameter 1 bis 5.
- **Parameter 1-5**: Felder für die Werte, die über die Variable in die Regel eingefügt werden. Die Felder werden entsprechend der ausgewählten Regel freigeschaltet. Wenn eine Regel ohne Variablen ausgewählt wurde, sind keine Felder freigeschaltet, z. B. bei Regel 201 - Rest der Kante >= Ausschnitttiefe.
- **Level**: Mit der Wahl der Option legen Sie fest, wie A+W Business bei einer Verletzung der Restriktionen reagieren soll:
  - **Info:** In der Positionserfassung wird nur eine Information angezeigt.
  - **Warnung:** In der Positionserfassung wird eine Warnung angezeigt. Der Anwender sollte dann die Details der Bearbeitung oder das Glas ändern.
  - **Fehler:** In der Positionserfassung wird eine Fehlermeldung angezeigt. Die Bearbeitung und die Position können nicht gespeichert werden. Der Anwender muss dann die Details der Bearbeitung oder das Glas ändern.

### Restriktionen
Übersicht der definierten Restriktionen mit den hinterlegten Parametern.

---

## Motive

**Stammdaten > Produkte > Artikel > Motive**

*[Screenshot: Motive Dialog]*

In diesem Dialog legen Sie Motive für Beschichtungen, Siebdrucke, Sandstrahlen, Emaillierungen, Kolorieren und Mattierungen an. Die angelegten Motive können Sie im Auftrag in der Positionserfassung im Register **Modelle/Bearbeitungen** über die Siebnummer einfügen.
- "Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlen, Kolorieren" auf Seite C-478

### Motiv
- **Siebnummer**: Nummer des Siebs.
- **Name**: Name des Motivs. Er sollte eindeutig und sprechend sein.
- **Datei**: Pfad und Name der Motivdatei. Eine Vorschau des Motivs wird in dem Rahmen in der rechten oberen Ecke des Dialogs angezeigt.
- **Max. Abmessungen**: Angabe der maximalen Breite und Höhe des Siebs in mm. Sie können Breite und Höhe des Motivs im Auftrag in der Positionserfassung im Register **Modelle/Bearbeitungen** bis zu dem angegebenen Maximalwert anpassen.

### Tabelle
Übersicht der definierten Motive mit den hinterlegten Parametern.

---

## Modellkantenqualitäten

**Stammdaten > Produkte > Artikel > Modellkantenqualitäten**

*[Screenshot: Modellkantenqualitäten]*

In diesem Dialog weisen Sie den einzelnen Kanten der verschiedenen Modelle bestimmte Kantenqualitäten zu.

### Selektion
- **Produkt**: Nummer und Bezeichnung der Bearbeitungsart.
- **Modell**: Nummer des Modells, dessen Kanten bearbeitet werden sollen. Standardmodelle verwenden die Modell-Nr. 1 – 99, das Modell für Stufen-Isolierglas hat die Nummer 999.

### Kantenqualitäten
**Segment 1-8**
Angabe der Kantenqualität pro Modellsegment. Die Felder sind je nach Kantenanzahl des Modells freigeschaltet. Die zugehörige Nummerierung der Segmente wird in der Grafik mit den roten Zahlen angezeigt.

### Tabelle
Übersicht der definierten Modelle mit den hinterlegten Parametern.

---

## Beschlagszuordnung

**Stammdaten > Produkte > Artikel > Beschlagszuordnung**

*[Screenshot: Beschlagszuordnung]*

In diesem Dialog legen Sie die Bearbeitungen fest, die für die Anbringung von Beschlägen an einer Glasscheibe notwendig sind. Wenn ein Beschlag im Auftrag in der Positionserfassung in die Stückliste eingefügt wird, werden die zugehörigen Bearbeitungen und Bearbeitungsparameter in die Stückliste übernommen. Wenn der Beschlag im Auftrag aus der Stückliste gelöscht oder geändert wird, werden auch die zugehörigen Bearbeitungen gelöscht oder geändert.

### Identifikation
- **Beschlag**: Nummer und Bezeichnung des Beschlags.
- **Anbringung**: Anbringungstyp des Beschlags.
- **Priorität Anbringung**: Reihenfolge, in der Beschläge mit derselben Produktnummer angebracht werden sollen. Wenn Beschläge im Auftrag in der Positionserfassung mehrfach in die Stückliste eingefügt werden, werden die Bearbeitungszuordnungen nach Priorität geordnet, z. B. wird Türband oben mit der Prioritätsnummer 1 an erster Stelle angezeigt, Türband mitte mit der Nummer 2 an zweiter Stelle, usw.
- **Bandseite**: Seite, an der das Band angebracht werden soll. Sie können zwischen **Links**, **Rechts** und **Beide** wählen.
  - **Links:** Das Band wird links angebracht.
  - **Rechts:** Das Band wird rechts angebracht.
  - **Beide:** Das Band kann an beiden Seiten angebracht werden.
- **Bearbeitung**: Anzeige der Bearbeitungsart. Im Bereich **Parameter** können Sie die Bearbeitungsparameter ändern.
- **Austausch**: Austauschbeschlag, der optional angegeben werden kann. Als Austauschbeschlag können z. B. Beschläge gewählt werden, die unterschiedliche Produktnummern für eine andere Bandseite haben. Die Bezeichnung des Austauschbeschlags wird nach Eingabe der Produktnummer automatisch angezeigt.

### Bearbeitungen
Über die Schaltfläche **[Einfügen]** können Sie Bearbeitungen an der Glasscheibe hinzufügen, die bei der Anbringung des ausgewählten Beschlags nötig werden. Im Bereich **Parameter** können Sie die zugehörigen Bearbeitungsparameter anpassen. Über die Schaltfläche **[Löschen]** können Sie Bearbeitungen entfernen.

### Parameter
Die angezeigten Felder unterscheiden sich je nach der Bearbeitung, die Sie gewählt haben.
Die Parameter sind ausführlich im Part **Verkauf** beschrieben.
- Verkauf, "Parameter" auf Seite C-469

> **Formeln statt Werte**
> Sie können in den Bearbeitungsparametern statt Werten auch Formeln eintragen.
>
> **Beispiel**
> Sie können z. B. für eine Griffstange in den Parametern Bohrung 1 [x/y], Bohrung 2 [x/y] auch Formeln eintragen.
> Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

### Beschläge
In der Übersicht werden alle angelegten Beschläge angezeigt, die den Suchkriterien entsprechen.

---

## iTOE Regeln

**Stammdaten > Produkte > Artikel > iTOE Regeln**

*[Screenshot: iTOE Regeln]*

In diesem Dialog legen Sie die Regeln für den Import von SN-Dateien mit Bearbeitungen (TOE = Technical Order Entry) fest. Jeder Bearbeitung aus dem A+W CAD Designer muss die entsprechende Bearbeitung in A+W Business zugeordnet werden.

> **Voraussetzungen**
> Das linzenzpflichtige TOE-Modul setzt das Datenbanksystem Microsoft SQL Server 2016 voraus. Wenn Sie sich an die A+W Software GmbH, wenn Sie das Modul einsetzen wollen.

### SN-Bearbeitungen
In diesem Bereich wählen Sie die Bearbeitungen aus, die in A+W CAD Designer definiert sind.
Pro ausgewählter Bearbeitung werden zusätzliche Felder angezeigt, um die Zuordnungen zu präzisieren. Eine ausführliche Beschreibung der Parameter finden Sie im Part Verkauf zur Positionserfassung.
- Verkauf, "Positionen - Bearbeitungen" auf Seite C-468

- **Bearbeitungstyp**: Nummer und Bezeichnung des Bearbeitungstyps aus A+W CAD Designer.
- **Prio**: Wenn Sie zu einem Bearbeitungstyp mehrere Zuordnungen anlegen, müssen Sie angeben, mit welcher Priorität das System die Angaben auswerten soll.
- **Auf Produktart**: Die Regel kann auf eine Produktart eingeschränkt werden.
  - **☐** Die Regel für die ausgewählte Bearbeitung kann an allen Produktarten angebracht werden.
  - **☑** Die Regel soll nur gelten, wenn die ausgewählte Bearbeitung an einem bestimmten Produkt angebracht wird. Das Feld zur Auswahl der in A+W CAD Designer hinterlegten Produkte wird freigeschaltet.
- **Formel**: Die Regel kann auf eine Bearbeitung eingeschränkt werden, die durch eine Formel berechnet wird.
  - **☐** Die Regel gilt für die ausgewählte Bearbeitung.
  - **☑** Die Regel gilt für die ausgewählte Bearbeitung nur dann, wenn die Bearbeitung durch eine Formel berechnet wird. Das Feld zur Auswahl der in A+W CAD Designer hinterlegten Formel wird freigeschaltet.
- **Kantenqualität**: Die Regel kann auf eine Bearbeitung eingeschränkt werden, wenn verschiedene Kantenqualitäten erzeugt werden können.
  - **☐** Die ausgewählte Bearbeitung bezieht sich nicht auf verschiedene Kantenqualitäten.
  - **☑** Die Regel gilt für die ausgewählte Bearbeitung nur dann, wenn die Bearbeitung eine bestimmte Kantenqualität erzeugt. Das Feld zur Auswahl der in A+W CAD Designer hinterlegten Kantenqualitäten wird freigeschaltet.

### Wird zu Produkt
- **Produkt**: Nummer und Bezeichnung der Bearbeitung in A+W Business, die zugeordnet wird.

### Regeln
In der Übersicht werden die definierten Regeln angezeigt.

---

# Preise

**Stammdaten > Preise**

Für die Preisfindung im Auftrag stehen Preislisten, Rabatte und Zu- und Abschläge zur Verfügung. In diesem Abschnitt werden die Dialoge zu den Preislisten und zu den Zu- und Abschlägen beschrieben.
Die Beschreibung zu den Rabatten finden Sie im Abschnitt **Marktpartner**.
- "Rabattverwaltung (Kunden, Lieferanten)" auf Seite B-804

> **Reihenfolge der Dialogbeschreibungen**
> Die Dialogbeschreibungen in diesem Kapitel richten sich nicht vollständig nach der Reihenfolge der Dialoge in der Software. Die Preisverwaltung ist aus Gründen der Lesbarkeit in einem separaten Kapitel beschrieben.

Im Menü **Preise** finden Sie folgende Dialoge:
- "Preisjahrgang" auf Seite B-662
- "Preisschlüssel" auf Seite B-663
- "Tarife" auf Seite B-664
- "Preisverwaltung" auf Seite B-712
- "Sonstige Zuschläge" auf Seite B-666
- "Austauschzuschläge" auf Seite B-668
- "Preisgruppen" auf Seite B-686
- "Preisgruppenzuordnung" auf Seite B-687
- "Gruppenzuschläge" auf Seite B-689
- "Mischkalkulation" auf Seite B-698
- "Modellbearbeitungszuschläge" auf Seite B-699
- "Preis- und Mengeneinheit" auf Seite B-702
- "Versicherungspreise" auf Seite B-704
- "Sprossenpreiselemente" auf Seite B-711

## Preisjahrgang

**Stammdaten > Preise > Jahrgang**

*[Screenshot: Preisjahrgang]*

In diesem Dialog legen Sie die Jahrgänge an. Ein Jahrgang fasst eine Sammlung von Preislisten zusammen. Die Preisjahrgänge werden in der A+W Business-Preisberechnung fest mit den Preisschlüsseln zu einem Tarif verknüpft.
- Tutorial 1, "Preisjahrgang" auf Seite B-222
- "Tarife" auf Seite B-664

Sie müssen angeben, welche Preisliste als Standard-Preisliste für die automatische Preisfindung herangezogen werden soll, indem Sie entsprechende Checkbox (Stn) markieren. Diese Einstellungen werden in die Tarife übernommen.

- **Stn VK**: Die Spalten ISO, EFG, Bearb. und Modell gelten für den Verkauf.
- **Stn EK**: Die Spalten EK, Bearb. und Modell gelten für den Einkauf.
- **Von, bis**: Zeitraum, in dem die Preisliste gültig sein soll. Diese Angaben haben keinen Einfluss auf die Verfügbarkeit der jeweiligen Preisliste.
- **Gesperrt**: Ein Jahrgang kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
  - **☐** Der Jahrgang kann zugewiesen werden.
  - **☑** Der Jahrgang ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er Produkten und in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.
- **Bemerkungen**: Kommentare, z. B. zu Besonderheiten der Preisliste.

---

## Preisschlüssel

**Stammdaten > Preise > Schlüssel**

*[Screenshot: Preisschlüssel]*

In diesem Dialog legen Sie Preisschlüssel an. Ein Preisschlüssel wird immer an eine Jahrgangspreisliste gekoppelt und stellt ihre Unterteilung dar.
Die Kombination eines Preisschlüssels mit einer oder mehreren Jahrgangspreislisten ergibt die Tarife, die zur Preisberechnung herangezogen werden.
- Tutorial 1, "Preisschlüssel" auf Seite B-222
- "Tarife" auf Seite B-664

**Gesperrt**: Ein Preisschlüssel kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
- **☐** Der Preisschlüssel kann zugewiesen werden.
- **☑** Der Preisschlüssel ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er Produkten und in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

---

## Tarife

**Stammdaten > Preise > Tarife**

*[Screenshot: Tarifzuordnung]*

In diesem Dialog definieren Sie, welcher Preisschlüssel mit welcher Preisliste zu einem Tarif kombiniert wird. Diese Kombination wird in der Auftrags- und Bestellungserfassung (Verkauf, Einkauf) übernommen und kann jeweils überschrieben werden.
Erst wenn die Tarife festgelegt worden sind, können Sie in der Preisverwaltung die Preise hinterlegen.
- Tutorial 1, "Tarifdefinition" auf Seite B-223

### Preisjahrgang
In diesem Bereich wird angezeigt, welche Preisliste im Preisjahrgang als Standard-Preisliste definiert ist. Auch die Preisliste `<k.A.>` kann zur Tarifkombination verwendet werden. Sie kann auch zur Definition von Preisen verwendet werden.

### Preisschlüssel
In diesem Bereich werden die angelegten Preisschlüssel angezeigt. Auch der Preisschlüssel `<k.A.>` kann zur Tarifkombination verwendet werden.

### Tarifzuordnung
In diesem Bereich kombinieren Sie die Jahrgangspreisliste und den Preisschlüssel, um einen Tarif zu erstellen.
Im Preisjahrgang selbst ist nur definiert, welche der Preislisten zur Standard-Preisberechnung herangezogen wird, z. B. für alle Verkaufspreise (VK) und Einkaufspreise (EK) dieselbe Preisliste.
Für den Tarif wird angegeben, dass z. B. für den VK ISO die Preisliste 07 mit dem Preisschlüssel Hütte 06 gültig ist, aber für den VK EFG (Einfachglas) die Preisliste 07 mit dem Preisschlüssel Festmaß.

> **Nur definierte Tarife stehen zur Preisberechnung zur Verfügung**
> Beachten Sie, dass Sie für jede Kombination von Preisjahrgang und Preisschlüssel, die Sie im Verkauf oder im Einkauf verwenden wollen, ein Tarif definiert werden muss. Dieser Tarif muss auch dann definiert werden, wenn er nicht als Standard verwendet werden soll.

Die markierten Checkboxen zeigen an, welcher Tarif als Standard für die Verkaufs- bzw. Einkaufspreisberechnung verwendet wird.

**ISO-Basistabelle**
Standardmäßig werden in A+W Business die ISO-Preise auf der Basis je einer ISO-Matrix für die Standard-Aufbauten berechnet, z. B. für ISO mit 2 x Float 4 mm, 2 x Float 6 mm, 2 x Float 8 mm.
Wenn Sie die Preise mit einer einzigen Matrix aufbauen und mit prozentualen Zu- und Abschlägen für die unterschiedlichen Glasdicken und Austauschgläser arbeiten, muss eine neue, sogenannte ISO-Basistabelle angelegt werden. Pro Tarif geben Sie die Nummer dieser ISO-Basistabelle an, damit die Preise nach diesem Muster berechnet werden.

**Herstellkostenkalkulation**
Wenn Sie mit dem Modul Herstellkostenkalkulation arbeiten, müssen Sie angeben, welcher der Tarife bei der Berechnung der Herstellkosten herangezogen werden soll.
- **☐** Der Tarif wird nicht zur Kostenkalkulation herangezogen.
- **☑** Der Tarif wird zur Kalkulation der Herstellkosten herangezogen.

---

## Sonstige Zuschläge

**Stammdaten > Preise > Sonstige Zuschläge**

*[Screenshot: Sonstige Zuschläge]*

In diesem Dialog legen Sie Preiszuschläge an und bearbeiten diese. Diese Zuschläge sind von der Länge, der Fläche, dem Gewicht, dem SZR usw. abhängig. Dabei können Sie für die Staffelung zwei Grenztypen verwenden.
- Tutorial 1, "Zuschläge" auf Seite B-267
- Tutorial 1, "Sonstigen Zuschlag anlegen" auf Seite B-318

> **Reihenfolge der Zuschlagsstufen beachten**
> Eine neue Stufe wird immer nach der letzten Stufe eingefügt. Die Reihenfolge der Stufen wird bei der Preisfindung nicht geändert oder analysiert. Das bedeutet, dass der Grenzwert 1200 mm dann nicht berücksichtigt wird, wenn er nach dem Grenzwert 1800 mm eingetragen ist. Für alle Größen unter 1800 mm wird dann derselbe Zuschlag berechnet.

Bei der Zuschlagsberechnung wird die Reihenfolge nur innerhalb der gleichen Zuschlagseinheit geprüft. Die Reihenfolge ist dann entscheidend und wird berücksichtigt, wenn eine Zuschlagseinheit, z. B. Brutto%, für mehrere unterschiedliche Grenztypen, z. B. kleinste Kantenlänge oder größte Kantenlänge, gilt.

- Zuschläge auf einzelne Elemente der Stücklisten werden früher berechnet als die Zuschläge, die von der Position auf die Stückliste wirken. Dies gilt auch umgekehrt: Zuschläge auf die Position werden früher berechnet als die Zuschläge, die aus der Stückliste heraus auf die Position wirken.
- Zuschläge auf qm, lfm und Stück werden vor Brutto-, Netto %-Zuschlägen berechnet. Hierbei ist entscheidend, worauf sie wirken: den Preis pro Preiseinheit, den Bruttopreis oder den Nettopreis.

Dabei muss außerdem die Zuschlagsart berücksichtigt werden. Bei **nicht additiver** Berechnung wird für die Berechnung des nachfolgenden Zuschlags der vorausgegangene Zuschlag nicht mit in die Berechnung einbezogen.

> **Beispiel: Basispreis 100,00 €**
>
> | | additiv | nicht additiv |
> | :--- | :--- | :--- |
> | Modellzuschlag + 20% | + 20,00 € | + 20,00 € |
> | **Zwischensumme** | **= 120,00 €** | |
> | Beschichtung + 25% | + 30,00 € | + 25,00 € |
> | **Gesamtsumme** | **= 150,00 €** | **= 145,00 €** |

### Register Zuschlag
In diesem Register werden die Staffelungen des Zuschlags angezeigt, der im Register **Tabelle** markiert ist.

#### Zuschlag für
- **Nummer**: Nummer der Zuschlagstabelle.
- **Bezeichnung**: Name der Zuschlagstabelle.

- **Grenztyp 1, 2**: Mit Hilfe der Grenztypen können Sie die Zuschläge staffeln. Der Grenztyp legt die Maßeinheit für die Staffelung fest. Sie können unterschiedliche Maßeinheiten für die beiden Grenztypen auswählen, z. B. Höhe und Breite.
- **Bis Grenze 1, 2**: Wert der Staffelung. Der Grenzwert bezieht sich auf den Grenztyp. Ist als Grenztyp `<k.A.>` angegeben, gilt der Zuschlag pro Preiseinheit.
- **ODER**: Wenn Sie zwei unterschiedliche Grenztypen für die Staffelung verwenden wollen, müssen Sie angeben, ob diese gemeinsam oder alternativ ausgewertet werden sollen.
  - **☑** Beide Grenzwerte und Grenztypen werden bei der Berechnung des Zuschlags berücksichtigt.
  - **☐** Nur einer von beiden Grenzwerten/Grenztypen wird berücksichtigt.

> **Beispiel**
> In der Preisverwaltung haben Sie für ein Ornamentglas eine Matrix angelegt, bei der Höhe und Breite nicht vertauscht werden dürfen.
> Für die Berechnung eines Zuschlags auf die Kantenlängen soll es keine Rolle spielen, ob die Höhe oder die Breite den Grenzwert erreicht.
> Sie tragen als Grenzwert 1 und 2 die Stufe 1200 ein.
> Als Grenztyp 1 wählen Sie Höhe und als Grenztyp 2 Breite.
> - Wenn Sie die Checkbox ODER markieren, wird jeweils die Kante berücksichtigt, die als erste die Stufe 1200 mm erreicht.
> - Wenn Sie die Checkbox nicht markieren, wird der Zuschlag erst erhoben, wenn beide Kanten mindestens die Länge 1200 mm erreichen.

- **Zuschlag, Einheit**: Höhe und Einheit des Zuschlags, z. B. 2,5 % des Bruttopreises.
- **Zuschlagsart**: Die Zuschlagsart bestimmt, auf welcher Basis der Zuschlag berechnet werden soll.
  - Tutorial 1, "Berechnungen nach Zuschlagsarten" auf Seite B-311
- **Gültig bei Preisvorgabe**: Im Auftrag kann der Preis manuell überschrieben werden. Dabei kann der Zuschlag wahlweise berechnet werden. Die Einstellung gilt für alle Aufträge und kann im Auftrag nicht geändert werden.
  - **☐** Der Zuschlag wird nicht berechnet, wenn der Preis im Auftrag manuell überschrieben wird.
  - **☑** Der Zuschlag wird immer berechnet.

### Register Tabelle
In der Tabelle werden alle sonstigen Zuschläge aufgeführt, die den Auswahlkriterien entsprechen.

---

## Austauschzuschläge

**Stammdaten > Preise > Austauschzuschläge**

Die Austauschzuschläge sind gruppenunabhängig und beziehen sich auf die Gläser, die nicht in Gruppen zusammengefasst werden können oder sollen. Sie können Produkt für Produkt definieren, welchen Zuschlag Sie hinzufügen möchten, wenn in einem ISO oder einem VSG ein Glas getauscht wird.

Im Dialog **Austauschzuschläge** finden Sie folgende Register:
- Austauschzuschläge - Tabelle
- Austauschzuschläge – Allgemein, nach Dicke, nach Produkt
- Austauschzuschläge – Kunden-, Lieferantenpreise
- Tutorial 1, "Austauschzuschläge" auf Seite B-287

### Menü Funktionen
Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog **Austauschzuschläge** zu schließen.

#### Gruppe Kopieren
- **Allgemein:** Öffnet den Dialog **Austauschpreise kopieren allgemein**, um die Preise für Eintauschgläser zu kopieren.
  - "Austauschpreise kopieren" auf Seite B-675
- **Pro Austauschartikel komplett:** Öffnet den Dialog **Preise pro Austauschartikel komplett kopieren**, um die Preise für Austauschgläser zu kopieren.
  - "Preise pro Austauschartikel komplett kopieren" auf Seite B-679

#### Gruppe Löschen
- **Preise löschen:** Öffnet den Dialog **Austauschpreise löschen**, um einen Austauschzuschlag zu löschen.
  - "Austauschpreise löschen" auf Seite B-682

#### Gruppe Ändern
- **Preise ändern:** Öffnet den Dialog **Preise ändern**, um einen Austauschzuschlag zu ändern.
  - "Austauschpreise ändern" auf Seite B-683

### Austauschzuschläge – Tabelle

**Stammdaten > Preise > Austauschzuschläge > Register Tabelle**

*[Screenshot: Austauschzuschläge – Tabelle]*

In diesem Register prüfen Sie, welche Austauschzuschläge angelegt sind.
- Tutorial 1, "Austauschzuschläge" auf Seite B-287
- Tutorial 1, "Austauschzuschlag anlegen" auf Seite B-291

#### Identifikation - Tarif
- **Tabelle**: In der Regel wird nur eine Tabelle (Nr. 0) angelegt. Wenn Sie unterschiedliche Tabellen für Austauschzuschläge anlegen, können Sie diese in den Produktstammdaten zuweisen.
  - "Tab. Austauschzuschl." auf Seite B-604
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (VK-Tarif), denen der Austauschzuschlag zugeordnet ist.
- **ISO, VSG**: Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also z. B. in einem Mehrfach-ISO das zweite oder dritte Glas.

#### Produkt
- **Eintausch**: Stücklisten-Komponente, die eingebaut wird.
- **Austausch**: Stücklisten-Komponente, die ausgebaut, also ersetzt wird. Das Feld wird bei einem allgemeinen und bei einem produktbezogenen Austauschzuschlag angezeigt.
- **Dicke Austausch**: Dicke der Stücklisten-Komponente, die ausgebaut, also ersetzt wird. Dabei spielt es keine Rolle, zu welcher Produktart oder -gruppe das Glas gehört. Das Feld wird bei einem dickenabhängigen Austauschzuschlag angezeigt.

#### Austauschpreise
Der Zuschlag kann in max. drei Stufen gestaffelt werden. Die Grenztypen werden dem Produkt entsprechend im Register **Allgemein** vorgegeben.
Die Grenzwerte der höchsten Stufe werden automatisch aus den Feldern der zweiten Stufe übernommen. Das bedeutet, dass nur noch der Zuschlagswert eingetragen werden kann. Dieser wird immer dann berechnet, wenn die Scheibe größer als die zweite Stufe.
- **Zuschlag**: Zuschlagswert pro Stufe. Der Wert wird je nach Zuschlagstyp als prozentualer Zuschlag oder als Betrag interpretiert.
  - "Zuschlagstypen" auf Seite B-672

#### Austausch-Tabelle
In der Übersicht sind alle Zuschläge aufgeführt, die den Auswahlkriterien entsprechen.
- **Produkt, Nummer:** Produktnummer des Eintauschprodukts, z. B. Glas, Gießharz.
- **Eintausch:** Bezeichnung des Eintauschprodukts.
- **Austausch:** Bezeichnung des Austauschs, also Produkt oder Dicke.
- **Tab.:** Nummer der Austauschtabelle, in der Regel Nummer 0.
- **Schlüssel:** Preisschlüssel, dem der Zuschlag zugeordnet ist.
- **Tarif:** Preisliste, dem der Zuschlag zugeordnet ist.

### Austauschzuschläge – Allgemein, nach Dicke, nach Produkt

**Stammdaten > Preise > Austauschzuschläge > Register Allgemein, nach Dicke, nach Produkt**

*[Screenshot: Austauschzuschläge – Allgemein]*

In den Registern **Allgemein**, **nach Dicke** und **nach Produkt** legen Sie Austauschzuschläge für ISO- oder VSG-Scheiben an. Die Zuschläge beziehen sich immer auf Tarife für Verkaufspreise (VK).
- Tutorial 1, "Austauschzuschläge" auf Seite B-287

Die Felder in den Bereichen **Identifikation - Tarif**, **Produkt** und **Austauschpreise** sind zum Register **Tabelle** erklärt.
- "Austauschzuschläge – Tabelle" auf Seite B-670

#### Zuschlagstypen
Der Zuschlagstyp gibt an, wie der Wert im Feld **Zuschlag** interpretiert werden soll, z. B. als prozentualen Aufschlag auf den Preis, als Betrag pro Länge usw.

#### Sonstige Zuschläge
**Nummer, Tabelle**
Sie können zusätzlich zum Austauschzuschlag einen Sonstigen Zuschlag erheben, z. B. für Zuschnittskosten. Die Sonstigen Zuschläge werden im gleichnamigen Dialog angelegt:
- "Sonstige Zuschläge" auf Seite B-666

#### Grenzmengentyp
Mit der Wahl der Option legen Sie fest, welche Grenztypen im Bereich **Austauschpreise** verwendet werden.
- **Breite x Höhe:** Die Grenztypen **Breite** und **Höhe** werden angezeigt.
- **Fläche tatsächlich:** Der Grenztyp **qm** (Quadratmeter) wird angezeigt. Als Fläche wird dabei die Fläche aus dem Auftrag herangezogen.
- **Kantenmaß:** Der Grenztyp **Kante** wird angezeigt.
- **Fläche gerundet:** Der Grenztyp **qm** (Quadratmeter) wird angezeigt. Für die Berechnung der Fläche werden dabei die Rundungen aus dem Auftrag und aus den Produktdaten herangezogen, in Deutschland meistens der Wert 30.
  - "Maßrundung Breite / Höhe" auf Seite B-606

#### Abw. Maßrundung
Sie können zur Berechnung der Fläche eine abweichende Maßrundung eingeben.
**Breite, Höhe**
Standardmäßig ist der Wert 0 eingetragen. Bei dieser Einstellung werden die Werte aus den Produktdaten übernommen.

#### Mindestangaben
Sie können Mindestwerte für die Berechnung des Zuschlags eingeben. Diese werden immer dann herangezogen, wenn die Werte im Auftrag darunterliegen.
- **Mindestfläche**: Wenn Sie eine Mindestfläche für ein Eintauschglas angeben, wird diese Fläche in all den Fällen als Zuschlagsbasis herangezogen, in denen die Fläche im Auftrag kleiner ist.
- **Preis brutto, netto**: Wenn Sie einen Mindestpreis angeben, wird dieser immer dann als Basis für den Zuschlag herangezogen, wenn der tatsächliche Preis des Eintauschproduktes darunterliegt.

### Austauschzuschläge – Kunden-, Lieferantenpreise

**Stammdaten > Preise > Austauschzuschläge > Register Kundenpreise, Lieferantenpreise**

*[Screenshot: Austauschzuschläge – Kundenpreise]*

In den Registern **Kundenpreise** und **Lieferantenpreise** legen Sie Austauschzuschläge an, die bei bestimmten Kunden oder Lieferanten berechnet werden sollen.
- Tutorial 1, "Austauschzuschläge" auf Seite B-287

Die Felder im Bereich **Identifikation - Tarif** sind zum Register **Tabelle** erklärt.
- "Austauschzuschläge - Tabelle" auf Seite B-670

#### Auswahl Kunden/Kundengruppe, Lieferanten/Lieferantengruppe
Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

#### Objektauswahl
Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten.

#### Übersicht nach Kunden/Kundengruppen, Lieferanten/Lieferantengruppen
In der Übersicht werden alle Zuschläge angezeigt, die den Auswahlkriterien entsprechen.

---

### Auswahl – Austauschzuschlag

**Stammdaten > Preise > Austauschzuschläge > Menü Bearbeiten > Neu**

*[Screenshot: Auswahl der Zuschlagsart]*

In diesem Dialog wählen Sie die Art des Zuschlags, den Sie anlegen wollen.

---

### Austauschpreise kopieren

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Allgemein**

Sie können einzelne oder mehrere Austauschzuschläge für Einbaugläser gemeinsam kopieren oder ändern.
In diesem Dialog finden Sie folgende Register:
- "Austauschpreise kopieren – Quelle, Ziel" auf Seite B-676
- "Austauschpreise kopieren - Preisänderung" auf Seite B-678

#### Austauschpreise kopieren – Quelle, Ziel

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Allgemein > Register Quelle**

*[Screenshot: Austauschpreise kopieren 1 – Quelle, Ziel]*

In den Registern kopieren Sie die Zuschläge einer Tabelle in eine andere Tabelle oder in einen anderen Tarif. Nur die Austauschzuschläge werden kopiert, die für Einbaugläser erhoben werden.
- Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-296

Wenn Sie die Zuschläge nur ändern wollen, geben als Quelle und Ziel dieselben Tabellen an. Im Register **Preisänderung** können Sie dann die Werte für die Änderung eintragen.
- "Austauschpreise kopieren - Preisänderung" auf Seite B-678

##### Kopieren von, Kopieren nach
- **Tabelle**: Nummer der Austauschtabelle.
- **Eintauschnummer von, bis**: Nummern der Produkte, die eingebaut werden.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.
- **ISO, VSG, Beides**: Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas. Mit der Option **Beides** werden die Austauschpreise für ISO und VSG kopiert.
- **Preise überschreiben**: Wenn Sie die Zuschläge in eine gefüllte Tabelle übertragen wollen, müssen Sie entscheiden, ob die Zuschläge in der Ziel-Tabelle überschrieben werden sollen.
  - **☐** Die Zuschläge der Ziel-Tabelle werden nicht überschrieben. Die zusätzlichen Zuschläge aus der Quell-Tabelle werden hinzugefügt.
  - **☑** Alle vorhandenen Zuschläge in der Ziel-Tabelle werden überschrieben.
- **Preisart**: Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
  - **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
  - **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
  - **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten
- **Objekt**: Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschlagstabelle geändert werden soll.

#### Austauschpreise kopieren – Preisänderung

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Allgemein > Register Preisänderung**

*[Screenshot: Austauschpreise kopieren – Preisänderung]*

In diesem Register geben Sie die Details für die Änderung an.
Wenn Sie als Quelle und Ziel dieselben Tabellen angegeben haben, werden die Zuschläge geändert, ohne sie in andere Tabellen zu kopieren.
Die Felder in den Bereichen **Kopieren von** und **Kopieren nach** sind zum Register **Quelle** beschrieben.
- "Austauschpreise kopieren – Quelle, Ziel" auf Seite B-676

- **Aufschlag, Abschlag**: Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.
- **Rundung**: Sie können die Rundung für die ausgewählte Tabelle ändern.
- **Prozent, Absolut**: Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

---

### Preise pro Austauschartikel komplett kopieren

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Pro Austauschartikel komplett**

Sie können einzelne oder mehrere Austauschzuschläge für Ausbaugläser gemeinsam kopieren oder ändern.
In diesem Dialog finden Sie folgende Register:
- "Preise pro Austauschartikel komplett kopieren – Quelle, Ziel" auf Seite B-679
- "Preise pro Austauschartikel komplett kopieren – Preisänderung" auf Seite B-681

#### Preise pro Austauschartikel komplett kopieren – Quelle, Ziel

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Pro Austauschartikel komplett > Register Quelle**

*[Screenshot: Austauschpreise komplett Kopieren – Quelle]*

In diesem Dialog kopieren Sie die Zuschläge einer Tabelle in eine andere Tabelle oder in einen anderen Tarif. Nur die Austauschzuschläge werden kopiert, die für Ausbaugläser erhoben werden.
- Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-296

Wenn Sie die Zuschläge nur ändern wollen, geben als Quelle und Ziel dieselben Tabellen an. Im Register **Preisänderung** können Sie dann die Werte für die Änderung eintragen.
- "Preise pro Austauschartikel komplett kopieren – Preisänderung" auf Seite B-681

##### Kopieren von, Kopieren nach
- **Tabelle**: Nummer der Austauschtabelle.
- **Austausch**: Nummer des Produkts, das aus der Einheit entfernt wird.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.
- **ISO, VSG, Beides**: Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas. Mit der Option **Beides** werden die Austauschpreise für ISO und VSG kopiert.
- **Preise überschreiben**: Wenn Sie die Zuschläge in eine gefüllte Tabelle übertragen wollen, müssen Sie entscheiden, ob die Zuschläge in der Ziel-Tabelle überschrieben werden sollen.
  - **☐** Die Zuschläge der Ziel-Tabelle werden nicht überschrieben. Die zusätzlichen Zuschläge aus der Quell-Tabelle werden hinzugefügt.
  - **☑** Alle vorhandenen Zuschläge in der Ziel-Tabelle werden überschrieben.
- **Preisart**: Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
  - **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
  - **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
  - **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten
- **Objekt**: Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschlagstabelle geändert werden soll.

#### Preise pro Austauschartikel komplett kopieren – Preisänderung

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Pro Austauschartikel komplett > Register Preisänderung**

*[Screenshot: Austauschpreise komplett kopieren – Preisänderung]*

In diesem Register geben Sie die Details für die Änderung an.
Wenn Sie als Quelle und Ziel dieselben Tabellen angegeben haben, werden die Zuschläge geändert, ohne sie in andere Tabellen zu kopieren.
Die Felder in den Bereichen **Kopieren von** und **Kopieren nach** sind zum Register **Quelle** beschrieben.
- "Preise pro Austauschartikel komplett kopieren - Quelle, Ziel" auf Seite B-679

- **Aufschlag, Abschlag**: Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.
- **Rundung**: Sie können die Rundung für die ausgewählte Tabelle ändern.
- **Prozent, Absolut**: Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

---

### Austauschpreise löschen

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise löschen**

*[Screenshot: Austauschzuschläge löschen]*

In diesem Dialog löschen Sie Austauschzuschläge einzeln oder eine Folge von Austauschzuschlägen.

#### Preisart
Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt, den Sie löschen wollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

#### Objekt
Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten. Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben.

#### Preisauswahl
- **Tabelle**: Nummer der Austauschtabelle, die gelöscht werden soll.
- **ISO, VSG, Beides**: Produktart, bei der der Zuschlag erhoben wird. Mit der Option **Beides** werden die Austauschpreise für ISO und VSG gelöscht.
- **Eintausch von, bis**: Produktnummern der Eintauschgläser, zu denen der Austauschzuschlag definiert ist.
- **Anzahl**: Anzahl der Datensätze, die gelöscht werden.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.

---

### Austauschpreise ändern

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise ändern**

Sie können einzelne oder mehrere Austauschzuschläge gemeinsam ändern.
In diesem Dialog finden Sie folgende Register:
- "Austauschpreise ändern - Preisart" auf Seite B-683
- "Austauschpreise ändern – Preisänderung" auf Seite B-685

#### Austauschpreise ändern – Preisart

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise ändern > Register Preisart**

*[Screenshot: Austauschpreise ändern – Register Preisart]*

In diesem Register wählen Sie die Austauschzuschläge aus, die Sie ändern wollen.
- Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-296

##### Preisauswahl
- **Tabelle**: Nummer der Austauschtabelle, deren Preise geändert werden.
- **Anzahl**: Anzahl der Datensätze.
- **Nummer von, bis**: Nummern der Datensätze, die geändert werden.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.
- **ISO, VSG, Beides**: Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas. Mit der Option **Beides** werden die Austauschpreise für ISO und VSG geändert.

##### Preisart
Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt, den Sie ändern wollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten
- **Objekt**: Das Feld ist gesperrt, wenn Sie die Option Allgemein gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschläge geändert werden sollen.

#### Austauschpreise ändern – Preisänderung

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise ändern > Register Preisänderung**

*[Screenshot: Austauschpreise ändern – Register Preisänderung]*

In diesem Register geben Sie die Details für die Änderung an.
Die Felder im Bereich **Preisauswahl** sind zum Register **Preisart** beschrieben.
- "Austauschpreise ändern - Preisart" auf Seite B-683

- **Aufschlag, Abschlag**: Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.
- **Rundung**: Sie können die Rundung für die ausgewählten Zuschläge ändern.
- **Prozent, Absolut**: Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

---

## Preisgruppen

**Stammdaten > Preise > Preisgruppen**

*[Screenshot: Preisgruppen]*

In diesem Dialog hinterlegen Sie Preisgruppen. Die Preisgruppen verwenden Sie für die Berechnung von Preisen für Ornamentgläser und von Austauschzuschlägen, damit Sie nicht für jedes Produkt eine eigene Preistabelle pflegen müssen.
Die Produkte ordnen Sie den Preisgruppen im Dialog **Preisgruppenzuordnung** zu.
- "Preisgruppenzuordnung" auf Seite B-687

- **Bezeichnung**: In der Regel sind die Preisgruppen alphabetisch nummeriert.
- **Bemerkung**: Ergänzende Bemerkung, z. B. zur Verwendung der Preisgruppe.

---

## Preisgruppenzuordnung

**Stammdaten > Preise > Preisgruppenzuordnung**

*[Screenshot: Preisgruppenzuordnung]*

In diesem Dialog ordnen Sie den Produkten eine Preisliste und eine Preisgruppe zu.
Jeder Preisgruppe können Sie dann im Dialog **Gruppenzuschläge** ein Austauschzuschlag zuweisen, wodurch die Verwaltung von Preisen und deren Zuschlägen erheblich vereinfacht ist.
- Tutorial 1, "Preisgruppen zuordnen" auf Seite B-275

### Menü Funktionen
Über dieses Menü können Sie den Dialog **Schlüssel kopieren** öffnen, in dem Sie den Schlüssel eines Jahrgangs in einen anderen kopieren können.
- "Preisgruppenzuordnung kopieren" auf Seite B-688

### Identifikation - Tarif
- **Verkaufsliste, Einkaufsliste**: Mit der Wahl der Option legen Sie fest, welcher Art von Tarifen Sie Preisgruppen zuordnen wollen.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), in denen der Preis festgelegt ist.

### Produktauswahl
In diesem Bereich wählen Sie Produkte aus, die Sie in einem Isolierglas und/oder in einem VSG eintauschen können.
- **Artikel/MCode, Bezeichnung**: Nummer, Matchcode und Bezeichnung des Produktes, das der Preisgruppe zugeordnet wird.

### Übersicht Zuordnungen
In der Übersicht werden alle Produkte angezeigt, die den Auswahlkriterien entsprechen.
- **PG ISO, PG VSG**: In den Spalten PG ISO und PG VSG wählen Sie die Preisgruppen aus, zu denen das Eintauschprodukt gehören soll.

---

## Preisgruppenzuordnung kopieren

**Stammdaten > Preise > Preisgruppenzuordnung > Menü Funktionen > Kopieren**

*[Screenshot: Preisgruppenzuordnung – Kopieren]*

In diesem Dialog kopieren Sie Preisgruppenzuordnung in einen anderen Tarif.
Die Felder sind zum Dialog **Preisgruppenzuordnung** beschrieben.
- "Preisgruppenzuordnung" auf Seite B-687

---

## Gruppenzuschläge

**Stammdaten > Preise > Gruppenzuschläge**

*[Screenshot: Preisgruppenabhängige Zuschläge]*

In diesem Dialog legen Sie allgemeine Zuschläge zu den Preisgruppen an, die beim Austausch eines Glases berechnet werden sollen. Im Unterschied zu den Austauschzuschlägen wird hier die Dicke des Glases als Grenztyp eingesetzt.
- Tutorial 1, "Gruppenzuschlag anlegen" auf Seite B-277

### Menü Funktionen
Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
- **Preise kopieren:** Öffnet den Dialog **Austauschpreise kopieren**, um Gruppenzuschläge zu kopieren.
  - "Austauschpreise kopieren" auf Seite B-675
- **Preis löschen:** Öffnet den Dialog **Preise nach Preisgruppen löschen**, um Gruppenzuschläge zu löschen.
  - "Gruppenzuschläge löschen" auf Seite B-694
- **Preis ändern:** Öffnet den Dialog **Preise ändern**, um einen oder eine Folge von Zuschlägen gleichzeitig zu ändern.
  - "Preise ändern" auf Seite B-725

### Identifikation - Tarif
- **Verkaufsliste, Einkaufsliste**: Mit der Wahl der Option legen Sie fest, welcher Art von Tarifen Sie Gruppenzuschläge zuordnen wollen.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.
- **Produktart ISO, VSG**: Produktart, bei der der Gruppenzuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas.
- **Dicke**: Dicke der auszutauschenden Scheibe. Das ist die Scheibe, die aus dem ISO oder VSG herausgenommen wird.

### Auswahl Kundengruppe/Kunden, Lieferantengruppe/Lieferanten
In diesem Bereich ordnen Sie einen Preisgruppenzuschlag einem Kunden, Lieferanten oder einer Kunden-, Lieferantengruppe zu.
Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gelten soll:
- **Allgemein:** Allgemeiner Zuschlag
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten
- **Name 1, Name 2**: Name der ausgewählten Partner.

### Übersicht
In der Übersicht werden alle Gruppenzuschläge angezeigt, die den Auswahlkriterien entsprechen.
- **Glasdicke:** Dicke der auszutauschenden Scheibe, das ist die Scheibe, die aus dem ISO oder VSG herausgenommen wird.
- **Preisgruppe:** Preisgruppe, für die der Zuschlag gilt.
- **Zuschlag:** Zuschlagswert pro Dicke. Der Wert wird je nach Zuschlagstyp als prozentualer Zuschlag oder als Betrag interpretiert.
- **Zuschlagstyp:** Der Zuschlagstyp gibt an, wie der Wert im Feld **Zuschlag** interpretiert werden soll, z. B. als prozentualer Aufschlag auf den Preis, als Betrag pro Länge usw.
- **Mindestfläche:** Wenn Sie eine Mindestfläche für ein Eintauschglas angeben, wird diese Fläche in all den Fällen als Zuschlagsbasis herangezogen, in denen die Fläche im Auftrag kleiner ist.
- **Brutto-Mindestpreis, Netto-Mindestpreis:** Wenn Sie einen Mindestpreis angeben, wird dieser immer dann als Basis für den Zuschlag herangezogen, wenn der Preis des Eintauschproduktes im Auftrag darunterliegt.
- **Rundung Breite, Rundung Höhe:** Sie können abweichende Rundungen für die Breite und Höhe angeben, die immer dann berechnet werden, wenn der Gruppenzuschlag zur Preisfindung herangezogen wird.
- **Sonstige Zuschläge:** Sie können zusätzlich zum Austauschzuschlag einen Sonstigen Zuschlag erheben, z. B. für Zuschnittskosten. Dieser Zuschlag wird für das Eintauschprodukt berechnet. Die Sonstigen Zuschläge werden im gleichnamigen Dialog angelegt:
  - "Sonstige Zuschläge" auf Seite B-666
- **Preisschlüssel, Preisliste:** Anzeige des zugeordneten Schlüssels und Jahrgangs.

### Objektauswahl
Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten.

### Tabelle
**Übersicht nach Kunden/Kundengruppen, Lieferanten/Lieferantengruppen**
In der Übersicht werden Kunden/Kundengruppen, Lieferanten/Lieferantengruppen oder Objekte angezeigt, zu denen Gruppenzuschläge in gewählten Tarif hinterlegt sind.

---

## Gruppenzuschläge kopieren

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise kopieren**

Sie können einzelne oder mehrere Gruppenzuschläge gemeinsam ändern.
In diesem Dialog finden Sie folgende Register:
- "Gruppenzuschläge kopieren – Quelle, Ziel" auf Seite B-692
- "Gruppenzuschläge kopieren – Preisänderung" auf Seite B-693

### Gruppenzuschläge kopieren – Quelle, Ziel

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise kopieren**
*[Screenshot: Preisgruppenabhängige Zuschläge kopieren - Register Quelle]*

In diesem Register kopieren Sie die Gruppenzuschläge, z. B. um die Zuschläge einer Dicke in einen anderen Tarif zu übertragen.
- Tutorial 1, "Gruppenzuschlag kopieren" auf Seite B-283

#### Kopieren von, Kopieren nach
- **Dicke von, bis**: Dicke der Gläser, für die ein Gruppenzuschlag berechnet wird.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.
- **ISO, VSG, Beides**: Produktart, bei der der Gruppenzuschlag erhoben wird. Mit der Option **Beides** werden die Gruppenzuschläge für ISO und VSG kopiert.
- **Preise überschreiben**: Wenn Sie die Zuschläge in eine gefüllte Tabelle übertragen wollen, müssen Sie entscheiden, ob die Zuschläge in der Ziel-Tabelle überschrieben werden sollen.
  - **☐** Die Zuschläge der Ziel-Tabelle werden nicht überschrieben. Die zusätzlichen Zuschläge aus der Quell-Tabelle werden hinzugefügt.
  - **☑** Alle vorhandenen Zuschläge in der Ziel-Tabelle werden überschrieben.
- **Preisart**: Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
  - **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
  - **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
  - **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten
- **Objekt**: Das Feld ist gesperrt, wenn Sie die Option Allgemein gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschlagstabelle geändert werden soll.

### Gruppenzuschläge kopieren – Preisänderung

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise kopieren**
*[Screenshot: Preisgruppenabhängige Zuschläge kopieren – Register Preisänderung]*

In diesem Register geben Sie die Details für die Änderung an.
Die Felder in den Bereichen **Kopieren von** und **Kopieren nach** sind zum Register **Quelle** beschrieben.
- "Gruppenzuschläge kopieren – Quelle, Ziel" auf Seite B-692

- **Aufschlag, Abschlag**: Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.
- **Rundung**: Sie können die Rundung für die ausgewählten Zuschläge ändern.
- **Prozent, Absolut**: Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

---

## Gruppenzuschläge löschen

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise löschen**

*[Screenshot: Preisgruppenabhängige Zuschläge löschen]*

In diesem Dialog löschen Sie Gruppenzuschläge einzeln oder eine Folge von Gruppenzuschlägen.

### Preisart
Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

### Objekt
Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten.

### Preisauswahl
- **Dicke von, Dicke bis**: Glasdicke, für die der Gruppenzuschlag angelegt ist.
- **Anzahl**: Anzahl der Datensätze.
- **ISO, VSG, Beides**: Produktart, bei der der Zuschlag erhoben wird. Mit der Option **Beides** werden die Zuschläge für ISO und VSG gelöscht.
- **Anzahl**: Anzahl der Datensätze, die gelöscht werden.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.

---

## Gruppenzuschläge ändern

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise ändern**

Sie können einzelne oder mehrere Gruppenzuschläge gemeinsam ändern.
In diesem Dialog finden Sie folgende Register:
- "Gruppenzuschläge ändern – Preisart" auf Seite B-695
- "Gruppenzuschläge ändern – Preisänderung" auf Seite B-697

### Gruppenzuschläge ändern – Preisart

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise ändern**
*[Screenshot: Preisgruppenabhängige Zuschläge ändern und Register Preisänderung]*

In diesem Register wählen Sie Gruppenzuschläge aus, die Sie ändern wollen.
Gruppenzuschläge werden auf die gleiche Weise geändert wie Austauschzuschläge.
- Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-296

#### Preisauswahl
- **Nummer von, Nummer bis**: Glasdicke, für die der Gruppenzuschlag angelegt ist.
- **Anzahl**: Anzahl der Datensätze.
- **Jahrgang, Schlüssel**: Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.
- **ISO, VSG, Beides**: Produktart, bei der der Zuschlag erhoben wird. Mit der Option **Beides** werden die Zuschläge für ISO und VSG geändert.

#### Preisart
Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partnergruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten
- **Objekt**: Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschläge geändert werden sollen.

### Gruppenzuschläge ändern – Preisänderung

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise ändern**
*[Screenshot: Preisgruppenabhängige Zuschläge ändern und Register Preisänderung]*

In diesem Register geben Sie die Details für die Änderung an.
- **Aufschlag, Abschlag**: Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.
- **Rundung**: Sie können die Rundung für die ausgewählten Zuschläge ändern.
- **Prozent, Absolut**: Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

---

## Mischkalkulation

**Stammdaten > Preise > Mischkalkulation**

*[Screenshot: Mischkalkulation]*

Für spezielle Aufbauten in ISO- oder VSG-Scheiben können Sie auf gesonderte Preise verweisen, z. B. bei einem ISO 4/6.
Voraussetzung ist, dass in den Firmendaten der Preisanteil der Komponenten für die Kalkulation angegeben ist.
- "Firmendaten - Dokumente" auf Seite B-929

In der Positionserfassung wird Isolierglas in Form von Mischkalkulation im Register **Zusatz** erfasst. Dabei muss die Position in einer bestimmten Reihenfolge eingegeben werden:
- Im Hauptprodukt selbst darf nichts eingetragen werden, sondern nur im Register **Zusatz > Mischkalkulation**.
- Die ISO-Produkte und ggf. der Mischfaktor werden von außen nach innen eintragen.
- Anschließend müssen im ersten Register die Stückzahl, Breite und Höhe und ggf. einen Austausch ergänzt werden.

Sonstige Zuschläge werden nur berücksichtigt, wenn sie in den Preisen hinterlegt sind.

---

## Modellbearbeitungszuschläge

**Stammdaten > Preise > Modellzuschläge**

*[Screenshot: Modellbearbeitungszuschläge]*

In diesem Dialog legen Sie Bearbeitungszuschläge für Modelle an. Diese Zuschläge können pro Preistabelle unterschiedlich sein, z. B. pro Modelle für die Kantenbearbeitungen und die Eckenbearbeitungen. Voraussetzung ist, dass für die unterschiedlichen Bearbeitungen jeweils eine Preistabelle angelegt ist.
- Tutorial 1, "Modellbearbeitungszuschlag anlegen" auf Seite B-302

### Menü Funktionen
Über dieses Menü öffnen Sie den Dialog **Zuschläge kopieren**, in dem Sie die Modellzuschläge einer Zuschlagstabelle in eine andere Tabelle kopieren können.
- "Zuschläge kopieren" auf Seite B-701

### Bearbeitung
- **Preistabelle**: Nummer der Preistabelle für Bearbeitungen.
- **Preisjahrgang, Preisschlüssel**: Preisjahrgang und -schlüssel (Tarif), die bei Bearbeitungen von Modellen herangezogen werden.
- **Preis-Typ**: Der Preistyp gibt an, wie die Werte in den Feldern Segment interpretiert werden sollen, z. B. als prozentualen Aufschlag auf den Preis, als Betrag pro Länge oder pro Stück.

### Zuschläge
Je nach Modell werden die Felder **Segment 1** bis **Segment 8** freigeschaltet, in denen Sie die Werte für den Zuschlag eingeben können. Der Wert wird je nach Preistyp als prozentualer Zuschlag oder als Betrag interpretiert (für alle Segmente).
Je nach Schwierigkeit der Bearbeitung können die Werte unterschiedlich groß sein. So kann z. B. für die Bearbeitung einer gebogenen Kante ein höherer Zuschlag berechnet werden als für eine gerade Kante.

### Modell
- **Nummer**: Nummer des Modells, für das der Zuschlag berechnet werden soll. Wenn Sie ein Modell angegeben haben, wird im Feld **Skizze** eine schematische Darstellung des Modells mit den Segmenten angezeigt, für die Werte eingegeben werden können.
- **Skizze**: Schematische Darstellung des Modells, aus der Sie die Nummern der Segmente ablesen können. Die äußeren Nummern bezeichnen die Kanten, die inneren die Ecken.

### Mindest-Angaben
- **Mindestpreis**: Wenn Sie einen Mindestpreis angeben, wird dieser immer dann als Basis für den Zuschlag herangezogen, wenn der Preis der Bearbeitung im Auftrag darunterliegt. Diese Angabe eignet sich nicht für den Preistyp **Stück**.
- **Mindestmenge**: Wenn Sie eine Mindestmenge angeben, wird diese immer dann als Basis für den Zuschlag herangezogen, wenn der Preis der Bearbeitung im Auftrag darunterliegt. Diese Angabe eignet sich besonders für den Preistyp **Stück**.

### Tabelle
In der Übersicht werden alle Modellzuschläge aufgelistet, die den Auswahlkriterien entsprechen.
