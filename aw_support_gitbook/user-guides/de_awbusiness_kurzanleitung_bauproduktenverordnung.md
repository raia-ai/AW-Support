---
description: "DE AWBusiness Kurzanleitung Bauproduktenverordnung"
---



# DE AWBusiness Kurzanleitung Bauproduktenverordnung

Umsetzung der Bauproduktenverordnung
in A+W Business




                                deutsch
    Editorial
    Anmerkungen zu diesem Dokument
    Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht. Diese Dokumentation und die da-
    rin beschriebene Software werden nur in Lizenz vergeben und dürfen nur gemäß dieser Lizenz verwendet und kopiert
    werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert
    werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem
    können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler
    oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln. Dieses Dokument
    beschreibt die volle Ausbaustufe von A+W Business in Verbindung mit A+W Production.

    Die A+W Software GmbH übernimmt keine Haftung für Datenfehler, welche auf den Grundlagen der von Microsoft oder
    Unix zur Verfügung gestellten Standardfunktionalitäten beruhen.


    Urheberrechte
    © 2013, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, blei-
    ben vorbehalten. Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivie-
    rungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Geneh-
    migung der A+W Software GmbH darf die Dokumentation weder elektronisch, noch mechanisch, per Aufzeichnung oder
    in sonstiger Form an Dritte übertragen werden.


    Warenzeichen
    Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken
    oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.



    Value+
                                                                                                             +
    Die Nutzungserlaubnis dieser Funktionen und Leistungen wird nur in Verbindung mit einem gültigen value -Vertrag
    oder einer gesonderten individual-vertraglichen Vereinbarung erteilt. Wir behalten uns die Möglichkeit eines Li-
    zenz- und Nutzungsaudits vor.


    Sollten Sie hierzu Fragen haben, wenden Sie sich bitte an Ihren zuständigen Ansprechpartner im A+W Vertrieb
    oder informieren Sie sich auf unserer Homepage http://www.a-w.com/.

                                          A+W Software GmbH  Konrad-Adenauer-Straße 15
                                          35440 Linden  Germany
                                          Tel. +49 6403 970-0  Fax +49 6403 64390
                                          www.a-w.com  zentrale@a-w.com
                                  2013 A+W Software GmbH
Inhaltsverzeichnis

Editorial                                                  2
   Anmerkungen zu diesem Dokument                           2
   Urheberrechte                                            2
   Warenzeichen                                             2
         +
   Value                                                    2

Inhaltsverzeichnis                                         3
Rechtlicher Hintergrund und Motivation                     4
Anlegen und Verwalten der Stammdaten                       6
   Verwaltung und Registrierung von Leistungserklärungen    6
   Modul Utilities                                          9
   Firmenstammdaten                                         9
   Produktstammdaten                                       10
   Stammdaten Marktpartner                                 12
   Formularverwaltung                                      13
   Rechteverwaltung                                        14

Anwendung in der Dokumentenverwaltung                      15
Formulardruck                                              17
Produktionsübergabe                                        18
Best Practise – Registrieren und Verwalten der LE          20
   Anlage der Stammdaten                                   20
   Zuordung der Leistungserklärungen                       21

Integrierte Lösung - Erstellung der LE mit A+W SLT         23
   Systemanforderungen A+W SLT Power User                  24
                                                                A+W Business – Kurzanleitung Bauproduktenverordnung




Inhaltsverzeichnis
Rechtlicher Hintergrund und Motivation
Die europäische Bauproduktenverordnung schreibt ab 01.07.2013 für alle Hersteller und Zwischenhändler
in der EU die Erstellung, Verwaltung und Zurverfügungstellung von Leistungserklärungen (kurz LE) für
Bauprodukte verbindlich vor.




Abbildung 1: Zusammenspiel Leistungserklärung und CE-Kennzeichen (direkter Prozess)




                                                                                                        A+W Business – Kurzanleitung Bauproduktenverordnung




Abbildung 2: Zusammenspiel Leistungserklärung und CE-Kennzeichen (Händler-Prozess)

