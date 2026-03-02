---
description: "DE_AWBusiness_Einkauf_3_1"
---


# Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

---
## Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 3.30/04-2020 | Wareneingang aktualisiert. |
| 3.20/11-2019 | Softwarereferenz: Aktualisierung Dialog Wareneingang, Tutorial: Kapitel für Kisten in den Part Kistenmanagement verschoben. |
| 3.10/10-2017 | Strukturelle Überarbeitung, neuer Dialog Nachbestellung, Dialog AB-Lieferant aktualisiert. |
| 3.01/01-2017 | Produkt- und Firmennamen angepasst. |
| 3.00/06-2013 | Vollständige Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business. |
| 2.10/02-2012 | Aktualisierung der Kapitel zum Wareneingang |
| 2.00/02-2010 | Aktualisierung und Umstellung auf Doku-Konzept 2010 |
| 1.00/10-2008 | Part Einkauf neu. Aus Part Dokumente ausgegliedert |

## Editorial

Das Editorial enthält Informationen zu folgenden Themen:
* Anmerkungen zu diesem Dokument
* Urheberrechte
* Warenzeichen
* Kontakte

### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von *A+W Business* gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe von *A+W Business*.

### Urheberrechte
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim

📞 +49 6404 2051-0
📠 +49 6404 2051-877
📧 aw.zentrale@a-w.com
🌐 http://www.a-w.com

# Tutorial

## Überblick

Das Tutorial zum Modul Einkauf beschäftigt sich mit den Grundlagen des Einkaufs in *A+W Business*. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zum Verkauf auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
>
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
* Grundgedanken zum Einkauf
* Stammdaten für den Einkauf
* Bestellungen
* Lieferungen im Wareneingang
* Elektronischer Dokumentenaustausch

### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in *A+W Business* den Einkauf abwickeln. Die Teilnehmer müssen das Konzept der Stammdaten in *A+W Business* und den Dialog *Dokumentenverwaltung* kennen.

### Dokumentation

Für das Modul *Einkauf* stehen folgende Dokumente zur Verfügung:

| | |
| :--- | :--- |
| **Handout** | Ausdruck des Tutorials für die Schulung |
| **PDF** | Vollständige Unterlagen<ul><li>Tutorial</li><li>Softwarereferenz</li><li>Index</li></ul> |
| **Online-Hilfe <F1>** | Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenzen und Tutorials der Basisversion |

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

*   **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    *   Lernziele: Was soll vermittelt werden?
    *   Nutzen: Wofür können Sie dieses Wissen einsetzen?
    *   Merksätze: Welche Zusammenhänge müssen Sie sich merken?
*   **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
*   **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
*   **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

**Lesehinweis**
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| | |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Nummernverwalter*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| **>** | Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Dokumente > Bestellung > Export*. |
| **[]** | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten. |
| **<>** | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit **<F1>** öffnen Sie die Online-Hilfe. |

### Menü-Übersicht

In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

Im Menü *Dokumente* finden Sie auch die Programmbereiche, mit denen Sie den Verkauf abwickeln. Diese werden im Part *Verkauf* beschrieben.

*Abb. D-1: Modul Dokumente – Menü Bestellung*

#### Bestellung
In diesem Bereich erstellen und verwalten Sie Bestellungen.
-> "Bestellungen" auf Seite D-43

#### Nachbestellung
In diesem Dialog verwalten Sie Aufträge mit Bestellteilen, die als Bruch gemeldet sind und entscheiden ob diese nachbestellt, reklamiert, verrechnet oder von der Auftragsmenge abgezogen werden sollen.
-> Softwarereferenz, "Nachbestellung" auf Seite D-191

#### Druck Bestellung
In diesem Dialog drucken Sie die Bestellungen, die Sie an Lieferanten senden wollen. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Druck" auf Seite C-190

#### Export
In diesem Dialog exportieren Sie Bestellungen, um sie über die EDI-Schnittstelle an den betreffenden Lieferanten zu übertragen.
-> "Bestellung exportieren" auf Seite D-182

#### Journal
In diesem Dialog verschaffen Sie sich einen Überblick über die Bestellungen. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Journal" auf Seite C-384

#### AB Lieferant
In diesem Dialog erfassen Sie die Auftragsbestätigungen, die Ihre Lieferanten gesendet haben.
-> "Lieferanten-AB" auf Seite D-87

#### Auftragsbestätigung
In diesem Bereich prüfen Sie die Preise von Auftragsbestätigungen.
-> "Rechnung kontrollieren" auf Seite D-146

#### Wareneingang
In diesem Bereich prüfen und erfassen Sie den Wareneingang zu Ihren Bestellungen.
-> "Wareneingang" auf Seite D-120

#### Rechnung
In diesem Bereich erfassen und kontrollieren Sie die Lieferantenrechnungen.
-> "Elektronisches Dokument prüfen" auf Seite D-170

#### FIBU-Übergabe
In diesem Dialog übergeben Sie die eingegangenen Rechnungen an Ihre Finanzbuchhaltung. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Sollstellung FiBu" auf Seite C-682

#### Übergabe Archiv
In diesem Dialog übergeben Sie Ihre Bestellungen an das Archiv. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Übergabe Archiv" auf Seite C-686

#### Dokumentendaten
In diesem Dialog können Sie sich Übersichten über Bestellungen und korrespondierende Aufträge anzeigen lassen und ggf. die Termine korrigieren. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Dokumentendaten" auf Seite C-737

#### Lagersuche
In diesem Dialog können Sie die Verfügbarkeit von Produkten prüfen und nach Lagermaßen suchen. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Lagersuche" auf Seite C-741

#### Artikel-Info
In diesem Dialog können Sie sich Informationen zu den Produkten anzeigen lassen, die in *A+W Business* angelegt sind. Sie können dabei den Produktaufbau, die Preise und die Verfügbarkeit prüfen. Diese Funktion ist ausführlich im Part *Verkauf* beschrieben.
-> Verkauf, "Artikel-Informationen" auf Seite C-602

