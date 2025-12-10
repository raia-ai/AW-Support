---
title: "DE_AWBusiness_Kapazitaetsplanung_4_2"
source: "DE_AWBusiness_Kapazitaetsplanung_4_2.pdf"
tags: ["A+W Business Pro", "Capacity Planning", "ERP", "Glass Manufacturing", "Production Scheduling", "Master Data", "Software Tutorial", "Technical Manual", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A German-language technical manual for A+W Business Pro Capacity Planning software. It includes a tutorial on master data management, production sequencing, capacity planning, and order scheduling, as well as a software reference guide for administrative settings."
long_description: "This document is a comprehensive guide for the A+W Business Pro Capacity Planning module, version 4.02. It is structured into two main parts: a Tutorial and a Software Reference. The Tutorial section provides step-by-step instructions and practical examples on how to use the software for production management. Key topics include setting up and assigning master data, defining production sequences, handling different product types, and managing capacity. It details the process of scheduling orders, both manually and automatically, dealing with bottlenecks, splitting production orders, and monitoring production progress and costs. The guide also covers the use of the 'Leitstand' (Control Center) for a high-level overview and management of production. The Software Reference section offers detailed descriptions of all relevant dialogs, settings, and administrative functions. It covers master data administration, organizational setup (like production areas, machines, and shifts), and system configurations for capacity planning and production feedback. This manual is intended for system administrators, production planners, and advanced users of the A+W Business Pro software in the glass, windows, and doors manufacturing industry."
---

# Tutorial

---
## Stammdaten

- **Manuell:**
  Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

Diese Einstellungen gelten nur für die automatische Einlastung. Wenn Sie Aufträge immer manuell einlasten, müssen Sie auch die Aggregate manuell auswählen.

> **Einstellungen ändern**
> Wenn Sie Einstellungen in den Firmendaten geändert haben, sollten Sie A+W Business Pro neu starten.

### Ergänzende Informationen
⇨ Softwarereferenz, "Voreinstellungen Firmendaten" auf Seite H-183
⇨ Softwarereferenz, "Besondere technische Restriktionen" auf Seite H-219
⇨ Softwarereferenz, "Besondere Prioritäten" auf Seite H-235
⇨ Softwarereferenz, "Sperren" auf Seite H-254
⇨ Softwarereferenz, "Aggregate Ausfall" auf Seite H-297

---

## Zuordnen der A+W Business Pro-Stammdaten

### Lernziele
- Zuordnungen für bestimmte Produkte oder Gruppen von Produkten nutzen.
- Produktionsreihenfolge festlegen.
- Besonderheiten bei Modellen und Bearbeitungen berücksichtigen.
- Erhöhung oder Verminderung der benötigten Zeit durch Faktoren einstellen.

### Nutzen
- Die Produktionsreihenfolge wird aus den Zuordnungen der erforderlichen Arbeitsarten ausgelesen.
- Durch die Zuordnungen der A+W Business Pro-Stammdaten können Besonderheiten der betrieblichen Organisation berücksichtigt werden, z. B. gleichartige Aggregate an unterschiedlichen Fertigungslinien.

### Merke

| Begriff | Beschreibung |
| --- | --- |
| **Produktionsreihenfolge** | Pro Arbeitsart muss festgelegt werden, in welcher Reihenfolge diese ausgeführt werden. Zum Beispiel sollen in einer Rechteckscheibe erst die Kanten 1 und 3 und dann die Kanten 2 und 4 bearbeitet werden. |
| **Explizite Zuordnungen** | Bei einer expliziten (direkten) Zuordnung wird das Produkt aus den Stammdaten der entsprechenden Arbeitsart in der Kapazitätsplanung zugeordnet, z. B. das Produkt Kanten polieren der Arbeitsart Kanten polieren. |
| **Implizite Zuordnungen** | Bei einer impliziten (indirekten) Zuordnung wird z. B. die Produktart Einfachglas der Arbeitsart Zuschnitt zugeordnet. Auch wenn in den A+W Business Pro-Stammdaten selbst kein Produkt Zuschnitt existiert, ist doch klar, dass das Einfachglas auf das jeweilige Auftragsmaß zugeschnitten werden muss. |
| **Voreinstellungen** | Produktstammdaten |

---

## Produktionsreihenfolge

In den A+W Business Pro-Stammdaten sind Basisprodukte angelegt, z. B. Einfachglas, VSG, ESG, Zuschläge, Modelle, Sprossen usw. Diesen Produkten müssen die Arbeitsarten und Maschinen zugeordnet werden, um festzulegen, in welcher Reihenfolge die Produktion ablaufen soll.

Hierbei wird zwischen expliziten und impliziten Zuordnungen unterschieden:
- Bei einer expliziten (direkten) Zuordnung wird z. B. die Produktgruppe Rundecken der Arbeitsart CNC-Bearbeitung zugeordnet.
- Bei einer impliziten (indirekten) Zuordnung wird z. B. die Produktart Einfachglas der Arbeitsart Zuschnitt zugeordnet. Auch wenn in den A+W Business Pro-Stammdaten selbst kein Produkt Zuschnitt existiert, ist doch klar, dass das Einfachglas auf das jeweilige Auftragsmaß zugeschnitten werden muss.

Sie können jeweils mehrere Arbeitsarten zuordnen. Dabei legen Sie auch fest, in welcher Reihenfolge diese Arbeitsarten ausgeführt werden.

> **Beispiel: Produktart ESG**
> - Glas waschen
> - Kontrolle
> - ESG fertigen
> - Verpacken verarbeitetes ESG
> - Verladen

**Abb. H-71: Beispiele für Zuordnungen von Arbeitsarten zu Produktarten**

| Arbeitsart | Produktart |
| --- | --- |
| Zuschneiden | Einfachglas |
| Waschen | VSG |
| ISO-Fertigen | Bearbeitungen |
| Versand | ISO |

Aber nicht jede Zuordnung ist sinnvoll: Die Arbeitsart Versand muss z. B. der Produktart Einfachglas zugeordnet werden, denn auch eine einfache Float-Scheibe kann in den Versand gehen. Die Zuordnung von Versand zu Bearbeitungen ist hingegen nicht sinnvoll.

Den unterschiedlichen Produktarten, Produktgruppen usw. können dieselben Arbeitsarten zugeordnet sein, z. B. die Arbeitsart Versand, die sowohl für VSG und ESG als auch für Beschläge ausgeführt wird.

Die Zuordnungen werden in Reihenfolge ausgewertet, in der die Dialoge angeordnet sind:
- Produktart
- Warengruppe
- Produktgruppe
- Produkt
- Kombi-Produktart
- Sonderzuordnung (1 bis 4)
- Kombi-Produktgruppe
- Lagerartikel

Das bedeutet, dass die Produktarten die oberste Ebene der Zuordnungen bilden. Alle weiteren Zuordnungen sind dann Ausnahmen davon.

> **Beispiel**
> Der Produktart Einfachglas wird die Arbeitsart Zuschnitt zugeordnet. Dadurch können alle Einfachgläser zugeschnitten werden.
> Die Produktgruppe Drahtornament kann dann z. B. die Arbeitsart Handzuschnitt zugeordnet werden.

Wenn keine Arbeitsart zugeordnet ist (<k. A.>), dann wird der entsprechende Eintrag ignoriert, z. B. die Produktgruppe Bearbeitungen.

---

## Dialoge für Zuordnungen

Arbeitsarten, die nicht zugeordnet sind, können an den Produkten aus dem Auftrag nicht ausgeführt werden. Das bedeutet, dass Sie keine einzige ISO-Einheit fertigen können, wenn die Arbeitsart ISO Fertigen nicht zugewiesen ist.

**Abb. H-72: Zuordnung der Produktart Einfachglas**
- **A:** Produktart A+W Business Pro-Stammdaten
- **B:** Reihenfolge der Arbeitsarten
- **C:** Arbeitsarten, die an der Produktart ausgeführt werden
- **D:** Faktor (siehe ISO-Beispiel)
  ⇨ "Fallbeispiel ISO und Modell" auf Seite H-65

Wenn Sie den Produktarten die entsprechenden Arbeitsarten zugeordnet haben, sind in der Regel die meisten Fälle erfasst. Jedoch ist diese Zuordnung sehr grob, da z. B. der Zuschnitt von Einfachglas nicht so unkompliziert ist, wie diese Zuordnung glauben lässt. Für das Float gibt es keine Schwierigkeiten, aber Ornamentgläser können unter Umständen nur von Hand zugeschnitten werden.

**Abb. H-73: Zuordnung der Produktgruppe Ornamentglas**
- **A:** Produktgruppe A+W Business Pro-Stammdaten
- **B:** Arbeitsart Handzuschnitt

Sie müssen zusätzlich die Produktgruppe Ornamentglas der Arbeitsart Handzuschnitt zuordnen. Die Arbeitsart Versand müsste nicht nochmals zugeordnet werden, da der Versand ja schon über die Produktart zugeordnet ist.

Die Dialoge zum Zuordnen sind analog aufgebaut, unterscheiden sich aber in der Art der Zuordnung. In der folgenden Übersicht werden diese unterschiedlichen Zuordnungen kurz charakterisiert:

- **Produktarten:**
  Diese Zuordnungen richten Sie für alle Arbeitsarten ein, die in der Regel immer ausgeführt werden, z. B. Zuschnitt, Versand.
- **WGR (Warengruppe):**
  Diese Zuordnungen richten Sie für Warengruppen ein, bei denen Arbeitsarten mit erhöhtem Aufwand ausgeführt werden und daher mit einem Zuschlag berechnet werden sollen, z. B. der Zuschnitt aller Antikgläser.
- **Produktgruppe:**
  Diese Zuordnungen richten Sie für Produktgruppen ein, für die von der Zuordnung der Produktart abgewichen werden soll, z. B. der Zuschnitt von Drahtgläsern, die zur Produktart Einfachglas gehören.
- **Produkte:**
  Diese Zuordnungen richten Sie für die Produkte ein, für die von den Zuordnungen der Produktarten und/oder Produktgruppen abgewichen werden soll, z. B. für ein 3-fach-VSG die Arbeitsart Sägen.
- **Kombi-Produktart:**
  Diese Zuordnungen richten Sie für einzelne Produkte ein, die Bestandteil der Stückliste in den Produkten einer Produktart sein können, z. B. das Produkt VSG 6 mm in einer ISO-Einheit (Produktart ISO).
- **Sonderzuordnungen:**
    - **Sonderzuordnung 1:** Diese Zuordnungen richten Sie für die Produktart Bearbeitungen ein, auf die eine andere Bearbeitung folgt.
    - **Sonderzuordnung 2:** Diese Zuordnungen richten Sie für die Bearbeitung von Modellen ein.
    - **Sonderzuordnung 3:** Diese Zuordnungen richten Sie für die Bearbeitung von Kanten ein.
    - **Sonderzuordnung 4:** Diese Zuordnungen richten Sie für die Bearbeitung und Folgebearbeitung von Modellen ein.
- **Kombi-Produktgruppe:**
  Diese Zuordnungen richten Sie für einzelne Produkte ein, die Bestandteil der Stückliste in den Produkten einer Produktgruppe sein können, z. B. das Produkt Float 6 mm in einer VSG-Einheit (Produktgruppe VSG).
- **Lagerartikel:**
  Diese Zuordnungen richten Sie für Lagerartikel (Lagerentnahme) ein, die nur verpackt und geliefert werden. Damit erreichen Sie, dass diese Produktgruppen z. B. in den Versand eingelastet und die Kosten und Zeiten kalkuliert werden.

> **Beschreibung der Zuordnungsdialoge**
> Eine detaillierte Beschreibung aller aufgeführten Dialoge finden Sie in der Softwarereferenz.

---

## Kombi-Produktart, Kombi-Produktgruppe

Produkte, die Bestandteil einer Stückliste sind oder als Bearbeitung auf eine Produktgruppe wirken, können abweichend zugeordnet werden. Das bedeutet, dass Sie dem Produkt verschiedene Arbeitsarten zuordnen können, je nachdem in welcher Kombi-Produktart oder Kombi-Produktgruppe es verwendet wird.

> **Beispiel**
> Floatglas ist Teil von ISO und von VSG. Der Schneidtisch für ISO steht in der Halle für die ISO-Linie. Der Schneidtisch für VSG steht in der Halle zur VSG-Fertigung. Dazu sind zwei unterschiedliche Arbeitsarten angelegt, die dem jeweiligen Zuschnitt gelten.
> Sie können daher dem Floatglas die Arbeitsart VSG-Zuschnitt zuordnen, wenn es als Teil in der Stückliste des VSG enthalten ist.

Wenn Sie zwei Arbeitsarten für den Zuschnitt eingerichtet haben, können Sie in den Vorgabezeiten den Arbeitsarten die entsprechenden Schneidtische (Aggregate) zuordnen. Entsteht jedoch bei dem einen Schneidtisch ein Engpass, wird der andere nicht angesteuert, da ihm die andere Arbeitsart nicht zugeordnet ist.

**Abb. H-74: Beispiel: Steuerung des Zuschnitts für Produktgruppe VSG**

| Zuordnung | Arbeitsart | Aggregat |
| :--- | :--- | :--- |
| **Produktart:** Einfachglas | Zuschnitt | Schneidtisch I, Halle A |
| **Kombi-Produktgruppe:** wenn Float 6 mm in Produktgruppe VSG | Zuschnitt VSG | Schneidtisch II, Halle B |

Mit diesen Vorgaben wird der Schneidtisch I ausgelastet. Wenn aber ein Float für ein VSG zugeschnitten werden soll, dann wird Schneidtisch I ignoriert und Schneidtisch II gewählt.

Die beiden Dialoge zum Zuordnen sind analog aufgebaut. Als Beispiel ist hier der Dialog Kombi-Produktart gezeigt.

**Abb. H-75: Beispiel für Zuordnung von Arbeitsart zu Produkt**
- **A:** Ausgewähltes Produkt
- **B:** Ausgewähltes Produkt ist Bestandteil von
- **C:** Arbeitsarten, die dem ausgewählten Produkt zugeordnet sind

In diesem Beispiel sehen Sie, dass dem Produkt Float 4 mm (A) die Arbeitsart VSG-Zuschnitt (C) zugeordnet ist, wenn es Komponente in der Produktart VSG (B) ist.

### Zuordnung festlegen

In diesem Beispiel wird eine Sonderzuordnung für die Kantenbearbeitung von Modellen festgelegt. Damit können nahezu alle Handlungsschritte gezeigt werden, die bei den Zuordnungen vorkommen. Die Zuordnungen in den anderen Dialogen werden entsprechend festgelegt.

**So legen Sie eine Sonderzuordnung fest**
1. Wählen Sie im Modul Kapazitätsplanung > Zuordnen > Sonderzuordnung 4.
Der gleichnamige Dialog wird geöffnet.
Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
2. Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

**Abb. H-76: Felder für neue Sonderzuordnung freigeschaltet**
- **A:** Auswahl des Produkts
- **B:** Auswahl der Bearbeitung
- **C:** Auswahl des Modells

3. Wählen Sie die A+W Business Pro-Stammdaten aus:
    - **Produkt**, z. B. Ornamentglas (A)
    - **Bearbeitung**, z. B. Säumen (B)
    - **Modell**, z. B. Modell mit 2 Rundecken (C).
Die Daten werden in der Übersicht angezeigt.

**Abb. H-77: Sonderzuordnung festlegen**
- **A:** Schematische Darstellung des Modells
- **B:** Felder freischalten
- **C:** Kanten des Modells

Im Bereich Identifikation wird eine Skizze des Modells (A) angezeigt, aus der Sie die Nummerierung der Kanten und Ecken ersehen können.
4. Klicken Sie im Bereich Arbeitsarten mit Kantenzuordnung auf [Neu] (B), um die erste Arbeitsart einzutragen.

5. Setzen Sie den Cursor in das Feld Arbeitsart und wählen Sie aus der Kombobox die erste Arbeitsart aus, z. B. Handzuschnitt.
6. Wiederholen Sie Schritt 4 und 5, um die nächsten Arbeitsarten auszuwählen, z. B. Säumen, Waschen.
7. Setzen Sie den Cursor in das Feld Faktor und tragen Sie den Faktor ein, um den diese Arbeitsart erhöht werden soll, z. B. 2,5.
Dieser Faktor bedeutet, dass der Zeitbedarf, der für das Säumen angegeben ist, mit 2,5 multipliziert wird, wenn ein Modell mit zwei Rundecken gefertigt wird.
8. Klicken Sie in die Checkboxen der Spalten 1 bis 6, um die Kanten zu markieren, die bearbeitet werden sollen und für die der Faktor berechnet werden soll.
Wenn der Faktor nicht für alle Kanten berechnet werden soll, müssen Sie eine zweite Zuordnung für die verbleibenden Seiten anlegen.

In diesem Beispiel sehen Sie, dass zunächst die Kante 1 bearbeitet werden soll. Dafür wird kein erhöhter Zeitbedarf berechnet. Für die Kanten 2 bis 6 wird der Zeitbedarf um einen Faktor erhöht.
9. Prüfen Sie die Reihenfolge der Arbeitsschritte.
Wenn Sie eine Zeile markieren, können Sie den Arbeitsschritt mit den Pfeil-Schaltflächen nach oben oder unten verschieben, bis die richtige Reihenfolge eingestellt ist.
10. Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
Die Daten werden gespeichert. Damit haben Sie die Reihenfolge der Arbeitsarten festgelegt.

### Übungen
- Legen Sie die vollständigen Zuordnungen für ISO-Einheiten mit Modell fest, so wie es in den Beispielen gezeigt ist.
Diese Übung ist sehr komplex. Sie können daher gerne die Beispiele übernehmen.
⇨ "Fallbeispiel ISO und Modell" auf Seite H-65

### Ergänzende Informationen
⇨ Softwarereferenz, "Zuordnen" auf Seite H-237

---

# Kapazitätsplanung

Aufträge müssen in die Kapazitätsplanung eingelastet werden, damit die Zeitkosten berechnet und die Produktionszeiten geplant werden. Dabei werden die verschiedenen Termine anhand der Vorgaben berechnet, die Sie in den Stammdaten festgelegt haben.

In diesem Themenblock lernen Sie, wie die Termine berechnet werden, wie Sie Aufträge einlasten, wie Sie auf Kapazitätsprobleme reagieren können, wie Sie die automatische Einlastung übergreifend steuern und wie Sie die Planung im Leitstand überwachen.

Dazu gehören folgende Lerneinheiten:
- "Einlastung der Aufträge" auf Seite H-113
- "Produktion" auf Seite H-136
- "Produktionskosten" auf Seite H-158
- "Leitstand" auf Seite H-166

## Einlastung der Aufträge

### Lernziele
- Terminberechnung kennenlernen.
- Planungsvorgänge erkennen.
- Ablauf der Einlastung kennenlernen.

### Nutzen
In der Regel werden die Aufträge durch einen Workflow-Task eingelastet. Sie müssen dann nur bei Engpässen eingreifen. Daher ist es wichtig zu wissen, wie die Einlastung abläuft.

### Merke

| Begriff | Beschreibung |
| --- | --- |
| **Terminberechnung** | Die Planung geht immer vom Liefertermin beim Kunden aus und berechnet die Termine für die Produktion so, dass die gefertigten Stückzahlen nicht gelagert werden müssen. |
| **Engpass** | Ein Kapazitätsengpass entsteht in aller Regel nur an Aggregaten, an denen aufwendigere Arbeitsarten ausgeführt werden. So ist z. B. der Zuschnitt i. d. R. problemlos. |
| **Restmengen** | Als Restmenge vom Vortag gelten Positionen, zu denen die Produktion noch nicht begonnen wurde. Sobald die erste Scheibe gefertigt ist, werden die restlichen Stückzahlen nicht mehr als Restmenge betrachtet. |
| **Sperrstunde** | Bei Sperrstunden legen Sie fest, bis zu welcher Uhrzeit Aufträge in eine Schicht eingelastet werden können. Damit stellen Sie sicher, dass die eingelasteten Aufträge auch produziert werden können und keine Restmengen für den nächsten Tag übrig bleiben. |
| **Voreinstellungen** | Firmendaten: Register Kapa-Planung |

### Terminberechnung

Ausgangspunkt für die Planung ist der Liefertermin, von dem aus die Arbeitsgänge zurückgerechnet werden. Die in der Stückliste vorgefundenen expliziten und impliziten Arbeitsgänge werden ihrer zeitlichen Reihenfolge und ihrer Position in der Stückliste entsprechend an der kostengünstigsten zugelassenen Maschine eingelastet. Wenn diese ausgelastet ist, wird (automatisch oder manuell) zu einer anderen Maschine gewechselt.

#### Rückwärtsterminierung
Ausschlaggebend für die Einlastung ist der Liefertermin. Die Prüfung der freien Kapazitäten beginnt immer mit der letzten Arbeitsart in der letzten Schicht vor dem Liefertermin, z. B. mit dem Verpacken in Schicht 2 und geht dann auf Schicht 1 zurück.

Sind für einen Arbeitsgang an einem Tag alle Maschinen (Aggregate) ausgelastet, wird versucht, den Vorgang auf den Vortag zu verlegen usw.

#### Vorwärtsterminierung
Wenn all die Rückwärtsterminierung nicht erfolgreich ist, sucht das Programm nach einem neuen Liefertermin anhand des nächstmöglichen Tourentags. Von diesem Termin aus beginnt dann erneut die Rückwärtsterminierung. Dieser Vorgang kann so lange wiederholt werden, bis die Terminierung erfolgreich ist.

#### Zeiten zur Terminberechnung
Neben den Fertigungszeiten eines Aggregats werden Verweil- und Übergangszeiten berücksichtigt. Diese Zeiten wurden in der Einheit Zeitvorgaben ausführlich beschrieben. Zusammengefasst geht es dabei um folgende Kriterien:
- Wechsel des Produktionsbereichs, z. B. vom Zuschnitt zum Nassbereich.
- Wechsel der Arbeitsart, z. B. vom Schneiden der Durchsprechöffnung zu Feinpolieren der Öffnungskante.
- Ruhezeit im Produktionsbereich, z. B. Abkühlen nach dem ESG-Ofen.

Bei einem Wechsel des Produktionsbereichs hat die Definition im Dialog Übergangsmatrix eine höhere Priorität als der Eintrag im Dialog Produktionsbereich.

Wenn in beiden Dialogen Zeiten hinterlegt sind, ist Folgendes zu beachten:
- VSG fertigen und VSG sägen sind z. B. zwei Arbeitsarten, die im gleichen Produktionsbereich VSG stattfinden. In diesem Fall wird nur die Übergangszeit berücksichtigt, die im Dialog Übergangszeiten definiert wurde.
- ESG fertigen und Kommissionieren sind zwei Arbeitsarten, die in unterschiedlichen Produktionsbereichen stattfinden. In diesem Fall prüft die Kapazitätsplanung sowohl den Wert im Dialog Übergangsmatrix als auch den Wert im Dialog Übergangszeiten. Der größere Wert wird berücksichtigt.

In den folgenden Ablaufbeispielen wird gezeigt, wie sich die Definitionen in den verschiedenen Dialogen auf die Berechnung des Produktionsbeginns auswirken. Wir gehen von einem Betrieb aus, der standardmäßig in drei Schichten arbeitet. Der Produktionsbereich Heat-Soak-Test arbeitet nur in einer Schicht.

#### Beispiel für Verweiltage
In diesem Beispiel gibt es nur Einträge im Dialog Produktionsbereich. Bei einer Vorgabe von je einem Verweiltag pro Produktionsbereich wirkt sich das auf die Berechnung des Starttages der Produktion wie folgt aus.

**Tab. H-1: Vorgaben für das Beispiel Verweiltage**

| Arbeitsarten | Berechnung der Termine |
| :--- | :--- |
| Zuschnitt -> Heat-Soak-Test -> Kommissionierung | - Liefertermin ist Freitag. <br> - Heat-Soak-Test am Mittwoch in der 1. Schicht. <br> - Kommissionierung am Donnerstag in der 1. Schicht. <br> - Zuschnitt (Produktionsstart) am Dienstag in der 1. Schicht. |

**Abb. H-78: Beispiel mit Verweiltagen im Produktionsbereich**
Dieses Zeitschema zeigt, dass bei einem Liefertermin am Freitag die Kommissionierung am Donnerstag, der Heat-Soak-Test am Mittwoch und der Zuschnitt am Dienstag stattfindet. Zwischen jedem Produktionsbereich liegt ein Verweiltag von 1 Tag.

In diesem Beispiel sehen Sie, dass die Schichten nicht berücksichtigt werden, weil jeweils ein Verweiltag für die Produktionsbereiche festgelegt wurde.

#### Beispiel für unterschiedliche Übergangszeiten
In diesem Beispiel gibt es Einträge in den Dialogen Übergangsmatrix und Übergangszeiten. Der Starttag der Produktion wird wie folgt berechnet.

**Tab. H-2: Vorgaben für das Beispiel Übergangszeiten**

| Arbeitsarten | Berechnung der Termine |
| :--- | :--- |
| Zuschnitt -> Heat-Soak-Test -> Kommissionierung | - Der Liefertermin ist Freitag. <br> - Im Dialog **Übergangsmatrix** wurde für alle Produktionsbereiche der Wert 0,1 Tage (= eine Schicht) definiert. Wenn der Versand für diese Tour standardmäßig in der 2. Schicht erfolgt, kann die Kommissionierung noch am Freitag in der 1. Schicht erfolgen. Anderenfalls wird am Donnerstag in der 3. Schicht kommissioniert. <br> - Im Dialog **Übergangszeit** ist der Wert 3 eingetragen. Ausgehend von der Kommissionierung in der 1. Schicht am Freitag, wird drei Schichten zurückgezählt. Auch wenn für den Heat-Soak-Test in den Schichten 2 und 3 der Wert 0 steht, werden diese bei der Zählung berücksichtigt. Folglich beginnt der Heat-Soak-Test am Donnerstag in der 1. Schicht. Der Wert im Dialog Übergangsmatrix bleibt unberücksichtigt, weil der Wert im Dialog Übergangszeiten größer ist. <br> - Der Zuschnitt (Produktionsstart) ist am Mittwoch in der 3. Schicht, da im Dialog Übergangsmatrix der Übergang vom Produktionsbereich Zuschnitt zum Heat-Soak-Test mit 0,1 Tage (= eine Schicht) definiert wurde. |

**Abb. H-79: Beispiel mit Übergangszeiten**
Dieses Zeitschema zeigt, dass bei einem Liefertermin am Freitag, die Kommissionierung am Freitag, der Heat-Soak-Test am Donnerstag und der Zuschnitt am Mittwoch stattfindet. Die Übergangszeiten zwischen den Arbeitsarten und Produktionsbereichen werden in Schichten (0.1 Tage oder 3 Schichten) berechnet.

In diesem Beispiel sehen Sie, wie die Schichten bei der Berechnung berücksichtigt werden.

#### Beispiel für Übergangszeiten bei mehreren Arbeitsgängen in einer Schicht
Der Starttag der Produktion wird wie folgt berechnet.

**Tab. H-3: Vorgaben für das Beispiel Übergangszeiten**

| Arbeitsarten | Berechnung der Termine |
| :--- | :--- |
| Zuschnitt -> Schleifen -> Siebdruck -> Kommissionierung | - Der Liefertermin ist Freitag. <br> - Im Dialog **Übergangsmatrix** wurde der Wert 0,1 Tage (= eine Schicht) definiert. Wenn der Versand für diese Tour in der 2. Schicht erfolgt, kann die Kommissionierung noch am Freitag in der 1. Schicht erfolgen. Anderenfalls wird am Donnerstag in der 3. Schicht kommissioniert. <br> - Im Dialog **Übergangszeit** ist der Wert 2 eingetragen. Ausgehend von der Kommissionierung in der 1. Schicht am Freitag, wird zwei Schichten zurückgezählt. Der Siebdruck beginnt am Donnerstag in der 2. Schicht. Der Wert im Dialog Übergangsmatrix bleibt unberücksichtigt, weil der Wert im Dialog Übergangszeiten größer ist. <br> - Im Dialog **Übergangsmatrix** wurde der Wert 0,1 Tage (= eine Schicht) definiert für den Übergang vom Produktionsbereich Schleifen zum Produktionsbereich Siebdruck. Das Schleifen beginnt am Donnerstag in der 1. Schicht. <br> - Der Zuschnitt (Produktionsstart) ist in der gleichen Schicht wie das Schleifen, da im Dialog Übergangsmatrix der Wert 0 (= gleiche Schicht) definiert wurde. |

**Abb. H-80: Beispiel mit unterschiedlichen Arbeitsarten in derselben Schicht**
In diesem Beispiel sehen Sie die Berechnung, wenn mehrere Arbeitsarten am selben Tag ausgeführt werden können.

### Einlastung
Aufträge können in drei Varianten in die Kapazitätsplanung eingelastet werden:
- Manuell pro Auftrag.
- Manuell per Nummernverwalter.
- Automatisch im Batch-Betrieb.
In diesem Fall werden die Aufträge per Workflow-Task in die Kapazitätsplanung eingelastet. Die automatisierte Suche nach neuen Aufträgen erfolgt in definierten Intervallen.

#### Manuell einlasten
Bei der manuellen Einlastung können Sie die Vorgaben so einrichten, dass Sie jeden einzelnen Schritt verfolgen können, indem Sie die Auftragspositionen einzeln an den verschiedenen Aggregaten einlasten. Sie werden die Vorgaben i. d. R. aber so einrichten, dass Sie nur bei Engpässen eingreifen müssen.
Manuelle Eingriffe sind erforderlich, wenn Sie mit den Ergebnissen der Einlastung nicht zufrieden sind. Sie müssen die Aufträge dann umlasten.
Eine Umlastung kann auch notwendig werden, wenn eine Maschine ausfällt und die nicht vorhergesehene Reparaturzeit dies erforderlich macht.
Beim manuellen Einlasten können Sie z. B. auch bestimmen, wann frühestens mit der Produktion begonnen werden soll.

> **Beispiel**
> Wenn ein im September eingelasteter Auftrag mit dem Liefertermin 25.11. so produziert werden soll, dass die gefertigten Einheiten nicht gelagert werden müssen, kann ein Termin für den frühesten Produktionsbeginn angegeben werden.

#### Automatisch einlasten
Mit einem Workflow-Task (Batch-Programm) können Aufträge automatisch in die Kapazitätsplanung eingelastet werden. Dabei wird automatisch nach freien Maschinen gesucht. Je nach Einstellung müssen Sie dann nur bei Engpässen manuell eingreifen, was z. B. erforderlich wird, wenn die Maschine A ausgelastet ist, Maschine B und C aber nicht.
In die Einlastung kann über den Dialog Leitstand manuell eingegriffen werden, um Positionen auf eine andere Maschine oder ein anderes Datum umzulasten.

#### Einstellungen für den Workflow-Task
Workflow-Tasks dienen der weitgehend automatischen Verarbeitung von Aufträgen. Inwieweit manuelle Eingriffe zwischen aufeinander folgenden Workflow-Tasks notwendig sind, hängt davon ab, wie die Abläufe in Ihrem Betrieb organisiert sind. Die notwendigen Einstellungen werden bei der Installation von A+W Business Pro festgelegt und sollten nachträglich nicht geändert werden. In diesem Abschnitt werden daher nur die grundlegenden Prinzipien dargestellt.

Ein Workflow-Task besteht aus einer oder mehreren Customizing-Formeln. In diesen Formeln sind die einzelnen Aktionen definiert, die ausgeführt werden sollen. Der ALFAK Interface Service führt den Task zu einem festen Zeitpunkt oder in Intervallen aus.

Um einen Workflow-Task einzurichten, sind drei Schritte erforderlich:
- Formeln unter Stammdaten > Firma > Formeln anlegen. Für die Kapazitätsplanung können das z. B. Formeln für die Suche nach Aufträgen sein:
    - die eingelastet werden sollen
    - die vom Vortag übrig geblieben sind (Restmengen)
- Formeln einem Workflow-Task unter Stammdaten > Firma > Customizing > Register Workflow Tasks zuordnen.
- Startzeit oder Intervall des Workflow-Task unter Stammdaten > Firma > Customizing > Register Autom. Prozessausführung einstellen.

Wenn Sie Workflow-Tasks einrichten wollen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.

> **Produktionsübergabe**
> Aufträge werden nicht automatisch aus der Kapazitätsplanung an die Produktion übergeben. Die Übergabe an die Produktion wird mit einem separaten Workflow-Task geregelt.

### Kapazitätsprobleme
In der Regel ist der Zuschnitt unproblematisch, da er am Anfang der Produktionskette steht. Kapazitätsengpässe entstehen aber leicht, wenn Arbeitsgänge aufwendiger sind, z. B. bei Modellen oder in der ISO-Produktion.
Wenn die (automatische) Einlastung auf Kapazitätsengpässe stößt, sollten Sie manuell eingreifen können. Natürlich können Sie die Voreinstellungen so festlegen, dass durch die automatische Verschiebung des Liefertermins jeder Auftrag eingelastet werden kann. Mit den manuellen Eingriffen behalten Sie jedoch die Möglichkeit, die weniger aufwendigen Aufträge zugunsten eines anderen zu verschieben.

### Positionssplit
Neben der Verschiebung von Terminen können große Positionen auch aufgeteilt werden, wenn die Schichtzeiten und die Auslastung dies erforderlich machen. Dadurch wird die Produktion der Position auf mehrere Schichten und/oder Tage verteilt.

Beim Aufteilen in Unterpositionen haben Sie folgende Möglichkeiten:
- Sie geben die Anzahl der gewünschten Unterpositionen ein.
- Sie lassen die notwendigen Unterpositionen vom Programm erzeugen.

Im folgenden Beispiel sollen 100 ISO-Einheiten mit zwei Rundecken gefertigt werden. Das ergibt eine Gesamtzahl von 400 Rundecken, für die eine Gesamtzeit von 11,6 Stunden verplant werden muss. Die Maschine arbeitet in einer Schicht 8 Stunden. Daher muss die Position aufgeteilt werden.

**Abb. H-81: Überschreitung der Maschinenkapazität – Splitting**
Aus den 100 Scheiben der Auftragsposition werden zwei Unterpositionen mit je 50 Scheiben für den Zuschnitt und die Bearbeitung erzeugt. Für den Zuschnitt wäre das Splitten nicht notwendig. Es wird aber gemacht, damit die geschnittenen Scheiben nicht gelagert werden müssen, bis sie zur Bearbeitung kommen.

Die Fertigung von 100 ISO-Einheiten wird danach folgendermaßen verteilt.
(UP = Unterposition)

| UP | Glas / Einheit | Aggregat | Datum |
| :--- | :--- | :--- | :--- |
| **UP 1** | Glas 1 | Zuschnitt 50 Scheiben | Schicht 2 am 02.08. |
| | Glas 2 | Zuschnitt 50 Scheiben | Schicht 2 am 02.08. |
| | Glas 1 + Glas 2 | Rundecken an 100 Scheiben | Schicht 1 am 03.08. |
| | ISO-Fertigung | 50 Stück | Schicht 1 am 04.08. |
| | Kommissionierung/Versand | 50 Stück | Schicht 1 am 05.08. |
| **UP 2** | Glas 1 | Zuschnitt 50 Scheiben | Schicht 1 am 03.08. |
| | Glas 2 | Zuschnitt 50 Scheiben | Schicht 1 am 03.08. |
| | Glas 1 + Glas 2 | Rundecken an 100 Scheiben | Schicht 1 am 04.08. |
| | ISO-Fertigung | 50 Stück | Schicht 2 am 04.08. |
| | Kommissionierung/Versand | 50 Stück | Schicht 1 am 05.08. |

### Produktionszeiten reservieren
Beim Splitten können die verbleibenden Zeiten einer Schicht für andere Aufträge gesperrt werden. Damit verhindern Sie, dass die Maschine zwischendurch umgerüstet werden muss.
Sie können außerdem das Produktionsdatum vorgeben. Diese Möglichkeit ist besonders dann hilfreich, wenn die Fertigungszeiten für die verschiedenen Arbeitsgänge stark voneinander abweichen.

> **Beispiel**
> 10 ISO-Scheiben in Übergröße müssen gefertigt werden.
> Dabei können alle Scheiben an einem Tag zugeschnitten werden. Die Produktion an der ISO-Linie erlaubt jedoch nur eine Einheit in dieser Größe pro Tag. Die zugeschnittenen Scheiben müssen dann bis zu 9 Tage gelagert werden.
> Beim Splitten entstehen 10 Unterpositionen (= eine ISO-Scheibe pro Tag), denen Sie jeweils das Produktionsdatum vorgeben.
> Jede Unterposition wird dann einzeln zugeschnitten und noch am selben Tag auf der ISO-Linie gefertigt.

### Sperrstunde
Logischerweise können Positionen dann nicht mehr gefertigt werden, wenn sie zum Schichtende eingelastet werden. Da nicht gefertigte Positionen als Restmengen aus dem Vortag am folgenden Tag gefertigt werden müssen, sollten Sie Zeiten für die letzte Einlastung festlegen.
Bei solchen Sperrstunden legen Sie fest, bis zu welcher Uhrzeit Aufträge in eine Schicht eingelastet werden können. Damit stellen Sie sicher, dass die eingelasteten Aufträge produziert werden können und keine Restmengen für den nächsten Tag übrig bleiben.

> **Beispiel**
> Am Freitag erhalten Sie um 12 Uhr einen neuen Auftrag. Bei der manuellen Einlastung tragen Sie 14 Uhr ein, obwohl die Schicht bis 16 Uhr geht. Damit wird der Auftrag nicht eingelastet, wenn er an diesem Tag nicht mehr gefertigt werden kann.
> Wenn der Auftrag wegen der Sperrstunde nicht mehr eingelastet werden kann, wird im Dialog Lieferdatum eine entsprechende Meldung angezeigt. Sie müssen dann das Lieferdatum ändern.

Die Sperrzeiten legen Sie übergreifend im Dialog Einstellung Schichten fest. Bei manuellen Eingriffen bei Kapazitätsproblemen können Sie die Zeiten prüfen.
⇨ "Einstellungen Schichten" auf Seite H-187

### Voreinstellungen für automatische Einlastung
Die Einstellungen für die Anzahl der Schichten und den Auslastungsgrad in den Firmendaten haben Sie bereits in der Einheit Schicht- und Arbeitszeiten kennengelernt. Diese Beschreibung wurde in der Einheit Auswahl der Aggregate durch die Einstellungen für die Aggregate ergänzt.
⇨ "Voreinstellungen für Schichten und Kapazitäten" auf Seite H-48
⇨ "Voreinstellungen zur Aggregatauswahl" auf Seite H-100

Neben diesen Einstellungen haben Sie zur Steuerung der automatischen Einlastung weitere Einstellungsmöglichkeiten.

**Abb. H-82: Firmendaten – Kapa-Planung**
- **A:** Liefertermin suchen
- **B:** Schichtfüllung
- **C:** Einlastung erzwingen
- **D:** Aufträge nicht splitten

Wenn Sie beim automatischen Einlasten zulassen, dass Auftragspositionen gesplittet werden, dann müssen Sie auch festlegen, wie weit ein Aggregat dabei ausgelastet werden darf (B). Diese Angabe entfällt, wenn Sie das automatische Splitten unterbinden (D). Bedenken Sie aber, dass eine Auftragsposition so umfangreich sein kann, dass die Fertigung die Kapazität eines Aggregats übersteigt. Der Auftrag kann dann nicht eingelastet werden und Sie müssen manuell eingreifen.

### Wahl des Liefertermins
Bei Engpässen kann automatisch nach einem neuen Liefertermin gesucht werden. Als nächstmöglicher Liefertermin sollte ein Tourentag (A) gewählt werden. Bei Eilaufträgen kann der vorgeschlagene Termin manuell geändert werden, z. B., wenn mit einer Sonder-Tour geliefert wird. Diese Einstellung ist natürlich nur dann sinnvoll, wenn Sie Touren eingerichtet und den Kunden zugewiesen haben.
Sie können die Einlastung zum Liefertermin aus dem Auftrag jedoch auch erzwingen (C). Mit dieser Einstellung werden die Aufträge ohne Suche nach einem alternativen Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht. Das kann dazu führen, dass ständig Restmengen aus dem Vortag entstehen. Eine echte Planung ist dann kaum noch möglich.

> **Einstellungen ändern**
> Wenn Sie Einstellungen in den Firmendaten geändert haben, sollten Sie A+W Business Pro neu starten.

### Auftrag einlasten
Aufträge werden in der Regel durch einen Workflow-Task in die Kapazitätsplanung eingelastet. Sie können alle Aufträge eines Nummernverwalters oder jeden Auftrag einzeln manuell in die Kapazitätsplanung einlasten.
In den folgenden Handlungsschritten wird die manuelle Einlastung eines einzelnen Auftrags gezeigt. Wie Sie eventuell auftretende Probleme bei der Einlastung auflösen, ist in der nachfolgenden Einheit beschrieben.
⇨ "Kapazitätsproblem lösen" auf Seite H-130

> **Einlastung nicht möglich**
> Der Auftrag kann nicht eingelastet werden, wenn er von einem anderen Mitarbeiter noch bearbeitet wird und daher im Modul Dokumente geöffnet ist.
> Wenn Sie die Kapazitäten über den Jahreswechsel hinaus planen, müssen Sie den Kalender für das neue Jahr mit allen Schichtzeiten angelegt haben.

> **Auftrag erneut einlasten**
> Wenn Sie einen Auftrag erneut einlasten wollen, müssen Sie die alte Einlastung zunächst löschen. Dies gilt insbesondere dann, wenn der Auftrag versehentlich manuell fertig gemeldet wurde und daher neu eingelastet werden muss.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So lasten Sie einen Auftrag ein" auf Seite H-125
- "So lasten Sie eine einzelne Auftragsposition ein" auf Seite H-129
- "So löschen Sie einen Auftrag aus der Kapazitätsplanung" auf Seite H-130

#### So lasten Sie einen Auftrag ein
1. Wählen Sie Fertigung > Kapazitätsplanung > Einlasten > Einlasten Auftrag.
(Siehe Abb. H-83 Auftrag einlasten)
Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
2. Geben Sie die Auftragsnummer ein und drücken Sie die <Tab>-Taste.
Der Auftrag wird eingelesen.
3. Wählen Sie im Menü Funktionen > Gruppe Einstellungen > Terminsuche, um die Kriterien für die Einlastung zu prüfen.

In diesem Beispiel sind folgende Einstellungen gewählt, damit die Einlastung Schritt für Schritt nachvollzogen werden kann:
- Automatisch Normalkapazität für die Bestimmung des Fertigungstermins.
- Manuell für die Auswahl der Aggregate.
4. Klicken Sie auf [OK], um die Einstellungen zu übernehmen und den Dialog zu schließen.

**Abb. H-84: Auftrag manuell einlasten**
- **A:** Priorität -1 = Aggregate zur manuellen Auswahl
- **B:** Liefertermin aus dem Auftrag darf nicht geändert werden
- **C:** Start der Produktion festlegen
- **D:** Priorität aus dem Auftrag

5. Legen Sie fest, ob die Aggregate zur manuellen Auswahl (A) in die Suche nach freien Kapazitäten einbezogen werden sollen.
Bei besonders eiligen Aufträgen ist diese Einstellung sinnvoll, denn die Aggregate mit der Priorität -1 werden sonst nicht berücksichtigt.
6. Legen Sie fest, ob der Liefertermin (B) aus dem Auftrag beibehalten werden soll oder ob er bei Engpässen geändert werden darf.
Wenn Sie die Checkbox markieren, darf der Liefertermin nicht geändert werden. Das kann bedeuten, dass andere Aufträge umgelastet werden müssen, um die benötigten Kapazitäten für den aktuellen Auftrag zu schaffen.
Wenn Sie die Checkbox nicht markieren, kann der Liefertermin entsprechend den freien Kapazitäten geändert werden.
Der geänderte Termin wird in den Auftrag zurückgeschrieben. Der neue Liefertermin wird der Tour entsprechend gesucht, wenn Sie in den Firmendaten die Einstellung so gewählt haben.
Wenn der Auftrag erst später produziert werden soll, dann geben Sie den Termin für den Produktionsstart (C) ein.
7. Prüfen Sie, ob die Priorität aus dem Auftrag (D) übernommen oder geändert werden soll.
Wenn Sie die Einstellung ändern, wird die neue Priorität nur dann übernommen und in den Auftrag zurück geschrieben, wenn Sie die Änderung über Menü Funktionen > Priorität in Auftrag übernehmen bestätigt haben.
Die Änderung der Priorität ist nur dann sinnvoll, wenn die entsprechenden Übergangszeiten zu allen Prioritäten eingerichtet sind.
8. Wählen Sie im Menü Start > Ausführen, um die Einlastung zu starten.
Wenn beim Einlasten Engpässe entstehen, werden folgende Dialoge angezeigt:
    - Lieferdatum
    - Aggregat-Auswahl bei Engpass
Das Vorgehen zum Lösen von Engpässen wird in den nachfolgenden Handlungssequenzen beschrieben.
Während des Einlastens wird angezeigt, welche Position oder Unterposition mit welcher Arbeitsart eingelastet wird.
Bei großen Stückzahlen durchläuft die Einlastung mehrere Phasen, bis ein optimales Ergebnis erzielt ist.
Damit ist der Auftrag vollständig eingelastet. In der Regel wird er nun durch einen Workflow-Task an die Produktion übergeben.
Sie können sich das Ergebnis anzeigen lassen.
9. Wählen Sie dazu im Menü Funktionen > Einlastungsergebnis.

**Abb. H-85: Ergebnis der Einlastung**

| Pos. | Aggregat | Arbeitsart | Zeit | Produkt/Bearb. | Stück | Datum | Schi... |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | Zuschnitt / Cutting | Zuschnitt / Cutting | 0,006000 | Float 5 mm A+W | 1 | 24.03.2014 | 1 |
| 1 | Zuschnitt / Cutting | Zuschnitt / Cutting | 0,006000 | Therm 6 mm A+W | 1 | 24.03.2014 | 1 |
| 1 | Rahmenbieger / Spa... | Rahmen biegen / ... | 0,001000 | Spacer 12 mm ALU A+W | 1 | 24.03.2014 | 1 |
| 1 | ISO Linie / IG Line | ISO-Fertigung / I... | 0,012500 | IG 5/12/Th6 A+W | 1 | 24.03.2014 | 1 |
| 1 | Versand / Shipping | Versand / Shipping | 0,015100 | IG 5/12/Th6 A+W | 1 | 24.03.2014 | 1 |
| ... | ... | ... | ... | ... | ... | ... | ... |

#### So lasten Sie eine einzelne Auftragsposition ein
Wenn im Auftrag nachträglich eine Position geändert wurde, kann diese gesondert eingelastet werden. Die übrigen Positionen des Auftrags bleiben unverändert eingelastet.
1. Wählen Sie Fertigung > Kapazitätsplanung > Einlasten > Einlasten Auftrag.
2. Geben Sie die Auftragsnummer ein und drücken Sie die <Tab>-Taste. Der Auftrag wird eingelesen.
3. Prüfen Sie den Versandtag und korrigieren Sie ihn ggf.

**Abb. H-86: Auftragsposition manuell einlasten**
- **A:** Einzelne Position einlasten
- **B:** Nummer der Position

4. Markieren Sie die Checkbox einzelne Position einlasten (A). Das Feld für die Nummer der Position wird freigeschaltet.
5. Tragen Sie die Nummer der Position (B) ein.
6. Wählen Sie im Menü Start > Ausführen, um die Position einzulasten. Wenn Engpässe auftreten, verfahren Sie weiter, wie in der nachfolgenden Einheit für den gesamten Auftrag beschrieben.
⇨ "Kapazitätsprobleme" auf Seite H-119

#### So löschen Sie einen Auftrag aus der Kapazitätsplanung
1. Wählen Sie Fertigung > Kapazitätsplanung > Einlasten > Einlasten Auftrag.
2. Geben Sie die Auftragsnummer ein und drücken Sie die <Tab>-Taste. Der Auftrag wird eingelesen.
3. Wählen Sie im Menü Funktionen > Einlastung löschen.
Die Daten der Einlastung werden gelöscht. Sie können den Auftrag nun erneut einlasten.
Mit dieser Funktion löschen Sie auch Aufträge aus der Kapazitätsplanung, die bereits fertig gemeldet wurden.

### Kapazitätsproblem lösen
Wenn Sie die Aufträge automatisch einlasten, müssen Sie nur bei Kapazitätsproblemen eingreifen - und das auch nur, wenn Sie die entsprechenden Einstellungen in den Firmendaten gewählt haben.
In den folgenden Handlungsschritten werden Problemfälle dargestellt, die auch bei der automatischen Einlastung oder beim Einlasten mehrerer Aufträge aus einem Nummernverwalter heraus entstehen können.

> **Position splitten**
> Wenn Sie eine Auftragsposition auf jeden Fall splitten wollen, müssen Sie den Auftrag manuell einlasten und im Dialog Terminsuche die Option manuell wählen.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So lösen Sie Engpässe beim Einlasten auf" auf Seite H-131
- "So splitten Sie eine Position" auf Seite H-132

#### So lösen Sie Engpässe beim Einlasten auf
Der Dialog Aggregat-Auswahl bei Engpass wird angezeigt, wenn die aktuelle Position nicht eingelastet werden kann.
1. Prüfen Sie, welche Position (A) an welchem Aggregat (B) nicht eingelastet werden kann.

**Abb. H-88: Manuelle Auswahl des Aggregats**
- **A:** Position, die eingelastet werden soll
- **B:** Aggregate, an denen der Engpass besteht. Aggregat mit Prio -1 ist farblich gekennzeichnet
- **C:** Zeitbedarf für die aktuelle Position
- **D:** Position einlasten
- **E:** Schichtzeit des Aggregats wird überschritten

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
2. Prüfen Sie, ob die Einlastung zum angezeigten Datum in einer anderen Schicht oder an einem anderen Aggregat möglich ist.
Über die Pfeilschaltflächen können Sie eine andere Schicht oder ein anderes Datum wählen.
Wenn Sie keine passenden Kapazitäten finden, müssen Sie die Position splitten, d. h. in mehrere Unterpositionen aufteilen. Dieser Vorgang ist in der nachfolgenden Handlungssequenz beschrieben.

3. Klicken Sie auf [Einlasten] (D), um die Position zu den geänderten Vorgaben einzulasten.
Die Positionen werden eingelastet und der Vorgang wird für das vorausgehende Aggregat wiederholt.
4. Wiederholen Sie die Schritte, bis keine Engpässe mehr angezeigt werden.
Die Einlastung des Auftrags wird durch eine Meldung bestätigt.

#### So splitten Sie eine Position
Der Dialog Aggregat-Auswahl bei Engpass wird angezeigt, wenn die aktuelle Position nicht eingelastet werden kann.

**Abb. H-89: Benötigte Zeit passt nicht in eine Schicht**
- **A:** Position, die eingelastet werden soll
- **B:** Aggregat, an dem der Engpass besteht
- **C:** Position teilen
- **D:** Zeit, die für die aktuelle Position benötigt wird
- **E:** Schichtzeit des Aggregats wird überschritten

1. Klicken Sie auf [Positionssplit] (C).

**Abb. H-90: Auftragsposition splitten**
- **A:** Auftragsposition
- **B:** Anzahl der Schichten oder Stückzahlen
- **C:** Produktionsdatum festlegen
- **D:** Übersicht über die Engpässe

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
In diesem Dialog geben Sie an, wie die Position aufgeteilt werden soll. Dazu haben Sie folgende Möglichkeiten:
- Sie geben die Stückzahl an, die problemlos an allen Aggregaten gefertigt werden kann.
- Sie geben an, in wie vielen Schichten die Gesamtstückzahl gefertigt werden soll. Die Stückzahlen für die entsprechenden Unterpositionen werden dann automatisch errechnet. Diese Version wird in den nachfolgenden Schritten vorgeführt.
- Sie lassen die Position automatisch splitten, indem Sie die Anzahl nicht angeben.
    - Mit [Anzahl = Schicht] wird die Stückzahl gleichmäßig auf die möglichen Schichten verteilt.
    - Mit [Anzahl = Stück pro Schicht] wird die Stückzahl gleichmäßig so aufgeteilt, dass die erste Schicht gefüllt wird und die restliche Stückzahl in der folgenden Schicht gefertigt wird.
    - Bei beiden Varianten wird die Teilung nur für das Aggregat berechnet, an dem die Einlastung stehen geblieben ist.
Wenn Sie mit der vorgeschlagenen Aufteilung nicht zufrieden sind, können Sie die Vorgaben löschen und die Aufteilung mit neuen Werten berechnen lassen.
2. Klicken Sie auf die Schaltfläche [Übersicht] (D), um zu prüfen, wo weitere Engpässe entstehen.
Anhand dieser Übersicht können Sie beurteilen, wie groß die Unterpositionen werden dürfen, damit an keinem der Aggregate Engpässe entstehen.

Wenn Sie den Dialog geschlossen haben, können Sie die Anzahl der Unterpositionen eintragen.
3. Geben Sie die Anzahl an (B), z. B. 3. Dieser Wert soll sich auf Schichten beziehen.
4. Klicken Sie auf [Anzahl = Schicht].

**Abb. H-91: Anzahl und Größe der Unterpositionen**
- **A:** Anzahl eingeben
- **B:** Anzahl für Schichten übernehmen
- **C:** Produktionsdatum festlegen
- **D:** Produktionsdatum, Schicht eingeben

Sie können nun für jede Position ein eigenes Produktionsdatum (C) festlegen.
5. Markieren Sie die Checkbox (C) und tragen Sie für alle Unterpositionen das Datum und die Schicht (D) ein.
6. Klicken Sie auf [OK], um die Aufteilung zu bestätigen und schließen Sie den Dialog mit [Ende].
Die Auftragsposition wird nach Ihren Angaben gesplittet.
Der Dialog Aggregat-Auswahl bei Engpass wird wieder angezeigt. Anschließend beginnt die Einlastung für jede der Unterpositionen wieder mit dem Versand.
7. Klicken Sie auf [Einlasten], um die Unterpositionen einzulasten.
Die Einlastung wird fortgesetzt und beim nächsten Engpass wieder unterbrochen. Beachten Sie hierbei, dass nun die Unterpositionen eingelastet werden und daher bei weiteren Engpässen diese unter Umständen wieder geteilt werden müssen.
8. Wiederholen Sie die Schritte 4 bis 7, bis keine Engpässe mehr angezeigt werden. Wenn Sie die Anzahl der Unterpositionen so gewählt haben, dass keine Engpässe mehr auftreten, wird die Einlastung erfolgreich beendet.

### Übungen
Mit den Aufträgen, die Sie in dieser Übung erfassen, sollen Sie die Einstellungen prüfen, die Sie in den Stammdaten der Kapazitätsplanung definiert haben. Es ist daher sinnvoll, dass Sie möglichst extreme Aufträge erfassen.
- Erfassen Sie mehrere Aufträge:
    - Zuschnitt von Einfachglas in großer Stückzahl.
    - Mehrere Positionen mit identischen Stücklisten, aber unterschiedlichen Maßen.
    - Positionen mit komplexen Arbeitsschritten, z. B. Modell in ISO mit Stufung.
- Lasten Sie die Aufträge manuell ein und verwenden Sie dazu unterschiedliche Modi (Einstellungen im Dialog Kriterien ändern):
    - automatisch
    - manuell
    - Einlasten ohne Kontrolle
Prüfen Sie die Unterschiede jeweils anhand des Einlastergebnisses.

> **Auftrag mehrfach einlasten**
> Sie können jeden Auftrag mehrmals einlasten, solange noch keine Position gefertigt wurde. Löschen Sie in dieser Übung die alte Einlastung, bevor Sie den Auftrag erneut, aber mit anderen Bedingungen, einlasten.

### Ergänzende Informationen
⇨ Softwarereferenz, “Voreinstellungen Firmendaten" auf Seite H-183
⇨ Softwarereferenz, "Einlasten NV" auf Seite H-278
⇨ Softwarereferenz, "Kriterien ändern (Modus Terminsuche)" auf Seite H-281
⇨ Softwarereferenz, "Lieferdatum" auf Seite H-283
⇨ Softwarereferenz, "Einlasten Auftrag" auf Seite H-284
⇨ Softwarereferenz, "Aggregat-Auswahl bei Engpass" auf Seite H-291
⇨ Softwarereferenz, "Positions-Split" auf Seite H-294

---

## Produktion

### Lernziele
- Rückmeldungen aus der Produktion einrichten.
- Erfassungsstellen einrichten.
- Statusmeldungen im Auftrag prüfen.
- Aufträge manuell fertig melden.
- Restmengen vom Vortag umlasten.

### Nutzen
- Aus der Produktion werden Rückmeldungen gesendet, die Auskunft über den aktuellen Status der Auftragspositionen und damit des Auftrags geben. Damit kann der Mitarbeiter im Verkauf prüfen, ob der Liefertermin eines Auftrags eingehalten wird.
- Verzögerungen durch Bruch oder Produktionsengpässe werden durch die Rückmeldungen sichtbar.

### Merke

| Begriff | Beschreibung |
| --- | --- |
| **Rückmeldungen** | Produktionsrückmeldungen dienen in A+W Business Pro dazu, Informationen über den Fortgang der Produktion zu liefern. Durch die Rückmeldungen wird der Status von Positionen und von Aufträgen aktualisiert. |
| **Statusmeldungen aus der Produktion** | Der Status jeder einzelnen Position wird während der Produktion umgesetzt. Wenn alle Positionen eines Auftrags denselben Status erreicht haben, wird der Status im Auftrag umgesetzt. |
| **Fertigmeldung** | Damit ein Auftrag fertig gemeldet werden kann, muss die Erfassungsstelle angelegt und in den Firmendaten zugeordnet sein, von der A+W Business Pro die Meldung erwartet. |
| **Manuelle Statusvergabe** | Jede (vergessene) Statusmeldung kann manuell nachgeholt werden. Sind die Meldungen an mehreren Aggregaten unterblieben, werden diese alle mit dem jüngsten Datum fertig gemeldet, das vergeben wurde. |
| **Voreinstellungen** | **Stammdaten:** Erfassungsstellen <br> **Firmendaten:** Register Lager/EK/EDI, Register Produktion, Register Kapa-Planung |

### Rückmeldungen zum Produktionsstand
Produktionsrückmeldungen dienen in A+W Business Pro dazu, Informationen über den Fortgang der Produktion zu liefern. Durch die Rückmeldungen wird der Status von Positionen und von Aufträgen aktualisiert.
Wenn Sie mit der Produktions-Software A+W Production arbeiten, können die Aufträge nach der Kapazitätsplanung an die Produktion übergeben werden. Die Produktion hat für jeden Produktionsbereich mindestens eine Erfassungsstelle. Von diesen Erfassungsstellen können Positionen oder Teilmengen an A+W Business Pro zurück gemeldet werden, um den Status umzusetzen.

Der Auftragsstatus kann auf folgende Arten umgesetzt werden:
- Wenn Sie nicht mit der Betriebsdatenerfassung (BDE) vom A+W Production arbeiten, können Sie Auftragspositionen und Aufträge manuell fertig melden.
- Wenn Sie mit der A+W Production-BDE arbeiten, werden Fertigmeldungen an die Kapazitätsplanung zurückgemeldet und setzen den Status der Auftragspositionen hoch. Sobald alle Positionen den gleichen Status haben, wird der Status im Auftragskopf hochgesetzt. Die Statusrückmeldungen werden im Dialog Übersicht Rückmeldungen angezeigt. So erhalten Sie einen zeitnahen Überblick über den Produktionsfortschritt eines Auftrags bzw. über den aktuellen Tag.

Ein Arbeitsgang, der durch A+W Production oder manuell fertig gemeldet worden ist, wird fixiert und kann in der Kapazitätsplanung nicht mehr verändert werden. Wenn der komplette Auftrag fertig gemeldet wurde, wird er in der Kapazitäts-Statistik angezeigt.
Rückmeldungen werden vom A+W Production erstellt und durch den A+W Business Pro-Interface-Service eingelesen. Dieses Programm läuft zentral auf dem Server und prüft periodisch die definierten Verzeichnisse nach Neueingängen.

> **Rückmeldungen aus der Produktion**
> Rückmeldungen von A+W Production können in A+W Business Pro auf unterschiedliche Weise empfangen und bearbeitet werden. Dieses Thema ist ausführlich im Part Fertigung dargestellt. Im Tutorial zur Kapazitätsplanung ist die Darstellung daher stark verkürzt. Dateilose Rückmeldung können nur mit Capacity Planning verarbeitet werden.

### Einstellungen für Rückmeldungen
In den Firmendaten müssen Sie die Einstellungen für die Produktionsrückmeldung prüfen.

**Abb. H-92: Stammdaten – Einstellungen für Produktionsrückmeldungen**
- **A:** Produktionsmanager
- **B:** URL für den PPS-Webservice
- **C:** URL für den ERP-Webservice
- **D:** Einstellungen für Produktionsrückmeldungen
- **E:** Dateilose Rückmeldungen

> **A+W Business Pro**
> Die Programmversion A+W Business Pro arbeitet standardmäßig mit dem Produktionsmanager (A). Damit sind dateilose Rückmeldungen nicht möglich.
> Die URL des ERP-Webservice ist für Produktionsübergabe und Produktionsrückmeldung im OrderXML-Format gültig. Diese Einstellungen sind im Tutorial Fertigung ausführlich beschrieben.

### Erfassungsstellen
Die Fertigmeldung der Arbeiten in einem Produktionsbereich erfolgt über die Barcode-Erfassungsstellen. In der Regel reicht eine Erfassungsstelle pro Produktionsbereich aus. Sie können jedoch auch zwei Erfassungsstellen in einem Produktionsbereich einrichten.

> **Beispiel: ESG-Versand**
> Eine Erfassungsstelle steht bei den gefertigten Gläsern, die auf den Gestellen abgestellt werden, und eine im Beschlagslager, wo die Beschläge zusammengestellt werden.
> Erst wenn alle Positionen (sowohl die Glas- als auch die Beschlagspositionen) denselben Status haben, z. B. 540, ist der Auftrag versandbereit und der Auftrag wird z. B. auf den Status *Ware außer Haus* gesetzt.

Produktionsrückmeldungen der Betriebsdatenerfassung (BDE) werden z. B. von folgenden Stationen erwartet:

| BDE-Status | Bedeutung |
| :--- | :--- |
| 455 | Bruch in Produktion |
| 460 | Zuschnitt fertig |
| 465 | Schleifen fertig |
| 470 | Bohren fertig |
| 475 | Kontrolle |
| 480 | Siebdruck fertig |
| 485 | ESG fertig |
| 490 | VSG fertig |
| 495 | Wölben fertig |
| 500 | Heat-Soak-Ofen fertig |
| 510 | ISO fertig |
| 515 | Clear Shield fertig |
| 540 | versandfertig |

Detaillierte Auskunft über den aktuellen Produktionsstand des Auftrags und der Positionen gibt der Dialog Übersicht Rückmeldungen. Dort sehen Sie für jede Position, welche Produktionsbereiche die Position durchlaufen hat und welche sie noch durchlaufen muss.
Sobald eine Position einen Produktionsbereich durchlaufen hat und durch die Erfassungsstelle registriert wurde, wird der Status hochgesetzt. Wenn für alle Positionen eines Auftrags alle Arbeitsgänge in einem Produktionsbereich erledigt sind, wird automatisch der Status des Auftrags hochgesetzt. Da zu diesem Zeitpunkt die Maschinen nicht mehr gewechselt werden, an denen die Arbeiten ausgeführt wurden, werden die Kosten neu berechnet und in den Auftrag zurückgeschrieben.

### Erfassungsstelle für Rückmeldungen
Wenn Sie die Rückmeldungen aus A+W Production in A+W Business Pro auswerten wollen, müssen Sie eine Erfassungsstelle für die Fertigmeldung zuordnen. Diese Zuordnung wird für Produktionsrückmeldungen und BDE-Rückmeldungen benötigt.

**Abb. H-93: Stammdaten – Erfassungsstelle für Rückmeldung**
Wenn Rückmeldungen von AWBar oder A+W Production in Dateien der folgenden Typen STSP, STSL, STSD, STSB, STSG geschrieben werden, muss eine Erfassungsstelle ausgewählt werden, die einem Statuspunkt zugewiesen ist. Wenn eine solche Erfassungsstelle nicht zugewiesen wurde, erzeugt die Rückmeldung einen Fehler.

### Statusmeldungen
In der Kapazitätsplanung müssen die Status-Rückmeldungen den Produktionsbereichen zugeordnet werden, in denen die Meldung den Positions- oder Auftragsstatus erhöhen soll. Sie können pro Produktionsbereich nur einen Status zuordnen.
⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-200

#### Positions- und Auftragsstatus
Nach dem Einlasten eines Auftrags in die Kapazitätsplanung wird der Auftragsstatus umgesetzt. In der Historie wird diese Umsetzung dokumentiert.
Die Vergabe des Status ist für die Positionen und den gesamten Auftrag unterschiedlich. Wenn eine Position vollständig gefertigt ist, erhält sie den Status versandbereit, der gesamte Auftrag ist jedoch noch nicht versandbereit.

**Abb. H-94: Übersicht Produktionsrückmeldungen**
- **A:** Status des Auftrags
- **B:** Status der Position

Erst wenn alle Positionen eines Auftrags auf den Status versandbereit gesetzt sind, wird auch der Status für den Auftrag hochgesetzt.

#### Automatische Statusvergabe bei verschiedenen Arbeitsarten
Im Auftrag können die Positionen so unterschiedlich sein, dass sie verschiedene Arbeitsarten durchlaufen, bevor ein gemeinsamer Positionsstatus erreicht ist.

> **Beispiel**
> Von fünf Positionen muss nur eine Position den Produktionsbereich ESG-Ofen durchlaufen. Wenn dies die einzige Position ist, die in diesem Produktionsbereich für den Auftrag fertig gemeldet werden muss, würde normalerweise der Status im Auftragskopf automatisch erhöht, sobald diese Position am ESG-Ofen fertig gemeldet wird.
> Dies darf jedoch nicht geschehen, wenn die anderen Auftragspositionen diesen Fertigungsstatus noch nicht erreicht haben. Diese befinden sich z. B. noch im Produktionsbereich Zuschnitt und müssen noch den Produktionsbereich Bohren durchlaufen, bevor der Auftragsstatus auf ESG-Ofen hochgesetzt werden kann.
> Die Kapazitätsplanung prüft daher, welchen Produktionsbereich die vier Positionen vor dem ESG-Ofen durchlaufen müssen, in diesem Beispiel den Produktionsbereich Bohren. Erst wenn die vier Positionen im Produktionsbereich Bohren fertig gemeldet werden, wird der Auftragsstatus auf den Status ESG-Ofen erhöht.

#### Manuelle Statusvergabe
Es kann vorkommen, dass Erfassungsstellen die Fertigmeldungen von Positionen nicht registrieren und dadurch der Status vorerst nicht hochgesetzt wird. Sobald jedoch ein nachfolgender Produktionsbereich diese Positionen fertig meldet, geht die Kapazitätsplanung (nicht A+W Production) stillschweigend davon aus, dass der vorherige Produktionsbereich durchlaufen wurde. Der Status wird automatisch gesetzt.

> **Beispiel**
> Angenommen, der Produktionsbereich Bohren hat die Positionen fertig gemeldet. Der Zuschnitt ist immer vor dem Bohren. Wurde die Position im Zuschnitt nicht fertig gemeldet, geht die Kapazitätsplanung trotzdem davon aus, dass der Zuschnitt gemacht wurde, und setzt auch für den Produktionsbereich Zuschnitt den Status hoch.
> Bei der Erfassungsstelle Bohren sind dann jedoch keine Daten mehr über den verwendeten Schneidtisch vorhanden. Auch die Daten für den Produktionsbeginn fehlen. In diesem Fall werden die Daten und die Kosten nur für den Produktionsbereich Bohren aktualisiert, nicht jedoch für den Bereich Zuschnitt. Deshalb sollten die Fertigmeldungen an jeder Erfassungsstelle ordnungsgemäß erfolgen.

### Fertigmeldung
Aufträge und Positionen werden durch die Rückmeldungen aus der Produktion fertig gemeldet.
Eine Fertigmeldung geht immer davon aus, dass der vorausgegangene Arbeitsschritt fertig war. Wenn diese Fertigmeldung unterblieben ist, wird sie automatisch nachgeholt. Dabei wird für den vorausgegangenen Bereich ohne Fertigmeldung das Datum der jüngsten Fertigmeldung übernommen. Dieses Datum entspricht daher nicht dem Datum, an dem die Position in dem Produktionsbereich tatsächlich gefertigt wurde.
Wenn Sie nicht mit den (automatischen) Rückmeldungen aus der Betriebsdatenerfassung (BDE) arbeiten, können Sie Aufträge oder Auftragspositionen manuell für die unterschiedlichen Stationen der Produktion fertig melden, z. B. pro Lauf, nach Datum oder pro Auftrag.

**Abb. H-95: Zuschnitt manuell fertig melden**
Im Dialog Leitstand werden die Daten entsprechend aktualisiert.

**Abb. H-96: Leitstand**
- **A:** Offener Auftrag
- **B:** Fertig gemeldeter Auftrag

Wenn der Auftrag manuell komplett fertig gemeldet ist, werden alle bis dahin noch nicht gemeldeten Werte auf den Tag verschoben, an dem fertig gemeldet wurde. In diesem Fall sind die Produktionsdaten in grüner Schrift angezeigt.
Der Dialog Leitstand wird in einer separaten Einheit ausführlich behandelt.

### Restmengen vom Vortag
Wenn Sie einen Auftrag haben, der am Vortag hätte produziert werden müssen – aber nicht produziert wurde – müssen Sie diese Restmenge in den aktuellen Tag umlasten. Die nicht begonnenen Aufträge werden über ein Batch-Programm (Workflow-Task) gesucht und umgelastet. Da dies ein sehr rechenintensiver Vorgang ist, ist der Batch als Workflow-Task hinterlegt und läuft automatisch vor Betriebsbeginn, also nach 24:00 Uhr. Weitere Erklärungen zum Workflow-Task finden Sie unter:
⇨ "Automatisch einlasten" auf Seite H-118

Über Statuseinstellungen sucht das Programm alle Aufträge, die am Vortag hätten produziert werden sollen. Dabei wird geprüft, ob mit der Produktion schon begonnen wurde. Die gefundenen Aufträge werden ohne Prüfung der Kapazitäten umgelastet.

> **Beispiel Arbeitstag 22.07.**
> **Auftrag A:** 100 Stk, Produktionsbeginn 21.07. Am 21.07. sind schon 20 Scheiben zugeschnitten. Diese Positionen werden nicht berücksichtigt: Die begonnene Arbeit steht in der Produktion und der Werker wird die Arbeit heute (22.07.) fortsetzen.
> **Auftrag B:** 30 Stk, Produktionsbeginn 21.07. Keine Scheibe ist zugeschnitten. Um 4:00 Uhr läuft der Batch und bucht den Auftrag auf den 22.07. (heute) um.

Die Statuseinstellungen für die Suche nach Aufträgen legen Sie in aller Regel nur einmal fest.

**Abb. H-97: Status für Restmengenübertragung**

Als Mindeststatus muss der Auftrag bereits in der Kapazitätsplanung (erfolgreich) eingelastet sein. Aufträge, die noch nicht eingelastet sind, können auch nicht umgelastet werden.
Der Höchststatus (Sperrstatus) hängt davon ab, wie Ihr Betrieb organisiert ist. Wenn Sie den Lieferschein erst nach der Fertigmeldung des Auftrags drucken, könnte dieser Druckstatus die obere Grenze für die Suche sein.

> **Rückstand aufholen**
> Wenn Sie feststellen, dass die Umlastung von Restmengen aus dem Vortag immer neue und größere Restmengen erzeugt, können Sie bei der Planung der nächsten Schichten eine geringere Auslastung anstreben. Damit schaffen Sie einen Puffer für die umgelasteten Aufträge. Alternativ dazu sind Überstunden, Sonderschichten oder ein ganzer Tag nur für die Alt-Aufträge denkbar.

### Bruchrückmeldung
Zu den Rückmeldungen aus der Produktion gehören auch die Bruchrückmeldungen. Beispiele für Bruchrückmeldungen sind:
- Scheiben, die nach dem Durchlauf einer Erfassungsstelle zu Bruch gegangen sind.
- Scheiben, die Produktionsmängel aufweisen und deshalb neu produziert werden müssen.

Damit A+W Business Pro Bruchrückmeldungen bei der Statusvergabe berücksichtigen kann, muss in den A+W Business Pro-Stammdaten eine Erfassungsstelle zugeordnet werden.
⇨ Stammdaten, "Erfassungsstellen Produktion" auf Seite B-860

> **Fertigmeldung vor Bruchmeldung**
> Wenn eine Einheit in den nächsten Produktionsbereich kommt, ist sie in der Regel an der vorigen Erfassungsstelle fertig gemeldet worden. Die Bruchmeldung kann dann sofort erfasst werden.
> Bei den manuellen Bruchmeldungen muss berücksichtigt werden, dass zunächst eine Fertigmeldung vorliegen muss. Wenn diese fehlt, muss die Einheit zuerst fertig gemeldet werden, um anschließend die Bruchmeldung zu erfassen.

#### Produktionspapiere drucken
Sie können auswerten lassen, welche Stückzahl von welchem Auftrag an einer bestimmten Maschine gefertigt werden muss und wann der Auftrag an welcher Folgemaschine benötigt wird.

**So drucken Sie eine Liste der Aufträge an einem bestimmten Aggregat**
1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigmeldung > Manuell.
2. Tragen Sie in den Feldern Datum von und Datum bis (A) den Zeitraum ein, für den Sie die Liste erzeugen wollen. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird die Liste nur für diesen einen Tag erzeugt.
3. Markieren Sie die Checkboxen für die Druckeinstellungen (B), z. B., um alle Aggregate aufzulisten. Wenn Sie die Liste nur zu einem einzelnen Aggregat erzeugen wollen, so wählen Sie dieses aus (C).
4. Wählen Sie im Menü Start > Suchen, um die Suche zu starten.

**Abb. H-99: Detaillierte Produktionsliste**
- **A:** Unterpositionen der Auftragsposition 1
- **B:** Auftragsnummer

In dieser Übersicht werden zu jeder Arbeitsart die Unterpositionen jeder Position aufgelistet.
Wenn Sie die Ausgabe an einen Drucker senden, achten Sie darauf, dass Sie ein Querformat benötigen, damit alle Daten dargestellt werden können.

**Abb. H-100: Beispiel Produktionsliste (Seite 1)**
Pro Aggregat und Tag wird eine Seite erstellt.

### Auftrag manuell fertig melden
Beim manuellen Fertigmelden haben Sie folgende Möglichkeiten:
- Aufträge komplett
- Einzelne Auftragspositionen komplett
- Teilmenge einer Auftragsposition

Im nachfolgenden Beispiel wird eine Teilmenge fertig gemeldet.

> **Scannen**
> Wenn Sie mit einem Scanner arbeiten, prüfen Sie zuerst im Menü Optionen, ob die Erfassung des Barcodes aktiviert ist. Der Cursor steht dann automatisch in dem Feld für den Barcode.

**So melden Sie einen Auftrag an einem Aggregat fertig**
1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigmeldung > Manuell. Der Dialog Manuelle Fertigmeldungen wird geöffnet.
2. Wählen Sie im Menü Funktionen > Einstellungen.
3. Wählen Sie die Aggregate aus, zu denen Sie die Fertigmeldungen erfassen wollen, und übernehmen Sie die Auswahl mit [OK]. Sie können mehrere Aggregate markieren.
4. Prüfen Sie, ob die Option Fertigmeldung (A) aktiviert ist.
5. Geben Sie die Auftragsnummer (C) ein oder erfassen Sie den Barcode. Der Cursor springt in das nächste Feld.
6. Geben Sie im Feld Position von (D) die Positionsnummer ein und drücken Sie die <Tab>-Taste. Die Position wird eingelesen und die Stückzahl wird angezeigt.
7. Markieren Sie die Checkbox mit Mengenangabe (F). Wenn Sie den Barcode per Scanner erfasst haben, wird genau 1 Scheibe fertig gemeldet. Sie müssen daher die Checkbox markieren und die Anzahl der fertigen Scheiben manuell eintragen. Wenn Sie aber die gesamte Position fertig melden wollen, dann markieren Sie die Checkbox Position komplett. Die Mengenangabe entfällt dann.
8. Tragen Sie im Feld Menge (E) die Stückzahl ein, die Sie fertig melden wollen.
9. Markieren Sie im Feld Aggregat-Auswahl (G) das Aggregat, an dem die Stückzahl fertiggestellt wurde.
10. Ergänzen Sie ggf. das Datum und die Schicht.
11. Klicken Sie auf [Position fertig melden (F9)].

**Abb. H-104: Teilmenge fertig gemeldet**
Die angegebene Stückzahl wird fertig gemeldet.

### Bruchmeldung manuell erfassen
Sie können Bruchmeldungen nur für Positionen erfassen, die bereits fertig gemeldet wurden. Für die manuelle Bruchmeldung haben Sie folgende Möglichkeiten:
- **Bruchmeldung Eingang:** Die angegebenen Stückzahlen werden am Eingang des Aggregats als Bruch gemeldet. Sie müssen an der vorherigen Maschine erneut gefertigt werden.
- **Bruchmeldung Ausgang:** Die angegebenen Stückzahlen werden am Ausgang des Aggregats als Bruch gemeldet. Sie müssen an derselben Maschine erneut gefertigt werden.

**So melden Sie zu einer Position einen Bruch**
1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigmeldung > Manuell. Der Dialog Manuelle Fertigmeldungen wird geöffnet.
2. Wählen Sie im ggf. Menü Funktionen > Einstellungen die Aggregate aus, zu denen Sie die Bruchmeldungen erfassen wollen.
3. Tragen Sie die Auftragsnummer (B) ein oder erfassen Sie den Barcode. Der Cursor springt in das nächste Feld.
4. Geben Sie die Positionsnummer (C) ein und drücken Sie die <Tab>-Taste. Die Position wird eingelesen und die Stückzahl wird angezeigt.
5. Wählen Sie die Meldungsart (A) aus. Mit dieser Einstellung entscheiden Sie, ob die fehlerhaften Scheiben am vorigen oder am selben Aggregat erneut gefertigt werden müssen.
6. Tragen Sie im Feld Menge (D) die Stückzahl ein, die Sie fertig melden wollen. Wenn Sie den Barcode per Scanner erfasst haben, wird genau 1 Scheibe gemeldet.
7. Markieren Sie im Feld Aggregat-Auswahl (G) das Aggregat, an dem der Bruch gemeldet werden soll.
8. Ergänzen Sie ggf. das Datum und die Schicht.
9. Klicken Sie auf [Position fertig melden (F9)].

**Abb. H-106: Bruchmeldung für Teilmenge**
Die Daten werden gespeichert. Die Bestätigung wird unter der Schaltfläche angezeigt.
Wenn die beanstandeten Scheiben neu gefertigt wurden, wird der Positionsstatus hochgesetzt.

> **Bruchmeldung kann nicht bestätigt werden**
> Wenn die Bruchmeldung nicht bestätigt wird, müssen Sie die Position zuerst fertig melden. Nachdem Sie die Fertigmeldung abgeschlossen haben, können Sie die Bruchmeldung erfassen.

### Fertigungsstand prüfen
Sie können den Fertigungsstand der Aufträge detailliert prüfen und vergessene Fertigmeldungen nachholen. Dazu können Sie sich die Aufträge eines Kunden oder alle Aufträge zu einem bestimmten Liefertermin gesammelt anzeigen lassen.

**So prüfen Sie den Fertigungsstand einzelner Auftragspositionen**
1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigungsstand Auftrag.
2. Tragen Sie die Nummer des Auftrags oder des Kunden ein. Wenn Sie das Lieferdatum eintragen, schränken Sie die Auswahl weiter ein. Oder Sie lassen sich damit alle Aufträge zum angegebenen Datum anzeigen.
3. Wählen Sie im Menü Start > Suchen, um die Daten einzulesen. Die Auftragsdaten werden eingelesen und im Register Auswahl angezeigt. Wenn Sie als Auswahlkriterium die Kundennummer gewählt haben, werden alle Aufträge des Kunden angezeigt, auch die bereits gefertigten.
4. Wechseln Sie zum Register Positionen, um den Fertigungsstand der einzelnen Auftragspositionen zu prüfen.
5. Prüfen Sie das Datum, zu dem Sie die Position fertig melden wollen.
6. Markieren Sie die Checkbox Fertig melden (C) in der Position, die bereits vollständig gefertigt wurde. Eine Sicherheitsabfrage wird angezeigt. Wenn Sie die Meldung bestätigt haben, wird die Stückzahl der Position in die Spalte komplett fertig eingetragen.

### Fertigmeldungen nachholen
Ob Aufträge nicht fertig gemeldet wurden, können Sie auch prüfen, indem Sie sich die Restmengen vom Vortag anzeigen lassen.

**So prüfen Sie, ob Restmengen vom Vortag übrig geblieben sind**
1. Wählen Sie im Modul Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Restmengen anzeigen.
2. Wählen Sie den Mindest-Status (A). Die Aufträge müssen mindestens in die Kapazitätsplanung eingelastet sein. Ein niedrigerer Status ist daher nicht sinnvoll.
3. Markieren Sie die Checkboxen fertig melden (B) aller Aufträge, die nicht fertig gemeldet wurden, aber vollständig gefertigt sind.
4. Klicken Sie auf [OK], um die Daten zu speichern. Der Status der Aufträge wird umgesetzt. Die fertig gemeldeten Aufträge werden aus der Übersicht gelöscht.

**Abb. H-110: Nachgeholte Fertigmeldungen**
Sie können im Dialog Leitstand (Auftrag) prüfen, ob die Daten korrekt umgesetzt wurden. Alle nachgeholten Fertigmeldungen werden auf das aktuelle Tagesdatum gesetzt.

> **Anzeige fertiger Aufträge**
> Sie können in den Einstellungen zum Leitstand angeben, dass fertig gemeldete Aufträge nicht angezeigt werden sollen. Bei der Wahl dieser Option können Sie die Statusumsetzung nicht wie in dem Beispiel prüfen.

### Übungen
- Melden Sie einen Ihrer Aufträge manuell komplett fertig.
- Melden Sie in einem Ihrer Aufträge eine Position fertig.
- Erfassen Sie zu einer ISO-Scheibe eine Bruchmeldung. Beachten Sie dabei, dass die Position oder der Auftrag zuvor fertig gemeldet sein muss.
- Melden Sie die Restmengen von Vortag fertig. Diese Übung können Sie nur ausführen, wenn Restmengen vorhanden sind.

### Ergänzende Informationen
⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-200
⇨ Softwarereferenz, "Restmengenübertragung" auf Seite H-300
⇨ Softwarereferenz, "Datum" auf Seite H-302
⇨ Softwarereferenz, "Manuelle Fertigmeldung" auf Seite H-308
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-317
⇨ Softwarereferenz, "Übersicht Rückmeldungen" auf Seite H-328
⇨ Softwarereferenz, "Auslastung zu Datum" auf Seite H-361
⇨ Softwarereferenz, "Restmengen anzeigen" auf Seite H-371

---

## Produktionskosten

### Lernziele
- Maschinen- und Zeitkosten im Auftrag oder Angebot prüfen.

### Nutzen
- Schon vor der Produktion eines Auftrags kann festgestellt werden, ob in der Preisgestaltung die Zeit- und Maschinenkosten im Auftrag ausreichend berücksichtigt sind.

### Merke

| Begriff | Beschreibung |
| --- | --- |
| **Produktionskosten** | Das sind: Lohnkosten pro Einheit, Maschinenkosten pro Stunde, Variable Kosten pro Stunde, z. B. für Versicherungen. Diese Kosten werden pro Maschine hinterlegt und bei der Einlastung geprüft. |
| **Produktionskosten im Angebot** | Um die Produktionskosten für ein Angebot zu ermitteln, muss ein Workflow-Task eingerichtet sein, der die Angebote an die Kapazitätsplanung übergibt. |
| **Tatsächliche Kosten** | Erst in der Produktion werden die tatsächlichen Kosten ermittelt, denn erst dann ist entschieden, welche Maschinen eingesetzt worden sind. Diese tatsächlichen Kosten werden mit den Rückmeldungen in den Auftrag zurückgeschrieben. |

### Zeitkosten
Die Zeitkosten für Aufträge und ggf. für Angebote werden vom Programm errechnet. So können Sie vor der Fertigung prüfen, ob der Auftragswert bei den voraussichtlichen Zeitkosten noch gedeckt ist.
Die Kalkulation der Produktionskosten basiert auf folgenden Vorgaben:
- Maschinenkosten pro Stunde
- Variable Kosten pro Stunde, z. B. Versicherungskosten
- Kosten pro Vorgabezeiteinheit, z. B. Lohnkosten pro Einheit

Diese Kosten werden pro Maschine hinterlegt und bei der Einlastung geprüft.

**Abb. H-111: Zusammensetzung der Kosten für eine Maschine**
- **A:** Kostensätze
- **B:** Gesamtkosten pro gefertigter Einheit

Die bei der Planung errechneten Werte für eine Auftragsposition und den gesamten Auftrag werden nach der Fertigmeldung erneut berechnet. Sie können sich dann vom ursprünglichen Wert unterscheiden, z. B., weil die Fertigung an einer anderen Maschine ausgeführt wurde als ursprünglich geplant.

Im Dialog Fertigungsstand Auftrag können Sie sich die aktuellen Produktionskosten anzeigen lassen.

**Abb. H-112: Aktuelle Produktionskosten prüfen**
- **A:** Geplante Produktionskosten für den gesamten Auftrag
- **B:** Bisher tatsächlich angefallene Produktionskosten

### Kostenstellen
Sie können für die Analyse der Produktionskosten eigene Kostenstellen einrichten. Damit können Sie die Kosten über definierbare Zeiträume auswerten.

**Abb. H-113: Kostenstellen für Produktionskosten auswerten**
- **A:** Sortierung nach Produktionsbereich – AV-Bereich oder AV-Bereich – Produktionsbereich
- **B:** Auswertung der Produktarten, Produktgruppen oder Produkte

In dieser Auswertung werden die Kostenstellen für Produktarten aufgeführt. Sie können die Auswertung nach Kostenstellen oder nach AV-Bereichen sortiert anzeigen lassen.
Die Kostenstellen und die Auswertung können Sie nach den Anforderungen in Ihrem Betrieb einrichten. In den folgenden Beispielen soll die letzte Zeile mit der Auswertung Kostenstelle ESG bearbeitet näher erklärt werden.

> **Kostenstellen in A+W Business Pro-Stammdaten**
> Die Kostenstellen der Kapazitätsplanung haben keine Verbindung zu den Kostenstellen, die Sie im Modul Stammdaten einrichten.

#### Prinzip der Auswertungsspalten
In den Spalten wird jeweils festgelegt, was die Abfrage auswerten soll.

**Abb. H-114: Kostenstellen definieren**

| Spalte | Beschreibung |
| --- | --- |
| **A** | **Hauptproduktart:** Nummer der Produktart aus den A+W Business Pro Stammdaten |
| **B** | **Nr 1, Nr 2:** Nummer der Produktgruppe oder Produktart im Feld Typ |
| **C** | **Typ 1, Typ 2:** 0 = Keine Vorgabe, 1 = Produktart, 2 = Produktgruppe |
| **D** | **Priorität:** Reihenfolge der Abfrage |
| **E** | **Ausschluss:** Produkte, die von der Auswertung ausgeschlossen sind. |

Mit der Kombination der Spalten Nr und Typ stellen Sie ein, was in der Stückliste gesucht werden soll.

> **Beispiel: Auswertung von ESG bearbeitet**
>
> | HPA | Nr 1 | Nr 2 | Typ 1 | Typ 2 | Priorität |
| :-- | :--- | :--- | :---- | :---- | :--- |
| 2 | 20 | 0 | 1 | 0 | 19 |
>
> **Hauptprodukt:** ESG
> **Produktart:** Bearbeitungen
> **Typ 1:** Produktart
>
> In diesem Beispiel sehen Sie, dass im Hauptprodukt der Produktart ESG (2) nach dem Typ 1 (also Produktart) mit der Nummer 20 (Bearbeitungen) gesucht werden soll. Das bedeutet, dass in diese Kostenstelle nur ESG mit Bearbeitungen einfließen soll.

Bevor Sie mit dem Anlegen von Kostenstellen beginnen, sollten Sie sich überlegen, in welcher Reihenfolge die Kostenstellen abgefragt werden sollen. Diese Reihenfolge wird in der Spalte Priorität festgelegt.

> **Beispiel ESG**
> Sie fragen erst ab, ob es sich um ein ESG mit Bearbeitung handelt (Kostenstelle Nr. 7 mit Prio 19).
> Wenn dies nicht der Fall ist, kommt die Folge-Abfrage, also Prio 20.
> Das ESG, das nicht bearbeitet ist, fließt automatisch in die Kostenstelle ESG (Kostenstelle Nr. 6 mit Prio 20).

In der Spalte Ausschluss können Sie ein Produkt von der Regel ausschließen, indem Sie die Produktnummer eintragen. Die Produktnummer muss in Klammern stehen.

> **Beispiel**
> Alle ESG-Scheiben werden gesäumt. Deshalb möchten Sie nicht, dass das gesäumte ESG-Scheiben in die Kostenstelle ESG mit Bearbeitung einfließt. Dies können Sie ausschließen, indem Sie die Produktnummer für Säumen eintragen.

Eine ausführliche Beschreibung zur Definition der Spalten finden Sie im Part Fertigung. Dort wird die Definition der Vorschauspalten beschrieben, die nach demselben Prinzip festgelegt werden.
⇨ Fertigung, "Prinzip der Vorschauspalten" auf Seite E-160

### Kostenkalkulation im Auftrag
Die Materialpreise werden in A+W Business Pro aufgrund der Einkaufspreise kalkuliert. Daneben können aber auch die Zeit- und Maschinenkosten im Auftrag eingesehen werden.
Diese Kosten werden pro Auftrag in der Kapazitätsplanung während der Einlastung ermittelt und im Auftrag angezeigt.
Die Material- und Zeitkosten werden im Auftragskopf im Register Summen angezeigt.

**Abb. H-115: Kostenkalkulation: Auftrag - Register Summen**
Die Kosten werden im Auftragskopf über das Menü Funktionen > Gruppe Dokumente > Kosten- und Aufschlagskalkulation angezeigt.

**Abb. H-116: Kostenkalkulation im Auftrag**

| Kostenart | Teilkosten | Vollkosten |
| :--- | :--- | :--- |
| Materialkosten | 756.800,00000 | 0,00000 |
| Maschinenkosten | 4.022,40000 | 0,00000 |
| Personalkosten | 0,00000 | 0,00000 |
| Sondereinzelkosten | 0,00000 | 0,00000 |

### Kostenkalkulation für Angebote
Angebote können mit einem eigenen Workflow-Task an die Kapazitätsplanung übergeben werden, um die Kosten zu berechnen. Mit dieser Funktion können die Kosten im Angebotskopf und in der Positionserfassung genauso angezeigt werden wie im Auftrag. Die Angebote werden dabei nicht in die Kapazitätsplanung eingelastet und nicht an die Produktion übergeben.

### Übungen
- Prüfen Sie in den Aufträgen, die Sie an die Kapazitätsplanung übergeben haben, ob die Maschinenkosten angezeigt werden.
- Wenn Kosten fehlen: Prüfen Sie, ob Sie in den Aggregaten die Kosten eingetragen haben. Holen Sie dies ggf. nach und lasten Sie die Aufträge erneut ein. Prüfen Sie dann, ob die Kosten angezeigt werden.

### Ergänzende Informationen
⇨ Softwarereferenz, "Konten" auf Seite H-272
⇨ Softwarereferenz, "Kostenstellen-Definitionen" auf Seite H-274

---

## Leitstand

### Lernziele
- Navigation im Dialog Leitstand.
- Auslastung der Maschinen prüfen.
- Aufträge oder Auftragspositionen umlasten.

### Nutzen
- Im Dialog Leitstand erhalten Sie einen Überblick über die Auslastung der Aggregate.
- Über diesen Dialog können Sie alle Programme zum Prüfen und Umlasten der Aufträge erreichen.

### Merke
**Leitstand:** Vom Dialog Leitstand aus können Sie alle Dialoge zum Prüfen und Umlasten aufrufen.

### Konzept des Leitstands
Im Dialog Leitstand erhalten Sie eine Übersicht über die verplanten Stunden pro Aggregat und können im Bedarfsfall Termine verschieben.

**Abb. H-117: Planzeiten im Leitstand**
- **A:** Verplante Zeit für Zuschnitt
- **B:** Aggregate, an denen die Zeit verplant ist
- **C:** Aufträge, die an den Aggregaten gearbeitet werden sollen.

In diesem Beispiel sehen Sie die Auslastung des Produktionsbereichs Zuschnitt (A) für eine Woche. Die Detaildaten für die einzelnen Aggregate des Produktionsbereichs Zuschnitt (B) und die Aufträge (C), die an einem bestimmten Aggregat beteiligt sind, können Sie sich ebenfalls im Dialog Leitstand anzeigen lassen.

Über den Dialog Leitstand können Sie alle Programme zum Prüfen und Umlasten der Aufträge erreichen. Dies sind im Einzelnen folgende Dialoge:
- **Über Menü Funktionen:**
    - Auftrag auswählen > Leitstand (Auftrag)
    - Restmengen anzeigen > Restmengen
    - Grafische Darstellung der Auslastung
    - Auslastung > Auslastung zum Datum
- **Über Leitstand > Register Vorprozesse:**
    - [im Detail] > Produktionslisten
- **Über Leitstand (Auftrag) > Menü Funktionen:**
    - Übersicht Rückmeldungen
    - Einlasten > Einlasten Auftrag
    - Manuelle Vorgaben (Fertigungsstand Auftrag)

Im Dialog Leitstand navigieren Sie auf folgende Weise:

| Register | Aktion | Register / Dialog |
| :--- | :--- | :--- |
| **Bereiche** | Doppelklick auf Zeilenkopf | -> Aggregate (alle Aggregate) |
| | Doppelklick auf Produktionsbereich | -> Aggregate (nur Aggregate im Produktionsbereich) |
| **Aggregate** | Doppelklick auf Aggregat | -> Aufträge |
| | Doppelklick auf Detaildaten | -> Auftrag umlasten |
| | Doppelklick in Zeilenkopf | -> Leitstand (Aggregat) |
| **Aufträge** | Doppelklick auf Nummer | -> Leitstand (Auftrag) |
| | Doppelklick auf Detaildaten | -> Position umlasten |
| **Auftrag umlasten** | Klick in Zeilenkopf | -> Position umlasten |
| | Klick auf [Teile] oder [Vorprozesse] | -> Vorprozesse |
| **Position umlasten** | Kontext-Menü auf Vorgang (rechte Maustaste) | -> Rüstzeit löschen / Rüstzeit hinzufügen |
| **Arbeitsarten** | Klick in Zeilenkopf | -> Details |
| **Details** | Doppelklick auf Nummer | -> Leitstand (Auftrag) |
| **Vorprozesse** | Klick auf [Im Detail] | -> Produktionslisten |

### Leitstand – Auftrag
Um die Einlastung eines einzelnen Auftrags zu prüfen, steht der Dialog Leitstand (Auftrag) zur Verfügung.
Sie erreichen den Dialog über Leitstand > Menü Funktionen > Auftrag auswählen.

**Abb. H-118: Leitstand für einzelnen Auftrag**
- **A:** Liefertermin
- **B:** Versandtag

In diesem Beispiel sehen Sie, wie die Terminierung vom Liefertermin aus rückwärts gerechnet wird: Ein Tag vor dem Liefertermin muss der Auftrag den Produktionsbereich Versand erreichen und verpackt werden. Alle anderen Arbeiten finden unter Berücksichtigung der Produktions- und Übergangszeiten entsprechend früher statt.

Im Dialog Leitstand – Auftrag navigieren Sie auf folgende Weise:

| Register | Aktion | Register / Dialog |
| :--- | :--- | :--- |
| **Aggregate** | Doppelklick auf Aggregat | -> Verschieben II |
| | Doppelklick auf Datum | -> Detail |
| **Detail** | Klick auf Zellenkopf | -> Arbeitsarten |

### Leitstand – Aggregat
Um die Auslastung eines einzelnen Aggregats zu prüfen, steht der Dialog Leitstand - Auftrag zur Verfügung.
Sie erreichen den Dialog über Leitstand > Register Aggregat > Doppelklick in Zeilenkopf.

**Abb. H-119: Leitstand für einzelnes Aggregat**
- **A:** Aggregat
- **B:** Benötigte Stunden

In diesem Beispiel sehen Sie die Aufträge mit den Stückzahlen und den benötigten Zeiten an dem ausgewählten Aggregat. Der angezeigte Zeitraum entspricht der Anzeige im Dialog Leitstand, von dem aus Sie diesen Dialog geöffnet haben.
Im nächsten Register können Sie sich die Zeiten detailliert anzeigen lassen. Dazu können Sie den angezeigten Zeitraum dann so ändern, dass Sie die Auslastung z. B. nur noch für einen Tag sehen.
Die durch ein Splitting erzeugten Unterpositionen werden einzeln aufgeführt. Um eine Einlastung zu verschieben, können Sie mit einem Doppelklick auf die Auftragsnummer in den Dialog Leitstand (Auftrag) wechseln.

### Einlastung für einzelnen Auftrag verschieben
Sie möchten prüfen, ob der Versand für einen Auftrag verschoben werden kann, z. B., weil sich die Lieferung der Bestellteile verzögert.
In diesem Beispiel soll die Auslieferung eines Auftrags um mehrere Tage verschoben werden. Das bedeutet, dass sowohl der Liefertermin als auch die Einlastung geändert werden sollen.

**So prüfen Sie die Einlastung eines Auftrags**
1. Wählen Sie Modul Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen. Der Dialog Leitstand - Auftrag wird geöffnet.
2. Tragen Sie die Auftragsnummer ein.
3. Wählen Sie im Menü Start > Suchen, um die Daten einzulesen.

**Abb. H-120: Plandaten des aktuellen Auftrags**
- **A:** Aktueller Liefertermin
- **B:** Versand: Fertigstellung ein Tag vor Liefertermin

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
4. Tragen Sie im Feld Liefertermin den neuen Termin ein (B).
5. Klicken Sie auf [Ändern]. Die Anzeige wird erst beim nächsten Öffnen des Dialogs aktualisiert.
6. Wählen Sie im Menü Funktionen > Einlasten.

**Abb. H-121: Auftrag zum neuen Liefertermin einlasten**
Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
Der Auftrag wird mit dem neuen Liefertermin angezeigt. Er ist aber noch nicht zu diesem Termin eingelastet. Dies können Sie prüfen, indem Sie über die Schaltfläche [Ergebnis] den Dialog Einlastungsergebnis öffnen.

**Abb. H-122: Alte Einlastung**
Sie sehen in diesem Beispiel, dass der Versand zum alten Termin angezeigt wird. Wenn Sie den Dialog geschlossen haben, wird die Einlastung fortgesetzt.
7. Wählen Sie im Menü Start > Ausführen, um den Auftrag erneut einzulasten. Die Einlastung beginnt. Je nach Einstellung müssen Sie den Liefertermin für die einzelnen Positionen bestätigen. Nach der erfolgreichen Einlastung können Sie sich das Ergebnis erneut anzeigen lassen.

**Abb. H-123: Neue Einlastung**
Sie sehen in diesem Beispiel, dass der Versand zum neuen Termin angezeigt wird. Alle Arbeitsschritte an den vorgelagerten Aggregaten sind entsprechend verschoben.
8. Wechseln Sie zum Dialog Leitstand (Auftrag) zurück. Um die Anzeige zu aktualisieren, müssen Sie den Auftrag neu einlesen.
9. Wählen Sie dazu im Menü Start > Filter, um in den Such-Modus zu wechseln.
10. Tragen Sie die Auftragsnummer wieder ein und starten Sie die Suche, um den Auftrag einzulesen.

**Abb. H-124: Geänderte Plandaten des Auftrags**
- **A:** Neuer Liefertermin
- **B:** Versand: Fertigstellung ein Tag vor Liefertermin

### Aggregat ändern
Sie können die Einlastung von Auftragspositionen auf ein anderes Aggregat verschieben, z. B. von der ISO-Linie I auf die ISO-Linie II.

**So lasten Sie eine Auftragsposition auf ein anderes Aggregat um**
1. Wählen Sie im Modul Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen. Der Dialog Leitstand (Auftrag) wird geöffnet.
2. Tragen Sie die Auftragsnummer ein und starten Sie die Suche. Die Auftragsdaten werden eingelesen.
3. Klicken Sie doppelt auf das Aggregat, um den Leitstand für das Aggregat zu öffnen. Der Dialog Leitstand (Aggregat) wird mit dem Register Verschieben II angezeigt.
4. Markieren Sie die Checkbox der Position, die an ein anderes Aggregat verschoben werden soll.
5. Wählen Sie im Bereich Verschieben ein anderes Aggregat aus. Zusätzlich können Sie einen neuen Termin und/oder eine andere Schicht eintragen.
6. Über [Belegung] können Sie prüfen, ob die Verschiebung sinnvoll ist.
7. Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten. Die Einlastung wird verschoben. Die Änderung wird nach dem Neustart des Dialogs angezeigt.

### Übungen
- **Navigation im Leitstand üben:**
  Ausgangspunkt für die folgenden Übungen ist immer der Leitstand. Schließen Sie den aufgerufenen Dialog, um die nächste Übung auszuführen.
    - Lassen Sie sich die Aggregate zu einem Produktionsbereich anzeigen.
    - Wechseln Sie zum Dialog Leitstand (Aggregat).
    - Wechseln Sie zum Dialog Leitstand (Auftrag).
    - Lassen Sie sich die Daten im Register Im Detail anzeigen.
> **Tipp zur Navigationsübung**
> Drucken Sie sich die Übersicht über die Navigation aus. Sie finden diese auch in der Softwarereferenz.
> ⇨ "Navigation durch die Register und Dialoge" auf Seite H-317

- Wechseln Sie aus dem Leitstand zu einem Auftrag und prüfen Sie die Einlastung.
- Verschieben Sie den Liefertermin eines Auftrags um eine Woche. Was müssen Sie noch tun? Wann werden Sie die neuen Termine angezeigt?
- Lasten Sie einen Auftrag mit 10 großen ISO-Scheiben so ein, dass nur eine Einheit pro Tag produziert wird (Positionssplit und Produktionstermin festlegen).

### Ergänzende Informationen
⇨ Softwarereferenz, "Leitstand (Dialog)" auf Seite H-336
⇨ Softwarereferenz, "Leitstand (Aggregat)" auf Seite H-354
⇨ Softwarereferenz, "Leitstand (Auftrag)" auf Seite H-372
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-317
⇨ Softwarereferenz, "Produktions-Zeiten ändern" auf Seite H-329

---
# Softwarereferenz

# Übersicht
A+W Business Pro Capacity Planning gliedert sich in zwei Bereiche:
- Verwaltung der Kapazitätsplanung
- Planung und Überwachung der Kapazitäten

Die zugehörigen Dialoge finden Sie in den Modulen Kapazitätsplanung und Fertigung.
In dieser Softwarereferenz sind die Dialoge aus den beiden Modulen in folgenden Abschnitten beschrieben:
- "Verwaltung" auf Seite H-182
- "Kapazitätsplanung" auf Seite H-276

---

# Verwaltung
Um mit A+W Business Pro Capacity Planning arbeiten zu können, müssen die Stammdaten eingerichtet werden. Diese Daten bilden die Grundlage für alle weiteren Zuordnungen, Zeitplanungen und Auswertungen.

In diesem Kapitel finden Sie Informationen zu folgenden Stammdaten:
- "Voreinstellungen Firmendaten" auf Seite H-183
- "Allgemein" auf Seite H-189
- "Organisation" auf Seite H-199
- "Vorgabezeiten" auf Seite H-223

Neben der Beschreibung der Stammdaten finden Sie Informationen zu folgenden Themen:
- "Zuordnen" auf Seite H-237
- "Sperren" auf Seite H-254
- "Übersichten" auf Seite H-265
- "Einlastung" auf Seite H-277
- "Produktionsmeldungen" auf Seite H-301
- "Leitstand" auf Seite H-335

## Voreinstellungen Firmendaten
**Stammdaten > Firma > Firmendaten > Register Kapa-Planung**

**Abb. H-127: Firmendaten – Kapa-Planung**

Im Modul Stammdaten legen Sie die Grundeinstellungen für A+W Business Pro Capacity Planning fest. Diese Einstellungen beziehen sich vor allem auf die automatische Einlastung. Sie können bei einer manuellen Einlastung überschrieben werden.

> **Einstellungen ändern**
> Wenn Sie die Einstellungen in den Firmendaten und in den Stammdaten der Kapazitätsplanung geändert haben, müssen Sie A+W Business Pro neu starten, damit die Daten neu eingelesen werden.

### Kapazitätsplanung

**Version** Bei der Wahl des Programms zur Kapazitätsplanung müssen Sie darauf achten, wie Sie Rückmeldungen aus der Produktion empfangen. Wenn Sie mit A+W Business Pro Capacity Planning arbeiten wollen, müssen Sie den Eintrag A+W Business Kapazitätsplanung auswählen. Mit dieser Einstellung können Sie die Online-Meldungen nicht nutzen.

**Fehlermeldung aus autom. Kapazitätsplanung**
Mit der Wahl der Option legen Sie fest, an wen Fehlermeldungen gesendet werden.
- **An Auftragserfasser:** Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat. Solche Fehlermeldungen beziehen sich in aller Regel auf Termine, die nicht eingehalten werden können, weil nicht genügend Kapazitäten zur Verfügung stehen. Dies ist die Standard-Einstellung.
- **An Mitarbeiter:** Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet. Wählen Sie diese Option, wenn nur ein einziger Mitarbeiter die Aufträge bearbeitet, die nicht problemlos eingelastet werden konnten.

> **Aufträge automatisch einlasten**
> In der Regel werden die Aufträge durch einen Workflow-Task automatisch in festgelegten Intervallen in die Kapazitätsplanung eingelastet. Diese Funktion ist im Tutorial beschrieben.

### A+W Business-Kapazitätsplanung

**Schichtenzahl** Anzahl der Schichten, in denen Sie arbeiten. Die Schichtzeiten legen Sie im Modul Kapazitätsplanung im Dialog Kalender fest.
⇨"Kalender" auf Seite H-211

**Fertigungsterminmodus** Angabe, ob Sie mit offenen oder geschlossenen Kapazitäten arbeiten wollen.
- **Automatisch Normalkapazität:** Die Aufträge werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung (geschlossene Kapazitäten).
- **Automatisch volle Tage:** Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus (offene Kapazitäten). Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
- **Nur Aggregatwechsel:** Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet ist, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
- **Einlasten ohne Kontrolle:** Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist.

**Schichtfüllung bei Positionssplit** Große Positionen können auf mehrere Aggregate, Schichten oder Tage verteilt werden. Dazu geben Sie an, zu wie viel Prozent die Schicht(en) eines Aggregats durch das Splitting gefüllt werden dürfen, um Platz für andere Aufträge zu behalten.

**Aggregatabgleich** Wenn Sie mit mehreren Maschinen arbeiten, die dieselben Arbeitsarten ausführen können, kann die Planung diese Maschinen auf unterschiedliche Weise berücksichtigen:
- **Automatisch:** Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **Semi-automatisch:** Das Programm bietet die alternativen Maschinen zur Auswahl an. Wenn der Liefertermin nicht eingehalten werden kann, müssen Sie eingreifen.
- **Manuell:** Mit dieser Option müssen Sie bei jedem möglichen Wechsel (Maschine, Schicht usw.) manuell eingreifen. Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

**Einlastpriorität** Die Prioritäten aus dem Auftrag können beim Einlasten berücksichtigt werden:
- **Standard:** Die Kapazitäten der benötigten Aggregate werden geprüft und die Aufträge werden entsprechend der eingetragenen Priorität eingelastet.
- **Niedrige Priorität:** Standardmäßig werden alle Aufträge mit niedriger Priorität eingelastet.
- **Geänderte Priorität in Auftrag übernehmen:** Wenn die Priorität beim Einlasten geändert wird, soll sie automatisch in den Auftrag zurückgeschrieben werden.

**Produktgruppen ohne Statusänderung**
Sie können die Erhöhung des Positionsstatus (Auftragsstatus) durch Fertigmeldungen für Produktgruppen unterdrücken. Markieren Sie dazu die gewünschten Einträge in der Liste.

**AV-Bereiche ohne Einlastung**
Sie können festlegen, dass in bestimmte AV-Bereiche nicht automatisch eingelastet wird. Das bedeutet, dass Aufträge für die markierten AV-Bereiche nur manuell eingelastet werden können.

**Automatische Lieferterminsuche nach Tour** Bei Engpässen kann automatisch nach einem neuen Liefertermin gesucht werden.
- Der nächstmögliche Termin wird als Liefertermin gewählt, unabhängig davon, ob es ein Tourentag ist oder nicht. Dies ist die Standard-Einstellung.
- Der neue Liefertermin wird nach den Tourentagen des Kunden gesucht.

**Auftrag nicht splitten** Große Aufträge müssen in kleinere Positionen aufgeteilt werden, wenn der Arbeitsgang nicht für eine Position insgesamt an einem Tag erledigt werden kann.
- Die Aufträge können bei der automatischen Einlastung gesplittet werden. Dies ist die Standard-Einstellung.
- Die Aufträge können nur manuell gesplittet werden. Bei der automatischen Einlastung großer Aufträge wird eine Meldung angezeigt, so dass Sie eingreifen können.

**Verkürzte Einlastprüfung bei gleichem Aufbau** In einem Auftrag können Positionen mit gleichem Stücklistenaufbau enthalten sein, die sich nur durch die Maße unterscheiden.
- Bei jeder Position wird der gesamte Stücklistenaufbau geprüft.
- Bei gleichem Stücklistenaufbau wird von der Einlastung der vorigen Position ausgegangen, ohne die Stückliste neu zu prüfen. Dies ist die Standard-Einstellung.

**Zum Liefertermin einlasten** Bei der automatischen Einlastung werden Aufträge standardmäßig zum Liefertermin eingelastet. Nur wenn keine Kapazitäten frei sind, wird nach einem neuen Liefertermin gesucht.
- Aufträge werden mit Lieferterminsuche eingelastet. Dies ist die Standard-Einstellung.
- Die Aufträge werden ohne Suche nach einem alternativen Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.

**Automatische Fertigmeldung berechneter Aufträge** Zurzeit nicht genutzt.

**Produktionsübergabe (OrderXML) mit Planungsdaten** Für die Übergabe an die Produktion können die ermittelten Daten aus der Kapazitätsplanung in die OrderXML-Datei geschrieben werden.
- Die Daten aus der Kapazitätsplanung werden nicht in die OrderXML-Datei geschrieben.
- Die Maschinenzuordnung, Produktionsdatum und -schicht, Zeitkosten werden in die Übergabedatei geschrieben.

**Schichtwechseltabelle verwenden** Wenn Sie mit mehr als einer Schicht arbeiten, können Sie festlegen, wann die Einlastung von einer Schicht zur nächsten wechselt.
- Die Schichtwechseltabelle wird nicht verwendet.
- Die Schichtwechseltabelle wird verwendet. Wenn noch keine Schichtwechsel festgelegt sind, wird der Dialog Einstellungen Schichten geöffnet.
⇨ "Einstellungen Schichten" auf Seite H-187

### Einstellungen Schichten
**Stammdaten > Firma > Firmendaten > Register Kapa-Planung > Checkbox Schichtwechseltabelle verwenden**

**Abb. H-128: Stammdaten – Einstellungen Schichten**

In diesem Dialog legen Sie die Schichtwechsel und Sperrzeiten fest, in denen z. B. kein Auftrag eingelastet werden kann.

> **Voraussetzungen**
> Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein.
> ⇨ "Schichtwechseltabelle verwenden" auf Seite H-186

#### Allgemein
Die Einstellungen in diesem Bereich werden aus den Firmendaten übernommen.
⇨ "A+W Business-Kapazitätsplanung" auf Seite H-184

**Schichtzahl** Anzahl der Schichten.

**Abgleichmodus** Modus, nach dem nach Aggregaten gesucht wird:
- **0 = Automatisch:** Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **1 = Semi-automatisch:** Das Programm bietet die alternativen Maschinen zur Auswahl an. Wenn der Liefertermin nicht eingehalten werden kann, müssen Sie eingreifen.
- **3 = Manuell:** Mit dieser Einstellung müssen Sie bei jedem möglichen Wechsel (Maschine, Schicht usw.) manuell eingreifen. Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

#### Optionen
**Beim Speichern Zeittabellen korrigieren** Wenn Sie die Werte geändert haben, können die Zeiten der eingelasteten Aufträge überrechnet werden.
- Die neuen Zeiten verändern die aktuell eingelasteten Aufträge nicht.
- Die neuen Zeiten werden sofort übernommen. Alle eingelasteten Aufträge werden neu berechnet.

#### Schichtwechselzeiten
**Schicht 1 > Schicht 2, ...** Angabe, wann der Übergang von einer Schicht zur nächsten Schicht stattfindet. Diese Einstellung ist z. B. wichtig für die Berechnung von Übergangszeiten. Die Anzahl der angezeigten Felder hängt von der Anzahl der Schichten ab, die in den Firmendaten angegeben sind.
⇨ "A+W Business-Kapazitätsplanung" auf Seite H-184

#### Schichtsperrzeiten
**1., 2., ... Schicht** Angabe, ab wann die jeweilige Schicht für neue Aufträge gesperrt ist.

> **Beispiel: 2. Schicht 10:00**
> Bis 10 Uhr können Aufträge in die zweite Schicht des aktuellen Tages eingelastet werden. Damit halten Sie sich die 2. Schicht so frei, dass alle eingelasteten Aufträge tatsächlich gefertigt werden können und keine Restmengen entstehen.
> Aufträge, die nach 10 Uhr eingelastet werden, werden für die 3. Schicht oder den folgenden Tag geplant.

## Allgemein
**Kapazitätsplanung > Stammdaten > Allgemein**

In diesen Dialogen hinterlegen Sie Daten für die Arbeitsgänge und Maschinen, die in der Produktion zur Verfügung stehen.

In diesem Kapitel finden Sie Informationen zu folgenden Stammdaten:
- "Aggregattypen" auf Seite H-189
- "Arbeitsarten" auf Seite H-192
- "Zugeordnete Aggregate" auf Seite H-195
- "Serienfaktoren" auf Seite H-196
- "Übergangszeiten" auf Seite H-197

### Aggregattypen
**Kapazitätsplanung > Stammdaten > Allgemein > Aggregattypen**

**Abb. H-129: Aggregattypen**

In diesem Dialog definieren Sie die Maschinentypen, die Sie in Ihrer Produktion einsetzen, z. B. Schneidtische, Bohrmaschinen, Schleifmaschinen, ESG-Öfen usw. Sie müssen zuerst die Maschinentypen definieren und festlegen, welche Restriktionen jeweils geprüft werden sollen.
Mit einem Klick in den Zeilenkopf öffnen Sie den Dialog Zugeordnete Aggregate.
⇨ "Zugeordnete Aggregate" auf Seite H-195

Durch das Aktivieren der Checkboxen werden die entsprechenden Felder im Dialog Aggregate freigeschaltet.
⇨ "Aggregate" auf Seite H-201

> **Achtung bei nachträglicher Aktivierung**
> Wenn Sie eine Checkbox nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Die neu freigeschalteten Felder sind standardmäßig leer. Das kann bei der Prüfung Fehler verursachen.

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Maschinentypen dient.

**Bezeichnung** Name des Maschinentyps.

#### Einstellungen
Im Folgenden wird jeweils die Funktion der aktivierten Checkbox genannt. Eine ausführliche Beschreibung der Funktion finden Sie im Dialog Aggregate mit der Beschreibung der einzelnen Einstellungen.
⇨ "Aggregate" auf Seite H-201

**Maschinentyp** Die Auswahl des Maschinentyps steht nur in A+W Business Pro zur Verfügung. Für diese Programmversion sind die Maschinentypen fest vorgegeben. Der Maschinentyp bezieht sich auf die konkreten Maschinen und die zu verwendeten Treiber. Die Auswahl legt fest, welche Maschinentreiber im Dialog Aggregate > Zusatz-Optionen zur Verfügung stehen. Mit diesen Treibern kann A+W Business Pro die Maschinen ansteuern. Im Unterschied zum Aggregattypen kann dieser Typ nicht konfiguriert werden.

**Maß-Check** Die Größenrestriktionen müssen bei diesem Maschinentyp geprüft werden.

**SZR** Die SZR-Restriktionen müssen bei diesem Maschinentyp geprüft werden.

**Gesamtstärke** Die Gesamtdicke einer ISO- oder einer VSG-Einheit muss geprüft werden.

**Einzelstärke** Die Dicke eines einzelnen Einfachglases muss geprüft werden.

**Gewicht** Das Gewicht der Scheibe muss geprüft werden.

**Scheibenanzahl** Die Anzahl der Scheiben eines Produkts (2-fach, 3-fach-ISO oder VSG) muss geprüft werden.

**Fläche** Die Fläche der Scheibe muss geprüft werden.

**Gas** Die Position muss auf Gasfüllung überprüft werden.

**Kantenschutz** Der Kantenschutz muss bei Isoliergläsern geprüft werden.

**Modell** Die Position muss auf Modelle geprüft werden.

**Sprossen** Die Position muss auf Sprossen geprüft werden.

**Anzahl** In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.
- Bohrmaschine = Anzahl Bohrlöcher
- Schleifmaschine = Anzahl der Kanten

**Seitenverhältnis** Das Seitenverhältnis der Scheibe muss geprüft werden.

**Drehbar** Bei jedem Glas muss geprüft werden, ob es gedreht werden darf.

**Bohrdurchmesser** Der Durchmesser einer Bohrung muss geprüft werden.

**Eck-Radius** Der Radius von gerundeten Ecken muss geprüft werden.

**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen, muss geprüft werden.

**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten muss geprüft werden.

### Arbeitsarten
**Kapazitätsplanung > Stammdaten > Allgemein > Arbeitsarten**

**Abb. H-130: Arbeitsarten**

In diesem Dialog hinterlegen Sie die Arbeitsarten. Das sind alle Tätigkeiten, für die Zeiten benötigt werden, also z. B. Zuschnitt, manueller Zuschnitt, Kanten säumen, Kanten polieren, VSG sägen, verpacken.
In einem Arbeitsprozess können mehreren Arbeitsarten nacheinander ausgeführt werden, z. B. für die ESG-Fertigung der Zuschnitt und das Härten. Sie müssen also entscheiden, ob Sie die einzelnen Schritte jeweils als eine Arbeitsart anlegen oder den gesamten Arbeitsprozess. Je nach der Organisation in Ihrem Betrieb kann es auch sinnvoll sein, beide Formen zu wählen.
⇨ Tutorial, "Arbeitsarten" auf Seite H-29

> **Arbeitsarten scannen**
> Wenn Sie mit einer Betriebsdatenerfassung (BDE) arbeiten, müssen Sie alle Arbeitsarten anlegen, die mit dem Scanner erfasst werden können. Nur dann können Sie auch die Rückmeldungen für den Status auswerten.

#### Menü Funktionen
Über dieses Menü können Sie sich eine Übersicht über die Maschinen anzeigen lassen, die der markierten Arbeitsart zugeordnet sind.

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Arbeitsarten dient. Wir empfehlen, die Nummern in Zehnersprüngen anzugeben, so dass Platz zum Einfügen neuer Arbeitsarten bleibt. Damit können Sie ähnliche Arbeitsarten zusammenhalten. Außerdem sollten die Arbeitsarten in der Reihenfolge nummeriert sein, in der sie im Fertigungsprozess aufeinander folgen.

**Bezeichnung** Name der Arbeitsart. Als Arbeitsart kann auch ein Zuschlag definiert werden, der die Maschinenzeit z. B. beim Zuschneiden von Modellen verlängert.

**RFOZ** Reihenfolge-Ordnungsziffer. Dieses Feld gibt die Priorität (Produktionsreihenfolge) der einzelnen Arbeitsarten innerhalb der Kapazitätsplanung an.

> **Beispiel**
> Kanten müssen vor dem Lochbohren geschliffen werden.
> VSG-Vorverbund nach dem Bohren.
> Daraus folgt, dass die RFZO für den Kantenschliff kleiner, für den VSG-Vorverbund größer ist als für die Lochbohrung.

Sie sollten bei der Zuordnung der Ziffern mindestens in 10er-Schritten, besser noch in 50er oder 100er-Schritten arbeiten, damit Sie genug Spielraum für neue Arbeitsarten haben.

**Nur Hauptprodukt** Einige Arbeitsarten sind nur beim Hauptprodukt sinnvoll, jedoch nicht für die Stücklistenelemente.
- Diese Arbeitsart kann sowohl beim Hauptprodukt als auch bei den Stücklisten-Komponenten angewendet werden.
- Diese Arbeitsart gilt nur für das Hauptprodukt, z. B. ist der Versand für Stücklisten-Komponenten nicht möglich.

**Masch. Nr.** Artikelnummer aus A+W Production. Arbeitsarten, die Bestandteil eines Auftrages bei einem Glasproduzenten sind, jedoch im Auftrag selbst nicht extra spezifiziert werden, benötigen eine A+W Production-Artikelnummer, z. B. Zuschnitt. Für diese Artikelnummer muss in A+W Business Pro ein Produkt der Produktart/Produktgruppe Bearbeitungen mit derselben Nummer angelegt werden.

**% Limit** Die Kapazitätsplanung lastet standardmäßig einen Auftrag so ein, dass dieser zeitnah zum Liefertermin gefertigt wird. Bei großen Aufträgen kann dies zu Problemen führen. Der Prozentwert legt fest, wie groß der Anteil eines Auftrags an der Tageskapazität sein darf. Größere Aufträge werden dann über mehrere Tage verteilt.

> **Beispiel**
> Sie erhalten einen großen Auftrag am 17. Juli. Der Liefertermin ist der 22. September.
> Die Kapazitätsplanung würde diesen Auftrag so einplanen, dass er kurz vor Liefertermin gefertigt würde. Damit wäre aber die Produktion für z. B. vier komplette Tage durch diesen Auftrag blockiert. Andere Aufträge könnten in dieser Zeit nicht mehr eingelastet werden.
> Da Sie aber Zeit haben, den Auftrag verteilt über den gesamten Zeitraum bis zum Liefertermin zu fertigen, können Sie hier eintragen, dass die Arbeitsart pro Auftragsposition nur z. B. 10 % der Tageskapazität beanspruchen darf.

Dieser Wert wird nur berücksichtig, wenn Sie die Option Pos. Control aktivieren. Diese Option finden Sie in folgenden Dialogen:
⇨ "Einlasten NV" auf Seite H-278
⇨ "Einlasten Auftrag" auf Seite H-284
⇨ "Aggregate Ausfall" auf Seite H-297

**Manuelle Aggregatauswahl** Wenn Sie mehrere Maschinen haben, die die gleiche Arbeitsart ausführen können, legen Sie eine Maschine mit Priorität 9 in den Vorgabezeiten fest, damit sie standardmäßig ausgewählt wird. Wenn diese Maschine an einem Tag ausgelastet ist, kann auf eine der anderen Maschinen zugegriffen werden.
- Der Auftrag wird automatisch einer anderen Maschine zugeordnet. Wenn dabei jedoch der Produktionstag gewechselt wird, müssen Sie manuell eingreifen.
- Wenn die Kapazität einer Maschine überschritten wird, müssen Sie manuell eine andere Maschine auswählen. Die möglichen Ausweichmaschinen werden in einem Dialog angezeigt.

**Ausweich-Arbeitsart** Sie können einer Arbeitsart eine Ausweich-Arbeitsart zuordnen, z. B. für das Bohren von Sondergrößen.

> **Beispiel**
> Sie haben die beiden Arbeitsarten Bohren und Sondergrößen bohren.
> In der Arbeitsart Bohren wird die Ausweicharbeitsart Sondergrößen bohren eingetragen.
> Der Standard-Bohrmaschine wird die Arbeitsart Bohren zugewiesen. Diese kann jedoch nur beschränkte Bohrdurchmesser bohren. Wenn diese Abmessungen überschritten werden, dann prüft die Kapazitätsplanung, ob eine Ausweich-Arbeitsart eingetragen ist. Wenn ja, sucht das Programm nach einer zugeordneten Maschine.

### Zugeordnete Aggregate
**Kapazitätsplanung > Stammdaten > Allgemein > Arbeitsarten > Menü Funktionen > Zugeordnete Aggregate**

**Abb. H-131: Zugeordnete Aggregate**

In diesem Dialog werden die Maschinen aufgelistet, die einem Aggregattyp oder einer Arbeitsart zugeordnet sind. Im Infobereich des Dialogs wird angezeigt, aus welchem Dialog heraus Sie die Übersicht geöffnet haben.

**Aggregat** Name der Maschine, die zugeordnet ist.

**Bemerkung** In dieser Spalte wird bei Arbeitsarten angezeigt, ob die Arbeitsart für die zugeordnete Maschine als Basiszeit oder als Zeitzuschlag ausgewertet wird.

**Prio** Priorität, mit der das Aggregat beim Einlasten automatisch ausgewählt wird.
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Priorität. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Prioritäten. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt. Die Maschine kann nur manuell ausgewählt werden.
- **-3:** wird nur bei der Rückmeldung vom Produktionssystem ausgewählt, wenn dort umgelastet wurde. Bei Umlasten in der Kapazitätsplanung werden nur noch Aggregate mit Prio > -3 angezeigt.

### Serienfaktoren
**Kapazitätsplanung > Stammdaten > Allgemein > Serienfaktoren**

**Abb. H-132: Serienfaktoren**

In diesem Dialog legen Sie fest, bei welchen Stückzahlen die geplanten Zeiten reduziert werden, z. B., weil das Rüsten beim Schleifen oder Bohren entfällt.
Die Nummer der Serientabelle ordnen Sie der Maschine im Dialog Aggregate zu.
⇨ "Serientabelle" auf Seite H-206

#### Identifikation
**Nummer** Die Nummer wird automatisch vergeben, wenn Sie eine neue Serientabelle anlegen.

**Bezeichnung** Name der Serientabelle. Geben Sie einen sprechenden Namen ein, wenn Sie mehrere Tabellen anlegen, z. B. für Bohren oder Schleifen.

#### Serientabellen
**Ab Stück** Menge, ab der ein Faktor berücksichtigt werden soll.

**Faktor** Faktor, mit dem die Basiszeit für den Arbeitsgang multipliziert wird.

> **Beispiel**
> 
> | Ab Stück | Faktor pro Stück | Zeit an der Maschine |
| :--- | :--- | :--- |
| 1 | 1 | 0,10 Std. |
| 10 | 0,9 | 10 x 0,9 x 0,1 = 0,90 Std. |
| 50 | 0,7 | 50 x 0,7 x 0,1 = 3,50 Std. |

#### Tabelle
In der Übersicht sind alle Serientabellen aufgeführt, die Sie eingerichtet haben.

### Übergangszeiten
**Kapazitätsplanung > Stammdaten > Allgemein > Übergangszeiten**

**Abb. H-133: Übergangszeiten**

In diesem Dialog geben Sie die Zeit in Schichten ein, die benötigt wird, um von einer Arbeitsart zum anderen zu wechseln. Zum Beispiel müssen nach dem ESG-Ofen die Scheiben erst abkühlen, bevor die nächste Arbeitsart beginnen kann.
⇨ Tutorial, “Übergangsmatrix und Übergangszeiten" auf Seite H-69

> **Übergangszeiten bearbeiten**
> Die Komboboxen in den Tabellenfeldern sind nur freigeschaltet, wenn Sie eine neue Übergangzeit festlegen. Sie können die zugeordneten Arbeitsarten einer Übergangszeit nach dem Speichern nicht ändern. Wenn Sie eine Zuordnung ändern wollen, müssen Sie sie neu anlegen und anschließend die ungültige Zuordnung löschen.

**Auftragspriorität** Auftragspriorität, bei der die Übergangzeit berücksichtigt werden soll. Sie können zwischen folgenden Prioritäten wählen:
- **Normal:** Die Übergangzeit gilt für alle Aufträge, in denen keine besondere Priorität angegeben ist. Dies ist die Standard-Einstellung.
- **Eilt:** Die angegebene Übergangzeit gilt für Eilaufträge. Wenn Übergangszeiten für Eilaufträge verkürzt werden können, dann muss für die entsprechende Kombination von Arbeitsarten eine abweichende Übergangszeit hinterlegt werden.
- **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
- **Abruf:** Die Übergangzeit gilt nur für Aufträge, die auf Abruf gefertigt werden.

> **Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann muss für die jeweilige Kombination von Arbeitsarten eine eigene Übergangszeit eingerichtet sein. Dies gilt für alle Übergangszeiten, die für Eilaufträge auch verkürzt werden können.

**Von Arbeitsart** Ausgangs-Arbeitsart, z. B. Polieren.

**Nach Arbeitsart** Folge-Arbeitsart, z. B. Bohren. Wenn Sie <k.A.> auswählen, gilt die Übergangzeit für alle Folge-Arbeitsarten.

**Zeit in Schichten** In diesem Feld tragen Sie die Anzahl der Schichten ein, die für den Wechsel von einer Arbeitsart zur anderen benötigt werden:
- **0** = Der Folgevorgang kann in der gleichen Schicht stattfinden.
- **1** = Der Folgevorgang findet frühestens in der nächsten Schicht statt.
- **2** = Der Folgevorgang findet frühestens in der übernächsten Schicht statt.

> **Beispiel**
> Sie arbeiten in Ihrem Betrieb regulär in 3 Schichten, im Heat-Soak-Test z. B. jedoch in nur einer Schicht à 12 Stunden.
> Wenn Sie erreichen möchten, dass die Folge-Arbeitsart generell erst am nächsten Tag beginnt, dann müssen Sie in diesem Feld den Wert 3 eintragen. Damit berechnet die Kapazitätsplanung den Termin für die Folge-Arbeitsart automatisch für den nächsten Tag.

**Inkl. arbeitsfreie Tage** Bei der Berechnung können die arbeitsfreien Tage berücksichtigt werden.
- Arbeitsfreie Tage werden nicht berücksichtigt.
- Arbeitsfreien Tage werden berücksichtigt. Das bedeutet, dass ein ESG, das am Freitag aus dem Ofen kommt, ganz regulär am Montag weiter verarbeitet werden kann, da das Wochenende schon länger ist als die Übergangzeit.

---

## Organisation
**Kapazitätsplanung > Stammdaten > Organisation**

In diesen Dialogen legen Sie fest, wie die Kapazitätsplanung organisiert ist, z. B. die Produktionsbereiche, Maschinen, Schichtzeiten.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktionsbereich" auf Seite H-200
- "Aggregate" auf Seite H-201
- "Kalender" auf Seite H-211
- "Übergangsmatrix” auf Seite H-216
- "Besondere technische Restriktionen" auf Seite H-219
- "Orga Übersicht" auf Seite H-222

### Produktionsbereich
**Kapazitätsplanung > Stammdaten > Organisation > Produktionsbereich**

**Abb. H-134: Produktionsbereiche**

In diesem Dialog definieren Sie die Produktionsbereiche, z. B. Zuschnitt, Schleiferei, Bohren. Gleichzeitig legen Sie fest, welcher Status vom jeweiligen Produktionsbereich gemeldet wird, wenn die Position fertig gemeldet wurde.
⇨ Tutorial, "Produktionsbereiche (Arbeitszentren)" auf Seite H-31

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Produktionsbereiche dient. Die Nummerierung stellt keine Hierarchie dar.

> **Der Produktionsbereich <k.A.>**
> Der Produktionsbereich Nr. 0 (Null) mit der Beschreibung <k.A.> muss einmal als Standard-Produktionsbereich definiert werden. Nachdem dieser Eintrag gespeichert wurde, wird er in diesem Dialog nicht mehr angezeigt. Prüfen Sie, ob dieser Eintrag besteht, indem Sie ihn neu anlegen. Eine Fehlermeldung zeigt an, wenn dieser Datensatz schon angelegt ist.

**Produktionsbereich** Name des Produktionsbereiches.

**Max. Einheit/Std** Angabe, wie viele Einheiten (Stück) im Produktionsbereich pro Stunde höchstens gearbeitet werden können.
Wenn Sie z. B. 6 Schleifmaschinen haben, aber nur drei Werker, die an diesen Maschinen arbeiten können, können Sie die Gesamtkapazität nur für drei Maschinen berechnen.
