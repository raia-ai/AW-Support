---
title: "DE_HB_AWProduction_2"
source: "DE_HB_AWProduction_2.pdf"
tags: ["A+W Production", "Grobplanung", "Arbeitsvorbereitung", "Läufe", "Töpfe", "Kapazitätsplanung", "Software-Dokumentation", "Benutzerhandbuch", "Tutorial", "Softwarereferenz"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein Benutzerhandbuch für das Modul 'Grobplanung' der Software A+W Production. Es enthält sowohl ein Tutorial zur Einführung in die Prozesse der Arbeitsvorbereitung als auch eine detaillierte Softwarereferenz für alle Dialoge und Funktionen."
long_description: "Dieses Handbuch behandelt das Modul 'Grobplanung' innerhalb der A+W Production Software, die für die Glas-, Fenster- und Türenindustrie entwickelt wurde. Das Dokument ist in zwei Hauptteile gegliedert: ein Tutorial und eine Softwarereferenz. Der Tutorial-Teil (Kapitel C) führt den Benutzer schrittweise durch den Prozess der Grobplanung. Er erklärt, wie man mit Ansichten arbeitet, diese konfiguriert (Register, Spalten, Filter), Aufträge verwaltet, 'Töpfe' (Sammelbehälter für Aufträge) und 'Läufe' (Produktionschargen) erstellt und verschiedene Laufstrategien anwendet. Ziel ist es, den Verantwortlichen in der Arbeitsvorbereitung zu ermöglichen, eine optimale Produktion durch strategische Lauf-Bildung zu planen. Der zweite Teil, die Softwarereferenz, dient als Nachschlagewerk. Er bietet detaillierte Beschreibungen aller Dialogfenster, Kontextmenüs, Felder und Schaltflächen, die in der Grobplanung verwendet werden. Themen wie Aufträge, Töpfe, Läufe, Positionen, Bearbeitungen und übergreifende Dialoge werden systematisch erklärt. Das Dokument richtet sich an Anwender, die für die Arbeitsvorbereitung und die Optimierung des Produktionsablaufs zuständig sind und setzt Kenntnisse des Stammdatenkonzepts von A+W Production voraus."
---

# Dokumentation

---
## Konventionen

### Register Suchen

Im Register Suchen wird die ganze Online-Hilfe nach dem gewünschten Begriff durchsucht. Das heißt, hier wird nicht nur das Thema WGR gefunden, sondern der Begriff WGR, in welchem Zusammenhang dieser auch immer verwendet wurde. Die Suche über das Register Suchen sollte immer dann angewendet werden, wenn Sie bei der Suche über das Register Inhalt oder Index erfolglos geblieben sind.

*Abb. A-9 Suche*

### Hilfetext nicht gefunden

Manche Hilfetexte können nicht direkt aufgerufen werden. In diesen Fällen können Sie über die Suchfunktionen der Online-Hilfe zur gesuchten Beschreibung finden.

- "Register Inhalt" auf Seite A-99
- "Register Index" auf Seite A-100
- "Register Suchen" auf Seite A-101

Zu manchen Dialogen ist noch kein Hilfetext vorhanden. Vielleicht finden Sie über die Register Index oder Suchen Antworten auf Ihre Fragen.

---
**A+W Production Überblick**
A-101
---

# C A+W Production Grobplanung

**Software for Glass, Windows & Doors**

## Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| 01-2023 | Vorgang suchen ergänzt. |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 07-2014 | Neuerstellung Tutorial und Softwarereferenz. |
| 08-2013 | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production |
| 03-2006 | Ersterstellung. |

**Zu diesem Modul finden Sie folgende Kapitel:**

- Tutorial
- Softwarereferenz

---
**A+W Production Grobplanung**
C-104
---

# Tutorial

## In diesem Kapitel finden Sie folgende Themen:

- Überblick
- Grobplanung

## Überblick

| Thema | Seite |
| :--- | :--- |
| **Überblick** | **C-107** |
| Aufbau des Tutorials | C-107 |
| **Grobplanung** | **C-109** |
| Prozess der Arbeitsvorbereitung | C-110 |
| **Ansichten** | **C-113** |
| Ansichten in der Grobplanung | C-114 |
| Konfigurieren von und arbeiten mit Ansichten | C-117 |
| Register anlegen und konfigurieren | C-117 |
| Spalten anlegen und konfigurieren | C-119 |
| Summenzeile anlegen und konfigurieren | C-121 |
| Neue Spalte oder Summenzeile definieren | C-123 |
| Filter anlegen und konfigurieren | C-126 |
| Weißer Screen in einer Ansicht | C-129 |
| Übungen: Konfigurieren von und arbeiten mit Ansichten | C-130 |
| **Aufträge / Pool** | **C-131** |
| Aufträge in der Grobplanung | C-132 |
| **Töpfe** | **C-134** |
| Töpfe in der Grobplanung | C-135 |
| **Läufe und Laufstrategien** | **C-140** |
| Läufe in der Grobplanung | C-141 |
| **Positionen** | **C-147** |
| Positionen in der Grobplanung | C-148 |
| **Vorgang suchen** | **C-150** |

---
**A+W Production Grobplanung**
C-106
---

## Überblick

Das Tutorial zum Prozess der Grobplanung beschäftigt sich mit der Lauf-Bildung in A+W Production. Die Verantwortlichen aus der Arbeitsvorbereitung verschaffen sich in der Grobplanung mit verschiedenen Ansichten einen Überblick und bilden mit verschiedenen Strategien Läufe, die eine optimale Produktion ermöglichen.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Production die Arbeitsvorbereitung verantworten und damit den optimalen Ablauf der Produktion organisieren. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Production kennen.

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - **Lernziele:** Was soll vermittelt werden?
  - **Nutzen:** Wofür können Sie dieses Wissen einsetzen?
  - **Merksätze:** Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.
- **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

---
**A+W Production Grobplanung**
C-107
---

### Lesehinweis

Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

---
**A+W Production Grobplanung**
C-108
---

# Grobplanung

In diesem Tutorial erfahren Sie, welche Bereiche von A+W Production zur Grobplanung gehören und wie Sie die Grobplanung durchführen.

Mit verschiedenen Ansichten (Ansichts-Dialoge) verschaffen Sie sich einen Überblick und wenden Strategien zur Lauf-Bildung an.

Zur Grobplanung gehören folgende Kapitel:

- "Prozess der Arbeitsvorbereitung" auf Seite C-110
- "Ansichten" auf Seite C-113
- "Aufträge / Pool" auf Seite C-131
- "Töpfe" auf Seite C-134
- "Läufe und Laufstrategien" auf Seite C-140
- "Positionen" auf Seite C-147

---
**A+W Production Grobplanung**
C-109
---

## Prozess der Arbeitsvorbereitung

*Abb. C-1 Prozess der Arbeitsvorbereitung*

**Prozessfluss:**
1.  **ERP-System** -> **Aufträge / Pool** (auflösen)
2.  **Aufträge / Pool** -> **Lauf / Topf** (Status: 100) (auflösen)
3.  **Lauf / Topf** (Status: 100) -> **Feinplanung** (Status: 150) (rücksetzen)
4.  **Feinplanung** (Status: 150) -> **Zur Produktion freigegeben** (Status: 200) (rücksetzen)
5.  **Zur Produktion freigegeben** (Status: 200) -> **Produktion** (Status: 300)

In der Grafik oben sehen Sie den Prozess der Arbeitsvorbereitung inklusive der Grobplanung. Die Aufträge und/oder Positionen befinden sich nach der Einlastung aus dem ERP-System im Pool, also im Dialog Aufträge. Sie verschaffen sich in den Übersichtsdialogen einen Überblick und wenden Strategien an, um Läufe zu bilden. Haben Sie Läufe gebildet, können Sie diese feinplanen (Abstellplatz-Zuordnung und Optimierung) und anschließend zur Produktion freigeben. Während des gesamten Prozesses sind die Aufträge in den Ansichten der Arbeitsvorbereitung sichtbar. Sie können also nachverfolgen, welche Aufträge sich gerade in welchem Status befinden.
Wenn Sie Läufe und Töpfe auflösen, werden diese in den Pool zurück gegeben. Sie können Aufträge aus höheren Status rücksetzen und neu feinplanen, oder neue Läufe oder Töpfe bilden.

---
**A+W Production Grobplanung**
C-110
---

## Grobplanung und Kapazitätsplanung

Einige Funktionen der Grobplanung stehen in Wechselwirkung mit der Kapazitätsplanung. Sie werden in diesem Tutorial an den entsprechenden Stellen darauf hingewiesen.

Mit der Kapazitätsplanung haben Sie einen direkten Einstiegspunkt in die Grobplanung und gelangen aus dem Produktionsmonitor heraus in den Dialog Arbeitsplan. Hier können Sie unter Berücksichtigung der Ergebnisse der Kapazitätsplanung Läufe erstellen und Auftragspositionen verwalten. Daher empfehlen wir bei aktiver Kapazitätsplanung, die Schritte der Arbeitsvorbereitung aus dem Produktionsmonitor heraus zu starten.

### Status setzen

Wenn Sie mit der Kapazitätsplanung arbeiten:
Wenn Sie den Status von Aufträgen auf *produziert*, *versandfertig* oder *ausgeliefert* setzen, gibt die Kapazitätsplanung die Kapazitäten wieder frei. Die jeweiligen Funktionen sind in der Anleitung der Kapazitätsplanung beschrieben.

### Begriffe in der Grobplanung

In den Beschreibungen für die Grobplanung werden folgende Begriffe verwendet.

| Begriff | Beschreibung |
| :--- | :--- |
| **Aufträge/Pool** | Nachdem Auftragsdaten aus dem EPR-System eingelastet wurden, sind die Aufträge in der Ansicht Aufträge, die auch Pool genannt wird, aufgelistet. |
| **Pool_Tabellen** | Die Datenbanktabellen Pool_ werden während der Einlastung der Auftragsdaten aus dem ERP-System mit Daten gefüllt. Pool_Tabellen beschreiben die Stückliste und den Auftragskopf eines Produkts. |
| **Stückliste** | Die Stückliste zeigt die enthaltenen Elemente eines Auftrags in einer Baumstruktur. In der Stückliste werden auch die Abhängigkeiten der Positionen zueinander beschrieben. |
| **Position** | Positionen sind Teile von Aufträgen. Eine Position enthält verschiedene Teile, z. B. Float 4 mm und Therm 4 mm. An die Teile sind verschiedene Bearbeitungen geknüpft, z. B. Zuschnitt oder Polieren. |
| **Bearbeitung** | Fertigungsverfahren, mit dem eine Position bearbeitet wird, z. B. Polieren oder Schleifen. |
| **Arbeitsgang** | Arbeitsgänge bringen die Eigenschaften der Bearbeitung, z. B. Polieren, mit den Eigenschaften des Werkstücks zusammen. Eine Position aus der Stückliste hat z. B. die Anforderung auf eine bestimmt Art geschliffen zu werden. Der Arbeitsgang definiert anhand dieser Anforderung die spezielle Art des Schleifens. |
| **Freigabeteile** | Explizit für die Produktion zu planende Teile. Freigabeteile werden in den Ansichten angezeigt. Freigabeteile werden in den Stammdaten definiert. |
| **Nicht-Freigabeteile**| Implizit für die Produktion zu planende Teile. Nicht-Freigabeteile werden in den Stammdaten definiert. |
| **Lauf** | Gruppe von Aufträgen und/oder Positionen, die zusammen produziert werden sollen. |
| **Topf** | Speicher oder Puffer, in dem Sie Aufträge verwalten, bei denen die weitere Vorgehensweise noch nicht geklärt ist. Sie können z. B. Aufträge so lange in einen Topf legen, bis genug Positionen mit der gleichen Glasart zusammen gekommen sind. Anschließend bilden Sie aus diesem Topf oder diesen Töpfen einen Lauf. |
| **Los** | Teil eines Laufs, der als Gruppe die gleichen Produktions-Prozesse durchläuft. Ein Los kann zur gleichen Zeit auf der gleichen Maschine mit dem gleichen Werkzeug gefertigt werden. |
| **Starttermin** | Termin, an dem die Produktion eines Laufs beginnt. |
| **Produktionstermin** | Zusammenbautermin des Kopteils. |

*Tab. C-1 Begriffe in der Grobplanung*

---
**A+W Production Grobplanung**
C-111 & C-112
---

# Ansichten

**Lernziele**
- Was sind Ansichten?
- Wie werden Ansichten konfiguriert?
- Wie arbeiten Sie mit Ansichten?

**Nutzen**
- Mit Ansichten haben Sie eine Übersicht über die Aufträge und/oder Positionen.
- Ansichten helfen Ihnen, sich für eine Laufstrategie zu entscheiden.
- Mit Ansichten sehen Sie, in welchem Status sich die Aufträge oder Positionen befinden.
- Sie bearbeiten die Aufträge aus den Ansichten heraus, indem Sie z. B. Läufe oder Töpfe bilden.

> **Merke**
> **Ansichten**: Übersichtsdialoge, in denen die Aufträge und/oder Positionen thematisch gruppiert dargestellt werden, z. B. nach Aufträgen, Bearbeitungen oder Töpfen.

---
**A+W Production Grobplanung**
C-113
---

## Ansichten in der Grobplanung

*Abb. C-2 Aufträge*

Die Übersichtsdialoge oder Ansichten in der Grobplanung sind vordefiniert, sodass Sie direkt damit arbeiten können. Sie können aus den Ansichten heraus die Aufträge und/oder Positionen bearbeiten, indem Sie z. B. Läufe oder Töpfe erstellen. Die Steuerung der Dialoge erfolgt dabei zum größten Teil über Kontextmenüs.

### Konfigurierbare Bestandteile

Die meisten Dialoge sind konfigurierbar, sodass Sie genau die Informationen angezeigt bekommen, die Sie für Ihre Produktion benötigen. In diesem Kapitel lernen Sie, wie Sie mit Übersichtsdialogen arbeiten und diese konfigurieren.

Folgende Bestandteile der Übersichtsdialoge sind konfigurierbar:
- Register
- Spalten
- Summenzeile
- Filter

---
**A+W Production Grobplanung**
C-114
---

### Dialogbeschreibungen

Folgende Dialoge sind Übersichten und in der Softwarereferenz ausführlich beschrieben:

**Dialog Aufträge**
Im Dialog Aufträge haben Sie eine Übersicht über alle eingelasteten Aufträge, die noch nicht weiter verarbeitet wurden. Von dieser Ansicht aus können Sie die Aufträge im Prozess der Arbeitsvorbereitung weiter bearbeiten, z. B. Läufe und Töpfe bilden.
⇨ "Aufträge" auf Seite C-156

**Dialog Auftragsübersicht**
Im Dialog Auftragsübersicht haben Sie eine Übersicht über Details in Aufträgen. Sie können die Auftragsübersicht nach Positionen, Teilen oder Bearbeitungen ordnen. Zudem können Sie Rahmen und Folien ein- oder ausblenden. Aus dem Dialog Auftragsübersicht heraus können Sie keine Läufe oder Töpfe erstellen.
⇨ "Auftragsübersicht" auf Seite C-159

**Dialog Füllaufträge**
Im Dialog Füllaufträge haben Sie eine Übersicht über alle Füllaufträge. Sie können sich z. B. anzeigen lassen, wie viele Positionen der Füllaufträge bereits produziert sind und wie viele noch produziert werden müssen.
⇨ "Füllaufträge" auf Seite C-162

**Dialog Töpfe**
Im Dialog Töpfe haben Sie eine Übersicht über die Töpfe in AWP. Sie können die Töpfe nach unterschiedlichen Kriterien sortieren und bearbeiten.
⇨ "Töpfe" auf Seite C-170

**Dialog Reservierungsaufträge**
Im Dialog Reservierungsaufträge können Sie sich Reservierungsaufträge anzeigen lassen. Der Dialog dient lediglich als Übersicht über die eingeplanten Kapazitäten, sie können aus dem Dialog heraus keine Läufe oder Töpfe bilden.
⇨ "Reservierungsaufträge-Topf" auf Seite C-173

**Dialog Bestellteile**
Im Dialog Bestellteile-Topf haben Sie eine Übersicht über Töpfe, die mit Bestellteilen erstellt wurden.
⇨ "Bestellteile-Topf" auf Seite C-177

**Dialog Läufe**
Im Dialog Läufe haben Sie eine Übersicht über die erstellten Läufe.
⇨ "Läufe" auf Seite C-184

**Dialog Positionen**
Im Dialog Positionen haben Sie eine Übersicht über die Positionen in den Aufträgen.
⇨ "Positionen" auf Seite C-195

**Dialog Bearbeitungen**
Im Dialog Bearbeitungen haben Sie eine Übersicht über die Bearbeitungen in den Aufträgen.
⇨ "Bearbeitungen" auf Seite C-205

**Dialog Glasarten**
Mit dem Dialog Glasarten können Sie sich in einer Übersicht die enthaltenen Glasarten ausgewählter Aufträge bzw. Positionen anzeigen lassen und einen Lauf bilden.
⇨ "Glasarten" auf Seite C-210

**Dialog Details**
Mit dem Dialog Details können Sie sich Details zu ausgewählten Aufträgen, Positionen, Teilen, Läufen oder Töpfen anzeigen lassen.
Sie können den Dialog Details aus jeder Ansicht in der Grobplanung öffnen, daher ist es empfehlenswert, diese Ansicht optimal zu konfigurieren.
⇨ "Details" auf Seite C-213

**Dialog BDE**
Im Dialog BDE bekommen Sie einen Überblick über Informationen, die sich auf die Betriebsdatenerfassung beziehen.
⇨ "BDE" auf Seite C-217

**Dialog Lose**
Im Dialog Lose bekommen Sie einen Überblick über die erstellten Lose der ausgewählten Läufe.
⇨ "Lose" auf Seite C-221

**Dialog Arbeitsplan**
Mit dem Dialog Arbeitsplan können Sie sich aus dem Produktionsmonitor heraus einen Überblick verschaffen. Der Arbeitsplan zeigt die geplanten Läufe auf einer Maschine, bzw. in einer Schicht.
⇨ "Arbeitsplan" auf Seite C-225

---
**A+W Production Grobplanung**
C-115 & C-116
---

## Konfigurieren von und arbeiten mit Ansichten

Sie können Ansichten nach Ihren Bedürfnissen konfigurieren. Fassen Sie die jeweils wichtigsten Informationen im ersten Register des Dialogs zusammen, andere Informationen folgen dann in weiteren Registern. Lassen Sie sich in den Ansichten so viel Informationen wie nötig anzeigen und so wenig wie möglich, um die Dialoge übersichtlich zu halten. Fügen Sie Summenzeilen ein, um einen schnellen Überblick zu bekommen. Nutzen Sie Filter für spezielle Anwendungsfälle.

### Register anlegen und konfigurieren

Zum Einfügen und Konfigurieren von Registern finden Sie folgende Handlungsanweisungen:
- "So fügen Sie ein Register ein" auf Seite C-117
- "So konfigurieren Sie ein Register" auf Seite C-118

#### So fügen Sie ein Register ein

1.  Öffnen Sie die Ansicht, in der Sie ein Register einfügen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü des Registers, nach dem Sie ein neues Register einfügen möchten.
    Oder öffnen Sie das Kontextmenü im Kopfteil des Dialogs, falls noch kein Register existiert.
    *Abb. C-3 Aufträge - Kontextmenü Register*
3.  Klicken Sie im Kontextmenü auf **Einfügen**.

Der Dialog **Eigenschaften von (Register)** wird geöffnet, in dem Sie dem Register einen Registertext und eine Beschreibung geben. Mit der Checkbox **Systemweite Anzeige** legen Sie fest, ob das Register für alle Anwender oder nur für Sie angezeigt wird.

*Abb. C-4 Eigenschaften von (Register)*

Das neue Register wird nach dem Register eingefügt, dessen Kontextmenü Sie geöffnet haben. Sie können ein Register verschieben, indem Sie es mit dem Mauszeiger an die gewünschte Stelle ziehen.

#### So konfigurieren Sie ein Register

1.  Öffnen Sie die Ansicht, die Sie konfigurieren möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü des Registers, das Sie bearbeiten möchten.
3.  Sie haben folgende Möglichkeiten:
    - Klicken Sie auf **Speicherautomatik**, damit alle Änderungen am jeweiligen Register automatisch gespeichert werden.
      Wenn Sie die Funktion Speicherautomatik nicht wählen, müssen Sie nach jeder Änderung am Register auf **Speichern** klicken, damit die Änderungen übernommen werden.
      Die Raute an der Bezeichnung des Registers zeigt, dass die Speicherautomatik aktiviert ist.
      *Abb. C-5 Aufträge - Aktivierte Speicherautomatik*
    - Klicken Sie im Kontextmenü des Registers auf **Eigenschaften**, um die Eigenschaften eines Registers zu bearbeiten.
      Der Dialog **Eigenschaften von (Register)** wird geöffnet, in dem Sie den Registertext und die Beschreibung bearbeiten. Mit der Checkbox **Systemweite Anzeige** legen Sie fest, ob das Register für alle Anwender oder nur für Sie angezeigt wird.
    - Sie können das konfigurierte Register importieren oder exportieren und somit als Schablonen für andere Dialoge oder Anwender verwenden.

---
**A+W Production Grobplanung**
C-117 & C-118
---

### Spalten anlegen und konfigurieren

Zum Einfügen und Konfigurieren von Spalten finden Sie folgende Handlungsanweisungen:
- "So fügen Sie eine Spalte ein" auf Seite C-119
- "So konfigurieren Sie eine Spalte" auf Seite C-120

#### So fügen Sie eine Spalte ein

1.  Öffnen Sie die Ansicht, in der Sie eine Spalte einfügen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü der Spalte, nach der Sie eine neue Spalte einfügen möchten.
3.  Klicken Sie im Kontextmenü auf **Einfügen**. Es stehen verschiedene Kategorien zur Auswahl.
    Die neue Spalte wird nach der Spalte eingefügt, deren Kontextmenü Sie geöffnet haben.
    *Abb. C-6 Aufträge - Kontextmenü Spalte*

#### So konfigurieren Sie eine Spalte

1.  Öffnen Sie die Ansicht, in der Sie eine Spalte konfigurieren möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü der Spalte, die Sie bearbeiten möchten.
3.  Sie haben folgende Möglichkeiten:
    - **Umsortieren:** Klicken Sie auf **Umsortieren**, um die jeweiligen Spalten in der umgekehrten Reihenfolge zu sortieren, z. B. nach aufsteigendem oder absteigendem Datum.
    - **Formatieren:** Klicken Sie im Kontextmenü einer Spalte auf **Formatieren**, um der Spalte eine Einheit zuzuordnen, z. B. eine Angabe in Millimetern. Es stehen verschiedene Kategorien zur Auswahl.
    - **Definition anzeigen:** Klicken Sie im Kontextmenü einer Spalte auf **Definition anzeigen**, um Details zur Spalte anzuzeigen. Der Dialog **Spaltendefinition** wird geöffnet.
      *Abb. C-7 Spaltendefinition*
    - **Spalte verschieben:** Sie können eine Spalte verschieben, indem Sie sie an die gewünschte Stelle ziehen.

> **Farben in Spalten**
> Setzen Sie sich bitte mit dem Kundenservice der A+W Software GmbH in Verbindung, wenn Sie den Spalten in Ansichten Farben zuordnen möchten.
> Spalten in verschiedenen Farben anzuzeigen, erfordert einen Eintrag in der Datenbank.

---
**A+W Production Grobplanung**
C-119 & C-120
---

#### So arbeiten Sie mit der Liste

1.  Öffnen Sie die Ansicht, mit der Sie arbeiten möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü der Liste.
    *Abb. C-8 Aufträge - Kontextmenü Liste*
3.  Wählen Sie eine Option aus der Liste. Die Kontextmenüs sind in der Softwarereferenz beschrieben.

### Summenzeile anlegen und konfigurieren

Zum Einfügen und Konfigurieren von Summenzeilen finden Sie folgende Handlungsanweisungen:
- "So fügen Sie eine Summenzeile ein" auf Seite C-121
- "So konfigurieren Sie eine Summenzeile" auf Seite C-122

#### So fügen Sie eine Summenzeile ein

1.  Öffnen Sie die Ansicht, in der Sie eine Summenzeile einfügen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü der Summenzeile, nach der Sie eine neue Summenzeile einfügen möchten.
    Oder öffnen Sie das Kontextmenü im Feld der Summenzeilen, falls noch keine Summenzeile besteht.
    *Abb. C-9 Aufträge - Kontextmenü Summenzeile*
3.  Wählen Sie ein Filter-Kriterium, z. B. **Summe Stück gesamt**.
    Die Summenzeile wird eingefügt. Jede weitere Summenzeile wird nach der Summenzeile eingefügt, deren Kontextmenü Sie geöffnet haben.

#### So konfigurieren Sie eine Summenzeile

1.  Öffnen Sie die Ansicht, in der Sie eine Summenzeile konfigurieren möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü der Summenzeile, die Sie konfigurieren möchten.
3.  Sie haben folgende Möglichkeiten:
    - Klicken Sie auf **Formatieren**, um der Summenzeile eine Einheit zuzuordnen, z. B. eine Angabe in Millimetern. Es stehen verschiedene Kategorien zur Auswahl.
    - Wählen Sie im Kontextmenü **Definition anzeigen**, um Einstellungen zur Summenzeile anzuzeigen. Der Dialog **Spaltendefinition** wird geöffnet.

---
**A+W Production Grobplanung**
C-121 & C-122
---

### Neue Spalte oder Summenzeile definieren

#### So definieren Sie Spalten oder Summenzeilen

1.  Öffnen Sie die Ansicht, in der Sie eine Spalte oder eine Summenzeile definieren möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontextmenü einer Spalte oder Summenzeile.
3.  Klicken Sie im Kontextmenü auf **Einfügen > Felddefinitionen > Editieren**.
    *Abb. C-10 Aufträge - Kontextmenü Spalte*
4.  Der Dialog **Felddefinition** wird geöffnet. Wählen Sie im Feld **Menü-Gruppe**, welcher Gruppe im Kontextmenü die Spalte oder die Summenzeile zugeordnet wird, z. B. **Teile kumuliert**.
5.  Geben Sie im Feld **Menü-Eintrag** einen Namen für die Spalte oder die Summenzeile ein, z. B. *Fertige Teile*.
6.  Geben Sie im Feld **Spaltenüberschrift** den Namen der Spalte oder die Summenzeile ein, mit der die Spalte oder Summenzeile im Dialog angezeigt wird, z. B. *Fertige Teile_alle*.
7.  Geben Sie in der Zeile **Beschreibung** eine Beschreibung für die Spalte oder die Summenzeile ein, z. B. *Zeigt alle fertigen Teile an*.
8.  Wählen Sie mit der Schaltfläche **Format**, das Format für die Spalte oder Summenzeile, z. B. **Text**.
9.  Wählen Sie mit der Schaltfläche **Auswahl öffnen** einen SQL-Ausdruck, der für die Spalte oder Summenzeile hinterlegt wird.
    Wählen Sie den Eintrag SQL-Ausdruck, um einen eigenen SQL-Ausdruck einzugeben.
10. Wählen Sie die Anzeigeoptionen für die Spalte oder die Summenzeile, z. B. ob die Sortierung der Daten aufsteigend oder absteigend erfolgen soll.
11. Klicken Sie auf **[Speichern]**, um die Änderungen zu übernehmen.
12. Klicken Sie auf **[Schließen]**, um den Dialog zu schließen.
    Die neue Spalte oder Summenzeile *Fertige Teile* ist jetzt im Kontextmenü verfügbar.

---
**A+W Production Grobplanung**
C-123, C-124, C-125
---

### Filter anlegen und konfigurieren

Zum Wählen, Einfügen, Konfigurieren und Definieren von Filtern finden Sie folgende Handlungsanweisungen:
- "So wählen Sie einen Filter" auf Seite C-126
- "So fügen Sie einen Filter ein" auf Seite C-127
- "So konfigurieren Sie Filter oder definieren neue Filter" auf Seite C-127

#### So wählen Sie einen Filter

1.  Öffnen Sie die Ansicht, in der Sie einen Filter wählen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Dropdown-Menü eines Filters, um einen Filter auszuwählen.
    *Abb. C-11 Aufträge - Dropdown-Menü Filter*
3.  Wählen Sie einen Filter. Damit ist die Ansicht gefiltert.

#### So fügen Sie einen Filter ein

1.  Öffnen Sie die Ansicht, in der Sie einen Filter einfügen möchten, z. B. **Anzeigen > Aufträge**.
2.  Klicken Sie auf **[Filter hinzufügen]**, um einen Filter einzufügen.
    Damit wurde der Filter hinzugefügt.

#### So konfigurieren Sie Filter oder definieren neue Filter

1.  Öffnen Sie die Ansicht, in der Sie Filter konfigurieren oder definieren möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontext-Menü des Filters, den Sie konfigurieren, oder nach dem Sie einen neuen Filter einfügen möchten. Der Dialog **(Filter Name)** wird geöffnet.
3.  Klicken Sie auf **[Verwalten]**. Der Dialog **Filter-Definition** wird geöffnet.
4.  Wählen Sie einen Filter aus der Liste, wenn Sie konfigurieren möchten, oder wählen Sie **Neuer Filter** aus der Liste, wenn Sie einen Filter neu definieren möchten.
    Wenn Sie einen bestehenden Filter konfigurieren, sind die Felder rechts im Dialog ausgefüllt und Sie nehmen Änderungen vor. Wenn Sie einen neuen Filter definieren, füllen Sie die Felder aus.
5.  Bearbeiten Sie im Feld **Name** die Bezeichnung des Filters, z. B. *Nur ISO*.
6.  Geben Sie im Feld **Beschreibung** eine Beschreibung des Filters ein, z. B. *Zeigt nur ISO-Aufträge an*.
7.  Geben Sie im Feld **Standard-Parameter** einen Standard-Wert ein, z. B. ein Standard-Datum, auf das zurückgegriffen wird, wenn die entsprechenden Datenbanktabellen oder -felder keinen Wert ermitteln.
8.  Wählen Sie im Feld **Zulässig für Ansicht**, in welchen Ansichten der Filter angezeigt wird, z. B. *Pool-Ansicht, Topf-Ansicht und Lauf-Ansicht*. Die Schaltflächen der gewählten Dialoge werden optisch verändert.
9.  Klicken Sie auf **[Speichern]**, um die Änderungen oder den neuen Filter zu speichern.
    Damit haben Sie den Filter konfiguriert oder angelegt und er steht in den jeweiligen Ansichten zur Verfügung.

Sie können die Filter mit den Schaltflächen **[Exportieren]** oder **[Importieren]** exportieren oder importieren und somit als Schablonen für andere Dialoge oder Anwender verwenden.

---
**A+W Production Grobplanung**
C-126, C-127, C-128
---

### Weißer Screen in einer Ansicht

Wenn in einer Ansicht keine Aufträge und/oder Positionen angezeigt werden, sind entweder keine vorhanden, oder Sie haben die Kriterien der Ansicht so gesetzt, dass keine Aufträge oder Positionen den Kriterien entsprechen. Mögliche Gründe für eine leere Liste sind beispielsweise:

- **Einzelne Spalte ohne Treffer:** Sie haben nur eine Spalte in der Ansicht. Der Spalte ist eine Kategorie hinterlegt, die nicht in den Aufträgen vorkommt.
  - Z. B. zeigt die Spalte VSG an und in den Aufträgen sind keine VSG enthalten.
  - **Abhilfe:** Hinterlegen Sie der Spalte ein Kriterium, das den Aufträgen entspricht.

- **Widersprüchliche Spaltenkriterien:** Sie haben mehrere Spalten in der Ansicht. Die Kriterien der Spalten grenzen die Aufträge so stark ein, dass keine mehr angezeigt werden, oder die Kriterien sind widersprüchlich.
  - Sie haben z. B. zwei Spalten, von denen eine VSG und die andere ISO anzeigt. Aufträge, die jeweils nur VSG oder ISO enthalten, können nicht beide Kriterien gleichzeitig erfüllen.
  - **Abhilfe:** Hinterlegen Sie den Spalten Kriterien, die den Aufträgen entsprechen.

- **Filter ohne Treffer:** Sie haben einen Filter aktiviert, dessen Kriterium keinem Auftrag entspricht.
  - Wenn z. B. ein Filter *nur ISO* aktiviert ist und keine ISO in den Aufträgen enthalten sind, ist die Liste leer.
  - **Abhilfe:** Entfernen Sie den Filter oder wählen Sie einen anderen.

- **Spalte für späteren Prozessschritt:** Sie haben eine Spalte eingefügt, die z. B. auf Lauf-bezogene Informationen filtert. Sofern Sie für die angezeigten Aufträge bzw. Positionen noch keinen Lauf gebildet haben, filtert die Spalte nicht vorhandene bzw. nicht zulässige Daten und damit entsteht ein weißer Screen.
  - **Abhilfe:** Fügen Sie Spalten für spätere Arbeitsprozesse in der Arbeitsvorbereitung auch nur in Ansichten ein, die spätere Prozesse der Arbeitsvorbereitung anzeigen, z. B. laufbezogene Daten in der Laufansicht.

---
**A+W Production Grobplanung**
C-129
---

### Übungen: Konfigurieren von und arbeiten mit Ansichten

Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
- Öffnen Sie eine Ansicht der Grobplanung.
- Aktivieren Sie die Speicherautomatik.
- Überlegen Sie, welche Informationen in dieser Ansicht noch fehlen.
- Legen Sie ein entsprechendes Register an.
- Legen Sie zugehörige Spalten an.
- Fügen Sie eine Summenzeile ein.
- Fügen Sie einen Filter ein.
- Definieren Sie eine eigene Spalte und/oder Summenzeile und fügen Sie diese in der Ansicht ein.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Grobplanung" auf Seite C-154

---
**A+W Production Grobplanung**
C-130
---

# Aufträge / Pool

**Lernziele**
- Wie arbeiten Sie mit der Ansicht Aufträge?

**Nutzen**
- In der Ansicht Aufträge haben Sie eine Übersicht über alle Aufträge, die aus dem ERP-System eingelastet wurden.
- Mit der Ansicht Aufträge gelangen Sie in andere Ansichten.

> **Merke**
> - **Aufträge**: Aufträge werden nach dem Import aus dem ERP-System im Dialog Aufträge angezeigt.
> - **Pool**: Der Dialog Aufträge wird auch Pool genannt.
> - **Auftragsübersicht**: Die Auftragsübersicht zeigt die Stückliste an.
> - **Positionen**: Im Dialog Positionen finden Sie alle Details zu den Positionen in Aufträgen.
> - **Füllaufträge**: Füllaufträge sind keinem Lauf zugeordnet und werden von der Feinplanung dazu verwendet, den Verschnitt zu optimieren.
> - **Übermengen**: Kaufmännische und produktionstechnische Übermengen bearbeiten Sie im Übermengen-Editor. (⇨ Softwarereferenz, “Übermengen-Editor" auf Seite C-165)
> - **Beschaffungsart ändern**: Im Dialog Änderung der Beschaffungsart können Sie die Beschaffungsart von ESG und VSG ändern. (⇨ Softwarereferenz, "Änderung der Beschaffungsart" auf Seite C-167)

---
**A+W Production Grobplanung**
C-131
---

## Aufträge in der Grobplanung

*Abb. C-12 Aufträge*

Im Dialog **Aufträge** haben Sie eine Übersicht über alle eingelasteten Aufträge, die noch nicht weiter verarbeitet wurden. Von dieser Ansicht aus können Sie die Aufträge im Prozess der Arbeitsvorbereitung weiter bearbeiten, z. B. Läufe und Töpfe bilden. Der Dialog Aufträge wird auch **Pool** genannt.

Aufgelöste Läufe und Töpfe landen automatisch wieder im Pool. Der Dialog Aufträge ist konfigurierbar.

Vom Pool aus gelangen Sie zur **Auftragsübersicht**, in der die Stückliste angezeigt wird. Sie können den **Übermengen-Editor** öffnen, in dem Sie produktionstechnische und kaufmännische Übermengen bearbeiten.
Zudem können Sie aus dem Pool heraus auf die Maschinenumlastung und die Maschinenzuordnung zugreifen.

Der Dialog Aufträge ist dazu gedacht, Ihnen einen Überblick über in den Aufträgen enthaltene Lieferdaten, Produkte und Bearbeitungen zu verschaffen. Halten Sie den Dialog Aufträge so einfach und übersichtlich wie möglich.
Wenn Sie Aufträge verplant haben, sind diese nicht mehr im Pool sichtbar. Sie finden die verplanten Aufträge dann in den anderen Ansichten, z. B. im Dialog Läufe. Legen Sie sich im Dialog Aufträge ein Register an, in dem Sie Kundendaten finden, z. B. Liefernamen, Lieferadressen und Routen.

> **Maschinenumlastung, -zuordnung und Kapazitätsplanung**
> Wenn Sie mit der Kapazitätsplanung arbeiten, müssen Sie Folgendes beachten:
> Eine erneute Maschinenumlastung oder Maschinenzuordnung aus der Grobplanung heraus hat Auswirkungen auf die geplanten und berechneten Kapazitäten.
> Die jeweiligen Funktionen sind im Handbuch der Kapazitätsplanung beschrieben.

### Aufträge mit fehlerhaften Angaben

Bei Aufträgen mit fehlenden oder fehlerhaften Angaben können Sie entweder die fehlerhaften Positionen oder den ganzen Auftrag bearbeiten. Entwoder Sie löschen die jeweiligen Aufträge oder Positionen, oder Sie schieben diese zurück in den Pool.

Entfernen Sie die fehlerhaften Positionen aus den Läufen, um sicher zu gehen, dass diese nicht weiter im System bleiben.

---
**A+W Production Grobplanung**
C-132 & C-133
---

# Töpfe

**Lernziele**
- Was ist ein Topf?
- Wie arbeiten Sie mit der Ansicht Töpfe?
- Wie wird ein Topf erstellt?

**Nutzen**
- Mit Töpfen können Sie Aufträge im Überblick behalten, die nicht sofort weiter verarbeitet werden.
- Mit Töpfen können Sie Puffer erstellen, in denen Sie z. B. Aufträge gleichen Typs sammeln.

> **Merke**
> - **Topf**: Ein Topf ist ein Speicher, in dem Sie Aufträge verwalten, bei denen das weitere Vorgehen unklar ist.
> - **Topf auflösen**: Aufträge aus aufgelösten Töpfen landen wieder im Pool.

---
**A+W Production Grobplanung**
C-134
---

## Töpfe in der Grobplanung

*Abb. C-13 Töpfe*

Im Dialog **Töpfe** haben Sie eine Übersicht über alle erstellten Töpfe in der Grobplanung. Ein Topf ist ein Speicher oder Puffer, in dem Sie Aufträge verwalten, bei denen die weitere Vorgehensweise noch nicht geklärt ist. Das kann z. B. dann der Fall sein, wenn Sie auf Auftragsänderungen, oder auf weitere Scheiben einer teuren Glasart warten.

Sie können Töpfe aus fast allen Übersichten heraus bilden oder Aufträge bestehenden Töpfen zuordnen. Die gebildeten Töpfe landen dann im Dialog **Töpfe**. Von dort aus können Sie die Töpfe verwalten, indem Sie z. B. Läufe bilden oder Töpfe auflösen. Aufträge aus aufgelösten Töpfen landen wieder im Pool.

Zur Arbeit mit Töpfen finden Sie folgende Handlungsanweisungen:
- "So erstellen Sie einen Topf" auf Seite C-136
- "So fügen Sie Aufträge einem bestehenden Topf hinzu" auf Seite C-137
- "So lösen Sie einen Topf auf" auf Seite C-139

### So erstellen Sie einen Topf

1.  Öffnen Sie die Ansicht, in der Sie einen Topf erstellen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontext-Menü der Aufträge, aus denen Sie einen Topf erstellen möchten und wählen Sie **Topf bilden**. Der Dialog **Topf-Bildung** wird geöffnet.
    *Abb. C-14 Aufträge - Kontextmenü Liste*
3.  Wählen Sie im Dropdown-Menü **Topf-Typ**, welchen Typ der Topf haben soll.
4.  AWP legt im Feld **Topf** einen neuen Topf an. Übernehmen Sie diese Bezeichnung, oder geben Sie einen eigenen Namen ein.
5.  Wählen Sie im Kalender-Feld **Produktionstermin** den Produktionsstart. Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss auf die Kapazitätsplanung hat.
6.  Tragen Sie im Feld **Produktionsschicht** ein, in welcher Schicht mit der Produktion begonnen werden soll. Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die Kapazitätsplanung hat.
7.  Wählen Sie im Feld **Artikeltyp-Filter**, ob für den Topf ein Artikeltyp-Filter hinterlegt wird.
8.  Wählen Sie mit der Checkbox **Auftrag zusammenhalten**, ob der Auftrag in der Produktion zusammen gehalten werden soll.
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Der Topf wurde gebildet und ist in der Ansicht **Töpfe** gelistet.

### So fügen Sie Aufträge einem bestehenden Topf hinzu

1.  Öffnen Sie die Ansicht, in der Sie Aufträge einem Topf hinzufügen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontext-Menü der Aufträge, die Sie einem Topf hinzufügen möchten, und wählen Sie **Topf bilden**. Der Dialog **Topf-Bildung** wird geöffnet.
    *Abb. C-15 Aufträge - Kontextmenü Liste*
3.  Wählen Sie im Dropdown-Menü **Topf-Typ**, welchen Typ der Topf haben soll.
4.  Wählen Sie im Feld **Topf** einen bestehenden Topf, um die Aufträge dem Topf hinzuzufügen.
5.  Wählen Sie im Kalender-Feld **Produktionstermin** den Produktionsstart. Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss auf die Kapazitätsplanung hat.
6.  Tragen Sie im Feld **Produktionsschicht** ein, in welcher Schicht mit der Produktion begonnen werden soll. Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die Kapazitätsplanung hat.
7.  Wählen Sie im Feld **Artikeltyp-Filter**, ob für den Topf ein Artikeltyp-Filter hinterlegt wird.
8.  Wählen Sie mit der Checkbox **Auftrag zusammenhalten**, ob der Auftrag in der Produktion zusammen gehalten werden soll.
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Die Aufträge wurden dem Topf hinzu gefügt.

### So lösen Sie einen Topf auf

1.  Wählen Sie **Stammdaten Anzeigen > Töpfe**.
2.  Öffnen Sie das Kontextmenü des Topfes oder der Töpfe, die Sie auflösen möchten und wählen Sie **Topf auflösen**. Die Aufträge befinden sich wieder im Pool.
    *Abb. C-16 Töpfe - Kontextmenü Liste*

---
**A+W Production Grobplanung**
C-135, C-136, C-137, C-138, C-139
---

# Läufe und Laufstrategien

**Lernziele**
- Was ist ein Lauf?
- Wie arbeiten Sie mit der Ansicht Läufe?
- Wie wird ein Lauf erstellt?
- Welche Strategien gibt es, um einen Lauf zu planen?

**Nutzen**
- In der Ansicht Läufe haben Sie einen Überblick über alle erstellten Läufe.
- In der Ansicht Läufe sehen Sie die Status der Läufe.
- In der Ansicht Läufe können Sie Läufe verwalten, indem Sie z. B. Status setzen, Läufe rücksetzen oder auflösen.
- In der Ansicht Läufe können Sie Läufe an die Feinplanung übergeben.

> **Merke**
> **Läufe** sind eine Gruppierung von Aufträgen und/oder Positionen, die im Prozess der Produktionsvorbereitung und Produktionsfreigabe gemeinsam bearbeitet werden sollen.
> Auf Basis der Läufe werden die Grobplanung, die Feinplanung, die Optimierung und die Lauffreigabe durchgeführt.

---
**A+W Production Grobplanung**
C-140
---

## Läufe in der Grobplanung

*Abb. C-17 Läufe*

Im Dialog **Läufe** haben Sie eine Übersicht über alle erstellten Läufe. Von dieser Ansicht aus können Sie Läufe im Prozess der Arbeitsvorbereitung weiter bearbeiten, indem Sie z. B. Läufe verlinken, auflösen oder an die Feinplanung übergeben.

Läufe sind eine Gruppierung von Aufträgen und/oder Positionen, die im Prozess der Produktionsvorbereitung und Produktionsfreigabe gemeinsam bearbeitet werden sollen. Auf Basis der Läufe werden die Feinplanung, die Optimierung und die Lauffreigabe durchgeführt.

Aufgelöste Läufe landen automatisch wieder im Pool. Der Dialog Läufe ist konfigurierbar. Sie können aus dem Dialog Läufe heraus z. B. auf die Maschinenumlastung zugreifen.

> **Maschinenumlastung, -zuordnung und Kapazitätsplanung**
> Wenn Sie mit der Kapazitätsplanung arbeiten, müssen Sie Folgendes beachten:
> Eine erneute Maschinenumlastung oder Maschinenzuordnung aus der Grobplanung heraus hat Auswirkungen auf die Kapazitätsplanung.
> Die jeweiligen Funktionen sind im Handbuch der Kapazitätsplanung beschrieben.

### Sinnvolle Läufe und Laufstrategien

Generell gilt: Eine Laufstrategie ist dann gut, wenn sie funktioniert. Mischen Sie unterschiedliche Scheibengrößen in einen Lauf, das verbessert die Ausbeute. Isolieren Sie keine speziellen Produkte, sondern nehmen Sie die speziellen Produkte mit in Läufe rein.

Sie können folgende Laufstrategien verfolgen:
- **Nach Glasart:** Sie können separate Läufe mit dicken Gläsern bilden. Dicke Gläser haben meist größere Abmessungen und damit einen schlechteren Ertrag, somit kann es von Vorteil sein, separate Läufe zu bilden und dicke Gläser dann zu produzieren, wenn es am besten in die Produktion passt.
- **Nach Produktart:** Bei komplexeren Produktionen, z. B. bei ISO, ESG oder VSG, kann es von Vorteil sein, Produktarten in Läufen zusammen zu fassen. Damit verschaffen Sie sich einen besseren Überblick über die Produktion und nehmen dabei eine schlechtere Ausbeute in Kauf.
- **Nach Bearbeitung:** Sie können Aufträge oder Positionen bearbeitungsorientiert zu Läufen zusammenfassen, z. B. um Rüstkosten und -zeiten zu minimieren.
- **Nach Produktionsdatum:** Die Kapazitätsplanung weist den einzelnen Bearbeitungen Produktions-Termine zu. Diese können Sie als Basis nehmen und aus den jeweiligen Bearbeitungen mit gleichem Datum Läufe bilden.
- **Nach Auftrag und/oder Position:** Sie können Läufe aus Positionen oder einzelnen Elementen von Aufträgen bilden. Bei mehrstufigen Produktionen hilft diese Strategie, die einzelnen Abteilungen zu organisieren. Wenn Sie Freiraum für Änderungen brauchen, können Sie verschiedene Produktarten eines Auftrags auf mehrere Läufe verteilen.
- **In mehreren Stufen planen:** Dabei trennen Sie Aufträge und/oder Positionen nach ihren Hauptkriterien und prüfen das Ergebnis. Je nach Ausbeute, Menge, Restplatten und Anzahl der benötigten Gestelle trennen Sie die Teile dann in einzelne Läufe oder fügen Teile Läufen hinzu.
- **Leerer Pool:** Bei dieser Strategie packen Sie neue Aufträge und/oder Positionen möglichst schnell in Töpfe oder Läufe. Der Vorteil dieser Strategie ist, dass Sie neue Aufträge und/oder Positionen sofort sehen, wenn Sie in den Pool kommen. Der Nachteil dieser Strategie ist, dass es schwieriger wird, den Überblick über bestehende Töpfe und Läufe zu behalten.
- **Voller Pool:** Sie lassen Aufträge und/oder Positionen möglichst lange im Pool. Der Vorteil dieser Strategie ist, dass Sie den vollen Überblick behalten. Der Nachteil dieser Strategie ist, dass Sie neue Aufträge und/oder Positionen schwerer bemerken.

> **Vorsicht bei Laufstrategien**
> A+W Production lässt Ihnen die volle Freiheit bei der Planung Ihrer Produktion und damit die volle Verantwortung.
> Sie können sich z. B. über Ergebnisse der Kapazitätsplanung hinweg setzen.

Sie sollten auf folgende Laufstrategien verzichten:
- Die morgigen kleineren Größen nutzen, um die heutige Ausbeute zu steigern. Diese Strategie führt zu Problemen am Folgetag.
- Zu viele Produkte oder Glasarten ohne die passende Organisation in den Läufen mischen. Diese Strategie führt zu einer unübersichtlichen Produktion und Staus.
- Eine zu kleine Menge an Standardgläsern.
- Läufe löschen, um Auftragsänderungen anzunehmen. Besser ist es Positionen oder Läufe zurück in den Pool zu schieben.

---
**A+W Production Grobplanung**
C-141 & C-142
---

### Arbeit mit Läufen

Zur Arbeit mit Läufen finden Sie folgende Handlungsanweisungen:
- "So bilden Sie einen Lauf" auf Seite C-143
- "So fügen Sie Aufträge einem bestehenden Lauf hinzu" auf Seite C-144
- "So verwalten Sie Läufe oder lösen Läufe auf" auf Seite C-146

#### So bilden Sie einen Lauf

1.  Öffnen Sie die Ansicht, in der Sie einen Lauf erstellen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontext-Menü der Aufträge, aus denen Sie einen Lauf erstellen möchten und wählen Sie **Lauf bilden**. Der Dialog **Lauf-Bildung** wird geöffnet.
    *Abb. C-18 Aufträge - Kontextmenü Liste*
3.  AWP legt im Feld **Lauf** automatisch eine neue Laufnummer an.
4.  Geben Sie im Feld **Bezeichnung** eine Bezeichnung für den Lauf ein.
5.  Wählen Sie im Kalender-Feld **Produktionstermin** den Produktionsstart. Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss auf die Kapazitätsplanung hat.
6.  Geben Sie im Feld **Produktionsschicht** ein, in welcher Schicht mit der Produktion begonnen werden soll. Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die Kapazitätsplanung hat.
7.  Wählen Sie im Feld **Artikeltyp-Filter**, ob für den Lauf ein Artikeltyp-Filter hinterlegt wird.
8.  Wählen Sie mit der Checkbox **Auftrag zusammenhalten**, ob der Auftrag in der Produktion zusammen gehalten werden soll.
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Der Lauf wurde gebildet und ist in der Ansicht **Läufe** gelistet.

#### So fügen Sie Aufträge einem bestehenden Lauf hinzu

1.  Öffnen Sie die Ansicht, in der Sie Aufträge einem Lauf hinzufügen möchten, z. B. **Anzeigen > Aufträge**.
2.  Öffnen Sie das Kontext-Menü der Aufträge, welche Sie einem Lauf hinzufügen möchten, und wählen Sie **Lauf bilden**. Der Dialog **Lauf-Bildung** wird geöffnet.
    *Abb. C-19 Aufträge - Kontextmenü Liste*
3.  Wählen Sie einen bestehenden Lauf im Dropdown-Menü um die Aufträge einem Lauf hinzuzufügen.
4.  Geben Sie im Feld **Bezeichnung** eine Bezeichnung für den Lauf ein.
5.  Wählen Sie im Kalender-Feld **Produktionstermin** den Produktionsstart. Beachten Sie dabei, dass ein geänderter Produktionstermin einen Einfluss auf die Kapazitätsplanung hat.
6.  Geben Sie im Feld **Produktionsschicht** ein, in welcher Schicht mit der Produktion begonnen werden soll. Beachten Sie dabei, dass eine geänderte Schicht einen Einfluss auf die Kapazitätsplanung hat.
7.  Wählen Sie im Feld **Artikeltyp-Filter**, ob für den Lauf ein Artikeltyp-Filter hinterlegt wird.
8.  Wählen Sie mit der Checkbox **Auftrag zusammenhalten**, ob der Auftrag in der Produktion zusammen gehalten werden soll.
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern. Die Aufträge wurden dem Lauf hinzu gefügt.

#### So verwalten Sie Läufe oder lösen Läufe auf

1.  Wählen Sie **Anzeigen > Läufe**.
2.  Öffnen Sie das Kontextmenü des Laufes oder der Läufe, die Sie bearbeiten oder auflösen möchten und wählen Sie die entsprechende Option im Kontextmenü. Der Lauf oder die Aufträge sind nun in den entsprechenden Ansichten zu finden.
    *Abb. C-20 Läufe - Kontextmenü Liste*

---
**A+W Production Grobplanung**
C-143, C-144, C-145, C-146
---

# Positionen

**Lernziele**
- Was sind Positionen?
- Wie arbeiten Sie mit der Ansicht Positionen?

**Nutzen**
- In der Ansicht Positionen haben Sie einen Überblick über Positionen in Aufträgen.

> **Merke**
> **Positionen** sind Teile von Aufträgen.

---
**A+W Production Grobplanung**
C-147
---

## Positionen in der Grobplanung

*Abb. C-21 Positionen*

Im Dialog **Positionen** haben Sie eine Übersicht über die Positionen von eingelasteten Aufträgen. Der Dialog Positionen ist konfigurierbar. Sie können jedoch aus der Ansicht heraus keine Läufe oder Töpfe bilden.

Positionen sind Teile von Aufträgen. Eine Position enthält verschiedene Teile, z. B. Float 4 mm und Therm 4 mm. An die Teile sind verschiedene Bearbeitungen geknüpft, z. B. Zuschnitt oder Polieren.

### Positionen splitten

Im Dialog **Positionssplit** können Sie Positionen aus Aufträgen nach verschiedenen Kriterien aufteilen. Sie können die Positionen in weitere Positionen aufteilen oder Positionen erzeugen, die eine bestimmte Anzahl von Scheiben enthalten. Außerdem können Sie die Positionen gemäß der Packmitteloptimierung aufteilen.

#### So splitten Sie eine Position

1.  Wählen Sie **Anzeigen > Aufträge > Kontextmenü auf die markierten Aufträge > Bearbeitungen > Kontextmenü > Positionen splitten**.
2.  Markieren Sie die Positionen (A), die Sie aufteilen wollen in der Liste **Markierte Positionen**.
3.  Wählen Sie die Option (B), mit der Sie aufteilen wollen.
4.  Klicken Sie auf die Schaltfläche **[Splitten]**. Die Positionen wurden aufgeteilt und stehen im Feld **Neue Positionen**.
5.  Klicken Sie auf die Schaltfläche **[Schließen]**, um den Dialog zu schließen.

---
**A+W Production Grobplanung**
C-148 & C-149
---

## Vorgang suchen

**Bearbeiten > Vorgang suchen**

*Abb. C-22 Vorgang suchen*

Hier haben Sie die Möglichkeit, Aufträge und/oder Angebote im System zu suchen. Wenn Sie den Dialog öffnen, ist dieser leer. Inhalte werden erst angezeigt, nachdem Sie die entsprechenden Auswahlen getroffen haben und die Schaltfläche Anzeigen betätigt haben.

Im ersten Schritt geben Sie im Bereich **Suche nach Vorgangsart** an, ob Sie nach einem Auftrag, einem Angebot oder nach beidem suchen möchten.

Anschließend müssen Sie im Bereich **Suchen nach ...** die entsprechende Vorgangsnummer (bei Auftrag oder Angebot) oder die gewünschte Kundennummer eingeben.

Im Bereich **Anzeigen nach** können Sie wählen, ob die Anzeige nach der Vorgangsnummer und der Position oder nach Läufen sortiert werden soll.

Im Bereich **Anzeigen von ...** haben Sie eine weitere Möglichkeit, die angezeigten Inhalte zu untergliedern. Sie können sich z.B. über die Radiotaste **Teilen** noch die entsprechenden Teile-Nummern anzeigen lassen. Die Radiotaste **Lauf** zeigt Ihnen den gesamten Lauf an.

---
**A+W Production Grobplanung**
C-150
---

# Softwarereferenz

## In diesem Kapitel finden Sie folgende Themen:

- Grobplanung
- Aufträge in der Grobplanung
- Töpfe in der Grobplanung
- Läufe in der Grobplanung
- Positionen in der Grobplanung
- Bearbeitungen in der Grobplanung
- Glasarten, Details, BDE und Lose
- Übergreifende Dialoge
- Übergreifende Kontextmenüs

## Inhaltsverzeichnis Softwarereferenz

| Thema | Seite |
| :--- | :--- |
| **Grobplanung** | **C-154** |
| **Aufträge in der Grobplanung** | **C-155** |
| Aufträge | C-156 |
| Auftragsübersicht | C-159 |
| Füllaufträge | C-162 |
| Übermengen-Editor | C-165 |
| Änderung der Beschaffungsart | C-167 |
| **Töpfe in der Grobplanung** | **C-169** |
| Töpfe | C-170 |
| Reservierungsaufträge-Topf | C-173 |
| Bestellteile-Topf | C-177 |
| Topf-Bildung | C-180 |
| Topfbezeichnung ändern | C-182 |
| **Läufe in der Grobplanung** | **C-183** |
| Läufe | C-184 |
| Lauf-Bildung | C-187 |
| Sonderglas-Lauf bilden | C-189 |
| Laufbezeichnung ändern | C-190 |
| Freigabe Lauf (Name): AUW – Wiederholung | C-191 |
| **Positionen in der Grobplanung** | **C-194** |
| Positionen | C-195 |
| Auftrag zu Positionen hinzufügen | C-198 |
| Positionssplit | C-199 |
| Felddefinition | C-201 |
| Export/Import Positionsansicht | C-203 |
| **Bearbeitungen in der Grobplanung** | **C-204** |
| Bearbeitungen | C-205 |
| Vorgabezeiten ändern | C-208 |
| **Glasarten, Details, BDE und Lose** | **C-209** |
| Glasarten | C-210 |
| Details | C-213 |
| BDE | C-217 |
| Lose | C-221 |
| **Übergreifende Dialoge** | **C-224** |
| Arbeitsplan | C-225 |
| Eigenschaften von (Register) | C-228 |
| Spaltendefinition | C-229 |
| (Filter Name) | C-230 |
| Filter-Definition | C-231 |
| Dokumentenverknüpfungen | C-233 |
| Entschichtungsflächen | C-234 |
| **Übergreifende Kontextmenüs** | **C-236** |

---
**A+W Production Grobplanung**
C-152 & C-153
---

# Grobplanung

In der Grobplanung bilden Sie Läufe, die Sie im Prozess der Produktionsvorbereitung anschließend feinplanen und optimieren. Die Laufgröße und -zusammensetzung entscheidet maßgeblich über die Optimierungsergebnisse und die Produktionsauslastung.

Nach der Einlastung der Aufträge finden Sie diese im Dialog **Aufträge**, der auch Pool genannt wird. Von dort aus können Sie die Aufträge in Töpfen vorsortieren oder direkt Läufe bilden. Mit den unterschiedlichen Ansichten verschaffen Sie sich einen Überblick über die Auftragsdaten und -details. Aus den Ansichten heraus bilden Sie Läufe und übergeben diese an den nächsten Prozessschritt in der Arbeitsvorbereitung: die Feinplanung.

Sie können die Ansichten der Grobplanung Ihren Bedürfnissen anpassen, damit diese genau die Informationen anzeigen, die Sie benötigen.

---
**A+W Production Grobplanung**
C-154
---

## Aufträge in der Grobplanung

In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie sich einen Überblick zu Aufträgen bzw. Auftragsdaten verschaffen können. Sie können Füllaufträge verwalten und Übermengen bearbeiten.

Das Kapitel enthält folgende Themen:
- "Aufträge" auf Seite C-156
- "Auftragsübersicht" auf Seite C-159
- "Füllaufträge" auf Seite C-162
- "Übermengen-Editor" auf Seite C-165

### Aufträge
**Anzeigen > Aufträge**
⇨ Bearbeitungen

*Abb. C-23 Aufträge - Summen (Beispiel)*

Im Dialog **Aufträge** haben Sie eine Übersicht über alle eingelasteten Aufträge, die noch nicht weiter verarbeitet wurden. Von dieser Ansicht aus können Sie die Aufträge im Prozess der Arbeitsvorbereitung weiter bearbeiten, z. B. Läufe und Töpfe bilden und Auftragsdetails aus verschiedenen Blickrichtungen anzeigen. Der Dialog Aufträge wird auch **Pool** genannt.

Folgende Bestandteile des Dialogs Aufträge können Sie frei konfigurieren:
- Register
- Spalten
- Summenzeile
- Filter

Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Das Register **Summen** enthält z. B. folgende Spalten:

- **Liefertermin:** Liefertermin für den Auftrag.
- **ESG Stk:** Anzahl der im Auftrag enthaltenen ESG.
- **Mod Stk:** Anzahl der im Auftrag enthaltenen Modelle.
- **Spr Stk:** Anzahl der im Auftrag enthaltenen Sprossen.
- **Sprossen produziert:** Anzahl der bereits für den Auftrag produzierten Sprossen.
- **Sprossen bestellt:** Anzahl der bereits für den Auftrag bestellten Sprossen.
- **3-fach:** Anzahl der im Auftrag enthaltenen 3-fach-ISO.
- **Stufen:** Anzahl der im Auftrag enthaltenen Stufen-ISO.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Summenzeile
- **Stück Endprodukt:** Stückzahl der markierten Endprodukte, z. B. ISO oder VSG.
- **ISO Stk:** Anzahl der markierten ISO bei Mehrfachauswahl.
- **nur Zuschnitt:** Summe aller Scheiben, die geschnitten werden müssen.

#### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
  - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
  - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche Verwalten gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
    ⇨ "Filter-Definition" auf Seite C-231

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Aufträge** werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| Liste | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog Umlastung zur Maschinenumlastung. ⇨ Kapazitätsplanung: Softwarereferenz, “Maschinenumlastung" auf Seite E-618 |
| | Arbeitsplan > Maschinen-Zuordnung | Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. Führt die Maschinenzuordnung für markierte Aufträge erneut durch. |
| | Arbeitsplan > Arbeitsplan neu berechnen | Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. Zur Zeit nicht genutzt. |
| | Beschaffungsart ändern | Öffnet den Dialog Änderung der Beschaffungsart. ⇨ "Änderung der Beschaffungsart" auf Seite C-167. Die Option funktioniert ausschließlich bei ESG und VSG. |

*Tab. C-2 Aufträge, Kontextmenüs*

#### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Aufträgen, Positionen oder Teilen einen Lauf.
- **[Glasarten]:** Zeigt die Glasarten der markierten Aufträge an.
- **[Details]:** Zeigt die Details der markierten Aufträge an.

---
**A+W Production Grobplanung**
C-156, C-157, C-158
---

### Auftragsübersicht

- **Anzeigen > Aufträge > Kontextmenü > Bearbeitungen > Kontextmenü > Auftragsübersicht**
- **Anzeigen > Aufträge > Kontextmenü > Glasarten > Kontextmenü > Auftragsübersicht**
- **Anzeigen > Aufträge > Kontextmenü > Details > Kontextmenü > Auftragsübersicht**
- **Anzeigen > Töpfe > Kontextmenü > Auftragsübersicht**
- **Anzeigen > Läufe > Kontextmenü > Auftragsübersicht**
- **Anzeigen > Füllaufträge > Kontextmenü > Auftragsübersicht**

*Abb. C-24 Auftragsübersicht, geordnet nach Bearbeitungen (Beispiel)*

Im Dialog **Auftragsübersicht** haben Sie eine Übersicht über Details in Aufträgen. Sie können die Auftragsübersicht nach Positionen, Teilen oder Bearbeitungen ordnen. Zudem können Sie Rahmen und Folien ein- oder ausblenden.
Aus dem Dialog Auftragsübersicht heraus können Sie keine Läufe oder Töpfe erstellen.

Sie können die Register und Spalten im Dialog Auftragsübersicht nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen.
Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

- **[Speicherautomatik]:** Aktiviert automatisches Speichern.
- **[Speichern]:** Speichert die aktuellen Daten.
- **[Systemweite Anzeige]:** Änderungen im Dialog Auftragsübersicht werden systemweit gespeichert.

Der Dialog Auftragsübersicht enthält z. B. folgende Informationen:
- **Auftrag:** Auftrag, zu dem Details angezeigt werden.
- **[Positionen]:** Ordnet die Ansicht nach Positionen.
- **[Teile]:** Ordnet die Ansicht nach Teilen.
- **[Bearbeitungen]:** Ordnet die Ansicht nach Bearbeitungen.
- **Rahmen, Folien anzeigen:** Checkbox mit folgenden Funktionen:
  - Bearbeitungen, die Rahmen und Folien enthalten, werden nicht angezeigt.
  - Bearbeitungen, die Rahmen und Folien enthalten, werden angezeigt.
- **Position:** Positionsnummer der Auftragsposition.
- **Name:** Artikel oder Auftragsposition.
- **Größe:** Größe der Scheiben.
- **Stückzahl:** Stückzahl der Artikel.
- **Maschine:** Maschine, auf der die Bearbeitung durchgeführt wird.
- **Prod.-Termin:** Datum, an dem die Bearbeitung durchgeführt wird.
- **Prod. Stückzahl:** Zahl der bereits produzierten Scheiben.
- **Lauf:** Lauf, dem die Bearbeitung zugeordnet wurde.
- **Beschaffungsart:** Beschaffungsart, die dem Artikel zugeordnet wurde.
- **Modellnummer:** Modellnummer der Scheibe.
- **Bearbeitungstext:** Anmerkungen zur Bearbeitung.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option Definition anzeigen öffnen Sie den Dialog Spaltendefinition. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Auftragsübersicht** werden Kontextmenüs angeboten: Schaltflächen-Leiste, Kopfzeile, Spalten.

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| **Kopfzeile** | Formatieren | Format oder Einheit für die Spalten in der Kopfzeile auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| | Einfügen | Fügt eine neue Spalte in die Kopfzeile ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Entfernen | Entfernt eine markierte Spalte. |
| | Definition anzeigen | Öffnet den Dialog Spaltendefinition. ⇨ "Spaltendefinition" auf Seite C-229 |
| **Spalten** | Formatieren | Format oder Einheit für die Spalten in der Liste auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| | Einfügen > Bearbeitungsdaten | Fügt eine neue Spalte mit Bearbeitungsdaten ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Stücklistendaten | Fügt eine neue Spalte mit Stücklistendaten ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Entfernen | Löscht eine markierte Spalte. |
| | Definition anzeigen | Öffnet den Dialog Spaltendefinition, in dem Details zur jeweiligen Spalte angezeigt werden. ⇨ "Spaltendefinition" auf Seite C-229 |

*Tab. C-3 Auftragsübersicht, Kontextmenüs*

---
**A+W Production Grobplanung**
C-159, C-160, C-161
---

### Füllaufträge
**Anzeigen > Füllaufträge**

*Abb. C-25 Füllaufträge (Beispiel)*

Im Dialog **Füllaufträge** haben Sie eine Übersicht über alle Füllaufträge. Sie können sich z. B. anzeigen lassen, wie viele Positionen der Füllaufträge bereits produziert sind und wie viele noch produziert werden müssen.

Folgende Bestandteile des Dialogs Füllaufträge können Sie frei konfigurieren:
- Register
- Spalten
- Summenzeile
- Filter

Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
Der Dialog Füllaufträge enthält z. B. folgende Spalten:

- **Auftrag:** Auftragsnummer des jeweiligen Auftrags.
- **Pos (int Pos):** Interne A+W Production Sub-Position, die z. B. nach einem Positionssplit vergeben wurde.
- **Artikelbezeichnung:** Bezeichnung des im Auftrag enthaltenen Artikels.
- **Produzierte Menge:** Anzahl der bereits produzierten Positionen des jeweiligen Auftrags.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Summenzeile
- **Stück Endprodukt:** Anzahl der markierten Endprodukte, z. B. ISO oder VSG.
- **ISO Stk:** Anzahl der markierten ISO.
- **nur Zuschnitt:** Anzahl der markierten Scheiben, die geschnitten werden müssen.

#### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
  - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
  - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
    ⇨ "Filter-Definition" auf Seite C-231

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Füllaufträge** werden Kontextmenüs angeboten: Register, Spalten, Liste, Summenzeile, Filter.
Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel **Übergreifende Kontextmenüs** gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| Liste | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog Umlastung zur Maschinenumlastung. ⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618 |
| | Arbeitsplan > Maschinen-Zuordnung | Führt die Maschinenzuordnung für markierte Aufträge bzw. Positionen erneut durch. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Arbeitsplan neu berechnen | Zur Zeit nicht genutzt. |
| | Beschaffungsart ändern | Öffnet den Dialog Änderung der Beschaffungsart. ⇨ "Änderung der Beschaffungsart" auf Seite C-167. Die Option funktioniert ausschließlich bei ESG und VSG. |

*Tab. C-4 Füllaufträge, Kontextmenüs*

#### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Aufträgen, Positionen oder Teilen einen Lauf.
- **[Glasarten]:** Zeigt die Glasarten der markierten Aufträge an.
- **[Details]:** Zeigt die Details der markierten Aufträge an.

---
**A+W Production Grobplanung**
C-162, C-163, C-164
---

### Übermengen-Editor
**Anzeigen > Aufträge > Kontextmenü > Nacherfassung > Übermengen**

*Abb. C-26 Übermengen-Editor*

Im Dialog **Übermengen-Editor** können Sie kaufmännische und produktionstechnische Übermengen in Aufträgen bearbeiten.

#### Auftragspositionen
- **Auftrag:** Nummer des Auftrags.
- **Pos:** Anzahl der im Auftrag enthaltenen Positionen.
- **Produkt:** Produktbezeichnung aus den Produktstammdaten.
- **Menge laut Auftrag:** Menge, die in der Bestellung angegeben wurde.
- **Übermenge:** Kaufmännische Übermenge, die Sie ändern können.
- **Mehrmenge:** Produktionstechnische Mehrmenge, die Sie ändern können.
- **Gesamtmenge:** Gesamtmenge der Positionen, nachdem Sie die Übermengen und Mehrmengen geändert haben.

#### Übersicht
- **Anzeige des Scheibenaufbaus.**
- **Modell:** Anzeige der Form des markierten Produkts.

#### Schaltflächen
- **[Speichern]:** Speichert die Daten.
- **[Beenden]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-165 & C-166
---

### Änderung der Beschaffungsart

**Anzeigen > Aufträge > Kontextmenü > Beschaffungsart ändern**
**Anzeigen > Füllauftr. > Kontextmenü > Beschaffungsart ändern**

*Abb. C-27 Änderung der Beschaffungsart*

Im Dialog **Änderung der Beschaffungsart** können Sie die Beschaffungsart von ESG und VSG ändern.

#### Änderbare Teile
Liste der Teile, deren Beschaffungsart Sie ändern können.

#### Details
- **Auftragsnummer:** Auftragsnummer des markierten Teils.
- **Positionsnummer:** Positionsnummer des markierten Teils.
- **Artikelbezeichnung:** Bezeichnung des markierten Teils.
- **Stück:** Anzahl der enthaltenen Teile.
- **Produktionsdatum:** Produktionsbeginn der Teile.
- **Aktuelle Beschaffungsart:** Aktuell definierte Beschaffungsart.
- **Aufbau:** Enthaltene Scheiben, für die Sie die Beschaffungsart ändern können.

- **[Pfeil nach unten]:** Bewegt markierte Teile ins Feld **Ausgewählte Teile**.
- **[Pfeil nach oben]:** Bewegt markierte Teile zurück ins Feld **Änderbare Teile**.

#### Ausgewählte Teile
Liste der ausgewählten Teile.

#### Auswahl der neuen Beschaffungsart
Auswahl der neuen Beschaffungsart, Sie wählen zwischen **Zuschnitt, Produktion, Bestellung** oder **Lagerentnahme**.

- **[Ausführen]:** Führt die Änderung der Beschaffungsart durch.
- **[Schließen]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-167 & C-168
---

## Töpfe in der Grobplanung

In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie sich zu Töpfen einen Überblick verschaffen. Sie können Töpfe bilden und bearbeiten und Reservierungsaufträge verwalten.

Das Kapitel enthält folgende Themen:
- "Töpfe" auf Seite C-170
- "Reservierungsaufträge-Topf" auf Seite C-173
- "Topf-Bildung" auf Seite C-180
- "Topfbezeichnung ändern" auf Seite C-182

### Töpfe
**Anzeigen > Töpfe**
Zu Dialogbeschreibung: ⇨ Reservierungsaufträge-Topf

*Abb. C-28 Töpfe - Töpfe (Beispiel)*

Im Dialog **Töpfe** haben Sie eine Übersicht über die Töpfe in A+W Production. Sie können die Töpfe nach unterschiedlichen Kriterien sortieren und bearbeiten.

Folgende Bestandteile des Dialogs Töpfe können Sie frei konfigurieren:
- Register
- Spalten
- Summenzeile
- Filter

Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
Das Register **Töpfe** enthält z. B. folgende Spalten:

- **Topf:** Bezeichnung des Topfs.
- **Beschreibung:** Beschreibung des Topfs.
- **Aufträge:** Anzahl der enthaltenen Aufträge im jeweiligen Topf.
- **Positionen:** Anzahl der enthaltenen Positionen im jeweiligen Topf.
- **ISO:** Anzahl der enthaltenen ISO im jeweiligen Topf.
- **VSG:** Anzahl der enthaltenen VSG im jeweiligen Topf.
- **ESG:** Anzahl der enthaltenen ESG im jeweiligen Topf.
- **Modelle:** Anzahl der enthaltenen Modelle im jeweiligen Topf.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Summenzeile
- **Summe Fläche:** Gesamtfläche aller Positionen.
- **Summe ISO:** Anzahl der enthaltenen ISO.
- **Summe ESG:** Anzahl der enthaltenen ESG.

#### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
  - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
  - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
    "Filter-Definition" auf Seite C-231

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Töpfe** werden Kontextmenüs angeboten: Register, Spalten, Liste, Summenzeile, Filter.
Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel **Übergreifende Kontextmenüs** gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| Liste | Topf auflösen | Löst die markierten Töpfe auf und schiebt die enthaltenen Aufträge zurück in den Dialog **Aufträge**. |
*Tab. C-5 Töpfe, Kontextmenüs*

#### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Aufträgen, Positionen oder Teilen einen Lauf.
- **[Glasarten]:** Zeigt die Glasarten der markierten Töpfe an.
- **[Details]:** Zeigt die Details der markierten Töpfe an.

> **Späte Übernahme produktionsirrelevanter Daten**
> Teile, die bereits in Töpfe eingeplant sind, werden bei der späten Übernahme von nicht produktionsrelevanter Daten in den Töpfen belassen. Mit dem Schalter **Geänderte Positionen aus Töpfen entfernen** im Parameter-Administrator steuern Sie, wie mit den Teilen einer geänderten Position verfahren werden soll. Mögliche Werte sind:
> 0: Teile bleiben in den Töpfen (Standard)
> 1: Werden Änderungen auf Auftragsebene übernommen, dann werden die Teile aus den Töpfen entfernt.

---
**A+W Production Grobplanung**
C-170, C-171, C-172
---

### Reservierungsaufträge-Topf
**Anzeigen > Reservierungsaufträge-Topf**

*Abb. C-29 Reservierungsaufträge-Topf (Beispiel)*

Im Dialog **Reservierungsaufträge-Topf** können Sie sich Reservierungsaufträge anzeigen lassen. Der Dialog dient lediglich als Übersicht über die eingeplanten Kapazitäten, sie können aus dem Dialog heraus keine Läufe oder Töpfe bilden.

Der Dialog **Reservierungsaufträge-Topf** ist in AWP nicht standardmäßig freigeschaltet, Sie müssen die Ansicht des Dialogs zuerst aktivieren.

Sie können die Register und Spalten im Dialog **Reservierungsaufträge-Topf** nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen.

Der Dialog **Reservierungsaufträge-Topf** enthält z. B. folgende Spalten:
- **Auftragsnummer:** Angabe der Auftragsnummer.
- **Laufnummer:** Angabe der Laufnummer.
- **Liefertermin:** Angabe des Liefertermins.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Summenzeile
**Stück:** Anzahl der Positionen, der im Dialog angezeigten Aufträge.

#### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
  - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
  - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
    ⇨ "Filter-Definition" auf Seite C-231

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Glasarten** werden Kontextmenüs angeboten: Spalten, Liste, Summenzeile, Filter.
Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel **Übergreifende Kontextmenüs** gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| **Spalten** | Umsortieren | Spalte aufsteigend oder absteigend sortieren. Wirkt sich auf die ersten drei Spalten im Dialog aus. |
| | Formatieren | Format oder Einheit für die Spalten auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| | Einfügen | Fügt eine neue Spalte ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Felddefinition > Editieren | Öffnet den Dialog, in dem Sie Abfragen auf Datenbank-Tabellen und -Felder formulieren können. Diese Abfragen können Sie dann z. B. teile-, positions- oder auftragsbezogen als Spalte einfügen. ⇨"Felddefinition" auf Seite C-201 |
| | Einfügen > Felddefinition > Importieren | Öffnet den Dialog Importieren von Felddefinitionen. |
| | Einfügen > Felddefinition > Exportieren | Öffnet den Dialog Exportieren von Felddefinitionen, mit dem Sie Felddefinitionen exportieren können. |
| | Entfernen | Löscht die markierte Spalte. |
| | Ändern | Derzeit nicht genutzt. |
| | Definition anzeigen | Öffnet den Dialog Spaltendefinition, in dem Details zur jeweiligen Spalte angezeigt werden. ⇨ "Spaltendefinition" auf Seite C-229 |
| **Liste** | Auftragsübersicht | Öffnet den Dialog Auftragsübersicht. ⇨ "Auftragsübersicht" auf Seite C-159 |
| | Positionen | Öffnet den Dialog Positionen. ⇨ "Positionen" auf Seite C-195 |
| **Summenzeile** | Umsortieren | Zur Zeit nicht genutzt. |
| | Formatieren | Format oder Einheit für die Spalten auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| | Einfügen | Fügt ein neues Feld in die Summenzeile ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Felddefinitionen > Editieren | Öffnet den Dialog Felddefinition, in dem Sie Abfragen auf Datenbank-Tabellen und -Felder formulieren können. Diese Abfragen können Sie dann z. B. teile-, positions- oder auftragsbezogen einfügen. ⇨"Felddefinition" auf Seite C-201 |
| | Einfügen > Felddefinitionen > Importieren | Öffnet den Dialog Importieren von Felddefinitionen. |
| | Einfügen > Felddefinitionen > Exportieren | Öffnet den Dialog Exportieren von Felddefinitionen, mit dem Sie Felddefinitionen exportieren können. |
| **Filter** | (Filterauswahl) | Öffnet den Dialog (Filter Name). Mit der Schaltfläche [Verwalten] gelangen Sie zum Dialog Filter-Definition, in dem Sie Filter bearbeiten können. ⇨"Filter-Definition" auf Seite C-231 |

*Tab. C-6 Reservierungsaufträge-Topf, Kontextmenüs*

#### Schaltflächen
- **[Laufbildung]:** Zur Zeit nicht aktiv.
- **[Glasarten]:** Zur Zeit nicht aktiv.
- **[Details]:** Zur Zeit nicht aktiv.

---
**A+W Production Grobplanung**
C-173, C-174, C-175, C-176
---

### Bestellteile-Topf
**Anzeigen > Bestellteile-Topf**

*Abb. C-30 Bestellteile-Topf (Beispiel)*

Im Dialog **Bestellteile-Topf** haben Sie eine Übersicht über Töpfe, die mit Bestellteilen erstellt wurden.

Sie können die Register und Spalten im Dialog **Bestellteile-Topf** nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen.

Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.
Der Dialog **Bestellteile-Topf** enthält z. B. folgende Spalten:

- **Auftrag:** Nummer des Auftrags.
- **Artikel:** Nummer des Artikels.
- **Liefertermin:** Termin, an dem ausgeliefert wird.
- **Artikelbezeichnung:** Bezeichnung des Artikels.
- **Liefername:** Name des Kunden.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Summenzeile
- **Summe Stück:** Summe der Teile in den markierten Aufträgen bzw. Positionen.
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.

#### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
  - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
  - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
    "Filter-Definition" auf Seite C-231

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Bestellteile-Topf** werden Kontextmenüs angeboten: Register, Spalten, Liste, Summenzeile, Filter.
Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel **Übergreifende Kontextmenüs** gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| Liste | Verschieben in Pool | Schiebt die ausgewählten Aufträge zurück in den Dialog **Aufträge** und damit in den Status vor der Grobplanung. ⇨ "Aufträge" auf Seite C-156 |
| | Arbeitsplan > Maschinen-Zuordnung | Führt die Maschinenzuordnung für markierte Aufträge erneut durch. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Arbeitsplan neu berechnen | Zur Zeit nicht aktiv. |
| | Nachläufer-bestellungen > Auslösen | Zur Zeit nicht aktiv. |
| | Nachläufer-bestellungen > Nicht auslösen | Zur Zeit nicht aktiv. |

*Tab. C-7 Bestellteiletopf, Kontextmenüs*

#### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Bestellteilen einen Lauf.
- **[Glasarten]:** Zur Zeit nicht aktiv.
- **[Details]:** Zur Zeit nicht aktiv.

---
**A+W Production Grobplanung**
C-177, C-178, C-179
---

### Topf-Bildung

- **Anzeigen > Aufträge > Kontextmenü > Topf bilden**
- **Anzeigen > Töpfe > Kontextmenü > Topf bilden**
- **Anzeigen > Läufe > Kontextmenü > Topf bilden**
- **Anzeigen > Füllaufträge > Kontextmenü > Topf bilden**
- **Glasarten > Kontextmenü > Topf bilden**
- **Bearbeitungen > Kontextmenü > Topf bilden**
- **Details > Kontextmenü > Topf bilden**

*Abb. C-31 Topf-Bildung*

Mit dem Dialog **Topf-Bildung** können Sie einen Topf bilden. Dieser wird im Dialog **Töpfe** angezeigt. Sie können Töpfe als Zwischenspeicher nutzen, z. B. wenn nicht genug Aufträge des gleichen Typs vorhanden sind.

- **Topf-Typ:** Auswahl des Topf-Typs:
  - Normal
  - Bestellteiltopf
- **Topf:** Sie können einen neuen Topf bilden oder den Auftrag einem bestehenden Topf hinzufügen.
  - Wenn Sie keine Änderungen vornehmen, wird ein neuer Topf gebildet.
  - Wenn Sie einen Topf aus der Auswahl-Liste wählen, wird der Auftrag einem bestehenden Topf hinzugefügt.
- **Bezeichnung:** Bezeichnung des Topfs.
- **Produktionstermin:** Auswahl des Produktionstermins für den Lauf.
- **Produktionsschicht:** Angabe der Schicht, in der der Lauf gestartet werden soll.
- **Artikeltyp-Filter:** Auswahl, für welche Teile Sie den Topf bilden. Zur Auswahl stehen: Sprossen, Folie, Rahmen oder Sonstige Nicht-Glas-Artikel. Die Teile müssen für die weitere Bearbeitung als Freigabeteile in den Artikelstammdaten angelegt sein.
- **Auftrag zusammenhalten:** Sie können die Positionen des Auftrags zusammen halten. Das heißt, alle Positionen – also auch die, die Sie nicht explizit ausgewählt haben, werden gemeinsam durch die Produktion geführt. Damit stellen Sie sicher, dass keine Positionen des Auftrags vergessen werden.
  - Die Positionen des Auftrags werden nicht zusammen gehalten.
  - Die Positionen des Auftrags werden zusammen gehalten.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-180 & C-181
---

### Topfbezeichnung ändern
**Anzeigen > Töpfe > Kontextmenü > Text ändern**

*Abb. C-32 Topfbezeichnung ändern*

Mit dem Dialog **Topfbezeichnung ändern** können Sie die Bezeichnung, den Produktionstermin und die Produktionsschicht eines Topfs ändern.

- **Topf:** Bezeichnung des Topfs.
- **Bezeichnung:** Bezeichnung des Topfs.
- **Produktionstermin:** Auswahl des Produktionsstarts für den Topf.
- **Produktionsschicht:** Angabe der Schicht, in der der Topf gestartet werden soll.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-182
---

## Läufe in der Grobplanung

In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie sich zu Läufen einen Überblick verschaffen. Sie können Läufe bilden und bearbeiten, Sonderglas-Läufe bilden und Läufe freigeben, die somit für die Produktion freigegeben werden.

Das Kapitel enthält folgende Themen:
- "Läufe" auf Seite C-184
- "Lauf-Bildung" auf Seite C-187
- "Sonderglas-Lauf bilden" auf Seite C-189
- "Laufbezeichnung ändern" auf Seite C-190

### Läufe
**Anzeigen > Läufe**
Zu Dialogbeschreibung: ⇨ Freigabe Lauf (Name): AUW – Wiederholung

*Abb. C-33 Läufe (Beispiel)*

Im Dialog **Läufe** haben Sie eine Übersicht über die erstellten Läufe. Läufe sind eine Gruppierung von Aufträgen bzw. Positionen, die im Prozess der Produktionsvorbereitung und Produktionsfreigabe gemeinsam bearbeitet werden sollen. Auf Basis der Läufe werden die Grobplanung, die Feinplanung, die Optimierung und die Lauffreigabe durchgeführt.

Sie können die Läufe nach unterschiedlichen Kriterien sortieren und bearbeiten. Die Steuerung des Dialogs **Läufe** erfolgt vorrangig über Kontextmenüs. Folgende Bestandteile des Dialogs **Läufe** können Sie frei konfigurieren:
- Register
- Spalten
- Summenzeile
- Filter

Das Register **Läufe** enthält z. B. folgende Spalten:

- **Lauf:** Bezeichnung des Laufs.
- **Status:** Status des Laufs.
- **Anzahl:** Anzahl der enthaltenen Aufträge im jeweiligen Lauf.
- **Modelle:** Anzahl der enthaltenen Modelle im jeweiligen Lauf.
- **Beschreibung:** Beschreibung des Laufs.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Summenzeile
In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen, Sie bekommen z. B. folgende Informationen angezeigt:
- **Modelle:** Summe der Modelle in den Aufträgen bzw. Positionen.
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.
- **Summe Stück:** Summe der Teile in den markierten Aufträgen bzw. Positionen.

#### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
  - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
  - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
    "Filter-Definition" auf Seite C-231

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Läufe** werden Kontextmenüs angeboten: Register, Spalten, Liste, Summenzeile, Filter.
Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel **Übergreifende Kontextmenüs** gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| Liste | Lauf freigeben | Markierte Läufe zur Produktion freigeben. |
| | Lauf verwalten > Lauf rücksetzen | Der Laufstatus wird zurückgesetzt. |
| | Lauf verwalten > Lauf auflösen | Der Lauf wird aufgelöst. Die Auftragsdaten gehen wieder in den Pool. |
| | Lauf verwalten > Lauf archivieren | Der Lauf wird archiviert. Die Erstellung der Archiv-Ansicht erfolgt durch den Service der A+W Software GmbH. |
| | Lauf verwalten > Status setzen | Öffnet den Dialog Status setzen, in dem Sie den Status des Laufs wählen: in Produktion, produziert, versandfertig, ausgeliefert. |
| | Feinplanung | Übergibt den Lauf an die Feinplanung und öffnet den Dialog Feinplanung für Lauf (Name). |
| | Sprossen-Druck | Startet den Druck von Produktionspapieren für Sprossen. |
| | Sprossen Maschinen-Ansteuerung | Übergibt die Produktionsdaten für Sprossen an die jeweiligen Maschinen. |
| | Maschinen-Umlastung | Öffnet den Dialog Umlastung zur Maschinenumlastung. ⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |

*Tab. C-8 Läufe, Kontextmenüs*

#### Schaltflächen
- **[Freigabe]:** Gibt die markierten Läufe zur Produktion frei.
- **[Feinplan.]:** Übergibt den markierten Lauf an die Feinplanung und öffnet den Dialog Feinplanung für Lauf (Name).
- **[Glasarten]:** Zeigt die Glasarten der markierten Läufe an.
- **[Details]:** Zeigt die Details der markierten Läufe an.

---
**A+W Production Grobplanung**
C-183, C-184, C-185, C-186
---

### Lauf-Bildung

- **Anzeigen > Aufträge > [Lauf]**
- **Anzeigen > Töpfe > [Lauf]**
- **Anzeigen > Läufe > Kontextmenü > Lauf bilden**
- **Anzeigen > Füllaufträge > [Lauf]**
- **Glasarten > [Lauf]**
- **Bearbeitungen > [Lauf]**
- **Details > [Lauf]**
- **Lose > [Lauf]**
- **BDE > [Lauf]**

Sie können den Dialog **Lauf-Bildung** jeweils auch über das Kontextmenü öffnen.

*Abb. C-34 Lauf-Bildung*

Mit dem Dialog **Lauf-Bildung** können Sie einen Lauf bilden, oder Aufträge zu einem bestehenden Lauf hinzufügen. Der Lauf erscheint dann im Dialog **Läufe**.
"Läufe" auf Seite C-184

- **Lauf:** Sie können einen neuen Lauf bilden, oder den Auftrag einem bestehenden Lauf hinzufügen.
  - Wenn Sie keine Änderungen vornehmen, wird ein neuer Lauf gebildet.
  - Wenn Sie einen Lauf aus der Auswahl-Liste wählen, wird der Auftrag einem bestehenden Lauf hinzugefügt.
- **Bezeichnung:** Bezeichnung des Laufs.
- **Feinplanungs-Orga:** Definiert, welche Abstellplatz-Organisation für die Optimierung des Laufs verwendet wird. Sie können diese Voreinstellung beim Arbeitsschritt **Feinplanung** ändern.
- **Ausgewählte Orga zur Standardvorgabe machen:** Im Feld Feinplanungs-Orga gewählte Abstellplatz-Organisation zum Standard machen.
  - Gewählte Abstellplatz-Organisation wird nicht Standard.
  - Gewählte Abstellplatz-Organisation wird Standard.
- **Produktionstermin:** Hier wählen Sie einen Produktions-Starttermin für den Lauf. Wenn Sie mit dem A+W Capacity Planner arbeiten, können Sie hier den errechneten Starttermin bestätigen oder diesen bewusst ändern.
- **Produktionsschicht:** Angabe, in welcher Schicht die Produktion des Laufs gestartet wird.
- **Artikeltyp-Filter:** Sie können spezielle Läufe für Sprossen, ISO-Rahmen, VSG-Folie und sonstige Nicht-Glasartikel bilden. Die Läufe werden nur aus den gewählten Artikeltypen gebildet. Für diese Option müssen die Artikeltypen in den Artikelstammdaten als Freigabeteile definiert werden.
- **Auftrag zusammenhalten:** Sie können die Positionen des Auftrags zusammenhalten. Das heißt, alle Positionen – also auch die, die Sie nicht explizit ausgewählt haben, werden gemeinsam durch die Produktion geführt. Damit stellen Sie sicher, dass keine Positionen des Auftrags vergessen werden.
  - Die Positionen des Auftrags werden nicht zusammen gehalten.
  - Die Positionen des Auftrags werden zusammen gehalten.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-187 & C-188
---

### Sonderglas-Lauf bilden
**Glasarten > Kontextmenü > Sonderglas > Hinzufügen**

*Abb. C-35 Sonderglas-Lauf bilden*

Im Dialog **Sonderglas-Lauf bilden** können Sie Läufe speziell für Sonderglas bilden.

- **Sonderglas-Lauf:** Sie können entweder einen neuen Sonderglas-Lauf bilden oder den Auftrag einem bestehenden Sonderglas-Lauf hinzufügen.
  - Wenn Sie keine Änderungen vornehmen, wird ein neuer Sonderglas-Lauf gebildet.
  - Wenn Sie einen Sonderglas-Lauf aus der Auswahl-Liste wählen, wird der Auftrag einem bestehenden Lauf hinzugefügt.
- **Bezeichnung:** Angabe der Bezeichnung des neuen Sonderglas-Laufs.
- **Feinplanungs-Orga:** Auswahl der Gestelle für den Sonderglas-Lauf.
- **Produktionstermin:** Auswahl des Produktionstermins für den Lauf.
- **Produktionsschicht:** Angabe der Schicht, in der der Lauf gestartet werden soll.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-189
---

### Laufbezeichnung ändern
**Anzeigen > Läufe > Kontextmenü > Text ändern**

*Abb. C-36 Laufbezeichnung ändern*

Mit dem Dialog **Laufbezeichnung ändern** können Sie die Bezeichnung, den Produktionstermin und die Produktionsschicht eines Laufs ändern.

- **Lauf:** Ausgewählter Lauf.
- **Bezeichnung:** Bezeichnung des Laufs.
- **Produktionstermin:** Auswahl des Produktionstermins für den Lauf.
- **Produktionsschicht:** Auswahl der Schicht, in der der Lauf gestartet werden soll.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

---
**A+W Production Grobplanung**
C-190
---

### Freigabe Lauf (Name): AUW – Wiederholung
**Läufe > Kontextmenü – Liste > Lauf freigeben.**

Im Dialog **Freigabe Lauf (Name): AUW – Wiederholung** können Sie Läufe zur Feinplanung freigeben.

#### Menü Datei
- **Aktualisieren:** Aktualisiert die Daten im Dialog.
- **Alle Reports auf Bildschirm:** Setzt alle Einstellungen im Feld **Listen** auf **Bildschirm**.
- **Alles aus:** Setzt alle Einstellungen im Feld **Listen** auf **Aus**.
- **Start:** Gibt den Lauf zur Produktion frei, startet den Druckvorgang für die ausgewählten Papiere und sendet die Daten an die ausgewählten Maschinen.
- **Abbrechen:** Schließt den Dialog, ohne die Daten zu übergeben.

#### Schneidtisch
- **Schneidtisch 1, Schneidtisch 2, VSG Schneidtisch 1:** Im Dropdown-Menü haben Sie folgende Optionen:
  - **Aus:** Es werden keine Daten übergeben.
  - **aktiv:** Die Daten werden an den Schneidtisch übergeben.
  - **Schneidplan:** Nur der Schneidplan wird an den Schneidtisch übergeben.
  - **Schneidcode:** Nur der NC-Code wird an den Schneidtisch übergeben.
- **Schneidplan:** Im Dropdown-Menü haben Sie folgende Optionen:
  - Drucker
  - Bildschirm-Vorschau

#### ISO
- **Bieger 1, Bieger 2, Sprossenansteuerung, ISO-Linie1, ISO-Linie 2, Line Server:** Checkbox mit folgenden Optionen:
  - Die Daten werden nicht an die Maschine übergeben.
  - Die Daten werden an die Maschine übergeben.

#### Initialisierung
- **Biegertexte INIT, Skizzen INIT, Rahmenskizzen INIT, PMO-Skizzen INIT:** Checkbox mit folgenden Optionen:
  - Die Daten werden nicht an die Maschine übergeben.
  - Die Daten werden an die Maschine übergeben.

#### Drucker
- **Drucker Listen:** Im Dropdown-Menü haben Sie folgende Optionen:
  - Windows Standard Drucker
  - Microsoft XPS Document Writer
- **Drucker Etiketten:** Im Dropdown-Menü haben Sie folgende Optionen:
  - TEC
  - Microsoft XPS Document Writer

#### Listen
- **Bereitstellungsliste, Abstellplatzliste Zuschnitt, Bockbelegungsliste Zuschnitt, Handzuschnittliste, Werkstattauftrag, VSG-Sortierliste, VSG-Produktionsliste, Bearbeitungsliste, ISO-Sortierliste, ISO-Produktionsliste, Rahmenliste, Sprossenliste, Versandliste, PMO-Gestellliste:** Im Dropdown-Menü haben Sie folgende Optionen:
  - Aus
  - Bildschirm
  - Microsoft XPS Document Writer
  Im Feld dahinter geben Sie die Anzahl der Ausdrucke an.
- **Produktionsetikett, Versandetikett:** Im Dropdown-Menü haben Sie folgende Optionen:
  - Aus
  - Bildschirm
  - TEC B-SX5

#### Auszuführende Prozesse
In der Liste werden alle Prozesse angezeigt, die mit diesem Lauf gestartet werden.
- **ID:** Die ID des Prozesses.
- **Station:** Die Station, an der der Prozess ausgeführt wird.
- **Lauf:** Der Lauf, bei dem der Prozess ausgeführt wird.
- **Computer:** Name des Rechners, auf dem der Prozess ausgeführt wird.
- **Beschreibung:** Beschreibung des Prozesses.
- **Status:** Status des Prozesses.
- **Fehler:** Gibt an, ob während der Prozessausführung ein Fehler vorliegt.

#### Schaltflächen
- **[Alle Reports auf Bildschirm]:** Setzt alle Einstellungen im Dialog auf Bildschirm.
- **[Alles aus]:** Setzt alle Einstellungen im Feld **Listen** auf **Aus**.
- **[Start]:** Gibt den Lauf zur Produktion frei und startet den Druckvorgang für die gewählten Dokumente.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu übergeben.

---
**A+W Production Grobplanung**
C-191, C-192, C-193
---

## Positionen in der Grobplanung

In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie sich zu Positionen einen Überblick verschaffen oder diese weiter bearbeiten können. Sie können Positionen überwachen, Positionen splitten und Positionsansichten importieren bzw. exportieren.

Das Kapitel enthält folgende Themen:
- "Positionen" auf Seite C-195
- "Auftrag zu Positionen hinzufügen" auf Seite C-198
- "Positionssplit" auf Seite C-199
- "Felddefinition" auf Seite C-201
- "Export/Import Positionsansicht" auf Seite C-203

### Positionen

- **Anzeigen > Aufträge > Kontextmenü > Positionen**
- **Anzeigen > Töpfe > Kontextmenü > Positionen**
- **Anzeigen > Läufe > Kontextmenü > Positionen**
- **Anzeigen > Füllaufträge > Kontextmenü > Positionen**
- **Glasarten > Kontextmenü > Positionen**
- **Bearbeitungen > Kontextmenü > Positionen**
- **Details > Kontextmenü > Positionen**
- **Lose > Kontextmenü > Positionen**
- **BDE > Kontextmenü > Positionen**

*Abb. C-37 Positionen (Beispiel)*

Im Dialog **Positionen** haben Sie eine Übersicht über die Positionen in den Aufträgen.
Sie können die Register und Spalten im Dialog **Positionen** nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen.
Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Der Dialog **Positionen** enthält z. B. folgende Informationen:

#### Navigation
Im Navigationsbereich wählen Sie, welche Details angezeigt werden sollen.
- **Auftrag (Auftragsnummer):** Auftragsnummer des gewählten Auftrags:
  - **Pos. (Positionsnummer):** Die einzelnen Positionen werden gelistet.
  - **Teil (Teilenummer):** Die einzelnen Teilenummern werden gelistet.
  - **Geometrie:** Zeigt Details zur Geometrie der Scheibe an.
  - **Texte:** Zeigt zum Auftrag hinterlegte Texte.
  - **Bearbeitungen:** Zeigt enthaltene Bearbeitungen an.

#### Datenbankspalten
- **Datenbankspalte:** Liste der zugehörigen Datenbankspalten zum Element, das Sie in der Navigation markiert haben.
- **Wert:** Wert der jeweiligen Datenbankspalte.

#### Liste
In der Liste werden Details zum Element angezeigt, das Sie in der Navigation markiert haben.
- **Freigabeteil:** Angabe, ob es sich um ein Freigabteil handelt.
- **Teile-Nr:** Angabe der Teilenummer.
- **Typ:** Angabe des Typs des Artikels bzw. des Teils.
- **Beschaffungsart:** Beschaffungsart des Artikels bzw. des Teils, z. B. Zukauf.
- **Artikel Nr.:** Artikelnummer des Artikels.
- **Artikelbezeichnung:** Bezeichnung des Artikels.
- **Prodtermin:** Produktionstermin des Kopfteils. Bei mehrteiligen Aufträgen ist das der Zusammenbautermin. Bei einteiligen Aufträgen sind Produktionstermin und Starttermin identisch.
- **SchichtPos:** Angabe, ob die Schicht zur Sonnenseite oder zur Innenseite zeigt. Die Angabe gilt pro Scheibe. Die Angabe erfolgt folgendermaßen:
  - 0: keine Beschichtung
  - 1: Sonnenseite
  - 2: Innenseite
- **Struktpos:** Angabe, ob die Struktur zur Sonnenseite oder zur Innenseite zeigt. Die Angabe gilt pro Scheibe. Die Angabe erfolgt folgendermaßen:
  - 0: keine Beschichtung
  - 1: Sonnenseite
  - 2: Innenseite
- **Stufe:** Angabe, ob es sich um ein Stufen-ISO oder VSG handelt.
- **Mod-Nr:** Nummer des verwendeten Modells.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

#### Kontextmenüs
In folgenden Bereichen des Dialogs **Positionen** werden Kontextmenüs angeboten: Navigation, Datenbankspalten, Liste.
Die Kontextmenüs variieren, je nachdem, welche Elemente Sie in der Navigation markiert haben.

| Gruppe | Pfad | Bemerkung |
| :--- | :--- | :--- |
| **Navigation** | Auftrag hinzufügen | Öffnet den Dialog **Auftrag zu Positionen hinzufügen**, mit dem Sie der jeweiligen Position einen Auftrag hinzufügen können. |
| | Ansicht exportieren | Öffnet den Dialog **Export/Import Positionsansicht**. |
| | Ansicht importieren | Öffnet den Dialog **Export/Import Positionsansicht**. |
| **Datenbankspalten** | Einfügen > Auftrag | Fügt ein neues Feld in die Liste ein. Verschiedene Kategorien zu Aufträgen stehen zur Verfügung. |
| **Liste** | Einfügen > Position | Fügt eine neue Spalte ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Teile | Fügt eine neue Spalte ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Teile kumuliert | Fügt eine neue Spalte ein. Verschiedene Kategorien stehen zur Verfügung. Die kumulierte Anzeige ist die gleichzeitige Abfrage mehrerer Datenbank-Tabellen und -Felder, z. B. Summen. |
*Tab. C-9 Positionen, Kontextmenüs*

---
**A+W Production Grobplanung**
C-195, C-196, C-197, C-198
---

### Auftrag zu Positionen hinzufügen
**Positionen > Navigation > Kontextmenü > Auftrag hinzufügen**

*Abb. C-38 Auftrag zu Positionen hinzufügen*

Im Dialog **Auftrag zu Positionen hinzufügen** können Sie weitere Aufträge in die Ansicht **Positionen** laden.

- **Auftragsnummer:** Angabe der Nummer des Auftrags, der hinzugefügt werden soll.
- **Auswahl vorher löschen:** Checkbox mit folgenden Optionen:
  - ☐ Die bisher angezeigten Aufträge werden vor dem Hinzufügen nicht gelöscht.
  - ☑ Die bisher angezeigten Aufträge werden vor dem Hinzufügen gelöscht.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

### Positionssplit
- **Anzeigen > Aufträge > Kontextmenü > Positionen splitten**
- **Bearbeitungen > Kontextmenü > Positionen splitten**
- **Details > Kontextmenü > Positionen splitten**

*Abb. C-39 Positionssplit*

Im Dialog **Positionssplit** können Sie Positionen aus Aufträgen aufsplitten. Der Positionssplit kann auch für mehrere Aufträge gleichzeitig durchgeführt werden.

#### Markierte Positionen
In der Liste werden die Bearbeitungen angezeigt, die Sie im Dialog **Bearbeitungen** ausgewählt haben.
⇨ "Bearbeitungen" auf Seite C-205
- **Auftrag:** Aufträge, die Sie zum Splitten ausgewählt haben.
- **Pos.:** Anzahl der Positionen in den Aufträgen.
- **UPos.:** Zur Zeit nicht genutzt.
- **Menge:** Anzahl der Teile in den Aufträgen.

#### Neue Positionen
In der Liste werden die gesplitteten Positionen angezeigt.
- **Auftrag:** Gesplittete Aufträge.
- **Pos.:** Anzahl der Positionen in den Aufträgen.
- **UPos.:** Zur Zeit nicht genutzt.
- **Neue Position:** Neue Position nach dem Split.
- **Menge:** Anzahl der Scheiben in den Aufträgen.

- **[Entfernen]:** Löscht eine markierte Position.
- **Je Position in ... Positionen aufteilen:** Angabe, in wie viele neue Positionen aufgeteilt wird.
- **Positionen mit maximal ... Scheiben erzeugen:** Angabe, wie viele Scheiben eine neue Position maximal enthalten darf.
- **Je Pos. eine Pos. mit ... Scheiben erzeugen:** Angabe, dass je Position eine neue Position mit einer bestimmten Anzahl an Scheiben erzeugt wird.
- **Teilung gemäß PMO Ergebnis:** Mit diesem Optionsschalter legen Sie fest, dass die Positionen passend zur Packmitteloptimierung gesplittet werden.
- **[Splitten]:** Splittet die Positionen.
- **[Schließen]:** Schließt den Dialog.

---
**A+W Production Grobplanung**
C-199 & C-200
---