#### Faxnachricht
In diesem Dialog können Sie direkt aus *A+W Business* Faxnachrichten an Ihre Kunden und Lieferanten erstellen und versenden. Diese Funktion ist ausführlich im Part *Überblick* beschrieben.
-> Einleitung, "Standard-Menüs" auf Seite A-53

## Grundgedanken zum Einkauf
Der Einkauf gehört zu den kaufmännischen Aufgaben im Unternehmen. Ein typischer Einkauf ist in *A+W Business* so oder ähnlich aufgebaut:

*Abb. D-2: Schema des Einkaufs in A+W Business*
*(Legende: Blau = Dokument, Gelb = Bereich, Gestrichelt = optional)*
*(Diagramm zeigt einen Ablauf: Anfrage (optional) führt zu Bestellung. Kunden-Auftrag führt über Übergabe ebenfalls zu Bestellung. Bestellung führt zu AB + Preiskontrolle, was dann zum Wareneingang führt. Kunden-Auftrag kann auch direkt zur Produktion führen. Wareneingang kann zum Lager oder zur Produktion führen. Vom Wareneingang gibt es eine weitere AB + Preiskontrolle.)*

Alle kaufmännischen Vorgänge in *A+W Business* basieren auf den Stammdaten. Nur wenn diese korrekt gepflegt sind, kann der Einkauf problemlos abgewickelt werden:

*   **Anfrage:**
    Mit der Anfrage holen Sie Angebote Ihrer Lieferanten ein. Wenn Sie das Angebot überzeugt, können Sie aus der Anfrage direkt die Bestellung erzeugen, ohne die Daten erneut eingeben zu müssen.
    -> "Anfrage" auf Seite D-110
*   **Bestellung:**
    Als manuelle Bestellung erfassen Sie die Bestellpositionen und wählen den gewünschten Lieferanten aus.
    Die referenzierte Bestellung wird aus dem Kundenauftrag über den Bestellpool erzeugt.
    -> "Manuelle Bestellung" auf Seite D-79
*   **Auftragsbestätigung (AB) vom Lieferanten:**
    Sie erfassen die Nummer der AB und prüfen die Preise und Liefertermine. Bei Verzögerungen benachrichtigen Sie ggf. den Kunden. Geänderte und bestätigte Preise können in die EK-Kalkulation zurückgeschrieben werden.
    -> "Auftragsbestätigung und Liefertermin" auf Seite D-87
*   **Wareneingang:**
    Sie prüfen den Wareneingang und buchen automatisch die Lagerbestellungen in den Lagerbestand. Referenzierte Bestellungen werden als Eingang an die Produktion und/oder den Verkauf übergeben, um den zugehörigen Kundenauftrag weiterzubearbeiten oder abzuschließen.
    -> "Wareneingang erfassen" auf Seite D-127
*   **Rechnungskontrolle:**
    Sie prüfen die Rechnung und korrigieren ggf. Ihre Einkaufspreise, sofern Sie die geänderten Preise akzeptieren. Anschließend kann die Rechnung zur Anweisung freigegeben werden.
    -> "Preis- und Rechnungskontrolle" auf Seite D-143

### Handlungsablauf im Einkauf
Üblicherweise bearbeiten Sie ein Einkaufsdokument in folgenden Schritten:
*   Anfrage erstellen (optional)
*   Bestellung
    *   Kopfdaten erfassen
    *   Positionen erfassen
    *   Stückliste bearbeiten
*   Bestellung drucken (senden per Fax, E-Mail, elektronisch)
*   Auftragsbestätigung vom Lieferanten erfassen
*   Preise prüfen
*   Termine und Tourenplanung nach Rückmeldungen korrigieren
*   Wareneingang erfassen
*   Rechnung prüfen
*   Übergabe an Archiv und Statistik
*   Dokument aus der Hauptdatenbank löschen

Wenn die Bestellung durch die Bestellübergabe aus einem Kundenauftrag erzeugt wurde, müssen die Daten nicht manuell erfasst werden.

> **Täglicher Arbeitsablauf**
> Am einfachsten gestalten Sie Ihren täglichen Arbeitsablauf über die *Nummernverwalter*. Leeren Sie dazu den entsprechenden Nummernverwalter oder legen Sie für den aktuellen Tag einen neuen an.
> Erstellen Sie dann die neuen Dokumente in diesem Nummernverwalter.
> Auf diese Weise behalten Sie am besten im Blick, welche Dokumente neu sind und weiterverarbeitet werden können oder müssen.

# Stammdaten für den Einkauf
In diesem Themenblock lernen Sie, wie Sie die Stammdaten für den Einkauf anpassen.

Dazu gehören folgende Lerneinheiten:
*   "Produktdefinition" auf Seite D-21
*   "Lieferanten" auf Seite D-30
*   "EK-Preise" auf Seite D-36
*   "Dokumentenstatus" auf Seite D-40

## Produktdefinition
**Lernziele**
*   Stammdaten der Produkte für den Einkauf anpassen.
*   Beschaffungsarten für Bestellung kennenlernen.
*   Nutzen des Bestellkennzeichens im Auftrag kennenlernen.

**Nutzen**
*   Anhand des Bestellkennzeichens erkennt *A+W Business* die Produkte, die bestellt werden müssen.
*   Über das Bestellkennzeichen wird zu einem Kundenauftrag im Bestellpool automatisch eine Bestellung erzeugt. Die Bestellung muss daher nicht manuell erfasst werden.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Beschaffungsart** | Das Kennzeichen *Beschaffungsart* legt fest, wie das im Auftrag oder in der Bestellung erfasste Produkt beschafft werden soll, z. B. durch Produktion, Lagerentnahme, Bestellung. |
| **Bestellkennzeichen** | Als Bestellkennzeichen werden folgende Beschaffungsarten bezeichnet: <ul><li>Bestellung</li><li>Bestellung (komplett)</li></ul> |
| **Bestellung (komplett)** | Dieses Kennzeichen wird bei Produkten mit Stückliste verwendet, die als Ganzes bestellt werden sollen, z. B. eine komplette Tür mit Beschlägen. |
| **Bestellung** | Dieses Kennzeichen wird bei Produkten verwendet, deren einzelne Komponenten bestellt werden sollen, z. B. nur die Beschläge. |
| **Voreinstellungen** | Stammdaten: Produktverwaltung: <ul><li>Register *Preis/Zuschlag*</li><li>Register *Lager/Einkauf*</li></ul> Firmendaten: <ul><li>Register *Lager/EK/EDI*</li><li>Register *Dokumente*</li><li>Register *Parameter*</li><li>Register *Kalkulation*</li></ul> |

