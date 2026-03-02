---
description: "DE_AWBusiness_Fertigung_5_4"
---


---
## Tutorial: Zusatzfunktionen

- Die Kiste wurde in den Auftrag übernommen und z. B. mit der Positionsmenge 3 gespeichert:

*(Screenshot: Abb. E-71 Positionsmenge 3 gespeichert)*

- Im Lager wurden 3 zusätzliche Reservierungen auf die Dummy-Kiste gebucht:

*(Screenshot: Abb. E-72 Reservierung)*
**A**: Reservierungen auf Dummy-Kiste um 3 erhöht

- Im Buchungsjournal (Lagerwirtschaft) ist die Positionsmenge als reserviert gekennzeichnet:

*(Screenshot: Abb. E-73 Position des Auftrags ist reserviert)*

Als nächstes sollen Kisten mit ID zugewiesen und nach dem Druck des Lieferscheins ausgebucht werden.

### So buchen Sie den Warenausgang von Kisten

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Warenausgang Kisten**.
    *(Screenshot: Abb. E-74 Warenausgang-Kiste – Kundenauftrag aufrufen)*

2.  Wählen Sie die Option **nach Scanner**.

3.  Erfassen Sie den Barcode der Auftragsnummer und der Positionsnummer. Die Nummern werden in den Feldern **Dokument** angezeigt.
    Wenn Sie nicht mit einem Scanner arbeiten, wählen Sie die Option **nach Auftragsnummer** und geben die Nummer ein.

4.  Wählen Sie im Menü **Start > Ausführen**, um die Auftragsdaten einzulesen. Die Anzeige wechselt zum Register **Identnummern**.
    *(Screenshot: Abb. E-75 Auftragsposition mit Unterpositionen)*

    Jede Kiste wird in einer eigenen Zeile als virtuelle Position angezeigt. Die Felder in der Spalte **Identnummer** sind leer, da noch keine Kiste mit ID zugewiesen wurde.

5.  Scannen Sie die Kisten-ID der ersten Kiste, die reserviert werden soll.
    Wenn Sie nicht mit einem Scanner arbeiten, wählen Sie im Feld **Identnummer** eine der angezeigten IDs aus. Nur Kisten-IDs von Kisten des erfassten Typs werden angezeigt.

6.  Wählen Sie im Menü **Start > Ausführen**, um die Kiste zuzuordnen.
    Die ID wird der ersten virtuellen Position zugeordnet. Gleichzeitig erhält die Zeile eine virtuelle Positionsnummer. Die Markierung springt in die nächste Zeile.

*(Screenshot: Abb. E-76 Unterposition mit zugewiesener Kisten-ID)*
**A**: Virtuelle Positionsnummer
**B**: ID ist zugewiesen

Damit ist die Reservierung von der Dummy-Kiste gelöscht und stattdessen die zugewiesene Kiste mit ID reserviert. Die beiden anderen Kisten sind immer noch auf die Dummy-Kiste reserviert.

Im Buchungsjournal wird dies ebenfalls angezeigt:

*(Screenshot: Abb. E-77 Reservierung von Dummy-Kiste aktualisiert)*
**A**: Verbleibende Dummy-Reservierungen
**B**: Virtuelle Position mit zugewiesener Kiste (ID)

7.  Wiederholen Sie die Schritte 5 und 6, um weitere Kisten mit ID zuzuordnen.

*(Screenshot: Abb. E-78 Kisten vollständig zugewiesen)*

Zu jeder Kiste wird eine fortlaufende virtuelle Positionsnummer angezeigt. Allen Positionen ist jetzt eine bestimmte, im Lager vorhandene, Kiste mit ID zugeordnet.

Diese tatsächlichen Kisten sind damit im Lager reserviert, was Sie z. B. im Buchungsjournal prüfen können:

*(Screenshot: Abb. E-79 Buchungsjournal – Reservierte Kisten)*

Die virtuellen Positionsnummern werden in den Auftrag zurückgeschrieben.

*(Screenshot: Abb. E-80 Unterpositionen im Auftrag)*

Im Dialog Lagerinfo sind die drei Kisten als Reservierung gekennzeichnet. Damit ist für den Erfasser eines Auftrags deutlich, dass diese Kisten nicht in einen anderen Auftrag übernommen werden können. Die Reservierungen wurden von der Dummy-Kiste storniert.

*(Screenshot: Abb. E-81 Reservierung in der Lagerinfo aktualisiert)*
**A**: Reservierung der Dummy-Kiste zurückgesetzt
**B**: Im Warenausgang Kiste gesetzte IDs
**C**: Reservierungen auf echte Kisten eingetragen

Je nach Einstellung werden die Kisten aus dem Bestand ausgebucht, wenn der Lieferschein oder die Rechnung gedruckt wird. Die ausgebuchten Kisten werden im Dialog Lagerinfo nicht mehr angezeigt:

*(Screenshot: Abb. E-82 Ausgebuchte Kisten werden in der Lagerinfo nicht angezeigt.)*

### Übungen

*   Erfassen Sie einen Auftrag mit Kisten.
*   Prüfen Sie im Dialog Lagerinfo die Reservierung und den Bestand der Kiste.
*   Erfassen Sie den Warenausgang der Kisten und vergleichen Sie anschließend, wie sich der Lagerbestand geändert hat.

### Ergänzende Informationen

⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-925
⇨ Stammdaten, "Virtuelle Positionsnummern verwenden" auf Seite B-931
⇨ Verkauf, "Lagerinfo" auf Seite C-731
⇨ Softwarereferenz, “Warenausgang" auf Seite E-237

## Gestellverwaltung

Mit A+W Business können Sie sowohl eigene als auch Fremdgestelle verwalten. Übersichten zeigen den aktuellen Bestand inkl. Außer-Haus-Gestellen und deren Rückgabetermin an.

### L-Gestellbelegung

Die Zusatzfunktion L-Gestellbelegung wird pro Kunde aktiviert. Außerdem können dazu eigene Zuschläge für L-Gestelle berechnet werden.

Bei der Nutzung der Funktion muss für den jeweiligen Kunden die Bock- und Fachnummer ermittelt werden. Hierzu werden die entsprechenden Auftragsnummern in einem Nummernverwalter zusammengestellt.

Eine Position kann über mehrere L-Gestelle verteilt werden. Dabei müssen die Restriktionen für L-Gestelle beachtet werden.

Das Programm ermittelt pro Position jeweils die Start- und Endenummer.

**Beispiel**
> 0101 = Gestell 1, Fach 1
>
> 0315 = Gestell 3, Fach 15

Das Ergebnis wird in der Übergabe-Datei in das Feld Kommission geschrieben. Hierzu werden die Start- und Endenummer dem Kommissionsfeld vorangestellt:

`0101-0421 + Kommissionsfeld aus Auftrag (bis maximale Feldlänge).`

Für die Aufträge werden dann Etiketten gedruckt und eine Liste der L-Gestellbelegung pro Auftrag. Die Information, ob eine Position auf einem L-Gestell verpackt werden kann, wird auch an den Formulardruck übergeben.

Außerdem werden die Daten in einer ASCII Datei gespeichert. Der Name der ASCII-Datei besteht aus der Kundennummer, Tag und Monat.

Für TPS und nicht TPS Positionen gibt es unterschiedliche Restriktionsprüfungen. Welcher Artikel zur Prüfung zu verwenden ist, ergibt sich aus der Zuordnung zu dem Abstandhalterartikel.

Geprüft wird:
*   **TPS**
    *   Maximales Maß 1100 x 1700
    *   Max. Einbaustärke 26 mm
    *   Anzahl Fächer: 22
*   **Nicht TPS**
    *   Maximales Maß 1080 x 1960
    *   Max. Einbaustärke 99 mm
    *   Anzahl Fächer: 21

Im Falle einer Restriktionsverletzung, wird der Text `SEPA/ + Kommission` übergeben. Falls eine Position nicht auf L-Gestell verpackt werden kann, wird kein Datensatz geschrieben.

### Gestellverwaltung

Zur A+W Business-Gestellverwaltung gehört die Verwaltung der Gestelle nach Typ und Nummer. Sie definieren pro Gestell dessen Eigenschaften, z. B. verfügbar, gesperrt, verloren, stationär, Fremdgestell, Anzahl Latten, Räder. Für das Mahnwesen legen Sie den Mietsatz und die Anzahl an kostenfreien Tagen fest.

Wird ein Gestell an einen Kunden ausgeliefert, tragen Sie in der Ausgangsbuchung das Ausgangsdatum, die Nummer des Lieferscheins und die Kundennummer ein. Die Rückkehr des Gestells buchen Sie über das Eingangsdatum. Das Gestell ist somit wieder für die Auslieferung verfügbar.

