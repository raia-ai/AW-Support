---
title: "A+W Business Stammdaten und Dokumente Tutorials"
source: "D-HB-AWBusiness_5.pdf"
tags: ["A+W Business", "Stammdaten", "Zuschläge", "Rabatte", "Mitarbeiterverwaltung", "Dokumentenverwaltung", "Preisberechnung", "Software-Tutorial", "ERP-System"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a collection of tutorials for the A+W Business software, covering master data management for surcharges (Zuschläge), discounts (Rabatte), and additional company settings (Zusatzinformationen zur Firma). It also includes a detailed tutorial on document management, including order entry, status management, and number ranges."
long_description: "This document serves as a comprehensive training guide for users of the A+W Business ERP system, focusing on master data (Stammdaten) and document processing. The first major section, 'Tutorial 1', details the configuration of surcharges and discounts. It explains how to create position-based and summary surcharges, fix automatic surcharges, and handle complex pricing scenarios using multi-dimensional price cubes (Würfel). It provides step-by-step instructions for defining various discount types, such as standard, tiered, and exchange discounts, and explains the discount hierarchy and search logic within the system. The second part of 'Tutorial 1' covers additional company information, including the setup of clients (Mandanten), branches (Filialen), employee data, user rights, and sales representative commissions. The second major section, 'Tutorial 2', focuses on 'Dokumente' (Documents). It explains the fundamentals of document processing, from creating a test order to understand the interaction of master data, to detailed status management which maps business workflows. It covers the function of number administrators (Nummernverwalter), number ranges (Nummernkreise), and rounding rules (Rundungen). Each section includes definitions, step-by-step instructions with screenshots, complex exercises, and references to other parts of the software documentation."
---

# Tutorial 1: Master Data

---
## Zuschläge (Surcharges)

In diesem Beispiel wird die Gültigkeit auf den 31.12. des aktuellen Jahres begrenzt.

**7. Tragen Sie die Position im Dokument (D) ein:**
- **0** für einen positionsbezogenen Zuschlag/Rabatt, z. B. bei einem Zuschlag für die Überschreitung der maximalen Fläche. Er wird bei jeder Position eingefügt, auf die er zutrifft.
- **900 - 999** für Zuschläge/Rabatte, die auf alle vorherigen oder Teile der vorherigen Positionen wirken sollen.

