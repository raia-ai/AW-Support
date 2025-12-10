---
title: "DE-HB-AWEnterprise_17"
source: "DE-HB-AWEnterprise_17.pdf"
tags: ["A+W Enterprise", "Einkauf", "Lager", "ERP", "Software Reference", "German", "Vorgangsverwaltung", "Bestellungen", "Wareneingang", "Rechnungen"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for the A+W Enterprise system, specifically covering the 'Einkauf' (Purchasing) and 'Lager' (Warehouse/Inventory) modules. It details functionalities for order management, goods receipt, invoicing, and inventory control."
long_description: "This comprehensive technical manual provides detailed descriptions of the A+W Enterprise software, focusing on the Purchasing (Einkauf) and Warehouse/Inventory (Lager) modules. The Purchasing section covers the entire procurement process, from creating and managing purchase orders (`Bestellungen`) to handling goods receipts (`Wareneingang`), and processing supplier invoices (`Rechnungen`) and credit notes (`Gutschriften`). It explains various fields, functions, and system dialogs, including order release (`Bestellfreigabe`), document management (`Dokumentenartenzuordnung`), and different order types. The Warehouse section details inventory management functions, such as goods movements (receipts and issues), managing different storage types (standard, bin, rack, batch), and performing inventory counts (`Inventur`) and valuations (`Bewertung`). The manual is structured to serve as a reference for users, providing technical information, database field names (`DB-Feld`), and step-by-step instructions for navigating the system. It is intended for users and administrators of the A+W Enterprise system to understand and effectively utilize its purchasing and inventory management capabilities."
---

# A+W Enterprise Einkauf
---
## Vorgangsverwaltung

**(CAD-Kennzeichen)** Kennzeichen, ob der Position eine CAD-Datei zugeordnet ist. Wenn eine CAD-Datei angehängt ist, wird das Kennzeichen CAD angezeigt. Bei S/N-Positionen wird der S/N-Code in Klammern hinter dem CAD-Kennzeichen angezeigt.
**Technische Info:** Anzeigefeld

**(Kostenstelle)** Bezeichnung der Kostenstelle, die der Position zugeordnet ist. Wenn der Position keine Kostenstelle zugeordnet ist, wird die marktpartnerspezifische Kostenstelle herangezogen. Wenn dem Marktpartner auch keine Kostenstelle zugeordnet ist, wird die Hauptkostenstelle herangezogen.
**Technische Info:** Anzeigefeld, DB-Feld: kpos.kostenst

**(Sprossenkennzeichen)** Kennzeichen, ob in der Position Sprossen erfasst sind.
*   **S:** In der Position sind Sprossen erfasst. Der Sprossenaufbau wurde nicht bearbeitet.
*   **E:** In der Position sind Sprossen erfasst. Der Sprossenaufbau wurde im Editor bearbeitet.
*   **(Kein Kennzeichen):** In der Position sind keine Sprossen erfasst.
**Technische Info:** Anzeigefeld

**(Kopfartikel, Artikel)** Bezeichnung des Kopfartikels. Bei Mehrfachgläsern werden neben dem Kopfartikel die Bezeichnungen der einzelnen Gläser angezeigt.
**Technische Info:** Anzeigefelder, DB-Feld: aufstrukt.artbez1

**(Austausch-, Zusatzartikel, Anzahl1/Anzahl2)** Bezeichnung der Austausch- und Zusatzartikel und Anzahl der Artikel in der Stückliste. Austausch-artikel werden mit einem A, Zusatzartikel mit einem Z vor der Bezeichnung angezeigt. Hinter der Artikelbezeichnung wird angezeigt, wie oft für den Artikel der Wert Breite und wie oft der Wert Höhe berechnet werden muss.
**Technische Info:** Anzeigefelder, DB-Felder: aufstrukt.artbez1, aufstrukt.an-zahl1, aufstrukt.anzahl2

**(Sprossenaustausch-, Sprossenzusatzartikel, Anzahl1/Anzahl2)** Bezeichnung der Sprossenaustausch- und/oder Sprossenzusatzartikel und Anzahl der Sprossen in der Stückliste. Sprossenaustauschartikel werden mit einem A, Sprossenzusatzartikel mit einem Z vor der Bezeichnung angezeigt. Hinter der Sprossenbezeichnung wird die Anzahl der waagerechten und/oder senkrechten Sprossen angezeigt.
**Technische Info:** Anzeigefelder, DB-Felder: aufstrukt.artbez1, aufstrukt.an-zahl1, aufstrukt.anzahl2

## Register Positionen (Info-Bereich – Grafik, Technische Werte)

Im rechten Bereich im Register Positionen werden, abhängig von der System-konfiguration und den Einstellungen, eine der folgenden Informationen angezeigt:

*   Beschaffung, Warengruppe und Modell
*   Technische Werte
*   Verdeckte Maßangaben

Die Informationen werden zu der markiert Position angezeigt.

