---
description: "DE_AWBusiness_Kistenmanagement_1_1"
---


# A+W Kistenmanagement

**A+W Business**

**A+W - Software for Glass, Windows and Doors**

---

---
## Vorspann

*1.10/12-2019*

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 1.10/012-2019 | Aktualisierung der Einstellungen in den Stammdaten. Übernahme der Kistenbestellungen aus dem Part Einkauf und der Lagerabbuchungen aus dem Part Fertigung. |
| 1.00/012-2018 | Ersterstellung Kistenmanagement: Ausgliederung aus den Parts Lager, Einkauf und Fertigung. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

#### Urheberrechte

© 2020, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte

**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim

- **Tel:** +49 6404 2051 0
- **Fax:** +49 6404 2051 877
- **Email:** aw.zentrale@a-w.com
- **Web:** http://www.a-w.com

---

## Inhalt

- **Vorspann** (K-3)
  - Revisionsübersicht (K-3)
  - Editorial (K-3)
- **Tutorial** (K-7)
  - Übersicht (K-9)
    - Dokumentation (K-10)
    - Menü-Übersicht (K-11)
  - Grundgedanken zum Lager (K-12)
    - Lagermaße (K-13)
    - Lagerverwaltung (K-14)
  - Grundeinstellungen (K-16)
    - Preise (K-16)
    - Firmendaten (K-18)
    - Statusänderungen durch Zu- und Abgänge (K-21)
    - Lagerkategorien (K-22)
  - Stammdaten für Kisten (K-23)
    - Kistendaten (K-24)
      - Lagermaß für Kiste anlegen (K-25)
      - Lagerartikel für Kiste anlegen (K-26)
    - Kiste mit Stückliste (K-29)
      - Stammdaten für Kisten mit Stückliste (K-30)
      - Stücklisten-Kiste in der Lagerverwaltung (K-35)
      - Stücklisten-Kiste in der Positionserfassung (K-36)
  - Aufträge (K-37)
    - Verkaufsauftrag mit Kiste (K-38)
    - Produktionsaufträge (K-42)
      - Einstellungen in der Lieferantenkartei (K-43)
      - Produktionsauftrag erfassen (K-45)
  - Lagerverwaltung für Kisten (K-49)
    - Lagerverwaltung von Kisten (K-49)
    - Lagerbestellung von Kisten (K-50)
    - Wareneingang per Barcode (K-55)
    - Warenausgang Kisten (K-56)
      - Ausbuchung von Kisten (K-56)
      - Warenausgang buchen (K-59)
    - Manuelle Lagerbuchungen (K-61)
      - Zugang manuell erfassen (K-61)
      - Lagerort einer Kiste ändern (K-65)
      - Kisteninhalt korrigieren (Blattanzahl) (K-66)
      - Kisten aufbrechen (auflösen) (K-67)
- **Softwarereferenz** (K-69)
  - Übersicht (K-71)
  - Lagerverwaltung (K-72)
    - Menüs in der Lagerverwaltung (K-72)
      - Menü Funktionen (K-72)
      - Menü Optionen (K-73)
    - Lagerverwaltung (K-73)
      - Lagerverwaltung - Lagerartikel (K-74)
      - Lagerverwaltung – Preise (K-78)
      - Lagerverwaltung - Zusatz (K-81)
  - Lagerbewegung (K-83)
    - Menü Optionen (K-83)
    - Lagerbewegung (K-83)
      - Lagerbewegung - Abgang, Zugang (K-84)
      - Lagerbewegung - Umbuchung (K-86)
      - Lagerbewegung – Blattanzahl (K-87)
      - Lagerbewegung - Aufbruch (K-88)
    - Bemerkung (Lagerbewegung) (K-89)
  - Suche (K-90)
    - Lagersuche - Lagersuche (K-91)
    - Lagersuche - Zukünftiger Lagerbestand (K-94)
  - Lagerbestellung (K-96)
    - Menüs im Bestellpool (K-96)
      - Menü Funktionen (K-96)
      - Menü Optionen (K-97)
    - Bestellpool (K-99)
  - Kisten - Ein- und Ausgang (K-102)
    - Wareneingang (Kisten) (K-102)
      - Wareneingang - Auswahl (K-103)
      - Wareneingang - Komplett (K-105)
      - Wareneingang - Positionsweise (K-107)
      - Wareneingang – Identnummer (K-110)
      - Wareneingang - Protokoll (Identnummern) (K-112)
    - Einstellungen (ID) (K-113)
    - Warenausgang Kisten (K-114)
- **Partindex** (K-115)
- **Index** (K-117)

---

## Tutorial

### Übersicht

Das Tutorial zum Kistenmanagement beschäftigt sich mit den Einstellungen zur Erfassung und Buchung von Kisten mit zugeschnittenen Gläsern.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
- Grundgedanken zum Lager
- Grundeinstellungen
- Stammdaten für Kisten
- Aufträge
- Lagerverwaltung für Kisten

#### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Business mit Kisten arbeiten. Die Teilnehmer müssen das Konzept der Stammdaten und der Lagerverwaltung, den Verkauf und den Einkauf in A+W Business kennen.

### Dokumentation

Für das Kistenmanagement stehen folgende Dokumente zur Verfügung:

| Format | Umfang |
| :--- | :--- |
| PDF | Vollständige Unterlagen<br>- Tutorial<br>- Softwarereferenz |
| Online-Hilfe `<F1>` | Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenz und Tutorials. |

Ergänzende Beschreibungen finden Sie in den Parts Lager, Einkauf und Fertigung, die jeweils auch über die Online-Hilfe zur Verfügung stehen.

#### Aufbau des Tutorials

Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick:** Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte.
- **Konzepte:** Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert.
- **Handlungsanleitung:** Die Handlungsanleitungen sind als Beispiele gedacht, um den Ablauf zu zeigen. Die darin dargestellten Bezeichnungen sind frei erfunden.

#### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

- ***Kursiv***: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Lagerinfo*.
- **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
- **`>`**: Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. `Stammdaten > Produkt > Artikel > Lagermaße`.
- **`[]`**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit `[OK]` speichern Sie die Daten.
- **`<>`**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe.

### Menü-Übersicht

In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, in denen Sie die Dialoge finden, die in dieser Dokumentation gezeigt werden.

**Abb. K-1: Menü für Kistenmanagement**

#### Stammdaten
- **Produkte > Artikel > Lagermaße:** In diesem Dialog erfassen Sie die Kisten mit unterschiedlichen Preisschlüsseln.

#### Lagerwirtschaft
- **Lagerverwaltung:** In diesem Dialog erfassen und pflegen Sie die Daten für Lagerartikel.
- **Lagerbewegung:** In diesem Dialog buchen Sie Warenzugänge und Warenabgänge, Änderungen von Lagerorten und den Aufbruch von Kisten.
- **Suche:** In diesem Dialog prüfen Sie die Verfügbarkeit von Produkten in einem bestimmten Zeitraum.