Mit Hilfe des Mahnwesens können Sie alle auswärtigen Gestelle anmahnen. Sie geben an, wie viel Tage das Gestell mindestens auswärtig sein muss, um die Auswahl für die Mahnung einzugrenzen. Sie erhalten dann automatisch eine Liste aller anzumahnenden Kunden. A+W Business kann unterschiedliche Mahnstufen unterscheiden.

### Fremdgestelle

Neben den eigenen Gestellen können Sie auch die Gestelle von Kunden und Lieferanten verwalten, die Ihnen zur Verfügung stehen.

Daneben können Sie in der Kundenkommission Details zu Standorten oder Abladeorten von (regelmäßigen) Lieferungen hinterlegen.

### BDE Gestellrückmeldung

Ihre mit Barcode-Etiketten versehenen Gestelle werden vor dem Versand bzw. nach ihrer Rückkehr per Barcode-Scanner erfasst. Diese Daten werden in A+W Business eingelesen und entsprechend verbucht. A+W Business verfügt dadurch immer über aktuelle Informationen, welche Gestelle wieder für den Versand zur Verfügung stehen und welche sich noch beim Kunden befinden.

### Gestellhistorie

Die Belegung eines Gestells wird in der Historie festgehalten, sodass Sie zurückverfolgen können, wann ein Gestell an wen ausgeliefert und zurückgemeldet wurde.

In der Gestellverwaltung können Sie Ihre Gestelle nach Gestellart und Gestellnummer organisieren. Versand und Erhalt der Gestelle dokumentieren Sie über die Ein-/Ausgangsbuchungen.

## Fertigungsvorschau

Der Dialog Fertigungsvorschau zeigt pro Liefertermin zu den Produktarten Isolierglas, Einfachglas, ESG und VSG die Summe der entsprechenden Aufträge an. Dazu werden alle Aufträge mit Liefertermin größer gleich dem aktuellen Tagesdatum ausgewertet.

Pro Liefertermin stehen 50 Spalten zur Verfügung, die individuell eingestellt werden können. Die Festlegung welcher Inhalt in welcher Spalte angezeigt werden soll, wird firmenübergreifend durch den Systemadministrator festgelegt. Die Auswertungskriterien sind jeweils eine Kombination von Produktart und Produktgruppe. Das Ergebnis kann sowohl in Stück als auch in qm dargestellt werden.

Die sichtbaren Spalten können für jede Produktart und für extra Zuordnungen pro Arbeitsplatz eingestellt werden. Auch die Spaltenbreite lässt sich pro Arbeitsplatz individuell einstellen.

### Prinzip der Vorschauspalten

In der Kombination der Spalten Typ HP und Typ 0 können folgende Kombinationen definiert werden:

| Kombination | Beispiel |
| :--- | :--- |
| Produktart/Produktart | Isolierglas/Isolierglas |
| Produktart/Produktgruppe | Einfachglas/Ornament |

Mit der Kombination der Spalten Typ 0 und Nr. 0 kann das Hauptprodukt auch in der Stückliste gesucht werden.

Mit der Kombination der Spalten Typ 1 und Nr. 1 wird auf der Stücklistenebene gesucht.

| Spalte | Kombination |
| :--- | :--- |
| Typ 1 | Typauswahl auf Basis 1. Stücklistenebene |
| Nr. 1 | Produktart/Produktgruppe je nach Typ |

Mit der Kombination der Spalten Typ 2 und Nr. 2 wird nach einem Produkt oder einer Bearbeitung in der Stückliste gesucht, z. B. in VSG nach ESG oder Einfachglas, Ornament, Modell usw.

| Spalte | Kombination |
| :--- | :--- |
| Typ 2 | Typauswahl auf Basis 2. Stücklistenebene |
| Nr. 2 | Produktart/Produktgruppe je nach Typ |

**Beispiel:** Konfiguration für Auswertung von Einfachglas

*(Screenshot: Abb. E-83 Definition für Einfachglas)*
- **A Typ HP:** 1=Produktart
- **B HP:** Produktart Schlüsselnr. 1=Einfachglas
- **C ST/QM (Darstellung der Menge):** 1=Stück, 2=Quadratmeter
- **D Typ 0:** Suche in der Stückliste nach 1=Produktart
- **E Nr 0:** Produktart Schlüsselnr. 1=Einfachglas
- **F Typ 1 (Stückliste):** 1=Produktart
- **G Nr 1:** Produktart Schlüsselnr. 20=Bearbeitungen

In Zeile 30 ist die Selektion so gewählt, dass alle Einfachgläser ohne weitere Einschränkung angezeigt werden.
Die Definitionen in Zeile 30 und 31 unterscheiden sich nur in der ausgewählten Maßeinheit für die Anzeige (qm bzw. Stück).
In Zeile 32 und 33 wird die Selektion von Einfachglas auf ausschließlich Ornamente eingegrenzt und keine weiteren Veredelungen berücksichtigt.
In Zeile 33 und 34 liegt der Schwerpunkt der Analyse auf der Bearbeitung und in Zeile 35 und 36 auf der Modellinformation.

*(Screenshot: Abb. E-84 Fertigungsvorschau für Einfachglas)*
Als Ergebnis der beschriebenen Einstellung werden in der Auswertung die Einfachgläser pro Datum angezeigt.

---

## Softwarereferenz

## A+W Business

### Übersicht

Im Modul **Fertigung** können Sie die Aufträge an die Produktion übergeben und den Versand steuern und überwachen.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   "Produktion" auf Seite E-169
*   "Barcode-Übergabe" auf Seite E-193
*   "Produktionsdaten" auf Seite E-198
*   "Lieferwesen" auf Seite E-203
*   "Tourenliste" auf Seite E-204
*   "Statusmeldung" auf Seite E-216
*   "Kommissionierung" auf Seite E-226
*   "Listendruck" auf Seite E-233
*   "Warenausgang Kisten" auf Seite E-237
*   "Gestellverwaltung" auf Seite E-253
*   "Gestelle" auf Seite E-238
*   "Terminübersicht" auf Seite E-267
*   "Zollverwaltung" auf Seite E-282
*   "Angebotsoptimierung" auf Seite E-290
*   "Versandsteuerung" auf Seite E-290

Im Modul **Fertigung** werden auch die Dialoge zur Kapazitätsplanung angezeigt. Diese Dialoge werden im Part **Kapazitätsplanung** beschrieben.

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass einige Dialoge und Funktionen zum Modul **Fertigung** in **A+W Business** aus unterschiedlichen Modulen heraus gestartet werden können. In dieser Anleitung werden sie jedoch nur einmal beschrieben. Sie finden an den entsprechenden Stellen aktive Querverweise, über die Sie direkt zu der zugehörigen Beschreibung springen können.

#### Nummernverwalter
- **Fertigung > Produktion > Nummernverwalter**
- **Fertigung > Lieferwesen > Nummernverwalter**
- **Fertigung > Terminübersicht > Nummernverwalter**
- **Fertigung > Zollverwaltung > Nummernverwalter**
- **Fertigung > Angebotsoptimierung > Nummernverwalter**

Der Dialog Nummernverwalter ist im Part Verkauf beschrieben.
⇨ Verkauf, "Nummernverwalter" auf Seite C-624

#### Formular-/Etikettendruck
- **Fertigung > Produktion > Formular**
- **Fertigung > Lieferwesen > Formular**
- **Fertigung > Zollverwaltung > Formular**

Der Dialog Formular-/Etikettendruck ist im Part Verkauf beschrieben.
⇨ Verkauf, "Formular-/Etikettendruck" auf Seite C-633

#### Dokumentendaten
- **Fertigung > Dokumentendaten**

Der Dialog Dokumentendaten ist im Part Verkauf beschrieben.
⇨ Verkauf, "Dokumentendaten" auf Seite C-727

#### Artikel-Info
- **Fertigung > Artikel-Info**

Der Dialog Artikelinfo ist Part Verkauf beschrieben.
⇨ Verkauf, "Artikel-Informationen" auf Seite C-595

#### Faxnachrichten
- **Fertigung > Faxnachrichten**

Der Dialog Faxnachrichten ist im Part Überblick beschrieben.
⇨ Überblick, "Standard-Menüs" auf Seite A-53

## Produktion

**Fertigung > Produktion**

Produktionsaufträge können automatisch oder manuell an die Produktion übergeben werden. In der Regel werden die Aufträge in einen Nummernverwalter gestellt und im Dialog Produktionsübergabe an die Produktion übergeben. Sie können jedoch auch einzeln gescannt und per Barcode übergeben werden.

