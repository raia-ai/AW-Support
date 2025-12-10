---
title: "D-AWBusiness-HB_2"
source: "D-AWBusiness-HB_2.pdf"
tags: ["A+W Business", "Stammdaten", "Kundendaten", "Lieferantendaten", "Aufträge", "Finanzen", "ERP", "Tutorial", "Auftragsverwaltung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial on managing master data in A+W Business software, focusing on creating and managing orders, customers, and suppliers. It covers order headers, positions, basic tables, and the overall commercial process flow."
long_description: "This document is an excerpt from a tutorial (Tutorial 1) for the A+W Business software, specifically focusing on the management of master data (Stammdaten). The tutorial provides an overview of how to create and manage orders, which form the basis of all commercial activities in the system. It details the necessary data for an order, including the order header (customer information, delivery terms) and order positions (products, dimensions, prices, surcharges). The document explains the structure of the software's user interface, with screenshots illustrating the 'Auftragskopf' (order header) and 'Auftragspositionen' (order items). It then delves into setting up master data, recommending a specific sequence to avoid data dependency issues: customer data, product groups, products, prices, and special discounts. The guide covers the creation and management of basic tables, customer data (including addresses, contacts, financial details), and supplier data. Specific topics include defining customer groups, tours for delivery planning, credit limits, payment terms, and handling of international currencies and taxes. The tutorial aims to equip users with the knowledge to set up and maintain the foundational data required for all subsequent sales, purchasing, and production processes within A+W Business."
---

# Tutorial 1: Überblick

---
## Aufträge in A+W Business

Alle kaufmännischen Vorgänge in A+W Business basieren auf den Stammdaten. Wenn Sie einen Auftrag erfassen, müssen (mindestens) folgende Daten eingetragen werden:

*   **Auftragskopf**
    *   Name und Anschrift des Kunden
    *   Lieferbedingungen und -termin
    *   Zahlungsbedingungen
*   **Auftragspositionen**
    *   Produkt und Produktaufbau, z. B. Glas, ISO, Sprossen
    *   Maße und Bearbeitungen, z. B. Modellformen, Ausschnitte
    *   Preise und Rabatte
    *   Zuschläge, z. B. für den Transport

*Abb. B-4 Auftrag im Verkauf*
*A Auftragskopf: Kunde, Liefertermin usw.*
*B Auftragspositionen: Produkt (Glas), Preise usw.*

Wenn die notwendigen Daten im Auftrag erfasst sind, müssen die Positionen produziert, verpackt und geliefert werden. Eventuell müssen für die Produktion zusätzliche Artikel eingekauft werden, die Sie nicht auf Lager halten. Aus dem Auftrag heraus entstehen also weitere Geschäftsabläufe, die so weit wie möglich automatisiert sind:

*   Druck von weiteren Dokumenten, z. B. Auftragsbestätigung, Lieferschein, Rechnung
*   Bestellung durch den Einkauf
*   Abruf der Lagerartikel für die Produktion
*   Übergabe der Auftragsdaten an die Produktion
*   Rückmeldung aus der Produktion, wenn der Auftrag fertig und versandbereit ist
*   Auslieferung
*   Prüfung der Zahlungen vom Kunden
*   Übergabe von Rechnungen an die Finanzbuchhaltung

Diese Abläufe werden in den Parts Verkauf, Einkauf, Lagerverwaltung und zur Fertigung behandelt.

Im Tutorial zu den Stammdaten lernen Sie, wie Sie die Daten der Marktpartner, Produkte und zu Preisen, Zuschlägen und Rabatten anlegen und pflegen. Im zweiten Teil der Schulung lernen Sie, wie diese Daten in Dokumenten getestet und wie die Abläufe gesteuert werden können.

### Stammdaten anlegen

Wenn Sie Ihre Stammdaten ganz neu anlegen, sollten Sie sich an die nachfolgende Empfehlung halten. Sie vermeiden damit, auf Daten zugreifen zu müssen, die noch nicht hinterlegt sind.

Aus der Kundenverwaltung heraus können Sie gleichzeitig auch viele Basisdaten anlegen und sich so an den aktuellen Erfordernissen für Ihre Kundenstammdaten orientieren.

> **Hinweis**
> Wenn Sie Basis- oder Stammdaten angelegt oder geändert haben, sollten Sie diese zunächst testen. Sie können so feststellen, ob das Resultat Ihren Vorstellungen entspricht, bevor Sie die neuen Daten tatsächlich einsetzen.

Folgende Reihenfolge wird zur Erfassung der Stammdaten empfohlen:

1.  **Kundendaten**
    Legen Sie zumindest die Kundendaten zur Adresse und zur Kommunikation an. Spezielle Preis- und Rabattvereinbarungen können Sie später bei Bedarf ergänzen.

2.  **Warengruppen**
    Entwerfen Sie zunächst das Warengruppenkonzept. Sie benötigen dieses zum Anlegen der Produkte.
    Die Warengruppen können auch aus der Produktverwaltung heraus angelegt werden.

3.  **Produkte**
    Gleichzeitig mit einem Produkt können Sie auch die Preise, Zuschläge und Rabatte anlegen. Sie können die Preise aber auch nach den Produkten anlegen und in der Produktdefinition nachträglich zuordnen.
    Wenn Sie neue Produkte und Preise angelegt haben, sollten Sie in der Angebots- bzw. Auftragserfassung testen, ob die Preise nach Ihren Vorstellungen berechnet werden. Sie verringern damit den eventuell nötigen Aufwand, nachträglich Stammdaten korrigieren zu müssen.

4.  **Preise**
    Wenn Sie Preise, Zuschläge und Rabatte angelegt haben, können Sie diese den Produkten zuordnen. Wenn bereits Sonstige Zuschläge vorhanden sind, können Sie diese den Preisen zuordnen.

5.  **Sonderrabatte/Teuerungszuschläge**
    Legen Sie die Rabatte oder Zuschläge an, die unabhängig von Preisen und Marktpartnern gültig sein sollen.
    Wenn Sie Sonderrabatte und Teuerungszuschläge angelegt haben, sollten Sie unbedingt in der Auftragserfassung testen, ob diese nach Ihren Vorstellungen eingefügt und berechnet werden.

## Basistabellen

In den verschiedenen Dialogen zum Erfassen von Stammdaten stehen Komboboxen mit Auswahllisten zur Verfügung, die die Eingabe von Daten erleichtern. Die Einträge in diesen Listen sind in aller Regel in sogenannten Basistabellen hinterlegt und können bearbeitet werden.

### Basistabelle erweitern

Das Anlegen von Daten in diesen einfachen Tabellen wird beispielhaft für Lieferantengruppen beschrieben.

**So hinterlegen Sie eine neue Lieferantengruppe**

1.  Wählen Sie Stammdaten > Marktpartner > Allgemein > Lieferantengruppen.
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    *Abb. B-5 Zeile für neue Lieferantengruppe freigeschaltet*
    ⇨ Softwarereferenz, "Lieferantengruppen" auf Seite B-758
3.  Tragen Sie mindestens den Namen der Lieferantengruppe ein. Achten Sie darauf, dass der Name sich auf die Besonderheit der Gruppe bezieht, z. B. Zubehörhändler.
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Lieferantengruppe wird gespeichert und steht zur Auswahl in den Dialogen zur Verfügung, in denen Gruppen zugewiesen werden können.

### Sperren

In fast allen diesen Dialogen können Einträge für die weitere Verwendung gesperrt werden.

*Abb. B-6 Beispiel für Basisdaten*
*A Fremdschlüssel*
*B Sperren*

Fremdschlüssel können zur Datenübergabe an andere Programme verwendet werden.

Gesperrte Einträge werden nicht mehr zur Auswahl angeboten. Wenn sie vor der Sperrung aber schon zugewiesen waren, werden sie weiterhin angezeigt.

### Löschen

Daten können nur dann gelöscht werden, wenn sie nirgends eingesetzt wurden, d. h., wenn sie nicht referenziert sind. Wenn referenzierte Daten nicht mehr verwendet werden sollen, müssen sie gesperrt werden.

Wenn Sie in den Übungen Testdaten anlegen, die nicht wirklich verwendet werden sollen, können Sie diese Daten allerdings sofort wieder löschen.

**Ergänzende Informationen**
⇨ Überblick, "Standard-Schaltflächen" auf Seite A-54

## Kundendaten

In diesem Themenblock lernen Sie, wie Sie die Stammdaten für Kunden einrichten.

Dazu gehören folgende Lerneinheiten:

*   "Marktpartner" auf Seite B-37
*   "Adressdaten" auf Seite B-42
*   "Auftrag und Kundenrechnung" auf Seite B-54
*   "Mitarbeiter und Filialen" auf Seite B-61
*   "Texte" auf Seite B-69
*   "Klassifikatoren" auf Seite B-75
*   "Finanzen und Saldo" auf Seite B-82
*   "Vertreter" auf Seite B-112
*   "Produktion" auf Seite B-116
*   "Ergänzende Daten für Partner" auf Seite B-121

Die Daten für Kunden und Lieferanten unterscheiden sich nur geringfügig. In dieser Lerneinheit gelten die Erklärungen und Handlungsschritte daher in den meisten Fällen auch für Lieferanten.

## Marktpartner

**Lernziele**

*   Unterschied der Stammdaten für Marktpartner, Kunden und Lieferanten kennenlernen.
*   Basistabellen für Marktpartner ergänzen.

**Nutzen**

*   Partnerdaten dienen zur schnellen Erfassung von Aufträgen und Bestellungen, ohne die Daten jeweils vollständig eingeben zu müssen.
*   Die Einträge in den Basistabellen werden in den komplexeren Dialogen mit einander verknüpft, um bestimmte Funktionen zu erfüllen, z. B. das Landeskürzel für die Auswahl der Formularsprache.

**Merke**

*   **Marktpartner**: In A+W Business wird zwischen Kunden, Lieferanten und sonstigen Partnern unterschieden:
    *   **Kunden** sind all diejenigen, zu denen Aufträge erstellt werden und die von Ihnen mit Produkten beliefert werden.
    *   **Lieferanten** sind alle diejenigen, bei denen Sie Produkte bestellen, die im eigenen Unternehmen nicht selbst hergestellt werden.
    *   **Partner** sind all diejenigen, die weder Kunden noch Lieferant sind, z. B. der Getränkeservice, der Steuerberater. Zu diesen Partnern können in A+W Business keine Dokumente erfasst werden. Partner aus diesem Bereich können nachträglich in die Stammdaten für Kunden oder Lieferanten kopiert werden.
*   **Partnerstammdaten**: In den Partnerstammdaten werden alle Informationen hinterlegt, die zum Erfassen eines Auftrags oder einer Bestellung (Dokumente) notwendig sind. Diese Daten werden automatisch in den Dokumentenkopf übernommen und können pro Dokument überschrieben werden. Solche Änderungen werden nicht in die Stammdaten des jeweiligen Partners zurückgeschrieben.
*   **Basistabellen**: Basistabellen werden als einfache Dialoge dargestellt. Sie sind in den Untermenüs des Moduls Stammdaten thematisch gruppiert.
*   **Checkbox Sperren**: Einträge in den Basistabellen können gesperrt werden. Gesperrte Einträge werden nicht mehr zur Auswahl angeboten. Wenn sie vor der Sperrung aber schon zugewiesen waren, werden sie weiterhin angezeigt.
*   **Datenexport**: Die Daten zu Marktpartnern können Sie für jeden Mandanten einzeln verwalten. Mit der integrierten Export-Funktion können Sie Partnerdaten exportieren, z. B. um Serienbriefe zu erstellen.

### Einführung in das Thema Marktpartner

In der Partnerverwaltung werden nicht nur die Adressen zu den Marktpartnern hinterlegt sondern auch Parameter, die die Angebots- und Auftragserfassung erleichtern, z. B. Tourenzuordnungen, abweichende Rundungen, Mitarbeiter und Filialen, Zahlungsbedingungen, Objekte.

*Abb. B-7 Zusammenwirken der Stammdaten zur Partnerverwaltung*

Die Abbildung zeigt das Zusammenspiel von Basisdaten für die Definition und Pflege der Partnerstammdaten. Damit Partnerdaten vollständig angelegt und gepflegt werden können, müssen die Basisdaten hinterlegt sein, z. B. Anreden, Rabatte, Rundungen.

### Dialog Partnerverwaltung

Die Daten zu Kunden und Lieferanten werden in A+W Business als Partnerstammdaten im Dialog Partnerverwaltung hinterlegt. Diese Stammdaten werden in den Dokumenten herangezogen und können bei Bedarf überschrieben werden. Änderungen aus den Dokumenten werden nicht in die Stammdaten zurückgeschrieben.

*Abb. B-8 Dialog Partnerverwaltung*
*A Register für die unterschiedlichen Kundendaten*
*B Basistabelle öffnen*
*C Zusatzinformationen und deren Anzeige*

⇨ Softwarereferenz, "Partnerverwaltung - Adresse" auf Seite B-771

Zu den Stammdaten der Kunden gehören neben den Adress- und Kommunikationsdaten auch Daten zu Finanzen und Kreditwürdigkeit und spezifische Produktionsdaten. Über das Ordner-Symbol (B) können Sie in die jeweilige Basistabelle wechseln, um die Daten zu ergänzen.

Weitere Besonderheiten zu den Lieferanten lernen Sie in der entsprechenden Lerneinheit kennen.

> **Datenschutz beachten**
> Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.

### Stammdatendialoge für Marktpartner

Im Menü Marktpartner finden Sie die Untermenüs Allgemein, Kunde und Lieferant, in denen Sie die allgemeinen und die partnerspezifischen Daten hinterlegen. Alle diese Dialoge sind ausführlich in der Softwarereferenz beschrieben.

⇨ Softwarereferenz, "Marktpartner" auf Seite B-754

Damit Sie die Kunden- und Lieferantendaten vollständig anlegen können, müssen folgende Basisdaten hinterlegt sein.

| Pfad > Dialog | Bedeutung |
| :--- | :--- |
| **Marktpartner > Allgemein > Anreden** | Neben den üblichen Anreden wie Herr, Frau und Firma können Sie auch andere Bezeichnungen hinterlegen, z. B., um ausländische Partner korrekt anzusprechen. |
| **Marktpartner > Allgemein > Titel** | Als Titel werden in A+W Business vor allem die Stellungen der Ansprechpartner verstanden, also z. B. Produktionsleiter, Geschäftsführer. |
| **Versand > Lieferbedingungen** | Die Lieferbedingungen beziehen sich auf das Transportmittel, mit dem ausgeliefert werden soll, z. B. Bahn, Spediteur. |
| **Versand > Touren** | In den Touren legen Sie neben dem Tag, an dem die Tour regelmäßig gefahren wird, auch die Lieferpauschale fest, die zur Berechnung der Frachtkosten herangezogen wird. Wichtig ist, dass Sie auch eine Tour für die Abholung und für den Transport mit einer Spedition anlegen - sofern Sie mit Speditionen zusammenarbeiten. |
| **Finanzen > Steuer** | Dies sind die unterschiedlichen Steuersätze, die Sie in den Aufträgen Ihrer Kunden berechnen. Sie können sowohl die inländischen als auch ausländischen Steuersätze hinterlegen und jedem einzelnen Kunden den passenden Steuersatz zuweisen. |
| **Finanzen > Zahlungsbedingungen** | Die Zahlungsbedingungen werden zur Berechnung des Zahlungsziels und des Skontobetrags herangezogen. |
| **Finanzen > Banken** | Dies sind Bankverbindungen, über die Sie die Geschäfte mit Ihren Kunden oder Lieferanten abwickeln. Wenn Sie die Angaben vollständig eingetragen haben, können Sie in den Partnerstammdaten die IBAN errechnen lassen. |
| **Finanzen > Währung** | Sie können die unterschiedlichen Währungen und dazu die Wechselkurse hinterlegen, wenn Sie mit mehreren Währungen arbeiten. Für den Euro-Raum selbst brauchen Sie keine Angaben zu machen. |
| **Finanzen > Zahlungswege** | Sie können die Zahlungsformen hinterlegen, die von Ihrem Unternehmen akzeptiert werden. Diese Angaben können auch an die Finanzbuchhaltung (FiBu) übergeben werden. |

*Tab. B-1 Stammdaten für die Vorbelegung von Feldern*

Neben den Daten, die in den Dialogen im Menü Marktpartner hinterlegt sind, können weitere Daten aus folgenden Dialogen bei der Definition von Kunden und Lieferanten herangezogen werden:

*   **Preise:**
    *   Jahrgang, Schlüssel, Tarif und Preis
*   **Zuschläge:**
    *   Sonstige Zuschläge, Austauschzuschläge, Modellzuschläge
*   **Finanzen:**
    *   Steuer, Kostenart, Kostenstellen

> **Beschreibung von Dialogen in weiteren Parts**
> Einige dieser Dialoge werden ausführlich in anderen Parts beschrieben. Diese Dialoge werden im Tutorial der Stammdaten nicht erläutert.

## Adressdaten

**Lernziele**

*   Dialog Partnerverwaltung erarbeiten.
*   Kundengruppen anlegen und zuweisen.
*   Touren und Lieferbedingungen anlegen und zuweisen.

**Nutzen**

*   Stammdaten von Kunden werden zentral eingegeben und gepflegt. Sie stehen damit immer aktuell für neue Aufträge zur Verfügung.
*   Die Adressdaten werden für die Lieferung und Rechnung verwendet. Abweichende Anschriften können jeweils eingegeben werden.

**Merke**

*   **Partnerverwaltung**: Im Dialog Partnerverwaltung hinterlegen Sie die Stammdaten eines jeden Kunden, die genau für diesen einen Partner gelten.
*   **Anschrift**: Zu jedem Marktpartner wird eine Hauptanschrift angegeben, die in aller Regel für die Lieferung und die Rechnung herangezogen wird.
*   **Branche**: Branchen stehen in der Statistik als zusätzliches Auswertungs- und Sortierkriterium zur Verfügung.
*   **Sprache**: Dokumente werden in den Formularen gedruckt, die der Sprache des Kunden entsprechen.
*   **Gruppen**: Kunden können einer Kundengruppen zugeordnet werden, z. B., um Rabatte oder Preise gemeinsam zu pflegen.
*   **Touren**: Touren bilden die Grundlage für die Versandplanung und -steuerung. Aus der Lieferdauer und dem Liefertermin wird der Versandtag berechnet.

### Vorgaben für Adressen

Im Register **Adresse** erfassen Sie die Daten zur Adresse, Kommunikation und zur Lieferung.

*Abb. B-9 Dialog Partnerverwaltung – Register Adresse*
*A Adressdaten für den Auftragskopf*
*B Verbindungsdaten werden ergänzt durch die Einstellung im Register Auftrag > Dokumentenversand*
*C Bereich Spezifikation: Auswahl und Anlegen der jeweiligen Angaben*

Die Einstellungen in diesem Register werden in den folgenden Abschnitten ausführlich erläutert.

**Branchen**

Jedem Kunden und Lieferanten können Sie eine Branche zuordnen, z. B. Glashandel, Fensterbau, Schreiner. Wenn ein neuer Kunde einer Branche angehört, die bisher nicht angelegt war, können Sie über das Ordner-Symbol in den Dialog **Branchen** wechseln, um die neue Branche einzutragen.

Die Branche steht in der Statistik als zusätzliches Auswertungs- und Sortierkriterium zur Verfügung.

**Sprache**

Jedem Kunden weisen Sie die Sprache zu, in der die Dokumente im Formular gedruckt werden sollen. Dem Kennzeichen entsprechend werden dann die jeweiligen Formulare ausgewählt.

Wenn Sie weitere Sprachen anlegen, sollten Sie jeweils auch die Preis- und Mengeneinheiten übersetzen.

**Gruppen**

Marktpartnern können in Gruppen zusammengefasst werden. Jeder Kunde kann einer Kundengruppe zugeordnet werden, jeder Lieferant einer Lieferantengruppe.

Wenn Sie z. B. Rabatte oder Preise für eine Gruppe festlegen, gelten diese Konditionen für alle Mitglieder der Gruppe. Damit vereinfachen Sie die Pflege der Konditionen.

Bei der Erfassung eines Dokuments können die Vorbelegungen überschrieben werden, die über die zugewiesene Gruppe in den jeweiligen Feldern angezeigt werden.

> **Beispiele für die Verwendung von Gruppen**
> 
> **Kundengruppe**
> *   Deckungsbeitrags-Grenzwerte
> *   Preise
> *   Rabatte
> *   Rundungen
> *   Zuschläge
> *   als Sortierkriterium in der Kunden-Umsatzstatistik
> 
> **Lieferantengruppe**
> *   Preise
> *   Rabatte
> *   Rundungen
> *   Zuschläge
> *   als Sortierkriterium in der Lieferanten-Umsatzstatistik

Die Gruppen für die Marktpartner legen Sie unter **Marktpartner > Allgemein > Partnergruppen, Kundengruppen, Lieferantengruppen** an. Gehen Sie dabei so vor, wie in der Einheit Basistabelle erweitern beschrieben.

⇨ "Basistabelle erweitern" auf Seite B-34

Wenn Sie die Gruppen angelegt haben, können Sie diese in der **Partnerverwaltung > Register Adresse** dem Kunden oder Lieferanten zuordnen.

*Abb. B-10 Partnerverwaltung - Gruppe zuordnen*

Bei der Berechnung von Aufträgen (oder Bestellungen) werden die Konditionen in folgender Reihenfolge berücksichtig:

*   Angaben aus dem Dokument
*   Definitionen aus den Partnerstammdaten
*   Gruppenspezifische Konditionen

Wenn keine Vereinbarungen gefunden werden, gelten die allgemeinen Preise, Zuschläge und Rundungen.

### Abweichende Kunden-/Lieferantengruppen

Wenn ein Kunde bei bestimmten Warengruppen andere Konditionen erhalten soll, kann er einer abweichenden Kundengruppe zugeordnet werden.

> **Beispiel**
> Sie haben u. a. die Kundengruppen Produzenten und Händler angelegt.
> Der Kunde A gehört zur Kundengruppe Händler. Wenn für diesen Kunden ein Auftrag mit einer Position aus der Warengruppe Wärmeschutz-ISO erfasst wird, sollen jedoch die Bedingungen der Kundengruppe Produzent gelten.
> Solche Ausnahmen legen Sie im Dialog **Abweichende Kundengruppen** fest.

*Abb. B-11 Zuordnung zu einer abweichenden Kundengruppe*
*A Zugeordneter Kunde*
*B Warengruppe*
*C Kundengruppe*

Ein Kunde kann einer abweichenden Kundengruppe auch dann zugeordnet werden, wenn er keiner (normalen) Kundengruppe zugeordnet ist. Die Konditionen der abweichenden Kundengruppe beziehen sich nur auf die angegebene Warengruppe. Alle anderen Konditionen, die für den Kunden gelten, bleiben unverändert bestehen.

Auf die gleiche Weise können Sie auch abweichende Zuordnungen zu Lieferantengruppen festlegen.

Wenn Sie die Partnergruppen sehr feingliedrig angelegt haben, können Sie für die einzelnen Marktpartner mehrere Abweichungen definieren. So kann z. B. ein Lieferant zur Gruppe *Händler* gehören, wenn Sie bei ihm Beschläge bestellen, und zur Gruppe *Produzent*, wenn Sie ESG-Scheiben bestellen.

### Touren und Lieferbedingungen

Im Zusammenspiel mit den Kundendaten und den Auftragsterminen bilden die Touren die Grundlage für die Versandplanung und -steuerung. Aus der Lieferdauer und dem Liefertermin wird der Versandtag berechnet, an dem die Lieferung an den Fahrer ausgegeben werden muss.

Die Lieferdauer ist in einer separaten Einheit beschrieben.

*Abb. B-12 Touren*

Pro Tour werden in den Stammdaten die Wochentage festgelegt, an denen sie gefahren wird. So kann eine Tour z. B. von Frankfurt nach Karlsruhe so eingerichtet sein, dass sie montags und donnerstags gefahren wird. Mit dieser Tour sollen alle Kunden beliefert werden, die auf dieser Strecke im Umkreis von 50 km liegen.

Dazu können Sie außerdem Frachtkosten angeben, über die im Auftrag geprüft werden kann, ob sich die Auslieferung eines einzelnen Auftrags lohnt. Die Art der Auslieferung stellen Sie als Lieferbedingung ein, z. B. Lkw oder Spedition.

Für Ihre ortsansässigen Kunden legen Sie außerdem eine Tour **Abholung** an, zu der jedoch keine Frachtkosten berechnet werden dürfen.

Jedem Kunden werden eine passende Tour und eine Rangfolgenummer zugewiesen. Die Rangfolge legen Sie im Register **Auftrag** fest.

Die Rangfolgenummer bestimmt die Reihenfolge, in der die Kunden pro Tour beliefert werden.

> **Beispiel**
> Kunde A und Kunde B werden mit Tour Süd beliefert. Kunde A hat die Tourrangfolge 1, Kunde B hat die Tourrangfolge 2.
> Kunde A wird also vor Kunde B beliefert.

Diese Einstellungen aus den Stammdaten werden in den Auftrag übernommen. Die Vorbelegung kann pro Auftrag geändert werden. Dabei wird automatisch geprüft, ob der eingegebene Liefertermin mit den Tourentagen des Kunden übereinstimmt. Bei einer Abweichung wird eine entsprechende Meldung ausgegeben. Abweichende Daten können gespeichert werden. Sie werden in der Tourenplanung übernommen.

**Zolltouren**

Für den grenzüberschreitenden Verkehr hinterlegen Sie Touren unter **Stammdaten > Versand > Zolltouren**. Sie können Grenzübergänge angeben oder den Namen der Tour. Die Zolltouren werden für die Versandplanung benötigt. Sie können in den Partnerstammdaten nicht zugewiesen werden.

Die Touren und Tourenplanung werden ausführlich im Part Fertigung beschrieben.

### Tour definieren

Sie können die hinterlegten Touren modifizieren oder durch neue Touren ergänzen. Wenn z. B. die Frachtkosten berechnet werden sollen, müssen Sie pro Tour die Kilometerpauschale eintragen.

**So legen Sie eine Tour an**

1.  Wählen Sie im Menü **Stammdaten > Versand > Touren**.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. B-13 Zeile für neue Touren freigeschaltet*
    *A Frei wählbare Nummer (ID)*
    *B Bezeichnung der Tour*
    *C Markierung der Wochentage, an denen die Tour gefahren wird.*
    
    ⇨ Stammdaten, "Touren" auf Seite B-873

3.  Geben Sie die Nummer (A) und Bezeichnung (B) ein. Beide können frei gewählt werden.
4.  Aktivieren Sie die Checkboxen (C) für die Tage, an denen die Tour regelmäßig gefahren wird. Die Angaben werden in der Auftragserfassung mit dem eingetragenen Liefertermin verglichen. Eine Meldung macht Sie darauf aufmerksam, wenn Termin und Tourentag nicht übereinstimmen.
5.  Verschieben Sie die Ansicht nach rechts (scrollen), um weitere Details festzulegen. Sie können dazu auch mit der `<Tab>`-Taste durch die Felder springen.

    *Abb. B-14 Versand-Touren anlegen - Abfahrtzeit*
    *A Abfahrtzeit pro Wochentag*
    *B Kilometerpauschale (Frachtkosten)*
    
    Sie müssen nicht sämtliche Daten eintragen. Wenn Sie z. B. nicht in Schichten arbeiten oder keinen eigenen Versand haben, können Sie die entsprechenden Felder überspringen.
6.  Verschieben Sie die Ansicht noch weiter nach rechts, um z. B. die Frachtkosten pro Kilometer (B) einzugeben.

    > **Bei Abholung keine Anlieferung berechnen**
    > Sie müssen für die Tour Abholung, für die keine Anlieferpauschale berechnet werden darf, die Checkbox ohne Liefer. Pausch. aktivieren.

7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.
8.  Wiederholen Sie ggf. die Schritte 2 bis 7 für weitere Touren.

### Partnerstammdaten anlegen

Die Dialoge zum Erfassen von Kunden-, Lieferanten- und Partnerdaten unterscheiden sich nur unwesentlich voneinander und sind daher zu einer Beschreibung zusammengefasst. In der folgenden Handlungsanleitung wird der Dialog **Partnerverwaltung** für Kunden geöffnet. Die Handlungsschritte gelten in gleicher Weise für Lieferanten und Partner.

> **Potenzielle Kunden oder Lieferanten**
> Sie können Daten zunächst als allgemeinen Marktpartner erfassen. Über die Kopierfunktion können die Daten nachträglich als Kunde oder Lieferant gespeichert werden.

Im Dialog **Partnerverwaltung** können Sie sich die freien Nummern anzeigen lassen, indem Sie auf die [Lupe] neben dem Eingabefeld für die Nummer klicken.

*Abb. B-15 Anzeige und Auswahl der freien Nummern*
*A Freie Nummern*
*B Nummer, die übernommen werden soll.*

Ein entsprechender Dialog steht auch beim Anlegen von Produktdaten zur Verfügung.

**So legen Sie Kundendaten an**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden**. Der Dialog **Partnerverwaltung** wird mit dem Register **Adresse** geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. B-16 Felder für neuen Partner freigeschaltet*
    *A Pflichtfelder*
    *B Standard-Anschrift für Lieferung und Rechnung*
    *C Kommunikationsdaten*
    *D Sprache des Kunden*
    *E Angaben zur Lieferung*
3.  Wählen Sie ggf. den Mandanten aus, wenn in Ihrer Firma mehrere Mandanten angelegt sind.
4.  Geben Sie in den Pflichtfeldern (A) die Nummer und den Matchcode ein. Sie können die Nummern Ihrer Kunden, Lieferanten und sonstigen Geschäftspartner frei wählen, jedoch darf jede Nummer nur einmal vergeben werden. Sie können sich die freien Nummern anzeigen lassen, indem Sie auf die [Lupe] klicken.
5.  Geben Sie die Daten für die Anschrift (B) ein. Wenn Sie die gewünschten Daten noch nicht in der Kombobox finden, können mit einem Klick auf das Ordner-Symbol den entsprechenden Dialog öffnen und die Daten ergänzen.
6.  Geben Sie die Daten für die Verbindungen zur Kommunikation (C) ein.
7.  Wählen Sie die Haupttour (Tour 1), eine Ersatztour (Tour 2) (E) und die Lieferbedingung aus. Wenn Sie mit dem neuen Kunden in einer anderen Sprache (D) kommunizieren, so wählen Sie diese Sprache aus. In den Dokumenten wird der entsprechende Sprachenschlüssel angezogen, so dass z. B. die Bezeichnungen für Produkte in der eingestellten Sprache gedruckt werden. Die Beschreibungen zur Mehrsprachigkeit finden Sie in der Softwarereferenz.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Damit haben Sie die wichtigsten Daten zur Identifikation des Kunden erfasst. Sie können jetzt im Register **Auftrag** die Daten für die Rechnung ergänzen.
    ⇨ “So ergänzen Sie die Daten für Kundendokumente" auf Seite B-59

## Auftrag und Kundenrechnung

**Lernziele**

*   Auftragspriorität festlegen.
*   Einstellungen für Rechnungen, Monatsrechnung, Sammelrechnung kennenlernen.
*   Einstellung für Teillieferung und Teilfakturierung kennenlernen.

**Nutzen**

*   Vorgaben aus den Kundenstammdaten werden in Auftrag übernommen und müssen nicht immer wieder neu erfasst werden.
*   Die meisten Vorgaben aus den Stammdaten können im Auftrag angepasst werden.

**Merke**

*   **Priorität**: Die Auftragspriorität gibt an, mit welcher Dringlichkeit ein Auftrag gefertigt werden soll. Sie wird an die Kapazitätsplanung und damit an die Produktion übergeben.
*   **Rechnung**: Für jeden Kunden legen Sie die Vorgaben für die Rechnung fest:
    *   Sammelrechnungen
    *   Rechnungsmindestwert
    *   Ausgabe der Rechnung (einzeln, gesammelt)
*   **Standardrundungen**: Für die Preisberechnung wird die Fläche des Glases gerundet. Diese Rundung gilt nicht für die Produktion.
*   **Rechnungsform**: Sammelrechnungen, Monatsrechnungen oder Teilrechnungen können nur erstellt werden, wenn diese Formen in den Kundenstammdaten zugelassen sind.

### Vorgaben für Aufträge

Im Register **Auftrag** legen Sie Details für die Rechnungen und die Lieferung fest.

*Abb. B-17 Partnerverwaltung - Auftrag*
*A Standardrundung für Höhe und Breite*
*B Angaben zur Rechnungsstellung*
*C Auftragspriorität*
*D Angaben zur Fakturierung*

Die Angaben zur Rechnung (A, B, D) und zur Priorität (C) können im Auftrag geändert werden. Diese Vorgaben werden im Folgenden ausführlich beschrieben.

**Auftragspriorität**

Die Auftragspriorität gibt an, mit welcher Dringlichkeit ein Auftrag gefertigt werden soll. Sie wird an die Kapazitätsplanung und damit an die Produktion übergeben.

*   **Eilt**: Die Aufträge werden mit oberster Priorität gefertigt.
*   **Normal**: Die Aufträge werden in den üblichen Ablauf eingeordnet.
*   **Zugabe**: Der Auftrag soll so gefertigt werden, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
*   **Abruf**: Die Aufträge werden auf Abruf gefertigt.

### Vorgaben für die Rechnung

Für jeden Kunden legen Sie die Vorgaben für die Rechnungen fest:

*   Standardrundungen
*   Rechnungsmindestwert
*   Ausgabe der Rechnung (einzeln, gesammelt)

*Abb. B-18 Kundenstammdaten - Register Auftrag*
*A Maßrundungen zur Preisberechnung*
*B Zuschlag für Rechnungsmindestwert*
*C Höhe des Mindestwerts*
*D Kennzeichen für Sammelrechnung*
*E Ausstellung der Rechnung und Druck der Preise*
*F Teillieferung und Teilfakturierung*
*G Aktivierung von Standardzuschlägen*
*Η Monatsrechnung*

**Standardrundungen**

Für die Preisberechnung wird die Fläche des Glases gerundet (A). In Deutschland basiert die Preisberechnung auf einer 30er-Maßrundung. Dies bedeutet, dass zur Berechnung der nächste durch 30 teilbare Wert zugrunde gelegt wird. Daraus ergibt sich bei einem Glas von 1000 mm x 1000 mm für die Preisberechnung die Fläche 1,04 qm (= 1020 x 1020). In Frankreich wird z. B. mit einer 10er-Maßrundung gerechnet.

Diese Rundung gilt nicht für die Produktion.

Die Maßrundung aus den Partnerdaten kann durch andere Vorgaben übersteuert werden. Dabei sucht A+W Business in folgender Reihenfolge nach den Angaben: Individualpreise > Rabatte > Preise > Partnerstammdaten. Die Preisfindung wird ausführlich im Part Verkauf geschult.

**Zuschlag für Rechnungsstellung**

Der Zuschlag zur Rechnungsstellung (G) muss als **Sonstiger Zuschlag** angelegt werden. Diese Zuschläge lernen Sie in der gleichnamigen Einheit kennen.

*   **Für 1. Rechnung im Monat:** Jeweils für die erste Rechnung im Monat wird der Zuschlag erhoben. Auf alle weiteren Rechnungen im laufenden Monat entfällt dann der Zuschlag.
*   **Für jede Rechnung:** Der Rechnungsstellungszuschlag wird für jede Rechnung erhoben.

**Mindestauftragswert**

Pro Auftrag kann ein Mindestwert (C) festgelegt werden. Die Differenz zum Mindestauftragswert kann im Auftrag auf zwei Arten ausgewiesen werden:

*   **Als separate Position:** Liegt der Auftragswert unter dem vereinbarten Mindestauftragswert, wird automatisch die Zuschlagsposition Mindestauftragswert hinzugefügt, die den Differenzbetrag ausweist.
*   **Auf alle Positionen umgerechnet:** Die Differenz wird auf alle Positionen umgelegt.

Zur Berechnung stehen zwei Möglichkeiten zur Verfügung:

*   Sie legen einen Zuschlag fest, der im Auftrag herangezogen wird, wenn der Mindestwert nicht erreicht wird.
*   Im Auftrag wird automatisch der Mindestwert berechnet, wenn der Auftragswert unter der festgelegten Grenze liegt.

**Monatsrechnung**

Rechnungen können einzeln, gesammelt oder als Monatsrechnung (H) gedruckt und versendet werden, z. B. im monatlichen oder 2-wöchentlichen Turnus. Die Aufträge dieses Kunden erhalten bei Lieferscheindruck automatisch das Kennzeichen **Monatsrechnung**, anhand dessen Sie diese bei Fälligkeit zur Fakturierung selektieren können.

Dazu müssen in den Firmendaten im Register Druck den entsprechenden Druckpunkt und Statuspunkt eintragen sein.

*Abb. B-19 Firmendaten – Druck*

**Sammelrechnung**

Wenn ein Kunde keine Einzelrechnungen wünscht, erhalten alle seine Aufträge das Kennzeichen für Sammelrechnungen (D). Über dieses Kennzeichen können Sie die fälligen Rechnungen selektieren.

Folgende Kriterien müssen in allen Aufträgen des jeweiligen Kunden übereinstimmen, damit alle Aufträge eines Kunden beim Druck in einer Sammelrechnung zusammengefasst werden können:

*   Kundennummer
*   Kennzeichen Sammelrechnungsdruck im Auftrag
*   Zahlungsbedingungen und Fälligkeitsdatum
*   Währung
*   Mehrwertsteuer-Kennzeichen 1 und 2
*   Automatische Zuschläge: Zuschlag für Rechnungsstellung.
*   AV-Bereich
*   Rechnungsadresse (Name 1)
*   Liefertermin

Sobald sich bei einem Auftrag eines dieser Kriterien unterscheidet, wird der Sammelrechnungsdruck bei diesem Auftrag unterbrochen. Dieser Auftrag und alle Aufträge, die ihm im Nummernverwalter nachfolgen, erhalten dann automatisch eine neue Rechnungsnummer. In diesem Fall werden also zwei Rechnungen gedruckt. Wenn weitere Unterschiede auftreten, wird eine weitere Rechnungsnummer vergeben.

**Teillieferung, Teilfakturierung**

Sind für einen Kunden Teillieferungen (F) vereinbart, müssen Sie entscheiden, ob die Teillieferung mit oder ohne Teilfakturierung erfolgen soll.

Bei der Teilfakturierung erhält der Kunde zu jeder Teillieferung eine Teilrechnung. Der Teilrechnungsbetrag und die -menge werden von dem Originalauftrag abgezogen.

Ist die Teilfakturierung nicht zugelassen, ist der Originalauftrag für die Fakturierung so lange gesperrt, bis die letzte Teillieferung erfolgt ist.

> **Teillieferung im Auftrag**
> Sie können aus einem Auftrag nur dann eine Teillieferung erzeugen, wenn in den Stammdaten des Kunden die Checkbox **Teillieferung** markiert ist.

### Einstellungen für den Kundenauftrag bearbeiten

Die folgende Handlungsanleitung baut auf den Schritten auf, die in der vorigen Einheit beschrieben wurden.

**So ergänzen Sie die Daten für Kundendokumente**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Auftrag**.

    *Abb. B-20 Adressen und Lieferdaten*
    *A Standard für Maßrundung*
    *B Rechnungsstellung*
    *C Versand der Dokumente*
    *D Teillieferung, Teilfakturierung*
    *E Tourrangfolge*
2.  Prüfen Sie, ob die Werte für die Maßrundung (A) korrekt angegeben sind.
3.  Legen Sie den Modus für die Rechnungsstellung (B) fest.
4.  Markieren Sie die Schaltflächen (C) für den Faxversand und den Mailversand von Dokumenten.

    Die Funktion kann für folgende Dokumente getrennt aktiviert werden:
    *   Auftragsbestätigung (AB)
    *   Angebot (An)
    *   Rechnung (Re)
    *   Gutschrift (Gu)

    Achten Sie darauf, dass Sie dazu auch die entsprechenden Faxnummern und die E-Mail-Adressen im Register Adresse hinterlegen.
5.  Legen Sie fest, ob für den Kunden Teillieferungen und Teilfakturierungen (D) möglich sind.
6.  Prüfen Sie, ob die Nummer für die Tourrangfolge (E) und die Priorität richtig eingestellt sind.
7ten. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

Die Daten werden gespeichert. Sie können jetzt zu diesem Kunden Filialen und Mitarbeiter hinzufügen.

⇨ "So legen Sie eine Filiale an" auf Seite B-65
⇨ "So legen Sie die Mitarbeiterdaten eines Marktpartners an" auf Seite B-66

## Mitarbeiter und Filialen

**Lernziele**

*   Filialen als zusätzliche Lieferanschriften verwenden.
*   Vorgänge kennenlernen.

**Nutzen**

*   Filialen dienen als weitere Lieferanschriften, wenn der Kunde z. B. mehrere Lagerorte hat. Im Auftrag kann jeweils die gültige Lieferanschrift ausgewählt werden.
*   Zusätzliche Angaben zu Mitarbeitern dienen der Kontaktpflege, so dass zuständige Personen direkt angesprochen werden können.

**Merke**

*   **Filialen**: Für die Filialen Ihrer Marktpartner werden die gleichen Daten hinterlegt, wie für den Hauptsitz.
*   **Mitarbeiter**: Die Daten zu Mitarbeitern Ihres Kunden dienen zur Information.
*   **Vorgang**: Über Vorgänge können Sie bestimmte Kontakte mit dem Kunden verfolgen.

### Filialen des Kunden

Für die Filialen Ihrer Marktpartner werden die gleichen Daten hinterlegt, wie für den Hauptsitz. Die Daten des Hauptsitzes werden als Vorbelegung in den entsprechenden Feldern angezeigt und können angepasst werden.

*Abb. B-21 Filiale*

**Standard-Lieferanschrift als Filiale anlegen**

Neben der Firmenanschrift können Sie weitere Anschriften für die Lieferungen und für die Rechnungen angeben. Diese Anschriften werden als Filialen erfasst. Für die Filiale muss dann im **Register Adresse** im Bereich **Anschrift** die Checkbox **Standard** aktiviert werden, wenn diese Filiale die Standardlieferanschrift ist.

### Mitarbeiter des Kunden

Die Namen der Mitarbeiter Ihres Kunden können Sie zur Information hinterlegen.

*Abb. B-22 Mitarbeiter*

Als zusätzliche Informationen können Sie Angaben zur Abteilung, in der er arbeitet, seiner Funktion, und seine Durchwahl ergänzen. Sie können kennzeichnen, ob der Mitarbeiter alleiniger Ansprechpartner bei Fragen zum Auftrag und/oder zum Vertrieb ist.

Diese Angaben können für Auswertungen über die ODBC-Schnittstelle herangezogen werden.

### Vorgang

Über sogenannte Vorgänge können Sie z. B. verfolgen, wann und welcher Mitarbeiter des Kunden angerufen hat, um Infomaterial zu erhalten.

Dazu dokumentieren Sie auch, wann und durch wen der Vorgang verfolgt und abgeschlossen wurde.

*Abb. B-23 Vorgänge*

### Filialen hinzufügen

Wählen Sie die Nummer für die Filiale so, dass aus ihr die Verbindung zum Hauptsitz erkennbar ist, z. B. 10000 für den Kunden, 10100, 10200, ... für die Filialen.

**So legen Sie eine Filiale an**

> **Partnerverwaltung öffnen**
> Der Dialog Partnerverwaltung kann für Partner, Kunden und Lieferanten geöffnet werden. In der folgenden Handlungsanleitung wird der Dialog Partnerverwaltung für Kunden geöffnet. Die Handlungsschritte gelten in gleicher Weise für Lieferanten und Partner.

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden**. Der Dialog Partnerverwaltung wird geöffnet.
2.  Suchen Sie den Datensatz des gewünschten Partners.
3.  Wählen Sie im Menü **Funktionen > Gruppe Details > Filiale**.

    *Abb. B-24 Felder für neue Filiale freigeschaltet*
    *A Standard für Lieferanschrift*
    *B Filiale schließen und Hauptfirma anzeigen*
    *C Eigenständige Filiale*
    
    ⇨ Softwarereferenz, "Partnerverwaltung - Adresse" auf Seite B-771
4.  Tragen Sie mindestens die Adress- und Kommunikationsdaten ein. Weitere Daten können Sie in den Registern ergänzen, so wie in der Handlungssequenz zum Anlegen der Kundendaten beschrieben.
    ⇨ "So bearbeiten Sie die Daten für die Rechnungsstellung" auf Seite B-102
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert. Im Register Adresse sind die Checkbox **Standard** (A) und die Schaltfläche **[zurück zur Hauptfirma]** (B) freigeschaltet.
6.  Passen Sie die Daten der Filiale an, z. B. die Touren. Beachten Sie folgende Einstellungen:
    *   Aktivieren Sie die Checkbox **Standard** (A), wenn diese Filiale die Standardanschrift für Lieferungen ist.
    *   Aktivieren Sie die Checkbox **eigenständige Filiale** (C), wenn diese Filiale eigene Aufträge vergeben kann.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.
8.  Klicken Sie auf die Schaltfläche (B), um den Dialog zu schließen. Die Daten der Hauptfirma werden wieder angezeigt.

### Mitarbeiter hinzufügen

Mit den Daten zu Mitarbeitern Ihrer Marktpartner können Sie auch angeben, für welchen Bereich dieser Mitarbeiter zuständig ist. Diese Angabe wird lediglich als Information hinterlegt.

**So legen Sie die Mitarbeiterdaten eines Marktpartners an**

> **Partnerverwaltung öffnen**
> Der Dialog Partnerverwaltung kann für Partner, Kunden und Lieferanten geöffnet werden. In der folgenden Handlungsanleitung wird der Dialog Partnerverwaltung für Kunden geöffnet. Die Handlungsschritte gelten in gleicher Weise für Lieferanten und Partner.

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden**. Der Dialog Partnerverwaltung wird geöffnet.
2.  Suchen Sie den Datensatz des gewünschten Partners.
3.  Wählen Sie im Menü **Funktionen > Gruppe Details > Mitarbeiter**.

    *Abb. B-25 Felder für neuen Mitarbeiter freigeschaltet*
    *A Name des Mitarbeiters beim Kunden*
    *B Funktion des Mitarbeiters (nur zur Info)*
    *C Kommunikationsdaten*
    *D Felder freischalten*
    
    ⇨ Softwarereferenz, "Mitarbeiter" auf Seite B-806
    
    Wenn bereits Mitarbeiter des Kunden eingetragen sind, werden deren Daten angezeigt.
4.  Klicken Sie auf **[Neu]** (D), um die Felder freizuschalten. Wenn bereits Mitarbeiter des Kunden eingetragen sind, können Sie die Daten überschreiben.
5.  Tragen Sie mindestens den Namen (A) und die Telefonnummer (C) ein.
6.  Ergänzen Sie weitere Angaben, sofern diese für die Kommunikation mit dem Mitarbeiter wichtig sind, z. B. die Funktion des Mitarbeiters (B). Damit haben Sie die wesentlichen Daten eingetragen.

    *Abb. B-26 Felder für neuen Mitarbeiter freigeschaltet*
    *A Mitarbeiterdaten speichern*
7.  Klicken Sie auf **[Neu]** (A), um die Daten zu speichern. Die Daten werden gespeichert. Sie können jetzt Daten von weiteren Mitarbeitern anlegen, indem Sie die Schritte 5 bis 7 wiederholen.
8.  Klicken Sie auf **[Ende]**, um den Dialog zu schließen. Der Dialog Partnerverwaltung wird wieder im Vordergrund angezeigt. Im Register **Mitarb./Filiale/Vorg.** werden alle Mitarbeiter aufgelistet.

## Texte

**Lernziele**

*   Kundenspezifische Texte eintragen.
*   Textkennzeichen kennenlernen.

**Nutzen**

*   Texte dienen der Information über bestimmte Sachverhalte, z. B. über Sonderwünsche bei der Produktion.

**Merke**

*   **Kundenspezifische Texte**: Texte, die nur für einen einzigen Kunden gelten, können Sie in den Kundenstammdaten eingeben und automatisch im Dokument einfügen lassen.
*   **Allgemeine Texte**: Häufig verwendete Texte können Sie als allgemeine Texte hinterlegen und über die Kundenstammdaten automatisch im Dokument einfügen lassen.
*   **Textkennzeichen**: Über die Textkennzeichen können Sie steuern, in welchen Dokumenten die Texte gedruckt werden sollen, z. B. in Auftragsbestätigungen, in Lieferscheinen.

### Texte und Textkennzeichen

Immer wiederkehrende Texte können Sie hinterlegen und automatisch z. B. im Dokument einfügen lassen. Bei diesen Texten wird zwischen System-, Standard- und Rahmentexten unterschieden.

Standardtexte werden anhand von Textkennzeichen unterschieden, z. B. das Textkennzeichen O für Angebote, P für Produktion, L für Lieferschein. Die Textkennzeichen können Sie nach den Erfordernissen in Ihrem Betrieb hinterlegen.

> **Beispiele**
> *   **Info-Texte (Textkennzeichen /):** Diese Texte sollen in allen Dokumenten gedruckt werden, z. B. die Ankündigung von Betriebsferien.
> *   **Lieferscheinspezifische Texte (Textkennzeichen L):** Diese Texte sollen nur auf den Lieferscheinen gedruckt werden, z. B. die Reklamationsfrist.
> *   **Angebotstexte (Textkennzeichen O):** Diese Texte sollen nur auf Angeboten gedruckt werden, z. B. Gültigkeitsdauer des Angebots.

Die Textkennzeichen dienen nicht nur der Gruppierung Ihrer Standardtexte. Über die Textkennzeichen können auch Sie steuern, wann die Texte gedruckt werden sollen.

> **Beispiel**
> Produktionstexte (Textkennzeichen P) sollen auf dem Lieferschein nicht gedruckt werden. Pro Formular legen Sie in der Formularverwaltung fest, welche Textkennzeichen nicht gedruckt werden sollen.

Für jede ISO-Einheit können spezielle Rahmentexte hinterlegt und dem Produkt zugeordnet werden.

In den Stammdaten der Partner und der Produkte können Texte hinterlegt werden, die immer in die Dokumente übernommen werden. Dies können entweder Standardtexte sein oder der Text wird nur für den Partner oder das Produkt eingetragen.

> **Ausführliche Beschreibung der Texte**
> Die Texte sind ausführlich im Tutorial 2 beschrieben.
> ⇨ Tutorial 2, "Texte" auf Seite B-468

### Text in Kundenstammdaten erfassen

In diesem Beispiel wird ein Text in den Kundenstammdaten beschrieben. Auf die gleiche Weise können Sie Texte für Lieferanten oder Produkte erfassen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So ordnen Sie einen Standardtext zu" auf Seite B-71
*   "So tragen Sie einen kundenspezifischen Text ein" auf Seite B-73

> **Schriftart und -größe**
> Die Einstellungen für die Schriftart und die Schriftgröße gelten nur für die Anzeige auf dem Bildschirm. Sie werden nicht in den Druck übernommen.

**So ordnen Sie einen Standardtext zu**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Texte**.

    *Abb. B-27 Felder für neuen Text freischalten*
    *A Felder freischalten*
    *B Nummer des Standardtextes*
    *C Textkennzeichen prüfen*
2.  Klicken Sie Symbolschaltfläche (A), um die Eingabefelder freizuschalten.
3.  Geben Sie die Nummer (B) des gewünschten Standardtextes ein oder wählen Sie ihn über die Lupe aus. Wenn Sie die Textnummer direkt eintragen, müssen Sie mit der `<Tab>`-Taste ins nächste Feld springen, damit der Text eingelesen wird.

    *Abb. B-28 Zugewiesener Standardtext*
    *A Liste der zugewiesenen Texte*
    *B Bearbeitungsfeld*
    
    Der Standardtext wird im Bearbeitungsfeld (B) angezeigt. Sie können ihn bearbeiten und für den aktuellen Kunden anpassen.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

Der Standardtext wird dem Textkennzeichen entsprechend auf die jeweiligen Formulare gedruckt oder an die Produktion übergeben. Auf die gleiche Weise tragen Sie einen Rahmentext ein.

**So tragen Sie einen kundenspezifischen Text ein**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Texte**.

    *Abb. B-29 Text anlegen*
    *A Felder freischalten*
    *B Textnummer*
    *C Textkennzeichen auswählen*
    *D Eingabe des Textes*
2.  Klicken Sie Symbolschaltfläche (A), um die Eingabefelder freizuschalten.
3.  Wählen Sie das Textkennzeichen (C) aus, z. B. I Informationstexte. Das Textkennzeichen entscheidet, wie der Text verwendet wird. Wenn der Text z. B. an die Produktion übergeben werden soll, müssen Sie das Kennzeichen P wählen. Wenn Sie kein Textkennzeichen eingeben, wird der Text nicht übergeben. Lassen Sie im Feld **Nummer** (B) die 0 stehen.
4.  Schreiben Sie den gewünschten Text in das Eingabefeld (D).

    *Abb. B-30 Kundenspezifischer Text*
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert und dem Textkennzeichen entsprechend nur für diesen Kunden verwendet.

Auf die gleiche Weise können Sie Texte für einzelne Lieferanten, Partner oder Produkte erstellen.

## Klassifikatoren

**Lernziele**

*   Klassifikatoren anlegen.
*   Klassifikatorenwerte zuweisen.

**Nutzen**

*   Klassifikatoren dienen als Filter für zusätzliche Auswertungen, z. B. Umsatz.

**Merke**

*   **Klassifikatoren**: Klassifikatoren werden für alle Marktpartner gemeinsam oder jeweils für Kunden, Lieferanten oder Partner angelegt.
*   **Klassifikatorenwerte**: Klassifikatorenwerte können numerisch, alphanumerisch oder als Datum eingetragen werden.

### Klassifikator und Klassifikatorenwert

Klassifikatoren legen Sie an, um sie als Filter für zusätzliche Auswertungen zu nutzen, z. B. Umsatz, Geburtstag, Hobbys. Dazu definieren Sie, ob der Wert numerisch, alphanumerisch oder als Datum eingetragen wird. Nicht mehr benötigte Klassifikatoren können Sie löschen.

Um mit Klassifikatoren zu arbeiten, sind zwei Schritte erforderlich:

*   **Sie legen einen Klassifikator an.**
    In der Klassifikatorendefinition legen Sie fest, wie der Klassifikator heißt und mit welchen Werten er belegt werden kann.
*   **Sie weisen einen Klassifikatorenwert zu.**

### Klassifikator anlegen

Klassifikatoren für Kunden, Lieferanten oder Partner können Sie auch aus der jeweiligen Partnerverwaltung heraus anlegen.

**So legen Sie einen Klassifikator an**

1.  Wählen Sie **Stammdaten > Marktpartner > Kunde > Kunden > Menü Funktionen > Gruppe Klassifikatoren > Klassifikatorendefinition**.

    *Abb. B-31 Klassifikator anlegen*
    *A Register für die Gültigkeit*
    *B Felder freischalten*
    
    ⇨ Softwarereferenz, "Klassifikatoren" auf Seite B-764
    
    Im Register **Gemeinsam** hinterlegte Klassifikatoren gelten für alle Marktpartner. In den drei weiteren Registern legen Sie die Klassifikatoren an, die nur für die jeweilige Gruppe gelten.
2.  Wählen Sie das gewünschte Register, z. B. **Gemeinsam**. In diesem Register legen Sie einen Klassifikator an, der für alle Marktpartner gilt.
3.  Klicken Sie auf **[Neu]** (B), um die nächste Zeile freizuschalten.

    *Abb. B-32 Felder für neuen Klassifikator freigeschaltet*
    *A Frei wählbare Bezeichnung*
    *B Bemerkung, z. B. zur Verwendung*
    *C Art des Klassifikators: N: numerisch, A: alphanumerisch, D: Datum*
4.  Tragen Sie die Werte ein:
    *   Im Feld **Bezeichnung** (A) z. B. Umsatz Gruppen.
    *   Im Feld **Bemerkung** (B) z. B. ABC Klassifizierung.
5.  Markieren Sie eine der Checkboxen (C), um zu definieren, ob der Wert numerisch, alphanumerisch oder als Datum eingetragen werden muss. Diese Angabe bestimmt, in welcher Form Sie die Klassifikatorenwerte in der Partnerverwaltung eingeben dürfen und wie sie ausgewertet werden.
6.  Klicken Sie auf **[Neu]**, um die Daten zu speichern.

Die Daten werden gespeichert. Alle Klassifikatoren im Register **Gemeinsam** werden bei allen Marktpartnern in der Partnerverwaltung im Register **Klassifikatoren** angezeigt. Alle anderen Klassifikatoren werden nur bei den entsprechenden Marktpartnern angezeigt.

### Klassifikatorenwert zuweisen

In der Klassifikatorendefinition legen Sie fest, welche Art von Werten ein Klassifikator annehmen kann. Von dieser Definition ist abhängig, wie Sie den Wert zuweisen.

⇨ "Klassifikator anlegen" auf Seite B-76

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So ordnen Sie einen alphanumerischen Wert zu" auf Seite B-78
*   "So ordnen Sie einen numerischen Wert zu" auf Seite B-80

> **Partnerverwaltung öffnen**
> Der Dialog Partnerverwaltung kann für Partner, Kunden und Lieferanten geöffnet werden. In der folgenden Handlungsanleitung wird der Dialog Partnerverwaltung für Kunden geöffnet. Die Handlungsschritte gelten in gleicher Weise für Lieferanten und Partner.

**So ordnen Sie einen alphanumerischen Wert zu**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Klassifikatoren**.

    *Abb. B-33 Klassifikatorenwert zuweisen*
    *A Art des Klassifikators*
    *B Zugewiesener Wert*
2.  Markieren Sie einen Klassifikator (A) mit dem Kennzeichen **A** (alphanumerisch). Die gesamte Zeile wird markiert.
3.  Wählen Sie im Menü **Funktionen > Gruppe Klassifikatoren > Klassifikatorenwerte**. Sie können auch doppelt in das Feld **Wert** (B) des markierten Klassifikators klicken. Der Dialog **Klassifikatoren Wertzuordnung** wird geöffnet.

    *Abb. B-34 Klassifikatorenwert anlegen*
    *A Eingabezeile*
    *B Eingabezeile freischalten*
    *C Wert übernehmen*
4.  Klicken Sie auf **[Neu]** (B), um die nächste Zeile freizuschalten. Die nächste Zeile wird freigeschaltet.
    ⇨ Softwarereferenz, "Klassifikatoren Wertzuordnung" auf Seite B-810
5.  Tragen Sie den neuen Wert ein, z. B. Region Süd 1 für einen alphanumerischen Klassifikator für Umsatz.
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Die Daten werden gespeichert. Sie können weitere Klassifikatoren anlegen, indem Sie die Schritte 4 bis 6 wiederholen. Diese Klassifikatorenwerte werden nicht automatisch für den aktuellen Partner übernommen.
7.  Markieren Sie die Zeile mit dem Wert und klicken Sie auf **[Übernahme]** (C), um dem Partner diesen Wert zuzuweisen.

Der Dialog **Klassifikatoren Wertzuordnung** wird geschlossen und der Dialog **Partnerverwaltung** wird wieder im Vordergrund angezeigt.

*Abb. B-35 Übernommener Klassifikatorenwert*

Wenn Sie den Wert übernommen haben, wird er im Bereich **Klassifikatoren** angezeigt.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Werte werden gespeichert. Sie können jetzt zur Auswertung herangezogen werden.

**So ordnen Sie einen numerischen Wert zu**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Klassifikatoren**.
2.  Setzen Sie im Bereich Klassifikatoren den Cursor in das Feld **Wert** eines Eintrags mit dem Kennzeichen **N** (numerisch) oder **D** (Datum).
3.  Wählen Sie im Kontextmenü **Einfügen**. Das Kontextmenü öffnen Sie mit der rechten Maustaste.
4.  Tragen Sie die Werte entsprechend der Vorgabe ein:
    *   **N (numerisch)**, z. B. 600000 (Umsatz)
    *   **D (Datum)**, z. B. 23.02.2012 (Geschenk zum Geburtstag des Abteilungsleiters)
    Mit `<Tab>` können Sie in die nächste Zeile wechseln, um einen weiteren Wert einzutragen.

    *Abb. B-36 Numerischer Wert*
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

### Übungen

Die Übungen bauen auf einander auf. Sie werden daher die Daten, die Sie zu Übungszwecken anlegen, immer wieder benötigen. Kennzeichnen Sie diese Daten so, dass sie schnell erkannt werden können, z. B. mit dem Zusatz Schulung oder Demo.

*   Legen Sie mindestens einen neuen Kunden an.
*   Legen Sie Touren für Ihren Landkreis, für Abholung und eine Spedition an.
*   Legen Sie die Kundengruppe Schulung an.
*   Ordnen Sie jeweils Ihren Kunden einer Gruppe zu.
*   Ordnen Sie den Kunden einer anderen Kundengruppe zu, wenn für ihn ein Auftrag zu ESG erfasst wird.
*   Standardrundung
*   Modus der Rechnungsstellung
*   Teillieferung und Teilrechnung erlaubt
*   Hinterlegen Sie eine abweichende Rechnungsanschrift.
*   Definieren Sie eine der Anschriften als Standard-Lieferanschrift.
*   Erfassen Sie für Ihren Schulungskunden einen Text, der nur für ihn gilt und nur auf Produktionspapiere gedruckt wird.
*   Legen Sie drei Klassifikatoren mit unterschiedlichen Eigenschaften (numerisch, alphanumerisch, Datum) an.
*   Weisen Sie Ihrem Schulungskunden für jeden der Klassifikatoren einen Wert zu.

> **Demo-Daten sperren**
> Wenn Sie die Übungsaufgaben im tatsächlichen Betrieb machen, sollten Sie die Demo-Daten für die Verwendung sperren, sobald Sie Ihre Tests durchgeführt haben.

## Finanzen und Saldo

**Lernziele**

*   Bedingungen für Rechnungen und die Zahlungen kennenlernen.
*   Kalender und Zahlungstagverschiebung einrichten.
*   Prüfung des Kreditlimits einstellen.

**Nutzen**

*   Kundenrechnungen werden nach den Vorgaben aus den Kundenstammdaten erstellt.
*   Saldo und Kreditlimit werden in der Auftragserfassung angezeigt, so dass die aktuellen Aufträge und offenen Posten berücksichtigt werden können.

**Merke**

*   **Fälligkeit**: Fälligkeiten werden automatisch errechnet. Dazu geben Sie den gewünschten Modus an und legen die Daten für die Rechnungslegung fest.
*   **Zahlungsziel**: Das Belegdatum und der Tag der Rechnungslegung ergeben das erste Bezugsdatum. Dieses dient als Basis zur Berechnung des Zahlungsziels.
*   **Zahlungstagverschiebung**: Damit während der Betriebsferien des Kunden keine Rechnungen fällig werden, kann der entsprechende Zeitraum im Kundenkalender angegeben werden.
*   **Zahlungsbedingung**: Jede Zahlungsbedingung kann mehrere Stufen von Zahlungszielen und Prozentsätzen für das Skonto berücksichtigen.
*   **Kontonummer**: Die Kundennummer wird als Hauptkonto verwendet und an die FiBu übergeben. Als Hauptdebitor, an den die Rechnungen und Gutschriften gesendet werden, kann die Kundennummer einer Filiale des Kunden verwendet werden.
*   **Kreditlimit**: Für jeden Kunden kann ein Wert für das versicherte Kreditlimit und ein Wert für ein internes (unversichertes) Kreditlimit angegeben werden. Das Kreditlimit kann automatisch bei der Erfassung neuer Aufträge geprüft werden.
*   **Steuern**: Nur die Steuern können berechnet werden, die als Steuersatz hinterlegt und dem Kunden zugewiesen sind.
*   **Währungen**: Preise können in unterschiedlichen Währungen gepflegt werden. Dabei können Aufträgen in Landeswährung (Eigenwährung) oder Fremdwährung erfasst werden. Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von A+W Business umgerechnet.

### Vorgaben für die Zahlung

Für jeden Kunden legen Sie die Vorgaben für die Rechnungen im Register **Finanzen** fest.

*Abb. B-37 Kundenstammdaten – Register Finanzen*
*A Bankverbindung*
*B Fälligkeitsberechnung*
*C Rechnungslegung*
*D Zahlungsbedingung*
*E Hauptkonto oder abweichende Rechnungsanschrift*
*F Gültiger Steuersatz*

Die Bankdaten (A) des Kunden hinterlegen Sie, z. B, um diese für Gutschriften oder den Belegdruck zu verwenden.

Zu den Kundenrechnungen geben Sie an:

*   Modus der Fälligkeitsberechnung (B)
*   Angabe des Tags der Rechnungslegung (C)
*   Zahlungsbedingung (D)
*   Gültiger Steuersatz (F): Dabei ist es möglich, bis zu 5 verschiedene Steuersätze zu aktivieren.

Die Steuersätze selbst werden unter **Finanzen > Steuer** hinterlegt. Zusätzlich können Sie in den Firmendaten noch angeben, ob die Steuer pro Position oder pro Stücklisten-Komponente berechnet werden soll. Diese Angabe gilt dann für alle Kunden. Die Einstellungen in den Firmendaten sind in der Softwarereferenz beschrieben.

### Fälligkeitsberechnung

Fälligkeiten werden automatisch errechnet. Dazu geben Sie den gewünschten Modus an und legen die Daten für die Rechnungslegung fest:

*   Tag der Rechnungslegung, z. B., wenn nicht das Rechnungsdatum ausschlaggebend ist.
*   Zahlungsziel (Bruttotage)
*   Zahlungstage

| Modus | Text |
| :--- | :--- |
| 0 | 1. Bezugsdatum |
| 1 | 1. Bezugsdatum + Bruttotage |
| 2 | 1. Bezugsdatum + Bruttotage + Rundung auf 1. Zahlungstag oder Monatsende |
| 3 | 1. Bezugsdatum + Bruttotage + Rundung auf den 15. oder Monatsende |
| 4 | 1. Bezugsdatum + Bruttotage + Rundung auf den 10., den 20. oder Monatsende |
| 5 | 1. Bezugsdatum wird auf das Monatsende gerundet + Bruttotage (0/30/60/90). Das errechnete Zahlungsziel wird immer auf das Monatsende gerundet. Achtung: Bei Kennzeichen 5 und 6 muss der Wert im Feld Bruttotage durch 30 teilbar sein. 30 Tage = 1 Monat, 60 Tage = 2 Monate, 90 Tage = 3 Monate, um die das erste Bezugsdatum erhöht wird. |
| 6 | 1. Bezugsdatum wird auf das Monatsende gerundet + Bruttotage (0/30/60/90) + Zahlungstag |
| 7 | 1. Bezugsdatum + Bruttotage + Rundung auf 1., 2. oder 3. Zahlungstag |
| 8 | 1. Bezugsdatum + Bruttotage + Rundung auf 1. oder 3. Zahlungstag in Abhängigkeit vom 2. Zahlungstag |
| 11 | Fälligkeitsdatum = Lieferdatum + Zahlungsziel |

Beispiele für die Berechnung von Fälligkeiten finden Sie im Part Verkauf.
⇨ Verkauf, "Fälligkeitsberechnung" auf Seite C-215

**Rechnungslegung**

Das Belegdatum und der Tag der Rechnungslegung ergeben das erste Bezugsdatum. Dieses dient als Basis zur Berechnung des Zahlungsziels.

*   **Tag der Rechnungslegung = 0:** Das 1. Bezugsdatum ist gleich Belegdatum.
*   **Tag der Rechnungslegung ≠ 0:** Das Belegdatum wird auf den Tag der Rechnungslegung gerundet und ergibt das erste Bezugsdatum.

**Beispiele**

| Belegdatum | RLT | 1. Bezugsdatum | Anmerkung |
| :--- | :---: | :--- | :--- |
| 13.03. | 0 | 13.03. | 1. Bezugsdatum = Belegdatum |
| 13.03. | 25 | 25.03. | Das Belegdatum wird auf den 25. des gleichen Monats gerundet. |
| 27.03. | 25 | 25.04. | Der Tag der Rechnungslegung ist kleiner als das Belegdatum, aus diesem Grund wird das Belegdatum auf den 25. des Folgemonats gerundet. |

*RTL = Rechnungslegungstag*

Diese Beispiele zeigen, wie das erste Bezugsdatum aus dem Belegdatum (Rechnungsdatum) und dem Tag der Rechnungslegung errechnet wird.

### Zahlungstagverschiebung

Sie können für die Berechnung des Zahlungstags eine Verschiebung festlegen, z. B. damit keine Rechnungen während der Betriebsferien des Kunden fällig werden. Den Zeitraum für die Verschiebung stellen Sie im Kundenkalender ein.

Die Berechnung bezieht sich auf die Einträge im Kundenkalender. Die Art der Verschiebung gilt unabhängig von den Tagen aus dem Kundenkalender.

⇨ "Kundenkalender bearbeiten" auf Seite B-105

| Option | Art der Verschiebung |
| :--- | :--- |
| 0 | Keine Verschiebung |
| 1 | Hälftige Aufteilung - Fälligkeitsdaten werden hälftig aufgeteilt: Eine Hälfte des Betrags wird in einem bestimmten Zeitbereich vor dem ursprünglichen Fälligkeitsdatum fällig. Die andere Hälfte wird in einem bestimmten Zeitbereich nach dem ursprünglichen Fälligkeitsdatum fällig. |
| 2 | Verschiebung um einen Zeitbereich - Fälligkeitsdaten werden um einen bestimmten Zeitbereich in die Zukunft verschoben. |
| 3 | Entspricht Option 2 plus Zuschlag. Bei der Wahl dieser Option muss ein entsprechender Zuschlag angelegt sein. |

#### Beispiele

**Ausgangssituation:**

*   Rechnungsbetrag: 300 Euro
*   Rechnungsdatum: 10.07.
*   Kunde akzeptiert keine Fälligkeiten im Monat August (01.08. - 31.08.)

**Beispiel 1**
Zahlungsziel 30 Tage = Fälligkeitsdatum 10.08.

*   **Option 1: Hälftige Aufteilung**
    *   Fälligkeitsdatum 1: 10.07. = 150 €
    *   Fälligkeitsdatum 2: 10.09. = 150 €
    *   Der Rechnungsbetrag wird je zur Hälfte vor und nach den Betriebsferien fällig.
*   **Option 2: Verschiebung um einen Zeitbereich**
    *   Fälligkeitsdatum: 10.09. = 300 €
    *   Der gesamte Rechnungsbetrag wird nach den Betriebsferien fällig.
*   **Option 3: Entspricht Option 2 + Zuschlag**
    *   Fälligkeitsdatum: 10.09. = 303 € (300 € + 1%)
    *   Der gesamte Rechnungsbetrag wird nach den Betriebsferien fällig. Zusätzlich wird ein Zuschlag erhoben.

**Beispiel 2**
Zahlungsziele 30, 60 Tage
Fälligkeitsdatum 1: 10.08. = 150 €
Fälligkeitsdatum 2: 10.09. = 150 €

*   **Option 1: Hälftige Aufteilung**
    *   Fälligkeitsdatum 1: 10.07. = 75 €
    *   Fälligkeitsdatum 2: 10.09. = 225 €
    *   Zum 1. Fälligkeitsdatum sind 150 € fällig. Dieser Betrag wird hälftig aufgeteilt, so dass zum vorgezogenen 1. Fälligkeitsdatum 75 € fällig werden. Die restlichen 75 € werden zum 2. Fälligkeitsdatum fällig, so dass zu diesem Datum 150 € + 75 € fällig sind.
*   **Option 2: Verschiebung um einen Zeitbereich**
    *   Fälligkeitsdatum: 10.09. = 300 €
    *   Zum 1. Fälligkeitsdatum sind 150 € fällig. Dieser Betrag wird zum 2. Fälligkeitsdatum fällig, so dass zu diesem Datum 300 € fällig sind.
*   **Option 3: Entspricht Option 2 + Zuschlag**
    *   Fälligkeitsdatum: 10.09. = 303 € (300 € + 1 %)
    *   Der gesamte Rechnungsbetrag wird zum 2. Fälligkeitsdatum verschoben. Zusätzlich wird ein Zuschlag berechnet.

**Beispiel 3**
Zahlungsziele 30, 60, 90 Tage
Fälligkeitsdatum 1: 10.08. = 100 €
Fälligkeitsdatum 2: 10.09. = 100 €
Fälligkeitsdatum 3: 10.10. = 100 €

*   **Option 1: Hälftige Aufteilung**
    *   Fälligkeitsdatum 1: 10.07. = 50 €
    *   Fälligkeitsdatum 2: 10.09. = 150 €
    *   Fälligkeitsdatum 3: 10.10. = 100 €
    *   In diesem Beispiel ist nur das 1. Fälligkeitsdatum betroffen, an dem 100 € fällig wären. Dieser Betrag wird aufgeteilt, so dass die erste Hälfte (50 €) vor dem ursprünglichen Datum fällig wird. Die zweite Hälfte wird am 2. Fälligkeitsdatum zusammen mit dem ursprünglichen (Drittel-)Betrag fällig (50 €+100 €).
*   **Option 2: Verschiebung um einen Zeitbereich**
    *   Fälligkeitsdatum 1: 10.09. = 200 €
    *   Fälligkeitsdatum 2: 10.10. = 100 €
    *   In diesem Beispiel wird der Betrag zum 1. Fälligkeitsdatum auf das 2. Fälligkeitsdatum verschoben.
*   **Option 3: Entspricht Option 2 + Zuschlag**
    *   Fälligkeitsdatum 1: 10.09. = 201 € (200 € + 1%)
    *   Fälligkeitsdatum 2: 10.10. = 100 € (100 €)
    *   In diesem Beispiel wird der Betrag zum 1. Fälligkeitsdatum auf das 2. Fälligkeitsdatum verschoben und ein Zuschlag auf die verschobene Summe erhoben.

Der Kundenkalender ist in einer separaten Einheit beschrieben.
⇨ "Kundenkalender bearbeiten" auf Seite B-105

### Kalender

Um Dokumente erfassen zu können, muss im allgemeinen Kalender das aktuelle Kalenderjahr angelegt sein. Damit die Termine in der Auftragserfassung berechnet werden können, z. B. Liefertermine, müssen die täglichen Arbeitszeiten hinterlegt werden. Für diese Berechnungen müssen Wochenenden und Feiertage (ohne Arbeitsstunden) eingetragen werden.

Dazu können Sie auch Betriebsferien eintragen, indem Sie die Tagesarbeitszeit im Zeitraum der Ferien auf null setzen. Bei der Berechnung von Lieferterminen werden diese Tage berücksichtigt.

*Abb. B-38 Allgemeiner Kalender*
*A Anzahl der Betriebsstunden*
*B Änderungen übernehmen*

Auf dem allgemeinen Kalender baut der Kundenkalender auf. Dieser dient vor allem dazu, die Tage für die Zahlungsverschiebung pro Kunden zu hinterlegen.
⇨ "Kundenkalender bearbeiten" auf Seite B-105

### Zahlungsbedingungen

Die Zahlungsbedingungen eines jeden Kunden geben Sie in den Kundenstammdaten im Register **Finanzen** an. Im Auftragskopf werden die Zahlungsbedingungen aus den Kundendaten eingelesen und können überschrieben werden. Die Vorgaben zu den Berechnungen des Skontos legen Sie im Dialog **Zahlungsbedingungen** fest.

*Abb. B-39 Zahlungsbedingungen*
*A Definition Skonto*
*B Definition Zahlungsziele*

Sie können in einer Zahlungsbedingung mehrere Stufen einrichten, nämlich in vollständigen Sätzen mit bis zu fünf Zahlungszielen (B) und drei Prozentsätzen (A) für das Skonto. Daneben können Sie beliebig viele Bedingungen anlegen, die nur das Skonto berücksichtigen.

> **Beispiel**
> 
> | Skonto | Satz 1 | Tage 1 | Satz 2 | Tage 2 | Ziel 1 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| | 3,00% | 10 | 1,5% | 20 | 30 |
>
> In diesem Beispiel sehen Sie, dass der Kunde in den ersten 10 Tagen 3% Skonto abziehen kann, in den nächsten 10 Tagen aber nur noch 1,5%. Nach 30 Tagen ist die Rechnung ohne jegliche Abzüge fällig.

### Zahlungswege, Bonität

Zahlungswege und Bonität dienen der Information. Die Einträge werden in einfachen Basistabellen hinterlegt. Sie können beliebig erweitert werden.

*Abb. B-40 Zahlungswege, Bonität*

### Hauptkonto oder abweichende Rechnungsanschrift

Sie können die Kundennummer des Hauptdebitors (Filiale) eintragen, an den die Rechnungen und Gutschriften gesendet werden. Voraussetzung hierfür ist, dass dieser als Filiale des Kunden angelegt ist. Das Hauptkonto entspricht also der Kundennummer des Hauptdebitors. Wenn das Feld leer bleibt, wird automatisch die Nummer des aktuellen Kunden als Hauptkonto verwendet.

### Banken

Für den Zahlungsverkehr mit Ihren Kunden und Lieferanten hinterlegen Sie die Bankdaten.

*Abb. B-41 Bankdaten*
*A Bankleitzahl erforderlich für IBAN*
*B BIC für internationalen Zahlungsverkehr*
*C Länderkennzeichen erforderlich für IBAN*

Die Bank weisen Sie den Partnern in der Partnerverwaltung im Register **Finanzen** zu. In der Partnerverwaltung können Sie die IBAN errechnen lassen, wenn mindestens folgende Daten für die Bank hinterlegt sind: BLZ (A), Länderkennzeichen (C) und Kontonummer (in den Kundenstammdaten). Diese Funktion starten Sie in der Partnerverwaltung über das Menü **Funktionen**.

> **Bank der Firma und Mandanten**
> Die Bankverbindungen für Ihre Firma und Ihre Mandanten hinterlegen Sie im Menü **Stammdaten > Firma > Banken**. Dabei greifen Sie ebenfalls auf die Bankdaten zu, die unter Finanzen angelegt sind.

### Kreditlimit für Kunden

Sie können für jeden Kunden zwei unterschiedliche Werte für ein Kreditlimit festlegen und automatisch bei der Erfassung neuer Aufträge prüfen lassen. Das Kreditlimit 2 kann als hausinternes, nicht versichertes Kreditlimit genutzt werden.

Für die Prüfung des Kreditlimits müssen Sie folgende Entscheidungen treffen:

*   **Das Kreditlimit pro Kunde in den Kundendaten bestimmen.**
    *   **Kreditlimit 1:** Bei diesem Wert geben Sie das versicherte Kreditlimit an.
    *   **Kreditlimit 2:** Bei diesem Wert geben Sie ein internes (unversichertes) Kreditlimit an, das Sie aufgrund der Bonität des Kunden gewähren.
*   **Reaktion bei Überschreitung des Kreditlimits festlegen:**
    *   In der Regel wird der Status erhöht. Wenn das Kreditlimit überschritten wird, werden neue Aufträge auf einen definierten Status gesetzt und für die Bearbeitung gesperrt. Dieser Status kann manuell zurückgesetzt werden, um die Aufträge zur Bearbeitung freizugeben.
    *   Ein neuer Auftrag kann erfasst und gespeichert werden. Eine Meldung macht aber auf den Umstand aufmerksam, dass damit das Kreditlimit überschritten wird. Es liegt dann in Ihrer Entscheidung, den Auftrag weiter zu bearbeiten oder abzulehnen.

**Art der Prüfung**
In der Partnerverwaltung stellen Sie die entsprechenden Kennzeichen für jeden Kunden bzw. für jede Filiale individuell ein.

*   Keine Prüfung
*   Limit 1 + Meldung Limit 2
*   Limit 2 + Meldung Limit 1
*   Prüfung von Limit 1
*   Prüfung von Limit 1 und 2
*   Prüfung von Limit 2
*   Vorauskasse

Wenn Sie mit Filialen arbeiten, kann das Kreditlimit auf zwei Ebenen geprüft werden:

*   Das Kreditlimit der Filiale selbst wird geprüft.
*   Das Kreditlimit des Hauptkunden wird geprüft:
    *   Prüfung über das Filialkennzeichen
    *   Prüfung über den Eintrag im Feld Hauptkonto: Das Kreditlimit der Filiale wird ignoriert.

*Abb. B-42 Partnerverwaltung – Einstellungen zur Prüfung des Kreditlimits*
*A Einstellung bei Kunden mit Filialen*
*B Art der Prüfung*

**Anzeige des aktuellen Auftragsvolumens**

Im Auftragskopf wird der Betrag des Kreditlimits zusammen mit den offenen Posten angezeigt. Damit können Sie in jedem einzelnen Auftrag prüfen und ggf. mit dem Kunden absprechen, ob ein neuer Auftrag erfasst werden kann. In diesem Bereich werden die Daten jeweils nach der Übergabe an die FiBu und nach deren Rückmeldung aktualisiert.

*Abb. B-43 Kreditlimit und Saldo*
*A Kreditlimit*
*B Saldo*

**Keine Prüfung**

Wenn das Kreditlimit nicht geprüft wird, werden die aktuellen Beträge lediglich angezeigt. Bei der Überschreitung des Kreditlimits und bei Vorauskasse können die Aufträge grundsätzlich weiter bearbeitet werden. Angebote können unabhängig vom Kreditlimit und von möglichen Sperren erfasst werden.

**Rückmeldung von Offenen Posten**

Im Zusammenspiel mit einem Programm zur Finanzbuchhaltung (FiBu), das offene Posten zurückmeldet, erhalten Sie einen aussagekräftigen Überblick über den aktuellen Finanzstatus eines Kunden. Wenn Sie ohne OP-Rückmeldung arbeiten, werden bei der Prüfung des Kreditlimits bzw. des Saldos alle Aufträge berücksichtigt, die noch nicht an die FiBu übergeben wurden.

Wenn in den Firmendaten die Funktion **Einzel-OP-Rückmeldung** aktiviert ist, kann in der Auftragserfassung und der Kundenverwaltung eine OP-Abfrage für den jeweiligen Kunden gestartet werden. Dabei werden alle offenen Rechnungen angezeigt.

Kunden, deren Saldo seit dem letzten Einlesen der offenen Posten ausgeglichen wurde, werden mit dem Saldo 0 in der Kundenverwaltung aktualisiert.

### Überschreitung des Kreditlimits

Über die Firmendaten und die Statuszuordnung legen Sie fest, wie A+W Business bei der Überschreitung des Kreditlimits reagieren soll:

*   Über die Statuszuordnung ist ein Sperrstatus festgelegt, nach dem keine weitere Erfassung möglich ist.
*   Der Status wird nur erhöht, wenn die Option **Status erhöhen, wenn Kreditlimit überschritten** in den Firmenstammdaten aktiviert ist.

In der Kombination dieser beiden Einstellungen können keine neuen Aufträge erfasst werden, wenn das Kreditlimit erreicht oder überschritten wird.

Die Meldung **Kreditlimit ist überschritten, Kunde ist gesperrt!** wird auch vor dem Kopieren des Dokuments angezeigt. Der Kopiervorgang wird nicht durchgeführt. Das Kreditlimit wird auch dann geprüft, wenn in einem erfassten und gespeicherten Auftrag ein anderer Kunde eingetragen wird.

Wenn ein neuer Auftrag bearbeitet werden soll, obwohl das Kreditlimit überschritten ist, muss der Auftragsstatus manuell heruntergesetzt werden. Nach der manuellen Statusumsetzung wird der Status für diesen Auftrag nicht mehr automatisch hochgesetzt. Die Statusumsetzung ist ausführlich im Part Verkauf beschrieben.

Aufträge können vom Kunden über die EDI-Schnittstelle (elektronisch) übergeben werden. Wenn ein Auftrag dabei das Kreditlimit überschreitet, erhält es den Status **Auftrag gesperrt wegen Kreditlimit**. Er wird trotz des Sperrstatus in die Kapazitätsplanung eingelastet. Dieser Auftrag muss manuell freigegeben werden, indem der Status heruntergesetzt wird. Danach wird er automatisch an die Produktion übergeben.

Die Funktionen der Statuserhöhung lernen Sie ausführlich in einer separaten Einheit kennen.
⇨ Tutorial 2, "Statusverwaltung" auf Seite B-426

### Ablauf der Prüfung

*Abb. B-44 Prüfung des Kreditlimits*

Die manuelle Umsetzung des Status kann unterbunden werden, z. B. durch entsprechende Einstellungen in den Mitarbeiterrechten.

### Kreditlimit-Analyse

In der Kreditlimit-Analyse können Sie über einen beliebigen Zeitraum die Entwicklung von bestimmten Finanzdaten eines oder mehrerer Kunden oder Kundengruppen auswerten.

Im Einzelnen werden dabei das Kreditlimit, der Betrag der offenen Posten, das Obligo, Saldo 1, Saldo 2 und die Auftragsbestände betrachtet.

Dabei gilt folgende Hierarchie:
1.  Nicht gelieferte Aufträge
2.  Gelieferte und noch nicht fakturierte Aufträge
3.  Fakturierte, aber noch nicht an die FiBu übergebene Aufträge
4.  Summe aus den Beständen 1 bis 3

*Abb. B-45 Kreditlimit-Snapshot für einen Kunden*

Der Kreditlimit-Snapshot wird über einen täglich laufenden Task erzeugt, der die Finanzdaten auswertet. Wenn Sie diese Funktion nutzen wollen, wenden Sie sich bitte an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

### Währungen

Für Ihre Kunden können die Preise in den Aufträgen in der Fremdwährung ausgewiesen werden, die Sie ihm zugewiesen haben. Dazu müssen die Währungen und die entsprechenden Wechselkurse hinterlegt und gepflegt werden.

Zum Erfassen von Aufträgen kann A+W Business auf der Basis von zwei verschiedenen Währungseinstellungen arbeiten:

*   **Landeswährung (Eigenwährung):** Die Währung im Land Ihres Hauptsitzes. In Europa ist dies in der Regel der Euro.
*   **Fremdwährung:** Die von der Landeswährung abweichende Währung, in der z. B. im Auftrag die Preise für ausländische Kunden ausgewiesen werden.

Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von A+W Business umgerechnet.

Für die Pflege der Preise und für die Berechnungen in den Aufträgen ergeben sich folgende Möglichkeiten:

*   Die Preislisten und Aufträge werden in der Landeswährung geführt.
*   Die Preislisten werden in der Landeswährung geführt, für ausländische Kunden können die Beträge in den Aufträgen wahlweise in Landes- oder Fremdwährung angezeigt werden. Dazu müssen die Wechselkurse für die Fremdwährungen hinterlegt und gepflegt werden.
*   Die Preislisten werden in Fremdwährung geführt, in den Aufträgen können die Beträge wahlweise in Landes- oder Fremdwährung angezeigt werden. Für interne Zwecke wird der Wechselkurs hinterlegt.

In den Firmendaten legen Sie fest, welche Währung die Grundlage für Berechnungen ist und mit welcher Währung die Aufträge erfasst werden.

*Abb. B-46 Firmendaten - Register Steuer, Währungseinstellungen*
*A Währung, in der A+W Business rechnet*
*B Default-Einstellung für Auftragserfassung*
*C Währung der Preisanzeige im Auftrag*

In diesem Beispiel sehen Sie, dass die Eigenwährung (A) Euro ist. In der Regel wählen Sie als Standard-Einstellung (B) für die Erfassung von Aufträgen die Landeswährung. Wenn Sie mit Preislisten in einer anderen als der Landeswährung arbeiten, dann wählen Sie für die Anzeige der Preise (C) in der Auftragserfassung die Einstellung Euro.

#### Preisberechnung bei Fremdwährungen

Sie können in A+W Business die Preise für den Einkauf und für den Verkauf pflegen, auch wenn diese in unterschiedlichen Währungen anfallen.

Die Berechnung von Preisen kann bei Fremdwährungen zu unterschiedlichen Ergebnissen führen, wenn Mengenpreise auf unterschiedlichen Ebenen ermittelt werden. Diese Einstellung legen Sie in den Firmendaten fest.
⇨ Softwarereferenz, "Fremdwährungsbetrag aus Stückpreis x Menge bilden" auf Seite B-963

Wenn der Fremdwährungsbetrag auf der Basis der Stückliste und der Menge gebildet werden soll, können die Beträge auf folgende Arten errechnet werden.

*   **Der Positionspreis wird aus dem Positionspreis in Landeswährung gebildet:**
    *   LW Preis/PE x Faktor = FW Preis/PE
    *   LW Bruttostückpreis x Faktor = FW Bruttostückpreis
    *   LW Nettostückpreis x Faktor = FW Nettostückpreis
    *   LW Positionspreis x Faktor = FW Positionspreis
    *   *Legende: LW = Landeswährung, PE = Preiseinheit, FW = Fremdwährung*

*   **Der Positionspreis wird aus dem Nettostückpreis in Fremdwährung gebildet:**
    *   LW Preis/PE x Faktor = FW Preis/PE
    *   LW Bruttostückpreis x Faktor = FW Bruttostückpreis
    *   LW Nettostückpreis x Faktor = FW Nettostückpreis
    *   FW Nettostückpreis x Menge = FW Positionspreis
    *   *Legende: LW = Landeswährung, PE = Preiseinheit, FW = Fremdwährung*

### Skonto

A+W Business unterscheidet drei Berechnungsarten für das Skonto, die in den folgenden Beispielen dargestellt sind.

*   **Auf Bruttobetrag:**

| Berechnung | Berechnung/Basis | Wert |
| :--- | :--- | :--- |
| Netto 100,00 | 100,00 | 100,00 |
| MwSt. 19 % | | 19,00 |
| Brutto | 119,00 | 119,00 |
| Skonto 2 % | | 2,38 |

*   **Auf Nettobetrag (brutto vermindert um Skonto):**

| Berechnung | Berechnung/Basis | Wert |
| :--- | :--- | :--- |
| Netto 100,00 | | 100,00 |
| Skonto 2 % | 100,00 | 2,00 |
| | | 98,00 |
| MwSt. 19 % | 98,00 | 18,62 |
| Brutto | | 116,62 |

*   **Auf Nettobetrag:**

| Berechnung | Berechnung/Basis | Wert |
| :--- | :--- | :--- |
| Netto 100,00 | 100,00 | 100,00 |
| Skonto 2 % | | 2,00 |
| | | 98,00 |
| MwSt. 19 % | | 18,62 |
| Brutto | 98,00 | 118,62 |

### Einstellungen in den Firmendaten

Wenn der Status bei der Überschreitung des Kreditlimits umgesetzt werden soll, muss in den Firmendaten im Register **Parameter** die Checkbox (A) markiert sein.

*Abb. B-47 Firmendaten – Parameter*
*A Statuserhöhung für Kreditlimit*
*B Steuerberechnung*

In der Statuszuordnung muss zusätzlich festgelegt werden, ob die Auftragserfassung bei der Statuserhöhung gesperrt werden soll. Die Statuszuordnungen sind in einer separaten Einheit beschrieben.
⇨ Tutorial 2, "Statusverwaltung" auf Seite B-426

### Offene Posten

Für die Rückmeldung der offenen Posten (OP) müssen Sie in den Firmendaten neben dem eingesetzten FiBu-Programm auch die Einstellungen für die Aktualisierung prüfen.

*Abb. B-48 Firmendaten – Register FiBu*
*A Auswahl der FiBu-Schnittstellen*
*B Pfad für Rückmeldung*
*C Aktualisierung nach OP-Meldung*
*D Einzelabfrage pro Kunde*

### Finanzdaten des Kunden bearbeiten

Die folgende Handlungsanleitung baut auf den Schritten auf, die in der vorigen Einheit beschrieben wurden.

**So bearbeiten Sie die Daten für die Rechnungsstellung**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Finanzen**.

    *Abb. B-49 Partnerverwaltung – Zahlungsvereinbarungen*
    *A Modus der Fälligkeitsberechnung*
    *B Steuerberechnung aktivieren*
    *C Steuersatz auswählen*
    *D Kunden sperren*
2.  Prüfen Sie die Einstellung des Sperrkennzeichens (D). Wenn Sie die neuen Partnerdaten sofort verwenden wollen, müssen Sie die Einstellung **nicht gesperrt** wählen. Sie sollten die Daten dann sperren, wenn z. B. Preis- und Zahlungsvereinbarungen mit dem neuen Partner noch nicht abgeschlossen sind. In diesem Fall können noch keine Dokumente, d. h. Aufträge oder Bestellungen, für ihn erfasst werden.
3.  Legen Sie die Einstellungen für die Fälligkeiten (A) fest, die Sie mit diesem Partner vereinbart haben.
4.  Aktivieren Sie die Steuerberechnung (B) und wählen Sie den Steuersatz (C) aus.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

Die Daten werden gespeichert. Sie können jetzt die Daten für Vertreter oder für die Produktion hinzufügen.

⇨ "So legen Sie eine Filiale an" auf Seite B-65
⇨ "So legen Sie die Mitarbeiterdaten eines Marktpartners an" auf Seite B-66

### Allgemeinen Kalender anlegen

Für jedes neue Kalenderjahr müssen Sie die Feiertage und Betriebsferien eintragen, damit diese in der Auftragserfassung erkannt und bei der Terminberechnung berücksichtigt werden. Wenn Sie in Dokumenten das Datum eines Feiertags eintragen, wird die Meldung angezeigt, dass der gewählte Termin kein Arbeitstag ist.

**So legen Sie einen neuen Kalender an**

1.  Wählen Sie im Menü **Stammdaten > Allgemein > Kalender**.

    *Abb. B-50 Daten des aktuellen Kalenderjahrs*
    *A Wochentage übernehmen*
    *B Anzahl der Betriebsstunden*
    *C Jahreszahl*
    
    ⇨ Softwarereferenz, "Kalender" auf Seite B-568
2.  Markieren Sie die Checkboxen (A) für die Wochentage.
3.  Tragen Sie pro Wochentag die reguläre Arbeitszeit (B) ein, z. B. Montag bis Donnerstag je 8 Stunden, Freitag 6 Stunden.
4.  Tragen Sie im Feld **Jahr** (C) die neue Jahreszahl ein.

    *Abb. B-51 Daten für neues Kalenderjahr*
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Das Kalenderjahr wird angelegt und im Feld **Übersicht** angezeigt. Die Wochenenden werden in roter Schrift angezeigt. Als Nächstes sollten Sie Ihre Landesfeiertage und Betriebsferien eintragen.

    *Abb. B-52 Daten des aktuellen Kalenderjahrs*
    *A Betriebsstunden am Feiertag*
    *B Übersicht Kalenderjahr*
    *C Änderungen auf die Kalenderwoche übertragen*
    *D Kalenderwoche auswählen*
    *E Feiertag ohne Arbeitsstunden*
6.  Wählen Sie im Feld **KW** (D) die Kalenderwoche aus, z. B. die KW 40.
7.  Markieren Sie in der Übersicht (B) den Tag, den Sie als Feiertag definieren möchten, z. B. den 03.10.
8.  Markieren Sie die Checkbox (E) des zugehörigen Wochentages.
9.  Tragen Sie im Feld **Stunden** (A) den Wert 0 ein.
10. Klicken Sie auf **[auf KW übertragen]** (C). Die Arbeitszeit wird in der Übersicht für den Wochentag mit 0 Stunden angezeigt.
11. Wiederholen Sie die Schritte 6 bis 10 für alle Feiertage und für Ihre Betriebsferien.
12. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

Damit ist der allgemeine Kalender vollständig eingerichtet. Sie können jetzt Ihre Kundenkalender bearbeiten.
⇨ "Kundenkalender bearbeiten" auf Seite B-105

### Kundenkalender bearbeiten

Im Dialog **Kalender** legen Sie pro Kunde und Jahr die Urlaubszeiten fest, in denen keine Zahlungsziele berechnet werden sollen.

Die Berechnungen haben Sie bereits in der Einheit **Zahlungstagverschiebung** kennengelernt.
⇨ "Zahlungstagverschiebung" auf Seite B-85

> **Voraussetzung**
> Ein Kalenderjahr muss im allgemeinen Kalender angelegt sein, bevor Sie Kundenkalender für ein neues Jahr anlegen oder bearbeiten können.

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So legen Sie einen Kundenkalender mit Urlaubstagen an" auf Seite B-106
*   "So tragen Sie die Urlaubstage ein" auf Seite B-107
*   "So löschen Sie die Urlaubstage" auf Seite B-108
*   "So löschen Sie einen Kundenkalender" auf Seite B-108
*   "So kopieren Sie die Urlaubstage auf einen anderen Kunden" auf Seite B-109

**So legen Sie einen Kundenkalender mit Urlaubstagen an**

1.  Wählen Sie **Marktpartner > Kunde > Kalender**. Der Dialog **Kalender** wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. B-53 Felder für neuen Kundenkalender freigeschaltet*
    *A Kunde auswählen*
    *B Kalenderjahr auswählen*
3.  Wählen Sie den Kunden (A) und das Jahr (B) aus. Wenn das gewünschte Jahr nicht zur Auswahl angeboten wird, müssen Sie es zuerst im allgemeinen Kalender anlegen. Sie finden diesen unter **Stammdaten > Allgemein > Kalender**.
    ⇨ Softwarereferenz, "Kalender" auf Seite B-568
4.  Markieren Sie die Kalendertage, an denen keine Rechnungen fällig werden sollen. Wenn Sie noch keine Tage für eine Verschiebung festlegen wollen, markieren Sie ein beliebiges Datum, z. B. einen Sonntag.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert. Sie können jetzt weitere Urlaubstage eintragen oder einen weiteren Kundenkalender anlegen.

**So tragen Sie die Urlaubstage ein**

1.  Wählen Sie **Marktpartner > Kunde > Kalender**.
2.  Markieren Sie den Kunden, dessen Urlaubstage Sie eintragen wollen. Kalender aus dem vorherigen Jahr können Sie löschen, um die Liste übersichtlich zu halten. Die Beschreibung zum Löschen finden Sie in der nächsten Handlungssequenz.
3.  Prüfen Sie, ob das richtige Jahr eingestellt ist.
4.  Markieren Sie die Tage, an denen der Kunde Betriebsferien macht. Diese Tage sollen bei der Berechnung des Zahlungsziels übersprungen werden.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert. Die Tage, für die keine Zahlungsziele berechnet werden dürfen, sind markiert.

*Abb. B-54 Urlaubstage für Kunden*
*A Urlaubstage (Betriebsferien)*
*B Kalenderjahr prüfen*

**So löschen Sie die Urlaubstage**

1.  Wählen Sie **Marktpartner > Kunde > Kalender**. In der Tabelle werden pro Jahr alle Kunden aufgelistet, für die Urlaubstage eingetragen sind.
2.  Markieren Sie den gewünschten Kunden und suchen Sie in der Übersicht nach den Tagen, bei denen Sie die Markierung entfernen wollen.
3.  Entfernen Sie die Markierungen. Aus den Checkboxen ist das Häkchen entfernt.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

**So löschen Sie einen Kundenkalender**

1.  Wählen Sie **Marktpartner > Kunde > Kalender**. In der Tabelle werden pro Jahr alle Kunden aufgelistet, für die Urlaubstage eingetragen sind.
2.  Markieren Sie den gewünschten Kunden.
3.  Wählen Sie im Menü **Start > Löschen**. Eine Sicherheitsabfrage wird angezeigt.
4.  Beantworten Sie die Sicherheitsabfrage mit **[Ja]**. Die Daten werden gelöscht. In der Liste wird der alte Kundenkalender nicht mehr angezeigt.

**So kopieren Sie die Urlaubstage auf einen anderen Kunden**

1.  Wählen Sie **Marktpartner > Kunde > Kalender**. In der Tabelle werden pro Jahr alle Kunden aufgelistet, für die ein Kalender angelegt ist.
2.  Markieren Sie den gewünschten Kunden und suchen Sie in der Übersicht nach den Tagen, die Sie kopieren wollen. Nur die markierten Kalendertage werden übertragen. Wenn Sie den gesamten Kalender kopieren wollen, müssen Sie alle Tage markieren.
3.  Markieren Sie die Tage, die Sie kopieren wollen, indem Sie die gesamte Zeile markieren. Halten Sie Taste `<Strg>` gedrückt, um mehrere Tage zu markieren.
4.  Wählen Sie im Menü **Funktionen > Daten übertragen**. Der Dialog **Kalenderdaten übertragen** wird geöffnet.

    *Abb. B-56 Kunden auswählen*
    *A Markierte Urlaubstage übernehmen*
    *B Ziel-Kunde*
5.  Markieren Sie den Ziel-Kunden (B), auf den Sie die Urlaubstage übertragen wollen.
6.  Achten Sie darauf, dass die Checkbox **Zahlung auslassen** (A) markiert ist, damit die Urlaubstage übernommen werden.
7.  Klicken Sie auf **[OK]**, um die Übertragung zu starten.

Die markierten Tage werden auf den Kalender des Ziel-Kunden übertragen. Gleichzeitig wird für den Ziel-Kunden ggf. ein Kalender angelegt. Der Dialog **Kalender** wird wieder angezeigt.

*Abb. B-57 Urlaubstage beim Ziel-Kunden*

## Vertreter

**Lernziele**

*   Außendienst-Bereich anlegen.
*   Vertreter zuweisen.
*   Formen der Provisionsberechnung kennenlernen.

**Nutzen**

*   Die Provision wird automatisch berechnet, wenn im Auftrag angegeben ist, welche Vertreter zuständig sind, und wie hoch der Provisionssatz ist.

**Merke**

*   **Vertreter**: Nur die Mitarbeiter stehen als Vertreter zur Auswahl, denen ein Außendienstbereich (AD-Bereich) zugeordnet ist.
*   **Außendienstbereiche**: AD-Bereiche dienen folgenden Funktionen:
    *   Provisionsberechnung (Vertreterprovisionierung)
    *   Sortierkriterium in der A+W Business-Umsatzstatistik.
*   **Provision**: Details zur Provision und zur Berechnung legen Sie im Dialog **Vertreterprovision** fest.

### Außendienst

Die Provisionen Ihrer Mitarbeiter im Außendienst können nach unterschiedlichen Vorgaben abgerechnet werden. Dazu werden z. B. die zugeteilten Gebiete, die Warengruppen und die abgeschlossenen Aufträge herangezogen. Im Dokument muss jeweils der zuständige Vertreter angegeben werden.

Vertreter werden als Mitarbeiter angelegt. Zur Kennzeichnung eines Mitarbeiters als Vertreter wird dem Mitarbeiter ein Außendienstbereich zugeordnet.

**AD-Bereiche und Vertreter**

AD-Bereiche (Außendienstbereiche) dienen folgenden Funktionen:

*   Provisionsberechnung (Vertreterprovisionierung)
*   Sortierkriterium in der A+W Business-Umsatzstatistik.

Nur die Mitarbeiter stehen in den Dokumenten als Vertreter zur Auswahl, denen ein AD-Bereich zugeordnet ist.

*Abb. B-58 Außendienst-Bereiche*
*A Mitarbeiter, die als Vertreter tätig sind*
*B Bereich der Zuständigkeit*
*C Vorwahlbereich, z. B. für Kleinkunden*
*D Typ für Provisionssplit*

Alle Angaben außer dem Namen (A) sind nicht zwingend erforderlich. Wenn Sie keine Auswertungen nach Bereichen machen wollen, lassen Sie die Felder leer.

Sie können die AD-Bereiche nach Postleitzahlen (B) oder nach Vorwahlnummern (C) zuordnen. Diese Angaben werden bei der Auswertung der Aufträge für die Provision ausgewertet.

Die Angabe des Typs (D) legt fest, welcher Prozentsatz aus dem Dokument beim Provisionssplitting herangezogen wird.

### Vertreter zuweisen

Die dem Kunden zugewiesenen Vertreter werden standardmäßig vorgeschlagen, wenn für den Kunden ein Auftrag erfasst wird. Diese Angaben können pro Auftrag überschrieben werden.

**So weisen Sie dem Kunden einen Vertreter zu**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Vertrieb**.

    *Abb. B-59 Voreinstellungen der Vertreter in den Partnerdaten*
    *A Vertreter 1 und 2*
    *B Provisionsanteil für Vertreter 2*
    *C Liste der Angebote*
    *D Liste der Aufträge*
2.  Wählen Sie die Vertreter (A) aus, die für diesen Kunden zuständig sind. Wenn Sie in beiden Feldern einen Vertreter auswählen, sollten Sie auch angeben, wie die Provision verteilt werden soll (B). Wenn keine Vertreter zur Auswahl angeboten werden, können Sie die entsprechenden Daten anlegen.
3.  Klicken Sie ggf. auf das Ordner-Symbol, um den Dialog **Außendienst** zu öffnen.
4.  Klicken Sie auf **[Neu]**, um die nächste Zeile freizuschalten.

    *Abb. B-60 Außendienst-Mitarbeiter*
5.  Wählen Sie den Mitarbeiter aus, der für den Kunden zuständig ist. Sie können zusätzlich angeben, ob er standardmäßig als Vertreter 1 oder Vertreter 2 betrachtet werden soll.
6.  Klicken Sie auf **[Neu]**, um die Daten zu speichern. Die Daten werden gespeichert. Der Dialog wird geschlossen und die Partnerverwaltung wird wieder angezeigt. Sie können den neuen Vertreter jetzt in einem der Felder auswählen.
7.  Tragen Sie den Umsatzanteil (B) ein, an dem der Vertreter 2 beteiligt ist. Aus diesem Anteil wird die Provision errechnet.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert. Die Provision wird den Einstellungen entsprechend beim Archivieren berechnet.

## Produktion

**Lernziele**

*   Kundenspezifische Vorgaben für die Produktion festlegen.

**Nutzen**

*   Standardvorgaben für die Produktion bestimmter Scheiben können im Auftrag aus den Kundendaten übernommen werden. So müssen sie nicht immer wieder neu erfasst werden.

**Merke**

*   **Produktionsvorgaben**: Vorgaben für Sprossen und Abstandhalter werden automatisch in den Auftrag übernommen, wenn für den Kunden ein entsprechendes Produkt erfasst wird. Die Werte können im Auftrag jeweils angepasst werden.
*   **Entfernung**: Die Entfernung wird für die Berechnung der Fahrtkosten herangezogen. Dazu muss in der Tour eine Entfernungspauschale eingetragen sein.
*   **Flächenkapazitäten**: Für die drei Hauptproduktarten (ISO, VSG, ESG) können Gesamtkapazitäten hinterlegt und Anteile für die Hauptkunden (Keykunden) reserviert werden.

### Vorgaben für die Produktion

Pro Kunde können Sie bereits in seinen Stammdaten Vorgaben für die Produktion hinterlegen. Diese Vorgaben werden standardmäßig in den Auftrag übernommern, der für ihn erfasst wird, z. B. ein bestimmter Sprossentyp.

*Abb. B-61 Partnerverwaltung – Produktionsvorgaben*
*A Produktionskapazitäten*
*B Vorgaben für das Kunden-Logo*
*C Vorgaben für Abstandhalter*
*D Vorgaben für Sprossen*
*E Anzahl der Kilometer bis zur Lieferadresse*

Auf den Scheiben kann jeweils ein Logo aufgebracht werden. Die Angaben zum Logo (B) müssen auch in der Formularverwaltung hinterlegt werden.

Die Vorgaben für Sprossen (D) und Abstandhalter (C) werden automatisch in den Auftrag übernommen, wenn für den Kunden ein entsprechendes Produkt erfasst wird. Die Werte können im Auftrag jeweils angepasst werden. Sprossen und Abstandhalter lernen Sie ausführlich in der Einheit für die Produktverwaltung kennen.

Die Entfernung (E) wird für die Berechnung der Fahrtkosten herangezogen. Dazu muss in der Tour eine Entfernungspauschale eingetragen sein.

### Flächenkapazitäten

Für die drei Hauptproduktarten (ISO, VSG, ESG) können Gesamtkapazitäten hinterlegt werden. Von diesen Gesamtkapazitäten können Anteile für die Hauptkunden (Keykunden) reserviert werden. Diese Anteile werden in den Stammdaten des entsprechenden Kunden hinterlegt. Alle Kunden, für die keine eigenen Kapazitäten hinterlegt sind, werden in einer Gruppe zusammengefasst und mit der Restkapazität belegt.

Diese Angaben werden von dem Modul **Kapazitäts-Informationssystem** auf Kundenbasis ausgewertet.

*Abb. B-62 Kapazitätsinformationssystem*

In der Auftragserfassung können Sie sich über die Funktion **Kapazitätsinfo nach Kunde** anzeigen lassen, wann wie viel Kapazität für die Produktion frei ist. Diese Information bietet ledigliche einen groben Überblick darüber, ob der Terminwunsch für einen Auftrag erfüllt werden kann.

> **Kapazitäten sind nicht eingelastet**
> Die Anzeige gibt keine Auskunft über die aktuelle Kapazitätsplanung. Um die Auslastung der Maschinen zu prüfen, müssen Sie die Kapazitätsplanung starten und die Aufträge einlasten.

### Daten für die Produktion bearbeiten

Die folgende Handlungsanleitung baut auf den Schritten auf, die in der vorigen Einheit beschrieben wurden.

**So legen Sie die Kundenvorgaben für die Produktion fest**

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Kunden > Register Produktion**.

    *Abb. B-63 Partnerverwaltung – Produktion*
    *A Layout und Produktnummer des Kunden-Logos*
    *B Vorgaben für Abstandhalter*
    *C Vorgaben für Sprossen*
    *D Entfernung*
2.  Geben Sie die Entfernung bis zur Lieferadresse (D) ein.
3.  Legen Sie die Standard-Einstellung für den Abstandhalter (B) und die Sprossen (C) fest.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

### Übungen

*   Richten Sie für Ihren Kunden ein Kreditlimit ein. Sie werden später in der Auftragserfassung prüfen, wie die Daten angezeigt werden.
    *Überspringen Sie diese Übungen, wenn in Ihrer Installation nicht mit dem Kreditlimit gearbeitet wird.*
*   Legen Sie einen neuen allgemeinen Kalender an.
*   Richten Sie für Ihren Kunden einen Kundenkalender mit Urlaubstagen ein. Wählen Sie die Tage so zeitnah, dass Sie die Verschiebung der Rechnungsstellung prüfen können.
*   Weisen Sie Ihrem Schulungskunden 2 Vertreter zu. Legen Sie dazu den Vertreter 2 neu an.

Prüfen Sie, ob für einen Ihrer Schulungskunden folgende Angaben vorhanden sind und ergänzen Sie die Daten ggf.:

*   Der Kunde hat eine Filiale und zwei Mitarbeiter.
*   Die Rechnungsanschrift entspricht der Lieferanschrift.
*   Der Kunde wird mit der Tour Nord beliefert. Geben Sie die Distanz zwischen Ihrem Auslieferungslager und dem Lieferort an.
*   Geben Sie die Kommunikationswege an (Dokumentenversand).
*   Geben Sie die Zahlungsbedingungen und die Steuersätze an.
*   Legen Sie zusätzlich einen weiteren Kunden und zwei Lieferanten an, damit Sie für die folgenden Übungen etwas mehr Auswahl und Vergleichsmöglichkeiten haben.

## Ergänzende Daten für Partner

**Lernziele**

*   Kundenspezifische Preisdarstellung angeben.
*   Kundenspezifische (abweichende) Rundungen festlegen.
*   Lieferdauer berechnen und einstellen.
*   Objekte anlegen und zuordnen.

**Nutzen**

*   Partnerspezifische Vorgaben erleichtern die Erfassung von Dokumenten.
*   Dokumente für Kunden und Lieferanten können sich auf dasselbe (Bau-)Objekt beziehen.

**Merke**

*   **Parameter**: Sie können festlegen, wie die Preise im Auftrag bei bestimmten Produkten oder Warengruppen dargestellt werden.
*   **Lieferdauer**: Die Lieferdauer ist die Zeit, die der Lkw vom Werk bis zum Kunden unterwegs ist. Sie wird pro Tour und Kunde festgelegt. Die Lieferdauer wird in der Auftragserfassung bei der Berechnung des Produktionstermins berücksichtigt.
*   **Rundungen**: Zur Berechnung von Rundungen werden zwei unterschiedliche Werte herangezogen:
    *   Die Anzahl der Stellen und die Rundungsart, z. B. nach oben oder nach unten.
    *   Der Rundungspunkt gibt an, was gerundet werden soll, z. B. der Zuschlag.
*   **Objekte**: Objekte sind konkrete Bauvorhaben oder Projekte, an denen Kunden und Lieferanten beteiligt sein können. An Objekte können besondere Konditionen gebunden sein, z. B. spezielle Preise oder Rabatte, die im Auftrag automatisch zur Preisberechnung herangezogen werden, wenn das Objekt zugewiesen ist.

### Auftragsparameter

Für die Erfassung von Aufträgen können Sie festlegen, wie die Preise dargestellt werden, wenn Sie ein bestimmtes Produkt oder eine bestimmte Warengruppe ausgewählt haben. Diese Einstellungen gelten jeweils für einen Kunden oder für eine Kundengruppe.

*Abb. B-64 Kunde - Auftragsparameter*
*A Kundengruppe*
*B Warengruppe*
*C Cursor-Position*
*D Preisdarstellung*

In diesem Beispiel sehen Sie, dass für die gewählte Kundengruppe (A) immer dann die Preise explizit (D) angezeigt werden, wenn ein Produkt der gewählten Warengruppen (B) erfasst wird.

Für die Erfassung von Bestellungen können Sie entsprechende Einstellungen unter **Lieferant > Parameter** festlegen.

### Lieferdauer

Die Lieferdauer wird pro Tour festgelegt. In der Regel wird eine Tour an einem Tag gefahren. Bei längeren Anfahrtszeiten können entsprechende Touren angelegt werden. Die eingetragene Lieferdauer wird in der Auftragserfassung bei der Berechnung des Produktionstermins berücksichtigt.

> **Beispiel**
> *   Versandtag: Tag der Warenausgabe an Fahrer
> *   Anlieferung: Liefertermin = Ankunftstag der Ware beim Kunden
> *   Lieferdauer: 3 Tage
>
> In diesem Beispiel muss der Auftrag am 18.05. fertig gemeldet werden.

Die Lieferdauer legen Sie im Dialog **Lieferdauer** fest.

*Abb. B-65 Lieferdauer für Kunden*
*A Tour*
*B Rangfolge*
*C Lieferdauer*

In diesem Beispiel sehen Sie, dass einige Kunden mit derselben Tour (A) beliefert werden. Für diese ist die Lieferdauer (C) identisch, aber die Reihenfolge, in der sie beliefert werden, ist unterschiedlich (B).

### Rundungen

Errechnete Werte für Preise, Steuern und Flächen werden in aller Regel gerundet. Rundungen werden in zwei Formen verwaltet:

*   Standardzuordnungen
*   Abweichende Rundungen bei bestimmten Produkten für Kunde/Lieferant oder Kundengruppe/Lieferantengruppe

*Abb. B-66 Rundungen für Kunden*

In diesem Beispiel sehen Sie, dass für einen Kunden der Glaspreis bei ISO-Scheiben gerundet werden soll.

Zur Berechnung von Rundungen werden zwei unterschiedliche Werte herangezogen. Zum einen die Rundung selbst, also die Anzahl der Stellen und die Rundungsart. Zum anderen der Rundungspunkt, also was gerundet werden soll.

Zur Berechnung von Rundungen werden folgende Einstellungen herangezogen:

*   **Stammdaten > Auftrag > Rundung** = Rundungswert, Stellen und Rundungsart
*   **Stammdaten > Auftrag > Rundungspunkte** = welche Berechnungsgröße kann gerundet werden
*   **Stammdaten > Auftrag > Rundungszuordnung** = welcher Rundungspunkt wird mit welcher Rundung berechnet

Diese Einstellungen werden ausführlich im Tutorial 2 behandelt.
⇨ Tutorial 2, "Rundungen" auf Seite B-449

### Objekte

Objekte sind konkrete Bauvorhaben, an denen Kunden und Lieferanten beteiligt sein können. A+W Business kann eine Fülle von Objektinformationen verwalten. Dazu gehören besondere Konditionen, z. B. spezielle Preise oder Rabatte, die im Auftrag automatisch zur Preisberechnung herangezogen werden, wenn das Objekt zugewiesen ist.

> **Voraussetzung**
> A+W Business bietet unterschiedliche Modi für die Objekt- und Abrechnungsverwaltung an. Objekte können nur mit einer der Objektverwaltungen angelegt und bearbeitet werden. Eine ausführliche Beschreibung zu den Modi finden Sie im Tutorial 2.
>
> ⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-502

Sie legen die Rahmenbedingungen für das Objekt fest, z. B. zeitliche Eingrenzungen. Nach Ablauf der Gültigkeit kann das Objekt im Dokument nicht mehr zugewiesen werden.

Die Werte für veranschlagte Auftragssummen oder Mengen werden nicht geprüft. Durch die spezifischen Übersichten für Kunden und für Lieferanten können Sie sich die zugeordneten Aufträge, Bestellungen und Mengen anzeigen lassen und so die verkauften Mengen im Blick behalten.

*Abb. B-67 Zuordnung von Objekten zu Partnern*

In diesen Beispielen sehen Sie, wie sich die Einstellungen und Konditionen bei Kunden- und Lieferantenobjekten unterscheiden können.

Eine detailliertere Beschreibung finden Sie in der Einheit Abrechnungsverwaltung.
⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-502

### Objekt anlegen und zuweisen

Um mit Objekten zu arbeiten, sind drei Schritte erforderlich:

*   In den Firmendaten muss der richtige Modus für die Objektverwaltung eingestellt sein.
*   Objekte werden zunächst in einfachen Basistabellen angelegt, wie Sie es in der Einheit zu den Basistabellen kennengelernt haben. Den Dialog finden Sie unter **Marktpartner > Allgemein > Objekte**.
    *Abb. B-96*
    ⇨ "Basistabelle erweitern" auf Seite B-34
*   Objekt den Kunden und/oder Lieferanten zuordnen. Dabei können Sie ein Objekt einem oder mehreren Kunden bzw. Lieferanten zuordnen. Für jeden Kunden bzw. Lieferanten geben Sie Höchstwerte für Betrag, Fläche und Stück an. Außerdem können Sie objektbezogen Preise und Konditionen anlegen.

> **Voraussetzung**
> A+W Business bietet unterschiedliche Modi für die Objekt- und Abrechnungsverwaltung an. Objekte können nur mit einer der Objektverwaltungen angelegt und bearbeitet werden. Eine ausführliche Beschreibung zu den Modi finden Sie im Tutorial 2.
>
> ⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-502

**So prüfen Sie den Modus der Objektverwaltung**

1.  Wählen Sie Menü **Stammdaten > Firma > Firmendaten**
2.  Wechseln Sie zum Register **Dokumente**.

    *Abb. B-68 Objektverwaltung aktivieren*
    *A Firmendaten – Dokumente*
    *B Modus der Objektverwaltung*
3.  Wählen Sie den Modus **Standard Objektverwaltung**. In diesem Modus können Sie Objekte anlegen und zuordnen.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

**So weisen Sie einem Kunden ein Objekt zu**

1.  Wählen Sie Menü **Stammdaten > Marktpartner > Kunde > Objekte**. Der Dialog **Objekte** wird angezeigt. Die Anzeige der Register ist von der aktivierten Objektverwaltung abhängig.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. B-69 Felder für neues Objekt freigeschaltet*
    *A Objekt*
    *B Kunde*
    *C Zeitraum, in dem zu diesem Objekt Aufträge erfasst werden können.*

    In diesem Beispiel ist die Standard-Objektverwaltung aktiviert.
    ⇨ Softwarereferenz, "Objekte (Kunde, Lieferant)" auf Seite B-833
3.  Wählen Sie das Objekt (A) und den Kunden (B) aus.
4.  Tragen Sie ggf. einen Zeitraum (C) für die Gültigkeit ein. Die Gültigkeit wird in der Auftragserfassung geprüft. Das Objekt wird nicht mehr zur Auswahl angeboten, wenn die Gültigkeit abgelaufen ist. Die Objektverwaltung ist in einer separaten Einheit beschrieben.
    ⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-502
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert. Für den Kunden kann nun ein Auftrag zu diesem Objekt erfasst werden.

### Übungen

*   Tragen Sie für Ihre Kunden die Lieferdauer ein.
*   Legen Sie ein Objekt an und ordnen Sie es Ihrem Kunden zu. Wenn Sie keine Objekte anlegen können: Welche Einstellung müssen Sie ändern?

**Ergänzende Informationen**
⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-502
⇨ Softwarereferenz, "Objekte" auf Seite B-762
⇨ Softwarereferenz, “Lieferdauer (Kunde, Lieferant)" auf Seite B-832
⇨ Softwarereferenz, "Objekte (Kunde, Lieferant)" auf Seite B-833
⇨ Softwarereferenz, "Objekte - Dokumente" auf Seite B-846
⇨ Softwarereferenz, “Forderungsberechnung" auf Seite B-849
⇨ Softwarereferenz, "Forderungs-Historie" auf Seite B-850
⇨ Softwarereferenz, "Abweichende Kunden-, Lieferantengruppen" auf Seite B-855

## Lieferantendaten

In diesem Themenblock lernen Sie, wie Sie die Stammdaten für Lieferanten einrichten.

Dazu gehören folgende Lerneinheiten:

*   "Lieferantenspezifische Daten" auf Seite B-131

Neben den Lieferantendaten, die in diesem Themenblock beschrieben werden, legen Sie weitere Daten zu Ihren Lieferanten an. Dazu stehen im Menü **Lieferant** folgende Dialoge zur Verfügung:

*   Lieferanten
*   Lieferantenrabatte
*   Parameter
*   Lieferdauer
*   Objekte
*   Rundung
*   Rundung Lieferantengruppe
*   Abweichende Lieferantengruppen

Diese Daten legen Sie in derselben Weise an, wie die Daten für Kunden.
⇨ "Kundendaten" auf Seite B-36