Eine Leistungserklärung muss dann erstellt werden, wenn ein Bauprodukt einer harmonisierten Norm
zugeordnet ist oder einer Europäischen Technischen Bewertung (ETB) entspricht. Aussagen und Angaben
über die Leistungen / Merkmale des Produktes dürfen nur dann gemacht werden (bspw. in Werbung), wenn
diese auch in der Leistungserklärung nachvollziehbar aufgeführt und spezifiziert sind.




Rechtlicher Hintergrund und Motivation
„Mit der Erstellung der Leistungserklärung übernimmt der Hersteller die Verantwortung für die Konformität
                                             1
des Bauprodukts mit der erklärten Leistung.“
Für die Umsetzung der Bauproduktenverordnung, ist es erforderlich, dass zu jedem Produkt / jedem
Produktaufbau, eine Leistungserklärung zur Verfügung gestellt wird. Die Leistungserklärung muss
spätestens zum Zeitpunkt der Lieferung, pro Auftragsposition in elektronischer Form (PDF/DOCX) zur
Verfügung gestellt werden. Sind in einem Auftrag mehrere, gleiche Produkte enthalten, so genügt es, dass
die Leistungserklärung je Produkt einmal bereitgestellt wird. Ebenfalls ist es zulässig eine
zusammenfassende Leistungserklärung für alle Auftragspositionen zu erstellen. Auf Wunsch des Kunden,
muss die Leistungserklärung in gedruckter Form zur Verfügung gestellt werden.
Die Leistungserklärung muss 10 Jahre aufbewahrt und auf Anfrage (bspw. Kunde oder Prüfung / Audit)
vorgelegt werden.




                                                                                                            A+W Business – Kurzanleitung Bauproduktenverordnung




Abbildung 3: Beispiel der Leistungserklärung




1
    Amtsblatt der Europäischen Union vom 04.04.2011 (L 88 / 12), Artikel 4, Absatz 3




Rechtlicher Hintergrund und Motivation
Anlegen und Verwalten der Stammdaten
Um die neuen Funktionen mit Bezug auf die durch die Bauproduktenverordnung geforderten
Leistungserklärungen nutzen zu können, müssen Sie zunächst die notwendigen Einstellungen in den
Stammdaten Ihres Systems vornehmen:
       Verwaltung Leistungserklärung: Registrierung von Leistungserklärungen
       Firmenstammdaten: Register Parameter - Mailversand, Standard-LE
       Modul Utilities: Leistungserklärung Produktaufbau
       Produktsammdaten: Register Anlagen
       Marktpartner-Stammdaten: Register Anlagen
       Formularverwaltung: Register Fomular
       Rechteverwaltung: Recht zur manuellen Änderung in den Dokumenten pro Mitarbeiter


Diese Einstellungen werden im Folgenden näher beschrieben.


Verwaltung und Registrierung von Leistungserklärungen
Um eine Leistungserklärung später an einen Vorgang (bspw. einen spezifischen Auftrag) anhängen zu
können oder eine Leistungserklärung einem Produkt oder einem Marktpartner als Standard (Default)
zuweisen zu können, müssen Sie diese Leistungserklärung zunächst im System registrieren.


Sie können diese Registrierung zentral unter Stammdaten > Produkte > Allgemein > Leistungserklärung
Verwaltung vornehmen.




                                                                                                                A+W Business – Kurzanleitung Bauproduktenverordnung




Abbildung 4: Dialog "Leistungserklärung Verwaltung" unter Stammdaten > Produkte > Allgemein > Leistungserklä-
rung Verwaltung



Anlegen und Verwalten der Stammdaten
Nummer
Nummer der Leistungserklärung (alphanumerisch)

Bezeichnung
Name der Leistungserklärung. Er sollte eindeutig und sprechend sein.

Sprache
Sprache, in der die Leistungserklärung verfasst ist. Aus der Kombination Nummer, Bezeichnung und Sprache
der Leistungserklärung, haben Sie so die Möglichkeit eine LE mit einer Nummer in verschiedenen Sprachen
vorzuhalten und zu registrieren.

Link
<DATEI_REF_PFAD>\dop; Pfad, in dem die Leistungserklärungen abgelegt sind. Diesen legen Sie in den
Firmenstammdaten > Register Dokumente fest.

