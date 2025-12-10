---
title: "DE_AWBusiness_LogisticOptimizer_2_4"
source: "DE_AWBusiness_LogisticOptimizer_2_4.pdf"
tags: ["logistics", "tour planning", "A+W Business", "software reference", "user manual", "Kundenverwaltung", "Fahrzeugmanagement", "Routenoptimierung", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for the A+W Business Logistic Optimizer. It provides detailed explanations of the administration and planning modules, covering customer data management, vehicle and driver setup, reporting, packaging materials, and data import functionalities."
long_description: "This is a comprehensive software reference guide for the A+W Business Logistic Optimizer, a tool designed for planning and optimizing delivery tours. The manual is divided into two main sections: Administration and Planning. The Administration section details how to manage core data, including customers (Kunden), departments (Abteilungen), vehicles (Fahrzeuge), drivers (Fahrer), reports (Reports), packaging materials (Packmittel), and data import processes (Datenimport). Each subsection explains the corresponding dialog windows, fields, and functionalities, complete with screenshots and field-by-field descriptions. The Planning section focuses on the operational aspects of tour management. It covers how to create, copy, load, and edit tours. It provides in-depth guidance on setting up new tours by defining general information, assigning vehicles and drivers, and configuring various optimization parameters like tour mode (fastest, shortest, most economical), road type preferences (tolls, highways, tunnels), and optimization factors (distance, weight, schedule). The manual also explains how to manage and edit destinations within a tour, view associated documents and items, and analyze tour costs. This guide serves as an essential resource for administrators and planners using the A+W Business Logistic Optimizer to ensure efficient and effective logistics operations."
---

# Softwarereferenz

---
## Kunden
**Administration > Kunden**

*Abb. 1-46 Kunden*

| Kunden-ID | Name | Adresse | Telefon |
| :--- | :--- | :--- | :--- |
| 201 | CLIENTE 201 FRANCE | 50, RUE SAINT-ROCH, 80000 AMIENS, FRANCIA | 0 |
| 202 | CLIENTE 202 FRANCE | 78R, RUE DE WAGRAM, 72000 LE MANS, FRANCIA | 0 |
| 203 | CLIENTE 203 FRANCE | 9, RUE MATHILDE ALANIC, 49100 ANGERS, FRANCIA | 0 |
| 204 | CLIENTE 204 FRANCE | 70, AVENUE ANDRÉ MAGINOT, 37100 TOURS, FRANCE | 0 |
| 1060 | WOLF GLASBAU | SPORTPARKSTRABE 24, 35578 WETZLAR, GERMANY | 0 |
| 1080 | CICEK GLASBAU | MERIANSTRABE 23, 35578 WETZLAR, DEUTSCHLAND | 0 |
| 1110 | HEYD GLASBAU | KONRAD-ADENAUER-STRABE 15, 35440 LINDEN, GERMANY | 0 |
| 1090 | PLA GLASBAU | KONRAD-ADENAUER-STRABE 15, 35440 LINDEN, GERMANY | 0 |
| 1020 | MAIER FENSTERBAU | AM GRABEN 10, 35466 RABENAU, GERMANY | 0 |
| 1130 | SCHEINKER GLASBAU | KONRAD-ADENAUER-STRABE 15, 35440 LINDEN, GERMANY | 0 |
| 1070 | BECKER GLASBAU | HAUPTSTRABE 99, 35745 HERBORN, DEUTSCHLAND | 0 |
| 1010 | GLASBAU MUELLER | HAUPTSTRABE 5, 50996 KÖLN, DEUTSCHLAND | 0 |
| 1030 | WOLF & SOHN GLASHANDEL G... | STEINWEG 1, 36124 EICHENZELL, DEUTSCHLAND | 0 |
| 1000 | JOHN & PARTNER | AM BAHNDAMM 5, 35041 MARBURG, DEUTSCHLAND | 0 |
| 1120 | LÜHMANN GLASBAU | KONRAD-ADENAUER-STRABE 15, 35440 LINDEN, DEUTSCHL... | 0 |
| 99999 | SCHMIDT GLAS | STEINSTRABE 11, 30453 HANNOVER, DEUTSCHLAND | 0 |

In diesem Dialog können Sie grundlegende Kundendaten hinzufügen, ändern oder löschen. Kunden werden automatisch gespeichert, wenn in den Parametern der Eintrag USE_CUSTOMERS_OTR den Wert Ja hat.

### Erläuterung der Felder im Register Haupt

**Kunden-Nr.** In diesem Feld wird Ihnen die Kundennummer angezeigt.

**Name** In diesem Feld wird Ihnen der Kundenname angezeigt.

**Telefon** Hier wird Ihnen die Telefonnummer angezeigt.

**Adresse** In diesem Feld wird Ihnen die Adresse des Kunden angezeigt.

**Priorität** Diese Checkbox ist aktiv, wenn es sich bei der Adresse um eine Prioritätsadresse handelt.

**Breitengrad** In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.

**Längengrad** In diesem Feld finden Sie den Längengrad der Firmen-Adresse.

**Zeit** In diesem Feld können Sie die Zeit in Minuten hinterlegen, die dem Fahrer zum Abladen und eventuellen neu Laden (Leergestelle) zur Verfügung steht.

**Uhr** Wenn Sie auf diese Schaltfläche klicken, öffnet sich ein Dialog, in dem Sie den Zeitbereich eingeben können, in dem der Fahrer beim Kunden sein soll. Geben Sie einen solchen Bereich an, wird Ihnen dieser im Feld Zeitbereich angezeigt.

**Ansprechpartner** In diesem Feld können Sie einen Ansprechpartner beim Kunden hinterlegen.

**E-Mail-Adresse Kontakt** In diesem Feld können Sie die E-Mail-Adresse des Kontaktes hinterlegen.

### Erläuterung der Felder im Register Informationen

**Name 2** In diesem Feld können Sie einen weiteren Namen hinterlegen.

**Name 3** In diesem Feld können Sie noch einen weiteren Namen hinterlegen.

**Telefon 2** In diesem Feld können Sie eine weitere Telefonnummer hinterlegen.

**Fax** In diesem Feld können Sie eine Faxnummer eingeben.

**Web** Wenn der Kunde über eine eigene Internetseite verfügt, können Sie hier die entsprechende Adresse hinterlegen.

**Beschreibung** In diesem Feld können Sie eine weitere Beschreibung zu dem Kunden hinterlegen.

> **Ergänzende Informationen**
> ⇨ Tutorial, “Kunden" auf Seite 1-40
> ⇨ Tutorial, "Die Kunden verwalten" auf Seite 1-41

## Abteilungen
**Administration > Abteilungen**

*Abb. 1-47 Abteilungen*

| Abteilung | Name | Beschreibung |
| :--- | :--- | :--- |
| EXPEDITION | DELIVERY AND EXPEDITION DEPARTMENT | |
| SUPPORT | ASSISTANT SUPPORT ASSISTANT SERVICE DEPARTMENT | |
| COMERCIAL | COMERCIAL AND MARKETING DEPARTMENT | |

In diesem Dialog können Sie Abteilungen hinzufügen, ändern oder löschen. Dies dient später einmal statischen Auswertungen.

### Erläuterung der Felder

**Abteilung** In diesem Feld geben Sie die Abteilung ein, z. B. Versand.

**Name** In diesem Feld geben Sie den Namen der Abteilung ein, z. B. Versand Nord.

**Beschreibung** In diesem Feld können Sie eine weitere Beschreibung hinterlegen.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Abteilungen" auf Seite 1-43
> ⇨ Tutorial, "Die Abteilungen verwalten" auf Seite 1-43

## Fahrzeuge
**Administration > Fahrzeuge**

*Abb. I-48 Fahrzeuge*

Der Dialog ist in zwei Bereiche unterteilt. Der obere Bereich liefert Ihnen eine Übersicht zu allen angelegten Fahrzeugen. Klicken Sie im oberen Bereich ein Fahrzeug an, zeigt Ihnen der untere Bereich Detail-Informationen zu dem ausgewählten Fahrzeug.

| Nummernschild | Marke | Modell | Maximale Beladung | Fahrer ID | Touren | Reihenfolge |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1234-A | Mercedes | Sprinter | 7.500,00 | DEF-1 | 0 | 1 |
| 1235-B | Mercedes | Sprinter | 7.500,00 | DEF-2 | 0 | 1 |
| 1236-C | Mercedes | Sprinter | 7.500,00 | DEF-3 | 0 | 1 |
| 1237-D | Mercedes | Sprinter | 7.500,00 | DEF-4 | 0 | 1 |
| 1238-E | Mercedes | Atego | 15.000,00 | DEF-5 | 0 | 1 |
| 1239-F | Mercedes | Atego | 15.000,00 | DEF-6 | 0 | 1 |
| 1240-G | Mercedes | Atego | 15.000,00 | DEF-7 | 0 | 1 |
| 1241-H | Mercedes | Actros | 25.000,00 | DEF-8 | 0 | 1 |
| 1242-1 | Mercedes | Actros | 25.000,00 | DEF-9 | 0 | 1 |

In diesem Dialog befinden sich alle angelegten Fahrzeuge, mit denen OTR arbeiten kann. Ein Fahrzeug kann ein LKW, ein Anhänger oder auch ein größerer Transporter sein.

### Erläuterung der Felder im Bereich Detail

**Nummernschild** In diesem Feld geben Sie das Nummernschild des Fahrzeugs an, z. B. HH-XY-123. Wenn Sie das Nummernschild nicht kennen, entnehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Marke** In diesem Feld geben Sie die Fahrzeugmarke ein, z. B. Iveco. Wenn Sie die Fahrzeugmarke nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Modell** In diesem Feld geben Sie das Fahrzeugmodell ein, z. B. Daily 50 C 14. Wenn Sie das Fahrzeugmodell nicht kennen, entnehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Fahrgestell-Nummer** In diesem Feld geben Sie die Fahrgestell-Nummer des Fahrzeugs an, z. B. WWW1256425DERE. Wenn Sie die Fahrgestell-Nummer nicht kennen, entnehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Kaufdatum** In diesem Feld geben Sie ein, wann Sie das Fahrzeug gekauft haben. So haben Sie einen Überblick, wie viele Kilometer mit dem Fahrzeug gefahren wurden.

**Nächste Wartung** In diesem Feld haben Sie die Möglichkeit, den nächsten Wartungstermin für das entsprechende Fahrzeug zu hinterlegen. In dem Parameter (Das Programm zeigt die Anzahl der Tage an, nach deren Ablauf die nächste Wartung fällig ist), können Sie die gewünschte Anzahl an Tagen einstellen.

**Abteilung** In diesem Feld können Sie dem Fahrzeug eine Abteilung zuordnen. Der Wert kommt aus Administration > Abteilung.

**Maximale Breite** In diesem Feld geben Sie die maximale Breite des Fahrzeugs in Metern ein, z. B. 2,85. Wenn Sie die Breite nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Maximale Höhe** In diesem Feld geben Sie die maximale Höhe des Fahrzeugs in Metern ein, z. B. 3,85. Wenn Sie die Höhe nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Maximale Länge** In diesem Feld geben Sie die maximale Länge des Fahrzeugs in Metern ein, z. B. 7,6. Wenn Sie die Länge nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Maximale Beladung** In diesem Feld geben Sie die maximale Beladung des Fahrzeugs in kg ein, z. B. 25650. Wenn Sie die Breite nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief). Bitte beachten Sie, dass auch die Transportgestelle zur Beladung dazu gehören.