#### Fertigung
- **Warenausgang Kisten:** In diesem Dialog erfassen Sie den Warenausgang von Kisten, die einem Auftrag zugeordnet sind.

#### Dokumente
- **Wareneingang:** In diesem Dialog erfassen Sie die Kisten, die in den Bestand aufgenommen werden sollen.

### Grundgedanken zum Lager

Im Modul *Lagerwirtschaft* von A+W Business können Sie Bandmaße, Lagermaße, Restblätter, Kisten, Ganzglastüren, Beschläge, Rahmenteile und Zubehör wie Spiegelaufhängungen, Dichtungsbänder usw. verwalten.
Eine ausführliche Beschreibung zum Lager finden Sie im Part *Lagerwirtschaft*. Daraus werden die wichtigsten Stichpunkte für das Kistenmanagement hier nur kurz zusammengefasst.

#### Lagerführung

Bevor Sie Ihr Lager in A+W Business einrichten, müssen Sie entscheiden, auf welcher Basis die Bestände geführt werden sollen: als Fläche (qm) oder in Stückzahlen. Als dritte Möglichkeit steht die kombinierte Lagerführung zur Verfügung, wobei der maßabhängige Lagermodus mit den Rückmeldungen aus der Optimierung kombiniert wird, so dass neben den Lagermaßen auch die zugeschnittenen Bandmaße automatisch ausgebucht werden können.
Nach der Entscheidung zum Modus ordnen Sie das entsprechende Lagerkennzeichen pro Glasprodukt zu und legen in den Firmendaten den Lagerführungsmodus fest.

#### Lagerführungsmodus und Reservierung

Wenn im (Produktions-)Auftrag ein Produkt mit der Beschaffungsart Lagerentnahme erfasst wird, wird die entsprechende Menge (plus Verschnitt bei Festmaßen) des Lagerartikels als reserviert gekennzeichnet. Die Reservierung kann wahlweise manuell aus dem aktuellen Bestand ausgebucht werden oder automatisch, wenn der Lieferschein oder die Rechnung gedruckt wird.
Die Einstellungen werden in der Anzeige von Bestandsmengen im Dialog *Lagerinfo* (Lagervorschau) und bei den automatischen Bestellvorschlägen sichtbar, die beim Erreichen von Mindestmengen angestoßen werden können.

#### Verbrauch von Stücklisten in Produktionsaufträgen

Bei Produktionsaufträgen kann der Verbrauch von Stücklistenelementen im Lager verbucht werden. Kisten haben dann eine Stückliste, wenn z. B. Bilderrahmen-Gläser in Papier verpackt sind und diese Papierverpackungen auf einer Palette stellen.

> **Beispiel**
> In einem Produktionsauftrag wird ein VSG mit 2 x Float 3 erfasst. Nach der Fertigmeldung des Produktionsauftrages wird das VSG auf das Lager gebucht, das Float 3 wird vom Lager abgebucht.
> Wenn für das gleiche VSG ein normaler Kundenauftrag erfasst wird, wird nur das VSG vom Lager abgebucht. Das Float 3 hat keine Lagerführung, da es bereits durch den Produktionsauftrag vom Lager gebucht worden ist.

#### Lieferantenkartei

Wenn eine Kiste mit den identischen Maßen auch eingekauft wird, müssen Sie den Lieferanten in der Lieferantenkartei eintragen. Über die Warengruppe, die der Kiste in den Lagermaßen zugeordnet ist, wird der Lieferant gefunden.

#### Lagermaße

Das Lagermaß Kiste ist für Lagerbuchungen zwingend erforderlich. Für die Erfassung einer Kiste als Auftrags- oder Bestellposition muss daher ein Lagerartikel/-maß Kiste angelegt sein.
Wenn Sie ein Lagermaß in den Stammdaten angelegt haben, bietet A+W Business die Möglichkeit, sofort in die Lagerverwaltung zu wechseln.

**Abb. K-2: Lagermaße (Produktverwaltung) und zugehörige Lagerartikel**
- **A**: Produktverwaltung Lagermaße (Stammdaten)
- **B**: Produktnummer, zu der die Lagermaße gehören
- **C**: Lagermaße mit verschiedenen Abmessungen
- **D**: Lagerartikel zu den Lagermaßen (Lagerverwaltung)
- **E**: Zuordnung der Preistabellen
- **F**: Ermittlung des EK im Lager

Jedem Lagermaß kann eine eigene Preistabelle zugeordnet werden.
Wenn Sie mit dem Lagerkennzeichen maßabhängig arbeiten, müssen Sie für alle Lagermaße auch Lagerartikel angelegen.

#### Lagerverwaltung

Zu jedem (Glas-)Produkt gehören auch ein Lagermaß und ein Lagerartikel. Jeder Lagerartikel kann in verschiedenen Ausprägungen angelegt werden, z. B. Float 5 mm in mehreren Abmessungen.

**Abb. K-3: Definition des Lagerartikels**
- **A**: Produktnummer
- **B**: Maße des Lagerartikels
- **C**: Standard-Lagerort
- **D**: Lagerkategorie
- **E**: Kennzeichen Lager-Hauptartikel
- **F**: Bestandsprüfung für Lagervorschau
- **G**: Definierte Lagerartikel
- **H**: Hauptartikel
- **I**: Blattzahl bei Kisten
- **J**: Lagerort (4 Ebenen)

In den Lagermaßen (Stammdaten) kann für jedes Produkt eine Kiste mit der Beschaffungsart Lagerentnahme angelegt werden, z. B. pro Abmessung eine Kiste.
Wenn es Kisten mit gleichen Maßen aber unterschiedlicher Blattanzahl (I) gibt, so muss auch dafür jeweils ein eigener Lagerartikel angelegt werden. Um den Kisten-Artikel exakt zu bestimmen, werden u. a. Breite und Höhe und die Blattanzahl ausgewertet, um den Mindestbestand zu bestimmen.
Für jede Ausprägung einer Kiste wird also ein Lagerartikel benötigt, in dem die Produktnummer, die Abmessung und die Blattanzahl hinterlegt sind.

Sie können in der Lagerverwaltung mehrere Lagermaße miteinander verknüpfen, indem Sie einen Lager-Hauptartikel (H) angeben. Die Bestandsprüfung im Dialog *Lagerinfo* wird dann nur für den Lager-Hauptartikel durchgeführt und nur für diesen müssen Sie einen Mindestbestand hinterlegen.
Wenn die Bestände nicht pro Lagerort (F) geprüft werden, muss ein Hauptartikel (E, H) zugeordnet werden, um die verfügbaren Quadratmeter des Glases zu ermitteln.

### Grundeinstellungen

Neben den Produkten und den Lagerartikeln müssen weitere Einstellungen festgelegt werden, damit die Kisten korrekt verwaltet werden können.
In diesem Kapitel finden Sie Informationen folgenden Grundeinstellungen:
- "Preise" auf Seite K-16
- "Firmendaten" auf Seite K-18
- "Statusänderungen durch Zu- und Abgänge" auf Seite K-21
- "Lagerkategorien" auf Seite K-22