### Bestellkennzeichen
Der Einkauf bezieht sich auf die Produkte, die in *A+W Business* verwaltet werden. Um ein Produkt einzukaufen, muss es in einer Bestellung erfasst werden.

Zu jedem Produkt legen Sie fest, wie es für die Preisberechnung, die Rabattfindung, die Fertigung oder Bestellung usw. herangezogen wird. Nur mit den entsprechenden Kennzeichen sind z. B. automatische Übergaben an die Schnittstellen, Berechnungen und Druck in den Dokumenten möglich.

Im Rahmen des Einkaufs muss die Beschaffungsart gesondert betrachtet werden, denn über sie erkennt *A+W Business*, wenn ein Produkt oder eine Komponente eines Produkts eingekauft werden muss.

*   **Bestellartikel (komplett):**
    Bestellung erfolgt inklusive aller Bearbeitungen, die in der Stückliste erfasst wurden. Besteht z. B. ein VSG aus einem Float 5 mm, einer Folie und einem ESG 5 mm, so wird das VSG als Ganzes bestellt. (Beachten Sie hierzu auch die Abgrenzung zu Bestellartikel.)
*   **Bestellartikel:**
    Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste (z. B. Bearbeitungen) zu beachten. Besteht wiederum z. B. ein VSG aus einem Float, einer Folie und einem ESG und ist das Kennzeichen *Bestellartikel* nun für das ESG gesetzt, so wird nur das ESG beim Lieferanten bestellt. Das VSG wird in Eigenfertigung produziert.

Dieses Bestellkennzeichen wird automatisch in die Auftragsposition übernommen. Im Auftrag kann aber außerdem jeder Position ein Bestellkennzeichen zugeordnet werden.

### Beschaffungsart
Diese Beschaffungsarten für die Bestellung (Bestellkennzeichen) werden in den Stammdaten der Produkte festgelegt. Es wird standardmäßig herangezogen, wenn ein Produkt im Dokument erfasst wird. Im Auftrag und in der Bestellung kann es überschrieben werden.

*Abb. D-3: Bestellkennzeichen in der Stückliste*
*(Diagramm zeigt, wie unterschiedliche Einstellungen für Bestellkennzeichen in einer Stückliste das Bestellverhalten beeinflussen. Zum Beispiel wird bei 'Bestellung (*)' für 'Float_4_Bronze' nur das Glas ungesäumt geliefert, während das ISO-Produkt im Haus produziert wird. Bei 'Bestellung komplett (**)' für das ISO-Produkt wird das gesamte ISO-Element geliefert.)*

Wenn eine Hauptposition oder eine übergeordnete Stücklisten-Komponente mit der Beschaffungsart *Bestellung (komplett)* gekennzeichnet ist, werden die zugehörigen Stücklisten-Komponenten nicht vom Lager abgebucht, wenn deren Beschaffungsart auf *Lagerentnahme* eingestellt ist. Die Beschaffungsart dieser Komponenten kann dann nicht geändert werden.

Die Beschaffungsart kann pro Mandant und/oder AV-Bereich festgelegt werden. In diesem Fall muss in den Firmendaten die Option *Abweichende Beschaffungsart pro Mandant/AV-Bereich aktivieren* aktiviert werden.

*Abb. D-4: Firmendaten - Register Parameter*

### Preise und Zuschläge
Preistabellen werden sowohl für den Einkauf als auch für den Verkauf angelegt. Sie müssen jedem einzelnen Produkt zugewiesen werden, damit die entsprechenden Preise automatisch berechnet werden.

### Stammdaten eines Produkts prüfen
Für den Einkauf müssen besonders all die Produktdaten vollständig erfasst sein, die standardmäßig bestellt werden.

Im Part *Stammdaten* ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Produkten anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten eines Produkts**
1.  Wählen Sie *Stammdaten > Produkte > Artikel > Artikel*.
    Der Dialog *Produktverwaltung* wird geöffnet.
    -> Stammdaten, "Produktverwaltung - Lager/Einkauf" auf Seite B-608
2.  Suchen Sie das Produkt, das Sie prüfen möchten, und wechseln Sie zum Register *Preis/Zuschlag*.

    *Abb. D-5: Produktverwaltung - Preis/Zuschlag*
    *(Screenshot zeigt das Register 'Preis/Zuschlag' in der Produktverwaltung. Markiert sind Bereiche A für die Preisberechnung für den Verkauf und B für die Preisberechnung für den Einkauf.)*

3.  Prüfen Sie, ob die Preistabellen und die Checkboxen *Preisrelevant für VK* (A) und *EK* (B) richtig gewählt sind.
    Die Checkbox *Preisrelevant EK* muss nur dann markiert sein, wenn Sie mit der EK-Kalkulation arbeiten.

4.  Wechseln Sie zum Register *Lager/Einkauf*.
    Weitere Informationen zu den Preisen finden Sie unter:
    -> "EK-Preise" auf Seite D-36

    *Abb. D-6: Produktverwaltung – Lager/Einkauf*
    *(Screenshot zeigt das Register 'Lager/Einkauf' in der Produktverwaltung. Markiert sind A für die Auswahl der Beschaffungsart und B für abweichende Kennzeichen.)*