**Leergewicht** In diesem Feld geben Sie das Leergewicht des Fahrzeugs in Kilogramm ein, z. B. 7800. Wenn Sie das Leergewicht nicht kennen, entnehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Verbrauch** In diesem Feld geben Sie den durchschnittlichen Kraftstoff-Verbrauch des Fahrzeugs in Litern auf 100 km ein, z. B. 18,5. Das bedeutet, dass das Fahrzeug auf 100 km 18,5 Liter Kraftstoff verbraucht. Wenn Sie hier keinen Wert eingeben, wird der Standard-Wert aus den Parametern zur Kalkulation der Tour-Kosten herangezogen.

**Kosten** In diesem Feld geben Sie die durchschnittlichen Kosten für einen Liter Kraftstoff ein, z. B. 1,43. Die entsprechende Währungseinheit können Sie in den Parametern hinterlegen. Wenn Sie hier keinen Wert eingeben, wird der Standard-Wert aus den Parametern zur Kalkulation der Tour-Kosten herangezogen.

**Fortbewegungstyp** Wählen Sie aus der Kombobox das entsprechende Fahrzeug aus, z. B. LKW, Auto, etc.

**Von/bis** Zeitfenster, in dem das Fahrzeug zur Verfügung steht. Sollte die Start- oder Endzeit der Tour außerhalb des Fensters liegen, erscheint in der Spalte Status in den Planungsanzeigen ein Warnsymbol.

**Fahrer ID** In diesem Feld wird Ihnen die Fahrer ID angezeigt. Der Wert kommt aus Konfiguration > Fahrer > Fahrer ID.

**Vorname** In diesem Feld wird Ihnen der Vorname des Fahrers angezeigt. Der Wert kommt aus Konfiguration > Fahrer > Vorname.

**Nachname** In diesem Feld wird Ihnen der Nachname des Fahrers angezeigt. Der Wert kommt aus Konfiguration > Fahrer > Nachname.

**Fahrer** Wenn Sie diese Symbol-Schaltfläche betätigen, öffnet sich der Dialog Fahrer. Aus diesem können Sie den entsprechenden Fahrer auswählen.

**Touren** Die in diesem Feld aufgeführten Tournummern werden durch AW-Business übergeben und dienen dazu, LKWs bestimmten Tournummern zuzuordnen.

**Reihenfolge** Ist für zwei oder mehrere LKWs die gleiche Tournummer erlaubt, dann können Sie über dieses Feld die Reihenfolge der LKWs bestimmen. Das Feld wird nur ausgewertet, wenn in den Parametern der Eintrag ROUTE_ORIGIN den Wert Ja hat.

**mit Anhänger** Über diese Checkbox steuern Sie, ob das Fahrzeug einen Anhänger mitführen kann.
- Das Fahrzeug kann keinen Anhänger mit sich führen.
- Das Fahrzeug kann mit Anhänger fahren.

**Fahrzeug verfügbar** Über diese Checkbox steuern Sie, ob das Fahrzeug generell zur Verfügung steht.
- Das Fahrzeug steht nicht generell zur Verfügung.
- Das Fahrzeug ist verfügbar und kann verplant werden.

**GPS-Typ** Wählen Sie aus der Kombobox den entsprechenden GPS-Typ aus, z. B. GDC (eigene Lieferapp), Atlantis (spanischer LKW-GPS-Systemanbieter) oder SkyeEye (US LKW-GPS-Systemanbieter).

**Kennung** Tragen Sie in diesem Feld die Kennung des entsprechenden GPS-Systems ein.

**Beschreibung** Hier haben Sie die Möglichkeit, eine Beschreibung zum Fahrzeug zu hinterlegen.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Fahrzeuge" auf Seite 1-45
> ⇨ Tutorial, "Die Fahrzeuge verwalten" auf Seite 1-46

## Fahrer
**Administration > Fahrer**

*Abb. 1-49 Fahrer*

| Fahrer ID | Name | Nachname | Nachname 2 | Telefon | E-Mail |
| :--- | :--- | :--- | :--- | :--- | :--- |
| DEF-1 | DEFAULT DRIVER | 1 | | | |
| DEF-2 | DEFAULT DRIVER | 2 | | | |
| DEF-3 | DEFAULT DRIVER | 3 | | | |
| DEF-4 | DEFAULT DRIVER | 4 | | | |
| DEF-5 | DEFAULT DRIVER | 5 | | | |
| DEF-6 | DEFAULT DRIVER | 6 | | | |
| DEF-7 | DEFAULT DRIVER | 7 | | | |
| DEF-8 | DEFAULT DRIVER | 8 | | | |
| DEF-9 | DEFAULT DRIVER | 9 | | | |
| DEF-10 | DEFAULT DRIVER | 10 | | | |
| DEF-11 | DEFAULT DRIVER | 11 | | | |

In diesem Dialog befinden sich alle angelegten Fahrer, die Sie im Zugriff haben. Es kann sich dabei sowohl um fest angestellte Mitarbeiter als auch um Personen handeln, die temporär für Sie arbeiten.

### Erläuterung der Felder im Bereich Detail

**Fahrer-ID** In diesem Feld geben Sie ein Kürzel für den Fahrer ein.

**Name** In diesem Feld geben Sie den Vornamen des Fahrers ein.

**Nachname** In diesem Feld geben Sie den Nachnamen des Fahrers ein.

**Nachname 2** In diesem Feld haben Sie die Möglichkeit, einen zweiten Nachnamen für den Fahrer zu hinterlegen.

**Steuer-ID** In diesem Feld geben Sie den Steuer-ID des Fahrers ein. Die ID können Sie bei dem Fahrer erfragen.

**E-Mail** In diesem Feld geben Sie die E-Mail-Adresse des Fahrers ein.

**Kosten** In diesem Feld haben Sie die Möglichkeit, für die unterschiedlichen Fahrer Kosten zu hinterlegen. Dieses Feld steht in Zusammenhang mit den dahinter liegenden Radiotasten **Nach Zeit** und **Nach Entfernung**. Der Wert, den Sie hier eintragen, bezieht sich darauf, welche Radiotaste Sie aktiviert haben.

**Nach Zeit** Über diese Radiotaste steuern Sie, ob sich die Kosten, die Sie im Feld **Kosten pro Fahrer** eingetragen haben auf die Tour-Zeit beziehen.

**Nach Entfernung** Über diese Radiotaste steuern Sie, ob sich die Kosten, die Sie im Feld **Kosten pro Fahrer** eingetragen haben auf die Tour-Entfernung beziehen.

**Adresse** In diesem Feld haben Sie die Möglichkeit, die Adresse des Fahrers zu hinterlegen.

**Telefon** In diesem Feld haben Sie die Möglichkeit, die Telefon-Nummer des Fahrers zu hinterlegen, z. B. Festnetz.

**Telefon 2** In diesem Feld haben Sie die Möglichkeit, die Telefon-Nummer des Fahrers zu hinterlegen, z. B. Mobil.

