---
title: "DE AWBusiness ProductionManager 2.21"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWBusiness_ProductionManager_2.21"]
version: "1.0"
last_updated: "2025-12-10"
description: "Produktionsmanager         I                              deutsch                 A+W Business Pro                                                                                                                Vorspann                                            Vorspann                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.                                          Revisionsübersicht                                        Part            Beschrei"
source_file: "DE_AWBusiness_ProductionManager_2.21.pdf"
---


# DE AWBusiness ProductionManager 2.21

Produktionsmanager         I




                         deutsch




            A+W Business Pro
                                                                                                               Vorspann




                                       Vorspann
                                       In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                       Revisionsübersicht
                                       Part            Beschreibung
                                       Version/Datum

                                       1.00/07-2013    Ersterstellung.

                                       2.00/07-2014    Anpassung: Layout, Struktur und Texte der Help Cards.

                                       2.10/02-2015    Überarbeitung.

                                       2.20/04-2016    Bruchscheiben ergänzt.

                                       2.21/01-2017    Produkt- und Firmennamen angepasst.



                                       Editorial
                                       Das Editorial enthält Informationen zu folgenden Themen:
                                       •   Anmerkungen zu diesem Dokument
                                       •   Urheberrechte
                                       •   Warenzeichen
                                       •   Kontakte

                                       Anmerkungen zu diesem Dokument
                                       Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business
                                       Pro gedacht.
                                       Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz
                                       vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden.
                                       Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
                                       ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Tex-
                                       ten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem kön-
                                       nen Fehler nicht vollständig ausgeschlossen werden. Die A+W Software
                                       GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei
                                       denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
                                       Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                I-3
                 Vorspann




                            Urheberrechte
                            © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
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

                            Kontakte
                            A+W Software GmbH

                            Am Pfahlgraben 4 - 10

                            D-35415 Pohlheim

                            Germany

                               +49 6404 2051 0

                               +6404 2051 877

                            Zentrale@a-w.com

                            http://www.a-w.com
2.21 / 01-2017




                 I-4                                            A+W Business Pro Production Manager
                                                                                                                                                             Inhalt




                                       Inhalt
                                       Vorspann ................................................................................................................. I-3
                                        Revisionsübersicht ............................................................................................... I-3
                                        Editorial ................................................................................................................ I-3

                                       Tutorial                                                                                                                I-7
                                       Überblick .................................................................................................................. I-9
                                         Dokumentation ................................................................................................... I-10
                                           Aufbau des Tutorials ....................................................................................... I-10
                                           Darstellungskonventionen ............................................................................... I-11
                                       Grundgedanken zum Produktionsmanager ........................................................... I-12
                                         Die Oberfläche ................................................................................................... I-13
                                           Standardmodus ............................................................................................... I-13
                                           Expertenmodus ............................................................................................... I-13
                                       Standardmodus ..................................................................................................... I-14
                                         Überblick ............................................................................................................ I-15
                                           Standardmodus starten ................................................................................... I-16
                                           Lauf bilden ...................................................................................................... I-17
                                           Lauf feinplanen ............................................................................................... I-17
                                           Ausgaben ........................................................................................................ I-18
                                           Ergebnisse ...................................................................................................... I-19
                                           Lagerplatten und Optimierungsparameter ...................................................... I-21
                                           Informationen .................................................................................................. I-22
                                       Expertenmodus ...................................................................................................... I-23
                                         Überblick ............................................................................................................ I-24
                                           Expertenmodus starten ................................................................................... I-25
                                         Auftragsselektion ................................................................................................ I-26
                                           Aufträge auswählen ........................................................................................ I-27
                                           Die Bereiche Aufträge und Positionen ............................................................ I-28
                                           Daten gruppieren ............................................................................................ I-30
                                             Daten sortieren ............................................................................................ I-30
                                           Daten übersichtlich darstellen ......................................................................... I-32
                                           Produkt ............................................................................................................ I-34
                                           Informationen .................................................................................................. I-34
                                           Bruchscheiben ................................................................................................ I-35
                                             Bruch erfassen ............................................................................................ I-35
                                             Einen Bruchlauf bilden ................................................................................. I-36
                                           Mit Bruch arbeiten ........................................................................................... I-37
                                         Läufe verwalten .................................................................................................. I-39
                                           Allgemein ........................................................................................................ I-40
                                           Läufe über bestimmte Kriterien auswählen ..................................................... I-44
                                           Detailansicht für Läufe .................................................................................... I-46
                                           Register Produkt und Zuschnitt ....................................................................... I-48
                                         Feinplanung ........................................................................................................ I-50
                                           Ablauf der Feinplanung ................................................................................... I-51
                                           Optimierungsmanager .................................................................................... I-52
                                           Läufe optimieren ............................................................................................. I-54
                                           Temporäre Optimierung .................................................................................. I-55
                                           Optimierung abbrechen .................................................................................. I-58
                                         Optimierungsübersicht ....................................................................................... I-59
                                           Detailansicht Optimierung ............................................................................... I-62
2.21 / 01-2017




                                         Ausgabe ............................................................................................................. I-63
                                           Reports und Schneidcodes ............................................................................. I-64
                                           Daten ausgeben .............................................................................................. I-68



                 A+W Business Pro Production Manager                                                                                                             I-5
                 Inhalt




                          Stammdaten .......................................................................................................... I-69
                            Abstellplätze ....................................................................................................... I-70
                              Logische Abstellplätze und Abstellplatztiefe ................................................... I-71
                              Abstellmodus für A-Böcke ............................................................................... I-72
                                Auffangabstellplatz ...................................................................................... I-73
                              Abstellplatzgruppen ........................................................................................ I-76
                              Mit Abstellplatzgruppen arbeiten ..................................................................... I-77
                              Kriterien ........................................................................................................... I-78
                                Formel ......................................................................................................... I-79
                              Mit Kriterien arbeiten ....................................................................................... I-80
                              Sortierschlüssel ............................................................................................... I-81
                              Mit Sortierschlüsseln arbeiten ......................................................................... I-82
                              Abstellplatzorganisation .................................................................................. I-83
                            Gruppierung und Sortierung ............................................................................... I-85
                              Allgemein ........................................................................................................ I-86

                          Softwarereferenz                                                                                                     I-87
                          Übersicht ................................................................................................................ I-89
                            Abstellplatzorganisation ..................................................................................... I-90
                            Kriterien .............................................................................................................. I-93
                            Logische Abstellplätze ........................................................................................ I-95
                            Abstellplatzgruppen ............................................................................................ I-97
                            Sortierschlüssel .................................................................................................. I-98
                          Standardmodus ..................................................................................................... I-99
                            Assistenten ....................................................................................................... I-100
                          Expertenmodus .................................................................................................... I-104
                            Auftragsselektion .............................................................................................. I-105
                            Ansicht speichern ............................................................................................. I-110
                            Produkt ............................................................................................................. I-111
                            Bruchpositionen ................................................................................................ I-113
                            Bruch erfassen ................................................................................................. I-116
                            Neuen Lauf erstellen ........................................................................................ I-117
                            Laufübersicht .................................................................................................... I-119
                            Detailansicht ..................................................................................................... I-121
                            Zuschnitt ........................................................................................................... I-123
                            Zuschnitt bearbeiten ......................................................................................... I-125
                            Laufstatus setzen ............................................................................................. I-127
                            Aggregatumlastung .......................................................................................... I-128
                            Optimierungsmanager ...................................................................................... I-130
                            Optimierung abbrechen .................................................................................... I-132
                            Temporäre Optimierung ................................................................................... I-133
                            Optimierungsübersicht ..................................................................................... I-135
                            Detailansicht Optimierung ................................................................................ I-137
                            Ausgabe ........................................................................................................... I-138
                            Druckeinstellungen ........................................................................................... I-141
                            Auftragssuche .................................................................................................. I-143

                          Partindex                                                                                                         I-145
                          Index .................................................................................................................... I-147
2.21 / 01-2017




                 I-6                                                                  A+W Business Pro Production Manager
Produktionsmanager         I

                      Tutorial




            A+W Business Pro
                 Tutorial                                                                                   Überblick




                                       Überblick
                                       Das Tutorial zum Modul Produktionsmanager beschäftigt sich mit den Grund-
                                       lagen der Produktionslösung in A+W Business Pro. Das Tutorial baut auf den
                                       Kenntnissen zu den Stammdaten und zum Nummernverwalter auf.

                                           Funktionen sind von den freigeschalteten Modulen abhängig
                                           Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                           Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                           liert und freigeschaltet sind.

                                           Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                           on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                           GmbH.

                                       Themenblöcke
                                       In diesem Tutorial finden Sie folgende Themenblöcke:
                                       •   Grundgedanken zum Produktionsmanager
                                       •   Standardmodus
                                       •   Expertenmodus

                                       Vorausgesetzte Kenntnisse
                                       Das Tutorial richtet sich an Teilnehmer, die in A+W Business Pro Aufträge zur
                                       Produktion vorbereiten. Die Teilnehmer müssen das Konzept der Stammdaten
                                       und des Nummernverwalters kennen.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-9
                 Überblick                                                                              Tutorial




                             Dokumentation
                             Für das Modul Production Manager stehen folgende Dokumente zur Verfü-
                             gung:

                             Handout                     Ausdruck des Tutorials für die Schulung

                             PDF                         Vollständige Unterlagen
                                                         • Tutorial
                                                         • Softwarereferenz
                                                         • Index

                             Online-Hilfe <F1>           Kontextsensitive Dialog-Hilfe der A+W Business-
                                                         Softwarereferenzen und Tutorials der Basisversion


                             Aufbau des Tutorials
                             Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinhei-
                             ten. Jede Lerneinheit besteht aus folgenden Komponenten:

                             Überblick                   Jede Lerneinheit beginnt mit einem Überblick über die
                                                         wichtigsten Inhalte:
                                                         • Lernziele: Was soll vermittelt werden?
                                                         • Nutzen: Wofür können Sie dieses Wissen einsetzen?
                                                         • Merksätze: Welche Zusammenhänge müssen Sie
                                                           sich merken?

                             Konzepte                    Konzepte und Begriffe der jeweiligen Lerneinheit
                                                         werden zunächst erläutert. Danach finden Sie Beispiele
                                                         und Handlungsanleitungen.

                             Übungen                     Zu einigen Lerneinheiten finden Sie Übungen mit
                                                         Aufgabenstellungen und Lösungsvorschlägen.

                             Querverweise                Am Ende jeder Lerneinheit finden Sie einen Abschnitt
                                                         mit Querverweisen, die auf ergänzende Informationen in
                                                         der Softwarereferenz und in anderen Parts hinweisen.
                                                         Damit können Sie das neu erworbene Wissen vertiefen.


                             Lesehinweis
                             Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der
                             vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine
                             Lerneinheiten zu überspringen.
                             Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die
                             Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu
                             vergegenwärtigen.
2.21 / 01-2017




                 I-10                                                A+W Business Pro Production Manager
                 Tutorial                                                                                     Überblick




                                       Darstellungskonventionen
                                       Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                       gende Bedeutung:

                                       Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                                Software bezeichnen, z. B. der Dialog
                                                                Nummernverwalter.

                                       Fett                     sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                                Tastatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                                       >                        Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                                kennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                                Fertigung > Produktion > Produktionsübergabe.

                                       []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                z. B.: Mit [OK] speichern Sie die Daten.

                                       <>                       Spitze Klammern bezeichnen Tasten oder
                                                                Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                                öffnen Sie die Online-Hilfe.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                  I-11
                 Grundgedanken zum Produktionsmanager                                                             Tutorial




                                      Grundgedanken zum Produk-
                                      tionsmanager
                                      Aufgabe des Produktionsmanageres ist es, Sie im Planungs- und Vorberei-
                                      tungsprozess für die Produktion zu unterstützen - von der Laufbildung bis hin
                                      zum Druck von Produktionspapieren und dem Erzeugen vom Maschinencode.
                                      Der Prozessablauf stellt sich wie folgt dar:


                                       Auftrags-           Laufbildung   Abstellplatz-   Optimierung   Freigabe
                                       Teileselektion                    organisation


                                      Abb. I-1          Standardprozess für Produktionslösung


                                      Die Aufträge werden automatisiert über einen vordefinierten Status oder ma-
                                      nuell durch den Anwender für die interne Kapazitätsplanung freigegeben. In
                                      diesem Zuge wird eine Tabelle mit allen erforderlichen Daten gefüllt. Auf diese
                                      Daten greift dann der Production Manager zu.
                                      Der Prozess wird in einem einzigen Dialog abgebildet, so dass für den Anwen-
                                      der ein Hin- und Herspringen nicht nötig ist.
                                      Das Modul befindet sich im Bereich Fertigung > Produktion:




                                      Abb. I-2          Der Produktionsmanager im Menü von A+W Business
2.21 / 01-2017




                 I-12                                                              A+W Business Pro Production Manager
                 Tutorial                                                 Grundgedanken zum Produktionsmanager




                                       Die Oberfläche
                                       Der Production Manager kann auf zwei unterschiedliche Weisen bedient wer-
                                       den:
                                       •   Standardmodus
                                       •   Expertenmodus


                                       Standardmodus
                                       In diesem Modus kann das Programm über eine vereinfachte Benutzerfüh-
                                       rung, den sogenannten Wizard bedient werden.
                                       Mittels des Wizards ist es möglich, den Gesamtprozess (Laufbildung, Optimie-
                                       rungen, etc.) mit wenigen Eingaben zu durchlaufen. Es werden am Ende des
                                       Prozesses die Optimierungsergebnisse angezeigt und Sie können entschei-
                                       den, ob Sie den Lauf und Optimierungsergebnisse akzeptieren.
                                       Den Standardmodus aktivieren Sie, indem Sie die entsprechende Symbol-
                                       Schaltfläche betätigen.
                                        “Standardmodus” auf Seite I-13


                                       Expertenmodus
                                       In diesem Modus werden die einzelnen Schritte (Laufbildung, Optimierungen,
                                       etc.) vom Benutzer manuell ausgeführt. Sie können so sehr detailliert und se-
                                       lektiv Einfluss nehmen auf die einzelnen Prozessschritte der Laufbildung und
                                       -verarbeitung.
                                       Den Expertenmodus aktivieren Sie, indem Sie die entsprechende Symbol-
                                       Schaltfläche betätigen.
                                        “Expertenmodus” auf Seite I-13
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-13
                 Standardmodus                                                                    Tutorial




                                 Standardmodus
                                 In diesem Themenblock lernen Sie, wie Sie den Umgang mit dem Production
                                 Manager im Standardmodus.
                                 Dazu gehören folgende Lerneinheiten:
                                 •   “Standardmodus starten” auf Seite I-16
                                 •   “Lauf bilden” auf Seite I-17
                                 •   “Lauf feinplanen” auf Seite I-17
                                 •   “Ausgaben” auf Seite I-18
                                 •   “Ergebnisse” auf Seite I-19
                                 •   “Lagerplatten und Optimierungsparameter” auf Seite I-21
2.21 / 01-2017




                 I-14                                                A+W Business Pro Production Manager
                 Tutorial                                                                               Standardmodus




                                       Überblick
                                       Lernziele

                                       • Standardmodus (Wizard) kennenlernen und verstehen


                                       Nutzen

                                       • Mit dem Wizard können Sie den Gesamtprozess mit nur wenigen Mausklicks
                                         durchlaufen. Das spart Zeit und minimiert das Fehlerrisiko.


                                       Merke

                                       Standardmodus              Der Produktionsmanager wird immer im Standardmodus
                                                                  geöffnet.

                                       Abstellplatzorganisation   Wird mit der Standard-Organisation aus den
                                                                  Stammdaten vorbelegt. Es kann eine andere gewählt
                                                                  werden.

                                       Abstellplatztiefe          Durch die Veränderung dieses Wertes hat man Einfluss
                                                                  auf das Optimierungsergebnis.

                                       Variante                   Die durchgeführten Varianten bleiben erhalten. Sie
                                                                  können sich so für die beste Variante entscheiden.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                   I-15
                 Standardmodus                                                                              Tutorial




                                        Standardmodus starten
                                        Der Produktionsmanager wird beim Starten im Standardmodus geöffnet. Aus
                                        dem Expertenmodus heraus können Sie in den Standardmodus wechseln, in-
                                        dem Sie die entsprechende Symbol-Schaltfläche betätigen. In diesem Modus
                                        präsentiert sich das Programm wie folgt:




                 Abb. I-3   Hauptdialog – Standardmodus


                                        Im Standardmodus kann das Programm über eine vereinfachte Benutzerfüh-
                                        rung (Wizard) bedient werden.
                                        Mittels des Wizards ist es möglich, den Gesamtprozess (Laufbildung, Optimie-
                                        rung, etc.) mit wenigen Eingaben zu starten. Es werden am Ende des Prozes-
                                        ses die Optimierungsergebnisse angezeigt und Sie können entscheiden, ob
                                        Sie den Lauf und Optimierungsergebnisse so akzeptieren (speichern) oder mit
                                        anderen Einstellungen wiederholen, um ein besseres Ergebnis zu erzielen.
2.21 / 01-2017




                 I-16                                                      A+W Business Pro Production Manager
                 Tutorial                                                                            Standardmodus




                                       Lauf bilden
                                       Im ersten Schritt wählen Sie einen Nummernverwalter (NV) aus. Alle Aufträge,
                                       welche in diesem NV enthalten sind, werden in einem Lauf zusammengefasst.
                                       Im Nummernverwalter fassen Sie diejenigen Aufträge zusammen, die später
                                       im Produktionsmanager in einem Lauf verarbeitet werden sollen.




                                       Abb. I-4     Bereich Laufbildung


                                       Die Lauf-Nummer wird automatisch vom System vergeben und kann nicht ge-
                                       ändert werden. Im Feld Status wird Ihnen der Status des Laufs angezeigt. Im
                                       Beispiel oben ist der Status Feingeplant, d. h. der Lauf hat die Feinplanung
                                       durchlaufen. Im Feld Beschreibung sehen Sie den Namen des Nummernver-
                                       walters, den Benutzer sowie das Datum der Laufbildung.
                                       Der Bereich Laufinhalt wird erst nach der Laufbildung gefüllt. Sie sehen dann,
                                       wie viele ISO, VSG, ESG und bearbeitete Gläser der Lauf enthält.


                                       Lauf feinplanen
                                       Im zweiten Schritt nehmen Sie die Einstellungen für die Feinplanung und Op-
                                       timierung vor. D. h. Sie wählen mittels der Kombobox eine vordefinierte Ab-
                                       stellplatzorganisation aus. Nun können Sie noch die Tiefe des Abstellplatzes
                                       einstellen.
                                       Die Verwaltung der Abstellplatzorganisationen und Abstellplatztiefe nehmen
                                       Sie in den Stammdaten vor (Stammdaten > Fertigung > Abstellplatzorganisa-
                                       tion).




                                       Abb. I-5     Bereich Feinplanung
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-17
                 Standardmodus                                                                         Tutorial




                                 Wenn man für die Abstellpatztiefe einen Bereich einstellt (z. B. 80-120 %),
                                 dann definiert das Feld Anzahl Varianten wie viele Varianten durch das Klicken
                                 auf die Symbol-Schaltfläche [Ausführen] entstehen. Beispiel:
                                 •   Abstellplatztiefe: 80 - 120 %
                                 •   Anzahl Varianten: 5
                                 •   Feinplanung mit 80, 90, 100 110 und 120 % Gestelltiefe.


                                 Ausgaben
                                 Über diesen Bereich werden alle Ausgaben, unabhängig davon, ob es sich um
                                 Ausgaben auf Papier oder in Dateiform handelt, eingestellt. Die Kombobox
                                 bietet Ihnen folgende Auswahlen:
                                 •   Keine: Es finden keine Ausgaben statt.
                                 •   Alle: Es werden folgende Medien ausgegeben:
                                     – Produktionslisten für den Lauf
                                     – Etiketten für den Lauf
                                     – Maschinenansteuerung für den Lauf
                                     – Standardlisten für die Optimierung (Rahmenbieger, ISO-Linie)
                                     – Schneidpläne für die Optimierung
                                     – Zuschnittetiketten für die Optimierung
                                     – Maschinenansteuerung für die Optimierung (Zuschnitttisch)
                                 •   Auswahl: Hier können Sie manuell die unter Punkt Alle aufgelisteten Medi-
                                     en aktivieren.




                                 Abb. I-6     Bereich Speichern
2.21 / 01-2017




                 I-18                                                 A+W Business Pro Production Manager
                 Tutorial                                                                           Standardmodus




                                       Ergebnisse
                                       Im Bereich Optimierungen werden Ihnen die möglichen Optimierungen ange-
                                       zeigt. Die Tabelle enthält erst dann Daten, wenn der Lauf gebildet und die
                                       Feinplanung durchlaufen wurde. Sie können wählen, welchen Glasarten Sie
                                       in welcher Reihenfolge optimieren möchten oder auch einzelne Glasarten auf
                                       Handzuschnitt setzen:




                                       Abb. I-7    Bereich Optimierungen


                                       Nachdem Sie die Symbol-Schaltfläche [Ausführen] betätigt haben, wird der
                                       vorgeschlagene Lauf erst grobgeplant und dann feingeplant. Anschließend
                                       werden nacheinander die Optimierungen der einzelnen Gläser in der ange-
                                       zeigten Reihenfolge durchgeführt.
                                       Nachdem Sie alle Optimierungen durchgeführt haben, können Sie diese über
                                       die Symbol-Schaltfläche [Speichern] speichern. Die gebildeten Läufe und
                                       durchgeführten Optimierungen werden in der Datenbank gespeichert.

                                          Ausgaben werden angestoßen
                                          Wenn Sie die Schaltfläche [Speichern] betätigen, werden ebenfalls alle ak-
                                          tivierten Ausgaben mit angestoßen inkl. Übergabe der Daten an die ent-
                                          sprechenden Maschinen.

                                       Erläuterung der Felder im Bereich Gesamtergebnis
                                       Im Bereich Gesamtergebnis werden Ihnen die verschiedenen Optimierungs-
                                       varianten angezeigt. Mittels verschiedener Einstellungen (bspw. Abstellplatz-
                                       tiefe, oder welche Glasart als erste optimiert wird), können Sie verschiedene
                                       Ergebnisse in der Optimierung erzeugen / berechnen (verschiedene Varian-
                                       ten). Aus diesen Varianten können Sie dann im nächsten Schritt die Beste
                                       auswählen und speichern. So werden die Ausgaben (Papiere und Maschinen-
                                       codes) nur für diese ausgewählte Variante erzeugt. Die Tabelle enthält erst
                                       dann Daten, wenn der Lauf gebildet und die Feinplanung und die Optimierung
                                       durchlaufen wurde:




                                       Abb. I-8    Bereich Gesamtergebnis
2.21 / 01-2017




                                       Das Feld Variante zeigt Ihnen, wie oft Sie die Feinplanung und die Optimie-
                                       rung durchlaufen haben. Mit jedem Klick auf die Symbol-Schaltfläche [Ausfüh-


                 A+W Business Pro Production Manager                                                           I-19
                 Standardmodus                                                                          Tutorial




                                 ren] wird eine weitere Variante erzeugt und dort gelistet. Die einzelnen
                                 Varianten bleiben Ihnen erhalten, so dass Sie sich schlussendlich für die beste
                                 Variante entscheiden können.
                                 Im Feld Abstellplatzorganisation wird Ihnen die verwendete Abstellplatzorga-
                                 nisation angezeigt. Es handelt sich dabei um die Abstellplatzorganisation, die
                                 Sie im Bereich Feinplanung und Optimierung ausgewählt haben (der Wert
                                 kommt aus den Stammdaten: Fertigung > Abstellplatzorganisation).
                                 Bei dem Feld Faktor handelt es sich um den Faktor der Abstellplatztiefe, den
                                 Sie im Bereich Feinplanung eingestellt haben.
                                 Werden die Gläser in Fächerwagen gestellt, wird Ihnen im Feld Anzahl Fä-
                                 cherwagen angezeigt, wie viele Fächerwagen nötig sind, um alle Gläser des
                                 Laufs abzustellen. Kommen die Gläser auf A-Böcke, sehen Sie im Feld Anzahl
                                 A-Böcke, wie viele A-Böcke dazu nötig sind.
                                 Im Feld Ergebnis wird Ihnen das Gesamtergebnis der Variante in % angezeigt
                                 und das Feld Verschnitt zeigt Ihnen den Gesamt-Verschnitt der Variante in Eu-
                                 ro.




                                 Abb. I-9     Bereich Optimierung je Variante


                                 Das Feld Optimierung zeigt Ihnen pro Variante die entsprechenden Optimie-
                                 rungen.
                                 Im Feld Glasart werden Ihnen die im Lauf enthaltenen Glasarten angezeigt.
                                 Die Ziffer davor zeigt Ihnen die Reihenfolge in der Optimierung. Anschließend
                                 sehen Sie den Schneidtisch, auf dem das Glas geschnitten wird, gefolgt von
                                 der Laufnummer. Im Feld Stückzahl wird Ihnen je Glasart die Stückzahl ange-
                                 zeigt und im nächsten Feld die Fläche in Quadratmetern.
                                 Im Feld Ergebnis wird Ihnen das Ergebnis der Optimierung für die jeweilige
                                 Glasart angezeigt. Zunächst sehen Sie das Ergebnis in %. Dahinter wird Ihnen
                                 in Klammern angezeigt, wie viele Muster und wie viele Lagerplatten die Opti-
                                 mierung benötigt sowie die verbleibende Restblattenlänge. Sollte der Produk-
                                 tionsmanager eine Glasart automatisch auf Handzuschnitt setzen, liegt das
                                 daran, dass die in den Stammdaten eingestellte Mindestfläche für die Optimie-
                                 rung nicht erreicht wird.
                                 Anschließend wird Ihnen der Verschnitt in Euro angezeigt.
2.21 / 01-2017




                 I-20                                                  A+W Business Pro Production Manager
                 Tutorial                                                                              Standardmodus




                                       Lagerplatten und Optimierungsparameter
                                       Am rechten Bildschirmrand befinden sich zwei weitere Register, die bei Bedarf
                                       aufgeklappt werden können:
                                       •   Register Lagerplatten
                                       •   Register Optimierungsparameter

                                           Register Lagerplatten und Optimierungsparameter
                                           Nachdem Sie die Feinplanung und die Optimierung für einen Lauf durch-
                                           laufen haben, sind auch die Register Lagerplatten und Optimierungspara-
                                           meter gefüllt.

                                       Klicken Sie mit der Maus das Register Lagerplatten an, wird dieses geöffnet:




                                       Abb. I-10    Register Lagerplatten, am rechten Bildschirmrand


                                       Dieses Register liefert Ihnen alle Informationen zu den Lagerplatten der ent-
                                       sprechenden Glasart. Die hier angezeigten Werte werden im Modul Lager ver-
                                       waltet.
                                       Klicken Sie mit der Maus das Register Optimierungsparameter an, wird dieses
                                       geöffnet:
