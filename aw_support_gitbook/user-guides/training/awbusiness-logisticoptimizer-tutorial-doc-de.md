---
title: "DE_AWBusiness_LogisticOptimizer_2_3"
source: "DE_AWBusiness_LogisticOptimizer_2_3.pdf"
tags: ["A+W Business", "Logistic Optimizer", "Tutorial", "Software Reference", "Tour Planning", "GPS Tracking", "Delivery Management", "Route Optimization", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive user manual for the A+W Business Logistic Optimizer software, provided in German. It is split into two main parts: a step-by-step tutorial and a detailed software reference guide. The tutorial covers practical workflows such as driving and monitoring tours, using the mobile app, and generating queries and reports. The reference section provides in-depth explanations of configuration settings, administrative functions, and system parameters."
long_description: "This document serves as a complete guide for the A+W Business Logistic Optimizer, a software designed for tour and delivery management. It is written in German and structured into a 'Tutorial' and a 'Softwarereferenz' (Software Reference). The Tutorial section guides users through the entire lifecycle of a tour, from preparation (setting tour status, uploading documents to the cloud) and execution (using the GDC mobile app, booking data, capturing signatures) to monitoring (live tracking of vehicles and delivery status). It also details how to generate various queries and reports, including tour histories, delivery lists, and statistical analyses. The Software Reference section acts as a technical dictionary for the application. It meticulously explains all configuration options (database connections, system parameters like routing behavior and cost factors), administrative tasks (user management, status definitions, vehicle and driver setup), and data import/export functionalities. This part is essential for administrators and advanced users who need to customize and maintain the system. Overall, the manual is designed to enable both new users to learn the software's core functionalities and experienced users to master its advanced features and settings."
---

# Tutorial

---
## Ergebnisse prüfen

6. Wenn Sie mit den Eingaben fertig sind, sehen Sie im Feld **Tatsächliche Tourkosten**, wie viel die Tour wirklich gekostet hat.

**Ergänzende Informationen**
> ⇨ Softwarereferenz, "Tour-Informationen" auf Seite I-209

---

## Touren fahren und überwachen

Dieser Themenblock befasst sich zum einen damit, welche Aktivitäten dem Fahrer auf der Tour zukommen und welche Möglichkeiten der Mitarbeiter in der Firma bezüglich des Trackings hat.

Dazu gehören folgende Lerneinheiten:
* "Vorbereitungen" auf Seite I-104
* "Touren fahren" auf Seite I-106
* "Touren überwachen" auf Seite I-114

### Überblick

**Lernziele**
*   Dokumente in die Cloud laden.
*   Die GDC-App für die Fahrer kennenlernen und verstehen.
*   Das Buchen über einen Browser kennenlernen und verstehen.
*   Die Möglichkeiten der Lieferüberwachung (im Folgenden auch Tracking genannt) kennenlernen und verstehen.

**Nutzen**
*   Über die Trackingfunktion werden die Mitarbeiter in der Firma ständig über den Stand der Route informiert. Auf viele Situationen kann direkt reagiert werden. So kann z. B. eine zu Bruch gegangene Scheibe nachproduziert werden, während der LKW noch auf der Tour ist.

**Definition**

| Begriff | Erklärung |
| :--- | :--- |
| **GDC-App** | App für Android, die über den Google Playstore kostenlos heruntergeladen werden kann. |

**Merke**

| Thema | Hinweis |
| :--- | :--- |
| **Android** | Für Android Systeme gibt es die im Google Playstore die App GDC. |
| **und Andere** | Die Benutzer von Nicht-Android-Systemen können sich über den Browser direkt einloggen. |
| **Aktualisieren** | Vergessen Sie nicht, im Routen Administrator von Zeit zu Zeit die Schaltfläche [Aktualisieren] zu drücken, damit Ihre Daten abgeglichen werden. |

### Vorbereitungen

Damit die App und das GPS-Tracking korrekt funktionieren, sind folgende Vorarbeiten nötig:

**Entsprechender Tourstatus**

Damit die Tourdaten an die Cloud gegeben werden können, müssen Sie den Tourstatus auf **Freigegeben** setzen.

Dazu markieren Sie die entsprechende Tour im Bereich **Ergebnis**, klicken auf die Symbol-Schaltfläche **Tour bearbeiten** und wählen aus der Kombobox **Tour-Status** den Status **Freigegeben**.

Eine detaillierte Erläuterung zum Ändern des Tourstatus finden Sie unter:
⇨ "So ändern Sie den Status einer Tour" auf Seite I-99

> **Tourstatus Freigegeben**
> Sobald Sie den Tourstatus auf **freigegeben** setzen, ist es nicht mehr möglich, die Aufträge noch einmal aus A+W Business an OTR zu übergeben. Sollte dies notwendig sein, so müssen Sie zunächst den Nummernverwalter kopieren um neue Auftragsnummern zu bekommen. Achten Sie dabei darauf, dass der neue Auftragsstatus im korrekten Statusbereich (meist 01 bis 800) liegt.

**Dokumente in die Cloud laden**

Möchten Sie dem Fahrer die Dokumente in digitaler Form zu Verfügung stellen, müssen Sie diese ebenfalls in die Cloud laden.

*Beispielhafte Ansicht: Dialog "Dateien anhängen"*
