---
title: "DE_AWProduction_Kapazitaetsplanung_4_3"
source: "DE_AWProduction_Kapazitaetsplanung_4_3.pdf"
tags: ["A+W Production", "Kapazitätsplanung", "Stammdaten", "Übergangszeiten", "Vorgabezeiten", "Maschinengruppen", "Lastverteilung", "Software-Tutorial", "Produktionsplanung", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial for setting up master data for capacity planning in the A+W Production software. It covers defining transition times, processing times (Vorgabezeiten), machine groups, and load distribution to accurately model the production environment."
long_description: "This document is a comprehensive tutorial from the A+W Production software suite, specifically focusing on the 'Stammdaten der Kapazitätsplanung' (Master Data for Capacity Planning). It guides users through the necessary steps to configure the foundational data required for effective production planning and scheduling. The tutorial is divided into several key sections. It begins with 'Übergangszeiten' (Transition Times), explaining how to define the time it takes for a product to move between different logical machines. Next, it covers 'Vorgabezeiten' (Processing Times), detailing how to create complex formulas (Vorgabezeitformeln) to calculate the duration of work steps based on various factors like glass thickness, area, or model type. The document also explains how to manage 'Maschinengruppen' (Machine Groups) to bundle similar machines and control their collective capacity. Finally, it addresses 'Lastverteilung' (Load Distribution), showing how to allocate capacity shares for specific tasks on a single physical machine. The tutorial includes step-by-step instructions, screenshots, and practical examples to help users correctly set up their production environment for accurate capacity planning. It also contains a software reference section for more detailed dialog descriptions."
---

# Tutorial: Stammdaten der Kapazitätsplanung

---
## Vorbereitung der Definition von Übergangszeiten

Um die Übergangszeiten für Ihre Produktion zu ermitteln, können Sie zunächst eine Matrix erstellen. Die Matrix hilft, die Übergangszeiten zwischen den logischen Maschinen zu visualisieren.

Unterscheiden Sie zwischen der Zeit beim Weggang und der Zeit bei Ankunft:
*   Der Weggang nach dem Arbeitsprozess kann z. B. bedeuten, dass eine Scheibe nach einer Bearbeitung darauf wartet umgepackt zu werden.
*   Die Ankunft am Eingang kann sich z. B. auf Vorarbeiten beziehen.

**Abb. E-54 Beispiel-Matrix für Übergangszeiten**

| von / nach | Säumen | Bieger | Heat Soak | VSG | ISO Sprossenbau | ISO Linie | Bohren |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Wareneingang** | 4 | | | 4 | 4 | 4 | 4 |
| **Zuschnitt** | | 4 | | | 4 | | |
| **Säumen** | 0 | 0 | 0 | | | | 0 |
| **Bieger** | | | 4 | | | | |
| **Heat Soak** | 8 | 8 | | | | | |
| **VSG** | 8 | 8 | | | | | |
| **Bohren** | | | 4 | | | | |
| **ISO Sprossenbau** | | | | | 4 | | |
| **ISO Linie** | | | | | 0 | | |

> **Legende:**
> *   **Zahl:** Übergangszeit in Stunden
> *   **Grün:** Übergangszeit bei Weggang
> *   **Rot:** Übergangszeit bei Ankunft

In diesem Beispiel sehen Sie, dass z. B. das Glas im Heat Soak immer acht Stunden verweilt. Daher beträgt die Übergangszeit vom Heat Soak zu allen anderen Arbeitsstationen immer 16 Stunden. Die so ermittelten Zeiten Ihrer Produktion rechnen Sie in Schichten um.

Eine solche Matrix zeigt, dass Sie nur wenige Übergangszeiten zwischen den Arbeitsstationen definieren müssen. Alle anderen können Sie mit der Einstellung Von allen Maschinen -> Maschine X oder Von Maschine X -> alle anderen Maschinen definieren.

Die Erstellung der Matrix und das Umsetzen im Dialog führen Sie am besten gemeinsam mit dem Service der A+W Software GmbH durch.

## Übergangszeiten anlegen und verwalten

In dieser Lerneinheit lernen Sie, wie Sie Übergangszeiten anlegen, bearbeiten oder löschen. Denken Sie daran, dass in den Übergangszeiten auch Rüstzeiten und Handlingszeiten berücksichtigt werden müssen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine Übergangszeit an" auf Seite E-102
*   "So bearbeiten Sie eine Übergangszeit" auf Seite E-104
*   "So löschen Sie eine Übergangszeit" auf Seite E-104

> **i Voraussetzung**
> Um Übergangszeiten anzulegen, müssen die entsprechenden logischen Maschinen in der Maschinenzuordnung definiert sein.

### So legen Sie eine Übergangszeit an
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Übergangszeiten.
2.  Klicken Sie auf [Neu].

**Abb. E-55 Übergangszeiten einrichten**
*Die Abbildung zeigt den Dialog "Übergangszeiten", in dem Übergangszeiten zwischen Maschinen definiert werden.*
*   **A** Neue Zeile
*   **B** Maschine, von der das Teil ausgeht
*   **C** Maschine, zu der das Teil kommt
*   **D** Typ der Übergangszeit
*   **E** Normale Übergangszeit in Stunden oder Schichten
*   **F** Maximale Übergangszeit in Stunden oder Schichten

3.  In der Liste der Maschinen wird oben eine neue Zeile eingefügt. Klicken Sie doppelt in das Feld (B), um den Dialog zur Auswahl der Maschine zu öffnen.
4.  Übernehmen Sie die gewünschte Maschine mit einem Doppelklick.
5.  Wiederholen Sie den Schritt für die Maschine (C), zu der Sie den Übergang festlegen.
    Nutzen Sie auch die Möglichkeiten Alle Maschinen auf Maschine X und Maschine X auf Alle Maschinen.
6.  Wählen Sie den Typ (D) für die Übergangszeit aus und tragen Sie die zugehörige Zeit (E) ein.
    Verwenden Sie bevorzugt Schichten. In Ausnahmefällen können Sie auch Zeitdauern verwenden, z. B. Trockungszeiten.
7.  Tragen Sie die maximale Übergangszeit (F) ein.
    Damit erlauben Sie dem System, die Übergangszeit maximal zu dehnen. Verwenden Sie auch hier entweder Stunden oder Schichten.

> **Tipp**
> Wählen Sie für den Übergang zur letzten Bearbeitung, z. B. Verpacken oder Versand, die größte Übergangszeit, die möglich ist. Damit haben Sie in kritischen Situationen größere Flexibilität.

8.  Wiederholen Sie die Schritte 2 bis 7 für den nächsten Übergangstyp (D) derselben Maschinenkombination.
9.  Klicken Sie auf [OK], um die Daten zu speichern.
    Damit haben Sie die Übergangszeiten in den verschiedenen Übergangstypen für einen Übergang angelegt.

### So bearbeiten Sie eine Übergangszeit
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Übergangszeiten.
2.  Korrigieren Sie die Übergangszeiten für die gewünschten Maschinen. Sie aktivieren die Felder mit einem Doppelklick.
3.  Ergänzen Sie ggf. eine Maschinenkombination, indem Sie die Daten für einen anderen Übergangstyp anlegen. Folgen Sie dazu der Beschreibung in der Handlungssequenz zum Anlegen der Übergangszeiten.
4.  Klicken Sie auf [OK], um die Änderungen zu speichern. Damit haben Sie die Übergangszeiten geändert.

### So löschen Sie eine Übergangszeit
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Übergangszeiten.
2.  Markieren Sie in der ersten Spalte die Übergangszeit, die Sie löschen wollen. Die gesamte Zeile der Übergangszeit wird markiert.

**Abb. E-56 Übergangszeiten löschen**
*Die Abbildung zeigt eine markierte Zeile im Dialog "Übergangszeiten", bereit zum Löschen.*

3.  Klicken Sie auf [Löschen].
    Die Übergangszeit wird aus der Liste gelöscht.
    Falls Sie eine Übergangszeit versehentlich aus der Liste gelöscht haben, klicken Sie auf [Ende].
    Wenn Sie die Meldung mit [Nein] bestätigen, wird der Dialog geschlossen, ohne die Änderung zu speichern. Die Übergangszeit steht wieder in der Liste, wenn Sie den Dialog erneut öffnen.
4.  Klicken Sie auf [OK], um den Dialog zu schließen.
    Die Änderungen werden in die Datenbank übernommen.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Legen Sie gemeinsam mit dem Trainer eine neue Maschine in der Maschinenzuordnung vollständig an, die Sie deutlich als Test-Maschine für die Kapazitätsplanung kennzeichnen.
*   Definieren Sie die Übergangszeiten für diese Maschine im Eil- und Normalraster.
*   Legen Sie Übergangszeiten zwischen zwei Maschinen für alle Typen von Übergangszeiten an, die für die Übergänge erforderlich sind.
*   Verändern Sie die Übergangszeiten.
*   Prüfen Sie die Ergebnisse mit einem Testauftrag im Produktionsmonitor.

### Ergänzende Informationen
⇨ Softwarereferenz, "Übergangszeiten" auf Seite E-227

## Vorgabezeiten

### Lernziele
*   Was sind Vorgabezeiten?
*   Wie werden Vorgabezeiten angelegt, bearbeitet oder gelöscht?
*   Aus welchen Elementen bestehen Vorgabezeiten?
*   Wie fließen die Elemente in Vorgabezeiten ein?
*   Wie funktioniert der Formeltest?

### Nutzen
*   Mit Vorgabezeiten definieren Sie, wie lange ein Arbeitsschritt auf einer Maschine für eine Scheibe dauert. Zusammen mit den Übergangszeiten werden damit die Zeiten durch die Produktionsstationen berechnet.

### Merke
*   **Vorgabezeit = Bearbeitungsdauer**: Mit der Vorgabezeit legen Sie fest, wie lange ein Arbeitsgang auf einer spezifischen Maschine dauert. Die Bearbeitungsdauer wird anhand von Formeln berechnet. Vorgabezeiten werden in der Maschinenzuordnung (MZO) als Bearbeitungsdauer bezeichnet.
*   **Logische Maschinen**: Vorgabezeiten werden zu den logischen Maschinen erstellt.
*   **Vorgabezeiten**: Die Vorgabezeiten werden zur Kapazitätsplanung und zur Kostenkalkulation herangezogen.
*   **Formel**: Vorgabezeiten können mit Formeln berechnet werden, um verschiedene Einflussgrößen zu berücksichtigen, z. B. Fläche, Laufmeter, Stückzahl, Dicke. Komplexe Vorgabezeiten hinterlegen Sie als Formel in der Maschinenzuordnung.
*   **Element**: Eine Zeile in einer Vorgabezeitformel, z. B. eine Dickenabhängigkeit, der Zeitanteil für die Fertigung eines Ausschnitts an einem Bearbeitungszentrum oder ein Zeitzuschlag für schwere Scheiben. Elemente können separat erfasst und getestet werden. Es gibt feste Elemente, bedingte Ausdrücke, Schwellenwerte, gewichtete Ausdrücke (freie Elemente) und Vektoren. Als benutzerdefinierte Elemente lassen sich zusätzlich Tabellen und dreidimensionale Abhängigkeiten (Würfel) verarbeiten.

## Definition der Vorgabezeiten

Mit einer Vorgabezeit definieren Sie, wie die Dauer eines Arbeitsgangs an einer logischen Maschine berechnet wird. Basis der Berechnung ist dabei z. B. die jeweilige Fläche oder Kantenlänge in der einzelnen Auftragsposition.

**Abb. E-57 Vorgabezeiten**
*Die Abbildung zeigt den Dialog "Vorgabezeiten", der eine Liste logischer Maschinen und die zugehörigen Vorgabezeitformeln anzeigt.*

In diesem Dialog sind die logischen Maschinen aufgelistet, über die Bearbeitungen gesteuert werden. Vorgabezeiten werden in A+W Production mit Vorgabezeitformeln festgelegt. Die Vorgabezeitformeln definieren Sie im Dialog Vorgabezeitformel.

> **i Vorgabezeiten**
> Die Vorgabezeiten werden in der Maschinenzuordnung (MZO) als Bearbeitungsdauer bezeichnet. Da die Vorgabezeiten an den logischen Maschinen festgemacht werden, können Sie auch in der Maschinenordnung Formeln für Vorgabezeiten hinterlegen. Sie tun dies im MZO-Editor > Register Logische Maschine > Feld Bearbeitungsdauer.
> Diese Formeln aus der MZO können nicht im Dialog Vorgabezeiten geändert werden.

## Struktur von Vorgabezeitformeln

Jede Vorgabezeitformel basiert auf einer Basiszeit, die in Sekunden angegeben ist. Vorgabezeitformeln können mit vorgegebenen Elementen definiert werden. Daneben können Sie auch eigene Elemente erstellen und in der Formel verwenden.

**Abb. E-58 Vorgabezeitformel**
*Die Abbildung zeigt den Dialog "Vorgabezeitformel" zur Definition der Berechnungslogik.*
*   **A** Elemente der Vorgabezeitformel
*   **B** Basiszeit in Sekunden
*   **C** Auswahl der Rechenoperation
*   **D** Reihenfolge der Elemente sortieren
*   **E** Multiplikator für die Bearbeitungsmenge

Mit jeder Zeile ist ein Zeitzuschlag angegeben, der entweder als Formel berechnet oder als Wert aus einer Tabelle ermittelt wird.

Sie können in einer Vorgabezeitformel mehrere unterschiedliche Elemente (A) verwenden. Dazu wählen Sie jeweils das gewünschte Element aus, geben einen Wert in Sekunden an und legen fest, wie der Wert in der Rechenoperation verwendet werden soll (C). Wichtig ist dabei, dass die Reihenfolge (D) korrekt sortiert ist. Das gilt insbesondere dann, wenn die nächste Rechenoperation auf dem Zwischenergebnis der vorausgegangenen Operation aufbaut.

Die Basiszeit gilt dabei als Startwert. Alle weiteren Elemente der Formel sind daher Zuschläge auf den Startwert. Wenn Sie keine Basiszeit eintragen, bauen alle Berechnungen auf dem Ergebnis des ersten Eintrags (A) auf.

Standardmäßig werden verschiedene Element zur Auswahl angeboten, die auch durch eigene Definitionen ergänzt werden können:
⇨ "Editor für Formelelemente" auf Seite E-113

### Beispiel Gas und Modell
| Element | Wert |
| :--- | :--- |
| Basiszeit | 23 s |
| Faktor für Größe | 23 * Größenfaktor |
| Faktor für Gas | Zwischenergebnis * Gasfaktor |
| Konstante für Modell | Zwischenergebnis + Modellkonstante |

Mit dieser Vorgabezeitformel können Sie Zeiten für Scheiben mit Gasfüllung und für Modelle berechnen. Wenn Sie aber VSG berechnen wollen, muss die Formel folgendermaßen aufgebaut werden:

### Beispiel VSG, Größe und Gas
| Element | Wert |
| :--- | :--- |
| Basiszeit | 23 s |
| Faktor VSG | + VSG-Faktor |
| Faktor für Größe | Zwischenergebnis 1 * Größenfaktor |
| Faktor für Gas | Zwischenergebnis 2 + (23 * Gasfaktor) |

### Feste Elemente
Festen Elementen wird kein Wert zugewiesen, sondern lediglich angegeben, wie sich die Elemente auf die Vorgabezeitformel auswirken. Zur Berechnung werden die tatsächlichen Werte des Glases herangezogen. So wird z. B. für das Feste Element 'Dicke' bei einer 4.00 mm dicken Scheibe der Wert 4 ermittelt. Bei dem Festen Element 'Menge' wird die Anzahl der Scheiben und bei einem Festen Element 'Fläche' wird die Fläche der Scheiben ermittelt.

Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitformeln an, wie der ermittelte Wert in der Vorgabezeitformel verwendet wird.

### Faktoren
Mit einem Faktor können Sie einen Zeitzuschlag festlegen, der immer dann berechnet wird, wenn die Voraussetzung für die Anwendung des Faktors erfüllt ist.

> **Beispiel**
> Mit dem Faktor Wert für 'Große Scheibe' legen Sie einen Zuschlag auf die Basiszeit fest, der immer für Übergrößen berechnet wird. Ab wann eine Scheibe als Übergröße gilt, geben Sie zu dem Faktor an.

Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitformeln an, wie der ermittelte Wert in der Vorgabezeitformel verwendet wird.

### Vektoren - Tabellen und Würfel

Vektoren ermöglichen eine exakte Planung der Vorgabezeiten in Abhängigkeit von den Werkstückeigenschaften. Mit Vektoren können Sie die Vorgabezeit z. B. auf die Glasdicke, die zu bearbeitende Fläche, die Beschaffenheit der Kanten und das Verhältnis von Breite zu Höhe einer Scheibe abstimmen.

**Abb. E-59 Vektor 'Dicke -> Wert' - Zeitzuschläge abhängig von der Scheibendicke**

| Dicke | Wert |
| :--- | :--- |
| 4.00 mm | 1 |
| 6.00 mm | 1.2 |
| 8.00 mm | 1.4 |
| 10.00 mm | 1.6 |
| 12.00 mm | 1.8 |
| 16.00 mm | 2 |

Unterschiedliche Dicken von Scheiben berücksichtigen Sie z. B. mit dem Vektor 'Dicke → Wert'. Damit legen Sie Zeitzuschläge abhängig von der Dicke einer Scheibe fest.

Wenn Sie den Wert im Vektor 'Dicke → Wert' als Tabelle festlegen, können Sie den Wert des Vektors staffeln, z. B. von 4.00 mm - 5.99 mm Dicke gilt der Wert 0.1, für 6.00 mm - 7.99 mm der Wert 0.2 usw.

Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitformeln an, wie Vektoren in der Vorgabezeitformel verwendet werden.

### Eingabehilfe für Vektoren
Vektoren werden im Dialog Vektor (Name) als Tabelle definiert. Diese Tabelle enthält pro Grenzwert (Staffelstufe) einen Zuschlagswert. Zum Anlegen einer solchen Tabelle stehen zwei Vorgehensweisen zur Verfügung:
*   Sie geben die Werte einzeln in die Tabelle ein. Dabei legen Sie z. B. mehrere Stufen von Dicken, Längen oder Gewichten fest und weisen diesen jeweils einen Wert zu.
*   Sie lassen sich die Staffelstufen und die gestaffelten Werte berechnen.

**Abb. E-60 Eingabehilfe für Vektoren – Resultat**
*Die Abbildung zeigt den Dialog "Eingabehilfe für Vektoren" und die resultierende Tabelle, die automatisch generiert wurde.*

| Dicke | Wert |
| :--- | :--- |
| 4.00 mm | 0.1 |
| 6.00 mm | 0.2 |
| 8.00 mm | 0.3 |
| 10.00 mm | 0.4 |
| 12.00 mm | 0.5 |
| 14.00 mm | 0.6 |
| 16.00 mm | 0.7 |
| 18.00 mm | 0.8 |
| 20.00 mm | 0.9 |

Für diese Berechnung legen Sie einen Anfangs- und einen Endwert fest, z. B. 4.00 - 20.00 mm für die Dicke. Wenn Sie als Schrittgröße 2.00 mm angeben, wird zwischen dem Anfangs- und dem Endwert alle 2.00 mm eine Stufe eingefügt.

Wenn Sie als Startwert für den Zuschlag 0.1 und als Schrittgröße 0.1 angeben, gilt für die erste Stufe der Wert 0.1, für alle weiteren Stufen wird dieser Wert jeweils um 0.1 erhöht.

Für die Tabelle ergibt sich daraus: Scheiben mit einer Dicke von 4,00 - 5,99 mm haben den Wert 0.1, von 6.00 mm - 8.00 mm den Wert 0.2 usw.

### Berechnung von Zeitzuschlägen
Im einfachsten Fall besteht eine Vorgabezeitformel lediglich aus einer Basiszeit. Sie können z. B. für eine logische Maschine eine Basiszeit von 30 Sekunden angeben. Damit ist festgelegt, dass jeder beliebige Arbeitsgang an dieser logischen Maschine 30 Sekunden dauert.

In der Praxis ist die Dauer eines Arbeitsgangs jedoch von verschiedenen Einflüssen abhängig, z. B. von der Dicke einer Scheibe oder von der Kantenlänge, die bearbeitet werden muss. Je dicker eine Scheibe und je länger die zu bearbeitende Kantenlänge, desto mehr Zeit nimmt ein Arbeitsgang in Anspruch.

Um diese Abhängigkeiten zu berücksichtigen, können Sie Zeitaufschläge festlegen. In der Vorgabezeitformel stehen dazu feste Elemente und/oder Vektoren zur Verfügung.

Für die Vorgabezeitformel stehen folgende Elemente zur Wahl:
*   Basiszeit oder Startwert.
*   Zeitzuschlag als festes Element, z. B. die Glasdicke.
*   Zeitzuschlag als fester Wert, z. B. für große Scheiben.
*   Zeitzuschlag als Vektor, z. B. Staffelung nach Gewicht.
*   Zeitzuschlag als Tabelle für Matrix, z. B. Kantenlänge.

Basiszeit und Zeitzuschläge werden in Sekunden angegeben.

### Reihenfolge der Berechnungen
Bei der Berechnung müssen Sie die Operatorrangfolge der Mathematik berücksichtigen: Multiplikation und Division werden vor Addition und Subtraktion gerechnet - es sei denn, Klammern geben die Reihenfolge vor.

**Beispiel**
| Formel | Ergebnis | Regel |
| :--- | :--- | :--- |
| 1 + 2 * 4 | = 9 | Multiplikation zuerst |
| (1 + 2) * 4 | = 12 | Klammer zuerst |
| 1 + (2 * 4) | = 9 | |
| 4 * (1 + 2) | = 12 | |
| 6 + (9 / 3) | = 9 | |
| (6 + 9) / 3 | = 5 | |

Zur Berechnung der Zeitzuschläge stehen folgende Einstellungen zur Wahl:

**Tab. E-1 Mögliche Einstellungen für die Vorgabezeitformel**
| Einstellung | Bedeutung |
| :--- | :--- |
| `+ Tabelle` | Der Wert aus der Tabelle wird zum Zwischenergebnis addiert. |
| `+ b * Wert` | Die Basiszeit wird mit dem Wert multipliziert. Das Ergebnis der Multiplikation wird zum Zwischenergebnis addiert. |
| `+ Wert` | Der Wert wird zum Zwischenergebnis addiert. |
| `* (1 + Wert)` | Der Wert wird zu 1 addiert und das Ergebnis mit dem Zwischenergebnis aus der vorausgehenden Zeile multipliziert. |
| `* Vektor` | Das Ergebnis der vorausgehenden Zeile wird mit dem Wert des Vektors multipliziert. |

Wenn die Berechnung mit der Ermittlung aus einer Formel beginnt, legen Sie als Startwert 0 fest, z. B. für die Berechnung einer Fläche, bevor der erste Siebdruck aufgetragen wird.

Wenn die Berechnung auf dem Ergebnis der vorausgehenden Zeile basiert, ist die Reihenfolge der Einträge wichtig.

## Editor für Formelelemente
Für die Definition eigener Formelelemente steht ein Editor zur Verfügung, in dem Sie eigene Formeln anlegen oder eine vordefinierte Formel auswählen können.

**Abb. E-61 Zeitformelelement erfassen**
*Die Abbildung zeigt den Editor zum Erfassen oder Ändern eines Formelelements.*
*   **A** Name des Formelelements
*   **B** Auswahl des Typs
*   **C** Beschriftung
*   **D** Berechnungsformel
*   **E** Eingabeformat
*   **F** Unabhängiger Parameter

Dem Formelelement geben Sie einen Namen (A), der in der Auswahl der Formelelemente angezeigt wird, und eine Beschriftung (C), die im Dialog Vorgabezeitformel angezeigt wird. Die zweite Beschriftung wird vor dem Berechnungswert angezeigt.

Die unterschiedlichen Elementtypen (B) verwenden Sie für folgende Berechnungen:
*   **Festes Element**: Ausdrücke ohne Benutzereingabe, z. B. Langkante. Diese Einstellung sollten Sie nicht mehr für neue Definitionen verwenden. Sie ist durch Freies Element abgelöst worden.
*   **Bedingung**: Ausdrücke mit einer Benutzereingabe, die verwendet wird, wenn die Bedingung wahr ist.
*   **Freies Element**: Ausdrücke, bei denen das Ergebnis mit der Benutzereingabe gewichtet wird, z. B. Sekunden pro Schleifmeter.
*   **Schwellenwert**: Ausdrücke, bei denen der Schwellenwert für die Bedingung einstellbar ist, ohne die Formeldefinition zu verändern, z. B. Mengenzuschlag ab Benutzereingabe.
*   **Vektor**: Ausdrücke, bei denen eine Tabelle mit Wertepaaren aus Mindestwerten und zu verwendenden Koeffizienten gepflegt wird.

Die eigentliche Formeldefinition (D) des Elements können Sie als Formel schreiben oder eine vordefinierte Formel auswählen und anpassen. Bei Vektoren können Sie die Definition nicht ändern, daher ist das Feld ausgeblendet.

### Beispiel – Vorgabezeit für die logische Maschine Zuschnitt
Aus einer Produktionsstatistik haben Sie die Flächenabhängigkeit Ihres Zuschnitts ermittelt. Außerdem wissen Sie, dass die Rundbogenmodelle im Schnitt 20 Sekunden länger dauern und der Tisch 10% mehr Zeit fürs Randentschichten von ISO-Komponenten benötigt.
Um schnell auf Produktionsveränderungen reagieren zu können, wollen Sie die komplette Vorgabezeitformel mit einem Steuerparameter auf schneller oder langsamer einstellen können.

**Abb. E-62 Beispiel - Vorgabezeitformel**
*Die Abbildung zeigt ein Beispiel einer konfigurierten Vorgabezeitformel für die Maschine "Cutting Table 1".*

**Tab. E-2 Beispiel - Bedingungen der Berechnung**

| Zeile | Definition | Erklärung |
| :--- | :--- | :--- |
| **Basiszeit** | 0.95 | Der Steuerparameter steht auf 95% der Vorgabezeit, also auf schneller. |
| **Randentschichtung** | * (1 + 0.1) | Der Zuschlag wird nur bei einer beschichteten Scheibe für ISO berechnet. |
| **Zuschnittfläche** | * Vektor | Das Ergebniss wird mit den Zeiten für die Scheibenfläche multipliziert. |
| **Rundbogenmodell** | + 20 | Bei einem Modell mit Rundbogen werden 20 Sekunden aufgeschlagen. |

Die eigentlichen Zeiten werden in dem Vektor für die Zuschnittsfläche gepflegt, z. B.:

| Fläche (qm) | Wert | Erklärung |
| :--- | :--- | :--- |
| 0.1 | 70 | bis 0.099 qm werden 70 Sekunden gerechnet |
| 0.5 | 45 | für 0.1 - 0.499 qm werden 45 Sekunden genrechnet |
| 1.0 | 60 | für 0.5 - 0.999 qm werden 60 Sekunden gerechnet |
| 2.0 | 150 | für 1.0 - 1.999 qm werden 150 Sekunden gerechnet |
| 3.0 | 210 | für 1.999 - 2.999 qm werden 150 Sekunden gerechnet |

In diesem Beispiel sehen Sie, dass für die ganz kleinen und für die großen Scheiben mehr Zeit für den Zuschnitt benötigt wird. Damit entfällt ein weiterer Größenzuschlag für den Zuschnitt. Für Flächenbearbeitungen kann ein solcher Zuschlag aber durchaus notwendig sein und muss dann an der entsprechenden logischen Maschine definiert werden.

### Bedingung: Modell mit Rundbogen
Die Bedingung soll nur dann die Benutzereingabe als Ergebnis liefern, wenn sie wahr ist.

> **Definition (Beispiel)**
> ```
> IF (($Parts_MODELL_NR >= 60 AND $Parts_MODELL_NR <= 81) OR
> ($Parts_MODELL_NR >= 113 AND $Parts_MODELL_NR <= 118) OR
> ($Parts_MODELL_NR >= 123 AND $Parts_MODELL_NR <= 125) OR
> ($Parts_MODELL_NR >= 133 AND $Parts_MODELL_NR <= 199))
> THEN 20 END
> ```

> **i Längenangabe in der Formel**
> Beachten Sie, dass die Längenwerte in einer Formel in µm angegeben werden müssen.

### Bedingung: Schwellenwert
Bei mehr als 11 Stück soll die Vorgabezeit 10 % kleiner sein.

> **Definition (Beispiel)**
> ```
> IF ($Parts_MENGE > 11) THEN - 0.1 END
> ```

### Bedingung: Vektor für Modellzuschnitt
Vektoren können von Einheiten abhängig sein oder auch nicht lineare Sachverhalte darstellen. Falls Ihnen z. B. der einfache Zuschlag für Modelle mit Rundbögen nicht präzise genug ist, definieren Sie einen Vektor, mit dessen Hilfe Sie die benötigten Koeffizienten einfach und sehr präzise abfragen können.

Im Dialog zur Erfassung eines Formelelements legen Sie dazu ein neues Element mit dem Elementtyp Vektor an. Für einen gültigen Vektor wählen Sie eine Formel für den unabhängigen Parameter, z. B. `AWF_ShapeNumber`.

**Abb. E-63 Vektor für modellabhängige Zeitzuschläge**
*Die Abbildung zeigt die Definition eines Vektors mit einem unabhängigen Parameter (A) und die zugehörige Tabelle für Modellnummern (B).*

Die Tabelle erlaubt die modellabhängige Abstufung der Zuschläge. Der Eintrag der linken Spalte gibt immer den Startwert des Gültigkeitsbereichs an. Es ist gute Praxis, ein Wertepaar für 0 zu definieren, damit der Wertebereich vollständig beschrieben ist.

## Zeitformel-Objekte
Sie können die Stückliste oder Teile der Stückliste als Formelobjekte abbilden, um die Kette der Bearbeitungen darzustellen. Diese Darstellung dient dazu, die Abhängigkeiten der Bearbeitungen in der Vorgabezeitformel zu testen, z. B. um zu prüfen, wie die Bearbeitung davon abhängt, was in der Gegenscheibe gemacht wird. Formelobjekte werden zum Testen von Formeln mit logischen Mengen verwendet.

Formelobjekte sind immer auf eine bestimmte Vorgabezeitformel bezogen. Sie können nicht übergreifend verwendet werden. Sie speichern die Formelobjekte dann, wenn Sie einen Nachweis führen wollen, dass die Formel korrekt angewendet wird.

**Abb. E-64 Stücklistenbaum aus der Sicht der einzelnen Bearbeitungen**
*Die Abbildung zeigt den "Zeitformeltest"-Dialog mit einem hierarchischen Baum von Formelobjekten (E).*
*   **A** Gesamtes Objekt speichern
*   **B** Objekt löschen
*   **C** Objekt hinzufügen
*   **D** Markiertes Objekt löschen
*   **E** Objekte

In diesem Beispiel sehen Sie die Bearbeitungsstückliste einer ISO-Scheibe. Beim Hinzufügen werden die Formelobjekte (E) nummeriert. Mit einem Doppelklick können Sie jedes Formelobjekt öffnen und umbenennen, z. B. das erste Objekt in ISO. Das ist sinnvoll, um die Struktur zu verdeutlichen. Beim Hinzufügen (C) wird unter dem markierten Objekt ein neues Objekt angelegt. Beim Löschen (D) wird das markierte Objekt mit allen Unterebenen gelöscht.

> **i Gespeichertes Objekt zum Testen laden**
> Ein gespeichertes Formelobjekt kann nur für die Formel verwendet werden, zu der es angelegt wurde, z. B. um die Berechnung nach Änderungen in der Vorgabezeitformel zu testen. Daher ist es sinnvoll, beim Speichern einen sprechenden Namen zu vergeben.

Ein Beispiel für ein Formelobjekt finden Sie zum Test der Vorgabezeitformel.
⇨ "So testen Sie die Berechnung der Zeitformel" auf Seite E-126

## Vorgabezeitformeln anlegen und verwalten

In dieser Lerneinheit erfahren Sie, wie Sie Vorgabezeitformeln anlegen, bearbeiten oder löschen.

In der ersten Zeile im Dialog Vorgabezeitformeln können Sie Formelelemente als Vorlagen für alle Maschinen definieren. Wenn Sie für die Maschine 0 eine Zeitformel definieren, wird diese zwar in der Datenbank gespeichert, die Formel wird jedoch nicht verwendet, da der Maschine 0 in der MZO keine Bearbeitung zugewiesen ist.

> **i Voraussetzung**
> Vorgabezeitformeln werden zu den logischen Maschinen definiert, die einen bestimmten Arbeitsgang ausführen. Daher müssen die entsprechenden logischen Maschinen in der Maschinenzuordnung definiert sein.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So definieren Sie eine Vorgabezeitformel” auf Seite E-119
*   "So erstellen Sie einen Vektor mit der Eingabehilfe" auf Seite E-122
*   "So löschen Sie eine Vorgabezeitformel" auf Seite E-124

> **i Komplexität von Vorgabezeitformeln**
> A+W Production bietet die Möglichkeit, Vorgabezeitformeln beliebig komplex zu definieren. Somit lassen sich alle erdenklichen Sonderfälle abdecken.
> Halten Sie Vorgabezeitformeln so einfach wie möglich. Sollte in Ihrer Produktion der Einsatz einer komplexen Vorgabezeitformel nötig sein, setzen Sie sich bitte mit dem Kundenservice der A+W Software GmbH in Verbindung.

### So definieren Sie eine Vorgabezeitformel
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten.
**Abb. E-65 Vorgabezeiten**
2.  Markieren Sie die logische Maschine, für die Sie eine Vorgabezeitformel erstellen wollen.
3.  Klicken Sie auf [Bearbeiten].
    Der Dialog Vorgabezeitformel wird geöffnet.
    Wenn für die logische Maschine bereits in der Maschinenzuordnung eine Formel zur Bearbeitungsdauer hinterlegt wurde, wird eine Warnmeldung angezeigt. Wenn Sie den Vorgang fortsetzen, wird die in der Maschinenzuordnung hinterlegte Formel überschrieben.

**Abb. E-66 Vorgabezeitformel**
*Die Abbildung zeigt den leeren Dialog "Vorgabezeitformel".*
*   **A** Basiszeit
*   **B** Multiplikator Bearbeitungsmenge
*   **C** Aktuelle logische Maschine
*   **D** Formelelement hinzufügen
*   **E** Vordefinierte Formel hinzufügen

4.  Geben Sie die Basiszeit (A) in Sekunden ein.
    Sie können entweder eine vordefinierte Formel hinzufügen (E) und die Daten speichern oder eine Formel mit Formelelementen aufbauen. In den folgenden Schritten wird der Aufbau mit Formelelementen gezeigt.
5.  Klicken Sie auf [Neu] (D), um ein Element auszuwählen.
6.  Wählen Sie das Element aus, z. B. einen Vektor, und übernehmen Sie die Auswahl mit [OK].
    Das ausgewählte Element wird im Dialog Vorgabezeitformel unter der Basiszeit eingefügt.

**Abb. E-67 Vorgabezeitformel mit neuem Element**
*Die Abbildung zeigt ein neu hinzugefügtes Element "Vektor 'Dicke -> Wert'" in der Vorgabezeitformel.*
*   **A** Werte festlegen
*   **B** Berechnung festlegen

7.  Klicken Sie auf [...] (A), um den Dialog zur Eingabe der Werte zu öffnen.
8.  Wenn Sie einen Vektor anlegen, können Sie die Grenzwerte und die Zeitwerte manuell oder über die Eingabehilfe eintragen.
    ⇨ "So erstellen Sie einen Vektor mit der Eingabehilfe" auf Seite E-122
9.  Wählen Sie den Operator (B) für die Berechnung aus.
10. Wiederholen Sie die Schritte 5 - 8, um weitere Elemente hinzuzufügen.
11. Prüfen Sie die Reihenfolge der Formelelemente.
    Die Reihenfolge ist für die Berechnung wichtig, wenn sich der Zuschlag auf die Zwischensumme des vorausgehenden Elements bezieht.
12. Klicken Sie auf [OK], um die Daten zu übernehmen.
    Der Dialog wird geschlossen. Damit haben Sie eine Vorgabezeitformel zusammengestellt. Sie können die Berechnung prüfen und mit einem Formel-Objekt eine Berechnung mit Beispielgrößen starten.
    ⇨ "Zeitformel testen" auf Seite E-125
    ⇨ "Zeitformel-Objekte" auf Seite E-117

### So erstellen Sie einen Vektor mit der Eingabehilfe
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel.
2.  Geben Sie die Basiszeit in Sekunden ein.
3.  Klicken Sie auf [Neu] und wählen Sie ein Element aus, z. B. Vektor 'Dicke -> Wert'.
**Tab. E-3 Vektor 'Dicke -> Wert'**
4.  Klicken Sie auf [Eingabehilfe].

**Tab. E-4 Eingabehilfe für Vektoren**
*Die Abbildung zeigt den Dialog "Eingabehilfe für Vektoren".*
*   **A** Grenzwerte für die Staffelung
*   **B** Werte für den Zeitzuschlag

Zunächst geben Sie die Grenzwerte für die Staffelung (A) und dann die Werte für den Faktor (B) ein. Aus diesen Angaben wird die Tabelle erstellt.
5.  Geben Sie den Startwert und den Endwert ein, z. B. 4.00 und 20.00.
    Diese Werte legen die kleinste und die größte Dicke fest.
6.  Geben Sie die Schrittgröße ein, z. B. 2.00.
    Dieser Wert legt fest, in welchen Schritten die Grenzwerte für die Staffelung zwischen dem Startwert und dem Endwert berechnet werden.
7.  Geben Sie die den Startwert und die Schrittgröße für den Faktor ein, z. B 0.1.
    Dieser Wert legt fest, um welche Größe der Faktor pro Grenzwert erhöht wird. Damit haben Sie alle notwendigen Werte eingetragen.
8.  Klicken Sie auf [OK], um die Berechnung der Tabelle zu starten.
    Der Dialog Eingabehilfe für Vektoren wird geschlossen. Die Tabellen wird berechnet und in den Dialog 'Vektor-> Dicke' übernommen.
    Sie können die Daten korrigieren und ergänzen.
9.  Klicken Sie auf [OK], um die Daten zu speichern.
    Der Dialog Vektor 'Dicke -> Wert' wird geschlossen. Die angelegte Staffelung wird in die Vorgabezeitformel übernommen.

### So löschen Sie eine Vorgabezeitformel
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel.
2.  Markieren Sie das Element, das Sie löschen wollen.
3.  Klicken Sie auf [Löschen].
4.  Wiederholen Sie die Schritte 2 und 3, bis alle Elemente in der Liste entfernt sind, die nicht mehr benötigt werden.
5.  Setzen Sie die Basiszeit auf den Wert Null.
6.  Klicken Sie auf [OK], um die Daten zu speichern.
    Der Dialog wird geschlossen.
    Um eine Vorgabezeitformel insgesamt zu löschen, markieren Sie die Vorgabezeit im Dialog Vorgabezeiten und klicken Sie auf [Löschen].

## Zeitformel testen

Im Dialog Zeitformeltest können Sie Formeln testen und damit die eingegebenen Werte und Berechnungseinstellungen prüfen. Sie können entweder die Formel testen, die Sie aktuell im Dialog Vorgabezeitformel bearbeiten, oder Sie laden eine gespeicherte Formel in den Dialog, um diese zu testen.

Der Formeltest gibt ein Ergebnis aus, das die Zeit des jeweiligen Arbeitsganges in Sekunden angibt.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So testen Sie die Zeitformel" auf Seite E-125
*   "So testen Sie die Berechnung der Zeitformel" auf Seite E-126
*   "So erstellen Sie eine Kopie der Zeitformelsyntax" auf Seite E-130

Daneben können Sie Formelobjekte definieren, die Sie zum Testen aller Formeln verwenden können. Dort geben Sie den konkreten Fall an, in dem Sie die Formel testen wollen, also z. B. die Dicke und die Breite einer Scheibe. Damit haben Sie immer die gleichen Vorgaben für den Test. Diese Funktion ist in einer separaten Einheit beschrieben.
⇨ "Zeitformel-Objekte" auf Seite E-117

### So testen Sie die Zeitformel
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel.
**Abb. E-68 Vorgabezeitformel**
2.  Markieren Sie das Formelelement, das Sie testen wollen.
Wenn Sie die gesamte Vorgabzeitformel testen wollen, müssen Sie das Element Basic Time markieren. Sie können aber auch jedes Element einzeln testen, indem Sie es markieren und die nachfolgenden Schritte ausführen.
3.  Klicken Sie auf [Formeltest].

**Abb. E-69 Zeitformeltest**
*Die Abbildung zeigt den Dialog "Zeitformeltest".*
*   **A** Testergebnis
*   **B** Auswertung starten

4.  Klicken Sie auf [Auswerten] (B).
    Das Berechnungsergebnis (A) wird angezeigt. Sie können die Formel ggf. weiter bearbeiten und korrigieren.
5.  Klicken Sie auf [OK], um die Daten zu speichern.
    Um die Formel mit Scheibendaten zu testen, können Sie für den Test ein Formelobjekt anlegen und Werte eingeben.

### So testen Sie die Berechnung der Zeitformel
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel.
    Der Dialog Vorgabezeitformel wird geöffnet.
2.  Klicken Sie auf [Formeltest].

**Abb. E-70 Zeitformel-Objekt**
*   **A** Objekt markieren
*   **B** Objekt hinzufügen

3.  Klicken Sie doppelt auf das Formelobjekt (A), um den Dialog zur Eingabe der Eigenschaften zu öffnen.

**Abb. E-71 Eigenschaften des Formel-Objekts**
*   **A** Frei wählbarer Name
*   **B** Auswahl des Typs

4.  Geben Sie einen Namen (A) ein und wählen Sie den Typ (B) aus, z. B. Teil.
5.  Klicken Sie auf [Hinzufügen].
    Die Felder in der Spalte Eigenschaften werden mit den Elementen vorbelegt, die in der aktuellen Vorgabezeitformel enthalten sind.
**Abb. E-72 Werte für Formelobjekt eingeben**
6.  Geben Sie zu jeder Eigenschaft die entsprechenden Werte ein, z. B. die Maße für Höhe und Breite.
    Beachten Sie, dass Sie die Maße in Mikrometer (µm) eingeben müssen.
7.  Klicken Sie auf [Schließen], um die Daten zu speichern und den Dialog zu schließen.
    Der Dialog Formeltest wird wieder im Vordergrund angezeigt.
**Abb. E-73 Berechnung mit Zeitformel-Objekt**
8.  Markieren Sie das Formelobjekt, für das die Berechnung gestartet werden soll.
9.  Klicken Sie auf [Formeltest].
    Das Ergebnis der Berechnung mit den eingegebenen Werten wird angezeigt. Wenn die Berechnung nicht Ihren Vorstellungen entspricht, können Sie die berechneten Werte prüfen.

### So erstellen Sie eine Kopie der Zeitformelsyntax
1.  Testen Sie die Zeitformel wie in der vorausgehenden Handlungssequenz angegeben.

**Abb. E-74 Zeitformeltest**
*   **A** Formel anzeigen

2.  Aktivieren Sie die Checkbox Formel anzeigen (A).

**Abb. E-75 Formelsyntax**
*Die Abbildung zeigt die natürliche und die native Syntax der Formel.*

In diesem Dialog können Sie die Syntax der kompletten Formel prüfen. Um die Syntax mit Unterstützung durch den A+W-Service zu korrigieren, kopieren Sie die Syntax und senden Sie den Text an A+W.

### Übungen
*   Wählen Sie eine logische Maschine Ihrer Test-Maschinen und planen Sie auf dem Papier die Vorgabezeiten für diese logische Maschine:
    *   Welche Scheiben werden auf der logischen Maschine bearbeitet?
    *   Welche Faktoren benötigen Sie, um die Vorgabezeiten für diese Scheiben zu definieren?
    *   Wie sollen diese Faktoren in die Vorgabezeitformel einfließen?
*   Stellen Sie die Vorgabezeitformel mit den benötigten Elementen zusammen.
*   Erfassen Sie für den Eintrag 0 - Alle Maschinen verschiedene Formelelemente, z. B. einen eigenen Vektor, eine Tabelle, einen Schwellenwert.
*   Legen Sie zu einer Formel ein Formelobjekt an und testen Sie die Vorgabezeitformel, um zu prüfen, ob das Ergebnis Ihren Erwartungen entspricht.

### Ergänzende Informationen
⇨ Softwarereferenz, "Vorgabezeiten" auf Seite E-206
⇨ Softwarereferenz, "Vorgabezeitformel" auf Seite E-208
⇨ Softwarereferenz, "Tabelle, Vektor (Name)" auf Seite E-213
⇨ Softwarereferenz, "Eingabehilfe für Vektoren" auf Seite E-214
⇨ Softwarereferenz, "Erfassung eines Formelelements" auf Seite E-217

## Maschinengruppen

### Lernziele
*   Was sind Maschinengruppen in der Kapazitätsplanung?
*   Wie werden Maschinengruppen erstellt, bearbeitet oder gelöscht?

### Nutzen
*   Mit Maschinengruppen fassen Sie Maschinen eines Bereichs zusammen und steuern über die Mitarbeiteranzahl die Kapazität der Gruppe.

### Merke
*   **Maschinengruppen**: Mit Maschinengruppen fassen Sie Maschinen von Bereichen zusammen, z. B. Zuschnitt oder Kantenbearbeitung.
*   **Personen**: Sie weisen Maschinengruppen jeweils eine Personenanzahl zu und legen damit die Kapazität der jeweiligen Maschinengruppe fest.
*   **Schichten**: Bei Maschinen einer Maschinengruppe müssen die Schichten übereinstimmen.
*   **Engpassbetriebsmittel**: Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden. Maschinen werden zu einem Engpassbetriebsmittel, wenn sie einer Maschinengruppe zugewiesen werden.

> **i Voraussetzung**
> Bei allen Maschinen, die zu einer Maschinengruppe hinzugefügt werden, müssen die Schichten übereinstimmen. Dies umfasst die Start- und die Endzeit der Schichten.

## Definition der Maschinengruppen
Sie können Maschinen zu Gruppen zusammenfassen. Maschinengruppen sind für Maschinen des gleichen Bereichs sinnvoll. So könnten Sie z. B. eine Maschinengruppe Zuschnitt erstellen, der Sie alle Maschinen des Zuschnitts zuordnen. Eine festgelegte Kapazität gilt dann für die gesamte Maschinengruppe, also z. B. für den Zuschnitt.
Sie können nur Maschinen zu einer Gruppe zusammenfassen, deren Schichten übereinstimmen, die also zur gleichen Zeit verfügbar sind. Maschinen, die Sie zu einer Maschinengruppe hinzufügen, werden automatisch zu einem Engpassbetriebsmittel.

**Abb. E-76 Maschinengruppen**
*Die Abbildung zeigt den Dialog "Maschinengruppen".*
*   **A** Maschinengruppe
*   **B** Verfügbare Maschinen
*   **C** Anzahl der Personen in der Gruppe
*   **D** Zugeordnete Maschinen

Den Maschinengruppen müssen Sie jeweils eine Anzahl von Personen (C) zuordnen. A+W Production geht grundsätzlich davon aus, dass an jeder Maschine eine Person arbeitet. Wenn Sie die Anzahl der Mitarbeiter in der Gruppe reduzieren, verringert sich die verfügbare Zeit pro Maschine.

> **Beispiel**
> In der Maschinengruppe Zuschnitt mit vier Maschinen werden vier Personen angenommen.
> Wenn die 4 Mitarbeiter 40 Stunden pro Woche arbeiten, sind 4 x 40 = 160 Arbeitsstunden pro Woche verfügbar.
> Bei 3 Mitarbeitern sind nur noch 3 x 40 = 120 Arbeitsstunden pro Woche verfügbar.

## Maschinengruppen anlegen und verwalten
In dieser Lerneinheit erfahren Sie, wie Sie Maschinengruppen anlegen, bearbeiten oder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine Maschinengruppe an" auf Seite E-134
*   "So bearbeiten Sie eine Maschinengruppe" auf Seite E-136
*   "So löschen Sie eine Maschinengruppe" auf Seite E-137

### So legen Sie eine Maschinengruppe an
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Maschinengruppen.
**Abb. E-77 Maschinengruppen**
2.  Klicken Sie auf [Neu].
3.  Geben Sie einen Namen für die Maschinengruppe ein, z. B. Zuschnitt.
4.  Klicken Sie auf [OK].
    Im Feld Maschinengruppen wird die neue Maschinengruppe angezeigt.
5.  Markieren Sie die neue Maschinengruppe.
    In der Liste Maschinen für Gruppe ... werden alle verfügbaren Maschinen angezeigt.
6.  Markieren Sie die Maschine, die Sie zu der Gruppe hinzufügen wollen, z. B. 180 Schneidetisch 8.
7.  Klicken Sie auf den Pfeil nach rechts und bestätigen Sie die Meldung.
    Die Maschine wurde zur Gruppe hinzugefügt.
8.  Wiederholen Sie die Schritte 5 bis 7, um weitere Maschinen hinzuzufügen.
9.  Klicken Sie im Feld Maschinengruppen doppelt in die Spalte Personen.
10. Geben Sie die Anzahl der Personen ein, die in dieser Maschinengruppe arbeiten.
11. Klicken Sie auf [OK], um die Daten zu speichern.
    Der Dialog wird geschlossen. Damit haben Sie die Maschinengruppe angelegt.

### So bearbeiten Sie eine Maschinengruppe
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Maschinengruppen.
**Abb. E-78 Markierte Maschinengruppe**
2.  Markieren Sie im Feld Maschinengruppen die Maschinengruppe, die Sie bearbeiten wollen.
    In der Liste Maschinen für Gruppe ... werden auf der rechten Seite alle Maschinen angezeigt, die der Gruppe zugeordnet sind. Auf der linken Seite werden die verfügbaren Maschinen angezeigt.
3.  Markieren Sie eine Maschine, die Sie aus der Gruppe entfernen oder zur Gruppe hinzufügen wollen.
4.  Klicken Sie auf den Pfeil nach links oder den Pfeil nach rechts, um eine Maschine aus der Gruppe zu entfernen oder um sie zur Gruppe hinzuzufügen.
5.  Wiederholen Sie die Schritte 3 bis 4, um weitere Maschinen aus der Gruppe zu entfernen oder zur Gruppe hinzuzufügen.
6.  Korrigieren Sie im Feld Maschinengruppen die Anzahl der Personen.
7.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen.

### So löschen Sie eine Maschinengruppe
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Maschinengruppen.
2.  Markieren Sie im Feld Maschinengruppen die Maschinengruppe, die Sie löschen wollen.
3.  Klicken Sie auf [Löschen].
    Die Maschinengruppe wird aus der Liste entfernt. Damit ändern Sie die verfügbare Kapazität für die Einlastung.
4.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Erarbeiten Sie, welche Maschinen Sie zu Gruppen zusammenfassen wollen.
*   Erstellen Sie mindestens eine Maschinengruppe im Dialog Maschinengruppen.
*   Bearbeiten Sie Ihre Maschinengruppe.
*   Löschen Sie eine Ihrer Maschinengruppen.

### Ergänzende Informationen
⇨ Softwarereferenz, "Maschinengruppen" auf Seite E-245

## Lastverteilung

### Lernziele
*   Was ist die Lastverteilung in der Kapazitätsplanung?
*   Wie wird eine Lastverteilung erstellt, bearbeitet oder gelöscht?

### Nutzen
*   Die Lastverteilung ist bei Maschinen mit einer Spezialqualifikation sinnvoll. Wenn diese Qualifikation nicht abgerufen wird, wird die Maschine für die Standardbearbeitung genutzt.

### Merke
*   **Physikalische Maschine**: Sie können eine Lastverteilung nur für eine Maschine einrichten, die als Engpassbetriebsmittel definiert ist. Sie können z. B. auf der Maschine 30% für Modelle freihalten, die aber für Rechtecke verwendet werden dürfen, wenn keine Modelle eingelastet sind.
*   **Logische Maschinen**: Die Lastverteilung wird unter den logischen Maschinen vorgenommen, die zu derselben physikalischen Maschine definiert sind. Damit können Sie die Lastverteilung eines CNC-Centers mit z. B. den drei logischen Maschinen Sonderkanten, Ausschnitte und Bohrungen prozentual aufteilen. Diese Lastverteilung wird bei der Einlastung berücksichtigt.
*   **Engpassbetriebsmittel**: Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

## Definition der Lastverteilung
Die Lastverteilung wird unter den logischen Maschinen festgelegt, die zu derselben physikalischen Maschine definiert sind. Damit legen Sie den prozentualen Anteil der logischen Maschinen an der Gesamtkapazität der physikalischen Maschine fest.

Lastverteilung nutzen Sie, um zu gewährleisten, dass eine Maschine eine garantierte Mindestkapazität für Spezialaufgaben freihält, z. B. für den Modellzuschnitt. Wenn die freigehaltene Kapazität nicht für Modelle genutzt wird, können auch Rechtecke bearbeitet werden. Diese Lastverteilung ist nur bei Maschinen möglich und sinnvoll, die als Engpassbetriebsmittel definiert sind.

**Abb. E-79 Lastverteilung**
*Die Abbildung zeigt den Dialog "Lastverteilung".*
*   **A** Physikalische Maschine
*   **B** Bearbeitung freischalten
*   **C** Logische Maschinen
*   **D** Anteile an der Gesamtkapazität

Sie teilen die Kapazität einer Maschine auf, indem Sie den zugehörigen logischen Maschinen (C) prozentuale Anteile (D) zuordnen.

> **Beispiel**
> Eine Maschine kann Formen bearbeiten, also Rechtecke und Modelle. Damit diese Spezialqualifikation nicht von den einfacheren Rechtecken belegt wird, halten Sie z. B. 30% für Modelle frei. Diese Lastverteilung wird bei der Einlastung berücksichtigt.
> Wenn diese 30% aber nicht für Modelle gebraucht werden, können auch Rechtecke bearbeitet werden.

## Lastverteilung einrichten und bearbeiten
In dieser Lerneinheit erfahren Sie, wie Sie Lastverteilungen einrichten, bearbeiten oder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So richten Sie eine Lastverteilung ein" auf Seite E-140
*   "So bearbeiten Sie eine Lastverteilung" auf Seite E-142
*   "So löschen Sie eine Lastverteilung" auf Seite E-143

> **i Voraussetzung**
> Sie können eine Lastverteilung nur für eine Maschine einrichten, die als Engpassbetriebsmittel definiert ist.

### So richten Sie eine Lastverteilung ein
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Lastverteilung.
**Abb. E-80 Lastverteilung definieren**
*   **A** Maschine
*   **B** Felder freischalten
2.  Wählen Sie die Maschine (A) aus, deren Kapazität Sie aufteilen wollen.
    In der Auswahl-Liste sind nur die Maschinen freigeschaltet, die als Engpassbetriebsmittel definiert sind.
**Abb. E-81 Logische Maschinen**
    Die zugehörigen logischen Maschinen werden in der Liste angezeigt.
3.  Aktivieren Sie die Checkbox Prüfung aktivieren (B), um die Felder freizuschalten.
    Die Felder der logischen Maschinen werden freigeschaltet. Ist noch keine Lastverteilung angegeben, steht in der rechten Spalte unbegrenzt.
4.  Klicken Sie doppelt in die rechte Spalte.
5.  Geben Sie den Prozentwert für die Kapazität ein.
6.  Wiederholen Sie die Schritte 4 bis 5, um bei allen logischen Maschinen den Anteil an der Gesamtkapazität der physikalischen Maschine einzurichten.
7.  Deaktivieren Sie die Checkbox Prüfung aktivieren, um versehentliche Änderungen zu verhindern.
8.  Klicken Sie auf [OK], um die Daten zu speichern und den Dialog Lastverteilung zu schließen.
    Die Daten werden gespeichert und der Dialog wird geschlossen.

### So bearbeiten Sie eine Lastverteilung
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Lastverteilung.
**Abb. E-82 Lastverteilung definieren**
*   **A** Maschine
*   **B** Felder freischalten
2.  Wählen Sie die Maschine (A), deren Lastverteilung Sie bearbeiten wollen.
    In der Auswahl-Liste sind nur die Maschinen freigeschaltet, die als Engpassbetriebsmittel definiert sind.
3.  Aktivieren Sie ggf. die Checkbox Prüfung aktivieren (B).
**Abb. E-83 Lastverteilung der ausgewählten Maschine**
4.  Ändern Sie bei allen logischen Maschinen den Prozentwert für die Kapazität.
5.  Deaktivieren Sie ggf. die Checkbox Prüfung aktivieren.
6.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen.

### So löschen Sie eine Lastverteilung
1.  Wählen Sie Stammdaten > Kapazitätsplanung > Lastverteilung.
2.  Wählen Sie im Feld Physikalische Maschinen die Maschine, deren Lastverteilung Sie löschen wollen.
    Die zugehörigen logischen Maschinen werden in der Liste angezeigt.
3.  Aktivieren Sie die Checkbox Prüfung aktivieren.
    Die Felder werden freigeschaltet.
4.  Ändern Sie bei allen logischen Maschinen den Prozentwert für die Kapazität auf 000%.
    In den Feldern wird unbegrenzt angezeigt.
5.  Deaktivieren Sie ggf. die Checkbox Prüfung aktivieren.
6.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen. Damit haben Sie die Lastverteilung für die Maschine gelöscht.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Prüfen Sie, bei welchen Ihrer Maschinen eine Lastverteilung sinnvoll ist. Legen Sie ggf. zuvor weitere logische Maschinen zu Ihren Test-Maschinen an.
*   Richten Sie mindestens eine Lastverteilung ein.
*   Bearbeiten Sie eine Lastverteilung.
*   Löschen Sie eine Lastverteilung.

### Ergänzende Informationen
⇨ Softwarereferenz, "Lastverteilung" auf Seite E-247

---

# Softwarereferenz

## Überblick
Für die Planung und Organisation der Kapazitäten Ihrer Produktion steht der Dialog Produktionsmonitor zur Verfügung. In diesem werden die Arbeitsschichten pro Maschine angezeigt.

Die Aufträge werden positionsweise eingelastet, wobei die Einlastung pro Position erfolgreich sein muss. Wenn eine Auftragsposition nicht erfolgreich eingelastet werden kann, wird der gesamte Auftrag nicht eingelastet.

Damit die Berechnungen im Produktionsmonitor korrekt ablaufen, müssen die Stammdaten der Kapazitätsplanung eingerichtet werden. Die Beschreibung der Dialoge ist zu Themengruppen zusammengefasst. Sie folgt nicht der Anordnung der Dialoge in der Softwarereferenz.

In dieser Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   "Einlastung" auf Seite E-148
*   "Kampagnen und Reservierungen" auf Seite E-187
*   "Bearbeitungen" auf Seite E-200
*   "Stammdaten für Zeiten" auf Seite E-205
*   "Stammdaten der Schichten" auf Seite E-230
*   "Maschinen und Kosten" auf Seite E-242

## Einlastung
Der Produktionsmonitor ist der zentrale Kapazitäts- und Auftrags-Leitstand und der Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlastung.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Produktionsmonitor" auf Seite E-149
*   "Angezeigte Maschinen" auf Seite E-153
*   "Einstellungen" auf Seite E-154
*   "Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)" auf Seite E-157
*   "Neuen Filter erstellen" auf Seite E-160
*   "Maschine (Name)" auf Seite E-161
*   "Schichten für Maschine anpassen" auf Seite E-163
*   "Schichteigenschaften" auf Seite E-164
*   "Reservierungsanzeige" auf Seite E-166
*   "Arbeitsplan aus Produktionsmonitor" auf Seite E-167
*   "Einlastung" auf Seite E-171
*   "Stücklistenkonfiguration" auf Seite E-172
*   "Aktion" auf Seite E-173
*   "Umlastung" auf Seite E-174
*   "Maschinenumlastung" auf Seite E-178
*   "Nachbearbeitung Einlastung" auf Seite E-179
*   "Fehlerhafte Aufträge" auf Seite E-182
*   "Asynchrone Verarbeitung" auf Seite E-183
*   "Änderung bereits verplanter Aufträge” auf Seite E-184
*   "Positionssplit" auf Seite E-185

## Produktionsmonitor
**Pfad:** Anzeigen > Produktionsmonitor
**Pfad:** Detailanzeige > Kontextmenü > Produktionsmonitor

**Abb. E-84 Produktionsmonitor**
*Die Abbildung zeigt die Hauptansicht des Produktionsmonitors, eine grafische Plantafel mit Maschinen auf der Y-Achse und Zeitschlitzen auf der X-Achse.*

In diesem Dialog werden die aktuelle Planung der Produktion und die kapazitive Auslastung der Maschinen pro Arbeitsschicht angezeigt. Damit ist der Produktionsmonitor der zentrale Kapazitäts- und Auftrags-Leitstand und der Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlastung.
⇨ Tutorial, "Produktionsmonitor" auf Seite E-22

### Schaltflächen

| Symbol | Funktion | Beschreibung |
| :--- | :--- | :--- |
| 🔲 | Ausgewählte Maschinen | ⇨ "Angezeigte Maschinen" auf Seite E-153 |
| ⚙️ | Einstellungen | ⇨ "Einstellungen" auf Seite E-154 |
| A | Anzeigeart für alle Maschinen ändern | Auswahl der Anzeige für alle Maschinen: Zeit, Menge, Fläche, Gewicht |
| 📅 | Anzeige ändern (Schicht, Tag, Woche) | Ändert die Anzeige. Die Maschinenkapazität wird entweder pro Arbeitsschicht, Tag oder Woche angezeigt |
| ↔️ | Ansicht umschalten | Schaltet die Ansicht um. Hauptansicht: Alle Schichten im angegebenen Zeitraum werden angezeigt. Detailansicht: Nur die Schichten des angegebenen Tags werden angezeigt. |
| 🔍 | Vergrößern, Verkleinern | Vergrößert, verkleinert die Darstellung der Arbeitsschichten. |
| 🔄 | Ansicht aktualisieren | Aktualisiert die Ansicht. |
| « » | Gegebene Anzahl von Tagen zurück, vor | Verschiebt den angezeigten Zeitraum um die Anzahl der Tage vor oder zurück, die im Feld Tage angegeben ist. |
|  lọc | Ansicht filtern, Filter entfernen | ⇨ "Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)" auf Seite E-157 |

*   **Starttermin**: Öffnet den Kalender, um den Starttag für die Anzeige der Arbeitsschichten auswählen.
*   **Tage**: Angabe, um wie viele Tage die Anzeige mit den Schaltflächen jeweils vor- oder zurückgestellt werden soll.
*   **Eingabefeld Filter**: Eingabe des Filterkriteriums, die Anzeige nach Aufträgen oder Läufen zu filtern.

> **i Darstellung**
> Die Darstellung kann individuell angepasst werden. Dies betrifft z. B. die Farben, ein Zeitraster, Statusinformationen usw.
> ⇨ "Einstellungen" auf Seite E-154

### Arbeitsschichten
Im Produktionsmonitor werden die Arbeitsschichten aller ausgewählten Maschinen angezeigt. Maschinen, die als Engpassbetriebsmittel definiert sind, werden in roter Schrift angezeigt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.