#### Preise

Über die Preislisten für Kisten werden die Preise im Einkauf und im Verkauf berechnet, z. B. auch, wenn einzelne Blätter einer Kiste verkauft werden.
Wenn Sie das Glas in Kisten mit anderen Preisen berechnen wollen, müssen Sie eine entsprechende Preisliste für den Verkauf und den Einkauf anlegen. Wenn Sie außerdem unterschiedliche Glaspreise je nach Stückzahl verwenden wollen, sind dafür ebenfalls zusätzliche Preislisten erforderlich.
Die Preise sind ausführlich im Part *Stammdaten* beschrieben.

**Abb. K-4: Beispiel Kistenpreise**
- **A**: Preisschlüssel für Kisten
- **B**: Preis pro Preisschlüssel

> **Beispiel Kistenpreise**
> In diesem Beispiel sehen Sie, dass der Preis für die Gläser einer Kiste unterschiedlich berechnet werden, z. B. für die komplette Kiste oder für ein einzelnes Blatt aus der Kiste.
> Damit der Durchschnitts-EK ermittelt werden kann, müssen folgende Bedingungen erfüllt sein:
> - Das Produkt muss auch als Lagerartikel angelegt sein.
> - Das Kennzeichen für den EK muss in den Firmendaten gesetzt sein.

#### Preislisten prüfen

**So prüfen Sie die Stammdaten Ihrer Preislisten**
1. Wählen Sie im Menü `Stammdaten > Preise` und prüfen Sie die Einstellungen in den Dialogen *Jahrgang*, *Schlüssel* und *Tarif*. Sie brauchen nur die Einträge zu prüfen, die für Preise (und sonstige Eigenkalkulationen) für Lagermaße und Kisten verwendet werden.
2. Wählen Sie im Menü `Stammdaten > Preise > Preise`.
   
   **Abb. K-5: EK-Preistabellen**
   (⇨ Stammdaten, "Preise" auf Seite B-714)

3. Prüfen Sie, ob alle EK- und VK-Preise definiert und auf dem aktuellen Stand sind, und ergänzen oder korrigieren Sie diese ggf.
4. Wechseln Sie zu dem Register, in dem der Preis definiert ist, und prüfen Sie, ob der EK-Preis korrekt eingetragen ist, oder korrigieren Sie diesen ggf.
   
   **Abb. K-6: Definierte Einkaufspreise**

5. Wählen Sie im Menü `Start > Speichern`, um die Änderungen zu speichern. Die Daten werden gespeichert.

#### Firmendaten

In den Firmendaten werden die Einstellungen zum Wareneingang von Kisten und zum Lagerzugang durch Produktionsaufträge festgelegt. Diese Einstellungen sind im Part *Lagerwirtschaft* ausführlich beschrieben.

**Einstellungen für Kisten prüfen**
1. Wählen Sie im Menü `Stammdaten > Firma > Firmendaten`. (⇨ Stammdaten, "Firmendaten" auf Seite B-918)
2. Wechseln Sie zum Register *Parameter* und prüfen Sie die Einstellungen für die virtuellen Positionsnummern.
   
   **Abb. K-7: Firmendaten - Parameter**
   - **A**: Virtuelle Positionsnummern für den Wareneingang von Kisten
   
   Die virtuelle Positionsnummer wird benötigt, damit der Wareneingang von Kistenpositionen mit einer Stückzahl > 1 korrekt verbucht werden kann.

3. Wechseln Sie zum Register *Lager / EK / EDI*.

Den Lagerzugang aus einem Produktionsauftrag können Sie auf zwei Arten erfassen:
- Sobald durch eine Produktionsrückmeldung der Status des Produktionsauftrages über diesen Status hinaus steigt, wird der Lagerzugang automatisch verbucht.
- Wenn Sie nicht mit Produktionsrückmeldungen arbeiten, können Sie den Zugang über die manuelle Statusmeldung im Modul *Fertigung* erfassen. Wenn Sie den Produktionsauftrag dort auf einen Status setzen, der über dem o. g. Grenzstatus liegt, werden der Lagerabgang der verbrauchten Materialien und der Lagerzugang der gefertigten Lagerartikel automatisch gebucht.

Wenn kein abweichender Lagerort definiert ist, werden die Auftragsmengen dem Standard-Lagerort zugeordnet.

**Abb. K-8: Firmendaten – Lager / EK / EDI**
- **A**: Einstellungen zur Ermittlung des Einkaufspreises
- **B**: Einstellung zur Aktualisierung des Lagerbestands
- **C**: Identnummern löschen
- **D**: Lagerbuchungen für Produktionsaufträge
- **E**: Anzahl der Vorschautage für den Dialog Lagerinfo
- **F**: Grenzstatus für die Erfassungsstellen (für Produktionsaufträge)

4. Wählen Sie die Einstellungen für Lagerbestellungen (A) aus. Für die Kisten ist nur wichtig, wie der Einkaufspreis ermittelt werden soll. Die Einstellungen zur Ermittlung des Einkaufspreises sind im Part *Stammdaten* beschrieben. Alle anderen Einstellungen in diesem Bereich sind ausführlich im Part *Lagerwirtschaft* beschrieben.
5. Wählen Sie im Bereich *Lagerführungsmodus* (B) die Funktionen aus, die bei der Aktualisierung des Lagerbestands berücksichtigt werden sollen.
   - **Reservierung ohne Bestandsaktualisierung:** Aktivieren Sie diese Option, wenn reservierte Mengen nicht aus dem aktuellen Bestand ausgebucht werden sollen. Die Abbuchungen müssen Sie dann zum gegebenen Zeitpunkt manuell durchführen. Bei der Auftragserfassung wird der aktuelle Bestand daher nicht angezeigt.
   - **Reservierung mit Bestandsaktualisierung:** Diese Option ist standardmäßig aktiviert, damit reservierte Mengen mit dem Druck des Lieferscheins bzw. der Rechnung aus dem aktuellen Bestand ausgebucht werden.
   - **Lagerführung auf Stücklistenebene:** Aktivieren Sie diese Checkbox, wenn Produkte im Lager auch dann geführt werden sollen, wenn sie Bestandteile einer Stückliste sind.
   - **Lagerabbuchung vor Formulardruck durchführen:** Aktivieren Sie diese Checkbox, wenn Lagerartikel abgebucht werden sollen, bevor der Formulardruck ausgeführt wird. Falls bei der Lagerabbuchung ein Problem auftritt, wird der Auftrag aus den zu druckenden Dokumenten entfernt, also nicht gedruckt.
   - **Artikel mit Identnummer löschen wenn kein Bestand (C):** Kisten mit dem Bestand = 0 sind nicht mehr im Lager vorhanden. Aktivieren Sie diese Checkbox, wenn in der Lagerverwaltung die Kisten mit Identnummer aus der Übersicht gelöscht werden sollen, für die kein Bestand angezeigt wird.
   - **Verbrauch von Stücklisten in Produktionsaufträgen (D):** Wenn Sie mit Produktionsaufträgen arbeiten, können Sie festlegen, ob der Verbrauch von Stücklistenelementen automatisch im Lager abgebucht wird.