5.  Prüfen Sie, ob die Beschaffungsart (A) richtig eingestellt ist.
    Für Bestellartikel können Sie folgende Einträge auswählen:
    *   **Bestellung (komplett):** Produkt mit Stückliste und Produkt, das als Ganzes bestellt wird, z. B. eine komplette Tür mit Beschlägen.
    *   **Bestellung:** Produkt ohne Stückliste und Produkt, das als Stücklisten-Komponenten (ganz oder teilweise) bestellt wird.
6.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
    Die Daten werden gespeichert.

### Lagermaß anlegen
Für die korrekte Preisberechnung können Sie Lagermaße zu den Produkten anlegen, z. B. Gläser mit festen Maßen. Wenn ein Produkt auch als Lagerartikel geführt werden soll, müssen Sie es außerdem in der Lagerverwaltung anlegen. Eine Beschreibung dazu finden Sie im Part *Lagerwirtschaft*.

**So legen Sie Lagermaße in den Stammdaten an**
1.  Wählen Sie *Stammdaten > Produkte > Artikel > Lagermaße*.
    Der Dialog *Produktverwaltung Lagermaße* wird geöffnet.
    -> Stammdaten, "Lagermaße" auf Seite B-637
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.

    *Abb. D-7: Felder für Lagermaß freigeschaltet*
    *(Screenshot zeigt den Dialog zur Anlage von Lagermaßen. A: Maße der Platte, B: Inhalt bei Kisten, C: Preistabellen für VK/EK, D: Preisermittlung im Lager.)*

3.  Geben Sie die Maße (A) an.
    Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerartikel definiert haben sollten, tragen Sie die gleichen Werte für Breite und Höhe ein.
4.  Wenn das Lagermaß als Kiste verwaltet wird, geben Sie an, wie viele Blätter (B) in der Kiste enthalten sind.
5.  Sie können zusätzlich folgende abweichende Angaben einstellen:
    *   Preisschlüssel (C) für den Verkauf und den Einkauf.
    *   Bezeichnung und Kurzbezeichnung (Matchcode), z. B. um den Lagerartikel besser identifizieren zu können.
    *   Beschaffungsart, z. B. *Lagerentnahme* bei Lagermaßen, die auch als Lagerartikeln vorhanden sind.
    
    Wenn Sie das Lagermaß auch als Lagerartikel anlegen wollen, müssen Sie entscheiden, ob die Preisermittlung auch im Lager durchgeführt werden soll.
6.  Markieren Sie die Checkbox *EK Suche Lager* (D), wenn das Lagermaß in die Preisermittlung einbezogen werden soll.

    *Abb. D-8: Neues Lagermaß für die Preisberechnung*

7.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
    Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt, ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
8.  Wählen Sie **[Ja]**, wenn das Lagermaß auch als Lagerartikel verwaltet werden soll.

    Der Dialog *Lagerverwaltung* wird geöffnet. Wie Sie Lagerartikel anlegen, ist ausführlich im Part *Lagerwirtschaft* beschrieben.
    -> Lagerwirtschaft, "Lagerartikel anlegen" auf Seite G-74

## Lieferanten
**Lernziele**
*   Lieferanten als Marktpartner anlegen.
*   Standard-Lieferant zuordnen.
*   Lieferantenkartei kennenlernen.

**Nutzen**
*   Bestellungen können über die hinterlegten Kommunikationswege direkt an den Lieferanten gesendet werden.
*   Standard-Lieferanten werden in der Bestellung automatisch erfasst. Sie können jedoch geändert werden, wenn dies erforderlich ist.
*   Über die Angaben zur Lieferdauer werden die Termine für Bestellungen und referenzierte Aufträge errechnet.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Marktpartner** | Alle Lieferanten werden im Dialog *Partnerverwaltung* angelegt. |
| **Lieferantenkartei** | In der Lieferantenkartei wird festgelegt, welche Lieferanten welche Produkte bzw. Warengruppen liefern. Diese Angaben werden u. a. für die Übergabe von Bestellpositionen an den Einkauf benötigt. |
| **Standard-Lieferant** | Wenn für ein Produkt oder eine Warengruppe mehrere Lieferanten eingetragen sind, wird ein Standard-Lieferant festgelegt. |
| **Voreinstellungen** | Stammdaten: <ul><li>Lieferantendaten (Marktpartner)</li><li>Lieferantenkartei</li></ul> |

### Marktpartner Lieferant
Lieferanten werden in *A+W Business* angelegt, damit Bestellungen automatisiert abgearbeitet werden können. Bei der Erfassung von Aufträgen und Bestellungen müssen die Daten der Lieferanten daher nicht gesondert erfasst werden.

Lieferanten werden wie die Kunden im Dialog *Partnerverwaltung* angelegt. In den Stammdaten der Lieferanten müssen die Daten für die Kommunikation korrekt hinterlegt sein, damit Dokumente direkt aus *A+W Business* heraus versendet werden können.

### Lieferantenkartei
In der Lieferantenkartei wird festgelegt, welche Lieferanten welche Produkte bzw. Warengruppen liefern. Werden für einen Lieferanten ein Produkt und die dazugehörigen Warengruppen angegeben, berücksichtigt die Bestellübergabe das Produkt vorrangig.

Die Angaben aus der Lieferantenkartei werden ignoriert, wenn im Dokumentenkopf zu einer Position oder zu einer Stücklisten-Komponente ein abweichender Lieferant eingegeben ist.

Wenn für ein Produkt mehrere Lieferanten angegeben sind, kann bei der Bestellübergabe ein Preisvergleich gestartet werden. Gleichzeitig wird die Lieferdauer angezeigt, so dass auch hinterlegte Lieferzeiten berücksichtig werden können.

### Standard-Lieferant
Wenn ein Standard-Lieferant festgelegt ist, muss die Bestellung nicht über den Bestellpool gesendet werden. Der Standard-Lieferant wird mit der Rangnummer 1 gekennzeichnet, alle weiteren Lieferanten erhalten die Folgenummern in der Reihenfolge, die ihrer Bedeutung für den Einkauf entspricht.