2.21 / 01-2017




                                       Abb. I-11    Register Optimierungsparameter, am rechten Bildschirmrand



                 A+W Business Pro Production Manager                                                            I-21
                 Standardmodus                                                                          Tutorial




                                 Dieses Register liefert Ihnen alle Informationen zu der Optimierung der ent-
                                 sprechenden Glasart. Die hier angezeigten Werte kommen aus den Stamm-
                                 daten (Artikel > Artikel).
                                 Im Bereich Allgemeine Einstellungen können Sie zwischen folgenden Opti-
                                 mierungsmodi wählen:
                                 •   XOPT: Bei dieser Variante erfolgt die Optimierung chaotisch. D. h, die Rei-
                                     henfolge der Scheiben nach der Optimierung ist nicht wichtig, die Scheiben
                                     einer Position müssen nicht zusammengehalten werden. Dadurch erzielt
                                     man zwar ein besseren Verschnitt, es müssen allerdings vor der ISO-Pro-
                                     duktion alle Scheiben auf den A-Böcken umsortiert werden.
                                 •   XOPT-S: Dies ist der Standard-Modus für ISO-Betriebe. Hier wird die in der
                                     Abstellplatzorganisation vorgegebene Reihenfolge der Scheiben auf den
                                     Abstellplätzen eingehalten. Eine Synchronoptimierung der Scheiben ist
                                     möglich, damit Scheibe und Gegenscheibe auf der ISO-Linie zusammen-
                                     passen. Die Scheiben einer Auftragsposition stehen nach der Optimierung
                                     immer zusammen auf einem A-Gestell, d. h. die Position wird nicht gesplit-
                                     tet.

                                     Register Lagerplatten und Optimierungsparameter
                                     Nachdem Sie die Feinplanung und die Optimierung für einen Lauf durch-
                                     laufen haben, sind auch die Register Lagerplatten und Optimierungspara-
                                     meter gefüllt.


                                 Informationen
                                 In diesem Bereich haben Sie die Möglickeit, einen Auftrag über dessen Num-
                                 mer gezielt zu suchen. Öffnen Sie hierzu das Menü Informationen und dann
                                 den Eintrag Auftrag suchen. Geben Sie die Auftragsnummer ein, die entspre-
                                 chenden Daten werden angezeigt.


                                  So finden Sie Aufträge
                                 1 Öffnen Sie im Menü den Eintrag Informationen.
                                 2 Betätigen Sie die Symbol-Schaltfläche [Auftrag]. Es öffnet sich die Auf-
                                   tragssuche.
                                 3 Geben Sie im Feld Auftragsnummer die gewünschte Nummer ein.
                                 4 Betätigen Sie die Symbol-Schaltfläche [Filter].


                                 Ergänzende Informationen
                                  Softwarereferenz, “Auftragssuche” auf Seite I-143
2.21 / 01-2017




                 I-22                                                  A+W Business Pro Production Manager
                 Tutorial                                                                    Expertenmodus




                                       Expertenmodus
                                       In diesem Themenblock lernen Sie den Umgang mit dem Produktionsmana-
                                       ger im Expertenmodus.
                                       Dazu gehören folgende Lerneinheiten:
                                       •   “Überblick” auf Seite I-24
                                       •   “Auftragsselektion” auf Seite I-26
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                   I-23
                 Expertenmodus                                                                              Tutorial




                                 Überblick
                                 Lernziele

                                 • Die Ansicht kennenlernen
                                 • Wie werden die Daten geladen.
                                 • Die Inhalte der Anzeigen übersichtlich aufbereiten.


                                 Nutzen

                                 • Im Expertenmodus führen Sie die einzelnen Schritte wie Läufe bilden, optimieren,
                                   etc. selber durch. Somit haben Sie die Möglichkeit über verschiedene Varianten
                                   zum bestmöglichen Ergebnis zu gelangen.


                                 Merke

                                 Expertenmodus               In den Expertenmodus muss explizit umgeschaltet
                                                             werden.
2.21 / 01-2017




                 I-24                                                    A+W Business Pro Production Manager
                 Tutorial                                                                             Expertenmodus




                                         Expertenmodus starten
                                         Den Expertenmodus starten Sie, indem Sie die entsprechende Symbol-
                                         Schalftläche betätigen. Er ist unter anderem für die mehrstufige Produktion
                                         von Gläsern gedacht. Sie nehmen alle notwendigen Schritte, wie z. B. die Zu-
                                         sammenstellung der einzelnen Läufe selbst vor. Sie können so Läufe bspw.
                                         aus verschiedenen Aufträgen und basierend auf spezifischen Bearbeitungs-
                                         schritten zusammenstellen, oder aber aus verschiedenen Läufen eine ge-
                                         meinsame Optimierung starten. In diesem Modus präsentiert sich das
                                         Programm wie folgt:




                 Abb. I-12   Hauptdialog, Expertenmodus


                                         Der Production Manager besteht aus dem Hauptdialog mit verschiedenen Re-
                                         gistern. Folgende Hauptregister stehen zur Verfügung:
                                         •   Auftragsselektion
                                         •   Laufübersicht
                                         •   Optimierungsmanager
                                         •   Optimierungsübersicht
                                         •   Ausgabe
                                         Neben den Hauptregistern gibt es noch Register, die während der Laufzeit ein-
2.21 / 01-2017




                                         geblendet werden. Dazu zählt z. B. die Detailansicht, die Sie aus dem Regis-
                                         ter Laufansicht öffnen können. Diese Ansicht erscheint dann rechts neben
                                         dem Register Laufansicht.



                 A+W Business Pro Production Manager                                                             I-25
                 Expertenmodus                                                                        Tutorial




                                 Auftragsselektion
                                 In der Auftragsselektion können Sie über verschiedene Selektionskriterien
                                 Stücklistenteile einer Auftragsposition zu einem Lauf zusammenfassen. Sie
                                 dienen dazu, die Menge der Aufträge/Auftragspositionen/Stücklistenteile ein-
                                 zuschränken, die für die Laufbildung herangezogen werden sollen. Wird ein
                                 Auftrag selektiert, werden alle Positionen des Aufrags selektiert. Sie können
                                 jedoch einzelne Positionen an- und abwählen. Wählen Sie im Bereich Positi-
                                 onen eine Position aus, wird im Bereich Aufträge der entsprechende Auftrag
                                 ausgewählt.
                                 Der Dialog ist in mehrere Bereiche eingeteilt. Rechts oben befindet sich die
                                 Liste der zu optimierenden Gläser. Hierüber können Sie sehen, wie groß der
                                 Lauf wird. Im unteren Bereich werden Ihnen Auftrags- und Positionsdaten zur
                                 Selektion angezeigt.




                                 Abb. I-13    Selektionskriterien


                                 Bei der Selektion können Sie wählen zwischen dem Nummernverwalter und
                                 dem Arbeitsgang. Innerhalb des Arbeitsganges können Sie zusätzlich auf das
                                 Produktionsdatum filtern.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Auftragsselektion” auf Seite I-105
2.21 / 01-2017




                 I-26                                                   A+W Business Pro Production Manager
                 Tutorial                                                                           Expertenmodus




                                       Aufträge auswählen
                                       In dieser Einheit lernen Sie, wie Sie Aufträge für den Produktionsmanager
                                       auswählen.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So selektieren Sie Aufträge über den Nummernverwalter
                                       •   So selektieren Sie Aufträge über den Arbeitsgang
                                       •   So finden Sie Aufträge


                                        So selektieren Sie Aufträge über den Nummernverwalter
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Be-
                                         arbeitung freigegeben.
                                       2 Aktivieren Sie die Radiotaste Nummernverwalter.
                                       3 Öffnen Sie die Kombobox.
                                       4 Wählen Sie einen entsprechenden NV aus.
                                       5 Betätigen Sie die Symbol-Schaltfläche [Suchen].
                                       6 Die Daten werden geladen.


                                        So selektieren Sie Aufträge über den Arbeitsgang
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Be-
                                         arbeitung freigegeben.
                                       2 Aktivieren Sie die Radiotaste Arbeitsgang.
                                       3 Öffnen Sie die Kombobox.
                                       4 Wählen Sie einen entsprechenden Arbeitsgang aus.
                                       5 Wenn nötig, verwenden Sie die Datumsfelder von und bis, um die Auswahl
                                         einzugrenzen. Diese Felder stehen in Zusammenhang mit der Auswahl,
                                         die Sie im Feld Arbeitgang getroffen haben. Sie haben hier die Möglichkeit,
                                         den Arbeitsgang mit einem Datum einzugrenzen. Dieses Datum bezieht
                                         sich dann auf das Produktionsdatum. Bsp.: Arbeitsgang Bohren, Produkti-
                                         onsdatum 15.06.2013 bis 20.06.2013. Haben Sie als Arbeitsgang Versand
                                         gewählt, ist das eingegebene Datum das Versanddatum.
                                       6 Betätigen Sie die Symbol-Schaltfläche [Suchen].
                                       7 Die Daten werden geladen.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Auftragsselektion” auf Seite I-105
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-27
                 Expertenmodus                                                                         Tutorial




                                 Die Bereiche Aufträge und Positionen
                                 In diesen Bereichen werden Ihnen die Daten gemäß den Einstellungen im Be-
                                 reich Selektionskriterien angezeigt. Der Bereich Aufträge gibt Ihnen einen
                                 Überblick zu den Aufträgen mit Auftragsnummer, Kundennummer, etc.
                                 Die Inhalte des Bereichs Positionen sind abhängig von den Selektionskriteri-
                                 en. Um dies zu verdeutlichen, zeigen wir Ihnen im Anschluss zwei Beispiele.
                                 Wir verwenden immer den selben Auftrag, jedoch lassen wir uns diesen in Be-
                                 zug auf unterschiedliche Arbeitsgänge anzeigen.
                                 Wählen wir als Selektion den Eintrag ISO-Fertigen, werden folgende Daten
                                 angezeigt:




                                 Abb. I-14    Arbeitsgang ISO-Fertigen


                                 Im Bereiche Aufträge werden Ihnen alle Aufträge angezeigt, welche Positio-
                                 nen enthalten die gesäumt werden müssen (oder eben gebohrt). Wir wählen
                                 den Auftrag 20143 aus.
                                 Im Bereich Positionen werden nun die einzelnen Positionen des Auftrags
                                 20143 markiert, welche gesäumt werden müssen. Dabei ist zu beachten, dass
                                 alle Auftragspositionen eines Auftrages selektiert und in der Auswahlliste ge-
                                 sperrt sind, sobald Sie im Bereich Aufträge einen Auftrag auswählen und mar-
                                 kieren.
                                 Hier könnten wir nun einzelne Positionen auswählen und diese für einen eige-
                                 nen Lauf berücksichtigen. Dazu müssen Sie im Bereich Aufträge zunächst die
                                 Markierung des Auftrags aufheben, und dann die relevanten Auftragspositio-
                                 nen im Bereich Positionen einzeln markieren (selektieren).
2.21 / 01-2017




                                 Wählen wir als Selektion den Eintrag Zuschneiden, werden folgende Daten
                                 angezeigt:


                 I-28                                                    A+W Business Pro Production Manager
                 Tutorial                                                                            Expertenmodus




                                       Abb. I-15    Arbeitsgang Zuschneiden


                                       Im Bereich Positionen sehen Sie jetzt alle einzelnen Gläser, die zugeschnitten
                                       werden müssen.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Auftragsselektion” auf Seite I-105
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-29
                 Expertenmodus                                                                       Tutorial




                                 Daten gruppieren
                                 Es kann unter Umständen vorkommen, dass eine große Anzahl von Daten an-
                                 gezeigt wird. Um dennoch den Überblick zu behalten, haben Sie Möglichkeit,
                                 die Daten zu gruppieren und innerhalb der Gruppierung zu sortieren. Das
                                 Gruppieren von Daten ist für die Bereiche Aufträge und Positionen identisch.
                                 Um doppelte Beschreibungen zu vermeiden, wird die Vorgehensweise am
                                 Beispiel der Aufträge erläutert.
                                 Die Gruppierungen nehmen Sie im Tabellenkpf vor:




                                 Abb. I-16    Daten gruppieren


                                 Über die Symbol-Schaltfläche [Spaltenauswahl] öffnen Sie ein Fenster, das
                                 alle Spalten enthält, nach denen gruppiert werden kann. Die folgende Grafik
                                 zeigt eine kleine Auswahl der Spalten.




                                 Abb. I-17    Spaltenauswahl


                                 Daten sortieren
                                 Um Daten innerhalb einer Gruppierung auf- oder absteigend zu sortieren, ste-
                                 hen Ihnen die Pfeile am Ende der Spalte zur Verfügung:
                                 sortiert die Daten aufsteigend
                                 sortiert die Daten absteigend.
                                 Ist am Ende der Spalte kein Pfeil, erfolgt keine Sortierung.
                                 Die Gruppierungen nehmen Sie in folgendem Bereich vor:
2.21 / 01-2017




                                 Abb. I-18    Daten gruppieren



                 I-30                                                 A+W Business Pro Production Manager
                 Tutorial                                                                           Expertenmodus




                                       Daten übersichtlich darstellen
                                       In dieser Einheit lernen Sie, wie Sie angezeigten Daten durch Gruppieren
                                       übersichtlich darstellen können.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So gruppieren Sie Aufträge
                                       •   Weitere Gruppierungen hinzufügen
                                       •   So speichern Sie eine Gruppierung
                                       •   So entfernen Sie eine Gruppierung


                                        So gruppieren Sie Aufträge
                                       1 Klicken Sie die Symbol-Schaltfläche [Spaltenauswahl] an.
                                       2 Es öffnet sich ein Auswahl-Dialog.
                                       3 Klicken Sie das gewünschte Feld (z. B. Kundennummer) mit der linken
                                         Maustaste an und halten Sie die Maustaste gedrückt.
                                       4 Mit gedrückter Maustaste ziehen Sie das Feld an die gewünsche Stelle im
                                         Tabellenkopf.
                                       5 An der entsprechenden Stelle angekommen, lassen Sie die Maustaste los.




                                           Abb. I-19   Daten nach Kundennummer gruppiert


                                        Weitere Gruppierungen hinzufügen
                                       1 Klicken Sie die Symbol-Schaltfläche [Spaltenauswahl] an.
                                       2 Es öffnet sich ein Auswahl-Dialog.
                                       3 Klicken Sie das gewünschte Feld (z. B. Erfassungsdatum) mit der linken
                                         Maustaste an und halten Sie die Maustaste gedrückt.
                                       4 Mit gedrückter Maustaste ziehen Sie das Feld an die gewünsche Stelle im
                                         Tabellenkopf.
                                       5 An der entsprechenden Stelle angekommen, lassen Sie die Maustaste los.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                          I-31
                 Expertenmodus                                                                       Tutorial




                                    Abb. I-20   Daten nach Kundennummer und Erfassungsdatum gruppiert


                                  So speichern Sie eine Gruppierung
                                 1 Nachdem Sie die Gruppierung(en) erstellt haben, können Sie diese spei-
                                   chern.
                                 2 Betätigen Sie die Symbol-Schaltfläche [Speichern].
                                 3 Es öffnet sich der Dialog Ansicht speichern.
                                 4 Geben Sie im Feld Name der Ansicht den entsprechenden Namen ein.
                                 5 Klicken Sie auf die Schaltfläche [OK].
                                 6 Der Dialog wird geschlossen und der Name wird Ihnen rechts im Tabellen-
                                   kopf angezeigt.


                                  So entfernen Sie eine Gruppierung
                                 1 Wählen Sie die Gruppierung aus, die gelöscht werden soll.
                                 2 Klicken Sie auf die Symbol-Schaltfläche [X].
                                 3 Die ausgewählte Gruppierung wird entfernt.

                                    Gruppierungen löschen
                                    Das Löschen von Gruppierungen erfolgt ohne Sicherheitsabfrage. Nach-
                                    dem Sie die Symbol-Schaltfläche [X] betätigt haben, wird die Gruppierung
                                    gelöscht!
2.21 / 01-2017




                 I-32                                               A+W Business Pro Production Manager
                 Tutorial                                                                           Expertenmodus




                                       Produkt
                                       Am rechten Bildschirmrand befindet sich ein weiteres Register, das bei Bedarf
                                       aufgeklappt werden kann:
                                       •   Register Produkt
                                       Klicken Sie mit der Maus das Register Produkt an, wird dieses geöffnet:




                                       Abb. I-21    Register Produkt, am rechten Bildschirmrand


                                       Dieses Register liefert Ihnen detaillierte Informationen zu der ausgewählten
                                       Position inklusive der Modellparameter und einer grafischen Vorschau mit
                                       Vermaßung.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Produkt” auf Seite I-111


                                       Informationen
2.21 / 01-2017




                                       Dieser Bereich ist identisch mit den gleichnamigen Bereichen im Standardmo-
                                       dus und wird an dieser Stelle nicht noch einmal erläutert.
                                        “Informationen” auf Seite I-22



                 A+W Business Pro Production Manager                                                             I-33
                 Expertenmodus                                                                        Tutorial




                                 Bruchscheiben
                                 Wenn bei der Produktion Scheiben mit Mängeln auftreten, können Sie diese
                                 zur Nachproduktion erfassen.
                                 Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Bruchscheiben], wird
                                 das Register Bruchpositionen geöffnet:




                                 Abb. I-22    Register Bruchpositionen


                                 Dieses Register zeigt Ihnen alle vorhandenen Bruchscheiben und liefert Ihnen
                                 detaillierte Informationen zu den noch zu verplanenenden Bruchscheiben. Um
                                 Inhalte zu filtern, stehen Ihnen die bereits oben erwähnten Gruppierungsmög-
                                 lichkeiten zur Verfügung.
                                 Sie haben an dieser Stelle folgende Möglichkeiten:
                                 •   Bruch erfassen
                                 •   Bruch löschen
                                 •   Einen Bruchlauf bilden

                                 Bruch erfassen
                                 Über diesen Dialog können Sie Bruchscheiben erfassen. Öffnen Sie im Regis-
                                 ter Bruchpositionen das Kontextmenü und anschließend den Eintrag Bruch er-
                                 fassen. Es öffnet sich der gleichnamige Dialog.
2.21 / 01-2017




                                 Abb. I-23    Bruch erfassen




                 I-34                                                    A+W Business Pro Production Manager
                 Tutorial                                                                            Expertenmodus




                                       Über die Eingabe der Auftrags- und Positionsnummer und anschließendes
                                       Klicken auf die Symbol-Schaltfläche [Suchen] können Sie sich alle Stücklis-
                                       tenteile zu der eingegebenen Auftrags- und Positionsnummer anzeigen las-
                                       sen.
                                       Anschließend markieren Sie die Stücklistenteile, die als Bruch erfasst werden
                                       sollen und geben im Feld Menge die gewünschte Stückzahl ein.

                                       Einen Bruchlauf bilden
                                       Über diesen Dialog können Sie einen Bruchlauf bilden. Markieren Sie im Re-
                                       gister Bruchpositionen die gewünschte Auftragsnummer, öffnen Sie das Kon-
                                       textmenü und anschließend den Eintrag Neuen Bruchlauf erzeugen. Es öffnet
                                       sich der Dialog Neuen Lauf erstellen.




                                       Abb. I-24    Bruchlauf bilden


                                       Dieser Dialog wird im folgenden Kapitel detailliert beschrieben:
                                        “Allgemein” auf Seite I-40
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-35
                 Expertenmodus                                                                        Tutorial




                                 Mit Bruch arbeiten
                                 In dieser Einheit lernen Sie, wie Sie mit Bruch umgehen.
                                 Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                 •   So erfassen Sie Bruchscheiben
                                 •   So löschen Sie Bruchscheiben
                                 •   So erzeugen Sie einen neuen Bruchlauf


                                  So erfassen Sie Bruchscheiben
                                 1 Klicken Sie die Symbol-Schaltfläche [Bruchscheiben] an.
                                 2 Es öffnet sich der Dialog Bruchpositionen.
                                 3 Geben Sie im Feld Auftrag die entsprechende Auftragsnummer ein.
                                 4 Geben Sie im Feld Position die entsprechende Positionsnummer ein.
                                 5 Klicken Sie auf die Symbol-Schaltfläche [Suchen]. In der Liste werden Ih-
                                   nen die gewünschten Daten angezeigt.
                                 6 Selektieren Sie mit der Maus die Scheibe, die nachproduziert werden soll.
                                 7 Geben Sie im Feld Stückzahl die Menge ein, die nochproduziert werden
                                   soll.
                                 8 Wählen Sie aus der Kombobox Grund den Bruchgrund aus.
                                 9 Wählen Sie aus der Kombobox Stelle den Ort aus, an dem der Bruch pas-
                                   siert ist.
                                 10 Klicken Sie auf die Schaltfläche [Speichern], um die Daten zu speichern.
                                    Der Dialog ist wieder leer.
                                 11 Klicken Sie auf die Schaltfläche [Schließen], um den Dialog zu schließen.
                                    Sie befinden sich wieder im Register Bruchscheiben.


                                  So löschen Sie Bruchscheiben
                                 1 Klicken Sie die Symbol-Schaltfläche [Bruchscheiben] an.
                                 2 Es öffnet sich der Dialog Bruchpositionen.
                                 3 Markieren Sie die Position, die gelöscht werden soll.
                                 4 Öffnen Sie das Kontextmenü.
                                 5 Wählen Sie Bruch löschen. Es erfolgt eine Sicherheitsabfrage. Wenn Sie
                                   diese bestätigen, wird die ausgewählte Position gelöscht.


                                  So erzeugen Sie einen neuen Bruchlauf
                                 1 Klicken Sie die Symbol-Schaltfläche [Bruchscheiben] an.
                                 2 Es öffnet sich der Dialog Bruchpositionen.
2.21 / 01-2017




                                 3 Markieren Sie die Auftragsnummer, mit der Sie den Bruchlauf bilden möch-
                                   ten.
                                 4 Öffnen Sie das Kontextmenü.


                 I-36                                                A+W Business Pro Production Manager
                 Tutorial                                                                           Expertenmodus




                                       5 Wählen Sie Neuen Bruchlauf erzeugen. Es öffnet sich der Dialog Neuen
                                         Lauf erstellen.
                                       6 Geben Sie im Feld Bezeichnung die gewünschten Bezeichnung für den
                                         Bruchlauf ein.
                                       7 Wählen Sie aus der Kombobox Abstellplatzorganisation die gewünschte
                                         Organisation aus.
                                       8 Geben Sie im Feld Faktor für Abstellplatztiefe den gewünschten Faktor an.
                                       9 Bei Bedarf aktivieren Sie die Checkbox Unbegrenzte Abstellplatztiefe.
                                       10 Über die darunter liegenden Checkboxen steuern Sie, wie mit dem Lauf
                                          verfahren werden soll. Aktivieren Sie die gewünschte(n) Checkbox(en).
                                       11 Klicken Sie auf die Schaltfläche [OK].
                                       12 Die markierte Auftragsnummer verschwindet aus dem Register Bruchposi-
                                          tionen.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Bruchpositionen” auf Seite I-113
                                        Softwarereferenz, “Bruch erfassen” auf Seite I-116
                                        Softwarereferenz, “Neuen Lauf erstellen” auf Seite I-117
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                         I-37
                 Expertenmodus                                                                              Tutorial




                                 Läufe verwalten
                                 Lernziele

                                 • Lernen, wie Sie einen Lauf erstellen.
                                 • Wie werden die Daten geladen.
                                 • Die Inhalte der Anzeigen übersichtlich aufbereiten.


                                 Nutzen

                                 • Wenn Sie Ihre Läufe optimal zusammenstellen, haben Sie einen geringeren
                                   Verschnitt.


                                 Merke

                                 Laufnummer                  Die Laufnummer wird vom System vergeben.

                                 Abstellplatzorganisation    Kann nach der Laufbildung noch geändert werden.

                                 Abstellplatztiefe           Durch die Veränderung der Abstellplatztiefe haben Sie
                                                             Einfluss auf das Optimierungsergebnis
2.21 / 01-2017




                 I-38                                                    A+W Business Pro Production Manager
                 Tutorial                                                                             Expertenmodus




                                       Allgemein
                                       Bei der Bildung von Läufen gehen alle selektierten und nicht anderweitig ver-
                                       planten Teile in den Lauf.
                                       Läufe werden entweder mit Hilfe des Nummerverwalters oder aber pro Ar-
                                       beitsgang im Register Auftragsselektion gebildet (Kontextmenü Neuen Lauf
                                       erstellen). Es erscheint folgender Dialog:




                                       Abb. I-25    Neuen Lauf erstellen


                                       Erläuterung der Felder
                                       Als Laufnummer wird vom Programm die nächst höhere Nummer vergeben.
                                       Im Feld Bezeichnung können Sie detaillierte Beschreibung zum Lauf hinterle-
                                       gen. Anschließend wählen Sie aus der Kombobox Abstellplatzorganisation die
                                       gewünschte Organisationsform aus. Die Kombobox enthält alle in Ihrem Haus
                                       angelegten Abstellplatzorganisationen.
                                       Bei dem Faktor für Abstellplatztiefe handelt es sich um den Faktor für die im
                                       Lauf zu verwendende Gestelltiefe in Prozent. Der Wert für die Abstellplatztiefe
                                       kommt aus dem Stammdaten (Fertigung > Logische Abstellplätze). Über den
                                       Faktor können Sie den Wert temporär verändern. 100 % bedeutet, dass der in
                                       den Stammdaten hinterlegte Wert verwendet wird. 90 % bedeutet, dass die in
                                       den Stammdaten hinterlegte Tiefe nur zu 90 % genutzt wird, d. h. es gehen
                                       weniger Scheiben auf den Abstellplatz. Eine Korrektur des Wertes nach oben
                                       führt zu einer Überbeladung.
                                       Aktivieren Sie die Checkbox Unbegrenzte Abstellplatztiefe überschreiben Sie
                                       jegliche Werte aus den Stammdaten.
                                       Über die Checkboxen im Bereich Aktionen nach Lauferstellung steuern Sie,
                                       wie mit dem Lauf verfahren wird.
                                       Aktivieren Sie die Checkbox Feinplanung, erfolgt nach der Laufbildung auto-
                                       matisch die Feinplanung. Die Checkbox Optimierungsmanager können Sie
                                       nur aktivieren, wenn die Checkox Feinplanung aktiv ist. Dann öffnet sich nach
                                       der Laufbildung und der Feinplanung das Register Optimierungsmanager. Es
                                       wird jedoch keine Optimierung erzeugt! Die Checkbox Kompletter Handzu-
2.21 / 01-2017




                                       schnitt können Sie ebenfalls nur aktivieren, wenn die Checkbox Feinplanung
                                       aktiv ist. Dann werden nach der Laufbildung und der Feinplanung alle Schei-
                                       ben auf Handzuschnitt gesetzt.
                                       Die Checkbox Ausgabe ist nur aktiv, wenn die Checkboxen Feinplanung und


                 A+W Business Pro Production Manager                                                             I-39
                 Expertenmodus                                                                                  Tutorial




                                          Kompletter Handzuschnitt aktiv sind. Dann wird nach der Laufbildung, der
                                          Feinplanung und dem Handzuschnitt direkt in das Register Ausgabe gewech-
                                          selt.

                                          Der Lauf wurde gebildet ...
                                          Nachdem der Lauf gebildet wurde, hat er den Status Grobgeplant. Die gebil-
                                          deten Läufe finden Sie im Register Laufübersicht.
                                          Mit grobgeplanten Läufen können Sie folgendes tun:
                                          •   Die bei der Laufbildung zugewiesene Abstellplatzorganisation kann geän-
                                              dert werden.
                                          •   Sie können weitere Teile diesem Lauf hinzufügen.
                                          •   Sie können Teile aus dem Lauf löschen.
                                          •   Sie können den Lauf auflösen.
                                          •   Sie können den Lauf an die Feinplanung übergeben.




                 Abb. I-26   Hauptdialog, Expertenmodus, Laufübersicht


                                          Der Dialog ist in mehrere Bereiche eingeteilt. Im oberen Bereich befinden sich
                                          die Selektionskriterien. Im unteren Bereich werden Ihnen die existierenden
                                          Läufe angezeigt.
