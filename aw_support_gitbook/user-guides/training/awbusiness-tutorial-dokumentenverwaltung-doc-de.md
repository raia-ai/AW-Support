---
title: "DE_AWBusiness_Verkauf_4_2-4"
source: "DE_AWBusiness_Verkauf_4_2-4.pdf"
tags: ["A+W Business Verkauf", "Tutorial", "Dokumentenverwaltung", "Faktura", "Nummernverwalter", "Druck", "Templates", "SN-Datei", "ERP-Software", "Software-Anleitung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial for the A+W Business Verkauf software, detailing the complete process from document creation to invoicing. It covers working with templates, using Shaping + Nesting (SN) files, managing documents with the Nummernverwalter (number manager), and various printing functionalities."
long_description: "This document is a detailed tutorial for the A+W Business Verkauf software, focusing on the end-to-end process of document management, from initial creation to final invoicing (Kompletterfassung von Dokumenten bis Faktura). The tutorial is divided into several key sections. It begins by explaining how to work with Shaping + Nesting (SN) files and templates, including steps for selecting, modifying, and saving models. It provides exercises for practical application. The next major section introduces the 'Nummernverwalter' (number manager), a tool for organizing and batch-processing documents like orders. It covers creating, filling, copying, and clearing these managers. The final extensive section is dedicated to 'Druck' (Printing), detailing how to print various documents such as order confirmations, delivery notes, and invoices. It explains settings for sketch printing, price display, direct printing, and using print jobs. The guide uses screenshots and step-by-step instructions to facilitate user learning."
---

# Kompletterfassung von Dokumenten bis Faktura - Tutorial

4. Markieren Sie die Checkbox **S+N-Datei** und klicken Sie auf das Ordner-symbol, um die Datei auszuwählen.
   Der Dialog **Shaping + Nesting - Datei auswählen** wird geöffnet.
5. Suchen Sie die Datei und übernehmen Sie diese mit **[Öffnen]**.
   Wenn diese Datei zu einem anderen Modell erstellt wurde, müssen Sie die Abfrage mit **[Ja]** bestätigen.
   Der Dialog wird geschlossen und der Dateiname wird im Feld **S+N-Datei** angezeigt. Die Darstellung und Maße werden in die zugehörigen Felder übernommen.
6. Passen Sie die Maße so an, wie der Kunde das Modell bestellt hat.
   Die grafische Darstellung wird angepasst.
   Achten Sie darauf, dass die Stücklisten in der SN-Datei und im Auftrag absolut identisch sind. Wenn Sie die Stückliste im Auftrag geändert haben, müssen Sie eine neue SN-Datei schreiben.
   Wenn die Stücklisten der Vorlage und der Position unterschiedlich sind, kann die Position in **A+W Production** nicht gefertigt werden.
7. Wählen Sie im Menü **Start > Speichern**, um die Daten zu übernehmen.
8. Wechseln Sie zum Register **Position**.
9. Wählen Sie im Menü **Start > Speichern**, um die Position zu speichern.
   Die Daten werden gespeichert.

---
## Mit Templates arbeiten

Die Namen von Template-Dateien beginnen immer mit T_. Diese Dateien können auch über das Modul Stammdaten erzeugt und bearbeitet werden.

### So übernehmen Sie ein Template

1. Wählen Sie **Dokumente > Auftrag > Auftrag auswählen > Register Positionen** oder **<F9>**.
   Die Positionserfassung wird geöffnet.
2. Erfassen Sie das Produkt und wechseln Sie zum Register **Modelle/Bearbeitungen**.
   ⇨ Softwarereferenz, "Positionen – Modelle/Bearbeitungen" auf Seite C-465
3. Tragen Sie die Modellnummer **99** ein und springen Sie mit der `<Tab>`-Taste weiter.

*(Abb. C-92 zeigt die Benutzeroberfläche zur Erfassung eines SN-Modells)*

*   **A**: Modell auswählen
*   **B**: SN-Template importieren
*   **C**: SN-Funktion freischalten

Die zugehörigen Eingabefelder werden freigeschaltet.

4. Markieren Sie die Checkbox **S+N-Datei** und klicken Sie auf das Ordner-symbol, um die Datei auszuwählen.
   Der Dialog **Datei auswählen** wird geöffnet.
5. Suchen Sie die gewünschte Template-Datei und übernehmen Sie diese mit **[Öffnen]**.
   Die Namen von Template-Dateien sind immer mit **T_** gekennzeichnet.

*(Abb. C-93 zeigt die Benutzeroberfläche zur Verwendung eines SN-Templates mit ausgefüllten Parameterwerten.)*

6. Geben Sie die Werte für die Parameter ein.
   Die grafische Darstellung wird entsprechend aktualisiert.
7. Wählen Sie im Menü **Start > Speichern**, um die Daten zu übernehmen.
   Die neuen Werte werden nicht in das Template zurückgeschrieben.
   Eine neue SN-Datei wird angelegt. Im Feld **S+N-Datei** wird der neue Dateiname angezeigt.
8. Wechseln Sie zum Register **Position**.
9. Wählen Sie im Menü **Start > Speichern**, um die Position zu speichern.
   Die Daten werden gespeichert.

## Übungen

**SN-Datei speichern**

Öffnen Sie Ihren Auftrag mit den Positionen, die Sie über die Schnellerfassung eingegeben haben.

*   Speichern Sie die Position 1 als SN-Datei.
*   Erfassen Sie eine neue Position, indem Sie die SN-Datei verwenden.

**Modell über Template erfassen**

*   Erfassen Sie eine neue Position, indem Sie eine Vorlage (Template) verwenden.
*   Passen Sie die Vorbelegungen an.
*   Speichern Sie das Modell mit den eingegebenen Maßen als SN-Datei.
*   Erfassen Sie eine neue Position, indem Sie die neue SN-Datei verwenden.
*   Bearbeiten Sie in der neuen Position die Maße.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Positionen – Modelle/Bearbeitungen" auf Seite C-465
⇨ Softwarereferenz, "Positionen – Modell-Template" auf Seite C-491

## Nummernverwalter

**Lernziele**

*   Funktion eines Nummernverwalters kennenlernen.
*   Nummernverwalter anlegen und füllen.
*   Dokument in einen Nummernverwalter kopieren.

**Nutzen**

*   Sie können den Ablauf bei der Arbeit mit Dokumenten über Nummernverwalter organisieren.
*   Funktionen können Sie für mehrere Dokumente gleichzeitig ausführen, ohne die einzelnen Dokumente zu öffnen.

**Merke**

| Thema | Beschreibung |
| :--- | :--- |
| **Organisation** | Nummernverwalter sind Organisationseinheiten, in denen Sie mehrere Dokumente sammeln, um diese gemeinsam weiter zu bearbeiten. Aufträge werden z. B. nach Lieferdatum gesammelt, um sie an die Kapazitätsplanung oder an die Produktion zu übergeben. |
| **Nummernverwalter können nicht leer sein** | Sie müssen einem neuen Nummernverwalter mindestens ein Dokument zuordnen. Ohne Dokument kann der Nummernverwalter nicht gespeichert werden. |
| **Nummernverwalter bearbeiten** | Alle Arbeiten mit den Nummernverwaltern ändern die einzelnen Dokumente nicht. |
| **Nummernverwalter in den A+W Business-Modulen** | Der Dialog **Nummernverwalter** ist für alle Dokumente gleich. |
| **Dokumente sammeln** | Funktionen für Dokumente mit identischem Status können über Nummernverwalter ausgelöst werden, z. B. der Druck von Lieferscheinen. |
| **Voreinstellungen** | Keine |

### Organisation der Dokumente

Jedes Dokument wird automatisch einem Nummernverwalter zugeordnet. Sie können unterschiedliche Nummernverwalter anlegen und z. B. bestimmten Mitarbeitern oder Arbeitsbereichen zuordnen, z. B. Auftragserfassung, Produktion, Lieferung usw. Mit den Nummernverwaltern können Sie Arbeitsabläufe im Verkauf automatisieren, z. B. Bestellaufträge erstellen oder Lieferscheine drucken.

*(Abb. C-94 zeigt die Benutzeroberfläche des Nummernverwalters.)*
*   **A**: Aktueller Nummernverwalter (NV)
*   **B**: Mitarbeiter, dem der NV zugeordnet ist
*   **C**: Liste der Nummernverwalter
*   **D**: Einstellung der Sortierung
*   **E**: Dokumente im aktuellen NV

Sie können die Arbeit mit den Nummernverwaltern so organisieren, dass Sie die Dokumente in unterschiedlichen Nummernverwaltern (C) sammeln. Die Nummernverwalter können dann in anderen Dialogen ausgewählt und die Weiterverarbeitung der Dokumente gestartet werden.

Nummernverwalter werden personengebunden angelegt und genutzt, d. h., dass jeder Mitarbeiter (B) mit seinen eigenen Nummernverwaltern arbeitet. Wenn ein Nummernverwalter von mehreren Kollegen gemeinsam genutzt werden soll, kann er für jeden einzelnen kopiert werden.

Haben Sie z. B. in einem Nummernverwalter alle Dokumente zusammengefasst, die am aktuellen Tag (heute) erfasst oder geändert wurden, so können Sie diesen Nummernverwalter im Formulardruck öffnen und den Druck der Auftragsbestätigungen für alle Dokumente gemeinsam starten.

Mit Nummernverwaltern arbeiten Sie z. B. bei folgenden Vorgängen:
*   Druck, z. B. Auftragsbestätigungen (AB), Lieferscheine, Rechnungen
*   Datenübergabe, z. B. FiBu, Bestellung, Produktion
*   Journale
*   Archivierung
*   Import von Aufträgen (EDI)
*   Bankbelege drucken
*   Bestandslisten erstellen
*   Dokumentendaten prüfen, z. B. Terminkontrolle

Ausschlaggebend für die Verarbeitung der Dokumente ist in der Regel der (gemeinsame) Status. Dokumente, die sich irrtümlich in einem Nummernverwalter befinden, werden daher nicht mit verarbeitet.

Sie können Dokumente auch in einem Nummernverwalter zusammenfassen, um in ihnen gemeinsam den Status oder das Bestellkennzeichen zu ändern.

Nummernverwalter können gelöscht werden. Die Dokumente in einem Nummernverwalter werden dabei nicht gelöscht.

### Nummernverwalter erstellen

Der Dialog Nummernverwalter ist für alle Dokumente gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.
In dieser Einheit lernen Sie, wie Sie mit Nummernverwaltern arbeiten.

**So erstellen Sie einen neuen Nummernverwalter**

1.  Wählen Sie **Dokumente > Auftrag > NV Auftrag**.
    Der Dialog **Nummernverwalter** wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

*(Abb. C-95 zeigt die freigeschalteten Felder für einen neuen Nummernverwalter.)*
*   **A**: Name des NV
*   **B**: Kriterien zur Auswahl der Dokumente

3.  Tragen Sie einen Namen (A) für den neuen Nummernverwalter ein.
4.  Ordnen Sie dem neuen Nummernverwalter mindestens ein Dokument zu.
    Sie haben die Möglichkeit, einen einzelnen Auftrag oder eine Reihe von Aufträgen auszuwählen, indem Sie in den Feldern **Auftrag** und/oder **Statusbereich** (B) die entsprechenden Daten eingeben.
    Sie können über die Suche die Aufträge auch nach selbst gewählten Kriterien auswählen, z. B. nach Kunden.
    In diesem Beispiel werden die Aufträge nach Status gesammelt.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Dokumente werden eingelesen. Der neue Nummernverwalter wird im Feld **Auswahl** aufgelistet. Die Daten werden gespeichert.

*(Abb. C-96 zeigt den neu erstellten Nummernverwalter mit einer Liste von Dokumenten.)*

Sie können Aufträge aus der Übersicht aus dem Nummernverwalter löschen. Dabei werden nicht die Aufträge gelöscht, sondern nur die Zuweisung zum Nummernverwalter.

6.  Markieren Sie den Auftrag, die Sie entfernen wollen, und drücken Sie auf `<Entf>`.

*(Abb. C-97 zeigt, wie ein Auftrag aus der Liste entfernt wird.)*

Der Auftrag wird aus der Liste entfernt. Die verbleibenden Aufträge werden mit einem Häkchen gekennzeichnet. Wiederholen Sie diesen Schritt, bis nur noch die gewünschten Aufträge angezeigt werden.

7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Der Nummernverwalter wird mit der aktuellen Liste der Aufträge gespeichert.

### Nummernverwalter kopieren

Sie können einen Nummernverwalter vollständig kopieren, z. B., um ihn einem anderen Mitarbeiter zuzuweisen.

**So kopieren Sie einen Nummernverwalter**

1.  Wählen Sie **Dokumente > Auftrag > NV Auftrag**.
    Der Dialog **Nummernverwalter** wird geöffnet.
2.  Wählen Sie im Menü **Funktionen > Gruppe Bearbeiten > Kopieren**.

*(Abb. C-98 zeigt den Dialog "Nummernverwalter kopieren".)*

3.  Wählen Sie in den Bereichen **Quelle** und **Ziel**:
    *   Den Mitarbeiter, wenn der Nummernverwalter einem bestimmten Mitarbeiter zugewiesen ist oder werden soll.
    *   Den Nummernverwalter, den Sie kopieren wollen.
4.  Tragen Sie im Bereich **Ziel** im Feld **Nummernverwalter** den Namen für den neuen Nummernverwalter ein.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Daten werden gespeichert.
6.  Klicken Sie auf **[Ende]**, um den Dialog zu schließen.
    Der Dialog **Nummernverwalter kopieren** wird geschlossen. Der neue Nummernverwalter wird im Dialog **Nummernverwalter** des entsprechenden Mitarbeiters im Feld **Auswahl** aufgelistet.

### Nummernverwalter leeren

Wenn alle Dokumente in einem Nummernverwalter abgearbeitet sind, können Sie den Nummernverwalter leeren, um anschließend darin neue Dokumente zu sammeln.

**So leeren Sie einen Nummernverwalter**

1.  Wählen Sie **Dokumente > Auftrag > NV Auftrag**.
    Der Dialog **Nummernverwalter** wird geöffnet.
2.  Markieren Sie den Nummernverwalter, den Sie leeren wollen.
3.  Wählen Sie im Menü **Funktionen > Gruppe Bearbeiten > Überschreiben**.

*(Abb. C-99 zeigt den geleerten Nummernverwalter.)*

Die Liste der Dokumente wird gelöscht.

4.  Tragen Sie im Feld **Auftrag** oder im Feld **Statusbereich** die Daten für die Zuordnung von Aufträgen ein.
    Sie müssen mindestens einen Auftrag zuordnen, damit der Nummernverwalter gespeichert werden kann.
5.  Wechseln Sie zum Menü **Start**.
6.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    In der Übersicht werden die zugeordneten Aufträge aufgelistet.

### Dokument in einen Nummernverwalter stellen

Sie können ein einzelnes Dokument in einen anderen Nummernverwalter stellen.

**So stellen Sie Dokumente in einen anderen Nummernverwalter**

1.  Wählen Sie **Dokumente > Auftrag > NV Auftrag**.
    Der Dialog **Nummernverwalter** wird geöffnet.
2.  Wählen Sie im Bereich **Auswahl** den Ziel-Nummernverwalter aus.
    In der Übersicht werden alle Dokumente angezeigt, die sich in diesem Nummernverwalter befinden.
3.  Tragen Sie in den Feldern **Auftrag von/bis** die Auftragsnummern ein, die verschoben werden sollen.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Dokumente werden in der Liste aufgeführt. Löschen Sie diese Dokumente ggf. aus dem Nummernverwalter, in dem sie sich zuvor befanden.

### Übungen

**Nummernverwalter erstellen**

Erstellen Sie einen neuen Nummernverwalter mit folgenden Dokumenten:
*   Aufträge von Nummer n bis nn.
    Wählen Sie für n die Nummer des ersten Auftrags, den Sie angelegt haben.
    Wählen Sie für nn eine beliebige höhere Nummer.
*   Status 1 bis 2.

**Nummernverwalter leeren**

*   Öffnen Sie einen Nummernverwalter und leeren Sie ihn, indem Sie Aufträge mit dem Status 30 einfügen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Statusänderung" auf Seite C-554
⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-631
⇨ Softwarereferenz, "Bestellkennzeichen ändern" auf Seite C-635

## Druck

**Lernziele**
*   Einstellungen für Skizzendruck kennenlernen.
*   Einstellungen für Preisdruck kennenlernen.
*   Auftragsbestätigungen, Lieferscheine, Rechnungen und Etiketten drucken.

**Nutzen**
*   Über das Layout von gedruckten Dokumenten müssen Sie sich keine Gedanken machen, da diese in hinterlegten Formularen gedruckt werden.
*   Preise und Skizzen können im Druck unterschiedlich dargestellt werden. Dazu lernen Sie die spezifischen Einstellungen kennen.

**Merke**

| Thema | Beschreibung |
| :--- | :--- |
| **Ausgabe** | Jeder Druck kann entweder auf dem Bildschirm ausgegeben oder an einen Drucker gesendet werden. Beide Druckmodi setzen den Status um. |
| **Formular** | Dokumente können nur gedruckt werden, wenn die zugehörigen Formulare im System hinterlegt sind. |
| **Bildschirmdruck** | Im Bildschirmdruck wird jeweils nur ein Dokument gedruckt. Nach dem Bildschirmdruck kann ein Dokument nur im Wiederholungsdruck an den Drucker gesendet werden. |
| **Druckpunkt** | Der Druckpunkt entspricht dem Statuspunkt, der programmintern genutzt wird, um ein bestimmtes Formular zu drucken. |
| **Voreinstellungen** | Stammdaten:<ul><li>Statuszuordnung</li><li>Formularverwaltung</li><li>Druckaufträge</li></ul>Firmendaten:<ul><li>Register Druck (Skizzendruck)</li><li>Register Archiv</li></ul> |

### Formular- und Etikettendruck

Für den Druck von Dokumenten werden in A+W Business Standardformulare genutzt. Die Dokumente können an einen Drucker gesendet oder als PDF-Datei auf dem Bildschirm angezeigt werden. Beide Ausgabeformen gelten als Druck.

*(Abb. C-100 zeigt die Druck-Benutzeroberfläche.)*
*   **A**: Formular, auf das gedruckt wird
*   **B**: Nummernverwalter, aus dem gedruckt wird
*   **C**: Druckmodus
*   **D**: Optionen für die Ausgabe des Drucks
*   **E**: Sonderdruck

Über den **Druckmodus** (C) legen Sie fest, was gedruckt werden soll, z. B. ein Lieferschein. Beachten Sie dabei, dass der Status den Druck einschränken kann. So kann z. B. vorgegeben sein, dass eine Rechnung erst nach dem Lieferschein gedruckt werden darf.

Die **Formulare** (A) werden in der Formularverwaltung den einzelnen Druckpunkten zugeordnet. Damit stehen sie für den Druck zum Auswählen (A) zur Verfügung. Wenn einem Druckpunkt mehrere Formulare zugeordnet sind, muss eines als Standard festgelegt sein.

Formulare werden für die unterschiedlichen Ausgabeformate hinterlegt, z. B. Auftragsbestätigungen (AB) per (Papier-) Druck, E-Mail, PDF. Das Formular selbst kann auch die Ausgabe steuern: Wenn Sie ein Dokument z. B. über den maxxPDFMailer drucken, wird es automatisch per E-Mail gesendet. Ohne diesen PDFMailer müssen Sie den Versand manuell aktivieren.

> **Kundenindividuelle Formulare**
> In Absprache mit der A+W Software GmbH können weitere Formulare zur Verfügung gestellt werden.
>
> Wenn Sie in A+W Business die Mehrsprachigkeit nutzen, werden Formulare standardmäßig in der Sprache des Kunden gedruckt. Diese Einstellung kann übersteuert werden, z. B. für Fertigungspapiere in Ihrer Landessprache.
> Für jedes Formular können Sie einen eigenen Text verfassen, der standardmäßig mit der E-Mail verschickt wird. Die PDF-Ausgabe erfolgt über den Standard-Formulardruck in A+W Business.

### Druckmodus im Nummernverwalter

Den Druck selbst steuern Sie aus den Dokumenten oder Nummernverwaltern heraus. Dabei entscheiden Sie, welches Formular und welches Ausgabefor-mat verwendet wird. Zu dem Druckauftrag legen Sie auch die Versandform fest, z. B. per Fax oder E-Mail.

Mit der Wahl des Druckmodus wird automatisch das zugehörige Standard-Formular ausgewählt. Folgende Druckmodi stehen zur Verfügung:
*   Auftragsbestätigung (Auftrag)
*   Fertigungsschein
*   Lieferschein
*   Rechnung
*   Sonstige

Nach dem Druck einer Rechnung wird das Dokument in der Regel gesperrt. Es kann dann nicht mehr bearbeitet werden.

*(Abb. C-101 zeigt die Formularauswahl für den Wiederholungsdruck.)*
*   **A**: Formularauswahl für Wiederholungsdruck
*   **B**: Einstellung Wiederholungsdruck

Standardmäßig wird beim Druck eines Dokuments der Status hochgesetzt. Soll ein Dokument erneut gedruckt werden, muss der Druckpunkt für den **Wiederholungsdruck (B)** ausgewählt werden. Dadurch werden die möglichen **Formulare (A)** zur Auswahl angeboten.

> **Erstdruck kann nur einmal gestartet werden**
> Sie können ein Dokument nur einmal auf einem (Original-) Formular drucken. Wenn es erneut gedruckt werden soll, müssen Sie einen Wiederholungsdruck starten. Dabei spielt es keine Rolle, ob der Erstdruck auf dem Drucker oder auf dem Bildschirm ausgegeben wurde.
> Nur wenn Sie ein Dokument in der Dokumentenansicht geöffnet haben und drucken, wird der Status nicht hochgesetzt. Das Dokument wird in diesem Fall jedoch nicht als Formular gedruckt.

Üblicherweise wird der Druck aus einem Nummernverwalter heraus gestartet. Die Dokumente werden vor dem Druckbeginn gesperrt. Falls eine Sperre nicht ausgeführt werden kann, können Sie entscheiden, ob der Druck dennoch begonnen wird. Kann ein Dokument wegen eines mangelhaften Status nicht gedruckt werden, wird dies vor Druckbeginn angezeigt.

Die Anzahl der nicht verarbeiteten Dokumente wird in einer Meldung angezeigt. Die nicht gedruckten Dokumente werden in der Übersicht im Zeilenkopf markiert. Sie müssen bearbeitet werden, damit sie gedruckt werden können.

### Rechnungsdruck

Der Auftrag erhält mit dem Rechnungsdruck eine Rechnungsnummer. Dabei ist es unerheblich, ob die Druckfunktion auf den Drucker geleitet wurde oder eine PDF-Datei (Bildschirmausgabe) erstellt wurde.

Die Rechnungs- und die Anlieferpauschale werden vor dem Druckbeginn in die Dokumente eingefügt. Bei Sammelrechnungen wird vor dem Druckbeginn die Steuerkorrektur ausgeführt.

Bei Teillieferungen mit Teilfakturierung und bei Anzahlungen wird die Abschlussrechnung aus dem Original-Auftrag gedruckt. Dabei wird nach dem Druck der einzelnen Positionen die Auftragssumme gebildet, die aus dem Nettobetrag, der MwSt. und dem Bruttobetrag besteht. Danach werden alle erstellten Anzahlungsrechnungen und Teilrechnungen mit ihren Einzelbeträgen (Nettobeträgen, der jeweiligen MwSt. und dem Bruttobetrag) und schließlich die verbleibende Rechnungsendsumme gedruckt.

Anhand der Rechnungsnummer kann geprüft werden, ob für das Dokument bereits eine Rechnung erstellt wurde. Dokumente mit einer Rechnungsnummer können für die Bearbeitung gesperrt werden. Das Dokument kann auch dann nicht mehr bearbeitet werden, wenn der Status geändert wird.

> **Rechnung schützen**
> PDF-Dokumente können mit einer digitalen Signatur oder mit Sicherheitsoptionen gespeichert werden. So können z. B. PDF-Dokumente durch ein Kennwort für Bearbeitungen gesperrt werden. Dies ist beim Versand von Rechnungen ein wichtiges Kriterium.

### Direktdruck

In den Stammdaten können Sie Formular-Einstellungen für den Direktdruck einzelner Dokumente festlegen. Diese werden in den Dialogen für ein Dokument jeweils im Menü **Start > Druck > Direktdruck** im Dialog **Formularauswahl** aufgelistet. Sie stehen nur dort zur Verfügung und vereinfachen den Druck, denn die Einstellungen müssen nicht über den allgemeinen Formulardruck gewählt werden.

*(Abb. C-102 zeigt Beispiele für den Direktdruck im Menü.)*

Mit der Wahl eines definierten Direktdrucks werden verschiedene Zuordnungen übernommen, z. B.:
*   Formular und Sprache
*   Kopf- und Fußtext
*   Skizzendruck
*   Preisdruck

### Druckauftrag

Wenn Sie mit einem zentralen Kommunikationsserver/Printserver arbeiten, können Sie in den Stammdaten Druckaufträge festgelegen. Dabei können Sie mehrere Ausgabeprozesse (Druckläufe) hintereinanderschalten, z. B.:
*   Drucken der Auftragsbestätigungen für interne Zwecke.
*   Auftragsbestätigungen als Wiederholungsdruck per Fax an die Kunden senden.
*   Auftragsbestätigungen als Wiederholungsdruck per E-Mail an den Vertreter senden.

### Einstellungen zu den Darstellungen im Druck

Im Formulardruck können Sie verschiedene Details zu Preisen und Stücklisten darstellen lassen.

**Zwischensummen**
Auftragspositionen können zu Gruppen zusammengefasst werden. Im Druck wird nach der Gruppe eine Zwischensumme eingefügt.

**Stückliste**
Die Stückliste kann wahlweise gedruckt werden. Dazu muss in der Produktverwaltung der Druck zugelassen werden.
Wenn Sie die Druckoptionen flexibel halten möchten, müssen Sie die allgemeine Einstellung in der Formularverwaltung so wählen, dass jeweils das Druckkennzeichen aus dem Auftrag ausschlaggebend ist.
Im Dokument selbst können Sie pro Stücklisten-Komponente festlegen, ob diese in der gedruckten Stückliste aufgeführt werden soll oder nicht.
In den Firmendaten legen Sie außerdem fest, wie viele Komponenten einer Stückliste maximal gedruckt werden. Diese Einstellung gilt pro Position eines Auftrags. Wenn in einer Stückliste mehr Komponenten enthalten sind, wird nur die festgelegte Höchstzahl gedruckt. Nicht gedruckte Stücklisten-Komponenten fließen dessen ungeachtet in die Preisberechnung ein und werden an die Produktion übergeben.

### Druck von Skizzen

Die Anzeige und der Druck der Skizzen werden in verschiedenen Dialogen festgelegt:
*   **Firmendaten:** Die Einstellungen legen fest, wie Sprossenskizzen standardmäßig gedruckt werden sollen.
*   **Formularverwaltung:** Die Einstellungen legen die Details des Skizzendrucks für Modelle und Sprossenkonstruktionen fest.
*   **Produktverwaltung:** Die Einstellungen legen für Modelle und Sprossenkonstruktionen fest, ob Skizzen gedruckt werden. Dabei kann zwischen maßstäblicher und schematischer Darstellung gewählt werden.
*   **Positionserfassung:** Die Einstellungen legen für Modelle und Sprossenkonstruktionen getrennt fest, ob und wie Skizzen gedruckt werden sollen. Dabei kann pro Position zwischen maßstäblicher und schematischer Darstellung gewählt werden.

Beim Skizzendruck wird zwischen Modell- und Sprossenskizzen unterschieden.
*   Sprossenaufbau
*   Modelle
*   Gebogenes Glas

Modell- und Sprossenskizzen können entweder maßstäblich oder schematisch gedruckt werden. Die Wölbung von gebogenem Glas wird immer schematisch dargestellt. Im Formulardruck können Sie außerdem die Größe der gedruckten Modellskizze definieren.
Wenn Skizzen maßstäblich gedruckt werden, sind auch die Maße in der Skizze dargestellt. Die Position der Maße in der Skizze können Sie in der Vorlage bearbeiten, damit diese im Druck deutlich zu erkennen sind.

#### Skizzendruck bei Rechteckscheiben

| Einstellung in der Position | Einstellung in der Formularverwaltung: kein Druck | Einstellung in der Formularverwaltung: schematisch | Einstellung in der Formularverwaltung: maßstäblich |
| :--- | :--- | :--- | :--- |
| **maßstäblich** | kein Druck | kein Druck | maßstäblich |
| **schematisch** | kein Druck | schematisch | schematisch |
| **kein Druck** | kein Druck | kein Druck | kein Druck |
| **Sprosse maßstäblich** | kein Druck | kein Druck | Sprosse maßstäblich |
| **Sprosse schematisch** | kein Druck | schematisch | Sprosse schematisch |

#### Skizzendruck bei Modellscheiben

| Einstellung in der Position | Einstellung in der Formularverwaltung: kein Druck | Einstellung in der Formularverwaltung: schematisch | Einstellung in der Formularverwaltung: maßstäblich |
| :--- | :--- | :--- | :--- |
| **maßstäblich** | kein Druck | schematisch | maßstäblich |
| **schematisch** | kein Druck | schematisch | schematisch |
| **kein Druck** | kein Druck | kein Druck | kein Druck |
| **Sprosse maßstäblich** | kein Druck | kein Druck | kein Druck |
| **Sprosse schematisch** | kein Druck | kein Druck | kein Druck |

In diesen Tabellen sehen Sie, dass Sprossen in einer Rechteckscheibe nur dann maßstäblich gedruckt werden, wenn sowohl im Dokument als auch in der Formularverwaltung der maßstäbliche Druck eingestellt ist.
Sprossen in einer Modellscheibe werden nie gedruckt.

### Vermaßte Skizze

Mit der Funktion **Vermaßte Skizze drucken** können Sie maßstäbliche Skizzen von Modellen und Sprossen auf ein separates Blatt zu drucken, z. B. für Produktionspapiere oder Ladelisten.

Mit der Einstellung **Sonderdruck > Erweitert** können Sie die Modellskizze auf das entsprechende Formular drucken.

Um vermaßte Skizzen zu nutzen, muss in den Firmendaten die Funktion aktiviert sein.
*(Abb. C-103 Firmendaten – Register Druck: zeigt eine Checkbox "Erweiterte Sprossenskizze im Formulardruck", die aktiviert ist.)*

Im Dialog **Vermaßte Skizze drucken** werden nur die Positionen angezeigt, in denen der Skizzendruck von Modellen oder Sprossen auf maßstäblich gesetzt ist.

*(Abb. C-104 Maßstäbliche Skizzen drucken: zeigt die Benutzeroberfläche zum Drucken von vermaßten Skizzen.)*
*   **A**: Positionen mit Sprossen markieren
*   **B**: Positionen mit Modell markieren
*   **C**: Details zu Sprossen
*   **D**: Produktskizze
*   **E**: Erweiterte Modellskizze

Über die Schaltflächen A und B können Sie die Positionen markieren, in denen Sprossen oder Modelle enthalten sind.

Wenn Sie Details zu den Sprossen (C) aktiviert haben, werden zusätzlich die Stückliste und Angaben zu den Sprossen gedruckt.

*(Abb. C-105 zeigt Beispiele für den Druck von vermaßten Skizzen.)*
*   **A**: Sprossenskizze
*   **B**: Sprossenzuschnittsliste
*   **C**: Modellskizze

Die **Produktskizze** (D) wird als Datei am Produkt angehängt. Sie können in der Produktverwaltung jedem Produkt eine Abbildung als Anhang hinzufügen. Die Abbildung kann nur gedruckt werden, wenn in der Produktverwaltung die Checkbox **Druck auf Formular** aktiviert ist.

*(Abb. C-106 Produktverwaltung - Register Produkt: zeigt die Einstellung für die Artikelskizze mit der Checkbox "Druck auf Formular".)*

Die Abbildung gibt das Produkt selbst wieder. Es zeigt weder das Modell noch die eingebauten Sprossen. Es ist daher nur für seltene Strukturgläser sinnvoll.

Das Bild kann ebenfalls auf Formulare gedruckt werden. Dazu muss die Checkbox (D) markiert sein.

### Darstellung der Preise im Druck

Die Darstellung der Preise im Formulardruck wird unabhängig davon eingestellt, wie die Preise berechnet werden. Grundsätzlich kann ein Preis nur dann aus den Stammdaten übernommen werden, wenn in der Produktverwaltung das Kennzeichen **Preisrelevant** gesetzt ist.

*(Abb. C-107 Preiskennzeichen in den Produktstammdaten: zeigt die Checkboxen "Preisrelevant VK", "Preisrelevant EK", "Rabattfähig", "Skontofähig".)*

Der Druck der Preise im Formular wird in verschiedenen Dialogen festgelegt:
*   **Formularverwaltung:** Die Einstellungen gelten übergreifend und legen fest, ob die Einstellung zum Preisdruck aus dem Dokument übernommen wird.
*   **Partnerverwaltung:** Die Einstellungen werden im Dokument vorgeschlagen und können überschrieben werden.
*   **Produktverwaltung:** Die Preise von Stücklisten-Komponenten können explizit oder implizit dargestellt werden.
*   **Dokumentenverwaltung:** Die Einstellung wird nur übernommen, wenn dies durch die Einstellung in der Formularverwaltung zugelassen ist.

Neben den Einstellungen zum Druck können Sie auch festlegen, ob Netto- oder Bruttopreise gedruckt werden sollen.

Eine Erklärung zur Anzeige der Preise im Dialog finden Sie unter:
⇨ "Anzeige der Preise im Dialog" auf Seite C-138