Pro Produkt gibt es nur einen Standard-Lieferanten. Wenn aber ein bestimmtes Produkt in großer Stückzahl bestellt wird, die der Standard-Lieferant nicht produzieren kann, kann zusätzlich ein Standard-Lieferant für Serienaufträge angelegt werden. In der Auftragserfassung aktivieren Sie in einem solchen Fall den Dokumententyp *Serienauftrag*. Bei der Bestellübergabe wird dann automatisch der Lieferant für Serienaufträge herangezogen.

### Stammdaten eines Lieferanten prüfen
Damit die Bestellungen korrekt abgewickelt werden können, müssen Sie die Stammdaten eines Lieferanten und die Zuordnung von Produkten zu Lieferanten einrichten.

Im Part *Stammdaten* ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Partnern anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten der Lieferanten**
1.  Wählen Sie *Stammdaten > Marktpartner > Lieferant > Lieferanten*.
    -> Stammdaten, "Partnerverwaltung" auf Seite B-756
2.  Suchen Sie den Lieferanten, dessen Daten Sie prüfen wollen.

    *Abb. D-9: Stammdaten - Lieferanten*
    *(Screenshot zeigt die Stammdaten eines Lieferanten. Markiert ist A: E-Mail-Adresse und B: Sprache für Formulare.)*

3.  Prüfen Sie im Register *Adresse*, ob die Daten für den Schriftverkehr und die Kommunikation vollständig und aktuell sind.
    Die E-Mail-Adresse kann auch für den Austausch von elektronischen Dokumenten genutzt werden, z. B. von PDF-Dateien. Achten Sie auf die korrekte und vollständige Schreibweise.
4.  Wechseln Sie zum Register *Auftrag* und prüfen Sie, ob der Dokumentenversand richtig aktiviert ist.

    *Abb. D-10: Fax- und E-Mail-Versand (Beispiel für Einstellungen)*
    *(A: Bestellung per Fax-Versand, B: Anfrage per E-Mail-Versand)*

5.  Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

### Lieferantenkartei anpassen
In der Lieferantenkartei legen Sie fest, welche Lieferanten welche Produkte bzw. Warengruppen liefern und wie lange die Lieferzeiten sind.

**So prüfen Sie die Lieferantenkartei**
1.  Wählen Sie *Stammdaten > Marktpartner > Lieferant > Kartei*.
    Der Dialog *Lieferantenkartei* wird mit dem Register *Produkte* geöffnet.
2.  Wählen Sie im Menü *Start > Filter*, um in den Such-Modus zu wechseln.

    *Abb. D-11: Lieferantenkartei – Produktsuche*
    *(Screenshot zeigt den Suchdialog der Lieferantenkartei. A: Option Produkt, B: Auswahl der Varianten.)*

3.  Wählen Sie die Option *Produkt* (A) und tragen Sie die Nummer des Produkts ein.
4.  Wählen Sie im Menü *Start > Suchen*, um in die Suche zu starten.
    Im Bereich *Produkt - Lieferanten* werden alle Lieferanten aufgeführt, die das gewählte Produkt liefern können. Mit dem Rang 1 ist der Standard-Lieferant gekennzeichnet.

    *Abb. D-12: Lieferantenkartei - Produkte*
    *(Screenshot zeigt die Ergebnisliste. A: Abweichende Bezeichnungen, B: Lieferzeit, C: Rang 1 = Standard-Lieferant, D: Pfeile zur Rangfolgeänderung.)*

5.  Tragen Sie die Anzahl (B) der Tage ein, die zur Berechnung der Lieferzeit herangezogen werden soll.
    Die Lieferzeit wird bei der Bestellübergabe im Preisvergleich und bei der Lieferterminkontrolle berücksichtigt.
6.  Prüfen Sie die Rangfolge der Lieferanten und korrigieren Sie diese ggf., indem Sie einen Eintrag markieren und mit den Pfeilschaltflächen (D) nach oben oder unten verschieben.
    Die Rangnummer 1 (C) bezeichnet den Standard-Lieferanten. Er wird automatisch bei Bestellungen eingesetzt, die nicht im Bestellpool geprüft werden.
7.  Wenn Ihr Lieferant abweichende Produktbezeichnungen benutzt, tragen Sie diese ein (A).
    Diese Bezeichnungen werden in der Bestellung aufgeführt und helfen, Missverständnisse zu vermeiden.
8.  Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
    Wenn Sie ganze Warengruppen prüfen möchten, wechseln Sie zum Register *Warengruppen* und verfahren analog.

## EK-Preise
**Lernziele**
*   Preisjahrgang, Preisschlüssel und Tarife für Einkaufspreise (EK) kennenlernen.
*   EK-Preise bearbeiten.

**Nutzen**
*   Einkaufspreise werden bei der Erfassung von Aufträgen und Bestellungen berechnet, so dass der Deckungsbeitrag automatisch berechnet werden kann.
*   EK-Preise können in der Bestellung überschrieben werden.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Preisliste** | Preisjahrgänge, -schlüssel und Tarife bilden den Rahmen für die Preislisten. |
| **Individualpreise** | Individuelle Preise von Lieferanten können Sie mit allen Bezugsgrößen einrichten, die auch für die allgemeinen Preislisten und Zuschläge gelten. |
| **Voreinstellungen** | **Stammdaten:**<ul><li>Jahrgang</li><li>Schlüssel</li><li>Tarife</li><li>Preise</li></ul>**Firmendaten:**<ul><li>Register Lager / EK / EDI</li><li>Register Preisberechnung</li><li>Register Fibu</li></ul>**Referenzen:**<ul><li>Preisimport VEGLA</li></ul>**Utilities:**<ul><li>Preislistenimport</li></ul> |

### Preislisten
Die Preisberechnung in *A+W Business* ist aus flexiblen Bausteinen zusammengesetzt, die alle Berechnungsmöglichkeiten abdecken. Sie können jedem Produkt die passende Art der Preisberechnung zuordnen.