**Ansprechpartner** In diesem Feld geben Sie den Namen des Ansprechpartners ein, falls der Fahrer nicht in Ihrem Hause angestellt ist, sondern evtl. bei einer anderen Firma.

**Kontakt-Adresse** In diesem Feld geben Sie die Kontakt-Adresse ein, falls der Fahrer nicht in Ihrem Hause angestellt ist, sondern evtl. bei einer anderen Firma.

**Telefon Kontakt** In diesem Feld geben Sie die Kontakt-Telefonnummer ein, falls der Fahrer nicht in Ihrem Hause angestellt ist, sondern evtl. bei einer anderen Firma.

**Beschreibung** In diesem Feld haben Sie die Möglichkeit, ein Beschreibung zu dem Fahrer oder dem Kontakt zu hinterlegen.

**E-Mail-Adresse-Kontakt** In diesem Feld geben Sie die E-Mail-Adresse des Kontaktes ein.

**Abteilung** In diesem Feld können Sie dem Fahrzeug eine Abteilung zuordnen. Der Wert kommt aus **Administration > Abteilung**.

**Firmen-Mitarbeiter** In diesem Feld legen Sie fest, ob es sich bei dem Fahrer um einen Mitarbeiter Ihres Unternehmens handelt oder nicht.
- Der Fahrer ist kein Mitarbeiter Ihrer Firma.
- Der Fahrer ist in Ihrem Unternehmen angestellt.

**Verfügbar** Über diese Checkbox steuern Sie, ob der Fahrer generell zur Verfügung steht.
- ☐ Der Fahrer steht nicht generell zur Verfügung.
- ☑ Der Fahrer ist verfügbar und kann verplant werden.

**Kennwort zurücksetzen** Über diese Checkbox wird das Kennwort, das beim Starten der GDC APP notwendig ist, zurückgesetzt.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Fahrer" auf Seite 1-49
> ⇨ Tutorial, "Die Fahrer verwalten" auf Seite 1-50

## Reports
**Administration > Reports**

*Abb. 1-50 Reports*

| Report-Name | Report-Pfad | Parameter |
| :--- | :--- | :--- |
| OTR\_ROUTE\_SMALL\_ML | C:\ProjectSVNDev\Src\Ort.App\bin\Debug\Router\Views\Result\OTR\_ROUTE\_SMALL... | RouteID |
| OTR\_ROUTE\_LONG | C:\Program Files (x86)\A+W ALFAK 2012\OTR\_APP\Router\Views\Result\OTR\_ROUT... | RouteID, RouteDrivers |

In diesem Dialog können Sie neue Reports anlegen oder Änderungen an bestehenden Reports vornehmen. Die Tabelle oben zeigt Ihnen alle bereits angelegten Reports.

### Erläuterung der Felder

**Report-Name** In diesem Feld geben Sie den Namen des Reports ein.

**Report-Pfad** In diesem Feld geben Sie ein, wo der Report gespeichert werden soll.

**Beschreibung** In diesem Feld können Sie eine weitere Beschreibung hinterlegen.

**Parameter** Über die Checkboxen wählen Sie aus, welche Parameter auf dem Report ausgegeben werden sollen.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Reports" auf Seite 1-52
> ⇨ Tutorial, "Die Reports verwalten" auf Seite 1-53

## Packmittel
**Administration > Packmittel-Typen**

*Abb. I-51 Packmittel*

| Packmittel ID | Packmittel-Typ | Abteilung |
| :--- | :--- | :--- |
| 1000100 | A-Bock | EXPEDITION |
| 1000105 | A-Bock | |
| 1000200 | L-Bock | |
| 1000300 | Box | |

In diesem Dialog können Sie neue Packmittel anlegen oder Änderungen an bestehenden Packmitteln vornehmen. Die Tabelle oben zeigt Ihnen alle bereits angelegten Packmittel.

> **Ladeflächenoptimierung**
> In der aktuellen Programmversion ist eine LKW-Ladeflächenoptimierung nicht umgesetzt. Bei den hier angelegten Packmitteln geht es um die Verbuchung der Ablade- / Aufladestation (im Sinne eines Packmittel-Trackings).

### Erläuterung der Felder

**Packmittel ID** In diesem Feld geben Sie die Packmittel ID ein.

**Packmittel-Typ** In diesem Feld geben Sie ein, um welches Packmittel es sich handelt, z. B. A-Bock, L-Bock, Kiste.

**Abteilung** In diesem Feld können Sie dem Packmittel eine Abteilung zuordnen. Der Wert kommt aus **Administration > Abteilung**. Über die dahinter liegende Symbol-Schaltfläche öffnen Sie den Dialog Abteilung auswählen.

**Breite** In diesem Feld können Sie die Breite des Packmittels in Metern eingeben, z. B. 2,50. Dieses Feld dient der zukünftigen Programmerweiterung (Ladeflächen-Optimierung).

**Höhe** In diesem Feld können Sie die Höhe des Packmittels in Metern eingeben, z. B. 1,98. Dieses Feld dient der zukünftigen Programmerweiterung (Ladeflächen-Optimierung).

**Länge** In diesem Feld können Sie die Länge des Packmittels in Metern eingeben, z. B. 0,95. Dieses Feld dient der zukünftigen Programmerweiterung (Ladeflächen-Optimierung).

**Leergewicht** In diesem Feld geben Sie das Leergewicht des Packmittels in Kilogramm ein, z. B. 250,00. Dieser Wert wird benötigt, um das zur Verfügung stehende Gesamtgewicht des Transportfahrzeug effizient zu nutzen.

**Kosten** In diesem Feld können Sie die Anschaffungskosten für das Packmittel eingeben, z. B. 300,00. Dieser Wert kann dann später zu statischen Auswertungen herangezogen werden.

**Keine Rückholung** Diese Checkbox können Sie aktivieren, wenn das Packmittel nicht zurückgeholt werden soll. Das kann z. B. bei Holzkisten der Fall sein. Diese verbleiben dann beim Kunden.

**Beschreibung** In diesem Feld können Sie eine weitere Beschreibung hinterlegen.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Packmittel-Typen" auf Seite 1-55

## Datenimport
**Administration > Datenimport**

*Abb. 1-52 Datenimport*

Über diesen Dialog können Sie Daten im CSV-Format importieren.

### Erläuterung der Felder

**Importieren CSV** Über die Kombobox wählen Sie aus, was Sie importieren möchten. Mögliche Werte sind:
- Kunden
- Abteilungen
- Fahrer
- Fahrzeuge

**Optionen** Wenn die erste Zeile ignoriert werden soll, aktivieren Sie bitte die Checkbox **Erste Zeile ignorieren**. In der Zeile darunter geben Sie an, welche Trennzeichen die Datei der zu importierenden Daten enthält, z. B. Semikolon, Komma, etc.

**Importiere CSV** Über diese Radiotasten steuern Sie, wie der Import abläuft. Ist diese Radiotaste aktiv, erfolgt der Import und die zu importierenden Daten (csv-Datei) bleiben erhalten. Aktivieren Sie die Radiotaste **Löschen und Import**, dann werden die zu importierenden Daten (csv-Datei) nach dem Import gelöscht.

**Import-Pfad** Wählen Sie hier aus, wo die zu importierende Datei liegt.

**Tabelle** Die darunter liegende Tabelle zeigt Ihnen, welche Felder importiert werden.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Datenimport" auf Seite 1-58

## Planung
**Menü Planung**

In diesem Bereich werden alle Daten eingerichtet und gepflegt, die zur Planung der Tour benötigt werden.

Der Bereich beinhaltet:
- **Tour kopieren:** Über diesen Dialog können Sie eine gespeicherte Tour kopieren.
    - ⇨ "Eine gespeicherte Tour kopieren" auf Seite I-165
- **Gespeicherte Touren laden:** Über diesen Dialog können Sie eine gespeicherte Tour laden.
    - ⇨ "Eine gespeicherte Tour laden" auf Seite 1-168
- **Neue Tour:** In diesem Dialog erstellen Sie eine neue Tour.
    - ⇨ "Eine neue Tour zusammenstellen - Allgemein" auf Seite I-170
    - ⇨ "Eine neue Tour zusammenstellen - Fahrzeuge" auf Seite 1-174
    - ⇨ "Eine neue Tour zusammenstellen - Parameter" auf Seite 1-180
    - ⇨ "Eine neue Tour zusammenstellen - Kosten" auf Seite 1-186
- **Tour bearbeiten:** Die Felder in diesem Dialog sind identisch mit den Feldern im Dialog **Eine neue Tour zusammenstellen**.
    - ⇨ "Eine neue Tour zusammenstellen - Allgemein" auf Seite I-170
- **Tour löschen:** Über diese Symbol-Schaltfläche können Sie die aktuelle Tour löschen.
- **Bereiche:** In diesem Dialog geben Sie die Anzahl der Bereiche ein.
    - ⇨ "Bereiche" auf Seite 1-189
- **Fahrzeuge:** In diesem Dialog weisen Sie einer Tour ein anderes Fahrzeug zu.
    - ⇨ "Fahrzeug wählen" auf Seite I-177