2.21 / 01-2017




                 I-40                                                          A+W Business Pro Production Manager
                 Tutorial                                                                            Expertenmodus




                                       Informationen und Filtereinstellungen




                                       Abb. I-27    Selektionskriterien für Läufe


                                       Über das Feld Laufnummer können Sie sich gezielt Läufe nach deren Num-
                                       mer anzeigen lassen. Das setzt voraus, dass Sie die Nummer des Laufes, den
                                       Sie sich anzeigen lassen wollen, kennen. Die Felder dienen auch dazu, die
                                       angezeigten Läufe zu limitieren, um den Überblick zu behalten.
                                       Über die Felder Erstelldatum können Sie sich die Läufe nach dem Datum an-
                                       zeigen lassen, an dem sie erstellt wurden.
                                       Mit hilfe der Komboboxen Status können Sie sich die Läufe nach deren Status
                                       anzeigen lassen. Folgende Status sind möglich:
                                       •   Grobgeplant: Für diese Läufe ist noch keine Abstellplatzvergabe erfolgt.
                                       •   Feingeplant: Für diese Läufe erfolgte eine Abstellplatzvergabe.
                                       •   Teiloptimiert: Einige Glasarten dieser Läufe wurden bereits optimiert.
                                       •   Optimiert: Alle Glasarten dieser Läufe wurden bereits optimiert.
                                       •   Teilfertig: Wird zur Zeit noch nicht ausgewertet.
                                       •   Fertig: Alle Teile, die zu diesen Läufen gehören, sind fertig.
                                       Über das Feld Bezeichnung können Sie sich die Läufe nach deren Bezeich-
                                       nung anzeigen lassen. Diese Bezeichnung haben Sie beim Erstellen eines
                                       Laufes im Dialog Neuen Lauf erstellen vergeben.

                                       Informationen und Filtereinstellungen im Bereich Läufe
                                       In der Spalte Laufnummer wird Ihnen die Laufnummer angezeigt, die Sie im
                                       Register Laufübersicht selektiert haben. Anschließend sehen Sie das Datum,
                                       an dem der Lauf erstellt wurde. In der Spalte Bezeichnung wird Ihnen die Lauf-
                                       bezeichnung angezeigt, die Sie beim Erstellen des Laufes angegeben haben.
                                       Dann folgt die Abstellplatzorganisation, die Sie bei der Laufbildung gewählt
                                       haben sowie der Laufstatus. Die Felder ISO, VSG, ESG und Glas zeigen Ih-
                                       nen die im Lauf enthaltenen Mengen der jeweiligen Art.
                                       Einträge, die in diesem Bereich hellgrau dargestellt werden, wurden bereits an
                                       den Optimierungsmanager übergeben. Klicken Sie einen solchen Eintrag an,
                                       erscheint eine entsprechende Meldung am Bildschirm. Sie können sich für
                                       diese Einträge die Detailansicht und die Feinplanungsergebnisse anzeigen
                                       lassen sowie die Ausgabe (Maschinen, Reports, etc.) starten.
                                       Es kann unter Umständen vorkommen, dass eine große Anzahl von Daten an-
                                       gezeigt wird. Um dennoch den Überblick zu behalten, haben Sie Möglichkeit,
                                       die Daten zu gruppieren und innerhalb der Gruppierung zu sortieren.
2.21 / 01-2017




                                       Die Vorgehensweise wurde bereits im Register Auftragsselektion erläutert und
                                       wird an dieser Stelle nicht noch einmal beschrieben.
                                        “Daten gruppieren” auf Seite I-30



                 A+W Business Pro Production Manager                                                            I-41
                 Expertenmodus                                                                      Tutorial




                                 Ergänzende Informationen
                                  Softwarereferenz, “Neuen Lauf erstellen” auf Seite I-117
                                  “Läufe über bestimmte Kriterien auswählen” auf Seite I-44
2.21 / 01-2017




                 I-42                                                  A+W Business Pro Production Manager
                 Tutorial                                                                           Expertenmodus




                                       Läufe über bestimmte Kriterien auswählen
                                       In dieser Einheit lernen Sie, wie Sie Läufe zur Produktion auswählen.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So selektieren Sie Läufe über die Laufnummer
                                       •   So selektieren Sie Läufe über das Erstelldatum
                                       •   So selektieren Sie Läufe über die Bezeichnung


                                        So selektieren Sie Läufe über die Laufnummer
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Be-
                                         arbeitung freigegeben.
                                       2 Tragen Sie im Feld von die kleinste Laufnummer ein und im Feld bis die
                                         größte Laufnummer. Wenn Sie in beiden Feldern dieselbe Nummer eintra-
                                         gen, wird nur dieser eine Lauf angezeigt.
                                       3 Klicken Sie auf die Symbol-Schaltfläche [Suchen].
                                       4 Die Daten werden geladen.


                                        So selektieren Sie Läufe über das Erstelldatum
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Be-
                                         arbeitung freigegeben.
                                       2 Tragen Sie in den Feldern von bis das entsprechende Erstelldatum ein.
                                         Wenn Sie in beiden Feldern dasselbe Datum eintragen, werden nur die
                                         Läufe angezeigt, die an diesem Tag erstellt wurden.
                                       3 Klicken Sie auf die Symbol-Schaltfläche [Suchen].
                                       4 Die Daten werden geladen.


                                        So selektieren Sie Läufe über den Status
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Be-
                                         arbeitung freigegeben.
                                       2 Tragen Sie in den Feldern von bis die entsprechenden Kriterien aus.
                                       3 Klicken Sie auf die Symbol-Schaltfläche [Suchen].
                                       4 Die Daten werden geladen.


                                        So selektieren Sie Läufe über die Bezeichnung
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Be-
                                         arbeitung freigegeben.
                                       2 Tragen Sie in den Felder Bezeichnung den entsprechenden Text ein.
                                       3 Klicken Sie auf die Symbol-Schaltfläche [Suchen].
2.21 / 01-2017




                                       4 Die Daten werden geladen.




                 A+W Business Pro Production Manager                                                           I-43
                 Expertenmodus                                                                       Tutorial




                                 Ergänzende Informationen
                                  Softwarereferenz, “Neuen Lauf erstellen” auf Seite I-117
2.21 / 01-2017




                 I-44                                                   A+W Business Pro Production Manager
                 Tutorial                                                                               Expertenmodus




                                           Detailansicht für Läufe
                                           Über das Kontextmenü haben Sie die Möglichkeit, sich Läufe im Detail anzu-
                                           sehen. Der entsprechende Lauf wird dann in einem separaten Register ange-
                                           zeigt.
                                           Im nachfolgenden Beispiel öffnen wir für den Lauf 1379 die Detailansicht.
                                           Dazu wird der Lauf in der Laufübersicht selektiert.
                                           Anschließend können Sie über das Kontextmenü den Eintrag Detailansicht
                                           wählen.
                                           Der Lauf wird mit allen seinen Bestandteilen in einem separaten Register an-
                                           gezeigt. Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt:




                 Abb. I-28   Detailansicht für Lauf 1379


                                           Informationen im Bereich Feinplanung:
2.21 / 01-2017




                                           Abb. I-29       Bereich Feinplanung




                 A+W Business Pro Production Manager                                                               I-45
                 Expertenmodus                                                                             Tutorial




                                 In diesem Bereich werden Ihnen die Daten angezeigt, die Sie bei der Bildung
                                 des Laufes eingegeben oder ausgewählt haben.
                                 Sie sehen die Laufbezeichnung, die Sie an dieser Stelle noch ändern können.
                                 Ebenso können Sie die Abstellplatzorganisation noch ändern, indem Sie die
                                 Kombobox öffnen und eine andere Organisationsform zuweisen. Die Felder
                                 Erstelldatum und Status können nicht geändert werden. Das Erstelldatum
                                 zeigt Ihnen, wann der Lauf erstellt wurde und das Feld Status zeigt Ihnen, in
                                 welchem Status sich der Lauf befindet. An dieser Stelle können Sie auch den
                                 Faktor für die Abstellplatztiefe noch ändern bzw. dem Abstellplatz eine unbe-
                                 grenzte Tiefe zuweisen.
                                 Informationen im Bereich Optimierungsartikel:




                                 Abb. I-30      Bereich Optimierungsartikel


                                 Hier sehen Sie, um welche Glasart es sich handelt, die zu optimierende Men-
                                 ge sowie die Quadratmeter pro Glasart und die entsprechende Quadratmeter-
                                 zahl im Verhältnis zur Gesamtfläche des Laufes.

                                    Beispiel:

                                    Der Lauf hat eine zu optimierende Gesamtfläche von 67,86 m². Der Artikel
                                    104 A+W Float 4 mm hat eine Fläche von 16,35 m². Diese 16,35 m² sind
                                    24,10 % von der Gesamtfläche.

                                    Im Bereich Aufträge und Positionen werden Ihnen alle auftragsrelevanten
                                    Informationen angezeigt, wie bspw. Auftragsnummer, Kundennummer und
                                    Versanddatum.

                                    Im Bereich Positionen werden nun die positionsbezogenen Informationen der
                                    entsprechenden Aufträge angezeigt, wie bspw. Stückzahl, Modellnummer,
                                    Beschaffungsart.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Detailansicht” auf Seite I-121
                                  “Erläuterung der Felder im Bereich Aufträge” auf Seite I-106
                                  “Erläuterung der Felder im Bereich Positionen” auf Seite I-107
2.21 / 01-2017




                 I-46                                                    A+W Business Pro Production Manager
                 Tutorial                                                                             Expertenmodus




                                       Register Produkt und Zuschnitt
                                       Am rechten Bildschirmrand befinden sich zwei weitere Register, die bei Bedarf
                                       aufgeklappt werden können:
                                       •   Register Produkt
                                       •   Register Zuschnitt

                                       Register Produkt
                                       Dieses Register ist identisch mit dem gleichnamigen Register im Bereich Auf-
                                       tragsselektion und wird an dieser Stelle nicht noch einmal erläutert.
                                        “Produkt” auf Seite I-34

                                       Register Zuschnitt
                                       Klicken Sie mit der Maus das Register Zuschnitt an, wird dieses geöffnet:




                                       Abb. I-31    Register Zuschnitt, am rechten Bildschirmrand


                                       Es liefert Ihnen detaillierte Informationen zu der ausgewählten Position inklu-
2.21 / 01-2017




                                       sive der Modellparameter und einer grafischen Vorschau mit Vermaßung. Die
                                       gestrichelte Linie kennzeichnet die Modellbruchränder.



                 A+W Business Pro Production Manager                                                             I-47
                 Expertenmodus                                                                          Tutorial




                                 Klicken Sie auf die Schaltfläche [Bearbeiten], öffnet sich der Dialog Zuschnitt
                                 bearbeiten.




                                 Abb. I-32    Zuschnitt bearbeiten


                                 In diesem Dialog können Sie diverse Änderungen vornehmen. Sie können
                                 z. B. ein anderes Modell auswählen, die Modellparameter sowie die Modell-
                                 bruchränder und die zu prozierende Stückzahl ändern. Die Modellbruchränder
                                 werden Ihnen durch die gestrichelte Linie angezeigt.
                                 Wenn Sie Änderungen vorgenommen haben, werden Ihnen diese sofort im
                                 Bereich Vorschau angezeigt.

                                    Zuschnittdaten bearbeiten
                                    Bitte bedenken Sie, dass Änderungen, die Sie hier vornehmen, lediglich
                                    den Zuschnitt betreffen. Diese Änderungen werden nicht an das Auftrags-
                                    bearbeitungssystem zurück gemeldet!

                                 Das Register Produkt
                                 Das Register Produkt ist identisch mit dem gleichnamigen Register in der De-
                                 tailansicht für Läufe und wird an dieser Stelle nicht noch einmal erläutert.
                                  “Register Produkt und Zuschnitt” auf Seite I-48
2.21 / 01-2017




                                 Ergänzende Informationen
                                  Softwarereferenz, “Zuschnitt bearbeiten” auf Seite I-125



                 I-48                                                   A+W Business Pro Production Manager
                 Tutorial                                                                               Expertenmodus




                                       Feinplanung
                                       Lernziele

                                       • Die Feinplanung kennen lernen und verstehen
                                       • Die Optimierungsmodi kennenlernen und verstehen
                                       • Unter welchen Umständen wird welcher Modus verwendet


                                       Nutzen

                                       • Wenn Sie die unterschiedlichen Optimierungsmodi kennen und verstehen, können
                                         Sie die Feinplanung auf Ihre Produktion so anpassen, dass diese kostengünstig
                                         und zeitsparend arbeitet.


                                       Merke

                                       Variante                  Die durchgeführten Optimierungsvarianten bleiben
                                                                 erhalten, so dass Sie die Beste auswählen können.

                                       Feinplanung               Aufteilen der Gläser eines Auftrags auf verschiedene
                                                                 Glasstapel und Abstellplätze (Gestelle) nach definierten
                                                                 Kriterien für Gruppierung und Sortierung.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                 I-49
                 Expertenmodus                                                                         Tutorial




                                 Ablauf der Feinplanung
                                 Die grobgeplanten Läufe können aus dem Register Laufübersicht an die Fein-
                                 planung übergeben werden. Aufgabe der Feinplanung ist es, für die in den
                                 Läufen enthaltenen Teile die Produktionsreihenfolge zu erstellen.
                                 Die Produktionsreihenfolge kann sich durch folgende Kriterien ergeben:
                                 •   Durch die Vorgaben des Kunden
                                 •   durch fertigungstechnische Restriktionen
                                 In diesem Schritt erfolgt auch die aktuell zugewiesene Abstellplatzorganisati-
                                 on. Der Status des Laufes wechselt von Grobgeplant in Feingeplant.
                                 Mit feingeplanten Läufen können Sie folgendes tun:
                                 •   Sie können die Feinplanung beliebig oft wiederholen (z. B. wegen geän-
                                     derter Stammdaten der Abstellplatzorganisation).
                                 •   Sie können feingeplante Läufe an den Optimierungsmanager übergeben.
                                 •   Sie können den Lauf auflösen.
                                 •   Sie können sich die Gestellbelegung anzeigen lassen.
2.21 / 01-2017




                 I-50                                                 A+W Business Pro Production Manager
                 Tutorial                                                                               Expertenmodus




                                         Optimierungsmanager
                                         Feingeplante Läufe können an den Optimierungsmanager übergeben werden.
                                         Nachdem Sie die erste Optimierung für einen Lauf durchgeführt und bestätigt
                                         haben, ändert sich der Status in Teiloptimiert.
                                         Mit teiloptimierten Läufen können Sie folgendes tun:
                                         •   Sie können die Ausgabe für einzelne Optimierungen des Laufs durchfüh-
                                             ren.
                                         •   Sie können mit diesen Läufen alles tun, was mit feingeplanten Läufen auch
                                             getan werden kann (außer dem Auflösen des Laufes).




                 Abb. I-33   Optimierungsmanager


                                         In diesem Register werden die Optimierungen der einzelnen Glasarten für die
                                         ausgewählten Läufe durchgeführt.
2.21 / 01-2017




                                         Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt.




                 A+W Business Pro Production Manager                                                             I-51
                 Expertenmodus                                                                          Tutorial




                                 Erläuterung der Felder im Bereich Läufe




                                 Abb. I-34    Bereich Läufe


                                 In der Spalte Laufnummer wird Ihnen die Laufnummer angezeigt, die Sie im
                                 Register Laufübersicht selektiert haben. Anschließend sehen Sie das Datum,
                                 an dem der Lauf erstellt wurde sowie den Laufstatus. In der Spalte Bezeich-
                                 nung wird Ihnen die Laufbezeichnung angezeigt, die Sie beim Erstellen des
                                 Laufes angegeben haben. Dann folgt die Abstellplatzorganisation, die Sie bei
                                 der Laufbildung gewählt haben. Die Felder ISO, VSG, ESG und Glas zeigen
                                 Ihnen die im Lauf enthaltenen Mengen der jeweiligen Art. Bei dem Faktor für
                                 Abstellplatztiefe handelt es sich ebenfalls um den Faktor, den Sie bei der Lau-
                                 ferstellung angegeben haben.

                                 Erläuterung der Felder im Bereich Glasarten




                                 Abb. I-35    Bereich Glasarten


                                 Hier werden Ihnen die einzelnen Glasarten, die im Lauf enthalten sind, ange-
                                 zeigt. Wenn Sie den Eintrag der Glasart aufklappen, erhalten Sie Informatio-
                                 nen zu der Stückzahl, der Fläche und dem Lauf.
                                 Da mehrere Läufe in den Optimierungsmanager geladen werden können, se-
                                 hen Sie hier, aus welchen Läufen die einzelnen Glasarten kommen.

                                 Die Bereiche Optimierungen und Gesamtergebnis
                                 Die Felder im Bereich Optimierungen und Gesamtergebnis sind identisch mit
                                 den gleichnamigen Bereichen im Standardmodus und werden an dieser Stelle
                                 nicht noch einmal erläutert.
                                  “Ergebnisse” auf Seite I-19
2.21 / 01-2017




                 I-52                                                 A+W Business Pro Production Manager
                 Tutorial                                                                          Expertenmodus




                                       Die Register Lagerplatten und Optmierungsparameter
                                       Die am rechten Bildschirmrand liegenden Register Lagerplatten und Optimie-
                                       rungsparameter sind identisch mit den gleichnamigen Registern im Bereich
                                       Standardmodus und werden an dieser Stelle nicht noch einmal erläutert.
                                        “Lagerplatten und Optimierungsparameter” auf Seite I-21


                                       Läufe optimieren
                                       In dieser Einheit lernen Sie, wie Sie Läufe optimieren.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So übergeben Sie Läufe an den Optimierungsmanager
                                       •   So setzen Sie eine Glasart auf Handzuschnitt
                                       •   So starten Sie die Optimierung
                                       •   So speichern Sie die Optimierung


                                        So übergeben Sie Läufe an den Optimierungsmanager
                                       1 Markieren Sie im Register Laufübersicht den oder die gewünschten Läufe.
                                       2 Öffnen Sie das Kontextmenü.
                                       3 Klicken Sie auf den Menü-Eintrag Optimierungsmanager.
                                       4 Das Register Optimierungsmanager wird geöffnet und die Daten werden
                                         geladen.

                                           Läufe übergeben
                                           Sie können nur Läufe an den Optimierungsmanager übergeben, die den
                                           Status Feingeplant haben!


                                        So setzen Sie eine Glasart auf Handzuschnitt
                                       1 Markieren Sie im Bereich Optimierungen den oder die gewünschten Glas-
                                         arten.
                                       2 Öffnen Sie das Kontextmenü.
                                       3 Klicken Sie auf den Menü-Eintrag Handzuschnitt. Das Häkchen vor der
                                         Glasart verschwindet und im Feld Ergebnis erscheint der Eintrag Handzu-
                                         schnitt.


                                        So starten Sie die Optimierung
                                       1 Markieren Sie im Register Optimierungsmanager im Bereich Optimierun-
                                         gen die gewünschte Glasart.
                                       2 Öffnen Sie das Kontextmenü.
                                       3 Klicken Sie auf den Menü-Eintrag Optimierung starten.
2.21 / 01-2017




                                       4 Nachdem die Optimierung durchlaufen wurde, wird der Bereich Gesamter-
                                         gebnis mit Daten gefüllt.




                 A+W Business Pro Production Manager                                                        I-53
                 Expertenmodus                                                                                Tutorial




                                             Ribbon-Leiste
                                             Die Optimierung können Sie auch über die Ribbon-Leiste (Ausführen) star-
                                             ten. Dann entfällt das Öffnen des Kontextmenüs.


                                           So speichern Sie die Optimierung
                                          1 Öffnen Sie das Kontextmenü.
                                          2 Klicken Sie auf den Menü-Eintrag Optimierung speichern.
                                          3 Die Optimierung wird gespeichert.

                                             Ribbon-Leiste
                                             Das Speichern können Sie auch über die Ribbon-Leiste (Speichern) durch-
                                             führen. Dann entfällt das Öffnen des Kontextmenüs.


                                          Temporäre Optimierung
                                          Mit jedem Klick auf die Symbol-Schaltfläche [Ausführen] wird eine neue Opti-
                                          mierung durchgeführt. Diese Vorgehensweise dient dazu, Läufe mit unter-
                                          schiedlichen Variationen zu optimieren. So können Sie z. B. Glasarten
                                          tauschen, Optimierungsparameter oder Lagerplatten ändern. Die durchge-
                                          führten Optimierungen werden als Varianten im Bereich Gesamtergebnis an-
                                          gezeigt.
                                          Im Bereich Optimierungen können Sie über das Kontextmenü die Detailan-
                                          sicht öffnen. Diese wird in einem separaten Register angezeigt.
2.21 / 01-2017




                 Abb. I-36   Optimierungsmanager, Detailansicht


                 I-54                                                         A+W Business Pro Production Manager
                 Tutorial                                                                             Expertenmodus




                                       Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt.

                                       Erläuterung der Felder im Bereich Gestell




                                       Abb. I-37    Bereich Gestell


                                       Hier werden Ihnen alle relevanten Informationen zu den Gestellen angezeigt.
                                       In der Spalte Laufnummer wird Ihnen die Laufnummer angezeigt, die Sie im
                                       Register Optimierungsmanager selektiert haben. Anschließend sehen Sie die
                                       Gestellnummer sowie den Gestell-Typ, auf dem die Scheiben abgestellt wer-
                                       den und dem logischen Abstellplatz.

                                       Erläuterung der Felder im Bereich Läufe




                                       Abb. I-38    Bereich Läufe


                                       In der Spalte Laufnummer wird Ihnen die Laufnummer angezeigt, die Sie im
                                       Register Optimierungsmanager sowie das Datum, an dem der Lauf erstellt
                                       wurde.

                                       Erläuterung der Felder im Bereich Lagermaße




                                       Abb. I-39    Bereich Lagermaße


                                       In der Spalte Menge wird Ihnen die benötigte Anzahl an Lagerplatten ange-
2.21 / 01-2017




                                       zeigt. Die Felder Höhe und Breite zeigen Ihnen die Abmessungen der verwen-
                                       deten Lagerplatten. Im Feld Fläche sehen Sie die Fläche in Quadratmeter und
                                       im Feld Priorität die entsprechende Priorität.


                 A+W Business Pro Production Manager                                                           I-55
                 Expertenmodus                                                                         Tutorial




                                 Erläuterung der Felder im Bereich Muster




                                 Abb. I-40    Bereich Muster


                                 In der Spalte Muster werden Ihnen die einzelnen Muster aufgelistet. Klicken
                                 Sie ein Muster an, wird es auf der rechten Sei im Bereich Schneidplan grafisch
                                 angezeigt. Das Feld Optigruppe zeigt Ihnen die Optimierungsgruppe. Im Feld
                                 Menge sehen Sie die Menge bezogen auf das Muster. Die Felder Höhe und
                                 Breite zeigen Ihnen die Abmessungen der verwendeten Lagerplatten.

                                 Erläuterung der Felder im Bereich Schneidplan




                                 Abb. I-41    Bereich Schneidplan


                                 In diesem Bereich wird Ihnen das bei der Optimierung erzeugte Schneidmus-
                                 ter grafisch dargestellt. Die Darstellung entspricht dem zu schneidenden La-
                                 germaß und enthält alle wichtigen Informationen über die Optimierung, den
                                 Artikel und die einzelnen Scheiben.
                                 Bei der oberen Zahl handelt es sich um die Gestell-Nr. (z. B. 7968). Anschlie-
                                 ßend folgt die Abmessung der Scheibe (z. B. 1200x800). Darunter befindet
                                 sich die Auftragsnummer und die dazugehörige Position.


                                 Ergänzende Informationen
                                  “Lagerplatten und Optimierungsparameter” auf Seite I-21
2.21 / 01-2017




                 I-56                                                  A+W Business Pro Production Manager
                 Tutorial                                                                              Expertenmodus




                                         Optimierung abbrechen
                                         Hier haben Sie die Möglichkeit, eine Optimierung, die gerade durchlaufen
                                         wird, duch Klicken auf die Schaltfläche [Abbrechen] zu stoppen.




                 Abb. I-42   Optimierung abbrechen


                                         Ergänzende Informationen
                                          Softwarereferenz, “Optimierung abbrechen” auf Seite I-132
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-57
                 Expertenmodus                                                                                    Tutorial




                                          Optimierungsübersicht
                                          Die Optimierungsübersicht verschafft Ihnen einen Überblick zu den durchge-
                                          führten Optimierungen.




                 Abb. I-43   Optimierungsübersicht


                                          In diesem Register werden die durchgeführten Optimierungen der einzelnen
                                          Glasarten angezeigt. Um die Inhalte überschaubar zu halten, stehen Ihnen
                                          unterschiedlichen Selektionskriterien zur Verfügung. Sie können sich an die-
                                          ser Stelle für eine markierte Glasart die Details anzeigen (Detailansicht) las-
                                          sen und die Ausgabe (Maschinenausgaben, Reports) starten.
                                          Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt.

                                          Erläuterung der Felder im Bereich Selektionskriterien
2.21 / 01-2017




                                          Abb. I-44    Bereich Selektionskriterien




                 I-58                                                            A+W Business Pro Production Manager
                 Tutorial                                                                              Expertenmodus




                                         Hier nehmen Sie die Auswahl der Daten vor, die angezeigt werden sollen. Im
                                         Feld Optimierung können Sie über die Komboboxen gezielt auf einzelne Op-
                                         timierungen zugreifen. Im Feld Erstelldatum können Sie sich Optimierungen
                                         bestimmter Tage anzeigen lassen und über die Komboboxen für die Laufnum-
                                         mer einzelne Laufnummern.
                                         Darunter befindet sich der Bereich der Optimierungen. Hier werden die Daten
                                         gemäß oben genannten Selektionskriterien angezeigt.

                                         Erläuterung der Felder im Bereich Optimierungen




                 Abb. I-45   Durchgeführte Optimierungen


                                         Es kann unter Umständen vorkommen, dass eine große Anzahl von Daten an-
                                         gezeigt wird. Um dennoch den Überblick zu behalten, haben Sie Möglichkeit,
                                         die Daten zu gruppieren und innerhalb der Gruppierung zu sortieren.
                                         Die Vorgehensweise wurde bereits im Register Auftragsselektion erläutert und
                                         wird an dieser Stelle nicht noch einmal beschrieben.
                                          “Daten gruppieren” auf Seite I-30
                                         Das Feld Optimierung zeigt Ihnen die Nummer der Optimierung. Im Anschluss
                                         folgt der Modus, mit dem die Optimierung durchgeführt wurde. Es sind folgen-
                                         de Werte möglich:
                                         •   XOPT: Bei dieser Variante erfolgt die Optimierung chaotisch. D. h, die Rei-
                                             henfolge der Scheiben nach der Optimierung ist nicht wichtig, die Scheiben
                                             einer Position müssen nicht zusammengehalten werden. Dadurch erzielt
                                             man zwar ein besseren Verschnitt, es müssen allerdings vor der ISO-Pro-
                                             duktion alle Scheiben auf den A-Böcken umsortiert werden.
                                         •   XOPT-S: Dies ist der Standard-Modus für ISO-Betriebe. Hier wird die in der
                                             Abstellplatzorganisation vorgegebene Reihenfolge der Scheiben auf den
                                             Abstellplätzen eingehalten. Eine Synchronoptimierung der Scheiben ist
                                             möglich, damit Scheibe und Gegenscheibe auf der ISO-Linie zusammen-
                                             passen. Die Scheiben einer Auftragsposition stehen nach der Optimierung
                                             immer zusammen auf einem A-Gestell, d. h. die Position wird nicht gesplit-
                                             tet.
                                         Im Feld Glasart werden Ihnen die in der Optimierung enthaltenen Glasarten
                                         angezeigt. Anschließend sehen Sie den Schneidtisch, auf dem das Glas ge-