6. Tragen Sie die Anzahl der Werktage (E) ein. Die Anzahl der Werktage wird für die Vorschau im Dialog *Lagerinfo* ausgewertet. Sie gibt an, über welchen Zeitraum in die Zukunft die zukünftigen Lagerbestände angezeigt werden.
7. Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern. Die Daten werden gespeichert. Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

> **Statuszuordnung für Lagerabbuchung**
> Wenn Sie die Option *Lagerabbuchung vor Formulardruck durchführen* aktiviert haben, sollten Sie die Statuszuordnung für die Lagerabbuchung prüfen. Die Mindest-, Vergabe- und Sperrstatus müssen so organisiert sein, dass die Lagerabbuchung vor dem Druck ausgeführt werden kann. Wenn die Statuszuordnung die Umkehrung der Reihenfolge nicht zulässt, wird unter Umständen die Lagerabbuchung nicht durchgeführt.

#### Statusänderungen durch Zu- und Abgänge

Warenab- und Warenzugänge können den Status von Dokumenten verändern und mit der Statusveränderung zu Bestandsänderungen im Lager führen. Wenn die Statuspunkte und Statuszuordnungen entsprechend definiert sind, gilt dies auch für Teillieferungen.

Wenn Sie in den Firmendaten die Option *Lagerabbuchung vor Formulardruck durchführen* aktiviert haben, müssen der Mindest-, Vergabe- und Sperrstatus so organisiert sein, dass die Lagerabbuchung vor dem Druck ausgeführt werden kann. Wenn die Statuszuordnung die Umkehrung der Reihenfolge nicht zulässt, wird unter Umständen die Lagerabbuchung nicht durchgeführt.

**Statuszuordnungen prüfen**
Eine ausführliche Beschreibung finden Sie im Part *Lagerwirtschaft*.

**So prüfen Sie die Statusverwaltung**
1. Wählen Sie im Menü `Stammdaten > Auftrag > Statusverwaltung`. (⇨ Stammdaten, "Statusverwaltung" auf Seite B-885)
2. Prüfen Sie, ob der Anwenderstatus für den Lagereingang und für den Lagerabgang vorhanden ist. Legen Sie diese ggf. an.
3. Prüfen Sie als Nächstes die Statuszuordnungen. Wählen Sie im Menü `Stammdaten > Auftrag > Statuszuordnung`. (⇨ Stammdaten, "Statuszuordnung" auf Seite B-887)
4. Prüfen Sie, ob die Statuszuordnungen von Lagereingang und Lagerabgang für die Dokumententypen *Auftrag* und *Bestellung* festgelegt sind:
   - **Warenabgang Lager:** Status Lieferschein gedruckt oder Rechnung gedruckt
   - **Wareneingang Lager:** Status Wareneingang gebucht
5. Legen Sie die fehlenden Zuordnungen an und korrigieren Sie die vorhandenen ggf.

#### Lagerkategorien

Lagerkategorien werden im Dialog *Lagerverwaltung* den Lagerartikeln zugeordnet. Dabei werden die Lagerartikel zu Gruppen (Lagerkategorien) zusammengefasst, die als Suchkriterium eingesetzt werden können.

**Lagerkategorie prüfen**
**So legen Sie eine Lagerkategorie fest**
1. Wählen Sie im Menü `Stammdaten > Lager > Kategorie`.
   
   **Abb. K-9: Lagerkategorien**
   (⇨ Stammdaten, "Lagerkategorien" auf Seite B-739)

2. Wählen Sie im Menü `Start > Neu`, um in den Erfassungs-Modus zu wechseln.
3. Geben Sie für die Lagerkategorie eine ID ein, z. B. Ziffern oder Bezeichnungen wie Rohmaterial, Kisten, Produktion.
4. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.

### Stammdaten für Kisten

In diesem Kapitel finden Sie Informationen dazu, wie Sie die Daten anlegen, um die Preisberechnung für Kisten differenzieren und Kisten im Lager verwalten zu können. Dazu gehören die Definition der Lagermaße und die Definition der Lagerartikel.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Kistendaten" auf Seite K-24
- "Kiste mit Stückliste" auf Seite K-29

#### Kistendaten

**Lernziele**
- Lagermaße und Lagerartikel für Kisten anlegen.
- Produkt (Artikel) für Kiste anlegen.

**Nutzen**
- Wenn Sie die Produkte korrekt anlegen, können die Berechnungen und die Reservierung von Stück und Flächen durchgeführt werden.
- Die jeweils aktuelle Anzeige des Bestands inklusive der Reservierungen erleichtert den Einkauf.

**Merke**
- **Produkte**: Die Produkte aus den Stammdaten dienen zur Erfassung und Preisfindung in Dokumenten. Sie werden nicht automatisch als Lagerbestand geführt, sondern nur aufgrund zusätzlicher Einstellungen und Definitionen.
- **Lagerartikel**: Alle Produkte, die im Lager mit Bestandsmengen geführt werden, müssen auch als Lagerartikel angelegt sein.
- **Bandmaß**: Platte, wie sie vom Hersteller geliefert wird. Aus ihr werden die Gläser für den Verkauf zugeschnitten.
- **Lagerplatte**: Tatsächlich im Lager befindliches Glas mit bestimmtem Maß, z. B. Float 4 mm in 1200 x 1800 mm oder 3500 x 5100 mm. Lagerplatten mit definierten Maßen werden als auch Lagermaß bezeichnet. Lagerplatten können als Ganzes (1200 x 1800) verarbeitet werden. Aus ihnen können aber auch Gläser zugeschnitten werden, z. B. 600 x 900 aus der Platte 1200 x 1800 oder aus der Platte 3210 x 5100.
- **Lagermaß (Festmaß)**: Die als Lagermaß festgelegten Gläser werden ohne Zuschnitt verkauft. Ihnen sind eigene Preistabellen (Lagermaßtabelle) zugeordnet. Ein maßabhängiger Lagerartikel ist immer auch ein Lagermaß.
- **Lagerkennzeichen (Lagerbuchungsart)**: Das Lagerkennzeichen legt fest, ob die Bestände eines Lagerartikels als Fläche (qm) oder in Stückzahlen gewertet werden.
- **Beschaffungsart**: Das Kennzeichen legt fest, wie ein Produkt standardmäßig beschafft wird, z. B. durch Zuschnitt, Lagerentnahme, Produktion, Bestellung.
- **Voreinstellungen**: Keine

#### Lagermaß für Kiste anlegen

Das Lagermaß Kiste ist für Lagerbuchungen zwingend erforderlich. Für die Erfassung einer Kiste als Auftrags- oder Bestellposition muss daher ein Lagerartikel/-maß Kiste angelegt sein.

