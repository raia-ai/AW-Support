---
title: "DE_AWBusiness_Verkauf_4_3"
source: "DE_AWBusiness_Verkauf_4_3.pdf"
tags: ["A+W Business", "ERP", "Sales Management", "Document Management", "Invoicing", "Tutorial", "German", "Formularverwaltung", "Preisdruck", "Mahnwesen"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive German-language tutorial for the A+W Business sales software. It guides users through the complete workflow from creating documents like quotes and orders to final invoicing, covering key functionalities such as form management, price printing settings, dunning processes, and status management."
long_description: "This tutorial provides a detailed, step-by-step guide to using the A+W Business Verkauf (Sales) module. It is designed for users who handle the entire sales process, from initial document creation to final invoicing and payment tracking. The document is structured into several key chapters. It begins with 'Formularverwaltung' (Form Management), explaining how to configure price printing options on different forms. The tutorial then moves to practical tasks like 'Dokument drucken' (Printing Documents), covering invoices, order confirmations, and labels, including procedures for handling reprints and collective print runs. A significant portion is dedicated to 'Rechnungen' (Invoices), which details different invoice types, due date calculations, and payment processing ('Zahlungseingang'). The 'Mahnwesen' (Dunning) section explains how to track open invoices, record payments, and issue reminders. The document also covers 'Dokumenten-Historie' (Document History) for auditing changes and 'Status' management to control the document lifecycle through various internal processes. Further sections explain how to manage user rights ('Mitarbeiterrechte') and how to use the copy function to efficiently create new documents like partial deliveries ('Teillieferungen'), down payments ('Anzahlungen'), complaints ('Reklamationen'), and credit notes ('Gutschriften'). The tutorial concludes with the 'Bestellung' (Purchasing) process, explaining how to handle order items and transfer them to the purchasing department. Throughout the document, screenshots, tables, and callout notes provide clear, visual instructions."
---

# Kompletterfassung von Dokumenten bis Faktura

---
## Formularverwaltung

Die Einstellung in der Formularverwaltung lässt folgende Möglichkeiten zu:

- **0 - Kein Druck:**
  Im Formulardruck werden die Angaben aus dem Dokument übernommen:
    - **0 - Kein Druck:** Preise werden nicht gedruckt.
    - **1 - Alle Preise:** Preise werden pro Auftragsposition gedruckt.
    - **2 - Nur Summen:** Nur die Positionssummen werden gedruckt.
- **1 - Alle Preise:**
  Die Einstellungen aus dem Dokument werden ignoriert. Die Preise werden pro Auftragsposition gedruckt.
- **2 - Nur Summen:**
  Im Formulardruck werden die Angaben aus dem Dokument übernommen:
    - **0 - Kein Druck:** Preise werden nicht gedruckt.
    - **1 - Alle Preise:** Preise werden pro Auftragsposition gedruckt.
    - **2 - Nur Summen:** Nur die Positionssummen werden gedruckt.

*(Seite C-201)*

---

### Einstellungen für den Preisdruck

Der Druck der Preise wird von der Formularverwaltung und von der Einstellung im Dokument gesteuert.

| Einstellungen | Druck |
| :--- | :--- |
| **Dokument** | **Formularverw.** | **Positionspreise** | **Summenpreise** |
| 0 | 0 | - | X |
| 1 | 0 | X | X |
| 2 | 0 | - | X |
| 0 | 1 | X | X |
| 1 | 1 | X | X |
| 2 | 1 | X | X |
| 0 | 2 | - | X |
| 1 | 2 | - | X |
| 2 | 2 | - | X |

**Legende:**
**Dokumente**
- 0 = Kein Druck
- 1 = Alle Preise
- 2 = Nur Summen

**Formularverwaltung**
- 0 = Standard (Dokument entscheidet)
- 1 = Preise immer drucken
- 2 = Preise immer drucken (Summenmodus)

- = kein Druck, X = Druck

> **Beispiel**
> Wenn im Dokument Summen drucken (2) eingestellt ist und in der Formularverwaltung Standard (0), werden nur Summenpreise gedruckt, jedoch keine Positionspreise.

*(Seite C-202)*

---

## Dokument drucken

In dieser Einheit lernen Sie, wie Sie Dokumente drucken. Die hinterlegten Formulare werden dem Druckmodus entsprechend zur Auswahl angeboten. In diesem Beispiel wird eine Rechnung gedruckt. Mit demselben Ablauf drucken Sie auch Auftragsbestätigungen, Lieferscheine, Fertigungsscheine usw.

> **Druck von Sammelrechnungen**
> Prüfen Sie vor dem Druck einer Sammelrechnung die Sortierreihenfolge in dem Nummernverwalter, in dem sich die Rechnungen befinden. Der Druck von Sammelrechnungen wird unterbrochen, wenn sich eines der Kriterien für Sammelrechnungen unterscheidet.

### So drucken Sie eine Rechnung

1.  Wählen Sie Dokumente > Auftrag > Druck Auftrag.