> **Automatische Übergabe**
> Die automatische Produktionsübergabe und das Abfrage-Intervall müssen in einem Workflow-Task als Formel eingerichtet sein.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Übergabe Produktion" auf Seite E-170
*   "Einstellungen Produktionsübergabe" auf Seite E-174
*   "Modellliste" auf Seite E-187
*   "Gestellbelegung prüfen" auf Seite E-188
*   "Einstellungen (Gestellbelegung prüfen)" auf Seite E-190
*   "Produktionsdaten (Dialog)" auf Seite E-198

**Ergänzende Informationen**
⇨ "Barcode-Übergabe" auf Seite E-193
⇨ "Produktionsdaten" auf Seite E-198

### Übergabe Produktion

**Fertigung > Produktion > Übergabe Produktion**

*(Screenshot: Abb. E-85 Produktionsübergabe)*

In diesem Dialog übergeben Sie die Aufträge aus einem Nummernverwalter an die Produktion. Die Übergabe starten Sie mit [OK]. Die Daten werden in eine XML-Datei geschrieben, die von A+W Production eingelesen werden kann.

Für die automatische Produktionsübergabe und den Abfrage-Intervall müssen Sie einen Workflow-Task einrichten. Eine Beschreibung dazu finden Sie im Tutorial.
⇨ Tutorial, "Produktionsübergabe mit A+W Business Kapazitätsplanung" auf Seite E-43

> **Übergabe von Angeboten**
> Angebote können über **Fertigung > Angebotsoptimierung > Übergabe Produktion** zur Optimierung an die Produktion übergeben werden. Der Dialog unterscheidet sich nicht von demjenigen für die Übergabe der Aufträge. Allerdings müssen die Einstellungen für die Übergabe von Angeboten getrennt eingerichtet werden.

#### Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
*   **Historie:**
    Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments.
    ⇨ Verkauf, "Historie" auf Seite C-550
*   **Einstellungen:**
    Öffnet den Dialog Einstellungen-Produktionsübergabe, in dem Sie die Einstellungen für die Datenübergabe festlegen.
    ⇨ "Einstellungen Produktionsübergabe" auf Seite E-174

#### Identifikation

- **Mandant**: Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.
- **Bereich**: Wenn in der Produktion mit verschiedenen Bereichen gearbeitet wird, können Sie denjenigen auswählen, an den die Aufträge übergeben werden sollen. Die Angabe wird für die Auswahl des Nummernkreises herangezogen, aus dem die Laufnummer für die Übergabe gezogen wird.
- **Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter**: Wenn Sie einen Nummernverwalter ausgewählt haben, werden alle Aufträge übergeben, die in diesem Nummernverwalter stehen und den Mindeststatus erreicht haben.
- **Modus**: Auswahl des Übertragungsmodus. Folgende Modi stehen zur Wahl:
    - **Produktionsübergabe:** Die in der Liste angezeigten Aufträge werden an die Produktion übergeben.
    - **Produktionsfreigabe:** Die in der Liste angezeigten Aufträge werden zur Produktion freigegeben und an die Produktion übergeben.
    - **Reservierungsauftrag:** Die in der Liste angezeigten Aufträge werden an die Produktion übergeben, um Kapazitäten in der Produktion zu reservieren. Die Aufträge sind nicht zur Produktion freigegeben.
    - **Kostenkalkulation:** Die in der Liste angezeigten Aufträge werden an die Produktion übergeben, um die Material- und Maschinenkosten zu ermitteln. Die Aufträge belegen keine Zeiten in der Produktion und sind nicht zur Produktion freigegeben.
    - **Übergabe nicht produktionsrelevanter Änderungen:** Wenn die in der Liste angezeigten Aufträge bereits an die Produktion übergeben sind, können Änderungen an nicht produktionsrelevanten Daten in den Positionen und Aufträgen nachträglich übergeben werden, z. B.:
        - Änderungen an Kundenadresse, Kunde und Lieferadresse, Änderungen der Tour,
        - Änderungen der Dateianhänge mit Kennzeichen für die Produktionsübergabe oder der Positionstexte mit Kennzeichen für die Produktionsübergabe,
        - Änderungen an Kommission und Kundenpositionen.
    - **Storno:** Die in der Liste angezeigten Aufträge werden mit einem Storno-Kennzeichen erneut übergeben. Der Dokumentenstatus wird auf *Übergabe Produktion storniert* umgesetzt.
        ⇨ Tutorial, "So stornieren Sie die Produktionsübergabe manuell" auf Seite E-40

#### Ausgabe

In diesem Bereich werden die Daten zu dem Auftrag angezeigt, der aktuell übertragen wird. Die Einstellungen zur Übergabedatei legen Sie über das Menü **Funktionen** fest:
⇨ "Einstellungen Produktionsübergabe" auf Seite E-174

- **Ausgabe-Datei**: Anzeige von Pfad und Namen der Übergabedatei.
- **Release**: Version der Übergabedatei.
- **Lauf-Nummer**: Anzeige der fortlaufenden Nummer der Produktionsübergabe. Die Nummer wird aus dem Nummernkreis für den Bereich gezogen, der in den Stammdaten hinterlegt ist. Die Trennung der Übergabe in verschiedene Bereiche ist dann sinnvoll, wenn Sie mehrere Produktionsstätten eingerichtet haben.
  ⇨ Stammdaten, "Nummernkreise" auf Seite B-885
- **Positionsläufe**: Anzahl der Läufe, die für die Positionen gebildet werden.
- **Gesamt, Gesamtpositionen**: Anzahl der übergebenen Aufträge und Positionen.
- **Auftrag**: Nummer des Auftrags, der aktuell übertragen wird.

#### Aufträge

In der Übersicht werden alle Aufträge aus dem Nummernverwalter aufgelistet.
- **Nummer:** Nummer des Auftrags
- **Nummer Kunde/Lief.:** Nummer des Kunden
- **Kunde/Lieferant:** Name des Kunden
- **Status:** Status des Auftrags
- **Datum Prod. ISO, VSG, ESG:** Datum, an dem das ISO, VSG oder ESG voraussichtlich produziert wird.
- **Lauf-Nr. ISO, VSG, ESG:** Nummer des Laufs, in dem das ISO, VSG oder ESG produziert wurde. Die Nummer wird nach der Rückmeldung angezeigt.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag
- **Lieferschein:** Das Feld bleibt in dieser Anzeige normalerweise leer. Nur wenn Lieferscheine vor der Produktionsübergabe gedruckt werden, wird das Feld gefüllt.
- **Tour:** Name der Tour, mit der geliefert wird.
- **Gewicht gesamt:** Gewicht aller Auftragspositionen.
- **Stück gesamt:** Stückzahl aller Auftragspositionen.
- **Qm gesamt:** Fläche aller Auftragspositionen.
- **LFM gesamt:** Laufmeter der Kanten.
- **Datum Erfassung:** Erfassungsdatum des Auftrags.

#### Export

Wenn Sie in der Übersicht auf das erste Feld in der Titelzeile der Tabelle klicken, können Sie weitere Einstellungen für den Export festlegen.
- **CSV-Datei schreiben:** Mit der Wahl dieser Funktion können Sie die Daten aus der Übersicht in eine CSV-Datei schreiben. Ein Dialog bietet Ihnen die Auswahl des Speicherortes.
- **Optionen:** Mit der Wahl dieser Funktion können Sie festlegen, nach welchen Einträgen eine neue Zeile geschrieben werden soll.
- **XML-Datei schreiben:** Mit der Wahl dieser Funktion können Sie die Daten aus der Übersicht in eine XML-Datei schreiben. Ein Dialog bietet Ihnen die Auswahl des Speicherortes.

### Einstellungen Produktionsübergabe

**Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen**
**Fertigung > Angebotsoptimierung > Übergabe Produktion > Menü Funktionen > Einstellungen**

Im Dialog **Einstellungen – Produktionsübergabe** können Sie Einstellungen für die Übergabe an die Produktion festlegen. Die Einstellungen werden für Angebote und Aufträge getrennt eingerichtet und gespeichert.

> **Einstellungen pro Arbeitsplatz**
> Die Einstellungen gelten pro Arbeitsplatz, d. h., dass für jeden Mitarbeiter eigene Einstellungen verwendet werden können.

In diesem Dialog finden Sie folgende Register:
*   "Einstellungen Produktionsübergabe – Schnittstelle" auf Seite E-175
*   "Einstellungen Produktionsübergabe – Übergabe Parameter" auf Seite E-177
*   "Einstellungen Produktionsübergabe – Zusätzliche Schnittstellen" auf Seite E-184
*   "Einstellungen Produktionsübergabe – Texte/Anlagen" auf Seite E-186

