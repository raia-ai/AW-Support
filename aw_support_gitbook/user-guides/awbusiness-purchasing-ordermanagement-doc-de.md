---
title: "DE_AWBusiness_Einkauf_3_5"
source: "DE_AWBusiness_Einkauf_3_5.pdf"
tags: ["A+W Business", "Purchasing", "Order Management", "Goods Receipt", "Invoice Control", "Software Reference", "ERP", "Supplier Management", "Price Control"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Business Purchasing module, covering order management, supplier confirmations, price control, goods receipt, and invoice verification."
long_description: "This is a detailed software reference manual for the A+W Business ERP system, specifically focusing on the Purchasing (Einkauf) module. The document provides a comprehensive overview of the processes and functionalities involved in managing procurement activities. Key sections include: 'Bestellpositionen' (Order Items), which details the fields and data related to individual items in a purchase order. 'Auftragsbestätigung' (Order Confirmation), which explains how to handle supplier confirmations, including both manual and electronic price control (Preiskontrolle) via openTRANS format. It covers checking prices, handling discrepancies, and managing collective invoices. 'Mahnung' (Dunning), which describes the process for sending reminders for overdue deliveries. 'Wareneingang' (Goods Receipt), which outlines the steps for recording incoming goods, either for complete or partial deliveries, and includes special procedures for items delivered in crates, such as assigning unique identification numbers (Identnummern). 'Rechnung' (Invoice), which details the invoice control (Rechnungskontrolle) process, where supplier invoices are checked against orders and goods receipts before being forwarded to accounting. The guide is intended for users of the A+W Business software to understand and effectively use the purchasing functionalities."
---

# Softwarereferenz: Bestellung (Menü)

---
## Bestellpositionen

Übersicht über alle Positionen der Bestellung. Wenn die Bestellung aus einem Kundenauftrag erzeugt wurde, können die Bestellpositionen zugleich die Positionen des referenzierten Auftrags sein.

*   **Pos. Nr.:**
    Nummer der Bestellposition. Bei einer Kundenbestellung kann dies auch die Positionsnummer aus dem Auftrag sein.
*   **Artikelbezeichnung:**
    Nummer und Bezeichnung der bestellten Position.
*   **Menge:**
    Menge der bestellten Position.
*   **Breite / Höhe:**
    Maße der bestellten Position.
*   **Lieferanten-AB:**
    Nummer der Auftragsbestätigung des Lieferanten. Wenn Sie die AB-Nummer für die gesamte Bestellung erfasst haben, wird für alle Positionen dieselbe Nummer angezeigt.
*   **Teilliefertermin:**
    Liefertermin für die Teillieferung.
*   **Pr./PE:**
    EK-Preis pro Preiseinheit der bestellten Position.
*   **Pr./PE Gesamt:**
    Gesamtpreis pro Preiseinheit der bestellten Position.
*   **Liste/Schlüssel:**
    Preisliste und Preisschlüssel, die für den zugrundegelegten Einkaufspreis (EK) gelten.
*   **Rabatt:**
    Rabatt, der auf den EK gewährt wird.
*   **Netto/Pos:**
    Betrag der Position ohne Rabatt und/oder Zuschläge.
*   **Netto/Pos Gesamt:**
    Betrag aller Positionen der Bestellung ohne Rabatt und/oder Zuschläge.
*   **Preiseinheit Anzahl:**
    Menge in der angezeigten Preiseinheit.
*   **Preiseinheit:**
    Preiseinheit für den angezeigten Preis.
*   **Stückpreis:**
    Stückpreis der markierten Position inklusive aller Komponenten. Er wird über die Preiseinheit, die Zuschläge und Rabatte errechnet.
*   **Auftrag:**
    Auftragsnummer.
*   **Bezeichnung:**
    Produktbezeichnung aus dem referenzierten Auftrag. Sie können in der Bestellung eine abweichende Lieferantenbezeichnung angeben.

## AB-Lieferant – Positionen

*Dokumente > Bestellung > AB Lieferant > Register Positionen*

