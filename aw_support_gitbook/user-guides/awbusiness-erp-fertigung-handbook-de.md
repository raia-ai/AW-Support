---
title: "D-HB-AWBusiness_25"
source: "D-HB-AWBusiness_25.pdf"
tags: ["A+W Business", "ERP", "Fertigung", "Lieferwesen", "Produktionsplanung", "Kommissionierung", "Gestellverwaltung", "Software-Tutorial", "Softwarereferenz"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial and software reference for the A+W Business Fertigung (Manufacturing) module, covering delivery organization, vehicle and driver management, picking, goods issue, and production planning."
long_description: "This document serves as a comprehensive guide for the 'Fertigung' (Manufacturing) module of the A+W Business software. It is divided into two main parts: a tutorial and a software reference. The tutorial section provides step-by-step instructions on various processes within the manufacturing and logistics workflow. Key topics include organizing deliveries, creating and managing vehicles and drivers, assembling vehicle loads (Kommissionierung), printing driver lists, and creating schedule and capacity overviews. It also details additional functions like handling production orders, calculating freight costs, and managing the goods issue of crates. The tutorial is supplemented with exercises and references to more detailed information. The second part of the document is a detailed software reference, offering an in-depth look at the dialogs, menus, and settings for functionalities like production handover, barcode scanning, production data management, delivery services, rack management, and customs administration. This reference section acts as a technical manual for users who need to understand the specifics of each function and its configuration options within the A+W Business system."
---

# Tutorial: Lieferwesen

---
## Organisation der Auslieferung
Mit der Tourenplanung haben Sie den Versand geplant. Sie können nun die Auslieferung der gefertigten Aufträge mit einem eigenen Fuhrpark planen. Die Kommissionierung dient dazu, die Aufträge pro Liefertermin und Tour zusammenzustellen und einem Fahrzeug zuzuweisen.

Damit Sie Fahrzeuge und Fahrer zuordnen können, müssen diese in den Stammdaten angelegt sein. Zu jedem Lkw hinterlegen Sie das Leergewicht und das zulässige Gesamtgewicht. A+W Business prüft bei der Zuordnung von Aufträgen, ob dieses Gesamtgewicht erreicht oder sogar überschritten ist. Wenn im Dialog Kommissionierung angezeigt wird, dass der Lkw überladen ist, müssen die selektierten Aufträge einer anderen Tour, einem anderen Lkw und/oder einem anderen Liefertermin zugeordnet werden.

Sie können jedem Fahrzeug auch einen Fahrer zuordnen, der jedoch nicht zwingend in die Kommissionierung übernommen wird.

Für die Kommissionierung können die Aufträge automatisch in einem Nummernverwalter gesammelt werden. Aus diesem heraus kann dann die entsprechende Packmittelbeladungsliste oder Empfangsbestätigungsliste gedruckt werden.

Mit dem Ausdruck verschiedener Listen unterstützen Sie die Fahrer bei der Beladung und bei der Lieferung.

> **Voraussetzung**
> Wenn Sie den Fahrzeugen Fahrer zuordnen wollen, müssen Sie zuerst die Namen der Fahrer in den Stammdaten hinterlegen.

### Fahrzeug anlegen
Um die Lieferungen einer Tour zusammenzustellen, ordnen Sie die Aufträge einem Fahrzeug zu. Nur wenn die Daten für die Fahrzeuge korrekt eingetragen sind, kann das System prüfen, ob das ausgewählte Fahrzeug richtig ausgelastet oder überladen ist. In diesem Abschnitt lernen Sie, wie Sie Stammdaten für Fahrzeuge anlegen.

**So legen Sie ein Fahrzeug an**
1. Wählen Sie im Menü Stammdaten > Versand > LKW.

   