#### Einstellungen Produktionsübergabe – Schnittstelle

**Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Schnittstelle**

*(Screenshot: Abb. E-86 Einstellungen-Produktionsübergabe - Schnittstelle)*

In diesem Register legen Sie die Details zur Schnittstelle fest, über die Aufträge an die Produktion gesendet werden.

**Schnittstelle Produktion**
In diesem Bereich legen Sie die Einstellungen für die Datei zur Produktionsübergabe fest. Wenn Sie das Format OrderXML verwenden, werden außer den Produktionsdaten auch die Daten für CAD Designer (Bars) in die jeweilige Übergabedatei geschrieben. Pro Auftrag wird eine Übergabedatei erstellt.

- **Version**: Standardmäßig werden die Daten per OrderXML übertragen. Wenn Sie Pool.asc-Dateien erzeugen wollen, müssen Sie die Version auswählen, die in Ihrem System installiert ist. In diesem Fall müssen Sie im Register **Übergabe Parameter** die Checkbox **A+W Production** deaktivieren.
  ⇨ "A+W Production" auf Seite E-178

- **Pfad/Dateiname**: Eingabe von Verzeichnis und den Dateinamen, unter dem die Übergabedatei gespeichert werden soll. Achten Sie bei der Übergabe an A+W Production darauf, dass die Datei in ein Verzeichnis geschrieben wird, das von A+W Production überwacht wird. Standardmäßig verwenden Sie den Dateinamen OrderXXXX.xml, wobei die Platzhalter (XXXX) durch die Auftragsnummer und einen Zeitstempel ersetzt werden.

**Schnittstelle AWDesign**
In diesem Bereich legen Sie die Einstellungen für die Übergabe an CAD Designer (Bars) fest.

- **Version**: Standardmäßig wird die Übergabe per OrderXML genutzt.
- **Pfad/Dateiname**: Angabe von Verzeichnis und den Dateinamen für die Übergabedatei an CAD Designer (Bars).

**OrderXML**
- **Version**: Auswahl der Version der OrderXML-Schnittstelle, die auf Ihrem System installiert ist.
- **ERP-Webservice-URL**: Webadresse, über die der ERP-Webservice angesteuert wird, z. B. `http://localhost/albwir.erp.webservice.2011`. Diese URL muss eingetragen werden, wenn Sie mit OrderXML arbeiten.
- **Speichern der OrderXML-Dateien durch ERP-Webservice**: Bei der OrderXML-Übergabe kann die Übergabedatei durch A+W Business oder durch den ERP-Webservice gespeichert werden.
  - [ ] Die Übergabedateien werden von A+W Business gespeichert (Standard).
  - [x] Die Übergabedateien werden durch den ERP-Webservice gespeichert.
- **Unicode-Format schreiben**: Die Übergabe-Daten können in zwei verschiedenen Formaten geschrieben werden.
  - [ ] Die Übergabedateien werden im Standard-Format geschrieben.
  - [x] Die Übergabedateien werden im Unicode-Format geschrieben.

**Modus der Übergabe**
Mit der Wahl der Option legen Sie den Modus für die automatische Übergabe fest:
- **Nach Mindest- und Sperrstatus Produktionsübergabe:** Für die automatische Produktionsübergabe wird der Auftragsstatus mit dem Mindest- und Sperrstatus für die Produktionsübergabe verglichen. Liegt der Auftragsstatus dazwischen, wird der Auftrag automatisch an die Produktion übergeben. Dies ist die Standardeinstellung.
- **Dokumente im Kapazitätsplanungs-Pool:** Mit dieser Einstellung werden die Aufträge zuerst an AWCapacity Planning übergeben. Sobald ein Auftrag neu erfasst oder geändert wird, landet er im Pool für die Kapazitätsplanung. Wenn die automatische Produktionsübergabe aktiviert ist, wird ein Auftrag in diesem Pool automatisch übergeben. Nach der Übergabe wird der Auftrag aus diesem Pool entfernt. Mit dieser Einstellung ist Übergabe zur Angebotsoptimierung gesperrt.

Sie können diese Einstellung ignorieren, wenn Sie die Übergabe nicht automatisiert haben. In diesem Fall wird im Dialog **Produktionsübergabe** die Datenübergabe aus dem Nummernverwalter manuell gestartet, wobei Mindest- und Sperrstatus berücksichtigt werden.
⇨ "Übergabe Produktion" auf Seite E-170

#### Einstellungen Produktionsübergabe – Übergabe Parameter

**Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Übergabe Parameter**

*(Screenshot: Abb. E-87 Einstellungen-Produktionsübergabe – Übergabe Parameter)*

In diesem Register legen Sie fest, welche Parameter in die Übergabedatei geschrieben und damit an die Produktion übergeben werden sollen.

- **Benutzerabhängige Einstellungen verwenden**: Die Einstellungen werden in die Datenbank geschrieben und beim Start von A+W Business geladen. Sie können Einstellungen pro Benutzer festlegen. Diese Checkbox wird nicht angezeigt, wenn Sie den Dialog über **Firmendaten > Register Produktion** geöffnet haben.
  - [ ] Die Einstellungen gelten für alle Mitarbeiter, die sich an A+W Business anmelden.
  - [x] Die Einstellungen gelten jeweils nur für den Mitarbeiter, der sich aktuell an A+W Business angemeldet hat.
- **A+W Production**: Sie können die Daten im Format OrderXML an A+W Production übergeben. Wenn Sie mit der Pool.asc-Übergabe arbeiten, dürfen Sie diese Einstellung nicht wählen.
  - [ ] Die Daten werden nicht an A+W Production übergeben. Wählen Sie diese Einstellung, wenn die Daten an A+W Standard Optimizer oder ALFERT übergeben werden sollen.
  - [x] Die Daten werden direkt an A+W Production übergeben. Dazu muss im Register **Schnittstelle** der Pfad angegeben werden, unter dem die Übergabedateien gespeichert werden. ⇨ "Pfad/Dateiname" auf Seite E-175
- **Laufnummer vorgeben**: Die Laufnummer (Nummer der Übergabe) kann von A+W Business aus dem Nummernkreis von AWPool gezogen werden.
  - [ ] Die Übergabelaufnummer wird in der Produktion selbst vergeben.
  - [x] Die Übergabelaufnummer wird von A+W Business aus dem Nummernkreis AWPool gezogen und in die Schnittstellendatei geschrieben. ⇨ Stammdaten, "Nummernkreise - Produktion" auf Seite B-888
- **Positions-Splitting lizenziert**: Nur Pool.asc-Übergabe. Wenn die Produktion von großen Aufträgen über mehrere Tage verteilt werden muss, können Sie bestimmen, ob die Teilung sich auch auf Positionen beziehen darf. Diese Einstellung betrifft nur die A+W Business-Kapazitätsplanung. Diese Checkbox ist nur freigeschaltet, wenn das Modul lizenziert ist.
  - [ ] Positionen sollen immer so verplant werden, dass sie an einem Tag produziert werden.
  - [x] Positionen können auf mehrere Tage verteilt produziert werden.
- **Automatische Übergabe bei Wareneingang**: Wenn Sie in Aufträgen Positionen mit den Kennzeichen Produktion erfasst haben, in denen zusätzlich Komponenten enthalten sind, die bestellt werden müssen, können diese Aufträge erst produziert werden, wenn die Komponenten eingetroffen sind, z. B. ein ISO mit einem Ornamentglas, das nicht auf Lager gehalten wird. Beim Eingang der bestellten Komponenten kann die Information über den Wareneingang an die Produktion weitergegeben werden. Voraussetzung ist, dass der PPS-Webservice installiert ist und die URL in den **Firmendaten > Register Produktion** angegeben wurde. ⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-972
  - [ ] Der Wareneingang der Bestellartikel wird nicht automatisch an die Produktion übergeben. Er muss nach der Eingangsbuchung manuell an die Produktion übergeben werden.
  - [x] Der Wareneingang der Bestellartikel wird automatisch an die Produktion übergeben. Dazu muss diese Funktion auch im Wareneingang aktiviert werden. ⇨ Einkauf, "Menü Optionen" auf Seite D-230
- **Bleiverglasung als Sprosse übergeben**: Nur Pool.asc-Übergabe. Bleiverglasungen können als Sprossensätze an die Produktion übergeben werden.
  - [ ] Bleiverglasungen werden als Bearbeitungen, nicht als Sprossensätze an die Produktion übergeben.
  - [x] Bleiverglasungen werden als Sprossensätze an die Produktion übergeben. Diese Information dient der Organisation der entsprechenden Arbeitsabläufe. Diese Einstellung sollten Sie nur in Absprache mit der A+W Software GmbH nutzen.