- **Neuer Bestimmungsort:** In diesem Dialog erfassen Sie einen neuen Bestimmungsort.
    - ⇨ "Eine neue Tour zusammenstellen - Allgemein" auf Seite I-170
- **Bestimmungsort bearbeiten:** In diesem Dialog können Sie einen bestehenden Bestimmungsort ändern.
    - ⇨ "Bestimmungsort bearbeiten" auf Seite I-191
- **Bestimmungsort löschen:** Über diese Symbol-Schaltfläche können Sie einen markierten Bestimmungsort löschen.
- **Positionen:** Hier sehen Sie die einzelnen Positionen der Tour.
    - ⇨ "Positionen anzeigen" auf Seite 1-196
- **Detailansicht:** Die Detailansicht liefert Ihnen einen Überblick zu den einzelnen Bestimmungsorten einer Tour.
    - "Detailansicht" auf Seite 1-202
- **Initialisieren:** Mittels dieser Symbol-Schaltfläche kehren Sie zur Ausgangssituation zurück. Haben Sie z. B. Datensätze gruppiert und möchten dies rückgängig machen, dann klicken Sie auf diese Schaltfläche.

### Eine gespeicherte Tour kopieren
**Planung > Gespeicherte Tour kopieren**

*Abb. 1-53 Gespeicherte Tour kopieren*

Dieser Dialog enthält alle im System gespeicherten Touren. Sie können Touren kopieren, um verschiedene Simulationen durchzuführen. Dazu markieren Sie die Tour, die Sie kopieren möchten und betätigen die Symbol-Schaltfläche [Tour].

#### Erläuterung der Felder im Bereich Touren

**TourStatus** In diesem Feld wird Ihnen der Tour-Status angezeigt.

**Liefertermin** Hier wird Ihnen der Liefertermin der ursprünglichen Tour angezeigt.

**Ursprüngliche Tour** Hier wird Ihnen die ursprüngliche Tour-Nummer angezeigt. Diese Tour-Nummer kommt von A+W Business.

**Tour-ID** Das Feld zeigt Ihnen die von A+W Business vergebene Tour-ID.

**Name der Tour** Hier wird Ihnen der Name der Tour angezeigt, den Sie seinerzeit vergeben haben.

**Entfernung** Hier sehen Sie, wie viele Kilometer die ursprüngliche Tour hatte.

**Tour-Zeit** Hier sehen Sie, wie lange die ursprüngliche Tour dauerte.

**Tour-Kosten** Hier sehen Sie, was die ursprüngliche Tour gekostet hat.

**Zugewiesenes Gewicht** Hier sehen Sie das Gewicht der ursprünglichen Tour.

**Nummernschild** Hier wird Ihnen das Nummernschild angezeigt. Anhand des Nummernschildes wissen Sie, welches Fahrzeug die ursprüngliche Tour gefahren hat.

**Marke und Modell** Hier wird Ihnen Marke und Modell des Fahrzeuges angezeigt, welches die ursprüngliche Tour gefahren hat.

**LKW-Ladung** In diesem Feld wird Ihnen das Gewicht der LKW-Ladung angezeigt.

**Abteilung** In diesem Feld sehen Sie, welche Abteilung die Tour veranlasst hat.

**Verkehr** In diesem Feld wird Ihnen angezeigt, ob die Route Verkehrsinformationen enthielt.

**Maut** In diesem Feld wird Ihnen angezeigt, ob die Route Mautgebühren enthielt.

#### Erläuterung der Felder im Bereich Bestimmungsorte

**Tour-Name** In diesem Feld wird Ihnen der Tour-Name angezeigt.

**Tour ID** In diesem Feld wird Ihnen die Tour ID angezeigt.

**Reihenfolge** Hier wird Ihnen angezeigt, in welcher Reihenfolge die einzelnen Bestimmungsorte angefahren wurden.

**Kunde** In diesem Feld wird Ihnen die Kundennummer angezeigt.

**Kunde** In diesem Feld wird Ihnen der Kundenname angezeigt.

**Adresse** In diesem Feld wird Ihnen die Kundenadresse angezeigt.

**Auftrag** In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

**Versandgewicht** In diesem Feld wird Ihnen das Versandgewicht pro Bestimmungsort angezeigt.

**Rückholgewicht** In diesem Feld wird Ihnen das Rückholgewicht pro Bestimmungsort angezeigt.

**Vor. Lieferung** In diesem Feld wird Ihnen das voraussichtliche Lieferdatum angezeigt.

**Priorität** In diesem Feld sehen Sie, ob es sich bei der Adresse um eine Prioritätsadresse handelt.

**Rechtzeitig** In diesem Feld sehen Sie, ob die Adresse pünktlich angefahren wurde.

**Typ** In diesem Feld sehen Sie, um welchen Typ (Anfangstyp, Mitteltyp, etc.) es sich bei dem Bestimmungsort handelte.

#### Erläuterung der Schaltfläche

**Filter** Nachdem Sie auf diese Schaltfläche geklickt haben, öffnet sich der Dialog Filter Routen.

**Kopieren** Nachdem Sie auf diese Schaltfläche geklickt haben, werden Sie gefragt, ob Sie die gespeicherte Tour der aktuellen Tour hinzufügen möchten.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Eine gespeicherte Tour kopieren" auf Seite 1-64
> ⇨ Tutorial, "So kopieren Sie eine gespeicherte Tour" auf Seite 1-71

### Eine gespeicherte Tour laden
**Planung > Gespeicherte Tour laden**

*Abb. I-54 Gespeicherte Tour-Liste*

Dieser Dialog enthält alle im System gespeicherten Touren. Touren werden automatisch gespeichert, wenn Sie im Ergebnis die Symbol-Schaltfläche [Beenden] betätigen. Sie können einer in Planung befindlichen Tour eine gespeicherte Tour dieser Liste hinzufügen. Dazu markieren Sie die Tour, die Sie hinzufügen möchten und betätigen die Symbol-Schaltfläche [OK]. Sie können auch einzelne Touren der Liste löschen, indem Sie die Tour markieren und anschließend die Symbol-Schaltfläche [Tour löschen] anklicken.

#### Erläuterung der Felder
Die Felder dieses Dialoges sind identisch mit den Feldern des Dialoges **Eine gespeicherte Tour kopieren**.
⇨ "Eine gespeicherte Tour kopieren" auf Seite I-165

> **Ergänzende Informationen**
> ⇨ Tutorial, "Eine gespeicherte Tour laden" auf Seite 1-63
> ⇨ Tutorial, "So laden Sie eine gespeicherte Tour" auf Seite 1-70

### Bestimmungsorte importieren
**Planung > Bestimmungsorte importieren**

*Abb. 1-55 Bestimmungsorte importieren*

Über diesen Dialog können Sie Bestimmungsorte im CSV-Format importieren.

#### Erläuterung der Felder

**Optionen** Wenn die erste Zeile ignoriert werden soll, aktivieren Sie bitte die Checkbox **Erste Zeile ignorieren**. In der Zeile darunter geben Sie an, welche Trennzeichen die Datei der zu importierenden Daten enthält, z. B. Semikolon, Komma, etc.

**Import-Pfad** Wählen Sie hier aus, wo die zu importierende Datei liegt.

**Tabelle** Die darunter liegende Tabelle zeigt Ihnen, welche Felder importiert werden.

### Eine neue Tour zusammenstellen – Allgemein
**Planung > Tour hinzufügen**

*Abb. 1-56 Neue Tour, Register Allgemein*

In diesem Dialog nehmen Sie alle Einstellungen vor, die notwendig sind, um eine neue Tour zu planen. Er ist in drei Register unterteilt:
- Eine neue Tour zusammenstellen - Allgemein
- Eine neue Tour zusammenstellen - Fahrzeuge
- Eine neue Tour zusammenstellen – Parameter

#### Erläuterung der Felder im Bereich Information

**Liefertermin** Öffnen Sie die Kombobox und wählen Sie den gewünschten Liefertermin aus.

**Startzeit** Geben Sie in diesem Feld geben die Uhrzeit an, wann die Tour starten soll. Sie können die Zeit entweder über die Tastatur eingeben oder über die Pfeiltasten einstellen.

**Tour Status** Hier wird Ihnen der Status der Tour angezeigt. Der Wert kann an dieser Stelle nicht geändert werden. Erst, wenn die Optimierung durchlaufen wurde, können Sie im Bereich **Ergebnis** den Status ändern. Dann stehen folgende Werte zur Verfügung:
- **Grobgeplant:** Das ist der Status der Tour nach der Optimierung.
- **Feingeplant:** Dieser Status wird zur Zeit noch nicht ausgewertet.
- **Freigegeben:** Wenn Sie den Status in Freigegeben ändern, wird der Liefertermin, die Reihenfolge und die Tour an A+W Business zurückgemeldet. Sie können den Status nur einmal auf Freigegeben ändern.

**Tour-ID** Das Feld zeigt Ihnen die von OTR vergebene Tour-ID. Der Wert kann nicht geändert werden.

**Tour-Name** In diesem Feld geben Sie den Namen der Tour an. Der Eintrag ist vorbelegt mit dem Inhalt des Feldes lblGeneralRoute, dem heutigen Datum und der ursprünglichen Tour.

