---
description: "DE_AWBusiness_LogisticOptimizer_2_1"
---


# A+W Logistic Optimizer

**A+W Business**

*A+W - Software for Glass, Windows and Doors*

---

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 1.00/05-2014 | Ersterstellung |
| 2.00/10-2015 | Komplette Überarbeitung |
| 2.01/01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
* Anmerkungen zu diesem Dokument
* Urheberrechte
* Warenzeichen
* Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von *A+W Business* gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.

#### Urheberrechte
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**

Am Pfahlgraben 4 - 10
D-35415 Pohlheim
Germany

Tel: +49 6404 2051 0
Fax: +49 6404 2051 877
E-Mail: Zentrale@a-w.com
Web: http://www.a-w.com

---

## Inhalt

| Thema | Seite |
| :--- | :--- |
| **Vorspann** | |
| Revisionsübersicht | 1-3 |
| Editorial | 1-3 |
| **Tutorial** | **1-9** |
| Überblick | 1-11 |
| Dokumentation | 1-12 |
| Aufbau des Tutorials | 1-12 |
| Darstellungskonventionen | 1-13 |
| Grundgedanken zu OTR | 1-14 |
| Datenbankverbindungen | 1-15 |
| Verbindung zur OTR-Datenbank | 1-15 |
| Verbindung zur ERP-Datenbank | 1-15 |
| Der dynamische Modus | 1-17 |
| Die Oberfläche | 1-18 |
| Die Menü- und Symbolleisten | 1-20 |
| Feldhilfe | 1-27 |
| **Administration** | **1-28** |
| Parameter | 1-29 |
| Stammdaten | 1-30 |
| Benutzer | 1-31 |
| Status | 1-32 |
| Die Status-Typen verwalten | 1-33 |
| Kunden | 1-34 |
| Die Kunden verwalten | 1-35 |
| Abteilungen | 1-37 |
| Die Abteilungen verwalten | 1-37 |
| Fahrzeuge | 1-39 |
| Die Fahrzeuge verwalten | 1-40 |
| Fahrer | 1-43 |
| Die Fahrer verwalten | 1-44 |
| Reports | 1-46 |
| Die Reports verwalten | 1-47 |
| Datenimport | 1-49 |
| **Planung** | **1-50** |
| Touren und Bestimmungsorte | 1-51 |
| Allgemein | 1-52 |
| Import | 1-53 |
| Touren | 1-54 |
| Eine gespeicherte Tour laden | 1-54 |
| Eine gespeicherte Tour kopieren | 1-55 |
| Mit Touren arbeiten | 1-57 |
| Bestimmungsorte | 1-64 |
| Dokumente anzeigen | 1-65 |
| Dokumente löschen | 1-65 |
| Positionen anzeigen | 1-66 |
| Informationen anzeigen | 1-67 |
| Die Detailansicht | 1-68 |
| Kundenadressen bearbeiten | 1-70 |
| Mit Bestimmungsorten arbeiten | 1-71 |
| Kosten | 1-74 |
| Ausgaben | 1-75 |
| Variable Kosten | 1-75 |
| Fixkosten | 1-76 |
| Tourkosten | 1-76 |
| **Optimierung** | **1-77** |
| Überblick | 1-78 |
| Touren optimieren | 1-79 |
| Unterschiedliche Kartenmodi | 1-82 |
| Touren verändern | 1-83 |
| **Ergebnis** | **1-86** |
| Überblick | 1-87 |
| Das Ergebnis der Optimierung | 1-88 |
| Touren | 1-88 |
| Tourenplan | 1-89 |
| Bestimmungsort | 1-89 |
| Tourstatus ändern | 1-90 |
| Tatsächliche Tourkosten | 1-91 |
| **Abfragen** | **1-93** |
| Überblick | 1-94 |
| Unterschiedliche Abfragen | 1-95 |
| Touren | 1-95 |
| Filtern | 1-95 |
| Ändern und Status | 1-96 |
| Löschen | 1-96 |
| Export | 1-97 |
| Export an Navigationssysteme | 1-97 |
| Laden der Daten auf mobile Endgeräte (über die Cloud) | 1-99 |
| Historie | 1-104 |
| Reports | 1-105 |
| Ausgewählte Tour | 1-105 |
| Listen drucken | 1-106 |
| Report Launcher | 1-107 |
| Statistiken | 1-107 |
| Eine Statistik erstellen | 1-108 |
| Ansicht | 1-110 |
| Tour | 1-110 |
| Bestimmungsort | 1-110 |
| Kalender | 1-110 |
| Routen Administrator | 1-112 |
| **Softwarereferenz** | **1-115** |
| Konfiguration | 1-117 |
| OTR-Verbindung | 1-118 |
| ERP-Verbindung | 1-119 |
| Parameter | 1-120 |
| Administration | 1-129 |
| Benutzer | 1-130 |
| Status | 1-131 |
| Kunden | 1-133 |
| Abteilungen | 1-135 |
| Fahrzeuge | 1-136 |
| Fahrer | 1-139 |
| Reports | 1-142 |
| Datenimport | 1-143 |
| Planung | 1-145 |
| Eine gespeicherte Tour kopieren | 1-147 |
| Eine gespeicherte Tour laden | 1-150 |
| Bestimmungsorte importieren | 1-151 |
| Eine neue Tour zusammenstellen - Allgemein | 1-152 |
| Geolokalisieren | 1-155 |
| Eine neue Tour zusammenstellen - Fahrzeuge | 1-156 |
| Fahrzeug wählen | 1-159 |
| Fahrer hinzufügen | 1-160 |
| Eine neue Tour zusammenstellen - Parameter | 1-162 |
| Tour-Faktoren | 1-166 |
| Eine neue Tour zusammenstellen - Kosten | 1-168 |
| Bereiche | 1-170 |
| Fahrzeuge | 1-171 |
| Bestimmungsort bearbeiten | 1-172 |
| Zeitbereich | 1-175 |
| Dokumente | 1-176 |
| Positionen anzeigen | 1-177 |
| Informationen anzeigen | 1-179 |
| Kunden | 1-181 |
| Detailansicht | 1-183 |
| Optimierung | 1-184 |
| Tour optimieren | 1-185 |
| Ergebnis | 1-187 |
| Ergebnis der Optimierung | 1-188 |
| Tour-Informationen | 1-190 |
| Abfrage | 1-192 |
| Routen filtern | 1-193 |
| Export | 1-195 |
| Statusänderung | 1-197 |
| Historie | 1-198 |
| Bestätigungs- und Lieferliste | 1-200 |
| Report Launcher | 1-203 |
| Statistik | 1-204 |
| Register Allgemein | 1-204 |
| Register Allgemeine Grafik | 1-205 |
| Register Fahrzeuge | 1-206 |
| Register Fahrer | 1-207 |
| Register Abteilungen | 1-208 |
| Register Kunden | 1-209 |
| Kalender | 1-210 |
| **Partindex** | **1-211** |
| Index | 1-213 |

---

## Tutorial

### Überblick

Der *A+W Logistic Optimizer* (auch *OTR* genannt - Optimizer of Transport Routes) beschäftigt sich mit den Grundlagen der Touren- und Routenplanung. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zum Nummernverwalter auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
>
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
* Grundgedanken zu OTR
* Administration
* Touren planen
* Touren optimieren
* Ergebnisse prüfen
* Abfragen

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in OTR Aufträge zur Auslieferung vorbereiten und im Büro die Lieferung mittels verschiedener LKW überwachen. Die Teilnehmer müssen das Konzept der Stammdaten und des Nummernverwalters kennen.

### Dokumentation
Für das Modul *OTR* stehen folgende Dokumente zur Verfügung:

*   **Handout**: Ausdruck des Tutorials für die Schulung
*   **PDF**: Vollständige Unterlagen
    *   Tutorial
    *   Softwarereferenz
    *   Index
