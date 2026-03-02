---
description: "DE_AWEnterprise_Preise_Konditionen_2.20"
---


# A+W Preise und Konditionen C

**A+W Enterprise**

A+W - Software for Glass, Windows and Doors

---

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 2.20 / 02-2023 | Div. Feldbeschreibungen aktualisiert |
| 2.10 / 05-2019 | Vollständige Überarbeitung der Softwarereferenz |
| 2.00 / 07-2018 | Ersterstellung Tutorial. |
| 1.01 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 1.00 / 10-2016 | Preise und Konditionen aus Part Stammdaten ausgegliedert. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakt

### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Enterprise gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.
Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte

**A+W Software GmbH**
Am Pfahlgraben 4-10
35415 Pohlheim
+49 6404 2051-0
+49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

---

## Inhalt

- **Vorspann**
  - [Revisionsübersicht](#revisionsübersicht) (C-3)
  - [Editorial](#editorial) (C-3)
- [Inhalt](#inhalt) (C-5)
- **Tutorial** (C-11)
  - **Einführung** (C-13)
    - [Dokumentation](#dokumentation) (C-14)
    - [Aufbau des Tutorials](#aufbau-des-tutorials) (C-14)
    - [Darstellungskonventionen](#darstellungskonventionen) (C-15)
    - [Menü-Übersicht](#menü-übersicht) (C-16)
    - [Grundgedanken der Preisermittlung](#grundgedanken-der-preisermittlung) (C-17)
    - [Charakteristika von Preisen und Konditionen](#charakteristika-von-preisen-und-konditionen) (C-19)
    - [Preisberechnung im Auftrag](#preisberechnung-im-auftrag) (C-20)
    - [Artikelstammdaten](#artikelstammdaten) (C-21)
    - [ISO- und PKZ-Preise](#iso--und-pkz-preise) (C-22)
  - **Preisdefinitionen** (C-24)
    - [Preisschlüssel](#preisschlüssel) (C-25)
    - [Preislistenkennzeichen (PLKZ)](#preislistenkennzeichen-plkz) (C-26)
    - [Preiskennzeichen (PKZ)](#preiskennzeichen-pkz) (C-27)
    - [Preisschlüssel für Matrizen, Vektoren und Listen](#preisschlüssel-für-matrizen-vektoren-und-listen) (C-31)
    - [Preisschlüssel für Sprossen](#preisschlüssel-für-sprossen) (C-33)
    - [Währungen](#währungen) (C-34)
    - [PLKZ-Logiken](#plkz-logiken) (C-36)
    - [Ab-PLKZ-Logik](#ab-plkz-logik) (C-38)
    - [Nur-PLKZ Logik](#nur-plkz-logik) (C-39)
    - [Basis-PLKZ mit Ab-PLKZ-Logik](#basis-plkz-mit-ab-plkz-logik) (C-40)
    - [Basis-PLKZ ohne Ab-PLKZ-Logik](#basis-plkz-ohne-ab-plkz-logik) (C-40)
    - [Preislistensteuerung](#preislistensteuerung) (C-41)
    - [Komponenten der Preisberechnung](#komponenten-der-preisberechnung) (C-44)
    - [Preismethoden](#preismethoden) (C-45)
    - [Rundungsmethoden (Preisberechnung)](#rundungsmethoden-preisberechnung) (C-46)
    - [Preisrelevante Menge](#preisrelevante-menge) (C-49)
    - [Preisarten](#preisarten) (C-50)
    - [Preistyp](#preistyp) (C-52)
    - [Mengenberechnung nach GME](#mengenberechnung-nach-gme) (C-53)
    - [Schlüssel anlegen](#schlüssel-anlegen) (C-55)
    - [Übungen](#übungen-preisdefinitionen) (C-57)
  - **Stammdaten für Preise** (C-58)
    - [Workflow: Preise anlegen](#workflow-preise-anlegen) (C-59)
    - [Preismatrizen für ISO-Scheiben](#preismatrizen-für-iso-scheiben) (C-60)
    - [Matrix-Editor](#matrix-editor) (C-62)
    - [Preismatrix für ISO-Scheiben anlegen](#preismatrix-für-iso-scheiben-anlegen) (C-66)
    - [Grundpreise für ISO-Scheiben](#grundpreise-für-iso-scheiben) (C-71)
    - [Übungen](#übungen-preismatrizen) (C-73)
    - [Preisvektoren](#preisvektoren) (C-74)
    - [Vektorpreise](#vektorpreise) (C-76)
    - [Vektorzuordnung](#vektorzuordnung) (C-80)
    - [Artikelpreise anlegen](#artikelpreise-anlegen) (C-81)
    - [Bearbeitungspreis anlegen](#bearbeitungspreis-anlegen) (C-87)
    - [Grundpreise für VSG-Scheiben](#grundpreise-für-vsg-scheiben) (C-90)
    - [Übungen](#übungen-preisvektoren) (C-91)
    - [Austausch- und Zusatzpreise](#austausch--und-zusatzpreise) (C-92)
    - [Austausch-/Zusatzlisten](#austausch-zusatzlisten) (C-93)
    - [Austauschpreise für Gussglas](#austauschpreise-für-gussglas) (C-95)
    - [Austauschpreise anlegen](#austauschpreise-anlegen) (C-97)
    - [Sprossenpreise](#sprossenpreise) (C-104)
    - [Definitionsschema für Sprossenpreise](#definitionsschema-für-sprossenpreise) (C-105)
    - [Sprossenpreis anlegen](#sprossenpreis-anlegen) (C-107)
    - [Zuschläge](#zuschläge) (C-110)
    - [Zuschlagsarten](#zuschlagsarten) (C-111)
    - [Modellzuschläge](#modellzuschläge) (C-111)
    - [Zuschlagsmatrix](#zuschlagsmatrix) (C-114)
    - [Größenzuschläge](#größenzuschläge) (C-116)
    - [Bearbeitungsgruppenzuschläge](#bearbeitungsgruppenzuschläge) (C-119)
    - [Stufenzuschläge](#stufenzuschläge) (C-120)
    - [Übungen](#übungen-zuschläge) (C-121)
    - [Globale Preisänderungen](#globale-preisänderungen) (C-122)
  - **Konditionen** (C-123)
    - [Prioritäten der Konditionsermittlung](#prioritäten-der-konditionsermittlung) (C-124)
    - [Komponenten der Konditionen](#komponenten-der-konditionen) (C-128)
  - **Stammdaten für Konditionen** (C-130)
    - [Allgemeine und spezielle Konditionen](#allgemeine-und-spezielle-konditionen) (C-131)
    - [Allgemeine Tageskonditionen](#allgemeine-tageskonditionen) (C-133)
    - [Warengruppen-Konditionen](#warengruppen-konditionen) (C-136)
    - [Artikelkonditionen](#artikelkonditionen) (C-138)
    - [Rabattstaffeln](#rabattstaffeln) (C-139)
    - [Spezielle Faktoren](#spezielle-faktoren) (C-140)
    - [Zuschläge für Modelle, SZR](#zuschläge-für-modelle-szr) (C-143)
    - [SZR-Zuschläge anlegen](#szr-zuschläge-anlegen) (C-144)
    - [Spezielle Preise](#spezielle-preise) (C-147)
    - [Spezielle Preise für Artikel und Farbartikel](#spezielle-preise-für-artikel-und-farbartikel) (C-149)
    - [Spezielle Preise für ISO-Einzelscheibenpreise](#spezielle-preise-für-iso-einzelscheibenpreise) (C-150)
    - [Komplexübung](#komplexübung) (C-153)
  - **Kostenkalkulation** (C-154)
    - [Materialkosten](#materialkosten) (C-156)
    - [Zusammenhang von Beschaffungsart und Kostenkalkulation](#zusammenhang-von-beschaffungsart-und-kostenkalkulation) (C-160)
- **Softwarereferenz** (C-161)
  - [Übersicht](#übersicht) (C-163)
  - [Menü Preise](#menü-preise) (C-164)
    - [Untermenü ISO-Preise](#untermenü-iso-preise) (C-164)
    - [Untermenü PKZ-Preise](#untermenü-pkz-preise) (C-165)
    - [Untermenü Zuschläge](#untermenü-zuschläge) (C-165)
    - [Untermenü Preisschlüssel](#untermenü-preisschlüssel) (C-166)
    - [Untermenü Preissteuerung](#untermenü-preissteuerung) (C-166)
  - [Menü Konditionen](#menü-konditionen) (C-167)
    - [Untermenü Spezielle Konditionen](#untermenü-spezielle-konditionen) (C-167)
    - [Untermenü Spezielle Preise](#untermenü-spezielle-preise) (C-168)
  - [Preisschlüssel](#preisschlüssel-softwarereferenz) (C-169)
    - [Preislisten (PLKZ)](#preislisten-plkz) (C-170)
    - [Preiskennzeichen (PKZ)](#preiskennzeichen-pkz-softwarereferenz) (C-171)
    - [Matrizen](#matrizen) (C-172)
    - [Austausch-/Zusatzlisten](#austausch-zusatzlisten-softwarereferenz) (C-173)
    - [Artikelvektoren](#artikelvektoren) (C-174)
    - [Bearbeitungsvektoren](#bearbeitungsvektoren) (C-175)
    - [Sprossenpreiskennzeichen](#sprossenpreiskennzeichen) (C-176)
    - [Sprossenpreisklassen](#sprossenpreisklassen) (C-177)
  - [Preise](#preise-softwarereferenz) (C-178)
    - [Globale Preispflege](#globale-preispflege) (C-179)
    - [Matrizen exportieren](#matrizen-exportieren) (C-183)
  - [ISO-Preise](#iso-preise-softwarereferenz) (C-184)
    - [ISO-Grundpreise](#iso-grundpreise) (C-185)
    - [Preise für ISO-Einzelscheiben](#preise-für-iso-einzelscheiben) (C-191)
    - [Matrix-Editor](#matrix-editor-softwarereferenz) (C-196)
    - [Matrix-Grenzmaße](#matrix-grenzmaße) (C-200)
    - [Matrix-Flächengrenzmaße](#matrix-flächengrenzmaße) (C-202)
    - [Matrix-Übernahme](#matrix-übernahme) (C-204)
    - [Matrixberechnung](#matrixberechnung) (C-205)
    - [Gussglas-Klassen](#gussglas-klassen) (C-208)
    - [Gussglas-Austauschpreise](#gussglas-austauschpreise) (C-209)
    - [ESG/VSG/Sonder Austauschpreise](#esgvsgsonder-austauschpreise) (C-211)
    - [SZR-Zuschläge](#szr-zuschläge) (C-217)
    - [UV-Abdeckung](#uv-abdeckung) (C-219)
  - [PKZ-Preise](#pkz-preise-softwarereferenz) (C-222)
    - [Artikelvektoren](#artikelvektoren-softwarereferenz) (C-223)
    - [Spezielle Artikelvektoren](#spezielle-artikelvektoren) (C-230)
    - [Artikel-Vektor-Zuordnung](#artikel-vektor-zuordnung) (C-232)
    - [Spezielle Artikel-Vektor-Zuordnung](#spezielle-artikel-vektor-zuordnung) (C-233)
    - [Bearbeitungsvektoren](#bearbeitungsvektoren-softwarereferenz) (C-234)
    - [Spezielle Bearbeitungsvektoren](#spezielle-bearbeitungsvektoren) (C-239)
    - [Bearbeitung-Vektorzuordnung](#bearbeitung-vektorzuordnung) (C-242)
    - [Bearbeitung-Matrixzuordnung](#bearbeitung-matrixzuordnung) (C-243)
    - [Mindestbearbeitungspreise](#mindestbearbeitungspreise) (C-245)
    - [VSG-Grundpreise](#vsg-grundpreise) (C-247)
    - [Spezielle VSG-Grundpreise](#spezielle-vsg-grundpreise) (C-251)
    - [VSG-Austausch-/Zusatzpreise](#vsg-austausch-zusatzpreise) (C-253)
    - [PKZ-Preise für farbige Artikel](#pkz-preise-für-farbige-artikel) (C-258)
    - [Spezielle PKZ-Preise für farbige Artikel](#spezielle-pkz-preise-für-farbige-artikel) (C-263)
    - [Variantenpreise](#variantenpreise) (C-265)
    - [Spezielle Variantenpreise](#spezielle-variantenpreise) (C-269)
    - [PKZ-Verglasungspreise](#pkz-verglasungspreise) (C-271)
    - [Sprossenpreise](#sprossenpreise-softwarereferenz) (C-274)
  - [Zuschläge](#zuschläge-softwarereferenz) (C-281)
    - [Modellzuschläge](#modellzuschläge-softwarereferenz) (C-282)
    - [Spezielle Modellzuschläge](#spezielle-modellzuschläge) (C-286)
    - [Zuschlagsmatrizen](#zuschlagsmatrizen) (C-288)
    - [Dickenzuschlagsvektoren](#dickenzuschlagsvektoren) (C-291)
    - [Größenzuschläge](#größenzuschläge-softwarereferenz) (C-293)
    - [Bearbeitungsgruppenzuschläge](#bearbeitungsgruppenzuschläge-softwarereferenz) (C-299)
  - [Preissteuerung](#preissteuerung-softwarereferenz) (C-301)
    - [Regelwerk VK-EK-Faktor](#regelwerk-vk-ek-faktor) (C-304)
    - [Bonusregelwerk](#bonusregelwerk) (C-305)
    - [Preislisten-Steuerung](#preislisten-steuerung-softwarereferenz) (C-306)
    - [Preislisten-Schranken](#preislisten-schranken) (C-307)
  - [Konditionen](#konditionen-softwarereferenz) (C-308)
    - [Tageskonditionen](#tageskonditionen) (C-309)
    - [Warengruppenkonditionen](#warengruppenkonditionen) (C-317)
    - [Spezielle Konditionen](#spezielle-konditionen) (C-323)
    - [Rabattstaffeln](#rabattstaffeln-softwarereferenz) (C-350)
    - [Warengruppenfaktoren](#warengruppenfaktoren) (C-352)
    - [Artikelfaktoren](#artikelfaktoren-softwarereferenz) (C-355)
    - [Sprossenfaktoren](#sprossenfaktoren) (C-358)
    - [Modellzuschläge](#modellzuschläge-softwarereferenz-2) (C-361)
    - [SZR-Zuschläge](#szr-zuschläge-softwarereferenz) (C-365)
    - [Austauschlistenfaktoren](#austauschlistenfaktoren) (C-369)
    - [ISO-Einzelscheiben-Konditionen](#iso-einzelscheiben-konditionen) (C-373)
  - [Spezielle Preise](#spezielle-preise-softwarereferenz) (C-379)
    - [Artikelpreise](#artikelpreise) (C-380)
    - [Spezielle Preise für Artikelvarianten](#spezielle-preise-für-artikelvarianten) (C-388)
    - [Preise für farbige Artikel](#preise-für-farbige-artikel) (C-393)
    - [Sprossenpreise](#sprossenpreise-softwarereferenz-2) (C-399)
    - [Bearbeitungspreise](#bearbeitungspreise) (C-404)
    - [ISO-Austauschpreise](#iso-austauschpreise) (C-411)
    - [Spezielle Preise für ISO-Einzelscheiben](#spezielle-preise-für-iso-einzelscheiben) (C-418)
    - [Spezielle ISO-Grundpreise](#spezielle-iso-grundpreise) (C-423)
    - [UV-Abdeckungspreise](#uv-abdeckungspreise) (C-432)
    - [Verglasungspreise](#verglasungspreise) (C-436)
    - [Austauschpreise Gussklassen](#austauschpreise-gussklassen) (C-440)
    - [Spezielle VSG-Austausch-/Zusatzpreise](#spezielle-vsg-austausch-zusatzpreise) (C-444)
- **Partindex** (C-451)
- [Index](#index) (C-453)

---

## Tutorial

### Einführung

Das Tutorial zum Modul Preise und Konditionen beschäftigt sich mit den Grundlagen der Preisberechnung in A+W Enterprise. Das Tutorial baut auf den Kenntnissen zu den Artikel-Stammdaten auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

**Themenblöcke**
In diesem Tutorial finden Sie folgende Themenblöcke:
- "Grundgedanken der Preisermittlung" auf Seite C-17
- "Preisdefinitionen" auf Seite C-24
- "Stammdaten für Preise" auf Seite C-58
- "Konditionen" auf Seite C-123
- "Stammdaten für Konditionen" auf Seite C-130
- "Komplexübung" auf Seite C-153

**Vorausgesetzte Kenntnisse**
Das Tutorial richtet sich an Anwender, die in A+W Enterprise die Stammdaten für die Preisberechnung verwalten.
Die Teilnehmer müssen das Konzept der allgemeinen Stammdaten und die Bedienelemente kennen, mit denen Funktionen aufgerufen und gestartet werden. Die Grundlagen der Bedienung sind im Part Überblick beschrieben.

**Ziel des Tutorials**
- Unterschied zwischen Preisen und Konditionen verstehen.
- Preise und Konditionen in den Stammdaten bearbeiten und definieren.
- Preisermittlung der Auftragserfassung nachvollziehen.

### Dokumentation

Für das Modul Preise und Konditionen stehen folgende Dokumente zur Verfügung:

| Format | Umfang |
| :--- | :--- |
| PDF | Vollständige Unterlagen<br>- Tutorial<br>- Softwarereferenz |
| Online-Hilfe <F1> | Kontextsensitive Dialog-Hilfe der A+W Enterprise-Softwarereferenz und des Tutorials. |

### Aufbau des Tutorials

Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - Lernziele: Was soll vermittelt werden?
  - Nutzen: Wofür können Sie dieses Wissen einsetzen?
  - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen, mit denen Sie die beschriebenen Handlungssequenzen anwenden können.

**Lesehinweis**
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.
Beachten Sie auch, dass die einzelnen Dialoge in der Softwarereferenz beschrieben sind. Auf diese Beschreibungen wird nicht im Einzelnen hingewiesen.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

- *Kursiv*: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog Preiseigenschaften.
- **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **5** ein.
- **>**: Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. **Stammdaten > Preise > ISO-Preise**.
- **[]**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten.
- **< >**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit **<F1>** öffnen Sie die Online-Hilfe.

### Menü-Übersicht

In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

**Abb. C-1: Menüs Preise, Konditionen**