2.21 / 01-2017




                                         schnitten wird, gefolgt von der Laufnummer. Das Feld Status zeigt Ihnen den
                                         Status der jeweiligen Optimierung. Es sind folgende Status möglich:
                                         •   Optimiert: Die Optimierung wurde durchgeführt


                 A+W Business Pro Production Manager                                                               I-59
                 Expertenmodus                                                                        Tutorial




                                 •   Freigegeben: Der Schneidcode für die Optimierung wurde ausgegeben
                                 •   Teilfertig. Der Zuschnitt hat begonnen
                                 •   Fertig: Alle Lagerplatten der Optimierung wurde zugeschnitten
                                 •   Abgebucht: Alle Lagerplatten der Optimierung wurden vom Lager abge-
                                     bucht.
                                 Im Feld Stückzahl wird Ihnen je Glasart die Stückzahl angezeigt und im nächs-
                                 ten Feld die Fläche in Quadratmetern.
                                 Im Feld Ergebnis wird Ihnen das Ergebnis der Optimierung für die jeweilige
                                 Glasart in % angezeigt.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Optimierungsübersicht” auf Seite I-135
2.21 / 01-2017




                 I-60                                                  A+W Business Pro Production Manager
                 Tutorial                                                                                   Expertenmodus




                                          Detailansicht Optimierung
                                          Im Bereich Optimierungsübersicht können Sie über das Kontextmenü die De-
                                          tailansicht für eine Optimierung öffnen. Diese wird dann für die ausgewählte
                                          Optimierungsnummer in einem separaten Register angezeigt.




                 Abb. I-46   Optimierungsübersicht, Detailansicht


                                              Identische Bereiche und Felder
                                              Der Dialog ist identisch mit dem Dialog Temporäre Optimierung und wird
                                              an dieser Stelle nicht noch einmal erläutert.

                                               “Temporäre Optimierung” auf Seite I-55


                                          Ergänzende Informationen
                                           Softwarereferenz, “Detailansicht Optimierung” auf Seite I-137
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                 I-61
                 Expertenmodus                                                                               Tutorial




                                 Ausgabe
                                 Lernziele

                                 • Unterschiedlichen Darstellungen des Registers kennenlernen.
                                 • Ausgabe der unterschiedlichen Medien lernen.


                                 Nutzen

                                 • Der Optimierungsmanager weiß, für welche Läufe welche Ausgaben zu erfolgen
                                   haben. Sie können daher nichts vergessen.


                                 Merke

                                 Grau unterlegte Einträge   Für grau unterlegte Einträge findet keine Ausgabe statt.

                                 Drucker                    Abgesehen von dem Standarddrucker, kann der
                                                            Ausdruck auf anderen Druckern erfolgen.

                                 Papier und Schneidcode     Über das Register Ausgabe werden alle notwendigen /
                                                            selektierten Produktionspapiere gedruckt und die
                                                            Übergabe der Daten an die Maschinen gestartet.
2.21 / 01-2017




                 I-62                                                   A+W Business Pro Production Manager
                 Tutorial                                                                             Expertenmodus




                                       Reports und Schneidcodes
                                       Über dieses Register werden alle Ausgaben, unabhängig davon, ob es sich
                                       um Ausgaben auf Papier oder in Dateiform handelt, gestartet.
                                       Der Dialog kann direkt (Register Ausgabe), über das Register Laufübersicht
                                       und über das Register Optimierungsübersicht aufgerufen werden.
                                       Aus der Laufübersicht heraus können Sie die Ausgabe nur für Läufe öffnen,
                                       deren Status Feingeplant, Optimiert bzw. Freigegeben ist. Für Läufe, die sich
                                       im Status Grobgeplant befinden, können Sie die Ausgabe nicht starten, da die
                                       gesamte Feinplanung fehlt.
                                       Aus der Optimierungsübersicht heraus können Sie die Ausgabe für alle Opti-
                                       mierungen öffnen.




                 Abb. I-47   Ausgabe


                                       Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-63
                 Expertenmodus                                                                                             Tutorial




                                          Erläuterung der Felder im Bereich Läufe
                                          Der Titel dieses Bereichs ist abhängig davon, von wo aus Sie die Ausgabe ge-
                                          startet haben. Kommen Sie aus der Laufübersicht, heißt der Bereich Läufe,
                                          kommen Sie aus der Optimierungsübersicht, hießt der Bereich Optimierun-
                                          gen.




                 Abb. I-48   Ausgabe, geöffnet aus der Laufübersicht


                                          In der Spalte Laufnummer wird Ihnen die Laufnummer angezeigt, die Sie im
                                          Register Laufübersicht selektiert haben. Anschließend sehen Sie das Datum,
                                          an dem der Lauf erstellt wurde sowie den dazugehörigen Benutzer. In der
                                          Spalte Bezeichnung wird Ihnen die Laufbezeichnung angezeigt, die Sie beim
                                          Erstellen des Laufes angegeben haben. Dann folgt die Abstellplatzorganisati-
                                          on, die Sie bei der Laufbildung gewählt haben und der Status. Die Felder ISO,
                                          VSG, ESG und Glas zeigen Ihnen die im Lauf enthaltenen Mengen der jewei-
                                          ligen Art. Als letztes folgt eine Spalte für Meldungen. Hier sind folgende Texte
                                          möglich:

                                          .
                                          Symbol       Erläuterung

                                                       Die Ausgabe ist nicht korrekt, z. B. weil der Lauf nicht komplett
                                                       optimiert wurde.

                                                       Die Ausgabe ist korrekt.


                                          Tab. I-1      Erläuterung der Symbole

                                          Erläuterung der Felder im Bereich Optimierungen




                 Abb. I-49   Ausgabe, geöffnet aus der Optimierungsübersicht


                                          In der Spalte Optimierung wird Ihnen die Optimierungsnummer angezeigt. An-
                                          schließend sehen Sie das Datum, an dem die Optimierung erstellt wurde. Die
                                          Spalte Glasart zeigt Ihnen, welche Glasart optimiert wurde und die Spalte Mo-
                                          dus den dazugehörigen Optimierungsmodus. In der Spalte Schneidtisch kön-
2.21 / 01-2017




                                          nen Sie sehen, auf welchem Ihrer Schneidtische die Glasart geschnitten wird.
                                          Es folgt die Laufnummer und der Status, wie viele Stück optimiert wurden, wie
                                          groß die entsprechende Fläche ist und das Ergebnis.



                 I-64                                                              A+W Business Pro Production Manager
                 Tutorial                                                                                Expertenmodus




                                          Erläuterung der Felder im Bereich Reports




                 Abb. I-50   Bereich Reports


                                          In der Spalte Name wird Ihnen der Report angezeigt. Folgende Reports sind
                                          möglich:
                                          •    Produktionslisten (ISO, VSG, etc.)
                                          •    Handzuschnittlisten
                                          •    Rahmenlisten
                                          •    Sprossenlisten
                                          •    Abarbeitungslisten
                                          •    Abstellplatzübersichten
                                          •    Etiketten
                                          Im Anschluss folgt die Spalte Drucker. Über die Kombobox können Sie auf alle
                                          installierten Drucker zugreifen und den entsprechenden auswählen. Die Spal-
                                          te wird mit dem Drucker vorbelegt, der in den Stammdaten eingestellt wurde.
                                          Die Spalte Exemplare ist ebenfalls editierbar. Klicken Sie in die Spalte, öffnet
                                          sich das Feld zum Ändern der Anzahl. Sie können den vorgegebenen Wert
                                          überschreiben. Die Spalte Einstellungen verfügt über Kontextmenüs, die von
                                          der Art des Reports abhängig sind.
                                          Für Etiketten haben Sie die Möglichkeiten, das Verhalten beim Ausdruck von
                                          Serienetiketten zu steuern:




                                          Im Feld Serie ab geben Sie ein, ab welcher Stückzahl eine Serie beginnt. Über
                                          die Radiotasten darunter steuern Sie, ob ein Etikett pro Position oder ein Eti-
                                          kett pro Stück gedruckt werden soll. Bei der Variante ein Etikett pro Stück kön-
                                          nen Sie darüber hinaus im Feld dahinter noch angeben, alle wie viel Stück ein
                                          Etikett gedruckt werden soll.
                                          Für die Listen können Sie über das Kontextmenü einen Drucker für alle Listen
2.21 / 01-2017




                                          zuweisen. Das gleiche geht auch für Etiketten. Sie können weiterhin die An-
                                          zahl der Exemplare global einstellen.



                 A+W Business Pro Production Manager                                                                 I-65
                 Expertenmodus                                                                                 Tutorial




                                         Das in der Spalte Meldung angezeigt Symbol informiert Sie über den Stand.
                                         Grau hinterlegte Einträge werden nicht gedruckt, da eine Ausgabe an dieser
                                         Stelle nicht möglich ist. Beispiel: Wenn es sich um ein ISO handelt, ist der
                                         Druck VSG-Produktionsliste nicht möglich.




                 Abb. I-51   Bereich Maschinen


                                         Über diesen Bereich erfolgt die Ausgabe der Maschinencodes. Es werden au-
                                         tomatisch alle Maschinen gelistet, die an der Produktion beteiligt sind. Unab-
                                         hängig davon, ob es sich um Bieger oder Linien handelt. Im Feld Namen wird
                                         Ihnen der Maschinenname angezeigt. Im Feld Ausgabe sehen Sie das Ver-
                                         zeichnis, in dem der Maschinencode gespeichert wird. Über das Feld dahinter
                                         haben Sie die Möglichkeit, den Code in einem anderen Verzeichnis zu spei-
                                         chern.


                                         Ergänzende Informationen
                                          Softwarereferenz, “Ausgabe” auf Seite I-138
2.21 / 01-2017




                 I-66                                                          A+W Business Pro Production Manager
                 Tutorial                                                                           Expertenmodus




                                       Daten ausgeben
                                       In dieser Einheit lernen Sie, wie Sie Listen drucken und Schneidcode generie-
                                       ren.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So drucken Sie eine Liste
                                       •   So generieren Sie den Schneidcode für eine Maschine


                                        So drucken Sie eine Liste
                                       1 Wählen Sie im Bereich Optimierungen die Optimierung aus, für die die Lis-
                                         te gedruckt werden soll
                                       2 Wählen Sie im Bereich Reports die gewünschte Liste aus.
                                       3 Betätigen Sie die Symbol-Schaltfläche [Ausführen].
                                       4 Die Ausgabe wird gestartet.


                                        So generieren Sie den Schneidcode für eine Maschine
                                       1 Wählen Sie im Bereich Optimierungen die Optimierung aus, für die der
                                         Schneidcode erzeugt werden soll.
                                       2 Wählen Sie im Bereich Maschine diejenige aus, für die der Code erzeugt
                                         werden soll
                                       3 Betätigen Sie die Symbol-Schaltfläche [Ausführen].
                                       4 Die Ausgabe der Maschinenansteuerung wird gestartet.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Ausgabe” auf Seite I-138
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-67
                 Stammdaten                                                                    Tutorial




                              Stammdaten
                              In diesem Themenblock lernen Sie die Stammdaten des Produktionsmana-
                              gers kennen und erfahren, wie Sie damit umgehen.
                              Dazu gehören folgende Lerneinheiten:
                              •   “Abstellplätze” auf Seite I-70
                              •   “Kriterien” auf Seite I-78
                              •   “Gruppierung und Sortierung” auf Seite I-85
2.21 / 01-2017




                 I-68                                             A+W Business Pro Production Manager
                 Tutorial                                                                                       Stammdaten




                                       Abstellplätze
                                       Lernziele

                                       • Abstellplätze kennenlernen und verstehen
                                       • Abstellmodi kennenlernen und verstehen
                                       • Die Auswirkung der Abstellmodi verstehen


                                       Nutzen

                                       • Wenn Sie die Funktionen der Abstellmodi verstanden haben, können Sie Ihre
                                         Produktion entsprechend organisieren. Eine gut organisierte Produktion spart
                                         Ihnen Zeit und Platz und somit Geld.


                                       Definitionen

                                       Physikalischer Abstellplatz Gestell (A-Gestell, L-Gestell, Fester Abstellplatz)

                                       Logischer Abstellplatz       Ein logischer Abstellplatz besteht aus einem oder
                                                                    mehreren Stapeln von Glas und definiert, wie diese
                                                                    Stapel zusammen gehören (bspw. um daraus ISO oder
                                                                    VSG zu produzieren). Abhängig ist dies vom gewählten
                                                                    Stapelmodus. Ein logischer Abstellplatz ist einfach ein
                                                                    Bereich auf einem physikalischen Abstellplatz mit
                                                                    Nummer, auf welchen die zusammengehörigen
                                                                    Glasstapel gestellt werden.

                                       Abstellplatztiefe            Über die Abstellplatztiefe definieren Sie die maximale
                                                                    Stapeltiefe (maximale Beladung) des Abstellplatzes.
                                                                    Geben Sie hier einen größeren Wert ein, können Sie
                                                                    mehr Scheiben voreinander stapeln.


                                       Merke

                                       Was darf auf einen           In einen Stapel oder auf einen Fächerwagen dürfen
                                       Abstellplatz?                grundsätzlich nur Teile aus einem Los.

                                       Verschiedene Glasarten auf Das Programm trennt grundsätzlich verschiedenen
                                       einen Stapel               Glasarten und weist sie verschiedenen Stapeln zu.

                                       Abstellmodus                 Verschiedene Glasarten können auf einem logischen
                                                                    Abstellplatz kombiniert werden.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                     I-69
                 Stammdaten                                                                                               Tutorial




                              Logische Abstellplätze und Abstellplatztiefe
                              Ein logischer Abstellplatz besteht aus einem oder mehreren Stapeln von Glas
                              und definiert, wie diese Stapel zusammen gehören (bspw. um daraus ISO
                              oder VSG zu produzieren).
                              Ein logischer Abstellplatz ist nur ein Bereich auf einem physikalischen Abstell-
                              platz mit einer Nummer, auf welchen die zusammengehörigen Glasstapel ge-
                              stellt werden.Das Abstellen von Scheiben auf den logischen Abstellplätzen
                              geschieht in der für den jeweiligen Abstellplatz definierten Produktionsreihen-
                              folge.
                              Aus den logischen Abstellplätzen werden physikalische Gestelle gebildet.
                              Dies geschieht für A-Böcke und L-Böcke unter Berücksichtigung der Gestell-
                              tiefe sowie der Anzahl der Gestellseiten (1 oder 2 für L- bzw. A-Gestell).




                                                                                                                 Abstellplatztiefe




                                                                                   Log. Abstellpl. 1001   Log. Abstellpl. 1002
                                       Abstellplatz Seitenansicht
                                                                                             Abstellplatz - Draufsicht
                              Abstellplatztiefe           Abstellplatztiefe


                              Abb. I-52           Logische Abstellplätze und Abstellplatztiefe


                              Über die Abstellplatztiefe definieren Sie die maximale Stapeltiefe (maximale
                              Beladung) des Abstellplatzes. Geben Sie hier einen größeren Wert ein, kön-
                              nen Sie mehr Scheiben voreinander stapeln.
                              Wenn die Abstellplatztiefe und damit die maximale Beladung erreicht ist, wird
                              ein neuer Stapel begonnen.
2.21 / 01-2017




                 I-70                                                         A+W Business Pro Production Manager
                 Tutorial                                                                                              Stammdaten




                                       Abstellmodus für A-Böcke
                                       Der Production Manager arbeitet mit einem Abstellmodus, in dem verschiede-
                                       ne Glasarten auf einem logischen Abstellplatz in mehreren Stapeln kombiniert
                                       abgestellt werden können. Es ist möglich, verschiedene Kombinationen von
                                       Produkten, welche gefertigt werden sollen, abzustellen.


                                           Grp.3   Float 4                                               Abstellplatztiefe

                                                                               Float 6

                                                                               Float 6
                                                   Float 4
                                                                                                       Thermisch

                                                                               Float 6




                                                                                               Grp.4
                                                    Float 4


                                                                                                       Thermisch
                                                                 Log. Abstellplatz 1001
                                                                       Draufsicht


                                       Abb. I-53              Abstellmodus für A-Böcke


                                       •           Jede Glasart befindet sich in einem anderen Stapel.
                                       •           Unterschiedliche Glasarten werden zusammen auf einem logischen (oder
                                                   physikalischen) Abstellplatz gestellt.
                                       •           Sobald ein Stapel das Maximum erreicht, ist die ganze Abstellplatznummer
                                                   "voll".
                                       •           Zusammengehörige Gruppen müssen definiert und beibehalten werden.
                                       •           Sie benötigen weniger physikalische Gestelle.
                                       •           Sie benötigen zusätzliche Hilfs- und Kontrollmechanismen wie bspw. Pro-
                                                   duktionspapiere oder Anzeigesysteme um die Kontrolle zu behalten.

                                                   Trennung von Glasarten
                                                   Das Programm trennt immer die Glasarten. Das gilt sowohl für das Abstel-
                                                   len der Glasarten als auch für die Optimierung.

                                       Abstellen geteilter Gruppen
                                       Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die
                                       Scheiben dieser Gruppe, die über der max. Beladung (Abstellplatztiefe) sind,
                                       und die betreffenden Scheiben der entsprechenden Gruppe innerhalb des an-
                                       deren Abstellplatzes gehen zusammen auf einen neuen Abstellplatz - mit ei-
                                       ner neuen Abstellplatznummer. (Gruppe 3 ist über dem Limit, also geht die
                                       letzte Scheibe der Gruppe 3 und die letzte Scheibe der Gruppe 4 auf einen
                                       neuen Abstellplatz: 1002). Auf diesem neuen Abstellplatz können Sie neue
                                       Glasarten und neue Gruppen abstellen. Abstellplatz 1001 gilt als voll, Abstell-
                                       platz 1002 kann mit weiteren Gruppen beladen werden, bis auch hier die ma-
                                       ximale Beladung erreicht wird.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                         I-71
                 Stammdaten                                                                                                            Tutorial




                                                                                                                        Abstellplatztiefe

                                                      Float 6
                  Grp.3




                                                      Float 6
                          Float 4


                                                       Float 6
                          Float 4




                                                                                                                              Grp.4
                                                                                                    Grp.3
                                                                               Thermisch                    Float 4                 Thermisch
                                     Logischer Abstellplatz 1001                                                Logischer Abstellplatz 1002
                                            Draufsicht                                                                  Draufsicht




                 Abb. I-54          Abstellen geteilter Gruppen


                                                     Auffangabstellplatz
                                                     Zu jedem der drei Bereiche ISO, VSG und Glas gibt es einen speziellen Ab-
                                                     stellplatz, der alle Stücklistenelemente auffängt, die auf keinem regulären Ab-
                                                     stellplatz landen. Bei diesen drei Abstellplätzen handelt es sich um A-Gestelle
                                                     mit einer unbegrenzte Abstellplatztiefe und festen Abstellplatznummern
                                                     9991(Glas), 9992 (VSG) und 9993 (ISO).

                                                         Sich überlappende Nummern
                                                         Bei der Zuordnung der Abstellplätze zur Abstellplatzorganisation wird je-
                                                         weils geprüft, ob die verwendeten Abstellplatznummern (von - bis) sich
                                                         nicht mit anderen oder den festen Abstellplatznummern 9991, 9992 und
                                                         9993 überlappen. Überlappende Bereiche sind nicht möglich! In ein sol-
                                                         chen Fall erfolgt ein Hinweis, welche Überlappungen existieren. Die Kon-
                                                         flikte müssen dann beseitigt werden.
2.21 / 01-2017




                 I-72                                                                      A+W Business Pro Production Manager
                 Tutorial                                                                                   Stammdaten




                                       Gestelle anlegen und verwalten
                                       Die Werte kommt aus den Stammdaten (Fertigung > Abstellplatzorganisation).
                                       Dort können Sie die Gestellarten anlegen und verwalten:
                                       Stammdaten > Fertigung > Logische Abstellplätze




                                       Abb. I-55     Logische Abstellplätze


                                       Der Dialog ist in mehrere Bereiche eingeteilt. Oben links befinden sich die Fel-
                                       der Abstellplatzname und Typ. Bei dem Typ handelt es sich um den entspre-
                                       chenden Feinplanungstyp aus. Es stehen folgende Typen zur Verfügung:
                                       •   ISO
                                       •   VSG
                                       •   Glas (Einzelgläser als fertige, auszuliefernde Gläser oder bearbeitete Glä-
                                           ser)

                                           Feinplanungstyp und Gestelle
                                           Die an dieser Stelle getroffene Zuordnung stellt auch sicher, dass die
                                           Scheiben auf die entsprechenden Gestelle kommen. D. h. wenn Sie bspw.
                                           den Feinplanungstyp VSG auswählen, dann kommen die Scheiben auto-
                                           matisch auf die Gestelle für VSG. Ein zusätzlicher Filter (Kriterium) ist nicht
                                           nötig. Innerhalb Abstellplatzorganisation der VSG-Gestelle (Zuordnung)
2.21 / 01-2017




                                           können Sie dann durch Kriterien bspw. zwischen Modellen und Recht-
                                           ecken unterscheiden und diese auf verschiedene Abstellplatznummern
                                           verteilen.


                 A+W Business Pro Production Manager                                                                 I-73
                 Stammdaten                                                                       Tutorial




                              Der Bereich darunter betrifft die Gruppierungen und Sortierungen innerhalb
                              der Gruppen. Sie können an dieser Stelle vorhandene Gruppierungen zuwei-
                              sen und festlegen, ob Gruppen sortiert werden sollen.
                               “Sortierschlüssel” auf Seite I-81
                              Anschließend finden Sie die Daten zu den physikalischen Abstellplätzen. Als
                              erstes kommt der Name des physikalischen Abstellplatzes, dann wählen Sie
                              aus der Kombobox Typ den entsprechenden Typ (A-Gestell, Fächerwagen, L-
                              Gestell) aus. Das Feld Tiefe kann nur ausgefüllt werden, wenn es sich beim
                              Typ um ein A- oder ein L-Gestell handelt. In diesem Fall geben Sie dort die
                              Tiefe Abstellplatzes ein. Das Feld Anzahl Fächer ist hingegen kann nur aus-
                              gefüllt werden, wenn es sich bei dem Abstellplatz um einen Fächerwagen han-
                              delt. Dann geben Sie hier ein, wie viele Fächer der Wagen hat. Das Feld
                              Scheiben pro Fach kommt auch nur bei Fächerwagen zum Einsatz und gibt
                              an, wie viele Scheiben in ein Fach gestellt werden können.
                              Die Felder Gestell Nr. von bis kennzeichnen den Nummernbereich für den je-
                              weiligen Abstellplatz.


                              Ergänzende Informationen
                               Softwarereferenz, “Logische Abstellplätze” auf Seite I-95
2.21 / 01-2017




                 I-74                                                A+W Business Pro Production Manager
                 Tutorial                                                                               Stammdaten




                                       Abstellplatzgruppen
                                       Abstellplatzgruppen dienen dazu, Abstellplätze vor der ISO-Linie bzw. dem
                                       VSG-Verbund im Wechsel abzuarbeiten. Sie sind dann erforderlich, wenn
                                       eine abstellplatzübergreifende Produktionsreihenfolge gewünscht wird. Ab-
                                       stellplätze, die keiner Abstellplatzgruppe zugeordnet sind, können in wahlfrei-
                                       er Abfolge zur Produktion verwendet werden.
                                       Beispiel:
                                       Scheiben (aus einer Abstellplatzgruppe) kleiner als 2500 x 1400 stehen in Fä-
                                       cherwagen. Alle anderen Scheiben auf A-Böcken. Die gewünschte Produkti-
                                       onsreihenfolge ist: Auftragsweise (Auftrag A, Auftrag B, Auftrag C).
                                       Scheiben von Auftrag A, B und C stehen sowohl in Fächerwagen als auch auf
                                       A-Böcken. In diesem Fall müssen für die ISO-Fertigung beide Abstellplätze
                                       gleichzeitig im Zugriff sein. Bei der Fertigung der ISO-Einheiten des Auftrags
                                       A müssen (abhängig von der Größe der Scheiben) manchmal Scheiben aus
                                       dem Fächerwagen und manchmal vom A-Gestell genommen werden. Diese
                                       Arbeitsweise kann nur durch die Verwendung einer Abstellplatzgruppe inner-
                                       halb der Abstellplatzorganisation erreicht werden.
                                       Der Abstellplatzgruppe wird ein Sortierschlüssel zugeordnet. Dieser Schlüssel
                                       sortiert die Teile, die auf den zur Gruppe gehörenden Abstellplätzen stehen.
                                       Die entsprechenden Einstellungen werden im Dialog Abstellplatzgruppen vor-
                                       genommen.
                                       Stammdaten > Fertigung > Logische Abstellplatzgruppen
2.21 / 01-2017




                                       Abb. I-56    Abstellplatzgruppen




                 A+W Business Pro Production Manager                                                             I-75
                 Stammdaten                                                                        Tutorial




                              Mit Abstellplatzgruppen arbeiten
                              In dieser Einheit lernen Sie, wie Sie mit Abstellplatzgruppen umgehen.
                              Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                              •   So legen Sie eine neue Abstellplatzgruppe an
                              •   So ändern Sie eine bestehende Abstellplatzgruppe
                              •   So löschen Sie eine Abstellplatzgruppe


                               So legen Sie eine neue Abstellplatzgruppe an
                              1 Klicken Sie auf die Symbol-Schaltfläche [Neu].
                              2 Geben Sie im Feld Namen den gewünschten Namen ein.
                              3 Wählen Sie aus der Kombobox Sortierschlüssel die entsprechende Sortie-
                                rung aus.
                              4 Klicken Sie auf die Symbol-Schaltfläche [Speichern].


                               So ändern Sie eine bestehende Abstellplatzgruppe
                              1 Markieren Sie im Bereich Abstellplatzgruppen die Gruppe, die geändert
                                werden soll.
                              2 Nehmen Sie die gewünschten Änderungen vor. Sie können sowohl den
                                Namen als auch den Sortierschlüssel ändern.
                              3 Klicken Sie auf die Symbol-Schaltfläche [Speichern].


                               So löschen Sie eine Abstellplatzgruppe
                              1 Markieren Sie im Bereich Abstellplatzgruppen die Gruppe, die gelöscht
                                werden soll.
                              2 Klicken Sie auf die Symbol-Schaltfläche [Löschen].
                              3 Es erfolgt eine Sicherheitsabfrage. Klicken Sie auf [Ja].
                              4 Der Eintrag wird gelöscht.


                              Ergänzende Informationen
                               Softwarereferenz, “Abstellplatzgruppen” auf Seite I-97