[Hinzufügen], [Entfernen]
Über diese Schaltflächen stellen Sie eine sprachliche Version der LE zur Verfügung oder entfernen sie aus
der Auswahl.


So registrieren Sie eine Leistungerklärung
1.   Wählen Sie Stammdaten > Produkte > Allgemein > Leistungserklärung Verwaltung.
2.   Wählen Sie im Menü > Start > Neu, um eine neue Leistungserklärung zu registrieren.
3.   Tragen Sie die Nummer und die Bezeichnung ein.
     Die Angaben können Sie frei wählen. Jede LE-Nummer darf jedoch nur einmal vergeben werden.
4.   Wählen Sie die Sprache der LE aus. Alternativ können Sie zu einer LE mit einer eindeutigen Nummer
     auch verschiedene Sprachen (Dokumente) zuordnen.
5.   Klicken Sie auf das [Ordner]-Symbol neben dem Feld Link, um das Verzeichnis zu öffnen.
6.   Wählen Sie die gewünschte Vorlage aus.
7.   Wählen Sie im Menü > Start > Speichern, um die Daten zu speichern.
     Die LE steht jetzt in der Produktverwaltung zur Verfügung und kann zugeordnet werden.


Alternativ haben Sie auch die Möglichkeit eine LE im Bereich der Produktstammdaten zu registrieren (als
Standard für ein Produkt) oder im Bereich der Firmenstammdaten (als Standard für einen Marktpartner).
Diese Leistungserklärungen werden so automatisch immer dann gezogen und versendet, wenn keine
spezifische, individuelle LE für einen Produktaufbau oder Vorgang zugewiesen wurde.                         A+W Business – Kurzanleitung Bauproduktenverordnung




Anlegen und Verwalten der Stammdaten
Abbildung 5: Registrierung von Leistungserklärungen in den Produktstammdaten oder Firmenstammdaten


Neu / Löschen (linke Dialogseite)
Erzeugen Sie einen neuen Datensatz (neuer, leerer Dialog) für die Erfassung einer neuen Leistungserklärung
oder löschen Sie den bestehenden Datensatz / die Einträge.

Neu (rechte Dialogseite)
Speichern Sie den neuen Datensatz.


Technische Info: Leistungserklärungs-Verwaltung (BA_LENR und BA_LENR_DETAIL)



     Registrieren von Leistungserklärungen
                                                                                                             A+W Business – Kurzanleitung Bauproduktenverordnung




Um eine Leistungserklärung an einen Vorgang (bspw. einen spezifischen Auftrag) anhängen zu können oder
eine Leistungserklärung als Standard (Default) einem Produkt zuordnen zu können, müssen Sie diese
Leistungserklärung zunächst im System registrieren.
In A+W Business wurde dazu eine neue Tabelle hinterlegt, in welcher alle erfassten Kombinationen
Produktaufbau (ID) – Leistungserklärung gespeichert werden. Hier werden sowohl Standard-
Produktaufbauten aus den Stammdaten als auch alternative Produktaufbauten, welche sich beispielsweise
durch einen Glasaustausch in der Positionserfassung ergeben, berücksichtigt.
Technische Info: Produktaufbau-Tabelle (BW_PRODUKT_AUFBAU_LENR)




Anlegen und Verwalten der Stammdaten
Modul Utilities
Modul Utilities > System > Leistungserklärung Produktaufbau




Abbildung 6: Leistungserklärung Produktaufbau



In diesem Dialog legen Sie fest, welche Unterscheidungsmerkmale bei Produktaufbauten ausgewertet
werden sollen. Dabei gilt jede hinterlegte Kombination von Produktart und Produktgruppe als eigenes
Kennzeichen.
Wenn diese Unterscheidung nicht ausreichend ist, geben Sie außerdem an, dass die jeweilige
Artikelnummer zusätzlich verwendet werden soll.


Technische Info: Produktaufbau-Tabelle (KA_AUFBAU_LENR )
                                                                                                      A+W Business – Kurzanleitung Bauproduktenverordnung




Firmenstammdaten
Stammdaten > Firma > Firmendaten > Register Parameter




Abbildung 7: Firmendaten – Register Parameter