*   **Online-Hilfe <F1>**: Kontextsensitive Dialog-Hilfe der *A+W Business*-Softwarereferenzen und Tutorials der Basisversion

### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

*   **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    *   **Lernziele**: Was soll vermittelt werden?
    *   **Nutzen**: Wofür können Sie dieses Wissen einsetzen?
    *   **Merksätze**: Welche Zusammenhänge müssen Sie sich merken?
*   **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
*   **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
*   **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

> **Lesehinweis**
> Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
> Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

*   *Kursiv*: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Nummernverwalter*.
*   **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
*   **>**: Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Fertigung > Produktion > Produktionsübergabe*.
*   **[]**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten.
*   **< >**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit <F1> öffnen Sie die Online-Hilfe.

---

## Grundgedanken zu OTR

Durch eine sinnvolle Routenoptimierung und Tourenplanung im Transportbereich können Fahrtzeiten und Fahrwege verkürzt und damit der Kraftstoffverbrauch erheblich vermindert werden. In der Folge werden die Umweltbelastungen reduziert, Fahrzeuge werden weniger abgenutzt und die Fahrer werden durch weniger überflüssig gefahrene Kilometer entlastet.

Sowohl eine Tourenplanung als auch eine Routenoptimierung spart also Kosten und erhöht die Produktivität.

Der *Optimizer for Transport Routes (OTR)* bringt Ihre Zielorte, Kundenadressen oder Haltepunkte in eine sinnvolle und effiziente Reihenfolge.

Diese Reihenfolge berücksichtigt neben dem individuellen Fuhrpark auch die hinterlegten Streckenanforderungen, wie z. B. Tunnel oder Mautstraßen. Die Technik basiert auf Nokia Maps in Kombination mit einem mathematischen Algorithmus.

Über die mobile App können Lieferungen durch den Fahrer direkt verbucht und zurückgemeldet werden. Weiterhin erhält der Fahrer alle notwendigen Informationen über die Gesamtstrecke und einzelne Ladestationen.

Via GPS können Sie im Büro die Lieferung überwachen.

Der Prozessablauf stellt sich wie folgt dar:

`Planung -> Optimierung -> Ergebnis`

**Abb. I-1: Standardprozess für die Lieferreihenfolge**

Der Prozess gliedert sich in vier Phasen:
*   **Planung**: In dieser Phase stellen Sie die Tour(en) zusammen. Sie können neue Touren erstellen, vorhandene Touren bearbeiten oder auch löschen. Innerhalb der Touren können Sie Bestimmungsorte (Haltepunkte) hinzufügen, bearbeiten oder aber auch einzelne Orte löschen. In dieser Phase haben Sie ebenfalls Zugriff auf die einzelnen Positionen, um sich einen Überblick zu verschaffen.
*   **Optimierung**: In dieser Phase findet die Optimierung der Strecke statt. Auf der Übersichtskarte sehen Sie die Streckenführung und auf der rechten Seite die Auflistung der einzelnen Stationen (Wegpunkte). Sie können einzelne Stationen miteinander tauschen und haben Zugriff auf die Optimierungs-Faktoren. In der Optimierung werden auch Einstellungen und Änderungen aus der Phase der Planung berücksichtigt - bspw. spezielle Abladezeiten oder Prioritäten von Kunden (Ladestationen).
*   **Ergebnis**: Diese Phase liefert Ihnen das Gesamtergebnis der Tour gegliedert in die einzelnen Touren, den grafischen Tourenplan sowie die Übersicht der Bestimmungsorte.

### Datenbankverbindungen

Um mit dem Modul arbeiten zu können, müssen Verbindungen zu den beiden folgenden Datenbanken bestehen:
*   OTR
*   ERP

#### Verbindung zur OTR-Datenbank
Die Verbindung zum OTR-Datenbank-Server ist nötig, um die Routen zu planen.

*(Abb. I-2: Datenbank-Einstellungen OTR. Ein Dialogfenster zur Konfiguration der SQL-Server-Verbindung für die OTR-Datenbank mit Feldern für Datenquelle, Start-Katalog, Benutzer-ID und Kennwort.)*

Beim erstmaligen Aufruf erscheint dieser Dialog automatisch. Geben Sie im Feld *Datenquelle* den Pfad zum OTR-Datenbankserver ein. Diese Informationen erhalten Sie von Ihrem zuständigen Ansprechpartner im A+W Support oder Qualified Service.

Im Feld *Start-Katalog* geben Sie die Standard-Datenbank ein. Diese ist *OTR*. Die Einträge für *Benutzer-ID* und *Kennwort* erhalten Sie ebenfalls von Ihrem zuständigen Ansprechpartner im A+W Support oder Qualified Service.

Nachdem Sie die Einstellungen vorgenommen haben, können Sie über die Symbol-Schaltfläche **[Test]** eine Testverbindung zur Datenbank aufbauen.

> **Datenbankverbindung**
> Bitte beachten Sie, dass diese Einstellungen für jeden Benutzer vorgenommen werden müssen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "OTR-Verbindung" auf Seite I-134

#### Verbindung zur ERP-Datenbank
Die Verbindung zum ERP-Datenbank-Server ist nötig, damit das Modul auf die Daten von *A+W Business* zugreifen kann.

*(Abb. I-3: Datenbank-Einstellungen ERP. Ein Dialogfenster zur Konfiguration der SQL-Server-Verbindung für die ERP-Datenbank, ähnlich dem OTR-Dialog.)*

Beim erstmaligen Aufruf erscheint dieser Dialog automatisch mit dem Register *OTR-Datenbank*. Wechseln Sie in das Register *ERP-Verbindung*.

Im Feld *Start-Katalog* geben Sie die Standard-Datenbank ein. Die Einträge für *Benutzer-ID* und *Kennwort* erhalten Sie ebenfalls von Ihrem zuständigen Ansprechpartner im A+W Support oder Qualified Service.

Nachdem Sie die Einstellungen vorgenommen haben, können Sie über die Symbol-Schaltfläche **[Test]** eine Testverbindung zur Datenbank aufbauen.

> **Datenbankverbindung**
> Bitte beachten Sie, dass diese Einstellungen für jeden Benutzer vorgenommen werden müssen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "OTR-Verbindung" auf Seite I-134

### Der dynamische Modus

Arbeiten Sie im dynamischen Modus, erscheint, nachdem Sie im Nummernverwalter die Symbol-Schaltfläche angeklickt haben, folgender Dialog:

*(Abb. I-4: Dynamischer Modus, Anzahl Liefergebiete. Ein kleines Dialogfenster fragt nach der "Anzahl der Liefergebiete".)*

An dieser Stelle fasst OTR die Bestimmungsorte anhand der Koordinaten unter Berücksichtigung des Gewichtes zu Liefergebieten (Gruppen) zusammen und es findet bereits die Geolokalisation statt.

Das Feld *Anzahl der Liefergebiete* zeigt Ihnen, in wie viele Gruppen OTR die einzelnen Bestimmungsorte zusammengefasst hat.

Sie können diesen Wert akzeptieren, ihn aber auch überschreiben. Wenn Sie ihn überschreiben, findet im Hintergrund eine neue Berechnung gemäß des neuen Wertes statt.

> **Geolokalisation im dynamischen Modus**
> Wurden alle Adressen erfolgreich lokalisiert, entfällt die Phase Geolokalisation im OTR.

Nachdem Sie die Schaltfläche [OK] angeklickt haben, erscheint der Dialog *Fahrzeug wählen*.

*(Abb. I-5: Dynamischer Modus, Fahrzeug wählen. Ein Dialogfenster mit einer Liste verfügbarer Fahrzeuge und deren Eigenschaften wie Nummernschild, Marke, Modell, maximale Beladung, etc.)*