- **Kantenschutz pro Auftrag**: Nur Pool.asc-Übergabe. Ein Kantenschutz erfordert die Korrektur der Maße einer Position. Diese Korrektur kann automatisch bei allen Aufträgen durchgeführt werden, um den Kantenschutz anzubringen.
  - [ ] Der Kantenschutz wird nur bei Aufträgen angebracht, in denen er als Bearbeitung eingetragen ist. Die Maßkorrektur ist dabei berücksichtigt.
  - [x] Der Kantenschutz wird standardmäßig bei allen Aufträgen angebracht.
- **Artikel übergeben**: Diese Einstellung betrifft alle Produkte der Produktart **Artikel**. Diese werden i. d. R. als Lagerartikel geführt, z. B. Handgriffe.
  - [ ] Artikel werden standardmäßig nicht an die Produktion übergeben.
  - [x] Artikel werden mit an die Produktion übergeben. Siehe dazu auch die Einstellungen in den Produktstammdaten (Register A+W Production) und in den Firmendaten (Register Produktion).
- **Folien (VSG) übergeben**: Nur Pool.asc-Übergabe. Wenn Sie VSG-Scheiben herstellen, können Sie festlegen, dass die Folien mit an die Produktion übergeben werden.
  - [ ] Die Folien werden nicht an die Produktion übergeben.
  - [x] Die Folien werden an die Produktion übergeben.
- **GH-Füllungen übergeben**: Nur Pool.asc-Übergabe. Wenn Sie Gießharzfüllungen produzieren, können Sie festlegen, ob diese an die Produktion übergeben werden.
  - [ ] Die Gießharzfüllung wird nicht an die Produktion übergeben.
  - [x] Die Gießharzfüllung wird an die Produktion übergeben.
- **A+W Production-Sondertext übergeben**: Nur Pool.asc-Übergabe. Diese Einstellung betrifft nur die Pool.asc-Übergabedateien. In diesen Dateien sind die Felder limitiert. Um bestimmte Texte, die für A+W Production wichtig sind, dennoch übergeben zu können, können Textnummern für entsprechende Zusatzinformationen festgelegt werden. Diese können übergeben werden. Die Textnummern werden durch die A+W Business- und A+W Production-Projektierung festgelegt.
  - [ ] Sondertexte werden nicht übergeben.
  - [x] Die Textnummer für den Sondertext wird übergeben.

| Textnummer | Text |
| :--- | :--- |
| 3100 plus x | Stücklistenbezeichnung Abstandhalter |
| 3150 plus x | Kurzbezeichnung aus den Basisdaten zum Abstandhalter |
| 3200 plus x | Stücklistenbezeichnung UV-Randverbund, Schmaler Randverbund |
| 3250 plus x | Kurzbezeichnung aus den Basisdaten zum UV-Randverbund, Schmaler Randverbund |
| 3300 plus x | Stücklistenfarbe zum Abstandhalter |
| 3400 plus x | Stücklistenbezeichnung Gas |
| 3450 plus x | Kurzbezeichnung aus den Basisdaten zum Gas |
| (dabei ist x ein fortlaufender Zähler, also 0, 1, 2, 3...) |
| 3600 | Positionsrückschnitt |
| 3700 | Teilegewicht in Gramm zur Satzart 8 |
| 4100 | CE-Kennzeichen |

- **Touren-Rangfolge übergeben**: Nur Pool.asc-Übergabe. Die Tour-Rangfolge wird aus den Stammdaten der Kunden ausgelesen. Sie kann für die Beladung der Lkws wichtig sein.
  - [ ] Die Tour-Rangfolge wird nicht übergeben.
  - [x] Die Tour-Rangfolge wird übergeben.
- **Direktanlieferung nicht übergeben**: Bestellartikel können vom Lieferanten direkt an den Kunden gesendet werden. Das Kennzeichen wird im Auftragskopf im Register **Abweichende Anschriften** gesetzt.
  - [ ] Alle Auftragspositionen werden an die Produktion übergeben. Das Kennzeichen zur Direktanlieferung wird nicht berücksichtigt.
  - [x] Bestellpositionen mit dem Kennzeichen zur Direktanlieferung werden nicht an die Produktion übergeben. Die Positionen werden direkt vom Lieferanten an den Kunden geliefert.
- **OrderXML: Kurzbez. statt Matchcode übergeben**: Bei der OrderXML-Übergabe wird für Produkte standardmäßig der Matchcode übergeben.
  - [ ] Der Matchcode wird als Produktbezeichnung übergeben.
  - [x] Statt des Matchcodes wird die Kurzbezeichnung übergeben. Wenn Sie von der Pool-Übergabe auf OrderXML umgestellt haben, können Sie diese Einstellung wählen, um weiterhin die Kurzbezeichnung zu übertragen.
- **Beschaffungsart Produktion aus Dokument vorr.**: Nur Pool.asc-Übergabe. In der Regel sind die Beschaffungsarten für A+W Business und A+W Production identisch. Bei Abweichungen können Sie festlegen, welche Angabe vorrangig ausgewertet werden soll. Die Einstellung ist z. B. wichtig für VSG, das sowohl produziert als auch zugeschnitten wird.
  - [ ] Die Beschaffungsart aus A+W Production wird vorrangig ausgewertet.
  - [x] Die Beschaffungsart aus dem Auftrag wird vorrangig ausgewertet.
- **Provinz in der Anschrift übergeben**: Nur Pool.asc-Übergabe. Diese Einstellung betrifft nur Staaten, in denen die Provinz wichtig ist.
  - [ ] Die Provinz wird nicht an die Produktion übergeben.
  - [x] Die Provinz wird an die Produktion übergeben und an den Namen des Ortes angehängt.
- **Mengenfelder im Positionssatz tauschen**: Nur Pool.asc-Übergabe. Wenn Sie mit der Kapazitätsplanung von A+W Business arbeiten, können deren Mengenfelder übernommen werden.
  - [ ] Die Mengenfelder werden nicht aus der Kapazitätsplanung übernommen.
  - [x] Die Mengenfelder sollen aus der Kapazitätsplanung übernommen werden. Dabei werden die Felder für die Menge (Feld 11) und für die Positionsmenge (Feld 85) getauscht.
- **Noppen-KZ in Sondertext 1 im Positionssatz**: Nur Pool.asc-Übergabe. Das Kennzeichen für Noppen kann an die Produktion übergeben werden. Diese Einstellung betrifft nur die Pool.asc-Schnittstelle in der Version 2.3.
  - [ ] Das Kennzeichen für Noppen wird nicht übergeben.
  - [x] Das Noppen-KZ der ersten Sprosse wird als Sondertext 1 (im Feld 133) des Positionssatzes übergeben.
- **Order-Tags erzeugen**: Zurzeit nur kundenspezifisch genutzt.
- **VSG-Auflösung (Rel. 2.1)**: In Pool.asc 2.1 können für VSG (als Position oder als Komponente in der Stückliste) zusätzliche Sätze erzeugt werden. Diese Checkbox ist gesperrt, wenn Sie ein anderes Format gewählt haben.
  - [ ] Bei der VSG-Auflösung werden keine zusätzlichen Sätze erzeugt.
  - [x] Für die VSG-Produktion werden Pseudopositionen erzeugt. Diese Einstellung sollten Sie nur in Absprache mit der A+W Software GmbH nutzen.
- **VSG (2.1) Maßzugabe aus Stückliste**: In Pool.asc 2.1 können für VSG, die Glaskomponenten mit Bearbeitungen enthalten, die Maßzugaben aus den Stücklisten übergeben werden. Diese Checkbox ist gesperrt, wenn Sie ein anderes Format gewählt haben.
  - [ ] Maßzugaben der Stücklisten-Komponenten werden nicht berücksichtigt.
  - [x] Maßzugaben der Stücklisten-Komponenten werden übergeben.
- **Inchwerte immer in 1/256 inch**: Nur Pool.asc-Übergabe. In den Firmendaten im Register System ist festgelegt, wie die Maß-Präzision gerechnet wird. Diese Einstellung kann übersteuert werden. ⇨ Stammdaten, "Maßsystem" auf Seite B-961
  - [ ] Die Maß-Präzision wird aus den Firmendaten übernommen.
  - [x] Für die Produktion soll die Maß-Präzision auf 1/256 fixiert werden.
