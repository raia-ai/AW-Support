---
title: "DE_AWEnterprise_Versandsteuerung"
source: "DE_AWEnterprise_Versandsteuerung.pdf"
tags: ["A+W Enterprise", "Versandsteuerung", "Logistik", "Software", "Handbuch", "Glas", "Fenster", "Türen", "shipping control", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is the software reference manual for A+W Enterprise Versandsteuerung (Shipping Control), a module within the A+W Enterprise software suite. It provides detailed instructions and descriptions for managing shipping processes, from order entry to delivery, specifically tailored for the glass, windows, and doors industry."
long_description: "This comprehensive software reference guide details the functionality of the A+W Enterprise Versandsteuerung (Shipping Control) module, part of the A+W software for the glass, windows, and doors industry. The document serves as a user manual for end-users, covering all aspects of shipping management. It begins with an editorial section, including a revision history and copyright information. The core of the manual is the 'Softwarereferenz,' which provides a detailed overview of the module's architecture, organized into four main levels: delivery dates, tours, orders, and positions. It explains the various start functions, such as program start, order search, and market partner search. A significant portion is dedicated to the 'Versand-Explorer,' a tree-structured interface for navigating shipping data. The manual meticulously describes the user interface elements, including menus, buttons, and registers (tabs) for different data levels like 'TourenInfo,' 'AuftragsInfo,' and 'PositionsInfo.' It covers a wide range of functions, such as searching, moving items, booking goods receipts, handling missing quantities, managing racks (Gestelle), printing documents (delivery notes, loading lists), and integrating with logistics optimizers. The document is highly structured, with clear references to page numbers, screenshots of the user interface, and detailed explanations of each field and function, including their technical database field names. It is an essential resource for planning, executing, and monitoring all shipping-related activities within the A+W Enterprise system."
---

# A+W Versandsteuerung

A+W - Software for Glass, Windows and Doors

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Software Version | Beschreibung |
| :--- | :--- | :--- |
| 2.00/04-2022 | 6 | Aktualisierung der Softwarereferenz. |
| 1.03/01-2017 | 5.2.4 | Produkt- und Firmennamen angepasst. |
| 1.02/02-2014 | 5.2.4 | Produktnamen aktualisiert |
| 1.01/01-2013 | 5.2.4 | Layout an CI 2013 angepasst |
| 1.00/11-2012 | 5.2.4 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen
*   Kontakte

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Enterprise gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

#### Urheberrechte

© 2022, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte

**A+W Software GmbH**
Am Pfahlgraben 4-10
35415 Pohlheim

+49 6404 2051-0
+49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

## Softwarereferenz

### Übersicht

Alle Ansichten, Dialoge und Funktionen für die Versandsteuerung sind über das Modul Logistik erreichbar. Sie können das Modul auch direkt aus dem Fix-Win starten. In der Standard-Konfiguration starten Sie direkt mit dem Versand-Explorer:
⇨ "Versand-Explorer"

Mit der Versandsteuerung finden, planen, bearbeiten und versenden Sie termingerecht Ihre Lieferaufträge. Die Versandsteuerung ist die Steuerzentrale für das Versandgeschäft und ermöglicht den einfachen und schnellen Zugriff auf alle Lieferaufträge. Sie erstellen z. B. eine Auflistung aller Liefertermine eines Zeitraums oder springen direkt in den gesuchten Lieferauftrag. Für die Übersicht der Versandvorgänge ist jeder Lieferauftrag in die folgenden vier Ebenen eingeteilt:

*   Liefertermine
*   Touren mit Routen
*   Aufträge
*   Positionen

Die Liefertermine sehen Sie in der ersten Ebene. Ein Liefertermin enthält die zugehörigen Touren oder Routen.

Die Touren mit den Routen sehen Sie in der zweiten Ebene. Eine Tour enthält die zugehörigen Aufträge und kann aus einer oder mehreren Routen bestehen. Eine Tour steht für mindestens eine Route, die zu einem bestimmten Liefertermin gefahren wird. Die Route steht für eine festgelegte Fahrstrecke. Die Routen können auf bestimmte Wochentage oder auf bestimmte Zeiten festgelegt werden. In der Tourenebene haben Sie eine Übersicht zu den vorhandenen Versandpapieren.

Die Aufträge sehen Sie in der dritten Ebene. Ein Auftrag enthält die zugehörigen Positionen und die Lieferanschrift. In der Auftragsebene haben Sie eine Übersicht zu den vorhandenen Versandpapieren.

Die Positionen sehen Sie in der vierten Ebene. Eine Position enthält die zugehörigen Einheiten.

Geöffnete Touren, Aufträge oder Positionen sind für andere Mitarbeiter zur Bearbeitung gesperrt. sie werden dann nur mit Leserecht geöffnet.

### Startfunktionen

In A+W Enterprise haben Sie die Möglichkeit, über verschiedene Suchfunktionen Ihre Liefertermine und Aufträge zu suchen.
Zu diesem Thema finden Sie folgende Informationen:
⇨ "Programmstart"
⇨ "Auftragssuche"
⇨ "Marktpartnersuche"

#### Programmstart

*Logistik > Versandsteuerung*

