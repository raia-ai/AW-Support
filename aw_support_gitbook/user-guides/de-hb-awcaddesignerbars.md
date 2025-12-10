---
description: "DE HB AWCADDesignerBars"
---



# DE HB AWCADDesignerBars

A+W CAD Designer
(Bars)

Handbuch




Deutsch
Editorial




            Editorial
            Revisionsübersicht der Dokumentation

            10-2024     Gesamthandbuch für PDF und HTML5-Format aktualisiert.


            Anmerkungen
            Diese Veröffentlichung ist ausschließlich für Endanwender von A+W CAD De-
            signer (Bars) gedacht.
            Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz
            vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden.
            Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
            ohne Vorankündigung geändert werden.
            Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter
            Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausge-
            schlossen werden. Die A+W Software GmbH übernimmt keine Haftung für
            Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem
            oder grobfahrlässigem Handeln.
            Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbau-
            stufe von A+W CAD Designer (Bars).

            Urheberrechte
            © 2024, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
            stellung von Kopien und der Übersetzung, bleiben vorbehalten.
            Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
            piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
            Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
            A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
            nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

            Warenzeichen
            Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen kön-
            nen gleichzeitig auch eingetragene Marken oder sonstige gewerbliche
            Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.




2                                                             A+W CAD Designer (Bars)
                                                                                              Editorial




                      Darstellungskonventionen
                      Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                      gende Bedeutung:

                      Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                               Software bezeichnen, z. B. der Dialog
                                               Preiseigenschaften.

                      Fett                     sind Zeichenfolgen ausgezeichnet, die Sie über die
                                               Tastatur eingeben, z. B.: Geben Sie den Wert 5 ein.

                      >                        Mit dem sogenannten Brotkrumenpfad ist der Weg
                                               gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                               Stammdaten > Preise > ISO-Preise.

                      []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                               z. B.: Mit [OK] speichern Sie die Daten.

                      <>                       Spitze Klammern bezeichnen Tasten oder
                                               Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                               öffnen Sie die Online-Hilfe.


                      Kontakt

                      A+W Software GmbH
                      Siemensstr. 3           Tel.:       +49 641 96620 0
                      D-35463 Fernwald        E-Mail:     info@a-w.com
                      Deutschland             Web:        http://www.a-w.com




A+W CAD Designer (Bars)                                                                                3
Editorial




4           A+W CAD Designer (Bars)
Inhalt
Überblick                                                                  A      Die Stammdaten ................................................. A-232
                                                                                   Stammdaten ..................................................... A-233
Tutorial .................................................................. A-9    Stammdaten-Editor .......................................... A-235
Überblick .............................................................. A-12      Passwort .......................................................... A-240
 Aufbau des Tutorials .......................................... A-13             Ansicht ................................................................ A-241
A+W CAD Designer (Bars) stellt sich vor ............. A-14                         Vermaßung ....................................................... A-242
Arbeiten mit A+W CAD Designer (Bars) .............. A-16                           Maße ................................................................ A-244
 Oberfläche von A+W CAD Designer (Bars) ....... A-16                               Sprachauswahl ................................................. A-245
 Einstellungen ..................................................... A-75         Die Hilfe verwenden ........................................... A-246
 Stammdaten in A+W CAD Designer (Bars) ....... A-85                                Über CAD Designer ......................................... A-247
Sprossen .............................................................. A-98
 Neue Konstruktionen ......................................... A-99               Help Cards ......................................................... A-249
 Zuschnitt und Messen ...................................... A-121                Informationen zu den HelpCards ........................ A-251
Spezialmuster .................................................... A-127          Stammdaten ....................................................... A-252
 Sondermuster .................................................. A-127              Werkzeuge ....................................................... A-253
 Fassaden ......................................................... A-130           Fangpunkte ...................................................... A-254
 Makros ............................................................. A-137         Sprossen anlegen ............................................ A-255
Datenaustausch ................................................. A-166              Stammdaten schützen ..................................... A-256
 Datenimport ..................................................... A-166          Sprossen ............................................................ A-257
 Datenexport ..................................................... A-169            Eigenschaften der Scheibe .............................. A-258
Konfiguration ...................................................... A-174          Einfaches Sprossenmuster platzieren .............. A-259
Anhang – Makrokatalog ..................................... A-175                   Sprossen über Werte platzieren ....................... A-260
                                                                                    Modell mit Sprossen platzieren ........................ A-261
Softwarereferenz .............................................. A-187               Freie Sprossenkonstruktion erstellen ............... A-262
Bedienung von A+W CAD Designer (Bars) ........ A-190                              Spezialmuster ..................................................... A-263
 Softwarebegriffe ............................................... A-191             Fassadenanlage erstellen ................................ A-264
 Programm beenden ......................................... A-195                   Makro laden ..................................................... A-265
Übersicht ............................................................ A-196        Ein Makro ändern und speichern ..................... A-266
Umgang mit Dateien .......................................... A-197                 Eigenes Makro erstellen ................................... A-267
 Neue Scheibe .................................................. A-199
 Übergabedatei importieren .............................. A-202                   Index                                                                      Z
 Neue Scheibenposition .................................... A-204
 Drucken ........................................................... A-205
 Listendruck ...................................................... A-206
 Druckereinrichtung ........................................... A-207
Werkzeuge verwenden ...................................... A-210
Mit Spezialmustern arbeiten ............................... A-212
 Muster Senkrecht-Waagerecht ........................ A-213
 Kundenvorgabe SW-Muster ............................. A-216
 Eingabe Sprossen-Abstände ........................... A-219
 Rautenmuster... ............................................... A-220
 Fassadenanlage... ........................................... A-222
 Sonne und Sterne ............................................ A-223
 Makro auswählen ............................................. A-225
 Makro-Parameter ............................................. A-226
 Relativer Abstand ............................................. A-227
Messen und Zuschnitt ........................................ A-228
 Abstand ............................................................ A-229
 Zuschnitt-Informationen ................................... A-230



A+W CAD Designer (Bars)                                                                                                                                     5
6   A+W CAD Designer (Bars)
A   A+W CAD Designer (Bars)
    Überblick
      Revisionsübersicht des Moduls:

      01-2017     Produkt- und Firmennamen angepasst.

      03-2013     Überarbeitung im Rahmen der Produktneuausrichtung

      10-2010     Ersterstellung


      Zu diesem Modul finden Sie folgende Kapitel
       Tutorial
       Softwarereferenz




A-8                                         A+W CAD Designer (Bars) Überblick
A   A+W CAD Designer (Bars)
    Überblick




                       Tutorial
                                                                                                                        Tutorial




       In diesem Kapitel finden Sie folgende Themen:
        Überblick
        A+W CAD Designer (Bars) stellt sich vor
        Arbeiten mit A+W CAD Designer (Bars)
        Sprossen
        Spezialmuster
        Datenaustausch
        Konfiguration
        Anhang – Makrokatalog


       Überblick ............................................................................................................... A-12
         Aufbau des Tutorials .......................................................................................... A-13
       A+W CAD Designer (Bars) stellt sich vor ............................................................. A-14
       Arbeiten mit A+W CAD Designer (Bars) ............................................................... A-16
         Oberfläche von A+W CAD Designer (Bars) ...................................................... A-16
           Programm-Präsentation ................................................................................. A-17
           Die Menüleiste ............................................................................................... A-18
           Die Symbolleiste ............................................................................................ A-18
           Das Wertefenster ........................................................................................... A-20
           Die Standard-Sprosse .................................................................................... A-21
           Der Mauszeiger ............................................................................................. A-21
           Die Fangpunkte .............................................................................................. A-22
             Das Arbeiten mit Fangpunkten ................................................................... A-22
           Die Werkzeuge .............................................................................................. A-40
             Die Werkzeuge verwenden ........................................................................ A-40
             Die Vermaßungswerkzeuge ....................................................................... A-74
         Einstellungen ..................................................................................................... A-75
           Vermaßungen ein- und ausblenden ............................................................... A-76
           Vermaßung von Bohrpunkten darstellen ........................................................ A-81
           Maße eingeben .............................................................................................. A-82
           Programmsprache wählen ............................................................................. A-84
         Stammdaten in A+W CAD Designer (Bars) ....................................................... A-85
           Sprossentypen ............................................................................................... A-86
           Sprossenstäbe ............................................................................................... A-88
           Wegfallsprossen ............................................................................................ A-89
           Stammdaten anlegen ..................................................................................... A-91
           Stammdaten schützen ................................................................................... A-95
           Übungen ........................................................................................................ A-96
       Sprossen ............................................................................................................... A-98
         Neue Konstruktionen ......................................................................................... A-99
           Allgemeine Vorgehensweise ........................................................................ A-100
             Form für die Konstruktion festlegen .......................................................... A-100
           Eigenschaften der Scheibe definieren ......................................................... A-101
           Sprossen platzieren ..................................................................................... A-102
             Gleiche lichte Felder ................................................................................. A-103
             Gleicher Bohrpunktabstand ...................................................................... A-104
             Gleicher Bohrpunktabstand (Bezug auf Scheibe) .................................... A-105
             Gleiche Sprossenlänge ............................................................................ A-106
             Kundendefiniert ........................................................................................ A-107
           Sprossen tauschen ...................................................................................... A-109
           Demos und Übungen ................................................................................... A-110


A-10                                                                   A+W CAD Designer (Bars) Überblick
Tutorial




                       Zuschnitt und Messen ..................................................................................... A-121
                          Zuschnittinformationen anzeigen ................................................................. A-122
                            Zuschnitt am Anfang und am Ende der Sprosse ...................................... A-123
                          Abstände oder Längen messen ................................................................... A-126
                      Spezialmuster ..................................................................................................... A-127
                       Sondermuster .................................................................................................. A-127
                          Sondermuster erstellen ................................................................................ A-128
                        Fassaden ......................................................................................................... A-130
                          Fassadenanlage .......................................................................................... A-131
                            Abmessungen der einzelnen Scheiben angeben ..................................... A-131
                          Demos und Übungen ................................................................................... A-132
                            Trainerdemo: Fassadenanlagen erläutern ................................................ A-132
                            Übung 1: Erstellen einer Fassadenanlage ............................................... A-132
                            Übung 2: Nachbildung einer Fassadenanlage ......................................... A-134
                        Makros ............................................................................................................. A-137
                          Allgemein ..................................................................................................... A-138
                            Makro laden .............................................................................................. A-138
                          Demos und Übungen ................................................................................... A-139
                            Trainerdemo: Vorhandene Makros erläutern ............................................ A-139
                            Trainerdemo: Ein vorhandenes Makros ändern ....................................... A-139
                            Trainerdemo: Eigene Makros erstellen ..................................................... A-139
                            Übung 1: Platzieren Sie das Makro York3H1S auf einer Scheibe ............ A-140
                            Übung 2: Änderungen am Makro York3H1S auf der Scheibe
                            vornehmen ................................................................................................ A-142
                            Übung 3: Änderungen am Makro York3H1S vornehmen und das Makro
                            unter einem anderen Namen speichern ................................................... A-144
                            Übung 4: Erstellen eines eigenen Makros ................................................ A-145
                            Übung 5: Makro erstellen und mittels Referenzpunkt platzieren .............. A-153
                      Datenaustausch .................................................................................................. A-166
                        Datenimport ..................................................................................................... A-166
                          Übergabedateien ......................................................................................... A-167
                          Dateien importieren - Neu ............................................................................ A-167
                        Datenexport ..................................................................................................... A-169
                          Konstruktionen und Übergabedateien ......................................................... A-169
                          Drucker einrichten ........................................................................................ A-169
                          Konstruktionen drucken ............................................................................... A-171
                          Übergabedatei drucken ................................................................................ A-171
                          Bild exportieren ............................................................................................ A-173
                          Nachrichten senden ..................................................................................... A-174
                      Konfiguration ....................................................................................................... A-174
                      Anhang – Makrokatalog ...................................................................................... A-175




A+W CAD Designer (Bars) Überblick                                                                                                        A-11
Überblick                                                                         Tutorial




            Überblick
            Die Schulung zum Produkt A+W CAD Designer (Bars) ist für Mitarbeiter kon-
            zipiert, die sich mit der Erstellung einfacher und komplexer Sprossenkonstruk-
            tionen beschäftigen. Die Teilnehmer lernen, Stammdaten anzulegen und
            Sprossenkonstruktionen zu erstellen.
            Für häufig vorkommende Konstruktionen lernen die Teilnehmer das Erstellen
            und den Umgang mit Makros. Mit Hilfe dieser Makros können sich Anwender
            in einfacher Weise einen Motiv-Katalog erstellen.

            Themenblöcke
            In diesem Tutorial finden Sie folgende Themenblöcke:
            •   A+W CAD Designer (Bars) stellt sich vor
            •   Arbeiten mit A+W CAD Designer (Bars)
            •   Einstellungen
            •   Stammdaten in A+W CAD Designer (Bars)
            •   Sprossen
            •   Zuschnitt und Messen
            •   Spezialmuster
            •   Datenaustausch
            •   Konfiguration
            •   Anhang – Makrokatalog

                Vorausgesetzte Kenntnisse
                EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwen-
                dung von A+W CAD Designer (Bars) vorausgesetzt.




A-12                                               A+W CAD Designer (Bars) Überblick
Tutorial                                                                                    Überblick




                      Aufbau des Tutorials
                      Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinhei-
                      ten. Jede Lerneinheit besteht aus folgenden Komponenten:

                      Überblick               Jede Lerneinheit beginnt mit einem Überblick über die
                                              wichtigsten Inhalte:
                                              • Lernziele: Was soll vermittelt werden?
                                              • Nutzen: Wofür können Sie dieses Wissen einsetzen?
                                              • Merksätze: Welche Zusammenhänge müssen Sie
                                                sich merken?

                      Konzepte                Konzepte und Begriffe der jeweiligen Lerneinheit
                                              werden zunächst erläutert. Danach finden Sie Beispiele
                                              und Handlungsanleitungen.

                      Übungen                 • Zu einigen Lerneinheiten finden Sie Übungen mit
                                                Aufgabenstellungen und Lösungsvorschlägen.
                                              • Die Übungen helfen Ihnen A+W CAD Designer (Bars)
                                                zu verstehen und anwenden zu lernen.

                      Querverweisteil         Am Ende jeder Lerneinheit finden Sie einen Abschnitt
                                              mit Querverweisen, die auf entsprechende
                                              Beschreibungen in der Softwarereferenz hinweisen.
                                              Damit können Sie das neu erworbene Wissen vertiefen.

                      Lesehinweis             Der Inhalt einer Lerneinheit baut auf den Kenntnissen
                                              auf, die in der vorausgegangenen Einheit vermittelt
                                              wurden. Es ist daher sinnvoll, keine Lerneinheiten zu
                                              überspringen.
                                              Sollten Sie mit einem Thema bereits vertraut sein, lesen
                                              Sie mindestens die Zusammenfassung am Beginn der
                                              Lerneinheit, um sich die wichtigsten Details zu
                                              vergegenwärtigen.


                      Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der
                      Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht
                      ein roter Faden durch die gesamte Dokumentation.




A+W CAD Designer (Bars) Überblick                                                                A-13
A+W CAD Designer (Bars) stellt sich vor                                                       Tutorial




                        A+W CAD Designer (Bars)
                        stellt sich vor
                        Originelle Architektur und individueller Geschmack finden immer mehr auch
                        Ausdruck in ausgefallenen Sprossenkonstruktionen. Die Häufung der Sonder-
                        konstruktionen macht den Einsatz eines leistungsfähigen Konstruktionspro-
                        gramms erforderlich, das auch in der Lage ist, sofort ein Bild der gewünschten
                        Sprossenanordnung auf dem Bildschirm, über einen Drucker oder Plotter in
                        Originalgröße auszugeben.
                        A+W CAD Designer (Bars) ist ein Sprossenkonstruktionsprogramm mit grafi-
                        scher Oberfläche, die es ermöglicht, die Mehrzahl gebräuchlicher Sprossen-
                        typen beliebig auf Rechteck- oder Modellscheiben anzuordnen. Es können
                        Sprossen mit unterschiedlichen Breiten in eine Konstruktion eingesetzt wer-
                        den, außerdem ist es möglich, verschiedene Sprossentypen innerhalb eines
                        Sprossenbildes zu verwenden. A+W CAD Designer (Bars) ermöglicht Konst-
                        ruktionen mit geraden Sprossen, Bogensprossen und Sprossen unter freiem
                        Winkel.
                        Zu beachten sind jedoch die landesüblichen Spezifikationen. So gibt es in
                        Deutschland überwiegend Dreh- und Kippfenster nach innen. In Amerika hin-
                        gegeben kommen überwiegend Schiebefenster bzw. Kurbelfenster nach au-
                        ßen zum Einsatz.

                        Sprossenaufteilung
                        A+W CAD Designer (Bars) stellt eine Automatik für die häufigsten Sprossen-
                        aufteilungen wie etwa gleiche lichte Felder zur Verfügung. Daneben können
                        auch komplett freie Konstruktionen bequem mit Hilfe von Hilfspunkten erstellt
                        werden. Diese Hilfspunkte können, wie in CAD-Programmen üblich, aus einer
                        Reihe von geometrischen Operationen (z. B. Schnittpunkt oder Abstand) er-
                        zeugt werden. Darüber hinaus können einzelne Sprossen oder auch Spros-
                        sengruppen auf vielfältige Weise manipuliert werden (verschieben, drehen,
                        spiegeln etc). Details lassen sich mit Hilfe von Ausschnittvergrößerungen
                        sichtbar machen.

                        Sprossenabgleich
                        Der Abgleich der Sprossen erfolgt auf einer Arbeitsfläche, auf der Scheiben
                        beliebig zueinander angeordnet und dargestellt werden können. Gleichzeitig
                        können Sie die Sprossenaufteilung der Fassadenfläche anpassen. D.h. der
                        optisch einwandfreie Verlauf von Sprossen kann über alle Scheiben einer
                        Fassade fortgesetzt werden.

                        Ausgabe
                        Zur Ausgabe wird eine maßstabgetreue Zeichnung gedruckt, die auch die Lis-
                        te der zu schneidenden Profile enthält. Diese Zeichnung enthält außerdem
                        alle relevanten Informationen für die Sprossenkreuzungen, wie z. B. den Fräs-
                        winkel. Alle Produktionspapiere sind frei gestaltbar und können auf dem Mo-
                        nitor oder als Ausdruck ausgegeben werden. Die Ausgabe kann auch über
                        einen Plotter im Maßstab 1:1 erfolgen.



A-14                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                  A+W CAD Designer (Bars) stellt sich vor




                      Makros
                      Bei häufig vorkommenden Konstruktionen finden sogenannte Makros ihren
                      Einsatz. Die Makros werden auf einfache Art und Weise erstellt. Bei ihrer An-
                      wendung müssen dann lediglich noch die für die Konstruktion zwingend erfor-
                      derlichen Maße eingegeben werden. Mit Hilfe dieser Makros können sich
                      Anwender in einfacher Weise einen Motiv-Katalog erstellen.

                      Vermaßung
                      Die Vermaßung der fertigen Konstruktion kann den individuellen Produktions-
                      anforderungen angepasst werden. So ist es z. B. möglich, die Bohrpunktinfor-
                      mation sowohl in Bezug auf die Innenkante als auch in Bezug auf die
                      Außenkante des Rahmens zu erstellen.

                      Weitere Details
                      Die integrierte Datenschnittstelle ermöglicht Ihnen einen reibungslosen Da-
                      tenimport. Weiterhin können NC-Codes für diverse Maschinen (z. B. Hegla
                      Sprossensäge, Rottler & Rüdiger-Säge und Montagezentrum) erzeugt wer-
                      den.




A+W CAD Designer (Bars) Überblick                                                            A-15
Arbeiten mit A+W CAD Designer (Bars)                                                                Tutorial




                       Arbeiten mit A+W CAD Desig-
                       ner (Bars)
                       In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                       A+W CAD Designer (Bars) kennen.


                       Oberfläche von A+W CAD Designer
                       (Bars)
                       Lernziele

                       •   Oberfläche von A+W CAD Designer (Bars) kennenlernen
                       •   Fangpunkte kennenlernen und verstehen
                       •   Die Werkzeuge kennenlernen und verstehen
                       •   Inhalte des Wertefensters verstehen
                       •   Unterschiedliche Darstellung der Mauszeiger kennenlernen


                       Nutzen

                       Das Arbeiten in A+W CAD Designer (Bars) ist nur dann sinnvoll möglich, wenn Sie die
                       zur Verfügung gestellten Werkzeuge anwenden können. Je besser Sie die
                       Werkzeuge von A+W CAD Designer (Bars) kennen um so effizienter können Sie
                       arbeiten.


                       Definitionen

                       Symbolleiste                ist die waagerechte Leiste mit kleinen, bebilderten
                                                   Schaltflächen.

                       Werkzeuge                   helfen Ihnen bei der Konstruktion von Sprossenbildern.

                       Wertefenster                Abhängig von der Auswahl erhalten Sie Informationen
                                                   zu verbauten Materialien bzw. deren Anzahl.

                       Konstruktionsbereich        In diesem Bereich erstellen Sie die
                                                   Sprossenkonstruktion.

                       Fangpunkte                  helfen Ihnen beim Platzieren von Sprossen.


                       Merke

                       Symbolleiste, Werkzeuge,    können mit der Maus an jede x-beliebige Stelle
                       Wertefenster und            verschoben werden.
                       Fangpunkte
                                                   Die Funktionen können über das Menü Ansicht beliebig
                                                   ein- und ausgeblendet werden.

                       Unterschiedliche            Abhängig von dem, was Sie tun, ändert sich in A+W
                       Mauszeiger                  CAD Designer (Bars) das Aussehen des Mauszeigers.




A-16                                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                         Arbeiten mit A+W CAD Designer (Bars)




                           Programm-Präsentation
                           Wenn Sie A+W CAD Designer (Bars) gestartet haben, stellt sich das Pro-
                           gramm wie folgt dar:


A
B

C


                                                                                                     F
D
                                                                                                     G




E




A   Menüleiste                      E Wertefenster
B   Symbolleiste                    F Konstruktionsbereich
C   Eingestellte Standard-Sprosse   G Fangpunkte
D   Werkzeuge
Abb. A-1      Oberfläche nach dem Programmstart


                           Im oberen Bereich befinden sich jeweils von links nach rechts die Menüleiste
                           (A), die Symbolleiste (B) sowie die definierte Standard-Sprosse (C). Unter der
                           Standard-Sprosse finden Sie die Werkzeuge (D) und das Wertefenster (E). Am
                           rechten Bildschirmrand befinden sich die Fangpunkte (G). Die große Fläche in
                           der Mitte ist der Konstruktionsbereich (F).

                               Elemente verschieben
                               Mit Ausnahme der Menüleiste können Sie alle Elemente mit der Maus an-
                               fassen und beliebig verschieben. Dadurch können Sie den Konstruktions-
                               bereich variabel gestalten.




A+W CAD Designer (Bars) Überblick                                                                  A-17
Arbeiten mit A+W CAD Designer (Bars)                                                               Tutorial




                       Die Menüleiste
                       Die Menüleiste beinhaltet die für den Anwender wichtigsten Funktionen. Die
                       einzelnen Menüs können per Mausklick geöffnet werden. Einige Menüpunkte
                       können mit Hilfe von Tastenkombinationen direkt geöffnet werden.




                       Die Symbolleiste
                       Die Funktion, die mit einer Symbolschaltfläche ausgeführt werden kann, steht
                       Ihnen auch über die Menüs zur Verfügung.
                       In A+W CAD Designer (Bars) gibt es folgende Symbolschaltflächen:




                       Erläuterung der einzelnen Symbole
                       Im Anschluss finden Sie eine Auflistung der Symbol-Schaltflächen und ihre
                       Bedeutung.

                       Symbol    Erläuterung

                                 Neue Konstruktion (Scheibe, Makro, Fassadenanlage)..
                                 Wenn Sie diese Symbol-Schaltfläche betätigen, erstellen Sie
                                 eine neue Datei. Befindet sich noch eine Konstruktion auf Ihrer
                                 Arbeitsfläche werden Sie gefragt, ob Sie diese speichern
                                 möchten. Anschließend wird die Arbeitsfäche geleert.

                                 Öffnen einer Konstruktion.
                                 Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie
                                 eine Datei öffnen. Es erscheint der Dialog Datei öffnen....

                                 Speichern einer Konstruktion.
                                 Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie
                                 eine Datei speichern.

                                 Drucken einer Konstruktion.
                                 Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie
                                 eine Konstruktion drucken. Bitte beachten Sie, dass der
                                 gewünschte Drucker eingerichtet ist.

                                 Importieren einer Übergabedatei.
                                 Wenn Sie diese Symbol-Schaltfläche betätigen, importieren
                                 Sie Dateien, die von übergeordneten Systemen an A+W CAD
                                 Designer (Bars) übergeben werden.

                                 Drucken einer Übergabedatei.
                                 Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie
                                 eine vom übergeordneten System übergebene Datei drucken.
                                 Bitte beachten Sie, dass der gewünschte Drucker eingerichtet
                                 ist.




A-18                                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                       Arbeiten mit A+W CAD Designer (Bars)




                      Symbol    Erläuterung

                                Ausschnitt vergrößern. Es stehen zwei Varianten zur
                                Verfügung:
                                • Pro Mausklick wird die Konstruktion um 10% vergrößert.
                                • Bei gehaltener Maustaste wird ein gewählter Bereich
                                  vergrößert.

                                Ausschnitt verkleinern. Pro Mausklick wird die Konstruktion
                                um 10% verkleinert.

                                Alles. Die Konstruktion wird so vergrößert oder verkleienert,
                                dass sie komplett dargestellt werden kann.

                                Rückgängigmachen der letzten Aktion.



                                Wiederherstellen der letzten rückgängig gemachten Aktion.



                                Hilfe aufrufen.



                                Stammdaten öffnen.
                                Wenn Sie diese Symbol-Schaltfläche betätigen, öffnet sich der
                                Dialog Stammdaten.

                         Symbolleiste verschieben
                         Sie können die Symbolleiste mit der Maus anfassen und an einer anderen
                         Stelle platzieren.




A+W CAD Designer (Bars) Überblick                                                               A-19
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       Das Wertefenster
                       Die Inhalte des Wertefensters ändern sich je nach Auswahl. Haben Sie inner-
                       halb einer Konstruktion eine Sprosse oder ein Segment ausgewählt, zeigt Ih-
                       nen A+W CAD Designer (Bars) den entsprechenden Artikel, die Breite, die
                       Farbe sowie die durchgehende Sprosse. Das Feld ID erscheint nur bei einer
                       A+W Business-Anbindung und wird dann automatisch gefüllt.




                          Werte für Vermaßung
                          Haben Sie die Vermaßung aktiviert, können Sie diese anklicken und der
                          Wert erscheint ebenfalls im Wertefenster. Etwaige Änderungen an den
                          Vermaßungen können im Wertefenster bequem vorgenommen werden.




                       Betätigen Sie die Schaltfläche [Mengen], zeigt Ihnen A+W CAD Designer
                       (Bars) die Anzahl der Konstruktionsmerkmale. Diese Merkmale sind relevant
                       für die Preisfindung.




A-20                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                      Die Standard-Sprosse
                      Bei der Sprosse, die Sie hier sehen, handelt es sich um die sogenannte Stan-
                      dard-Sprosse. D. h. solange Sie keine andere Sprosse wählen, werden Kons-
                      truktionen mit dieser Sprosse erstellt. Diese Sprosse wird bei jedem
                      Programm-Start aktiviert. Sie können die Sprosse jederzeit temporär wech-
                      seln, indem Sie aus der Kombobox eine andere Sprosse wählen.




                      Welche Sprosse als Standard-Sprosse definiert ist, legen Sie im Dialog
                      Stammdaten-Editor fest.


                      Der Mauszeiger
                      In Abhängigkeit von dem, was Sie gerade tun, kann der Mauszeiger von A+W
                      CAD Designer (Bars) sein Aussehen verändern. Im Anschluss haben wir die
                      unterschiedlichen Mauszeiger aufgelistet:
                      Im normalen Arbeitsbetrieb sieht der Mauszeiger sieht wie folgt aus:




                      Sie können mit ihm einzelne Elemente markieren bzw. Werkzeuge und Fang-
                      punkte aktivieren.
                      Wenn Sie mit Fangpunkten arbeiten und den Mauszeiger auf einem solchen
                      Fangpunkt platzieren, ändert er sein Aussehen zu einem Fadenkreuz:




                      Das Fadenkreuz erleichtert Ihnen das Arbeiten. Immer, wenn sich der Maus-
                      zeiger zu dem Fadenkreuz ändert, haben Sie den Fangpunkt quasi getroffen.
                      Zum Ändern der durchgehenden Sprosse, ändert der Mauszeiger sein Ausse-
                      hen wie folgt:




                      Wie Sie das Werkzeug anwenden, wird im Bereich Die Werkzeuge detailliert
                      erklärt.


A+W CAD Designer (Bars) Überblick                                                              A-21
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                       ZumVerlängern von Sprossen, ändert der Mauszeiger sein Aussehen wie
                       folgt:




                       Wie Sie das Werkzeug anwenden, wird im Bereich Die Werkzeuge detailliert
                       erklärt.


                       Ergänzende Informationen
                        “Die Werkzeuge verwenden” auf Seite A-40
                        “Ändert den Sprossendurchgang” auf Seite A-59
                        “Verlängert eine Sprosse” auf Seite A-60


                       Die Fangpunkte
                       In A+W CAD Designer (Bars) haben Sie die Möglichkeit, Hilfspunkte soge-
                       nannte Fangpunkte auf der Konstruktion zu platzieren. Diese Fangpunkte
                       können beliebig eingefügt werden und helfen Ihnen, Segmente (Sprossen,
                       Bögen, etc.) korrekt zu platzieren. Steht Ihr Mauszeiger auf der Scheibe und
                       Sie betätigen die rechte Maustaste, setzt A+W CAD Designer (Bars) automa-
                       tisch jeweils in den Ecken und in der Mitte der Fläche einen Fangpunkt. Diese
                       automatisch gesetzten Fangpunkte werden in grüner Farbe dargestellt. Fang-
                       punkte, die Sie manuell platzieren, werden in roter Farbe dargestellt.




                       Abb. A-2    Fangpunkte automatisch (grün), manuell (rot)


                       Das Arbeiten mit Fangpunkten
                       Die folgende Tabelle gibt Ihnen eine Überblick zu den Fangpunkten, die Ihnen
                       in A+W CAD Designer (Bars) zur Verfügung stehen. Detaillierte Beispiele zu
                       den einzelnen Fangpunkten finden Sie unter Beispiele zu Fangpunkten.

                       Symbol      Erläuterung

                                   Lösche
                                   Löscht einen Fangpunkt.
                                    “Löscht einen Fangpunkt” auf Seite A-39

                                   Lösche alle
                                   Löscht alle Fangpunkte.
                                    “Löscht alle Fangpunkt” auf Seite A-39




A-22                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                       Arbeiten mit A+W CAD Designer (Bars)




                      Symbol        Erläuterung

                                    Einteilung
                                    Eingabe der Anzahl der Intervall-Teilungen für Objekt, Distanz und
                                    Parallel.
                                     “Erzeugt Fangpunkt(e)” auf Seite A-24

                                    Schnittpunkt
                                    Erzeugt Fangpunkte in allen Schnittpunkten zweier Objekte.
                                     “Erzeugt Fangpunkt in Schnittpunkt” auf Seite A-25

                                    Relativ
                                    Erzeugt einen Fangpunkt relativ zu einem beliebigen Punkt.
                                     “Erzeugt einen relativen Fangpunkt” auf Seite A-25

                                    Objekt
                                    Erzeugt Fangpunkte auf Sprosse, Rahmen oder Scheibenrand.
                                     “Erzeugt Fangpunkte auf Objekten” auf Seite A-26

                                    Rechteck
                                    Erzeugt vier Fangpunkte auf den Ecken eines durch zwei Mausklicks
                                    beschriebenen Rechtecks.
                                     “Erzeugt vier Fangpunkte auf den Ecken eines Rechtecks” auf
                                      Seite A-27

                                    Flucht
                                    Erzeugt Fangpunkte in allen Schnittpunkten mit anderen Sprossen.
                                     “Erzeugt Fangpunkte in Kreuzungen” auf Seite A-28

                                    Distanz
                                    Erzeugt Fangpunkte auf einer Geraden.
                                     “Anzahl Fangpunkte von (Startpunkt) bis (Endpunkt) erzeugen” auf
                                      Seite A-29

                                    Bogenlänge I
                                    Erzeugt in wählbarer Entfernung einen Fangpunkt auf einem Bogen.
                                     “Anzahl Fangpunkte von (Startpunkt) bis (Endpunkt) erzeugen” auf
                                      Seite A-29

                                    Mittelpunkt I
                                    Erzeugt Fangpunkte in möglichen Mittelpunkten von Kreisen (2
                                    Punkte).
                                     “Platziere Fangpunkt in möglichem Mittelpunkt” auf Seite A-30

                                    Parallel
                                    Erzeugt Fangpunkte parallel versetzt zu einer Geraden.
                                     “Erzeugt Fangpunkte parallel zu einer Geraden” auf Seite A-33

                                    Bogenlänge II
                                    Erzeugt einen Fangpunkt in wählbarer Entfernung entlang des
                                    Bogens.
                                     “Platziere Fangpunkt in wählbarer Entfernung entlang eines Bo-
                                      gens” auf Seite A-34




A+W CAD Designer (Bars) Überblick                                                                    A-23
Arbeiten mit A+W CAD Designer (Bars)                                                             Tutorial




                       Symbol      Erläuterung

                                   Mittelpunkt II
                                   Erzeugt Fangpunkte im Mittelpunkt eines Kreises (3 Punkte).
                                    “Erzeugt Fangpunkt im Mittelpunkt eines Kreises (3 Punkte)” auf
                                     Seite A-35

                                   Richtung
                                   Erzeugt Fangpunkte vom Bezugspunkt aus unter einem einstellbaren
                                   Winkel.
                                    “Erzeugt Fangpunkte unter einstellbarem Winkel” auf Seite A-37

                                   Vektor
                                   Erzeugt einen Fangpunkt auf einer Geraden im wählbaren Abstand
                                   vom Startpunkt.
                                    “Erzeugt einen Fangpunkt auf einer Geraden mit wählbarem Ab-
                                     stand vom Startpunkt” auf Seite A-38


                       Beispiele zu Fangpunkten
                       Nachfolgend finden Sie zu jedem Fangpunkt ein Beispiel, in dem die Vorge-
                       hensweise erläutert wird.


                        Erzeugt Fangpunkt(e)
                          Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte durch die
                          Eingabe von Intervallen zu setzen.




                       1 Wählen Sie das Werkzeug aus. Es öffnet sich der Dialog Eingabe-Interval-
                         le für Fangpunkte.
                       2 Geben Sie die Anzahl der Intervalle (Bereiche zwischen den Fangpunkten)
                         ein, z. B. 3.
                       3 Es werden vier Fangpunkte werden gesetzt.




A-24                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt Fangpunkt in Schnittpunkt
                         Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte in den
                         Schnittpunkten von Sprossen zu setzen.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie die erste Sprosse an, z. B. die Horizontale.
                      3 Klicken Sie die zweite Sprosse an, z. B. die Vertikale.
                      4 Der Fangpunkt wird in dem Schnittpunkt der beiden ausgewählten Spros-
                        sen gesetzt.




                       Erzeugt einen relativen Fangpunkt
                         Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt relativ
                         zu einem bestimmten Punkt zu setzen.




                      1 Wählen Sie das Werkzeug aus.




A+W CAD Designer (Bars) Überblick                                                           A-25
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                       2 Klicken Sie den Bezugspunkt an, z. B. Schnittpunkt beider Sprossen.




                       3 Es öffnet sich der Dialog Eingabe - Relativer Abstand.
                       4 Geben Sie im Feld dx den horizontalen Abstand zum Bezugspunkt an,
                         z. B. 80 mm.
                       5 Geben Sie im Feld dy den vertikalen Abstand zum Bezugspunkt an, z. B.
                         40 mm.
                       6 Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.
                       7 Der Fangpunkt wird gemäß den eingegebenen Koordinaten gesetzt.




                        Erzeugt Fangpunkte auf Objekten
                          Mit dem Begriff Objekte können Sprossen, Rahmen oder der Scheiben-
                          rand gemeint sein.




                       1 Wählen Sie das Werkzeug aus.
                       2 Klicken Sie das Objekt an, auf dem die Fangpunkte platziert werden sollen,
                         z. B. die horizontale Sprosse.




                       3 Die Fangpunkte werden auf der Sprosse platziert.




                          Anzahl der Fangpunkte
                          Die Anzahl der Fangpunkte, die Sie platzieren, können Sie im Werkzeug
                          Anzahl ? einstellen.


A-26                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt vier Fangpunkte auf den Ecken eines Rechtecks
                         Mit diesem Werkzeug haben Sie die Möglichkeit, in einem Kreuz vier Fang-
                         punkte zu setzen. Sie müssen lediglich zwei Fangpunkte angeben und
                         A+W CAD Designer (Bars) setzt die beiden fehlenden automatisch.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie den ersten Fangpunkt an.




                      3 Klicken Sie den zweiten Fangpunkt an.




                      4 Die beiden fehlenden Fangpunkte werden platziert.




A+W CAD Designer (Bars) Überblick                                                          A-27
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                        Erzeugt Fangpunkte in Kreuzungen
                          Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte in Kreuzun-
                          gen zu setzen.




                       1 Wählen Sie das Werkzeug aus.
                       2 Klicken Sie das Objekt an, auf dem die Fangpunkte platziert werden sollen,
                         z. B. die horizontale Sprosse.




                       3 Der Fangpunkt wird in der Kreuzung platziert.




A-28                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                       Anzahl Fangpunkte von (Startpunkt) bis (Endpunkt) erzeugen
                         Mit diesem Werkzeug haben Sie die Möglichkeit, eine gewünschte Anzahl
                         von Fangpunkten auf einer Sprosse zu setzen. Sie geben lediglich den
                         Start- und Endpunkt an und A+W CAD Designer (Bars) platziert die Fang-
                         punkte automatisch.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie auf dem Objekt den Startpunkt an, z. B. die horizontale Spros-
                        se.




                      3 Klicken Sie auf dem Objekt den Endpunkt an.




                      4 Die Fangpunkte werden auf der Sprosse platziert.




                         Anzahl der Fangpunkte
                         Die Anzahl der Fangpunkte, die Sie platzieren, können Sie im Werkzeug
                         Anzahl ? einstellen.




A+W CAD Designer (Bars) Überblick                                                           A-29
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                        Platziere Fangpunkte entlang eines Bogens
                          Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt in einer
                          frei wählbaren Entfernung (Radius) auf einem Bogen zu platzieren.




                       1 Wählen Sie das Werkzeug aus.
                       2 Klicken Sie den Mittelpunkt des Bogens an.




                       3 Klicken Sie einen Punkt auf dem Bogen an. Es öffnet sich der Dialog Ein-
                         gabe: Bogen-Segmentlänge. Geben Sie -45 ein. Schließen Sie den Dialog
                         mit der Schaltfläche [OK].




                       4 Der Fangpunkt wird entsprechend platziert.




                          Fangpunkte setzen
                          Wie Sie auf dem Werkzeug-Symbol erkennen können, wird der Fangpunkt
                          im Uhrzeigersinn gesetzt. Durch die Eingabe der negativen 45 wurde der
                          Fangpunkt entgegen des Uhrzeigersinns gesetzt.


                        Platziere Fangpunkt in möglichem Mittelpunkt
                          Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt als Mit-
                          telpunkt eines Kreises zu platzieren.




                       1 Wählen Sie das Werkzeug aus.
                       2 Klicken Sie den ersten Punkt auf dem Bogen an.



A-30                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                      3 Klicken Sie den zweiten Punkt auf dem Bogen an. Es öffnet sich der Dialog
                        Eingabe: Radius. Geben Sie 200 ein. Schließen Sie den Dialog mit der
                        Schaltfläche [OK].




                      4 Die Fangpunkte werden entsprechend platziert.




A+W CAD Designer (Bars) Überblick                                                           A-31
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       Durch diese Eingabe war es A+W CAD Designer (Bars) möglich, zwei Fang-
                       punkte zu setzen. Zur Verdeutlichung haben wir in der folgenden Grafik die
                       entsprechenden Kreise eingezeichnet. Wir erinnern uns, als Radius 200 ein-
                       gegeben zu haben.




                                                           20
                                                             0




A-32                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                     Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt Fangpunkte parallel zu einer Geraden
                         Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte parallel zu
                         einer Sprosse zu platzieren.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie den Startpunkt des Objektes an, zu dem die Fangpunkte par-
                        allel platziert werden sollen, z. B. die horizontale Sprosse.




                      3 Klicken Sie den Endpunkt des Objektes an, zu dem die Fangpunkte paral-
                        lel platziert werden sollen. Es öffnet sich der Dialog Eingabe: Paralleler Ab-
                        stand. Geben Sie 100 ein. Schließen Sie den Dialog mit [OK].




                      4 Die Fangpunkte werden platziert.




A+W CAD Designer (Bars) Überblick                                                               A-33
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                        Platziere Fangpunkt in wählbarer Entfernung entlang eines Bogens
                          Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt in ei-
                          nem definierten Abstand entlang eines Bogens zu platzieren.




                       1 Wählen Sie das Werkzeug aus.
                       2 Klicken Sie den Mittelpunkt des Kreises an.




                       3 Klicken Sie einen Punkt auf dem Bogen an. Es öffnet sich der Dialog Ein-
                         gabe: Bogenlänge. Geben Sie 100 ein. Schließen Sie den Dialog mit der
                         Schaltfläche [OK].




A-34                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                      4 Der Fangpunkt wird platziert.




                      Zur Verdeutlichung haben wir in der folgenden Grafik den entsprechenden
                      Kreis eingezeichnet. Wir erinnern uns, als Bogenlänge 100 eingegeben zu ha-
                      ben.




                                                 0
                                               10




                       Erzeugt Fangpunkt im Mittelpunkt eines Kreises (3 Punkte)
                         Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt in den
                         Mittelpunkt eines durch drei Punkte definierten Bogens zu platzieren.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie den ersten Punkt auf dem Bogen an.




A+W CAD Designer (Bars) Überblick                                                          A-35
Arbeiten mit A+W CAD Designer (Bars)                                                     Tutorial




                       3 Klicken Sie den zweiten Punkt auf dem Bogen an.




                       4 Klicken Sie den dritten Punkt auf dem Bogen an.




                       5 Der Fangpunkt wird platziert.




                       Zur Verdeutlichung haben wir in der folgenden Grafik den entsprechenden
                       Kreis eingezeichnet.




A-36                                                        A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt Fangpunkte unter einstellbarem Winkel
                         Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte in einem de-
                         finierten Winkel zu platzieren.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie den Bezugspunkt an. Es öffnet sich der Dialog Eingabe: Rich-
                        tung Winkel (Grad). Geben Sie ein, wie viel Grad der Winkel haben soll,
                        z. B. 45°. Es öffnet sich ein zweiter Dialog Eingabe: Richtung Länge (in
                        mm), z. B. 200.




                      3 Die Fangpunkte werden entsprechend gesetzt.




                         Anzahl der Fangpunkte
                         Die Anzahl der Fangpunkte, die Sie platzieren, können Sie im Werkzeug
                         Anzahl ? einstellen.




A+W CAD Designer (Bars) Überblick                                                         A-37
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                        Erzeugt einen Fangpunkt auf einer Geraden mit wählbarem Abstand
                         vom Startpunkt
                          Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt auf ei-
                          ner Geraden zu platzieren.




                       1 Wählen Sie das Werkzeug aus.
                       2 Klicken Sie den Bezugspunkt an.




                       3 Klicken Sie einen Punkt in der gewünschten Richtung an. Es öffnet sich der
                         Dialog Eingabe: Abstand. Geben Sie den Abstand ein, z. B. 200.




                       4 Der Fangpunkt wird entsprechend gesetzt.




A-38                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Löscht einen Fangpunkt
                         Mit diesem Werkzeug haben Sie die Möglichkeit, einen einzelnen Fang-
                         punkt durch anklicken zu löschen.




                      1 Wählen Sie das Werkzeug aus.
                      2 Klicken Sie den Fangpunkt an, den Sie löschen möchten (zweiter von
                        links).
                      3 Der Fangpunkt wird gelöscht.




                       Löscht alle Fangpunkt
                         Mit diesem Werkzeug haben Sie die Möglichkeit, alle Fangpunkt mit einem
                         Klick zu löschen.




                      1 Wählen Sie das Werkzeug aus.
                      2 Die Fangpunkte werden alle gelöscht.




A+W CAD Designer (Bars) Überblick                                                          A-39
Arbeiten mit A+W CAD Designer (Bars)                                                            Tutorial




                       Die Werkzeuge
                       A+W CAD Designer (Bars) verfügt über eine Reihe von Werkzeugen, deren
                       Funktion Ihnen das Arbeiten erleichtern. Die Werkzeuge stehen Ihnen auch
                       über die Menüs zur Verfügung.




                       Die Werkzeuge verwenden
                       Die folgende Tabelle gibt Ihnen eine Überblick zu den Werkzeugen, die Ihnen
                       in A+W CAD Designer (Bars) zur Verfügung stehen. Detaillierte Beispiele zu
                       den einzelnen Werkzeugen finden Sie unter Beispiele zu den Werkzeugen.

                       Symbol     Erläuterung

                                  Element auswählen.



                                  Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten.
                                   “Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten” auf
                                    Seite A-42

                                  Erzeugt eine gerade (horizontale) Sprosse zwischen zwei
                                  Fangpunkten.
                                   “Erzeugt eine horizontale Sprosse” auf Seite A-43

                                  Erzeugt eine gerade (vertikale) Sprosse zwischen zwei Fangpunkten.
                                   “Erzeugt eine vertikale Sprosse” auf Seite A-44

                                  Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten unter
                                  Eingabe des Winkels.
                                   “Erzeugt eine gerade Sprosse mit zwei Mausklicks unter Angabe
                                    des Winkels” auf Seite A-45

                                  Erzeugt eine gebogene Sprosse zwischen drei Fangpunkten.
                                   “Erzeugt eine gebogene Sprosse mit drei Mausklicks” auf
                                    Seite A-47

                                  Erzeugt einen Sprossenkreis zwischen zwei Fangpunkten.
                                   “Erzeugt einen Sprossenkreis mit zwei Mausklicks” auf Seite A-49

                                  Erzeugt eine Sonne in einem lichten Feld.
                                   “Erzeugt eine Sonne in einem lichten Feld” auf Seite A-51

                                  Erzeugt einen Halbmond.
                                   “Erzeugt einen Halbmond” auf Seite A-54



A-40                                                            A+W CAD Designer (Bars) Überblick
Tutorial                                                         Arbeiten mit A+W CAD Designer (Bars)




                      Symbol        Erläuterung

                                    Erzeugt einen Bogen in einem lichten Feld.
                                     “Erzeugt einen Bogen in einem lichten Feld” auf Seite A-56

                                    Für eine 90° Kreuzung wird die Durchgangsrichtung geändert.
                                     “Ändert den Sprossendurchgang” auf Seite A-59

                                    Sprosse wird bis auf wählbares Objekt verlängert.
                                     “Verlängert eine Sprosse” auf Seite A-60

                                    Teilt alle Sprossen.
                                     “Alle Sprossen teilen” auf Seite A-64

                                    Verbindet alle Sprossen.
                                     “Alle Sprossen verbinden” auf Seite A-65

                                    Setzt oder löscht eine Sprosse in einem lichten Feld.
                                     “Löscht oder erzeugt eine Sprosse in einem lichten Feld” auf
                                      Seite A-66

                                    Erzeugt eine neue Scheibe. Nachdem Sie das Werkzeug aktiviert
                                    haben, klicken Sie auf die Scheibe und es öffnet sich der Dialog
                                     Softwarereferenz, “Neue Scheibe” auf Seite A-199

                                    Erzeugt aus Makro Sprossen-Aufteilung in der Scheibe.



                                    Öffnet den Dialog zur Eingabe von senkrechten und waagerechten
                                    Sprossen.

                                    Zeigt die entsprechenden Mengen im Wertebereich an.



                                    Ändert den YT-Zuschnitt.
                                     “YT-Zuschnitt ändern” auf Seite A-68


                      Abgesehen von den Werkzeugen, die Ihnen über die Symbole zur Verfügung
                      stehen, gibt es in A+W CAD Designer (Bars) noch die folgenden Werkzeuge
                      (Menü Bearbeiten):
                      •   Drehen
                           “Eine Sprosse drehen” auf Seite A-69
                      •   Spiegeln
                           “Eine Sprosse spiegeln” auf Seite A-71
                      •   Bewegen
                           “Eine Sprosse bewegen” auf Seite A-73




A+W CAD Designer (Bars) Überblick                                                                      A-41
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       Beispiele zu den Werkzeugen
                       Nachfolgend finden Sie zu jedem Werkzeug ein Beispiel, in dem die Vorge-
                       hensweise erläutert wird.


                        Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten
                          Mit diesem Werkzeug haben Sie die Möglichkeit, eine gerade Sprosse in
                          einem freien Winkel zu platzieren. Zum Starten der Sprosse dient ein
                          Fangpunkt. Die Länge der Sprosse definiert sich durch den von Ihnen ge-
                          wählten Endpunkt.




                       1 Setzen Sie entsprechende Fangpunkte.




                       2 Wählen Sie das Werkzeug aus.
                       3 Klicken Sie den Start(fang)punkt der Geraden an.




A-42                                                        A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                      4 Klicken Sie den End(fang)punkt der Geraden an.




                      5 Die Sprosse wird gesetzt.




                       Erzeugt eine horizontale Sprosse
                         Mit diesem Werkzeug haben Sie die Möglichkeit, eine horizontale Sprosse
                         zu platzieren. Zum Starten der Sprosse dient ein Fangpunkt. Die Länge der
                         Sprosse definiert sich durch den von Ihnen gewählten Endpunkt.




                      1 Setzen Sie entsprechende Fangpunkte.
                      2 Wählen Sie das Werkzeug aus.
                      3 Klicken Sie den Start(fang)punkt der Geraden an.




A+W CAD Designer (Bars) Überblick                                                            A-43
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       4 Klicken Sie den Endpunkt der Geraden an.




                       5 Die Sprosse wird gesetzt.




                        Erzeugt eine vertikale Sprosse
                          Mit diesem Werkzeug haben Sie die Möglichkeit, eine vertikal Sprosse zu
                          platzieren. Zum Starten der Sprosse dient ein Fangpunkt. Die Länge der
                          Sprosse definiert sich durch den von Ihnen gewählten Endpunkt.




                       1 Setzen Sie entsprechende Fangpunkte.
                       2 Wählen Sie das Werkzeug aus.
                       3 Klicken Sie den Start(fang)punkt der Geraden an.




A-44                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                      4 Klicken Sie den Endpunkt der Geraden an.




                      5 Die Sprosse wird gesetzt.




                       Erzeugt eine gerade Sprosse mit zwei Mausklicks unter Angabe des
                        Winkels
                         Mit diesem Werkzeug haben Sie die Möglichkeit, eine gerade Sprosse un-
                         ter Angabe eines frei definierbaren Winkels zu platzieren. Zum Starten der
                         Sprosse dient ein Fangpunkt. Die Länge der Sprosse definiert sich durch
                         den von Ihnen gewählten Endpunkt.




                      1 Setzen Sie entsprechende Fangpunkte.
                      2 Wählen Sie das Werkzeug aus.
                      3 Klicken Sie den Start(fang)punkt der Geraden an.




A+W CAD Designer (Bars) Überblick                                                            A-45
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       4 Klicken Sie den Endpunkt der Geraden an. Der Endpunkt dient gleichzeitig
                         als Sprossenlänge.




                       5 Es öffnet sich der Dialog Eingabe: Winkel. Geben Sie den gewünschten
                         Winkel ein, z. B. -45.
                       6 Die Sprosse wird gesetzt.




                          Negative Werte
                          Wie Sie auf dem Werkzeug-Symbol erkennen können, wird die Sprosse
                          entgegen des Uhrzeigersinns gesetzt. Durch die Eingabe der negativen 45
                          wird das Setzen der Sprosse im Uhrzeigersinn erreicht.




A-46                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt eine gebogene Sprosse mit drei Mausklicks




                         Mit diesem Werkzeug haben Sie die Möglichkeit, eine gebogene Sprosse
                         zu platzieren. Bei diesem Werkzeug stehen Ihnen zwei unterschiedliche
                         Vorgehensweisen zur Verfügung:
                         1. Sie klicken erst den Mittelpunkt des Bogens an, dann den Anfangs- und
                         anschließend den Endpunkt. Oder
                         2. Sie klicken erst den Anfangspunkt des Bogens an, dann den Endpunkt
                         und anschließend einen beliebigen Punkt auf dem Bogen.
                         Wir erläutern die unter 1. beschriebene Vorgehensweise:
                      1 Setzen Sie entsprechende Fangpunkte.




                      2 Wählen Sie das Werkzeug aus.
                      3 Klicken Sie den Mittelpunkt des Kreises an.




A+W CAD Designer (Bars) Überblick                                                           A-47
Arbeiten mit A+W CAD Designer (Bars)                                                  Tutorial




                       4 Klicken Sie den Startpunkt des Kreises an.




                       5 Klicken Sie den Endpunkt des Kreises an.




                       6 Die Sprosse wird gesetzt.




A-48                                                        A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt einen Sprossenkreis mit zwei Mausklicks




                         Mit diesem Werkzeug haben Sie die Möglichkeit, einen Sprossenkreis zu
                         erstellen. Den Sprossenkreis definieren Sie durch den Mittelpunkt des
                         Kreises und einen beliebigen Punkt auf dem Kreis.
                      1 Setzen Sie entsprechende Fangpunkte.




                      2 Wählen Sie das Werkzeug aus.
                      3 Klicken Sie den Mittelpunkt des Kreises an.




A+W CAD Designer (Bars) Überblick                                                        A-49
Arbeiten mit A+W CAD Designer (Bars)                                                  Tutorial




                       4 Klicken Sie den beliebigen (Fang)punkt auf dem Kreis an.




                       5 Der Sprossenkreis wird gesetzt.




A-50                                                        A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                       Erzeugt eine Sonne in einem lichten Feld




                         Mit diesem Werkzeug haben Sie die Möglichkeit, ein Strahlenmuster mit ei-
                         ner definierten Anzahl von Strahlen in einem lichten Feld zu erstellen. Die
                         einzelnen Strahlen können auf vier unterschiedliche Weisen platziert wer-
                         den. Wir erläutern zunächst die Platzierung von fünf Strahlen in gleichem
                         Winkel.
                      1 Erstellen Sie die Scheibe.




                      2 Wählen Sie das Werkzeug aus.
                      3 Klicken Sie die Scheibe (lichtes Feld) an, in der das Strahlenmuster plat-
                        ziert werden soll.




                         Es öffnet sich der Dialog Sonne und Sterne. Aktivieren Sie die Radiotaste
                         Gleiche Winkel. Wählen Sie aus der Kombobox Anzahl der Strahlen 5.
                         Schließen Sie den Dialog mit der Schaltfläche [OK].




A+W CAD Designer (Bars) Überblick                                                             A-51
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                       4 Das Strahlenmuster wird platziert.




                       5 Hätten Sie im Schritt 3 statt der Radiotaste Gleiche Winkel die Radiotaste
                         Strahlen in die Ecken aktiviert und als Zuschnittmethode Zuschnitt in Ecke
                         gewählt, wäre das Ergebnis wie folgt:




A-52                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                      6 Hätten Sie im Schritt 3 statt der Radiotaste Gleiche Winkel die Radiotaste
                        Strahlen in die Ecken aktiviert und als Zuschnittmethode Zuschnitt auf
                        senkrechten Rahmen gewählt, wäre das Ergebnis wie folgt:




                      7 Hätten Sie im Schritt 3 statt der Radiotaste Gleiche Winkel die Radiotaste
                        Strahlen in die Ecken aktiviert und als Zuschnittmethode Zuschnitt auf
                        waagerechten Rahmen gewählt, wäre das Ergebnis wie folgt:




A+W CAD Designer (Bars) Überblick                                                            A-53
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                        Erzeugt einen Halbmond




                          Dieses Werkzeug kommt dort zum Einsatz, wo ein Strahlenmuster platziert
                          wurde. Dort, wo sich die Strahlen der Sonne treffen, können Sie einen
                          Halbkreis einsetzen.
                       1 Erstellen Sie die Scheibe mit dem Strahlenmuster.




                       2 Wählen Sie das Werkzeug aus.
                       3 Bewegen Sie den Mauszeiger zu der Stelle, wo der Halbmond eingefügt
                         werden soll. An der entsprechenden Stelle ändert der Mauszeiger sein
                         Aussehen zu einem Halbkreis. Um dies zu verdeutlichen, haben wir die
                         weißen Sprossen gegen gelbe Sprossen ausgetauscht:




A-54                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                      Arbeiten mit A+W CAD Designer (Bars)




                         An der gewünschten Stelle angekommen, drücken Sie die linke Maustaste.
                      4 Im Wertefenster können Sie die notwendigen Einstellungen vornehmen:




                         Im Feld Radius stellt Ihnen A+W CAD Designer (Bars) die möglichen Werte
                         zur Verfügung. Wählen Sie den entsprechenden Wert aus.
                         Das Feld Orientierung bezieht sich auf die Ausrichtung des Strahlenmus-
                         ters. Sie können wählen, wie der Halbmond verlaufen soll:




                         Orientierung von unten nach oben        Orientierung von oben nach unten




                         Orientierung von rechts nach links      Orientierung von links nach rechts
                         Abb. A-3    Unterschiedliche Orientierungen




A+W CAD Designer (Bars) Überblick                                                             A-55
Arbeiten mit A+W CAD Designer (Bars)                                                         Tutorial




                        Erzeugt einen Bogen in einem lichten Feld




                          Mit diesem Werkzeug haben Sie die Möglichkeit, einen Sprossenbogen in
                          einem lichten Feld zu platzieren.
                       1 Erstellen Sie die Scheibe.




                       2 Wählen Sie das Werkzeug aus.
                       3 Klicken Sie die Scheibe (lichtes Feld) an, in der der Bogen platziert werden
                         soll.




A-56                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                      4 Im Wertefenster können Sie die notwendigen Einstellungen vornehmen:




                         Im Feld Modus stellt Ihnen A+W CAD Designer (Bars) folgende Möglich-
                         keiten zur Verfügung:
                         - Schneidet senkrechten Rahmen
                         - Trifft Ecke
                         - Schneidet waagerechten Rahmen
                         - Hat Radius von unten gemessen
                         - Hat Radius von oben gemessen
                         Das Feld Radius kann genutzt werden, wenn Sie im Feld Modus entweder
                         die Einstellung Hat Radius von unten gemessen oder die Einstellung Hat
                         Radius von oben gemessen gewählt haben. Dann können Sie einen ent-
                         sprechenden Radius eingeben.
                         Im Feld Orientierung können Sie angeben, wie der Sprossenbogen verlau-
                         fen soll. Erläuterungen zu finden Sie im Beispiel Erzeugt einen Halbmond.
                         Für die folgende Grafik wurden die Einstellungen Schneidet senkrechten
                         Rahmen und Von unten nach oben gewählt.




A+W CAD Designer (Bars) Überblick                                                           A-57
Arbeiten mit A+W CAD Designer (Bars)                                                     Tutorial




                       5 Für die folgende Grafik wurden die Einstellungen Schneidet waagerechten
                         Rahmen und Von unten nach oben gewählt.




                       6 Für die folgende Grafik wurden die Einstellungen Radius (100) von unten
                         gemessen und Von unten nach oben gewählt.




A-58                                                        A+W CAD Designer (Bars) Überblick
Tutorial                                                 Arbeiten mit A+W CAD Designer (Bars)




                       Ändert den Sprossendurchgang




                         Mit diesem Werkzeug haben Sie die Möglichkeit, die durchgehende Spros-
                         se zu ändern.
                      1 Ausgangssituation. Die senkrechte Sprosse ist die Durchgehende.




                      2 Wählen Sie das Werkzeug aus. Der Mauszeiger sieht wie folgt aus:




                      3 Klicken Sie die Sprossenkreuzung an.




A+W CAD Designer (Bars) Überblick                                                          A-59
Arbeiten mit A+W CAD Designer (Bars)                                                     Tutorial




                       4 Der Sprossendurchgang wird geändert. Die waagerechte Sprosse geht
                         durch.




                        Verlängert eine Sprosse




                          Mit diesem Werkzeug haben Sie die Möglichkeit, eine Sprosse zu verlän-
                          gern oder abzuschneiden.
                       1 Eine Sprosse soll verlängert werden.




                       2 Wählen Sie das Werkzeug aus. Der Mauszeiger sieht wie folgt aus:




A-60                                                        A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                      3 Klicken Sie die Sprosse an die verlängert werden soll. Die Sprosse wird in
                        roter Farbe dargestellt.




                      4 Klicken Sie das Objekt an, auf das die Sprosse verlängert werden soll.




                      5 Die Sprosse wird verlängert.




A+W CAD Designer (Bars) Überblick                                                            A-61
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       Oder, wenn Sie eine Sprosse schneiden möchten:




                       6 Wählen Sie das Werkzeug aus.




                       7 Klicken Sie die Sprosse an, die abgeschnitten werden soll. Die Sprosse
                         wird in roter Farbe dargestellt.




A-62                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                      8 Klicken Sie das Objekt an der Stelle an, an der die Sprosse geschnitten
                        werden soll.




                      9 Die Sprosse wird geschnitten.




A+W CAD Designer (Bars) Überblick                                                          A-63
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                        Alle Sprossen teilen




                          Mit diesem Werkzeug haben Sie die Möglichkeit, mit einem Mausklick alle
                          Sprossen zu teilen.
                       1 Ausgangssituation: Die beiden senkrechten Sprossen sind durchgehend.




                       2 Wählen Sie das Werkzeug aus. Die Sprossen werden geteilt:




A-64                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Alle Sprossen verbinden




                         Mit diesem Werkzeug haben Sie die Möglichkeit, mit einem Mausklick alle
                         Sprossen zu verbinden.
                      1 Ausgangssituation: Alle Sprossen sind geteilt.




                      2 Wählen Sie das Werkzeug aus. Die Sprossen werden verbunden:




A+W CAD Designer (Bars) Überblick                                                          A-65
Arbeiten mit A+W CAD Designer (Bars)                                                       Tutorial




                        Löscht oder erzeugt eine Sprosse in einem lichten Feld




                          Mit diesem Werkzeug haben Sie die Möglichkeit, einzelne Sprossen zu lö-
                          schen oder in einem lichten Feld eine gelöschte Sprosse erneut zu setzen.
                          Sprossendurchgänge werden entsprechend angepasst.
                       1 Ausgangssituation:




                       2 Wählen Sie das Werkzeug aus und platzieren Sie den Mauszeiger auf der
                         Sprosse, die entfernt werden soll. Der Mauszeiger ändert sein Aussehen.
                       3 Klicken Sie die linke Sprosse an.




A-66                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                      4 Die Sprosse wird entfernt und die Sprossendurchgänge werden ange-
                        passt.




                      5 Bewegen Sie den Mauszeiger an die Stelle, an der die Sprosse gelöscht
                        wurde, ändert er sein Aussehen und Sie können durch Betätigen der linken
                        Maustaste die gelöschte Sprosse wieder setzen.




A+W CAD Designer (Bars) Überblick                                                          A-67
Arbeiten mit A+W CAD Designer (Bars)                                                       Tutorial




                        YT-Zuschnitt ändern




                          Mit diesem Werkzeug können Sie bei einem Sprossenkreuz und zusätzlich
                          auftreffenden Y-Sprossen den Zuschnitt für die Y-Sprossen bestimmen.
                       1 Ausgangssituation: Werkzeug ist nicht aktiv. Es werden alle in den Kreu-
                         zungspunkt treffende Sprossen symmetrisch geschnitten.




                       2 Aktivieren Sie das Werkzeug aus. Das Sprossenkreuz wird normal berech-
                         net und nur die beiden Y-Teile auf das Kreuz geschnitten:




A-68                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Eine Sprosse drehen
                         Mit diesem Menüpunkt haben Sie die Möglichkeit, mit drei Mausklicks eine
                         Sprosse gedreht zu duplizieren.
                         Bearbeiten > Drehen
                      1 Ausgangssituation: Die zu drehende Sprosse ist markiert.




                      2 Wählen Sie den Menüpunkt aus. Klicken Sie den Rotationsmittelpunkt an.




A+W CAD Designer (Bars) Überblick                                                           A-69
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       3 Klicken Sie den ersten Bezugspunkt für die Rotation an.




                       4 Klicken Sie den zweiten Bezugspunkt für die Rotation an.




                       5 Die Sprosse wird dupliziert gedreht.




A-70                                                            A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                       Eine Sprosse spiegeln
                         Mit diesem Menüpunkt haben Sie die Möglichkeit, mit zwei Mausklicks eine
                         Sprosse horizontal oder vertikal zu spiegeln.
                         Bearbeiten > Spiegeln
                      1 Ausgangssituation: Die zu spieglende Sprosse ist markiert.




                      2 Wählen Sie den Menüpunkt aus. Klicken Sie den ersten Punkt auf der
                        Spiegelgeraden an.




A+W CAD Designer (Bars) Überblick                                                           A-71
Arbeiten mit A+W CAD Designer (Bars)                                                   Tutorial




                       3 Klicken Sie den zweiten Punkt auf der Spiegelgeraden an.




                       4 Die Sprosse wird dupliziert gespiegelt.




A-72                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                 Arbeiten mit A+W CAD Designer (Bars)




                       Eine Sprosse bewegen
                         Mit diesem Menüpunkt haben Sie die Möglichkeit, eine markierte Sprosse
                         zu verschieben.
                         Bearbeiten > Bewegen
                      1 Ausgangssituation: Die zu bewegende Sprosse ist markiert.




                      2 Wählen Sie den Menüpunkt aus. Drücken Sie die linke Maustaste und hal-
                        ten Sie diese gedrückt. Bewegen Sie die Sprosse.




A+W CAD Designer (Bars) Überblick                                                         A-73
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       Die Vermaßungswerkzeuge
                       A+W CAD Designer (Bars) verfügt über zwei Vermaßungswerkzeuge, die Sie
                       bei Ihrer täglichen Arbeit unterstützen. Mit diesen Werkzeugen können Sie
                       zwischen der Vermaßung von absoluten und relativen Bohrpunkten hin und
                       her schalten und festlegen, ob die Scheibe oder der Rahmen der Bezugspunkt
                       für die Vermaßung sein soll.
                       Mit diesem Werkzeug können Sie wählen, wie die Darstellung der Vermaßung
                       erfolgen soll. Das Programm unterscheidet zwischen der Vermaßungsdarstel-
                       lung von:
                       •   Absoluten Bohrpunkten
                       •   Relativen Bohrpunkten
                       In deaktiviertem Zustand erfolgt die Vermaßung der absoluten Bohrpunkte
                       und das Werkzeug sieht wie folgt aus:




                       In aktiviertem Zustand erfolgt die Vermaßung der relativen Bohrpunkte und
                       das Werkzeug sieht wie folgt aus:




                       Mit diesem Werkzeug wählen Sie, ob die Vermaßung mit Bezug auf den Rah-
                       men oder mit Bezug auf die Scheibe erfolgen soll.
                       In deaktiviertem Zustand erfolgt die Vermaßung mit Bezug auf den Rahmen
                       und das Werkzeug sieht wie folgt aus:




                       In aktiviertem Zustand erfolgt die Vermaßung mit Bezug auf die Scheibe und
                       das Werkzeug sieht wie folgt aus:




                           Checkbox Vermaßung aktivieren
                           Um die Symbol-Schaltflächen benutzen zu können, müssen Sie die Check-
                           box Vermaßung im Dialog Einstellungen... aktivieren.


                       Weitere Informationen zu den Vermaßungswerkzeugen
                        “Vermaßung von Bohrpunkten darstellen” auf Seite A-81
                        Softwarereferenz, “Vermaßung” auf Seite A-242



A-74                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                     Arbeiten mit A+W CAD Designer (Bars)




                      Einstellungen
                      Lernziele

                      • Vermaßung in A+W CAD Designer (Bars) kennenlernen und verstehen
                      • Nummerieren der Sprossen verstehen
                      • Unterschied zwischen der Vermaßung von absoluten und relativen Bohrpunkten
                        verstehen
                      • Unterschied bei der Vermaßung von Bohrpunkten in Bezug auf Rahmen und
                        Scheibe verstehen
                      • Maßsysteme kennenlernen
                      • Programm in einer anderen Sprache starten


                      Nutzen

                      Um A+W CAD Designer (Bars) effizient bedienen zu können ist es wichtig, die
                      Einstellungen korrekt vorzunehmen. Für mehrsprach ig-arbeitende Unternehmen
                      kann A+W CAD Designer (Bars) während der Laufzeit auf eine andere Sprache
                      gestellt werden. So entfällt das Speichern, Schließen und der Neustart.


                      Merke

                      Vermaßung                 Die Vermaßung von Sprossen-Konstruktionen kann
                                                aktiviert oder deaktiviert werden.

                      Maßsystem                 A+W CAD Designer (Bars) kann mm oder Inch
                                                darstellen.

                      Sprache zur Laufzeit      Die Programm-Sprache kann zur Laufzeit umgestellt
                      umstellen                 werden.

                      Ziffern, Fräspunkte und   Die Darstellung von Ziffern, Fräspunkten und Pfeilen
                      Pfeile                    kann nur erfolgen, wenn die Checkbox Vermaßung
                                                aktiv ist!




A+W CAD Designer (Bars) Überblick                                                                 A-75
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                       Vermaßungen ein- und ausblenden
                       In A+W CAD Designer (Bars) können Sie entscheiden, ob und wenn ja wie
                       eine Vermaßung erfolgen soll. Für einen besseren Überblick können Sie sich
                       die Sprossen Ihrer Konstruktion alphabetisch nummeriert darstellen lassen.
                       Bei Bedarf kann die Vermaßung auch mit Pfeilen erfolgen. Darüber hinaus ha-
                       ben Sie die Möglichkeit, die Fräspunkte optisch darzustellen.
                       Je nachdem, welche Informationen Sie benötigen, können Sie in A+W CAD
                       Designer (Bars) für die Bohrpunkte verschiedene Vermaßungsdarstellungen
                       wählen.


                        So aktivieren Sie die Vermaßung
                       1 Wählen Sie im Menü Ansicht > Einstellungen.
                          Der Dialog Einstellungen... wird geöffnet. Das Register Vermaßung wird
                          automatisch geöffnet.
                       2 Aktivieren Sie die Checkbox Vermaßung.




A-76                                                         A+W CAD Designer (Bars) Überblick
Tutorial                                                    Arbeiten mit A+W CAD Designer (Bars)




                         Die beiden folgenden Grafiken zeigen den Unterschied zwischen ohne und
                         mit Vermaßung:




                         Abb. A-4    Ergebnis, wenn Checkbox nicht aktiv ist




                         Abb. A-5    Ergebnis, wenn Checkbox aktiv ist




A+W CAD Designer (Bars) Überblick                                                          A-77
Arbeiten mit A+W CAD Designer (Bars)                                                               Tutorial




                        So erfolgt eine Vermaßung mit Pfeilen
                       1 Wählen Sie im Menü Ansicht > Einstellungen.
                          Der Dialog Einstellungen... wird geöffnet. Das Register Vermaßung wird
                          automatisch geöffnet.
                       2 Aktivieren Sie die Checkbox Vermaßung.
                       3 Aktivieren Sie die Checkbox Pfeile.




                          Die folgende Grafik zeigt das entsprechende Ergebnis:




                          Abb. A-6     Mit dieser Einstellung erfolgt eine Vermaßung mit Pfeilen




A-78                                                             A+W CAD Designer (Bars) Überblick
Tutorial                                                   Arbeiten mit A+W CAD Designer (Bars)




                       So werden die Sprossen mit Ziffern versehen
                      1 Wählen Sie im Menü Ansicht > Einstellungen.
                         Der Dialog Einstellungen... wird geöffnet. Das Register Vermaßung wird
                         automatisch geöffnet.
                      2 Aktivieren Sie die Checkbox Vermaßung.
                      3 Aktivieren Sie die Checkbox Ziffern an Sprossen.




                         Die folgende Grafik zeigt das entsprechende Ergebnis:




                         Abb. A-7    Ergebnis der Vermaßung mit Ziffern


                         Gleiche Sprossen erhalten dann den gleichen Buchstaben.




A+W CAD Designer (Bars) Überblick                                                          A-79
Arbeiten mit A+W CAD Designer (Bars)                                                      Tutorial




                        So können Sie sich Fräspunkte anzeigen lassen
                       1 Wählen Sie im Menü Ansicht > Einstellungen.
                          Der Dialog Einstellungen... wird geöffnet. Das Register Vermaßung wird
                          automatisch geöffnet.
                       2 Aktivieren Sie die Checkbox Vermaßung.
                       3 Aktivieren Sie die Checkbox Fräspunkte.




                          Die folgende Grafik zeigt das entsprechende Ergebnis:




                          Abb. A-8     Ergebnis der Darstellung von Fräspunkten




A-80                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                        Arbeiten mit A+W CAD Designer (Bars)




                         Vermaßung von Bohrpunkten darstellen
                         In A+W CAD Designer (Bars) können Sie wählen, wie die Darstellung der Ver-
                         maßung erfolgen soll. Das Programm unterscheidet zwischen der Verma-
                         ßungsdarstellung von:
                         •   Absoluten Bohrpunkten
                         •   Relativen Bohrpunkten
                         Die Vermaßungsdarstellung der Bohrpunkte ist immer in Zusammenhang mit
                         der Einstellung des Bereiches Bezug auf zu sehen. Dort geben Sie vor, ob die
                         Vermaßung mit Bezug auf den Rahmen oder mit Bezug auf die Scheibe erfol-
                         gen soll.
                         Um Ihnen die unterschiedlichen Einstellungen zu verdeutlichen, folgen im An-
                         schluss einige Bilder.
                         Unterschied absolute Bohrpunkte/relative Bohrpunkte mit Bezug auf Rahmen:




Vermaßung: Relative Bohrpunkte                     Vermaßung: Absolute Bohrpunkte
Abb. A-9    Unterschied relative Bohrpunkte zu absoluten Bohrpunkten mit Bezug auf Rahmen


                         Die Vermaßungsdarstellung der relativen Bohrpunkte nimmt im Gegensatz
                         zur Vermaßungsdarstellung der absoluten Bohrpunkte weniger Platz auf der
                         Arbeitsfläche in Anspruch. Dafür werden Sie mit weniger Informationen ver-
                         sorgt. Bei der Vermaßung der relativen Bohrpunkte können Sie z. B. auf den
                         ersten Blick nicht erkennen, bei wie vielen mm ein zweiter Bohrpunkt sitzt. Die
                         für Sie sinnvolle Vermaßungsdarstellung hängt auch von der Komplexität Ihrer
                         Arbeit ab.
                         Unterschied absolute Bohrpunkte/relative Bohrpunkte mit Bezug auf Scheibe




A+W CAD Designer (Bars) Überblick                                                                 A-81
Arbeiten mit A+W CAD Designer (Bars)                                                            Tutorial




Vermaßung: Relative Bohrpunkte                      Vermaßung: Absolute Bohrpunkte
Abb. A-10   Unterschied relative Bohrpunkte zu absoluten Bohrpunkten mit Bezug auf Scheibe


                         Zu dieser Schulungseinheit gehören:
                          Softwarereferenz, “Vermaßung” auf Seite A-242


                         Maße eingeben
                         In A+W CAD Designer (Bars) haben Sie die Möglichkeit, die Maßeinheit ein-
                         zustellen.
                         Maße können in folgenden Einheiten dargestellt werden:
                         •   mm
                         •   Zoll
                         Für die Maßeinheit Zoll kann darüber hinaus zwischen folgenden Eingaben
                         gewählt werden:
                         •   Eingabe in Brüchen
                         •   Eingabe Dezimal

                             Umrechnung von Maßeinheiten
                             A+W CAD Designer (Bars) kann in unterschiedlichen Maßeinheiten arbei-
                             ten. Es ist sogar möglich, die eingestellte Maßeinheit während der Laufzeit
                             umzustellen. Vorhandene Stammdaten werden dann umgerechnet!




A-82                                                               A+W CAD Designer (Bars) Überblick
Tutorial                                                    Arbeiten mit A+W CAD Designer (Bars)




                       So stellen Sie die Maßeinheit ein, in der Sie arbeiten möchten
                      1 Wählen Sie im Menü Ansicht > Einstellungen.
                         Der Dialog Einstellungen... wird geöffnet. Wechseln Sie zum Register Ma-
                         ße.
                      2 Möchten Sie in mm arbeiten, aktivieren Sie die Radiotaste Maßeingabe in
                        mm.




                         Möchten Sie in Inch arbeiten, müssen Sie entscheiden, ob Sie die Eingabe
                         in Brüchen oder dezimal vornehmen.
                         Soll die Eingabe in Brüchen erfolgen, aktivieren Sie die Radiotaste Maß-
                         eingabe in Zoll (Brüche). Sie müssen dann im Feld Bruch Nenner noch den
                         Nenner angeben. Bsp.: 32 für 1/32
                         Soll die Eingabe dezimal erfolgen, aktivieren Sie die Radiotaste Maßeinga-
                         be in Zoll (dezimal). Sie müssen dann im Feld Genauigkeit (dezimal) die
                         Anzahl der Nachkommastellen angeben. Bsp.: 3 für 2,345.


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Maße” auf Seite A-244




A+W CAD Designer (Bars) Überblick                                                            A-83
Arbeiten mit A+W CAD Designer (Bars)                                                              Tutorial




                       Programmsprache wählen
                       A+W CAD Designer (Bars) kann zur Zeit in sieben Sprachen betrieben wer-
                       den. Die Programmsprache kann während der Laufzeit umgestellt werden.
                       Ein Neustart ist nicht erforderlich.


                        So wählen Sie eine andere Sprache
                       1 Wählen Sie im Menü Ansicht > Einstellungen.
                          Der Dialog Einstellungen... wird geöffnet. Wechseln Sie zum Register
                          Sprachauswahl.




                          Abb. A-11    CAD Designer arbeitet in der Sprache des Betriebssystems


                       2 Wählen Sie aus der Kombobox die gewünschte Sprache aus.
                       3 Schließen Sie den Dialog über die Schaltfläche [OK]. Das Programm prä-
                         sentiert sich in der gewählten Sprache.


                       Zu dieser Schulungseinheit gehören:
                        Softwarereferenz, “Sprachauswahl” auf Seite A-245




A-84                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                     Arbeiten mit A+W CAD Designer (Bars)




                      Stammdaten in A+W CAD Designer
                      (Bars)
                      Lernziele

                      •   Unterschiedliche Sprossentypen kennenlernen
                      •   Unterschied zwischen den Sprossentypen verstehen
                      •   Anlegen neuer Sprossen beherrschen
                      •   Festlegen der Standard-Sprosse beherrschen
                      •   Den Stammdaten-Bereich mit einem Passwort schützen


                      Nutzen

                      Um mit A+W CAD Designer (Bars) arbeiten zu können, müssen als erstes die
                      Stammdaten also die Sprossen definiert werden.


                      Definitionen

                      Glasteilende Sprosse      Glasteilende Sprossen sind echte Sprossen, die eine
                                                Scheibe in mehrere kleine Scheiben teilen.

                      Innenliegende Sprosse     Innenliegende Sprosse sind Sprosse, die in den
                                                Scheibenzwischenraum eingebaut werden.

                      Aufgesetzte Sprosse       Aufgesetzte Sprossen bestehen aus eingebauten
                                                Abstandhalterprofilen, und sind mit der Oberfläche
                                                verbunden.

                      Wegfallsprosse            Sprossen oder auch Sprossenteile, die zur Erstellung
                                                einer Sprossenkonstruktion benötigt werden.

                      Randstopfen               Schließt die Sprosse und dient als Verbindung zum
                                                umlaufenden Abstandhalter.

                      Durchgang                 Dieser Bereich dient der Festlegung von
                                                Sprossendurchgängen, die von außen mittels
                                                Übergabedateien an A+W CAD Designer (Bars)
                                                übergeben werden. Beim eigenen Konstruieren von
                                                Sprossenbildern werden die Durchgänge im Dialog
                                                Muster Senkrecht/Waagerecht festgelegt.


                      Merke

                      Konfiguration             Der Stammdatenbereich kann vom Anwender selbst
                                                konfiguriert werden.




A+W CAD Designer (Bars) Überblick                                                                    A-85
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                       Sprossentypen
                       Sprossen verändern das Aussehen Ihres Hauses dezent aber wirkungsvoll,
                       indem sie das Fassadenbild elegant untergliedern und ihm einen unverwech-
                       selbaren Charakter verleihen. Schon auf den ersten Blick vermitteln sie den
                       Eindruck eines liebevollen aber nicht aufdringlichen Details.
                       Es gibt verschiedene Arten von Sprossen. Grundsätzlich unterscheiden wir
                       zwischen:
                       •   Glasteilenden Sprossen
                       •   Innenliegenden Sprossen
                       •   Aufgesetzten Sprossen
                       Im Anschluss finden Sie entsprechende Erläuterungen zu den Sprossenty-
                       pen:

                       Glasteilende Sprossen
                       Glasteilende Sprossen sind echte Sprossen bei einem Fenster. In den Fens-
                       terrahmen ist nicht eine Scheibe eingelassen, vielmehr sind vier und mehr
                       kleinere Glasscheiben mit Holz- oder Kunststoffsprossen eingebaut, die ihrer-
                       seits wiederum das gesamte Fenster bilden. Echte Sprossenfenster sind na-
                       turgemäß wesentlich teuerer als Imitate wie geklebte Sprossen, aufgesetzte
                       Sprossen oder Vorsatzsprossen.




                       Abb. A-12    Darstellung einer glasteilenden Sprosse


                       Vorteile von glasteilenden Sprossen:
                       •   Echte Sprossen können das Element stabilisieren, da sie Last abtragen
                       •   Sie haben eine sehr gute plastische optische Wirkung
                       •   Sie sind bis zu einer Breite von 138 mm machbar.
                       Nachteile von glasteilenden Sprossen:
                       •   Durch die erhöhten laufenden Meter am Scheibenrandverbund kommt es
                           zu erhöhtem Wärmeverlust
                       •   Die Sprossen können nicht sehr schmal gefertigt werden
                       •   Nicht reinigungsfreundlich.




A-86                                                            A+W CAD Designer (Bars) Überblick
Tutorial                                                      Arbeiten mit A+W CAD Designer (Bars)




                      Innenliegende Sprossen
                      Bei größeren Glasflächen, vor allem auch bei verglasten Fassaden- oder Ge-
                      bäudeteilen kann die innenliegende Sprosse schnell zur ersten Wahl werden.
                      Das problemlose Reinigen aufgrund der nicht unterbrochenen Oberflächen ist
                      nur ein Vorteil. Auch im Segment der Sicherheitsgläser ist die innenliegende
                      Sprosse im Vorteil. Letztendlich ist die innenliegende Sprosse auch die preis-
                      werteste Variante, um den Fenstern des Gebäudes ein mehr an Individualität
                      zu verleihen.




                      Abb. A-13     Darstellung einer innenliegenden Sprosse


                      Vorteile von innenliegenden Sprossen:
                      •   Günstige Variante
                      •   Scheiben können komplett geputzt werden
                      •   Geringerer Wärmeverlust als bei glasteilenden Sprossen.
                      Nachteile von innenliegenden Sprossen:
                      •   Eine plastische optische Wirkung fehlt
                      •   In seltenen Fällen kann es zu Klappergeräuschen kommen
                      •   Eignet sich nicht für jeden Luftzwischenraum.

                      Aufgesetzte Sprossen
                      Geklebte Sprossen sind schmale Holzleisten, die von außen auf die Scheibe
                      geklebt werden, um den Effekt eines Sprossenfensters zu erzielen.




                      Abb. A-14     Darstellung einer aufgesetzten Sprosse




A+W CAD Designer (Bars) Überblick                                                             A-87
Arbeiten mit A+W CAD Designer (Bars)                                                     Tutorial




                       Vorteile von aufgesetzten Sprossen:
                       •   Sehr schmale Sprossen mit einer guten plastischen Wirkung sind machbar
                       •   Geringerer Wärmeverlust als bei glasteilenden Sprossen.
                       Nachteile von aufgesetzten Sprossen:
                       •   Teuerer als innenliegende Sprossen
                       •   In seltenen Fällen kann es zu Klappergeräuschen kommen
                       •   Nur bis zu einer geringen Breite machbar
                       •   Nicht reinigungsfreundlich.


                       Sprossenstäbe
                       Sprossen werden in Form von Stäben geliefert. Die Sprossenstäbe haben in
                       der Regel eine Länge von 6000 mm. Sprossenstäbe gibt es in unterschiedli-
                       chen Materialien:
                       •   Aluminium
                       •   Kunststoff
                       •   Holz
                       Durch verschiedene Breiten, Rundungen oder Profilierungen prägen sie das
                       Erscheinungsbild.




A-88                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                     Arbeiten mit A+W CAD Designer (Bars)




                      Wegfallsprossen
                      Bei den Wegfallsprossen handelt es sich um Sprossen, die zur Konstruktion
                      eines Bildes benötigt werden und anschließend ganz oder teilweise wieder
                      gelöscht werden.
                      Beispiel:
                      Fenster aus einem Halbkreis. Darin befindet sich ein Sprossenbogen mit
                      strahlenförmigen Sprossen.




                      Abb. A-15     Rundbogen mit Strahlenmuster


                      Das Strahlenmuster soll aber nur bis zur Bogensprosse gehen und nicht bis
                      zum oberen Scheibenrand. Wir teilen zunächst alle Sprossen mit dem ent-
                      sprechenden Werkzeug.




                      Abb. A-16     Rundbogen mit Strahlenmuster, Durchgang geteilt




A+W CAD Designer (Bars) Überblick                                                           A-89
Arbeiten mit A+W CAD Designer (Bars)                                                     Tutorial




                       Dann markieren wir die Sprossenteile zwischen dem Rundbogen und dem
                       oberen Scheibenrand.




                       Abb. A-17   Rundbogen mit Strahlenmuster, Sprossen markieren


                       Durch Betätigen der Taste <Entf> werden die markierten Sprossen gelöscht.
                       Diese Sprossen nennt man Wegfallsprossen.




                       Abb. A-18   Rundbogen mit Strahlenmuster, Sprossen gelöscht




A-90                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                  Arbeiten mit A+W CAD Designer (Bars)




                      Stammdaten anlegen
                      Bei den Stammdaten von A+W CAD Designer (Bars) handelt es sich aus-
                      schließlich um Sprossendaten. Als Stammdaten einer Sprosse gelten alle An-
                      gaben, die für eine hinreichende Beschreibung des Produktes erforderlich
                      sind. A+W CAD Designer (Bars) benötigt zur Verarbeitung von Sprossendaten
                      bzw. für die Konstruktion und Abbildung von Sprossenbildern die im Stamm-
                      daten-Editor erfragten technischen Angaben. Der Stammdaten-Editor stellt
                      alle Funktionen für das Verwalten und Ändern von Sprossendaten zur Verfü-
                      gung.
                      Den Stammdaten-Editor öffnen Sie über Stammdaten > Stammdaten-Editor:




A+W CAD Designer (Bars) Überblick                                                         A-91
Arbeiten mit A+W CAD Designer (Bars)                                                       Tutorial




                        So erfassen Sie eine neue Sprosse
                       1 Um eine neue Sprosse anzulegen, betätigen Sie die Schaltfläche [Hinzu-
                         fügen]. Es öffnet sich der Dialog Eingabe neuer Artikel.
                       2 Geben Sie die gewünschte Artikel-Nummer ein und betätigen Sie die
                         Schaltfläche [OK]. Der Dialog wird geschlossen.
                       3 Das Feld Name wird automatisch mit der eingegebenen Artikel-Nummer
                         vorbelegt. Sie können den Inhalt durch einen sprechenden Namen erset-
                         zen.
                       4 Im Feld Breite geben Sie die Breite der Sprosse ein.
                       5 Geben Sie im Feld Frästiefe den entsprechenden Wert ein. Das Feld Fräs-
                         tiefe wird bestimmt durch den verstellbaren Begrenzungsanschlag, gegen
                         den das vorher gekappte Sprossenende positioniert wird.
                          Die Frästiefe wird in A+W CAD Designer (Bars) optisch dargestellt:




                          Frästiefe 6,5 mm                         Frästiefe 3 mm
                          Abb. A-19    Darstellung unterschiedlicher Frästiefen


                       6 Das Feld Offset dient der Spezialbehandlung von Bohrmaschinen mit Off-
                         set-Bemaßung. Der Offset-Wert ist abhängig von der Sprosse.
                       7 Randabzug: Die Verbindung zum umlaufenden Abstandhalter erfolgt durch
                         angepasste Kunststoff-Stopfen und in seltenen Fällen mit einer Klemmfe-
                         der aus Stahl. Werden Kunststoff-Stopfen verwendet, müssen Sie beim
                         Anlegen der Stammdaten diesen Wert hinterlegen. Die Sprosse wird dann
                         automatisch um die Stärke des Stopfens gekürzt.




A-92                                                             A+W CAD Designer (Bars) Überblick
Tutorial                                                     Arbeiten mit A+W CAD Designer (Bars)




                         Die Randstopfen werden in A+W CAD Designer (Bars) optisch dargestellt:




                            A       B        C        D


                         A: Randstopfen 0 mm
                         B: Randstopfen 5 mm
                         C: Randstopfen 10 mm
                         D: Randstopfen 15 mm

                         Beispiel: Randabzug bei Sprossen

                         Das Fenster ist 600 mm breit von Rahmeninnenkante zu
                         Rahmeninnenkante. Der Kunststoff-Stopfen hat eine Breite von 3 mm (rechte
                         Seite/linke Seite). Somit ergibt sich eine Sprossenlänge von 594 mm.


                      8 Die Felder Spezial-Kreuzung und Breite-Kreuz gehören zusammen. Wenn
                        Sie die Checkbox Spezial-Kreuzung aktivieren können Sie im Feld Breite-
                        Kreuz einen Wert hinterlegen. Bei den Spezial-Kreuzungen gibt es keine
                        durchgehenden Sprossen. Dort, wo die Sprossen aufeinander treffen, wer-
                        den Steckverbindungen eingesetzt. Diese Steckverbindungen oder auch
                        Kreuzverbindungen nennt man in A+W CAD Designer (Bars) Spezial-
                        Kreuzung.
                         Um dies zu verdeutlichen, wurde im folgenden Beispiel das Kreuz um 4
                         mm breiter gemacht, als die Sprosse:




                         Breite der Sprosse: 26 mm              Breite Kreuz: 40 mm




A+W CAD Designer (Bars) Überblick                                                                A-93
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                       9 Geben Sie im Feld Stablänge die Länge des Sprossenstabes ein (die Län-
                         ge, in der Sie die Sprossenstäbe angeliefert bekommen).
                       10 Das Feld T-Zugabe wird verwendet, wenn eine Sprosse im rechten Winkel
                          auf eine andere Sprosse zugeschnitten wird. Dann wird die hier eingestell-
                          te Längenangabe zu der eigentlichen Sprossenlänge hinzuaddiert.
                       11 Die Radiotasten im Bereich Durchgang dienen der Festlegung von Spros-
                          sendurchgängen, die von außen mittels Übergabedateien an A+W CAD
                          Designer (Bars) übergeben werden. Beim eigenen Konstruieren von
                          Sprossenbildern werden die Durchgänge im Dialog Muster Senkrecht/
                          Waagerecht festgelegt.
                       12 Für einige Sprossensysteme (z. B. aufgesetzte Sprossen) und für 3-fach
                          ISO wird die doppelte Sprossenmenge benötigt. Wenn Sie die Checkbox
                          Doppelter Zuschnitt aktivieren, werden für den verwendeten Sprossentyp
                          die Zuschnittmengen automatisch verdoppelt.
                       13 Wenn Sie die Checkbox L-Felder mit Abzug aktivieren, werden die Rand-
                          stopfen der Sprosse nicht mit vermaßt. Das angezeigte Maß bezieht sich
                          nur auf die Sprossenlänge.
                          Um dies zu verdeutlichen, wurde im folgenden Beispiel eine Sprosse mit
                          einem Randstopfen von 3 mm gewählt:




                          Abb. A-20    Darstellung L-Felder mit Abzug


                       14 Wenn es in Ihrem Hause mehrere Sprossenfertigungslinien gibt, können
                          Sie die Sprossentypen auf unterschiedlichen Linien fertigen lassen. Das
                          Feld Liniennummer wird über spezielle Einstellungen in der INI-Datei akti-
                          viert.




A-94                                                            A+W CAD Designer (Bars) Überblick
Tutorial                                                     Arbeiten mit A+W CAD Designer (Bars)




                      15 Im letzten Schritt müssen Sie der Sprosse noch einen Farbcode zuweisen.
                         Sie können z. B. die RAL-Farbe als Farbcode definieren und im Feld Na-
                         men den dazugehörigen Namen hinterlegen. Beispiel: Farbcode: RAL
                         2000 Name: Gelborange.
                      16 Auf dem Dialog befinden sich noch zwei weitere Schaltflächen: [Start]. Bei-
                         de Schaltflächen dienen zur Definition der Standard-Sprosse. Ausführliche
                         Erläuterungen zur Standard-Sprosse finden Sie unter:
                          “Die Standard-Sprosse” auf Seite A-21


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Stammdaten-Editor” auf Seite A-235


                      Stammdaten schützen
                      Das Ändern der Stammdaten kann unter Umständen verherende Auswirkun-
                      gen auf die Produktion haben. Um dieses Risiko so gering wie möglich zu hal-
                      ten, gibt es in A+W CAD Designer (Bars) die Möglichkeit, die Stammdaten
                      durch ein Passwort zu schützen.


                       So schützen Sie Ihre Stammdaten mit einem Passwort
                      1 Öffnen Sie Stammdaten-Editor über Stammdaten > Stammdaten-Editor.
                      2 Aktivieren Sie die Checkbox Passwortschutz.
                      3 Verlassen Sie den Dialog mit der Schaltfläche [OK]. Beantworten Sie die
                        Sicherheitsabfrage mit [Ja]. Es öffnet sich der Dialog Passwort.
                      4 Geben Sie im Feld Passwort das gewünschte Passwort ein.
                      5 Wiederholen Sie das Passwort im Feld 1.
                      6 Betätigen Sie die Schaltfläche [OK]. Die Dialoge werden geschlossen.


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Passwort” auf Seite A-240




A+W CAD Designer (Bars) Überblick                                                             A-95
Arbeiten mit A+W CAD Designer (Bars)                                                        Tutorial




                       Übungen
                       In diesem Abschnitt lernen Sie, wie Sie einen Sprossenartikel in A+W CAD
                       Designer (Bars) anlegen, diesen als Standard-Sprosse definieren und den
                       Stammdaten-Bereich mit einem Passwort schützen.

                       Übung 1: Einen Sprossenartikel anlegen
                       Erfassen Sie einen Sprossenartikel. Dieser Sprossenartikel soll Ihnen bei der
                       Konstruktion von Sprossenbildern als Standard-Sprosse dienen. Um den
                       Stammdaten-Bereich vor unerwünschten Änderungen zu schützen, versehen
                       Sie ihn bitte mit einem Passwort.

                       Aufgabenstellung
                       Legen Sie einen Artikel mit folgenden Spezifikationen an:
                       •   Artikelnummer: 8500
                       •   Name der Sprosse: Aufgesetzte Sprosse
                       •   Farbcode: RAL 1004
                       •   Farbname: Goldgelb
                       •   Breite: 26 mm
                       •   Frästiefe: 6,5 mm
                       •   Randabzug: 3 mm
                       •   Stablänge: 6000 mm
                       •   Doppelter Zuschnitt

                       Weitere Anforderungen
                       •   Dieser Artikel soll zukünftig die Standard-Sprosse sein.
                       •   Schützen Sie den Stammdaten-Bereich mit einem Passwort (1111).

                       Übung 1: Lösung
                       Die einzelnen Schritte dieser Aufgabe werden in zwei Dialogen vorgenom-
                       men:
                       •   Dialog Stammdaten-Editor
                       •   Dialog Passwort (öffnet sich automatisch)


                        Artikel anlegen
                       1 Öffnen Sie den Dialog Stammdaten-Editor.
                       2 Betätigen Sie die Schaltfläche [Hinzufügen]. Es öffnet sich der Dialog Ein-
                         gabe neuer Artikel.
                       3 Geben Sie 8500 ein. Betätigen Sie die Schaltfläche [OK].
                       4 Geben Sie im Feld Name Aufgesetzte Sprosse ein.
                       5 Betätigen Sie die Schaltfläche [Start] um die Sprosse als Standard-Sprosse
                         zu definieren.
                       6 Geben Sie im Feld Breite 26 mm ein.
                       7 Geben Sie im Feld Frästiefe 6,5 mm ein.

A-96                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                    Arbeiten mit A+W CAD Designer (Bars)




                      8 Geben Sie im Feld Randabzug 3 mm ein.
                      9 Geben Sie im Feld Stablänge 6000 mm ein.
                      10 Aktivieren Sie die Checkbox Doppelter Zuschnitt.
                      11 Betätigen Sie im Bereich Farbcode die Schaltfläche [Hinzufügen]. Es öffnet
                         sich der Dialog Eingabe neuer Farbcode.
                      12 Geben Sie RAL 1004 ein. Betätigen Sie die Schaltfläche [OK]. Der neue
                         Eintrag wird in der Liste Farbcode aufgenommen und erscheint gleichzeitig
                         im Feld Name.
                      13 Markieren Sie den Eintrag RAL 1004 im Feld Name und überschreiben Sie
                         ihn mit Goldgelb.
                      14 Markieren Sie den Eintrag RAL 1004 und betätigen Sie die Schaltfläche
                         [Ändere]. Wählen Sie einen Gelbton aus und betätigen Sie die Schaltfläche
                         [OK].
                      15 Betätigen Sie anschließend die Schaltfläche [Start], um die Standard-Far-
                         be zuzuweisen.
                      16 Aktivieren Sie die Checkbox Passwortschutz.
                      17 Betätigen Sie die Schaltfläche [OK]. Es öffnet sich der Dialog Stammdaten
                         sichern?
                      18 Betätigen Sie die Schaltfläche [OK]. Es öffnet sich der Dialog Passwort.
                      19 Geben Sie im Feld Passwort 1111 ein.
                      20 Wiederholen Sie diese Eingabe im Feld Bestätigung.
                      21 Betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen.


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Stammdaten-Editor” auf Seite A-235
                       Softwarereferenz, “Passwort” auf Seite A-240




A+W CAD Designer (Bars) Überblick                                                            A-97
Sprossen                                                                       Tutorial




           Sprossen
           In diesem Abschnitt wird Ihnen gezeigt, wie Sie eigene Sprossenkonstruktio-
           nen erstellen. Dies ist immer dann notwendig, wenn keine Daten von einem
           übergeordneten Auftragsbearbeitungssystem übergeben werden, oder wenn
           Sie kein Standard-Sprossengitter erfassen wollen.




A-98                                             A+W CAD Designer (Bars) Überblick
Tutorial                                                                                      Sprossen




                      Neue Konstruktionen
                      Lernziele

                      •   Vorgehensweise zum Erstellen neuer Sprossenkonstruktionen verstehen
                      •   Modellrestriktionen kennenlernen und verstehen
                      •   Aufteilung von Sprossen kennenlernen und verstehen
                      •   Sprossen in vorhandenen Konstruktionen austauschen


                      Nutzen

                      Die vom Kunden gewünschten Sprossenkonstruktionen abbilden und umsetzen zu
                      können.


                      Definitionen

                      Modellparameter            Es gibt folgende Modellparameter:
                                                 • W(idth) = Gesamtbreite
                                                 • H(eight) Gesamthöhe
                                                 • H1, 2, ... = bei unterschiedlichen Höhen
                                                 • W1, 2, ... = bei unterschiedlichen Breiten
                                                 • R = Radius
                                                 • R1, 2, .... = bei unterschiedlichen Radien
                                                 • S = Stichhöhe
                                                 • <--> = Gespiegelte Darstellung:
                                                 • 0: ohne Spiegelung
                                                 • 1: horizontale Spiegelung
                                                 • @ = Drehwinkel:
                                                 • 90: Modell wird um 90 Grad im Uhrzeigersinn
                                                   gedreht.
                                                 • 180: Modell wird um 180 Grad im Uhrzeigersinn
                                                   gedreht.
                                                 • 270: Modell wird um 270 Grad im Uhrzeigersinn
                                                   gedreht.

                      Rückschnitt                Breite des Rahmens plus Versiegelungstiefe

                      SZR                        Abkürzung für Scheibenzwischenraum


                      Merke

                      Modell-Nummer              Die Modell-Nummer ist abhängig von dem
                                                 verwendeten Modell-Katalog.

                      Eigene Konstruktionen      Die nachfolgenden Erläuterungen betreffen A+W CAD
                                                 Designer (Bars)-Installationen ohne Anbindung an
                                                 A+W Business, A+W Enterprise oder A+W Production.




A+W CAD Designer (Bars) Überblick                                                                  A-99
Sprossen                                                                          Tutorial




           Allgemeine Vorgehensweise
           Das Erstellen von Sprossenkonstruktionen geschieht in drei Schritten:
           •   Form für die Konstruktion festlegen
           •   Eigenschaften definieren
           •   Sprossen platzieren
               – Waagerechtes und/oder senkrechtes Muster platzieren
               – Sprossen frei platzieren
               – Makro verwenden

           Form für die Konstruktion festlegen
           Die Arbeit beginnt mit der Auswahl einer entsprechenden Form, dem soge-
           nannten Modell. Die mögliche Auswahl hängt vom Umfang des benutzten Mo-
           dell-Katalogs in Ihrem Hause ab.




           A




                                                                              C




           B




           A Parameterübersicht                    C Modellvorschau-Fenster
           B In CAD Designer ohne Funktion
           Abb. A-21    Dialog: Modell-Erfassung


           Parameterübersicht (A)
           Die benötigten Eingaben für das gewählte Modell entnehmen Sie dem Fenster
           oben links in dem Dialog. Ihre Eingaben werden sofort im Modellvorschau-
           Fenster (C) in dem Dialog umgesetzt und das Modell proportional dargestellt.
           Die Modellskizze (D) dient zur Veranschaulichung der Eingabeparameter. Die
           Modellparameter können Sie innerhalb der Restriktionsgrenzen nach Ihren
           Wünschen ändern. Welche Parameter das sind, hängt vom gewählten Modell
           ab. Sollten Sie die Restriktionsgrenzen für das gewählte Modell bei einer Ein-
           gabe verletzen, wird Ihnen dies sofort durch eine Fehlermeldung, welche die
           entsprechenden Restriktionsgrenzen ausgibt, angezeigt.



A-100                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                                    Sprossen




                      Modellvorschau-Fenster (C)
                      In diesem Fenster wird das gewählte Modell (schwarze Linie) und das um-
                      schreibende Rechteck (gestrichelte Linie) maßstäblich angezeigt. Änderun-
                      gen, die Sie für die Modell-Parameter durchführen, werden sofort ins
                      Vorschaufenster übernommen.


                      Eigenschaften der Scheibe definieren
                      Im nächsten Schritt legen Sie die Eigenschaften fest. Die Eigenschaften be-
                      treffen:
                      •   Die Scheibe
                      •   Auftrags-und Kundendaten
                      Der dazugehörige Dialog heißt Eigenschaften Scheibe und öffnet sich auto-
                      matisch nach dem Verlassen des Dialoges Modell-Erfassung.




                      Für die Scheibe legen Sie fest, an welcher X- und Y-Position auf Ihrer Arbeits-
                      fläche sie positioniert werden soll. Das Feld Ausrichtung lässt Sie die Scheibe
                      auch gedreht platzieren.
                      Bei den Auftragsdaten können Sie neben der Auftragsnummer auch die Posi-
                      tionsnummer hinterlegen. Es steht Ihnen ein Feld für den Kundennamen und
                      die Kundennummer zur Verfügung. Sie können auch eingeben, wie viel Stück
                      dieser Konstruktion gefertigt werden sollen. Ist die Konstruktion ein 3fach ISO,
                      können Sie zwei unterschiedliche Scheibenzwischenräume eingeben sowie
                      das entsprechende Gas hinterlegen.
                      Darüber hinaus haben Sie die Möglichkeit für diverse Sachen (z. B. Lieferter-
                      min, Abstandhalter, Gaskürzel, etc.) Texte zu hinterlegen. Im Falle einer AL-
                      CIM-Anbindung, werden diese Felder bei der Übergabe automatisch gefüllt.
                      Welche Felder angezeigt und gefüllt werden können, wird in der INI-Datei kon-
                      figuriert. Die vorhandenen Felder erscheinen auch im Ausdruck.


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Neue Scheibe” auf Seite A-199



A+W CAD Designer (Bars) Überblick                                                              A-101
Sprossen                                                                        Tutorial




           Sprossen platzieren
           Die Vorgehensweise zum Platzieren von Sprossen ist abhängig von der Kom-
           plexität der Konstruktion. Einfache Konstruktionen bestehen aus ein oder
           mehreren senkrechten und/oder waagerechten Sprossen.
           A+W CAD Designer (Bars) verfügt über Möglichkeiten, die Ihnen helfen, sol-
           che Konstruktionen automatisch zu platzieren.
           Der dazugehörige Dialog heißt Muster: Senkrecht/Waagerecht und wird ent-
           weder über das Menü Makro > SW Muster oder über die Symbol-Schaltfläche
           (in den Werkzeugen) geöffnet.




           Im ersten Schritt geben Sie die Anzahl der senkrechten und waagerechten
           Sprossen an. Dann bestimmen Sie die Aufteilung der Sprossen und welche
           Sprosse die durchgängige Sprosse sein soll. Bei der Aufteilung der Sprossen
           unterscheidet A+W CAD Designer (Bars) zwischen:
           •   Gleiche lichte Felder
           •   Gleicher Bohrpunktabstand
           •   Gleicher Bohrpunktabstand (Scheibe)
           •   Gleiche Sprossenlänge
           •   Kundenspezifisch
           Um die Unterschiede der einzelnen Einstellungen zu verdeutlichen, finden Sie
           im Anschluss einige Konstruktionen. Zum besseren Verständnis wurde die
           Vermaßung bei den folgenden Beispielen aktiviert.


           Zu dieser Schulungseinheit gehören:
            Softwarereferenz, “Muster Senkrecht-Waagerecht” auf Seite A-213




A-102                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                               Sprossen




                      Gleiche lichte Felder
                      Diese Einstellung bedeutet, dass A+W CAD Designer (Bars) die waagerech-
                      ten Sprossen so platziert, dass alle waagerechten Felder gleich groß sind.
                      Das gleiche gilt auch für senkrechte Sprossen und deren Felder.




                       A



                       B




                       C




                       D



                      A Rückschnitt                             C Ziffern an Sprosse
                      B Randstopfen                             D Bezugspunkt
                      Abb. A-22     Sprossenkonstruktion, gleiche lichte Felder


                      Erläuterung der horizontalen Vermaßung:
                      •    800 mm: Scheibenbreite
                      •    778 mm: Scheibenbreite abzüglich Rückschnitt (1mal 11 mm rechts, 1mal
                           11 mm links
                      •    523 mm: 2 lichte Felder à 242 mm plus 1 Sprossenbreite 26 mm plus 1/2
                           Sprossenbreite 13 mm
                      •    255 mm: 1 lichtes Feld à 242 mm plus 1/2 Sprossenbreite 13 mm
                      Erläuterung der vertikalen Vermaßung:
                      •    600 mm: Scheibenhöhe
                      •    578 mm: Scheibenhöhe abzüglich Rückschnitt (1mal 11 mm oben, 1mal 11
                           mm unten)
                      •    389,7 mm: 2 lichte Felder à 175,3 mm plus 1 Sprossenbreite 26 mm plus
                           1/2 Sprossenbreite 13 mm
                      •    188,3 mm: 1 lichtes Feld à 175,3 mm plus 1/2 Sprossenbreite 13 mm
                      Wie Sie sehen, sind die beiden senkrechten Sprossen duchgehend und die
                      beiden waagerechten Sprossen wurden geteilt. Aufgrund der Einstellung Glei-
                      che lichte Felder, wurden die Sprossen automatisch so platziert, dass alle
                      waagerechten Felder 242 mm und alle senkrechten Felder 175,3 mm groß
                      sind.



A+W CAD Designer (Bars) Überblick                                                         A-103
Sprossen                                                                        Tutorial




           Gleicher Bohrpunktabstand




           A



           B




           C




           D



           A Rückschnitt                          C Ziffern an Sprosse
           B Randstopfen                          D Bezugspunkt
           Abb. A-23    Sprossenkonstruktion, gleicher Bohrpunktabstand


           Durch die Einstellung Gleicher Bohrpunktabstand ändert sich die Abmessung
           der senkrechten lichten Felder. Das obere und das untere Feld sind gleich,
           das mittlere Feld wird durch diese Einstellung kleiner:
           Erläuterung der horizontalen Vermaßung:
           •   800 mm: Scheibenbreite
           •   778 mm: Scheibenbreite abzüglich Rückschnitt (1mal 11 mm rechts, 1mal
               11 mm links
           •   523 mm: 2 lichte Felder à 242 mm plus 1 Sprossenbreite 26 mm plus 1/2
               Sprossenbreite 13 mm
           •   255 mm: 1 lichtes Feld à 242 mm plus 1/2 Sprossenbreite 13 mm
           Erläuterung der vertikalen Vermaßung:
           •   600 mm: Scheibenhöhe
           •   578 mm: Scheibenhöhe abzüglich Rückschnitt (1mal 11 mm oben, 1mal 11
               mm unten)
           •   385,3 mm: 1 lichtes Felder à 179,7 mm plus 1 lichtes Feld à 166,7 plus 1
               Sprossenbreite 26 mm plus 1/2 Sprossenbreite 13 mm
           •   192,7 mm: 1 lichtes Feld à 179,7 mm plus 1/2 Sprossenbreite 13 mm




A-104                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                                        Sprossen




                      Gleicher Bohrpunktabstand (Bezug auf Scheibe)




                       A




                       B




                       C




                       D



                      A Rückschnitt                            C Ziffern an Sprosse
                      B Randstopfen                            D Bezugspunkt
                      Abb. A-24     Sprossenkonstruktion, gleicher Bohrpunktabstand (Scheibe)


                      Durch die Einstellung Gleicher Bohrpunkt (Scheibe) ändert sich die Abmes-
                      sung der senkrechten lichten Felder. Das obere und das untere Feld sind
                      gleich, das mittlere Feld wird durch diese Einstellung kleiner. Die Scheibe hat
                      eine Höhe von 600 mm. Für zwei horizontalen Sprossen sind zwei Bohrlöcher
                      nötig. Diese sitzen bei 200 mm und bei 400 mm:
                      Erläuterung der horizontalen Vermaßung:
                      •    800 mm: Scheibenbreite
                      •    778 mm: Scheibenbreite abzüglich Rückschnitt (1mal 11 mm rechts, 1mal
                           11 mm links
                      •    523 mm: 2 lichte Felder à 242 mm plus 1 Sprossenbreite 26 mm plus 1/2
                           Sprossenbreite 13 mm
                      •    255 mm: 1 lichtes Feld à 242 mm plus 1/2 Sprossenbreite 13 mm
                      Erläuterung der vertikalen Vermaßung:
                      •    600 mm: Scheibenhöhe
                      •    578 mm: Scheibenhöhe abzüglich Rückschnitt (1mal 11 mm oben, 1mal 11
                           mm unten)
                      •    389 mm: 1 lichtes Felder à 176 mm plus 1 lichtes Feld à 174 plus 1 Spros-
                           senbreite 26 mm plus 1/2 Sprossenbreite 13 mm. Oder: 400 mm minus 11
                           mm Rückschnitt
                      •    189 mm: 1 lichtes Feld à 176 mm plus 1/2 Sprossenbreite 13 mm




A+W CAD Designer (Bars) Überblick                                                                 A-105
Sprossen                                                                        Tutorial




           Gleiche Sprossenlänge




           A




           B




           C




           D



           A Rückschnitt                          C Ziffern an Sprosse
           B Randstopfen                          D Bezugspunkt
           Abb. A-25    Sprossenkonstruktion, gleiche Sprossenlänge


           Durch die Einstellung Gleiche Sprossenlänge ändert sich die Abmessung der
           senkrechten lichten Felder. Die Scheibe hat eine Höhe von 600mm abzüglich
           Rückschnitt von 2mal 11 mm und 2 Randstopfen à 1 mm. Daraus ergibt sich
           eine Sprossenlänge von 576 mm für die durchgehenden senkrechten Spros-
           sen. Das obere und das untere Feld sind gleich, das mittlere Feld wird durch
           diese Einstellung kleiner:
           Erläuterung der horizontalen Vermaßung:
           •   800 mm: Scheibenbreite
           •   778 mm: Scheibenbreite abzüglich Rückschnitt (1mal 11 mm rechts, 1mal
               11 mm links
           •   523 mm: 2 lichte Felder à 242 mm plus 1 Sprossenbreite 26 mm plus 1/2
               Sprossenbreite 13 mm
           •   255 mm: 1 lichtes Feld à 242 mm plus 1/2 Sprossenbreite 13 mm
           Erläuterung der vertikalen Vermaßung:
           •   600 mm: Scheibenhöhe
           •   578 mm: Scheibenhöhe abzüglich Rückschnitt (1mal 11 mm oben, 1mal 11
               mm unten)
           •   387,2 mm: 1 lichtes Felder à 177,8 mm plus 1 lichtes Feld à 170,3 plus 1
               Sprossenbreite 26 mm plus 1/2 Sprossenbreite 13 mm
           •   190,8 mm: 1 lichtes Feld à 177,8 mm plus 1/2 Sprossenbreite 13 mm




A-106                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                               Sprossen




                      Kundendefiniert
                      In dieser Einstellung können Sie die Sprossen über Eingabe von Werten plat-
                      zieren. Geben Sie zunächst die Anzahl der waagerechten und senkrechten
                      Sprossen an. Betätigen Sie die Schaltfläche [OK], es öffnet sich der Dialog
                      Kundenvorgabe SW-Muster.




                      Hier können Sie entweder fixe Werte für die Position der Sprossen angeben
                      oder aber die Abstände zwischen den Sprossen.
                      Beispiel für fixe waagerechte Werte:
                      •   150 mm (vom Scheibenrand)
                      •   300 mm (vom Scheibenrand)
                      und senkrechte Werte:
                      •   200 mm (vom Scheibenrand)
                      •   400 mm (vom Scheibenrand)
                      liefert folgendes Ergebnis:




                      Abb. A-26     Sprosseneingabe fixe Werte




A+W CAD Designer (Bars) Überblick                                                         A-107
Sprossen                                                                     Tutorial




           Erläuterung der waagerechten Vermaßung:
           •   800 mm: Scheibenbreite
           •   778 mm: Scheibenbreite abzüglich Rückschnitt (1mal 11 mm rechts, 1mal
               11 mm links
           •   189 mm (Wert für senkrechte Sprosse bei 200 mm): Vom Scheibenrand
               200 mm abzüglich Rückschnitt (11 mm)
           •   389 mm (Wert für senkrechte Sprosse bei 400 mm): Vom Scheibenrand
               400 mm abzüglich Rückschnitt (11 mm)
           Erläuterung der senkrechten Vermaßung:
           •   600 mm: Scheibenhöhe
           •   578 mm: Scheibenhöhe abzüglich Rückschnitt (1mal 11 mm oben, 1mal 11
               mm unten)
           •   139 mm (Wert für senkrechte Sprosse bei 150 mm): Vom Scheibenrand
               150 mm abzüglich Rückschnitt (11 mm)
           •   289 mm (Wert für senkrechte Sprosse bei 300 mm): Vom Scheibenrand
               300 mm abzüglich Rückschnitt (11 mm)
           Im nächsten Beispiel arbeiten wir mit den selben Werten. Wir lassen A+W
           CAD Designer (Bars) jetzt die Werte aufsummieren, was zu folgendem Ergeb-
           nis kommt:




           Abb. A-27    Werte aufsummieren


           Erläuterung der waagerechten Vermaßung:
           •   800 mm: Scheibenbreite
           •   778 mm: Scheibenbreite abzüglich Rückschnitt (1mal 11 mm rechts, 1mal
               11 mm links
           •   189 mm (Wert für senkrechte Sprosse bei 200 mm): Vom Scheibenrand
               200 mm abzüglich Rückschnitt (11 mm)
           •   589 mm (Wert für senkrechte Sprosse nach weiteren 400 mm): Vom Schei-
               benrand 200 mm für die erste Sprosse und weitere 400 mm für die zweite
               Sprosse abzüglich Rückschnitt (11 mm)
           Erläuterung der senkrechten Vermaßung:


A-108                                            A+W CAD Designer (Bars) Überblick
Tutorial                                                                                   Sprossen




                      •   600 mm: Scheibenhöhe
                      •   578 mm: Scheibenhöhe abzüglich Rückschnitt (1mal 11 mm oben, 1mal 11
                          mm unten)
                      •   139 mm (Wert für senkrechte Sprosse bei 150 mm): Vom Scheibenrand
                          150 mm abzüglich Rückschnitt (11 mm)
                      •   439 mm (Wert für senkrechte Sprosse nach weiteren 300 mm): Vom Schei-
                          benrand 150 mm für die erste Sprosse und weitere 300 mm für die zweite
                          Sprosse abzüglich Rückschnitt (11 mm)


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Kundenvorgabe SW-Muster” auf Seite A-216


                      Sprossen tauschen
                      In A+W CAD Designer (Bars) haben Sie die Möglichkeit, Sprossen in Konst-
                      ruktionen zu tauschen. Bsp.: Sie haben eine Konstruktion mit einer weißen
                      Sprosse erstellt und möchten anstelle der weißen Sprosse eine gelbe Sprosse
                      haben. Es ist dann nicht nötig, die Konstruktion neu zu erstellen. Sie tauschen
                      die entsprechende Sprosse einfach gegen eine andere aus.


                       So tauschen Sie Sprossen aus
                      1 Markieren Sie die Sprosse, die getauscht werden soll.
                      2 Öffnen Sie im Menü Bearbeiten den Menüpunkt Artikel ändern...
                      3 Es öffnet sich der Dialog Stammdaten.
                      4 Wählen Sie die gewünschte Sprosse.
                      5 Betätigen Sie die Schaltfläche [OK]. Die Sprosse wird getauscht.


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Stammdaten” auf Seite A-233




A+W CAD Designer (Bars) Überblick                                                             A-109
Sprossen                                                                         Tutorial




           Demos und Übungen
           In diesem Abschnitt erfahren Sie, wie Sie Sprossenkonstruktionen in A+W
           CAD Designer (Bars) erstellen.

           Trainerdemo: Modelle erläutern
           Es werden unterschiedliche Modelle gezeigt und etwaige Restriktionen erläu-
           tert.
           Folgender Dialog wird unter diesem Aspekt erklärt:
           •   Dialog Modell-Erfassung
           Dieser Dialog öffnet sich, wenn Sie die Symbol-Schaltfläche Neue Scheibe
           betätigen.

           Trainerdemo: Eigenschaften der Scheibe definieren
           Es wird gezeigt, welche Eingaben erforderlich sind, um die Scheibe korrekt zu
           platzieren und welche Möglichkeiten dem Anwender darüber hinaus zur Erfas-
           sung von Texten zur Verfügung stehen.
           Folgender Dialog wird unter diesem Aspekt erklärt:
           •   Dialog Eigenschaften Scheibe
           Dieser Dialog öffnet sich automatisch, wenn Sie den Dialog der Modell-Erfas-
           sung mit [OK] verlassen.

           Trainerdemo: Einfaches Sprossenmuster einfügen
           Es wird gezeigt, welche Eingaben erforderlich sind, um eine Sprossenkonst-
           ruktion bestehend aus zwei waagerechten und zwei senkrechten Sprossen zu
           erstellen.
           Folgender Dialog wird unter diesem Aspekt erklärt:
           •   Dialog Muster Senkrecht Waagerecht

           Übung 1: Eine Konstruktion mit Hilfe eines Sprossenmusters er-
           stellen
           Erstellen Sie eine Sprossenkonstruktion gemäß den unten aufgeführten Spe-
           zifikationen. Die Sprossenkonstruktion ist einfach gehalten und dient als Vor-
           bereitung zum Einstieg in komplexere Konstruktionen.




A-110                                             A+W CAD Designer (Bars) Überblick
Tutorial                                                                                     Sprossen




                      Aufgabenstellung
                      Legen Sie mit der Standard-Sprosse eine Sprossenkonstruktion mit folgenden
                      Spezifikationen an:




                      •   Modell-Nummer:
                          Für die Sprossenkonstruktion dient das Modell Nr. 65 mit einer Höhe von
                          800 mm und einer Breite von 600 mm.
                      •   Eigenschaften der Scheibe:
                          Der Rahmen hat eine Stärke von 11 mm. Bei dem Kunden handelt es sich
                          um die Firma Albrecht GmbH. Die Kundennummer ist 811. Die Firma Alb-
                          recht GmbH hat mit Auftrag Nummer 2123 5 Stück dieser Konstruktion für
                          die Baustelle Europaplatz bestellt. Es handelt es sich um ein Isolierglas mit
                          einem Abstandhalter von 16 mm.
                      •   Muster Senkrecht-Waagerecht
                          Die Sprossenkonstruktion besteht aus zwei waagerechten und einer senk-
                          rechten Sprosse. Die senkrechte Sprosse ist durchgängig. Die Sprossen
                          sollen so platziert werden, dass gleiche lichte Felder entstehen.

                      Übung 1: Lösung
                      Die einzelnen Schritte dieser Aufgabe werden in drei Dialogen vorgenommen:
                      •   Dialog Modell-Erfassung
                      •   Dialog Eigenschaften der Scheibe (öffnet sich automatisch)
                      •   Dialog Muster Senkrecht-Waagerecht




A+W CAD Designer (Bars) Überblick                                                               A-111
Sprossen                                                                         Tutorial




            Sprossenkonstruktion erstellen




           1 Öffnen Sie den Dialog Modell-Erfassung.
           2 Wählen Sie die Modell-Nummer 065 aus der Kombobox aus.
           3 Geben Sie im Feld Breite 600 ein.
           4 Geben Sie im Feld Höhe 800 ein.
           5 Betätigen Sie die Schaltfläche [OK.]. Es öffnet sich der Dialog Eigenschaf-
             ten Scheibe.
           6 Geben Sie im Feld X-Position 0 ein.
           7 Geben Sie im Feld Y-Position 0 ein.
           8 Geben Sie im Feld Ausrichtung 0 ein.
           9 Geben Sie im Feld Rückschnitt 11 mm ein.
           10 Geben Sie im Feld Auftragsnummer 2123 ein.
           11 Geben Sie im Feld Positionsnummer 1 ein.
           12 Geben Sie im Feld Kundenname Albrecht GmbH ein.
           13 Geben Sie im Feld Kundennummer 811 ein.
           14 Geben Sie im Feld Auftragsmenge 5 ein.
           15 Geben Sie im Feld SZR1 16 mm ein.
           16 Markieren Sie im Bereich Extra den Eintrag Kommisionstext und geben Sie
              Baustelle Europaplatz ein.
           17 Betätigen Sie die Schaltfläche [OK]. Das Modell wird auf der Arbeitsfläche
              platziert.




           18 Betätigen Sie die Symbol-Schaltfläche [Neues senkrecht/waagerecht Mus-
              ter]. Platzieren Sie den Mauszeiger auf dem Modell und betätigen Sie die
              linke Maustaste. Es öffnet sich der Dialog Muster Senkrecht-Waagerecht.
           19 Geben Sie im Feld Anzahl Waagerecht 2 ein.
           20 Geben Sie im Feld Anzahl Senkrecht 1 ein.
           21 Aktivieren Sie im Bereich Teilung Waagerecht die Radiotaste Gleiche lich-
              te Felder.
           22 Aktivieren Sie im Bereich Durchgängige Sprossen die Checkbox Senk-
              rechte.
           23 Aktivieren Sie im Bereich Teilung Senkrecht die Radiotaste Gleiche lichte
              Felder.


A-112                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                                Sprossen




                      24 Betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen. Die
                         Sprossenkonstruktion sieht wie folgt aus:




                      Abb. A-28     Ergebnis Übung 1, einfache Sprossenkonstruktion




A+W CAD Designer (Bars) Überblick                                                          A-113
Sprossen                                                                     Tutorial




           Übung 2: Eine freie Sprossenkonstruktion erstellen
           Erstellen Sie eine Sprossenkonstruktion mit den Vorgaben, die Sie unter
           Übung 1 finden. Verwenden Sie aber nicht Muster Senkrecht/Waagerecht,
           sondern erstellen Sie die Konstruktion frei.




           Übung 2: Lösung
           Die einzelnen Schritte dieser Aufgabe werden in zwei Dialogen vorgenom-
           men:
           •   Dialog Modell-Erfassung
           •   Dialog Eigenschaften der Scheibe (öffnet sich automatisch)


            Freie Sprossenkonstruktion erstellen
           Schritt 1 bis 17 entnehmen Sie bitte der Übung 1.
           1 Entfernen Sie die automatischen Fangpunkte, indem Sie auf der Scheibe
             die rechte Maustaste betätigen.




           2 Öffnen Sie im Bereich der Fangpunkte das Werkzeug Anzahl?. Geben Sie
             eine 2 ein.




           3 Betätigen Sie im Bereich der Fangpunkte das Werkzeug Anzahl auf Objekt
             erzeugen.
           4 Klicken Sie die untere Innenkante des Rahmens an. A+W CAD Designer
             (Bars) setzt drei Fangpunkte.




A-114                                             A+W CAD Designer (Bars) Überblick
Tutorial                                                                                Sprossen




                      5 Klicken Sie die Rahmeninnenkante des Bogens an. A+W CAD Designer
                        (Bars) setzt drei Fangpunkte entlang des Bogens und einen auf der Schei-
                        be.




                      6 Aktivieren Sie das Werkzeug Sprosse (senkrecht).
                      7 Bewegen Sie den Mauszeiger zum mittleren Fangpunkt des Bogens. Der
                        Mauszeiger ändert sein Aussehen zu einem Fadenkreuz. Betätigen Sie die
                        linke Maustaste.
                      8 Bewegen Sie den Mauszeiger zum mittleren Fangpunkt der unteren Innen-
                        kante und betätigen Sie die linke Maustaste. Die Sprosse wird eingefügt.




                      9 Im Bereich der Fangpunkte betätigen Sie das Werkzeug Alle löschen. Es
                        werden alle Fangpunkte gelöscht.
                      10 Öffnen Sie anschließend das Werkzeug Anzahl?. Geben Sie eine 3 ein.
                      11 Betätigen Sie im Bereich der Fangpunkte das Werkzeug Anzahl auf Objekt
                         erzeugen.
                      12 Klicken Sie die Sprosse an, die Sie eingefügt haben. Es erscheinen vier
                         Fangpunkte (drei lichte Felder).




                      13 Aktivieren Sie das Werkzeug Sprosse (waagerecht).




A+W CAD Designer (Bars) Überblick                                                          A-115
Sprossen                                                                          Tutorial




           14 Klicken Sie auf den zweiten Fangpunkt von unten und anschließend auf die
              rechte Rahmeninnenkante. Die Sprosse wird eingefügt:




           Abb. A-29   Ergebnis Übung 2, Sprossenkonstruktion manuell erstellen


           15 Wiederholen Sie diesen Schritt für die fehlenden drei Sprossen.




A-116                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                                      Sprossen




                      Übung 3: Nachbildung einer Sprossenkonstruktion
                      Bilden Sie die folgende Sprossenkonstruktion nach:




                      Abb. A-30     Foto zu Übung 3, Sprossenkonstruktion manuell erstellen


                      Aufgabenstellung
                      Legen Sie mit einer Sprosse von 12 mm Breite eine Sprossenkonstruktion mit
                      folgenden Spezifikationen an:
                      •   Breite: 500 mm
                      •   Höhe: 600 mm
                      •   Drei waagerechte Sprossen
                      •   Zwei senkrechte Sprossen
                      •   Sonne mit drei Strahlen
                      •   Die Eigenschaften der Scheibe können von Übung Nr. 1 übernommen wer-
                          den.

                      Übung 3: Lösung
                      Die einzelnen Schritte dieser Aufgabe werden in drei Dialogen vorgenommen:
                      •   Dialog Modell-Erfassung
                      •   Dialog Eigenschaften der Scheibe (öffnet sich automatisch)
                      •   Dialog Muster Senkrecht-Waagerecht




A+W CAD Designer (Bars) Überblick                                                               A-117
Sprossen                                                                         Tutorial




            Sprossenkonstruktion erstellen
           1 Öffnen Sie den Dialog Modell-Erfassung.
           2 Wählen Sie die Modell-Nummer 065 aus der Kombobox aus.
           3 Geben Sie im Feld Breite 500 ein.
           4 Geben Sie im Feld Höhe 600 ein.
           5 Betätigen Sie die Schaltfläche [OK.]. Es öffnet sich der Dialog Eigenschaf-
             ten Scheibe.
           6 Geben Sie im Feld X-Position 0 ein.
           7 Geben Sie im Feld Y-Position 0 ein.
           8 Geben Sie im Feld Ausrichtung 0 ein.
           9 Geben Sie im Feld Rückschnitt 11 mm ein.
           10 Geben Sie im Feld Auftragsnummer 2123 ein.
           11 Geben Sie im Feld Positionsnummer 1 ein.
           12 Geben Sie im Feld Kundenname Albrecht GmbH ein.
           13 Geben Sie im Feld Kundennummer 811 ein.
           14 Geben Sie im Feld Auftragsmenge 5 ein.
           15 Geben Sie im Feld SZR1 16 mm ein.
           16 Markieren Sie im Bereich Extra den Eintrag Kommisionstext und geben Sie
              Baustelle Europaplatz ein.
           17 Betätigen Sie die Schaltfläche [OK]. Das Modell wird auf der Arbeitsfläche
              platziert.
           18 Betätigen Sie die Symbol-Schaltfläche [Neues senkrecht/waagerecht Mus-
              ter]. Platzieren Sie den Mauszeiger auf dem Modell und betätigen Sie die
              linke Maustaste. Es öffnet sich der Dialog Muster Senkrecht-Waagerecht.
           19 Geben Sie im Feld Anzahl Waagerecht 3 ein.
           20 Geben Sie im Feld Anzahl Senkrecht 2 ein.
           21 Aktivieren Sie im Bereich Teilung Waagerecht die Radiotaste Kundendefi-
              niert.
           22 Aktivieren Sie im Bereich Durchgängige Sprossen die Checkbox Waage-
              rechte.
           23 Aktivieren Sie im Bereich Teilung Senkrecht die Radiotaste Gleiche lichte
              Felder.
           24 Betätigen Sie die Schaltfläche [OK].
           25 Es öffnet sich der Dialog Kundenvorgabe SW-Muster. Aktivieren Sie im Be-
              reich Waagerechte Sprossen die Checkbox Aufsummieren.
           26 Betätigen Sie die Schaltfläche [Hinzufügen]. Es öffnet sich der Dialog Ein-
              gabe Sprossen-Abstände. Geben Sie 120 ein. Betätigen Sie die Schaltflä-
              che [OK].




A-118                                                A+W CAD Designer (Bars) Überblick
Tutorial                                                                                 Sprossen




                      27 Wiederholen Sie diesen Schritt, bis alle drei waagerechten Sprossen vor-
                         handen sind.
                      28 Betätigen Sie die Schaltfläche [OK] um den Dialog zu schließen. Die Kons-
                         truktion sieht wie folgt aus:




                         Abb. A-31    Übung 3, Zwischenstandbm bei A+W


                      29 Setzen Sie auf die oberen Teile der senkrechten Sprossen jeweils drei
                         Fangpunkte.
                      30 Verbinden Sie die mittleren Fangpunkte mit einer waagerechten Sprossen.
                      31 Löschen Sie die Fangpunkte.




                      32 Aktivieren Sie das Werkzeug Schneiden auf.
                      33 Markieren Sie auf der linken Seite die Sprosse, die geschnitten (gekürzt)
                         werden soll. In unserem Beispiel ist das die senkrechte Sprosse.
                      34 Anschließend markieren Sie die Sprosse, auf die die geschnittene Sprosse
                         verlängert werden soll. In unserem Beispiel ist das die waagerechte Spros-
                         se. Das obere Stück der senkrechten Sprosse wird automatisch gelöscht.




A+W CAD Designer (Bars) Überblick                                                           A-119
Sprossen                                                                         Tutorial




           35 Wiederholen Sie diese Schritte für die rechte Seite.




           36 Aktivieren Sie das Werkzeug Sonne.
           37 Klicken Sie in das Feld, in dem die Sonne eingefügt werden soll. Es öffnet
              sich der Dialog Sonne und Sterne.
           38 Aktivieren Sie die Radiotaste Stern sowie die Checkbox Gemeinsamer Zu-
              schnitt.
           39 Unser Strahlenmuster hat gleiche Winkel und drei Strahlen.
           40 Betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen und das
              Strahlenmuster eingefügt.




              Abb. A-32    Ergebnis Übung 3


           Zu dieser Schulungseinheit gehören:
            Softwarereferenz, “Neue Scheibe” auf Seite A-199
            Softwarereferenz, “Muster Senkrecht-Waagerecht” auf Seite A-213
            Softwarereferenz, “Kundenvorgabe SW-Muster” auf Seite A-216




A-120                                              A+W CAD Designer (Bars) Überblick
Tutorial                                                                                      Sprossen




                      Zuschnitt und Messen
                      Lernziele

                      • Informationen zum Zuschnitt kennenlernen und verstehen
                      • Strecken vermessen


                      Nutzen

                      Mit dem Dialog können Sie sich die Informationen zum Zuschnitt am Bildschirm
                      anzeigen lassen. Um sich einen Überblick zu verschaffen, brauchen Sie nichts
                      ausdrucken.


                      Definitionen

                      A:                         Kennzeichnet den Anfang der Sprosse.

                      E:                         Kennzeichnet das Ende der Sprosse.

                      F:                         Kennzeichnet die Fräspunkte einer Sprosse.

                      P:                         Punkt, an dem das Sprossenende seine größte
                                                 Ausdehnung hat.


                      Merke

                      Messpunkte                 Um Messpunkte genau zu treffen, kann es sinnvoll
                                                 sein, Fangpunkte zu setzen.

                      Positive Winkelangaben     Zuschnitt gegen den Uhrzeigersinn.

                      Negative Winkelangaben     Zuschnitt im Uhrzeigersinn.




A+W CAD Designer (Bars) Überblick                                                               A-121
Sprossen                                                                        Tutorial




           Zuschnittinformationen anzeigen
           A+W CAD Designer (Bars) liefert Ihnen auf Knopfdruck alle für den Zuschnitt
           wichtigen Informationen. Den entsprechenden Dialog erreichen Sie über
           Info > Zuschnitt-Info ...
           Der Dialog zeigt Ihnen die Zuschnitt-Informationen zu der aktuellen Sprossen-
           konstruktion. Zum besseren Verständnis zeigen wir im Anschluss die dazuge-
           hörige Sprossenkonstruktion:




           Abb. A-33     Sprossenkonstruktion: Zuschnitt-Informationen


           Der obere Bereich des Dialoges zeigt Ihnen Informationen zur Scheibe und zu
           den Stammdaten, z. B. Sprossenbezeichnung (Kieler) und Farbe (Gold).
           Im Feld Materialmenge sehen Sie die für die Sprossenkonstruktion benötigte
           Menge an Material in der jeweils eingestellten Maßeinheit.
           Die im oberen Beispiel angezeigte Materialmenge von 2.614 setzt sich wie
           folgt zusammen:
           •   Sprosse A kommt zweimal vor: 279,9+279,5 = 550
           •   Sprosse B kommt einmal vor: 286
           •   Sprosse C kommt einmal vor: 386
           •   Sprosse D kommt einmal vor: 386
           •   Sprosse E kommt einmal vor: 996,8
           Werden die Werte addiert, ist das Ergebnis: 2.613,8 - gerundet auf 2.614.




A-122                                                A+W CAD Designer (Bars) Überblick
Tutorial                                                                                     Sprossen




                      In der ersten Tabellenspalte steht die Ziffer der Sprosse innerhalb der Scheibe
                      (A, B, C, ...). Wie oft diese Sprosse in der Scheibe vorkommt, ist in der zweiten
                      Spalte angegeben. 1 bedeutet, die Sprosse ist einmal vorhanden, 2 bedeutet,
                      die Sprosse ist zweimal vorhanden, usw.
                      Die dritte Spalte gibt die Länge der Sprosse an. Werden die Längen addiert,
                      erhält man die Materialmenge.

                      Zuschnitt am Anfang und am Ende der Sprosse




                      Wie die Sprosse am Anfang und am Ende zugeschnitten wird, sehen Sie an
                      den Maßangaben hinter A: (Anfang) und E: (Ende):
                      Beispiel für A (Anfang): 45° 0° -45° / E (Ende): -- 0° --

                                  B


                       A                    C




                       D                     F

                                  E
                      A A: 45°                                 D E: --
                      B A: 0°                                  E E: 0°
                      C A: -45°                                F E: --




A+W CAD Designer (Bars) Überblick                                                               A-123
Sprossen                                                                             Tutorial




           In der Reihe befindet sich eine Zahl (z. B. -- 0° --)
           Ist nur eine Zahl angegeben (im Beispiel Sprosse A (E), Sprosse B (A), Spros-
           se C (E) und Sprosse D (E)), so wird diese Sprosse am entsprechenden Ende
           glatt unter dem angegebenen Winkel geschnitten. Dies trifft zum Beispiel für
           Sprossen zu, die einfach auf den Rahmen stoßen.

           In der Reihe befinden sich zwei Zahlen (z. B. 45° 0° -45°)
           Sind zwei Zahlen angegeben (im Beispiel Sprosse A (A), Sprosse B (E),
           Sprosse C (A) und Sprosse D (A)), werden die Sprossen unter den beiden ge-
           gebenen Winkeln von der Mitte der entsprechenden Seite geschnitten. Im Fall
           der Sprosse B (E) also links von der Mitte unter dem Winkel von 45° und
           rechts davon unter dem Winkel von -45° (negativer Winkel, da im Uhrzeiger-
           sinn).

           In der Reihe befinden sich drei Zahlen (z. B. 56 22 -68)
           Sind drei Werte angegeben, handelt es sich um Winke (im Beispiel E (A)+(E)).
           Dann trifft die Sprosse mit der entsprechenden Seite unter dem mittleren Win-
           kel (hier 22°) auf eine andere Sprosse auf. Die beiden äußeren Winkel werden
           nur benötigt, falls die Säge die Fräsung nicht automatisch mitschneidet.

           In der Reihe befinden sich Zahlen in Klammern (z. B. 68(15,4) -
           22(4.1) -56(6,5))
           Werden Zahlen in Klammern angegeben, treffen mehrere Sprossen in einem
           Punkt zusammen und müssen darüber hinaus noch auf ein weiteres Objekt
           (Sprosse oder Rahmen) zugeschnitten werden. Die Zahlen in Klammern ge-
           ben die Breite des Zuschnitts an. Am Beispiel für die Sprosse E: E (68(15,4) -
           22(4.1) -56(6,5)) soll die Bearbeitungsweise verdeutlicht werden:




                                                                 6,5             4
                                                                             15,
                                                                       4,1

                                          B
                                          A
                                      C
                                  D



           A P (15,4 mm)                          D Letzter Zuschnitt: Winkel -56°, Breite
           B Zuschnitt links von P unter 68°        6,5 mm.
           C Sprossenende: Winkel -22° Breite 4,1
             mm




A-124                                               A+W CAD Designer (Bars) Überblick
Tutorial                                                                                    Sprossen




                      •   Erster Schritt
                          Im ersten Schritt sucht man nach dem Punkt P. Dies ist der Punkt, an dem
                          das Sprossenende seine größte Ausdehnung hat. Zum besseren Ver-
                          ständnis zeigt die grüne Linie die ungeschnittene Sprosse. Im Beispiel
                          oben ist der Punkt P bei 15,4 (68), d. h. der Punkt liegt 15,4 mm vom linken
                          Rand entfernt zwischen Zuschnitt 1 und Zuschnitt 2.
                      •   Zweiter Schritt
                          Vom gefunden Punkt P können nun nach beiden Seiten die einzelnen Zu-
                          schnitte ausgeführt werden. Im Beispiel oben gibt es nur einen Zuschnitt
                          links des Punktes unter 68°. Rechts des Punktes gibt es noch zwei Zu-
                          schnitte. Zunächst wird das Sprossenende unter einem Winkel von -22°
                          (im Uhrzeigersinn, daher negativ) zugeschnitten. Die Breite dieses Zu-
                          schnittes (NICHT die Zuschnittkante) muss 4.1 mm betragen. Dadurch er-
                          gibt sich der nächste Punkt von dem aus der letzte Zuschnitt unter einem
                          Winkel von -56° erfolgt. Zur Kontrolle verbleibt noch die Breite der letzten
                          Scheidzone von 6.5mm.

                      Fräspunkte
                      Im Beispiel oben werden die Sprossen C und D gefräst. Dies ist an der Zeile
                      mit dem F: ersichtlich. Hinter diesem Kennbuchstaben folgen die relativen
                      Fräsmaße vom Anfang bis zum Ende der Sprosse. Sprosse C wird also bei
                      259,3 (R) mm gefräst. Der Buchstabe in den Klammern kennzeichnet die
                      Richtung. R steht für rechts und L für links. Sprosse D wird ebenfalls bei 259,3
                      mm jedoch links gefräst.




                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Zuschnitt-Informationen” auf Seite A-230




A+W CAD Designer (Bars) Überblick                                                              A-125
Sprossen                                                                         Tutorial




           Abstände oder Längen messen




           Das Vermessen von Abständen und Längen geht in A+W CAD Designer
           (Bars) über zwei Mausklicks. Nachdem Sie das Werkzeug ausgewählt haben,
           klicken Sie den Startpunkt der Messstrecke an und anschließend den End-
           punkt.




           Der Dialog Abstand erscheint automatisch und zeigt Ihnen folgende Informa-
           tionen:
           •   Absolut
           •   x
           •   y
           Der Wert Absolut: 348,4 mm ist die Länge der Messstrecke. Der Wert x: 194,5
           mm bedeutet, der Startpunkt der Messstrecke liegt auf der x-Achse bei 194,5
           mm. Der Wert y: 289 mm bedeutet, der Endpunkt der Messstrecke liegt auf
           der y-Achse bei 289 mm.
           Das entsprechende Werkzeug aktivieren Sie entweder über das Menü
           Info > Messen
           oder über die Symbol-Schaltfläche.

               Genaues Messen
               Um möglichst genau die gewünschten Punkte zu treffen, ist es sinnvoll, zu-
               vor Fangpunkte auf die Arbeitsfläche zu setzen. Sie können diese Fang-
               punkte auch einsetzen, um rasch die Information über Längen einzelner
               Sprossen zu erhalten.


           Zu dieser Schulungseinheit gehören:
            Softwarereferenz, “Abstand” auf Seite A-229




A-126                                               A+W CAD Designer (Bars) Überblick
Tutorial                                                                                 Spezialmuster




                      Spezialmuster
                      In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit Sondermustern, Fassaden
                      und Makros umgehen bzw. diese erstellen.


                      Sondermuster
                      Lernziele

                      • Sondermuster kennenlernen und verstehen
                      • Sinn und Zweck von Sondermustern verstehen
                      • Eigene Sondermuster erstellen


                      Nutzen

                      Das Platzieren von Rauten und Rechtecken geht mit Hilfe dieses Dialoges schneller
                      als die Muster manuell zu erstellen.


                      Merke

                      Dialog Rauten- bzw.        ändert, in Abhängigkeit von der Auswahl (Rauten oder
                      Rechteckmuster             Rechteck) seinen Namen.

                      Rauten und Rechtecke       können symmetrisch oder sprossensymmetrisch
                                                 platziert werden.




A+W CAD Designer (Bars) Überblick                                                                A-127
Spezialmuster                                                                       Tutorial




                Sondermuster erstellen
                Mit A+W CAD Designer (Bars) können Sie ein Sondermuster automatisch
                platzieren. Anhand der Scheibenabmessungen errechnet A+W CAD Designer
                (Bars) wie viele Elemente auf die Scheibe passen.Das Sondermuster gibt es
                in zwei verschiedenen Ausführungen:
                •   In Form von Rauten
                •   In Form von Rechtecken


                 So legen Sie ein Sondermuster an
                1 Platzieren Sie eine Scheibe auf der Arbeitsfläche.
                2 Wählen Sie im Menü Makro > Spezial Muster > Sondermsuter.
                3 Klicken Sie die Scheibe an. Der Dialog Rauten- bzw. Rechteckmuster...
                  wird geöffnet.




                4 Soll das Muster aus Rauten bestehen, aktivieren Sie die Checkbox Rau-
                  ten.
                5 Soll das Muster aus Rechtecken bestehen, aktivieren Sie die Checkbox
                  Rechteck.
                6 Im Feld Breite geben Sie die Breite der Rauten/des Rechtecks ein.
                7 Im Feld Höhe geben Sie die Höhe der Rauten/des Rechtecks ein.
                8 Die Checkbox Übertrag auf alle Scheiben ist nur aktiv, wenn sich mehr als
                  eine Scheibe auf der Arbeitsfläche befindet. Dann haben Sie die Möglich-
                  keit, durch Aktivierung dieser Checkbox das Muster auf allen Scheiben zu
                  platzieren.
                9 Über die Radiotasten im unteren Bereich des Dialogs steuern Sie die Auf-
                  teilung. Sie können wählen zwischen:
                    •   Rauten- bzw. Rechtecksymmetrisch.
                    •   Sprossensymmetrisch.



A-128                                                 A+W CAD Designer (Bars) Überblick
Tutorial                                                                            Spezialmuster




                         Die folgenden Grafiken zeigen den Unterschied:




                         A Rautensymmetrisch                      B Sprossensymmetrisch
                         Abb. A-34     Symmetriebeispiele für Rauten




                         A Rechteckymmetrisch                     B Sprossensymmetrisch
                         Abb. A-35     Symmetriebeispiele für Rechtecke


                      Sprossensymmetrisch Ist diese Radiotaste aktiv, erfolgt die Aufteilung der
                      Rauten bzw. Rechtecke sprossensymmetrisch.


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Rautenmuster...” auf Seite A-220




A+W CAD Designer (Bars) Überblick                                                         A-129
Spezialmuster                                                                                    Tutorial




                Fassaden
                Lernziele

                • Fassaden kennenlernen und verstehen
                • Sinn und Zweck von Fassaden verstehen
                • Eigene Fassade erstellen


                Nutzen

                Das Platzieren von zwei bis vier Scheiben (Modell Nr. 0) geht mit Hilfe dieses
                Werkzeuges schneller als die Scheiben einzeln zu platzieren.


                Definitionen

                Fassadenanlage              hat ein bis vier Scheiben von Modell-Nr. 0.


                Merke

                Anzahl Scheiben             Sie müssen nicht zwingend vier Scheiben platzieren.
                                            Sie können auch nur zwei oder drei Scheiben
                                            platzieren.




A-130                                                       A+W CAD Designer (Bars) Überblick
Tutorial                                                                              Spezialmuster




                      Fassadenanlage
                      In der Architektur bezieht sich der Begriff Fassade auf die Hauptansichtsseite
                      oder Schauseite eines Gebäudes. Mit A+W CAD Designer (Bars) können Sie
                      bis zu vier Scheiben auf der Arbeitsfläche positionieren und so Ihrem Kunden
                      einen Eindruck bieten, wie seine Fassade mit den Scheiben aussieht bzw.
                      aussehen kann. Die einzelnen Scheiben können angefasst und verschoben
                      werden. Ihr Kunde bekommt so ein Gefühl für die Proportionen und die Auftei-
                      lung.
                      Die Vorgehensweise zum Erstellen einer Fassade ist wie folgt:
                      •   Abmessungen der einzelnen Scheiben angeben
                      •   Eigenschaften der Scheibe definieren

                      Abmessungen der einzelnen Scheiben angeben
                      Im Menü Makro befindet sich im Menüpunkt Spezial-Muster der Eintrag Fas-
                      sadenanlage. Damit öffnet sich der Dialog Fassadenanlage... .




                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Fassadenanlage...” auf Seite A-222




A+W CAD Designer (Bars) Überblick                                                            A-131
Spezialmuster                                                                         Tutorial




                Demos und Übungen
                In diesem Abschnitt erfahren Sie, wie Sie in A+W CAD Designer (Bars) mit
                Fassaden arbeiten.

                Trainerdemo: Fassadenanlagen erläutern
                Es wird die Vorgehensweise zum Erstellen einer Fassadenanlage gezeigt.
                Folgender Dialog wird unter diesem Aspekt erklärt:
                •   Dialog Fassadenanlage...
                Dieser Dialog öffnet sich über Makro > Spezial-Makro > Fassadenanlage.

                Übung 1: Erstellen einer Fassadenanlage
                Erstellen Sie eine Fassadenanlage gemäß den unten aufgeführten Spezifika-
                tionen.

                Aufgabenstellung
                Legen Sie folgende Fassade an:




                Abb. A-36    Ergebnis Übung 1


                •   Zwei Scheiben mit einer Höhe von 800 mm und einer Breite von 600 mm.
                •   Eine Scheibe mit einer Höhe von 400 mm und einer Breite von 300 mm.
                •   Eine Scheibe mit einer Höhe von 200 mm und einer Breite von 100 mm.
                •   Die durch A+W CAD Designer (Bars) ermittelten Abstände werden über-
                    nommen.
                •   Eigenschaften der Scheibe:
                    Der Rahmen hat eine Stärke von 11 mm. Bei dem Kunden handelt es sich
                    um die Firma Augustin. Die Kundennummer ist 311. Die Firma Augustin hat
                    mit Auftrag Nummer 5 1Stück dieser Konstruktion bestellt. Es handelt sich
                    um ein Isolierglas mit einem Abstandhalter von 10 mm.




A-132                                                   A+W CAD Designer (Bars) Überblick
Tutorial                                                                               Spezialmuster




                      Übung 1: Lösung
                      Die einzelnen Schritte dieser Aufgabe werden in zwei Dialogen vorgenom-
                      men:
                      •   Dialog Fassadenanlage
                      •   Dialog Eigenschaften der Scheibe (öffnet sich automatisch)


                       Fassade erstellen
                      1 Öffnen Sie den Dialog Fassadenanlage.
                      2 Wählen Sie die Modell-Nummer 000 aus der Kombobox aus.
                      3 Geben Sie für Scheibe A im Feld Breite 800 und im Feld Höhe 600 ein.
                      4 Geben Sie für Scheibe D im Feld Breite 800 und im Feld Höhe 600 ein
                      5 Geben Sie für Scheibe B im Feld Breite 400 und im Feld Höhe 300 ein.
                      6 Geben Sie für Scheibe C im Feld Breite 200 und im Feld Höhe 100 ein.
                      7 Betätigen Sie die Schaltfläche [OK]. Es öffnet sich der Dialog Eigenschaf-
                        ten Scheibe.
                      8 Geben Sie im Feld X-Position 0 ein.
                      9 Geben Sie im Feld Y-Position 0 ein.
                      10 Geben Sie im Feld Ausrichtung 0 ein.
                      11 Geben Sie im Feld Rückschnitt 11 mm ein.
                      12 Geben Sie im Feld Auftragsnummer 5 ein.
                      13 Geben Sie im Feld Positionsnummer 1 ein.
                      14 Geben Sie im Feld Kundenname Augustin in.
                      15 Geben Sie im Feld Kundennummer 311 ein.
                      16 Geben Sie im Feld Auftragsmenge 1 ein.
                      17 Geben Sie im Feld SZR1 10 mm ein.
                      18 Markieren Sie im Bereich Extra den Eintrag Kommisionstext und geben Sie
                         Nordring ein.
                      19 Betätigen Sie die Schaltfläche [OK]. Die Fassade sieht wie folgt aus:




                      Abb. A-37     Ergebnis Übung 1




A+W CAD Designer (Bars) Überblick                                                            A-133
Spezialmuster                                                                          Tutorial




                Übung 2: Nachbildung einer Fassadenanlage
                Bilden Sie die folgende Fassadenanlage nach:




                                                 B
                A




                                                D
                C




                Abb. A-38    Foto Übung 2, Nachbildung dieser Fassadenanlage


                Aufgabenstellung
                Legen Sie mit Sprossen von 12 mm Breite eine Fassadenanlage mit folgen-
                den Spezifikationen an:
                •   Scheibe A: Breite von 400 mm und eine Höhe von 550 mm
                •   Scheibe B: Breite von 400 mm und eine Höhe von 550 mm
                •   Scheibe C: Breite von 150 mm und eine Höhe von 320 mm
                •   Scheibe D: Breite von 800 mm und eine Höhe von 200 mm
                •   Scheibe A und Scheibe B haben in der Mitte eine senkrechte Sprosse
                •   Scheibe D hat zwei senkrechte Sprossen
                •   Eigenschaften der Scheibe:
                    Der Rahmen hat eine Stärke von 11 mm. Bei dem Kunden handelt es sich
                    um die Firma Müller GmbH. Die Kundennummer ist 11. Die Firma Müller
                    GmbH hat mit Auftrag Nummer 21 1 Stück dieser Konstruktion für die Bau-
                    stelle Nordring bestellt. Es handelt es sich um Isoliergläser mit einem Ab-
                    standhalter von 16 mm.

                Übung 2: Lösung
                Die einzelnen Scheiben werden in einem Dialog erfasst:
                •   Dialog Fassadenanlage...


                 Scheiben platzieren
                1 Öffnen Sie den Dialog Fassadenanlage... .
                2 Geben Sie für Scheibe A im Feld Breite 400 und im Feld Höhe 550 ein.
                3 Geben Sie für Scheibe B im Feld Breite 400 und im Feld Höhe 550 ein.
                4 Geben Sie für Scheibe C im Feld Breite 150 und im Feld Höhe 320 ein.
                  Nachdem Sie den Wert für die Breite eingegeben haben, errechnet A+W


A-134                                                   A+W CAD Designer (Bars) Überblick
Tutorial                                                                             Spezialmuster




                         CAD Designer (Bars) automatisch den Wert für Abstand a. In diesem Fall
                         125 mm. Wenn Sie zur Scheibe D wechseln, wird der Wert für Abstand b
                         ebenfalls automatisch gefüllt. Die Abstände sind in diesem Fall irrelevant,
                         da wir die Scheiben erst auf der Arbeitsfläche richtig positionieren.
                      5 Geben Sie für Scheibe D im Feld Breite 800 und im Feld Höhe 200 ein
                      6 Betätigen Sie die Schaltfläche [OK]. Es öffnet sich der Dialog Eigenschaf-
                        ten Scheibe.
                      7 Die Felder X-Position, Y-Position sowie Ausrichtung werden nicht gefüllt,
                        da die Positionierung manuell erfolgt.
                      8 Geben Sie im Feld Auftragsnummer 21 ein.
                      9 Geben Sie im Feld Positionsnummer 1 ein.
                      10 Geben Sie im Feld Kundenname Müller GmbH ein.
                      11 Geben Sie im Feld Kundennummer 11 ein.
                      12 Geben Sie im Feld Auftragsmenge 1 ein.
                      13 Geben Sie im Feld SZR1 16 mm ein.
                      14 Markieren Sie im Bereich Extra den Eintrag Kommisionstext und geben Sie
                         Nordring ein.
                      15 Betätigen Sie die Schaltfläche [OK]. Das Modell wird auf der Arbeitsfläche
                         platziert.




                         Abb. A-39    Zwischenergebnis Übung 2


                      16 Aktivieren Sie das Werkzeug Element auswählen.
                      17 Verschieben Sie die Scheiben an ihre jeweilige Postion.

                         Scheiben ausrichten
                         Bei der Fassade geht es darum, dem Kunden einen Eindruck davon zu ver-
                         mitteln, wie die fertige Fassade aussehen kann. Es geht nicht darum, die
                         Fassade maßstabgetreu nachzubilden.



A+W CAD Designer (Bars) Überblick                                                            A-135
Spezialmuster                                                                      Tutorial




                   Abb. A-40    Zwischenergebnis Übung 2


                18 Fügen Sie die Sprossen ein.




                   Abb. A-41    Ergebnis Übung 2


                Zu dieser Schulungseinheit gehören:
                 Softwarereferenz, “Fassadenanlage...” auf Seite A-222




A-136                                                    A+W CAD Designer (Bars) Überblick
Tutorial                                                                                 Spezialmuster




                      Makros
                      Lernziele

                      • Sinn und Zweck von Makros verstehen
                      • Vorhandene Makros kennenlernen und verstehen
                      • Eigene Makros erstellen und speichern


                      Nutzen

                      Bei häufig vorkommenden Konstruktionen ist der Einsatz von Makros zeitsparend.


                      Definitionen

                      Makro                      Ein Makro ist ein Programm, das eine fest
                                                 vorgegebene Folge von Befehlen oder Aktionen
                                                 enthält. Alle Anweisungen des Makros werden
                                                 automatisch ausgeführt, wenn das Makro platziert wird.


                      Merke

                      Motiv-Katalog              Mit Makros können eigene Motiv-Kataloge erstellt
                                                 werden.




A+W CAD Designer (Bars) Überblick                                                                   A-137
Spezialmuster                                                                        Tutorial




                Allgemein
                Makros sind Vorlagen, die Sie einmal erstellen und anschließend immer wie-
                der verwenden können. A+W CAD Designer (Bars) wird mit einer Reihe von
                Makros ausgeliefert. Diese Makros dienen in erster Linie dazu, den Aufbau
                und die Vorgehensweise zu verstehen. Sollten Sie eines dieser Muster ver-
                wenden können, steht dem natürlich nichts im Wege. Eine Übersicht der mit-
                gelieferten Makros finden Sie im Anhang unter Makros.
                Die Vorgehensweise zum Laden eines vorhandenen Makros ist wie folgt:
                •   Form für die Konstruktion festlegen
                •   Eigenschaften der Scheibe definieren
                •   Makro laden
                Detaillierte Beschreibungen zu Form für die Konstruktion festlegen und Eigen-
                schaften der Scheibe definieren finden Sie weiter oben.

                Makro laden
                Im nächsten Schritt wird das Makro platziert. Wir öffnen im Menü Makro den
                Menüpunkt Freies Muster und klicken mit der Maus auf die Scheibe. Es öffnet
                sich der Dialog Makro auswählen.




                Zu dieser Schulungseinheit gehören:
                 Softwarereferenz, “Makro auswählen” auf Seite A-225
                 “Anhang – Makrokatalog” auf Seite A-175




A-138                                                   A+W CAD Designer (Bars) Überblick
Tutorial                                                                            Spezialmuster




                      Demos und Übungen
                      In diesem Abschnitt erfahren Sie, wie Sie in A+W CAD Designer (Bars) mit
                      Makros arbeiten.

                      Trainerdemo: Vorhandene Makros erläutern
                      Es werden zwei Makros gezeigt und erläutert.
                      Folgende Dialoge werden unter diesem Aspekt erklärt:
                      •   Dialog Makro auswählen
                      •   Dialog Makro - Parameter
                      •   Dialog Relativer Abstand
                      Der Dialog Makro auswählen öffnet sich, wenn Sie die Symbol-Schaltfläche
                      Neues Makro betätigen und anschließend auf die Scheibe klicken. Der Dialog
                      Makro - Parameter öffnet sich automatisch, wenn seitens des Anwenders nö-
                      tig sind. Den Dialog Relativer Abstand öffnen Sie, indem Sie den Wert markie-
                      ren und anschließend die Schaltfläche [Ändern] betätigen.

                      Trainerdemo: Ein vorhandenes Makros ändern
                      Es wird gezeigt, dass und wie Sie ein vorhandenes Makro nach dem Platzie-
                      ren bearbeiten können.

                      Trainerdemo: Eigene Makros erstellen
                      Es wird gezeigt, wie Sie anhand von Makros einen eigenen Motivkatalog zu-
                      sammen stellen können.




A+W CAD Designer (Bars) Überblick                                                           A-139
Spezialmuster                                                                           Tutorial




                Übung 1: Platzieren Sie das Makro York3H1S auf einer Scheibe




                Erstellen Sie eine Scheibe gemäß den unten aufgeführten Spezifikationen und
                platzieren das Makro York3H1S.

                Aufgabenstellung
                Legen Sie folgende Scheibe an:
                •   Modell-Nummer:
                    Für die Sprossenkonstruktion dient das Modell Nr. 0 mit einer Höhe von
                    800 mm und einer Breite von 600 mm.
                •   Eigenschaften der Scheibe:
                    Der Rahmen hat eine Stärke von 11 mm. Bei dem Kunden handelt es sich
                    um die Firma Albrecht GmbH. Die Kundennummer ist 811. Die Firma Alb-
                    recht GmbH hat mit Auftrag Nummer 2125 2 Stück dieser Konstruktion für
                    die Baustelle Wohnanlage II bestellt. Es handelt sich um ein Isolierglas mit
                    einem Abstandhalter von 10 mm.
                •   Da die Firma Albrecht GmbH dieses Fenster häufig in Wohnanlagen ver-
                    baut, gibt es bereits ein Makro dafür. Das Makro heißt York3H1S.

                Übung 1: Lösung
                Die einzelnen Schritte dieser Aufgabe werden in drei Dialogen vorgenommen:
                •   Dialog Modell-Erfassung
                •   Dialog Eigenschaften der Scheibe (öffnet sich automatisch)
                •   Dialog Neues Makro




A-140                                                    A+W CAD Designer (Bars) Überblick
Tutorial                                                                             Spezialmuster




                       Sprossenkonstruktion erstellen
                      1 Öffnen Sie den Dialog Modell-Erfassung.
                      2 Wählen Sie die Modell-Nummer 000 aus der Kombobox aus.
                      3 Geben Sie im Feld Breite 600 ein.
                      4 Geben Sie im Feld Höhe 800 ein.
                      5 Betätigen Sie die Schaltfläche [OK.]. Es öffnet sich der Dialog Eigenschaf-
                        ten Scheibe.
                      6 Geben Sie im Feld X-Position 0 ein.
                      7 Geben Sie im Feld Y-Position 0 ein.
                      8 Geben Sie im Feld Ausrichtung 0 ein.
                      9 Geben Sie im Feld Rückschnitt 11 mm ein.
                      10 Geben Sie im Feld Auftragsnummer 2125 ein.
                      11 Geben Sie im Feld Positionsnummer 1 ein.
                      12 Geben Sie im Feld Kundenname Albrecht GmbH ein.
                      13 Geben Sie im Feld Kundennummer 811 ein.
                      14 Geben Sie im Feld Auftragsmenge 2 ein.
                      15 Geben Sie im Feld SZR1 10 mm ein.
                      16 Markieren Sie im Bereich Extra den Eintrag Kommisionstext und geben Sie
                         Wohnanlage II ein.
                      17 Betätigen Sie die Schaltfläche [OK]. Das Modell wird auf der Arbeitsfläche
                         platziert.
                      18 Betätigen Sie die Symbol-Schaltfläche [Neues Makro]. Platzieren Sie den
                         Mauszeiger auf dem Modell und betätigen Sie die linke Maustaste. Es öff-
                         net sich der Dialog Makro auswählen.
                      19 Wählen Sie das Marko York3H1S aus.
                      20 Betätigen Sie die Schaltfläche [OK].
                      21 Es öffnet sich der Dialog Makro-Parameter. Markieren Sie Breite der Raute
                         und betätigen Sie die Schaltfläche [Ändern...].
                      22 Es öffnet sich der Dialog Relativer Abstand. Geben Sie für die Breite der
                         Rauten 125 mm ein. Schließen Sie den Dialog mit der Schaltfläche [OK].
                      23 Markieren Sie Höhe der Raute und betätigen Sie die Schaltfläche [Än-
                         dern...].
                      24 Es öffnet sich der Dialog Relativer Abstand. Geben Sie für die Höhe der
                         Rauten 150 mm ein. Schließen Sie den Dialog mit der Schaltfläche [OK].
                      25 Schließen Sie den Dialog Makro-Parameter mit der Schaltfläche [OK].




A+W CAD Designer (Bars) Überblick                                                           A-141
Spezialmuster                                                                        Tutorial




                26 Das Makro wird platziert. Die Sprossenkonstruktion sieht wie folgt aus:




                    Abb. A-42   Ergebnis Übung 1


                Übung 2: Änderungen am Makro York3H1S auf der Scheibe vor-
                nehmen




                Sie sind gerade mit dem Platzieren des Makros York3H1S fertig, da ruft ein
                Mitarbeiter der Firma Albrecht GmbH an. Er ändert die Konstruktion wie folgt:
                Die mittlere Raute soll oben und unten keine Sprossen mehr haben. Diese
                Konstruktion wird zukünftig für einen neuen Fertighaustyp benötigt. Sie wird
                als Datei unter dem Namen York3H1S-WAII gespeichert.

                Aufgabenstellung
                •   Wählen Sie das entsprechende Werkzeug aus.
                •   Entfernen Sie die gewünschten Sprossen.




A-142                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                            Spezialmuster




                      Übung 2: Lösung
                      Für diese Übung sind vier Schritte notwendig:
                      •   Werkzeug Element auswählen aktivieren.
                      •   Sprosse oberhalb der mittleren Raute markieren und die <Entf>-Taste be-
                          tätigen.
                      •   Sprosse unterhalb der mittleren Raute markieren und die <Entf>-Taste be-
                          tätigen. Die Sprossenkonstruktion sieht wie folgt aus:




                          Abb. A-43   Ergebnis übung 2


                      •   Menü Datei öffnen. Menüpunkt Speichern unter auswählen.
                      •   Im Feld Dateiname York3H1S-WAII eingeben und den Dialog mit der
                          Schaltfläche [OK] schließen.
                      Sie haben diese Konstruktion jetzt als Datei gespeichert. Das heißt, wann im-
                      mer Sie diese Konstruktion mit diesen Abmessungen benötigen, können Sie
                      einfach die Datei öffnen.




A+W CAD Designer (Bars) Überblick                                                           A-143
Spezialmuster                                                                        Tutorial




                Übung 3: Änderungen am Makro York3H1S vornehmen und das
                Makro unter einem anderen Namen speichern




                Die Firma Albrecht GmbH setzt Sie davon in Kenntnis, dass die Sprossen-
                konstruktion York3H1S-WAII am Markt so gut ankommt, dass man sie zukünf-
                tig auch bei anderen Scheibenmaßen verwenden wird.
                Um in Zukunft Zeit zu sparen, erstellen Sie sich ein Makro und speichern die-
                ses ebenfalls unter dem Namen York3H1S-WAII gespeichert.

                Aufgabenstellung
                •   Öffnen Sie das Makro York3H1S.
                •   Nehmen Sie die entsprechenden Änderungen vor.
                •   Speichern Sie das neue Marko unter York3H1S-WAII.

                Übung 3: Lösung
                Für diese Übung sind vier Schritte notwendig:
                •   Makro York3H1S laden.
                •   Sprosse oberhalb der mittleren Raute markieren und die <Entf>-Taste be-
                    tätigen. Die Sprosse wird gelöscht.
                •   Sprosse unterhalb der mittleren Raute markieren und die <Entf>-Taste be-
                    tätigen. Die Sprosse wird gelöscht.
                •   Im Menü Makro klicken Sie den Menüpunkt Speichern an. Es öffnet sich
                    der Dialog Makro speichern. Im Feld Speichern unter geben Sie
                    York3H1S-WAII ein. Im Feld Beschreibung können Sie einen weiteren
                    Text hinterlegen. Den Dialog schließen Sie mit der Schaltfläche [OK].




A-144                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                            Spezialmuster




                          Abb. A-44   Ergebnis Übung 3


                      Sie haben diese Konstruktion jetzt als Makro gespeichert. Das heißt, wann im-
                      mer Sie diese Konstruktion mit anderen Abmessungen benötigen, können Sie
                      einfach eine Scheibe mit den entsprechenden Maßen erstellen und das Makro
                      platzieren.

                      Übung 4: Erstellen eines eigenen Makros




                      Die Firma Müller GmbH hat eine neue Konstruktion in ihren Sprossenkatalog
                      aufgenommen. Es handelt sich dabei um eine Konstruktion, die wie ein T aus-
                      sieht.
                      Um in Zukunft Zeit zu sparen, erstellen Sie sich ein Makro und speichern die-
                      ses unter dem Namen T-Sprosse.

                      Aufgabenstellung
                      •   Erstellen Sie das Makro.
                      •   Speichern Sie das Makro.



A+W CAD Designer (Bars) Überblick                                                           A-145
Spezialmuster                                                                       Tutorial




                Übung 4: Lösung
                Für diese Übung sind vier Schritte notwendig:
                Die einzelnen Schritte dieser Aufgabe werden in drei Dialogen vorgenommen:
                •   Menüpunkt Neues Makro aktivieren
                •   Werkzeug Eingabe Intervalle für Fangpunkte aktivieren
                •   Werkzeug Anzahl auf Objekt erzeugen aktivieren
                •   Werkzeug Gerade Sprosse aktivieren
                •   Makro speichern


                 Makro erstellen und speichern
                1 Öffnen Sie im Menü Makro den Menüpunkt Neues Makro.
                2 Auf Ihrem Bildschirm erscheint dann eine Scheibe. Die Scheibe hat die
                  Maße 3 m x 3 m und hat 8 Fangpunkte (je 4 am Innenrahmen und 4 an der
                  Scheibenaußenkante).




                3 Wenn Sie sich im Vergrößerungsmodus eine der Rahmenecken vergrö-
                  ßern, können Sie die Fangpunkte deutlich erkennen.
                4 Setzen Sie jetzt je einen Fangpunkt (Intervall = 2) auf den oberen und un-
                  teren Rahmen.
                    Im nächsten Schritt definieren Sie den Abstand der horizontalen Sprosse
                    vom Scheibenrand.




                5 Klicken Sie auf die SchaltflächeRelativ und anschließend auf den Fang-
                  punkt des oberen Scheibenrandes.
                6 Es öffnet sich nachstehende Dialogbox




A-146                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                             Spezialmuster




                         Hier werden die Eingaben für die x- und y-Achse definiert. Unter Relativ-
                         DX geben Sie den Abstand von 0 an, da sich der neue Fangpunkt auf der
                         x-Achse nicht verändert.
                      7 Bestätigen Sie nun die Angaben, werden Sie zur Eingabe von Relativ-DY
                        aufgefordert. Hier geben Sie den Abstand von 300 mm an. Da sich die ho-
                        rizontale Sprosse unterhalb des Fangpunktes (am oberen Scheibenrand)
                        befindet, müssen Sie eine -300 eingeben.




                         Dieser Wert ist editierbar und wird bei erneutem Laden des Makros abge-
                         fragt. Erfassen Sie bitte einen Text als Erklärung; in unserem Beispiel Ab-
                         stand Scheibenrand bis Sprossenmitte.




A+W CAD Designer (Bars) Überblick                                                            A-147
Spezialmuster                                                                         Tutorial




                8 Wenn Sie die Eingaben jetzt bestätigen, sehen Sie folgendes Bild:




                   Abb. A-45   Zwischenergebnis Übung 4


                   Im nächsten Schritt setzen Sie die Fangpunkte am rechten und am linken
                   Scheibenrand. Sie beginnen mit dem linken Scheibenrand.




                9 Klicken Sie bitte wieder auf Relativ und anschließend auf den oberen
                  Fangpunkt des linken Scheibenrandes. Es öffnet sich erneut die Dialogbox
                  Relativer Abstand. Der Relativ-DX ist wieder 0. Beim Relativ-DY klicken
                  Sie auf Wie andere Eingabe und anschließend auf [OK]. Es öffnet sich die
                  nächste Dialogbox.




                   Hier finden Sie eine Auswahl vorhandener Eingaben mit Bezeichnungen
                   und Werten vor. Schauen Sie sich alle Nummern in Ruhe an. Bei #7 ange-



A-148                                                 A+W CAD Designer (Bars) Überblick
Tutorial                                                                           Spezialmuster




                         kommen, werden Sie feststellen, dass hier Wert und Text von unserem
                         ersten relativen Fangpunkt hinterlegt ist.




                      10 Bestätigen Sie nun die Auswahl mit [OK] und Sie erhalten folgendes Bild:




                         Abb. A-46   Zwischenergebnis Übung 4


                      11 Setzen Sie nun bitte den noch fehlenden Fangpunkt auf dem rechten
                         Scheibenrand.
                         Anschließend setzen Sie die Sprossen ein.




A+W CAD Designer (Bars) Überblick                                                          A-149
Spezialmuster                                                                        Tutorial




                12 Aktivieren Sie zunächst die SchaltflächeSprosse, klicken Sie dann auf den
                   linken und anschließend auf den rechten Fangpunkt des Scheibenrandes.
                   Sie erhalten folgende Darstellung.




                   Abb. A-47   Zwischenergebnis Übung 4


                13 Fügen Sie nun die noch fehlende senkrechte Sprosse ein. A+W CAD De-
                   signer (Bars) zeichnet wie folgt




                   Abb. A-48   Zwischenergebnis Übung 4



A-150                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                            Spezialmuster




                      14 Wählen Sie nun im Menü Makro den Eintrag Speichern.
                         Es öffnet sich der Dialog




                         Im Feld Speichern unter vergeben Sie den Namen für das Makro (im Bei-
                         spiel oben T-Sprosse).
                         Im Feld Beschreibung können Sie noch weitere Bemerkungen hinterlegen.
                         Die Felder Artikelbeschreibung und Artikelnummer sind nur aktiv, wenn ein
                         Auftragserfassungssystem (wie z. B. A+W Enterprise, A+W Business) vor-
                         geschaltet ist. Sie könnten dann hier die entsprechenden Nummern hinter-
                         legen.
                      15 Betätigen Sie die Schaltfläche [OK]. Das Makro ist gespeichert.
                         Um das Makro abspielen zu können, müssen Sie als nächstes eine Schei-
                         be auf Ihrem Bildschirm platzieren.




A+W CAD Designer (Bars) Überblick                                                          A-151
Spezialmuster                                                                         Tutorial




                16 Ist dies geschehen, klicken Sie auf die SchaltflächeNeues Makro und dann
                   auf die Scheibe. Sie sehen die folgende Dialogbox




                   Wählen Sie jetzt das Makro T-Sprosse und klicken auf [OK].
                   In der nächsten Dialogbox werden die Makro-Parameter abgefragt, deren
                   Wert im Dialog Relativer Abstand auf Editierbar steht.




                   Durch ein Doppelklick auf den Eintrag im Feld Wert, öffnet sich der Dialog
                   Relativer Abstand, dessen Wert Sie dann ggf. ändern können.
                17 Bestätigen Sie die Eingabe mit [OK]. Das Makro wird platziert.




A-152                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                           Spezialmuster




                      Übung 5: Makro erstellen und mittels Referenzpunkt platzieren




                      Aufgabenstellung
                      •   Definieren Sie einen Punkt als Referenzpunkt.
                      •   Erstellen Sie das Makro.
                      •   Speichern Sie das Makro.
                      •   Platzieren Sie zwei Scheiben.
                      •   Platzieren Sie auf der ersten Scheibe das Makro mittels des Referenz-
                          punktes.
                      •   Platzieren Sie auf der zweiten Scheibe das Makro mittels des Referenz-
                          punktes.




A+W CAD Designer (Bars) Überblick                                                          A-153
Spezialmuster                                                                         Tutorial




                Übung 5: Lösung
                Für diese Übung sind vier Schritte notwendig:
                Die einzelnen Schritte dieser Aufgabe werden in drei Dialogen vorgenommen:
                •   Menüpunkt Neues Makro aktivieren
                •   Werkzeug Eingabe Intervalle für Fangpunkte aktivieren
                •   Werkzeug Anzahl auf Objekt erzeugen aktivieren
                •   Fangpunkt als Referenzpunkt deklarieren
                •   Makro speichern
                •   Zwei Scheiben auf der Arbeitsfläche platzieren
                •   Makro auf der unteren Scheibe platzieren
                •   Makro auf der oberen Scheibe platzieren.


                 Makro erstellen, speichern und platzieren (Referenzpunkt)
                1 Öffnen Sie im Menü Makro den Menüpunkt Neues Makro.
                2 Auf Ihrem Bildschirm erscheint dann eine Scheibe.
                3 Setzen Sie jetzt einen Fangpunkt, um den Mittelpunkt auf der unteren
                  Scheibengeraden zu ermitteln. Dieser Fangpunkt dient gleichzeitig als Re-
                  ferenzpunkt und ist später in der Dialogbox Makro Auswählen mit einem ro-
                  ten X gekennzeichnet.




                4 Klicken Sie jetzt auf dieSymbol-Schaltfläche [Referenz-Punkt], öffnet sich
                  die Dialogbox Referenz-Punkt.




                5 Klicken Sie jetzt bitte den Fangpunkt an, der als Referenzpunkt gelten soll;
                  die Koordinaten werden übernommen. Erfassen Sie eine Bezeichnung für
                  den Referenzpunkt (in unserem Beispiel Start), klicken Sie anschließend
                  auf [Setzen] und bestätigen die Eingabe mit [OK].
                6 Sollten Sie mehrere Fangpunkte gesetzt haben, werden Sie feststellen,
                  dass alle gelöscht wurden - es ist lediglich der Referenzfangpunkt geblie-
                  ben. Fangpunkte können jetzt nur noch durch die Eingabe von relativen
                  Abständen zum Referenzpunkt gesetzt werden. Somit beziehen sich alle
                  Maße auf diesen Referenzpunkt.




A-154                                                   A+W CAD Designer (Bars) Überblick
Tutorial                                                                             Spezialmuster




                         Als nächstes setzen Sie einen mittleren Fangpunkt am oberen Scheiben-
                         rand, damit die Sprossen zum Schluss mit dem Scheibenrand verbunden
                         werden können.




                      7 Klicken Sie bitte auf Relativ und dann auf den Referenzpunkt. Es öffnet
                        sich die Dialog-Box Relativer Abstand.
                      8 Bei Relativ - DX tragen Sie den festen Wert mit 0 ein und bei Relativ - DY
                        Wie andere Eingabe. In der dann erscheinenden Auswahl wählen Sie #2
                        Wie Rahmenhöhe: Bestätigen Sie die Eingaben mit [OK], der Fangpunkt
                        wird gesetzt.
                      9 Anschließend erfassen Sie den Fangpunkt in der Mitte. Gehen Sie vor wie
                        oben beschrieben, allerdings geben Sie bei Relativ - DY Wie andere Ein-
                        gabe #2 = Rahmenhöhe Faktor 0,5 ein.




                         Abb. A-49    Zwischenergebnis Übung 5


                         In den jetzt folgenden Schritten platzieren Sie die Fangpunkte für die Rau-
                         te.




A+W CAD Designer (Bars) Überblick                                                            A-155
Spezialmuster                                                                           Tutorial




                10 Klicken Sie wieder auf Relativ und dann auf den mittleren Fangpunkt. Re-
                   lativ - DX erfassen Sie mit 0 und Fester Wert, den Relativ - DY mit 100 (hal-
                   be Rautenhöhe), Editierbar und als Text Halbe Rautenhöhe.




                11 Für den unteren Fangpunkt gehen Sie in gleicher Weise vor, jedoch geben
                   Sie bei Relativ - DY Wie andere Eingabe #7 = Halbe Rautenhöhe Faktor -
                   1,0 ein.




                   Abb. A-50    Zwischenergebnis Übung 5




A-156                                                    A+W CAD Designer (Bars) Überblick
Tutorial                                                                           Spezialmuster




                      12 Beim Setzen der Fangpunkte für die Rautenbreite gehen Sie bitte in glei-
                         cher Weise vor (halbe Rautenbreite = 75). Die Darstellung ist dann wie
                         folgt.




                         Abb. A-51   Zwischenergebnis Übung 5




A+W CAD Designer (Bars) Überblick                                                          A-157
Spezialmuster                                                                        Tutorial




                13 Aktivieren Sie jetzt den Sprossenmodus durch Klicken auf Sprosse und
                   verbinden Sie die einzelnen Fangpunkte der Raute. Die Darstellung ist wie
                   folgt




                   Abb. A-52   Zwischenergebnis Übung 5




A-158                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                           Spezialmuster




                      14 Anschließend verbinden Sie die Raute mit den Fangpunkten am Scheiben-
                         rahmen. Das Makro sieht jetzt wie folgt aus:




                         Abb. A-53   Zwischenergebnis Übung 5


                      15 Speichern Sie das Makro im Menüpunkt Makro unter Speichern (in unse-
                         rem Beispiel unter Raute 1). In der Makro Auswahl werden nun 2 Makros
                         mit dem Namen Raute 1 zu finden sein. Eins als Raute 1-1 und das zweite
                         als Raute 1-2. Das Makro Raute 1-1 ist ohne Referenzpunkt und das Ma-
                         kro 1-2 ist mit Referenzpunkt (rotes X).
                      16 Im nächsten Schritt platzieren wir zwei Scheiben auf unserem Bildschirm.
                         Dazu gehen Sie bitte wie folgt vor:
                         Platzieren Sie zunächst die erste Scheibe mit den Maßen 800 x 600. An-
                         schließend wiederholen Sie den Vorgang für die zweite Scheibe (identi-
                         sche Abmessungen). Nach dem Dialog Modell-Erfassung erscheint der
                         Dialog Neue Scheibenposition ... Dieser Dialog dient dem Platzieren der
                         zweite Scheibe in Relation zur ersten Scheibe.




A+W CAD Designer (Bars) Überblick                                                          A-159
Spezialmuster                                                                            Tutorial




                17 Für die X-Position geben Sie -400 ein und für die Y-Position 100. Die linke,
                   ausgegraute Scheibe symbolisiert die bereits platzierte Scheibe. Bei der
                   rechten Scheibe mit dem Text "Einzugebende Scheibe" handelt es sich um
                   die Scheibe, die Sie jetzt platzieren. Achten Sie auf die ausgewählten
                   Ecken beider Scheiben. In unserem Beispiel ist die untere rechte Ecke für
                   die bereits platzierte Scheibe aktiv und die obere linke Ecke für die jetzt zu
                   setzende Scheibe.




A-160                                                    A+W CAD Designer (Bars) Überblick
Tutorial                                                                         Spezialmuster




                      18 Nachdem Sie die Eingaben mit [OK] bestätigt haben, erscheint folgendes
                         Bild:




                         Abb. A-54   Zwischenergebnis Übung 5




A+W CAD Designer (Bars) Überblick                                                        A-161
Spezialmuster                                                                         Tutorial




                19 Anschließend setzen Sie fünf Fangpunkte auf den Scheibenrand der unte-
                   ren Scheibe.




                20 Dann wechseln Sie in den Makro-Modus durch klicken auf Makro. Wenn
                   Sie jetzt auf die untere Scheibe klicken, öffnet sich wieder die Dialogbox
                   Makro auswählen. Wählen Sie bitte das oben erstellte Makro - Raute 1-2.
                   Wenn Sie die Eingabe bestätigen, sehen Sie wieder die zwei Scheiben auf
                   Ihrem Bildschirm. Klicken Sie jetzt auf den zweiten Fangpunkt von links
                   und Sie werden wieder zur Eingabe der Relativen Abstände aufgefordert.
                   In unserem Beispiel hat die Raute eine Höhe von 150 mm und eine Breite
                   von 100 mm.




A-162                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                          Spezialmuster




                      21 Nach dem Bestätigen dieser Eingaben wird die Raute platziert.




                         Abb. A-55   Zwischenergebnis Übung 5




A+W CAD Designer (Bars) Überblick                                                        A-163
Spezialmuster                                                                       Tutorial




                22 Aktivieren Sie nun das Symbol In Schnittpunkten, klicken Sie dann auf das
                   obere, senkrechte Sprossensegment (siehe Pfeil, oben) und im Anschluss
                   auf den unteren Scheibenrahmen der 2. Scheibe. Dort wird dann - genau
                   in der Verlängerung zur Sprosse der 1. Scheibe - ein Fangpunkt gesetzt,
                   den Sie dann wiederum als Ausgangspunkt für das weitere Makro verwen-
                   den können.




                   Abb. A-56   Zwischenergebnis Übung 5




A-164                                                 A+W CAD Designer (Bars) Überblick
Tutorial                                                                         Spezialmuster




                      23 Beim Platzieren des neuen Makros gehen Sie vor, wie bereits oben be-
                         schrieben. Die Darstellung ist dann wie folgt




                         Abb. A-57     Ergebnis Übung 5


                      Zu dieser Schulungseinheit gehören:
                       Softwarereferenz, “Makro auswählen” auf Seite A-225
                       Softwarereferenz, “Makro-Parameter” auf Seite A-226
                       Softwarereferenz, “Relativer Abstand” auf Seite A-227
                       “Anhang – Makrokatalog” auf Seite A-175




A+W CAD Designer (Bars) Überblick                                                        A-165
Datenaustausch                                                                            Tutorial




                 Datenaustausch
                 In diesem Themenblock lernen Sie, wie Sie die Daten aus übergeordneten
                 Programmen importieren und exportieren.


                 Datenimport
                 Lernziele

                 • Das Arbeiten mit Übergabedateien kennenlernen und verstehen
                 • Postionen importieren


                 Nutzen

                 Wenn Sie A+W CAD Designer (Bars) in Verbindung mit einem übergeordneten
                 System (z. B. A+W Business) nutzen, müssen Sie wissen, wie Dateien zu importieren
                 sind.


                 Definition

                 Übergabedatei              enthält Positionen, die von einem übergeordneten
                                            System an A+W CAD Designer (Bars) übergeben
                                            wurden.

                 Schnittstelle              Über diese werden Daten an A+W CAD Designer
                                            (Bars) übergeben.


                 Merke

                 Order.XML                  Dieser Modus muss entsprechend konfiguriert werden.




A-166                                                     A+W CAD Designer (Bars) Überblick
Tutorial                                                                           Datenaustausch




                      Übergabedateien
                      Daten werden importiert, wenn A+W CAD Designer (Bars) mit einem überge-
                      ordneten Auftragsbearbeitungssystem eingesetzt wird. Dann haben Sie die
                      Möglichkeit, Sprossendaten aus dem Auftragsbearbeitungssystem (z. B.
                      A+W Business) an A+W CAD Designer (Bars) zu übergeben. Das kann z. B.
                      notwendig sein, um nachträgliche Änderungen an Sprossenkonstruktionen
                      vorzunehmen. Dazu verfügt A+W CAD Designer (Bars) über eine spezielle
                      Schnittstelle.
                      Im entsprechend eingestellten Modus liest A+W CAD Designer (Bars) beim
                      Importvorgang alle *.xml-Dateien auf einmal ein. Eine Order.XML Datei enthält
                      immer nur einen Datensatz.

                         Schnittstelle konfigurieren
                         Das Einrichten und Konfigurieren der Schnittstelle sowie alle damit verbun-
                         denen Einstellungen werden grundsätzlich von A+W-Mitarbeitern vor Ort
                         vorgenommen und an dieser Stelle nicht weiter vertieft.

                      Ist der Importvorgang erfolgreich, wird die Order.xml Datei in das Verzeichnis
                      Archive verschoben. Tritt während des Imports ein Fehler auf, wird die Datei
                      in das Verzeichnis Probleme verschoben.


                      Dateien importieren - Neu

                       So importieren Sie eine Datei
                      1 Wählen Sie im Menü Datei > Importieren > Übergabedatei.
                         Der Dialog Auswahl - Auftrag/Position wird geöffnet.




                      2 Der Status Konstruiert zeigt Ihnen, dass der Datensatz fertig ist und ge-
                        druckt werden kann. Sie können sich die einzelnen Konstruktionen anzei-
                        gen lassen, indem Sie eine Position markieren und die Schaltfläche [OK]



A+W CAD Designer (Bars) Überblick                                                            A-167
Datenaustausch                                                                       Tutorial




                    betätigen. Dann wird die Position in A+W CAD Designer (Bars) geöffnet.
                    Die weiteren Positionen öffnen Sie über das Menü Datei > Öffnen.
                 3 Betätigen Sie die Schaltfläche [Abbrechen] werden die Positionen impor-
                   tiert ohne sie zu öffnen. Zum Öffnen der Postionen gehen Sie wieder über
                   das Menü Datei > Öffnen.
                 4 Die Schaltfläche [Abgleich] kommt bei Fassadenanlagen zum Einsatz.
                   Wenn Sie diese Schaltfläche betätigen, können Sie eine Übergabepostion
                   nach der anderen auf der Arbeitsfläche als Fassade platzieren. Sie werden
                   ab der zweiten Position nach den entsprechenden Referenzpunkten ge-
                   fragt.


                 Weitere Informationen zu Daten importieren
                  Softwarereferenz, “Übergabedatei importieren” auf Seite A-202
                  Softwarereferenz, “Neue Scheibenposition” auf Seite A-204




A-168                                                     A+W CAD Designer (Bars) Überblick
Tutorial                                                                               Datenaustausch




                      Datenexport
                      Lernziele

                      •   Drucken und plotten von Konstruktionen kennenlernen
                      •   Drucken von Übergabedateien kennenlernen
                      •   Zuschnittlisten verstehen
                      •   Konstruktionen als Grafiken exportieren


                      Definition

                      Plotter                     Ausgabegerät, das technische Zeichnungen auf
                                                  verschiedenen Materialien darstellt.


                      Merke

                      Drucker einrichten          Bevor Sie etwas drucken können, müssen Sie in der
                                                  Druckereinrichtung den bzw. die Drucker einrichten.

                      Produktionspapiere          Werden den Kundenwünschen angepasst.


                      Konstruktionen und Übergabedateien
                      Zur Ausgabe wird eine maßstabgetreue Zeichnung gedruckt, die auch die Lis-
                      te der zu schneidenden Profile enthält. Diese Zeichnung enthält außerdem
                      alle relevanten Informationen für die Sprossenkreuzungen, wie z. B. den Fräs-
                      winkel. Alle Produktionspapiere sind frei gestaltbar und können auf dem Mo-
                      nitor oder als Ausdruck ausgegeben werden. Die Ausgabe kann auch über
                      einen Plotter im Maßstab 1:1 erfolgen.


                      Drucker einrichten
                      Bevor Sie etwas drucken können, müssen Sie den Drucker einrichten. In A+W
                      CAD Designer (Bars) können Sie zwei unterschiedliche Drucker definieren:
                      •   Drucker 1
                      •   Drucker 2
                      Sollten Sie über einen Plotter verfügen, wird dieser in A+W CAD Designer
                      (Bars) unter Drucker 2 geführt.




A+W CAD Designer (Bars) Überblick                                                                 A-169
Datenaustausch                                                                        Tutorial




                 Den entsprechenden Dialog öffnen Sie über Datei > Druckereinrichtung...




                  So richten Sie den Drucker ein
                 1 Öffnen Sie den Dialog Druckereinrichtung...
                 2 Geben Sie im Bereich Drucker 1 den Standarddrucker ein. Um in die Win-
                   dows Druckereinrichtung zu wechseln, betätigen Sie die Schaltfläche [Än-
                   dern...].
                 3 Es öffnet sich der Dialog Druckeinrichtung. Dort sind alle für Ihren Compu-
                   ter installierten Drucker gelistet. Wählen Sie den entsprechenden Drucker
                   aus. Schließen Sie den Dialog mit der Schaltfläche [OK]. Sie befinden sich
                   wieder im Dialog Druckereinrichtung von A+W CAD Designer (Bars).
                 4 Im Bereich Drucker 2 haben Sie die Möglichkeit einen Drucker zuzuwei-
                   sen, auf dem nur bestimmte Elemente einer Konstruktion gedruckt werden.
                   So können Sie z. B. definieren, dass auf Drucker 2 nur Bögen einer Kons-
                   truktion gedruckt werden.
                   Darüber hinaus ist dieser Bereich dem Plotten vorbehalten. Arbeiten Sie in
                   Ihrem Hause mit einem Plotter, dann wird dieser im Bereich 2 eingetragen.
                   Zusätzlich müssen Sie dann die Checkbox Plotter aktivieren. Erst nach-
                   dem die Checkbox Plotter aktiviert ist, werden die Radiotasten Maximale
                   Größe und 1:1 aktiv. Sie müssen dann wählen, in welcher Größe der Aus-
                   druck auf dem Plotter erfolgen soll.
                 5 Rechts oben können Sie die Anzahl der Kopien einstellen. Bei mehreren
                   Kopien können Sie im Feld darunter die Sortierreihenfolge durch Aktivie-
                   rung der entsprechenden Radiotasten festlegen.

                    Anzahl der Kopieen
                    Die Anzahl der Kopieen wird nach jedem Druck auf 1 zurück gesetzt.




A-170                                                   A+W CAD Designer (Bars) Überblick
Tutorial                                                                             Datenaustausch




                      Konstruktionen drucken
                      Die erstellten Konstruktionen können Sie auf Drucker 1, auf Drucker 2 oder auf
                      beiden Druckern ausgeben.
                      Über Datei > Drucken > Konstruktion öffnen Sie den Dialog. Auf dem zweiten
                      Drucker können Sie angebeben, was gedruckt werden soll. Sie haben die
                      Möglichkeit alle Scheiben zu drucken, einzelnen Scheiben zu drucken oder
                      auch nur einen aktuellen Ausschnitt zu drucken. Die Auswahl treffen Sie durch
                      Aktivierung der entsprechenden Radiotaste.


                       So drucken Sie eine Konstruktion
                      1 Öffnen Sie den Dialog Drucken.
                      2 Für die gewünschte Auswahl aktivieren Sie die entsprechende Radiotaste.
                      3 Über die Schaltfläche [OK] starten Sie den Druck.


                      Übergabedatei drucken
                      Übergabedateien sind Dateien, die von anderen Pogrammen (A+W Enterpri-
                      se, A+W Business, etc.) an A+W CAD Designer (Bars) übergeben werden.
                      Weitere Informationen zu den Übergabedateien finden Sie unter
                       “Datenimport” auf Seite A-166
                      Zum Drucken dieser Dateien wurden in A+W CAD Designer (Bars) eigene Me-
                      nüpunkte geschaffen. Sie können Übergabedateien in zwei verschiedenen
                      Varianten drucken:
                      •   Übergabedatei
                          Wählen Sie diesen Menüpunkt, erhalten Sie einen Ausdruck, der im obe-
                          ren Bereich eine Liste mit Informationen zum Auftrag (Auftragsnummer,
                          Position, Kunde, etc.) und Artikel (Sprosse, Farbe, etc.) zeigt und im unte-
                          ren Bereich die Skizze.




A+W CAD Designer (Bars) Überblick                                                              A-171
Datenaustausch                                                                       Tutorial




                     Abb. A-58   Ausdruck: Übergabedatei


                 •   Übergabedatei - Liste
                     Wählen Sie diesen Menüpunkt, erhalten Sie einen Ausdruck der Zuschnitt-
                     Liste mit Informationen zu Auftrag und Position sowie zum Zuschnitt der
                     Sprosse(n).




                     Abb. A-59   Ausdruck: Übergabedatei-Liste


                     Unterhalb von Auftrag und Pos wird Ihnen die Auftragsnummer sowie die
                     Positionsnummer angezeigt. Die Werte hinter BxH zeigen Ihnen die Ab-
                     messungen der Scheibe. Im oberen Beispiel ist die Scheibe 800 breit und
                     1200 hoch. Der in Klammern gesetzte Wert (Menge=1) zeigt Ihnen, dass


A-172                                                      A+W CAD Designer (Bars) Überblick
Tutorial                                                                            Datenaustausch




                         es sich um ein Stück handelt.
                         Anhand der Einträge hinter Waagerecht sehen Sie, um welche Sprosse es
                         sich handelt. Im Beispiel oben ist es eine Wiener Sprosse. Beidseitig be-
                         deutet, dass die Sprossenfarbe beidseitig ist. Die Zahl in Klammern (6)
                         zeigt Ihnen, wie oft es diese Sprosse in der Konstruktion gibt. Der Wert da-
                         hinter liefert Ihnen die Sprossenlänge.
                         Im Beispiel oben gibt es bei den senkrechten Sprossen noch die Werte F:
                         397 B - 803 B.
                         Der Buchstabe F kennzeichnet den bzw. die Fräspunkte, die bei 397 und
                         803 liegen. Der Buchstabe B bedeutet, dass die Fräspunkte auf beiden
                         Seiten sind. Abgesehen von B gibt es noch L für Fräspunkt auf der linken
                         Seite und R für Fräspunkt auf der rechten Seite.
                         Die Werte hinter Höhe zeigen Ihnen, wo die Sprossenmitten platziert sind.
                         Die waagerechten Sprossenmitten (A) liegen bei 397 und 803. Die senk-
                         rechten Sprossenmitten (B) liegen bei 263,7 und 536,3.


                       So drucken Sie eine Übergabedatei
                      1 Öffnen Sie im Menü Datei > Drucken > Übergabedatei den Dialog Listen-
                        druck.
                      2 Die Liste enthält alle Übergabedateien. Wählen Sie die gewünschte Datei
                        aus und betätigen Sie die Schaltfläche [OK].
                      3 Die Liste wird gedruckt.


                      Weitere Informationen zum Drucken
                       Softwarereferenz, “Drucken” auf Seite A-205
                       Softwarereferenz, “Druckereinrichtung” auf Seite A-207


                      Bild exportieren
                      Um eine Konstruktion als Grafik zu exportieren, steht Ihnen in A+W CAD De-
                      signer (Bars) der Menüpunkt Bild exportieren... zur Verfügung.
                      Sie haben so auch jederzeit die Möglichkeit, Konstruktionen in Form von Bil-
                      dern zu speichern oder aber die Konstruktion als Bild zu verschicken.


                       So exportieren Sie eine Konstruktion als Bild
                      1 Öffnen Sie im Menü Datei den Menüpunkt Bild exportieren. Es öffnet sich
                        der Dialog Speichern unter...
                      2 Wählen Sie aus, wo die Datei gespeichert und wie sie heißen sol und be-
                        tätigen Sie die Schaltfläche [Speichern].
                      3 Die Datei wird an der entsprechenden Stelle gespeichert.

                         Dateitypen
                         Sie können die Konstruktion als JPG, BMP und PNG speichern.




A+W CAD Designer (Bars) Überblick                                                             A-173
Konfiguration                                                                        Tutorial




                Nachrichten senden
                Um sich mit Kollegen oder Kunden austauschen zu können, wurde in A+W
                CAD Designer (Bars) die Möglichkeit geschaffen, die aktuelle Konstruktion auf
                Knopfdruck als Email zu versenden. Wenn Sie den Menüpunkt wählen, wird
                automatisch Ihr Email-Programm gestartet. Die Konstruktion wird unter dem
                Namen Object.awd der Mail als Anhang zugefügt.

                   Mail-System muss installiert sein
                   Eine Konstruktion kann nur dann als Email versendet werden, wenn ein
                   entsprechendes Mail-System installiert und konfiguriert ist.


                 So versenden Sie eine Konstruktion als Email
                1 Öffnen Sie im Menü Datei den Menüpunkt Nachricht senden. Ihr Mail-Sys-
                  tem wird geöffnet.
                2 Geben Sie den Empfänger.
                3 Geben Sie einen Text ein.
                4 Versenden Sie die Email.

                   Dateiformate
                   Die Konstruktion wird im Dateiformat awd versendet. Das setzt voraus,
                   dass beim Empfänger ein A+W CAD Designer (Bars) installiert ist. Hat der
                   Empfänger kein A+W CAD Designer (Bars) können Sie die Konstruktion
                   als Bild exportieren.




                Konfiguration
                Das Programm A+W CAD Designer (Bars) wird durch A+W-Mitarbeiter vor Ort
                konfiguriert und befindet sich danach im arbeitsfähigen Zustand. Es sind sei-
                tens des Benutzers keine weiteren Einstellungen vorzunehmen. Sollten Sie je-
                doch im Laufe Ihrer Arbeit mit A+W CAD Designer (Bars) Änderungen an der
                Konfiguration vornehmen müssen, finden Sie die Konfiguration unter:
                Stammdaten > Konfiguration bearbeiten

                   Änderungen an der Konfiguration
                   Gehen Sie mit Änderungen an der Konfiguration sensibel um. Wenn Sie
                   sich bezüglich von Änderungen nicht sicher sind, halten Sie Rücksprache
                   mit der A+W Software GmbH um unerwünschte Ergebnisse zu vermeiden!




A-174                                                  A+W CAD Designer (Bars) Überblick
Tutorial                                                                    Anhang – Makrokatalog




                      Anhang – Makrokatalog
                      Die A+W Software GmbH liefert Ihnen A+W CAD Designer (Bars) mit einer
                      Vielzahl fertiger Makros aus. Das erspart Ihnen Zeit und Arbeit. Sie können die
                      Makros gemäß den Vorgaben Ihrer Kunden schnell und einfach anpassen. Im
                      Anschluss finden Sie eine Auflistung aller Makros sowie eventuell notwendige
                      Eingaben.

                      Makro 2S2W
                      Bei diesem Makro werden zwei senkrechte und zwei waagerechte Sprossen
                      platziert. Es sind keine weiteren Eingaben nötig. Die senkrechten Sprossen
                      sind durchgehend.




A+W CAD Designer (Bars) Überblick                                                             A-175
Anhang – Makrokatalog                                                                        Tutorial




                        Makro 2S3W
                        Bei diesem Makro werden zwei senkrechte und drei waagerechte Sprossen
                        platziert. Hier ist der Abstand vom Rand anzugeben. Dieser Abstand bezieht
                        sich auf die beiden senkrechten Sprossen. Geben Sie z. B. 50 ein, werden die
                        beiden senkrechten Sprossen jeweils 50 mm vom rechten und linken Rand
                        platziert.




                        Makro 2SX4W
                        Bei diesem Makro werden drei senkrechte und vier waagerechte Sprossen
                        platziert. Es sind keine weiteren Eingaben nötig. Die senkrechten Sprossen
                        sind durchgehend.




A-176                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                                 Anhang – Makrokatalog




                      Makro Crowder
                      Bei diesem Makro werden 21 senkrechte und 13 waagerechte Sprossen plat-
                      ziert. Es sind keine weiteren Eingaben nötig. Es gibt keine durchgehenden
                      Sprossen.




                      Makro Cumbria
                      Bei diesem Makro werden vier Rauten platziert. Es ist der Abstand vom rech-
                      ten und linken Rand anzugeben sowie der Abstand vom oberen und unteren
                      Rand. Des weiteren müssen Sie die Breite und die Höhe der Raute angeben.
                      Im folgenden Beispiel wurden für die Abstände zum Rand jeweils 200 mm und
                      für die Breite und Höhe der Rauten jeweils 150 mm angegeben.




A+W CAD Designer (Bars) Überblick                                                         A-177
Anhang – Makrokatalog                                                                          Tutorial




                        Makro Diamond1
                        Bei diesem Makro werden fünf waagerechte und drei senkrechte Sprossen
                        platziert. In der mittleren senkrechten Sprosse sind zusätzlich drei Rauten in-
                        tegriert. Es ist die halbe Rautenhöhe sowie die halbe Rautenbreite anzuge-
                        ben. Im folgenden Beispiel wurden jeweils 40 mm angegeben.




                        Makro Dumfries
                        Bei diesem Makro werden vier waagerechte und vier senkrechte Sprossen so
                        platziert, dass quasi ein Rahmen entsteht. Es gibt keine durchgehenden
                        Sprossen. Die Schnittpunkte der Sprossen werden über Kreuz mit einander
                        verbunden. Es ist der Abstand zwischen den beiden Sprossen sowie der Ab-
                        stand der ersten Sprosse zum Rand hin anzugeben. Im folgenden Beispiel ist
                        der Abstand der beiden Sprossen zueinander 50 mm und der Abstand der ers-
                        ten Sprosse zum Rahmen 100 mm.




A-178                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                                   Anhang – Makrokatalog




                      Makro Durham
                      Bei diesem Makro wird ein Achteck platziert, welches an den Ecken jeweils mit
                      dem Rand durch Sprossen verbunden ist. In der Mitte der vier Schenkel befin-
                      det sich eine weitere Sprosse zum Rand hin. Es ist der Abstand der senkrech-
                      ten Sprosse zum linken bzw. rechten Rand (A) sowie der Abstand der
                      waagerechten Sprosse zum oberen bzw. unteren Rand (B) hin anzugeben. Im
                      folgenden Beispiel ist der Abstand der senkrechten Sprossen 100 mm und der
                      Abstand der waagerechten Sprosse 200 mm.




                       A




                                 B


                      Makro Galloway
                      Bei diesem Makro wird eine Form platziert, die sich aus einem Achteck mit
                      Halbkreisen sowie einem Rechteck zusammen setzt. Die Sprossen des Acht-
                      ecks sind durchgehend. Es ist der Abstand des Achtecks zum Rand, der Ra-
                      dius der Halbkreise sowie der Abstand des Rechtecks anzugeben. Im
                      folgenden Beispiel ist der Abstand des Achtecks 100 mm, der Halbkreis hat
                      einen Radius von 200 mm und der Abstand des Rechtecks ist 150 mm.




A+W CAD Designer (Bars) Überblick                                                           A-179
Anhang – Makrokatalog                                                                            Tutorial




                        Makro Kent1
                        Bei diesem Makro wird eine waagerechte und drei senkrechte Sprossen plat-
                        ziert. In der mittleren senkrechten Sprosse ist zusätzlich eine Raute integriert.
                        Es ist die Breite und die Höhe der Raute anzugeben. Im folgenden Beispiel ist
                        die Raute 125 mm breit und 210 mm hoch.




                        Makro Kent2
                        Bei diesem Makro werden zwei waagerechte und drei senkrechte Sprossen
                        platziert. In der mittleren senkrechten Sprosse sind zusätzlich zwei Rauten in-
                        tegriert. Es ist die Breite und die Höhe der Rauten anzugeben. Im folgenden
                        Beispiel sind die Rauten 125 mm breit und 210 mm hoch.




A-180                                                            A+W CAD Designer (Bars) Überblick
Tutorial                                                                    Anhang – Makrokatalog




                      Makro Kent3
                      Bei diesem Makro werden drei waagerechte und drei senkrechte Sprossen
                      platziert. In der mittleren senkrechten Sprosse sind zusätzlich drei Rauten in-
                      tegriert. Es ist die Breite und die Höhe der Rauten anzugeben. Im folgenden
                      Beispiel sind die Rauten 125 mm breit und 150 mm hoch.




                      Makro Kent4
                      Bei diesem Makro werden vier waagerechte und drei senkrechte Sprossen
                      platziert. In der mittleren senkrechten Sprosse sind zusätzlich vier Rauten in-
                      tegriert. Es ist die Breite und die Höhe der Rauten anzugeben. Im folgenden
                      Beispiel sind die Rauten 125 mm breit und 100 mm hoch.




A+W CAD Designer (Bars) Überblick                                                             A-181
Anhang – Makrokatalog                                                                          Tutorial




                        Makro Kent5
                        Bei diesem Makro werden fünf waagerechte und drei senkrechte Sprossen
                        platziert. In der mittleren senkrechten Sprosse sind zusätzlich fünf Rauten in-
                        tegriert. Es ist die Breite und die Höhe der Rauten anzugeben. Im folgenden
                        Beispiel sind die Rauten 85 mm breit und 100 mm hoch.




                        Makro Multi
                        Bei diesem Makro werden acht waagerechte und fünf senkrechte Sprossen
                        platziert. Der Abstand der Sprossen zueinander ist jeweils 202 mm. Es sind
                        keine weiteren Angaben zu machen. Aufgrund des festen Abstands der
                        Sprossen zueinander ist allerdings darauf zu achten, dass die Scheibe groß
                        genug ist, um die Sprossen zu platzieren.




A-182                                                           A+W CAD Designer (Bars) Überblick
Tutorial                                                                   Anhang – Makrokatalog




                      Makro NewVersi
                      Bei diesem Makro werden fünf waagerechte und fünf senkrechte Sprossen
                      platziert. Es sind keine weiteren Angaben nötig.




                      Makro QueenAnn
                      Bei diesem Makro werden fünf waagerechte und drei senkrechte Sprossen
                      platziert. In der rechten und linken senkrechten Sprosse sind zusätzlich drei
                      Rauten integriert. Es sind keine weiteren Angaben zu machen.




A+W CAD Designer (Bars) Überblick                                                            A-183
Anhang – Makrokatalog                                                                         Tutorial




                        Makro Sonne
                        Bei diesem Makro wird eine Sonne bestehend aus einem Halbkreis mit fünf
                        Strahlen platziert. Es ist der Abstand vom Kreismittelpunkt anzugeben. Im fol-
                        genden Beispiel sind das 300 mm.




                        Makro Sonne1
                        Bei diesem Makro wird eine Bogensprosse mit einem drei Strahlen platziert.
                        Es ist der Abstand vom oberen Rand sowie der Radius für den Bogen anzu-
                        geben. Im folgenden Beispiel sind das -500 mm als Abstand für oben und -400
                        mm als Radius.




A-184                                                          A+W CAD Designer (Bars) Überblick
Tutorial                                                                   Anhang – Makrokatalog




                      Makro York0Add1
                      Bei diesem Makro wird eine senkrechte Sprossen mit einer Raute in der Mitte
                      platziert. Es ist die Breite und die Höhe der Raute anzugeben. Im folgenden
                      Beispiel ist die Raute 125 mm breit und 210 mm hoch.




                      Makro York3H1S
                      Bei diesem Makro wird eine waagerechte und drei senkrechte Sprossen plat-
                      ziert. In den senkrechten Sprossen befinden sich mittig jeweils eine Raute. Es
                      ist die Breite und die Höhe der Raute anzugeben. Im folgenden Beispiel ist die
                      Raute 125 mm breit und 210 mm hoch.




A+W CAD Designer (Bars) Überblick                                                            A-185
Anhang – Makrokatalog                             Tutorial




A-186                   A+W CAD Designer (Bars) Überblick
A   A+W CAD Designer (Bars)
    Überblick




                  Softwarereferenz
                                                                                                         Softwarereferenz




        In diesem Kapitel finden Sie folgende Themen:
         Bedienung von A+W CAD Designer (Bars)
         Übersicht
         Umgang mit Dateien
         Werkzeuge verwenden
         Mit Spezialmustern arbeiten
         Messen und Zuschnitt
         Die Stammdaten
         Ansicht
         Die Hilfe verwenden


        Bedienung von A+W CAD Designer (Bars) ........................................................ A-190
          Softwarebegriffe .............................................................................................. A-191
            Schaltflächen ............................................................................................... A-191
            Schnelltaste/Hot-Key ................................................................................... A-191
            Radiotaste .................................................................................................... A-192
            Kombobox .................................................................................................... A-192
            Checkbox ..................................................................................................... A-192
            Register ........................................................................................................ A-192
            Menüleiste/Menüpunkt ................................................................................. A-193
            Tabellen-/Spaltenüberschrift ........................................................................ A-193
            Tastaturbefehle ............................................................................................ A-194
          Programm beenden ......................................................................................... A-195
        Übersicht ............................................................................................................. A-196
        Umgang mit Dateien ........................................................................................... A-197
          Neue Scheibe .................................................................................................. A-199
          Übergabedatei importieren .............................................................................. A-202
          Neue Scheibenposition ................................................................................... A-204
          Drucken ........................................................................................................... A-205
          Listendruck ...................................................................................................... A-206
          Druckereinrichtung .......................................................................................... A-207
        Werkzeuge verwenden ....................................................................................... A-210
        Mit Spezialmustern arbeiten ............................................................................... A-212
          Muster Senkrecht-Waagerecht ........................................................................ A-213
          Kundenvorgabe SW-Muster ............................................................................ A-216
          Eingabe Sprossen-Abstände ........................................................................... A-219
          Rautenmuster... ............................................................................................... A-220
          Fassadenanlage... ........................................................................................... A-222
          Sonne und Sterne ........................................................................................... A-223
          Makro auswählen ............................................................................................ A-225
          Makro-Parameter ............................................................................................ A-226
          Relativer Abstand ............................................................................................ A-227
        Messen und Zuschnitt ......................................................................................... A-228
          Abstand ........................................................................................................... A-229
          Zuschnitt-Informationen ................................................................................... A-230
        Die Stammdaten ................................................................................................. A-232
          Stammdaten .................................................................................................... A-233
          Stammdaten-Editor ......................................................................................... A-235
          Passwort .......................................................................................................... A-240
        Ansicht ................................................................................................................ A-241
          Vermaßung ...................................................................................................... A-242


A-188                                                                   A+W CAD Designer (Bars) Überblick
Softwarereferenz




                        Maße ............................................................................................................... A-244
                        Sprachauswahl ................................................................................................ A-245
                      Die Hilfe verwenden ............................................................................................ A-246
                        Über CAD Designer ......................................................................................... A-247




A+W CAD Designer (Bars) Überblick                                                                                                      A-189
Bedienung von A+W CAD Designer (Bars)                                         Softwarereferenz




                      Bedienung von A+W CAD De-
                      signer (Bars)
                      Das Programm starten Sie entweder über einen Desktop-Shortcut, den Sie
                      sich selber anlegen können oder über den entsprechenden Eintrag im Menü
                      Start > Programme (unter Windows).
                      Im Anschluss finden Sie Erläuterungen zu den in der Dokumentation verwen-
                      deten Begriffe und wie Sie das Programm beenden.
                      •   Softwarebegriffe
                      •   Programm beenden




A-190                                                      A+W CAD Designer (Bars) Überblick
Softwarereferenz                                         Bedienung von A+W CAD Designer (Bars)




                      Softwarebegriffe
                      In diesem Abschnitt wird Ihnen der allgemeine Umgang mit den Menüs und
                      den Dialogen vorgestellt.
                      Nachfolgend erhalten Sie Informationen zu:
                      •   Schaltflächen
                      •   Schnelltaste/Hot-Key
                      •   Radiotaste
                      •   Kombobox
                      •   Checkbox
                      •   Register
                      •   Menüleiste/Menüpunkt
                      •   Tabellen-/Spaltenüberschrift
                      •   Tastaturbefehle


                      Schaltflächen




                      Schnelltaste/Hot-Key




                      Die meisten Funktionalitäten können – zusätzlich zum Mausklick – über be-
                      stimmte Tastenkombinationen ausgelöst werden. Auf den Schaltflächen oder
                      Menüleisten ist jeweils ein Buchstabe unterstrichen. Wenn Sie die Taste <Alt>
                      und die Taste für den unterstrichenen Buchstaben gleichzeitig drücken, führt
                      A+W CAD Designer (Bars) die Funktionalität aus.




A+W CAD Designer (Bars) Überblick                                                           A-191
Bedienung von A+W CAD Designer (Bars)                                             Softwarereferenz




                      Radiotaste




                      In einem Rahmen mit Radiotasten kann immer nur eine Radiotaste angewählt
                      werden! In der Abbildung oben ist die Radiotaste Senkrecht angewählt. Kli-
                      cken Sie z. B. nun die Radiotaste Waagerecht an, wird automatisch die Radio-
                      taste Senkrecht abgewählt.


                      Kombobox




                      Wenn Sie in einer Kombobox auf den Pfeil rechts klicken, öffnet sich eine Aus-
                      wahlliste. Wählen Sie aus dieser Liste den gewünschten Eintrag durch Ankli-
                      cken aus. Ihre Auswahl wird in der Anzeige dargestellt.


                      Checkbox




                      Checkboxen dienen zur Auswahl mehrerer Optionen. Sie können durch Ankli-
                      cken einer Checkbox diese aktivieren bzw. deaktivieren (leeres Kästchen). Es
                      können mehrere Checkboxen gleichzeitig aktiviert sein!


                      Register




                      Zur besseren Übersicht teilen Register den Dialog nach unterschiedlichen
                      Themen. Um in ein anderes Register zu wechseln, klicken Sie mit der Maus
                      auf den gewünschten Registerkopf.




A-192                                                        A+W CAD Designer (Bars) Überblick
Softwarereferenz                                        Bedienung von A+W CAD Designer (Bars)




                      Menüleiste/Menüpunkt




                      Auch Pull–Down–Menü–Leiste genannt. Wenn Sie z. B. eine Fassadenanlage
                      erstellen möchten, klicken Sie mit der Maus auf den Menüeintrag Makros, das
                      entsprechende Pull– Down– Menü öffnet sich (siehe Abbildung oben) und hier
                      auf den Menüeintrag Fassadenanlage.


                      Tabellen-/Spaltenüberschrift




                      Durch den Klick auf einen Eintrag im Spaltenkopf ändert sich automatisch die
                      Sortierfolge. Die Tabelle wird beim ersten Klick aufsteigend und beim nächs-
                      ten Klick absteigend sortiert.




A+W CAD Designer (Bars) Überblick                                                          A-193
Bedienung von A+W CAD Designer (Bars)                                               Softwarereferenz




                      Tastaturbefehle
                      Tastaturbefehle sind Tasten oder Tastenkombinationen, mit denen ein Befehl
                      aufgerufen bzw. eine Funktion ausgeführt wird. Tastaturbefehle helfen dem
                      geübten Benutzer schnell zum gewünschten Ergebnis zu gelangen. Nachfol-
                      gend erhalten Sie einen Überblick über die wichtigsten A+W CAD Designer
                      (Bars) Tastaturbefehle:

                      Tastaturbefehl          Erläuterung

                      <Strg> + <N>            Datei Neu

                      <Strg> + <O>            Eine vorhandene Datei öffnen bzw.
                                              laden. Der Dialog Datei öffnen wird
                                              geöffnet.

                      <Strg> + <S>            Datei speichern. Der Dialog Datei
                                              speichern unter ... wird geöffnet.

                      <Strg> + <A>            Alles auswählen

                      <Strg> + <X>            Auswahl ausschneiden und in die
                                              Zwischenablage kopieren

                      <Strg> + <C>            Auswahl in die Zwischenablage kopieren

                      <Strg> + <V>            Auswahl aus der Zwischenablage
                                              einfügen

                      <Strg> + <M>            Auswahl bewegen

                      <Strg> + <R>            Werkzeug: Schneiden auf

                      <Strg> + <T>            Werkzeug: Teilen

                      <Strg> + <F>            Werkzeug: Durchgang ändern


                         Aktive bzw. inaktive Schaltflächen
                         In den verschiedenen Programmdialogen finden Sie aktive und inaktive
                         Schaltflächen vor. Die Schaltflächen werden abhängig von den Eingaben
                         aktiv oder inaktiv!




A-194                                                        A+W CAD Designer (Bars) Überblick
Softwarereferenz                                         Bedienung von A+W CAD Designer (Bars)




                      Programm beenden
                      Es bestehen verschiedene Möglichkeiten A+W CAD Designer (Bars) zu been-
                      den.
                      •   Mausklick auf die Schaltfläche [Schließen] in der rechten oberen Pro-
                          gramm-Fensterecke beendet das Programm.
                      •   Über das Menü Datei > Beenden.

                          Hinweis zum Beenden
                          Wurden Daten geändert bzw. neue Daten erfasst, die noch nicht gesichert
                          wurden, erscheint ein entsprechender Hinweis. Wählen Sie [Ja] um den Di-
                          alog Datei speichern unter... zu aktivieren. Sie können hier die Datei bzw.
                          Ihre Änderungen speichern. Anschließend wird das Programm beendet.
                          Wählen Sie [Nein] um das Programm ohne Speichern der Datei bzw. der
                          Änderungen zu beenden. Wählen Sie [Abbrechen] um den Vorgang Been-
                          den abzubrechen und mit dem Programm weiter zu arbeiten.




A+W CAD Designer (Bars) Überblick                                                             A-195
Übersicht                                                             Softwarereferenz




            Übersicht
            In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
            •   Umgang mit Dateien
            •   Werkzeuge verwenden
            •   Mit Spezialmustern arbeiten
            •   Messen und Zuschnitt
            •   Die Stammdaten
            •   Ansicht
            •   Die Hilfe verwenden

                Dialoge können von unterschiedlichen Stellen aus geöffnet werden
                Bitte beachten Sie, dass Funktionen und Dialoge auf verschiedenen We-
                gen geöffnet werden können. In dieser Anleitung werden die entsprechen-
                den Dialoge nur einmal beschrieben.




A-196                                             A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                               Umgang mit Dateien




                      Umgang mit Dateien
                      Menü Datei öffnen
                      Im Menü Datei befinden sich folgende Programmpunkte:
                      •   Neu:
                          Mit diesen Menüpunkt erstellen Sie eine neue Datei. Befindet sich noch
                          eine Konstruktion auf Ihrer Arbeitsfläche werden Sie gefragt, ob Sie diese
                          speichern möchten. Anschließend wird die Arbeitsfäche geleert.
                      •   Öffnen:
                          Dieser Menüpunkt hat zwei Funktionen. Zum einen können Sie eine Datei
                          öffnen. Es erscheint der Dialog Datei öffnen...
                          Zum anderen öffnen Sie damit Positionen einer Übergabedatei. Es er-
                          scheint der Dialog Auswahl Auftrag/Position.
                           “Übergabedatei importieren” auf Seite A-202
                      •   Speichern:
                          Sie können eine Datei in einem Ordner auf Ihrer Festplatte, an einer Netz-
                          werkadresse, auf einem Datenträger, auf einer CD, auf dem Desktop oder
                          an einem anderen Speicherort speichern. Sie müssen den Zielspeicherort
                          in der Liste Speichern in angeben. Unabhängig vom ausgewählten Spei-
                          cherort ist die Vorgehensweise beim Speichern immer gleich.
                      •   Speichern unter:
                          Wählen Sie diesen Menüpunkt um eine Datei mit dem von Ihnen angege-
                          benen Dateinamen, Format und Speicherort zu speichern. Wenn Sie eine
                          Datei erstmalig speichern, wird automatisch der Dialog Speichern unter an-
                          gezeigt, wenn Sie auf Speichern klicken.
                      •   Importieren:
                          Mit diesem Menüpunkt importieren Sie Dateien, die von übergeordneten
                          Systemen an A+W CAD Designer (Bars) übergeben werden.
                           “Übergabedatei importieren” auf Seite A-202
                      •   Export:
                          Mit diesem Menüpunkt können Sie Daten für verschiedene Maschinen er-
                          zeugen. Bitte beachten Sie, dass dafür Ihr System entsprechend konfigu-
                          riert sein muss.
                      •   Zurück zur Auftragsbearbeitung:
                          Wird A+W CAD Designer (Bars) zusammen mit A+W Business oder A+W
                          Enterprise genutzt, wechselt A+W CAD Designer (Bars) mit diesem Menü-
                          punkt direkt zur Auftragsbearbeitung zurück. Die Daten werden gespei-
                          chert und an das Auftragsbearbeitungssystem übergeben.
                      •   Zurücksetzen der Auftragsbearbeitung:
                          Mit diesem Menüpunkt wechselt A+W CAD Designer (Bars) zurück zur
                          Auftragsbearbeitung. Änderungen werden verworfen.
                      •   Bild exportieren:
                          Mit diesem Menüpunkt exportieren Sie eine Konstruktion als Bild. Der Dia-
                          log Speichern unter wird geöffnet.
                      •   Konstruktion drucken:
                          Wählen Sie diesen Menüpunkt um eine Konstruktion zu drucken. Bitte be-
                          achten Sie, dass der gewünschte Drucker eingerichtet ist.
                           “Drucken” auf Seite A-205
                           “Druckereinrichtung” auf Seite A-207


A+W CAD Designer (Bars) Überblick                                                            A-197
Umgang mit Dateien                                                                  Softwarereferenz




                     •   Übergabedatei drucken:
                         Wählen Sie diesen Menüpunkt um eine vom übergeordneten System über-
                         gebene Datei zu drucken. Bitte beachten Sie, dass der gewünschte Dru-
                         cker eingerichtet ist.
                          “Listendruck” auf Seite A-206
                          “Druckereinrichtung” auf Seite A-207
                     •   Übergabedatei-Liste drucken:
                         Über diesen Menüpunkt drucken Sie die Zuschnitt-Liste. Bitte beachten
                         Sie, dass der gewünschte Drucker eingerichtet ist.
                          “Listendruck” auf Seite A-206
                          “Druckereinrichtung” auf Seite A-207
                     •   Druckereinrichtung:
                         Über diesen Menüpunkt richten Sie Ihre(n) Drucker ein. Bitte beachten Sie,
                         dass dies notwendig ist um drucken zu können.
                          “Druckereinrichtung” auf Seite A-207
                     •   Nachricht senden:
                         Über diesen Menüpunkt versenden Sie die Konstruktion auf der Arbeitsflä-
                         che per Mail.




A-198                                                             A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                               Umgang mit Dateien




                      Neue Scheibe
                      Datei > Neu > Symbol-Schaltfläche Neue Scheibe > Dialog Modell-Erfassung
                      füllen > Schaltfläche [OK] betätigen
                      oder über die Symbol-Schaltfläche




                      oder
                      eine auf der Arbeitsfläche platzierte Scheibe per Doppelklick öffnen




                      Abb. A-60     Eigenschaften Scheibe


                      In diesem Dialog definieren Sie die Eigenschaften der Scheibe. Sie haben da-
                      rüber hinaus die Möglichkeit, Informationen zum Auftrag und zum Kunden zu
                      hinterlegen. Diese Informationen werden Ihnen an entsprechenden Stellen im
                      Programm angezeigt.

                      Erläuterung der Felder

                      X-Position In diesem Feld geben Sie ein, an welcher X-Position die Scheibe
                      anfangen soll.
                      Technische Info: Pflichtfeld, Numerisch

                      Y-Position In diesem Feld geben Sie ein, an welcher Y-Position die Scheibe
                      anfangen soll.
                      Technische Info: Pflichtfeld, Numerisch

                      Ausrichtung Mit diesem Feld haben Sie die Möglichkeit, die Scheibe gedreht
                      darzustellen. Geben Sie die Gradzahl ein, um die die Scheibe gedreht werden
                      soll.
                      Technische Info: Eingabe optional, Numerisch




A+W CAD Designer (Bars) Überblick                                                            A-199
Umgang mit Dateien                                                              Softwarereferenz




                     Ausrichtung Mit diesem Feld haben Sie die Möglichkeit, die Scheibe gedreht
                     darzustellen. Geben Sie die Zahl ein, um die die Scheibe gedreht werden soll.
                     Technische Info: Eingabe optional, Numerisch

                     Rückschnitt Der Rückschnitt ist der Abstand der Sprosse zur Scheibenau-
                     ßenkante. Er beinhaltet die Breite des Rahmens zuzüglich der Versiegelungs-
                     tiefe. Der Rückschnitt wird optisch auf der Scheibe dargestellt und beim
                     Berechnen des Sprossenzuschnitts mit berücksichtigt.
                     Technische Info: Eingabe optional, Numerisch

                     Auftragsnummer In diesem Feld können Sie die Nummer des Auftrags hin-
                     terlegen, zu dem Sie die Sprossen erfassen.
                     Technische Info: Eingabe optional, Alphanumerisch

                     Positionsnummer In diesem Feld können Sie die Nummer der Auftragspo-
                     sition hinterlegen, zu dem Sie die Sprossen erfassen.
                     Technische Info: Eingabe optional, Numerisch

                     Kundenname In diesem Feld können Sie den Namen des Kunden hinterle-
                     gen, zu dem Sie die Sprossen erfassen.
                     Technische Info: Eingabe optional, Alphanumerisch

                     Kundennummer In diesem Feld können Sie die Nummer des Kunden hinter-
                     legen, zu dem Sie die Sprossen erfassen.
                     Technische Info: Eingabe optional, Alphanumerisch

                     Auftragsmenge In diesem Feld geben Sie die Anzahl der Sprossen ein, die
                     Sie für den Auftrag benötigen.
                     Technische Info: Pflichtfeld, Numerisch

                     SZR1 In diesem Feld geben Sie den Scheibenzwischenraum für ein ISO ein.
                     Technische Info: Eingabe optional, Numerisch

                     SZR2 Handelt es sich bei der Scheibe um ein dreifach ISO, erfassen Sie in
                     diesem Feld den zweiten Scheibenzwischenraum.
                     Technische Info: Eingabe optional, Numerisch

                     Gas In diesem Feld geben Sie das Gas ein.
                     Technische Info: Eingabe optional, Numerisch




A-200                                                       A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                               Umgang mit Dateien




                      Erläuterung der Felder im Bereich Extra

                      Eingabefeld In diesem Feld haben Sie die Möglichkeit, einen Text betreffend
                      einer Auswahl zu hinterlegen. Markieren Sie in der darüber liegenden Liste zu-
                      nächst den Eintrag, zu dem Sie einen Text hinterlegen möchten. Anschlie-
                      ßend geben Sie den Text in diesem Eingabefeld ein. Im Falle einer ALCIM-
                      Anbindung, werden diese Felder bei der Übergabe automatisch gefüllt. Wel-
                      che Felder angezeigt und gefüllt werden können, wird in der INI-Datei konfigu-
                      riert. Die vorhandenen Felder werden im Ausdruck platziert.
                      Technische Info: Eingabe optional, Alphanumerisch


                      Weitere Informationen zu Eigenschaften der Scheibe
                       Tutorial, “Neue Konstruktionen” auf Seite A-99




A+W CAD Designer (Bars) Überblick                                                            A-201
Umgang mit Dateien                                                               Softwarereferenz




                     Übergabedatei importieren
                     Datei > Import > Übergabedatei




                     Abb. A-61    Auftrag bzw. Positionen auswählen


                     Dieser Dialog zeigt die Positonen, die von einem übergeordneten System
                     (z. B. A+W Business) an A+W CAD Designer (Bars) übergeben wurden. Sie
                     können sich die Postionen anzeigen lassen und Änderungen vornehmen.

                     Erläuterung der Felder

                     Status Diesem Feld können Sie den Status der Position entnehmen. Folgen-
                     de Stati sind möglich:
                     - Nacherfassung: Der Datensatz ist nicht oder noch nicht fertig. Er kann noch
                     nicht gedruckt werden.
                     - Konstruiert: Der Datensatz ist fertig und kann ohne Bearbeiung gedruckt wer-
                     den.
                     - Bereit zum Drucken: Der Datensatz wurde mit A+W CAD Designer (Bars) be-
                     arbeitet und ist bereit zum Drucken.
                     - Gedruckt: Die Sprossenskizze wurde gedruckt.
                     - Exportiert: Der Maschinentreiber wurde exportiert.
                     - Abgleich: Betrifft Fassadenanlagen. Die Scheiben einer Fassadenanlage
                     werden im übergeordneten Auftragsbearbeitungssystem als einzelne Positio-
                     nen erfasst. Um die Fassadenanlage in A+W CAD Designer (Bars) kombiniert
                     bearbeiten zu können, wird die Hauptscheibe gekennzeichnet, mit der bei
                     Fassaden abgeglichen wird.

                     Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                     Position In diesem Feld sehen Sie die Positionsnummer.

                     Laufnummer In diesem Feld wird Ihnen (falls vorhanden) die Laufnummer
                     angezeigt.


A-202                                                        A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                              Umgang mit Dateien




                      Scheibe In diesem Feld wird Ihnen die Abmessung der Scheibe(n) ange-
                      zeigt. Befindet sich hinter der Abmessung eine eckige Klammer, wird Ihnen in
                      dieser die Modellnummer angezeigt. Bsp.: [#=3] bedeutet, es handelt sich um
                      Modell Nummer 3. Die Definition der Werte ist kundenindividuell.

                      Auftragsmenge In diesem Feld sehen Sie, wie viele Stück von dieser Posi-
                      tion bestellt sind.

                      Erläuterung der Schaltflächen

                      Abgleich Wenn Sie diese Schaltfläche betätigen, können Sie eine Überga-
                      bepostion nach der anderen auf der Arbeitsfläche als Fassade platzieren. Sie
                      werden ab der zweiten Position nach den entsprechenden Referenzpunkten
                      gefragt. Siehe auch Dialog Neue Scheibenposition.

                      OK Wenn Sie diese Schaltfläche betätigen, wird die gewählte Position auf der
                      Arbeitsfläche platziert.

                      Abbrechen Wenn Sie die Schaltfläche betätigen, schließen Sie den Dialog.


                      Weitere Informationen zum Importieren von Übergabedateien
                       Tutorial, “Datenimport” auf Seite A-166




A+W CAD Designer (Bars) Überblick                                                          A-203
Umgang mit Dateien                                                                 Softwarereferenz




                     Neue Scheibenposition
                     Datei > Import > Übergabedatei > Abgleich > ab zweiter Position




                                                                            B




                     A




                     Abb. A-62    Neue Scheibenposition...


                     Dieser Dialog dient dazu, Positionen im A+W CAD Designer (Bars) zu einer
                     Fassade zusammenzufassen. Er erscheint, wenn Sie im Dialog Auswahl-Auf-
                     trag/Position eine Position markieren und anschließend die Schaltfläche [Ab-
                     gleich] betätigen. Um die Position korrekt zu platzieren, werden Sie zur
                     Angabe der Bezugspunkte aufgefordert.
                     A symbolisiert die zuletzt eingegebene Scheibe. Wählen Sie mit der Maus die
                     Ecke, die als Bezugspunkt dienen soll. B symbolisiert die Scheibe, die Sie jetzt
                     platzieren. Wählen Sie auch hier mit der Maus die Ecke aus, die als Bezugs-
                     punkt dienen soll. Über die Felder X und Y können Sie die entsprechenden
                     Abstände festlegen.

                     Weitere Informationen zum Importieren von Übergabedateien
                      Tutorial, “Datenimport” auf Seite A-166




A-204                                                            A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                               Umgang mit Dateien




                      Drucken
                      Datei > Drucken > Konstruktion




                      Abb. A-63     Drucken


                      Mit diesem Dialog können Sie Konstruktionen drucken. Sie können alle Schei-
                      ben, einzelne Scheiben oder auch einen aktuellen Ausschnitt drucken.

                      Erläuterung der Felder

                      Alle Scheiben Ist diese Radiotaste aktiviert, werden alle Scheiben, die sich
                      auf der Arbeitsfläche befinden, gedruckt.

                      Einzelne Scheiben Befinden sich mehrere Scheiben auf der Arbeitsfläche,
                      können Sie über diese Radiotaste bestimmen, welche der Scheiben gedruckt
                      werden soll. Aktivieren Sie die Radiotaste und geben Sie im Feld dahinter ein,
                      welche Scheibe gedruckt werden soll.

                      Aktueller Ausschnitt Ist diese Radiotaste aktiviert, wird ein zuvor festgeleg-
                      ter Aussschnitt gedruckt.


                      Weitere Informationen zum Drucken
                       Tutorial, “Datenexport” auf Seite A-169




A+W CAD Designer (Bars) Überblick                                                            A-205
Umgang mit Dateien                                                                 Softwarereferenz




                     Listendruck
                     Datei > Drucken > Übergabedatei
                     Datei > Drucken > Übergabedatei-Liste




                     Abb. A-64    Listendruck


                     Mit diesem Dialog können Sie die einzelnen Positionen einer Übergabedatei
                     drucken. Es gibt zwei unterschiedliche Druck-Varianten:
                     •   Übergabedatei
                         Wählen Sie diesen Menüpunkt, erhalten Sie einen Ausdruck, der im obe-
                         ren Bereich eine Liste mit Informationen zum Auftrag (Auftragsnummer,
                         Position, Kunde, etc.) und Artikel (Sprosse, Farbe, etc.) zeigt und im unte-
                         ren Bereich die Skizze.
                     •   Übergabedatei - Liste
                         Wählen Sie diesen Menüpunkt, erhalten Sie einen Ausdruck der Zuschnitt-
                         Liste mit Informationen zu Auftrag und Position sowie zum Zuschnitt der
                         Sprosse(n).

                     Erläuterung der Felder

                     Status Diesem Feld können Sie den Status der Position entnehmen. Folgen-
                     de Stati sind möglich:
                     - Nacherfassung: Der Datensatz ist nicht oder noch nicht fertig. Er kann noch
                     nicht gedruckt werden.
                     - Konstruiert: Der Datensatz ist fertig und kann ohne Bearbeiung gedruckt wer-
                     den.
                     - Bereit zum Drucken: Der Datensatz wurde mit A+W CAD Designer (Bars) be-
                     arbeitet und ist bereit zum Drucken.
                     - Gedruckt: Die Sprossenskizze wurde gedruckt.
                     - Exportiert: Der Maschinentreiber wurde exportiert.
                     - Abgleich: Betrifft Fassadenanlagen. Die Scheiben einer Fassadenanlage
                     werden im übergeordneten Auftragsbearbeitungssystem als einzelne Positio-
                     nen erfasst. Um die Fassadenanlage in A+W CAD Designer (Bars) kombiniert

A-206                                                         A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                              Umgang mit Dateien




                      bearbeiten zu können, wird die Hauptscheibe gekennzeichnet, mit der bei
                      Fassaden abgegelichen wird.

                      Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                      Position In diesem Feld sehen Sie die Positionsnummer.

                      Laufnummer In diesem Feld wird Ihnen (falls vorhanden) die Laufnummer
                      angezeigt.

                      Scheibe In diesem Feld wird Ihnen die Abmessung der Scheibe(n) ange-
                      zeigt. Befindet sich hinter der Abmessung eine eckige Klammer, wird Ihnen in
                      dieser die Gasnummer angezeigt. Bsp.: [#=3] bedeutet, es handelt sich um
                      Modell Nummer 3. Die Definition der Werte ist kundenindividuell.

                      Auftragsmenge In diesem Feld sehen Sie, wie viele Stück von dieser Posi-
                      tion bestellt sind.


                      Weitere Informationen zur Übergabedateien
                       Tutorial, “Übergabedatei drucken” auf Seite A-171



                      Druckereinrichtung
                      Datei > Drucken > Druckereinrichtung




                      Abb. A-65     Druckereinrichtung


                      In diesem Dialog nehmen Sie die Einstellungen zum Drucken vor. Sie können
                      zwei unterschiedliche Drucker angeben. Sollten Sie mit einem Plotter arbei-
                      ten, wird dieser unter Drucker 2 geführt.




A+W CAD Designer (Bars) Überblick                                                          A-207
Umgang mit Dateien                                                                  Softwarereferenz




                     Erläuterung der Felder im Bereich

                     Drucker 1 In diesem Feld definieren Sie den Standard-Drucker. Über die
                     Schaltfläche [Ändern...] können Sie einen anderen Drucker auswählen.

                     Erläuterung der Felder im Bereich Drucker 2

                     Drucker 2 In diesem Feld können Sie einen zweiten Drucker definieren. Ar-
                     bieten Sie in Ihrem Hause mit einem Plotter, wird dieser hier definiert. Über die
                     Schaltfläche [Ändern...] können Sie einen anderen Drucker auswählen.

                     Alles Dieses Feld steht in Zusammenhang mit dem Feld Drucker 2. Ist in die-
                     sem Feld ein Drucker angegeben, dann können Sie mit dieser Radiotaste fest-
                     legen, was auf dem Drucker 2 ausgegeben werden soll. Aktivieren Sie diese
                     Radiotaste, wird alles auf Drucker 2 ausgegeben.

                     Freie Sprossen Dieses Feld steht in Zusammenhang mit dem Feld Drucker
                     2. Ist in diesem Feld ein Drucker angegeben, dann können Sie mit dieser Ra-
                     diotaste festlegen, was auf dem Drucker 2 ausgegeben werden soll. Aktivie-
                     ren Sie diese Radiotaste, werden Scheiben mit Sprossen die nicht
                     waagerecht oder senkrecht laufen auf Drucker 2 ausgegeben.

                     Bögen Dieses Feld steht in Zusammenhang mit dem Feld Drucker 2. Ist in
                     diesem Feld ein Drucker angegeben, dann können Sie mit dieser Radiotaste
                     festlegen, was auf dem Drucker 2 ausgegeben werden soll. Aktivieren Sie die-
                     se Radiotaste, werden Scheiben mit gebogenen Sprossen auf Drucker 2 aus-
                     gegeben.

                     Ausschnitt Dieses Feld steht in Zusammenhang mit dem Feld Drucker 2. Ist
                     in diesem Feld ein Drucker angegeben, dann können Sie mit dieser Radiotas-
                     te festlegen, was auf dem Drucker 2 ausgegeben werden soll. Aktivieren Sie
                     diese Radiotaste, werden Ausschnitte auf Drucker 2 ausgegeben.

                     Form Dieses Feld steht in Zusammenhang mit dem Feld Drucker 2. Ist in die-
                     sem Feld ein Drucker angegeben, dann können Sie mit dieser Radiotaste fest-
                     legen, was auf dem Drucker 2 ausgegeben werden soll. Aktivieren Sie diese
                     Radiotaste, werden Modelle der Modell-Nr. > 0 auf Drucker 2 ausgegeben.

                     Maximale Größe Ist diese Radiotaste aktiviert, wird die Ausgabe der Papier-
                     größe des Druckers angepasst.

                     1 : 1 Ist diese Radiotaste aktiviert, erfolgt die Ausgabe 1 : Papiergröße des
                     Druckers.

                     Anzahl Mit diesem Feld legen Sie die Anzahl der Exemplare fest, die ge-
                     druckt werden soll. Über die Pfeiltasten können Sie die Anzahl erhöhen oder
                     reduzieren.




A-208                                                         A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                 Umgang mit Dateien




                      Sortierung Dieser Bereich regelt die Sortierung und wird erst aktiv, wenn die
                      Anzahl der Ausdrucke größer 1 ist. Mögliche Werte:
                      - [1][1]...[2][2]: Es werden erst alle ersten Seiten, dann alle zweiten Seiten,
                      usw. gedruckt. D. h. es erfolgt keine Sortiertung.
                      - [1][2]...[1][2]: Es wird erst die erste Seite, dann die zweite Seiten, usw. ge-
                      druckt. D. h. hier erfolgt eine Sortiertung.


                      Weitere Informationen zur Druckereinrichtung
                       Tutorial, “Drucker einrichten” auf Seite A-169




A+W CAD Designer (Bars) Überblick                                                               A-209
Werkzeuge verwenden                                                                   Softwarereferenz




                      Werkzeuge verwenden
                      Menü Bearbeiten öffnen
                      Im Menü Bearbeiten befinden sich folgende Menüpunkte:
                      •   Rückgängig:
                          In A+W CAD Designer (Bars) können Sie die zuletzt ausgeführten Aktio-
                          nen rückgängig machen. Für diese Funktion steht auch eine Symbol-
                          Schaltfläche zur Verfügung.
                      •   Wiederholen:
                          Wählen Sie diesen Menüpunkt, wenn Sie eine Aktion wiederherstellen
                          möchten, die Sie zuvor rückgängig gemacht haben. Für diese Funktion
                          steht auch eine Symbol-Schaltfläche zur Verfügung.
                      •   Fangpunkte:
                          Unter diesem Menüpunkt finden Sie die Fangpunkte, die für Ihre Arbeit mit
                          A+W CAD Designer (Bars) notwendig sein können. Für diese Funktionen
                          stehen auch Symbol-Schaltflächen zur Verfügung. Die Fangpunkte wer-
                          den an folgender Stelle ausführlich erläutert:
                           Tutorial, “Das Arbeiten mit Fangpunkten” auf Seite A-22
                      •   Einschränkungen:
                          In diesem Menüpunkt befinden sich die Werkzeuge zum Platzieren von ho-
                          rizontalen und vertikalen Sprossen sowie von Sprossen unter festen und
                          freiem Winkel. Für diese Funktionen stehen auch Symbol-Schaltflächen
                          zur Verfügung. Die Werkzeuge werden an folgender Stelle ausführlich er-
                          läutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Auswählen:
                          Mit diesem Menüpunkt wählen Sie ein Element aus. Für diese Funktion
                          steht auch eine Symbol-Schaltfläche zur Verfügung. Das Werkzeug wird
                          an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Alles auswählen:
                          Mit diesem Menüpunkt wählen Sie alle Elemente aus, die sich auf der Ar-
                          beitsfläche befinden.
                      •   Entfernen:
                          Mit diesem Menüpunkt löschen Sie ein gewähltes Element.
                      •   Hinzufügen:
                          In diesem Menüpunkt befinden sich die Werkzeuge zum Hinzufügen von
                          Scheiben, geraden Sprossen, Bogensprossen und Kreissprossen sowie
                          von Sonne, Mond und Bogen. Für diese Funktionen stehen auch Symbol-
                          Schaltflächen zur Verfügung. Die Werkzeuge werden an folgender Stelle
                          ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Kopieren:
                          Mit diesem Menüpunkt kopieren Sie eine gewählte Sprosse.
                      •   Drehen:
                          Mit diesem Menüpunkt duplizieren und drehen Sie eine gewählte Sprosse.
                          Das Werkzeuge wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40




A-210                                                           A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                 Werkzeuge verwenden




                      •   Spiegeln:
                          Mit diesem Menüpunkt spiegeln Sie eine gewählte Sprosse. Das Werkzeu-
                          ge wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Bewegen:
                          Mit diesem Menüpunkt bewegen Sie eine gewählte Sprosse. Das Werk-
                          zeug wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Artikel ändern:
                          Mit diesem Porgrammpunkt tauschen Sie eine gewählte Sprosse gegen
                          eine Andere aus.
                      •   Schneiden auf:
                          Mit diesem Menüpunkt verlängern Sie eine gewählte Sprosse auf ein Ob-
                          jekt. Das Werkzeug wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Teilen:
                          Mit diesem Menüpunkt teilen Sie alle Sprossen. Das Werkzeug wird an fol-
                          gender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40
                      •   Durchgang ändern:
                          Mit diesem Menüpunkt ändern Sie für eine 90° Kreuzung die Durchgangs-
                          richtung. Das Werkzeug wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Werkzeuge verwenden” auf Seite A-40




A+W CAD Designer (Bars) Überblick                                                             A-211
Mit Spezialmustern arbeiten                                                             Softwarereferenz




                        Mit Spezialmustern arbeiten
                        Menü Makro öffnen
                        Im Menü Makro befinden sich folgende Menüpunkte:
                        •     SW-Muster:
                              Über diesen Menüpunkt platzieren Sie senkrechte und/oder waagerechte
                              Sprossen auf der Scheibe.
                               “Muster Senkrecht-Waagerecht” auf Seite A-213
                        •     Sondermuster
                              Über diesen Menüpunkt platzieren Sie ein Sondermuster auf der Scheibe.
                               “Rautenmuster...” auf Seite A-220
                        •     Fassadenanlage
                              Über diesen Menüpunkt erstellen Sie eine Fassadenanlage auf der Schei-
                              be.
                               “Fassadenanlage...” auf Seite A-222
                        •     Strahlenmuster
                              Über diesen Menüpunkt erstellen Sie ein Strahlenmuster auf der Scheibe.
                               “Sonne und Sterne” auf Seite A-223
                        •     Freies Muster
                              Über diesen Menüpunkt platzieren Sie ein Makro auf der Scheibe.
                               “Makro auswählen” auf Seite A-225
                        •     Neues Makro
                              Über diesen Menüpunkt können Sie eigene Makros erstellen.




A-212                                                                 A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                      Mit Spezialmustern arbeiten




                      Muster Senkrecht-Waagerecht
                      Makro > SW Muster> Mit Maus auf Scheibe klicken
                      oder über die Symbol-Schaltfläche




                      Abb. A-66     Muster Senkrecht-Waagerecht


                      In diesem Dialog nehmen Sie die Einstellungen für das Sprossenmuster vor.
                      Die Sprossenmuster ersparen Ihnen die Arbeit, jede Sprosse einzeln einzuge-
                      ben. Darüber hinaus können Sie über spezielle Einstellungen Sprossen auto-
                      matisch platzieren.

                      Erläuterung der Felder im Bereich Anzahl Sprossen

                      Anzahl waagerecht In diesem Feld geben Sie die Anzahl der waagerechten
                      Sprossen ein. Beispiel: Eingabe 3 bedeutet, es werden drei waagerechte
                      Sprossen eingefügt.
                      Technische Info: Pflichtfeld, Eingabe, numerisch

                      Anzahl senkrecht In diesem Feld geben Sie die Anzahl der senkrechten
                      Sprossen ein. Beispiel: Eingabe 5 bedeutet, es werden fünf senkrechte Spros-
                      sen eingefügt.
                      Technische Info: Pflichtfeld, Eingabe, numerisch




A+W CAD Designer (Bars) Überblick                                                          A-213
Mit Spezialmustern arbeiten                                                      Softwarereferenz




                        Erläuterung der Felder im Bereich Teilung Waagerecht

                        Gleiche lichte Felder Wenn Sie diese Radiotaste aktivieren, platziert A+W
                        CAD Designer (Bars) die Anzahl der waagerechten Sprossen so, dass alle
                        waagerechten Felder gleich groß sind.
                        Technische Info: Optional, Auswahl

                        Gleicher Bohrpunktabstand Wenn Sie diese Radiotaste aktivieren, plat-
                        ziert A+W CAD Designer (Bars) die Anzahl der waagerechten Sprossen so,
                        dass die Abstände der Bohrpunkte vom Rahmen aus gleich sind. Das kann
                        dazu führen, dass das innen liegende Feld kleiner wird.
                        Technische Info: Optional, Auswahl

                        Gleicher Bohrpkt. (Scheibe) Wenn Sie diese Radiotaste aktivieren, plat-
                        ziert A+W CAD Designer (Bars) die Anzahl der waagerechten Sprossen so,
                        dass die Abstände der Bohrpunkte auf der Scheibe gleich sind.
                        Technische Info: Optional, Auswahl

                        Gleicher Sprossenlänge Wenn Sie diese Radiotaste aktivieren, platziert
                        A+W CAD Designer (Bars) die Anzahl der waagerechten Sprossen so, dass
                        alle Sprossen die gleiche Länge haben.
                        Technische Info: Optional, Auswahl

                        Kundendefiniert Wenn Sie diese Radiotaste aktivieren, öffnet sich der Dia-
                        log Kundenvorgabe SW-Muster (nach Betätigen der Schaltfläche [OK]).
                        Technische Info: Optional, Auswahl

                        Erläuterung der Felder im Bereich Durchgängige Sprossen

                        Senkrechte Wenn Sie diese Checkbox aktivieren, werden alle senkrechten
                        Sprossen, die Sie einfügen, durchgängig sein.
                        Technische Info: Optional, Auswahl

                        Waagerechte Wenn Sie diese Checkbox aktivieren, werden alle waagerech-
                        ten Sprossen, die Sie einfügen, durchgängig sein.
                        Technische Info: Optional, Auswahl

                        Erläuterung der Felder im Bereich Scheiben

                        Übertrag auf alle Scheiben Diese Checkbox ist nur aktiv, wenn es sich um
                        eine Fassadenanlage mit Sprossen handelt. Dann können Sie das Sprossen-
                        muster auf alle Scheiben übertragen.
                        Technische Info: Optional, Auswahl

                        Sprossen fortsetzen Diese Checkbox ist nur aktiv, wenn es sich um eine
                        Fassadenanlage mit Sprossen handelt. Dann können Sie die Sprossen quasi
                        weiter laufen.
                        Technische Info: Optional, Auswahl




A-214                                                         A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                         Mit Spezialmustern arbeiten




                      Erläuterung der Felder im Bereich Teilung Senkrecht

                      Gleiche lichte Felder Wenn Sie diese Radiotaste aktivieren, platziert A+W
                      CAD Designer (Bars) die Anzahl der senkrechten Sprossen so, dass alle
                      senkrechten Felder gleich groß sind.
                      Technische Info: Optional, Auswahl

                      Gleicher Bohrpunktabstand Wenn Sie diese Radiotaste aktivieren, plat-
                      ziert A+W CAD Designer (Bars) die Anzahl der senkrechten Sprossen so,
                      dass die Abstände der Bohrpunkte vom Rahmen aus gleich sind. Das kann
                      dazu führen, dass das innen liegende Feld kleiner wird.
                      Technische Info: Optional, Auswahl

                      Gleicher Bohrpkt. (Scheibe) Wenn Sie diese Radiotaste aktivieren, plat-
                      ziert A+W CAD Designer (Bars) die Anzahl der senkrechten Sprossen so,
                      dass die Abstände der Bohrpunkte auf der Scheibe gleich sind.
                      Technische Info: Optional, Auswahl

                      Gleicher Sprossenlänge Wenn Sie diese Radiotaste aktivieren, platziert
                      A+W CAD Designer (Bars) die Anzahl der senkrechten Sprossen so, dass alle
                      Sprossen die gleiche Länge haben.
                      Technische Info: Optional, Auswahl

                      Kundendefiniert Wenn Sie diese Radiotaste aktivieren, öffnet sich der Dia-
                      log Kundenvorgabe SW-Muster (nach Betätigen der Schaltfläche [OK]).
                      Technische Info: Optional, Auswahl


                      Weitere Informationen zu Muster Senkrecht-Waagerecht
                       Tutorial, “Neue Konstruktionen” auf Seite A-99
                       “Kundenvorgabe SW-Muster” auf Seite A-216




A+W CAD Designer (Bars) Überblick                                                            A-215
Mit Spezialmustern arbeiten                                                         Softwarereferenz




                        Kundenvorgabe SW-Muster
                        Makro > SW Muster> Mit Maus auf Scheibe klicken > Radiotaste Kundendefi-
                        niert aktivieren > Schaltfläche [OK] betätigen
                        oder über die Symbol-Schaltfläche




                        Abb. A-67   Kundenvorgabe SW-Muster


                        In diesem Dialog nehmen Sie die kundenspezifische Einstellungen für das
                        Sprossenmuster vor. Im unteren Bereich des Dialogs wird Ihnen die Auftrags-
                        und Positionsnummer angezeigt.

                        Erläuterung der Felder im Bereich Waagerechte Sprossen

                        Scheibenrand Aktivieren Sie diese Radiotaste, wenn der Bezugspunkt für
                        die Sprossen der Scheibenrand ist. Die Zahl hinter dem Feld zeigt Ihnen die
                        Anzahl der waagerechten Sprossen an, die Sie im Dialog Muster Senkrecht-
                        Waagerecht eingegeben haben.
                        Technische Info: Optional, Auswahl

                        Rahmeninnenkante Aktivieren Sie diese Radiotaste, wenn der Bezugspunkt
                        für die Sprossen die Rahmeninnenkante ist.
                        Technische Info: Optional, Auswahl

                        Lichte Felder Aktivieren Sie diese Radiotaste, wenn Sie gleiche lichte Felder
                        wünschen.
                        Technische Info: Optional, Auswahl




A-216                                                          A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                       Mit Spezialmustern arbeiten




                      Aufsummieren Die Checkbox ist nur in Verbindung mit den Radiotasten
                      Scheibenrand und Rahmeninnenkante aktiv.
                      Technische Info: Optional, Auswahl

                      Von oben Über diese Radiotaste steuern Sie, dass die Sprossen von oben
                      nach unten eingefügt werden.
                      Technische Info: Optional, Auswahl

                      Von unten Über diese Radiotaste steuern Sie, dass die Sprossen von unten
                      nach oben eingefügt werden.
                      Technische Info: Optional, Auswahl

                      Erläuterung der Felder im Bereich Senkrechte Sprossen

                      Scheibenrand Aktivieren Sie diese Radiotaste, wenn der Bezugspunkt für
                      die Sprossen der Scheibenrand ist. Die Zahl hinter dem Feld zeigt Ihnen die
                      Anzahl der waagerechten Sprossen an, die Sie im Dialog Muster Senkrecht-
                      Waagerecht eingegeben haben.
                      Technische Info: Optional, Auswahl

                      Rahmeninnenkante Aktivieren Sie diese Radiotaste, wenn der Bezugspunkt
                      für die Sprossen die Rahmeninnenkante ist.
                      Technische Info: Optional, Auswahl

                      Lichte Felder Aktivieren Sie diese Radiotaste, wenn Sie gleiche lichte Felder
                      wünschen.
                      Technische Info: Optional, Auswahl

                      Aufsummieren Die Checkbox ist nur in Verbindung mit den Radiotasten
                      Scheibenrand und Rahmeninnenkante aktiv. Eingegebene Werte werden ad-
                      diert. Bsp.: Sie geben für zwei waagerechte Sprossen jeweils 100 mm ein und
                      aktivieren diese Checkbox. Dann platziert A+W CAD Designer (Bars) die erste
                      Sprosse im Abstand von 100 mm je nach Auswahl zum Scheibenrand/Rah-
                      meninnenkante und die nächste Sprosse weitere 100 mm von der ersten
                      Sprosse entfernt.
                      Technische Info: Optional, Auswahl

                      Von rechts Über diese Radiotaste steuern Sie, dass die Sprossen von rechts
                      nach links eingefügt werden.
                      Technische Info: Optional, Auswahl

                      Von links Über diese Radiotaste steuern Sie, dass die Sprossen von links
                      nach rechts eingefügt werden.
                      Technische Info: Optional, Auswahl




A+W CAD Designer (Bars) Überblick                                                           A-217
Mit Spezialmustern arbeiten                                                       Softwarereferenz




                        Erläuterung der Schaltflächen

                        Hinzufügen Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog
                        Eingabe Sprossen-Abstände. Über diese Schaltfläche fügen Sie sowohl waa-
                        gerechte als auch senkrechte Sprossen ein. Bitte denken Sie daran, vorher
                        die entsprechende Auswahl in den Bereichen Waagerechte Sprossen bzw.
                        Senkrechte Sprossen zu treffen.

                        Entfernen Wenn Sie diese Schaltfläche betätigen, wird der in der Liste mar-
                        kierte Eintrag gelöscht.

                        Ändern Wenn Sie diese Schaltfläche betätigen, können Sie Änderungen an
                        dem in der Liste markierten Eintrag vornehmen.


                        Weitere Informationen zur Kundenvorgabe SW-Muster
                         Tutorial, “Neue Konstruktionen” auf Seite A-99
                         “Muster Senkrecht-Waagerecht” auf Seite A-213




A-218                                                           A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                         Mit Spezialmustern arbeiten




                      Eingabe Sprossen-Abstände
                      Makro > SW Muster> Mit Maus auf Scheibe klicken > Radiotaste Kundendefi-
                      niert aktivieren > Schaltfläche [OK] betätigen > Schaltfläche [Hinzufügen] be-
                      tätigen
                      oder über die Symbol-Schaltfläche




                      Abb. A-68     Eingabe Sprossenabstände


                      Über diesen Dialog können Sie die Sprossen durch Eingabe von Abständen
                      platzieren.

                      Erläuterung der Felder im Bereich Waagerechte Sprossen

                      Abstand In diesem Feld geben Sie den Abstand der Sprossen zueinander
                      ein. Beispiel: Eingabe 50 bedeutet, nach 50 mm wird eine Sprosse eingefügt.
                      Über die Felder Scheibenrand und Rahmeninnenkante können Sie den Bezug
                      festlegen.
                      Technische Info: Pflichtfeld, Eingabe, numerisch


                      Weitere Informationen zur Kundenvorgabe SW-Muster
                       Tutorial, “Neue Konstruktionen” auf Seite A-99
                       “Kundenvorgabe SW-Muster” auf Seite A-216




A+W CAD Designer (Bars) Überblick                                                            A-219
Mit Spezialmustern arbeiten                                                        Softwarereferenz




                        Rautenmuster...
                        Makro > Spezial Muster > Sondermuster




                        Abb. A-69   Rautenmuster


                        In diesem Dialog haben Sie die Möglichkeit, Rauten oder Rechtecke automa-
                        tisch auf der Scheibe zu platzieren. Mit den Feldern Breite und Höhe bestim-
                        men Sie die Abmessungen der Rauten bzw. der Rechtecke. A+W CAD
                        Designer (Bars) errechnet dann, wie viele Rauten oder Rechtecke auf der
                        Scheibe Platz haben und positioniert sie dem entsprechend.

                        Erläuterung der Felder im Bereich Muster

                        Rauten Ist diese Radiotaste aktiviert, werden Rauten auf der Scheibe plat-
                        ziert.

                        Rechteck Ist diese Radiotaste aktiviert, werden Rechtecke auf der Scheibe
                        platziert.

                        Erläuterung der Felder im Bereich Rechteck

                        Breite In diesem Feld geben Sie an, wie breit die Raute oder das Rechteck
                        sein soll.

                        Höhe In diesem Feld geben Sie an, wie hoch die Raute oder das Rechteck
                        sein soll.

                        Übertrag auf alle Scheiben Das Feld ist nur aktiv, wenn sich mehrere Schei-
                        ben auf der Arbeitsfläche befinden. Dann haben Sie die Möglichkeit, durch Ak-
                        tivierung dieser Checkbox das Muster auf allen Scheiben zu platzieren.




A-220                                                          A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                             Mit Spezialmustern arbeiten




                      Rauten-/Rechtecksymmetrisch Abhängig von der Auswahl, die Sie im Be-
                      reich Muster treffen, erscheinen folgende Einträge:
                      Bei Auswahl Raute erscheint Rautensymmetrisch.
                      Bei Auswahl Rechteck erscheint Rechtecksymmetrisch.
                      Ist die entsprechende Radiotaste aktiviert, erfolgt die Aufteilung Rauten- bzw.
                      Rechtecksymmetrisch.

                      Sprossensymmetrisch Ist diese Radiotaste aktiv, erfolgt die Aufteilung der
                      Rauten bzw. Rechtecke sprossensymmetrisch.


                      Weitere Informationen zum Rautenmuster
                       Tutorial, “Sondermuster erstellen” auf Seite A-128




A+W CAD Designer (Bars) Überblick                                                                A-221
Mit Spezialmustern arbeiten                                                        Softwarereferenz




                        Fassadenanlage...
                        Makro > Spezial Muster > Fassadenanlage




                        Abb. A-70    Fassadenanlage


                        Mit diesem Dialog haben Sie die Möglichkeit bis zu vier Scheiben von Modell
                        Nr. 0 gleichzeitig zu erfassen und auf der Arbeitsfläche zu platzieren.

                        Erläuterung der Felder

                        Breite In diesen Feldern geben Sie die Breite für die einzelnen Scheiben ein.

                        Höhe In diesen Feldern geben Sie die Höhe für die einzelnen Scheiben ein.

                        Abstände Diese beiden Felder werden von A+W CAD Designer (Bars) auto-
                        matisch gefüllt, wenn Sie die Breiten und Höhen der einzelnen Scheiben ein-
                        gegeben haben. Sie können die Werte aber auch überschreiben.


                        Weitere Informationen zur Fassadenanlage
                         Tutorial, “Fassaden” auf Seite A-130




A-222                                                            A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                       Mit Spezialmustern arbeiten




                      Sonne und Sterne
                      Makro > Strahlenmuster
                      oder über die Symbol-Schaltfläche




                      Abb. A-71     Sonne und Sterne


                      Mit diesem Dialog können Sie die Strahlen einer Sonne in einem lichten Feld
                      platzieren.

                      Erläuterung der Felder

                      Stern Wenn Sie den Dialog öffnen, ist diese Radiotaste automatisch aktiviert.
                      Es handelt sich um die Strahlen der Sonne in Form von einem Stern.

                      Gemeinsamer Zuschnitt Diese Checkbox bezieht sich auf den Zuschnitt der
                      Sprossen am Anfang. Mögliche Werte:
                      ☐ Ist die Checkbox deaktiviert, werden die Sprossen nebeneinander platziert.
                      ☑ Ist die Checkbox aktiviert, werden die Sprossen gebündelt.

                      Gleiche Winkel Wenn Sie diese Checkbox aktivieren, berechnet A+W CAD
                      Designer (Bars) die Platzierung der Winkel in Abhängigkeit von der Anzahl der
                      Winkel und der Scheibengröße.

                      Strahlen in die Ecke Wenn Sie diese Checkbox aktivieren, werden die bei-
                      den äußeren Strahlen in den Ecken platziert. Darüber hinaus müssen Sie
                      noch angeben, wie der Zuschnitt erfolgen soll (Kombobox Zuschnittmethode).




A+W CAD Designer (Bars) Überblick                                                           A-223
Mit Spezialmustern arbeiten                                                              Softwarereferenz




                        Zuschnittmethode Die Kombobox ist nur aktiv, wenn Sie die Checkbox
                        Strahlen in die Ecke aktiviert haben. In diesem Fall müssen Sie hier auswäh-
                        len, wie der Zuschnitt erfolgen soll. Mögliche Werte:
                        - Zuschnitt auf senkrechten Rahmen
                        - Zuschnitt in Ecke
                        - Zuschnitt auf waagerechten Rahmen

                        Anzahl der Strahlen Wählen Sie aus der Kombobox die Anzahl der Strahlen
                        aus. Mögliche Werte:
                        - 2: Die Sonne hat zwei Strahlen
                        - 3: Die Sonne hat drei Strahlen
                        - 4: Die Sonne hat vier Strahlen
                        - 5: Die Sonne hat fünf Strahlen


                        Weitere Informationen zu Sonne und Sternen
                         Tutorial, “Erzeugt eine Sonne in einem lichten Feld” auf Seite A-51




A-224                                                              A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                            Mit Spezialmustern arbeiten




                      Makro auswählen
                      Makro > Freies Muster > Scheibe anklicken
                      oder über die Symbol-Schaltfläche




                      Abb. A-72     Makro auswählen


                      A+W CAD Designer (Bars) wird bereits mit einer Reihe von fertigen Makros
                      ausgeliefert. In diesem Dialog wählen Sie auf der linken Seite das gewünschte
                      Makro aus. Auf der rechten Seite erhalten Sie eine Vorschau des Makros so-
                      wie eine Erläuterung. haben Sie die Möglichkeit, vier Scheiben von Modell Nr.
                      0 gleichzeitig zu erfassen und auf der Arbeitsfläche zu platzieren.

                      Erläuterung der Felder

                      Breite In diesen Feldern geben Sie die Breite für die einzelnen Scheiben ein.

                      Höhe In diesen Feldern geben Sie die Höhe für die einzelnen Scheiben ein.

                      Abstände Diese beiden Felder werden von A+W CAD Designer (Bars) auto-
                      matisch gefüllt, wenn Sie die Breiten und Höhen der einzelnen Scheiben ein-
                      gegeben haben. Sie können die Werte aber auch überschreiben.


                      Weitere Informationen zu Makros
                       Tutorial, “” auf Seite A-137
                       Tutorial, “Anhang – Makrokatalog” auf Seite A-175




A+W CAD Designer (Bars) Überblick                                                               A-225
Mit Spezialmustern arbeiten                                                           Softwarereferenz




                        Makro-Parameter
                        Makro platzieren > [OK]




                        Abb. A-73     Makro-Parameter


                        Bei dem einen oder anderen Makro fordert A+W CAD Designer (Bars) Sie zur
                        Eingabe von Werten auf. Diese Werte sind abhängig vom gewälten Makro.
                        Folgende Werte können abgefragt werden:
                        •     Breite der Raute
                        •     Höhe der Raute
                        •     Halbe Rautenhöhe
                        •     Halbe Rautenbreite
                        •     Abstand vom Rand
                        •     Abstand vom rechten und linken Scheibenrand
                        •     Abstand vom oberen und unteren Scheibenrand
                        •     Abstand zwischen den Sprossen
                        •     Erste Sprosse von der Kante
                        •     Radius
                        •     Abstand vom normalen Rechteck zum Rahmen
                        •     Abstand vom Mittelpunkt
                        Werden Sie zur Eingabe aufgefordert, markieren Sie den Wert, den Sie än-
                        dern möchten und betätigen die Schaltfläche [Ändern...]. Es öffnet sich der Di-
                        alog Relativer Abstand.

                        Weitere Informationen zu Makro-Parametern
                         Tutorial, “Makros” auf Seite A-137
                         Tutorial, “Makro laden” auf Seite A-138




A-226                                                               A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                      Mit Spezialmustern arbeiten




                      Relativer Abstand
                      Makro platzieren > [OK] > [Ändern...]




                      Abb. A-74     Relativer Abstand


                      In diesem Dialog können Sie die Werte, die zur Platzierung eines Makros not-
                      wendig sind, eingeben.
                      Geben Sie den gewünschten Wert ein und schließen Sie den Dialog mit der
                      Schaltfläche [OK].


                      Weitere Informationen zu relativem Abstand
                       Tutorial, “Makros” auf Seite A-137
                       Tutorial, “Makro laden” auf Seite A-138




A+W CAD Designer (Bars) Überblick                                                          A-227
Messen und Zuschnitt                                                               Softwarereferenz




                       Messen und Zuschnitt
                       Menü Info öffnen
                       Im Menü Info befinden sich folgende Menüpunkte:
                       •   Messen:
                           Über diesen Menüpunkt messen Sie Längen oder Abstände.
                            “Abstand” auf Seite A-229
                       •   Zuschnitt-Info
                           Über diesen Menüpunkt erhalten Sie die Zuschnitt-Informationen.
                            “Zuschnitt-Informationen” auf Seite A-230




A-228                                                            A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                              Messen und Zuschnitt




                      Abstand
                      Info > Messen
                      oder über die Symbol-Schaltfläche




                      Abb. A-75     Abstand


                      Dieser Dialog misst die Distanz zwischen zwei Mausklicks. Zunächst wählen
                      Sie das Werkzeug aus:
                      Info > Messen
                      Klicken Sie den Startpunkt der Messstrecke an und anschließend den End-
                      punkt der Messstrecke. Der Dialog Abstand wird automatisch angezeigt.

                         Genaues Messen
                         Um möglichst genau die gewünschten Punkte zu treffen, ist es sinnvoll, zu-
                         vor Fangpunkte auf die Arbeitsfläche zu setzen. Sie können diese Fang-
                         punkte auch einsetzen, um rasch die Information über Längen einzelner
                         Sprossen zu erhalten.


                      Weitere Informationen zum Messen
                       Tutorial, “Abstände oder Längen messen” auf Seite A-126




A+W CAD Designer (Bars) Überblick                                                           A-229
Messen und Zuschnitt                                                                Softwarereferenz




                       Zuschnitt-Informationen
                       Info > Zuschnitt-Info...




                       Abb. A-76     Zuschnitt-Informationen


                       Dieser Dialog liefert Ihnen die Zuschnitt-Informationen zu der aktuellen Spros-
                       senkonstruktion.

                       Erläuterung der Felder

                       Scheibe: Dieses Feld zeigt Ihnen die Nummer der Scheibe. Befinden sich
                       mehrere Scheiben auf der Arbeitsfläche, werden die Scheiben durchnumme-
                       riert.

                       Sprosse: In diesem Feld sehen Sie die Artikelnummer der Sprosse. Dieser
                       Wert kommt aus den Stammdaten.

                       Farbe: In diesem Feld sehen Sie die Farbe der Sprosse. Dieser Wert kommt
                       aus den Stammdaten.

                       Farbe waagr.: Sollten waagerechte und senkrechte Sprossen unterschiedli-
                       che Farben haben, zeigt Ihnen dieses Feld die Farbe der waagerechten
                       Sprosse an. Der Wert kommt aus den Stammdaten.

                       Farbe senkr.: Sollten waagerechte und senkrechte Sprossen unterschiedli-
                       che Farben haben, zeigt Ihnen dieses Feld die Farbe der senkrechten Spros-
                       se an. Der Wert kommt aus den Stammdaten.

                       Materialmenge: In diesem Feld sehen Sie die für die Sprossenkonstruktion
                       benötigte Menge an Material in der jeweils eingestellten Maßeinheit.




A-230                                                          A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                 Messen und Zuschnitt




                      Tabelle: Der folgenden Tabelle entnehmen Sie alle relevanten Informationen
                      für den Zuschnitt. In der ersten Spalte steht die Ziffer der Sprosse innerhalb
                      der Scheibe (A, B, C, ...). Die Häufigkeit der Sprosse in dieser Scheibe ist in
                      der zweiten Spalte gegeben. 1 bedeutet, die Sprosse ist einmal vorhanden, 2
                      bedeutet, die Sprosse ist zweimal vorhanden, usw.
                      Die dritte Spalte gibt die Länge der Sprosse an. Addiert man die Längen, er-
                      hält man die Materialmenge. In den übrigen Spalten steht die Information über
                      Zuschnitt und Fräspunkte der Sprossen. Eine detaillierte Erläuterung hierzu
                      finden Sie unter:
                       Tutorial, “Zuschnittinformationen anzeigen” auf Seite A-122


                      Weitere Informationen zum Zuschnitt
                       Tutorial, “Zuschnittinformationen anzeigen” auf Seite A-122




A+W CAD Designer (Bars) Überblick                                                             A-231
Die Stammdaten                                                             Softwarereferenz




                 Die Stammdaten
                 Menü Stammdaten öffnen
                 Im Menü Stammdaten befinden sich folgende Menüpunkte:
                 •   Stammdaten:
                     Über diesen Menüpunkt können Sie sich einen Überblick über die Stamm-
                     daten verschaffen.
                      “Stammdaten” auf Seite A-233
                 •   Stammdaten-Editor:
                     Über diesen Menüpunkt bearbeiten Sie die Stammdaten.
                      “Stammdaten-Editor” auf Seite A-235
                     – Passwortschutz:
                       Mit dieser Checkbox können Sie die Stammdaten schützen.
                         “Passwort” auf Seite A-240
                 •   Konfiguration bearbeiten:
                     Über diesen Menüpunkt haben Sie Zugriff auf die Konfiguration.




A-232                                                    A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                Die Stammdaten




                      Stammdaten
                      Stammdaten > Stammdaten
                      oder über die Symbol-Schaltfläche




                      Abb. A-77     Stammdaten


                      Dieser Dialog dient zur Auswahl der Stammdaten und zum Tauschen von
                      Sprossen innerhalb einer Konstruktion. Änderungen an den Stammdaten neh-
                      men Sie im Dialog Stammdaten-Editor vor.

                      Erläuterung der Felder im Bereich Artikelnummer

                      Artikelnummer In diesem Feld wird Ihnen die Artikelnummer der Sprosse
                      angezeigt.

                      Breite In diesem Feld wird Ihnen die Breite der Sprosse angezeigt.

                      Frästiefe In diesem Feld wird Ihnen die Frästiefe der Sprosse angezeigt.

                      Randabzug In diesem Feld wird Ihnen der Randabzug angezeigt.

                      Breite In diesem Feld wird Ihnen die Breite der Sprosse angezeigt.

                      Anzeigefeld In diesem Feld wird Ihnen der Name der Sprosse angezeigt.

                      Erläuterung der Felder im Bereich Farbcode

                      Farbcode Das Feld zeigt Ihnen den Farbcode der Sprosse.

                      Anzeigefeld In diesem Feld wird Ihnen die Farbe der Sprosse angezeigt.




A+W CAD Designer (Bars) Überblick                                                          A-233
Die Stammdaten                                                              Softwarereferenz




                 Erläuterung der Schaltflächen

                 OK Mit dieser Schaltfläche verlassen Sie den Dialog. Änderungen werden
                 gesichert.

                 Abbrechen Mit dieser Schaltfläche verwerfen Sie Änderungen bzw. schlie-
                 ßen Sie die Maske. Befinden Sie sich im Änderungs-, bzw. Einfügenmodus
                 (Editierfelder aktiv) können Sie Eingaben bzw. Änderungen verwerfen. Befin-
                 den Sie sich im Auswahlmodus wird der Dialog geschlossen.


                 Weitere Informationen zu Stammdaten
                  Tutorial, “Sprossen tauschen” auf Seite A-109




A-234                                                     A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                  Die Stammdaten




                      Stammdaten-Editor
                      Stammdaten > Stammdaten-Editor




                      Abb. A-78     Stammdaten-Editor


                      Der Stammdaten-Editor stellt Funktionen für das Verwalten und Ändern der
                      Sprossendaten zur Verfügung. Sie haben damit die Möglichkeit, komplette
                      Sprossendateien bzw. Sprossenlisten anzulegen, diesen Listen einzelne Arti-
                      kel hinzuzufügen oder einzelne Artikel daraus zu entfernen. Sie können den
                      Sprossen verschiedene Attribute zuweisen und jederzeit ändern.

                      Erläuterung der Felder im Bereich Stammdaten

                      Artikelnummer In diesem Bereich werden Ihnen alle definierten Artikelnum-
                      mern angezeigt.
                      Technische Info: Anzeigefeld

                      Breite In diesem Feld geben Sie die Breite der Sprosse ein.
                      Technische Info: Pflichtfeld, Numerisch

                      Frästiefe In diesem Feld geben Sie die Frästiefe ein.
                      Technische Info: Pflichtfeld, Numerisch

                      Offset Dieses Feld dient der Spezialbehandlung von Bohrmaschinen mit Off-
                      set-Bemaßung. Der Offset-Wert ist abhängig von der Sprosse. Sollte in Ihrem
                      Hause eine solche Bohrmaschine installiert sein, kontaktieren Sie bitte unsere
                      Mitarbeiter.
                      Technische Info: Optional, Auswahl




A+W CAD Designer (Bars) Überblick                                                            A-235
Die Stammdaten                                                              Softwarereferenz




                 Randabzug Dieses Feld bezieht sich auf Sprossen mit Randstopfen. In die-
                 sem Fall geben Sie hier den Wert ein, um den die Sprosse kürzer sein muss,
                 damit der Randstopfen auf die Sprosse passt. Randstopfen werden auf dem
                 Bildschirm grafisch dargestellt.
                 Technische Info: Optional, Numerisch

                 Spezial-Kreuzung Über diese Checkbox haben Sie die Möglichkeit, einer
                 Sprosse eine Spezial-Kreuzung zuzuweisen. Den entsprechenden Wert ge-
                 ben Sie im Feld Breite Kreuz ein.
                 Technische Info: Pflichtfeld, Numerisch

                 Breite Kreuz Dieses Feld bezieht sich auf die Checkbox Spezial-Kreuzung.
                 Ein Wert kann nur eingetragen werden, wenn die Checkbox Spezial-Kreuzung
                 aktiv ist. Geben Sie dann die Breite für die Kreuzung ein.
                 Technische Info: Pflichtfeld, Numerisch

                 Stablänge A+W CAD Designer (Bars) ist in der Lage, eine Sprossenoptimie-
                 rung durchzuführen. Dazu ist die Angabe der Stablänge (Sprossenlänge) not-
                 wendig. In diesem Feld geben Sie die Länge des Stabes ein.
                 Technische Info: Pflichtfeld, Numerisch

                 T-Zugabe Wird eine Sprosse im rechten Winkel auf eine andere Sprosse zu-
                 geschnitten, so wird die hier eingestellte Längenangabe zu der eigentlichen
                 Sprossenlänge hinzuaddiert.
                 Technische Info: Pflichtfeld, Numerisch

                 Name In diesem Feld geben Sie den Namen der Sprosse ein.
                 Technische Info: Pflichtfeld, Alphanumerisch

                 Erläuterung der Felder im Bereich Durchgang
                 Dieser Bereich dient der Festlegung von Sprossendurchgängen, die von au-
                 ßen mittels Übergabedateien an A+W CAD Designer (Bars) übergeben wer-
                 den. Beim eigenen Konstruieren von Sprossenbildern werden die Durchgänge
                 im Dialog Muster Senkrecht/Waagerecht festgelegt.

                 Keine Sprosse Das Feld bezieht sich auf Sprossen, die übergeben werden.
                 Durch Aktivieren der Radiotaste legen Sie fest, dass keine der Sprosse durch-
                 gehend ist.
                 Technische Info: Optional, Auswahl

                 Waagerecht Das Feld bezieht sich auf Sprossen, die übergeben werden.
                 Durch Aktivieren der Radiotaste legen Sie fest, dass die waagerechte Sprosse
                 durchgehend ist.
                 Technische Info: Optional, Auswahl

                 Senkrecht Das Feld bezieht sich auf Sprossen, die übergeben werden.
                 Durch Aktivieren der Radiotaste legen Sie fest, dass die senkrechte Sprosse
                 durchgehend ist.
                 Technische Info: Optional, Auswahl




A-236                                                   A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                     Die Stammdaten




                      Alle Sprossen Das Feld bezieht sich auf Sprossen, die übergeben werden.
                      Durch Aktivieren der Radiotaste legen Sie fest, dass alle Sprosse durchge-
                      hend sind.
                      Technische Info: Optional, Auswahl

                      Default aus INI Das Feld bezieht sich auf Sprossen, die übergeben werden.
                      Durch Aktivieren der Radiotaste legen Sie fest, dass die Standard-Werte aus
                      der INI-Datei verwendet werden.
                      Technische Info: Optional, Auswahl

                      Beide+Fräspunkte Dieses Feld dient internen Auswertungen.
                      Technische Info: Optional, Auswahl

                      Scheibensymmetrie Das Feld bezieht sich auf Sprossen, die übergeben
                      werden. Durch Aktivieren der Radiotaste legen Sie fest, dass die durchgehen-
                      de Sprosse automatisch (in Bezug auf die Scheibensymmetrie) bestimmt wird.
                      Aufgrund der Stabilität ist es sinnvoll, dass die durchgehende Sprosse auf der
                      Seite durchgeht, auf der die Scheibe kürzer ist.
                      Technische Info: Optional, Auswahl

                      Doppelter Zuschnitt Für einige Sprossensysteme wird die doppelte Spros-
                      senmenge benötigt (z. B. aufgesetzte Sprossen oder 3-fach ISO). Wenn diese
                      Angabe in der Stammdaten aktiv ist, werden für den verwendeten Sprossen-
                      typ die Zuschnittmengen verdoppelt.
                      Diese wird hier eingestellt und für jeden Sprossentyp hinterlegt.
                      Technische Info: Optional, Auswahl

                      L-Felder mit Abzug Das Aktivieren dieser Checkbox ist nur sinnvoll, wenn
                      Sie im Dialog Muster Senkrecht/Waagerecht als Teilung Gleiche lichte Felder
                      wählen. Dann erfolgt die Vermaßung beim ersten und beim letzten Feld ohne
                      Berücksichtigung der Randstopfen.
                      Technische Info: Optional, Auswahl

                      Liniennummer Wenn es in Ihrem Hause mehrere Sprossenfertigungslinien
                      gibt, können Sie die Sprossentypen auf unterschiedlichen Linien fertigen las-
                      sen. Das Feld wird über spezielle Einstellungen in der INI-Datei aktiviert, hier-
                      zu kontaktieren Sie bitte unsere Mitarbeiter.
                      Technische Info: Eingabe optional

                      Erläuterung der Schaltfläche

                      Start Mit dieser Schaltfläche definieren Sie einen Sprossenartikel als Stan-
                      dardsprosse zum Erstellen von Sprossenkonstruktionen. Sofern Sie keine an-
                      dere Auswahl getroffen haben, werden Sprossen die Sie neu einfügen, von
                      diesem Typ eingefügt. Damit Sie erkennen können, welcher Sprossenartikel
                      als Standard definiert wurde, wird Ihnen dieser im Feld darunter angezeigt.




A+W CAD Designer (Bars) Überblick                                                              A-237
Die Stammdaten                                                               Softwarereferenz




                 Erläuterung der Felder im Bereich Optionen

                 Passwortschutz Da es sich bei den Stammdaten um einen sensiblen Be-
                 reich handelt, können Sie diesen Bereich durch ein Passwort schützen. Wenn
                 Sie diese Checkbox aktivieren, öffnet sich beim Sichern der Stammdaten der
                 Dialog Passwort.
                 Technische Info: Optional, Auswahl

                 Erläuterung der Schaltflächen

                 Umbenennen Mit dieser Schaltfläche können Sie eine Artikelnummer än-
                 dern. Nachdem Sie die Schaltfläche betätigt haben, öffnet sich der Dialog Ein-
                 gabe neuer Artikel.

                 Hinzufügen Mit dieser Schaltfläche können Sie eine Artikelnummer hinzufü-
                 gen. Nachdem Sie die Schaltfläche betätigt haben, öffnet sich der Dialog Ein-
                 gabe neuer Artikel.

                 Entfernen Mit dieser Schaltfläche können Sie eine Artikelnummer löschen.
                 Nachdem Sie die Schaltfläche betätigt haben, wird die Artikelnummer aus der
                 Liste der Artikelnummern gelöscht.

                 Erläuterung der Felder im Bereich Farbe

                 Farbcode In diesem Bereich werden Ihnen alle Farbcodes (z. B. RAL-Töne)
                 angezeigt, die im System vorhanden sind. Befindet sich vor dem Farbcode ein
                 Häckchen, ist die im Feld Artikelnummer ausgewählte Sprosse in dem ent-
                 sprechenden (angehakten) Farbcode vorhanden. Um einen neuen Farbcode
                 anzulegen, betätigen Sie die Schaltfläche [Hinzufügen]. Um einen Farbcode
                 zu löschen, betätigen Sie die Schaltfläche [Entfernen].
                 Technische Info: Anzeigefeld

                 Name In diesem Feld wird Ihnen der Farbname angezeigt.
                 Technische Info: Pflichtfeld, Alphanumerisch

                 Erläuterung der Schaltflächen

                 Hinzufügen Mit dieser Schaltfläche können Sie eine Farbe hinzufügen.
                 Nachdem Sie die Schaltfläche betätigt haben, öffnet sich der Dialog Eingabe
                 neuer Farbcode.

                 Entfernen Mit dieser Schaltfläche können Sie eine Farbe löschen. Nachdem
                 Sie die Schaltfläche betätigt haben, wird die Farbe aus der Liste der Farb-
                 codes gelöscht.

                 Ändern Mit dieser Schaltfläche haben Sie die Möglichkeit, die Sprossen in
                 der jeweiligen Farbe optisch darzustellen. Sie können jeden Farbcode optisch
                 hinterlegen. Markieren Sie dazu den gewünschten Eintrag im Bereich Farb-
                 code und betätigen Sie anschließend diese Schaltfläche. Es öffnet sich der Di-
                 alog Farbe. Wählen Sie entweder eine Grundfarbe aus oder betätigen Sie die
                 Schaltfläche [Farben definieren >>] um eine eigene Farbe zusammen zustel-
                 len.


A-238                                                   A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                    Die Stammdaten




                      Start Gibt es eine Sprosse in mehreren Farben, können Sie festlegen, wel-
                      che Farbe die Standardfarbe sein soll. Hierzu wählen Sie im Bereich Farbcode
                      die entsprechende Farbe aus und betätigen anschließend diese Schaltfläche.
                      Zukünftig werden alle Sprossen in dieser Farbe auf der Scheibe platziert. Da-
                      mit Sie erkennen können, welche Farbe die Standardfarbe ist, wird Ihnen die-
                      se im Feld darunter angezeigt.

                      Clipboard Die Inhalte des Dialogs können mithilfe dieser Schaltfläche in die
                      Zwischenablage kopiert werden. Von dort können sie in Textverarbeitungs-
                      programme oder Tabellenkalkulationen übernommen werden.


                      Weitere Informationen zum Stammdaten-Editor
                       Tutorial, “Stammdaten in A+W CAD Designer (Bars)” auf Seite A-85
                       Tutorial, “Übung 1: Einen Sprossenartikel anlegen” auf Seite A-96




A+W CAD Designer (Bars) Überblick                                                           A-239
Die Stammdaten                                                              Softwarereferenz




                 Passwort
                 Stammdaten > Stammdaten-Editor > Checkbox Passwortschutz aktivieren >
                 Schaltfläche [OK] betätigen




                 Abb. A-79    Passwort


                 Da es sich bei den Stammdaten um einen sensiblen Bereich handelt, können
                 Sie den Zugriff durch ein Passwort schützen.

                 Erläuterung der Felder

                 Passwort In diesem geben Sie das Passwort ein.
                 Technische Info: Pflichtfeld, Eingabe, alphanumerisch

                 Bestätigung In diesem müssen Sie das Passwort zur Bestätigung noch ein-
                 mal wiederholen.
                 Technische Info: Pflichtfeld, Eingabe, alphanumerisch


                 Weitere Informationen zum Passwort
                  “Stammdaten-Editor” auf Seite A-235
                  Tutorial, “Stammdaten schützen” auf Seite A-95




A-240                                                     A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                            Ansicht




                      Ansicht
                      Menü Ansicht öffnen
                      Im Menü Ansicht befinden sich folgende Menüpunkte:
                      •   Größer:
                          Über diesen Menüpunkt können Sie die Ansicht vergrößern.
                      •   Kleiner:
                          Über diesen Menüpunkt können Sie die Ansicht verkleinern.
                      •   Voll:
                          Über diesen Menüpunkt bringen Sie die Ansicht zum Vollbild.
                      •   Einstellungen:
                          Über diesen Menüpunkt können Sie die Einstellungen für die Vermaßung,
                          die Sprache und das Maßsystem bearbeiten.
                           “Vermaßung” auf Seite A-242
                           “Maße” auf Seite A-244
                           “Sprachauswahl” auf Seite A-245
                      •   Werkzeuge:
                          Über diesen Menüpunkt blenden Sie die Symbolleiste ein oder aus. Die
                          Werkzeuge werden an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Symbolleiste” auf Seite A-18
                      •   Statuszeile:
                          Über diesen Menüpunkt blenden Sie die Statuszeile am unteren Bild-
                          schirmrand ein oder aus.
                      •   Fangpunkte:
                          Über diesen Menüpunkt blenden Sie die Symbolleiste für die Fangpunkte
                          ein oder aus. Die Fangpunkte werden an folgender Stelle ausführlich erläu-
                          tert:
                           Tutorial, “Das Arbeiten mit Fangpunkten” auf Seite A-22
                      •   Sprossenartikel:
                          Über diesen Menüpunkt blenden Sie die Standardsprosse ein oder aus.
                          Die Standardsprosse wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Die Standard-Sprosse” auf Seite A-21
                      •   Zuschnitt:
                          Über diesen Menüpunkt blenden Sie das Symbol für den YT-Zuschnitt ein
                          oder aus.
                      •   Messen:
                          Über diesen Menüpunkt blenden Sie das Symbol zum Messen ein oder
                          aus. Das Werkzeug wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Abstände oder Längen messen” auf Seite A-126
                      •   Zeichenwerkzeug:
                          Über diesen Menüpunkt blenden Sie die Symbole für die Zeichenwerkzeu-
                          ge ein oder aus. Die Zeichenwerkzeuge werden an folgender Stelle aus-
                          führlich erläutert:
                           Tutorial, “Die Werkzeuge” auf Seite A-40
                      •   Wertefenster:
                          Über diesen Menüpunkt blenden Sie das Wertefenster ein oder aus. Das
                          Wertefenster wird an folgender Stelle ausführlich erläutert:
                           Tutorial, “Das Wertefenster” auf Seite A-20



A+W CAD Designer (Bars) Überblick                                                            A-241
Ansicht                                                              Softwarereferenz




          •   Vermaßung:
              Über diesen Menüpunkt belnden Sie die Symbole für die Vermaßung ein
              oder aus. Die Vermaßung wird an folgender Stelle ausführlich erläutert:
               Tutorial, “Die Vermaßungswerkzeuge” auf Seite A-74



          Vermaßung
          Ansicht > Einstellungen > Register Vermaßung




          Abb. A-80    Einstellungen, Register Vermaßung


          In diesem Dialog nehmen Sie die Einstellungen für die Vermaßung vor. Sie le-
          gen fest, ob und wie Ihnen die Vermaßung am Bildschirm angezeigt wird.

          Erläuterung der Felder

          Vermaßung Über diese Checkbox steuern Sie, ob eine Vermaßung ange-
          zeigt wird oder nicht.
          ☐ Es wird keine Vermaßung angezeigt.
          ☑ Die Vermaßung wird angezeigt.
          Technische Info: Optional, Auswahl

          Modell Hier fehlt noch was.

          Absolute Bohrpunkte Die Vermaßung erfolgt in Bezug auf die absoluten
          Bohrpunkte.

          Relative Bohrpunkte Die Vermaßung erfolgt in Bezug auf die relativen Bohr-
          punkte.




A-242                                              A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                          Ansicht




                      Erläuterung der Felder im Bereich Bezug auf

                      Rahmen Wenn Sie diese Radiotaste wählen, erfolgt die Vermaßung mit Be-
                      zug auf den Rahmen.
                      Technische Info: Optional, Auswahl

                      Scheibe Wenn Sie diese Radiotaste wählen, erfolgt die Vermaßung mit Be-
                      zug auf die Scheibe.
                      Technische Info: Optional, Auswahl

                      Erläuterung der Felder im Bereich Bezugspunkt

                      Oben links Wenn Sie diese Radiotaste wählen, startet die Vermaßung oben
                      links.

                      Unten links Wenn Sie diese Radiotaste wählen, startet die Vermaßung un-
                      ten links.

                      Oben rechts Wenn Sie diese Radiotaste wählen, startet die Vermaßung
                      oben rechts.

                      Unten rechts Wenn Sie diese Radiotaste wählen, startet die Vermaßung un-
                      ten rechts.

                      Erläuterung der weiteren Felder

                      Ziffern an Sprosse Wenn Sie diese Checkbox aktivieren, werden die Spros-
                      sen alphabetisch gekennzeichnet.

                      Fräspunkte Wenn Sie diese Checkbox aktivieren, wird Ihnen die Vermaßung
                      der Fräspunkte angezeigt.

                      Pfeile Wenn Sie diese Checkbox aktivieren, wird Ihnen die Vermaßung mit
                      Pfeilspitzen angezeigt.

                      Erläuterung der Felder im Bereich Zeichengröße

                      Breite In diesem Feld legen Sie fest, in welcher Zeichenbreite die Verma-
                      ßung dargestellt wird.

                      Höhe In diesem Feld legen Sie fest, in welcher Zeichenhöhe die Vermaßung
                      dargestellt wird.

                      Skalierbar mit Scheibe Wenn Sie diese Checkbox aktivieren, wird die
                      Schrift beim Skalieren der Scheibe angepasst.


                      Weitere Informationen zu Vermaßung
                       Tutorial, “Einstellungen” auf Seite A-75




A+W CAD Designer (Bars) Überblick                                                          A-243
Ansicht                                                              Softwarereferenz




          Maße
          Ansicht > Einstellungen > Register Maße




          Abb. A-81    Einstellungen, Register Maße


          In diesem Dialog nehmen Sie die Einstellungen für die Maße vor.

          Erläuterung der Felder

          Maßeingabe in mm Wenn Sie diese Radiotaste aktivieren, erfolgt die Ver-
          maßung in mm.
          Technische Info: Optional, Auswahl

          Maßeingabe Zoll (Brüche) Wenn Sie diese Radiotaste aktivieren, erfolgt die
          Vermaßung in Inch (1/24).
          Technische Info: Optional, Auswahl

          Maßeingabe Zoll (Dezimal) Wenn Sie diese Radiotaste aktivieren, erfolgt
          die Vermaßung in Inch (3,52).
          Technische Info: Optional, Auswahl

          Bruch Nenner Dieses Eingabefeld ist nur dann aktiv, wenn Sie die Radiotas-
          te Maßeingabe Zoll (Brüche) angeklickt haben. Dann geben Sie in diesem
          Feld den Nenner an. Bsp.: 32 für 1/32.

          Genauigkeit Dezimal Dieses Eingabefeld ist nur dann aktiv, wenn Sie die
          Radiotaste Maßeingabe Zoll (Dezimal) angeklickt haben. Dann geben Sie in
          diesen Feld die Anzahl der Nachkommastellen ein. Bsp.: 3 für 2,345.


          Weitere Informationen zu Maßen
           Tutorial, “Maße eingeben” auf Seite A-82



A-244                                              A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                                          Ansicht




                      Sprachauswahl
                      Ansicht > Einstellungen > Register Sprachauswahl




                      Abb. A-82     Einstellungen, Register Sprachauswahl


                      In diesem Dialog wählen Sie die Sprache für A+W CAD Designer (Bars) aus.
                      Nachdem Sie den Dialog mit der Schaltfläche [OK] verlassen haben, stellt
                      A+W CAD Designer (Bars) die Sprache um.

                      Erläuterung der Felder

                      Wählen Sie die Sprache aus Wählen Sie aus der Kombobox die gewünsch-
                      te Sprache aus und betätigen Sie die Schaltfläche [OK]. Die Sprache wird so-
                      fort umgestellt. Es ist kein Neustart erforderlich.
                      Technische Info: Optional, Auswahl


                      Weitere Informationen zur Sprache
                       Tutorial, “Programmsprache wählen” auf Seite A-84




A+W CAD Designer (Bars) Überblick                                                          A-245
Die Hilfe verwenden                                                           Softwarereferenz




                      Die Hilfe verwenden
                      Menü Hilfe öffnen
                      Im Menü Hilfe befinden sich folgende Menüpunkte:
                      •   Hilfethemen:
                          Über diesen Menüpunkt starten Sie die Hilfe.
                      •   Programminformationen:
                          Über diesen Menüpunkt erhalten Sie Informationen zu A+W CAD Designer
                          (Bars).
                           Tab. auf Seite A-247




A-246                                                      A+W CAD Designer (Bars) Überblick
Softwarereferenz                                                              Die Hilfe verwenden




                      Über CAD Designer
                      Hilfe > Info über CAD Designer




                      Abb. A-83     Über CAD Designer


                      In diesem Dialog erhalten Sie weitere Informationen zu dem Programm A+W
                      CAD Designer (Bars), z. B. Version und Release-Stand.
                      Wenn Sie die Schaltfläche [Info] betätigen, öffnet sich der Dialog Programm-
                      informationen. Dort erhalten Sie Informationen bezüglich Dateiversionen.




A+W CAD Designer (Bars) Überblick                                                          A-247
Die Hilfe verwenden                     Softwarereferenz




A-248                 A+W CAD Designer (Bars) Überblick
A   A+W CAD Designer (Bars)
    CAD Designer




                     Help Cards
                                                                                                                               Help Cards




In diesem Kapitel finden Sie folgende Informationen:
 Informationen zu den HelpCards
 Stammdaten
 Sprossen
 Spezialmuster


Informationen zu den HelpCards ........................................................................ A-251
Stammdaten ........................................................................................................ A-252
  Werkzeuge ....................................................................................................... A-253
  Fangpunkte ...................................................................................................... A-254
  Sprossen anlegen ............................................................................................ A-255
  Stammdaten schützen ..................................................................................... A-256
Sprossen ............................................................................................................. A-257
  Eigenschaften der Scheibe .............................................................................. A-258
  Einfaches Sprossenmuster platzieren ............................................................. A-259
  Sprossen über Werte platzieren ...................................................................... A-260
  Modell mit Sprossen platzieren ........................................................................ A-261
  Freie Sprossenkonstruktion erstellen .............................................................. A-262
Spezialmuster ..................................................................................................... A-263
  Fassadenanlage erstellen ................................................................................ A-264
  Makro laden ..................................................................................................... A-265
  Ein Makro ändern und speichern ..................................................................... A-266
  Eigenes Makro erstellen .................................................................................. A-267




A-250                                                                                                   A+W CAD Designer (Bars) Überblick
Help Cards                                                        Informationen zu den HelpCards




Informationen zu den HelpCards
Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W CAD Designer 2014. Ein-
zelne Schritte in den Workflows können je nach Konfiguration abweichen.




A+W CAD Designer (Bars) Überblick                                                          A-251
Stammdaten                                                               Help Cards




Stammdaten
Help Card               Themen

• Werkzeuge             • Sie erhalten einen Überblick über die Werkzeuge.

• Fangpunkte            • Sie erhalten einen Überblick über die Fangpunkte.

• Sprossen anlegen      • Einen Sprossenartikel anlegen.

• Stammdaten schützen   • Die Stammdaten mit einem Passwort schützen.




A-252                                        A+W CAD Designer (Bars) Überblick
Stammdaten
Werkzeuge                                                                              Bar 01-001




 Ziel der Handlung
Sie erhalten einen Überblick über die Werkzeuge.

 Voraussetzungen

 Zusatzinfo


 Übersicht
      Element auswählen.

      Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten.

      Erzeugt eine horizontale Sprosse zwischen zwei Fangpunkten.

      Erzeugt eine vertikale Sprosse zwischen zwei Fangpunkten.

      Erzeugt eine Sprosse zwischen zwei Fangpunkten unter Eingabe des Winkels.

      Erzeugt eine gebogene Sprosse zwischen drei Fangpunkten.

      Erzeugt einen Sprossenkreis zwischen zwei Fangpunkten.

      Erzeugt eine Sonne in einem lichten Feld.

      Erzeugt einen Halbmond.

      Erzeugt einen Bogen in einem lichten Feld.

      Für eine 90° Kreuzung wird die Durchgangsrichtung geändert.

      Sprosse wird bis auf wählbares Objekt verlängert.

      Teilt alle Sprossen.

      Verbindet alle Sprossen.

      Setzt oder löscht eine Sprosse in einem lichten Feld.

      Erzeugt eine neue Scheibe.

      Erzeugt aus Makro Sprossen-Aufteilung in der Scheibe.

      Öffnet den Dialog zur Eingabe von senkrechten und waagerechten Sprossen.

      Zeigt die entsprechenden Mengen im Wertebereich an.

      Ändert den YT-Zuschnitt.



A+W CAD Designer (Bars) Überblick                                                 Help Cards   A-253
Stammdaten
Fangpunkte                                                                                 Bar 01-002




 Ziel der Handlung
Sie erhalten einen Überblick über die Fangpunkte.

 Voraussetzungen

 Zusatzinfo


 Übersicht
      Löscht einen Fangpunkt.

      Löscht alle Fangpunkte.

      Eingabe der Anzahl der Intervalle für ein Objekt.

      Erzeugt Fangpunkte in allen Schnittpunkten zweier Objekte.

      Erzeugt einen Fangpunkt relativ zu einem beliebigen Punkt.

      Erzeugt Fangpunkte auf Sprossen, Rahmen oder Scheibenrand.

      Erzeugt vier Fangpunkte auf den Ecken eines durch 2 Klicks beschr. Rechtecks.

      Erzeugt Fangpunkte in allen Schnittpunkten mit anderen Sprossen.

      Erzeugt Fangpunkte auf einer Geraden.

      Erzeugt in wählbarer Entfernung einen Fangpunkt auf einem Bogen.

      Erzeugt Fangpunkte in möglichen Mittelpunkten von Kreisen (2 Punkte).

      Erzeugt Fangpunkte parallel versetzt zu einer Geraden.

      Erzeugt einen Fangpunkt in wählbarer Entfernung entlang eines Bogens.

      Erzeugt Fangpunkte im Mittelpunkt eines Kreises (3 Punkte).

      Erzeugt Fangpunkte vom Bezugspunkt aus unter einem einstellbaren Winkel.

      Erzeugt einen Fangpunkt auf einer Geraden im wählbaren Abstand vom
      Startpunkt.




A+W CAD Designer (Bars) Überblick                                                     Help Cards   A-254
Stammdaten
Sprossen anlegen                                                                                       Bar 01-003




 Ziel der Handlung
Einen Sprossenartikel anlegen.

 Voraussetzungen



 Zusatzinfo



 Workflow
1 Öffnen Sie den Dialog Stammdaten-Editor [Stammdaten        8 Geben Sie im Feld T-Zugabe einen Wert ein, wenn die
  > Stammdaten-Editor].                                        Sprosse im rechten Winkel auf eine andere Sprosse zu-
                                                               geschnitten wird.
2 Klicken Sie auf die Schaltfläche [Hinzufügen]. Geben Sie
  die gewünschte Artikel-Nummer ein.                         9 Die Radiotasten im Bereich Durchgang dienen der Fest-
                                                               legung von Sprossendurchgängen, die von außen mit-
3 Geben Sie im Feld Breite die Sprossenbreite ein.
                                                               tels Übergabedateien an A+W CAD Designer (Bars)
4 Geben Sie im Feld Frästiefe (verstellbare Begrenzungs-       übergeben werden.
  anschlag, gegen den das vorher gekappte Sprossenen-
                                                             10 Aktivieren Sie die Checkbox Doppelter Zuschnitt, wenn
  de positioniert wird) den entsprechenden Wert ein.
                                                                für den verwendeten Sprossentyp die Zuschnittmenge
5 Geben Sie im Feld Randabzug (Stärke des Kunststoff-           automatisch verdoppelt werden soll (3fach ISO)
  Stopfen) den entsprechenden Wert ein.
                                                             11 Wenn Sie die Checkbox L-Felder mit Abzug aktivieren,
6 Wenn gewünscht, aktivieren Sie die Checkbox Spezial-          werden die Randstopfen der Sprosse nicht mit vermaßt.
  Kreuzung (keine durchgehende Sprosse - Steckverbin-
                                                             12 Bei mehreren Sprossenfertigungslinien können Sie im
  dungen) und geben im Feld Breite Kreuz den entspre-
                                                                Feld Liniennummer die entsprechende Nummer einge-
  chenden Wert ein.
                                                                ben.
7 Geben Sie im Feld Stablänge die Länge des Sprossen-
                                                             13 Im Feld Farbcode weißen Sie der Sprosse die RAL-Far-
  stabes ein.
                                                                be zu.
                                                             14 Handelt es sich bei der Sprosse um die Standard-Spros-
                                                                se, klicken Sie auf die Schaltflächen [Start].




A+W CAD Designer (Bars) Überblick                                                                Help Cards     A-255
Stammdaten
Stammdaten schützen                                                                                        Bar 01-004




 Ziel der Handlung
Die Stammdaten mit einem Passwort schützen.

 Voraussetzungen
Stammdaten sind angelegt

 Zusatzinfo



 Workflow
1 Öffnen Sie den Dialog Stammdaten-Editor [Stammdaten           5 Geben Sie im Feld Passwort das gewünschte Passwort
  > Stammdaten-Editor].                                           ein.
2 Aktivieren Sie die Checkbox Passwortschutz im Bereich         6 Wiederholen Sie im Feld Bestätigung das eingegebene
  Optionen.                                                       Passwort.
3 Klicken Sie auf die Schaltfläche [OK]. Es folgt eine Abfra-   7 Klicken Sie auf die Schaltfläche [OK].
  ge, ob die Stammdaten gesichert werden sollen.
                                                                8 Wenn Sie das nächste Mal den Stammdaten-Editor öff-
4 Klicken Sie auf die Schaltfläche [Ja]. Es öffnet sich der       nen, werden Sie nach dem Passwort gefragt.
  Dialog Passwort?




A+W CAD Designer (Bars) Überblick                                                                    Help Cards   A-256
Help Cards                                                                                 Sprossen




Sprossen
Help Card                                Themen

• Eigenschaften der Scheibe              • Die Eigenschaften der Scheibe definieren.

• Einfaches Sprossenmuster platzieren    • Zwei senkrechte und zwei waagerechte Sprossen platzieren.

• Sprossen über Werte platzieren         • Sprossen über feste Werte platzieren.

• Modell mit Sprossen platzieren         • Ein Modell mit Sprossen platzieren.

• Freie Sprossenkonstruktion erstellen   • Eine freie Sprossenkonstruktion erstellen.




A+W CAD Designer (Bars) Überblick                                                             A-257
Sprossen
Eigenschaften der Scheibe                                                                               Bar 02-001




    Ziel der Handlung
Die Eigenschaften der Scheibe definieren.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo



    Workflow
1 Klicken Sie auf die Symbol-Schaltfläche [Neue Scheibe].    4 Die Felder im unteren Bereich des Dialogs dienen der
  Der Dialog Modell-Erfassung öffnet sich.                     Eingabe der Auftragsdaten. Füllen Sie diese entspre-
                                                               chend aus.
2 Wählen Sie die Modell-Nr. aus und geben Sie die Maße
  ein.                                                       5 Im Bereich Extra haben Sie die Möglichkeit für diverse
                                                               Einträge (z. B. Liefertermin, Abstandhalter, Gaskürzel,
3 Anschließend öffnet sich der Dialog Eigenschaften
                                                               etc.) Texte zu hinterlegen. Im Falle einer A+W Produc-
  Scheibe. Über die Felder X- und Y-Position können Sie
                                                               tion-Anbindung, werden diese Felder bei der Übergabe
  die Position auf Ihrer Arbeitsfläche bestimmen. Zum Dre-
                                                               automatisch gefüllt.
  hen der Scheibe dient das Feld Ausrichtung.
                                                             6 Über die Schaltfläche [OK] verlassen Sie den Dialog. Die
                                                               Scheibe wird platziert.




A+W CAD Designer (Bars) Überblick                                                                 Help Cards     A-258
Sprossen
Einfaches Sprossenmuster platzieren                                                                    Bar 02-002




    Ziel der Handlung
Zwei senkrechte und zwei waagerechte Sprossen platzie-
ren.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.                      •   Scheibe muss platziert sein.

    Zusatzinfo



    Workflow
1 Klicken Sie auf die Symbol-Schaltfläche [Neues senk-      4 Aktivieren Sie im Bereich Teilung Senkrecht die Option
  recht/waagerecht Muster] und anschließend auf die           Gleiche lichte Felder.
  Scheibe. Der Dialog Muster Senkrecht-Waagerecht öff-
                                                            5 Aktivieren Sie im Bereich Durchgängige Sprossen die
  net sich.
                                                              Option Senkrechte.
2 Geben Sie die Anzahl der Sprossen ein.
                                                            6 Über die Schaltfläche [OK] verlassen Sie den Dialog. Die
3 Aktivieren Sie im Bereich Teilung Waagerecht die Option     Sprossen werden platziert.
  Gleiche lichte Felder.




A+W CAD Designer (Bars) Überblick                                                                Help Cards     A-259
Sprossen
Sprossen über Werte platzieren                                                                             Bar 02-003




    Ziel der Handlung
Sprossen über feste Werte platzieren.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.                         •   Scheibe muss platziert sein.

    Zusatzinfo



    Workflow
1 Klicken Sie auf die Symbol-Schaltfläche [Neues senk-             wird geschlossen. Wiederholen Sie den Vorgang mit 300
  recht/waagerecht Muster] und anschließend auf die                mm. Aktivieren Sie die Radiotaste Von unten.
  Scheibe. Der Dialog Muster Senkrecht-Waagerecht öff-
                                                               4 Aktivieren Sie im Bereich Senkrechte Sprosse die Option
  net sich.
                                                                 Scheibenrand. Aktivieren Sie die Radiotaste Senkr.. Kli-
2 Geben Sie in den Feldern Anzahl Waagerecht und An-             cken Sie auf die Schaltfläche [Hinzufügen]. Es öffnet sich
  zahl Senkrecht jeweils eine 2 ein. Aktivieren Sie in den       der Dialog Eingabe Sprossen-Abstände. Geben Sie 200
  Bereichen Teilung Waagerecht und Teilung Senkrecht             mm ein. Klicken Sie auf [OK]. Der Dialog wird geschlos-
  die Option Kundendefiniert. Klicken Sie auf die Schaltflä-     sen. Wiederholen Sie den Vorgang mit 400 mm. Aktivie-
  che [OK]. Es öffnet sich der Dialog Kundenvorgabe SW-          ren Sie die Radiotaste Von links. Über die Schaltfläche
  Muster.                                                        [OK] verlassen Sie den Dialog.
3 Aktivieren Sie im Bereich Waagerechte Sprosse die Op-        5 Aktivieren Sie im Dialog Muster Senkrecht-Waagerecht
  tion Scheibenrand. Aktivieren Sie die Radiotaste Waa-          im Bereich Durchgängige Sprossen die Option Senk-
  ger.. Klicken Sie auf die Schaltfläche [Hinzufügen]. Es        rechte.
  öffnet sich der Dialog Eingabe Sprossen-Abstände. Ge-
                                                               6 Über die Schaltfläche [OK] verlassen Sie den Dialog. Die
  ben Sie 150 mm ein. Klicken Sie auf [OK]. Der Dialog
                                                                 Sprossen werden platziert.




A+W CAD Designer (Bars) Überblick                                                                    Help Cards     A-260
Sprossen
Modell mit Sprossen platzieren                                                                           Bar 02-004




    Ziel der Handlung
Ein Modell mit Sprossen platzieren.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo



    Workflow
1 Klicken Sie auf die Symbol-Schaltfläche [Neue Scheibe]         dell. Der Dialog Muster Senkrecht-Waagerecht öffnet
  und anschließend auf die Arbeitsfläche. Der Dialog Mo-         sich.
  dell-Erfassung öffnet sich.
                                                              5 Geben Sie in dem Feld Anzahl Waagerecht eine 2 und in
2 Öffnen Sie die Kombobox Modell-Nummer und wählen              dem Feld Anzahl Senkrecht eine 1 ein.
  Sie das Modell 065 aus. Das Modell hat eine Höhe von
                                                              6 Aktivieren Sie in den Bereichen Teilung Waagerecht und
  800 und eine Breite von 600. Klicken Sie auf die Schalt-
                                                                Teilung Senkrecht jeweils die Option Gleiche lichte Fel-
  fläche [OK]. Das Modell wird platziert und der Dialog Ei-
                                                                der.
  genschaften Scheibe öffnet sich.
                                                              7 Aktivieren Sie im Bereich Durchgängige Sprosse die Op-
3 Füllen Sie die Felder entsprechend aus und klicken Sie
                                                                tion Senkrechte. Klicken Sie auf die Schaltfläche [OK].
  auf [OK].
                                                              8 Die Sprossen werden platziert.
4 Klicken Sie auf die Symbol-Schaltfläche [Neues senk-
  recht/waagerecht Muster] und anschließend auf das Mo-




A+W CAD Designer (Bars) Überblick                                                                  Help Cards     A-261
Sprossen
Freie Sprossenkonstruktion erstellen                                                                         Bar 02-005




    Ziel der Handlung
Eine freie Sprossenkonstruktion erstellen.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo



    Workflow
1 Die Schritte 1 bis 3 entnehmen Sie der Übung Freie             4 Setzen Sie auf die oberen Teile der senkrechten Spros-
  Sprossenkonstruktion erstellen (Abmessungen: Brei-               sen jeweils drei Fangpunkte und verbinden Sie die mitt-
  te=500, Höhe=600).                                               leren Fangpunkte mit einer waagerechten Sprosse.
2 Klicken Sie auf die Symbol-Schaltfläche [Neues senk-           5 Löschen Sie die Fangpunkte und aktivieren Sie das
  recht/waagerecht Muster] und anschließend auf das Mo-            Werkzeug Sprosse setzen/löschen. Markieren Sie auf
  dell. Der Dialog Muster Senkrecht-Waagerecht öffnet              der linken Seite die senkrechte Sprosse dort, wo sie ab-
  sich. Geben Sie in dem Feld Anzahl Waagerecht eine 3             geschnitten werden soll. Das obere Stück der senkrech-
  und in dem Feld Anzahl Senkrecht eine 2 ein.                     ten Sprosse wird gelöscht. Wiederholen Sie den Vorgang
                                                                   für die rechte Seite.
3 Aktivieren Sie im Bereich Teilung Waagerecht die Radio-
  taste Kundendefiniert. Aktivieren Sie im Bereich Durch-        6 Aktivieren Sie das Werkzeug Sonne. Klicken Sie in das
  gängige Sprossen die Checkbox Waagerechte.                       Feld, in dem die Sonne eingefügt werden soll. Es öffnet
  Aktivieren Sie im Bereich Teilung Senkrecht die Radio-           sich der Dialog Sonne und Sterne. Aktivieren Sie die Ra-
  taste Gleiche lichte Felder. Klicken Sie auf [OK]. Es öffnet     diotaste Stern sowie die Checkbox Gemeinsamer Zu-
  sich der Dialog Kundenvorgabe SW-Muster. Aktivieren              schnitt. Das Strahlenmuster hat gleiche Winkel und drei
  Sie im Bereich Waagerechte Sprossen die Checkbox                 Strahlen.
  Aufsummieren. Fügen Sie drei Sprossen mit einem Ab-
                                                                 7 Klicken Sie auf die Schaltfläche [OK]. Der Dialog wird ge-
  stand von 120 ein. Betätigen Sie die Schaltfläche [OK].
                                                                   schlossen und das Strahlenmuster eingefügt.




A+W CAD Designer (Bars) Überblick                                                                      Help Cards     A-262
Help Cards                                                                     Spezialmuster




Spezialmuster
Help Card                           Themen

• Fassadenanlage erstellen          • Eine Fassadenanlage platzieren.

• Makro laden                       • Ein vorhandenes Makro laden.

• Ein Makro ändern und speichern    • Ein vorhandenes Makro abändern und speichern.

• Eigenes Makro erstellen           • Ein eigenes Makro erstellen.




A+W CAD Designer (Bars) Überblick                                                     A-263
Spezialmuster
Fassadenanlage erstellen                                                                                Bar 03-001




    Ziel der Handlung
Eine Fassadenanlage platzieren.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo



    Workflow
1 Wählen Sie im Menü Makro > Spezial Muster > Fassa-          Die vom Programm ermittelten Abstände werden über-
  denanlage. Es öffnet sich der Dialog Fassadenanlage...      nommen.
2 Geben Sie folgende Scheibenabmessungen ein:                 Betätigen Sie die Schaltfläche [OK]. Es öffnet sich der Di-
                                                              alog Eigenschaften Scheibe. Nehmen Sie die entspre-
     •   Scheibe A und D: Breite=800, Höhe=600
                                                              chenden Eintragungen vor.
     •   Scheibe B: Breite=400, Höhe=300
     •   Scheibe C: Breite=200, Höhe=100                   3 Klicken Sie auf die Schaltfläche [OK]. Der Dialog wird ge-
                                                             schlossen und die Fassade platziert.




A+W CAD Designer (Bars) Überblick                                                                 Help Cards      A-264
Spezialmuster
Makro laden                                                                                            Bar 03-002




    Ziel der Handlung
Ein vorhandenes Makro laden.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo



    Workflow
1 Platzieren Sie Modell-Nr. 0 mit einer Breite=800 und ei-   6 Es öffnet sich der Dialog Relativer Abstand. Geben Sie
  ner Höhe=600.                                                für die Breite der Rauten 125 mm ein. Schließen Sie den
                                                               Dialog mit der Schaltfläche [OK].
2 Füllen Sie den Dialog Eigenschaften Scheibe. Markieren
  Sie im Bereich Extra den Eintrag Kommisionstext und        7 Markieren Sie Höhe der Raute und klicken Sie auf die
  geben Sie Wohnanlage II ein.                                 Schaltfläche [Ändern...].
3 Betätigen Sie die Symbol-Schaltfläche [Neues Makro].       8 Es öffnet sich der Dialog Relativer Abstand. Geben Sie
  Platzieren Sie den Mauszeiger auf dem Modell und betä-       für die Höhe der Rauten 150 mm ein. Schließen Sie den
  tigen Sie die linke Maustaste. Es öffnet sich der Dialog     Dialog mit der Schaltfläche [OK].
  Makro auswählen.
                                                             9 Schließen Sie den Dialog Makro-Parameter mit der
4 Wählen Sie das Marko York3H1S aus und klicken Sie auf        Schaltfläche [OK].
  [OK].
                                                             10 Das Makro wird platziert.
5 Es öffnet sich der Dialog Makro-Parameter. Markieren
  Sie Breite der Raute und betätigen Sie die Schaltfläche
  [Ändern...].




A+W CAD Designer (Bars) Überblick                                                                Help Cards     A-265
Spezialmuster
Ein Makro ändern und speichern                                                                   Bar 03-003




    Ziel der Handlung
Ein vorhandenes Makro abändern und speichern.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo



    Workflow
1 Platzieren Sie das Makro York3H1S wie in der Übung     4 Wiederholen Sie den Vorgang mit der unteren Sprosse
  Makro laden beschrieben.                                 der mittleren Raute.
2 Aktivieren Sie das Werkzeug Element auswählen.         5 Menü Datei öffnen. Menüpunkt Speichern unter auswäh-
                                                           len.
3 Markieren Sie die obere Sprosse der mittleren Raute.
  Drücken Sie die <Entf>-Taste auf Ihrer Tastatur.       6 Im Feld Dateiname York3H1S-WAII eingeben und den
                                                           Dialog mit der Schaltfläche [OK] schließen.




A+W CAD Designer (Bars) Überblick                                                          Help Cards    A-266
Spezialmuster
Eigenes Makro erstellen                                                                                    Bar 03-004




    Ziel der Handlung
Ein eigenes Makro erstellen.

    Voraussetzungen
•    Stammdaten müssen vorhanden sein.

    Zusatzinfo

    Workflow
1 Öffnen Sie im Menü Makro den Menüpunkt Neues Mak-             4 Setzen Sie die Fangpunkte am rechten und am linken
  ro. Auf Ihrem Bildschirm erscheint eine Scheibe. Die            Scheibenrand. Sie beginnen mit dem linken Scheiben-
  Scheibe hat die Maße 3 m x 3 m und hat 8 Fangpunkte             rand. Klicken Sie wieder auf Relativ und anschließend
  (je 4 am Innenrahmen und 4 an der Scheibenaußenkan-             auf den oberen Fangpunkt des linken Scheibenrandes.
  te).                                                            Es öffnet sich erneut die Dialogbox Relativer Abstand.
                                                                  Der Relativ-DX ist wieder 0. Beim Relativ-DY klicken Sie
2 Setzen Sie jetzt je einen Fangpunkt (Intervall = 2) auf den
                                                                  auf Wie andere Eingabe und anschließend auf [OK]. Es
  oberen und unteren Rahmen.
                                                                  öffnet sich die Dialogbox Auswahl vorhandener Einga-
3 Im nächsten Schritt definieren Sie den Abstand der hori-        ben. Wählen Sie den Eintrag Abstand Scheibenrand bis
  zontalen Sprosse vom Scheibenrand. Klicken Sie auf die          Sprossenmitte. Bestätigen Sie die Auswahl mit [OK].
  Schaltfläche Relativ und anschließend auf den Fang-
                                                                5 Setzen Sie nun den noch fehlenden Fangpunkt auf dem
  punkt des oberen Scheibenrandes. Es öffnet sich die Di-
                                                                  rechten Scheibenrand.
  alogbox Relativer Abstand. Unter Relativ-DX geben Sie
  den Abstand von 0 an, da sich der neue Fangpunkt auf          6 Anschließend setzen Sie die Sprossen ein. Aktivieren
  der x-Achse nicht verändert. Bestätigen Sie nun die An-         Sie zunächst die Schaltfläche Sprosse, klicken Sie dann
  gaben, werden Sie zur Eingabe von Relativ-DY aufgefor-          auf den linken und anschließend auf den rechten Fang-
  dert. Hier geben Sie den Abstand von 300 mm an. Da              punkt des Scheibenrandes. Fügen Sie nun die noch feh-
  sich die horizontale Sprosse unterhalb des Fangpunktes          lende senkrechte Sprosse ein.
  (am oberen Scheibenrand) befindet, müssen Sie eine -
                                                                7 Wählen Sie nun im Menü Makro den Eintrag Speichern.
  300 eingeben. Dieser Wert ist editierbar und wird bei er-
                                                                  Es öffnet sich der Dialog Makro speichern. Geben Sie
  neutem Laden des Makros abgefragt. Erfassen Sie bitte
                                                                  den Namen T-Sprosse ein.
  einen Text als Erklärung; in unserem Beispiel Abstand
  Scheibenrand bis Sprossenmitte.                               8 Betätigen Sie die Schaltfläche [OK]. Das Makro ist ge-
                                                                  speichert.


A+W CAD Designer (Bars) Überblick                                                                    Help Cards     A-267
Spezialmuster                          Help Cards




A-268           A+W CAD Designer (Bars) Überblick
Z   A+W CAD Designer (Bars)
    Index
A                                        – Bogenlänge I A-23
Aktionen                                 – Bogenlänge II A-23
– Rückgängig machen A-210                – Distanz A-23
– Wiederholen A-210                      – Einteilung A-23
Anischt verklenern A-241                 – Entlang Bogen A-23
Ansicht vergrößern A-241                 – Fangpunkt löschen A-22
Aufgesetzte Sprossen A-85, A-87          – Flucht A-23
Ausgabe A-14                             – Im Kreismittelpunkt (3 Punkte) A-24
                                         – Im Kreismittelpunkt (Radius) A-23
                                         – Im Rechteck A-23
B
                                         – In Kreuzungen A-23
Bearbeiteiten
                                         – In Schnittpunkten A-23
– Alles auswählen A-210
                                         – Löschen A-22
– Auswählen A-210
                                         – Mittelpunkt I A-23
Bearbeiten
                                         – Mittelpunkt II A-24
– Einschränkungen A-210
                                         – Objekt A-23
– Elemente hinzufügen A-210
                                         – Parallel A-23
– Entfernen A-210
                                         – Rechteck A-23
– Fangpunkte A-210
                                         – Relativ A-23
                                         – Richtung A-24
D                                        – Schnittpunkt A-23
Darstellungskonventionen -3              – Vektor A-24
Datei                                    Fangpunkte aktivieren A-241
– Bild exportieren A-197                 Fassadenanlage A-212
– Daten an Maschinen exportieren A-197
– Drucker einrichten A-198
                                         G
– Eine Datei öffnen A-197
                                         Glasteilende Sprossen A-85, A-86
– Eine Datei speichern A-197
– Eine neue Datei erstellen A-197
– Eine neue Datei speichern A-197        H
– Eine Übergabedatei importieren A-197   Hilfe starten A-246
– Konstruktion drucken A-197
– Nachricht senden A-198                 I
– Übergabedatei drucken A-198            Innenliegende Sprossen A-85, A-87
– Zurück zur Auftragsbearbeitung A-197
Durchgang A-85
                                         K
                                         Konstruktionsbereich A-16
E
Einstellungen öffnen A-241
                                         M
Elemente verschieben A-17
                                         Makro platzieren A-212
                                         Makros A-15
F                                        Maßeinheit A-82
Fangpunkte A-16                          – Einstellen A-83
– Alle Fangpunkt löschen A-22            Maßsystem A-75
– Alle löschen A-22                      Mauszeiger
– Anzahl ? A-23                          – Ändern der durchgehenden Sprosse A-21
– Anzahl auf Objekt erzeugen A-23        – In Verbindung mit Fangpunkten A-21
– Anzahl im Winkel erzeugen A-24         – Normal A-21
– Anzahl parallel zu erzeugen A-23       – Sprossen verlängern A-21
– Anzahl von bis erzeugen A-23           Muster senkrecht/waagerecht A-212
– Auf Bogen A-23
– Auf Gerade A-24


Z-270                                                          A+W CAD Designer (Bars)
N                                   V
Neues Makro erstellen   A-212       Vermaßung A-15, A-75
                                    – Bohrpunkte A-81
P                                   – einblenden A-76
Programminformationen A-246         – Fräspunkte anzeigen A-80, A-128
                                    – mit Pfeilen A-78
                                    – mit Ziffern A-79
R                                   Vermaßungen ein- und ausblenden A-76
Randstopfen A-85                    Vermaßungssymbole aktivieren A-242
                                    Vorausgesetzte Kenntnisse A-12
S
Sondermuster A-212                  W
Sprache                             Wegfallsprossen A-85
– auswählen A-84                    Werkzeuge A-16, A-40
– zur Laufzeit umstellen A-75       – Beispiele A-42
Sprossen bewegen A-211              – Element auswählen A-40, A-253, A-254
Sprossen drehen A-210               – Erzeugt aus Makro Sprossen-Aufteilung in der
Sprossen kopieren A-210               Scheibe A-41, A-253
Sprossen schneiden A-211            – Erzeugt eine gerade (horizontale) Sprosse
Sprossen spiegeln A-211               zwischen zwei Fangpunkten A-40, A-253,
Sprossen tauschen A-211               A-254
Sprossen teilen A-211               – Erzeugt eine gerade (vertikale) Sprosse
Sprossenabgleich A-14                 zwischen zwei Fangpunkten A-40, A-253,
Sprossenartikel aktivieren A-241      A-254
Sprossenaufteilung A-14             – Erzeugt eine gerade Sprosse zwischen zwei
Sprossendurchgang ändern A-211        Fangpunkten unter Eingabe des Winkels A-40,
Sprossentypen A-86                    A-253, A-254
Stammdaten                          – Erzeugt eine gerade Sprosse zwischen zwei
– Überblick A-232                     Fangpunkten. A-40, A-253, A-254
Stammdaten beabeiten A-232          – Erzeugt eine neue Scheibe A-41, A-253,
Stammdaten schützen A-232             A-254
Standard-Sprosse A-21               – Erzeugt eine Sonne in einem lichten
Statuszeile aktivieren A-241          Feld A-40, A-253, A-254
Strahlenmuster A-212                – Erzeugt einen Bogen in einem lichten
Strecken vermessen A-228              Feld A-41, A-253, A-254
Symbol Messen aktivieren A-241      – Erzeugt einen Halbmond A-40, A-253, A-254
Symbol Zuschnitt aktivieren A-241   – Erzeugt einen Sprossenkreis zwischen zwei
Symbole                               Fangpunkten A-40, A-253, A-254
– Alles A-19                        – Erzeugt gebogene Sprosse zwischen drei
– Ausschnitt vergrößern A-19          Fangpunkten A-40, A-253, A-254
– Ausschnitt verkleinern A-19       – Für eine 90° Kreuzung wird die
– Drucken A-18                        Durchgangsrichtung geändert A-41, A-253,
– Drucken Übergabedatei A-18          A-254
– Hilfe A-19                        – Öffnet den Dialog zur Eingabe von senkrechten
– Importieren A-18                    und waagerechten Sprossen A-41, A-253
– Neue Konstruktion A-18            – Sprosse wird bis auf wählbares Objekt
– Öffnen A-18                         verlängert A-41, A-253, A-254
– Rückgängigmachen A-19             – Teilt alle Sprossen A-41, A-253, A-254
– Speichern A-18                    – Verbindet alle Sprossen A-41, A-253, A-254
– Stammdaten öffnen A-19            – Zeigt die entsprechendenMengen im
– Wiederherstellen A-19               Wertebereich an A-41, A-253
Symbolleiste A-16                   Werkzeuge aktivieren A-241


A+W CAD Designer (Bars)                                                      Z-271
Werkzeugsymbole aktivieren A-241
Wertefenster A-16, A-20
Wertefenster aktivieren A-241

Z
Ziffern, Fräspunkte und Pfeile A-75
Zuschnitt-Informationen A-228




Z-272                                 A+W CAD Designer (Bars) Index