Technische Info: Tabelle (KU_KUNDEN ,LI_LIEFERANTEN, PA_PARTNER, Feld TRANSFER_LE)

Anlegen und Verwalten der Stammdaten
Versand von Leistungserklärungen
Mit dieser Einstellung aktivieren Sie den Versand von Leistungserklärungen für diesen Marktpartner.
Zusätzlich können Sie in der Formularverwaltung festlegen, ob die LE beim Druck versendet werden soll.

Standard-Leistungserklärung
In diesem Feld legen Sie fest, welche LE per Default an den Marktpartner gesendet werden soll, wenn zu
einer Auftragsposition keine spezifische, separate LE zugewiesen wurde. Die Leistungserklärungen sind im
Standardverzeichnis der Dateianhänge unter <DATEI_REF_PFAD>\dop abgelegt. Dieses Verzeichnis legen
Sie in den Firmendaten > Register Dokumente fest.
Über die Schaltfläche [Ordner] können Sie eine Leistungserklärung für dieses Produkt / diesen
Produktaufbau registrieren. Zur Auswahl über das Symbol [Lupe] werden Ihnen die Leistungserklärungen
angezeigt, welche bereits im System registriert und unter dem <DATEI_REF_PFAD>\dop gespeichert
wurden.



Produktstammdaten
Stammdaten > Produkte > Artikel > Register Anlagen




                                                                                                           A+W Business – Kurzanleitung Bauproduktenverordnung




Abbildung 8: Zuordnung / Registrierung von LE in den Artikelstammdaten


In den Produktstammdaten können Sie eine Leistungserkklärung zuweisen, welche bezogen auf dieses
Produkt / diesen Produktaufbau per Standard (Default) gesendet werden soll. Im Auftrag können Sie diese
LE später an der Position manuell überschreiben, bspw. nach einem Glasaustausch.


Technische Info: Tabelle (BA_PRODUKTE, Felder LENR und LE_FLAG)



Anlegen und Verwalten der Stammdaten
Nummer
Nummer der spezifischen Leistungserklärung, welche diesem Produkt / diesem Aufbau als Standard
zugewiesen wurde. Die Kombination aus Produktaufbau (Produktaufbau-ID) und LE-Nummer wird im
System hinterlegt.


Über die Schaltfläche [Ordner] können eine Leistungserklärungen für dieses Produkt / diesen
Produktaufbau registrieren. Zur Auswahl über die [Lupe] werden Ihnen die Leistungserklärungen angezeigt,
welche bereits im System registriert und auf dem festgelegten Verzeichnis unter <DATEI_REF_PFAD>\dop
gespeichert wurden.

Leistungserklärung erforderlich
Mit dieser Einstellung geben Sie an, ob eine LE für das aktuelle Produkt erforderlich ist (bspw. ist für einen
Abstandhalter keine eigenständige LE erforderlich). Das Kennzeichen und die zugeordnete LE werden in die
Auftragsposition übernommen. Wenn Sie keine LE zugeordnet haben, wird die Standard-LE aus den
Firmendaten verwendet.



     Registrieren von Leistungserklärungen
Um eine Leistungserklärung an einen Vorgang (bspw. einen spezifischen Auftrag) anhängen zu können oder
eine Leistungserklärung als Standard (Default) einem Produkt zuordnen zu können, müssen Sie diese
Leistungserklärung zunächst im System registrieren.




                                                                                                                 A+W Business – Kurzanleitung Bauproduktenverordnung




Anlegen und Verwalten der Stammdaten
Stammdaten Marktpartner
Stammdaten > Marktpartner > Kunde > Kunden > Register Anlagen




Abbildung 9: Stammdaten Marktpartner (Beispiel Kunde)

Versand von Leistungserklärungen
Mit dieser Einstellung aktivieren Sie den Versand von Leistungserklärungen für den aktuellen Marktpartner
(Kunden).



                                                                                                            A+W Business – Kurzanleitung Bauproduktenverordnung




Anlegen und Verwalten der Stammdaten
Formularverwaltung
Stammdaten > Formulare > Formularverwaltung > Register Formular




Abbildung 10: Formularverwaltung