Dieser Dialog liefert Ihnen einen Überblick zu den einzelnen Fahrzeugen, die im System angelegt sind. Sie können entweder bestimmte Fahrzeuge auswählen (nur eigene LKWs oder auch Speditionen) oder *Alle*. Wählen Sie alle Fahrzeuge aus, bieten Sie dem System die Freiheit, die Aufträge optimal auf die LKWs zu verteilen. Aktivieren Sie die Checkbox *Maximale Beladung und Zeit vor Ort*, dann wird sowohl die maximale Beladung des Fahrzeugs berücksichtigt, die Sie in den Stammdaten hinterlegt haben als auch die beim Kunden hinterlegte Zeit.

Klicken Sie auf [OK], erscheint folgende Anzeige:

*(Abb. I-6: Oberfläche nach dem Start. Die Hauptansicht der Anwendung mit einer Karte auf der linken Seite und Tabellen für Touren und Bestimmungsorte auf der rechten Seite.)*

Mit den oben genannten Eingaben nimmt OTR die entsprechenden Berechnungen vor. Auf der linken Seite sehen Sie die Karte mit den einzelnen Gruppen, die angefahren werden. Rechts oben sehen Sie die Touren und darunter die Bestimmungsorte.

Die Nummer, die in den Feldern *Gruppen* zu sehen ist, ist identisch mit der entsprechenden Nummer auf der Karte (s.o.).

Die Symbol-Schaltfläche **[Liefergebiete]** beinhaltet die Menüeinträge:
*   Hierarchisch
*   EM

Dabei handelt es sich um zwei Berechnungsarten, die zu verschiedenen Ergebnissen führen. Welchen Modus Sie verwenden, hängt davon ab, wie viele Liefergebiete und wie viele Bestimmungsorte angefahren werden.

Um dies zu verdeutlichen, haben wir im Anschluss 94 Bestimmungsorte in unterschiedlich viele Liefergebiete aufgeteilt und das Ergebnis beider Modi abgebildet:

*(Mehrere Kartenbilder, die 94 Bestimmungsorte in Barcelona zeigen. Die Bilder vergleichen die Gruppierung in 3, 4, 6 und 9 Liefergebiete mit dem "Hierarchische Modus" und dem "EM Modus".)*

*   **Werden diese Bestimmungsorte in drei Liefergebiete aufgeteilt, ist das Ergebnis wie folgt:**
    *   A: Hierarchische Modus
    *   B: EM Modus (empfohlen)
*   **Werden diese Bestimmungsorte in vier Liefergebiete aufgeteilt, ist das Ergebnis wie folgt:**
    *   A: Hierarchische Modus
    *   B: EM Modus (empfohlen)
*   **Werden diese Bestimmungsorte in sechs Liefergebiete aufgeteilt, ist das Ergebnis wie folgt:**
    *   A: Hierarchische Modus (empfohlen)
    *   B: EM Modus
*   **Werden diese Bestimmungsorte in neun Liefergebiete aufgeteilt, ist das Ergebnis wie folgt:**
    *   A: Hierarchische Modus (empfohlen)
    *   B: EM Modus

Erfahrungsgemäß liefert der *EM Modus* bei einer geringen Anzahl von Liefergebieten eine effizientere Aufteilung der Bestimmungsorte. Haben Sie jedoch eine große Anzahl von Liefergebieten, dann liefert der *hierarchische Modus* eine effizientere Aufteilung.

Mithilfe der Menüeinträge *Hierarchisch* und *EM* können Sie die Aufteilung jederzeit simulieren und sich dann für das passende Ergebnis entscheiden.

> **Berechnung der Liefergebiete**
> Die Aufteilung in Liefergebiete erfolgt immer unter Berücksichtigung der in den Stammdaten hinterlegten Werte je Fahrzeug.

Das Register *Tour-Informationen* liefert Ihnen einen Überblick zu der LKW-Ladung, den Gewichten und der jeweiligen Tour-Zeit.

Der Fortschritt-Balken in der Spalte *Status* zeigt Ihnen, zu welchem Prozentsatz der LKW beladen ist.

**Nächster Schritt:**
*   Optimierung, Seite 1-88

**Ergänzende Informationen**
⇨ Softwarereferenz, "Bereiche" auf Seite 1-189

---

## Die Oberfläche

Das Modul *OTR* öffnen Sie, indem Sie im Nummernverwalter die Symbol-Schaltfläche **[OTR]** betätigen.

Wenn Sie OTR gestartet haben, stellt sich das Modul wie folgt dar:

*(Abb. I-7: Oberfläche nach dem Start. Eine beschriftete Ansicht der Hauptoberfläche.)*

*   **A**: Menüleiste
*   **B**: Symbolleiste
*   **C**: Prozess-Darstellung
*   **D**: Karte
*   **E**: Kartenwerkzeuge
*   **F**: Übersicht der Touren
*   **G**: Übersicht der Bestimmungsorte
*   **H**: Schaltfläche

Im oberen Bereich befinden sich jeweils von links nach rechts die Menüleiste (A), die Symbolleiste (B) sowie die Darstellung des Gesamtprozesses (C) von der Planung bis zur Datenübertragung und -auswertung. Mittels des Wizards ist es möglich, den Gesamtprozess (Planung, Geolokalisierung, etc.) mit wenigen Eingaben zu durchlaufen.

Über die Symbol-Schaltflächen **[Weiter]** gehen Sie im Prozess einen Schritt weiter. Bitte beachten Sie, dass Sie nur dann weitergehen können, wenn im jeweiligen Prozess-Schritt keine Fehler aufgetreten sind. Beispiel: Im Bereich Geolokalisierung können Sie nur dann einen Schritt weiter gehen, wenn alle Bestimmungsorte lokalisiert werden konnten.

Über die Symbol-Schaltfläche **[Zurück]** gehen Sie im Prozess einen Schritt zurück.

Es werden am Ende des Prozesses die Optimierungsergebnisse angezeigt und Sie können entscheiden, ob Sie die Route und Optimierungsergebnisse so akzeptieren (speichern) oder mit anderen Einstellungen wiederholen, um ein besseres Ergebnis zu erzielen.

Die Karte (D) zeigt Ihnen die zu Bereichen zusammengefassten Bestimmungsorte. Darunter befinden sich die Werkzeuge zum Bearbeiten der Touren auf der Karte (E). Im Bereich der *Touren* (F) befinden sich alle anstehenden Touren und im Bereich der *Bestimmungsorte* (G) werden Ihnen die einzelnen Anfahrpunkte aufgelistet. Die Schaltfläche (H) führt Sie im Prozess jeweils einen Schritt weiter.

Unterhalb der Karte befinden sich folgende Werkzeuge:

### Erläuterung der einzelnen Symbole

Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre Bedeutung.