**So legen Sie Lagermaße in den Stammdaten an**
1. Wählen Sie im Menü `Stammdaten > Produkt > Artikel > Lagermaße`. Der Dialog *Lagermaße* wird geöffnet. (⇨ Stammdaten, "Lagermaße" auf Seite B-637)
2. Wählen Sie im Menü `Start > Neu` und legen Sie das Lagermaß an.

   **Abb. K-10: Lagermaß für Preisfindung anlegen**
   - **A**: Maße der Scheiben und Inhalt der Kiste
   - **B**: Preistabellen für Verkauf und Einkauf
   - **C**: Preisermittlung im Lager
   - **D**: Beschaffungsart

   Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerartikel definiert haben sollten, tragen Sie die gleichen Werte für Breite und Höhe (A) ein.
3. Geben Sie im Feld *Inhalt* an, wie viele Blätter in der Kiste enthalten sind.
4. Geben Sie die Preisschlüssel für den Verkauf und den Einkauf (B) an. Sie müssen je ein eigenes Lagermaß anlegen, wenn Sie unterschiedliche Preise berechnen, z. B. für den Verkauf der gesamten Kiste, für einzelne Blätter aus der Kiste und/oder für den Zuschnitt einzelner Blätter, die der Kiste entnommen werden.
5. Markieren Sie die Checkbox *EK Suche Lager* (C), wenn das Lagermaß in die Preisermittlung einbezogen werden soll.
6. Sie können zusätzlich eine *Bezeichnung* und *Kurzbezeichnung* (Matchcode) eingeben, um z. B. den Lagerartikel besser identifizieren zu können.
7. Geben Sie die *Beschaffungsart* (D) an, z. B. bei Lagerartikeln *Lagerentnahme*.
8. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt, ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
9. Wählen Sie `[Ja]`, wenn das Lagermaß auch als Lagerartikel verwaltet werden soll. Der Dialog *Lagerverwaltung* wird geöffnet.

#### Lagerartikel für Kiste anlegen

Für einen Lagerartikel Kiste müssen Sie mindestens folgende Einstellungen festlegen, um ihn im Lager verwalten zu können:
- Artikelnummer und Bezeichnung
- Maße bei Lagermaßen, Maße und Inhalt
- Lagerort und Standard-Lagerort (Default-Lagerort)
- Bestände

> **Inbetriebnahme des Lagers**
> Wenn noch gar keine Lagerartikel angelegt sind, können Sie sich diese Aufgabe durch die sogenannte Erstinventur erleichtern. Dieser Ablauf ist im Part *Lagerwirtschaft* beschrieben.

**So legen Sie einen Lagerartikel an**
1. Wählen Sie im Menü `Lagerwirtschaft > Lagerverwaltung`. Der Dialog *Lagerverwaltung* wird geöffnet. (⇨ Softwarereferenz, "Lagerverwaltung - Lagerartikel" auf Seite G-186)
2. Wählen Sie im Menü `Start > Neu`, um in den Erfassungs-Modus zu wechseln. Wenn Sie den Dialog *Lagerverwaltung* aus den Stammdaten heraus geöffnet haben, entfällt dieser Schritt. Die Felder für Artikel und Maße sind dann bereits gefüllt.

   **Abb. K-11: Felder für neuen Lagerartikel freigeschaltet**
   - **A**: Nummer des Lagerartikels
   - **B**: Maße und Inhalt der Kiste
   - **C**: Lagerort
   - **D**: Hauptartikel
   - **E**: Bestände
   - **F**: Bestandsprüfung

3. Geben Sie die Nummer (A), die Maße und den Inhalt der Kiste (B) ein.
4. Wählen Sie einen Lagerort aus (C). Wenn Sie keinen Lagerort auswählen, wird der Lagerort `<k.A.>` eingetragen. In der Lagerwirtschaft wird dieser wie die definierten Lagerorte behandelt, z. B. bei der Inventur und bei Abfragen. Wenn Sie einen Lagerartikel an mehreren Lagerorten verwalten, müssen Sie einen dieser Lagerorte als Standard festlegen.
5. Markieren Sie dazu die Checkbox *Default-Lagerort*.
6. Wählen Sie im Feld *Hauptartikel* (D) den Artikel aus, für den Sie einen Mindestbestand für die Bestandsprüfung hinterlegen wollen. Für Kisten ist das die Lagerplatte, aus der die Blätter geschnitten werden.
7. Aktivieren Sie die Checkbox *Bestandsprüfung pro Lagerort* (F), wenn für den Lagerartikel alle Lagerorte bei der Bestandsprüfung getrennt bewertet werden sollen.
8. Wechseln Sie zum Register *Preise* und geben Sie die Mengeneinheit an, mit der der Durchschnittspreis berechnet wird.

   **Abb. K-12: Durchschnittspreis für Lagerartikel**
   - **A**: Durchschnittspreis
   - **B**: Mengeneinheit

9. Wechseln Sie zum Register *Zusatz* und prüfen Sie, ob für die Kisten aus der Produktion der Lieferant **0** eingetragen ist. Mit dieser Einstellung geben Sie an, dass Sie selbst der Lieferant sind. Diese Einstellung hat keine Auswirkungen auf die Kisten, die Sie alternativ auch bei einem Lieferanten bestellen können, denn solche Kisten werden nicht im Lager vorgehalten.
10. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.
11. Wiederholen Sie die Schritte für alle Festmaße, die als Kisten erfasst werden können. Für Kisten legen Sie pro Glas, Abmessung, Inhalt und Preisschlüssel einen Lagerartikel an. Damit sind alle Informationen hinterlegt, die A+W Business braucht, um Reservierungen und Buchungen durchzuführen.

#### Kiste mit Stückliste

**Lernziele**
- Produktaufbau bei Kisten mit Stücklisten (Paletten) kennenlernen.

**Nutzen**
- Kisten mit einer tief gestaffelten Stückliste können als Produkt angelegt und erfasst werden.

**Merke**
- **Produktaufbau**: Kisten mit Stückliste sind Artikel, die einen komplexeren Aufbau haben als einfache Glas-Kisten.
- **Voreinstellungen**:
  - Lagerverwaltung
  - Stammdaten:
    - Produktverwaltung
    - Lieferantenkartei
  - Firmendaten:
    - Register Parameter
    - Register Lager / EK / EDI

#### Stammdaten für Kisten mit Stückliste

Unter Kisten mit Stückliste sind Artikel zu verstehen, die einen komplexeren Aufbau haben als die bisher bekannten Glas-Kisten. Man kann beispielsweise Bilderrahmen-Gläser in Papier einpacken und diese Papierverpackungen auf eine Palette stellen.
Dazu wird die Palette als Hauptprodukt und die Papierbox mit den Gläsern als dessen Stückliste angelegt. Sowohl die Palette als auch die Papierbox gehören dabei zur Produktart Kiste.