Versand per Mail
Mit dieser Einstellung legen Sie fest, bei welchem Druckpunkt die LE per E-Mail gesendet werden soll.


Technische Info: Formularvariable LENR vom Typ String
                                                                                                        A+W Business – Kurzanleitung Bauproduktenverordnung




Anlegen und Verwalten der Stammdaten
Rechteverwaltung
Stammdaten > Firma > Mitarbeiterrechte




Abbildung 11: Beispiel Mitarbeiterberechtigung



In diesem Dialog legen Sie die Berechtigungen Ihrer Mitarbeiter in Bezug auf die Verwaltung von
Leistungserklärungen fest. Hier können Sie zum Beispiel definieren, ob ein Mitarbeiter das Recht hat eine
Leistungserklärung in der Positionserfassung manuell zuzuordnen.


                                                                                                            A+W Business – Kurzanleitung Bauproduktenverordnung




Anlegen und Verwalten der Stammdaten
Anwendung in der Dokumentenverwaltung
Bei der Erfassung einer neuen Position wird
zunächst immer die Leistungserklärungsnummer
aus den Produktsammdaten in die Position
übernommen.


Bei      einer     Positionsänderung    (bspw.
Glasaustausch), wird der Produktaufbau der
aktuellen Position geprüft / neu bestimmt.
Dieser      Produktaufbau     wird   in    der
Produktaufbau-Tabelle gesucht, und die
Produktaufbau-ID sowie die zugehörige LE-
Nummer werden in die Position übernommen.
Kann der Aufbau nicht ermittelt werden, wird
die Leistungserklärungsnummer aus der Position
entfernt.


Nun erfolgt die Eingabeprüfung in der
Positionserfassung. Hier wird geprüft, ob für das
aktuelle Produkt in den Produktstammdaten das
Flag zur Leistungserklärungs-Ermittlung aktiviert
ist und, wenn ja, ob eine Leistungserklärung in
der Position vorhanden ist. Ist das Kennzeichen
gesetzt     aber     keine     Leistungserklärung
zugewiesen,      wird     eine     entsprechende
Hinweismeldung ausgegeben. Sie können so
nachträglich, manuell eine LE zuweisen. Diese
Meldung      kann     Benutzerabhängig       auch
deaktiviert werden.
                                                    Abbildung 12: Prozessablauf der LE-Ermittlung in der Doku-
                                                    mentenerfassung

Nun wird die Position gespeichert. Wurde die Leistungserklärungsnummer für die aktuelle Position manuell
geändert, so wird diese in der Position gespeichert. Wurde der Produktaufbau in der Position verändert
(bspw. Glasaustausch), wird der neue Produktaufbau zusammen mit der zugeordneten
Leistungserklärungsnummer in der Produktaufbau-Tabelle gespeichert. Ist der Produktaufbau bereits in
dieser Tabelle eingetragen, so wird die darin zugeordnete Leistungserklärungsnummer überschrieben.
                                                                                                                 A+W Business – Kurzanleitung Bauproduktenverordnung




Anwendung in der Dokumentenverwaltung
Modul Dokumente > Auftrag > Auftrag > Register Positionen




Abbildung 13: Zuweisung einer Leistungserklärung zu einer Position


Leistungserklärung
Nummer der zugewiesenen Leistungserklärung


LE-Suche
Startet den Suchdialog für die manuelle Suche einer registrierten Leistungserklärung




                                                                                       A+W Business – Kurzanleitung Bauproduktenverordnung




Anwendung in der Dokumentenverwaltung
Formulardruck
Beim Formularduck wird zunächst geprüft, in welcher Sprache das Formular (Auftragsbestätigung,
Lieferschein, etc.) erstellt wird. Anschließen wird in den Kundendaten geprüft, welche Sprache als Standard
für den Kunden zugeordnet ist. Wenn keine entsprechenden sprachlichen Vorgaben für die
Leistungserklärung einer Position gefunden wurden (weder im Bereich Formulare, noch in den
Kundenstammdaten), wird die Standard-LE aus den Firmendaten verwendet.