**Ursprüngliche Tour** Hier wird Ihnen die ursprüngliche Tour-Nummer angezeigt. Diese Tour-Nummer kommt von A+W Business. Da Sie eine neue Tour anlegen, ist das Feld mit 0 belegt. Der Wert kann nicht geändert werden.

**Tour-Name (Original)** In diesem Feld wird Ihnen der Original Tour-Name angezeigt. Dieser Name kommt von A+W Business und kann nicht geändert werden.

**Abteilung** In diesem Feld wird Ihnen die Abteilung angezeigt. Über die darunter liegenden Symbol-Schaltflächen können Sie die Vorbelegung ändern.

**Beschreibung** In diesem Feld können Sie eine detaillierte Beschreibung zur Tour hinterlegen.

#### Erläuterung der Felder im Bereich Ausgangspunkt

**Firmen-Name** In diesem Feld steht der Firmen-Name, bei dem die Tour anfängt. Der Wert kommt aus den Parametern (Initial_Companyname).

**Adresse** In diesem Feld steht die Firmen-Adresse, wo die Tour anfängt. Der Wert kommt aus den Parametern (Initial_Address). Straße, Ort und Land müssen durch Komma separiert sein. Bsp.: Hauptstr. 15, 35440 Mittelstadt, Deutschland.

**Breitengrad** In diesem Feld finden Sie den Breitengrad der Firmen-Adresse. Ist das Feld leer, können Sie den Standort durch Betätigen der Symbol-Schaltfläche [Geolokalisieren] ermitteln. Es öffnet sich der Dialog Einfache Geolokalisierung.

**Längengrad** In diesem Feld finden Sie den Längengrad der Firmen-Adresse. Ist das Feld leer, können Sie den Standort durch Betätigen der Symbol-Schaltfläche [Geolokalisieren] ermitteln. Es öffnet sich der Dialog Einfache Geolokalisierung.

**Ausgangspunkt verwenden** Über diese Checkbox steuern Sie, ob die Firmen-Adresse als Ausgangpunkt verwendet werden soll.
- Die Firmen-Adresse wird nicht als Ausgangspunkt verwendet
- Die Firmen-Adresse dient als Ausgangspunkt.

**Geolokalisieren** Wenn Sie die Symbol-Schaltfläche [Geolokalisieren] betätigen, öffnet sich der Dialog **Einfache Geolokalisierung**.

> **Ergänzende Informationen**
> ⇨ "Geolokalisieren" auf Seite 1-173
> ⇨ Tutorial, "So legen Sie eine neue Tour an" auf Seite 1-66

#### Geolokalisieren
**Planung > Neue Tour > Allgemein > [Geolokalisieren]**

*Abb. 1-57 Einfache Geolokalisierung*

Dieser Dialog dient zur Geolokalsierung Ihrer Adresse.

##### Erläuterung der Felder

**Adresse** In diesem Feld steht die Firmen-Adresse. Der Inhalt des Feldes kommt aus dem Feld **Adresse** im Dialog **Tour Allgemein**. Sie können die Adresse bei Bedarf ändern. Achten Sie darauf, dass die Straße, der Ort sowie das Land durch Komma getrennt werden.

**Breitengrad** In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.

**Längengrad** In diesem Feld finden Sie den Längengrad der Firmen-Adresse.

**Vorschläge** Wenn Sie die Symbol-Schaltfläche [Vorschläge] betätigen, öffnet sich eine kleine Tabelle, die entsprechende Vorschläge zu der Adresse enthält. Bei mehreren Einträgen, können Sie einen auswählen. Betätigen Sie die Schaltfläche [Akzeptieren], werden die Daten in den Dialog **Tour** übernommen.

> **Ergänzende Informationen**
> ⇨ "Eine neue Tour zusammenstellen - Allgemein" auf Seite I-170

### Eine neue Tour zusammenstellen – Fahrzeuge
**Planung > Neue Tour > Fahrzeuge**

*Abb. 1-58 Neue Tour, Register Fahrzeuge*

In diesem Register nehmen Sie alle Einstellungen vor, die das Fahrzeug betreffen, mit dem die Tour gefahren wird. Das Register ist in folgende Bereiche unterteilt:
- Fahrzeuge
- Fahrer

#### Erläuterung der Felder im Bereich Fahrzeuge

**Nummernschild** In diesem Feld geben Sie das Nummernschild des Fahrzeugs an, z. B. HH-XY-123. Wenn Sie das Nummernschild nicht kennen, entnehmen Sie dieses den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Marke und Modell** In diesem Feld geben Sie die Fahrzeugmarke und das Modell ein, z. B. Iveco. Wenn Sie die Angaben nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Kraftstoffkosten** In diesem Feld geben Sie die durchschnittlichen Kosten für einen Liter Kraftstoff ein, z. B. 1,43. Die entsprechende Währungseinheit können Sie in den Parametern hinterlegen.

**Kraftstoffverbrauch** In diesem Feld geben Sie den durchschnittlichen Kraftstoff-Verbrauch des Fahrzeugs in Litern ein, z. B. 18,5.

**Maximale Breite** In diesem Feld geben Sie die maximale Breite des Fahrzeugs in Metern ein, z. B. 2,85. Wenn Sie die Breite nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Maximale Höhe** In diesem Feld geben Sie die maximale Höhe des Fahrzeugs in Metern ein, z. B. 3,85. Wenn Sie die Höhe nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Maximale Länge** In diesem Feld geben Sie die maximale Länge des Fahrzeugs in Metern ein, z. B. 7,6. Wenn Sie die Länge nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**LKW Ladung** In diesem Feld geben Sie das zulässige Gesamtgewicht des Fahrzeugs an. Wenn Sie die Angaben nicht kennen, entnehmen Sie diese den Fahrzeugpapieren (Fahrzeugschein oder -brief).

**Fahrzeug-Typ** Wählen Sie aus der Kombobox den entsprechenden Fahrzeug-Typ aus. Mögliche Werte:
- LKW
- Auto

**LKW mit Anhänger** Über diese Checkbox steuern Sie, ob der LKW einen Anhänger hat. Das ist wichtig, um die korrekte Route zu berechnen. OTR berücksichtigt unter anderem harte Kurven.
- Der LKW oder das Auto haben keinen Anhänger.
- Der LKW oder das Auto haben einen Anhänger.

**Fahrzeug wählen** Wenn Sie diese Symbol-Schaltfläche [Fahrzeug wählen] betätigen, öffnet sich der Dialog **Fahrzeug wählen**.

#### Erläuterung der Felder im Bereich Fahrer

**Fahrer ID** In diesem Feld wird Ihnen die Fahrer ID angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Fahrer ID**.

**Vorname** In diesem Feld wird Ihnen der Vorname des Fahrers angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Vorname**.

**Nachname** In diesem Feld wird Ihnen der Nachname des Fahrers angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Nachname**.

**Kosten pro Fahrer** In diesem Feld werden Ihnen die Kosten pro Fahrer angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Kosten**.

**Nach Zeit** Ist diese Checkbox aktiv, beziehen sich die Kosten pro Fahrer auf die Tour-Zeit.

**Nach Entfernung** Ist diese Checkbox aktiv, beziehen sich die Kosten pro Fahrer auf die Entfernung.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Fahrzeuge" auf Seite 1-45
> ⇨ Tutorial, "Die Fahrzeuge verwalten" auf Seite 1-46

#### Fahrzeug wählen
**Planung > Neue Tour > Fahrzeuge > [Fahrzeug wählen]**

*Abb. 1-59 Fahrzeug wählen*

| Nummernschild | Marke | Modell | Maximale Beladung | Fahrer ID | Kraftstoffverbrauch | Kraftstoffkosten | Von | Bis | Abteilung |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1234-A | Mercedes | Sprinter | 7500,000 | DEF-1 | 5,000 | 1,220 | 08:00:00 | 12:00:00 | |
| 1235-B | Mercedes | Sprinter | 7500,000 | DEF-2 | 5,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1236-C | Mercedes | Sprinter | 7500,000 | DEF-3 | 5,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1237-D | Mercedes | Sprinter | 7500,000 | DEF-4 | 5,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1238-E | Mercedes | Atego | 15000,000 | DEF-5 | 10,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1239-F | Mercedes | Atego | 15000,000 | DEF-6 | 10,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1240-G | Mercedes | Atego | 15000,000 | DEF-7 | 10,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1241-H | Mercedes | Actros | 25000,000 | DEF-8 | 15,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1242-1 | Mercedes | Actros | 25000,000 | DEF-9 | 15,000 | 1,220 | 08:00:00 | 22:00:00 | |
| 1243-K | Mercedes | Actros | 25000,000 | DEF-10 | 15,000 | 1,220 | 08:00:00 | 22:00:00 | |

Aus diesem Dialog können Sie das Fahrzeug auswählen, mit dem die Tour gefahren werden soll. Die Daten kommen aus den Parametern.

##### Erläuterung der Felder

**Nummernschild** In diesem Feld wird Ihnen das Nummernschild des Fahrzeugs angezeigt.

**Marke** In diesem Feld wird Ihnen die Fahrzeug-Marke angezeigt.

**Modell** In diesem Feld wird Ihnen das Fahrzeug-Modell angezeigt.