2.21 / 01-2017




                 I-76                                                A+W Business Pro Production Manager
                 Tutorial                                                                                 Stammdaten




                                         Kriterien
                                         Kriterien prüfen, ob ein bestimmtes Stücklistenelement einem logischen Ab-
                                         stellplatz zugewiesen werden kann. Sie sind nichts anderes als ein datentech-
                                         nisches Regelwerk, welches über Formeln festgelegt, ob ein Element die
                                         angegebenen Bedingungen des logischen Abstellplatzes erfüllt.
                                         Unter Umständen ist es gewünscht, Scheiben abhängig von einem bestimm-
                                         ten Kriterium einem neuen Folgeabstellplatz zuzuordnen. Dies geschieht
                                         dann über die Checkbox Abstellplatzwechsel bei. Der bereits teilbeladene Ab-
                                         stellplatz wird nicht weiter beladen.
                                         Stammdaten > Fertigung > Kriterien
                                         Der zugehörige Dialog sieht wie folgt aus:




                 Abb. I-57   Kriterien


                                         Der Dialog ist in mehrere Bereiche eingeteilt. Im oberen Bereich befinden sich
                                         die Angaben zu dem selektierten Kriterium.
2.21 / 01-2017




                                         Abb. I-58    Bereich Kriterium



                 A+W Business Pro Production Manager                                                              I-77
                 Stammdaten                                                                         Tutorial




                              Im Feld Name wird Ihnen der Name des Krtieriums angezeigt. Den Namen
                              können Sie frei vergeben. Im Feld Beschreibung sehen Sie eine entsprechen-
                              de nähere Beschreibung, die Sie ebenfalls frei wählen können. Der Bereich
                              Formel zeigt Ihnen die Formel, aus der sich das Kriterium zusammensetzt.
                              Beispiel:
                              •   Große Scheiben auf Abstellplatz 1000
                              •   Modellscheiben auf Abstellplatz 2000
                              Da die Kriterien der Zuordnung sich nicht gegenseitig ausschließen, z. B. gro-
                              ße Modellscheiben, kann mit hilfe des Registers Prüfreihenfolge (Stammdaten
                              > Fertigung > Abstellplatzorganisation) die Priorität der Kriterien festgelegt
                              werden.

                              Formel
                              Unter dem Begriff Formel verstehen wir eine (mathematische) Funktion auf
                              den Eigenschaften der Stücklistenelemente, die einen Wert (Variable) hat. Die
                              Variablen, die in Formeln verwendet werden können, haben englische Be-
                              zeichnungen und werden in der jeweiligen Landessprache angezeigt, bspw.
                              Width (Breite).


                              Ergänzende Informationen
                               Softwarereferenz, “Kriterien” auf Seite I-93
2.21 / 01-2017




                 I-78                                                 A+W Business Pro Production Manager
                 Tutorial                                                                             Stammdaten




                                       Mit Kriterien arbeiten
                                       In dieser Einheit lernen Sie, wie Sie mit Kriterien umgehen.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So legen Sie ein neues Kriterium an
                                       •   So ändern Sie ein bestehendes Kriterium
                                       •   So löschen Sie ein Kriterium


                                        So legen Sie ein neues Kriterium an
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Neu].
                                       2 Vergeben Sie im Feld Name den gewünschten Namen, z. B. Serien.
                                       3 Im Feld Beschreibung können Sie eine ergänzende Beschreibung hinter-
                                         legen, z. B. Menge > 15.
                                       4 Im Feld Formel weisen Sie die Kriterien der Formel aus der Baumstruktur
                                         rechts zu. Bsp.: Eintrag Menge (Quantity) doppelt anklicken, dann er-
                                         scheint der Eintrag im Bereich Formel. Anschließend gehen Sie mit der
                                         Maus direkt hinter den Eintrag und geben >15 ein.


                                        So ändern Sie ein bestehendes Kriterium
                                       1 Markieren Sie im Bereich Auswahl den Eintrag, der geändert werden soll.
                                       2 Nehmen Sie im Bereich Kriterium die entsprechenden Änderungen vor.
                                       3 Betätigen Sie die Symbol-Schaltfläche [Speichern]


                                        So löschen Sie ein Kriterium
                                       1 Markieren Sie im Bereich Auswahl die Formel, die gelöscht werden soll.
                                       2 Klicken Sie auf die Symbol-Schaltfläche [Löschen].
                                       3 Es erfolgt eine Sicherheitsabfrage. Klicken Sie auf [Ja].
                                       4 Der Eintrag wird gelöscht.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Kriterien” auf Seite I-93
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                        I-79
                 Stammdaten                                                                         Tutorial




                              Sortierschlüssel
                              Um eine Menge von Elementen zu sortieren, kommen sog. Sortierschlüssel
                              zum Einsatz. Ein Sortierschlüssel kann ein einzelnes Feld, wie z. B Auftrags-
                              nummer oder Kundennummer sein oder aus der Verkettung mehrerer Felder
                              bestehen. Innerhalb der Abstellplatzorganisation wird einer Abstellplatzgrup-
                              pe ein Sortierschlüssel zugeordnet. Dieser Schlüssel sortiert die Teile inner-
                              halb einer Gruppe.
                              Die entsprechenden Einstellungen werden im Dialog Sortierschlüssel vorge-
                              nommen.
                              Stammdaten > Fertigung > Sortierschlüssel




                              Abb. I-59     Sortierschlüssel


                              Der Dialog ist in unterschiedliche Bereiche unterteilt. Im oberen Bereich wird
                              Ihnen der Name des Sortierschlüssels angezeigt.
                              Der Bereich Sortierschlüssel zeigt Ihnen den Namen und die Vorschau. Die
                              Felder Formel und Sortierung im Bereich Details sind Komboboxen, die auf-
                              geklappt werden können. Die Kombobox Formel enthält alle im Dialog Kriteri-
                              um (Stammdaten > Fertigung > Kriterien) angelegten Werte. Über die
                              Kombobox Sortierung können Sie steuern, ob die Sortierung auf- oder abstei-
                              gend ist.
                              Die Sortierschlüssel dienen auch als Gruppierung und Sortierung in den Grup-
                              pen auf den logischen Abstellplätzen.
2.21 / 01-2017




                              Ergänzende Informationen
                               Softwarereferenz, “Sortierschlüssel” auf Seite I-98



                 I-80                                                 A+W Business Pro Production Manager
                 Tutorial                                                                              Stammdaten




                                       Mit Sortierschlüsseln arbeiten
                                       In dieser Einheit lernen Sie, wie Sie mit den Sortierschlüsseln umgehen.
                                       Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
                                       •   So legen Sie einen neuen Sortierschlüssel an
                                       •   So ändern Sie eine bestehende Abstellplatzgruppe
                                       •   So löschen Sie einen Sortierschlüssel


                                        So legen Sie einen neuen Sortierschlüssel an
                                       1 Klicken Sie auf die Symbol-Schaltfläche [Neu].
                                       2 Geben Sie im Feld Namen den gewünschten Namen ein, z. B. Auftrag.
                                       3 Wählen Sie aus der Kombobox Formel den gewünschten Eintrag aus.
                                       4 Wählen Sie aus der Kombobox Sortierung die gewünschte Sortierung aus.
                                       5 Klicken Sie auf die Symbol-Schaltfläche [Speichern].


                                        So ändern Sie eine bestehende Abstellplatzgruppe
                                       1 Markieren Sie im Bereich Sortierschlüssel den Eintrag, die geändert wer-
                                         den soll.
                                       2 Nehmen Sie die gewünschten Änderungen für die Felder Formel und Sor-
                                         tierung vor.
                                       3 Klicken Sie auf die Symbol-Schaltfläche [Speichern].


                                        So löschen Sie einen Sortierschlüssel
                                       1 Markieren Sie im Bereich Sortierschlüssel den Eintrag, der gelöscht wer-
                                         den soll.
                                       2 Klicken Sie auf die Symbol-Schaltfläche [Löschen].
                                       3 Es erfolgt eine Sicherheitsabfrage. Klicken Sie auf [Ja].
                                       4 Der Eintrag wird gelöscht.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Sortierschlüssel” auf Seite I-98
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-81
                 Stammdaten                                                                             Tutorial




                              Abstellplatzorganisation
                              Im Programm können, auf den jeweiligen Produktionsbetrieb zugeschnitten,
                              unterschiedliche Abstellplatzorganisationen angelegt werden.
                              Eine dieser Abstellplatzorganisationen kann als Standardorganisation ausge-
                              wählt werden. Bei der Erstellung des Laufes wird dann standardmäßig diese
                              Abstellplatzorganisation dem Lauf zugeordnet. Vor der eigentlichen Feinpla-
                              nung können Sie diese Zuordnung noch ändern.
                              Die Abstellplatzorganisation beschreibt im Wesentlichen die folgenden Aspek-
                              te der Produktion:

                              Welche Produkte werden produziert (Was):
                              Im ersten Schritt werden die unterschiedliche Produktarten, die zu einem Lauf
                              zusammengefasst werden (ISO, VSG, ESG, bearbeitete Gläser) mittels der
                              Abstellplatzorganisation in folgende drei Typen eingeteilt:
                              •   ISO
                              •   VSG
                              •   Glas (enthält auch ESG).
                              Durch diese Einteilung entstehen Lostypen.

                              Auf welchen Abstellplätzen werden beteiligte Scheiben oder Zwi-
                              schenprodukte abgestellt (Wo):
                              Im zweiten Schritt wird entschieden, auf welchen logischen Abstellplatz die
                              beteiligten Gläser des jeweiligen (Zwischen-) Produktes abgestellt werden.
                              Dazu wird das Kriterium eines jeden logischen Abstellplatzes mit den Eigen-
                              schaften des einzusortierenden (Zwischen-) Produktes berechnet und sobald
                              dieses Kriterium bei einem logischen Abstellplatz zutrifft, wird das (Zwischen-
                              ) Produkt diesem logischen Abstellplatz zugeordnet. Wenn für ein (Zwischen-
                              ) Produkt keines der Kriterien der Abstellplatzorganisation zutrifft, so geht die-
                              ses (Zwischen-) Produkt auf den automatisch generierten Auffängerabstell-
                              platz.

                              Wie ist der zeitliche und organisatorische Ablauf der Produktion
                              (Wie):
                              Im Dialog der Abstellplatzorganisation sind alle in Ihrem Haus definierten Ab-
                              stellplatzorganisationen aufgeführt.
                              Die Abfolge der Zeilen von oben nach unten entspricht der zeitlichen Abfolge,
                              in der die logischen Abstellplätze vor der ISO-Linie (Typ ISO) bzw. vor dem
                              VSG-Verbund (Typ VSG) abgearbeitet werden. D. h., die Scheiben werden
                              von diesen Abstellplätzen zur jeweiligen Fertigung der entsprechenden Ein-
                              heit abgenommen.
                              Scheiben, die einem logischen Abstellplatz zugeordnet werden, stehen in der
                              Realität auf sogenannten physikalischen Abstellplätzen (Fächerwagen, A-Ge-
                              stell, L-Gestell). Diese physikalischen Abstellplätze haben natürliche Restrik-
2.21 / 01-2017




                              tionen, wie z. B. Anzahl der Fächer oder Gestelltiefe. Um dies zu
                              berücksichtigen, werden die Teile, die aufgrund eines bestimmten Kriteriums




                 I-82                                               A+W Business Pro Production Manager
                 Tutorial                                                                                     Stammdaten




                                          einem logischen Abstellplatz zugewiesen werden, zusätzlich auf physikali-
                                          sche Abstellplätze verteilt.
                                          Bei A-Gestellen ist das Kriterium die Gestelltiefe, die bei der Sortierreihenfolge
                                          (Brechreihenfolge) der Scheiben berücksichtigt wird. Die Gestelltiefe ent-
                                          scheidet darüber, wie viele physikalische Abstellplätze erforderlich sind, um
                                          die in einem Lauf befindlichen Scheiben auf diese Abstellplätze zu verteilen.
                                          Der zugehörige Dialog sieht wie folgt aus:
                                          Stammdaten > Fertigung > Abstellplatzorganisation




                 Abb. I-60   Abstellplatzorganisation


                                          Ergänzende Informationen
                                           Softwarereferenz, “Abstellplatzorganisation” auf Seite I-90
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                   I-83
                 Stammdaten                                                                             Tutorial




                              Gruppierung und Sortierung
                              Lernziele

                              • Gruppierungen kennenlernen und verstehen
                              • Sortierungen kennenlernen und verstehen
                              • Die Auswirkungen von Gruppierungen und Sortierungen verstehen.


                              Nutzen

                              • Über die Gruppierungen und Sortierungen wird das Abstellen der einzelnen
                                Scheiben in der von Ihnen gewünschten Reihenfolgen organisiert. Ohne diese
                                Gruppierungen und/oder Sortierungen müssten die Scheiben vor dem jeweiligen
                                nächsten Produktionsschritt immer neu sortiert werden.


                              Definitionen

                              Gruppierung               Erfolgt nach unterschiedlichen und eindeutigen Werten
                                                        für eine Eigenschaft, z. B. nach Kundennummer,
                                                        Glasdicke.

                              Sortierung                Erfolgt nach Eigenschaften, die einen fortlaufenden Wert
                                                        innerhalb der gegebenen Gruppe annehmen
                                                        (beispielsweise Größe).


                              Merke

                              Bildung                   Gruppierungen und Sortierungen werden durch eine
                                                        beliebige Kombination aus Eigenschaften und Formeln
                                                        gebildet.
2.21 / 01-2017




                 I-84                                              A+W Business Pro Production Manager
                 Tutorial                                                                               Stammdaten




                                       Allgemein
                                       Die Gruppierungen und Sortierungen dienen dazu, den verschiedenen Ab-
                                       stellplätzen die gewünschte Produktionsreihenfolge zuzuweisen.
                                       Der Production Manager erlaubt es Ihnen, Gruppierungskriterien zu definieren
                                       und gibt Ihnen die Möglichkeit zu entscheiden, ob die Gruppierung in einer ge-
                                       wissen Reihenfolge (sortierte Gruppen) sein soll und ob die Inhalte der Grup-
                                       pen sortiert sein sollen (Sortierung innerhalb der Gruppe). Jeder logische
                                       Abstellplatz kann seine eigene Gruppierung und Sortierung haben.
                                       Die Optimierung berechnet unter Berücksichtigung von Gruppierung und Sor-
                                       tierung den bestmöglichen Verschnitt. Einmal eingerichtet, kann die so ermit-
                                       telte Reihenfolge für passende Scheiben einer ISO- und VSG-Einheit
                                       verwendet werden.

                                                           Gruppiert nach Glasart




                                         Sortiert nach Abmessung

                                       Abb. I-61     Gruppierung und Sortierung


                                       Die Grafik oben zeigt eine Gruppierung nach der Glasdicke. Innerhalb jeder
                                       Gruppe (eventuell ein Gestell pro Dicke) erfolgt die Sortierung nach der Höhe.
                                       Gruppierung und Sortierung hängen davon ab, wie die Produktion in Ihrem
                                       Hause aufgebaut ist und abläuft. Sie werden durch eine beliebige Kombination
                                       aus Eigenschaften und Formeln gebildet.
                                       Gruppiert wird nach unterschiedlichen und eindeutigen Werten für eine Eigen-
                                       schaft wie z. B. nach Kundennummer, Glasdicke/-farbe, Modelltyp. Es kann
                                       nach unterschiedlichen Kriterien gruppiert werden, ohne dass innerhalb der
                                       Gruppen eine Sortierung vorhanden sein muss.
                                       Die entsprechenden Einstellungen werden im Dialog Sortierschlüssel vorge-
                                       nommen.


                                       Ergänzende Informationen
                                        “Sortierschlüssel” auf Seite I-81
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-85
                 Stammdaten                                Tutorial
2.21 / 01-2017




                 I-86         A+W Business Pro Production Manager
Produktionsmanager                 I

                     Softwarereferenz




            A+W Business Pro
                 Softwarereferenz                                                                           Übersicht




                                       Übersicht
                                       Menü Stammdaten > Fertigung öffnen
                                       Im Modul Stammdaten (Bereich Fertigung) werden alle Daten zum Produkti-
                                       onsmanager eingerichtet und gepflegt, die zu einer korrekten Arbeitsweise be-
                                       nötigt werden.
                                       Die Stammdaten sind in folgende Menüs gegliedert:
                                       •   Abstellplatzorganisation:
                                           Mit diesem Menüpunkt richten Sie Abstellplatzorganisationen ein.
                                            “Abstellplatzorganisation” auf Seite I-90
                                       •   Kriterien:
                                           Mit diesem Menüpunkt legen Sie die Kriterien an.
                                            “Kriterien” auf Seite I-93
                                       •   Logische Abstellplätze:
                                           Mit diesem Menüpunkt legen Sie die logischen Abstellplätze an.
                                            “Logische Abstellplätze” auf Seite I-95
                                       •   Abstellplatzgruppen:
                                           Mit diesem Menüpunkt legen Sie die Abstellplatzgruppen an.
                                            “Abstellplatzgruppen” auf Seite I-97
                                       •   Sortierschlüssel:
                                           Mit diesem Menüpunkt legen Sie die Sortierschlüssel an.
                                            “Sortierschlüssel” auf Seite I-98

                                           Schaltflächen in den Dialogen
                                           Die Standard-Schaltflächen und -menüs sind ausführlich im Part Übersicht
                                           und in den Tutorials beschrieben. Auf sie wird daher in der Beschreibung
                                           der Dialoge nicht eingegangen.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-89
                 Übersicht                                                               Softwarereferenz




                             Abstellplatzorganisation
                             Stammdaten > Fertigung > Abstellplatzorganisation




                             Abb. I-62    Abstellplatzorganisation


                             In diesem Dialog definieren Sie die Abstellplatzorganisation oder nehmen Än-
                             derungen an vorhandenen Organisationen vor.

                             Erläuterung der Felder im Bereich Auswahl

                             Name In diesem Feld geben Sie den Namen der Abstellplatzorganisation ein
                             oder ändern den Namen einer bereits vorhandenen Abstellplatzorganisation.

                             Standard Mit der Checkbox steuern Sie, ob die Abstellplatzorganisation als
                             Standardorganisation dienen soll. Es kann immer nur eine Abstellplatzorgani-
                             sation als Standard dienen.
                              Die Abstellplatzorganisation ist nicht die Standardorganisation.
                              Bei dieser Abstellplatzorganisation handelt es sich um die Standardorgani-
                             sation.
2.21 / 01-2017




                 I-90                                                A+W Business Pro Production Manager
                 Softwarereferenz                                                                           Übersicht




                                       Erläuterung der Felder im Bereich Abstellplatzorganisation

                                       Name In diesem Feld wird Ihnen der Namen der Abstellplatzorganisation an-
                                       gezeigt.

                                       Standard Mit der Checkbox steuern Sie, ob die Abstellplatzorganisation als
                                       Standardorganisation dienen soll. Mögliche Werte:
                                       • Ja: Bei der Abstellplatzorganisation handelt es sich um die Standardorga-
                                          nisation.
                                       • Nein: Die Abstellplatzorganisation ist keine Standardorganisaton.

                                       Erläuterung der Felder im Bereich Details

                                       Typ In diesem Feld wird Ihnen der Feinplanungstyp angezeigt. Möglichen
                                       Werte sind:
                                       • ISO
                                       • VSG
                                       • Glas

                                       Formel In diesem Feld wird Ihnen die Formel für Abstellplatzorganisation an-
                                       gezeigt. Die Werte kommen aus den Kriterien (Stammdaten > Fertigung > Kri-
                                       terien). Über die Pfeiltaste am Ende des Feldes haben Sie Zugriff auf alle
                                       definierten Kriterien und können diese hier zuweisen.

                                       Abstellplatz (log.) In diesem Feld wird Ihnen der logische Abstellplatz ange-
                                       zeigt. Die Werte kommen aus den logischen Abstellplätzen (Stammdaten >
                                       Fertigung > Logische Abstellplätze). Über die Pfeiltaste am Ende des Feldes
                                       haben Sie Zugriff auf alle definierten logischen Abstellplätze und können diese
                                       hier zuweisen.

                                       Abstellplatzgruppe n diesem Feld wird Ihnen die Abstellplatzgruppe ange-
                                       zeigt. Die Werte kommen aus den Abstellplatzgruppen (Stammdaten > Ferti-
                                       gung > Abstellplatzgruppen). Über die Pfeiltaste am Ende des Feldes haben
                                       Sie Zugriff auf alle definierten Abstellplatzgruppen und können diese hier zu-
                                       weisen.

                                       Produktionsreihenfolge Hat die Abstellplatzorganisation mehr als einen
                                       Feinplanungstyp, müssen Sie die entscheiden, wie die Produktionsreihenfol-
                                       ge sein soll. Die Reihenfolge wird durch Zahlen gekennzeichnet. 1 bedeutet,
                                       dass dieser Feinplanungstyp zuerst produziert wird, dann 2, usw. Um Zahlen
                                       zu ändern, klicken Sie mit der Maus in das Feld und überschreiben die Zahl.

                                       Prüfreihenfolge Über dieses Feld legen Sie die Reihenfolge fest, in der die
                                       logischen Abstellplätze geprüft werden.

                                       Gestell Nr. (von) In diesem Feld wird Ihnen der Beginn des Gestellnum-
                                       mernkreises für den Abstellplatz angezeigt. Die Werte kommen aus den logi-
                                       schen Abstellplätzen (Stammdaten > Fertigung > Logische Abstellplätze).
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                             I-91
                 Übersicht                                                                Softwarereferenz




                             Gestell Nr. (bis) In diesem Feld wird Ihnen das Ende des Gestellnummern-
                             kreises für den Abstellplatz angezeigt. Die Werte kommen aus den logischen
                             Abstellplätzen (Stammdaten > Fertigung > Logische Abstellplätze).

                             Gestell Nr. (aktuell) In diesem Feld wird Ihnen die aktuelle Gestellnummer
                             angezeigt.

                             Abstellplatz (phys.) In diesem Feld wird Ihnen der Name des physikalischen
                             Abstellplatzes angezeigt. Die Werte kommen aus den logischen Abstellplät-
                             zen (Stammdaten > Fertigung > Logische Abstellplätze).

                             Gestelltiefe In diesem Feld wird Ihnen die Tiefe des physikalischen Abstell-
                             platzes angezeigt, wenn es sich bei dem Abstellplatz um ein A- oder L-Gestell
                             handelt. Die Werte kommen aus den logischen Abstellplätzen (Stammdaten >
                             Fertigung > Logische Abstellplätze).

                             Anzahl Fächer Wenn es sich bei dem Abstellplatz um einen Fächerwagen
                             handelt, wird Ihnen in diesem Feld angezeigt, wie viele Fächer der Fächerwa-
                             gen hat. Die Werte kommen aus den logischen Abstellplätzen (Stammdaten >
                             Fertigung > Logische Abstellplätze).

                             Anzahl Scheiben pro Fach Wenn es sich bei dem Abstellplatz um einen Fä-
                             cherwagen handelt, wird Ihnen in diesem Feld angezeigt, wie viele Scheiben
                             in ein Fach gestellt werden können. Die Werte kommen aus den logischen Ab-
                             stellplätzen (Stammdaten > Fertigung > Logische Abstellplätze).


                             Ergänzende Informationen
                              Tutorial, “Abstellplätze” auf Seite I-70
2.21 / 01-2017




                 I-92                                                 A+W Business Pro Production Manager
                 Softwarereferenz                                                                           Übersicht




                                       Kriterien
                                       Stammdaten > Fertigung > Kriterien




                                       Abb. I-63    Kriterien


                                       In diesem Dialog definieren Sie die Kriterien für die Abstellplätze oder nehmen
                                       Änderungen an diesen vor.

                                       Erläuterung der Felder im Bereich Auswahl

                                       Name In diesem Feld geben Sie den Namen des Kriteriums ein oder ändern
                                       den Namen eines bereits vorhandenen Kriteriums.

                                       Sortierschlüssel Die Kombobox enthält alle in Ihrem Hause angelegten Sor-
                                       tierschlüssel. Klappen Sie die Box auf und wählen Sie den gewünschten Sor-
                                       tierschlüssel aus. Der Wert kommt aus den Stammdaten (Fertigung >
                                       Sortierschlüssel).
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                             I-93
                 Übersicht                                                                Softwarereferenz




                             Erläuterung der Felder im Bereich Abstellplatzgruppen

                             Name In diesem Feld wird Ihnen der Namen der Abstellplatzgruppe ange-
                             zeigt. Der Wert kommt aus den Stammdaten (Fertigung > Abstellplatzgrup-
                             pen).

                             Sortierschlüssel In diesem Feld wird Ihnen der Namen des Sortierschlüs-
                             sels angezeigt Der Wert kommt aus den Stammdaten (Fertigung > Sortier-
                             schlüssel).

                             Sortierschlüssel-Vorschau Das Feld zeigt Ihnen die Formel an, aus der
                             sich der Sortierschlüssel zusammensetzt. Der Wert kommt aus den Stamm-
                             daten (Fertigung > Sortierschlüssel).


                             Ergänzende Informationen
                              Tutorial, “Kriterien” auf Seite I-78
2.21 / 01-2017




                 I-94                                                 A+W Business Pro Production Manager
                 Softwarereferenz                                                                      Übersicht




                                       Logische Abstellplätze
                                       Stammdaten > Fertigung > Logische Abstellplätze




                                       Abb. I-64   Logische Abstellplätze


                                       In diesem Dialog definieren Sie die Ihrem Hause vorhandenen logischen Ab-
                                       stellplätze oder nehmen Änderungen an vorhandenen Abstellplätzen vor.

                                       Erläuterung der Felder im Bereich logische Abstellplätze

                                       Name In diesem Feld geben Sie den Namen des logischen Abstellplatzes
                                       ein.

                                       Typ Aus der Kombobox wählen Sie den entsprechenden Typ aus. Möglichen
                                       Werte sind:
                                       • ISO
                                       • VSG
                                       • Glas
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                       I-95
                 Übersicht                                                                       Softwarereferenz




                             Erläuterung der Felder im Bereich Gruppierung/Sortierung

                             Gruppierung Die Kombobox enthält alle in Ihren Hause angelegten Gruppie-
                             rungen. Wählen Sie die entsprechende Gruppierung aus. Der Wert kommt aus
                             den Stammdaten (Fertigung > Abstellplatzgruppen).

                             Sortierung in den Gruppen Die Kombobox enthält alle in Ihren Hause an-
                             gelegten Sortierungen. Wählen Sie die entsprechende Sortierung aus. Der
                             Wert kommt aus den Stammdaten (Fertigung > Sortierschlüssel).

                             Gruppen sortiert Über diese Checkbox steuern Sie, ob die Gruppen sortiert
                             werden. Die
                              Die Gruppen werden nicht sortiert.
                              Die Gruppen werden sortiert.


                             Ergänzende Informationen
                              Tutorial, “Logische Abstellplätze und Abstellplatztiefe” auf Seite I-71