Nach dem Versand der Leistungserklärung wird in den Kundendaten ein systeminterner Vermerk
gespeichert (technische Info: Tabelle DR_KUNDEN_LENR). Dadurch wird diese LE nicht nochmals gesendet,
wenn der Kunde den selben Produktaufbau erneut bestellt. Als zusätzliche Informationen werden das
Druckdatum und die Versandinformationen (Art des Ausdruck und Dokumentennummer) mit in die Tabelle
geschrieben. Bei einem weiteren Druck wird diese Tabelle geprüft und der Mailversand der
Leistungserklärung unterdrückt.




                                                                                                              A+W Business – Kurzanleitung Bauproduktenverordnung




Formulardruck
Produktionsübergabe
Für die Übergabe an das Produktionsplanungssystem A+W Production muss die LE-Nummer als Textsatz in
der Order.xml mit übergeben werden. Die entsprechenden Standardtexte hinterlegen Sie mit einem
eigenen Textkennzeichen und ordnen dies in den Produktdaten zu.


Modul Stammdaten > Texte > Texte




Abbildung 14: Beispiel: Standardtext für Produktionsübergabe


Weiterhin kann der Link zur Leistungserklärung ebenfalls via Order.xml an A+W Production übergeben
werden. Aktivieren Sie hierzu das Kennzeichen von zu übertragenden Dateianhängen > A Alle

                                                                                                      A+W Business – Kurzanleitung Bauproduktenverordnung




Produktionsübergabe
Modul Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register
Texte/Anlagen.




Abbildung 15: Produktionsübergabe von Texten und Anhängen




                                                                                                  A+W Business – Kurzanleitung Bauproduktenverordnung




Produktionsübergabe
Best Practise – Registrieren und Verwalten der LE
Aufbauend auf den oben beschriebenen Funktionen zur Verwaltung der Leistungserklärungen in ALFAK /
A+W Business, wollen wir Ihnen nun in einem Best-Practice-Beispiel zeigen, wie sie die
Leistungserklärungen schnell und gezielt verwalten und Ihren Produkten zuordnen können.




Anlage der Stammdaten
Der Pfad zum Dokument und Bezeichnung der LE sollte standardisiert sein, sprechend und möglichst LE-
und CE- Kennzeichnung enthalten. Weiterhin sollten Sie nach Sprachen trennen. Beispiele:
     \\jupiter\Anlagen\dop\Standard\AWTopEnergie\Deutsch\10.0.01-LE.pdf
     \\jupiter\Anlagen\dop\Standard\AWTopEnergie\Englisch\10.0.01-LE.pdf
     \\jupiter\Anlagen\dop\Standard\AWSonnenschutz\Deutsch\40-37.0.7-LE.pdf
     \\jupiter\Anlagen\dop\Standard\AWSonnenschutz\Englisch\40-37.0.7-LE.pdf

So erleichtern Sie nicht nur die Registrierung der Leistungserklärung im System sondern auch Ihren AV-
Mitarbeitern die Zuordnung im Auftrag.




Abbildung 16: Standardisierte Pfadangaben erleichtern die Registrierung der LE


Die Anlage / Registrierung kann manuell erfolgen oder durch ein Script unterstützt werden. Dies setzt
                                                                                                         A+W Business – Kurzanleitung Bauproduktenverordnung




jedoch voraus, dass Sie die Bezeichnung (Dateinamen) der Leistungserklärungen entsprechend
strukturieren und durchgängig verwenden. Die verwendung von klaren und gutstrukturierten
Verzeichnispfaden unterstützt und vereinfacht die Registrierung (sowohl per Script als auch manuell).



      A+W SLT Power User
Für die Erstellung der Leistungserklärung und die Vergabe der Dateinamen als eindeutigen und
sprechenden Schlüssel empfehlen wir Ihnen die Lösung A+W SLT Power User.