| Symbol | Erläuterung |
| :--- | :--- |
| (Cursor-Symbol) | **Menü**: Wenn Sie diese Symbol-Schaltfläche aktivieren, können Sie mithilfe der `<Strg>`-Taste einen oder mehrere Bestimmungsorte auswählen. Diese werden dann in Rot angezeigt. Es öffnet sich ein Popup-Menü mit Aktionen, die Sie an dieser Stelle ausführen können. |
| (Pin-Symbol) | **Bestimmungsorte**: Wenn Sie diese Symbol-Schaltfläche aktivieren, bekommen Sie auf der Karte die letzten beiden Ziffern der Tour-ID angezeigt. Ist die Symbol-Schaltfläche nicht aktiv, werden Ihnen die Nummern der Liefergebiete angezeigt. |
| (Linien-Symbol) | **Bereiche**: Mittels dieser Symbol-Schaltfläche werden die außen liegenden Bestimmungsorte durch Linien verbunden. |
| (Kreis-Symbol) | **Bereiche**: Mittels dieser Symbol-Schaltfläche werden die Lieferbereiche kreisförmig dargestellt. |
| (Info-Symbol) | **Informationen**: Mittels dieser Symbol-Schaltfläche blenden Sie Streckeninformationen (Nokia Maps) ein oder aus. |
| (Routen-Symbol) | **Optimierte Tour**: Nach erfolgter Optimierung können Sie die Route mit dieser Symbol-Schaltfläche ein- und ausblenden. |
| (Plus-Symbol) | **Bestimmungsorte**: Mittels dieser Symbol-Schaltfläche blenden Sie die Bestimmungsorte ein oder aus. |
| (Lupe-Symbol) | **Zoom**: Mittels dieser Symbol-Schaltfläche wird die Karte vergrößert. Die Bereiche *Touren* und *Bestimmungsorte* werden ausgeblendet. Ein erneuter Klick auf die Symbol-Schaltfläche blendet die Bereiche wieder ein und verkleinert die Karte. |

Aktivieren Sie die Symbol-Schaltfläche *Menü*, halten Sie die `<Strg>` Taste gedrückt und klicken Sie auf einen Bestimmungsort. Es öffnet sich folgendes Menü:

*(Kontextmenü mit Optionen wie "Vereinigen Liefergebiete - Touren", "Bestimmungsort löschen" und "Bestimmung" (Priorität: Ausgangspunkt, Mittelpunkt, Endpunkt).)*

Mithilfe dieses Menüs können Sie z. B. Liefergebiete zusammenlegen. Dazu halten Sie die `<Strg>`-Taste gedrückt und klicken Sie den Bestimmungsort an, den Sie verschieben möchten. Das Menü öffnet sich und Sie klicken in dem Menü das Liefergebiet an, in das der Bestimmungsort verschoben werden soll. Das Menü schließt sich und der Bestimmungsort befindet sich in dem gewünschten Liefergebiet.

Sie können auch ganz einfach einen Bestimmungsort löschen, indem Sie mit gedrückter `<Strg>`-Taste diesen markieren. Im Menü ist dann dieser Bestimmungsort im Bereich *Bestimmungsort löschen* zu finden. Klicken Sie ihn an, wird er gelöscht.

> **Bestimmungsort löschen**
> Wenn Sie einen Bestimmungsort löschen, wird zum jetzigen Programmstand der Status für diesen Auftrag (Aufträge) im ERP-System nicht geändert. Für die anderen Aufträge hingegen schon (geplant, optimiert, freigegeben, etc.)

Im Bereich *Bestimmung* können Sie dem Bestimmungsort als Priorität kennzeichnen oder ihm einen anderen Punkt zuweisen. Folgende Punkte sind möglich:
*   Ausgangspunkt
*   Mittelpunkt
*   Endpunkt

---

## Die Menü- und Symbolleisten

Die Menüleiste beinhaltet die für den Anwender wichtigsten Funktionen. Die einzelnen Menüs können per Mausklick geöffnet werden. Einige Menüpunkte können mit Hilfe von Tastenkombinationen (Bsp.: `<Strg>+<S>` = Starten) direkt geöffnet werden.

### Bereich Starten

Der Bereich *Starten* beinhaltet folgende Symbol-Schaltflächen:

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (X-Symbol) | Schließen | Mittels dieser Symbol-Schaltfläche schließen Sie das Modul. |
| (Server-Symbol) | Überprüfen Sie den Service | Mittels dieser Symbol-Schaltfläche überprüfen Sie die Verbindung zum Service. |
| (Logbuch-Symbol) | Logbuch | Mittels dieser Symbol-Schaltfläche öffnen Sie das Logbuch, welches die täglichen Ereignisse protokolliert. |
| (Hilfe-Symbol) | Hilfe | Mittels dieser Symbol-Schaltfläche starten Sie die A+W Business-Hilfe. |
| (Info-Symbol) | Über A+W Business | Mittels dieser Symbol-Schaltfläche öffnen Sie den Dialog mit Informationen zu der Version und dem Lizenzschlüssel. |

### Bereich Ansicht

Der Bereich *Ansicht* beinhaltet folgende Einträge, mit denen Sie das Erscheinungsbild von OTR einstellen können (z.B. 2010 Blue, 2007 Silver, etc.).

### Bereich Konfiguration

Der Bereich *Konfiguration* beinhaltet folgende Symbol-Schaltflächen:

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (Einstellungen-Symbol) | Einstellungen | Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die Datenbankeinstellungen. Es öffnet sich der Dialog *Einstellungen*. |
| (Parameter-Symbol) | Parameter | Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die Parameter. Es öffnet sich der Dialog *Parameter*. |
| (Import/Export-Symbol) | Import/Export | Mittels dieser Symbol-Schaltfläche können Sie zu Sicherungszwecken die Parameter im XML-Format exportieren. |
| (Dropdown-Box) | Sprache | Mittels dieser Kombobox wählen Sie die Programm-Sprache für OTR aus. |

### Bereich Administration

Der Bereich *Administration* beinhaltet folgende Symbol-Schaltflächen:

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (Benutzer-Symbol) | Benutzer | Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die Benutzer. Es öffnet sich der Dialog *Benutzer*. |
| (Status-Symbol) | Status | Mittels dieser Symbol-Schaltfläche haben Sie Zugriff auf die Status. Es öffnet sich der Dialog *Status*. |
| (Kunden-Symbol) | Kunden | Mittels dieser Symbol-Schaltfläche können Sie auf die Kunden zugreifen. Es öffnet sich der Dialog *Kunden*. |
| (Abteilungen-Symbol) | Abteilungen | Mittels dieser Symbol-Schaltfläche können Sie auf die Abteilungen zugreifen. Es öffnet sich der Dialog *Abteilungen*. |
| (Fahrzeug-Symbol) | Fahrzeuge | Mittels dieser Symbol-Schaltfläche können Sie auf Ihren Fuhrpark zugreifen. Es öffnet sich der Dialog *Fahrzeuge*. |
| (Fahrer-Symbol) | Fahrer | Mittels dieser Symbol-Schaltfläche können Sie auf Ihre Fahrer zugreifen. Es öffnet sich der Dialog *Fahrer*. |
| (Reports-Symbol) | Reports | Mittels dieser Symbol-Schaltfläche können Sie auf die Reports zugreifen. Es öffnet sich der Dialog *Reports*. |
| (Packmittel-Symbol) | Packmittel-Typen | Mittels dieser Symbol-Schaltfläche können Sie auf die Packmittel zugreifen. Es öffnet sich der Dialog *Packmittel-Typen*. |
| (Datenimport-Symbol) | Datenimport | Mittels dieser Symbol-Schaltfläche können Sie Daten im CSV-Format importieren. Es öffnet sich der Dialog *Datenimport*. |

### Bereich Abfrage