Preisjahrgänge, -schlüssel und Tarife bilden den Rahmen für die Preislisten. In den Preistabellen selbst sind die Beträge hinterlegt, die in den Dokumenten herangezogen werden.

Preise legen Sie als Standard-Preislisten oder als Preislisten für bestimmte Kunden- oder Lieferantengruppen, für einzelne Kunden oder für einzelne Lieferanten fest.

Im Einkauf arbeiten Sie in der Regel nur mit einem Preisschlüssel, z. B. dem Schlüssel *EK*. Sie können aber auch im Einkaufsbereich nach verschiedenen Preisschlüsseln differenzieren.

Bei der Preisfindung wird folgende Hierarchie durchlaufen:
1.  Manuelle Preiseingaben im Auftrag oder Angebot (oberste Priorität)
2.  Objektbezogene Vereinbarungen
3.  Kunden-/lieferantenbezogene Vereinbarungen
4.  Gruppenspezifische Vereinbarungen
5.  Allgemeine Vereinbarungen

Innerhalb dieser Hierarchiestufen können allgemeine Preise, Sonderbedingungen für Warengruppen und einzelne Produkte, Austauschpreise und Zuschläge für Modelle und Sprossen hinterlegt werden.

#### Individualpreise
Bei der Gestaltung individueller Preise für Kunden und Lieferanten können Sie alle Bezugsgrößen nutzen, die auch für die allgemeinen Preislisten und Zuschläge gelten. So können Sie entweder Preistabellen für Ihre einzelnen Kunden oder Lieferanten anlegen oder die Preise im Dokument vereinbarungsgemäß anpassen.

#### Preislistenimport
Preislisten Ihrer Lieferanten können Sie importieren, wenn diese als Datei vorliegen.

> **Historie der Preisänderungen**
> Wenn Sie mit einer Gupta-Datenbank arbeiten, können Sie Änderungen der Preise in einer Historie verfolgen. Diese Funktion ist im Part *Stammdaten* beschrieben.

### Stammdaten der Preise prüfen
In Bestellungen können die Preise nur berechnet werden, wenn die Einkaufspreise korrekt sind. Im Part *Stammdaten* ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Preisen anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten Ihrer Preislisten**
1.  Wählen Sie *Stammdaten > Preise > Preise* und prüfen Sie, ob der Jahrgang, der Schlüssel und der Tarif für die Einkaufspreise (EK) richtig definiert sind.
2.  Wechseln Sie zum Dialog *Preise* und lassen Sie sich die Tabelle und den Tarif für die EK-Preise anzeigen.
    Wenn Sie die Suche nicht einschränken, werden alle Preistabellen aufgelistet.

    *Abb. D-13: EK-Preistabellen – Preisauswahl*
    *(Screenshot zeigt die Preisauswahl. A: Einzelpreisregister, B: Preistabelle.)*
    -> Stammdaten, "Preise - Preisauswahl" auf Seite B-715

3.  Markieren Sie die Preistabelle (B), die Sie prüfen wollen, und wechseln Sie zu dem Register, in dem der Preis festgelegt ist.
    In diesem Beispiel ist der Einzelpreis (A) geprüft.

    *Abb. D-14: Preisauswahl – Einzelpreis*
    *(Screenshot zeigt das Einzelpreis-Register. A: Preis, B: Preiseinheit, C: Währung.)*

    In der Übersicht sind alle Tarife der ausgewählten Preistabelle aufgeführt. Die nicht definierten Preise sind in roter Schrift angezeigt.
4.  Prüfen Sie, ob der Preis auf dem aktuellen Stand ist, oder korrigieren Sie ihn. Setzen Sie dazu den Cursor in die Zelle *Preis* und überschreiben Sie den Eintrag.
5.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Ergänzende Informationen**
*   -> Stammdaten, "Stammdaten für Preise" auf Seite B-211
*   -> Stammdaten, "Einzelpreise anlegen" auf Seite B-236
*   -> Stammdaten, "Firmendaten - Kalkulation" auf Seite B-981

## Dokumentenstatus
**Lernziele**
*   Statusumsetzung von referenzierten Dokumenten kennenlernen.
*   Statuszuordnung prüfen.

**Nutzen**
*   Statuszuordnungen für referenzierte Dokumente werden neben den Statuszuordnungen für unabhängige Dokumente gepflegt. Anhand des Status kann also erkannt werden, ob eine Bestellung referenziert ist.
*   Wareneingänge zu einer Bestellung setzen den Status des referenzierten Auftrags um. So kann am Auftrag der aktuelle Stand erkannt werden.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Statuszuordnungen** | Statuszuordnungen für referenzierte Dokumente müssen den gleichen Mindeststatus haben. |
| **Statusumsetzung** | Der Status des referenzierten Auftrags wird beim Wareneingang der Bestellung umgesetzt. |
| **Voreinstellungen** | Stammdaten: Statuszuordnung |

### Statuszuordnung
Die Einkaufsdokumente durchlaufen von der Erfassung bis zur Archivierung mehrere Programmpunkte, die jeweils durch einen Status gekennzeichnet sind. An diesen Status können Bedingungen und Sperren geknüpft sein.

Wie Sie die Statuspunkte und -zuordnungen einrichten, hängt von den Geschäftsabläufen in Ihrem Unternehmen ab. Eine ausführliche Beschreibung finden Sie dazu im Part *Stammdaten*.

*Abb. D-15: Statuszuordnung für referenzierte Dokumente*
*(Screenshot zeigt die Statuszuordnung. A: Status für Auftrag mit referenzierter Bestellung, B: Korrespondierender Status für Bestellung.)*

Statuszuordnungen werden für referenzierte Dokumente und für unabhängige Dokumente getrennt eingerichtet, z. B. für den Wareneingang.

### Statusvergabe
Der Status der Dokumente wird in der Regel umgesetzt, wenn eine Bestellung geändert, versendet usw. wird. Dabei wird unterschieden, ob die Bestellung durch einen Auftrag oder unabhängig erzeugt wurde.