> **Vorkenntnisse für diese Einheit**
> In dieser Einheit werden keine neuen Dialoge oder Funktionen erarbeitet. Die Sonderform von Kisten mit Stücklisten stellt einen speziellen Produktaufbau dar, der mit den bereits bekannten Mitteln eingerichtet wird. Informationen zu den Produktstücklisten finden Sie im Part *Stammdaten*.

**Stücklistenaufbau**

**Abb. K-13: Produktverwaltung – Stückliste mit komplexer Kiste**
- **A**: Hauptprodukt: Palette
- **B**: Stückliste: Box mit Gläsern

In der Abbildung ist der Stücklistenaufbau für eine solche Palette dargestellt. Sie benötigen also ein Produkt für die Palette, ein Produkt für die Box und das Glas selbst.

**Produktart**
Damit die Palette und die Box von A+W Business als Kisten interpretiert werden, muss für beide die Produktart **200 - Kiste** eingestellt sein.

**Abb. K-14: Produktverwaltung - Register Produkt**

**Beschaffungsart und Lagerbuchungsart**
Damit beide Produkte im Lager geführt werden können, muss die Beschaffungsart auf **Lagerentnahme** und die Lagerbuchungsart **maßabhängig** eingestellt sein.

**Abb. K-15: Produktverwaltung - Register Lager/Einkauf**

> **Palette mit Stückliste anlegen**
> Wenn Sie die Palette mit der Stückliste anlegen, müssen Sie darauf achten, dass die Beschaffungsart richtig übernommen wird.

**Standardmaße**
Die Erfassung des Produktes in der Positionserfassung wird etwas einfacher, wenn eine Standard-Breite und eine Standard-Höhe für das Produkt eingetragen sind. In der Positionserfassung wird dann nach der Eingabe der Produktnummer automatisch der passende Kistenartikel ausgewählt.

**Abb. K-16: Produktverwaltung – Register Produkt (optional)**

**Preiskennzeichen**
Im Gegensatz zu den bisher bekannten Kisten werden die Kennzeichen *Preisrelevant VK / EK* auf Ebene des Hauptproduktes und der Stückliste zur Preisberechnung ausgewertet.
Zuvor wurde der Preis der Kisten immer nur in dessen Stückliste berechnet und dargestellt. Über die Kennzeichen *Preisrelevant* ist das für Kisten mit Stücklisten konfigurierbar. Abhängig von diesen Kennzeichen wird der Preis im Verkauf also durch den Preis der Stücklisten-Komponente, der Hauptposition oder durch beide bestimmt.
Wenn in unserem Beispiel der Preis der Palette nur aus der Summe der Preise der Boxen, also aus der Stückliste, zusammensetzt werden soll, dann muss das Kennzeichen des Hauptartikels deaktiviert und das der ersten Stücklisten-Komponente, also der Box, aktiviert werden.

| Produkt | Preisrelevant | Preisberechnung |
| :--- | :--- | :--- |
| Palette | Ja | Preis pro Palette und Anzahl der Boxen |
| Box | Ja | |
| Palette | Ja | Preis pro Palette |
| Box | nein | |
| Palette | Nein | Preis aus Anzahl der Boxen |
| Box | Ja | |

**Tab. K-1: Preisberechnung bei Einstellung des Kennzeichens Preisrelevant**

**Preisverwaltung**
In der Preisverwaltung können die Preise der Kisten wie gewohnt eingegeben werden.

**Abb. K-17: Preisverwaltung - Register Matrix**

Sinnvoll ist z. B. eine Matrix mit den beiden Grenztypen *Breite exakt* und *Höhe exakt*. Damit können Stückpreise für verschiedene Abmessungen hinterlegt werden.

**Lagermaße (Produktverwaltung)**
Für jede Ausprägung der Palette und der Box muss im Dialog *Lagermaße* ein Lagermaß angelegt werden. Als Ausprägung gelten dabei die Maße der Gläser. Die Beschaffungsart muss auf *Lagerentnahme* gesetzt werden, damit das Lagermaß im Bestand geführt werden kann.

> **Beispiel**
> Das Lagermaß *Palette mit Boxen* soll aus jeweils 80 Boxen bestehen, die jeweils 25 Gläsern enthalten.
> Wichtig ist, dass für jede Abmessung nur jeweils ein Lagermaß mit einem eindeutigen Inhalt hinterlegt wird. D. h., dass für das Maß 600 x 700 nicht Paletten mit 50 und mit 80 Boxen angelegt werden dürfen.

**Abb. K-18: Produktverwaltung Lagermaße – Palette mit 80 Boxen und Box mit 25 Gläsern**

Für die Lagermaße kann (wie gewohnt) eine Umleitung auf andere Preisschlüssel angegeben werden.
Wenn das neue Lagermaß gespeichert wird, können Sie über die Abfrage direkt in die Lagerverwaltung wechseln, um die zugehörigen Lagerartikel anzulegen.

**Stücklisten-Kiste in der Lagerverwaltung**
Die Lagerartikel werden analog zu den Produkt-Lagermaßen angelegt. Der Artikel wird mit der gleichen Abmessung und dem gleichen Inhalt angelegt. Ergänzend werden der aktuelle Bestand und der Lagerort angegeben.
Für die automatische Erzeugung von Lagerbestellungen müssen außerdem Werte in den Feldern *Mindestbestand* und *Bestellmenge* eingegeben sein.

**Abb. K-19: Lagerverwaltung – Paletten mit 80 Boxen, Box mit 25 Gläsern**

**Stücklisten-Kiste in der Positionserfassung**
Wenn Sie die Palette in einer Position erfassen, geben Sie zunächst wie gewohnt die Produktnummer ein:
- Wenn in den Produktstammdaten eine Standard-Breite und Standard-Höhe eingegeben sind, wird die Kiste automatisch mit den Inhalten aus den Produkt-Lagermaßen erstellt.
- Wenn Sie das Produkt mit einer anderen Abmessung erfassen wollen oder wenn keine Standard-Abmessung angegeben ist, können Sie über die Lagersuche die gewünschte Palette auswählen.
Im Register *Stückliste* sind die Komponenten mit den entsprechenden Inhalten vorbelegt.

**Abb. K-20: Dokumentenverwaltung - Register Stückliste: Palette**
- **A**: Anzahl der Boxen auf der Palette
- **B**: Anzahl der Gläser pro Box

Die Kiste mit Stückliste kann wie jedes andere Produkt erfasst werden. Wenn sie als Lagerartikel geführt wird, kann sie auch dazu dienen, den Lagerbestand durch Produktionsaufträge aufzufüllen.

**Ergänzende Informationen**
- Verkauf, "Auftragskopf" auf Seite C-39
- Verkauf, "Bestellkennzeichen ändern" auf Seite C-310

### Aufträge