Der Bereich *Abfrage* beinhaltet folgende Symbol-Schaltflächen:

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (Filter-Symbol) | Filtern | Mittels dieser Symbol-Schaltfläche können Sie nach einzelnen Routen filtern. Es öffnet sich der Dialog *Filter Routen*. |
| (Bearbeiten-Symbol) | Tour bearbeiten | Mittels dieser Symbol-Schaltfläche können Sie den Tour-Status und die tatsächlichen Kosten ändern. Es öffnet sich der Dialog *Tour bearbeiten*. |
| (Löschen-Symbol) | Tour löschen | Mittels dieser Symbol-Schaltfläche können Sie eine zuvor ausgewählte Tour löschen. |
| (Export-Symbol) | Tour exportieren | Mittels dieser Symbol-Schaltfläche können Sie die Daten an ein Navigationssystem exportieren. Es öffnet sich der Dialog *Export*. |
| (Statusänderung-Symbol) | Status ändern | Mittels dieser Symbol-Schaltfläche können Sie den Status einer Tour ändern. Es öffnet sich der Dialog *Statusänderung*. |
| (Historie-Symbol) | Historie | Mittels dieser Symbol-Schaltfläche können Sie sich die Dokumenten-Historie anzeigen lassen. Es öffnet sich der Dialog *Historie*. |
| (Report-Symbol) | Ausgewählte Tour | Mittels dieser Symbol-Schaltfläche öffnet sich der Crystal Report Bestätigungs- und Lieferliste für die ausgewählte Tour. |
| (Launcher-Symbol) | Report Launcher | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Report Launcher* für die ausgewählte Tour. |
| (Statistik-Symbol) | Statistik | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Statistik* für die ausgewählte Tour. |
| (Tour-Ansicht-Symbol) | Siehe Tour | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Tour*. |
| (Bestimmungsort-Ansicht-Symbol) | Siehe Bestimmungsort | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Bestimmungsort*. |
| (Kalender-Symbol) | Kalender | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Kalender*. Der Kalender zeigt Ihnen die gefahrenen Touren nach Fahrzeugen und Fahrer. |
| (Admin-Symbol) | Routen Administrator | Dieser Eintrag dient dem Online-Tracking der Touren, die gerade gefahren werden. |
| (Anhang-Symbol) | Dateien anhängen | Mittels dieser Symbol-Schaltfläche können Sie einer Route, einem Bestimmungsort oder Dokument einen Dateipfad zufügen. |

### Die Symbolleiste der Planungs-Phase
Die Symbolleiste der Planungs-Phase beinhaltet den Zugriff auf alle Funktionen bzw. Dialoge, die in dieser Phase von Bedeutung sind.

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (Kopieren-Symbol) | Gespeicherte Tour kopieren | Mittels dieser Symbol-Schaltfläche können Sie eine gespeicherte Tour kopieren. Es öffnet sich der Dialog *Gespeicherte Touren*. |
| (Laden-Symbol) | Gespeicherte Tour laden | Mittels dieser Symbol-Schaltfläche können Sie einer neuen Tour eine gespeicherte Tour hinzufügen. Es öffnet sich der Dialog *Gespeicherte Tour-Liste*. |
| (Import-Symbol) | Bestimmungsorte importieren | Mittels dieser Symbol-Schaltfläche können Sie Bestimmungsorte importieren. Es öffnet sich der Dialog *Datenimport*. |
| (Hinzufügen-Symbol) | Neue Tour | Mittels dieser Symbol-Schaltfläche können Sie eine neue Tour zusammenstellen. Es öffnet sich der Dialog *Tour*. |
| (Bearbeiten-Symbol) | Tour bearbeiten | Mittels dieser Symbol-Schaltfläche können Sie eine zuvor ausgewählte Tour bearbeiten. |
| (Löschen-Symbol) | Tour löschen | Mittels dieser Symbol-Schaltfläche können Sie eine zuvor ausgewählte Tour löschen. |
| (Gruppen-Symbol) | Gruppen | Mittels dieser Symbol-Schaltfläche können Sie die Touren in Bereiche unterteilen. |
| (Fahrzeug-Symbol) | Fahrzeuge | Mittels dieser Symbol-Schaltfläche können Sie der Tour ein anderes Fahrzeug zuweisen. Es öffnet sich der Dialog *Fahrzeug wählen*. |
| (Hinzufügen-Symbol) | Neuer Bestimmungsort | Mittels dieser Symbol-Schaltfläche können Sie einer Tour einen neuen Bestimmungsort hinzufügen. Es öffnet sich der Dialog *Bestimmungsort*. |
| (Bearbeiten-Symbol) | Bestimmungsort bearbeiten | Mittels dieser Symbol-Schaltfläche können Sie einen zuvor ausgewählten Bestimmungsort bearbeiten. Es öffnet sich der Dialog *Bestimmungsort bearbeiten*. |
| (Löschen-Symbol) | Bestimmungsort löschen | Mittels dieser Symbol-Schaltfläche können Sie einen zuvor ausgewählten Bestimmungsort löschen. |
| (Packmittel-Symbol) | Packmittel | Mittels dieser Symbol-Schaltfläche öffnen Sie das Register *Packmittel*. |
| (Detailansicht-Symbol) | Detailansicht | Mittels dieser Symbol-Schaltfläche erhalten Sie eine Detailansicht zu den Bestimmungsorten einer Tour. |
| (Initialisieren-Symbol) | Initialisieren | Mittels dieser Symbol-Schaltfläche kehren Sie zur Ausgangssituation zurück. Haben Sie z. B. Datensätze gruppiert und möchten dies rückgängig machen, dann klicken Sie auf diese Schaltfläche. |

### Die Symbolleiste der Optimierungs-Phase
Die Symbolleiste der Optimierungs-Phase beinhaltet den Zugriff auf alle Funktionen bzw. Dialoge, die in dieser Phase von Bedeutung sind.

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (Optimieren-Symbol) | Tour optimieren | Mittels dieser Symbol-Schaltfläche wird die Route erneut optimiert. |
| (Stopp-Symbol) | Optimierung stoppen | Mittels dieser Symbol-Schaltfläche wird die Optimierung der Route unterbrochen. |
| (Verkehr-Symbol) | Verkehr | Mittels dieser Symbol-Schaltfläche wird die Verkehrslage aufgrund von statistischen Werten (Nokia Maps) ermittelt. |
| (Verkehr-Stopp-Symbol) | Verkehr stoppen | Mittels dieser Symbol-Schaltfläche wird die Ermittlung der Verkehrslage gestoppt. |
| (Bearbeiten-Symbol) | Tour bearbeiten | Mittels dieser Symbol-Schaltfläche können Sie die Eigenschaften der Tour bearbeiten. Es öffnet sich der Dialog *Tour*. |

### Die Symbolleiste der Ergebnis-Phase
Die Symbolleiste der Ergebnis-Phase beinhaltet den Zugriff auf alle Funktionen bzw. Dialoge, die in dieser Phase von Bedeutung sind.

#### Erläuterung der einzelnen Symbole

| Symbol | Name | Erläuterung |
| :--- | :--- | :--- |
| (Report-Symbol) | Ausgewählte Tour | Mittels dieser Symbol-Schaltfläche öffnet sich der Crystal Report Bestätigungs- und Lieferliste für die ausgewählte Tour. |
| (Multi-Report-Symbol) | Alle angezeigten Touren | Mittels dieser Symbol-Schaltfläche öffnet sich der Crystal Report Bestätigungs- und Lieferliste für alle optimierten Touren. |
| (Tour-Ansicht-Symbol) | Siehe Tour | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Tour*. |
| (Bestimmungsort-Ansicht-Symbol) | Siehe Bestimmungsort | Mittels dieser Symbol-Schaltfläche öffnet sich der Dialog *Bestimmungsort*. |
| (Export-Symbol) | Tour exportieren | Mittels dieser Symbol-Schaltfläche können Sie die Daten an ein Navigationssystem exportieren. Es öffnet sich der Dialog *Export*. |
| (Bearbeiten-Symbol) | Tour bearbeiten | Mittels dieser Symbol-Schaltfläche können Sie den Tour-Status und die tatsächlichen Kosten ändern. Es öffnet sich der Dialog *Tour bearbeiten*. |

---

## Feldhilfe
Befindet sich hinter einem Feld die nebenstehende Symbol-Schaltfläche **[Hilfe]**, können Sie den Mauszeiger darauf platzieren und erhalten eine Information zu dem Feld.

*(Abb. I-8: Feldhilfe. Ein Tooltip über dem Feld "Mautkosten" zeigt die Beschreibung: "Geschätzten Mautkosten, die zur Berechnung der Tourkosten herangezogen werden.")*