- **Verbundtyp an 2. Stelle**: Nur Pool.asc-Übergabe. Wenn in der Stückliste ein Artikel der Produktgruppen UV-Randverbund oder Schmaler Randverbund vorhanden ist, kann an Stelle 2 des Randverbund-Feldes (Feld 77 des Positionssatzes) das Kennzeichen 1 (für UV-Randverbund) oder 2 (für Schmaler Randverbund) geschrieben werden.
  - [ ] Für diese Bearbeitungen wird kein Kennzeichen übergeben.
  - [x] Der Verbundtyp des Abstandhalter-Kennzeichens wird an Stelle 2 im Feld des Abstandhalter-Kennzeichens (Feld 80) exportiert.
- **Kundenlogo anhand von Lieferanschrift**: Wird nur kundenspezifisch genutzt.
- **Stufung VSG auf Stücklistenebene übergeben**: Nur Pool.asc-Übergabe. Die Übergabe der Stufung kann für die Produktion von VSG in einem ISO gesondert eingestellt werden.
  - [ ] Die Stufung wird auf der Ebene des Hauptprodukts übergeben.
  - [x] Die VSG-Stufung wird als Bearbeitung an den gestuften Gläsern übergeben.
  > **ISO mit VSG**
  > Für die korrekte Übergabe von Daten an A+W Production sollten Sie das Kennzeichen immer dann setzen, wenn in Isolierglas-Einheiten ein VSG mit Stufung eingebaut wird.
- **Übergabe Stufung am Stücklistenelement**: Nur Pool.asc-Übergabe. Die Übergabe der Stufung aller Positionen, in denen kein VSG verarbeitet wird, kann insgesamt eingestellt werden.
  - [ ] Die Stufung wird auf der Ebene des Hauptprodukts übergeben.
  - [x] Die Stufung wird als Bearbeitung an den entsprechenden Gläsern übergeben.
- **Fremdschlüssel Verpackung übergeben**: Nur Pool.asc-Übergabe. Pro Auftrag kann eine geeignete Verpackungsart angegeben werden. Wenn in den Stammdaten Fremdschlüssel für Verpackungsarten hinterlegt sind, können diese an die Produktion übergeben werden.
  - [ ] Der Fremdschlüssel wird nicht übergeben.
  - [x] Der Fremdschlüssel wird als Gestellvorgabe mit an die Produktion übergeben.
- **Artikel in Stückliste exportieren**: Standardmäßig werden nur Artikel aus der Hauptproduktebene an die Produktion übergeben. Die Übergabe der einzelnen Stücklistenartikel kann eingestellt werden.
  - [ ] Artikel aus der Stückliste werden nicht übergeben.
  - [x] Die einzelnen Artikel in der Stückliste werden übergeben.

**Sonstiges**
- **Positionslimit pro Übergabedatei**: Bei der Pool.asc-Übergabe werden die Positionen aller Aufträge eines Nummernverwalters in eine Übergabedatei geschrieben. Wenn regelmäßig sehr viele Aufträge und/oder sehr viele Positionen übergeben werden, kann festgelegt werden, wann eine neue (zweite) Datei begonnen werden soll, z. B. nach 50 Positionen. Wenn Sie mit OrderXML arbeiten, wird für jeden Auftrag eine eigene Datei erzeugt. In diesem Feld sollte dann eine 0 (null) stehen.

#### Einstellungen Produktionsübergabe – Zusätzliche Schnittstellen

**Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Spezielle Einstellungen**

*(Screenshot: Abb. E-88 Einstellungen-Produktionsübergabe - Zusätzliche Schnittstellen)*

In diesem Register legen Sie die Daten für weitere Schnittstellen fest.

**RONA / LIOPT**
Wenn Sie nicht mit A+W Production arbeiten, müssen Sie den Export und den Pfad für zusätzliche Übergabedateien für diese Schnittstellen festlegen.
Die LIOPT-Schnittstelle steht ab A+W Business-Release 2012 nicht mehr zur Verfügung.

- **Export aktiv**: Der Export der zusätzlichen Übergabedatei muss für die entsprechende Schnittstelle aktiviert werden.
  - [ ] Die Schnittstelle wird nicht benutzt, es wird keine Übergabedatei geschrieben.
  - [x] Eine zusätzliche Übergabedatei für RONA oder LIOPT soll in dem unten angegebenen Pfad geschrieben werden.
- **Pfad/Dateiname**: Wenn Sie den Export aktiviert haben, müssen Sie den Pfad und Dateinamen angeben.

**Sicherheitskopien**
Diese Einstellungen betreffen nur die Pool.asc-Schnittstelle.

- **Erstellen**: Wenn Sie mit der Pool.asc-Schnittstelle arbeiten, können Sie eine Sicherheitskopie von der Übergabedatei erstellen lassen.
  - [ ] Eine Sicherheitskopie wird nicht erstellt.
  - [x] Von jeder Pool.asc-Datei wird automatisch eine Sicherheitskopie gespeichert.
- **Pfad/Dateiname**: Wenn Sie eine automatische Sicherheitskopie speichern, müssen Sie den Pfad und Dateinamen angeben.
- **Datei löschen nach ... Tag(en)**: Wenn Sie eine automatische Sicherheitskopie speichern, können Sie festlegen, nach wie vielen Tagen diese automatisch wieder gelöscht werden soll. Wenn Sie 0 (null) eintragen, werden die Sicherheitskopien nicht automatisch gelöscht. Sie sollten dann das entsprechende Verzeichnis manuell von den nicht mehr benötigen Dateien bereinigen.

#### Einstellungen Produktionsübergabe – Texte/Anlagen

**Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Texte/Anlagen**

*(Screenshot: Abb. E-89 Einstellungen-Produktionsübergabe – Texte/Anlagen)*

In diesem Register legen Sie fest, welche Texte und Dateianhänge mit an die Produktion übergeben werden sollen.

**Kennzeichen von zu übertragenden Texten**
Im Auftrag können für den gesamten Auftrag und/oder für einzelne Positionen Texte hinterlegt werden. Über ein Textkennzeichen ist jeder Text einer Textart zugeordnet. Sie können die Checkbox der Textart markieren, die an die Produktion übergeben werden soll. In der Regel ist dies das Kennzeichen P. Sie können mehrere Textkennzeichen markieren.

**Kennzeichen von zu übertragenden Dateianhängen**
Im Auftrag können für den gesamten Auftrag und/oder für einzelne Positionen Dateien mit zusätzlichen Informationen angehängt werden, z. B. grafische Darstellungen zu einem Modell oder zur Sprossenkonstruktion.
- [ ] Dateianhänge werden nicht an die Produktion übergeben.
- [x] Dateianhänge werden mit übergeben.

### Modellliste

**Fertigung > Produktion > Modellliste**

*(Screenshot: Abb. E-90 Modellliste)*

In diesem Dialog können Sie sich die Aufträge anzeigen lassen, in denen ein bestimmtes Modell zu einem bestimmten Termin geliefert werden soll. Sie können sich damit z. B. einen Überblick über die Aufträge mit freien Formen verschaffen, die manuell zugeschnitten werden müssen.

Das Ergebnis der Suche kann als Report gedruckt werden.

**Selektion**
- **Artikelnummer**: Eingabe der Artikelnummer (Produktnummer), nicht der Modellnummer.
- **Lieferdatum**: Eingabe des Lieferdatums, zu dem das angegebene Modell geliefert werden soll.

**Artikel**
- **Bezeichnung, Bezeichnung 2**: Bezeichnung des gewählten Produkts aus den Stammdaten.

**Übersicht**
In der Übersicht werden alle Aufträge aufgelistet, in denen das gewählte Modell zum angegebenen Termin geliefert werden soll.
- **Auftragsnummer:** Nummer des Auftrags, in dem das gesuchte Modell enthalten ist.
- **Pos:** Nummer der Auftragsposition.
- **Kunde:** Name des Kunden, für den dieser Auftrag gefertigt wird.
- **Artikelnummer:** Nummer des Produkts.
- **Bezeichnung 1, 2, 3:** Bezeichnungen zum Produkt.
- **Tour:** Tour, mit der der Auftrag ausgeliefert werden soll.

### Gestellbelegung prüfen

**Fertigung > Produktion > Gestellbelegung**

*(Screenshot: Abb. E-91 Gestellbelegung)*

In diesem Dialog können Sie die Gestellbelegung für die Aufträge prüfen, die produziert werden. Den Aufträgen müssen bereits Gestelle zugeordnet sein.

#### Menü Funktionen
Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
*   **ASCII-Datei erstellen:** Schreibt die Daten werden in eine ASCII-Datei.
*   **Einstellungen:** Öffnet den Dialog Einstellungen, in dem Sie die Einstellungen für die ASCII-Datei festlegen.
    ⇨ "Einstellungen (Gestellbelegung prüfen)" auf Seite E-190