Aufträge für Kisten fallen in zweierlei Formen an:
- Verkaufsauftrag für einen Kunden. Wenn Sie außer den produzierten Kisten auch bestellte Kisten verkaufen, müssen die Einstellungen für den Lieferanten auch in der Lieferantenkartei festgelegt sein.
- Produktionsauftrag, um den Lagerbestand zu füllen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Verkaufsauftrag mit Kiste" auf Seite K-38
- "Produktionsaufträge" auf Seite K-42

#### Verkaufsauftrag mit Kiste

In einen Verkaufsauftrag erfassen Sie eine Kiste für einen Kunden. Diese Kiste kann aus Ihrem Lagerbestand entnommen werden oder bei einem Lieferanten bestellt werden.

**So erfassen Sie eine Kiste als Auftragsposition**
1. Wählen Sie `Dokumente > Auftrag` und erfassen Sie die Kopfdaten.

   **Abb. K-21: Auftragskopf für Verkaufsauftrag**
   - **A**: Auftragsbereich
   - **B**: Auftragstyp

   Achten Sie auf die Einstellungen zum Auftragsbereich und zum Auftragstyp.
2. Speichern Sie die Daten und wechseln Sie zum Register *Positionen*. Die Positionserfassung wird geöffnet.
3. Wählen Sie im Menü `Start > Neu`, um eine neue Position zu erfassen.

   **Abb. K-22: Produktnummer für das Glas in der Kiste eingeben**

4. Geben Sie die Produktnummer des Glases ein, das Sie als komplette Kiste erfassen wollen.
5. Wählen Sie im Menü `Start > Lagersuche`, um den Dialog *Lagerinfo* zu öffnen.

   **Abb. K-23: Lagerinformation zu Kisten**
   - **A**: Produktnummer des Glases
   - **B**: Kiste (ohne Bestand)

   Der Dialog *Lagerinfo* wird mit einer Liste aller Kisten und Lagermaße angezeigt, die für die Produktnummer vorhanden sind. Kisten mit dem Lagerort `<k.A>-<k.A>-<k.A>` sind Kisten, die als Lagerartikel angelegt sind. Kisten mit Bestand haben in aller Regel eine ID.
6. Übernehmen Sie die markierte Kiste mit einem Doppelklick. Achten Sie dabei auf die angegebenen Maße, wenn Sie mit unterschiedlichen Kisten für ein Produkt arbeiten.
   
   Der Dialog wird geschlossen und die Positionserfassung wird wieder angezeigt.

   **Abb. K-24: Position mit Kiste erfasst**
   - **A**: Beschaffungsart

7. Wählen Sie die Beschaffungsart (A).
   - **Lagerentnahme**: Die Kiste wird aus dem Lagerbestand entnommen.
   - **Bestellung (komplett)**: Die Kiste wird bei dem Lieferanten bestellt, der in der Lieferantenkartei eingetragen ist. Bei dieser Einstellung muss der Auftrag anschließend an den Einkauf übergeben werden.
8. Korrigieren Sie ggf. die Stückzahl, wenn Sie mehr als eine Kiste erfassen wollen.
9. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert. Sie können jetzt weitere Positionen erfassen und den Auftrag auf die gewohnte Weise abschließen. Wenn Sie den Wareneingang der Kistenlieferung durch einen Lieferanten buchen, wird die gelieferte Kiste dem Auftrag zugeordnet. Eine ausführliche Beschreibung finden Sie im Part *Einkauf*.

#### Produktionsaufträge

Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen. Alle Artikel, die in einem solchen Auftrag erfasst werden, werden automatisch auf die Beschaffungsart *Produktion* umgesetzt. Im Gegensatz zu Kunden-Aufträgen werden die Positionen nicht im Lager reserviert, sondern als bestellt markiert.

**Manuelle und automatische Lagerbestellung**

**Abb. K-25: Lagerbestellung vs. Produktionsauftrag**
(Ablaufplan zeigt Entscheidungsprozess von Lagerbestellung über Mindestbestand, Standard-Bestellmenge und Lieferantenkartei, was entweder zu einem Bestellvorschlag oder einem Produktionsauftrag führt.)

In diesem Ablaufplan ist dargestellt, wie A+W Business auf die unterschiedlichen Voreinstellungen in der Lieferantenkartei reagiert.

**Einstellungen in der Lieferantenkartei**
Wenn im Dialog *Lagerverwaltung* ein Mindestbestand und eine (Standard-) Bestellmenge für den Lagerartikel hinterlegt sind, kann das System automatische Bestellvorschläge generieren. Diese werden im Dialog *Lagerbestellung* aufgelistet.
Normalerweise werden auf diesem Weg Bestellungen vom Typ *Lagerbestellung* generiert. Wenn jedoch in der Lieferantenkartei statt eines Standard-Lieferanten ein interner Kunde hinterlegt ist, können Produktionsaufträge automatisch erzeugt werden.

**Abb. K-26: Interner Kunde für Produktionsaufträge**

In der Lieferantenkartei wird ein interner Kunde eingetragen, für den der Produktionsauftrag automatisch erfasst wird. Die Option *Interner Kunde* kann auf der Ebene der Warengruppen oder der Produkte aktiviert werden. Dabei haben die Einstellungen für Produkte Vorrang vor denen für Warengruppen.

**Bestellmenge**
Der Multiplikator wird so berechnet, dass durch den Vorschlag der Mindestbestand überschritten wird.

**Abb. K-27: Mengenangaben für Lagerartikel (Dialog Lagerverwaltung)**

> **Beispiel**
> Das VSG mit der Produktnummer 107 wird als Lagerartikel geführt.
> Aktueller Lagerbestand: 10 Stk.
> Mindestbestand: 30 Stk.
> Bestellmenge: 5 Stk.
>
> Die Bestellmenge für das VSG 107 wird folgendermaßen berechnet:
> Differenz zwischen aktuellem Bestand und Mindestbestand: 20 Stk. In dieser Differenz ist die Bestellmenge 5 Stk. viermal enthalten.
> Bestellmenge: 4 x 5 = 20 Stk.
> Aktueller Bestand plus bestellte Menge: 10 + 20 = 30 Stk.

Die errechnete Menge wird in den Bestellvorschlag übernommen. Sie kann im Dialog *Lagerbestellung* angepasst werden. Wie Sie die Bestellungen bearbeiten und übergeben, ist im Part *Einkauf* beschrieben.
Der Produktionsauftrag wird erst durch die Übergabe erzeugt und in dem Auftragsnummernverwalter angelegt, der zuletzt aktiviert war. Der Produktionsauftrag kann bearbeitet und an die Produktion weitergeleitet werden.

**Produktionsauftrag erfassen**
Wenn Sie Produktionsaufträge manuell erfassen, können Sie einen früher erfassten Auftrag immer wieder durch Kopieren erneut erfassen und an die Produktion übergeben.

> **Etiketten für den Wareneingang**
> Um eine selbst produzierte Kiste im Wareneingang per BDE zu erfassen, wird ein Etikett/Barcode benötigt. Dafür muss der Druckpunkt 973 zugeordnet werden.