**Maximale Beladung** In diesem Feld wird Ihnen die maximale Beladung des Fahrzeugs in kg angezeigt.

**Kraftstoffverbrauch** In diesem Feld wird Ihnen der durchschnittliche Kraftstoffverbrauch in Litern angezeigt.

**Kraftstoffkosten** In diesem Feld werden Ihnen die durchschnittlichen Kosten für einen Liter Kraftstoff angezeigt.

**Von/bis** Das Zeitfenster, in dem das Fahrzeug zur Verfügung steht.

**Abteilung** In diesem Feld wird Ihnen die Abteilung angezeigt.

> **Ergänzende Informationen**
> ⇨ "Fahrzeuge" auf Seite I-152
> ⇨ Tutorial, "Fahrzeuge" auf Seite 1-45

#### Fahrer hinzufügen
**Planung > Neue Tour > Fahrzeuge > [Fahrer hinzufügen]**

*Abb. 1-60 Fahrer Übersicht*

| Fahrer-ID | Vorname | Nachname | Adresse |
| :--- | :--- | :--- | :--- |
| PDK | PETER | DIRK | Carrer del ajuntament, 1, Sabadell, ... |
| MPR | PEPE | | noveno ve, 12, Barcelona |
| MANT | | | |

In diesem Dialog werden Ihnen alle gespeicherten Fahrer angezeigt.

##### Erläuterung der Felder

**Text finden** Dieses Feld dient dem Filtern der angezeigten Daten. Es steht in direktem Zusammenhang mit dem Feld **Filter-Typ**. Wählen Sie zunächst den Filter-Typ (Fahrer ID, Vorname, Nachname oder Adresse) aus und geben Sie dann im Feld **Text finden** die Angaben ein, nach denen gefiltert werden soll.

**Filter-Typ** Über diese Kombobox steuern Sie, nach welchen Einträgen gefiltert werden soll, Fahrer ID, Vorname, Nachname oder Adresse. Anschließend geben Sie im Feld **Text finden** die Angaben ein, nach denen gefiltert werden soll.

**Filtern** Nachdem Sie die entsprechenden Kriterien in den Feldern **Text finden** und **Filter-Typ** eingegeben haben, betätigen Sie diese Symbol-Schaltfläche. Danach wird die Liste der Einträge entsprechend aktualisiert.

**Filter löschen** Um die eingegebenen Filter-Kriterien zu löschen, betätigen Sie diese Symbol-Schaltfläche. Danach wird die Liste der Einträge entsprechend aktualisiert und es werden wieder alle Einträge angezeigt.

**Fahrer ID** In diesem Feld wird Ihnen die Fahrer ID angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Fahrer ID**.

**Vorname** In diesem Feld wird Ihnen der Vorname des Fahrers angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Vorname**.

**Nachname** In diesem Feld wird Ihnen der Nachname des Fahrers angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Nachname**.

**Adresse** In diesem Feld wird Ihnen die Adresse des Kunden angezeigt. Der Wert kommt aus **Konfiguration > Fahrer > Adresse**.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Die Fahrer verwalten" auf Seite 1-50

### Eine neue Tour zusammenstellen – Parameter
**Planung > Neue Tour > Parameter**

*Abb. I-61 Neue Tour, Register Parameter*

In diesem Register legen Sie die Kriterien fest, anhand derer die Tour gefahren wird.

#### Erläuterung der Felder im Bereich Parameter

**Tour-Modus** Hier stellen Sie das gewünschte Merkmal der Route ein. Mögliche Werte sind:
- **Schnellste:** Mit dieser Einstellung wird die schnellste Verbindung zwischen den Wegpunkten ermittelt. Die Optimierung basiert auf der Fahrtzeit.
- **Kürzeste:** Mit dieser Einstellung wird die kürzeste Verbindung zwischen den Wegpunkten ermittelt. Die Optimierung basiert auf der Entfernung.
- **Wirtschaftlichste:** Mit dieser Einstellung wird die wirtschaftlichste Route ermittelt. Die Optimierung basiert auf dem Benzinverbrauch.
Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern und kann dort geändert werden (Parameter: Nokia_Mode).

**Multi-Tour** Diese Checkbox ist für Touren, die Sie manuell erstellen, nicht aktiv.

**Liefertermin** Diese Checkbox ist für Touren, die Sie manuell erstellen, nicht aktiv.

**Start der Tour** Diese Checkbox ist für Touren, die Sie manuell erstellen, nicht aktiv.

**Verkehr** Ist diese Checkbox nicht aktiv, wird die Verkehrslage nicht ermittelt. Sie können diese Option später im Dialog **Optimierung** über die Schaltfläche **Verkehr** aufrufen.

**Optimierung überspringen** Ist diese Checkbox aktiv, wird die Optimierung zunächst übersprungen. Sie können diese Option später im Dialog **Optimierung** über die Schaltfläche **Route optimieren** aufrufen.

**Maut-Modus** Mit diesem Feld steuern Sie, ob Mautstraßen für die Streckenführung erlaubt sind. Mögliche Werte sind:
- **Mautstraßen gänzlich vermeiden:** Die Optimierung garantiert, dass Verkehrsverbindungen, die Mautstraßen enthalten, gänzlich ausgeschlossen werden. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
- **Mautstraßen teilweise vermeiden:** Die Optimierung berücksichtigt keine Verkehrverbindungen, die Mautstraßen enthalten. Wenn durch diese Einschränkung keine Route gefunden werden kann, wird die Bedingung gelockert.
- **Strafe für Mautstraßen:** Die Optimierung belegt Verbindungen, die Mautstraßen enthalten, mit Strafen.
- **Normal:** Die Optimierung behält die Reihenfolge der Verbindungen, die Mautstraßen enthalten.
- **Bevorzugte:** Die Optimierung bevorzugt Verkehrsverbindungen, die Mautstraßen enthalten.
Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern und kann dort geändert werden (Parameter: Nokia_Avoid_Tolls).

**Autobahn-Modus** Mit diesem Feld steuern Sie, ob Autobahnen für die Streckenführung erlaubt sind. Mögliche Werte sind:
- **Autobahnen gänzlich vermeiden:** Die Optimierung garantiert, dass Verkehrsverbindungen, die Autobahnen enthalten, gänzlich ausgeschlossen werden. Dies ist z. B. bei HOV Lanes in USA und Kanada der Fall. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
- **Autobahnen teilweise vermeiden:** Die Optimierung berücksichtigt keine Verkehrverbindungen, die Autobahnen enthalten. Wenn durch diese Einschränkung keine Route gefunden werden kann, wird die Bedingung gelockert.
- **Strafe für Autobahnen:** Die Optimierung belegt Verbindungen, die Autobahnen enthalten, mit Strafen.
- **Normal:** Die Optimierung behält die Reihenfolge der Verbindungen, die Autobahnen enthalten.
- **Bevorzugte:** Die Optimierung bevorzugt Verkehrsverbindungen, die Autobahnen enthalten.
Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern und kann dort geändert werden (Parameter: Nokia_Avoid_Motorways).

**Tunnel-Modus** Mit diesem Feld steuern Sie, ob Straßen mit Tunnel für die Streckenführung erlaubt sind. Mögliche Werte sind:
- **Tunnel gänzlich vermeiden:** Die Optimierung garantiert, dass Verkehrsverbindungen, die Tunnel enthalten, gänzlich ausgeschlossen werden. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
- **Tunnel teilweise vermeiden:** Die Optimierung berücksichtigt keine Verkehrverbindungen, die Tunnel enthalten. Wenn durch diese Einschränkung keine Route gefunden werden kann, wird die Bedingung gelockert.
- **Strafe für Tunnel:** Die Optimierung belegt Verbindungen, die Tunnel enthalten, mit Strafen.
- **Normal:** Die Optimierung behält die Reihenfolge der Verbindungen, die Tunnel enthalten.
- **Bevorzugte:** Die Optimierung bevorzugt Verkehrsverbindungen, die Tunnel enthalten.
Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern und kann dort geändert werden (Parameter: Nokia_Avoid_Tunnels).

**Fähren-Modus** Mit diesem Feld steuern Sie, ob Fähren für die Streckenführung erlaubt sind. Mögliche Werte sind:
- **Fähren gänzlich vermeiden:** Die Optimierung garantiert, dass Verkehrsverbindungen, die Fähren enthalten, gänzlich ausgeschlossen werden. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
- **Fähren teilweise vermeiden:** Die Optimierung berücksichtigt keine Verkehrverbindungen, die Fähren enthalten. Wenn durch diese Einschränkung keine Route gefunden werden kann, wird die Bedingung gelockert.
- **Strafe für Fähren:** Die Optimierung belegt Verbindungen, die Fähren enthalten, mit Strafen.
- **Normal:** Die Optimierung behält die Reihenfolge der Verbindungen, die Fähren enthalten.
- **Bevorzugte:** Die Optimierung bevorzugt Verkehrsverbindungen, die Fähren enthalten.
Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern und kann dort geändert werden (Parameter: Nokia_Avoid_Ferrys).