**Ergänzende Informationen**
⇨ "Die Oberfläche" auf Seite 1-22

---

## Administration

In diesem Themenblock lernen Sie die Stammdaten in OTR kennen.
Dazu gehören folgende Lerneinheiten:
*   "Parameter" auf Seite 1-35
*   "Benutzer" auf Seite 1-37
*   "Status" auf Seite 1-38
*   "Kunden" auf Seite 1-40
*   "Abteilungen" auf Seite 1-43
*   "Fahrzeuge" auf Seite 1-45
*   "Fahrer" auf Seite 1-49
*   "Reports" auf Seite 1-52
*   "Datenimport" auf Seite 1-58

### Parameter

In diesem Bereich nehmen Sie die Standard-Einstellungen zum Arbeiten mit OTR vor.
Die Parameter werden zunächst in zwei Gruppen unterteilt:
*   **Parameter zur Konfiguration der Anwendung**: Diese Parameter dienen der allgemeinen Konfiguration, z. B. Textformat, Einheitensystem, Währung, etc.
*   **Parameter für die Routen**: Auf Basis dieser Werte werden die Routen gebildet und optimiert. Über den Dialog *Route bearbeiten* haben Sie jederzeit die Möglichkeit, auf diese Werte zuzugreifen und temporäre Änderungen durchzuführen.

Eine detaillierte Erläuterung hierzu finden Sie in der Softwarereferenz.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Parameter" auf Seite I-136

---

## Stammdaten

#### Lernziele
*   Die Parameter kennenlernen
*   Den Umgang mit dem Fuhrpark kennenlernen und verstehen
*   Den Umgang mit Benutzern und Abteilungen kennenlernen und verstehen
*   Den Umgang mit den Fahrer kennenlernen und verstehen

#### Nutzen
*   Zum Ermitteln der Tourkosten ist es notwendig, die Fuhrparkdaten möglichst detailliert zu pflegen. Nur so erhalten Sie genaue Werte. Darüber hinaus kann es jederzeit notwendig sein, Ihre Fahrer telefonisch zu kontaktieren. Daher ist es empfehlenswert, die Personendaten auf dem aktuellen Stand zu halten.

#### Definition
*   **Fixkosten**: Kosten, die bei Änderung einer Bezugsgröße (Gesamtstrecke, Kraftstoffkosten) konstant bleiben.

#### Merke
*   **Neue Fahrzeuge anlegen**: Zum Anlegen neuer Fahrzeuge ist es ratsam, die Fahrzeugpapiere zur Hand zu haben.
*   **Wartungstermin**: Sie haben die Möglichkeit, für Ihre Fahrzeuge den nächsten Wartungstermin zu hinterlegen. Das Modul erinnert Sie dann rechtzeitig, dass dieser Termin ansteht.
*   **Fahrer zuweisen**: Sie können einem Fahrzeug einen festen Fahrer zuweisen.
*   **Kosten**: Die Kosten können pro Fahrer nach der Zeit oder der Entfernung hinterlegt werden.
*   **Personal**: OTR unterscheidet eigenes Personal (Mitarbeiter) von fremdem Personal (angemietete Fahrer).

### Benutzer

Dieser Bereich dient dazu, die Profile der Benutzer, die unter Windows oder in einer Domäne registriert sind, zu verwalten. Die Daten werden automatisch generiert, wenn ein Benutzer das Programm (OTR) startet.

*(Abb. I-9: Benutzer. Ein Dialogfenster mit einer Liste der Benutzerprofile (Benutzer-ID, Name) und einem Detailbereich zum Kopieren von Profilen.)*

Die Tabelle oben zeigt Ihnen, welche Profile bereits angelegt sind. Als Administrator können Sie z. B. Benutzer mit einem Standard-Profil (Sprache, Aussehen der Oberfläche, etc.) anlegen, die dann einfach kopiert werden können.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

> **Rechte**
> Zum Editieren muss der Anwender Mitglied der Administratoren-Gruppe sein. Die Anwender werden erfasst, wenn OTR aus dem A+W Business heraus gestartet wird. Ansonsten werden die Anwender vom Betriebssystem erfasst.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Benutzer" auf Seite 1-146

### Status

Je nachdem, in welchem Zustand sich eine Route befindet, hat sie einen entsprechenden Status.

*(Abb. I-10: Status. Ein Dialogfenster zur Verwaltung von Status-Typen. Es zeigt eine Liste von Status (z.B. Erstellt, Geplant, Freigegeben, Tour Problem) mit zugehörigen IDs und der Möglichkeit, sie zu bearbeiten.)*

Die Tabelle oben zeigt Ihnen, welche Status-Typen bereits angelegt sind. Sie können einen neuen Status anlegen oder einen vorhandenen Status ändern. Welcher Status geändert werden kann, zeigt Ihnen das Feld *Editierbar*. Hat der Status dort einen grünen Haken, kann er geändert werden. Alle Status-Typen ohne grünen Haken können nicht geändert werden.

Eine manuelle Änderung des Status kann nötig sein, wenn Sie z. B. eine geplante Tour für den Fahrer manuell freigeben und damit die Daten in die Cloud hochladen wollen.

Die einzelnen Status sind zu Gruppen zusammengefasst. So gibt es z. B. eine Gruppe (650), die sich mit unterschiedlichen Gegebenheiten bezüglich des Bestimmungsortes befasst. Die Gruppe enthält folgende Status:
*   **Bestimmungsort Problem**: Bei diesem Status war es dem LKW z. B. nicht möglich, den Bestimmungsort anzufahren.
*   **Bestimmungsort nicht gefunden**: Hier wurde der Bestimmungsort schlichtweg nicht gefunden.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

#### Die Status-Typen verwalten

In dieser Einheit lernen Sie, wie Sie neue Status-Typen anlegen, bearbeiten oder auch löschen.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
*   "So legen Sie einen neuen Status an"
*   "So löschen Sie einen bestehenden Status"
*   "So nehmen Sie Änderungen an einem bestimmten Status vor"

**So legen Sie einen neuen Status an**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Status]**. Es öffnet sich der Dialog *Status*.
3.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**. Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
4.  Klicken Sie auf die Symbol-Schaltfläche. Es öffnet sich der Dialog *Status Typ*. Wählen Sie aus der Liste den Typ aus, zu dem der Status gehören wird. Klicken Sie auf [OK]. Der Dialog wird geschlossen. Die Informationen werden übernommen.
5.  Das Feld *Status* wird mit der nächst freien Nummer vorbelegt.
6.  Geben Sie im Feld *Statusnamen* den Namen ein.
7.  Ob die Checkboxen *Touren* und *Bestimmungsorte* aktiv oder nicht aktiv sind, richtet sich nach der Gruppe, der sie zugeordnet sind.
8.  Im Feld *Beschreibung* können Sie eine detaillierte Beschreibung zu dem Status hinterlegen.

**So löschen Sie einen bestehenden Status**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Status]**. Es öffnet sich der Dialog *Status*.
3.  Markieren Sie in der Tabelle den Status, das gelöscht werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**. Der Eintrag wird gelöscht.

**So nehmen Sie Änderungen an einem bestimmten Status vor**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Status]**. Es öffnet sich der Dialog *Status*.
3.  Markieren Sie in der Tabelle den Status, der geändert werden soll. Ob ein Status geändert werden kann, sehen Sie in der Tabelle daran, dass im Feld *Editierbar* ein Haken ist.
4.  Betätigen Sie die Symbol-Schaltfläche **[Bearbeiten]**.
5.  Nehmen Sie die gewünschten Änderungen vor.
6.  Betätigen Sie die Symbol-Schaltfläche **[Speichern]**. Die Daten werden gespeichert.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Status" auf Seite 1-147