**Beispiele**

| für Aufträge | für Bestellungen |
| :--- | :--- |
| 30 - Auftrag in Einkauf übergeben | |
| 31 - AB Lieferant teilweise/Auftrag | 62 - AB Lieferant teilweise/Bestellung |
| 32 - AB Lieferant komplett/Auftrag | 63 - AB Lieferant komplett/Bestellung |
| 33 - Wareneingang teilweise/Auftrag | 64 - Wareneingang teilweise/Bestellung |
| 34 - Wareneingang komplett/Auftrag | 65 - Wareneingang komplett/Bestellung |
| | 66 - Rechnungskontrolle |

Wenn im Wareneingang die Nummer der Auftragsbestätigung (AB) des Lieferanten eingegeben ist, wird der Status der Bestellung umgesetzt.

Wenn ein Wareneingang zu einer Bestellung aus einem Kundenauftrag (referenzierte Bestellung) verbucht wird, zu dem weitere Bestellungen noch offen sind, wird der Status des Auftrages auf *Wareneingang teilweise/Auftrag* gesetzt.

**Ergänzende Informationen**
*   -> Verkauf, "Status" auf Seite C-221
*   -> Stammdaten, "Geschäftsabläufe abbilden" auf Seite B-420
*   -> Stammdaten, "Statuszuordnung" auf Seite B-887

# Bestellungen
In diesem Themenblock lernen Sie, wie Sie Bestellungen erzeugen und Termine prüfen.

Dazu gehören folgende Lerneinheiten:
*   "Bestellübergabe vs. manuelle Bestellung" auf Seite D-44
*   "Bestellpositionen im Auftrag" auf Seite D-50
*   "Bestellübergabe" auf Seite D-60
*   "Manuelle Bestellung" auf Seite D-79
*   "Auftragsbestätigung des Lieferanten" auf Seite D-86
*   "Lieferterminkontrolle" auf Seite D-100
*   "Anfrage" auf Seite D-110

Üblicherweise erfassen Sie eine Bestellung in folgenden Schritten:
*   Anfrage erstellen (optional)
*   Bestellung erfassen
*   Bestellung an den Lieferanten senden
*   Auftragsbestätigung vom Lieferanten erfassen
    *   Preise prüfen
    *   Termine und Tourenplanung nach Rückmeldungen korrigieren
    *   Kunden über Terminänderungen informieren
*   Auftragsbestätigung des Lieferanten anmahnen

Diese Reihenfolge entspricht im Wesentlichen auch der Reihenfolge der Dialoganordnung in *A+W Business*. Einige der Schritte können jedoch über mehrere Dialoge ausgeführt werden. Sie sind daher in einer Lerneinheit zusammengefasst.

Die Preise können bereits auf einer Auftragsbestätigung des Lieferanten geprüft werden. In der Praxis kann durchaus vorkommen, dass Auftragsbestätigung und Lieferung zusammen mit der Rechnung eintreffen. Da die Dialoge für die Preiskontrolle und die Rechnungskontrolle identisch sind, wird das Konzept der Preis- und Rechnungskontrolle im Themenblock *Wareneingang* beschrieben.
-> "Eingangsrechnung" auf Seite D-144

Eine Anfrage wird logischerweise vor der Bestellung erstellt, sie ist jedoch nicht zwingend erforderlich. In diesem Tutorial wird die Anfrage nach den Bestellungen behandelt, weil Sie dann bereits mit allen Details der Bestellung vertraut sind.

## Bestellübergabe vs. manuelle Bestellung
**Lernziele**
*   Unterschied zwischen automatischer (referenzierter) und unabhängiger Bestellung kennenlernen.

**Nutzen**
*   Auftragspositionen, die bestellt werden müssen, können automatisch in eine (referenzierte) Bestellung geleitet werden.
*   Lagerbestände werden durch Lagerbestellungen ergänzt. Diese werden manuell erfasst. Sie können auch durch Unterschreitung von Mindestbeständen angelegt werden. (Diese Funktion ist im Part *Lagerwirtschaft* beschrieben.)

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Bestellung aus Auftrag** | Auftragspositionen, die bestellt werden müssen, werden im Bestellpool an den Einkauf übergeben. Mit der Übergabe wird automatisch eine Bestellung erzeugt. |
| **Referenzierte Bestellung** | Aus einer Auftragsposition, die an den Einkauf übergeben wurde, wird eine referenzierte Bestellung mit einer eigenen Dokumentennummer erzeugt. |
| **Unabhängige Bestellung** | Unabhängige Bestellungen werden manuell erfasst. Bei unabhängigen Bestellungen wird der Lagerbestand nicht aktualisiert, wenn der Wareneingang gebucht wird. |
| **Lagerbestellung** | Lagerbestellungen dienen dazu, den Lagerbestand aufzufüllen. Sie können manuell erfasst werden. |
| **Voreinstellungen** | **Stammdaten:**<ul><li>Lieferantendaten (Marktpartner)</li><li>Lieferantenkartei</li></ul>**Firmendaten:**<ul><li>Register *Dokumente*</li><li>Register *Parameter*</li><li>Register *Lager/EK/EDI*</li></ul> |

### Dokument Bestellung
Bestellungen können entweder auftragsabhängig oder unabhängig eingegeben werden:

*   **Auftragsabhängige (referenzierte) Bestellungen** beziehen sich auf eine Position im Kundenauftrag. Sie werden durch die Bestellübergabe erzeugt. Im Bestellpool schlägt *A+W Business* aufgrund der Daten aus der Lieferantenkartei einen Lieferanten vor.
*   **Unabhängige Bestellungen** dienen in der Regel nicht dazu, den Lagerbestand aufzufüllen, da der Wareneingang nicht automatisch den Lagerbestand aktualisiert. Sie werden manuell erfasst.
*   **Lagerbestellungen** dienen dazu, den Lagerbestand aufzufüllen. Sie können manuell erfasst oder durch Unterschreitung eines Mindestbestands erzeugt werden.

