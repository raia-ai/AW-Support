---
title: "DE_AWBusiness_Einkauf_3_3"
source: "DE_AWBusiness_Einkauf_3_3.pdf"
tags: ["A+W Business", "Einkauf", "Bestellungen", "Liefertermine", "Wareneingang", "Rechnungskontrolle", "Tutorial", "ERP-Software", "EDI", "openTRANS"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the purchasing module of the A+W Business software. It covers the complete procurement process, from checking and correcting delivery dates, handling customer notifications, creating inquiries, processing goods receipts for various item types (including crates), and performing price and invoice verification."
long_description: "This comprehensive tutorial guides users through the procurement functionalities of the A+W Business ERP software. It is structured to train users on the entire purchasing workflow, starting with the management of delivery dates. It details how to check and adjust delivery dates received from suppliers, notify customers of any changes, and modify dates across different system dialogs like Document Management and Customer Notification. The guide then moves to creating and managing inquiries for purchase items, explaining how to generate an inquiry from a customer order and subsequently create a purchase order from a referenced inquiry. A significant portion is dedicated to the goods receipt process. It explains how to record complete or partial deliveries, handle items with and without stock IDs, process overages, and manage the receipt of crated goods with unique identifiers (IDs). The tutorial also covers how to check the completeness of deliveries using the incoming goods control dialog. The final major section focuses on price and invoice verification. It details the process of checking supplier invoices against purchase orders, handling price discrepancies, managing collective invoices, and the impact of these checks on document statuses and purchase price updates in related customer orders. The document concludes with a section on electronic document interchange (EDI and openTRANS), explaining how orders, order confirmations, and invoices can be exchanged electronically. Throughout the tutorial, step-by-step instructions are provided, supplemented with screenshots of the user interface to ensure clarity."
---

---
## Prüfung und Korrektur von Lieferterminen

Ihr Lieferant wird die Termine aus Ihren Bestellungen bestätigen oder korrigieren. Die vom Lieferanten erhaltenen Auftragsbestätigungen und Liefertermine ordnen Sie den Bestellungen zu, indem Sie die Lieferanten-AB erfassen. Dabei werden die geänderten Termine automatisch in die referenzierten Dokumente übernommen.

Für die Benachrichtigung des Kunden können Sie den Dialog Kundenbenachrichtigung oder die Möglichkeiten im Menü Kommunikation nutzen – oder einfach anrufen.

Den Liefertermin selbst können Sie in verschiedenen Dialogen ändern:

*   Dokumentenverwaltung (Auftrag, Bestellung)
*   Dokumentendaten
*   Kundenbenachrichtigung (Lieferterminkontrolle)
*   AB Lieferant
*   Eingangskontrolle

Sie korrigieren die Termine in aller Regel in den Bestellungen, wodurch sie in die referenzierten Aufträge zurückgeschrieben werden.

### Kundenbenachrichtigung

Sie können den Kunden aus dem Dialog Kundenbenachrichtigung (Lieferterminkontrolle) heraus über die Terminverschiebung informieren. Dazu muss in den Stammdaten des Kunden eine E-Mail-Adresse hinterlegt sein. Im Auftrag muss im Bereich Anschrift die Checkbox Mail aktiviert sein.

## Liefertermine ändern und Kunden benachrichtigen

Zu den Bestellungen und referenzierten Aufträgen müssen Sie Liefertermine prüfen, korrigieren und den ggf. den Kunden benachrichtigen, wenn die Termine nicht eingehalten werden können. Diese Schritte sind über den Dialog Kundenbenachrichtigung möglich.

Sie können ihn auf folgende Weise öffnen:
*   Auftrag oder Bestellung > Funktionen > Gruppe Dokument > Lieferterminkontrolle
*   Dokumente > Kundenbenachrichtigung

Wenn Sie auch die Termine für die Produktion prüfen und korrigieren wollen, können Sie den Dialog Dokumentendaten nutzen.
⇨ "So prüfen und ändern Sie die Dokumentendaten" auf Seite D-105

### So ändern Sie den Liefertermin

1.  Öffnen Sie ggf. den Auftrag, dessen Termine Sie prüfen wollen oder geändert haben.
2.  Wählen Sie Dokumente > Kundenbenachrichtigung.