### Kunden

In OTR haben Sie die Möglichkeit, eigene, zusätzliche Kundendaten (Adressen) zu verwalten. Dies ist hilfreich, um bspw. Adressen für Be- und Entladestationen zu verwalten, ohne dass diese Daten im ERP-System (*A+W Business* Kundenstammdaten) angelegt sein müssen. Diese Eigenschaft aktivieren Sie in den Parametern, indem Sie den Eintrag `USE_CUSTOMERS_OTR` auf den Wert **Ja** setzen.

*(Abb. I-11: Kunden. Ein Dialogfenster zur Verwaltung von Kundendaten mit einer Liste von Kunden und einem Detailbereich mit Feldern wie Kunden-ID, Name, Adresse, Koordinaten, Kontaktinformationen und Zeitfenstern.)*

Ist der Parameter aktiv, prüft OTR während des Imports im Hintergrund, ob der Kunden bereits gespeichert ist. Ist er nicht gespeichert, speichert ihn das Programm und er steht ab sofort zur Verfügung.

#### Die Kunden verwalten

In dieser Einheit lernen Sie, wie Sie neue Kunden anlegen (manuell), bearbeiten oder auch löschen.

**So legen Sie einen neuen Kunden manuell an**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Kunden]**. Es öffnet sich der Dialog *Kunden*.
3.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**. Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
4.  Geben Sie im Feld *Kunden-Nr.* die gewünschte Nummer ein. Hinweis: Jede Nummer darf nur einmal vorkommen.
5.  Geben Sie im Feld *Namen* den Namen des Kunden ein.
6.  Geben Sie im Feld *Telefon* die Telefonnummer des Kunden ein.
7.  Im Feld *Adresse* geben Sie die Kunden-Adresse ein. Bitte achten Sie darauf, den Straßennamen und den Ortsnamen kommasepariert einzugeben.
8.  Sind die Felder *Längen-* und *Breitengrad* nicht gefüllt, klicken Sie auf die Symbol-Schaltfläche **[Geolokalisieren]**.
9.  Im Feld *Zeit (Minuten)* haben Sie die Möglichkeit zu hinterlegen, in welcher Zeitspanne der Fahrer beim Kunden sein soll.
10. Im Feld *Zeitbereich* haben Sie die Möglichkeit zu hinterlegen, von welcher Uhrzeit bis zu welcher Uhrzeit der Fahrer beim Kunden abladen kann.
11. Im Feld *Ansprechpartner* können Sie eine Kontaktperson beim Kunden hinterlegen.
12. Im Feld *E-Mail-Adresse Kontakt* können Sie die E-Mail-Adresse des Kontaktes hinterlegen.

**So löschen Sie einen bestehenden Kunden**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Kunden]**. Es öffnet sich der Dialog *Kunden*.
3.  Markieren Sie in der Tabelle den Kunden, das gelöscht werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**. Der Eintrag wird gelöscht.

**So nehmen Sie Änderungen an einem bestimmten Kunden vor**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Kunden]**. Es öffnet sich der Dialog *Kunden*.
3.  Markieren Sie in der Tabelle den Kunden, der geändert werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Bearbeiten]**.
5.  Nehmen Sie die gewünschten Änderungen vor.
6.  Betätigen Sie die Symbol-Schaltfläche **[Speichern]**. Die Daten werden gespeichert.

**Ergänzende Informationen**
⇨ Softwarereferenz, “Kunden" auf Seite 1-149

### Abteilungen

In diesem Bereich können Sie einzelne Abteilungen hinzufügen, ändern oder löschen. Das dient später einmal statistischen Zwecken. So können Sie z. B. statistische Auswertungen auf Basis von Abteilungen erstellen. Fremdfirmen (Speditionen) die für Sie ausliefern könnten beispielsweise als Abteilung definiert und so erfasst werden.

*(Abb. I-12: Abteilungen. Ein Dialogfenster zur Verwaltung von Abteilungen, das eine Liste bestehender Abteilungen (z.B. EXPEDITION, SUPPORT) und einen Detailbereich zur Bearbeitung zeigt.)*

Die Tabelle oben zeigt Ihnen, welche Abteilungen bereits angelegt sind.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

#### Die Abteilungen verwalten
In dieser Einheit lernen Sie, wie Sie neue Abteilungen anlegen, bearbeiten oder auch löschen.

**So legen Sie eine neue Abteilung an**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Abteilungen]**. Es öffnet sich der Dialog *Abteilungen*.
3.  Geben Sie im Feld *Abteilung* die Nummer der Abteilung ein, z. B. **5318**.
4.  Geben Sie im Feld *Namen* den Namen der Abteilung ein, z. B. **Versand**.
5.  Im Feld *Beschreibung* können Sie eine Beschreibung zur Abteilung hinterlegen.

**So löschen Sie eine bestehende Abteilung**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Abteilungen]**. Es öffnet sich der Dialog *Abteilungen*.
3.  Markieren Sie in der Tabelle die Abteilung, die gelöscht werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**. Der Eintrag wird gelöscht.

**So nehmen Sie Änderungen an einer bestimmten Abteilung vor**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Abteilungen]**. Es öffnet sich der Dialog *Abteilungen*.
3.  Markieren Sie in der Tabelle die Abteilung, die geändert werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Bearbeiten]**.
5.  Nehmen Sie die gewünschten Änderungen vor.
6.  Betätigen Sie die Symbol-Schaltfläche **[Speichern]**. Die Daten werden gespeichert.

**Ergänzende Informationen**
⇨ Softwarereferenz, “Abteilungen" auf Seite 1-151

### Fahrzeuge

In diesem Bereich sind alle Fahrzeuge zu finden, die zur Auslieferung von Ware zur Verfügung stehen. Das können sein:
*   LKW
*   Auto
*   Anhänger

*(Abb. I-13: Fahrzeuge. Ein umfassendes Dialogfenster zur Verwaltung von Fahrzeugen. Es enthält eine Liste von Fahrzeugen und einen detaillierten Bereich mit zahlreichen Feldern wie Nummernschild, Marke, Modell, Maße, Gewicht, Kosten, Fahrerzuweisung, etc.)*

Die Tabelle oben zeigt Ihnen, welche Fahrzeuge bereits angelegt sind. Sie können neue Fahrzeuge anlegen, aber auch Änderungen an bereits angelegten Fahrzeugen vornehmen.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

> **Fahrzeugdaten**
> Zum Anlegen neuer Fahrzeuge ist es ratsam, die Fahrzeugpapiere (Fahrzeugschein und/oder Fahrzeugbrief) zur Hand zu haben. Es werden Daten abgefragt, die in diesen Papieren zu finden sind, wie z. B. Leergewicht.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Fahrzeuge" auf Seite 1-152

#### Die Fahrzeuge verwalten

In dieser Einheit lernen Sie, wie Sie neue Fahrzeuge anlegen, bearbeiten oder auch löschen.