*Abb. D-16: Arten der Bestellung*
*(Diagramm zeigt, dass sowohl auftragsabhängige als auch unabhängige Bestellungen zu einem Wareneingang führen. Ein Wareneingang aus einer auftragsabhängigen Bestellung aktualisiert den zugehörigen Auftrag. Manuelle und automatische Lagerbestellungen führen ebenfalls zu einem Wareneingang, der den Lagerbestand aktualisiert.)*

In dieser vereinfachten Darstellung sehen Sie, wozu die unterschiedlichen Bestellungen erfasst werden. In den folgenden Einheiten werden die auftragsabhängigen und die unabhängigen Bestellungen ausführlich beschrieben.
Lagerbestellungen werden ausführlich im Part *Lagerwirtschaft* beschrieben.

Alle Bestellungen sind eigene Dokumente mit einem eigenen Nummernkreis. Sie werden im Dialog zur *Dokumentenverwaltung* angezeigt und können unabhängig davon, wie sie erzeugt wurden, bearbeitet werden.

*Abb. D-17: Dokument Bestellung*
*(Screenshot zeigt die Kopfdaten einer Bestellung. A: Anlieferung durch den Lieferanten, B: Zusatz-Informationen, z.B. Referenz auf Auftrag, C: Dokumententyp wie automatische/manuelle Bestellung oder Lagerbestellung.)*

Bestellungen müssen an den Lieferanten gesendet werden. Dazu steht neben dem Fax- und dem E-Mail-Versand auch die Datenübertragung über Schnittstellen zur Verfügung.

## Voreinstellungen für Bestellungen prüfen
Für die Bestellungen müssen Sie die Voreinstellungen in den Firmendaten prüfen. Im Part *Stammdaten* ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie *A+W Business* neu starten.

**So prüfen Sie die Einstellungen für Bestellungen**
1.  Wählen Sie *Stammdaten > Firma > Firmendaten*.
    Der Dialog *Firmendaten* wird geöffnet.
    -> Stammdaten, "Firmendaten" auf Seite B-918
2.  Wechseln Sie zum Register *Dokumente* und prüfen Sie die Einstellungen für den Fax- und E-Mail-Versand.

    *Abb. D-18: Firmendaten - Dokumente*
    *(Screenshot des Registers 'Dokumente'. A: Faxversand einzeln/gesammelt. B: E-Mail-Versand einzeln/gesammelt. C: Dateiformat für E-Mail-Anhang.)*

3.  Wechseln Sie zum Register *Parameter* und prüfen Sie die Einstellungen wie in der folgenden Abbildung gezeigt.

    *Abb. D-19: Firmendaten - Parameter*
    *(Screenshot des Registers 'Parameter'. A: Änderungen in einer Position in das referenzierte Dokument übernehmen. B: Bestelltexte aus dem Kundenauftrag für den openTRANS-Austausch übernehmen. C: Positionen mit Maßen über den Lagermaßen automatisch als Bestellung kennzeichnen. D: Virtuelle Positionsnummern für den Wareneingang von Kisten.)*

    Die Einstellungen werden in separaten Einheiten ausführlich beschrieben.
    *   **Checkbox A:** -> "Bestellte Auftragsposition ändern" auf Seite D-57
    *   **Checkboxen B und D:** -> "Kistengeschäft" auf Seite D-136, -> "Export/Import (openTRANS)" auf Seite D-151
    *   **Lagerbestellungen (C)** sind ausführlich im Part *Lagerwirtschaft* beschrieben.

4.  Wechseln Sie zum Register *Lager/EK/EDI* und prüfen Sie die Einstellung im Bereich *Einkauf*.

    *Abb. D-20: Firmendaten – Lager/EK/EDI*
    *(Screenshot des Registers 'Lager/EK/EDI'. A: Bestellkennzeichen bei ISO-Einheiten mit Bearbeitungen. B: Positionen aus Lagerbestellungen anzeigen, obwohl sie keine Lagerartikel sind.)*

5.  Markieren Sie die Checkbox *ISO als Bestellartikel (Bearb. können Eigenfertigung sein)* (A).
    Wenn bei Isolierglas (ISO) Bearbeitungen mit der Beschaffungsart *Produktion* (Eigenfertigung) in der Stückliste vorhanden sind, können diese mit bestellt werden. Diese Einstellung ist sinnvoll, wenn Sie ISO-Einheiten nur bei Engpässen in der Produktion bestellen.
6.  Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

## Bestellpositionen im Auftrag
**Lernziele**
*   Bestellposition erfassen und Kennzeichen zuordnen.
*   Lieferanten in der Auftragsposition ändern.
*   Lieferanten für den gesamten Auftrag ändern.
*   Bestellte Position ändern.

**Nutzen**
*   Aus Auftragspositionen können Bestellungen erzeugt werden, ohne die Positionen als Bestellung neu zu erfassen.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Bestellposition** | Bestellpositionen aus Aufträgen erzeugen pro Standard-Lieferant eine eigene Bestellung. |
| **Bestellkennzeichen** | Als Bestellkennzeichen werden folgende Beschaffungsarten bezeichnet: <ul><li>Bestellung</li><li>Bestellung (komplett)</li></ul> |
| **Bestellung (komplett)** | Dieses Kennzeichen wird bei Produkten mit Stückliste verwendet, die als Ganzes bestellt werden sollen, z. B. eine komplette Tür mit Beschlägen. |
| **Bestellung** | Dieses Kennzeichen wird bei Produkten verwendet, deren einzelne Komponenten bestellt werden sollen, z. B. nur die Beschläge. |
| **Voreinstellungen** | **Stammdaten:** <ul><li>Lieferantendaten (Marktpartner)</li><li>Lieferantenkartei</li></ul> **Firmendaten:** <ul><li>Register *Dokumente*</li><li>Register *Parameter*</li><li>Register *Lager/EK/EDI*</li></ul> |