In diesem Kapitel finden Sie folgende Handlungssequenzen:
- "So erfassen Sie die Kopfdaten für einen Produktionsauftrag" auf Seite K-45
- "So erfassen Sie das Glas für die Kiste" auf Seite K-47
- "So erfassen Sie einen Produktionsauftrag durch Kopieren" auf Seite K-48

**So erfassen Sie die Kopfdaten für einen Produktionsauftrag**
1. Wählen Sie `Dokumente > Auftrag > Auftrag`. Der Dialog *Dokumentenverwaltung* wird geöffnet. In dieser Beschreibung ist dies der Modus *Bearbeiten*.
2. Prüfen Sie im Menü `Funktionen > Dokument > NV Auswahl`, ob der richtige Nummernverwalter eingestellt ist, und korrigieren Sie ggf. die Einstellung. Sie können die Zuordnung des Auftrags zu einem Nummernverwalter auch im Auftragskopf sehen.
3. Wählen Sie ggf. im Menü `Start > Neu`, um in den Erfassungs-Modus zu wechseln.
4. Geben Sie die erforderlichen Kopfdaten ein.
5. Tragen Sie ggf. in den Feldern unter dem Namen eine Erläuterung zum Auftrag ein, z. B. dass die Scheiben in Kisten verpackt werden sollen.
6. Wählen Sie den Auftragstyp *Produktionsauftrag* (B).
7. Prüfen Sie die weiteren Angaben.
8. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Kopfdaten werden gespeichert. Sie können jetzt zum Register *Positionen* wechseln und die Auftragspositionen erfassen. Wenn Sie Daten im Auftragskopf ändern, wird das Register *Positionen* wieder gesperrt. Sie müssen die Änderungen speichern, um das Register *Positionen* wieder freizuschalten.

   **Abb. K-28: Kopfdaten für Produktionsauftrag**
   - **A**: Auftragsbereich
   - **B**: Produktionsauftrag

**So erfassen Sie das Glas für die Kiste**
1. Wählen Sie `Dokumente > Auftrag > Auftrag auswählen > Register Positionen` oder `<F9>`. Die Positionserfassung wird geöffnet.
2. Wählen Sie im Menü `Start > Neu`, um eine neue Position zu erfassen.
3. Geben Sie die Produktnummer des Glases ein, das als Kiste produziert werden soll.

   **Abb. K-29: Produktnummer für das Glas in der Kiste eingeben**

4. Setzen Sie die Stückzahl auf den Inhalt der Kiste oder ein Vielfaches des Inhalts.
5. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert. Übergeben Sie den Produktionsauftrag an die Produktion. Wenn Sie regelmäßig Produktionsaufträge erfassen, können Sie den zuvor erfassten Auftrag kopieren und sich so die Arbeit erleichtern. Eine ausführliche Beschreibung finden Sie im Part *Verkauf*.
   - Vor dem Kopieren müssen Sie den Dokumententyp des Ziel-Dokuments auf *Produktionsauftrag* einstellen.

**So erfassen Sie einen Produktionsauftrag durch Kopieren**
1. Wählen Sie `Dokumente > Auftrag > Auftrag` auswählen. Die Auftragserfassung wird geöffnet.
2. Wählen Sie im Menü `Funktionen > Dokumente kopieren`.

   **Abb. K-30: Produktionsauftrag durch Kopieren erstellen**
   - **A**: Kopieren von Auftrag nach Auftrag
   - **B**: Dokumententyp des Ziel-Auftrags

3. Wechseln Sie zum Register *Kopieren positionsweise* und markieren Sie die Position(en), die kopiert werden sollen.
4. Korrigieren Sie ggf. die Zielmenge.
5. Wählen Sie im Menü `Start > Ausführen`, um die Kopie zu erzeugen.

### Lagerverwaltung für Kisten

Für Lagerartikel werden sowohl der Wareneingang als auch der Warenabgang erfasst, damit Sie die Bestände verwalten können.
Der Warenein- und Warenabgang von Kisten kann über Barcodes (BDE) oder manuell erfasst werden.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Lagerverwaltung von Kisten" auf Seite K-49
- "Lagerbestellung von Kisten" auf Seite K-50
- "Wareneingang per Barcode" auf Seite K-55
- "Manuelle Lagerbuchungen" auf Seite K-61
- "Warenausgang Kisten" auf Seite K-56

#### Scannen

In Verbindung mit AWPort können Lagerbuchungen auch über Barcodes erfasst werden. Dazu gehören nicht nur die Wareneingänge und Warenausgänge, sondern auch die Auflösung einer Kiste und andere Umbuchungen.
Durch Scannen können ganze Kisten einem bestimmten Auftrag oder einer Auftragsposition zugeordnet werden oder mit der entsprechenden Blattanzahl für die Inventur erfasst werden.
(⇨ "Wareneingang per Barcode" auf Seite K-55)
Weitere Informationen zum Barcode und den Formaten entnehmen Sie bitte der Dokumentation zu AWPort.

#### Lagerverwaltung von Kisten

Gelieferte Kisten haben in aller Regel eine ID vom Lieferanten, mit der sie im Wareneingang erfasst werden.
Jede Kiste wird mit einer eigenen Kisten-ID im verbucht und im Lager geführt. Dazu muss in den Firmendaten die Checkbox für die virtuellen Identnummern aktiviert sein.
(⇨ "Firmendaten" auf Seite K-18)
(⇨ "Wareneingang per Barcode" auf Seite K-55)

**Kisten aufbrechen**
Um einzelne Blätter aus einer Kiste zu erfassen, muss die Kiste aufgelöst werden. Dabei wird eine Kiste (mit ID) zunächst aus dem Lagerbestand entfernt. Die Anzahl der Blätter wird dann dem Lagerbestand des entsprechenden Lagerartikels (Lagermaß) zugebucht.

#### Lagerbestellung von Kisten

Der Bestand von Kisten kann entweder durch einen automatisch oder einen manuell erzeugten Produktionsauftrag aufgefüllt werden.
Lagerbestellungen können auch manuell über die Dokumentenverwaltung erzeugt werden.
(⇨ "So erfassen Sie eine Lagerbestellung mit Kisten" auf Seite K-52)

**Bestellvorschläge**
In der Regel werden Bestellungen aus der Lagerwirtschaft heraus erzeugt, um die Bestände auf dem gewünschten Niveau zu halten.

**Abb. K-31: Lagerverwaltung - Bestandszahlen**
- **A**: Mindestbestand
- **B**: Menge für Bestellvorschlag

Wenn Sie im Dialog *Lagerverwaltung* Mindestmengen (A) für einen Lagerartikel hinterlegt haben, werden Bestellvorschläge automatisch mit der hinterlegten Bestellmenge (B) erzeugt. Sie können diese vor der Übergabe an den Einkauf prüfen und ggf. den Lieferanten und den Termin ändern. Mit der Übergabe an den Einkauf wird aus dem Vorschlag eine Lagerbestellung erzeugt.