Best Practise – Registrieren und Verwalten der LE
Zuordung der Leistungserklärungen
Die Zuordnung der LE zu spezifischen Produktaufbauten findet in der Dokumentenerfassung statt.
Folgende Vorgehensweise ist empfehlenswert:
    1.   Aktivierung aller zum Leistungserklärungsversand freigegebenen Artikel (ggf. per Script) zunächst
         für einen Testkunden
    2.   Erfassung aller Aufbauten und Zuordnung der LE in Testaufträgen
    3.   Zu beachten ist, dass für „diverse“ Kunden der LE-Versand jedes Mal aufs Neue stattfindet. Die
         Auswahl „Diverser“ wird daher nicht empfohlen.
    4.   Die „Default Leistungserklärung“ kann in den Firmenstammdaten hinterlegt werden, hierbei wäre
         es sinnvoll, dass hier der aller höchste Ug-Wert und alle übrigen Parameter mit „npd“ angegeben
         sind.
    5.   Sollten die Einstellungen und Testaufträge für den Testkunden problemlos funktionieren, so
         können Sie die Einstellungen entsprechend auf Ihre Echt-Kunden übertragen.




                                                                                                             A+W Business – Kurzanleitung Bauproduktenverordnung




Abbildung 17: Best Practice in Pfadangabe und Dokumentenname



Best Practise – Registrieren und Verwalten der LE
Um zu prüfen, welchen Produkten noch keine LE zugeordnet wurden, können Sie Abfragen und Reports
benutzen (bspw. CR). Ebenfalls ist es möglich auszuwerten, welche Leistungserklärungen bereits erfasst,
aber noch nicht zugeordnet wurden. Dazu haben wir Ihnen in dieser Kurzanleitung die technischen
Informationen zu Datenbank-Tabellen und –Feldern angegeben.




Abbildung 18: Auswertung der bereits erfassten und noch nicht zugeordneten Leistungserklärungen




     Auswertungen und Abfragen mit CR erstellen
Wir empfehlen Ihnen, bevor Sie Reports erstellen, Kontakt mit dem A+W Support aufzunehmen, um sicher
zu stellen, dass Sie auf die richtigen Daten referenzieren. Auch helfen Wir Ihnen als Value+ Kunde gern bei
der Anpassung / Erstellung von Reports.




                                                                                                              A+W Business – Kurzanleitung Bauproduktenverordnung




Best Practise – Registrieren und Verwalten der LE
Integrierte Lösung - Erstellung der LE mit A+W SLT
Um bereits mit dem Service Pack I eine praktikable und durchgängige Lösung für Sie bereitzustellen, haben
wir in Kooperation mit Sommer-Informatik eine teilintegrierte Prozess-Lösung für Sie erstellt.


Mit der Lösung A+W SLT Power User können Sie schon heute die Leistungserklärungen erstellen (basierend
auf technischen Werten und Restriktionen, welche Sie im System hinterlegen). Diese können Sie
anschließend in ALFAK / A+W Business registrieren, verwalten und Ihren Produkten und Kunden zuordnen
und via Mail versenden.


Mit dem Service Pack II für die ERP-Systeme ALFAK / A+W Business und ALCIB / A+W Enterprise wird A+W
die tiefe Integration der Lösungen forcieren und entsprechend ausbringen. Hier werden Sie dann auch über
die Lösung mit vordefinierten Stammdatensätzen arbeiten können.


Bei beiden Lösungen lassen sich die ermittelten Leistungsdaten für die jeweiligen Produktvarianten einfach
in die Leistungserklärung übertragen und ausdrucken.


Mit den Lösungen A+W SLT Power User und A+W SLT Standard User können Sie basierend auf den
technischen Werten der Produktaufbauten die Leistungswerte berechnen und Leistungserklärungen
erstellen lassen. Diese können Sie anschließend wie beschrieben registrieren und als Dateinanhang oder via
Mail versenden.




                                                                                                             A+W Business – Kurzanleitung Bauproduktenverordnung




Integrierte Lösung - Erstellung der LE mit A+W SLT
Systemanforderungen A+W SLT Power User
Für die Lösung A+W SLT Power User gelten folgende Systemvoraussetzungen:


Prozessor:                        Intel Core I5 oder I7 oder vergleichbar
Arbeitsspeicher:                  min. 1 GB RAM
Festplattenspeicherplatz:         min. 10 GB
Betriebssystem:                   Windows XP, Vista, Windows 7, Windows 8
Monitor (min. Auflösung):         1024 x 768




                                                                            A+W Business – Kurzanleitung Bauproduktenverordnung




Integrierte Lösung - Erstellung der LE mit A+W SLT