2.21 / 01-2017




                 I-96                                                 A+W Business Pro Production Manager
                 Softwarereferenz                                                                         Übersicht




                                       Abstellplatzgruppen
                                       Stammdaten > Fertigung > Abstellplatzgruppen




                                       Abb. I-65     Abstellplatzgruppen


                                       In diesem Dialog können gewisse Abstellplätze zu einer Abstellplatzgruppe
                                       zusammengefasst werden. Dies bedeutet, dass auf die Abstellplätze, die zu
                                       derselben Gruppe gehören, bei der Produktion des Verbundproduktes im
                                       Wechsel zugegriffen wird, bevor der nächste Abstellplatz (oder der erste Ab-
                                       stellplatz der nächsten Gruppe) abgearbeitet wird.

                                       Erläuterung der Felder

                                       Name In diesem Feld geben Sie den Namen der Abstellplatzgruppe ein.

                                       Sortierschlüssel Die Kombobox enthält alle in Ihrem Hause angelegten Sor-
                                       tierschlüssel. Klappen Sie die Box auf und wählen Sie den gewünschten Sor-
                                       tierschlüssel aus. Der Wert kommt aus den Stammdaten (Fertigung >
                                       Sortierschlüssel).

                                       Sortierschlüssel-Vorschau Das Feld zeigt Ihnen die Formel an, aus der
                                       sich der Sortierschlüssel zusammensetzt. Der Wert kommt aus den Stamm-
                                       daten (Fertigung > Sortierschlüssel).
2.21 / 01-2017




                                       Ergänzende Informationen
                                        Tutorial, “Abstellplatzgruppen” auf Seite I-76



                 A+W Business Pro Production Manager                                                           I-97
                 Übersicht                                                                 Softwarereferenz




                             Sortierschlüssel
                             Stammdaten > Fertigung > Sortierschlüssel




                             Abb. I-66     Sortierschlüssel


                             In diesem Dialog können Sie Sortierschlüssel anlegen, um eine Menge von
                             Elementen zu sortieren. Dieser Schlüssel sortiert die Teile, die auf den zur
                             Gruppe gehörenden Abstellplätzen stehen.

                             Erläuterung der Felder im Bereich logische Abstellplätze

                             Name In diesem Feld geben Sie den Namen des Sortierschlüssels ein.

                             Formel Wählen Sie aus der Kombobox die gewünschte Formel aus. Hierzu
                             klicken Sie einmal in das Feld, um das Feld zu aktivieren. Ein zweiter Klick öff-
                             net die Kombobox. Die Werte kommen aus den Stammdaten (Fertigung > Kri-
                             terien)

                             Sortierung Wählen Sie aus der Kombobox die gewünschte Sortierung aus.
                             Hierzu klicken Sie einmal in das Feld, um das Feld zu aktivieren. Ein zweiter
                             Klick öffnet die Kombobox.Es stehen folgende Werte zur Verfügung:
                             • Aufsteigend: Die Sortierung erfolgt aufsteigend.
                             • Absteigend: Die Sortierung erfolgt absteigend.
2.21 / 01-2017




                             Ergänzende Informationen
                              Tutorial, “Sortierschlüssel” auf Seite I-81



                 I-98                                                 A+W Business Pro Production Manager
                 Softwarereferenz                                                                 Standardmodus




                                       Standardmodus
                                       In diesem Bereich sind die Daten, die Sie benötigen, wenn Sie den Produkti-
                                       onsmanager im Standardmodus betreiben möchten.
                                       Sie finden folgende Einträge:
                                       •   “Auftragsselektion” auf Seite I-105
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                         I-99
                 Standardmodus                                                              Softwarereferenz




                                 Assistenten
                                 Produktionsmanager > Standardmodus




                                 Abb. I-67   Standardmodus


                                 Im Standardmodus kann das Programm über eine vereinfachte Benutzerfüh-
                                 rung (Wizard) bedient werden.
                                 Mittels des Wizards ist es möglich, den Gesamtprozess (Laufbildung, Optimie-
                                 rung, etc.) mit wenigen Eingaben zu starten. Es werden am Ende des Prozes-
                                 ses die Optimierungsergebnisse angezeigt und Sie können entscheiden, ob
                                 Sie den Lauf und Optimierungsergebnisse so akzeptieren (speichern) oder mit
                                 anderen Einstellungen wiederholen, um ein besseres Ergebnis zu erzielen.
2.21 / 01-2017




                 I-100                                              A+W Business Pro Production Manager
                 Softwarereferenz                                                                     Standardmodus




                                       Erläuterung der Felder im Bereich Laufbildung

                                       Nummernverwalter Über die Kombobox haben Sie Zugriff auf die entspre-
                                       chenden Daten. Die Kombobox enthält alle Einträge, die Sie im Bereich des
                                       Nummernverwalters angelegt haben.

                                       Lauf Nachdem Sie im Nummernverwalter die entsprechende Auswahl ge-
                                       troffen haben, wird Ihnen in diesem Feld die Laufnummer angezeigt.

                                       Status In diesem Feld wird Ihnen der Laufstatus angezeigt.

                                       Bezeichnung In diesem Feld sehen Sie den Namen des Nummernverwal-
                                       ters, den Benutzer sowie das Datum der Laufbildung.

                                       Laufinhalt Dieses Feld wird erst nach der Laufbildung gefüllt. Sie sehen
                                       dann, wie viele ISO, VSG, ESG und bearbeitete Gläser der Lauf enthält.

                                       Erläuterung der Felder im Bereich Feinplanung und Optimierung

                                       Abstellplatzorganisation Die Kombobox enthält alle in Ihrem Hause ange-
                                       legten Abstellplatzorganisationen. Wählen Sie die gewünschte Organisations-
                                       form aus. Der Wert kommt aus den Stammdaten (Fertigung >
                                       Abstellplatzorganisation).

                                       Faktor für Abstellplatztiefe Bei diesem Wert handelt es sich um den Faktor
                                       für die im Lauf zu verwendende Gestelltiefe in Prozent. Der Wert für die Ab-
                                       stellplatztiefe kommt aus dem Stammdaten (Fertigung > Logische Abstellplät-
                                       ze). Über den Faktor können Sie den Wert temporär verändern. 100 %
                                       bedeutet, dass der in den Stammdaten hinterlegte Wert verwendet wird. 90 %
                                       bedeutet, dass die in den Stammdaten hinterlegte Tiefe nur zu 90 % genutzt
                                       wird, d. h. es gehen weniger Scheiben auf den Abstellplatz. Eine Korrektur des
                                       Wertes nach oben führt zu einer Mehrbelegung.

                                       Unbegrenzte Abstellplatztiefe Über diese Checkbox steuern Sie, ob der
                                       Abstellplatz eine unbegrenzte Tiefe hat.
                                        Der Abstellplatz hat die Tiefe, die in den Stammdaten hinterlegt wurde unter
                                       Berücksichtigung des Feldes Faktor für Abstellplatztiefe.
                                        Der Abstellplatz hat eine unbegrenzte Tiefe. Der in den Stammdaten hinter-
                                       legte Wert wird überschrieben.

                                       Anzahl Varianten Dieses Feld steht in Zusammenhang mit dem Feld Faktor
                                       für Abstellplatztiefe. Wenn man für die Abstellpatztiefe einen Bereich einstellt
                                       (z. B. 80-120 %), dann definiert dieses Feld, wie viele Varianten durch das Kli-
                                       cken auf die Symbol-Schaltfläche [Ausführen] entstehen. Beispiel:
                                       • Abstellplatztiefe: 80 - 120 %
                                       • Anzahl Varianten: 5
                                       • Feinplanung mit 80, 90, 100 110 und 120 % Gestelltiefe.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-101
                 Standardmodus                                                              Softwarereferenz




                                 Erläuterung der Felder im Bereich Speichern

                                 Ausgaben Über diesen Bereich werden alle Ausgaben, unabhängig davon,
                                 ob es sich um Ausgaben auf Papier oder in Dateiform handelt, eingestellt. Die
                                 Kombobox bietet Ihnen folgende Auswahlen:
                                 • Keine: Es finden keine Ausgaben statt.
                                 • Alle: Es werden folgende Medien ausgegeben:
                                    – Produktionslisten für den Lauf
                                    – Etiketten für den Lauf
                                    – Maschinenansteuerung für den Lauf
                                    – Standardlisten für die Optimierung (Rahmenbieger, ISO-Linie)
                                    – Schneidpläne für die Optimierung
                                    – Zuschnittetiketten für die Optimierung
                                    – Maschinenansteuerung für die Optimierung (Zuschnitttisch)
                                 • Auswahl: Hier können Sie manuell die unter Punkt Alle aufgelisteten Medi-
                                    en aktivieren.

                                 Erläuterung der Felder im Bereich Optimierungen

                                 Glasart In diesem Feld werden Ihnen die im Lauf enthaltenen Glasarten an-
                                 gezeigt. Die Ziffer davor zeigt Ihnen die Reihenfolge in der Optimierung.

                                 Schneidtisch Hier sehen Sie, auf welchem Tisch das Glas geschnitten wird.

                                 Läufe In diesem Feld wird Ihnen die Laufnummer angezeigt.

                                 Stückzahl In dieser Spalte sehen Sie, wie viele Stück optimiert werden.

                                 Fläche In dieser Spalte wird Ihnen die Gesamtfläche des zu optimierenden
                                 Artikels angezeigt.

                                 Ergebnis In diesem Feld wird Ihnen das Ergebnis der Optimierung für die je-
                                 weilige Glasart angezeigt. Zunächst sehen Sie das Ergebnis in %. Dahinter
                                 wird Ihnen in Klammern angezeigt, wie viele Muster und wie viele Lagerplatten
                                 die Optimierung benötigt sowie die verbleibende Restblattenlänge.

                                 Verschnitt Dieses Feld zeigt Ihnen den Gesamt-Verschnitt der Glasart der
                                 im A+W Business Pro eingestellten Währung.

                                    Inhalte im Bereich Optimierungen
                                    Die Tabelle enthält erst dann Daten, wenn der Lauf gebildet und die Fein-
                                    planung und die Optimierung durchlaufen wurden!

                                 Erläuterung der Felder im Bereich Gesamtergebnis

                                 Variante In diesem Feld werden Ihnen die verschiedenen Optimierungsvari-
                                 anten angezeigt.
2.21 / 01-2017




                 I-102                                               A+W Business Pro Production Manager
                 Softwarereferenz                                                                 Standardmodus




                                       Abstellplatzorganisation Hier wird Ihnen die Abstellplatzorganisation ange-
                                       zeigt, die Sie bei der Laufbildung gewählt haben.

                                       Anzahl Fächerwagen Hier wird Ihnen angezeigt, wie viele Fächerwagen nö-
                                       tig sind, um alle Gläser des Laufs abzustellen.

                                       Anzahl A-Böcke Hier wird Ihnen angezeigt, wie viele Fächerwagen nötig
                                       sind, um alle Gläser des Laufs abzustellen.

                                       Ergebnis Hier wird Ihnen das Gesamtergebnis der Variante in % angezeigt.

                                       Verschnitt Dieses Feld zeigt Ihnen den Gesamt-Verschnitt der Glasart der
                                       im A+W Business Pro eingestellten Währung.


                                       Ergänzende Informationen
                                        Tutorial, “Standardmodus” auf Seite I-14
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                        I-103
                 Expertenmodus                                                             Softwarereferenz




                                 Expertenmodus
                                 In diesem Bereich sind die Daten, die Sie benötigen, wenn Sie den Produkti-
                                 onsmanager im Expertenmodus betreiben möchten.
                                 Sie finden folgende Einträge:
                                 •   “Auftragsselektion” auf Seite I-105
                                 •   “Bruchpositionen” auf Seite I-113
                                 •   “Neuen Lauf erstellen” auf Seite I-117
                                 •   “Zuschnitt” auf Seite I-123
                                 •   “Optimierungsmanager” auf Seite I-130
                                 •   “Ausgabe” auf Seite I-138
2.21 / 01-2017




                 I-104                                               A+W Business Pro Production Manager
                 Softwarereferenz                                                                    Expertenmodus




                                       Auftragsselektion
                                       Produktionsmanager > Register Auftragsselektion




                                       Abb. I-68    Auftragsselektion im Expertenmodus


                                       In diesem Dialog erstellen Sie Ihre Produktionsläufe und Optimierungen. Dazu
                                       stehen Ihnen verschiedene Selektionskriterien zur Verfügung. Der Dialog ist
                                       in verschiedene Bereiche unterteilt. Im Bereich Selektionskriterien können Sie
                                       über den Nummernverwalter oder den Arbeitsgang die gewünschten Daten
                                       auswählen.

                                       Erläuterung der Felder im Bereich Selektionskriterien

                                       Nummernverwalter Nachdem Sie die Radiotaste aktiviert haben, können
                                       Sie aus der Kombobox auf die entsprechenden Daten zugreifen. Die Kombo-
                                       box enthält alle Einträge, die Sie im Bereich des Nummernverwalters angelegt
                                       haben.

                                       Arbeitsgang Nachdem Sie die Radiotaste aktiviert haben, können Sie aus
                                       der Kombobox auf die entsprechenden Daten zugreifen. Die Kombobox ent-
                                       hält alle Arbeitsgänge, die in den Aufträgen vorkommen, die an die A+W Busi-
                                       ness Pro Kapazitätsplanung übergeben wurden.

                                       Datum von bis Diese Felder stehen in Zusammenhang mit der Auswahl, die
                                       Sie im Feld Arbeitgang getroffen haben. Sie haben hier die Möglichkeit, den
                                       Arbeitsgang mit einem Datum einzugrenzen. Dieses Datum bezieht sich dann
2.21 / 01-2017




                                       auf das Produktionsdatum. Bsp.: Arbeitsgang Bohren, Produktionsdatum
                                       15.06.2013 bis 20.06.2013. Haben Sie als Arbeitsgang Versand gewählt, ist
                                       das eingegebene Datum das Versanddatum.



                 A+W Business Pro Production Manager                                                           I-105
                 Expertenmodus                                                              Softwarereferenz




                                 Erläuterung der Felder im Bereich Optimierungsartikel

                                 Produkt In dieser Spalte wird Ihnen die Produktnummer angezeigt. Die Wer-
                                 te kommen aus den Stammdaten (Produkte > Artikel).

                                 Produktbezeichnung 1 In dieser Spalte wird Ihnen die Produktbezeichnung
                                 angezeigt. Die Werte kommen aus den Stammdaten (Produkte > Artikel).

                                 Stückzahl In dieser Spalte sehen Sie, wie viele Stück optimiert werden.

                                 Fläche In dieser Spalte wird Ihnen die Gesamtfläche des zu optimierenden
                                 Artikels angezeigt.

                                 m²% In dieser Spalte wird Ihnen die Fläche des Artikels im Verhältnis zur Ge-
                                 samtfläche des Laufes angezeigt. Beispiel:




                                 Der Lauf hat eine zu optimierende Gesamtfläche von 67,86 m². Der Artikel 104
                                 A+W Float 4 mm hat eine Fläche von 16,35 m². Diese 16,35 m² sind 24,10 %
                                 von der Gesamtfläche.

                                 Erläuterung der Felder im Bereich Aufträge

                                 Auftragsnummer In dieser Spalte wird Ihnen die Auftragsnummer ange-
                                 zeigt.

                                 Kundennummer In dieser Spalte wird Ihnen die Kundennummer angezeigt.

                                 Status In dieser Spalte wird Ihnen der Auftragsstatus angezeigt.

                                 Erfassungsdatum In dieser Spalte sehen Sie, wann der Auftrag erfasst wur-
                                 de.

                                 AV-Bereich In dieser Spalte wird Ihnen der AV-Bereich angezeigt. Die Werte
                                 kommen aus den Stammdaten (AV-Bereiche).

                                 Fachberater In dieser Spalte wird Ihnen der Fachberater angezeigt. Die
                                 Werte kommen aus den Stammdaten der Mitarbeiter. Ist ein Mitarbeiter einem
                                 Kunden fest zugewiesen, handelt es sich dabei um einen Fachberater.

                                 Vertreter In dieser Spalte wird Ihnen der Vertreter angezeigt. Die Werte kom-
                                 men aus den Stammdaten.
2.21 / 01-2017




                 I-106                                               A+W Business Pro Production Manager
                 Softwarereferenz                                                                       Expertenmodus




                                       Bestelldatum Sollte es sich bei der Position um eine Bestellposition handeln,
                                       wird Ihnen hier das Bestelldatum angezeigt.

                                       Versanddatum In diesem Feld wird Ihnen das geplante Versanddatum ange-
                                       zeigt.

                                       Wunschtermin In diesem Feld sehen Sie den gewünschten Liefertermin.

                                       Liefertermin In diesem Feld wird Ihnen der Anliefertermin angezeigt.

                                       Tour In diesem Feld wird Ihnen die Tournummer angezeigt. Die Werte kom-
                                       men aus den Stammdaten (Versand > Touren).

                                       Priorität In diesem Feld wird Ihnen die Priorität des Auftrags angezeigt. Fol-
                                       gende Werte sind möglich:
                                       • Normal
                                       • Eilt
                                       • Zugabe
                                       • Abruf

                                       Kundendaten In den nächsten Feldern werden Ihnen Informationen zum
                                       Kunden angezeigt, wie Straße, PLZ, Ort, Telefon, etc.

                                       Erläuterung der Felder im Bereich Positionen

                                       Auftragsnummer In dieser Spalte wird Ihnen die Auftragsnummer ange-
                                       zeigt.

                                       Positionsnummer In dieser Spalte wird Ihnen die Positionssummer ange-
                                       zeigt.

                                       Stücklistenposition Diese Spalte zeigt Ihnen die Stücklistenebene. Bsp.:
                                       Stücklistenposition 0 ist das fertige Produkt. Stücklistenposition 1 ist der Arti-
                                       kel, der direkt darunter kommt. Gibt es darunter noch einen Artikel (Zwischen-
                                       produkt), hat der die Position 1.1. Gibt es neben diesem Artikel noch einen
                                       Artikel, hat der die Position 1.2.

                                       Erfassungsdatum In dieser Spalte sehen Sie, wann der Auftrag erfasst wur-
                                       de.

                                       Produkt In dieser Spalte wird Ihnen die Produktnummer angezeigt. Die Wer-
                                       te kommen aus den Stammdaten (Produkte > Artikel).

                                       Produktbezeichnung 1+2 In dieser Spalte wird Ihnen die Produktbezeich-
                                       nung angezeigt. Die Werte kommen aus den Stammdaten (Produkte > Arti-
                                       kel).

                                       Kurzinfo In dieser Spalte wird Ihnen eine kurze Information zum Artikel an-
                                       gezeigt. Die Werte kommen aus den Stammdaten (Artikel).
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-107
                 Expertenmodus                                                                Softwarereferenz




                                 Stückzahl In dieser Spalte sehen Sie, wie viele Stück bestellt wurden.

                                 Breite In dieser Spalte wird Ihnen die Breite des Stücklistenteils angezeigt.

                                 Höhe In dieser Spalte wird Ihnen die Höhe des Stücklistenteils angezeigt.

                                 Fläche In dieser Spalte wird Ihnen die Gesamtfläche des Artikels angezeigt.

                                 lfm In dieser Spalte sehen Sie die Laufmeter der Kanten.

                                 Modellnummer In dieser Spalte wird Ihnen die Modellnummer angezeigt.

                                 Produktart In dieser Spalte wird Ihnen die Produktart angezeigt. Der Wert
                                 kommt aus den Stammdaten (Produkte > Allgemein > Produktarten).

                                 Produktgruppe In dieser Spalte wird Ihnen die Produktgruppe angezeigt.
                                 Der Wert kommt aus den Stammdaten (Produkte > Allgemein > Produktgrup-
                                 pen).

                                 Beschaffungsart In dieser Spalte wird Ihnen die Beschaffungsart angezeigt.
                                 Folgende Werte sind möglich:
                                 • 0: Produktion
                                 • 1: Zuschnitt
                                 • 2: Lagerentnahme
                                 • 3: Bearbeitung
                                 • 7: Kundeneigenes Glas
                                 • 9: Bestellung
                                 • 102: Lagerzugang durch Produktion
                                 • 109: Bestellung (komplett)

                                 Gläser In dieser Spalte werden Ihnen die in der Position enthaltenen Gläser
                                 angezeigt.

                                 SZR In dieser Spalte wird Ihnen die Breite des Abstandhalters angezeigt.

                                 Gasfüllung In dieser Spalte wird Ihnen die Gasfüllung angezeigt. Der Wert
                                 kommt aus den Stammdaten (Produkte > Artikel > Artikel).

                                 Stufe In dieser Spalte wird Ihnen angezeigt, ob sich in der Stückliste unter-
                                 halb dieses Stücklistenteils ein gestuftes Stücklistenteil befindet. Der Wert
                                 kommt aus den Stammdaten. Mögliche Werte:
                                 • Ja: Es ist ein Stufenglas vorhanden
                                 • Nein: Es ist kein Stufenglas vorhanden

                                 Sprossen In dieser Spalte wird Ihnen angezeigt, ob sich in der Stückliste un-
                                 terhalb dieses Stücklistenteils Sprossen befinden. Mögliche Werte:
                                 • Ja: Es sind Sprossen vorhanden
2.21 / 01-2017




                                 • Nein: Es sind keine Sprossen vorhanden




                 I-108                                                A+W Business Pro Production Manager
                 Softwarereferenz                                                                   Expertenmodus




                                       Folien In dieser Spalte wird Ihnen die einzubauende Folie angezeigt. Der
                                       Wert kommt aus den Stammdaten (Produkte > Artikel > Artikel).

                                       Kopfteile In dieser Spalte wird Ihnen das Kopfteil angezeigt. Der Wert kommt
                                       aus den Stammdaten (Produkte > Artikel > Artikel).

                                       Kopfteiletyp In dieser Spalte wird Ihnen der Kopfteiletyp angezeigt. Der Wert
                                       kommt aus den Stammdaten (Produkte > Artikel > Artikel).


                                       Ergänzende Informationen
                                        Tutorial, “Auftragsselektion” auf Seite I-26
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                          I-109
                 Expertenmodus                                                                Softwarereferenz




                                 Ansicht speichern
                                 Produktionsmanager > Register Auftragsselektion > Aufträge gruppieren >
                                 Symbol-Schaltfläche [Speichern]




                                 Abb. I-69     Ansicht speichern


                                 In diesem Dialog haben Sie die Möglichkeit, eine Gruppierung, die Sortierung,
                                 die Reihenfolge und die Anzahl der Felder in der Liste für die Ansicht zu spei-
                                 chern. Das hat den Vorteil, dass Sie mehrere Gruppierungen mit unterschied-
                                 lichen Kriterien anlegen können.

                                 Name der Ansicht In diesem Feld geben Sie den Namen an, unter dem Sie
                                 die Gruppierung speichern möchten.


                                 Ergänzende Informationen
                                  Tutorial, “Daten gruppieren” auf Seite I-30
2.21 / 01-2017




                 I-110                                                   A+W Business Pro Production Manager
                 Softwarereferenz                                                                   Expertenmodus




                                       Produkt
                                       Produktionsmanager > Register Auftragsselektion > Register Produkt




                                       Abb. I-70   Register Produkt, am rechten Bildschirmrand


                                       Dieses Register liefert Ihnen detaillierte Informationen zu der ausgewählten
                                       Scheibe inklusive der Modellparameter und einer grafischen Vorschau.

                                       Erläuterung der Felder

                                       Stückzahl In diesem Feld wird Ihnen die Stückzahl angezeigt.

                                       Breite In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.

                                       Höhe In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.

                                       Modellnummer Wenn es sich bei der Scheibe um ein Modell handelt, wird Ih-
                                       nen in diesem Feld die Modellnummer angezeigt.
2.21 / 01-2017




                                       SN-Datei Wenn es sich bei der Scheibe um eine freie Form handelt, wird Ih-
                                       nen in diesem Feld die entsprechende SN-Datei angezeigt.



                 A+W Business Pro Production Manager                                                           I-111
                 Expertenmodus                                                              Softwarereferenz




                                 Modellparameter Wenn es sich bei der Scheibe um ein Modell handelt, wer-
                                 den Ihnen in diesem Bereich die entsprechenden Parameter (Höhe, Höhe 1,
                                 etc.) angezeigt.

                                 Vorschau Dieser Bereich liefert Ihnen eine Vorschau der Scheibe inklusive
                                 Vermaßung.


                                 Ergänzende Informationen
                                  Tutorial, “Produkt” auf Seite I-34
2.21 / 01-2017




                 I-112                                                  A+W Business Pro Production Manager
                 Softwarereferenz                                                                       Expertenmodus




                                       Bruchpositionen
                                       Produktionsmanager > Register Bruchpositionen




                                       Abb. I-71    Register Bruchpositionen


                                       Dieses Register erscheint, wenn Sie auf die Symbol-Schaltfläche Bruchschei-
                                       ben klicken. Hier können Sie Bruchscheiben erfassen oder Bruchläufe mit vor-
                                       handenen Bruchscheiben bilden.

                                       Erläuterung der Felder

                                       Auftragsnummer In dieser Spalte wird Ihnen die Auftragsnummer ange-
                                       zeigt.

                                       Positionsnummer In dieser Spalte wird Ihnen die Positionsnummer ange-
                                       zeigt.

                                       Unterpositionsnummer In dieser Spalte wird Ihnen die Unterpositionsnum-
                                       mer angezeigt.

                                       Stücklistenposition Diese Spalte zeigt Ihnen die Stücklistenebene. Bsp.:
                                       Stücklistenposition 0 ist das fertige Produkt. Stücklistenposition 1 ist der Arti-
                                       kel, der direkt darunter kommt. Gibt es darunter noch einen Artikel (Zwischen-
                                       produkt), hat der die Position 1.1. Gibt es neben diesem Artikel noch einen
                                       Artikel, hat der die Position 1.2.

                                       Lauf In dieser Spalte wird Ihnen die Laufnummer angezeigt.

                                       Produkt In dieser Spalte wird Ihnen die Produktnummer angezeigt. Die Wer-
                                       te kommen aus den Stammdaten (Produkte > Artikel).

                                       Produktbezeichnung 1+2 In dieser Spalte wird Ihnen die Produktbezeich-
                                       nung angezeigt. Die Werte kommen aus den Stammdaten (Produkte > Arti-
                                       kel).

                                       Kurzinfo In dieser Spalte wird Ihnen eine kurze Information zum Artikel an-
                                       gezeigt. Die Werte kommen aus den Stammdaten (Artikel).

                                       Stückzahl In dieser Spalte sehen Sie, wie viele Stück bestellt wurden.
