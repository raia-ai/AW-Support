---
title: "D-AWBusiness-HB_10"
source: "D-AWBusiness-HB_10.pdf"
tags: ["A+W Business", "Stammdaten", "ERP", "Software-Referenz", "Kundenverwaltung", "Lieferantenverwaltung", "Auftragsverwaltung", "Fertigungssteuerung", "Glasindustrie"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W Business, focusing on master data management (`Stammdaten`). It provides detailed instructions on configuring and managing data for customers (`Kunde`), suppliers (`Lieferant`), orders (`Auftrag`), and production (`Fertigung`). It covers topics like article management, delivery times, object billing, rounding rules, and production settings."
long_description: "This comprehensive technical manual serves as a software reference for the A+W Business ERP system, specifically detailing the setup and maintenance of master data (`Stammdaten`). The guide is structured into several key areas, providing users with a step-by-step approach to configuring the system's core data entities. The 'Kunde' (Customer) section explains how to manage customer-specific articles, delivery durations, and object-based billing. The 'Lieferant' (Supplier) section mirrors this structure, covering supplier data, product catalogs, and delivery terms. The 'Auftrag' (Order) section details the configuration of rounding rules, status management, document types, and number ranges essential for order processing. The 'Fertigung' (Production) section outlines the setup for production-related data, including optimization parameters, production feedback stations, cutting tables, and work processes. The document is highly structured, using screenshots, field descriptions, and practical examples to illustrate the software's functionality. It is intended for system administrators and power users responsible for the initial setup and ongoing management of the A+W Business system, particularly within the glass and window manufacturing industry."
---

# A+W Business Stammdaten

---
## Kunde

### Artikel
Alphanumerische Artikelnummer (Produktnummer), unter der das Produkt z. B. beim Kunden geführt wird. Im Auftrag kann das Produkt über diese Nummer erfasst werden.

> **Beispiel**
> Der Kunde bestellt regelmäßig ein ESG mit Beschichtung in der Größe 1200 x 1800 mm. Sie legen dieses Produkt in den Stammdaten an und weisen es dann als kundenindividuelles Produkt dem Kunden zu. Dabei verwenden Sie bronze als Artikelnummer.
> In der Positionserfassung tragen Sie im Eingabefeld als Produktnummer bronze ein. Das Produkt wird mit den Maßen aus der Produktverwaltung angezeigt.

### Bezeichnung (1-3)
Name und kurze Beschreibung des Produkts. Die Bezeichnung wird in der Positionserfassung angezeigt und beim Formulardruck ausgewertet.
Bei Einzelscheiben, die in eine ISO-Einheit eingebaut werden, wird nur die erste Bezeichnung ausgewiesen.

### EAN
EAN-Code (European Article Number) oder GTIN-Code (Global Trade Item Number). In den USA kann das Feld für den UPC-Code (Universal Product Code) verwendet werden.

### Zusatztext
Sie können dem Produkt einen Text zuordnen, auf den bei der Erfassung als Position hingewiesen wird.

### Eigener Artikel

**Artikel**
Produktnummer, unter der das Produkt in A+W Business geführt wird.

### Übersicht
In der Übersicht werden alle Kunden aufgelistet, zu denen kundenindividuelle Produkte angelegt sind.

## Lieferdauer (Kunde, Lieferant)

**Stammdaten > Marktpartner > Kunde, Lieferant > Lieferdauer**