#### Auswahl
- **Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter**: Auswahl des Nummernverwalters, auf den der Dialog zugreifen soll.

#### Sortierkriterien
Mit der Wahl der Option legen Sie fest, in welcher Reihenfolge die Aufträge in der Übersicht dargestellt werden sollen:
*   **Nach Auftrags- + Positionsnummern:** Die Anzeige wird zuerst nach Auftrags- und dann nach Positionsnummern sortiert.
*   **Nach Bestelltext1 + Kundenposition:** Die Anzeige wird zuerst nach Bestelltext 1 und dann nach Kundenposition sortiert.
*   **Alle:** Alle Aufträge im gewählten Nummernverwalter werden angezeigt.
*   **Außer TPS:** Aufträge mit TPS werden nicht angezeigt.
*   **Nur TPS:** Nur die Aufträge mit TPS werden angezeigt.

#### Übersicht
In der Übersicht werden die Aufträge angezeigt, die sich im gewählten Nummernverwalter befinden.
- **Nummer:** Laufende Nummer in der Übersicht.
- **Nummer Kunde/Lief., Kunde/Lieferant:** Nummer und Name des Kunden oder Lieferanten.
- **Status:** Status des Auftrags oder der Position.
- **Bestelltext1:** Bestelltext 1 aus dem Auftrag.
- **Block-/Fachnummer:** Block- oder Fachnummer auf dem Gestell.
- **Sortierung:** Kennzeichen für die Sortierung.
- **Verpackungsart:** Art der Verpackung, z. B. Gestell, Kiste.
- **Datum Prod. ISO, VSG, ESG:** Datum, an dem das ISO, VSG oder ESG produziert wird.
- **Lauf-Nr. ISO, VSG, ESG:** Nummer des Laufs, in dem das ISO, VSG oder ESG produziert wird.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag.
- **Lieferschein:** Nummer des Lieferscheins.
- **Tour:** Name der Tour, mit der geliefert wird.
- **Gewicht gesamt:** Gewicht aller Auftragspositionen.
- **Stück gesamt:** Stückzahl aller Auftragspositionen.
- **Qm gesamt:** Fläche aller Auftragspositionen.
- **LFM gesamt:** Laufmeter der Kanten.
- **Datum Erfassung:** Erfassungsdatum des Auftrags.

### Einstellungen (Gestellbelegung prüfen)

**Fertigung > Produktion > Gestellbelegung > Menü Funktionen > Einstellungen**

Für L-Gestelle können Sie zusätzliche Voreinstellungen festlegen. Diese Einstellungen sind insbesondere für TPS wichtig.

In diesem Dialog finden Sie folgende Register:
*   "Einstellungen – Gemeinsam" auf Seite E-191
*   "Einstellungen – Kunden" auf Seite E-192

#### Einstellungen – Gemeinsam

**Fertigung > Produktion > Gestellbelegung > Menü Funktionen > Einstellungen**

*(Screenshot: Abb. E-92 Gestellbelegung – Einstellungen für den Datenexport)*

In diesem Dialog können Sie die Kriterien für die Übergabedatei festlegen. Die Gestellbelegung kann in eine ASCII-Datei geschrieben werden.

- **Pfad ASCII-Datei**: Eingabe des Pfads für die ASCII-Datei. Standardmäßig wird in ein temporäres Verzeichnis auf C:\ gespeichert. Der Name der Datei wird aus Kundennummer, Tag und Monat gebildet.
- **Verpackungsart**: Sie können die Verpackungsart für die Aufträge einstellen, deren Daten exportiert werden sollen. Nur die Verpackungsarten werden zur Auswahl angeboten, die in den Stammdaten hinterlegt sind.
- **Druck**: Mit der Wahl der Option legen Sie fest, wie die Daten gedruckt werden sollen.
- **L-Gestelle TPS, L-Gestelle**: Geben Sie an, wie groß die Anzahl der Fächer für die Gestelle sein darf. Die Höchstzahl für TPS ist 22, für die restlichen L-Gestelle 21. Sie können außerdem die Höchstmaße für die jeweiligen Fächer angeben. Die Daten werden vor dem Schreiben der ASCII-Datei geprüft.

#### Einstellungen – Kunden

**Fertigung > Produktion > Gestellbelegung > Menü Funktionen > Einstellungen > Kunden**

*(Screenshot: Abb. E-93 Gestellbelegung – Einstellungen für den Datenexport)*

Sie können für einzelne Kunden festlegen, mit welcher Startnummer die Zählung der benötigten Gestelle standardmäßig beginnen soll.

**Kundenindividuelle Einstellungen**
- **Kunde**: Nummer und Name des Kunden, für den die Einstellungen festgelegt werden.
- **Zuschlagartikel**: Produktnummer des Zuschlags, der berechnet wird.
- **Gestellstartnummer**: Startnummer des Gestells.
- **[Neu], [Löschen]**: Schaltet eine neue Zeile in der Übersicht frei, löscht einen markierten Eintrag.

## Barcode-Übergabe

**Fertigung > Produktion > Übergabe Barcode Prod.**

Sie können die einzelnen Positionen von Aufträgen per Barcode an die Produktion übergeben. Dazu steht Ihnen der Dialog **Produktionsübergabe (pos. orient.)** zur Verfügung.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite E-193
*   "Übergabe Barcode Produktion" auf Seite E-194

### Menü Funktionen

**Fertigung > Produktion > Übergabe Barcode Produktion**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Produktionsübergabe zu schließen.

**Gruppe Produktion**
*   **Einstellungen:** Öffnet den gleichnamigen Dialog, in dem Sie die Einstellungen für die Übergabedatei festlegen können.
    ⇨ "Einstellungen Produktionsübergabe" auf Seite E-174
*   **Übersicht Auftrag:** Öffnet den Dialog **Übersicht Statusrückmeldungen**, in dem Sie sich pro Auftrag und Position anzeigen lassen können, welcher Status aus der Produktion zurückgemeldet wurde.
    ⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-572
*   **Läufe löschen:** Löscht die angegebenen Läufe.

**Gruppe Kapazitätsplanung**
*   **Bearbeitungen:** Öffnet den Dialog **Arbeitsarten**, in dem Sie sich die Auslastung pro Arbeitsarten anzeigen lassen können. Die entsprechenden Daten stehen nur zur Verfügung, wenn Sie mit der Kapazitätsplanung von A+W Business arbeiten.
    ⇨ Kapazitätsplanung, "Arbeitsarten" auf Seite H-196

### Übergabe Barcode Produktion

**Fertigung > Produktion > Übergabe Barcode Produktion**

Wenn Sie mit Scannern arbeiten, können Sie die einzelnen Auftragspositionen per Barcode an die Produktion übergeben.

In diesem Dialog finden Sie folgende Register:
*   "Übergabe Barcode Produktion – Übersicht" auf Seite E-194
*   "Übergabe Barcode Produktion – Details" auf Seite E-195

#### Übergabe Barcode Produktion – Übersicht

**Fertigung > Produktion > Übergabe Barcode Produktion > Register Übersicht**

*(Screenshot: Abb. E-94 Übergabe Barcode Produktion – Übersicht)*

In diesem Register legen Sie Läufe nach Arbeitsarten an. Die Laufnummer wird aus dem Nummernkreis für AWPool gewählt. Dabei können Mandanten und AV-Bereiche berücksichtigt werden.

**Identifikation**
- **Mandant**: Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.
- **Bereich**: Wenn Sie unterschiedliche AV-Bereiche angelegt haben, werden diese zur Auswahl angeboten.
- **Kommentar**: Sie können einen Kommentar für die Mitarbeiter schreiben, um z. B. auf Besonderheiten aufmerksam zu machen.

**Läufe**
In der Übersicht sind alle Läufe aufgelistet, die an die Produktion übergeben werden sollen oder wurden. Dabei werden zuerst alle Läufe aufgeführt, die noch nicht übergeben wurden, und anschließend die bereits übergebenen. Die Anzahl der anzuzeigenden Läufe kann über das Menü **Funktionen > Anzahl Läufe** eingeschränkt werden.
- **Nummer:** Nummer des Laufs.
- **Status:** Aktueller Status des Laufs.
- **Kommentar:** Text, der im Feld **Kommentar** eingegeben wurde.

#### Übergabe Barcode Produktion – Details

**Fertigung > Produktion > Übergabe Barcode Produktion > Register Details**

*(Screenshot: Abb. E-95 Übergabe Barcode Produktion – Details)*

