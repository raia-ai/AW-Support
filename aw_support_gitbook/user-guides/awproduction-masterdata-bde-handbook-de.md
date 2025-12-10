---
title: "DE_HB_AWProduction_11"
source: "DE_HB_AWProduction_11.pdf"
tags: ["A+W Production", "Software Reference", "Master Data", "BDE", "Packing Optimization", "Stammdaten", "Packmitteloptimierung", "Tutorial", "PackView", "Gestelle"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference and tutorial for the A+W Production system, focusing on Master Data (Stammdaten) for Shop Floor Data Collection (BDE) and the Packing Material Optimization (Packmitteloptimierung) module. It provides detailed explanations of dialogs, fields, and functions related to managing racks (Gestelle), statuses (Zustände), employees (Mitarbeiter), and various feedback settings."
long_description: "This extensive manual serves as a comprehensive guide for users of the A+W Production software. It is divided into two main parts: a software reference for master data management and a tutorial for the Packing Material Optimization (PMO) module. The first part, \"Softwarereferenz - Stammdaten,\" details the setup and configuration of essential master data for Shop Floor Data Collection (BDE). This includes in-depth descriptions of dialogs for managing equipment (Betriebsmittel), feedback settings, racks (Gestelle), status types (Zustandstypen), employees (Mitarbeiter), and column mappings (Spaltenzuordnung). Each section explains the purpose of various fields, checkboxes, and their corresponding database fields. The second part, \"Packmitteloptimierung,\" begins with a tutorial that explains the fundamental concepts, master data setup (*.RUL and *.VAL files), and visualization of optimization results using the PackView tool. It covers different display modes, editing functions, and manual manipulation of packing layouts. The tutorial is followed by a software reference section for PMO, providing a detailed breakdown of menus, dialogs, and functions within the PackView application, enabling users to understand and effectively manage the packing of finished goods onto transport racks."
---

# Softwarereferenz - Stammdaten

---
## Betriebsmittel der Auftragserfassung
In diesem Feld wird Ihnen das Betriebsmittel der Auftragserfassung angezeigt. Dieses Feld wird an die Auftragserfassung zurück gemeldet. D. h., wenn Sie den Eintrag ändern, wird das geänderte Betriebsmittel zurück gemeldet.

**Technische Info:** Datenbankfeld: Maschinennr

## Erläuterung der Felder im Bereich Rückmeldung von Buchungen

### Bearbeitungsrückmeldung
Diese Checkbox steuert, ob Rückmeldungen bezüglich der Bearbeitungen erfolgen oder nicht. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Wird eine Scheibe auf eine Erfassungsstelle gebucht, dann wird der Bearbeitungsfortschritt scheibengenau als Änderungsmeldung in die Datei STSD*.ASC geschrieben.

### Gestellrückmeldung
Diese Checkbox steuert, ob Rückmeldungen bezüglich der Gestellbelegung erfolgen oder nicht. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Wird ein Gestell auf eine Erfassungsstelle gebucht, dann wird die Gestellbelegung scheibengenau als Snapshot (Momentaufnahme) in die Datei STSG*.ASC geschrieben.

### Gestellbelegung an Gestellserver melden
Diese Checkbox steuert, ob die Gestellbelegung an den Gestellserver gemeldet werden soll oder nicht. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung an den Gestellserver.
- Die Gestellbelegung wird an den Gestellserver zurück gemeldet.

### Einheitenrückmeldung (STSU*.asc)
Über diese Checkbox ist es möglich, im A+W Business eine Zuordnung der A+W Production-Etiketten zur A+W Business-Auftragspositionen vorzunehmen. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Wird eine Einheit auf eine Erfassungsstelle gebucht, dann wird der Bearbeitungsfortschritt scheibengenau als Änderungsmeldung in die Datei STSU*.ASC geschrieben.

### Produktionsrückmeldung
Diese Checkbox dient dazu, den aktuellen Auftragsstatus im A+W Business zu aktualisieren. Mögliche Werte sind:
- Es erfolgt keine Rückmeldung.
- Der aktuelle Auftragsstatus im A+W Business wird aktualisiert.

### Ergänzende Informationen
- ⇨ Tutorial, "Erfassungsstellen" auf Seite H-923
- ⇨ Tutorial, "Fehlergestell (Error-Rack)" auf Seite H-924
- ⇨ Tutorial, "Erfassungsstelle Lkw" auf Seite H-929
- ⇨ "Zustände" auf Seite H-1008
- ⇨ "Erfassungsstellen-Typen" auf Seite H-997

---
*A+W Production Betriebsdatenerfassung*
*H-1001*
---

# Stammdaten - Gestelle
Stammdaten > BDE > Gestelle

**Abb. H-5 Gestelle**