2.21 / 01-2017




                                       Breite In dieser Spalte wird Ihnen die Breite des Stücklistenteils angezeigt.

                                       Höhe In dieser Spalte wird Ihnen die Höhe des Stücklistenteils angezeigt.


                 A+W Business Pro Production Manager                                                               I-113
                 Expertenmodus                                                                Softwarereferenz




                                 Fläche In dieser Spalte wird Ihnen die Gesamtfläche des Artikels angezeigt.

                                 lfm In dieser Spalte sehen Sie die Laufmeter der Kanten.

                                 Modellnummer In dieser Spalte wird Ihnen die Modellnummer angezeigt.

                                 Produktart In dieser Spalte wird Ihnen die Produktart angezeigt. Der Wert
                                 kommt aus den Stammdaten (Produkte > Allgemein > Produktarten).

                                 Produktgruppe In dieser Spalte wird Ihnen die Produktgruppe angezeigt.
                                 Der Wert kommt aus den Stammdaten (Produkte > Allgemein > Produktgrup-
                                 pen).

                                 Beschaffungsart In dieser Spalte wird Ihnen die Beschaffungsart angezeigt.
                                 Folgende Werte sind möglich:
                                 • 0: Produktion
                                 • 1: Zuschnitt
                                 • 2: Lagerentnahme
                                 • 3: Bearbeitung
                                 • 7: Kundeneigenes Glas
                                 • 9: Bestellung
                                 • 102: Lagerzugang durch Produktion
                                 • 109: Bestellung (komplett)

                                 Gläser In dieser Spalte werden Ihnen die in der Position enthaltenen Gläser
                                 angezeigt.

                                 SZR In dieser Spalte wird Ihnen die Breite des Abstandhalters angezeigt.

                                 Gasfüllung In dieser Spalte wird Ihnen die Gasfüllung angezeigt. Der Wert
                                 kommt aus den Stammdaten (Produkte > Artikel > Artikel).

                                 Stufe In dieser Spalte wird Ihnen angezeigt, ob sich in der Stückliste unter-
                                 halb dieses Stücklistenteils ein gestuftes Stücklistenteil befindet. Der Wert
                                 kommt aus den Stammdaten. Mögliche Werte:
                                 • Ja: Es ist ein Stufenglas vorhanden
                                 • Nein: Es ist kein Stufenglas vorhanden

                                 Sprossen In dieser Spalte wird Ihnen angezeigt, ob sich in der Stückliste un-
                                 terhalb dieses Stücklistenteils Sprossen befinden. Mögliche Werte:
                                 • Ja: Es sind Sprossen vorhanden
                                 • Nein: Es sind keine Sprossen vorhanden

                                 Folien In dieser Spalte wird Ihnen die einzubauende Folie angezeigt. Der
                                 Wert kommt aus den Stammdaten (Produkte > Artikel > Artikel).

                                 Kopfteile In dieser Spalte wird Ihnen das Kopfteil angezeigt. Der Wert kommt
2.21 / 01-2017




                                 aus den Stammdaten (Produkte > Artikel > Artikel).

                                 Kopfteiletyp In dieser Spalte wird Ihnen der Kopfteiletyp angezeigt. Der Wert
                                 kommt aus den Stammdaten (Produkte > Artikel > Artikel).


                 I-114                                                A+W Business Pro Production Manager
                 Softwarereferenz                                                                  Expertenmodus




                                       Bearbeitungen In dieser Spalte wird Ihnen - falls vorhanden - die Bearbei-
                                       tung für die jeweilige Position angezeigt.

                                       Produktionsdatum In dieser Spalte wird Ihnen das Produktionsdatum für die
                                       jeweilige Position angezeigt.

                                       Aggregat In dieser Spalte werden Ihnen das Aggregate für die jeweilige Po-
                                       sition angezeigt.


                                       Ergänzende Informationen
                                        Tutorial, “Produkt” auf Seite I-34
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                         I-115
                 Expertenmodus                                                             Softwarereferenz




                                 Bruch erfassen
                                 Produktionsmanager > Register Bruchpositionen > Kontextmenü > Bruch er-
                                 fassen




                                 Abb. I-72   Bruch erfassen


                                 In diesem Dialog haben Sie die Möglichkeit, Bruchscheiben manuell zu erfas-
                                 sen.

                                 Erläuterung der Felder

                                 Auftrag In diesem Feld geben Sie die Auftragsnummer ein, zu der die Bruch-
                                 scheiben gehören.

                                 Position In diesem Feld geben Sie die Positionsnummer ein.

                                 Stückzahl In diesem Feld geben Sie die Stückzahl ein, d. h. die Anzahl der
                                 Scheiben, die Sie nachproduzieren möchten.

                                 Grund In diesem Feld wählen Sie aus der Kombobox den Bruchgrund aus.

                                 Stelle In diesem Feld wählen Sie aus der Kombobox den Ort aus, an dem
                                 der Bruch passiert ist.

                                 Unterpositionsnummer In dieser Spalte wird Ihnen die Unterpositionsnum-
                                 mer angezeigt.
2.21 / 01-2017




                 I-116                                              A+W Business Pro Production Manager
                 Softwarereferenz                                                                   Expertenmodus




                                       Neuen Lauf erstellen
                                       Produktionsmanager > Register Auftragsselektion > Auftrag selektieren >
                                       Kontext-Menü öffnen > Neuen Lauf erstellen
                                       Produktionsmanager > Register Bruchscheiben > Auftrag selektieren > Kon-
                                       text-Menü öffnen > Neuen Bruchlauf erzeugen




                                       Abb. I-73    Neuen Lauf erstellen


                                       Mit hilfe dieses Dialogs erstellen Sie neue Läufe. Der Dialog wird über das
                                       Kontext-Menü, Eintrag Neuen Lauf erstellen, geöffnet.

                                       Erläuterung der Felder

                                       Laufnummer In diesem Feld wird Ihnen die Laufnummer angezeigt. Die
                                       Laufnummer wird vom System aufsteigend vergeben. Sie können die Lauf-
                                       nummer nicht ändern.

                                       Bezeichnung In diesem Feld geben Sie die Bezeichnung für den Lauf ein.
                                       Standardmäßig enthält das Feld das Selektionskriterium (z. B. Zuschneiden)
                                       und den Anwender. Die Daten kommen aus den Stammdaten. Sie können die
                                       Einträge überschreiben.

                                       Abstellplatzorganisation Die Kombobox enthält alle in Ihrem Hause ange-
                                       legten Abstellplatzorganisationen. Wählen Sie die gewünschte Organisations-
                                       form aus. Der Wert kommt aus den Stammdaten (Fertigung >
                                       Abstellplatzorganisation).

                                       Faktor für Abstellplatztiefe Bei diesem Wert handelt es sich um den Faktor
                                       für die im Lauf zu verwendende Gestelltiefe in Prozent. Der Wert für die
                                       Abstellplatztiefe kommt aus dem Stammdaten (Fertigung > Logische Abstell-
                                       plätze). Über den Faktor können Sie den Wert temporär verändern. 100 % be-
                                       deutet, dass der in den Stammdaten hinterlegte Wert verwendet wird. 90 %
                                       bedeutet, dass die in den Stammdaten hinterlegte Tiefe nur zu 90 % genutzt
                                       wird, d. h. es gehen weniger Scheiben auf den Abstellplatz. Eine Korrektur des
2.21 / 01-2017




                                       Wertes nach oben führt zu einer Mehrbelegung.




                 A+W Business Pro Production Manager                                                           I-117
                 Expertenmodus                                                               Softwarereferenz




                                 Unbegrenzte Abstellplatztiefe Über diese Checkbox steuern Sie, ob der
                                 Abstellplatz eine unbegrenzte Tiefe hat.
                                  Der Abstellplatz hat die Tiefe, die in den Stammdaten hinterlegt wurde unter
                                 Berücksichtigung des Feldes Faktor für Abstellplatztiefe.
                                  Der Abstellplatz hat eine unbegrenzte Tiefe. Der in den Stammdaten hinter-
                                 legte Wert wird überschrieben.

                                 Erläuterung der Checkboxen

                                 Feinplanung Wenn Sie diese Checkbox aktivieren, erfolgt nach der Laufbil-
                                 dung automatisch die Feinplanung.

                                 Optimierungsmanager Diese Checkbox ist nur in Verbindung mit der
                                 Checkbox Feinplanung aktiv. Wenn Sie die Checkbox aktivieren, wird nach
                                 der Laufbildung und der Feinplanung in das Register Optimierungsmanager
                                 gewechselt. Es wird aber keine Optimierung erzeugt!

                                 Kompletter Handzuschnitt Diese Checkbox ist nur in Verbindung mit der
                                 Checkbox Feinplanung aktiv. Wenn Sie die Checkbox aktivieren, werden nach
                                 der Laufbildung und der Feinplanung alle Scheiben auf Handzuschnitt ge-
                                 setzt.

                                 Ausgabe Diese Checkbox ist aktiv, wenn die Checkboxen Feinplanung und
                                 Kompletter Handzuschnitt aktiviert wurden. Dann wird nach der Laufbildung,
                                 der Feinplanung und dem Handzuschnitt in das Register Ausgabe gewech-
                                 selt.


                                 Ergänzende Informationen
                                  Tutorial, “Läufe verwalten” auf Seite I-39
2.21 / 01-2017




                 I-118                                                   A+W Business Pro Production Manager
                 Softwarereferenz                                                                          Expertenmodus




                                             Laufübersicht
                                             Produktionsmanager > Register Laufübersicht




                 Abb. I-74   Laufübersicht


                                             In diesem Dialog werden Ihnen die gebildeten Läufe angezeigt. Der Dialog ist
                                             in zwei Bereiche eingeteilt. Im oberen Bereich befinden sich die Selektionskri-
                                             terien. Im unteren Bereich werden Ihnen die existierenden Läufe angezeigt.

                                             Erläuterung der Felder im Bereich Selektionskriterien

                                             Laufnummer Über die Felder von bis können Sie sich gezielt Läufe nach de-
                                             ren Nummer anzeigen lassen. Die Felder dienen auch dazu, die angezeigten
                                             Läufe zu limitieren, um den Überblick zu behalten.

                                             Erstelldatum Über dieses Feld können Sie sich die Läufe nach dem Datum
                                             anzeigen lassen, an dem sie erstellt wurden.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                  I-119
                 Expertenmodus                                                                  Softwarereferenz




                                 Status Mit hilfe dieser Komboboxen können Sie sich die Läufe nach deren
                                 Status anzeigen lassen. Folgende Stati sind möglich:
                                 •   Grobgeplant: Für diese Läufe ist noch keine Abstellplatzvergabe erfolgt.
                                 •   Feingeplant: Für diese Läufe erfolgte eine Abstellplatzvergabe.
                                 •   Teiloptimiert: Einige Glasarten dieser Läufe wurden bereits optimiert.
                                 •   Optimiert: Alle Glasarten dieser Läufe wurden bereits optimiert.
                                 •   Freigegeben: Für die Optimierungen des Laufs wurden bereits Produkti-
                                     onspapiere gedruckt und Maschinencodes erzeugt.
                                 •   Teilfertig: Einige Teile des Laufs wurden bereits produziert, aber noch nicht
                                     alle.
                                 •   Fertig: Alle Teile des Laufs wurden produziert.

                                 Bezeichnung Über dieses Feld können Sie sich die Läufe nach deren Be-
                                 zeichnung anzeigen lassen. Diese Bezeichnung haben Sie beim Erstellen ei-
                                 nes Laufes im Dialog Neuen Lauf erstellen vergeben.

                                 Erläuterung der Felder im Bereich Läufe

                                 Laufnummer In dieser Spalte wird Ihnen die Laufnummer angezeigt.

                                 Erstelldatum In diesem Feld wird Ihnen angezeigt, wann der Lauf erstellt
                                 wurde.

                                 Status In diesem Feld wird Ihnen angezeigt, in welchem Status sich der Lauf
                                 befindet.

                                 Bezeichnung In diesem Feld wird Ihnen die Bezeichnung angezeigt, die Sie
                                 bei der Laufbildung vergeben haben.

                                 Abstellplatzorganisation Hier wird Ihnen die Abstellplatzorganisation ange-
                                 zeigt, die Sie bei der Laufbildung gewählt haben.

                                 ISO In diesem Feld sehen Sie die im Lauf enthaltene Menge an ISO.

                                 VSG In diesem Feld sehen Sie die im Lauf enthaltene Menge an VSG.

                                 ESG In diesem Feld sehen Sie die im Lauf enthaltene Menge an ESG.

                                 Glas (Einzel und Bearbeitet) Hier sehen Sie die im Lauf enthaltenen Einzel-
                                 gläser und die bearbeiteten Gläser.

                                 Faktor für Abstellplatztiefe Hier wird Ihnen der Faktor angezeigt, den Sie
                                 bei der Laufbildung angegeben haben.


                                 Ergänzende Informationen
                                  Tutorial, “Läufe verwalten” auf Seite I-39
2.21 / 01-2017




                 I-120                                                   A+W Business Pro Production Manager
                 Softwarereferenz                                                                       Expertenmodus




                                           Detailansicht
                                           Produktionsmanager > Register Laufübersicht > Lauf selektieren > Kontext-
                                           Menü öffnen > Detailansicht




                 Abb. I-75   Detailansicht für einen Lauf


                                           Mit diesem Dialog haben Sie die Möglichkeit, sich einen selektierten Lauf im
                                           Detail anzusehen. Der Dialog wird über das Kontext-Menü, Eintrag Detailan-
                                           sicht, geöffnet und besteht aus mehreren Bereichen.

                                           Erläuterung der Felder im Bereich Feinplanung

                                           Bezeichnung Hier wird Ihnen die Laufbezeichnung angezeigt. Diese Be-
                                           zeichnung haben Sie beim Erstellen des Laufes im Dialog Neuen Lauf erstel-
                                           len vergeben. Sie können den Eintrag an dieser Stelle noch ändern.

                                           Abstellplatzorganisation Hier wird Ihnen die Abstellplatzorganisation ange-
                                           zeigt. Es handelt sich um die Abstellplatzorganisation, die Sie beim Erstellen
                                           des Laufes im Dialog Neuen Lauf erstellen ausgewählt haben. Die Abstell-
                                           platzorganisation kann nur geändert werden, wenn sich der Lauf im Status
                                           Grobgeplant befindet.
2.21 / 01-2017




                                           Erstelldatum Hier wird Ihnen das Datum angezeigt, an dem der Lauf erstellt
                                           wurde.




                 A+W Business Pro Production Manager                                                               I-121
                 Expertenmodus                                                                      Softwarereferenz




                                 Status Hier wird Ihnen der Laufstatus angezeigt.

                                 Faktor für Abstellplatztiefe Hier wird Ihnen der Faktor für die im Lauf zu ver-
                                 wendende Gestelltiefe in Prozent angezeigt. Der Wert kann nur geändert wer-
                                 den, wenn sich der Lauf im Status Grobgeplant oder Feingeplant befindet.

                                 Unbegrenzte Abstellplatztiefe Über diese Checkbox steuern Sie, ob der
                                 Abstellplatz eine unbegrenzte Tiefe hat. Der Wert kann nur geändert werden,
                                 wenn sich der Lauf im Status Grobgeplant oder Feingeplant befindet.
                                  Der Abstellplatz hat die Tiefe, die in den Stammdaten hinterlegt wurde unter
                                 Berücksichtigung des Feldes Faktor für Abstellplatztiefe.
                                  Der Abstellplatz hat eine unbegrenzte Tiefe. Der in den Stammdaten hinter-
                                 legte Wert wird überschrieben.

                                 Erläuterung der Felder im Bereich Optimierungsartikel

                                 Produkt In dieser Spalte wird Ihnen die Produktnummer angezeigt. Die Wer-
                                 te kommen aus den Stammdaten (Produkte > Artikel).

                                 Produktbezeichnung 1 In dieser Spalte wird Ihnen die Produktbezeichnung
                                 angezeigt. Die Werte kommen aus den Stammdaten (Produkte > Artikel).

                                 Stückzahl In dieser Spalte sehen Sie, wie viele Stück optimiert werden.

                                 Fläche In dieser Spalte wird Ihnen die Gesamtfläche des zu optimierenden
                                 Artikels angezeigt.

                                 Fläche % In dieser Spalte wird Ihnen die Fläche der Artikels im Verhältnis zur
                                 Gesamtfläche des Laufes angezeigt. Beispiel:




                                 Der Lauf hat eine zu optimierende Gesamtfläche von 67,86 m². Der Artikel 104
                                 A+W Float 4 mm hat eine Fläche von 16,35 m². Diese 16,35 m² sind 24,10 %
                                 von der Gesamtfläche.

                                    Felder im Bereich Aufträge und Positionen
                                    Die Felder im Bereich Aufträge und Positionen sind identisch mit den
                                    gleichnamigen Feldern im Register Auftragsselektion und werden an die-
                                    ser Stelle nicht noch einmal erläutert.


                                 Ergänzende Informationen
2.21 / 01-2017




                                  Tutorial, “Detailansicht für Läufe” auf Seite I-46
                                  “Erläuterung der Felder im Bereich Aufträge” auf Seite I-106
                                  “Erläuterung der Felder im Bereich Positionen” auf Seite I-107



                 I-122                                                  A+W Business Pro Production Manager
                 Softwarereferenz                                                                   Expertenmodus




                                       Zuschnitt
                                       Produktionsmanager > Register Detailanzeige > Register Zuschnitt




                                       Abb. I-76   Register Zuschnitt, am rechten Bildschirmrand


                                       Dieses Register liefert Ihnen detaillierte Informationen zu der ausgewählten
                                       Scheibe inklusive der Modellparameter und einer grafischen Vorschau.

                                       Erläuterung der Felder

                                       Stückzahl In diesem Feld wird Ihnen die Stückzahl angezeigt.

                                       Breite In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.

                                       Höhe In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.

                                       Modellnummer Wenn es sich bei der Scheibe um ein Modell handelt, wird Ih-
                                       nen in diesem Feld die Modellnummer angezeigt.
2.21 / 01-2017




                                       SN-Datei Wenn es sich bei der Scheibe um eine freie Form handelt, wird Ih-
                                       nen in diesem Feld die entsprechende SN-Datei angezeigt.



                 A+W Business Pro Production Manager                                                          I-123
                 Expertenmodus                                                                Softwarereferenz




                                 Modellparameter Wenn es sich bei der Scheibe um ein Modell handelt, wer-
                                 den Ihnen in diesem Bereich die entsprechenden Parameter (Höhe, Höhe 1,
                                 etc.) angezeigt.

                                 Modellbruchränder Wenn es sich bei der Scheibe um ein Modell handelt,
                                 werden Ihnen in diesem Bereich die entsprechenden Parameter (Höhe, Höhe
                                 1, etc.) angezeigt.

                                 Vorschau Dieser Bereich liefert Ihnen eine Vorschau der Scheibe inklusive
                                 Vermaßung.

                                 Bearbeiten Wenn Sie auf diese Schaltfläche klicken, öffnet sich der Dialog
                                 Zuschnitt bearbeiten.


                                 Ergänzende Informationen
                                  Softwarereferenz, “Zuschnitt bearbeiten” auf Seite I-125
                                  Tutorial, “Register Zuschnitt” auf Seite I-48
2.21 / 01-2017




                 I-124                                                  A+W Business Pro Production Manager
                 Softwarereferenz                                                                    Expertenmodus




                                       Zuschnitt bearbeiten
                                       Produktionsmanager > Register Detailanzeige > Register Zuschnitt > Schalt-
                                       fläche [Bearbeiten]




                                       Abb. I-77    Zuschnitt bearbeiten


                                       Dieser Dialog liefert Ihnen detaillierte Zuschnitt-Informationen zu der ausge-
                                       wählten Scheibe inklusive der Modellparameter und einer grafischen Vor-
                                       schau.

                                       Erläuterung der Felder

                                       Stückzahl In diesem Feld wird Ihnen die Stückzahl angezeigt.

                                       Breite In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.

                                       Höhe In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.

                                       SN-Datei Wenn es sich bei der Scheibe um eine freie Form handelt, wird Ih-
                                       nen in diesem Feld die entsprechende SN-Datei angezeigt.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                            I-125
                 Expertenmodus                                                                Softwarereferenz




                                 Modellparameter Wenn es sich bei der Scheibe um ein Modell handelt, wer-
                                 den Ihnen in diesem Bereich die entsprechenden Parameter (Höhe, Höhe 1,
                                 etc.) angezeigt.

                                 Modellbruchränder Wenn es sich bei der Scheibe um ein Modell handelt,
                                 werden Ihnen in diesem Bereich die entsprechenden Modellbruchränder für
                                 links, rechts, oben und unten angezeigt.

                                 Vorschau Dieser Bereich liefert Ihnen eine Vorschau der Scheibe inklusive
                                 Vermaßung. Die gestrichelte Linie kennzeichnet die Modellbruchränder.


                                 Ergänzende Informationen
                                  Tutorial, “Register Zuschnitt” auf Seite I-48
2.21 / 01-2017




                 I-126                                                    A+W Business Pro Production Manager
                 Softwarereferenz                                                                  Expertenmodus




                                       Laufstatus setzen
                                       Produktionsmanager > Register Laufübersicht > Auftrag selektieren > Kon-
                                       text-Menü öffnen > Laufstatus setzen




                                       Abb. I-78   Laufstatus setzen


                                       Mit Hilfe dieses Dialogs können Sie den Status eines Laufes ändern.

                                       Erläuterung der Felder

                                       Neuer Laufstatus Über die Kombobox können Sie den Laufstatus auf Fertig
                                       setzen.

                                          Laufstatus manuell ändern
                                          Den Laufstatus können Sie manuell ändern für Läufe, die z. B. nur aus be-
                                          stellten Gläsern bestehen.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                         I-127
                 Expertenmodus                                                                        Softwarereferenz




                                         Aggregatumlastung
                                         Produktionsmanager > Register Laufübersicht > Lauf selektieren > Kontext-
                                         Menü öffnen > Aggregatumlastung




                 Abb. I-79   Aggregatumlastung


                                         Mit diesem Dialog haben Sie die Möglichkeit, Produkte auf andere Aggregate
                                         umzulasten. Der Dialog ist in zwei Bereiche unterteilt:
                                         •   Aktuelle Aggregatzuordnung
                                         •   Alternative Aggregate
                                         Im Bereich Aktuelle Aggregatzuordnung sehen Sie eine Baumansicht mit den
                                         folgenden Ebenen:
                                         •   Aggregat
                                         •   Arbeitsgang
                                         •   Produkt
                                         Im Bereich Alternative Aggregate werden Ihnen die entsprechenden Alterna-
                                         tiven angeboten. Dieser Bereich dient u. a. für Mitteilungstexte. Folgende Tex-
                                         te sind möglich:
                                         •   Bitte wählen sie ein Produkt zur Aggregatumlastung aus
                                             In diesem Fall haben Sie die falsche Ebene ausgewählt.
                                         •   Eine Aggregatumlastung ist aufgrund des Laufstatus nicht möglich
                                             In diesem Fall befindet sich der Lauf bereits in einem Status, in dem eine
                                             Umlastung nicht mehr möglich ist.
                                         •   Es sind keine alternativen Aggregate zur Umlastung verfügbar
                                             Das Produkt kann nicht umgelastet werden, da es keine alternativen Ag-
                                             gregate gibt.
2.21 / 01-2017




                 I-128                                                        A+W Business Pro Production Manager
                 Softwarereferenz                                                                Expertenmodus




                                       Erläuterung der Schaltflächen

                                       Umlasten Wenn Sie die Schaltfläche betätigen, wird das Produkt auf das
                                       ausgewählte Aggregat umgelastet.

                                       Schließen Wenn Sie die Schaltfläche betätigen, wird der Dialog geschlos-
                                       sen.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                       I-129
                 Expertenmodus                                                                     Softwarereferenz




                                         Optimierungsmanager
                                         Produktionsmanager > Register Optimierungsmanager




                 Abb. I-80   Optimierungsmanager


                                         In diesem Dialog werden Ihnen die Läufe angezeigt, die an den Optimierungs-
                                         manager übergeben wurden. Der Dialog ist in vier Bereiche eingeteilt. Oben
                                         links werden Ihnen die Läufe angezeigt. Rechts daneben stehen alle Glasar-
                                         ten aus allen Läufen, die an den Optimierungsmanager übergeben wurden.
                                         Wird eine Glasart aufgeklappt, so sieht man, in welchen Läufen die Glasart
                                         vorkommt. Im unteren Bereich werden Ihnen die jeweiligen Optimierungen
                                         und das Gesamtergebnis angezeigt.

                                         Erläuterung der Felder im Bereich Läufe

                                         Laufnummer In dieser Spalte wird Ihnen die Laufnummer angezeigt, die Sie
                                         im Register Laufübersicht selektiert haben.

                                         Erstelldatum In diesem Feld wird Ihnen angezeigt, wann der Lauf erstellt
                                         wurde.
2.21 / 01-2017




                                         Status Hier wird Ihnen der Laufstatus angezeigt.

                                         Bezeichnung> In diesem Feld wird Ihnen die Laufbezeichnung angezeigt.


                 I-130                                                      A+W Business Pro Production Manager
                 Softwarereferenz                                                                      Expertenmodus




                                       Abstellplatzorganisation Hier wird Ihnen die Abstellplatzorganisation ange-
                                       zeigt, die Sie bei der Laufbildung gewählt haben.

                                       ISO In diesem Feld sehen Sie die im Lauf enthaltene Menge an ISO.

                                       VSG In diesem Feld sehen Sie die im Lauf enthaltene Menge an VSG.

                                       ESG In diesem Feld sehen Sie die im Lauf enthaltene Menge an ESG.

                                       Glas (Einzel und Bearbeitet) Hier sehen Sie die im Lauf enthaltenen Einzel-
                                       gläser und die bearbeiteten Gläser.

                                       Faktor für Abstellplatztiefe Hier wird Ihnen der Faktor angezeigt, den Sie
                                       bei der Laufbildung angegeben haben.

                                       Erläuterung der Felder im Bereich Glasarten
                                       Hier werden Ihnen alle Glasarten angezeigt, die in den Läufen enthalten sind.
                                       Wenn Sie den Eintrag der Glasart aufklappen, erhalten Sie Informationen zu
                                       der Stückzahl, der Fläche und dem Lauf.

                                          Felder im Bereich Optimierungen und Gesamtergebnis
                                          Die Felder im Bereich Optimierungen und Gesamtergebnis sind identisch
                                          mit den gleichnamigen Feldern im Standardmodus und werden an dieser
                                          Stelle nicht noch einmal erläutert.


                                       Ergänzende Informationen
                                        Tutorial, “Optimierungsmanager” auf Seite I-52
                                        “Erläuterung der Felder im Bereich Optimierungen” auf Seite I-102
                                        “Erläuterung der Felder im Bereich Gesamtergebnis” auf Seite I-102
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                           I-131
                 Expertenmodus                                                                      Softwarereferenz




                                         Optimierung abbrechen
                                         Produktionsmanager > Register Optimierungsmanager > Ausführen > Opti-
                                         mierungen > [Abbrechen]




                 Abb. I-81   Optimierungen


                                         In diesem Dialog werden Ihnen die Optimierungen zu den entsprechenden
                                         Läufe angezeigt. Sie können die Optimierung abbrechen, indem Sie auf die
                                         Schaltfläche [Abbrechen] klicken.


                                         Ergänzende Informationen
                                          Tutorial, “Optimierung abbrechen” auf Seite I-58
2.21 / 01-2017




                 I-132                                                          A+W Business Pro Production Manager
                 Softwarereferenz                                                                     Expertenmodus




                                         Temporäre Optimierung
                                         Produktionsmanager > Register Optimierungsmanager > Detailansicht




                 Abb. I-82   Temporäre Optimierung


                                         Dieser Dialog zeigt Ihnen die Detailansicht für eine Optimierungsvariante. Er
                                         wird aus dem Optimierungsmanager über das Kontext-Menü, Eintrag Detail-
                                         ansicht, geöffnet und besteht aus mehreren Bereichen.

                                         Erläuterung der Felder im Bereich Gestell

                                         Laufnummer Hier wird Ihnen die Laufnummer angezeigt, die Sie im Register
                                         Optimierungsmanager ausgewählt haben.

                                         Gestell Hier wird Ihnen die Gestellnummer angezeigt, auf die das Glas abge-
                                         stellt wird.

                                         Gestell-Typ Hier wird Ihnen der Gestell-Typ angezeigt, auf den das Glas ab-
                                         gestellt wird. Mögliche Werte sind:
                                         • A-Bock