**So legen Sie ein neues Fahrzeug an**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Fahrzeuge]**. Es öffnet sich der Dialog *Fahrzeuge*.
3.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**. Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
4.  Erfassen Sie die Felder *Nummernschild*, *Marke*, *Modell* und *Fahrgestell-Nummer* auf Grund der Angaben in den Fahrzeugpapieren.
5.  Erfassen Sie das Feld *Kaufdatum*.
6.  Im Feld *Nächste Wartung* können Sie das Datum für die nächste Wartung eingeben. In den Parametern gibt es den Eintrag *Nächster Wartungstermin für Fahrzeuge*. Steht dieser Eintrag auf **Ja**, dann wird dieses Feld hier entsprechend ausgewertet.
7.  Im Feld *Abteilung* können Sie dem Fahrzeug eine Abteilung fest zuordnen. Dies dient später statistischen Auswertungen. Über die Symbol-Schaltfläche öffnen Sie den Dialog *Abteilung auswählen*.
8.  Erfassen Sie die Felder *Maximale Breite*, *Maximale Höhe*, *Maximale Länge*, *Maximale Beladung* und *Leergewicht* auf Grund der Angaben in den Fahrzeugpapieren.
9.  Im Feld *Verbrauch* geben Sie den durchschnittlichen Kraftstoff-Verbrauch des Fahrzeugs in Litern ein, z. B. **18,5**.
10. Im Feld *Kraftstoffkosten* geben Sie die durchschnittlichen Kosten für einen Liter Kraftstoff ein, z. B. **1,43**. Die entsprechende Währungseinheit können Sie in den Parametern hinterlegen.
11. Im Feld *Fixkosten* geben Sie die durchschnittlichen Kosten für einen Liter Kraftstoff ein, z. B. **1,43**. Die entsprechende Währungseinheit können Sie in den Parametern hinterlegen.
12. Aus der Kombobox *Fortbewegungstyp* wählen Sie den Fahrzeug-Typ aus.
13. Die Felder *Fahrer ID*, *Name* und *Nachname* stehen in Verbindung mit der Symbol-Schaltfläche **[Fahrer hinzufügen]**. Wenn Sie die Schaltfläche betätigen, öffnet sich der Dialog *Fahrer*. Aus diesem Dialog können Sie einen Fahrer auswählen.
14. Die im Feld *Touren* aufgeführten Tournummern werden durch *A+W Business* übergeben und dienen dazu, LKWs bestimmten Tournummern zuzuordnen.
15. Das Feld *Reihenfolge* steht in Zusammenhang mit dem Feld *Touren*. Ist für zwei oder mehrere LKWs die gleiche Tournummer erlaubt, dann können Sie über dieses Feld die Reihenfolge (Priorität) der LKWs bestimmen. Das Feld wird nur ausgewertet, wenn in den Parametern der Eintrag `ROUTE_ORIGIN` den Wert **Ja** hat.
16. Über die Checkbox *Fahrzeug verfügbar* steuern Sie, ob das Fahrzeug generell und für alle Touren zur Verfügung steht.
17. Sollte Ihr Fahrzeug über eine Anhängevorrichtung verfügen, aktivieren Sie die Checkbox *LKW mit Anhänger*.

**So löschen Sie ein bestehendes Fahrzeug**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Fahrzeuge]**. Es öffnet sich der Dialog *Fahrzeuge*.
3.  Markieren Sie in der Tabelle das Fahrzeug, das gelöscht werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Löschen]**. Der Eintrag wird gelöscht.

**So nehmen Sie Änderungen an einem bestimmten Fahrzeug vor**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Fahrzeuge]**. Es öffnet sich der Dialog *Fahrzeuge*.
3.  Markieren Sie in der Tabelle das Fahrzeug, das geändert werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Bearbeiten]**.
5.  Nehmen Sie die gewünschten Änderungen vor.
6.  Betätigen Sie die Symbol-Schaltfläche **[Speichern]**. Die Daten werden gespeichert.

**So weisen Sie einem Fahrzeug einen festen Fahrer zu**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Fahrzeuge]**. Es öffnet sich der Dialog *Fahrzeuge*.
3.  Markieren Sie in der Tabelle das Fahrzeug, dem ein Fahrer zugewiesen werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Bearbeiten]**.
5.  Betätigen Sie die Symbol-Schaltfläche **[Fahrer hinzufügen]**. Es öffnet sich der Dialog *Fahrer*.
6.  Wählen Sie den gewünschten Fahrer aus.
7.  Betätigen Sie die Symbol-Schaltfläche **[OK]**. Der Dialog wird geschlossen.
8.  Betätigen Sie die Symbol-Schaltfläche **[Speichern]**. Die Daten werden gespeichert.

**So entfernen Sie einen fest zugewiesenen Fahrer**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Fahrzeuge]**. Es öffnet sich der Dialog *Fahrzeuge*.
3.  Markieren Sie in der Tabelle das Fahrzeug, von dem der Fahrer entfernt werden soll.
4.  Betätigen Sie die Symbol-Schaltfläche **[Bearbeiten]**.
5.  Betätigen Sie die Symbol-Schaltfläche **[Fahrer löschen]**. Der Fahrer wird gelöscht.
6.  Betätigen Sie die Symbol-Schaltfläche **[Speichern]**. Die Daten werden gespeichert.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Fahrzeuge" auf Seite 1-152
⇨ Softwarereferenz, "Fahrer" auf Seite 1-155

### Fahrer

In diesem Bereich können Sie die Daten zu Ihren Fahrern verwalten. Es sind alle Fahrer zu finden, die zur Auslieferung von Ware zur Verfügung stehen. Das können sein:
*   Angestellte Fahrer
*   Fahrer anderer Unternehmen (angemietete Fahrer)

*(Abb. I-14: Fahrer. Ein Dialogfenster zur Verwaltung von Fahrern mit einer Liste und einem Detailbereich für Stammdaten wie ID, Name, Kontaktdaten, Kosten und Abteilung.)*

Die Tabelle oben zeigt Ihnen, welche Fahrer bereits angelegt sind. Sie können neue Fahrer anlegen, aber auch Änderungen an bereits angelegten Fahrern vornehmen.

Eine detaillierte Erläuterung der einzelnen Felder finden Sie in der Softwarereferenz.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Fahrer" auf Seite 1-155

#### Die Fahrer verwalten

In dieser Einheit lernen Sie, wie Sie neue Fahrer anlegen, bearbeiten oder auch löschen.

**So legen Sie einen neuen Fahrer an**
1.  Gehen Sie in der Menü-Leiste auf den Eintrag *Administration*.
2.  Betätigen Sie die Symbol-Schaltfläche **[Fahrer]**. Es öffnet sich der Dialog *Fahrer*.
3.  Betätigen Sie die Symbol-Schaltfläche **[Neu]**. Der untere Teil des Dialogs wird zur Bearbeitung freigegeben.
4.  Im Feld *Fahrer ID* geben Sie eine Kurzbezeichnung für den Fahrer ein.
5.  Erfassen Sie die Felder *Name*, *Nachname* und *Nachname 2*.
6.  Im Feld *Steuer ID* geben Sie die Steuernummer des Mitarbeiters ein.
7.  Im Feld *E-Mail* können Sie die E-Mail-Adresse des Mitarbeiters hinterlegen.
8.  Im Feld *Kosten* können Sie für den Mitarbeiter einen Betrag hinterlegen, den dieser als Kosten auf der Tour verursacht. Es werden Kosten *Nach Zeit* und *Nach Entfernung* unterschieden. Aktivieren Sie die entsprechende Radiotaste.
9.  Erfassen Sie im Feld *Adresse* die Adresse des Mitarbeiters und in den Feldern *Telefon* und *Telefon 2* die entsprechenden Telefonnummern.
10. Im Feld *Ansprechpartner* können Sie den Namen einer Kontaktperson hinterlegen, falls der Fahrer nicht in Ihrem Unternehmen angestellt ist (z.B. Fahrer einer Spedition).
11. Im Feld *Kontakt-Adresse* geben Sie die Adresse Ihres Kontaktes an.
12. Im Feld *Telefon-Kontakt* geben Sie die entsprechende Telefonnummer an.
13. Im Feld *Beschreibung* können Sie eine Beschreibung zu dem Fahrer oder dem Kontakt hinterlegen und im Feld *E-Mail-Adresse Kontakt* die entsprechende E-Mail-Adresse.
14. Im Feld *Abteilung* können Sie dem Fahrer eine Abteilung fest zuordnen. Über die Symbol-Schaltfläche öffnen Sie den Dialog *Abteilung auswählen*.