**Zug-Modus** Mit diesem Feld steuern Sie, ob Züge für die Streckenführung erlaubt sind. Mögliche Werte sind:
- **Züge gänzlich vermeiden:** Die Optimierung garantiert, dass Verkehrsverbindungen, die Züge enthalten, gänzlich ausgeschlossen werden. Wenn die Bedingung nicht erfüllt werden kann, wird keine Route ermittelt.
- **Züge teilweise vermeiden:** Die Optimierung berücksichtigt keine Verkehrverbindungen, die Züge enthalten. Wenn durch diese Einschränkung keine Route gefunden werden kann, wird die Bedingung gelockert.
- **Strafe für Züge:** Die Optimierung belegt Verbindungen, die Züge enthalten, mit Strafen.
- **Normal:** Die Optimierung behält die Reihenfolge der Verbindungen, die Züge enthalten.
- **Bevorzugte:** Die Optimierung bevorzugt Verkehrsverbindungen, die Züge enthalten.
Der Standardwert, mit dem das Feld vorbelegt ist, kommt aus den Parametern und kann dort geändert werden (Parameter: Nokia_Avoid_Trains).

#### Erläuterung der Felder im Bereich Optimierung

**Entfernungs-Faktor** In diesem Bereich wird Ihnen der Entfernungs-Faktor angezeigt.

**Gewichts-Faktor** In diesem Bereich wird Ihnen der Gewichts-Faktor angezeigt.

**Termin-Faktor** In diesem Bereich wird Ihnen der Termin-Faktor angezeigt.

**Prioritäts-Faktor** In diesem Bereich wird Ihnen der Prioritäts-Faktor angezeigt.

**Zeit-Faktor** In diesem Bereich wird Ihnen der Zeit-Faktor angezeigt.

**Tour-Faktoren** Wenn Sie die Symbol-Schaltfläche [Tour-Faktoren] betätigen, öffnet sich der Dialog **Tour-Faktoren**. Hier können Sie die einzelnen Faktoren ändern.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Mit Touren arbeiten" auf Seite 1-66
> ⇨ Tutorial, "So legen Sie eine neue Tour an" auf Seite 1-66

#### Tour-Faktoren
**Planung > Neue Tour > Parameter > [Tour-Faktoren]**

*Abb. I-62 Tour-Faktoren*

In diesem Dialog legen Sie die Einflussgrößen der einzelnen Merkmale fest. Bitte beachten Sie, dass die einzelnen Prozentzahlen addiert 100% ergeben müssen. Um die Werte zu verändern, klicken Sie den Schieber des jeweiligen Wertes an und bewegen ihn in die gewünschte Richtung. Über die Symbol-Schaltfläche [Sperren] können Sie einzelne Werte sperren, deren Wert dann nicht mehr verändert wird.

Es stehen folgende Einflussgrößen zur Verfügung:
- **Entfernungs-Faktor:** Der Entfernungs-Faktor basiert auf der Länge der Tour. Er sucht die kürzeste Strecke.
- **Gewichts-Faktor:** Der Gewichts-Faktor bewertet das Verhältnis von Gewicht zur Länge der Tour. Er multipliziert das Gewicht der transportierten Güter mit der Länge jedes einzelnen Abschnitts der Tour und berücksichtigt dabei die an jedem Bestimmungsort ausgelieferten und abgeholten Güter. Der Faktor sucht ein geringeres Gewicht-Strecken-Verhältnis.
- **Termin-Faktor:** Der Termin-Faktor zählt die Anzahl an Zielen, die innerhalb der vorgegebenen Auslieferungs- und Abholzeiten erreicht werden. Er sucht die Tour mit der größten Anzahl an Zielen mit zeitgerechter Lieferung.
- **Prioritäts-Faktor:** Der Prioritäts-Faktor bewertet die Tour nach der Anzahl der als vorrangig gekennzeichneten Ziele, die als erste angefahren werden. Er sucht Touren mit einer größeren Zahl von vorrangigen Zielen in den ersten Orten.
- **Zeit-Faktor:** Der Zeit-Faktor basiert einfach auf der Zeitdauer der Tour. Er sucht die Tour mit der kürzesten Zeit.

**Standardwerte** Wenn Sie die Symbol-Schaltfläche [Standardwerte] betätigen, werden die vorgenommenen Änderungen verworfen und die Werte werden auf die Standardwerte aus den Parametern (Ga_Distance_Proportion, Ga_Weight_Proportion, Ga_OnTime_Proportion, Ga_Priority_Proportion, Ga_Time_Proportion) zurückgesetzt. Das gilt ebenfalls für gesperrte Werte!

> **Ergänzende Informationen**
> ⇨ Tutorial, "So bearbeiten Sie die Tour" auf Seite 1-93

### Eine neue Tour zusammenstellen – Kosten
**Planung > Neue Tour > Kosten**

*Abb. 1-63 Neue Tour, Register Kosten*

In diesem Register erhalten Sie eine Übersicht zu allen Kosten, die während der Tour anfallen. Es wird unterschieden, zwischen geschätzten und tatsächlichen Kosten. Die Felder des rechten Bereiches (Tatsächliche Kosten) werden ergänzt, wenn der Fahrer von seiner Tour zurück ist und Ihnen den Tour-Report gegeben hat. Dann können Sie diese tatsächlichen Werte eintragen.

#### Erläuterung der Felder im Bereich Variable Kosten

**Gesamtstrecke** In diesem Feld wird Ihnen die Gesamtstrecke der Tour angezeigt.
**Zeit** Hier sehen Sie, wie viel Zeit die Tour in Anspruch nimmt.
**Kraftstoffkosten** In diesem Feld werden Ihnen die Kraftstoffkosten angezeigt, die Sie im Register **Allgemein** im Feld Krafststoffkosten eingegeben haben.
**Kraftstoffverbrauch** In diesem Feld wird Ihnen der Verbrauch angezeigt, den Sie im Register **Allgemein** im Feld Krafststoffverbrauch eingegeben haben.
**Kosten pro Fahrer** In diesem Feld werden Ihnen die Kosten angezeigt, die pro Fahrer anfallen.
**Mautkosten** Falls Mautstraßen in der Tour enthalten sind, können Sie die zu erwartenden Mautkosten hier hinterlegen.
**Kraftstoffkosten** In diesem Feld werden Ihnen die Kraftstoffkosten für die Tour angezeigt.
**Extrakosten** In diesem Feld werden Ihnen die Extrakosten für die Tour angezeigt.

#### Erläuterung der Felder im Bereich Tatsächliche variable Kosten

**Tatsächliche Kosten pro Fahrer** In diesem Feld werden Ihnen die Kosten angezeigt, die pro Fahrer anfallen.
**Tatsächliche Mautkosten** Falls Mautstraßen in der Tour enthalten sind, werden Ihnen hier die Mautkosten angezeigt.
**Tatsächliche Kraftstoffkosten** In diesem Feld werden Ihnen die Kraftstoffkosten für die Tour angezeigt.
**Tatsächliche Gesamtstrecke** In diesem Feld wird Ihnen die Gesamtstrecke der Tour angezeigt.
**Tatsächliche Zeit** Hier sehen Sie, wie viel Zeit die Tour in Anspruch nimmt.
**Tatsächliche Extrakosten** In diesem Feld werden Ihnen die Extrakosten für die Tour angezeigt.

#### Erläuterung der Felder im Bereich Fixe Kosten

**Fixkosten** In diesem Feld sehen Sie, wie groß der Anteil der Fixkosten ist.

#### Erläuterung der Felder im Bereich Tatsächliche Fixkosten

**Tatsächliche Fixkosten** In diesem Feld sehen Sie, wie groß der Anteil der Fixkosten ist.

#### Erläuterung der Felder im Bereich Tourkosten

**Tourkosten** In diesem Feld sehen Sie, wie viel die gesamte Tour kosten wird.

#### Erläuterung der Felder im Bereich Tatsächliche Tourkosten

**Tatsächliche Tourkosten** In diesem Feld sehen Sie, wie viel die gesamte Tour kosten wird.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Fahrzeuge" auf Seite 1-45
> ⇨ Tutorial, "Fahrer" auf Seite 1-49

### Bereiche
**Planung > Gruppen**

*Abb. 1-64 Bereiche*

In diesem Dialog stellen Sie ein, in wie viele Bereiche die Touren aufgeteilt werden.
Geben Sie die Anzahl ein und schließen Sie den Dialog. Die Bereiche werden automatisch angepasst.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Der dynamische Modus" auf Seite 1-17

### Fahrzeuge (Planung)
**Planung > Fahrzeuge**

*Abb. 1-65 Fahrzeug wählen*

Über diesen Dialog können Sie einer Tour ein anderes Fahrzeug zuweisen. Markieren Sie das gewünschte Fahrzeug und verlassen Sie den Dialog über die Schaltfläche [OK].
Der ausgewählten Tour wird das oder die gewünschten Fahrzeuge zugewiesen.
Die Checkbox **Maximale Beladung und Zeit vor Ort** ist standardmäßig aktiv. Damit wird sichergestellt, dass das gewünschte Fahrzeug nicht überladen wird und dass z. B. die zulässigen Fahrzeiten, sowie die Be- und Entladezeiten eingehalten werden. Ist dies nicht der Fall, wird automatisch ein weiteres Fahrzeug eingesetzt.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Fahrzeuge" auf Seite 1-45