2.21 / 01-2017




                                         • Fächerwagen




                 A+W Business Pro Production Manager                                                            I-133
                 Expertenmodus                                                               Softwarereferenz




                                 Log. Abstellplatz Hier wird Ihnen der logische Abstellplatz angezeigt.

                                 Menge Hier wird Ihnen die Anzahl der Scheiben auf dem Abstellplatz ange-
                                 zeigt.

                                 Erläuterung der Felder im Bereich Läufe

                                 Laufnummer Hier werden Ihnen die Laufnummern der Läufe angezeigt, die
                                 an der Optimierung beteiligt sind.

                                 Erstelldatum In diesem Feld wird Ihnen angezeigt, wann der Lauf erstellt
                                 wurde.

                                 Bezeichnung In diesem Feld wird Ihnen die Laufbezeichnung angezeigt.

                                 Erläuterung der Felder im Bereich Lagermaße

                                 Menge In dieser Spalte sehen Sie die Anzahl Lagermaße dieser Größe, die
                                 in der Optimierung verwendet wurde.

                                 Breite In dieser Spalte wird Ihnen die Breite des Lagermaßes angezeigt.

                                 Höhe In dieser Spalte wird Ihnen die Höhe des Lagermaßes angezeigt.

                                 Fläche In dieser Spalte wird Ihnen die Fläche des Lagermaßes in Quadrat-
                                 metern angezeigt.

                                 Priorität In dieser Spalte wird Ihnen angezeigt, welche Priorität das Lager-
                                 maß hat.

                                 Erläuterung der Felder im Bereich Muster

                                 Muster In dieser Spalte werden Ihnen die einzelnen Muster aufgelistet.

                                 Optimierungsgruppe In dieser Spalte werden Ihnen die Optimierungsgrup-
                                 pen angezeigt.

                                 Menge In dieser Spalte sehen Sie, wie oft dieses Muster zugeschnitten wer-
                                 den soll.

                                 Breite In dieser Spalte wird Ihnen die Breite des Musters angezeigt.

                                 Höhe In dieser Spalte wird Ihnen die Höhe des Musters angezeigt.


                                 Ergänzende Informationen
                                  Tutorial, “Temporäre Optimierung” auf Seite I-55
2.21 / 01-2017




                 I-134                                                  A+W Business Pro Production Manager
                 Softwarereferenz                                                                        Expertenmodus




                                          Optimierungsübersicht
                                          Produktionsmanager > Register Optimierungsübersicht




                 Abb. I-83   Optimierungsübersicht


                                          In diesem Dialog werden die durchgeführten Optimierungen der einzelnen
                                          Glasarten angezeigt. Um die Inhalte überschaubar zu halten, stehen Ihnen
                                          unterschiedlichen Selektionskriterien zur Verfügung. Sie können sich an die-
                                          ser Stelle für eine markierte Glasart die Details anzeigen (Detailansicht) las-
                                          sen und die Ausgabe (Maschinenausgaben, Reports) starten. Darüber hinaus
                                          können Sie die Optimierung verwerfen, Lagerplatten abbuchen und Muster
                                          neu bearbeiten.

                                          Erläuterung der Felder im Bereich Selektionskriterien

                                          Optimierung Über die Felder von bis können Sie sich gezielt Optimierungen
                                          nach deren Nummer anzeigen lassen. Die Felder dienen auch dazu, die an-
                                          gezeigten Optimierungen zu limitieren, um den Überblick zu behalten.

                                          Erstelldatum Über dieses Feld können Sie sich die Optimierungen nach
                                          dem Datum anzeigen lassen, an dem sie erstellt wurden. Die Felder dienen
2.21 / 01-2017




                                          auch dazu, die angezeigten Optimierungen zu limitieren, um den Überblick zu
                                          behalten.



                 A+W Business Pro Production Manager                                                               I-135
                 Expertenmodus                                                               Softwarereferenz




                                 Laufnummer Über die Felder von bis können Sie gezielt nach Optimierun-
                                 gen suchen, die zu einem oder mehreren Läufen gehören.

                                 Erläuterung der Felder im Bereich Optimierung

                                 Optimierung In dieser Spalte wird Ihnen die Optimierungsnummer ange-
                                 zeigt.

                                 Optimierungsmodus In diesem Feld wird Ihnen angezeigt, welcher Opti-
                                 mierungsmodus verwendet wurde. Mögliche Werte sind:
                                 • XOPT
                                 • XOPTS

                                 Erstelldatum In diesem Feld wird Ihnen angezeigt, wann die Optimierung
                                 erstellt wurde.

                                 Glasart In diesem Feld wird Ihnen angezeigt, welche Glasart optimiert wur-
                                 de.

                                 Schneidtisch Hier sehen Sie, auf welchem Tisch das Glas geschnitten wird.

                                 Läufe In diesem Feld werden Ihnen die Laufnummern angezeigt, die Schei-
                                 ben in der Optimierung haben.

                                 Status In diesem Feld wird Ihnen der Status angezeigt.

                                 Stückzahl In diesem Feld wird Ihnen die optimierte Stückzahl angezeigt.

                                 Fläche In dieser Spalte wird Ihnen die Gesamtfläche des zu optimierenden
                                 Artikels angezeigt.

                                 Ergebnis In diesem Feld wird Ihnen das Ergebnis der Optimierung für die je-
                                 weilige Glasart angezeigt.


                                 Ergänzende Informationen
                                  Tutorial, “Optimierungsübersicht” auf Seite I-59
2.21 / 01-2017




                 I-136                                                   A+W Business Pro Production Manager
                 Softwarereferenz                                                                      Expertenmodus




                                          Detailansicht Optimierung
                                          Produktionsmanager > Register Optimierungsübersicht > Detailansicht




                 Abb. I-84   Detailansicht Optimierung


                                          Dieser Dialog zeigt Ihnen die Detailansicht für eine Optimierung. Er wird aus
                                          der Optimierungsübersicht über das Kontext-Menü, Eintrag Detailansicht, ge-
                                          öffnet und besteht aus mehreren Bereichen.
                                          Die Inhalte dieses Dialogs sind identisch mit den Inhalten des Dialogs Tempo-
                                          räre Optimierung und werden an dieser Stelle nicht noch einmal beschrieben.
                                           “Temporäre Optimierung” auf Seite I-133


                                          Ergänzende Informationen
                                           Tutorial, “Temporäre Optimierung” auf Seite I-55
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                             I-137
                 Expertenmodus                                                             Softwarereferenz




                                 Ausgabe
                                 Produktionsmanager > Register Ausgabe




                                 Abb. I-85   Ausgabe


                                 Über dieses Register werden alle Ausgaben, unabhängig davon, ob es sich
                                 um Ausgaben auf Papier oder in Dateiform handelt, gestartet.
                                 Der Dialog kann direkt (Register Ausgabe), über das Register Laufübersicht
                                 und über das Register Optimierungsübersicht aufgerufen werden.

                                 Erläuterung der Felder im Bereich Läufe (aus Laufübersicht)

                                 Laufnummer In dieser Spalte wird Ihnen die Laufnummer angezeigt, die Sie
                                 im Register Laufübersicht selektiert haben.

                                 Erstelldatum In diesem Feld wird Ihnen angezeigt, wann der Lauf erstellt
                                 wurde.

                                 Benutzer In diesem Feld wird Ihnen angezeigt, wer den Lauf erstellt hat.

                                 Bezeichnung In diesem Feld wird Ihnen die Laufbezeichnung angezeigt.

                                 Abstellplatzorganisation Hier wird Ihnen die Abstellplatzorganisation ange-
                                 zeigt, die Sie bei der Laufbildung gewählt haben.
2.21 / 01-2017




                 I-138                                              A+W Business Pro Production Manager
                 Softwarereferenz                                                                         Expertenmodus




                                       Status Hier wird Ihnen der Laufstatus angezeigt.

                                       ISO In diesem Feld sehen Sie die im Lauf enthaltene Menge an ISO.

                                       VSG In diesem Feld sehen Sie die im Lauf enthaltene Menge an VSG.

                                       ESG In diesem Feld sehen Sie die im Lauf enthaltene Menge an ESG.

                                       Glas Hier sehen Sie die im Lauf enthaltenen Einzelgläser und die bearbeite-
                                       ten Gläser.

                                       Meldung Hier wird Ihnen ein Meldungstext angezeigt. Folgende Texte mög-
                                       lich:

                                       .
                                       Symbol     Erläuterung

                                                  Die Ausgabe ist nicht korrekt, z. B. weil der Lauf nicht komplett
                                                  optimiert wurde.

                                                  Die Ausgabe ist korrekt.



                                       Erläuterung der Felder im Bereich Optimierung (aus Optimierun-
                                       gen)

                                       Optimierung In dieser Spalte wird Ihnen die Optimierungsnummer ange-
                                       zeigt.

                                       Erstelldatum In diesem Feld wird Ihnen angezeigt, wann die Optimierung
                                       erstellt wurde.

                                       Glasart In diesem Feld wird Ihnen angezeigt, welche Glasart optimiert wur-
                                       de.

                                       Modus In diesem Feld wird Ihnen angezeigt, welcher Optimierungsmodus
                                       verwendet wurde.

                                       Schneidtisch Hier sehen Sie, auf welchem Tisch das Glas geschnitten wird.

                                       Läufe In diesem Feld werden Ihnen die Laufnummern angezeigt.

                                       Status In diesem Feld wird Ihnen der Status angezeigt.

                                       Stückzahl In diesem Feld wird Ihnen die optimierte Stückzahl angezeigt.

                                       Fläche In dieser Spalte wird Ihnen die Gesamtfläche der optimierten Artikel
                                       angezeigt.

                                       Ergebnis In diesem Feld wird Ihnen das Ergebnis der Optimierung für die je-
                                       weilige Glasart angezeigt.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                                  I-139
                 Expertenmodus                                                              Softwarereferenz




                                 Erläuterung der Felder im Bereich Reports

                                 Name In dieser Spalte wird Ihnen der Name des Reports angezeigt, z. B. Pro-
                                 duktionsliste, Rahmenliste, etc.

                                 Drucker In diesem Feld wird Ihnen angezeigt, auf welchem Drucker die Aus-
                                 gabe erfolgt.

                                 Exemplare In diesem Feld wird Ihnen angezeigt, wie viele Exemplare aus-
                                 gegeben werden.

                                 Einstellungen Diese Spalte verfügt über Kontextmenüs, die von der Art des
                                 Reports abhängig sind.

                                 Meldung Das in dieser Spalte angezeigte Symbol informiert Sie über den
                                 Stand der Ausgabe.

                                 Erläuterung der Felder im Bereich Maschinen

                                 Maschine In dieser Spalte wird Ihnen die Maschine, für die der Maschinen-
                                 code ausgegeben wird, angezeigt.

                                 Ausgabe In diesem Feld wird Ihnen angezeigt, in welchem Verzeichnis der
                                 Maschinencode gespeichert wird.


                                 Ergänzende Informationen
                                  Tutorial, “Ausgabe” auf Seite I-63
2.21 / 01-2017




                 I-140                                                  A+W Business Pro Production Manager
                 Softwarereferenz                                                                      Expertenmodus




                                       Druckeinstellungen
                                       Produktionsmanager > Register Ausgabe > Druckeinstellungen




                                       Abb. I-86    Druckeinstellungen


                                       In diesem Dialog nehmen Sie die Einstellungen für folgenden Ausgabe vor:
                                       •   Etiketten
                                       •   Schneidplan
                                       •   Drucker

                                       Erläuterung der Felder im Bereich Etiketten

                                       Serie ab In diesem Feld geben Sie ein, ab welcher Stückzahl eine Serie be-
                                       ginnt. Über die Radiotasten darunter steuern Sie, ob ein Etikett pro Position
                                       oder ein Etikett pro Stück gedruckt werden soll. Bei der Variante ein Etikett pro
                                       Stück können Sie darüber hinaus im Feld dahinter noch angeben, alle wie viel
                                       Stück ein Etikett gedruckt werden soll.

                                       Erläuterung der Felder im Bereich Schneidplan

                                       Alles drucken Wenn Sie diese Radiotaste aktivieren, werden alle Schneid-
                                       pläne gedruckt.

                                       Letzte Seite drucken Wenn Sie diese Radiotaste aktivieren, wird nur die
                                       letzte Seite des Schneidplans gedruckt.
2.21 / 01-2017




                 A+W Business Pro Production Manager                                                              I-141
                 Expertenmodus                                                            Softwarereferenz




                                 Erläuterung der Felder im Bereich Drucker

                                 Reports Aus der Kombobox können Sie den Drucker auswählen, auf dem die
                                 Reports gedruckt werden sollen.

                                 Etiketten Aus der Kombobox können Sie den Drucker auswählen, auf dem
                                 die Etiketten gedruckt werden sollen.

                                 Exemplare Hier können Sie einstellen, wie viele Exemplare standardmäßig
                                 gedruckt werden sollen.

                                 Erläuterung der Schaltflächen

                                 Speichern Über diese Schaltfläche können Sie die globalen Druckeinstellun-
                                 gen speichern. Sie stehen dann immer so zur Verfügung und müssen nicht für
                                 jeden Druck neu gemacht werden.
2.21 / 01-2017




                 I-142                                              A+W Business Pro Production Manager
                 Softwarereferenz                                                                    Expertenmodus




                                       Auftragssuche
                                       Informationen > Auftrag




                                       Abb. I-87    Auftrag suchen


                                       Über diesen Dialog haben Sie die Möglichkeit, einen Auftrag gezielt zu su-
                                       chen. Dazu stehen Ihnen mehrere Suchkriterien zur Verfügung. Der Dialog ist
                                       in verschiedene Bereiche unterteilt. Im Bereich Selektionskriterien können Sie
                                       über die Auftragsnummer, den Nummernverwalter oder den Kunden die ge-
                                       wünschten Daten auswählen.

                                       Erläuterung der Felder im Bereich Selektionskriterien

                                       Auftragsnummer Nachdem Sie die Radiotaste aktiviert haben, können Sie
                                       im Feld dahinter die gewünschte Auftragssnummer eingeben.

                                       Nummernverwalter Nachdem Sie die Radiotaste aktiviert haben, können
                                       Sie aus der Kombobox auf die entsprechenden Daten zugreifen. Die Kombo-
                                       box enthält alle Einträge, die Sie im Bereich des Nummernverwalters angelegt
                                       haben.
2.21 / 01-2017




                                       Kunde Nachdem Sie die Radiotaste aktiviert haben, können Sie aus der
                                       Kombobox auf die entsprechenden Daten zugreifen. Die Kombobox enthält




                 A+W Business Pro Production Manager                                                           I-143
                 Expertenmodus                                                                      Softwarereferenz




                                 alle Kunden, für die es Aufträge in der Zeitwirtschaft des A+W Business Pro
                                 gibt.

                                 Die Bereiche Aufträge und Positionen
                                 Die Bereiche Aufträge und Positionen sind identisch mit den gleichnamigen
                                 Feldern im Bereich Auftragsselektion und werden an dieser Stelle nicht noch
                                 einmal erläutert.
                                  “Erläuterung der Felder im Bereich Aufträge” auf Seite I-106
                                  “Erläuterung der Felder im Bereich Positionen” auf Seite I-107


                                 Ergänzende Informationen
                                  Tutorial, “Aufträge auswählen” auf Seite I-27
2.21 / 01-2017




                 I-144                                                  A+W Business Pro Production Manager
Produktionsmanager          I

                     Partindex




            A+W Business Pro
                 Partindex                                                                       Index




                 Index
                 A                                      – Gasfüllung (Positionen) I-108
                 Abstellplätze                          – Gläser (Positionen) I-108
                 – Logischer Abstellplatz I-95, I-97    – Höhe (Positionen) I-108
                 – Sortierschlüssel I-98                – Kopfteile (Positionen) I-109
                 Abstellplatzgruppe                     – Kopfteiletyp (Positionen) I-109
                 – Name I-97                            – Kundendaten I-107
                 – Sortierschlüssel I-97                – Kundennummer I-106
                 – Sortierschlüssel-Vorschau I-97       – Kurzinfo (Positionen) I-107
                 Abstellplatzorganisation I-90          – Laufmeter (Positionen) I-108
                 – Abstellplatzgruppe I-91              – Liefertermin I-107
                 – Anzahl Fächer I-92                   – Modellnummer (Positionen) I-108
                 – Anzahl Scheiben pro Fach I-92        – Nummernverwalter I-105
                 – Formel I-91                          – Positionsnummer (Positionen) I-107
                 – Gestell-Nr. aktuell I-92             – Priorität I-107
                 – Gestell-Nr. bis I-92                 – Produkt I-106
                 – Gestell-Nr. von I-91                 – Produkt (Positionen) I-107
                 – Gestelltiefe I-92                    – Produktart (Positionen) I-108
                 – Logischer Abstellplatz I-91          – Produktbezeichnug 1/2 (Positionen) I-107
                 – Name I-91                            – Produktbezeichnung 1 I-106
                 – Name (Auswahl) I-90                  – Produktgruppe (Positionen) I-108
                 – Physikalischer Abstellplatz I-92     – Sprossen (Positionen) I-108
                 – Produktionsreihenfolge I-91          – Status I-106
                 – Prüfreihenfolge I-91                 – Stücklistenposition (Positionen) I-107
                 – Standard I-91                        – Stückzahl I-106
                 – Standard (Auswahl) I-90              – Stückzahl (Positionen) I-108
                 – Typ I-91                             – Stufe (Positionen) I-108
                 Aggregatumlastujng I-128               – SZR (Positionen) I-108
                 Ansicht speichern I-110, I-117         – Tour I-107
                 – Name I-110                           – Versanddatum I-107
                 Auftrag suchen                         – Vertreter I-106
                 – Auftragsnummer I-143                 – Wunschtermin I-107
                 – Kunde I-143                          Ausgabe I-138
                 – Nummernverwalter I-143               – Abstellplatzorganisation I-138
                 Auftragsselektion                      – Ausgabe (Maschine) I-140
                 – Arbeitsgang I-105                    – Benutzer I-138
                 – Auftragsnummer I-106                 – Drucker I-140
                 – Auftragsnummer (Positionen) I-107    – Einstellungen I-140
                 – AV-Bereich I-106                     – Ergebnis (Optimierungen) I-139
                 – Beschaffungsart (Positionen) I-108   – Erstelldatum I-138
                 – Bestelldatum I-107                   – Erstelldatum (Optimierung) I-139
                 – Breite (Positionen) I-108            – ESG I-139
                 – Datum von/bis I-105                  – Fläche (Optimierungen) I-139
                 – Erfassungsdatum I-106                – Glas I-139
                 – Erfassungsdatum (Positionen) I-107   – Glasart I-139
                 – Fachberater I-106                    – ISO I-139
                 – Fläche I-106                         – Laufbezeichnung I-138
2.21 / 01-2017




                 – Fläche (Positionen) I-108            – Läufe I-139
                 – Fläche im Verhältnis I-106           – Laufnummer I-138
                 – Folien (Positionen) I-109            – Maschine I-140


                 A+W Business Pro Production Manager                                            I-147
                 Index                                                                                 Partindex




                 – Meldung I-139, I-140                       – Erstelldatum I-121
                 – Modus I-139                                – Faktor für Abstellplatztiefe I-122
                 – Name des Reports I-140                     – Fläche I-122
                 – Optimierungsnummer I-139                   – Fläche % I-122
                 – Schneidtisch I-139                         – Produkt I-122
                 – Status I-139                               – Produktbezeichnung 1 I-122
                 – Stückzahl I-139                            – Status I-122
                 – VSG I-139                                  – Stückzahl I-122
                                                              Detailansicht Optimierung I-133, I-137
                 B                                            Dokumentation
                 Bruch erfassen                               – Arten I-10
                 – Auftrag I-116                              Druckeinstellungen I-141
                 – Grund I-116                                – Alles drucken I-141
                 – Position I-116                             – Drucker für Etiketten I-142
                 – Stelle I-116                               – Drucker für Reports I-142
                 – Stückzahl I-116                            – Exemplare I-142
                 Bruchscheiben                                – Letzte Seite drucken I-141
                 – Aggregat I-115                             – Serie ab I-141
                 – Auftragsnummer I-113
                 – Bearbeitungen I-115                        E
                 – Beschaffungsart (Positionen) I-114         Expertenmodus
                 – Breite (Positionen) I-113                  – Überblick I-24, I-70
                 – Fläche (Positionen) I-114
                 – Folien (Positionen) I-114                  G
                 – Gasfüllung (Positionen) I-114              Gruppierungen
                 – Gläser (Positionen) I-114                  – Ansicht speichern    I-110, I-117
                 – Höhe (Positionen) I-113
                 – Kopfteile (Positionen) I-114
                 – Kopfteiletyp (Positionen) I-114            K
                 – Kurzinfo (Positionen) I-113                Kriterien I-93
                 – Lauf I-113                                 Kriterium
                 – Laufmeter (Positionen) I-114               – Name I-93
                 – Modellnummer (Positionen) I-114            – Sortierschlüssel    I-93
                 – Positionsnummer I-113
                 – Produkt (Positionen) I-113                 L
                 – Produktart (Positionen) I-114              Läufe
                 – Produktbezeichnug 1/2 (Positionen) I-113   – Aggregatumlastung I-128
                 – Produktgruppe (Positionen) I-114           – Detailansicht I-121
                 – Produktionsdatum I-115                     – Laufübersicht I-119
                 – Sprossen (Positionen) I-114                Läufe erstellen
                 – Stücklistenposition (Positionen) I-113     – Übersicht I-39, I-50, I-63
                 – Stückzahl (Positionen) I-113               Laufstatus setzen I-127
                 – Stufe (Positionen) I-114                   – Neu I-127
                 – SZR (Positionen) I-114                     Laufübersicht I-119
                 – Unterpositionsnummer I-113, I-116          – Abstellplatzorganisation I-120
                                                              – Bezeichnung I-120
                 D                                            – Erstelldatum I-119, I-120
                 Darstellungskonventionen I-11                – ESG I-120
                 Detailansicht für Läufe I-121                – Faktor für Abstellplatztiefe I-120
2.21 / 01-2017




                 Detailansicht Lauf                           – Glas (Einzel und Bearbeitet) I-120
                 – Abstellplatzorganisation I-121             – ISO I-120
                 – Bezeichnung I-121                          – Laufnummer I-119, I-120



                 I-148                                                 A+W Business Pro Production Manager
                 Partindex                                                                     Index




                 – Status I-120                          P
                 – VSG I-120                             Produkt
                 Logischer Abstellplatz                  – Breite I-111
                 – Gruppen sortiert I-96                 – Höhe I-111
                 – Gruppierung I-96                      – Modellnummer I-111
                 – Name I-95                             – Modellparameter I-112
                 – Sortierung in den Gruppen   I-96      – SN-Datei I-111
                 – Typ I-95                              – Stückzahl I-111
                                                         – Vorschau I-112
                 M
                 Modul                                   S
                 – Funktion   I-9                        Sortierschlüssel
                                                         – Formel I-98
                 N                                       – Name I-98
                 Name der Ansicht I-110                  – Sortierung I-98
                 Neuer Lauf                              Stammdaten
                 – Abstellplatzorganisation I-117        – Allgemein I-99, I-104
                 – Ausgabe I-118                         Standardmodus
                 – Bezeichnung I-117                     – Abstellplatzorganisation I-101
                 – Faktor für Abstellplatztiefe I-117    – Abstellplatzorganisation
                 – Feinplanung I-118                       (Gesamtergebnis) I-103
                 – Kompletter Handzuschnitt I-118        – Anzahl A-Böcke (Gesamtergebnis) I-103
                 – Laufnummer I-117                      – Anzahl Fächerwagen (Gesamtergebnis) I-103
                 – Optimierungsmanager I-118             – Anzahl Varianten I-101
                 – Unbegrenzte Abstellplatztiefe I-118   – Ausgaben I-102
                                                         – Bezeichnung I-101
                                                         – Ergebnis I-103
                 O
                                                         – Ergebnis (Optimierungen) I-102
                 Optimierung abbrechen I-132
                                                         – Faktor für Abstellplatztiefe I-101
                 Optimierungsmanager I-130
                                                         – Fläche (Optimierungen) I-102
                 – Abstellplatzorganisation I-131
                                                         – Glasart (Optimierungen) I-102
                 – Erstelldatum I-130
                                                         – Läufe (Optimierungen) I-102
                 – ESG I-131
                                                         – Laufnummer I-101
                 – Faktor für Abstellplatztiefe I-131
                                                         – Nummernverwalter I-101
                 – Glas (Einzel und Bearbeitet) I-131
                                                         – Schneidtisch (Optimierungen) I-102
                 – ISO I-131
                                                         – Status I-101
                 – Laufbezeichnung I-130
                                                         – Stückzahl (Optimierungen) I-102
                 – Laufnummer I-130
                                                         – Unbegrenzte Abstellplatztiefe I-101
                 – Status I-130
                                                         – Variante (Gesamtergebnis) I-102
                 – VSG I-131
                                                         – Verschnitt (Gesamtergebnis) I-103
                 Optimierungsübersicht I-135
                 – Ergebnis I-136
                 – Erstelldatum I-135, I-136             T
                 – Fläche I-136                          Temporäre Optimierung
                 – Glasart I-136                         – Bezeichnung I-134
                 – Läufe I-136                           – Breite (Lagermaße) I-134
                 – Laufnummer I-136                      – Breite (Muster) I-134
                 – Optimierung I-135, I-136              – Erstelldatum I-134
                 – Optimierungsmodus I-136               – Fläche I-134
                                                         – Gestell I-133
2.21 / 01-2017




                 – Schneidtisch I-136
                 – Status I-136                          – Gestelltyp I-133
                 – Stückzahl I-136                       – Höhe (Lagermaße) I-134
                                                         – Höhe (Muster) I-134


                 A+W Business Pro Production Manager                                           I-149
                 Index                                                         Partindex




                 – Laufnummer I-133, I-134
                 – Log. Abstellplatz I-134
                 – Menge I-134
                 – Menge (Lagermaße) I-134
                 – Menge (Muster) I-134
                 – Muster I-134
                 – Optimierungsgruppe I-134
                 – Priorität I-134

                 U
                 Überblick
                 – Expertenmodus   I-24, I-70

                 Z
                 Zuschnitt
                 – Breite I-123
                 – Höhe I-123
                 – Modellbruchränder I-124, I-126
                 – Modellnummer I-123
                 – Modellparameter I-124, I-126
                 – Schaltfläche Bearbeiten I-124
                 – SN-Datei I-123
                 – Stückzahl I-123
                 – Vorschau I-124, I-126
                 Zuschnitt bearbeiten
                 – Breite I-125
                 – Höhe I-125
                 – SN-Datei I-125
                 – Stückzahl I-125
2.21 / 01-2017




                 I-150                              A+W Business Pro Production Manager