In diesem Register fügen Sie Positionen per Barcode oder manuell hinzu.
Die aktuelle Laufnummer aus dem Register **Übersicht** wird angezeigt. Nur zu diesem Lauf können Aufträge und Positionen eingefügt werden.

**Eingabe**
- **Barcode**: Anzeige des gescannten Barcodes. Wenn Sie die Position manuell erfassen, können Sie je nach gewähltem Typ den Arbeitsgang, die Auftragsnummer und/oder Gruppen- oder Positionsnummer eingeben. Im linken Feld können Sie maximal 11 Zeichen eingeben, im rechten 3.
- **Typ**: Mit der Wahl der Option legen Sie fest, welche Nummern Sie scannen bzw. eingeben:
    - **Arbeitsgang:** Mit dieser Option scannen Sie den Arbeitsgang.
    - **Auftrags-/Gruppennummer:** Mit dieser Option scannen Sie im linken Feld die Nummer des Auftrags, im rechten die Nummer der Gruppe.
    - **Auftrags-/Positionsnummer:** Mit dieser Option scannen Sie im linken Feld die Nummer des Auftrags, im rechten die Nummer der Position.
Die Daten von Aufträgen oder Positionen werden nicht weiterverarbeitet, wenn sie schon in anderen Läufen vorhanden sind.

**Einstellungen**
- **Anzahl Läufe**: Anzahl der Läufe, die maximal angezeigt werden. Ein neuer Lauf kann auch dann angelegt werden, wenn diese Höchstzahl erreicht ist. In diesem Fall wird der älteste Lauf (kleinste Laufnummer) gelöscht.
- **Erfassungsstelle**: Angabe der Erfassungsstelle.

**Prüfziffern**
In diesem Bereich können Sie zu den Barcodes von Arbeitsgängen, Gruppen- und Auftragsnummern und/oder Auftrags- und Positionsnummern eine einstellige Prüfziffer eingeben.
Die Prüfziffer kann eine Zahl oder Buchstabe sein. Die Prüfziffern müssen nicht fortlaufend sein, z. B. sind folgende Eingaben möglich: 1, 2, 3 oder 7, 4, 6 oder G, 3, Z.
- **Arbeitsgang**: Prüfziffer für den Barcode des Arbeitsgangs, der gescannt wird.
- **Auftrags-/Gruppennummer**: Prüfziffer für den Barcode der Gruppe oder des Auftrags, die gescannt werden.
- **Auftrags-/Positionsnummer**: Prüfziffer für den Barcode der Aufträge oder Positionen, die gescannt werden.

**Arbeitsgang**
- **Arbeitsgänge auswählen**: Sie können nur Arbeitsgänge auswählen, die in den Stammdaten zur Fertigung eingerichtet sind. Die Arbeitsgänge können gescannt werden. Wenn Sie die Option Arbeitsgang gewählt haben, können Sie in der Kombobox den gewünschten Arbeitsgang auswählen.
- **Enthaltene Bearbeitungen**: In diesem Feld werden alle Bearbeitungen angezeigt, die in dem gewählten Arbeitsgang enthalten sind.
- **[Alles löschen]**: Löscht alle Einträge aus dem Lauf. Wenn Sie einen einzelnen Eintrag aus dem Lauf entfernen möchten, müssen Sie diesen markieren und im Menü **Start > Löschen** wählen.

**Lauf**
In der Übersicht werden alle Auftragspositionen aufgelistet, die zu dem aktuellen Lauf hinzugefügt wurden.
- **Auftr.Nr.:** Nummer des Auftrags.
- **Pos.Nr.:** Nummer der Position im Auftrag.
- **Bezeichnung:** Produktbezeichnung.
- **Menge:** Menge der Position oder Gruppe.
- **QM:** Gesamtfläche der Position oder Gruppe.
- **Gewicht:** Gesamtgewicht der Position oder Gruppe.
- **Arbeitsgang:** Arbeitsgang, in dem die Position gefertigt wird.
- **Gesamt:** Gesamtsummen über alle aufgeführten Positionen.

## Produktionsdaten

**Fertigung > Produktion > Produktionsdaten**

Aufträge des Typs **Produktionsauftrag** dienen dazu, Produkte für das eigene Lager zu produzieren. In Produktionsaufträgen werden die verwendeten Rohmaterialien und alle produktionsrelevanten Daten erfasst.

Als zusätzliche Möglichkeit kann durch die Eingabe der Produktionsdaten und den anschließenden Buchungsvorgang das verwendete Rohmaterial vom Lager abgebucht und die jeweiligen Positionen des Produktionsauftrages dem Lager zugebucht werden.

### Produktionsdaten (Dialog)

**Fertigung > Produktion > Produktionsdaten**

In diesem Dialog können Sie alle Daten, die zur Produktion erforderlich sind, erfassen und verbuchen.

In diesem Dialog finden Sie folgende Register:
*   "Produktionsdaten – Auftrag" auf Seite E-199
*   "Produktionsdaten - Tabelle" auf Seite E-201
*   "Produktionsdaten - Buchung" auf Seite E-202

#### Produktionsdaten – Auftrag

**Fertigung > Produktion > Produktionsdaten**

*(Screenshot: Abb. E-96 Produktionsdaten – Auftrag)*

In diesem Dialog können Sie alle Daten, die zur Produktion erforderlich sind, erfassen und verbuchen. Beachten Sie dabei, dass alle Felder zwingend gefüllt werden müssen, bis auf die Angabe eines Ausfallgrundes.

**Allgemein**
- **Datum**: Datum der Fertigung. Wenn Sie die Daten für die Zugangsbuchung im Lager eingeben, ist dies das Datum, an dem der Produktionsauftrag gefertigt werden soll oder gefertigt wurde.
- **Aggregat**: Hier wählen Sie die Maschine aus, mit der der Produktionsauftrag gefertigt wird.
- **Schicht**: Schichten werden bei Produktionsaufträgen nicht berücksichtigt. Das Feld kann leer bleiben.
- **Bearbeiter**: Name des Mitarbeiters.

**Produktionsdetails**
- **Rüstzeit/Laufzeit (Minuten)**: Die Rüstzeit und die Dauer der Fertigung geben Sie in Minuten ein.
- **Personenanzahl**: Anzahl der Personen, die für die Fertigung des Produktionsauftrags eingesetzt werden.
- **Ausfallzeit (Minuten)**: Die Ausfallzeit wird in Minuten angegeben.
- **Grund des Ausfalls**: Wenn Sie eine Ausfallzeit angegeben haben, können Sie zusätzlich angeben, wodurch der Ausfall verursacht wurde. Einmal eingegebene Ausfallgründe bleiben in der Kombobox erhalten und können anschließend ausgewählt werden.

**Produktionsauftragsdaten**
- **Auftrag**: Nummer des Produktionsauftrags.
- **Position/Menge**: Nummer und Menge der Position im Auftrag.

**Fertigprodukt**
- **Artikel**: Produktnummer der gefertigten Einheiten, die in den Produktstammdaten hinterlegt ist. Mit dieser Nummer wird das Fertigprodukt in den Lagerbestand gebucht.
- **Breite/Höhe**: Wenn die Nummer eingetragen ist, werden die Beschreibungen, Maße und Gewicht aus den Stammdaten automatisch angezeigt.
- **Anzahl Einheiten**: Anzahl der gefertigten Einheiten der aktuellen Position.
- **Identnummer automatisch erzeugen**: Bei der Verbuchung können automatisch Kisten-Identnummern (Kisten-ID) vergeben werden.
  - [ ] Kisten werden nicht verbucht.
  - [x] Im Produktionsauftrag sind Kisten enthalten, denen bei der Verbuchung automatisch IDs zugewiesen werden sollen. Nur so ist es auch möglich abweichende Inhalte anzugeben. Handelt es sich bei dem Produkt jedoch um eine Kiste mit tiefer Stückliste und enthält diese die Gläser nicht direkt als erstes Stücklistenelement, können die Inhalte nicht geändert werden.
- **Scheiben pro Einheit**: ISO-Scheiben können aus 2, 3 oder sogar 4 Scheiben bestehen. In der Regel werden 2 Scheiben pro Einheit verbaut.
- **Scheiben fertiggestellt**: Anzahl der zugeschnittenen Scheiben.

**Rohmaterial**
- **Artikel**: Produktnummer des Glases (oder der Lagerplatte), das geschnitten wird.
- **Breite/Höhe**: Maße des Rohmaterials.
- **Bruch**: In diesem Feld können Sie den Bruch von Rohmaterial eintragen.
- **Bruch auf Maschine**: Das Feld wird durch die Rückmeldung aus A+W Production gefüllt.