### Bestimmungsort bearbeiten
**Planung > Bestimmungsort bearbeiten**

*Abb. 1-66 Bestimmungsort bearbeiten*

In diesem Dialog können Sie den Bestimmungsort innerhalb einer Tour bearbeiten.

> **Adresse ändern**
> Die Änderungen, die Sie hier machen, haben keinen Einfluss auf die eigentlichen Stammdaten aus A+W Business. Die Änderungen werden in der OTR-Datenbank gespeichert und stehen dort zur Verfügung.

#### Erläuterung der Felder

**Kunden-Nr.** In diesem Feld wird Ihnen die Kunden-Nr. angezeigt.

**Kunden** In diesem Feld wird Ihnen der Kunden-Name angezeigt.

**Symbol-Schaltfläche** Diese Symbol-Schaltfläche ist nur aktiv, wenn in den Parametern der Wert **OTR-Kundenadresse** aktiv ist. Wenn Sie diese Symbol-Schaltfläche betätigen, öffnet sich der Dialog **Kunde**. Er enthält alle in der OTR-Datenbank gespeicherten Kunden.

**Typ** Wählen Sie aus der Kombobox den entsprechenden Tour-Typ aus. Mögliche Werte sind:
- **Mittelpunkt:** Der Mittelpunkt ist ein beliebiger Wegpunkt innerhalb der Tour.
- **Start-Punkt:** Der Start-Punkt ist der Anfangspunkt der Tour.
- **End-Punkt:** Der End-Punkt ist der Endpunkt der Tour.

**Zeit** In diesem Feld können Sie die Zeit in Minuten hinterlegen, die dem Fahrer zum Abladen und eventuellen neu Laden (Leergestelle) zur Verfügung steht.

**Ausgewählte Tour** Hier werden Ihnen die Touren angezeigt, die in der Tabelle **Touren** im Bereich **Planung** zu sehen sind. Sie können die Kombobox aufklappen und eine andere Tour auswählen.

**Liefertermin** In diesem Feld wird Ihnen der Liefertermin angezeigt. Den Wert können Sie an dieser Stelle nicht ändern, da Liefertermine nur für gesamte Touren geändert werden können und nicht für einzelne Bestimmungsorte. Um den Termin zu ändern, öffnen Sie den Dialog **Touren**, indem Sie eine Tour doppelt anklicken.

**Tour** Hier sehen Sie die ursprünglichen Tour-Nummer. Dieser Wert kann nicht geändert werden.

**Reihenfolge** Ist für zwei oder mehrere LKWs die gleiche Tournummer erlaubt, dann können Sie über dieses Feld die Reihenfolge der LKWs bestimmen. Das Feld wird nur ausgewertet, wenn in den Parametern der Eintrag **ROUTE_ORIGIN** den Wert Ja hat.

**Versandgewicht** In diesem Feld wird Ihnen das Gewicht der Lieferung für den jeweiligen Kunden angezeigt. Sie können den Wert überschreiben.

**Rückholgewicht** Sollte der Fahrer an einem Bestimmungsort leere Gestelle aufladen und zurück transportieren, haben Sie in diesem Feld die Möglichkeit, das entsprechende Gewicht zu hinterlegen. So haben Sie immer einen Überblick bezüglich des Gesamtgewichtes der Tour.

**Priorität** Aktivieren Sie diese Checkbox, wenn es sich bei der Adresse um eine Prioritätsadresse handelt.

**Rechtzeitig** Aktivieren Sie diese Checkbox, wenn die Adresse pünktlich angefahren werden soll.

**Zeitbereich** Klicken Sie auf die Symbol-Schaltfläche dahinter und es öffnet sich der Dialog **Zeitbereich**. In diesem können Sie dann angeben, wann der Kunde angefahren werden kann.

**Beschreibung** In diesem Feld können Sie eine detaillierte Beschreibung hinterlegen.

**Adresse** In diesem Feld wird Ihnen die Adresse des Kunden angezeigt.

**Breitengrad** In diesem Feld finden Sie den Breitengrad der Firmen-Adresse.

**Längengrad** In diesem Feld finden Sie den Längengrad der Firmen-Adresse.

**Vorschläge** Wenn Sie die Symbol-Schaltfläche [Vorschläge] betätigen, öffnet sich eine kleine Tabelle, die entsprechende Vorschläge zu der Adresse enthält. Bei mehreren Einträgen, können Sie einen auswählen. Betätigen Sie die Schaltfläche [Akzeptieren], werden die Daten in den Dialog **Tour** übernommen.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Bestimmungsorte" auf Seite 1-73
> ⇨ Tutorial, "So bearbeiten Sie einen Bestimmungsort" auf Seite 1-82

### Zeitbereich
**Planung > Bestimmungsort bearbeiten > von...bis...**

*Abb. I-67 Zeitbereich*

In diesem Dialog können Sie einen Zeitbereich für einen Kunden hinterlegen.

#### Erläuterung der Felder

**Von/Bis** Sollten Ihre Kunden fixe Abladezeiten haben, dann können Sie diese hier hinterlegen. Bsp.: von 11.30 Uhr bis 13.00 Uhr. Im Feld **Von** geben Sie dann **11:30** ein und im Feld **Bis** **13:00**.

### Dokumente
**Planung > Bestimmungsort bearbeiten > Register Dokumente**

*Abb. 1-68 Bestimmungsort bearbeiten, Register Dokumente*

In diesem Dialog werden Ihnen die Dokumente für den selektierten Bestimmungsort angezeigt. Es handelt sich dabei um reine Anzeigefelder. Sie können keine Änderungen vornehmen.

#### Erläuterung der Felder

**Status** In diesem Feld wird Ihnen der Status des Wegpunktes angezeigt.

**Auftrags-Nr.** In diesem Feld wird Ihnen die Auftrags-Nr. des Kundenauftrags angezeigt.

**Kunde** In diesem Feld wird Ihnen die Kunden-Nummer angezeigt.

**Name** In diesem Feld wird Ihnen der Kunden-Name angezeigt.

**Versandgewicht** In diesem Feld wird Ihnen das Gewicht der Lieferung für den jeweiligen Kunden angezeigt.

**Rückholgewicht** Sollte der Fahrer an einem Bestimmungsort leere Gestelle aufladen und zurück transportieren, wird Ihnen das Gewicht dieser Gestelle hier angezeigt.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Dokumente anzeigen" auf Seite 1-74

### Positionen anzeigen
**Planung > Bestimmungsort bearbeiten > Register Positionen**

*Abb. 1-69 Bestimmungsort bearbeiten, Register Positionen*

In diesem Dialog werden Ihnen die einzelnen Positionen der Tour(en) in einer tabellarischen Übersicht angezeigt.

#### Erläuterung der Felder

**Auftrag** In diesem Feld sehen Sie die Auftragsnummer.

**Pos.** In diesem Feld sehen Sie die Positionsnummer des Auftrages.

**Produkt** In diesem Feld sehen Sie die Artikelnummer.

**Bezeichnung 1-3** In diesem Feld wird Ihnen die Bezeichnung 1-3 des Produktes angezeigt.

**Datum** In diesem Feld sehen Sie das Bestelldatum des Auftrages.

**Menge** In diesem Feld wird Ihnen die bestellte Menge je Position angezeigt.

**Breite** In diesem Feld wird Ihnen die Breite der Einheit angezeigt.

**Höhe** In diesem Feld wird Ihnen die Höhe der Einheit angezeigt.

**Dicke** In diesem Feld wird Ihnen die Dicke der Einheit angezeigt.

**Gesamtgewicht** In diesem Feld wird Ihnen das Gesamtgewicht der Position angezeigt. Es ergibt sich aus dem Gewicht der Einheit multipliziert mit der Menge.

**M²** In diesem Feld werden Ihnen die Quadratmeter der Position angezeigt. Diese ergeben sich aus den Abmessungen und werden von A+W Business übergeben.

> **Ergänzende Informationen**
> ⇨ Tutorial, "Positionen anzeigen" auf Seite 1-75

### Informationen anzeigen
**Planung > Bestimmungsort bearbeiten > Register Informationen**

*Abb. 1-70 Bestimmungsort bearbeiten, Register Informationen*

In diesem Dialog werden Ihnen zusätzliche Informationen zum Bestimmungsort angezeigt.

#### Erläuterung der Felder

**Ansprechpartner** In diesem Feld können Sie einen Ansprechpartner beim Kunden hinterlegen.

**Telefon** In diesem Feld können Sie die Telefonnummer des Kontaktes hinterlegen.

**E-Mail-Adresse** In diesem Feld können Sie die E-Mail-Adresse des Kontaktes hinterlegen.

**Beschreibung** In diesem Feld können Sie eine weitere Beschreibung zu dem Kunden hinterlegen.

**Adresse** In diesem Feld wird Ihnen die Adresse des Kunden angezeigt. Die Daten können an dieser Stelle geändert werden.

**Längengrad** In diesem Feld finden Sie den Längengrad der Firmen-Adresse. Die Daten können an dieser Stelle geändert werden.

**Breitengrad** In diesem Feld finden Sie den Breitengrad der Firmen-Adresse. Die Daten können an dieser Stelle geändert werden.
