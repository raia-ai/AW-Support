---
title: "DE AWProduction Realtime Optimizer 3.30"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWProduction_Realtime_Optimizer_3.30"]
version: "1.0"
last_updated: "2025-12-10"
description: "A+W Realtime Optimizer      J                                deutsch                     A+W Production                                                                                                              Vorspann                                               Vorspann                                           In diesem Teil der Dokumentation finden Sie editorische Notizen.                                             Revisionsübersicht                                           Part"
source_file: "DE_AWProduction_Realtime_Optimizer_3.30.pdf"
---


# DE AWProduction Realtime Optimizer 3.30

A+W Realtime Optimizer      J




                           deutsch




                A+W Production
                                                                                                             Vorspann




                                          Vorspann
                                          In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                          Revisionsübersicht
                                          Part                     Beschreibung
                                          Version / Datum

                                          3.30/01-2023             Diverse Ergänzungen

                                          3.20/10-2020             Dialog Tischoptimierung hinzugefügt

                                          3.10/04-2019             Dialog DynOpt-Einstellungen hinzugefügt

                                          3.02/ 09-2018            Felder hinzugefügt

                                          3.01 / 01-2017           Produkt- und Firmennamen angepasst

                                          3.00 / 03-2015           Komplette Überarbeitung

                                          2.01 / 07-2013           Vollständige Überarbeitung der XOPT-ON-
                                                                   Dokumentation und Anpassung auf A+W Realtime
                                                                   Optimizer.

                                          2.00 / 09-2007           Komplette Überarbeitung

                                          1.00 / 03-2003           Ersterstellung



                                          Editorial
                                          Das Editorial enthält Informationen zu folgenden Themen:
                                          •   Anmerkungen zu diesem Dokument
                                          •   Urheberrechte
                                          •   Warenzeichen
                                          •   Kontakt

                                          Anmerkungen zu diesem Dokument
                                          Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Realtime
                                          Optimizer gedacht.
                                          Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz
                                          vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden.
                                          Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
                                          ohne Vorankündigung geändert werden.
                                          Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter
                                          Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausge-
3.30 / 01-2023




                                          schlossen werden. Die A+W Software GmbH übernimmt keine Haftung für
                                          Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem
                                          oder grobfahrlässigem Handeln.



                 A+W Realtime Optimizer                                                                           J-3
                 Vorspann




                            Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbau-
                            stufe von A+W Production.

                            Urheberrechte
                            © 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
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

                            Kontakt
                            A+W Software GmbH
                            Siemensstr. 3
                            D-35463 Fernwald
                            Germany
                               +49 641 96620-0
                            info@a-w.com
                            http://www.a-w.com
3.30 / 01-2023




                 J-4                                                            A+W Realtime Optimizer
                                                                                                                                                                  Inhalt




                                          Inhalt
                                          Vorspann ................................................................................................................ J-3
                                            Revisionsübersicht .............................................................................................. J-3
                                            Editorial ............................................................................................................... J-3
                                          Inhalt ....................................................................................................................... J-5

                                          Tutorial                                                                                                                 J-9
                                          Grundgedanken .................................................................................................... J-11
                                            Leistungsmerkmale ........................................................................................... J-12
                                          Arbeiten mit A+W Realtime Optimizer .................................................................. J-13
                                            Überblick ........................................................................................................... J-14
                                            Datenübernahme ............................................................................................... J-15
                                              Anbindung an A+W Production ...................................................................... J-16
                                                Stammdaten ............................................................................................... J-17
                                              Verwendung als stand alone-System ............................................................ J-17
                                                Optimierungen importieren ......................................................................... J-17
                                          Erfassung .............................................................................................................. J-19
                                            Überblick ........................................................................................................... J-20
                                              Bruch, Eilscheiben und Füllaufträge .............................................................. J-21
                                                Scheiben manuell erfassen ........................................................................ J-22
                                              Manuelle Planerstellung ................................................................................. J-25
                                              Chargen-Editor ............................................................................................... J-26
                                          Optimierung .......................................................................................................... J-27
                                            Überblick ........................................................................................................... J-28
                                            Tischoptimierungen ........................................................................................... J-29
                                              Tischoptimierungen erstellen ......................................................................... J-29
                                              Ergebnis der Tischoptimierung prüfen und bearbeiten .................................. J-31
                                              Tischoptimierung auflösen ............................................................................. J-32
                                              Tischoptimierungen verlinken ........................................................................ J-34
                                            Schnelloptimierung erstellen ............................................................................. J-35
                                            Verlinken von Läufen ......................................................................................... J-36
                                            Tischansteuerung .............................................................................................. J-37
                                          Zuschnitt ............................................................................................................... J-38
                                            Überblick ........................................................................................................... J-39
                                              Läufe zum Zuschnitt auswählen .................................................................... J-40
                                              Optimierung prüfen und schneiden ................................................................ J-43
                                              Arbeit unterbrechen und fortsetzen ................................................................ J-45
                                              Die Zuschnitt-Übersicht .................................................................................. J-46
                                            Schneidstatus zurücksetzen .............................................................................. J-48
                                          Zusammenarbeit mit anderen Modulen ................................................................ J-49
                                            Überblick ........................................................................................................... J-50
                                            A+W Residual Stock Manager .......................................................................... J-50
                                              A+W Planning Web ........................................................................................ J-50
                                                Oberfläche .................................................................................................. J-51
                                                Stammdaten ............................................................................................... J-51
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                                                              J-5
                 Inhalt




                             A+W Pattern Viewer .......................................................................................... J-59
                              Einstellungen ................................................................................................. J-59
                              Die Oberfläche ............................................................................................... J-60
                                Die Menüleiste ............................................................................................ J-60
                                Informationen zu Scheibe und Verschnitt ................................................... J-69
                                Verlinkte Läufe anzeigen ............................................................................ J-69
                                Abstellkante anzeigen ................................................................................ J-70
                                Symbol für Stempel, Logo oder Referenzmarke anzeigen ......................... J-70
                                Farbauswahl für Auftragspositionen ........................................................... J-71
                                Erste und letzte Scheibe markieren ............................................................ J-71
                                Bruchscheiben ............................................................................................ J-71
                             A+W PlanEditor ................................................................................................. J-72
                             A+W Continuous Cutting ................................................................................... J-73
                              Übersicht der geplanten Läufe ....................................................................... J-73
                                Gruppieren .................................................................................................. J-76
                                Eilgruppen .................................................................................................. J-77
                                Zurücksetzen von Läufen ........................................................................... J-77
                              Zuschneiden .................................................................................................. J-78
                             A+W Defect Optimizer ....................................................................................... J-80
                             A+W DynOpt Compact ...................................................................................... J-81
                              A+W DynOpt Compact Import ....................................................................... J-81
                              A+W DynOpt Compact Optimierung .............................................................. J-81
                                A+W DynOpt Compact-Lauf erzeugen ....................................................... J-82

                          Softwarereferenz                                                                                                  J-85
                          Übersicht ............................................................................................................... J-87
                            Menüs ................................................................................................................ J-87
                            Symbol-Schaltflächen ........................................................................................ J-88
                          Erfassung .............................................................................................................. J-89
                            Eilscheiben ........................................................................................................ J-90
                            Eilscheiben-Eingabe .......................................................................................... J-92
                            Form-Erfassung ................................................................................................. J-94
                            Modell-Nummer ................................................................................................. J-96
                            Manuelle Planerstellung .................................................................................... J-97
                            Chargen-Editor ................................................................................................ J-100
                          Optimierung ........................................................................................................ J-102
                            Selektieren Sie die zu optimierenden Gläser .................................................. J-103
                              Tischoptimierung in der Variante Standard .................................................. J-103
                              Tischoptimierung in der Variante Produktionstermin ................................... J-106
                            Tischoptimierung Lauf [Nr] .............................................................................. J-107
                              Übersicht ...................................................................................................... J-107
                            Optimieren ....................................................................................................... J-110
                                 Erläuterung der Felder im Bereich Optimierungsreihenfolge ................... J-110
                                 Erläuterung der Schaltflächen im Bereich Rangfolge ............................... J-111
                                 Erläuterung der Felder im Bereich Automatische Zusammenstellung ..... J-111
                                 Erläuterung der Felder im Bereich Lauf-Parameter .................................. J-112
                                 Erläuterung der Felder im Bereich Tisch .................................................. J-112
                                 Erläuterung der Felder im Bereich Optimierungs-Parameter ................... J-112
                            Restplattlagerplatten und Lagerplatten ........................................................... J-113
                            Parameter ........................................................................................................ J-115
                            Anzahl der Lagerplatten .................................................................................. J-118
                            Zurücksetzen eines Zuschnitt Laufes .............................................................. J-119
                            Pausierende Glasarten .................................................................................... J-121
3.30 / 01-2023




                            Aktuell geänderte Einstellungen ...................................................................... J-123
                          Zuschnitt ............................................................................................................. J-124
                            Wählen Sie einen Lauf aus ............................................................................. J-125
                            Lauf [Nummer] - Lauf [Nummer] ...................................................................... J-129


                 J-6                                                                                          A+W Realtime Optimizer
                                                                                                                                                              Inhalt




                                            Optimierungsreihenfolge ................................................................................. J-131
                                            Lauf: Nummer .................................................................................................. J-132
                                            Auswahl der zu verlinkenden Optimierung ...................................................... J-136
                                            Optimierungsergebnis ..................................................................................... J-137
                                            Bruchpool ........................................................................................................ J-138
                                            Brucherfassung ............................................................................................... J-141
                                              Suchfelder .................................................................................................... J-142
                                            Modell-Erfassung ............................................................................................ J-143
                                            A+W DynOpt - Editor ....................................................................................... J-144
                                                Erläuterung der Schaltflächen .................................................................. J-145
                                          Einstellungen ...................................................................................................... J-148
                                            Einstellungen ................................................................................................... J-149
                                            Tischoptimierung ............................................................................................. J-151
                                          Ansicht ................................................................................................................ J-152
                                            Import .............................................................................................................. J-153
                                            Fehlermeldungen ............................................................................................ J-154
                                          A+W Residual Stock Manager ............................................................................ J-155
                                            A+W Planning Web ......................................................................................... J-155
                                            Lager ............................................................................................................... J-155
                                            Abstellplatzinformationen ................................................................................ J-157
                                            Gestelle ........................................................................................................... J-159
                                            Gestelleigenschaften ....................................................................................... J-161
                                                Eindeutiger Name zur Identifizierung eines Gestelltyp. ............................ J-161
                                            Glasübersicht .................................................................................................. J-163
                                                Wenn Sie auf diese Schaltfläche klicken, wird der Datensatz zur Bearbeitung
                                                freigegeben und Sie können Änderungen vornehmen. ............................ J-165
                                            Neuen Datensatz hinzufügen/bearbeiten ........................................................ J-166

                                          Partindex                                                                                                      J-169
                                          Index A+W Realtime Optimizer .......................................................................... J-171
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                                                          J-7
                 Inhalt
3.30 / 01-2023




                 J-8      A+W Realtime Optimizer
A+W Realtime Optimizer        J

                         Tutorial




                A+W Production
                 Tutorial                                                                             Grundgedanken




                                          Grundgedanken
                                          Ein wesentliches Einsparpotential bei der Flachglasverarbeitung ist die opti-
                                          male Ausnutzung der Lagerplatten beim Zuschnitt. Je weniger Verschnitt oder
                                          Restblätter, desto höher die Materialausnutzung und desto geringer die Mate-
                                          rialkosten. Die Ansteuerung von Zuschnitttischen mit den optimierten Schnitt-
                                          bildern direkt aus der Optimierung beschleunigt den Arbeitsprozess.
                                          A+W Realtime Optimizer basiert auf diesen beiden Grundgedanken:
                                          •   Zuschnittoptimierung für den angeschlossenen Zuschnitttisch.
                                          •   Übertragung von Schneidcode an den angeschlossenen Zuschnitttisch.




                                          Abb. J-1    Zuschnittoptimierung und Tischansteuerung
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-11
                 Grundgedanken                                                                         Tutorial




                                 Leistungsmerkmale
                                 A+W Realtime Optimizer unterstützt die genannten Grundgedanken mit fol-
                                 genden Leistungsmerkmalen:
                                 •   A+W Realtime Optimizer steuert Ihren Zuschnitt mit optimierten Feinpla-
                                     nungsdaten.
                                 •   In ein Restblatt können automatisch Eil-, Bruch- oder Füllscheiben nach-
                                     optimiert werden.
                                 •   Die Ansteuerung der Schneidtische erfolgt hauptsächlich online über die
                                     Kommunikationsprotokolle, die von den Tischherstellern unterstützt wer-
                                     den.
                                 •   Eilscheiben, Bruchscheiben und Füller werden direkt am Zuschnitt opti-
                                     miert.
                                 •   Es besteht die Möglichkeit, bereits vorhandene Optimierungen für eine
                                     Tischoptimierung zu prüfen, aufzulösen und nochmals neu zusammenzu-
                                     fassen. Dabei können gemeinsam mit Bruch-, Füll- und Eilscheiben Opti-
                                     mierungen größerer Mengen erzeugt werden. Vorgegebene Reihenfolgen
                                     auf A-Böcken bleiben dabei erhalten.
                                 •   A+W Production bietet bereits bei der Feinplanung die Möglichkeit, den Zu-
                                     schnitt für jeden Lauf auf den geplanten Schneidtisch zu optimieren.
                                 •   A+W Realtime Optimizer wird speziell für einen Schneidtisch konfiguriert
                                     und kann die für diesen Schneidtisch vorgeplanten und bereits optimierten
                                     Läufe mit dem Schneidcode an den Schneidtisch übertragen.
                                 •   Wenn der erforderliche Maschinencode an den Schneidtisch übermittelt
                                     wurde, dann kann das Brechbild mit XTV angezeigt werden.
3.30 / 01-2023




                 J-12                                                                A+W Realtime Optimizer
                 Tutorial                                                      Arbeiten mit A+W Realtime Optimizer




                                          Arbeiten mit A+W Realtime
                                          Optimizer
                                          In diesem Themenblock lernen Sie die Arbeitsweise des A+W Realtime Opti-
                                          mizer kennen.
                                          Der Themenblock beinhaltet folgende Schulungseinheiten:
                                          •   Datenübernahme
                                              – Anbindung an A+W Production
                                              – Verwendung als stand alone-System
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                      J-13
                 Arbeiten mit A+W Realtime Optimizer                                                              Tutorial




                                         Überblick
                                         Lernziele

                                         • Die Datenübernahme kennenlernen und verstehen.
                                         • Die Anbindung an A+W Production kennenlernen und verstehen.
                                         • Die Verwendung als stand alone-System kennenlernen und verstehen.


                                         Nutzen

                                         Zum optimalen Arbeiten mit dem A+W Realtime Optimizer müssen die Daten korrekt
                                         übernommen werden.


                                         Definitionen

                                         Vorsysteme                Liefern Aufträge (Läufe), in denen Stammdaten und
                                                                   Zuschnittoptimierungen enthalten sind.

                                         Stand-alone Variante      Hier erfolgt die Datenübernahme mithilfe von save-
                                                                   Dateien, die in einem bestimmten Verzeichnis zur
                                                                   Verfügung gestellt werden.

                                         Restelager                Mit einem Restelager-Magazin werden Restplatten am
                                                                   Zuschnitttisch verwaltet.


                                         Merke

                                         A+W Realtime Optimizer    Kann an alle gängigen Zuschnitttische angepasst
                                                                   werden.

                                         Stand-alone Variante      Der A+W Realtime Optimizer kann auch stand-alone
                                                                   eingesetzt werden.

                                         Anbindung                 Die Datenübernahme wird im Rahmen der Installation
                                                                   von A+W Mitarbeitern konfiguriert.
3.30 / 01-2023




                 J-14                                                                          A+W Realtime Optimizer
                 Tutorial                                                                Arbeiten mit A+W Realtime Optimizer




                                             Datenübernahme
                                             Je nach dem, welches Vorsystem verwendet wird, erfolgt die Datenübernah-
                                             me aus dem Vorsystem voll- oder halbautomatisch. Vorsysteme liefern an
                                             A+W Realtime Optimizer Aufträge (Läufe), in denen Stammdaten und Zu-
                                             schnittoptimierungen enthalten sind.

                     Datenübernahme                       Datenerfassung und -                        Tischansteuerung
                                                              verarbeitung

                                                        A+W Realtime Optimizer
                            Läufe                           Optimierung und
                                                         Schneidcodegenerierung

                                                                                                        Zuschnitttisch




                                                               Datenbank




                 Abb. J-2      Übersicht der Arbeiten mit A+W Realtime Optimizer, die in kursiver Schrift dargestellten Arbeiten
                               kommen nur bei stand alone-Systemen zum Einsatz


                                             Die vielfältigen Konfigurationsmöglichkeiten erlauben folgende Einsatzmög-
                                             lichkeiten des A+W Realtime Optimizer:
                                             •   Eingebettet in eine A+W Production oder A+W Business Pro-Umgebung.
                                             •   Anpassung an alle gängigen Zuschnitttische.
                                             •   Anbindung an ein Restelager.
                                             •   Einsatz als stand alone-System.
                                             Die Konfiguration und Installation für die verschiedenen Einsatzmöglichkeiten
                                             wird von A+W-Mitarbeitern durchgeführt.
                                             Mögliche Vorsysteme sind:
                                             •   A+W Production
                                             •   A+W Business Pro

                                                 Anbindung an ein Vorsystem
                                                 Welches Vorsystem bei Ihnen eingesetzt wird und die Art und Weise, wie
                                                 Daten übernommen werden, wird im Rahmen der Installation von A+W-
                                                 Mitarbeitern konfiguriert.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                      J-15
                 Arbeiten mit A+W Realtime Optimizer                                                          Tutorial




                                                                               A+W Realtime
                                                                                 Optimizer
                                                    Import-Dateien           Import und Prüfung
                                                                                 der Daten,
                                                                              Übernahme in die
                                                                                Datenbank




                                                                        A+W Production-Datenbank
                                                                          Läufe mit Optimierungen
                                                                          und Stammdaten:
                                          A+W Production                  Artikel
                                                                          Glasarten
                                                                          Tische
                                                                          Optimierungsparameter
                                                                          Lagerplatten


                                         Abb. J-3       Datenübernahme in A+W Realtime Optimizer


                                         Wenn A+W Realtime Optimizer mit A+W Production zusammenarbeitet, dann
                                         verwendet A+W Realtime Optimizer die A+W Production-Datenbank mit.
                                         Kommt ein anderes Vorsystem zum Einsatz, dann benötigt A+W Realtime Op-
                                         timizer eine leere A+W Production-Datenbank. Stammdaten und Optimierun-
                                         gen, die in den Läufen des Vorsystems enthalten sind, werden von A+W
                                         Realtime Optimizer in die leere A+W Production-Datenbank übernommen.
                                         Dabei werden die Daten geprüft.
                                         Daten, die bei der Übernahme einen Fehler verursacht haben, werden abge-
                                         wiesen. Im erstellten Fehlerprotokoll können Sie nachvollziehen, welche Da-
                                         tensätze warum abgewiesen wurden. Diese Daten können Sie dann
                                         nachbearbeiten.


                                         Anbindung an A+W Production
                                         Bei der Anbindung von A+W Realtime Optimizer an ein bestehendes A+W
                                         Production-System erfolgt ein vollautomatischer Datenaustausch. Stammda-
                                         ten, Läufe, Bruch, Eil- und Füllaufträge werden direkt aus der A+W Produc-
                                         tion-Datenbank genommen. Darüber hinaus werden Statusmeldungen für die
                                         einzelnen Läufe in die Datenbank zurückgeschrieben.
3.30 / 01-2023




                 J-16                                                                         A+W Realtime Optimizer
                 Tutorial                                                         Arbeiten mit A+W Realtime Optimizer




                                          Stammdaten
                                          Wenn bei der Konfiguration der Zugang zu den Stammdaten freigegeben wur-
                                          de, dann können diese eingesehen und bearbeitet werden.
                                          Zu den Stammdaten zählen:
                                          •   Artikel
                                          •   Glasarten
                                          •   Tische
                                          •   Optimierungsparameter
                                          •   Lagerplatten
                                          Beschrieben sind diese Stammdaten und das Arbeiten damit im Part Feinpla-
                                          nung des Anwenderhandbuches A+W Production.


                                          Verwendung als stand alone-System
                                          A+W Realtime Optimizer wird bei der Installation mit einer leeren A+W Pro-
                                          duction-Datenbank eingerichtet. Diese Datenbank wird beim Import von Läu-
                                          fen nach und nach mit Stammdaten gefüllt.
                                          Beim stand alone-System erfolgt die Datenübernahme mit Hilfe von save-Da-
                                          teien, die A+W Realtime Optimizer in einem bestimmten Verzeichnis zur Ver-
                                          fügung gestellt werden müssen. Die save-Dateien müssen eine definierte
                                          Struktur einhalten und werden üblicherweise im Arbeitsverzeichnis …\Xop-
                                          ton\import\work\*save.* bereit gestellt. Eingelesene Daten werden aus dem
                                          Arbeitsverzeichnis entfernt und in ein Archivverzeichnis verschoben.

                                          Optimierungen importieren
                                          Die Funktion Optimierungen importieren ist nur bei A+W Realtime Optimizer
                                          stand alone-Versionen erforderlich und möglich.
                                          A+W Realtime Optimizer kann nur dann einen Zuschnitttisch mit Zuschnittda-
                                          ten versorgen oder Tischoptimierungen erstellen, wenn Läufe aus einem vor-
                                          gelagerten System zur Verfügung gestellt werden. Wenn solche Läufe
                                          bereitgestellt werden, dann kann A+W Realtime Optimizer diese zur Weiter-
                                          bearbeitung importieren.
                                          Folgende Arbeitsschritte können Sie im Rahmen der Importierung von Läufen
                                          durchführen:
                                          •   Import einschalten.
                                          •   Import ausschalten.
                                          •   Auf Fehlermeldungen reagieren.


                                           Import einschalten
                                          1 Öffnen Sie den Dialog Import. Wählen Sie dazu im Menü Ansicht > Import.
                                          2 Um den Import zu starten, betätigen Sie die Schaltfläche [Start].
3.30 / 01-2023




                                              A+W Realtime Optimizer prüft, ob im Arbeitsverzeichnis Importdateien vor-
                                              liegen. Werden solche Dateien gefunden, so werden diese Daten in die
                                              Datenbank importiert und die Importdateien werden ins Archiv-Verzeichnis
                                              verschoben.


                 A+W Realtime Optimizer                                                                           J-17
                 Arbeiten mit A+W Realtime Optimizer                                                             Tutorial




                                            Importierte Läufe werden in den Dialogen Wählen Sie einen Lauf aus und
                                            Selektieren Sie die zu optimierenden Gläser zur Weiterbearbeitung zur
                                            Verfügung gestellt.
                                            Die Schaltfläche [Start] wechselt die Darstellung auf [Stop].
                                         3 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [Schließen].
                                            A+W Realtime Optimizer überwacht das Arbeitsverzeichnis so lange, bis
                                            die Importfunktion ausgeschaltet wird.
                                            Wenn während des Imports Fehler auftreten, dann werden diese protokol-
                                            liert und die entsprechenden Läufe nicht importiert. Fehler können manuell
                                            nachbearbeitet werden.


                                          Import ausschalten
                                         1 Öffnen Sie den Dialog Import. Solange der Import eingeschaltet ist, befin-
                                           det sich der Dialog in minimierter Darstellung links unten im A+W Realtime
                                           Optimizer-Dialog.
                                         2 Um den Import zu beenden, betätigen Sie die Schaltfläche [Stopp].
                                            Neu ins Arbeitsverzeichnis gespeicherte Importdateien verbleiben dort un-
                                            bearbeitet.
                                            Die Schaltfläche [Stopp] wechselt die Darstellung auf [Start].
                                         3 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [Schließen].


                                          Auf Fehlermeldungen reagieren
                                            Wenn während des Imports Fehler auftreten, dann werden diese protokol-
                                            liert und die entsprechenden Läufe nicht importiert.
                                            Der Import wird nur dann gestoppt, wenn Datenverlust droht. Dies ist z. B.
                                            dann der Fall, wenn eine bereits vorhandene Optimierung überschrieben
                                            werden soll. Je nach Konfiguration erscheint eine entsprechende Fehler-
                                            meldung.
                                         1 Beantworten Sie die Frage im Fehlermeldungs-Dialog xopt-on.
                                           Wählen Sie dazu die entsprechende Schaltfläche [Ja] oder [Nein].
                                            Der Datenimport wird fortgesetzt.
                                         2 Öffnen Sie den Dialog Fehlermeldungen. Wählen Sie dazu im Menü An-
                                           sicht > Fehlermeldungen.
                                         3 Prüfen Sie die Fehlermeldungen und reagieren Sie entsprechend.


                                         Ergänzende Informationen
                                          “Auf Fehlermeldungen reagieren” auf Seite J-18
                                          Softwarereferenz, “Fehlermeldungen” auf Seite J-154
3.30 / 01-2023




                 J-18                                                                            A+W Realtime Optimizer
                 Tutorial                                                                                 Erfassung




                                          Erfassung
                                          In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit der Erfassung umgehen.
                                          Der Themenblock beinhaltet folgende Schulungseinheiten:
                                          •   Bruch, Eilscheiben und Füllaufträge
                                          •   Manuelle Planerstellung
                                          •   Chargen-Editor
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                        J-19
                 Erfassung                                                                               Tutorial




                             Überblick
                             Lernziele

                             • Bruchscheiben und den Umgang damit kennen lernen und verstehen.
                             • Eilscheiben und den Umgang damit kennen lernen und verstehen.
                             • Füllaufträge und den Umgang damit kennen lernen und verstehen.


                             Nutzen

                             Unter Verwendung von Bruch-, Eilscheiben und Füllaufträgen können Sie den
                             Verschnitt erheblich verbessern.


                             Definitionen

                             Bruchscheibe              Eine Scheibe, die beim Zuschnitt kaputt gegangen ist.

                             Eilscheibe                Eine Scheibe, die schnell geschnitten werden muss.

                             Füllauftrag               Dienen dazu, Kapazitäten und Material effizient
                                                       auszunutzen.


                             Merke

                             Bruchscheiben             Können manuell mit dem A+W Realtime Optimizer oder
                                                       an einer anderen Stelle einer vernetzten Produktion
                                                       erfasst werden.

                             Eilscheiben               Werden mit dem A+W Realtime Optimizer angelegt und
                                                       in der Datenbank gespeichert.

                             Füllaufträge              Können nur verwendet werden, wenn der A+W Realtime
                                                       Optimizer mit einem A+W Production -System
                                                       verwendet wird.
3.30 / 01-2023




                 J-20                                                              A+W Realtime Optimizer
                 Tutorial                                                                                      Erfassung




                                          Bruch, Eilscheiben und Füllaufträge
                                          Bruch kann manuell mit A+W Realtime Optimizer oder an einer anderen Stelle
                                          einer vernetzten Produktion erfasst werden. Je nach Konfiguration werden
                                          Bruchscheiben direkt im Bruchpool von A+W Realtime Optimizer angezeigt.
                                          Bei nächster Gelegenheit werden Bruchscheiben automatisch auf das Rest-
                                          blatt optimiert oder manuell (je nach Konfiguration) in eine Tischoptimierung
                                          integriert.
                                          Eilscheiben werden mit A+W Realtime Optimizer angelegt und in der Daten-
                                          bank gespeichert. Eilscheiben können ebenfalls bei der nächsten Tischopti-
                                          mierung, die eine passenden Glasart und Dicke verwendet, in die Optimierung
                                          integriert werden.
                                          Füllaufträge können nur verwendet werden, wenn A+W Realtime Optimizer
                                          mit einem A+W Production-System verwendet wird. Füllaufträge werden dann
                                          direkt aus der A+W Production-Datenbank entnommen.

                                            Eilscheiben        Bruch         Füller




                                                       Realtime Optimizer
                                                          Tischoptimierung
                                                              erstellen




                                                 A+W Production-Datenbank
                                                     Läufe mit Optimierungen
                                                     und Stammdaten:
                                                     Artikel
                                                     Glasarten
                                                     Tische
                                                     Optimierungsparameter
                                                     Lagerplatten




                                          Abb. J-4      Datenerfassung und -verarbeitung in A+W Realtime Optimizer
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                              J-21
                 Erfassung                                                                       Tutorial




                             Scheiben manuell erfassen
                             Zusätzlich zu den Läufen aus einem Vorsystem, können in A+W Realtime Op-
                             timizer Scheiben erfasst, in Tischoptimierungen eingebracht und zum
                             Schneidtisch übertragen werden.
                             Mit folgende Arbeitsschritten können Sie unterschiedliche Scheiben manuell
                             erfassen oder wieder löschen:
                             •   Eilscheiben erfassen.
                             •   Eilscheiben bearbeiten.
                             •   Eilscheiben löschen.
                             •   Bruchscheiben erfassen.
                             •   Bruchscheiben löschen.


                              Eilscheiben erfassen
                             1 Öffnen Sie dein Dialog Eilscheiben.
                               Wählen Sie dazu im Menü Erfassung > Eilscheiben. Im Dialog Eilscheiben
                               werden alle erfassten und noch nicht in einer Optimierung verwendeten Eil-
                               scheiben angezeigt.
                             2 Öffnen Sie den Dialog Eilscheibeneingabe. Betätigen Sie dazu die Schalt-
                               fläche [Hinzufügen].
                             3 Wählen Sie im Feld Glasart die Glasart, für die Sie Eilscheiben erfassen
                               wollen. Wenn für die Glasart mehrere Dicken möglich sind, dann geben Sie
                               im Feld Dicke die Dicke an, die Sie benötigen.
                             4 Geben Sie im Feld Bock ein, auf welchen Abstellplatz die Eilscheiben nach
                               dem Zuschnitt gestellt werden. Je nach Arbeitsorganisation kann dieses
                               Feld auch leer bleiben.
                             5 Geben Sie im Feld Menge ein, wieviele Scheiben Sie erfassen wollen.
                             6 Wählen Sie im Feld Modell-Nr. die entsprechende Nummer, wenn Sie Mo-
                               dellscheiben erfassen wollen.
                                 Wenn Sie Modellscheiben erfassen wollen, können Sie die Form der Mo-
                                 dellscheiben bearbeiten. Betätigen Sie dazu die Schaltfläche [^]. Es ist
                                 auch möglich für Eilscheiben eine freie Form zu hinterlegen. Geben Sie
                                 dazu die Modelnummer 99 ein. Wählen Sie anschließend aus dem Kata-
                                 log-Verzeichnis die entsprechende SN-Datei aus (diese muss vorher sepa-
                                 rat via CAD Designer Shapes erfasst und als Block-Ind-Datei exportiert
                                 worden sein).
                             7 Geben Sie in den Feldern Breite und Höhe die Maße der Scheiben ein, die
                               Sie erfassen wollen.
                                 Wenn Sie eine Modellscheibe erfasst haben, dann werden in diesen Fel-
                                 dern automatisch die Maße des umschreibenden Rechtecks angezeigt.
                             8 Speichern Sie die Eilscheibeneingabe. Betätigen Sie dazu die Schaltfläche
                               [OK].
3.30 / 01-2023




                                 Die erfassten Daten werden gespeichert und in der Liste angezeigt.




                 J-22                                                           A+W Realtime Optimizer
                 Tutorial                                                                                    Erfassung




                                          9 Erfassen Sie weitere Scheiben oder schließen Sie den Dialog.
                                             Um weitere Scheiben zu erfassen, wiederholen Sie die Arbeitsschritte ab
                                             Schritt 2.
                                             Um den Dialog zu schließen, betätigen Sie die Schaltfläche [Beenden].


                                           Eilscheiben bearbeiten
                                          1 Öffnen Sie den Dialog Eilscheiben-Eingabe.
                                            Wählen Sie dazu im Menü Erfassung > Eilscheiben. Im Dialog Eilscheiben
                                            werden alle erfassten und noch nicht in einer Optimierung verwendeten Eil-
                                            scheiben angezeigt.
                                          2 Markieren Sie die Zeile in der Liste der Eilscheiben, die Sie bearbeiten
                                            möchten.
                                          3 Betätigen Sie die Schaltfläche [Bearbeiten]. Es öffnet sich der Dialog Eil-
                                            scheiben-Eingabe. Die Felder enthalten die Werte der Eilscheibe, die Sie
                                            ändern möchten.
                                          4 Nehmen Sie die Änderungen vor und verlassen Sie den Dialog mit der
                                            Schaltfläche [OK].


                                           Eilscheiben löschen
                                          1 Öffnen Sie den Dialog Eilscheiben-Eingabe.
                                            Wählen Sie dazu im Menü Erfassung > Eilscheiben. Im Dialog Eilscheiben
                                            werden alle erfassten und noch nicht in einer Optimierung verwendeten Eil-
                                            scheiben angezeigt.
                                          2 Markieren Sie eine Zeile in der Liste der Eilscheiben.
                                          3 Betätigen Sie die Schaltfläche [Löschen].
                                             Die markierte Eilscheibe wird gelöscht.
                                          4 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].


                                           Bruchscheiben erfassen
                                             Wenn Sie am Zuschnitttisch mit A+W Production Terminal (XTV) arbeiten,
                                             dann kann Bruch direkt am Tisch erfasst werden und wird automatisch an
                                             A+W Realtime Optimizer übertragen. Bruch kann aber auch manuell er-
                                             fasst werden:
                                          1 Öffnen Sie den Dialog Brucherfassung.
                                            Wählen Sie dazu im Menü Zuschnitt > Bruchpool > [Hinzufügen].
                                          2 Geben Sie im Bereich Teile-ID die Auftragsnummer, Positionsnummer und
                                            Unterpositionsnummer an, zu der die zu Bruch gegangenen Scheiben ge-
                                            hören.
                                          3 Wenn Sie mit der BDE arbeiten, können Sie einen Bruchgrund angeben.
                                            Wählen Sie dazu den entsprechenden Eintrag in der Kombobox Bruch-
3.30 / 01-2023




                                            grund.
                                          4 Speichern Sie die Eingaben. Betätigen Sie dazu die Schaltfläche [Spei-
                                            chern].


                 A+W Realtime Optimizer                                                                           J-23
                 Erfassung                                                                            Tutorial




                              Bruchscheiben löschen
                             1 Öffnen Sie dein Dialog Bruchpool.
                               Wählen Sie dazu im Menü Zuschnitt > Bruchpool. Im Dialog Bruchpool
                               werden alle erfassten und noch nicht in einer Optimierung verwendeten
                               Bruchscheiben angezeigt.
                             2 Markieren Sie eine oder mehrere Zeilen in der Liste der Bruchscheiben.
                             3 Betätigen Sie die Schaltfläche [Löschen].
                                Die markierten Bruchscheiben werden gelöscht.
                             4 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [Schließen].

                                Bruchscheiben buchen
                                Über die Schaltfläche [Buchen F5] werden die Bruchscheiben wieder der
                                Produktion zugeführt. Haben Sie versehentlich Scheiben zu Bruch gemel-
                                det, können Sie diese ebenfalls über die Schaltfläche als Gut melden.


                             Ergänzende Informationen
                              Softwarereferenz, “Modell-Erfassung” auf Seite J-143
                              Softwarereferenz, “Eilscheiben” auf Seite J-90
                              Softwarereferenz, “Bruchpool” auf Seite J-138
                              Softwarereferenz, “Brucherfassung” auf Seite J-141
3.30 / 01-2023




                 J-24                                                                 A+W Realtime Optimizer
                 Tutorial                                                                                     Erfassung




                                          Manuelle Planerstellung
                                          Mit dieser Option haben Sie die Möglichkeit, einen rein manuellen Plan zu er-
                                          stellen und als Tischoptimierung in der Datenbank zu speichern. Der manuelle
                                          Plan kann nach der Erstellung erneut editiert und geändert werden. Dies ge-
                                          schieht mithilfe des Moduls A+W PlanEditor. Nähere Erläuterungen zu diesem
                                          Modul finden Sie in der entsprechenden Dokumentation. Es ist keine Barcode-
                                          information für den manuellen Plan verfügbar.


                                           So erstellen Sie einen neuen Plan
                                          1 Wählen Sie dazu im Menü Eingabe > Manueller Plan. Es öffnet sich der Di-
                                            alog Manuelle Planerstellung für Tisch ….
                                          2 Wählen Sie im Bereich Glasarten die Glasart aus, für die Sie einen neuen
                                            Plan erstellen möchten.
                                          3 Wählen Sie auf der linken Seite im Bereich Lagerplatten das Lagermaß
                                            aus, welches für das manuelle Schnittbild als Grundlage verwendet wer-
                                            den soll.
                                          4 Definieren Sie ggf. im Bereich Restplatten die Höhe und Breite, welche als
                                            Restplatte angelegt werden soll.
                                          5 Klicken Sie auf die Symbol-Schaltfläche [Neu]. Es öffnet sich der A+W Pla-
                                            nEditor.
                                          6 Über das Kontext-Menü können Sie nun die gewünschten Scheiben erfas-
                                            sen. Wählen Sie dazu die Option Einfügen und erfassen Sie anschließend
                                            die gewünschten Scheibendaten.
                                          7 Über Datei > Speichern unter, können Sie den Scheidplan als Datei spei-
                                            chern.
                                          8 Mittels Ausgabe > AWC erfolgt die Übergabe an den Zuschnitt.


                                           So editieren Sie einen manuellen Plan
                                          1 Um einen manuell erfassten Schneidplan zu ändern, wählen Sie im Menü
                                            Eingabe > Manuellen Plan. Es öffnet sich der Dialog Manuelle Planerstel-
                                            lung für Tisch …. Im unteren Bereich Plan erscheint der im Vorfeld manuell
                                            erfasste Plan.
                                          2 Mittels der Schaltfläche [Editieren] öffnen Sie den vorher erstellten Plan
                                            und können diesen editieren.
                                          3 Vergessen Sie nicht, die Änderungen zu speichern oder mittels Ausgabe >
                                            AWC die Daten zum Scheiden freizugeben.


                                           So wählen Sie einen manuell erfassten Plan zum Zuschnitt aus
                                          1 Einen manuell erfassten Plan können Sie nur via Zuschnitt direkt zuschnei-
                                            den.
                                          2 Über die Schaltfläche [Schneiden] können Sie alle optimierten und für den
3.30 / 01-2023




                                            Zuschnitt vorbereiteten Läufe auswählen.




                 A+W Realtime Optimizer                                                                            J-25
                 Erfassung                                                                          Tutorial




                             3 Der manuell erstellte Plan erscheint in der Liste der verfügbaren Läufe mit
                               einer Laufnummer >15000 und hat die Zusatzinformation PlanEdit.
                             4 Wählen Sie den Lauf aus und bereiten Sie ihn für den Zuschnitt vor (Schalt-
                               fläche [Optionen]) oder schneiden Sie ihn direkt (Schaltfläche [Zuschnitt]).


                             Ergänzende Informationen
                              Softwarereferenz, “Manuelle Planerstellung” auf Seite J-97


                             Chargen-Editor
                             Über diesen Dialog haben Sie die Möglichkeit, eine Chargen-Nummer zu hin-
                             terlegen. Mit Hilfe der aktivierten Checkbox können Sie die eingegebene
                             Chargen Nummer auf die nachfolgenden Lagerplatten der gleichen Glasart/
                             Dicke vererben. Die letzte Chargen Nummer wird pro Glasart/Dicke/Lagerplat-
                             te gespeichert. Mit diesem Wert wird bei dem nächsten Aufruf des Editors das
                             Eingabefeld wieder vorbelegt. Die Zuweisung wirkt immer auf das ausgewähl-
                             te Lagermaß (und bei Vererbung auf die darunterliegenden).
                             Es ist auch möglich, über diesen Editor eine gesetze Charge wieder zu lö-
                             schen (inklusive Vererbung).
                             Läuft der Zuschnittsprozess auf eine Lagerplatte ohne Chargenzuordnung, so
                             muss der Mitarbeiter am Brechtisch zunächst eine Chargen-Nummer einge-
                             ben. Hierzu erscheint wieder der Dialog Chargen-Editor mit einer entspre-
                             chenden Info im A+W Production Terminal (XTV). Die eingegebene Chargen
                             Nummer wird beim Weiterschalten des A+W Production Terminal (XTV) für
                             alle Scheiben des jeweiligen Lagerblattes verbucht.


                             Ergänzende Informationen
                              Softwarereferenz, “Chargen-Editor” auf Seite J-100
3.30 / 01-2023




                 J-26                                                               A+W Realtime Optimizer
                 Tutorial                                                                                Optimierung




                                          Optimierung
                                          In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit der Optimierung umgehen.
                                          Der Themenblock beinhaltet folgende Schulungseinheiten:
                                          •   Tischoptimierungen
                                          •   Schnelloptimierung erstellen
                                          •   Verlinken von Läufen
                                          •   Tischansteuerung
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-27
                 Optimierung                                                                               Tutorial




                               Überblick
                               Lernziele

                               •   Tischoptimierungen kennenlernen und verstehen.
                               •   Schnelloptimierungen kennenlernen und verstehen.
                               •   Das Verlinken von Restplatten kennenlernen und verstehen.
                               •   Tischansteuerung kennenlernen und verstehen.


                               Nutzen

                               Je effizienter die Optimierung arbeiten kann, umso höher ist die Ausbeute. Das spart
                               Geld.


                               Definitionen

                               Tischoptimierungen          Sind Optimierungen, die mit A+W Realtime Optimizer
                                                           erzeugt werden.

                               Schnelloptimierung          Platten, die noch nicht an den Tisch gesandt wurden,
                                                           können komplett aufgelöst und neu optimiert werden.


                               Merke

                               Lauf                        Ein Lauf ist eine Zusammenstellungen von Gläsern aus
                                                           einem oder mehreren Aufträgen, welche in der
                                                           Optimierung und Produktion gemeinsam betrachtet und
                                                           produziert werden sollen (bspw. gleiche Tour, gleicher
                                                           Kunde, gleiche Glasarten, gleiche Produktionstermine).
                                                           Die Optimierungen von vorgelagerten Systemen liegen
                                                           in Form von Läufen vor.

                               Los                         Ein Teil / eine Glasart eines Laufes, welcher unter
                                                           gleichen Bedingungen zur gleichen Zeit in der
                                                           Produktion bearbeitet / geschnitten werden soll (bspw.
                                                           alles Float 4 eines Laufes).

                               Tischansteuerung            Bei der Installation wird festgelegt, welcher
                                                           Zuschnitttisch mit einem A+W Realtime Optimizer
                                                           angesteuert werden.

                               Bruchscheiben               Können entweder in der Nachoptimierung am Ende
                                                           eines zu schneidenden Laufes geschnitten werden oder
                                                           landen im Bruchpool und können zusammen mit dem
                                                           nächsten Lauf geschnitten werden.
3.30 / 01-2023




                 J-28                                                                  A+W Realtime Optimizer
                 Tutorial                                                                                    Optimierung




                                          Tischoptimierungen
                                          Tischoptimierungen sind Optimierungen, die mit A+W Realtime Optimizer er-
                                          zeugt werden. Vorgelagerte Systeme liefern bereits fertige Optimierungen, die
                                          mit A+W Realtime Optimizer aufgelöst und neu zusammengestellt werden
                                          können. Dabei können so viele Läufe zusammengefasst werden, wie Platz für
                                          die benötigten Abstellplätze am Zuschnitttisch in einer Produktion vorhanden
                                          ist.
                                          Bei der Erstellung von Tischoptimierungen können Sie Restblätter auf dem
                                          Zuschnitttisch berücksichtigen, unterschiedliche Lagerplatten verwenden
                                          oder ein Restelager nutzen. Bruch, Eilscheiben oder Füllaufträge können aus-
                                          geschlossen oder mit einbezogen werden.
                                          Erstellte Tischoptimierungen werden in der Datenbank abgespeichert und bei
                                          Bedarf zum Zuschnitt aufgerufen.


                                          Tischoptimierungen erstellen
                                          Zum Erstellen neuer Tischoptimierungen müssen folgende Arbeitsschritte
                                          durchgeführt werden:
                                          •   Glasart und Lauf für eine Tischoptimierung auswählen.
                                          •   Tischoptimierung erstellen.


                                           Glasart und Lauf für eine Tischoptimierung auswählen
                                          1 Öffnen Sie den Dialog Selektieren Sie die zu optimierenden Gläser.
                                            Wählen Sie dazu Optimierung > Tischoptimierung.
                                          2 Wählen Sie in der Liste Glasart die Glasart aus, für die Sie eine Optimie-
                                            rung erstellen wollen. In der Liste Glasart wird ihnen angezeigt, ob für eine
                                            Glasart im A+W Realtime Optimizer besondere Aufträge (Bruchscheiben,
                                            Eilscheiben, etc.) existieren.
                                              Wenn Sie eine Glasart wählen, für die Bruchscheiben oder Eilaufträge
                                              existieren, so werden diese Bruchscheiben oder Eilaufträge automatisch
                                              (wenn konfiguriert) in die zu erstellende Tischoptimierung integriert.
                                              Wenn Ihr System für die Zusammenarbeit mit einem Restelager-Magazin
                                              konfiguriert wurde, dann wird in dieser Liste angezeigt, ob für die entspre-
                                              chende Glasart ein Restplatte verfügbar ist.
                                              In der Liste Verfügbare Optimierungen werden alle Läufe angezeigt, in de-
                                              nen Optimierungen für die in der Liste Glasart gewählte Glasart und Dicke
                                              enthalten sind.
                                          3 Markieren Sie die Checkbox Erlaube Handzuschnitt, wenn Sie auch die
                                            Glasarten anzeigen wollen, die nur für den Handzuschnitt vorgesehen
                                            sind.
                                          4 Wählen Sie in der Liste Verfügbare Optimierungen die Läufe aus, die Sie
                                            zu einer Tischoptimierung zusammenfassen wollen.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-29
                 Optimierung                                                                             Tutorial




                                  Nur Bruch- und Eilscheiben auswählen
                                  Wenn für die gewählte Glasart Bruch- oder Eilscheiben vorhanden sind,
                                  dann können Sie diese Scheiben ohne einen weiteren Lauf optimieren.
                                  Wählen Sie in diesem Fall keinen Lauf aus der Liste aus.

                                  Wenn sie einen Lauf markiert haben, aber keinen Lauf wählen wollen,
                                  dann wechseln Sie die gewählte Glasart. Bei erneuter Auswahl der ge-
                                  wünschten Glasart ist kein Lauf markiert.
                               5 Klicken Sie auf [Auswählen], wenn Sie die ausgewählten Läufe zu einer
                                 Tischoptimierung zusammenstellen wollen.
                                  Der Dialog wird geschlossen. Der Dialog Tischoptimierung öffnet sich mit
                                  dem Register Optimieren und zeigt die gewählten Läufe an.


                                Tischoptimierung erstellen
                               1 Stellen Sie sicher, dass mit dem vorherigen Arbeitsschritt So wählen Sie
                                 Läufe für eine Tischoptimierung aus Läufe für die Tischoptimierung ausge-
                                 wählt wurden.
                                  Der Dialog Tischoptimierung wird mit dem Register Optimieren angezeigt.
                               2 Wählen Sie die erforderlichen Optimierungsparameter.
                               3 Wählen Sie die erforderlichen Parameter im Register Lagerplatten.
                               4 Wählen Sie die erforderlichen Parameter im Register Füller.
                               5 Um die Optimierung zu erstellen, wechseln Sie wieder in das Register Op-
                                 timieren und betätigen Sie die Schaltfläche [Optimieren].
                                  Die Berechnung der Optimierung startet, der Dialog wird ausgeblendet und
                                  die Berechnung läuft im Hintergrund. So lange die Berechnung läuft, kön-
                                  nen Sie weitere Arbeiten mit A+W Realtime Optimizer durchführen.
                                  Sobald das Ergebnis der Optimierung vorliegt, wird der Dialog automatisch
                                  wieder eingeblendet. Das Optimierungsergebnis wird im Register Über-
                                  sicht angezeigt.
                               6 Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Spei-
                                 chern].
                                  Die Optimierung steht jetzt im Dialog Wählen Sie einen Lauf aus zur Aus-
                                  wahl bereit und kann an den Schneidtisch übertragen werden.


                               Ergänzende Informationen
                                Softwarereferenz, “Selektieren Sie die zu optimierenden Gläser” auf Seite J-103
                                Softwarereferenz, “Optimieren” auf Seite J-110
                                Softwarereferenz, “Restplatten und Lagerplatten” auf Seite J-113
                                “Läufe zum Zuschnitt auswählen” auf Seite J-40
3.30 / 01-2023




                 J-30                                                                 A+W Realtime Optimizer
                 Tutorial                                                                                  Optimierung




                                          Ergebnis der Tischoptimierung prüfen und bearbei-
                                          ten
                                          Tischoptimierungen, die noch nicht zum Schneidtisch übertragen wurden,
                                          können jederzeit geprüft werden. Sollen Tischoptimierungen geändert oder
                                          um Bruch-, Eil- oder Füllscheiben ergänzt werden oder sollen ganze Läufe zu-
                                          gefügt oder daraus gelöscht werden, so muss die gesamte Optimierung auf-
                                          gelöst und neu erstellt werden.
                                          Folgende Arbeitsschritte können beim Erstellen einer Tischoptimierung durch-
                                          geführt werden:
                                          •   Andere Lagerplatten für die Optimierung wählen.
                                          •   Restblatt der vorherigen Optimierung verwenden.
                                          •   Füllaufträge zur Optimierung zufügen.
                                          Sobald eine Tischoptimierung gespeichert wurde, können keine Änderungen
                                          mehr durchgeführt werden.


                                           Andere Lagerplatten für die Optimierung wählen
                                          1 Wählen Sie im Dialog Tischoptimierung das Register Lagerplatten.
                                              In der rechten Liste werden alle Lagerplatten angezeigt, die in den Stamm-
                                              daten für die Glasart und Dicke des Laufes definiert wurden und dem
                                              Schneidtisch zur Verfügung stehen.
                                          2 Markieren Sie die Lagerplatten, die A+W Realtime Optimizer für die Zu-
                                            schnittoptimierung verwenden kann.
                                              Während der Optimierung prüft A+W Realtime Optimizer, mit wievielen
                                              Platten welcher Größe das beste Optimierungsergebnis erzielt wird.
                                          3 Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren
                                            und betätigen Sie die Schaltfläche [Start].
                                          4 Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Spei-
                                            chern].


                                           Restblatt der vorherigen Optimierung verwenden
                                          1 Wählen Sie im Dialog Tischoptimierung das Register Lagerplatten.
                                              Wenn auf dem Schneidtisch noch ein Restblatt der gleichen Glasart und
                                              Dicke liegt, wie in der angezeigten Optimierung, dann können Sie dieses
                                              Restblatt in die Tischoptimierung integrieren.
                                          2 Geben Sie die Höhe und Breite des Restblatts auf dem Schneidtisch im Be-
                                            reich Restblatt ein.
                                          3 Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren
                                            und betätigen Sie die Schaltfläche [Start].
                                          4 Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Spei-
                                            chern].
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-31
                 Optimierung                                                                            Tutorial




                                Füllaufträge zur Optimierung zufügen
                               1 Wählen Sie im Dialog Tischoptimierung das Register Füller.
                                  In der rechten Liste werden alle Füllaufträge angezeigt, die für die Glasart
                                  des Laufes definiert wurden.
                               2 Markieren Sie die Füllaufträge, die Sie in die Tischoptimierung integrieren
                                 wollen.
                                  Idealer Weise werden Füllaufträge so verwendet, dass möglichst geringer
                                  Verschnitt oder Restblätter entstehen.
                               3 Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren
                                 und betätigen Sie die Schaltfläche [Optimieren].
                               4 Wiederholen Sie das Zufügen oder Entfernen von Füllaufträgen so lange,
                                 bis das für Sie optimale Ergebnis ermittelt wurde.
                               5 Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Spei-
                                 chern].


                               Ergänzende Informationen
                                “Tischoptimierung auflösen” auf Seite J-32


                               Tischoptimierung auflösen
                               Tischoptimierungen können nur dann aufgelöst werden, wenn sie nach dem
                               Erstellen gespeichert wurden. Solange der Dialog Tischoptimierung noch mit
                               einer Tischoptimierung geöffnet ist, und diese Optimierung nicht gespeichert
                               wurde, kann die Optimierung durch betätigen der Schaltfläche Abbrechen ver-
                               worfen werden.
                               Wenn Sie eine Tischoptimierung auflösen, dann werden die enthaltenen Läufe
                               wieder in die Laufliste gestellt. Evtl. enthaltene Bruch-, Eil- oder Füllscheiben
                               stehen in den entsprechenden Pools (Sammelbehälter) für neue Optimierun-
                               gen wieder zur Verfügung.
                               Optimierungen, deren Zuschnitt bereits begonnen und dann abgebrochen
                               wurde, können ebenfalls aufgelöst werden. Läufe, bei denen bereits Scheiben
                               geschnittenen wurden, werden zurückgesetzt und so behandelt, als ob noch
                               kein Zuschnitt erfolgt wäre.


                                Erstellte und gespeicherte Tischoptimierungen auflösen
                               1 Öffnen Sie den Dialog Zurücksetzen eines Zuschnitt Laufes.
                                 Wählen Sie dazu im Menü Optimierung > Zurücksetzen.
                                  Im Dialog Zurücksetzen eines Zuschnitt Laufes wird eine Liste aller Läufe
                                  angezeigt, für die Sie Statusänderungen vornehmen können. Die Liste er-
                                  scheint nach Laufnummern sortiert. Tischoptimierungen werden als Lauf
                                  im Nummernbereich ab 15000 (konfigurierbar) angezeigt.
3.30 / 01-2023




                 J-32                                                                A+W Realtime Optimizer
                 Tutorial                                                                               Optimierung




                                          2 Wählen Sie die Tischoptimierung, die Sie auflösen wollen.
                                            Markieren Sie dazu im Nummernbereich ab 15000 den entsprechenden
                                            Lauf.
                                             Sie können mehrere Tischoptimierungen markieren und gleichzeitig auflö-
                                             sen.
                                          3 Um die Tischoptimierung aufzulösen, betätigen Sie die Schaltfläche [OK].
                                            Es erscheint eine Sicherheitsabfrage.
                                          4 Bestätigen Sie die Sicherheitsabfrage. Wählen Sie dazu die Schaltfläche
                                            [Ja].
                                             Die Läufe und Scheiben der gewählten Tischoptimierung stehen wieder für
                                             neue Tischoptimierungen zur Verfügung. Wurden in der Tischoptimierung
                                             Remasterplatten verwendet, so stehen diese nach der Auflösung der Opti-
                                             mierung wieder zur Verfügung.


                                          Ergänzende Informationen
                                           “Tischoptimierungen erstellen” auf Seite J-29
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                        J-33
                 Optimierung                                                                           Tutorial




                               Tischoptimierungen verlinken
                               Zur Verbesserung des Verschnitts haben Sie die Möglichkeit, Tischoptimierun-
                               gen miteinander zu verlinken. Sie können nur Tischoptimierungen der glei-
                               chen Glasart miteinander verlinken. D. h., die Tischoptimierungen müssen
                               vorhanden sein.
                               Zum Verlinken von Tischoptimierungen müssen folgende Arbeitsschritte
                               durchgeführt werden:
                               •   Glasart und Lauf für eine Tischoptimierung auswählen.
                               •   Tischoptimierung erstellen.


                                Tischoptimierungen verlinken
                               1 Öffnen Sie den Dialog Selektieren Sie die zu optimierenden Gläser.
                                 Wählen Sie dazu Optimierung > Tischoptimierung.
                               2 Wählen Sie in der Liste Glasart die Glasart aus, für die Sie eine Optimie-
                                 rung erstellen wollen. In der Liste Glasart wird ihnen angezeigt, ob für eine
                                 Glasart im A+W Realtime Optimizer besondere Aufträge (Bruchscheiben,
                                 Eilscheiben, etc.) existieren.
                                   Wenn Sie eine Glasart wählen, für die Bruchscheiben oder Eilaufträge
                                   existieren, so werden diese Bruchscheiben oder Eilaufträge automatisch
                                   (wenn konfiguriert) in die zu erstellende Tischoptimierung integriert.
                                   Wenn Ihr System für die Zusammenarbeit mit einem Restelager-Magazin
                                   konfiguriert wurde, dann wird in dieser Liste angezeigt, ob für die entspre-
                                   chende Glasart ein Restplatte verfügbar ist.
                                   In der Liste Verfügbare Optimierungen werden alle Läufe angezeigt, in de-
                                   nen Optimierungen für die in der Liste Glasart gewählte Glasart und Dicke
                                   enthalten sind.
                               3 Markieren Sie die Checkbox Erlaube Handzuschnitt, wenn Sie auch die
                                 Glasarten anzeigen wollen, die nur für den Handzuschnitt vorgesehen
                                 sind.
                               4 Wählen Sie in der Liste Verfügbare Optimierungen die Läufe aus, die Sie
                                 zu einer Tischoptimierung zusammenfassen wollen.


                               Ergänzende Informationen
                                “Tischoptimierungen verlinken” auf Seite J-34
3.30 / 01-2023




                 J-34                                                               A+W Realtime Optimizer
                 Tutorial                                                                                  Optimierung




                                          Schnelloptimierung erstellen
                                          Bereits optimierte Platten / Muster (durch A+W Production oder via Tischopti-
                                          mierung in A+W Realtime Optimizer), welche aber noch nicht an den Tisch ge-
                                          sandt wurden, können komplett aufgelöst und neu optimiert werden. Dadurch
                                          werden beispielsweise Eilscheiben oder Bruchscheiben mit hinein-optimiert
                                          und es entsteht ein komplett neues Schnittmuster für die neu optimierten Plat-
                                          ten.
                                          Zum Erstellen einer Schnelloptimierung müssen folgende Arbeitsschritte
                                          durchgeführt werden:
                                          •   Tischoptimierung erstellen.
                                          •   Tischoptimierung wurde begonnen zu schneiden.
                                          Entsteht beim Zuschnitt Bruch, kann dieser zeitnah und bequem über die so-
                                          genannte Schnelloptimierung nachgeschnitten werden.




                 Abb. J-5   Zuschnitt-Übersicht


                                          Über das Kontextmenü können Sie die Optimierung ab dem nächst möglichen
                                          Muster auflösen und neu optimieren.
                                          Im Beispiel Abb. J-5 (Zuschnitt-Übersicht) wurden die Muster / Platten 1 und
                                          2 an den Tisch gesandt und geschnitten. Die Platten / Muster 3-6 können mit-
                                          tels Rechtsklick aufgelöst und neu optimiert werden (Schnell-Optimierung).
3.30 / 01-2023




                                          Abb. J-6     Kontextmenü




                 A+W Realtime Optimizer                                                                           J-35
                 Optimierung                                                                            Tutorial




                               Nachdem die Meldung bestätigt wurde, werden die noch zu schneidenden
                               Platten zunächst entfernt. Im Anschluss werden die zu Bruch gegangenen
                               Scheiben inklusive der noch zu schneidenden Platten neu optimiert.


                               Ergänzende Informationen
                                “Die Zuschnitt-Übersicht” auf Seite J-46



                               Verlinken von Läufen
                               Mit dem Verlinken von Läufen hat A+W die Möglichkeit geschafften, Restplat-
                               ten zu vermeiden. In der Vergangenheit mussten solche Restplatten manuell
                               zusammengelegt werden. Dies ist jetzt nicht mehr notwendig.
                               Das Verlinken findet während des Zuschnittprozesses statt und wird mit die-
                               sem synchronisiert.
                               Im Dialog Lauf: # kann im Bereich Restblatt-Verwaltung die Option zum Ver-
                               linken von Läufen aktiviert werden.
                               Nachdem der Zuschnitt gestartet wurde, wird nach dem Senden des 1. Mus-
                               ters eines Loses, das geschnitten wird, in der Datenbank beginnend mit dem
                               Folgelauf nach einem passenden Los dieser Glasart für diesen Tisch gesucht
                               und die entsprechenden Daten geladen.
                               Das Folgelos muss den Status Freigegeben besitzen. Das Laden geschieht im
                               Hintergrund, damit der Zuschnitt am Tisch weiterlaufen kann. Ist das vorletzte
                               Blatt (konfigurierbar) einer Glasart geschnitten, erhält der Benutzer optional
                               eine Abfrage, mit welchem Lauf und Los das Restblatt verlinkt werden soll.
                               Der Benutzer hat dann die Möglichkeit, das Verlinken abzubrechen oder eben
                               ein entsprechendes Los auszuwählen.
                               Wird das Verlinken bestätigt, werden Bruch- und Eilscheiben dieser Glasart
                               geladen und mit der Priorität 0 zu der Folgeoptimierung hinzugefügt. Das
                               Restblatt des zur Zeit geschnittenen Loses wird zu der Folgeoptimierung als
                               Startblatt hinzugefügt. Anschließend wird die Optimierung gestartet. Nach
                               dem Optimieren wird die Folgeoptimierung mit der Ursprungsoptimierung ver-
                               bunden, so dass das Restblatt der Ursprungsoptimierung mit den Scheiben
                               des 1. Blatts der Folgeoptimierung aufgefüllt wird. Alle weiteren Muster der
                               Folgeoptimierung werden in der gerade geschnittenen Optimierung aufgelöst.
                               Anschließend wird neuer Schneidcode erstellt und übertragen.
                               Das 1. Muster der Folgeoptimierung wird als Geschnitten markiert. Die Folge-
                               optimierung wird mit dem vorhandenen Mechanismus aus der Tischoptimie-
                               rung zunächst als Tischoptimierung abgespeichert und dann mit der Lauf- und
                               Losnummer der ursprünglichen Folgeoptimierung versehen. Der Status der
                               Folgeoptimierung wird auf Begonnen gesetzt.


                               Ergänzende Informationen
                                Softwarereferenz, “Auswahl der zu verlinkenden Optimierung” auf Seite J-136
3.30 / 01-2023




                 J-36                                                                A+W Realtime Optimizer
                 Tutorial                                                                                   Optimierung




                                          Tischansteuerung
                                          A+W Realtime Optimizer arbeitet als Leitstand für einen Zuschnitttisch.

                                             Parameter des angeschlossenen Tischs
                                             Bei der Installation wird festgelegt, welche Zuschnitttische mit einem A+W
                                             Realtime Optimizer angesteuert werden. Entsprechend werden die Para-
                                             meter bei der Installation hinterlegt. Die Optimierungen werden mit den ein-
                                             gestellten Parametern von A+W Production oder A+W Realtime Optimizer
                                             erstellt.

                                          Bei der Tischansteuerung wird Schneidcode generiert und für die Ansteue-
                                          rung des Zuschnitttischs seriell an den Tisch übertragen oder in einem verein-
                                          barten Verzeichnis bereitgestellt. Je nach angeschlossenem Tisch und
                                          technischer Lösung zur Tischansteuerung wird der Schneidcode mit einem
                                          weiteren Programm an den Tisch übertragen oder von der Software des Tisch-
                                          herstellers aus dem vereinbarten Verzeichnis abgerufen.


                                          A+W Realtime Optimizer
                                           Schneidcodegenerierung
                                              Nachoptimierung
                                              Statusverwaltung
                                                                            Zuschnitttisch




                                                 Production
                                                 -Datenbank
                                                 Optimierung


                                          Abb. J-7     Datenerfassung und -verarbeitung in A+W Realtime Optimizer


                                          Sobald der Schneidcode für eine Lagerplatte an den Tisch geschickt wurde,
                                          behandelt A+W Realtime Optimizer die Lagerplatte als abgearbeitet. Wird die
                                          Übertragung von Schneidcode für mehrere Platten eines Laufes unterbro-
                                          chen, so kann die Arbeit an dieser Stelle wieder fortgesetzt werden.
                                          In Zusammenarbeit mit XTV wird Bruch am Tisch direkt an A+W Realtime Op-
                                          timizer zurückgemeldet. Ist der Schneidcode der letzten Lagerplatte einer
                                          Glasart (eines Loses) noch nicht an den Zuschnitttisch übertragen, so kann
                                          der Bruch automatisch nachoptimiert und mit der letzten Lagerplatte des Lo-
                                          ses zugeschnitten werden.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-37
                 Zuschnitt                                                                      Tutorial




                             Zuschnitt
                             In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit dem Zuschnitt umgehen.
                             Der Themenblock beinhaltet folgende Schulungseinheiten:
                             •   Läufe zum Zuschnitt auswählen
                             •   Optimierung prüfen und schneiden
                             •   Arbeit unterbrechen und fortsetzen
                             •   Die Zuschnitt-Übersicht
3.30 / 01-2023




                 J-38                                                         A+W Realtime Optimizer
                 Tutorial                                                                                         Zuschnitt




                                          Überblick
                                          Lernziele

                                          • Die Abläufe im Zuschnitt kennenlernen und verstehen.


                                          Nutzen

                                          Das Arbeiten mit dem A+W Realtime Optimizer ist nur dann sinnvoll möglich, wenn
                                          Sie die Abläufe kennen.


                                          Definition

                                          Panorama                   Konfigurierbarer Programmteil für die Ansteuerung von
                                                                     komplexen Maschinen oder Maschinenverbünden
                                                                     (Schneidanlagen).


                                          Merke

                                          Laufnummer 1000-9999       Stammen aus einem vorgelagerten System.

                                          Laufnummer ab 15000        Diese Läufe enthalten Tischoptimierungen, die mit dem
                                                                     A+W Realtime Optimizer erstellt wurden. Der
                                                                     Nummernkreis ist konfigurierbar.

                                          Panorama                   Die Administration im Panorama ist passwort-geschützt.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                               J-39
                 Zuschnitt                                                                        Tutorial




                             Läufe zum Zuschnitt auswählen
                             Die Optimierungen liegen in Form von Läufen vor. Wählen Sie die Läufe aus,
                             in denen die Optimierungen enthalten sind, die Sie auf dem Schneidtisch zu-
                             schneiden wollen.


                              Läufe zum Zuschnitt auswählen
                             1 Öffnen Sie den Dialog Wählen Sie einen Lauf aus.
                               Wählen Sie dazu im Menü Zuschnitt > Schneide Optimierung.
                             2 Wählen Sie einen Lauf aus. Markieren Sie dazu in der Liste Läufe einen
                               Eintrag. In der Liste Optimierungen werden die Optimierungen angezeigt,
                               die für diesen Lauf existieren.

                                Nummern der Läufe
                                Läufe mit den Nummern 1000-9999 stammen aus einem vorgelagerten
                                System und enthalten eine oder mehrere Optimierungen. Läufe ab Num-
                                mer 15000 enthalten Tischoptimierungen, die mit A+W Realtime Optimizer
                                erstellt wurden.

                             3 Wählen Sie eine oder alle Optimierungen aus. Wenn keine Optimierung
                               markiert wird, gelten alle Optimierungen als ausgewählt. Es kann konfigu-
                               riert werden, ob einzelne Optimierungen gewählt werden dürfen.

                                Nummern der Optimierungen
                                Die Optimierungen sind Losweise (je Glasart) angelegt und je Lauf fortlau-
                                fend durchnummeriert.

                             4 Betätigen Sie [OK]. Die gewählten Optimierungen werden zum Zuschnitt
                               ausgewählt und im Dialog Lauf [Nummer -] - Lauf [Nummer] angezeigt.
                             5 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].
                             6 Starten Sie den Zuschnitt. Betätigen Sie dazu die Schaltfläche [START].


                              Geschnittene Läufe erneut schneiden
                                Wenn alle Platten einer Optimierung geschnitten wurden, wird der ganze
                                Lauf in den Status Produziert gesetzt. Dieser Status kann in den Status
                                Freigegeben zurückgesetzt und der ganze Lauf erneut zugeschnitten wer-
                                den.
                             1 Öffnen Sie den Dialog Zurücksetzen eines Zuschnitt Laufes.
                               Wählen Sie dazu im Menü Optimierung > Zurücksetzen.
                                Im Dialog Zurücksetzen eines Zuschnitt Laufes wird eine Liste aller Läufe
                                angezeigt, für die Sie Statusänderungen vornehmen können. Die Liste er-
                                scheint nach Laufnummern sortiert. Vollständig geschnittene Läufe werden
                                mit dem Status Produziert angezeigt.
                             2 Wählen Sie die den Lauf, den Sie vom Status Produziert in den Status Frei-
3.30 / 01-2023




                               gegeben zurücksetzen wollen. Sie können mehrere Läufe markieren und
                               gleichzeitig zurücksetzen.




                 J-40                                                           A+W Realtime Optimizer
                 Tutorial                                                                                      Zuschnitt




                                          3 Um den Lauf zurückzusetzen, betätigen Sie die Schaltfläche [OK].
                                             Der Lauf steht als fertige Optimierung für einen erneuten Zuschnitt zur Ver-
                                             fügung.


                                           Muster überspringen
                                             Wenn Sie für eine Platte Muster überspringen wählen, dann wird für diese
                                             Platte kein Schneidcode erzeugt und kein Brechbild angezeigt.
                                          1 Öffnen Sie den Dialog Restblatt Behandlung.
                                            Betätigen Sie dazu die Schaltfläche [Optionen] im Dialog Lauf: [Nr.] - Lauf:
                                            [Nr.] des Laufes, den Sie bearbeiten wollen.
                                          2 Markieren Sie in der Liste Optimierungen die Glasart, von der einzelne La-
                                            gerplatten nochmals geschnitten werden sollen.
                                             In der Liste Platten werden alle zu der markierten Glasart gehörigen Plat-
                                             ten des Laufes angezeigt. In der Spalte Status sehen Sie den Status jeder
                                             einzelnen Lagerplatte.
                                             Sie können nur solche Platten überspringen, die nicht im Status Geschnit-
                                             ten sind.
                                          3 Klicken Sie mit der rechten Maustaste auf die Platte, die Sie beim Zuschnitt
                                            überspringen wollen.
                                             Es erscheint ein Kontext-Menü mit den Einträgen Muster überspringen und
                                             Kein Schneidcode senden.
                                          4 Wählen Sie Muster überspringen um für diese Platte keinen Schneidcode
                                            zu erzeugen und kein Brechbild anzuzeigen.
                                          5 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].


                                           Erzeugung von Schneidcode unterdrücken
                                             Wenn Sie für eine Platte Kein Schneidcode senden wählen, dann wird für
                                             diese Platte kein Schneidcode erzeugt aber in A+W Production Terminal
                                             (XTV) ein Brechbild angezeigt.
                                          1 Öffnen Sie den Dialog Restblatt Behandlung.
                                            Betätigen Sie dazu die Schaltfläche [Optionen] im Dialog Lauf: [Nr.] - Lauf:
                                            [Nr.] des Laufes, den Sie bearbeiten wollen.
                                          2 Markieren Sie in der Liste Optimierungen die Glasart, von der einzelne La-
                                            gerplatten nochmals geschnitten werden sollen.
                                             In der Liste Platten werden alle zu der markierten Glasart gehörigen Plat-
                                             ten des Laufes angezeigt. In der Spalte Status sehen Sie den Status jeder
                                             einzelnen Lagerplatte.
                                             Sie können nur bei solchen Platten keinen Schneidcode senden, die nicht
                                             im Status Geschnitten sind.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-41
                 Zuschnitt                                                                         Tutorial




                             3 Klicken Sie mit der rechten Maustaste auf die Platte, die Sie beim Zuschnitt
                               überspringen wollen.
                                Es erscheint ein Kontext-Menü mit den Einträgen Muster überspringen und
                                Kein Schneidcode senden.
                             4 Wählen Sie Kein Schneidcode senden um für diese Platte keinen Schneid-
                               code zu erzeugen, aber in A+W Production Terminal (XTV) ein Brechbild
                               anzuzeigen.
                             5 Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].


                             Ergänzende Informationen
                              Softwarereferenz, “Lauf: Nummer” auf Seite J-132
                              Softwarereferenz, “Wählen Sie einen Lauf aus” auf Seite J-125
3.30 / 01-2023




                 J-42                                                              A+W Realtime Optimizer
                 Tutorial                                                                                     Zuschnitt




                                          Optimierung prüfen und schneiden
                                          Wenn Sie Optimierungen zum Zuschnitt ausgewählt haben, können Sie einige
                                          Prüfungen vornehmen und dann die Optimierungen zum Schneidtisch über-
                                          tragen.
                                          Folgende Arbeitsschritte sind in diesem Kapitel erklärt:
                                          •   Vorgesehene Zuschnittreihenfolge anzeigen.
                                          •   Restblätter überprüfen.
                                          •   Zuschnittbeginn festlegen und Zuschnitt starten.
                                          Die nachfolgenden Beschreibungen setzen voraus, dass Sie den vorherigen
                                          Arbeitsschritt Läufe zum Zuschnitt auswählen durchgeführt haben und der Di-
                                          alog Lauf [Nummer] - Lauf [Nummer] angezeigt wird.


                                           Vorgesehene Zuschnittreihenfolge anzeigen
                                          1 Betätigen Sie die Schaltfläche [Reihenfolge].
                                            Der Dialog Zuschnittreihenfolge wird angezeigt.

                                              Reihenfolge bei mehreren Losen
                                              Wurden mehrere Lose zum Zuschnitt ausgewählt, so werden die Zuschnitt-
                                              platten so sortiert, wie das A+W Realtime Optimizer konfiguriert wurde. Z.
                                              B. können alle Restblätter am Ende des gesamten Laufes geschnitten wer-
                                              den oder jeweils am Ende einer Glasart. A+W Realtime Optimizer kann
                                              auch so konfiguriert werden, dass Lagerplatten alternierend (z. B.: be-
                                              schichtet - unbeschichtet) geschnitten werden.

                                          2 Betätigen Sie [OK], um den Dialog zu schließen.


                                           Restblätter überprüfen
                                          1 Betätigen Sie die Schaltfläche [Restblätter].
                                            Der Dialog Restblatt Behandlung wird angezeigt.
                                          2 Prüfen Sie die angezeigten Werte.
                                          3 Ändern Sie den Status für einzelne Platten oder die Einstellungen für den
                                            Umgang mit Bruchscheiben, falls erforderlich.
                                          4 Wenn an Ihrem Arbeitsplatz das Softwaremodul PlanEdit installiert ist,
                                            dann können Sie die durch Betätigen der Schaltfläche Muster bearbeiten
                                            das Schneidmuster für die markierte Platte anzeigen.
                                          5 Betätigen Sie [OK], um den Dialog zu schließen.


                                           Zuschnittbeginn festlegen und Zuschnitt starten
                                          1 Markieren Sie in der Liste Optimierungen das Los, ab dem der Zuschnitt
                                            erfolgen soll.
                                          2 Markieren Sie in der Liste Muster die Lagerplatte, ab der der Zuschnitt er-
3.30 / 01-2023




                                            folgen soll.




                 A+W Realtime Optimizer                                                                           J-43
                 Zuschnitt                                                                         Tutorial




                             3 Betätigen Sie die Schaltfläche [START].
                                Für die angezeigten Optimierungen wird der Schneidcode erzeugt und für
                                den angeschlossenen Schneidtisch bereitgestellt.
                                Die Beschriftung und Funktion der Schaltfläche ändert sich zu [STOP].
                                Wenn A+W Realtime Optimizer mit einem A+W Production Terminal (XTV)
                                zusammenarbeitet, dann kann die Brechbildanzeige des A+W Production
                                Terminal (XTV) jetzt mit den Tasten [Stopp] und [<<] gesteuert werden.


                             Ergänzende Informationen
                              Softwarereferenz, “Lauf: Nummer” auf Seite J-132
                              Softwarereferenz, “Lauf [Nummer] - Lauf [Nummer]” auf Seite J-129
3.30 / 01-2023




                 J-44                                                             A+W Realtime Optimizer
                 Tutorial                                                                                    Zuschnitt




                                          Arbeit unterbrechen und fortsetzen
                                          Eine Optimierung, deren Lagerplatten nach und nach am Zuschnitttisch ge-
                                          schnitten werden, kann auf Grund technischer Störungen oder Arbeitsende
                                          unterbrochen werden. A+W Realtime Optimizer registriert, an welcher Stelle
                                          die Arbeit unterbrochen wurde und bietet die Möglichkeit, an der Unterbre-
                                          chungsstelle die Arbeit fortzusetzen.
                                          Nachfolgend finden Sie folgende Arbeitsschritte erklärt:
                                          •   Zuschnitt innerhalb einer Optimierung unterbrechen.
                                          •   Einen unterbrochenen Zuschnitt einer Optimierung fortsetzen.


                                           Zuschnitt innerhalb einer Optimierung unterbrechen
                                          1 Sie befinden sich in dem Dialog Zuschnitt-Übersicht ein.
                                          2 Betätigen Sie die Schaltfläche [STOPP].
                                          3 Schließen Sie den Dialog.


                                           Einen unterbrochenen Zuschnitt einer Optimierung fortsetzen
                                              A+W Realtime Optimizer merkt sich, wenn eine begonnene Optimierung
                                              nicht zu Ende zugeschnitten wurde.
                                          1 Wählen Sie im Menü Zuschnitt > Schneide Optimierung, um eine Optimie-
                                            rung zum Zuschnitt auszuwählen.
                                              Es erscheint eine Sicherheitsabfrage. Es wird angegeben, welcher Lauf
                                              nicht zu Ende geführt wurde und abgefragt, ob dieser Lauf weiter ausge-
                                              führt werden soll.
                                          2 Um den unterbrochenen Lauf anzuzeigen, wählen Sie [Ja].
                                              A+W Realtime Optimizer zeigt den Lauf im Dialog Lauf [Nummer] - Lauf
                                              [Nummer] an, der abgebrochen wurde.
                                              Wenn Sie die Sicherheitsabfrage mit Nein beantworten, dann wird die un-
                                              terbrochene Optimierung auf den Status Begonnen gesetzt. Bereits über-
                                              tragene Zuschnittsmuster behalten den Status Geschnitten. Der Dialog
                                              Wählen Sie einen Lauf aus wird angezeigt.
                                          3 Um den unterbrochenen Zuschnitt fortzusetzen, wählen Sie [Start].
                                              Der Schneidcode der bereits geschnittenen Scheiben wird nicht erneut
                                              zum Schneidtisch übertragen.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-45
                 Zuschnitt                                                                                    Tutorial




                                          Die Zuschnitt-Übersicht
                                          Die Zuschnitt-Übersicht zeigt Ihnen, was als nächstes zugeschnitten werden
                                          soll.


                        A




                                                                                                               B




                                                                                                               C



                 A Menü                              B Plattenanzeige              C Scheibenanzeige
                 Abb. J-8    Zuschnitt-Übersicht


                                          Das Menü (A) auf der linken Seite des Dialogs können Sie ein- und ausblen-
                                          den, indem Sie die entsprechendeSymbol-Schaltfläche anklicken. Darüber hi-
                                          naus können Sie die einzelnen Einträge (Zuschnitt, Panorama,
                                          Administration) auf- und zuklappen.
                                          Über die Optionen im Eintrag Zuschnitt können Sie sich die Anzeige konfigu-
                                          rieren.
3.30 / 01-2023




                                          Abb. J-9       Plattenanzeige



                 J-46                                                                       A+W Realtime Optimizer
                 Tutorial                                                                                      Zuschnitt




                                          Die Plattenanzeige (B) können Sie proTisch konfigurieren. Über die Checkbo-
                                          xen können Sie bequem einstellen, welche Felder in der Tabelle angezeigt
                                          werden sollen und welche nicht.
                                          Soll die Plattengrafik gespiegelt werden, aktivieren Sie im Bereich Plattengra-
                                          fik die gewünschte Achse.
                                          Gleiches gilt für die Scheibenanzeige (C). Auch hier können Sie die ge-
                                          wünschten Optionen zur Anzeige ein- und ausblenden:




                                          Abb. J-10    Scheibenanzeige


                                          Der Punkt Modell im Eintrag Panorama visualisiert das Modell, das zur Ma-
                                          schinenansteuerung im A+W Realtime Optimizer hinterlegt ist.
                                          Der Bereich Administration ist passwortgeschützt. Hier nehmen Sie allgemei-
                                          ne Einstellungen vor.
                                          Durch Klicken auf die Symbol-Schaltfläche [Start] starten Sie den Zuschnitt.
                                          Um den Zuschnitt zu stoppen, klicken Sie auf die Symbol-Schaltfläche [Stopp].
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-47
                 Zuschnitt                                                                          Tutorial




                             Schneidstatus zurücksetzen
                             Wenn ein Lauf oder einzelne Lagerplatten bereits den Status Geschnitten er-
                             halten haben, aber noch einmal geschnitten werden sollen, dann kann der
                             Schneidstatus zurückgesetzt und das Schneiden wiederholt werden.
                             Mit folgenden Arbeitsschritten können Sie mit den Schneidstatus zurückset-
                             zen:
                             •   Geschnittene Platten erneut schneiden.
                             •   Geschnittene Läufe erneut schneiden.
                             Wenn eine Optimierung als ganzes zurückgesetzt wurde, aber nur einzelne
                             Lagerplatten erneut geschnitten werden sollen, dann können Sie mit folgen-
                             den Arbeitsschritten Teile einer Optimierung vom erneuten Zuschnitt aus-
                             schließen:
                             •   Muster überspringen.
                             •   Erzeugung von Schneidcode unterdrücken.


                              Geschnittene Platten erneut schneiden
                                 Einzelne Platten oder ganze Läufe können erneut geschnitten werden, so-
                                 lange die Läufe noch im Zugriff von A+W Realtime Optimizer sind. Der Zu-
                                 schnitt für den entsprechenden Lauf muss gewählt und im Dialog Lauf: [Nr.]
                                 - Lauf: [Nr.] angezeigt werden.
                             1 Öffnen Sie den Dialog Restblatt Behandlung.
                               Betätigen Sie dazu die Schaltfläche [Restblätter] im Dialog Lauf: [Nr.] -
                               Lauf: [Nr.] des entsprechenden Laufes.
                             2 Markieren Sie in der Liste Optimierungen die Glasart, für die eine Lager-
                               platte erneut geschnitten werden soll.
                                 In der Liste Platten werden alle zu der markierten Glasart gehörigen Plat-
                                 ten des Laufes angezeigt. In der Spalte Status sehen Sie den Status jeder
                                 einzelnen Lagerplatte.
                                  Softwarereferenz, “Lauf: Nummer” auf Seite J-132
                             3 Klicken Sie mit der rechten Maustaste auf die Platte, die Sie vom Status
                               Geschnitten zurücksetzen und erneut schneiden wollen.
                                 Es erscheint ein Kontext-Menü mit dem Eintrag Geschnitten.
                             4 Wählen Sie Geschnitten um die Platte zurückzusetzen.


                             Ergänzende Informationen
                              Softwarereferenz, “Lauf: Nummer” auf Seite J-132
3.30 / 01-2023




                 J-48                                                             A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          Zusammenarbeit mit anderen
                                          Modulen
                                          Lernziele

                                          • Die Zusammenarbeit mit dem A+W Residual Stock Manager kennenlernen und
                                            verstehen.
                                          • Die Zusammenarbeit mit dem A+W Pattern Viewer kennenlernen und verstehen.
                                          • Die Zusammenarbeit mit dem A+W PlanEditor kennenlernen und verstehen.
                                          • Die Zusammenarbeit mit dem A+W Continuous Cutting kennenlernen und
                                            verstehen
                                          • Die Zusammenarbeit mit dem A+W Defect Optimizer kennenlernen und verstehen.


                                          Nutzen

                                          Die Leistungsfähigkeit des A+W Realtime Optimizer kann durch die Anbindung
                                          anderer Module erhöht werden.


                                          Definitionen

                                          A+W Residual Stock        Das Restelager-Magazin verwaltet Restplatten am
                                          Manager                   Zuschnitttisch.

                                          A+W Pattern Viewer        Stellt die Brechbildanzeige am Zuschnitttisch zur
                                                                    Verfügung.

                                          A+W PlanEditor            Zeigt die Daten von zu schneidenden Mustern in
                                                                    tabellarischer und in grafischer Form an.

                                          A+W Continuous Cutting    Steuert vom Büro aus, was geschnitten wird, so dass die
                                                                    Bediener automatisch wissen, was zu tun ist.

                                          A+W Defect Optimizer      Ist die intelligente Fehlerstellenoptimierung.

                                          A+W DynOpt Compact        A+W Einstiegslösung im Bereich Dynamische
                                                                    Optimierung.


                                          Merke

                                          Konfiguration             Der A+W Realtime Optimizer muss zur Zusammenarbeit
                                                                    mit den anderen Modulen entsprechend konfiguriert
                                                                    werden.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                 J-49
                 Zusammenarbeit mit anderen Modulen                                                          Tutorial




                                       Überblick
                                       A+W Realtime Optimizer kann zur Zusammenarbeit mit unterschiedlichen Mo-
                                       dulen konfiguriert werden. Informationen zur Anbindung verschiedener Vor-
                                       systeme wurden in dem vorherigen Kapitel bereits gegeben.
                                       Wenn A+W Realtime Optimizer entsprechend konfiguriert wurde, kann es mit
                                       folgenden Modulen zusammenarbeiten:
                                       •   A+W Residual Stock Manager
                                       •   A+W Pattern Viewer
                                       •   A+W PlanEditor
                                       •   A+W Continuous Cutting
                                       •   A+W Defect Optimizer
                                       •   A+W DynOpt Compact


                                       A+W Residual Stock Manager
                                       Bei diesem Modul handelt es sich um ein Restelager-Magazin, in dem Rest-
                                       platten am Zuschnitttisch verwaltet werden. Bleibt beim Zuschnitt eine Rest-
                                       platte übrig, so wird dieses nicht verworfen sondern im A+W Residual Stock
                                       Manager zwischengespeichert. Informationen über Glasart, Dicke und Ab-
                                       messungen der Restplatten werden in einem Verwaltungsprogramm (A+W
                                       Planning Web) erfasst und gespeichert. A+W Realtime Optimizer kann mit
                                       dem A+W Planning Web zusammenarbeiten. Dabei werden Daten über die
                                       Restplatten ausgetauscht. Restplatten können anschließend vom A+W Real-
                                       time Optimizer in Tischoptimierungen integriert werden. Wird eine Optimie-
                                       rung geschnitten, kann die Restplatte durch eine Platte aus dem Restelager
                                       ersetzt werden (ohne Neuoptimierung).
                                       Sobald eine Restplatte in eine Optimierung eingeplant ist, informiert A+W
                                       Realtime Optimizer das A+W Planning Web über diesen Status. Die Restplat-
                                       te kann dann nicht mehr für andere Zuschnitte verwendet werden.
                                       Wird ein Tisch mit Schneidcode angesteuert, der für eine Resteplatte optimiert
                                       wurde, so steuert der Schneidcode das Restelager-Magazin an und die benö-
                                       tigte Restplatte wird zum Zuschnitt auf den Tisch aufgelegt.


                                       A+W Planning Web
                                       In diesem Modul nehmen Sie die Konfiguration für den A+W Residual Stock
                                       Manager vor.

                                           A+W Planning Web-Konfiguration
                                           Die Standard-Konfiguration wird bei der Installation durch A+W-Mitarbeiter
                                           vorgenommen. Wir erläutern in dieser Dokumentation, wie Sie Lager, Ab-
                                           stellplätze und Gestelle im A+W Planning Web anlegen.
3.30 / 01-2023




                 J-50                                                                      A+W Realtime Optimizer
                 Tutorial                                                      Zusammenarbeit mit anderen Modulen




                                          Oberfläche
                                          Wenn Sie das A+W Planning Web gestartet haben, erscheint folgende An-
                                          sicht:




                 Abb. J-11   Oberfläche A+W Planning Web


                                          Im Anschluss wählen Sie den Eintrag Lager aus. Sie befinden sich im Bereich
                                          Aufträge.




                 Abb. J-12   Bereich: Aufträge


                                          Stammdaten
                                          In diesem Bereich befinden sich die Einstellungen für die Stammdaten. Dazu
                                          zählen:
                                          •      Lager
                                          •      Abstellplätze
                                          •      Gestelle
                                          •      Gruppen
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                         J-51
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                         Lager
                                         Über die Symbol-Schaltflächen Lager können Sie sich die entsprechenden In-
                                         halte anzeigen lassen.




                 Abb. J-13   Bereich: Stammdaten


                                         In diesem Bereich werden Ihnen alle in Ihrem Hause angelegten Lager ange-
                                         zeigt.
                                         Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                         •   Den Namen eines bestehenden Lagers ändern
                                         •   Ein neues Lager hinzufügen
                                         •   Ein bestehendes Lager löschen


                                          So ändern Sie den Namen eines bestehenden Lagers
                                         1 Klicken Sie mit der Maus in das Feld Bezeichnung. Das Feld wird zur Be-
                                           arbeitung freigegeben.
                                         2 Ändern Sie den Namen und verlassen Sie das Feld.
                                         3 Das Feld bekommt oben links in der Ecke ein kleines rotes Dreieck. Das
                                           Dreieck signalisiert, dass es Änderungen gibt, die noch nicht gespeichert
                                           wurden. Es wird so lange angezeigt, bis Sie auf die Schaltfläche [Spei-
                                           chern] klicken.
                                         4 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.
                                         5 Das kleine rote Dreieck ist nicht mehr da.


                                          So fügen Sie ein neues Lager hinzu
                                         1 Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben
                                           in der Tabelle eingefügt.
                                         2 Im Feld ID wird die nächst mögliche Nummer automatisch vorgeschlagen.
                                           Sie können diese Nummer überschreiben.
                                         3 Geben Sie im Feld Bezeichnung den Namen für das Lager ein und verlas-
                                           sen Sie das Feld.
                                         4 Das Feld bekommt oben links in der Ecke ein kleines rotes Dreieck. Das
3.30 / 01-2023




                                           Dreieck signalisiert, dass es Änderungen gibt, die noch nicht gespeichert
                                           wurden. Es wird so lange angezeigt, bis Sie auf die Schaltfläche [Spei-
                                           chern] klicken.


                 J-52                                                                       A+W Realtime Optimizer
                 Tutorial                                                          Zusammenarbeit mit anderen Modulen




                                           5 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.
                                           6 Das kleine rote Dreieck ist nicht mehr da.


                                            So löschen Sie ein Lager
                                           1 Klicken Sie in die Zeile mit dem entsprechenden Lager.
                                           2 Klicken Sie auf die Schaltfläche [Löschen].
                                           3 Das Lager wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.


                                           Ergänzende Informationen
                                            Softwarereferenz, “Lager” auf Seite J-155

                                           Abstellplätze
                                           Abstellplätze sind Plätze oder Bereiche, auf denen Scheiben abgestellt wer-
                                           den können.
                                           Um einem Lager weitere Abstellplätze hinzufügen, bestehende Abstellplätze
                                           zu ändern oder zu löschen, klicken Sie in dem Eintrag für das entsprechende
                                           Lager auf die Schaltfläche [Bearbeiten]. Im Anschluss werden Ihnen alle Ab-
                                           stellplätze angezeigt, die für das Lager angelegt sind.




                 Abb. J-14   Bereich: Abstellplatzinformationen


                                           Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                           •   Einen neuen Abstellplatz hinzufügen
                                           •   Einen bestehenden Abstellplatz löschen
                                           •   Änderungen an einem bestehenden Abstellplatz vornehmen


                                            So fügen Sie einen neuen Abstellplatz hinzu
                                           1 Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben
                                             in der Tabelle eingefügt.
                                           2 Im Feld ID wird die nächst mögliche Nummer automatisch vorgeschlagen.
                                             Sie können diese Nummer überschreiben.
                                           3 Geben Sie im Feld Bezeichnung den Namen für den Abstellplatz ein.
                                           4 Wählen Sie aus der Kombobox Lagertyp den entsprechenden Typ aus (La-
                                             gerplatz/Lagereingang).
3.30 / 01-2023




                                           5 Wählen Sie aus der Kombobox Zuordnungsstatus den entsprechenden
                                             Status aus.
                                           6 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.


                 A+W Realtime Optimizer                                                                            J-53
                 Zusammenarbeit mit anderen Modulen                                                               Tutorial




                                          So löschen Sie einen Abstellplatz
                                         1 Klicken Sie in die Zeile mit dem entsprechenden Abstellplatz.
                                         2 Klicken Sie auf die Schaltfläche [Löschen].
                                         3 Der Abstellplatz wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsab-
                                           frage.


                                          So nehmen Sie Änderungen an einem Abstellplatz vor
                                         1 Klicken Sie in das Feld mit dem entsprechenden Eintrag.
                                         2 Überschreiben Sie den Eintrag oder wählen Sie aus der Kombobox den
                                           gewünschten Eintrag aus.
                                         3 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.


                                         Ergänzende Informationen
                                          Softwarereferenz, “Abstellplatzinformationen” auf Seite J-157

                                         Gestelle
                                         In diesem Bereich werden Ihnen die für einen Abstellplatz angelegten Gestelle
                                         angezeigt.




                 Abb. J-15   Stammdaten: Gestelle


                                         Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                         •   Ein neues Gestell hinzufügen
                                         •   Ein bestehendes Gestell löschen
                                         •   Änderungen an einem bestehenden Gestell vornehmen


                                          So fügen Sie ein neues Gestell hinzu
                                         1 Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben
                                           in der Tabelle eingefügt.
                                         2 Im Feld ID wird die nächst mögliche Nummer automatisch vorgeschlagen.
                                           Sie können diese Nummer überschreiben.
                                         3 Im Feld Bezeichnung vergeben Sie einen eindeutigen Namen zur Identifi-
                                           zierung eines Gestelltyp.
                                         4 Wählen Sie aus der Kombobox Zuordnungsstatus den entsprechenden
3.30 / 01-2023




                                           Status aus.
                                              A+W Realtime Optimizer: Softwarereferenz, “Zuordnungsstatus” auf
                                               Seite J-159



                 J-54                                                                           A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          5 Wählen Sie aus der Kombobox Eigenschaft den entsprechenden Typ aus.
                                          6 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.


                                           So löschen Sie ein bestehendes Gestell
                                          1 Klicken Sie in die Zeile mit dem entsprechenden Gestell.
                                          2 Klicken Sie auf die Schaltfläche [Löschen].
                                          3 Das Gestell wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.


                                           So nehmen Sie Änderungen an einem Gestell vor
                                          1 Klicken Sie in das Feld mit dem entsprechenden Eintrag.
                                          2 Überschreiben Sie den Eintrag oder wählen Sie aus der Kombobox den
                                            gewünschten Eintrag aus.
                                          3 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Gestelle” auf Seite J-159

                                          Gestelleigenschaften
                                          In diesem Bereich werden Ihnen die Eigenschaften der unterschiedlichen Ge-
                                          stelltypen angezeigt. Als Eigenschaft ist hier der Gestelltyp zu verstehen (A-
                                          Bock, L-Bock, Fächerwagen, etc.).




                 Abb. J-16   Stammdaten: Gestelleigenschaften


                                          Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                          •   Eine neue Gestelleigenschaft hinzufügen
                                          •   Eine bestehende Gestelleigenschaft löschen
                                          •   Änderungen an einer bestehenden Gestelleigenschaft vornehmen


                                           So fügen Sie eine neue Gestelleigenschaft hinzu
                                          1 Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben
                                            in der Tabelle eingefügt.
                                          2 Im Feld Bezeichnung vergeben Sie einen eindeutigen Namen zur Identifi-
                                            zierung eines Gestelltyp.
3.30 / 01-2023




                                          3 Geben Sie im Feld Zugangsart wählen Sie aus der Kombobox die entspre-
                                            chende Art aus.
                                               A+W Realtime Optimizer: Softwarereferenz, “Zugangsart” auf Seite J-161


                 A+W Realtime Optimizer                                                                              J-55
                 Zusammenarbeit mit anderen Modulen                                                              Tutorial




                                           4 Wählen Sie aus der Kombobox Lagertyp den entsprechenden Typ aus (La-
                                             gerplatz/Lagereingang).
                                           5 Wählen Sie aus der Kombobox Zuordnungsstatus den entsprechenden
                                             Status aus.
                                           6 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.


                                            So löschen Sie eine bestehende Gestelleigenschaft
                                           1 Klicken Sie in die Zeile mit der entsprechenden Eigenschaft.
                                           2 Klicken Sie auf die Schaltfläche [Löschen].
                                           3 Die Gestelleigenschaft wird gelöscht. Vorsicht: Es erscheint keine Sicher-
                                             heitsabfrage.


                                            So nehmen Sie Änderungen an einer Gestelleigenschaft vor
                                           1 Klicken Sie in das Feld mit dem entsprechenden Eintrag.
                                           2 Überschreiben Sie den Eintrag oder wählen Sie aus der Kombobox den
                                             gewünschten Eintrag aus.
                                           3 Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.


                                           Ergänzende Informationen
                                            Softwarereferenz, “Gestelleigenschaften” auf Seite J-161

                                           Übersicht
                                           In diesem Bereich werden Ihnen alle Restblätter angezeigt, die eingelagert
                                           wurden.




                 Abb. J-17   Übersicht: Eingelagerte Restblätter


                                           Die Daten können in der Ansicht editiert werden, z. B. die Größe der eingela-
                                           gerten Restscheibe. Über die Filterfunktionen, die Ihnen im Tabellenkopf jedes
                                           Feldes zur Verfügung stehen, können Sie die Ergebnisse der Anzeige ein-
                                           schränken.
3.30 / 01-2023




                                           Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                           •   Änderungen an einem eingelagerten Rest vornehmen
                                           •   Einen neuen Rest hinzufügen


                 J-56                                                                            A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          •   Einen bestehenden Rest löschen


                                           So nehmen Sie Änderungen an einem eingelagerten Rest vor
                                          1 Klicken Sie in dem Eintrag den Sie ändern möchten auf die Schaltfläche
                                            [Bearbeiten]. Es öffnet sich der Dialog Hinzufügen/Bearbeiten.
                                          2 Nehmen Sie die gewünschten Änderungen vor.
                                          3 Klicken Sie auf die Schaltfläche [Anwenden], um die Angaben zu spei-
                                            chern.


                                           So fügen Sie einen neuen Rest hinzu
                                          1 Klicken Sie auf die Schaltfläche [Neuen Datensatz hinzufügen]. Es öffnet
                                            sich der Dialog Hinzufügen/Bearbeiten.
                                          2 Im Feld Lager wählen Sie aus der Kombobox das entsprechende Lager
                                            aus.
                                          3 Im Feld Abstellplatzinformationen wählen Sie aus der Kombobox den Ab-
                                            stellplatz aus, auf dem der Rest steht.
                                          4 Im Feld Gestell wählen Sie aus der Kombobox das entsprechende Gestell
                                            aus, auf dem der Rest steht.
                                          5 Im Feld Gruppe wählen Sie aus der Kombobox die entsprechende Gruppe
                                            aus.
                                          6 Im Feld Glastyp wählen Sie aus der Kombobox aus, um welchen Glastyp
                                            es sich bei dem Rest handelt.
                                          7 In den Feldern Breite und Höhe geben Sie die Abmessungen des Restes
                                            ein.
                                          8 Im Feld Info können Sie eine zusätzliche Information zu dem Rest hinter-
                                            legen.
                                          9 Im Feld Zuordnungsstatus wählen Sie aus der Kombobox den entspre-
                                            chenden aus.
                                               Softwarereferenz, “Zuordnungsstatus” auf Seite J-164
                                          10 Im Feld Datum geben Sie ein, wann der Rest eingelagert wurde.
                                          11 Klicken Sie auf die Schaltfläche [Anwenden], um die Angaben zu spei-
                                             chern.


                                           So löschen Sie einen eingelagerten Rest
                                          1 Klicken Sie in die Zeile mit der entsprechenden Eigenschaft.
                                          2 Klicken Sie auf die Schaltfläche [Löschen].
                                          3 Der eingelagerte Rest wird gelöscht. Vorsicht: Es erscheint keine Sicher-
                                            heitsabfrage.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-57
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                          Restelager-Platten und Restblätter nicht gleichzeitig möglich!
                                          Wenn Sie für eine Optimierung Platten aus dem Restelager verwenden
                                          wollen, dann wird ein zuvor eingetragenes Restblatt ignoriert. A+W Real-
                                          time Optimizer zeigt dann eine entsprechende Meldung an.


                                        Restelager-Platten bei der Optimierung verwenden
                                       1 Wählen Sie im Dialog Tischoptimierung das Register Restelagerplatten.
                                          In der rechten Liste werden alle Platten angezeigt, die im A+W Residual
                                          Stock Manager für die Glasart und Dicke des Laufes vorhanden sind und
                                          dem Schneidtisch zur Verfügung stehen.
                                       2 Markieren Sie die Restelager-Platte, die A+W Realtime Optimizer für die
                                         Zuschnittoptimierung verwenden soll.
                                          Sie können bis zu zehn Restelager-Platte in eine Optimierung integrieren.
                                       3 Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren
                                         und betätigen Sie die Schaltfläche [Optimieren].
                                          Anschließend wird die Restelager-Platte im Programm, das die Restela-
                                          ger-Platten verwaltet, für diesen Lauf reserviert und kann von keinem an-
                                          deren Lauf mehr verwendet werden.
                                       4 Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Spei-
                                         chern].


                                       Ergänzende Informationen
                                        Softwarereferenz, “Restplatten und Lagerplatten” auf Seite J-113

                                       Etiketten drucken
                                       Das Drucken der entsprechenden Etiketten ist ebenfalls aus der Übersicht he-
                                       raus möglich. Dazu klicken Sie in dem Eintrag auf die Schaltfläche [Drucken].

                                          Etiketten drucken
                                          Zum Drucken der Etiketten muss der entsprechende Drucker eingerichtet
                                          sein.
3.30 / 01-2023




                 J-58                                                                         A+W Realtime Optimizer
                 Tutorial                                                       Zusammenarbeit mit anderen Modulen




                                          A+W Pattern Viewer
                                          Der A+W Pattern Viewer stellt eine Brechbildanzeige am Zuschnitttisch zur
                                          Verfügung, mit der, je nach Konfiguration, auch Bruch erfasst werden kann.
                                          Der A+W Realtime Optimizer gibt die Informationen an den A+W Pattern Vie-
                                          wer, wenn Schneidcode für den angeschlossenen Tisch erstellt wurde. Der
                                          A+W Pattern Viewer kann darauf hin das zur jeweiligen Optimierung gehören-
                                          de Brechbild anzeigen. Die Darstellung entspricht dem zu schneidenden La-
                                          germaß bzw. Restblatt und enthält alle wichtigen Informationen über die
                                          Optimierung, den Artikel und die einzelnen Scheiben. Wird mit A+W Pattern
                                          Viewer Bruch erfasst, so gibt das Modul eine entsprechende Information an
                                          den A+W Realtime Optimizer.


                                          Einstellungen
                                          Über das A+W Logo erreichen Sie die Einstellungen:




                 Abb. J-18   Menü


                                          Der Eintrag Sprache enthält alle Sprachen, in denen das Modul verfügbar ist.
                                          Die Sprache kann zur Laufzeit umgeschaltet werden.
                                          Die Bereiche Anwendung registrieren und Bruchgründe werden von A+W-Mit-
                                          arbeitern benötigt, um das Modul in Ihrem Haus entsprechend Ihren Anforde-
                                          rungen zu konfigurieren. Wir gehen daher nicht weiter auf diese Bereiche ein.
                                          Im Bereich Über wird Ihnen die Versionsnummer des Moduls angezeigt.
                                          Über die Schaltfläche Zurück gelangen Sie wieder in die Brechbildanzeige.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-59
                 Zusammenarbeit mit anderen Modulen                                                              Tutorial




                                          Abb. J-19       Zurück zur Brechbildanzeige


                                          Die Oberfläche




                 Abb. J-20   Die Brechbildanzeige


                                          Die Menüleiste
                                          Die Menüleiste im A+W Pattern Viewer beinhaltet die Einträge:
                                          •   Ansicht
                                          •   Maße

                                          Ansicht
                                          Klicken Sie auf Ansicht, öffnet sich die Menüleiste:




                 Abb. J-21   Menüleiste - komplett
3.30 / 01-2023




                                          Die Menüleiste ist in einzelne Bereiche unterteilt:
                                          •   Brechbild


                 J-60                                                                            A+W Realtime Optimizer
                 Tutorial                                                       Zusammenarbeit mit anderen Modulen




                                          •   Zoom
                                          •   Eingabetyp
                                          •   Ansicht konfigurieren
                                          •   Tooltipp
                                          •   Validierung
                                          Direkt unterhalb der Menüleiste befindet sich der Informationsbereich. Dieser
                                          enthält weiterreichende Informationen zu dem aktuellen Muster.



                 Abb. J-22   Menüleiste - Informationsbereich


                                          Ganz links wird Ihnen die Lauf-, Los- und Musternummer angezeigt. Im Bei-
                                          spiel oben heißt das:
                                          Laufnummer: 2689
                                          Losnummer: 3
                                          Musternummer: 3
                                          Als nächstes wird Ihnen die Nummer des aktuellen Muster und die Gesamtan-
                                          zahl der Muster angezeigt. Im Beispiel oben Muster Nummer 3 von insgesamt
                                          5. Dann wird Ihnen die Glasart angezeigt. Im Beispiel oben Star S 4 mm 4.00.
                                          Im Anschluss folgt die Breite x Höhe der verwendeten Lagerplatte. Rechts au-
                                          ßen wird das Optimierungsergebnis für das aktuelle Muster angezeigt.

                                          Brechbild
                                          In diesem Bereich können Sie die Art der Anzeige durch Klicken auf die ent-
                                          sprechende Schaltfläche auswählen. Es gibt zwei Möglichkeiten:
                                          •   Brechbild
                                          •   JSON
                                          Bei Ihrer täglichen Arbeit werden Sie die Einstellung Brechbild verwenden.
                                          Beim Auftreten von Problemen können Sie dann in die Einstellung JSON
                                          wechseln, über das Kontextmenü den Inhalt kopieren und diesen anschlie-
                                          ßend einem A+W-Mitarbeiter für eine detaillierte Analyse zur Verfügung stel-
                                          len.

                                          Zoom
                                          In diesem Bereich befinden sich die Einstellungen für die Größendarstellung
                                          des Brechbildes und dem Informationsbereich direkt unterhalb der Menüleis-
                                          te.
                                          Brechbild:
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-61
                 Zusammenarbeit mit anderen Modulen                                                              Tutorial




                                           Abb. J-23   Zoom Brechbild


                                           Die Kombobox enthält die Werte 0 bis 4. Die im Anschluss folgende Grafik soll
                                           die unterschiedlichen Einstellungen verdeutlichen:




                                           Abb. J-24   Unterschiedlichen Schnitte


                                           0: Es wird das komplette Brechbild einer Platte angezeigt:
3.30 / 01-2023




                 Abb. J-25   Brechbild - komplett



                 J-62                                                                         A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          1: Es werden die einzelnen X-Schnitte angezeigt. Ein X-Schnitt (üblicherweise
                                          der Traverenschnitt) verläuft parallel zum linken bzw. rechten Plattenrand (-
                                          schnitt) bzw. senkrecht zum unteren Plattenrand. Dieser Schnitt teilt die La-
                                          gerplatte in Teile bzw. Traveren. Über die Pfeiltasten rechts und links können
                                          Sie die einzelnen Traveren weiter bzw. zurück schalten.




                                          Abb. J-26    Brechbild - Travere


                                          2: Es werden die einzelnen Y-Schnitte angezeigt (von unten nach oben). Ein
                                          Y-Schnitt verläuft parallel zum oberen bzw. unteren Plattenrand (-schnitt). Die-
                                          ser Schnitt teilt eine Travere in obere und untere Abschnitte. Über die Pfeiltas-
                                          ten rechts und links können Sie die einzelnen Schnitte weiter bzw. zurück
                                          schalten.




                                          Abb. J-27    Brechbild - Y-Schnitt


                                          3: Es werden die einzelnen Z-Schnitte angezeigt (von links nach rechts). Ein
                                          Z-Schnitt verläuft wieder parallel zu einem linken bzw. rechten Plattenrand (-
3.30 / 01-2023




                                          schnitt) und/oder einem X-Schnitt. Er unterteilt die durch Y-Schnitte gebildeten
                                          Abschnitte. Über die Pfeiltasten rechts und links können Sie die einzelnen
                                          Schnitte weiter bzw. zurück schalten.



                 A+W Realtime Optimizer                                                                              J-63
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                       Abb. J-28    Brechbild - Z-Schnitt


                                       4: Es werden die einzelnen W-Schnitte angezeigt (von unten nach oben). Ein
                                       W-Schnitt verläuft parallel zu einem Y-Schnitt und befindet sich zwischen ei-
                                       nem X-Schnitt (bzw. linkem oder rechten Plattenrand (-schnitt)) und einem Z-
                                       Schnitt. Über die Pfeiltasten rechts und links können Sie die einzelnen Schnit-
                                       te weiter bzw. zurück schalten.




                                       Abb. J-29    Brechbild - W-Schnitt


                                       Schriftgröße
                                       Über die Kombobox können Sie steuern, in welcher Größe der Informations-
                                       bereich direkt unterhalb der Menüleiste dargestellt wird.
                                       Es stehen die Werte klein, mittel und groß zur Verfügung:
                                       Klein:



                                       Abb. J-30    Schriftgröße klein


                                       Mittel:
3.30 / 01-2023




                                       Abb. J-31    Schriftgröße mittel


                                       Groß:


                 J-64                                                                      A+W Realtime Optimizer
                 Tutorial                                                      Zusammenarbeit mit anderen Modulen




                                          Abb. J-32      Schriftgröße groß


                                          Eingabetyp
                                          In diesem Bereich befindet sich der Eintrag Einzelscheibe. In diesem Modus
                                          arbeiten automatisierte Betriebe. Es wird jede Scheibe einzeln zur Abarbei-
                                          tung vorgegeben. Der entsprechende Modus wird bei Einrichtung des A+W
                                          Pattern Viewer von A+W Mitarbeitern eingestellt.

                                          Ansicht konfigurieren
                                          In diesem Bereich befinden sich verschiedene Eigenschaften, mit deren Hilfe
                                          Sie sich die Brechbildanzeige nach Ihren Bedürfnissen einstellen können.
                                          Koordinaten:




                                          Abb. J-33      Koordinaten


                                          Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Ko-
                                          ordinaten:




                                          A Koordinaten deaktiviert             B Koordinaten aktiviert


                                          Maße:




                                          Abb. J-34      Maße


                                          Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Ab-
                                          messungen der Scheibe:
3.30 / 01-2023




                                          A Maße deaktiviert                    B Maße aktiviert




                 A+W Realtime Optimizer                                                                          J-65
                 Zusammenarbeit mit anderen Modulen                                                          Tutorial




                                       Gestellnummer:




                                       Abb. J-35    Gestellnummer


                                       Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Ge-
                                       stellnummer:




                                       A Gestellnummer deaktiviert            B Gestellnummer aktiviert


                                       Brechreihenfolge:




                                       Abb. J-36    Brechreihenfolge


                                       Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der
                                       Brechreihenfolge. Die Scheibe mit der kleinsten Nummer wird zuerst gebro-
                                       chen:




                                       A Brechreihenfolge deaktiviert         B Brechreihenfolge aktiviert


                                       Zweite Glasart oder Laufnummer:




                                       Abb. J-37    Zweite Glasart oder Laufnummer


                                       Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der zwei-
                                       ten Glasart oder der Laufnummer. Im Beispiel unten wird die Laufnummer an-
3.30 / 01-2023




                                       gezeigt:




                 J-66                                                                      A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          A Laufnummer deaktiviert                B Laufnummer aktiviert


                                          Barcode:




                                          Abb. J-38      Barcode


                                          Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige des Bar-
                                          codes:




                                          A Barcode deaktiviert                   B Barcode aktiviert


                                          Zusatztexte:




                                          Abb. J-39      Zusatztexte


                                          Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Zu-
                                          satztexte. Zusatztexte können im Kopf- und im Fußbereich angezeigt werden.
                                          Ist ein Kopftext konfiguriert, ändert sich die Hintergrundfarbe von blau auf
                                          lachs. Ist ein Fußtext konfiguriert, ändert sich die Hintergrundfarbe von rot auf
                                          gelb. Entsprechende Texte werden von A+W Mitarbeitern bei der Installation
                                          nach Ihren Wünschen eingerichtet:




                                          A Kopfbereich ohne Zusatztext           B Kopfbereich mit Zusatztext
3.30 / 01-2023




                                          A Fußbereich ohne Zusatztext            B Fußbereich mit Zusatztext


                                          Travere drehen:


                 A+W Realtime Optimizer                                                                               J-67
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                       Abb. J-40    Travere drehen


                                       Über diese Schaltfläche ist es möglich, Traveren automatisch um 90° zu dre-
                                       hen, wenn das Größenverhältnis der Travere besser zum Bildschirm passt,
                                       um eine größere Darstellung zu erzielen:




                                       A Travere nicht gedreht          B Travere gedreht


                                       Tooltipp
                                       In diesem Bereich befindet sich eine Kombobox, mit deren Hilfe Sie die Anzei-
                                       gedauer für einen Tooltipp einstellen können. Sie können von einer bis zu acht
                                       Sekunden wählen.




                                       Abb. J-41    Anzeigedauer Tooltipp


                                       Validierung
                                       In diesem Bereich befindet sich die Schaltfläche über die Sie die Arbeitsrich-
                                       tung wechseln können.




                                       A Normal                               B Umkehren
3.30 / 01-2023




                 J-68                                                                       A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          Normalerweise liegt die Platte so auf dem Tisch, dass Sie auf der linken Seite
                                          anfangen zu brechen. Die Brechbildanzeige schalten Sie dann zum nächsten
                                          Muster weiter, indem Sie auf den rechten Pfeil klicken.
                                          Es gibt aber auch Konstellationen, wo die Platte so auf dem Tisch liegt, dass
                                          Sie auf der rechten Seite anfangen zu brechen. Damit Sie dann ebenfalls den
                                          rechten Pfeil zum Umschalten auf das nächste Muster verwenden können,
                                          aktvieren Sie die Schaltfläche [umkehren].

                                          Informationen zu Scheibe und Verschnitt
                                          Wenn Sie die Maus auf einer Scheibe oder auf einem leeren Bereich platzie-
                                          ren, werden Ihnen die entsprechenden Informationen angezeigt:




                                          A Scheibeninformation                   B Verschnittinformation
                                          Abb. J-42    Informationen zu Scheibe und Verschnitt


                                             Informationen
                                             Die angezeigten Informationen sind abhängig vom Kunden und der Konfi-
                                             guration. Sie werden bei der Installation von A+W-Mitarbeitern entspre-
                                             chend eingerichtet. Wenn Sie Änderungen an Ihrer Konfiguration
                                             wünschen (z. B. der Name des Kunden soll angezeigt werde), kontaktieren
                                             Sie bitte einen A+W-Mitarbeiter.

                                          Verlinkte Läufe anzeigen
                                          Das blaue Dreieck an der oberen Kante im A+W Pattern Viewer zeigt an, wo
                                          der verlinkte Lauf beginnt:
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-69
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                       Abb. J-43    Beginn des verlinkten Laufes


                                       Abstellkante anzeigen
                                       Wurde bei einer freien Form in der SN-Datei eine Markierung für die Abstell-
                                       kante hinterlegt (z. B. in der Auftragserfassung mit iTOE), wird diese Kante im
                                       A+W Pattern Viewer durch einen gelben Pfeil angezeigt:




                                       Abb. J-44    Abstellkante für freie Formen


                                       Symbol für Stempel, Logo oder Referenzmarke anzeigen
                                       Der A+W Pattern Viewer bietet auch die Möglichkeit, ein Bild an der Stelle ei-
                                       nes Stempels oder eines Logos zu zeigen.

                                          Symbole
                                          Die Symbole sind abhängig vom Kunden und der Konfiguration. Sie wer-
                                          den bei der Installation von A+W-Mitarbeitern entsprechend eingerichtet.
                                          Wenn Sie Änderungen an Ihrer Konfiguration wünschen (z. B. Logo oder
                                          Stempel anzeigen), kontaktieren Sie bitte einen A+W-Mitarbeiter.
3.30 / 01-2023




                 J-70                                                                       A+W Realtime Optimizer
                 Tutorial                                                       Zusammenarbeit mit anderen Modulen




                                          Farbauswahl für Auftragspositionen
                                          Der A+W Pattern Viewer bietet auch die Möglichkeit, Glas in einer benutzer-
                                          definierten Farbe einzufärben. Es stehen verschiedene Farben zur Auswahl.

                                              Farben
                                              Die Auswahl der Farben basiert auf den Wünschen der einzelnen Kunden.
                                              Sie werden bei der Installation von A+W-Mitarbeitern entsprechend einge-
                                              richtet. Wenn Sie Änderungen an Ihrer Konfiguration wünschen (z. B. Logo
                                              oder Stempel anzeigen), kontaktieren Sie bitte einen A+W-Mitarbeiter.

                                          Erste und letzte Scheibe markieren
                                          Der A+W Pattern Viewer bietet die Möglichkeit, die ersten und letzten Schei-
                                          ben auf einem Abstellplatz entsprechend zu markieren.

                                              Ersten und letzten Scheibe markieren
                                              Ob die ersten und letzten Scheiben auf einem Abstellplatz markiert wer-
                                              den, basiert auf den Wünschen der einzelnen Kunden. Das wird bei der In-
                                              stallation von A+W-Mitarbeitern entsprechend eingerichtet. Wenn Sie
                                              Änderungen an Ihrer Konfiguration wünschen, kontaktieren Sie bitte einen
                                              A+W-Mitarbeiter.

                                          Maße
                                          Klicken Sie auf Maße, öffnet sich der Bereich Einheitensystem:




                                          Abb. J-45      Menü Maße


                                          Im Eintrag Einheitensystem können Sie wählen zwischen:
                                          •   Metrisch
                                          •   Imperial
                                          Die darunter liegende Kombobox ist abhängig von der Auswahl des Einheiten-
                                          systems. Haben Sie Metrisch gewählt, können Sie über die Kombobox Nach-
                                          kommastellen entscheiden, wie viele Nachkommastellen (bis zu drei) Sie sich
                                          anzeigen lassen. Haben Sie Imperial gewählt, können Sie über die Kombobox
                                          Genauigkeit diese auswählen (1/16, 1/32, 1/64, 1/128, 1/256).

                                          Bruchscheiben
                                          Im A+W Pattern Viewer können Sie Scheiben als Bruch markieren, indem Sie
                                          in der Brechbildanzeige die entsprechende Scheibe markieren. Es erscheint
                                          eine Auswahl mit allen angelegten Bruchgründen. Wählen Sie den entspre-
                                          chenden Bruchgrund aus. Die Auswahl wird geschlossen und die ausgewähl-
3.30 / 01-2023




                                          te Scheibe entsprechend gekennzeichnet.




                 A+W Realtime Optimizer                                                                          J-71
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                       A+W PlanEditor
                                       Der A+W PlanEditor zeigt die Daten von zu schneidenden Mustern in tabella-
                                       rischer und in grafischer Form an. Die Ergebnisanzeige zeigt übersichtlich die
                                       statistische Auswertung der vorhandenen Muster. Sie erhalten einen schnel-
                                       len Überblick über die zu produzierenden Scheiben, Lagermaße, Restblätter,
                                       Verschnitt, usw.
                                       Der grafische Editor zeigt, je nach Konfiguration, die zu schneidenden Muster
                                       an und stellt eine Reihe von Bearbeitungsmöglichkeiten zur Verfügung. Sie
                                       können Muster anlegen, verändern, Scheiben zufügen, speichern und dru-
                                       cken.
                                       Wenn der A+W PlanEditor an Ihrem Arbeitsplatz installiert ist, dann können
                                       Sie nach Erstellung einer Tischoptimierung durch Doppelklick auf die optimier-
                                       te Zuschnittplatte den A+W PlanEditor starten. Dieser zeigt dann das Schneid-
                                       muster der Zuschnittplatte an. Veränderungen, die Sie mit dem A+W
                                       PlanEditor an einem solchen Muster vornehmen, werden in den A+W Real-
                                       time Optimizer übernommen.


                                       Ergänzende Informationen
                                        Weitere Informationen zu dem A+W PlanEditor finden Sie in der entsprechenden
                                         Dokumentation.
3.30 / 01-2023




                 J-72                                                                       A+W Realtime Optimizer
                 Tutorial                                                        Zusammenarbeit mit anderen Modulen




                                          A+W Continuous Cutting
                                          Läuft der A+W Realtime Optimizer am Schneidtisch im Modus Kontinuierlicher
                                          Zuschnitt wird vor dem Start des Zuschnitts eine Übersicht der für diesen Tisch
                                          geplanten Läufe angezeigt. Hier besteht auch noch die Möglichkeit, einen
                                          Lauf wieder zurückzusetzen. Fahren Sie mit dem Zuschnitt fort, wird die erste
                                          Gruppe in den Zuschnitt geladen und der Zuschnitt gestartet. Ist eine Eilgrup-
                                          pe vorhanden, wird diese zuerst geladen und die darauffolgende Gruppe an-
                                          gehängt. Wenn der letzte Lauf der aktuellen Gruppe fast fertig zugeschnitten
                                          ist, wird die nächste Gruppe automatisch in den Zuschnitt geladen. So werden
                                          nach und nach alle geplanten Läufe entsprechend der in der Planung vorge-
                                          nommenen Einstellungen automatisch abgearbeitet.


                                          Übersicht der geplanten Läufe
                                          In der Planungsansicht werden alle in A+W Production optimierten und zum
                                          Zuschnitt freigegebenen Läufe und ihre Eigenschaften angezeigt. Hier können
                                          Sie nun auswählen, welche Läufe am Schneidtisch, für den sie optimiert wur-
                                          den, zugeschnitten werden sollen. Dabei kann die Reihenfolge festgesetzt
                                          und verschiedene Einstellungen vorgenommen werden. Für bereits geplante
                                          Läufe können Änderungen vorgenommen werden, vorausgesetzt der Zu-
                                          schnitt wurde noch nicht begonnen.
                                          Klicken Sie im A+W Realtime Optimizer auf Zuschnitt > Kontinuierliches
                                          Schneiden ..., erscheint eine Liste mit den freigegebenen Losen:




                                          Abb. J-46    Freigegebene Lose


                                          Über die Kombobox Schneidtische können Sie bei Bedarf die Anzeige ein-
                                          schränken. Klicken Sie dann unten rechts auf die Schaltfläche [Planung F5],
                                          öffnet sich die Planungsansicht:
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-73
                 Zusammenarbeit mit anderen Modulen                                                      Tutorial




                                       Abb. J-47   Planungsansicht


                                       Erläuterung der Felder

                                       Filter
                                       Für eine bessere Übersicht können Filter angewendet werden, um die ange-
                                       zeigten Läufe beispielsweise nach Glasart zu filtern.
                                       Die entsprechenden Einstellungen befinden sich in A+W Production > Konfi-
                                       guration > Parameter > A+W Production > Kontinuierliches Schneiden >
                                       AUW_CONTINUOUS_CUTTING > Filter.
3.30 / 01-2023




                 J-74                                                                   A+W Realtime Optimizer
                 Tutorial                                                         Zusammenarbeit mit anderen Modulen




                                          Abb. J-48    Filtereinstellungen


                                          Um einen neuen Filter anzulegen oder aber um Änderungen an einem beste-
                                          henden Filter vorzunehmen, klicken Sie bitte auf die drei Punkte. Es öffnet sich
                                          der Dialog:




                                          Abb. J-49    Neuen Filter anlegen oder bestehenden Filter ändern


                                          Um Änderungen an einem bestehenden Filter vorzunehmen, markieren Sie
                                          den entsprechenden Filter und klicken auf die Schaltfläche [Bearbeiten]. Um
3.30 / 01-2023




                                          einen neuen Filter anzulegen, klicken Sie auf die Schaltfläche [Neu]. Es öffnet
                                          sich der Dialog Filter anlegen/bearbeiten:




                 A+W Realtime Optimizer                                                                             J-75
                 Zusammenarbeit mit anderen Modulen                                                           Tutorial




                                       Abb. J-50    Bestehenden Filter bearbeiten


                                       Geben Sie dem Filter einen aussagekräftigen Namen und achten Sie auf den
                                       korrekten Syntax des Filters. Sie können einen festen Filter definieren, z. B.
                                       pool_teile.glasart = 1004 oder einen Filter mit bis zu zwei Platzhaltern, z. B.
                                       pool_teile.glasart = [TTV1NUM]. Bei Filtern mit Platzhalter geben Sie später
                                       den gewünschten Wert selbst ein.

                                       Produktionstermin
                                       Wird hier eine Zeitspanne angegeben, werden nur Läufe angezeigt, deren
                                       Produktionstermin in dieser Zeitspanne liegt.

                                       Nachoptimierung
                                       Hier wird der Modus für die Nachoptimierung und die Menge an Bruchschei-
                                       ben, ab der dieser ausgelöst werden soll, festgelegt.

                                       Eiloptimierung
                                       Hier legen Sie fest, ob für den Lauf eine Eiloptimierung durchgeführt werden
                                       soll, wenn eine bestimmte Menge an Bruchscheiben erreicht wurde.

                                       Restplattenverwaltung
                                       Hier legen Sie fest, ob und in welchem Modus das Restblatt verlinkt werden
                                       soll.

                                       Restblatt bearbeiten
                                       Hier legen Sie fest, ob das Restblatt bearbeitet werden kann und ab welcher
                                       Länge.

                                       Gruppieren
3.30 / 01-2023




                                       Mehrere Läufe lassen sich zu einer Gruppe zusammenfassen. Läufe dersel-
                                       ben Gruppe werden im A+W Realtime Optimizer am Schneidtisch zusammen


                 J-76                                                                       A+W Realtime Optimizer
                 Tutorial                                                       Zusammenarbeit mit anderen Modulen




                                          an den Zuschnitt geschickt. Wurde für eine Gruppe der Zuschnitt begonnen,
                                          darf kein Lauf dieser Gruppe verändert werden. Ein Lauf muss einer Gruppe
                                          zugeordnet sein, um für den Zuschnitt freigegeben werden zu können.


                                           So erstellen Sie eine Gruppe für einen Lauf
                                          1 Wählen Sie den entsprechenden Tisch aus.
                                          2 Markieren Sie die gewünschten Läufe.
                                          3 Betätigen Sie die Schaltfläche [Gruppieren].
                                          4 Betätigen Sie die Schaltfläche [Freigabe].
                                          5 Die Gruppe wird erstellt und hinter die bereits freigegebenen Läufe ge-
                                            hängt.


                                           So verschieben Sie eine Gruppe für einen Lauf
                                          Freigegebene und noch nicht begonnene Läufe können in der Reihenfolge ge-
                                          ändert werden.
                                          1 Wählen Sie entsprechende Gruppe aus.
                                          2 Verschieben Sie die ausgewählte Gruppe mit den Pfeiltasten an die ge-
                                            wünschte Stelle.
                                          3 Betätigen Sie die Schaltfläche [Freigabe].
                                          4 Die Gruppe wird an die gewünschte Stelle verschoben.


                                           So lösen Sie eine Gruppe auf
                                          1 Markieren Sie die gewünschten Lose einer Gruppe.
                                          2 Betätigen Sie die Schaltfläche [Zurücksetzen].
                                          3 Betätigen Sie die Schaltfläche [Freigabe].
                                          4 Die Gruppe wird aufgelöst.

                                          Eilgruppen
                                          Eilgruppen beinhalten Läufe, die bevorzugt behandelt werden.


                                           So erstellen Sie eine Eilgruppe
                                          1 Wählen Sie die gewünschten Läufe aus.
                                          2 Betätigen Sie die Schaltfläche [Eilgruppe].
                                          3 Betätigen Sie die Schaltfläche [Freigabe]. Sollte die Eilgruppe nicht an der
                                            gewünschten Stelle stehen, können Sie diese (solange der Zuschnitt noch
                                            nicht begonnen hat) mit Hilfe der Pfeiltasten an die gewünschte Stelle ver-
                                            schieben.
3.30 / 01-2023




                                          Zurücksetzen von Läufen
                                          Bereits geplante Läufe und Einstellungen können wieder zurückgesetzt wer-
                                          den, sodass sie nicht automatisch zugeschnitten werden.


                 A+W Realtime Optimizer                                                                           J-77
                 Zusammenarbeit mit anderen Modulen                                                          Tutorial




                                       Zuschneiden
                                       Klicken Sie im A+W Realtime Optimizer Menü auf Einstellungen > Zuschnitt.
                                       Es öffnet sich der Dialog:




                                       Abb. J-51    Automatischer Zuschnitt


                                       Wählen Sie aus der Kombobox Automatisch und klicken Sie auf [OK].
                                       Öffnen Sie nun den Zuschnitt über die Symbol-Schaltfläche in der Menüleiste




                                       Sie sehen eine Übersicht über den geplanten Zuschnitt




                                       Abb. J-52    Geplanter Zuschnitt


                                       Über die Schaltfläche [Optionen] können Sie (wenn nötig) den Status der Läu-
                                       fe zurücksetzen.
                                       Klicken Sie auf die Schaltfläche [Start] um mit dem Zuschnitt zu beginnen. Die
                                       Optimierungen der ersten Gruppe werden an den Zuschnitt übergeben.
3.30 / 01-2023




                 J-78                                                                      A+W Realtime Optimizer
                 Tutorial                                                      Zusammenarbeit mit anderen Modulen




                                          Abb. J-53   Zuschnitt-Übersicht


                                          Wenn das letzte Muster der Gruppe an den Schneidtisch gesendet und zuge-
                                          schnitten wurde, wird die nächste Gruppe automatisch in den Zuschnitt gela-
                                          den.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                         J-79
                 Zusammenarbeit mit anderen Modulen                                                            Tutorial




                                       A+W Defect Optimizer
                                       … die intelligente Fehlerstellenoptimierung!
                                       In Verbindung mit z. B. einem Qualitätsscanner der Firma Viprotron werden
                                       die Lagerplatten gescannt und etwaige Fehler bzw. Fehlerstellen (Defekte)
                                       noch vor dem Beginn des Zuschnitts erkannt und visualisiert. Je früher die
                                       Fehlerstellen im Prozess erkannt werden, um so geringer sind die anfallenden
                                       Kosten.
                                       Die Fehlerstellen werden in der Optimierung für die Neu- und Restrukturierung
                                       des Schnittbildes berücksichtigt. Gibt es einzuhaltende Reihenfolgen, werden
                                       diese selbstverständlich berücksichtigt.
                                       Selbst auf Restplatten werden die Fehlerstellen gespeichert und können so
                                       später ohne erneute Kontrolle wiederverwendet werden.
                                       Lassen sich Defekte durch die Optimierung nicht vermeiden (z. B. Anzahl und
                                       Größe der Scheiben auf dem Muster), so versucht die Optimierung kleine und
                                       somit kostengünstigere Gläser auf die Defekte zu legen.
                                       Gläser, die auf Defekten liegen, werden automatisch als Bruch gemeldet und
                                       nachgeschnitten.

                                          Voraussetzung
                                          Für den Einsatz des A+W Defect Optimizers ist das Produktionssystem
                                          A+W Production sowie der A+W Realtime Optimizer Voraussetzung.


                                       Ergänzende Informationen
                                        Weitere Informationen zu dem A+W Defect Optimizer finden Sie in der entspre-
                                         chenden Dokumentation.
3.30 / 01-2023




                 J-80                                                                        A+W Realtime Optimizer
                 Tutorial                                                        Zusammenarbeit mit anderen Modulen




                                          A+W DynOpt Compact
                                          A+W DynOpt Compact ist die clevere Einstiegslösung von A+W im Bereich
                                          Dynamische Optimierung.
                                          Das System baut auf dem A+W Realtime Optimizer auf und lädt die Läufe,
                                          welche voroptimiert vom vorgelagerten Produktionssystem A+W Production
                                          gesendet werden. Diese Läufe werden komplett aufgelöst und systematisch
                                          und dynamisch neu optimiert. Dieses Verfahren verbessert den Verschnitt er-
                                          heblich und reduziert die Anzahl an zu speichernden Restplatten.
                                          Sie können A+W DynOpt Compact daher auch als automatischen A+W Real-
                                          time Optimizer sehen.
                                          A+W DynOpt Compact arbeitet mit folgenden zwei Modulen:
                                          •   A+W DynOpt Compact Import
                                          •   A+W DynOpt Compact Optimierung


                                          A+W DynOpt Compact Import
                                          Beim Import werden die für A+W DynOpt Compact freigegebenen Läufe in so
                                          genannte Cluster umgewandelt. Bei einem Cluster handelt es sich um eine,
                                          zunächst beliebige Produktionseinheit, also z. B. um ein Gestell, eine Gruppe
                                          von Gestellen oder auch um einzelne Scheibe.


                                          A+W DynOpt Compact Optimierung
                                          Nach dem Import wird, anhand des verfügbaren Platzes, die Abarbeitungsrei-
                                          henfolge der Cluster erzeugt. Diese entspricht weitgehend der Produktionsrei-
                                          henfolge, wobei in besonderen Fällen Cluster vorgezogen werden können,
                                          damit der Verschnitt verbessert wird. Sie können sowohl Fächerwagen als
                                          auch A-Böcke oder beide Gestelle zusammen verweden.
                                          Etwa die Hälfte der berechneten Cluster werden zu primären Clustern, der
                                          Rest wird zu sekundären Clustern. Die primären Cluster bekommen die Prio-
                                          rität 1 und werden in der aktuellen Optimierung komplett optimiert. Die sekun-
                                          dären Cluster dienen als Füller und die Optimierung entscheidet selbst, ob
                                          diese benötigt werden oder nicht.
                                          Beispiel:
                                          Verfügbarer Platz: 6. Der Platz für ein Fächerwagen entspricht 1, der Platz für
                                          ein A-Bock entspricht 0,5 (gerechnet in Fächerwagen, d. h. 1 Fächerwagen =
                                          2 A-Böcke.
                                          Wenn etwa genauso viele Fächerwagen wie A-Böcke zur Verfügung stehen
                                          und die Verteilung auf die Cluster übertragen wird, dann gilt: 4 Fächerwagen
                                          plus 4x0,5 A-Böcke = 6. Jeweils die Hälfte der Anzahlen ergibt je zwei primäre
                                          und zwei sekundäre Fächerwagen und A-Böcke.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-81
                 Zusammenarbeit mit anderen Modulen                                                          Tutorial




                                                        Eingelesen     Verwendet        Primär          Sekundär

                                       Fächerwagen      16             4                2               2

                                       A-Bock           17             4                2               2

                                       Tab. J-1      Beispiel

                                       Bei der Ermittlung der Timeline werden folgende Bedingungen eingehalten:
                                       •   Die primäre Sortierung der Cluster ist die Produktionsreihenfolge.
                                       •   Solange Cluster des aktuellen Laufs den verfügbaren Platz füllen können,
                                           werden keine Cluster des nachfolgenden Laufs zur Erstellung der Timeline
                                           verwendet.
                                       •   Falls man in den sekundären Clustern eine Glasart hat, die in den primären
                                           Clustern nicht vorkommt, so gibt es zwei Möglichkeiten:
                                           – Besteht der Cluster auch aus Scheiben einer Glasart, zu denen es auch
                                              primäre Scheiben gibt, so werden nur diese optimiert. Die Scheiben der
                                              Glasart, die in den primären Clustern nicht vorkommt, werden dann op-
                                              timiert, wenn der Cluster primär wird.
                                           – Besteht der Cluster komplett aus Scheiben einer Glasart, die in den pri-
                                              mären Clustern nicht vorkommt, wo wird innerhalb des aktuellen Laufes
                                              nach einem alternativen Cluster gesucht, der (zumindest teilweise) aus
                                              Scheiben einer primären Glasart besteht. Falls man einen solchen fin-
                                              det, werden die Cluster getauscht, ansonsten wird der aktuelle Cluster
                                              nicht mit optimiert.
                                       In jedem A+W DynOpt Compact-Schritt werden alle primären und alle sekun-
                                       dären Cluster zusammen der Optimierung zur Verfügung gestellt. Die primä-
                                       ren Scheiben werden stets von der Optimierung verwendet, die sekundären
                                       Scheiben nur bei Bedarf. Nach einem solchen Schritt sind alle primären Clus-
                                       ter gefüllt und können durch sekundäre und in manchen Fällen auch neue
                                       Cluster ersetzt werden. Eine Abarbeitung von mehreren Clustern sieht wie
                                       folgt aus:

                                       A+W DynOpt Compact-Lauf erzeugen
                                       A+W DynOpt Compact-Läufe können auf zwei Arten erstellt werden.
                                       •   Bilden von A+W DynOpt Compact-Läufen aus der Cluster-Ansicht.
                                       •   Bilden eines A+W DynOpt Compact-Laufes aus dem Zuschnitt heraus.


                                        Bilden von A+W DynOpt Compact-Läufen aus der Cluster-Ansicht
                                       1 Öffnen Sie den Dialog Cluster-Ansicht.
                                         Wählen Sie dazu Zuschnitt > A+W DynOpt Compact.
                                       2 Markieren Sie im linken Bereich den bzw. die Läufe, mit denen Sie einen
                                         A+W DynOpt Compact-Lauf erzeugen möchten.
                                       3 Öffnen Sie für diese Auswahl das Kontext-Menü und wählen Sie A+W Dy-
                                         nOpt Compact-Lauf erzeugen.
3.30 / 01-2023




                                       4 Nachdem die A+W DynOpt Compact-Läufe gebildet wurden, erscheinen
                                         diese im linken, oberen Bereich des Dialogs. Sie sind jetzt mit einem +-Zei-



                 J-82                                                                       A+W Realtime Optimizer
                 Tutorial                                                       Zusammenarbeit mit anderen Modulen




                                             chen versehen. Wenn Sie die Baumstruktur aufklappen, können Sie sich
                                             die Abstellplatzdaten zu den Läufen ansehen.


                                           Bilden eines A+W DynOpt Compact-Laufes aus dem Zuschnitt heraus
                                          1 Öffnen Sie den Dialog Wählen Sie einen Lauf aus.
                                            Wählen Sie dazu entweder Zuschnitt > Schneide Optimierung oder betäti-
                                            gen Sie die entsprechende Symbol-Schaltfläche.
                                          2 Markieren Sie im Bereich der Läufe den Lauf, mit dem Sie einen A+W Dy-
                                            nOpt Compact-Lauf erzeugen möchten.
                                          3 Öffnen Sie für diese Auswahl das Kontext-Menü und wählen Sie A+W Dy-
                                            nOpt Compact für Lauf XXXX erzeugen.
                                          4 Nachdem der A+W DynOpt Compact Lauf gebildet wurde, erscheint dieser
                                            im linken, oberen Bereich des Dialogs und ist mit Cut&Go gekennzeichnet.
                                            Markieren Sie den Lauf im linken Bereich, erhalten Sie im Bereich der Op-
                                            timierungen entsprechende Informationen dazu.

                                             Voraussetzung
                                             Für den Einsatz von A+W DynOpt Compact ist das Produktionssystem
                                             A+W Production sowie der A+W Realtime Optimizer Voraussetzung.


                                          Ergänzende Informationen
                                           Weitere Informationen zu dem A+W DynOpt Compact finden Sie in der entspre-
                                            chenden Dokumentation.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-83
                 Zusammenarbeit mit anderen Modulen                   Tutorial
3.30 / 01-2023




                 J-84                                 A+W Realtime Optimizer
A+W Realtime Optimizer          J

                   Softwarereferenz
                 Softwarereferenz                                                                          Übersicht




                                          Übersicht
                                          Im nachfolgenden Kapitel werden alle Dialoge beschrieben, die im A+W Real-
                                          time Optimizer insgesamt zur Verfügung stehen. Je nach Programmvariante
                                          sind manche Dialoge oder Felder in den Dialogen nicht zu sehen. Folgende
                                          Varianten sind möglich:
                                          •   In die A+W Production-Umgebung eingebetteter A+W Realtime Optimizer.
                                          •   In die A+W Production-Umgebung eingebetteter A+W Realtime Optimizer
                                              im Einsatz mit einem Remaster-Magazin.
                                          •   A+W Realtime Optimizer-Stand alone.
                                          Bei der Beschreibung des jeweiligen Dialogs ist angegeben, wenn eine Infor-
                                          mation nur für eine bestimmte Variante gilt.


                                          Menüs
                                          Nach dem Start von Realtime Optimizer erscheinen folgende Menüs:




                                          A Beim Start von A+W Realtime Optimizer
                                          Abb. J-54   Menü des A+W Realtime Optimizer


                                          In den Menüs befinden sich Funktionen, Untermenüs und Dialog-Aufrufe. In
                                          der nachfolgenden Tabelle werden die Funktionen kurz beschrieben und die
                                          Untermenüs und Dialogaufrufe genannt. Die Beschreibung der Dialoge in den
                                          nachfolgenden Kapiteln erfolgt nach Menü sortiert.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                         J-87
                 Übersicht                                                                  Softwarereferenz




                             Symbol-Schaltflächen
                             Einige Dialoge können direkt über Symbol-Schaltflächen aufgerufen werden:

                             Icon         Dialog/Funktion

                                          Öffnet den Dialog “Eilscheiben” auf Seite J-90

                                          Öffnet den Dialog “Selektieren Sie die zu optimierenden Gläser” auf
                                          Seite J-103

                                          Öffnet den Dialog “Wählen Sie einen Lauf aus” auf Seite J-125

                                          Öffnet den Dialog “Bruchpool” auf Seite J-138

                                          Öffnet den Dialog “Fehlermeldungen” auf Seite J-154

                                          Öffnet den Dialog mit Informationen zum A+W Realtime Optimizer.

                             Tab. J-2    Symbol-Schaltflächen und ihre Funktion
3.30 / 01-2023




                 J-88                                                              A+W Realtime Optimizer
                 Softwarereferenz                                                                            Erfassung




                                          Erfassung
                                          Menü Erfassung öffnen
                                          Im Menü Erfassung befinden sich folgende Programmpunkte:
                                          •   Eilscheiben:
                                              Über diesen Menüpunkt können Sie Eilscheiben direkt im Realtime Optimi-
                                              zer erfassen.
                                               Softwarereferenz, “Eilscheiben-Eingabe” auf Seite J-92
                                          •   Manueller Plan:
                                              Über diesen Menüpunkt können Sie einen rein manuellen Plan erstellen
                                              und als Tischoptimierung in der Datenbank speichern.
                                               Softwarereferenz, “Manuelle Planerstellung” auf Seite J-97
                                          •   Stammdaten:
                                              Über diesen Menüpunkt haben Sie Zugriff auf die Stammdaten. Diese sind
                                              im Handbuch A+W Production detailliert beschrieben.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-89
                 Erfassung                                                               Softwarereferenz




                             Eilscheiben
                             Erfassung > Eilscheiben




                             Abb. J-55   Eilscheiben


                             Eilscheiben können in die Tischoptimierung mit einbezogen werden. Dieser
                             Dialog zeigt Ihnen alle bereits erfassten Eilscheiben. Über die Kombobox für
                             das Feld Tisch haben Sie die Möglichkeit, sich die Eilscheiben pro Tisch oder
                             aber für alle Tische anzeigen zu lassen. Nähere Erläuterungen zu Eilscheiben
                             finden Sie im Part Feinplanung.

                             Erläuterung der Felder

                             Glasart In diesem Feld wird die Artikelnummer der Glasart angezeigt. Der
                             Wert kommt aus dem Feld Glasart des Dialoges Eilscheiben-Eingabe.

                             Dicke In diesem Feld wird die Dicke der Glasart angezeigt. Der Wert kommt
                             aus dem Feld Dicke des Dialoges Eilscheiben-Eingabe.

                             Bock In diesem Feld wird die Abstellplatznummer angezeigt. Der Wert
                             kommt aus dem Feld Bock des Dialoges Eilscheiben-Eingabe.

                             Menge In diesem Feld wird die Eilscheibenmenge angezeigt. Der Wert
                             kommt aus dem Feld Menge des Dialoges Eilscheiben-Eingabe.

                             Form Wenn es sich bei der Eilscheibe um ein Modell handelt, wird in diesem
                             Feld die Modellnummer angezeigt. Steht in dem Feld eine 0, ist die Eilscheibe
                             kein Modell. Der Wert kommt aus dem Feld Form des Dialoges Eilscheiben-
                             Eingabe.

                             Breite In diesem Feld wird die Breite der Eilscheibe angezeigt. Der Wert
                             kommt aus dem Feld Breite des Dialoges Eilscheiben-Eingabe.
3.30 / 01-2023




                             Höhe In diesem Feld wird die Höhe der Eilscheibe angezeigt. Der Wert
                             kommt aus dem Feld Höhe des Dialoges Eilscheiben-Eingabe.




                 J-90                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                            Erfassung




                                          Prio In diesem Feld wird die beim Erzeugen der Eilscheibe gewählte Priorität
                                          angezeigt. Die Standardpriorität ist 0.

                                          Alle Stationen Mit dieser Checkbox steuern Sie, welche Eilscheiben ange-
                                          zeigt werden. Normalerweise werden nur die Eilscheiben angezeigt, die mit
                                          der eigenen Arbeitsstation angelegt worden sind um diese zu bearbeiten oder
                                          zu löschen. Damit wird verhindert, dass andere Arbeitsstation diese Datensät-
                                          ze verändern oder gar löschen. Wollen Sie sich jedoch darüber informieren,
                                          welche Eilscheiben es insgesamt in der Datenbank gibt, so können Sie diese
                                          Checkbox aktivieren und bekommen eine Übersicht über alle vorhandenen
                                          Eilscheiben. Eilscheiben, die von anderen Arbeitsstation erfasst wurden, wer-
                                          den farblich gekennzeichnet und im Info-Fenster unterhalb der Checkbox Alle
                                          Stationen angezeigt.
                                           Es werden alle erfassten Eilscheiben angezeigt. Auch die, die an anderen
                                          Arbeitsstationen erfasst wurden.
                                           Es werden nur die Eilscheiben angezeigt, die an der eigenen Arbeitsstation
                                          erfasst wurden.
                                          Technische Info: Datenbankfeld: FEIN_TEILE:STATIONID

                                          Tisch Die Kombobox enthält alle in Ihrem Hause angelegten Schneidtische.
                                          Somit haben Sie die Möglichkeit, Eilscheiben gezielt für einen bestimmten
                                          Schneidtisch zu erfassen. Mithilfe der Auswahl Alle Tische verschaffen Sie
                                          sich einen Überblick über alle erfassten Eilscheiben. Markieren Sie anschlie-
                                          ßend einen Datensatz in der Liste, erscheint im grauen Bereich unterhalb der
                                          Checkbox Alle Stationen der Tisch, auf dem Eilscheibe geschnitten werden
                                          soll.

                                          Erläuterung der Schaltflächen

                                          Hinzufügen Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog
                                          Eilscheiben-Eingabe.

                                          Bearbeiten Wenn Sie diese Schaltfläche betätigen, öffnet sich für einen mar-
                                          kierten Datensatz der Dialog Eilscheiben-Eingabe.

                                          Löschen Über diese Schaltfläche löschen Sie eine zuvor markierte Eilschei-
                                          be. Es folgt eine Sicherheitsabfrage. Anschließend wird der Eintrag gelöscht.


                                          Ergänzende Informationen
                                           Tutorial, “Bruch, Eilscheiben und Füllaufträge” auf Seite J-21
                                           Softwarereferenz, “Form” auf Seite J-92
                                           Softwarereferenz, “Eilscheiben-Eingabe” auf Seite J-92
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-91
                 Erfassung                                                              Softwarereferenz




                             Eilscheiben-Eingabe
                             Erfassung > Eilscheiben > [Hinzufügen]




                             Abb. J-56   Eilscheiben


                             In diesem Dialog haben Sie die Möglichkeit, Eilscheiben zu erfassen. Nähere
                             Erläuterungen zu Eilscheiben finden Sie im Part Feinplanung.
                             Technische Info: Datenbanktabelle: FEIN_TEILE

                             Erläuterung der Felder

                             Glasart Die Kombobox listet alle in Ihrem Hause angelegten Glasarten. Wäh-
                             len Sie aus der Kombobox die entsprechende Glasart aus. Die Glasarten wer-
                             den in den Stammdaten angelegt.
                             Technische Info: Pflichtfeld, Datenbankfeld: POOL_TEILE:GLASART

                             Dicke Die Kombobox listet alle in Ihrem Hause angelegten Dicken zu der im
                             Feld Glasart gewählten Glasart. Wählen Sie aus der Kombobox den entspre-
                             chenden Dicke aus. Die Dicken werden in den Stammdaten angelegt.
                             Technische Info: Pflichtfeld, Datenbankfeld: POOL_TEILE:DICKE

                             Bock In diesem Feld geben Sie die Abstellplatznummer ein, auf den die Eil-
                             scheibe gestellt werden soll. Die Abstellplätze werden in den Stammdaten an-
                             gelegt.
                             Technische Info: Pflichtfeld, 4stellig, Datenbankfeld: FEIN_TEILE:BOCK

                             Menge In diesem Feld geben Sie die Menge der Eilscheiben ein.
                             Technische Info: Pflichtfeld, Datenbankfeld: FEIN_TEILE:MENGE

                             Form Wenn es sich bei der Eilscheibe um ein Modell handelt, geben Sie in
                             diesem Feld die vordefinierte Modell-Nr. (Modell-Katalog) ein. Haben Sie die
                             Modell-Nr. eingegeben und verlassen das Feld, öffnet sich automatisch der Di-
                             alog Form-Erfassung.
                             Technische Info: Pflichtfeld, Datenbankfeld: POOL_MODELL:MODELL_NR
3.30 / 01-2023




                 J-92                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                             Erfassung




                                          Breite In diesem Feld geben Sie die Breite der Eilscheibe ein. Handelt es sich
                                          bei der Eilscheibe um ein Modell, ist die Breite die, des umschreibenden
                                          Rechtecks.
                                          Technische Info: Pflichtfeld, Datenbankfeld: POOL_MODELL:BREITE

                                          Höhe In diesem Feld geben Sie die Höhe der Eilscheibe ein. Handelt es sich
                                          bei der Eilscheibe um ein Modell, ist die Höhe die, des umschreibenden
                                          Rechtecks.
                                          Technische Info: Pflichtfeld, Datenbankfeld: POOL_ MODELL:HOEHE

                                          Erläuterung der Schaltflächen

                                          Lupe Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog Form-Er-
                                          fassung.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Form-Erfassung” auf Seite J-94
                                           Feinplanung: Softwarereferenz, “Abstellplätze” auf Seite F-146
                                           Tutorial, “Bruch, Eilscheiben und Füllaufträge” auf Seite J-21
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-93
                 Erfassung                                                                      Softwarereferenz




                             Form-Erfassung
                             Erfassung > Eilscheiben > [Hinzufügen] > [Lupe]

                                             A       B



                                                                                            C

                                                                                            D




                             F




                                         E
                             A Benötigten Eingaben pro Modell        D Modellvorschaufenster
                             B Modell-Nummern                        E Parameterübersicht
                             C Grafische Modell-Übersicht            F Eingabefeld
                             Abb. J-57   Form-Erfassung


                             Dieser Dialog dient zur Erfassung von vordefinierten Modellen. Die mögliche
                             Auswahl hängt vom Umfang des benutzten Modellkataloges ab. Die benötig-
                             ten Eingaben für das gewählte Modell entnehmen Sie dem Fenster oben links
                             (A) in dem Dialog. Ihre Eingaben werden sofort in dem Fenster rechts (D) in
                             dem Dialog umgesetzt, das Modell proportional dargestellt. Das untere Fens-
                             ter (E) dient zur Veranschaulichung der Eingabeparameter.
                             Die Werte vor den benötigten Eingaben für das gewählte Modell haben folgen-
                             de Bedeutung:

                             Wert        Erläuterung

                             W           Breite des Modells. Bei mehreren Breiten = W, W1, W2, etc.

                             H           Höhe des Modells. Bei mehreren Höhen = H, H1, H2, etc.

                             T           Trims. Bei mehreren Trims = T, T1, T2, etc.
3.30 / 01-2023




                             Tab. J-3    Erläuterung der Eingabewerte für das gewählte Modell




                 J-94                                                                  A+W Realtime Optimizer
                 Softwarereferenz                                                                           Erfassung




                                          Wert       Erläuterung

                                          <-->       Spiegelflag. Mögliche Werte:
                                                     0: Normal
                                                     1: Um die Senkrechte gespiegelt.

                                          @          Drehflag. Mögliche Werte:
                                                     90: Drehen um 90°
                                                     180: Drehen um 180°
                                                     270: Drehen um 270°.

                                          Tab. J-3   Erläuterung der Eingabewerte für das gewählte Modell
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                         J-95
                 Erfassung                                                              Softwarereferenz




                             Modell-Nummer
                             Erfassung > Eilscheiben > [Hinzufügen] > [Lupe] > [Lupe]




                             Abb. J-58   Modell-Nummer


                             Wenn Sie die zur Erfassung benötigte Modell-Nummer nicht kennen, und
                             auch keinen Modell-Katalog in gedruckter Ausgabe zur Hand haben, können
                             Sie sich in diesem Dialog einen Überblick zu den vorhanden Modellen ver-
                             schaffen. Die Nummer des Modells aus der Form-Erfassung ist mit Punkten
                             unterlegt. Im oben abgebildeten Dialog ist das Modell-Nummer 1. Haben Sie
                             das gewünschte Modell gefunden, klicken Sie es in der Übersicht doppelt an
                             und es wird automatisch in die Feld-Nr. des Dialogs Form-Erfassung über-
                             nommen.
3.30 / 01-2023




                 J-96                                                          A+W Realtime Optimizer
                 Softwarereferenz                                                                          Erfassung




                                          Manuelle Planerstellung
                                          Erfassung > Manueller Plan




                                          Abb. J-59   Manuelle Planerstellung


                                          In diesem Dialog haben Sie die Möglichkeit, einen rein manuellen Plan zu er-
                                          stellen und als Tischoptimierung in der Datenbank zu speichern. Der manuelle
                                          Plan kann nach der Erstellung erneut editiert und geändert werden. Dies ge-
                                          schieht mithilfe des Moduls PlanEdit. Nähere Erläuterungen zu diesem Modul
                                          finden Sie in der entsprechenden Dokumentation. Es ist keine Barcodeinfor-
                                          mation für den manuellen Plan verfügbar.

                                          Erläuterung der Felder im Bereich Glasarten

                                          Glasart In diesem Feld sehen Sie die Glasart. Der Wert dieses Feldes kommt
                                          aus den Stammdaten.

                                          Dicke In diesem Feld sehen Sie die Dicke der Glasart.Der Wert dieses Fel-
                                          des kommt aus den Stammdaten.

                                          Glasart Bezeichnung In diesem Feld wird Ihnen die Klartextbezeichnung
                                          der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.

                                          Rand links Von der Optimierung nicht nutzbarer linker Rand der Lagerplatte
                                          in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

                                          Rand rechts Von der Optimierung nicht nutzbarer rechter Rand der Lager-
3.30 / 01-2023




                                          platte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

                                          Rand oben Von der Optimierung nicht nutzbarer oberer Rand der Lagerplat-
                                          te in mm. Der Wert dieses Feldes kommt aus den Stammdaten.


                 A+W Realtime Optimizer                                                                          J-97
                 Erfassung                                                               Softwarereferenz




                             Rand unten Von der Optimierung nicht nutzbarer unterer Rand der Lager-
                             platte in mm. Der Wert dieses Feldes kommt aus den Stammdaten.

                             Erläuterung der Felder im Bereich Plan

                             Lauf In diesem Feld sehen Sie die Nummer des Laufes, in dem der manuell
                             zugefügte Plan geschnitten wird.

                             Gesperrt In dieser Spalte sehen Sie, ob und von welcher Station der Lauf zur
                             Bearbeitung oder Verwendung in einer Optimierung gesperrt ist.

                             Glasart In diesem Feld sehen Sie für welche Glasart Sie einen manuellen
                             Plan hinzugefügt haben.

                             Dicke In diesem Feld sehen Sie, welche Dicke die Glasart hat, die Sie dem
                             manuellen Plan hinzugefügt haben.

                             Glasart Bezeichnung In diesem Feld wird Ihnen die Klartextbezeichnung
                             der Glasart, die Sie dem manuellen Plan hinzugefügt haben.

                             Tisch In diesem Feld sehen Sie, auf welchem Tisch der manuell hinzugefüg-
                             te Plan geschnitten wird.

                             Scheibenmenge In diesem Feld sehen Sie die Anzahl der Scheiben, die der
                             manuell hinzugefügte Plan enthält.

                             Scheibenfläche In diesem Feld sehen Sie die Fläche der Scheiben in qm,
                             die der manuell hinzugefügte Plan enthält.

                             Scheibenfläche In diesem Feld sehen Sie die Fläche der Scheiben in qm,
                             die der manuell hinzugefügte Plan enthält.

                             Platten In diesem Feld sehen Sie die Anzahl der Platten, die der manuell hin-
                             zugefügte Plan in Anspruch nimmt.

                             Verschnitt In dieser Spalte sehen Sie, wieviel Verschnitt in % bei dem manu-
                             ell hinzugefügten Plan entstehen würde.

                             Restblatt In dieser Spalte sehen Sie, wie lange das Restblatt ist, dass bei
                             dem manuell hinzugefügten Plan übrig bleibt.

                             Erläuterung der Felder im Bereich Lagerplatten

                             Breite Das Feld zeigt Ihnen die Breite der Lagerplatte in mm oder inch (kon-
                             figurierbar).

                             Höhe Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm oder inch (konfi-
                             gurierbar).
3.30 / 01-2023




                 J-98                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                           Erfassung




                                          XY? In dieser Spalte ist angegeben, in welcher Richtung die Travere gebildet
                                          wird. Mögliche Werte:
                                             X: Die Travere verläuft zwingend senkrecht zum unteren Plattenrand.
                                             Y: Die Travere verläuft zwingend parallel zum unteren Plattenrand.
                                             ?: Die Optimierung kann sich wahlweise für eine der beiden Traverenrich-
                                             tungen entscheiden.

                                          Menge Der Wert dieses Feldes zeigt Ihnen die Anzahl der zur Verfügung ste-
                                          henden Lagerplatten.

                                          Erläuterung der Felder im Bereich Restblatt

                                          Breite Falls ein Restblatt der entsprechenden Glasart/Dicke-Kombination
                                          vorhanden ist, kann das Restblatt an dieser Stelle verwendet werden. Geben
                                          Sie hier die Breite des Restblattes in mm an.

                                          Höhe Falls ein Restblatt der entsprechenden Glasart/Dicke-Kombination vor-
                                          handen ist, kann das Restblatt an dieser Stelle verwendet werden. Geben Sie
                                          hier die Höhe des Restblattes in mm an.

                                          Erläuterung der Felder und Schaltfläche im unteren Bereich

                                          Feld ohne Namen In diesem Feld sehen Sie die Nummer des Laufes, in dem
                                          der manuell zugefügte Plan geschnitten wird.

                                          Tisch In diesem Feld wird Ihnen der Tisch angezeigt, auf dem der manuell
                                          zugefügte Plan geschnitten wird.

                                          Neu Über diese Schaltfläche starten Sie das Modul PlanEdit. Nähere Infor-
                                          mationen zu diesem Modul finden Sie in der entsprechenden Dokumentation.

                                          Editieren Diese Schaltfläche ist erst aktiv, wenn Sie einen manuellen Plan
                                          hinzugefügt haben. Anschließend haben Sie die Möglichkeit, über diese
                                          Schaltfläche den hinzugefügten Plan erneut zu bearbeiten.

                                          Schneiden Über diese Schaltfläche starten Sie den Zuschnitt.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Parameter” auf Seite J-115
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-99
                 Erfassung                                                              Softwarereferenz




                             Chargen-Editor
                             Erfassung > Erfassung [F3]




                             Abb. J-60   Chargen-Editor


                             In diesem Dialog haben Sie die Möglichkeit, eine Chargen-Nummer einzuge-
                             ben.

                             Erläuterung der Felder im Bereich Lagerplatten

                             Glasart In diesem Feld sehen Sie die Glasart. Der Wert dieses Feldes kommt
                             aus den Stammdaten.

                             Dicke In diesem Feld sehen Sie die Dicke der Glasart.Der Wert dieses Fel-
                             des kommt aus den Stammdaten in mm oder inch (konfigurierbar).

                             Breite Das Feld zeigt Ihnen die Breite der Lagerplatte in mm oder inch (kon-
                             figurierbar).

                             Höhe Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm oder inch (konfi-
                             gurierbar).

                             Chargen Bezeichnung In diesem Feld wird Ihnen die eingegebene Chargen
                             Bezeichnung angezeigt.

                             Glasart Bezeichnung In diesem Feld wird Ihnen die Klartextbezeichnung
                             der Glasart angezeigt.
3.30 / 01-2023




                 J-100                                                         A+W Realtime Optimizer
                 Softwarereferenz                                                                       Erfassung




                                          Erläuterung der Felder im Bereich Chargen Bezeichnung

                                          Checkbox Wenn Sie diese Checkbox aktivieren, wird die eingegebene Char-
                                          gen Nummer auf die nachfolgenden Lagerplatten der gleichen Glasart/Dicke
                                          vererbt.

                                          Feld In diesem Feld geben Sie die Chargen Bezeichnung ein.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Chargen-Editor” auf Seite J-100
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                     J-101
                 Optimierung                                                                   Softwarereferenz




                               Optimierung
                               Menü Optimierung öffnen
                               Im Menü Erfassung befinden sich folgende Programmpunkte:
                               •   Tischoptimierung:
                                   Über diesen Menüpunkt können Sie eine Tischoptimierung erstellen.
                                    Softwarereferenz, “Selektieren Sie die zu optimierenden Gläser” auf
                                     Seite J-103
                               •   Zurücksetzen:
                                   Über diesen Menüpunkt haben Sie die Möglichkeit, Läufe zurückzusetzen.
                                    Softwarereferenz, “Zurücksetzen eines Zuschnitt Laufes” auf Seite J-119
3.30 / 01-2023




                 J-102                                                                A+W Realtime Optimizer
                 Softwarereferenz                                                                               Optimierung




                                          Selektieren Sie die zu optimierenden
                                          Gläser
                                          Optimierung > Tischoptimierung
                                          Diesen Dialog gibt es in zwei unterschiedlichen Varianten. Welche Variante
                                          angezeigt wird, hängt davon ab, welche Einstellungen Sie für die Tischopti-
                                          mierung getroffen haben:
                                          •   Standard
                                          •   Produktionstermin
                                           Kapitel “Tischoptimierung” auf Seite J-151


                                          Tischoptimierung in der Variante Standard




                                          Abb. J-61    Selektieren Sie die zu optimierenden Gläser - Standard


                                          In diesem Dialog listet Ihnen A+W Realtime Optimizer alle Glasarten auf, für
                                          die Läufe und Eilscheiben zur Optimierung bereit stehen. Zu der gewählten
                                          Glasart werden die verfügbaren Läufe angezeigt.

                                          Erläuterung der Felder im Bereich Verfügbare Glasarten

                                          Glasart Dieses Feld zeigt Ihnen die Artikelnummer der Glasart, für die Läufe
                                          verfügbar sind. Der Wert dieses Feldes kommt aus den Stammdaten.

                                          Dicke In diesem Feld wird die Dicke der Glasart angezeigt. Der Wert dieses
                                          Feldes kommt aus den Stammdaten.

                                          Restelager Diese Spalte wird nur angezeigt, wenn Ihr A+W Realtime Optimi-
3.30 / 01-2023




                                          zer zur Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde. In
                                          dieser Spalte steht ein Eintrag, wenn im Restelager-Magazin eine Scheibe der
                                          entsprechenden Glasart und Dicke vorhanden ist. Die angegebene Zahl ist die


                 A+W Realtime Optimizer                                                                              J-103
                 Optimierung                                                               Softwarereferenz




                               Länge des Restblattes in mm im Restelager-Magazin. Wenn im Restelager-
                               Magazin mehrere Restblätter der entsprechenden Glasart und Dicke liegen,
                               dann wird das längste Restblatt hier angezeigt.

                               Bruchmenge Wenn für diese Glasart Bruchscheiben erfasst sind, wird in die-
                               sem Feld die Anzahl der Bruchscheiben angegeben.

                               Bruchfläche Wenn für diese Glasart Bruchscheiben erfasst sind, wird in die-
                               sem Feld die Gesamtfläche der Bruchscheiben angegeben.

                               Eilmenge Wenn für diese Glasart Eilscheiben erfasst sind, wird in diesem
                               Feld die Anzahl der Eilscheiben angegeben.

                               Eilfläche Wenn für diese Glasart Eilscheiben erfasst sind, wird in diesem
                               Feld die Gesamtfläche der Eilscheiben angegeben.

                               Glasart Bezeichnung In diesem Feld wird Ihnen die Klartextbezeichnung
                               der Glasart angezeigt. Der Wert dieses Feldes kommt aus den Stammdaten.

                               Erläuterung der Felder im Bereich Verfügbare Optimierungen

                               Lauf In dieser Spalte sehen Sie die Nummer des Laufes, der Optimierungen
                               für die gewählte Glasart enthält.

                               Los In dieser Spalte sehen Sie die Losnummer des Laufes, der die Opti-
                               mierungen für die gewählte Glasart enthält.

                               Gesperrt In dieser Spalte sehen Sie, ob und von welcher Station das Los zur
                               Bearbeitung oder Verwendung in einer Optimierung gesperrt ist.

                               Parameter In dieser Spalte sehen Sie, für welchen Tisch das angezeigte Los
                               optimiert wurde.

                               Platten In dieser Spalte sehen Sie, wieviele Lagerplatten die Losoptimierung
                               benötigt.

                               Scheibenmenge In dieser Spalte sehen Sie, wieviele Scheiben die Losopti-
                               mierung beinhaltet.

                               Scheibenfläche In dieser Spalte sehen Sie, wieviele Quadratmeter Glas die
                               Losoptimierung beinhaltet.

                               Verschnitt In dieser Spalte sehen Sie, wieviel Verschnitt in % bei der aktuel-
                               len Losoptimierung entstehen würde.

                               Rest (mm) In dieser Spalte sehen Sie, wie lange das Restblatt ist, dass bei
                               der Losoptimierung auf dem Schneidtisch übrig bleibt.

                               Information In dieser Spalte werden Ihnen Laufbezeichnung angezeigt.
3.30 / 01-2023




                               Termin In dieser Spalte sehen Sie den Produktionstermin, der bei der Lauf-
                               erstellung durch die Kapazitätsplanung ermittelt wurde.



                 J-104                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                          Optimierung




                                          Schicht In dieser Spalte sehen Sie die Produktionsschicht, die bei der Lauf-
                                          erstellung durch die Kapazitätsplanung ermittelt wurde.

                                          Erläuterung der Checkbox

                                          Erlaube Handzuschnitt Wenn diese Checkbox markiert ist, dann werden in
                                          der Liste Glasarten auch die Glasarten zur Optimierung angezeigt, die bei der
                                          Artikeldefinition in den Stammdaten nur für Handzuschnitt vorgesehen wur-
                                          den.
                                           nur Glasarten für den automatischen Zuschnitt anzeigen
                                           auch Glasarten für den Handzuschnitt anzeigen
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-105
                 Optimierung                                                                   Softwarereferenz




                               Tischoptimierung in der Variante Produktionster-
                               min




                               Abb. J-62    Selektieren Sie die zu optimierenden Gläser - Produktionstermin


                               Dieser Dialog zeigt die Produktionstermine und ermöglicht es Ihnen, die Opti-
                               mierungen nach den Produktionstermin zu filtern. Dies erleichtert die Einhal-
                               tung von Fristen und die Planung des Produktionsablaufs.
                               Wählen Sie zunächst einen Produktionstermin aus der Liste Produktionsda-
                               tum.
                               Im Bereich Verfügbare Glasarten werden Ihnen alle Glasarten angezeigt, die
                               in Optimierungen mit dem ausgewählten Produktionsdatum enthalten sind.
                               Wählen Sie anschließend die Glasart aus, die Sie schneiden möchten.
                               Im Bereich Verfügbare Optimierungen werden Ihnen alle Optimierungen an-
                               gezeigt, die bis zum ausgewählten Produktionsdatum produziert sein sollten.
                               Für eine bessere Übersicht sind die Optimierungen sind farbig markiert:
                               •   Grün: Der Produktionstermin liegt in der Zukunft.
                               •   Gelb: Der Produktionstermin ist heute.
                               •   Rot: Der Produktionstermin liegt in der Vergangenheit.
                               Die Felder der Bereiche Verfügbare Glasarten und Verfügbare Optimierungen
                               sind identisch mit den Feldern im Dialog Tischoptimierung in der Variante
                               Standard und werden an dieser Stelle erläutert.
                                Kapitel “Tischoptimierung in der Variante Standard” auf Seite J-103


                               Ergänzende Informationen
                                Tutorial, “Läufe zum Zuschnitt auswählen” auf Seite J-40
3.30 / 01-2023




                 J-106                                                                 A+W Realtime Optimizer
                 Softwarereferenz                                                                            Optimierung




                                          Tischoptimierung Lauf [Nr]
                                          Mit diesem Dialog werden verschiedene Parameter für die Optimierung einge-
                                          stellt. Der Dialog ist in folgende Register unterteilt:
                                          •   Übersicht
                                          •   Optimieren
                                          •   Restplatten und Lagerplatten
                                          •   Parameter


                                          Übersicht
                                          Optimierung > Tischoptimierung > Gläser selektieren - [Auswählen] > Über-
                                          sicht




                                          Abb. J-63    Tischoptimierung - Übersicht


                                          Dieser Dialog zeigt die im Dialog Selektieren Sie die zu optimierenden Gläser
                                          gewählten Läufe an. Wurde eine Optimierung durchgeführt, so wird deren Er-
                                          gebnis angezeigt. Wenn noch keine Optimierung durchgeführt wurde, sind die
                                          Felder Platten, Verschnitt und Rest (mm) leer.
                                          Nach einer durchgeführten Optimierung, kann per Doppelklick auf die Glasart
                                          das Programm PlanEdit gestartet werden, falls dieses an Ihrem Arbeitsplatz
                                          installiert ist. PlanEdit zeigt Ihnen das Brechbild der Lagerplatte grafisch an.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-107
                 Optimierung                                                               Softwarereferenz




                               Erläuterungen der oberen Liste

                               Glasart In diesem Feld werden Ihnen die Artikelnummern der Glasarten an-
                               gezeigt, die in der gewählten Tischoptimierung enthalten sind. Der Wert die-
                               ses Feldes kommt aus den Stammdaten.

                               Dicke In diesem Feld wird Ihnen die Dicke der Glasart angezeigt. Der Wert
                               dieses Feldes kommt aus den Stammdaten in mm oder inch (konfigurierbar).

                               Parameter Wenn die Optimierung durchgeführt wurde, dann sehen Sie in
                               diesem Feld, mit welchen Optimierungsparametern die Optimierung durchge-
                               führt wurde.

                               Menge Der Wert dieses Feldes zeigt Ihnen die Anzahl der Scheiben.

                               Fläche In diesem Feld sehen Sie die gesamte Fläche der optimierten Glasart
                               in Quadratmeter.

                               Platten Diese Feld zeigt Ihnen die Anzahl der Lagerplatten, die für die Opti-
                               mierung benötigt werden (Anzeige erst nach durchgeführter Optimierung).

                               Verschnitt In diesem Feld sehen Sie die Glasfläche in %, die als Verschnitt
                               anfällt (Anzeige erst nach durchgeführter Optimierung).

                               Rest (mm) Hier sehen Sie die Breite des Restblatts in mm, das nach dem Zu-
                               schnitt noch auf dem Tisch liegt und weiterverwendet werden könnte (Anzeige
                               erst nach durchgeführter Optimierung).

                               Erläuterungen der unteren Liste

                               Lauf Das Feld zeigt Ihnen die Nummer der Läufe, von denen ein Los in der
                               angezeigten Tischoptimierung enthalten ist.

                               Los Das Feld zeigt Ihnen die Nummer des Loses, dessen Scheiben in der an-
                               gezeigten Tischoptimierung enthalten sind.

                               Zuschnitts-Böcke In diesem Feld sehen Sie die Anzahl der Zuschnittsbö-
                               cke, die von der Feinplanung für die Scheiben dieses Losen eingeplant wur-
                               den.

                               Sonderglaslauf Hier wird angegeben, ob es sich um einen Sonderglaslauf
                               handelt. Ein Sonderglaslauf liegt dann vor, wenn die gewählte Glasart in den
                               Stammdaten als Sonderglas definiert wurde. Mögliche Werte:
                               • Ja
                               • Nein

                               Platten In diesem Feld sehen Sie die Anzahl an Lagerplatten, die für den Zu-
                               schnitt des Loses ermittelt wurden. Es handelt sich hierbei um das Berech-
                               nungsergebnis der Feinplanung, nicht der Tischoptimierung.
3.30 / 01-2023




                 J-108                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                        Optimierung




                                          Verschnitt Das Feld zeigt Ihnen die Glasfläche in %, die beim Zuschnitt des
                                          Loses als Verschnitt anfällt. Es handelt sich hierbei um das Berechnungser-
                                          gebnis der Feinplanung, nicht der Tischoptimierung.

                                          Rest (mm) In diesem Feld sehen Sie die Breite des Restblatts in mm, das
                                          nach dem Zuschnitt des Loses noch auf dem Tisch liegt und weiterverwendet
                                          werden könnte. Es handelt sich hierbei um das Berechnungsergebnis der
                                          Feinplanung, nicht der Tischoptimierung.


                                          Ergänzende Informationen
                                           Tutorial, “Tischoptimierungen erstellen” auf Seite J-29
                                           Tutorial, “Tischoptimierungen” auf Seite J-29
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                        J-109
                 Optimierung                                                             Softwarereferenz




                               Optimieren
                               Optimierung > Tischoptimierung > Gläser selektieren - [Auswählen] > Optimie-
                               ren




                               Abb. J-64   Optimieren


                               In diesem Dialog nehmen Sie die Einstellungen für die Optimierung vor. Die
                               Liste liefert Ihnen Informationen zu der gewählten Glasart.

                               Erläuterung der Felder im Bereich Optimierungsreihenfolge

                               Lauf In diesem Feld sehen Sie, welcher Lauf bzw. welche Läufe optimiert
                               werden sollen.

                               Los Dieses Feld zeigt Ihnen, die Losnummer der einzelnen Läufe.

                               Rang Dieses Feld zeigt Ihnen den Optimierungsrang. Durch Betätigen der
                               Schaltflächen ∧ oder ∨ können Sie Rangfolge ändern. Gleiche Ränge werden
                               gemischt, unterschiedliche getrennt.

                               Positionen In diesem Feld sehen Sie, wie viele Positionen in dem Lauf ent-
                               halten sind.

                               A-Böcke Das Feld zeigt Ihnen die Anzahl der A-Böcke, die für diesen Lauf
                               notwendig sind.

                               Fächerwagen Das Feld zeigt Ihnen die Anzahl der Fächerwagen, die für die-
3.30 / 01-2023




                               sen Lauf notwendig sind.

                               Scheibenmenge Das Feld zeigt Ihnen die Anzahl Scheiben, die in diesem
                               Lauf enthalten sind.

                 J-110                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                         Optimierung




                                          Scheibenfläche Das Feld zeigt Ihnen die Scheibenfläche in qm, die in die-
                                          sem Lauf enthalten sind.

                                          Platten Das Feld zeigt Ihnen die Anzahl der Platten, die zum Schneiden die-
                                          ses Laufes notwendig sind.

                                          Erläuterung der Schaltflächen im Bereich Rangfolge

                                          ˄ Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie z. B. einen
                                          Lauf mit dem Rang 1 gewählt und betätigen dann die Schaltfläche ˄, ändert
                                          sich der Rang von 1 nach 2. Gleichzeitig ändert sich gegebenenfalls die Sor-
                                          tierung der Tabelle.

                                          ˅ Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie z. B. einen
                                          Lauf mit dem Rang 1 gewählt und betätigen dann die Schaltfläche ˅, ändert
                                          sich der Rang von 2 nach 1. Gleichzeitig ändert sich gegebenenfalls die Sor-
                                          tierung der Tabelle.

                                          Auswählen Mit dieser Kombobox steuern Sie den Rang. Die Kombobox ent-
                                          hält soviel Ränge, wie Läufe in der Tabelle zu sehen sind. Sie können dann
                                          aus der Tabelle einen Lauf auswählen, die Kombobox öffnen und dem ausge-
                                          wählten Lauf den gewünschten Rang zuweisen. Die Ränge sind fortlaufend zu
                                          vergeben, d. h. es kann kein Rang übersprungen werden. Nach Rang 1 folgt
                                          Rang 2 und danach Rang 3. Rang 2 kann nicht übersprungen werden. Haben
                                          Sie einem Lauf einen niederen Rang zugewiesen, ändert sich ebenfalls die
                                          Sortierung der Tabelle.

                                          Erläuterung der Felder im Bereich Automatische Zusammenstel-
                                          lung

                                          Lose trennen Mit dieser Checkbox steuern Sie, ob ein Trennen der Lose ge-
                                          wünscht ist oder nicht. Mögliche Werte:
                                           Lose werden nicht getrennt.
                                           Lose werden getrennt. Wenn Sie die Checkbox aktivieren, hat das u. U.
                                          Auswirkung auf das Feld Rang.

                                          Lose nach maximaler Anzahl der Zuschnittsböcke trennen Mit dieser
                                          Checkbox steuern Sie, ob und wenn ja wann Lose getrennt werden. Wenn Sie
                                          wünschen, dass Lose nach einer gewissen Anzahl von Zuschnittsböcken ge-
                                          trennt werde, müssen Sie die Checkbox aktivieren und im Feld dahinter die
                                          Menge eingeben, nach der getrennt werden soll.

                                          Mindestscheibenfläche für das Trennen von Losen verwenden Mit die-
                                          ser Checkbox steuern Sie, ob und wenn ja wann Lose getrennt werden. Wenn
                                          Sie wünschen, dass Lose ab einer gewissen Scheibenfläche (in qm) getrennt
                                          werde, müssen Sie die Checkbox aktivieren und im Feld dahinter die Fläche
                                          eingeben, nach der getrennt werden soll.
3.30 / 01-2023




                                             Trennen von Losen
                                             Lose können entweder nach einer maximalen Anzahl von Zuschnittsbö-
                                             cken oder einer Mindestscheibenfläche getrennt werden. Beide Checkbo-
                                             xen können zusammen nicht aktiviert werden.


                 A+W Realtime Optimizer                                                                         J-111
                 Optimierung                                                                   Softwarereferenz




                               Erläuterung der Felder im Bereich Lauf-Parameter

                               XOPT-S Verwenden Sie in Ihrem Betrieb A-Böcke, dann muss dieser Para-
                               meter gesetzt werden. Die Optimierung berücksichtigt dann, dass die Schei-
                               ben auf A-Böcke gestellt werden und für die nachfolgende Bearbeitungen in
                               einer bestimmten Reihenfolge stehen müssen.

                               Bruchscheiben Wenn Sie diesen Parameter wählen, dann lassen Sie zu,
                               dass immer dann, wenn zu der gewählten Glasart Bruchscheiben existieren,
                               diese automatisch in die anstehende Optimierung mit einbezogen werden.

                               Eilscheiben Wenn Sie diesen Parameter wählen, dann lassen Sie zu, dass
                               immer dann, wenn zu der gewählten Glasart Eilaufträge existieren, diese au-
                               tomatisch in die anstehende Optimierung mit einbezogen werden.

                               Füller nur für Lücken Existieren in Ihrem System Füllaufträge der gleichen
                               Glasart und haben Sie diesen Parameter gesetzt, dann werden bei der Opti-
                               mierung eventuell vorhandene Lücken in der Optimierung mit Füllaufträgen
                               gefüllt. Das Restblatt wird nicht mit Füllaufträgen aufgefüllt. Existieren Füllauf-
                               träge zur gewählten Glasart, so werden diese im Register Füller angezeigt.

                               Restelager Diese Checkbox wird nur angezeigt, wenn Sie über ein entspre-
                               chendes Restelager verfügen.
                                Das Restelager wird nicht verwendet
                                Das Restelager wird verwendet

                               Erläuterung der Felder im Bereich Tisch

                               Tisch Die Kombobox enthält alle in Ihrem Hause konfigurierten Tische. Wäh-
                               len Sie aus der Kombobox den entsprechenden Tisch aus. Im darunter liegen-
                               den Bereich wird Ihnen der Name des Tisches angezeigt.

                               Erläuterung der Felder im Bereich Optimierungs-Parameter

                               Optimierungsparameter Die Kombobox enthält die Optimierungsparame-
                               ter, mit denen die Optimierung erstellt werden soll. Es stehen nur die Optimie-
                               rungsparameter zur Verfügung, mit denen der ausgewählte Tisch arbeiten
                               kann. Wählen Sie aus der Kombobox den entsprechenden Parameter aus. Im
                               darunter liegenden Bereich wird Ihnen der Name des Parameters angezeigt.

                               Erläuterung der Schaltflächen

                               Optimieren Mit dieser Schaltfläche starten Sie die Optimierung. Die Optimie-
                               rung läuft im Hintergrund. Sobald das Ergebnis vorliegt, kann es im Register
                               Übersicht angesehen werden. Das Optimierungsergebnis wird erst dann in die
                               Datenbank gespeichert, wenn die Schaltfläche [Speichern] oder [Schneiden]
                               betätigt wird.
3.30 / 01-2023




                               Ergänzende Informationen
                                Tutorial, “Tischoptimierungen” auf Seite J-29




                 J-112                                                                A+W Realtime Optimizer
                 Softwarereferenz                                                                              Optimierung




                                          Restplatten und Lagerplatten
                                          Optimierung > Tischoptimierung > Restplatten und Lagerplatten




                                          Abb. J-65    Restplatten und Lagerplatten


                                          In diesem Dialog wählen Sie für die zuvor ausgewählte Glasart die Restplatten
                                          und die Lagerplatten aus, die Sie für die Optimierung verwenden möchten. Auf
                                          der linken Seite sehen Sie die gewählte Glasart. Die rechte Seite zeigt Ihnen
                                          die zur Glasart passende(n) Lagerplatte oder, wenn vorhanden, die passen-
                                          den Restplatten. Diese sind nach Verfügbarkeit sortiert und gruppiert im Sinne
                                          der Entladereihenfolge des Gestells.

                                          Erläuterung der Felder im Bereich Liste Lagerplatten (rechts)

                                          Breite Das Feld zeigt Ihnen die Breite der Lagerplatte in mm.

                                          Höhe Das Feld zeigt Ihnen die Höhe der Lagerplatte in mm.

                                          XY? In dieser Spalte ist angegeben, in welcher Richtung die Travere gebildet
                                          wird. Mögliche Werte:
                                          • X: Die Travere verläuft zwingend senkrecht zum unteren Plattenrand.
                                          • Y: Die Travere verläuft zwingend parallel zum unteren Plattenrand.
                                          • ?: Die Optimierung kann sich wahlweise für eine der beiden Traverenrich-
                                             tungen entscheiden.

                                          Restelagerfach Das Feld zeigt Ihnen, wo sich die Lagerplatte befindet. Steht
                                          in diesem Feld der Begriff Lager, handelt es sich bei der Platte um eine Lager-
                                          platte. Steht in dem Feld eine Ziffer, z. B. 2, dann handelt es sich bei der Platte
                                          um eine Restlagerplatte, die sich im Restelagerfach mit der Nummer 2 befin-
3.30 / 01-2023




                                          det. Steht in dem Feld WH (Warehouse) befindet sich die Platte in einem ver-
                                          tikalen Remaster. Steht in dem Feld RM, befindet sich die Platte in einem
                                          (horizontalen) Remaster.



                 A+W Realtime Optimizer                                                                               J-113
                 Optimierung                                                               Softwarereferenz




                               Einlagerzeit / Menge Wenn es sich bei der Platte um eine Restlagerplatte
                               handelt, können Sie in diesem Feld das Datum und die Uhrzeit der Einlage-
                               rung (in das Restelager) sehen. Steht in dem Feld eine Zahl, z. B. 7670, dann
                               handelt es sich bei der Platte um eine Lagerplatte, von der noch 7670 Stück
                               auf Lager sind.

                               Erläuterung der Felder im Bereich Restblatt

                               Höhe/Breite Liegt auf dem Zuschnitttisch vom vorherigen Zuschnitt noch ein
                               Restblatt der gleichen Glasart und Dicke, so können Sie dieses weiter verwen-
                               den. Geben Sie hier Höhe und Breite des Restblatts ein. Die Optimierung nutzt
                               dann zuerst dieses Restblatt aus, bevor eine neue Lagerplatte verwendet
                               wird.

                                  Restblatt und Restelager-Platte nicht gleichzeitig möglich!
                                  Wenn Sie bereits eine Restelager-Platte verwenden, kann kein Restblatt
                                  mehr verwendet werden. Wenn Ihr A+W Realtime Optimizer zur Zusam-
                                  menarbeit mit einem Restelager-Magazin konfiguriert wurde, dann kann
                                  die Verwendung einer Restelager-Platte im Register Optimieren mit der
                                  Checkbox Verwenden ein- und ausgeschaltet werden.


                               Ergänzende Informationen
                                Tutorial, “A+W Residual Stock Manager” auf Seite J-50
3.30 / 01-2023




                 J-114                                                              A+W Realtime Optimizer
                 Softwarereferenz                                                                          Optimierung




                                          Parameter
                                          Optimierung > Tischoptimierung > Parameter




                                          Abb. J-66    Parameter


                                          In diesem Dialog nehmen Sie die Parameter-Einstellungen für die Tischopti-
                                          mierung vor. Die Liste zeigt Ihnen die für die Optimierung zur Verfügung ste-
                                          henden Lagerplatten.

                                          Erläuterung der Felder im Bereich Beschichtung

                                          Keine/Oben/Unten Falls die Lagerplatte über eine Beschichtung verfügt, ge-
                                          ben Sie mit diesen Radiotasten an, ob sich die Beschichtung oben oder unten
                                          befindet. Hat die Lagerplatte keine Beschichtung, aktivieren Sie die Radiotas-
                                          te Keine.

                                          Erläuterung der Schaltfläche

                                          Anzahl Mit dieser Schaltfläche öffnen Sie den Dialog Anzahl der Lagerplat-
                                          ten.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-115
                 Optimierung                                                               Softwarereferenz




                               Erläuterung der Felder im Bereich Optimierungs-Parameter

                               Ränder Die Felder Rand links, Rand rechts, Rand oben und Rand unten zei-
                               gen Ihnen die für den entsprechenden Glasartikel erfassten Bruchränder. Die
                               grau unterlegten Felder beziehen sich auf die aus den Glasartikel-Stammda-
                               ten gezogenen Werte. In den weiß unterlegten Feldern können Sie diesen
                               Wert überschreiben. Es handelt sich dabei um ein temporäres Ändern der
                               Bruchrändern für den jeweiligen Lauf.

                               Autotravere Die Checkbox steuert, ob die angegebene maximale Traveren-
                               breite vergrößert werden darf.
                                Die angegebene maximale Traverenbreite darf vergrößert werden.
                                Die angegebene maximale Traverenbreite darf nicht vergrößert werden.

                               Max. Travere Das Feld Max. Travere bezieht sich auf die maximale Traver-
                               enbreite des gewählten Glasartikels. Das grau unterlegte Feld bezieht sich auf
                               den aus dem Glasartikel-Stammdaten gezogenen Wert. In dem weiß unterleg-
                               ten Feld können Sie diesen Wert überschreiben. Es handelt sich dabei um ein
                               temporäres Ändern der maximalen Traverenbreite für den jeweiligen Lauf.

                               Schneidmodus Das Feld legt den Schneidmodus für die XOPT(S)-Opti-
                               mierungen fest. Die gesetzte Radiotaste zeigt Ihnen, mit welchem Schneid-
                               modus die Feinplanung durchlaufen wurde. Die Auswahl des richtigen
                               Schneidmodus richtet sich nach dem Schneidtisch und den betrieblichen An-
                               forderungen. Generell gilt, dass mit Schneidmodus 1 die besten und mit
                               Schneidmodus 4 geringfügig schlechtere Verschnittergebnisse entstehen.
                               Diese höheren Materialverluste lassen sich unter Umständen durch schnelle-
                               res Brechen und Abräumen (aufgrund des einfacheren Schneidmodus) kom-
                               pensieren. Der Schneidmodus bestimmt die Lage der Scheiben innerhalb
                               einer Travere zwischen zwei benachbarten Y- Schnitten. Mögliche Werte:
                               • 1: Zwischen zwei Y-Schnitten dürfen Scheiben verschiedener Breite und
                                  Höhe nebeneinander liegen. Es können also auch W - Schnitte vorkom-
                                  men.
                               • 2: Zwischen zwei Y-Schnitten dürfen nur Scheiben mit unterschiedlicher
                                  Breite aber gleicher Höhe nebeneinander liegen.
                               • 3: Zwischen zwei Y-Schnitten dürfen nur Scheiben der gleichen Position
                                  nebeneinander liegen.
                               • 4: Zwischen zwei Y-Schnitten dürfen höchstens zwei Scheiben der glei-
                                  chen Position nebeneinander liegen.
                               • 5-7: Spezialmodus für einen Coopmes-Tisch. Dieser Modus ist identisch
                                  mit Modus 2-4.
3.30 / 01-2023




                 J-116                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                         Optimierung




                                          Erläuterung der Schaltflächen

                                          PlanEdit Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung durch-
                                          geführt haben. Betätigen Sie diese Schaltfläche, öffnet sich das Programm
                                          PlanEdit.

                                          Schneiden Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung
                                          durchgeführt haben. Betätigen Sie diese Schaltfläche, starten Sie den Zu-
                                          schnitt.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Anzahl der Lagerplatten” auf Seite J-118
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                         J-117
                 Optimierung                                                           Softwarereferenz




                               Anzahl der Lagerplatten
                               Optimierung > Tischoptimierung > Parameter > [Anzahl]




                               Abb. J-67   Anzahl der Lagerplatten


                               In diesem Dialog sehen Sie die Anzahl der zur Verfügung stehenden Lager-
                               platten für die gewählte Glasart.
3.30 / 01-2023




                 J-118                                                          A+W Realtime Optimizer
                 Softwarereferenz                                                                              Optimierung




                                          Zurücksetzen eines Zuschnitt Laufes
                                          Optimierung > Zurücksetzen




                                          Abb. J-68     Zurücksetzen eines Zuschnitt Laufes


                                          Mit diesem Dialog können Sie Läufe, die bereits begonnen oder produziert
                                          wurden, wieder zurücksetzen und erneut bearbeiten. Tischoptimierungen, die
                                          bereits gespeichert wurden, können hier wieder aufgelöst werden. Läufe, die
                                          bereits produziert sind aber nicht gebucht wurden, können als produziert ge-
                                          bucht werden. Die Löschroutinen für alte (produzierte) Läufe übernimmt der
                                          ALCIMServer. Informationen zum Löschen von Läufen finden Sie in der zuge-
                                          hörigen Dokumentation.

                                          Erläuterung der Liste Läufe

                                          Lauf Hier werden die Nummern der Läufe angezeigt, deren Status verändert
                                          werden kann. Die Nummern 1000 - 9999 stehen für fertig optimierte Läufe (z.
                                          B. aus A+W Production), die zum Schneiden zur Verfügung stehen. Die Num-
                                          mern 15000 - 19999 (Nummernkreise konfigurierbar) sind für selbst erstellte
                                          Tischoptimierungen reserviert.

                                          Gesperrt In dieser Spalte erscheint ein Eintrag, wenn ein anderes A+W Real-
                                          time Optimizer oder ein anderer Prozess den entsprechenden Lauf in Bearbei-
                                          tung hat.

                                          Status Hier wird angezeigt, in welchen Bearbeitungsstand sich die einzelnen
                                          Läufe befinden. Folgende Anzeigen sind hier möglich:

                                          Status              Bedeutung

                                          Freigegeben         Es liegt eine Optimierung vor, die zum Zuschnitt
                                                              freigegeben ist. Solche Läufe können in einer
                                                              Tischoptimierung weiterbearbeitet werden, bevor der
                                                              Zuschnitt erfolgt.
3.30 / 01-2023




                                          Tab. J-4      Status der Läufe




                 A+W Realtime Optimizer                                                                             J-119
                 Optimierung                                                                    Softwarereferenz




                               Status              Bedeutung

                               Begonnen            Die Bearbeitung des Laufes wurde begonnen. Es sind
                                                   Lose aus diesem Lauf bereits beim Zuschnitt oder in einer
                                                   Tischoptimierung. Auch wenn eine Tischoptimierung nicht
                                                   geschnitten, sondern wieder aufgelöst wurde, wird dieser
                                                   Status angezeigt.

                               Produziert          Der Lauf wurde produziert.

                               Tab. J-4     Status der Läufe

                               Erläuterung der Schaltflächen

                               Produziert Wenn ein freigegebener Lauf markiert ist und diese Schaltfläche
                               gewählt wird, dann wird der Lauf als produziert markiert und steht für die Op-
                               timierung nicht mehr zur Verfügung.

                               OK Wenn eine freigegebene Tischoptimierung (Lauf ab Nr. 15000) (konfigu-
                               rierbar) markiert ist und diese Schaltfläche gewählt wird, dann wird die Tisch-
                               optimierung aufgelöst. Die enthaltenen Läufe, Bruchscheiben, Eilscheiben
                               oder Füllscheiben stehen für neue Optimierungen wieder zur Verfügung. Vor
                               der Ausführung dieser Funktion erfolgt eine Sicherheitsabfrage.
                               Wenn ein produzierter Lauf markiert ist und diese Schaltfläche gewählt wird,
                               dann wird der Lauf zurückgesetzt und kann erneut produziert werden.


                               Ergänzende Informationen
                                Tutorial, “Schneidstatus zurücksetzen” auf Seite J-48
3.30 / 01-2023




                 J-120                                                                   A+W Realtime Optimizer
                 Softwarereferenz                                                                           Optimierung




                                          Pausierende Glasarten
                                          Optimierung > DynOpt Einstellungen




                                          Abb. J-69    Pausierende Glasarten


                                          Wird ein Lauf in das DynOpt importiert, muss sichergestellt werden, dass es
                                          genug Glasplatten dieser Glasart auf Lager gibt. Sie dürfen auf keinen Fall ei-
                                          nen Lauf importieren, der die fehlenden Glasarten enthält.
                                          Manchmal kommt jedoch vor, dass Sie erst während der Produktion feststel-
                                          len, dass einige Glasarten nicht zur Verfügung stehen. Mit diesem Dialog ha-
                                          ben Sie jetzt die Möglichkeit, die einzelnen Glasarten zu sperren oder aus der
                                          Produktion zu entfernen. Der Dialog zeigt Ihnen alle Glasarten, die sich in der
                                          Produktion befinden.

                                          Erläuterung der einzelnen Felder

                                          Filter Mithilfe dieser Kombobox können Sie Liste der Glasarten einschrän-
                                          ken. Folgende Werte stehen zur Verfügung:
                                          • Alle: Es werden alle Glasarten angezeigt, die sich in der Produktion befin-
                                              den.
                                          • Gesperrt: Es werden nur gesperrte Glasarten angezeigt.
                                          • Dringend: Es werden nur dringende Glasarten angezeigt. Unter dringend
                                              versteht man solche Scheiben dieser Glasart, die vor den DynOpt Aus-
3.30 / 01-2023




                                              gangslinien warten.




                 A+W Realtime Optimizer                                                                           J-121
                 Optimierung                                                               Softwarereferenz




                               Ausgang Diese Kombobox ist nur aktiv, wenn Sie in der Kombobox Filter die
                               Einstellung Dringend gewählt haben. Sie haben dann die Möglichkeit, sich die
                               dringenden Glasarten pro Ausgang anzeigen zu lassen. Hierzu müssen die
                               Ausgänge entsprechend konfiguriert werden.

                               Grund für das Pausieren Um eine Glasart zu sperren, markieren Sie diese
                               und wählen aus der Kombobox den Grund aus.

                               Optimierung stoppen Über diese Schaltfläche stoppen Sie die Optimierung.
                               Das ist nötig, wenn Sie eine Glasart komplett aus der Produktion entfernen
                               möchten. Dazu müssen Sie zunächst die Optimierung stoppen und dann die
                               Glasart entfernen.

                               Entfernen Diese Schaltfläche ist nur aktiv, wenn Sie für eine Glasart die Op-
                               timierung gestoppt haben. Anschließend können Sie die Glasart entfernen.

                               Sperren Über diese Schaltfläche sperren Sie eine Glasart für den nächsten
                               Optimierungsvorgang. Wählen Sie zunächst die Glasart, dann den Grund und
                               klicken Sie dann auf [Sperren].

                               Freigeben Über diese Schaltfläche geben Sie eine gesperrte Glasart wieder
                               frei. Wählen Sie zunächst die Glasart und klicken Sie dann auf [Freigeben].

                               Übersicht Mit dieser Schaltfläche öffnen Sie den Dialog Aktuell geänderte
                               Einstellungen mit einer Übersicht der jeweiligen Einstellungen.

                               Auflösen Diese Schaltfläche ist nur aktiv, wenn die Produktion aktiv ist. Dann
                               können Sie über diese Schaltfläche eine neue DynOpt-Optimierung erzwin-
                               gen.

                               Übernehmen Über diese Schaltfläche bestätigen Sie die Aktionen. Bsp.: Sie
                               haben eine Glasart gesperrt, dann klicken Sie auf [Übernehmen] um die Akti-
                               on abzuschließen.
3.30 / 01-2023




                 J-122                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                      Optimierung




                                          Aktuell geänderte Einstellungen
                                          Optimierung > DynOpt Einstellungen > [Übersicht]




                                          Abb. J-70   Aktuell geänderte Einstellungen - Übersicht


                                          Dieser Dialog gibt Ihnen eine zusammenfassende Übersicht zu den Einstel-
                                          lungen der Register
                                          •   Allgemein
                                          •   Eingänge
                                          •   Ausgänge
                                          •   Puffer
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                      J-123
                 Zuschnitt                                                                  Softwarereferenz




                             Zuschnitt
                             Menü Zuschnitt öffnen
                             Im Menü Zuschnitt befinden sich folgende Programmpunkte:
                             •   Schneide Optimierung:
                                 Über diesen Menüpunkt schneiden Sie einen Lauf.
                                  Softwarereferenz, “Wählen Sie einen Lauf aus” auf Seite J-125
                             •   Bruchpool:
                                 Über diesen Menüpunkt greifen Sie auf den Bruchpool zu.
                                  Softwarereferenz, “Bruchpool” auf Seite J-138
                             •   Panorama:
                                 Über diesen Menüpunkt greifen Sie auf das Panorama zu (optional)
3.30 / 01-2023




                 J-124                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                                   Zuschnitt




                                          Wählen Sie einen Lauf aus
                                          Zuschnitt > Schneide Optimierung




                                          Abb. J-71     Wählen Sie einen Lauf aus


                                          Mit diesem Dialog wählen Sie einen verfügbaren Lauf aus. Im gewählten Lauf
                                          wählen Sie eine oder alle Optimierungen aus. Diese Optimierungen werden
                                          dann zum Zuschnitt vorbereitet.

                                          Erläuterungen der Liste Läufe

                                          Lauf Hier werden die Nummern der Läufe angezeigt, deren Status verändert
                                          werden kann. Die Nummern 1000 - 9999 stehen für fertig optimierte Läufe (z.
                                          B. aus A+W Production), die zum Schneiden zur Verfügung stehen. Die Num-
                                          mern 15000 - 15999 (Nummernkreise konfigurierbar) sind für selbst erstellte
                                          Tischoptimierungen reserviert. Befindet sich an dieser Stelle der Begriff Dy-
                                          nOpt Compact, handelt es sich um einen DynOpt Compact Lauf.

                                          Status Hier wird angezeigt, in welchem Bearbeitungszustand sich die einzel-
                                          nen Läufe befinden. Folgende Anzeigen sind möglich:

                                          Status              Bedeutung

                                          Freigegeben         Es liegt eine Optimierung vor, die zum Zuschnitt
                                                              freigegeben ist. Solche Läufe können in einer
                                                              Tischoptimierung weiterbearbeitet werden, bevor der
                                                              Zuschnitt erfolgt oder direkt zugeschnitten werden.

                                          Tab. J-5      Status der Läufe
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                               J-125
                 Zuschnitt                                                                  Softwarereferenz




                             Status             Bedeutung

                             Begonnen           Die Bearbeitung des Laufes wurde begonnen. Es sind
                                                Lose aus diesem Lauf bereits beim Zuschnitt oder in einer
                                                Tischoptimierung. Auch wenn eine Tischoptimierung nicht
                                                geschnitten, sondern wieder aufgelöst wurde, wird dieser
                                                Status angezeigt.

                             Produziert         Der Lauf wurde produziert.

                             Tab. J-5     Status der Läufe

                             Information In dieser Spalte werden Ihnen Laufbezeichnung angezeigt.

                             Termin In dieser Spalte sehen Sie den Produktionstermin, der bei der Lauf-
                             erstellung durch die Kapazitätsplanung ermittelt wurde.

                             Schicht In dieser Spalte sehen Sie die Produktionsschicht, die bei der Lauf-
                             erstellung durch die Kapazitätsplanung ermittelt wurde.

                                Sortierung ändern
                                Durch einen Klick auf die Spaltenüberschriften können Sie die Listeninhalte
                                auf- bzw. absteigend sortieren.

                             Erläuterungen der Liste Optimierung

                             Nr Losnummer der in einem Lauf enthaltenen Optimierungen.

                             Status Hier wird angezeigt, in welchen Bearbeitungszustand sich die einzel-
                             nen Optimierungen befinden.

                             Glasart In diesem Feld sehen Sie die Artikelnummer der Glasart, die in dieser
                             Optimierung enthalten ist. Der Wert dieses Feldes kommt aus den Stammda-
                             ten.

                             Dicke In diesem Feld sehen Sie die Dicke der Glasart, die in dieser Optimie-
                             rung enthalten ist. Der Wert dieses Feldes kommt aus den Stammdaten.

                             Glasart Bezeichnung In diesen Feld sehen Sie die Bezeichnung der Glas-
                             art. Der Wert dieses Feldes kommt aus den Stammdaten.

                             Parameter Dieses Feld zeigt Ihnen die Bezeichnung des Tisches, für den die
                             Optimierung erzeugt wurde. Der Wert dieses Feldes kommt aus den Stamm-
                             daten.

                             Platten In diesem Feld sehen Sie die Anzahl der benötigten Lagerplatten in
                             dieser Optimierung.

                             Verschnitt Das Feld zeigt Ihnen die Verschnittglasfläche in %, die bei dieser
                             Optimierung anfällt.
3.30 / 01-2023




                             Rest (mm) In diesem Feld sehen Sie die Länge des Restblattes, das nach
                             dem Zuschnitt der Optimierung übrig bleibt.



                 J-126                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                                Zuschnitt




                                          Erläuterungen der Felder

                                          Alte Läufe Wenn Sie diese Checkbox markieren, dann werden auch die Läu-
                                          fe angezeigt, die bereits produziert wurden und sich noch im Status Produziert
                                          befinden.
                                           keine Läufe mit dem Status Produziert anzeigen.
                                           nur Läufe mit dem Status Produziert anzeigen.

                                          Geschnittene Optimierungen ausblenden Wenn Sie diese Checkbox mar-
                                          kieren, dann werden die bereits geschnittenen Optimierungen nicht angezeigt.
                                           Geschnittene Optimierungen anzeigen.
                                           Geschnittenen Optimierungen nicht anzeigen.

                                          Reoptimierung Über diese Kombobox steuern Sie Neuoptimierungen. Mög-
                                          liche Werte sind:
                                          • Nein: Es erfolgt keine Neuoptimierung.
                                          • Ja: Es erfolgt eine Neuoptimierung ohne Benutzereingriff. Wird eine Opti-
                                              mierung, die nicht für den konfigurierten Tisch optimiert wurde, an den Zu-
                                              schnitt übergeben, so wird automatisch ohne Dialoganzeige eine
                                              Tischoptimierung erstellt und anstelle der originalen Optimierung in den
                                              Zuschnittprozess eingefügt.
                                          • Erweitert: Neuoptimierung mit Anzeige der vorhandenen Optimierung der
                                              zu schneidenden Glasart. Hier können Sie der neu zu optimierenden Opti-
                                              mierung noch weitere Optimierungen für die Tischoptimierung hinzufügen.
                                              Die Tischoptimierung kann dann wie gewohnt erstellt werden. Nach erfolg-
                                              ter Optimierung kann die Optimierung verworfen oder über die Schaltfläche
                                              [Zuschnitt] an den Zuschnittprozess übergeben werden. Wird die Optimie-
                                              rung verworfen, haben Sie die Möglichkeit, die originale Optimierung zu
                                              schneiden oder die Optimierung zu überspringen.
                                          • Tischoptimierung: Neuoptimierung mit Anzeige des Dialgos Tischoptimie-
                                              rung. Wird eine Optimierung, die nicht für den konfigurierten Tisch optimiert
                                              wurde, an den Zuschnitt übergeben, so wird der Dialog Tischoptimierung
                                              gestartet. Hier können die Optimierungsparameter wie z. B. Randschnitte
                                              und Schneidmodus geändert werden. Nach erfolgter Optimierung kann die
                                              Optimierung verworfen oder über die Schaltfläche [Zuschnitt] an den Zu-
                                              schnittprozess übergeben werden. Wird die neue Optimierung verworfen,
                                              so haben Sie die Möglichkeit, die originale Optimierung zu schneiden oder
                                              die Optimierung zu überspringen.
                                          Wurde die Optimierung versehentlich an den Zuschnitt übergeben, so kann
                                          der Zuschnitt beendet und die Tischoptimierung aufgelöst werden. Danach
                                          steht die originale Optimierung wieder für den Zuschnitt zur Verfügung.

                                          Komboboxen Die obere Kombobox kennzeichnet den Status der Maschine.
                                          Mögliche Werte sind:
                                          • Bereit: Am Schneidtisch kann gearbeitet werden.
                                          • Aus: Der Schneidtisch ist nicht arbeitsbereit (z. B. bei Pause).
                                          Mit der darunter liegenden Kombobox können Sie entscheiden, welche Läufe
3.30 / 01-2023




                                          angezeigt werden sollen. Mögliche Werte sind:
                                          • Läufe für den eigenen Tisch: Zeigt Ihnen nur Zuschnittläufe für den eigenen
                                             Schneidtisch an.



                 A+W Realtime Optimizer                                                                             J-127
                 Zuschnitt                                                                  Softwarereferenz




                             •   Läufe für alternative Tische: Zeigt Ihnen auch die Zuschnittläufe für alter-
                                 native Schneidtische an.
                             •   Läufe für alle Tische: Zeigt Ihnen Läufe für alle Schneidtische an.

                             Tischauswahl Mithilfe der Kombobox können Sie die Anzeige einschränken.
                             Die Kombobox enthält alle in Ihrem Hause angelegten Tische. Sie können
                             auswählen, ob die Optimierungs-Läufe aller Tische angezeigt werden sollen,
                             oder nur die, die für den Tisch optimiert wurden, der in Ihrer A+W Realtime Op-
                             timizer-Installation konfiguriert wurde. Ist das A+W Realtime Optimizer für eine
                             "Tisch-9-Logik" konfiguriert, so steht auch die Auswahl Alternative Tische zur
                             Verfügung.

                             Erläuterung der Schaltflächen

                             Optionen Durch Betätigen dieser Schaltfläche werden aus den Optimie-
                             rungsdaten Zuschnittdaten erzeugt und an den Schneidtisch übertragen. Der
                             Zuschnitt am angeschlossenen Schneidtisch beginnt. Die Anzeige der Schalt-
                             fläche wechselt auf STOPP.

                             Sortieren Diese Schaltfläche ist nur aktiv, wenn für einen Lauf mehr als eine
                             Optimierung gibt. Durch Betätigen dieser Schaltfläche starten Sie den Dialog
                             Optimierungs-Reihenfolge.

                             Schneiden Durch Betätigen dieser Schaltfläche starten Sie den Dialog Zu-
                             schnitt-Übersicht.



                             Ergänzende Informationen
                              Tutorial, “Läufe zum Zuschnitt auswählen” auf Seite J-40
                              Tutorial, “Tischansteuerung” auf Seite J-37
3.30 / 01-2023




                 J-128                                                              A+W Realtime Optimizer
                 Softwarereferenz                                                                                 Zuschnitt




                                          Lauf [Nummer] - Lauf [Nummer]
                                          Zuschnitt > Schneide Optimierung > [OK]




                                          Abb. J-72    Lauf nnn - Lauf mmm


                                          In diesem Dialog werden die zuvor im Dialog Wählen Sie einen Lauf aus ge-
                                          wählten Läufe und Lose angezeigt und können geschnitten werden.

                                          Erläuterungen der Liste Optimierungen
                                           Softwarereferenz, “Erläuterungen der Liste Optimierung” auf Seite J-126

                                          Erläuterungen der Liste Muster

                                          Nr. Dieses Feld enthält die fortlaufende Nummerierung der Lagerplatten, die
                                          in dieser Optimierung verwendet werden. Die Nummern entsprechen der Zu-
                                          schnittsreihenfolge.

                                          Breite In diesem Feld sehen Sie die Breite der Lagerplatte in mm. Der Wert
                                          dieses Feldes kommt aus den Stammdaten.

                                          Höhe In diesem Feld sehen Sie die Höhe der Lagerplatte in mm. Der Wert
                                          dieses Feldes kommt aus den Stammdaten.

                                          Opt. Gr. Hier wird angezeigt, welche Optimierungsgruppen die Lagerplatte
                                          mit Scheiben belegen. Es sind nur zwei Gruppen je Lagerplatte möglich. Eine
                                          Optimierungsgruppe kann ein Lauf oder eine Nachoptimierung sein.

                                          Status Hier wird der Status der einzelnen Lagerplatten der Optimierung an-
                                          gezeigt. Folgende Stati sind möglich:
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                               J-129
                 Zuschnitt                                                                    Softwarereferenz




                                Status               Bedeutung

                                Gesendet             Der Schneidcode wurde erzeugt.

                                Überspringen         Für diese Lagerplatte wird kein Schneidcode erzeugt und
                                                     kein Brechbild zur Verfügung gestellt.

                                Kein Schneidcode     Für diese Lagerplatte wird kein Schneidcode erzeugt aber
                                senden               ein Brechbild zur Verfügung gestellt.

                                Geschnitten          Dieser Status wird gesetzt, wenn der Schneidtisch den
                                                     Schneidcode empfangen oder abgeholt hat (seriell oder
                                                     über das Netzwerk). Es findet keine überprüfung statt, ob
                                                     die Platte auch tatsächlich geschnitten wurde.

                                Tab. J-6       Status der Läufe

                             Erläuterung der Schaltflächen

                             Tisch - START Durch Betätigen dieser Schaltfläche werden aus den Opti-
                             mierungsdaten Zuschnittdaten erzeugt und an den Schneidtisch übertragen.
                             Der Zuschnitt am angeschlossenen Schneidtisch beginnt. Die Anzeige der
                             Schaltfläche wechselt auf STOPP.

                             Tisch - STOPP Durch Betätigen dieser Schaltfläche werden keine weiteren
                             Zuschnittdaten an den Schneidtisch übertragen. Der Zuschnitt der aktuellen
                             Lagerplatte am angeschlossenen Schneidtisch wird zu Ende geführt. Die An-
                             zeige der Schaltfläche wechselt auf START.

                             Muster - Folge Durch Betätigen dieser Schaltfläche wird der Dialog Optimie-
                             rungsreihenfolge aufgerufen.

                             Muster - Optionen Durch Betätigen dieser Schaltfläche wird der Dialog Lauf:
                             Nummer aufgerufen.

                             XTV - Stopp Mit dieser Schaltfläche wird die Kommunikation gestoppt. Das
                             letzte Brechbild bleibt erhalten.

                             XTV - << Mit dieser Schaltfläche wird die Brechbildanzeige in einem ange-
                             schlossenen XTV zurückgeblättert.

                             Beenden Mit dieser Schaltfläche wird der Dialog geschlossen. Dies ist je-
                             doch erst dann möglich, wenn keine Schneidcodegenerierung läuft. Wenn
                             eine Schneidcodegenerierung läuft, dann muss diese zuvor mit [STOPP] be-
                             endet werden.


                             Ergänzende Informationen
                              Softwarereferenz, “Optimierungsreihenfolge” auf Seite J-131
                              Softwarereferenz, “Lauf: Nummer” auf Seite J-132
                              Tutorial, “Ergebnis der Tischoptimierung prüfen und bearbeiten” auf Seite J-31
3.30 / 01-2023




                              Tutorial, “Tischoptimierungen” auf Seite J-29




                 J-130                                                               A+W Realtime Optimizer
                 Softwarereferenz                                                                           Zuschnitt




                                          Optimierungsreihenfolge
                                          Zuschnitt > Schneide Optimierung > Optimierung wählen > [Sortieren]




                                          Abb. J-73   Optimierungssreihenfolge


                                          Wenn mehrere Glasarten im gewählten Lauf zur Optimierung anstehen, dann
                                          wird in diesem Dialog die vorgesehene Reihenfolge der Glasarten angezeigt.
                                          Sollten Sie mit der Reihenfolge nicht einverstanden sein, können Sie diese
                                          mithilfe der Pfeiltasten ändern.

                                          Felder

                                          Status In diesem Feld sehen Sie den Status der Optimierung.

                                          Glasart In diesem Feld sehen Sie die Artikelnummer der Glasart. Der Wert
                                          dieses Feldes kommt aus den Stammdaten.

                                          Dicke In diesem Feld sehen Sie die Dicke der Glasart in mm. Der Wert dieses
                                          Feldes kommt aus den Stammdaten.

                                          Glasart Bezeichnung In diesem Feld sehen Sie die Bezeichnung der Glas-
                                          art. Der Wert dieses Feldes kommt aus den Stammdaten.

                                          Parameter In diesem Feld sehen Sie, auf welchem Schneidtisch die Optimie-
                                          rung geschnitten werden soll.

                                          Platten In diesem Feld sehen Sie, wie viele Lagerplatten die Optimierung be-
                                          nötigt.

                                          Verschnitt In diesem Feld sehen Sie den Verschnitt der Optimierung.

                                          Rest In diesem Feld sehen Sie den Plattenrest.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                         J-131
                 Zuschnitt                                                               Softwarereferenz




                             Lauf: Nummer
                             Zuschnitt > Schneide Optimierung > Optimierung auswählen > [Optionen]




                             Abb. J-74   Restblattbehandlung


                             In diesem Dialog wird u. a. angegeben, was mit den Bruchscheiben und Rest-
                             blättern jeder Glasart in der ausgewählten Optimierung geschehen kann oder
                             soll.

                             Erläuterung der Liste Optimierungen

                             Los In diesem Feld sehen Sie die Losnummer der angezeigten Glasart in der
                             Optimierung.

                             Glasart In diesem Feld sehen Sie die Artikelnummer der Glasart. Der Wert
                             dieses Feldes kommt aus den Stammdaten.

                             Dicke In diesem Feld sehen Sie die Dicke der Glasart in mm. Der Wert dieses
                             Feldes kommt aus den Stammdaten.

                             Glasart Bezeichnung In diesem Feld sehen Sie die Bezeichnung der Glas-
                             art. Der Wert dieses Feldes kommt aus den Stammdaten.

                             Parameter In diesem Feld sehen Sie, für welchen Zuschnitttisch die Optimie-
                             rung durchgeführt wurde.

                             Platten Diese Feld zeigt Ihnen die Anzahl der Platten, die für den Zuschnitt
3.30 / 01-2023




                             dieses Loses benötigt wird.

                             Verschnitt Das Feld zeigt Ihnen die Verschnittglasfläche in %, die bei dieser
                             Optimierung anfällt.


                 J-132                                                          A+W Realtime Optimizer
                 Softwarereferenz                                                                                    Zuschnitt




                                          Rest (mm) In diesem Feld sehen Sie die Länge des Restblattes, das nach
                                          dem Zuschnitt der Optimierung übrig bleibt.

                                          Erläuterung der Liste Platten

                                          Nr. In diesem Feld sehen Sie die Nummer der Lagerplatte, die für die in der
                                          Liste Optimierungen markierte Optimierung benötigt wird.

                                          Breite In diesem Feld sehen Sie die Breite der Lagerplatte in mm. Der Wert
                                          dieses Feldes kommt aus den Stammdaten.

                                          Höhe In diesem Feld sehen Sie die Höhe der Lagerplatte in mm. Der Wert
                                          dieses Feldes kommt aus den Stammdaten.

                                          Opt. Gr. In diesem Feld sehen Sie, welche Optimierungsgruppen die Lager-
                                          platte mit Scheiben belegen. Es sind nur zwei Gruppen je Lagerplatte möglich.
                                          Eine Optimierungsgruppe kann ein Lauf oder eine Nachoptimierung sein.

                                          Schneidstatus In diesem Feld wird Ihnen der Schneidstatus der einzelnen
                                          Lagerplatten der Optimierung angezeigt. Folgende Stati sind möglich:

                                          Status               Bedeutung

                                          Gesendet             Der Schneidcode wurde erzeugt.

                                          Überspringen         Für diese Lagerplatte wird kein Schneidcode erzeugt und
                                                               kein Brechbild zur Verfügung gestellt.

                                          Kein Schneidcode     Für diese Lagerplatte wird kein Schneidcode erzeugt aber
                                          senden               ein Brechbild zur Verfügung gestellt.

                                          Geschnitten          Dieser Status wird gesetzt, wenn der Schneidtisch den
                                                               Schneidcode empfangen oder abgeholt hat (seriell oder
                                                               über das Netzwerk). Es findet keine überprüfung statt, ob
                                                               die Platte auch tatsächlich geschnitten wurde.

                                          Tab. J-7       Schneidstatus der Läufe

                                          Erläuterung der Felder im Bereich Bruchscheibenoptimierung

                                          Optimiere Bruchscheiben Hier stellen Sie ein, wie A+W Realtime Optimizer
                                          mit Bruchscheiben umgehen soll, die an den Zuschnitt übergeben werden.
                                          Folgende Einstellungen sind möglich:
                                          • Nein: Es erfolgt keine Nachoptimierung.
                                          • Trennen: Die neu erstellte Nachoptimierung wird am Ende der vorhande-
                                             nen Optimierung angefügt. Dadurch entsteht zwangsläufig ein Traveren-
                                             schnitt zwischen der vorhandenen Optimierung und dem neu erstellten
                                             Teil.
                                          • Mischen: Das letzte Lagerblatt wird komplett neu optimiert. Das führt in den
                                             meisten Fällen zu einer Verschnittverbesserung.
3.30 / 01-2023




                                          Schneide Bruchscheiben nach Restblattlänge Mit dieser Checkbox wird
                                          festgelegt, ob die Bruchscheiben auch auf ein neues Restblatt optimiert wer-
                                          den sollen, wenn das bisherige Restblatt dafür nicht ausreicht. Wenn diese


                 A+W Realtime Optimizer                                                                                    J-133
                 Zuschnitt                                                               Softwarereferenz




                             Checkbox markiert ist, dann ist der Eintrag im nachfolgenden Feld von Bedeu-
                             tung.
                              Keine neue Lagerplatte für den Zuschnitt von Bruchscheiben beginnen.
                              Eine neue Lagerplatte für den Zuschnitt beginnen, wenn das neu entstan-
                             dene Restblatt kleiner ist als die im nachfolgendem Feld Länge angegebene
                             neue Restblattlänge.

                             Schneide Restblatt unter einer Länge von Dieses Feld ist nur aktiv, wenn
                             die vorherige Checkbox markiert wurde. Geben Sie hier an, wie groß das neu
                             entstandene Restblatt höchstens sein darf. Wenn die Nachoptimierung ein
                             größeres Restblatt erzeugt, wird kein neues Restblatt begonnen. Die Bruch-
                             scheiben werden im Bruchpool gesammelt.

                             Erläuterung der Felder im Bereich Restblattverwaltung

                             Verlinken Hier stellen Sie ein, wie A+W Realtime Optimizer mit Restblätter
                             umgehen soll. Folgende Einstellungen sind möglich:
                             • Nein: Es erfolgt keine Verlinkung.
                             • Trennen: Die neu erstellte Nachoptimierung wird am Ende der vorhande-
                                nen Optimierung angefügt. Dadurch entsteht zwangsläufig ein Traveren-
                                schnitt zwischen der vorhandenen Optimierung und dem neu erstellten
                                Teil.
                             • Mischen: Die Scheiben werden auf dem Restblatt aufgelöst und mit der zu
                                optimierenden Menge neu optimiert.

                             Restblatt vor dem Schneiden bearbeiten Wenn diese Checkbox markiert
                             ist, erfolgt eine Abfrage, ob PlanEdit gestartet werden soll.

                             Erläuterung der Felder im Bereich Schnelloptimierung

                             Schnelloptimierung
                             • Standard: In diesem Modus können Sie während des Zuschnittprozesses
                               die Muster einer Glasart, für die noch kein Schneidcode übertragen wurde,
                               auflösen und neu optimieren. Der Sinn ist, dass bei Optimierungen mit vie-
                               len Mustern die Bruchscheiben nicht erst auf das letzte Blatt optimiert wer-
                               den. Die Bruchscheiben kommen in der neuen Optimierung am Anfang
                               (ohne weiteren Benutzereingriff).
                             • Erweitert: In diesem Modus sind weitere Benutzereingaben nötig. Es wird
                               automatisch das Glasauswahlmenü für die Tischoptimierung geöffnet. Dort
                               ist aber nur die Glasart der aufgelösten Optimierung zu sehen. Hier können
                               Sie noch weitere Optimierungen hinzufügen. Anschließend öffnet sich der
                               Dialog Tischoptimierung. Dort können z. B. Ränder geändert werden.
                               Wenn fertig optimiert ist, kann die Optimierung über die Schaltfläche
                               [Schneiden] direkt wieder an den Zuschnittprozess übergeben werden.

                             Nachladen Über diese Einstellung können Sie einen weiteren Lauf laden.
                             Folgende Einstellungen sind möglich:
                             • Manuell: Das Nachladen erfolgt manuell.
3.30 / 01-2023




                             • Anforderung: Es wird eine Meldung angezeigt, sobald im A+W Realtime
                                Optimizer eine konfigurierbare Anzahl noch nicht geschnittener Muster un-



                 J-134                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                                Zuschnitt




                                              terschritten wird. Sie können dann das Nachladen ablehmen oder im Lauf-
                                              auswahlmenü einen neuen Lauf laden.
                                          •   Automatisch: Das Nachladen erfolgt automatisch.

                                          Erläuterung der Felder im Bereich Etikettendruck

                                          Aktiv Über diese Checkbox können Sie den Etikettendruck aktivieren bzw.
                                          deaktivieren.
                                           Der Etikettendruck ist deaktiviert.
                                           Der Etikettendruck ist aktiviert. Sie können Etiketten direkt drucken.

                                          Erläuterung der Schaltflächen

                                          PlanEdit Wenn Sie diese Schaltfläche wählen und das Modul PlanEdit bei Ih-
                                          nen installiert ist, dann startet PlanEdit und zeigt die Optimierung grafisch an.

                                          Schneiden Wenn Sie diese Schaltfläche wählen, startet die Zuschnitt-Über-
                                          sicht.

                                          Erläuterung des Kontextmenüs
                                          Durch Klicken mit der rechten Maustaste auf eine Platte mit dem Status Ge-
                                          schnitten kann der Status Geschnitten gelöscht und die Platte erneut geschnit-
                                          ten werden.
                                          Durch Klicken mit der rechten Maustaste auf eine Platte ohne Status kann der
                                          Status Kein Schneidcode senden oder Überspringen für die gewählte Platte
                                          gesetzt werden.


                                          Ergänzende Informationen
                                           Tutorial, “A+W Pattern Viewer” auf Seite J-59
                                           Tutorial, “A+W Residual Stock Manager” auf Seite J-50
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-135
                 Zuschnitt                                                                Softwarereferenz




                             Auswahl der zu verlinkenden Optimie-
                             rung
                             Zuschnitt > Schneide Optimierung > Lauf auswählen > [OK] > Dialog Aktiver
                             Lauf: xxx wird geöffnet > Optimierung auswählen > [Start]




                             Abb. J-75   Auswahl der zu verlinkenden Optimierung


                             Die Liste Verfügbare Optimierungen enthält alle Läufe, in denen Optimierun-
                             gen für die gewählte Glasart und Dicke enthalten sind. Im Kopf des Dialoges
                             wird Ihnen der ausgewählte Lauf, das Los und die Glasart angezeigt. Wählen
                             Sie aus der Tabelle den Lauf aus, den Sie verlinken möchten und betätigen
                             Sie anschließend [Verwenden].

                             Erläuterung der Felder im Bereich Auswahl-Parameter und Rest-
                             blatt

                             Alle Tische Mit dieser Checkbox steuern Sie, welche Optimierungen ange-
                             zeigt werden. Ist die Checkbox aktiv, werden hier auch Optimierungen ange-
                             zeigt, die für andere Tische bestimmt sind.

                             Erlaube Handzuschnitt Wenn diese Checkbox markiert ist, dann werden in
                             der Liste Verfügbare Optimierungen auch die Glasarten angezeigt, die bei der
                             Artikeldefinition in den Stammdaten nur für Handzuschnitt vorgesehen wur-
                             den.

                             Restblatt In diesem Feld sehen Sie, wie lange das Restblatt ist, dass bei der
                             gewählten Optimierung (Dialog Aktiver Lauf: xxx) übrig bleibt.
3.30 / 01-2023




                 J-136                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                                Zuschnitt




                                          Optimierungsergebnis
                                          Zuschnitt > Schneide Optimierung > Lauf auswählen > [OK] > Dialog Aktiver
                                          Lauf: xxx wird geöffnet > Optimierung auswählen > [Start] > Lauf auswählen >
                                          [Verlinken]




                                          Abb. J-76    Optimierungsergebnis


                                          Dieser Dialog zeigt Ihnen das Optimierungsergebnis nach dem Verlinken. Er
                                          ist in zwei Bereiche unterteilt. Im Bereich Neue Optimierung nach dem Verlin-
                                          ken sehen Sie das Ergebnis nach dem Verlinken. Der Bereich Original-Opti-
                                          mierung zeigt Ihnen das Ergebnis vor dem Verlinken bzw. ohne ein Verlinken.
                                          In dem grauen Bereich oberhalb der Schaltflächen sehen Sie, was und wie viel
                                          zusätzlich optimiert wurde.

                                          Erläuterung der Schaltflächen

                                          Wiederholen Wenn Sie diese Schaltfläche betätigen, kehren Sie zurück zur
                                          Auswahl der Linkoptimierung, wo Sie einen Lauf auswählen können.
                                           Softwarereferenz, “Auswahl der zu verlinkenden Optimierung” auf Seite J-136

                                          Verlinken Wenn Sie diese Schaltfläche betätigen, bestätigen Sie das Ergeb-
                                          nis und die Optimierung wird geschnitten.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-137
                 Zuschnitt                                                               Softwarereferenz




                             Bruchpool
                             Zuschnitt > Bruchpool




                             Abb. J-77    Bruchpool


                             Dieser Dialog zeigt alle Scheiben an, die als Bruch gemeldet oder erfasst wur-
                             den. Scheiben aus dem Bruchpool können bei passender Glasart und Dicke
                             bei Tischoptimierungen und in der Nachoptimierung erneut optimiert werden.

                             Erläuterung der Liste Bruchscheiben

                             Glasart In diesem Feld sehen Sie die Artikelnummer der Glasart. Der Wert
                             dieses Feldes kommt aus den Stammdaten.

                             Bezeichnung In diesem Feld sehen Sie die Bezeichnung der Glasart. Der
                             Wert dieses Feldes kommt aus den Stammdaten.

                             Dicke In diesem Feld sehen Sie die Dicke der Glasart in mm. Der Wert dieses
                             Feldes kommt aus den Stammdaten.

                             Breite In diesem Feld sehen Sie die Breite der Lagerplatte in mm. Der Wert
                             dieses Feldes kommt aus den Stammdaten.

                             Höhe In diesem Feld sehen Sie die Höhe der Lagerplatte in mm. Der Wert
                             dieses Feldes kommt aus den Stammdaten.
3.30 / 01-2023




                             Lauf In diesem Feld sehen Sie die Laufnummer, zu der die Scheibe ursprüng-
                             lich gehörte.




                 J-138                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                            Zuschnitt




                                          DynOpt Mit diesem Feld haben Sie die Möglichkeit, für einzelne Bruchschei-
                                          ben ein DynOpt-Flag zu setzen, sodass diese vom DynOpt reoptimiert werden
                                          können. Wählen Sie dazu den bzw. die entsprechenden Scheiben aus und kli-
                                          cken Sie anschließend auf die Schaltfläche DynOpt. Es können nur Scheiben
                                          ausgewählt werden, für die keine Sperrstation eingetragen ist.

                                          Kunde In diesem Feld ist der Name des Kunden angegeben, zu dem die
                                          Bruchscheibe gehört.

                                          Auftrag In diesem Feld ist die Nummer des Auftrags angegeben, zu dem die
                                          Bruchscheibe gehört.

                                          Pos In diesem Feld ist die Positionsnummer des Auftrags angegeben, zu
                                          dem die Bruchscheibe gehört.

                                          Menge In diesem Feld sehen Sie die Anzahl der Scheiben.

                                          FormNr. Wenn es sich bei der Bruchscheibe um ein Modell handelt, dann
                                          wird Ihnen in diesem Feld die Modellnummer angezeigt.

                                          Bock In diesem Feld sehen Sie die Nummer des Abstellplatzes (Bock oder
                                          Fächerwagen), auf dem die Scheibe hätte stehen sollen, wenn sie nicht zu
                                          Bruch gegangen wäre.

                                          Etikett-Nr. In diesem Feld sehen Sie die Etikett-Nummer der Bruchscheibe.

                                          Los Dieses Feld wird nur programm-intern verwendet und hat keine Aussa-
                                          gekraft.

                                          Erläuterung der Schaltflächen

                                          Aktualisieren Wenn während der Arbeit mit diesem Dialog weitere Bruch-
                                          scheiben gemeldet werden (z. B. via A+W Production Terminal XTV), dann
                                          werden diese erst dann angezeigt, wenn die Anzeige im Dialog mit dieser
                                          Schaltfläche aktualisiert wird.

                                          Löschen Mit dem Betätigen dieser Schaltfläche wird die markierte Bruch-
                                          scheibe aus dem Bruchpool gelöscht. Es können auch mehrere Scheiben
                                          gleichzeitig markiert und gelöscht werden. Arbeiten Sie mit einer BDE, haben
                                          Sie die Möglichkeit, die Scheiben zu buchen.

                                          Modell-Info … Mit dieser Schaltfläche wird die Modellscheibenanzeige von
                                          A+W Production gestartet.

                                          Drucken Mit dieser Schaltfläche wird ein Ausdruck gestartet, in dem alle
                                          Bruchscheiben des Bruchpools aufgelistet werden. Diese Schaltfläche steht
                                          nur dann zur Verfügung, wenn dies im System konfiguriert wurde.

                                          Hinzufügen Mit dieser Schaltfläche wird der Dialog Brucherfassung aufgeru-
3.30 / 01-2023




                                          fen.




                 A+W Realtime Optimizer                                                                         J-139
                 Zuschnitt                                                                      Softwarereferenz




                             Erläuterung der Kombobox
                             Mithilfe der Kombobox können Sie auswählen, zu welchem Tisch der Bruch,
                             den Sie hinzufügen möchten, gebucht werden soll.
                             Öffnen Sie den Bruchpool zum ersten Mal, ist als Standard der Tisch ausge-
                             wählt, an dem der A+W Realtime Optimizer hängt.


                             Ergänzende Informationen
                              Tutorial, “Bruch, Eilscheiben und Füllaufträge” auf Seite J-21
                              Softwarereferenz, “Form-Erfassung” auf Seite J-94
                              Softwarereferenz, “Brucherfassung” auf Seite J-141
3.30 / 01-2023




                 J-140                                                                A+W Realtime Optimizer
                 Softwarereferenz                                                                          Zuschnitt




                                          Brucherfassung
                                          Zuschnitt > Bruchpool > [Hinzufügen]




                 Abb. J-78   Brucherfassung


                                          Mit diesem Dialog können Sie Scheiben erfassen, die zu Bruch gegangen sind
                                          und nochmals in eine Optimierung aufgenommen werden sollen.

                                          Erläuterung der Felder

                                          Auftrag In diesem Feld erfassen Sie die Auftragsnummer, zu der die Bruch-
                                          scheibe gehört.

                                          Position In diesem Feld geben Sie Positionsnummer des Auftrags ein, zu
                                          dem die Bruchscheibe gehört.

                                          Bruchgrund Wählen Sie aus der Kombobox den Bruchgrund der Scheiben.
                                          Bruchgründe, die hier ausgewählt werden können, müssen in den Stammda-
                                          ten definiert worden sein.

                                          Erläuterung der Liste Teile

                                          AuftNr In diesem Feld sehen Sie die Auftragsnummer, zu der die Bruchschei-
                                          be gehört.

                                          TeileNr In diesem Feld sehen Sie die Teilenummer der Scheibe.
3.30 / 01-2023




                                          Bezeichnung In diesem Feld sehen Sie die Bezeichnung der Glasart. Der
                                          Wert dieses Feldes kommt aus den Stammdaten.




                 A+W Realtime Optimizer                                                                       J-141
                 Zuschnitt                                                                      Softwarereferenz




                             Breite In diesem Feld sehen Sie die Breite der Glasart in mm oder inch (kon-
                             figurierbar).

                             Höhe In diesem Feld sehen Sie die Höhe der Glasart in mm oder inch (kon-
                             figurierbar).


                             Suchfelder
                             Zuschnitt > Bruchpool > [Hinzufügen] > <Strg> + <F12>




                             Abb. J-79     Suchfelder


                             Im Dialog Brucherfassung können bis zu drei frei konfigurierbare Suchfelder
                             hinzugefügt werden. Es handelt sich dabei um die Felder Searchfield1, Se-
                             archfield2 und Searchfield3. Die Felder werden über die Formadministration
                             hinzugefügt:
                             •   Control with action: Entry can freely be defined
                             •   Selected part: Searchfield1, ...) .
                             •   Action: Kombobox Searchfield1, ...
                             Sollten Sie sich nicht mit dieser Technologie auskennen, wenden Sie sich bitte
                             an einen A+W-Mitarbeiter.


                             Ergänzende Informationen
                              Tutorial, “Bruch, Eilscheiben und Füllaufträge” auf Seite J-21
3.30 / 01-2023




                 J-142                                                                A+W Realtime Optimizer
                 Softwarereferenz                                                                           Zuschnitt




                                          Modell-Erfassung
                                          Zuschnitt > Bruchpool > [Modell-Info]

                                                          A        B



                                                                                                    C

                                                                                                    D



                                          F




                                                      E
                                          A Benötigten Eingaben pro Modell        D Modellvorschaufenster
                                          B Modell-Nummern                        E Parameterübersicht
                                          C Grafische Modell-Übersicht            F Eingabefeld
                                          Abb. J-80    Form-Erfassung


                                          Die Felder und Schaltflächen diesen Dialoges sind identisch mit den Feldern
                                          und Schaltflächen des Dialoges Form-Erfassung im Bereich der Eilscheiben.
                                          Der Dialog wird an dieser Stelle erläutert.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Form-Erfassung” auf Seite J-94
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                        J-143
                 Zuschnitt                                                                Softwarereferenz




                             A+W DynOpt - Editor
                             Zuschnitt > DynOpt Compact …




                             Abb. J-81    Editor


                             Der Editor zeigt Ihnen auf der linken Seite im Bereich Freigegebene Läufe alle
                             Feinplanungs-Läufe, die mit DynOpt Compact verarbeitet werden können.

                             Erläuterung der Felder im Bereich Freigegebene Läufe

                             Lauf In diesem Feld sehen Sie die Laufnummer der Feinplanung.

                             Text In diesem Feld sehen Sie den Namen der Laufnummer.
                             Der Bereich Importierte Läufe zeigt Ihnen die Läufe, die bereits optimiert oder
                             importiert wurden. Durch das Aufklappen der Baumstruktur können Sie sich
                             nähere Informationen zu dem jeweiligen Lauf anzeigen lassen. Die Baum-
                             struktur zeigt Ihnen in der ersten Ebene die Laufnummer, in der zweiten Ebene
                             die Abstellplatznummer und in der dritten Ebene den Status, die Anzahl der
                             Scheiben und die Art des Abstellplatzes. Klicken Sie mit der Maus die zweite
                             Ebene (Abstellplatznummer) der Baumstruktur an, zeigt Ihnen die Liste Impor-
                             tierte Scheiben Detailinformationen zu jeder einzelnen Scheibe.
3.30 / 01-2023




                 J-144                                                           A+W Realtime Optimizer
                 Softwarereferenz                                                                           Zuschnitt




                                          Erläuterung der Schaltflächen

                                          > Mit dieser Schaltfläche verschieben Sie einen markierten Lauf aus dem Be-
                                          reich Freigegebene Läufe in den Bereich Importierte Läufe.

                                          < Mit dieser Schaltfläche verschieben Sie einen markierten Lauf aus dem Be-
                                          reich Importierte Läufe wieder zurück in den Bereich Freigegebene Läufe.

                                          ˄ Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie im Bereich
                                          Freigegebene Läufe einen Lauf gewählt und betätigen dann die Schaltfläche
                                          ∧, rückt der Lauf in der Liste eine Stelle weiter noch oben.

                                          ˅ Mit dieser Schaltfläche verändern Sie die Rangfolge. Haben Sie im Bereich
                                          Freigegebene Läufe einen Lauf gewählt und betätigen dann die Schaltfläche
                                          ∨, rückt der Lauf in der Liste eine Stelle weiter noch unten.

                                          Erläuterung der Felder im Bereich Importierte Scheiben

                                          Lauf In diesem Feld sehen Sie die Laufnummer der Feinplanung.

                                          Sequenzlauf In diesem Feld wird der Sequenzlauf des Gestells angezeigt.
                                          Es handelt sich hierbei um eine laufende Nummer der importierten Gestelle
                                          innerhalb des Laufes.

                                          Laufende Nr. In diesem Feld wird in aufsteigender Reihenfolge die laufende
                                          Nummer innerhalb des Laufes angezeigt.

                                          Fach Nr. Wenn es sich bei dem Abstellplatz um einen Fächerwagen handelt,
                                          wird in diesem Feld die Fachnummer angezeigt. Bei A-Böcken steht hier 0.

                                          Glasart In diesem Feld wird die Artikelnummer der Glasart angezeigt.

                                          Dicke In diesem Feld wird die Dicke der Scheibe in mm oder inch (konfigu-
                                          rierbar) angezeigt.

                                          Breite In diesem Feld wird die Breite der Scheibe in mm oder inch (konfigu-
                                          rierbar) angezeigt.

                                          Höhe In diesem Feld wird die Höhe der Scheibe in mm oder inch (konfigurier-
                                          bar) angezeigt.

                                          Auftrag In diesem Feld wird die Auftragsnummer angezeigt.

                                          Pos In diesem Feld wird die Positionsnummer des Auftrags angezeigt.

                                          Status In diesem Feld wird der Status angezeigt. Nähere Erläuterungen fin-
                                          den Sie weiter unten.

                                          DynOpt Compact Lauf In diesem Feld sehen Sie die Laufnummer der Dy-
3.30 / 01-2023




                                          nOpt Compact Optimierung.

                                          DynOpt Compact Los In diesem Feld sehen Sie die Losnummer der Dy-
                                          nOpt Compact Optimierung.

                 A+W Realtime Optimizer                                                                          J-145
                 Zuschnitt                                                                    Softwarereferenz




                             DynOpt Compact Muster In diesem Feld wird die Nummer des Musters an-
                             gezeigt, auf dem die einzelne Scheibe liegt.
                             Markieren Sie im linken Bereich einen Lauf, finden Sie entsprechende Detail-
                             Informationen bezüglich der einzelnen Scheiben dazu im linken Fenster.
                             Im unteren Bereich des Dialogs wird Ihnen eine Zeitleiste angezeigt. Jedes
                             farbige Rechteck kennzeichnet den Zustand eines entsprechenden Abstell-
                             platzes.
                             Folgende Farben sind möglich:

                             Farbe        Erläuterung

                                          Alle Scheiben des Gestells wurden geschnitten.

                                          Alle Scheiben des Gestells wurden optimiert.

                                          Scheiben des Gestells wurden teilweise optimiert.

                                          Das Gestell wurde noch nicht optimiert.

                             Tab. J-8     Erläuterung der Symbole

                             Die Zahlen unter dem farbigen Rechteck zeigen Ihnen die Lauf- und Abstell-
                             platznummer. Beispiel: 1187/9951 bedeutet, Laufnummer 1187 und die Ab-
                             stellplatznummer 9951.

                             Erläuterung der Felder

                             Status Die Kombobox enthält die für DynOpt Compact relevanten Stati. Mög-
                             liche Werte:
                             0: Unbearbeitet
                             100: Komplette Abstellplätze, die jedoch nur teilweise optimiert wurden.
                             200: Optimiert.
                             300: Geschnitten.
                             500: Sollten während der Optimierung Fehler aufgetreten sein, bekommen
                             diese Scheiben den Status 500. Darüber hinaus werden Sie im rechten Be-
                             reich des Editors in einem roten Balken dargestellt.

                             Zeitleisten-Darstellung Mit der Zeitleisten-Darstellung bestimmen Sie die
                             Art der Ansicht. Sie können sich den Editor für den Zuschnitt und für die Opti-
                             mierung darstellen lassen.
3.30 / 01-2023




                 J-146                                                              A+W Realtime Optimizer
                 Softwarereferenz                                                                             Zuschnitt




                                          Erläuterung der Schaltflächen

                                          Aktualisieren Mithilfe dieser Schaltfläche aktualisieren Sie den Editor.

                                             Bilden von DynOpt Compact-Läufen
                                             Sie können DynOpt Compact-Läufe aus dem Editor heraus bilden, aber
                                             auch aus dem Zuschnitt heraus. Im Editor können Sie einen oder mehrere
                                             Läufe markieren und über das Kontext-Menü die Funktion DynOpt Com-
                                             pact-Lauf erzeugen wählen. Im Zuschnitt können Sie das immer nur für ei-
                                             nen Lauf tun.


                                          Ergänzende Informationen
                                           Tutorial, “A+W DynOpt Compact” auf Seite J-81
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-147
                 Einstellungen                                                                    Softwarereferenz




                                 Einstellungen
                                 Menü Einstellungen öffnen
                                 Im Menü Einstellungen befindet sich folgender Programmpunkt:
                                 •   Tische
                                     Über diesen Menüpunkt greifen Sie auf die konfigurierten Tische zu.
                                      Softwarereferenz, “Einstellungen” auf Seite J-149
                                 •   Tischoptimierung
                                     Über diesen Menüpunkt greifen Sie auf die Tischoptimierung zu.
                                      Softwarereferenz, “Tischoptimierung” auf Seite J-151
3.30 / 01-2023




                 J-148                                                                     A+W Realtime Optimizer
                 Softwarereferenz                                                                          Einstellungen




                                          Einstellungen
                                          Einstellungen > Tische




                                          Abb. J-82    Tische


                                          Dieser Dialog steht Ihnen für alle konfigurierten Tische zur Verfügung.
                                          Er bietet die Möglichkeit, zur Laufzeit Einstellungen zu ändern, die sonst nur
                                          über die Konfigurationsdatei (xopton.cfg) angepasst werden können. Somit
                                          muss der A+W Realtime Optimizer nicht beendet und anschließend neu ge-
                                          startet werden.

                                          Erläuterung der Felder im Bereich Restplattenlager

                                          Aktiv Die Checkbox steuert, ob das Restplattenlager verwendet wird oder
                                          nicht.
                                           Das Restplattenlager wird verwendet.
                                           Das Restplattenlager wird nicht verwendet.

                                          Platten einlagern Die Checkbox steuert, ob Restplatten in das Restplatten-
                                          lager gefahren werden oder nicht.
                                           Restplatten werden in das Restplattenlager gefahren.
                                           Restplatten werden nicht in das Restplattenlager gefahren.

                                          Platten verwenden Die Checkbox steuert, ob die Optimierung die Restplat-
                                          ten aus dem Restplattenlager verwendet oder nicht.
                                           Restplatten aus dem Restplattenlager werden verwendet.
                                           Restplatten aus dem Restplattenlager werden nicht verwendet.

                                          Mindesteinlagerungslänge In diesem Feld geben Sie die Mindestlänge in
                                          mm ein, ab der ein Rest eingelagert wird.

                                          Erläuterung der Felder im Bereich Zuschnitt
3.30 / 01-2023




                                          Aktiv Die Checkbox steuert den Etikettendruck während des Zuschnitts.
                                           Etiketten werden während des Zuschnitts gedruckt.
                                           Etiketten werden nicht gedruckt.

                 A+W Realtime Optimizer                                                                             J-149
                 Einstellungen                                                             Softwarereferenz




                                 Restblatt editieren In diesem Feld geben Sie die Mindestlänge eines Rest-
                                 blatts in mm ein, damit während des Zuschnitts mit PlanEdit editiert werden
                                 kann.

                                 Erläuterung der Schaltflächen

                                 Übernehmen Wenn Sie diese Schaltfläche betätigen, werden die Änderun-
                                 gen übernommen.

                                 Verwerfen Wenn Sie diese Schaltfläche betätigen, werden die Änderungen
                                 verworfen.
3.30 / 01-2023




                 J-150                                                             A+W Realtime Optimizer
                 Softwarereferenz                                                                              Einstellungen




                                          Tischoptimierung
                                          Einstellungen > Tischoptimierung




                                          Abb. J-83    Tischoptimierung


                                          Mit diesem Dialog steuern Sie, ob bei der Auswahl der Tischoptimierung das
                                          Produktionsdatum mit angezeigt wird oder nicht.
                                          Die Kombobox enthält folgende Modi:
                                          •   Standard
                                          •   Produktionsdatum
                                          Wählen Sie den Modus Standard, wird Ihnen die Tischoptimierung ohne Pro-
                                          duktionsdatum angezeigt.
                                           Kapitel “Tischoptimierung in der Variante Standard” auf Seite J-103
                                          Wählen Sie den Modus Produktionstermin, wird Ihnen die Tischoptimierung
                                          mit Produktionsdatum angezeigt.
                                           Kapitel “Tischoptimierung in der Variante Produktionstermin” auf Seite J-106
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-151
                 Ansicht                                                               Softwarereferenz




                           Ansicht
                           Menü Ansicht öffnen
                           Im Menü Ansicht befinden sich folgende Programmpunkte:
                           •   Import starten und beenden (nur bei A+W Realtime Optimizer Stand alone)
                               Über diesen Menüpunkt starten und beenden Sie den Import.
                                Softwarereferenz, “Import” auf Seite J-153
                           •   Fehlermeldungen:
                               Über diesen Menüpunkt greifen Sie auf die Fehlermeldungen zu.
                                Softwarereferenz, “Fehlermeldungen” auf Seite J-154
                           •   Statusleiste:
                               Über diesen Menüpunkt blenden Sie die Statusleiste ein oder aus.
3.30 / 01-2023




                 J-152                                                          A+W Realtime Optimizer
                 Softwarereferenz                                                                               Ansicht




                                          Import
                                          Ansicht > Import




                                          Abb. J-84    Import


                                          Mit diesem Dialog wird das Arbeitsverzeichnis für Importdateien überwacht
                                          und der Status des Imports angezeigt.
                                          Läufe, die hier ohne Fehlermeldungen importiert wurden, stehen im Dialog
                                          Wählen Sie einen Lauf aus zur weiteren Bearbeitung bereit. Die importierten
                                          Daten werden in die Datenbank geschrieben, die Importdateien werden ins Ar-
                                          chiv-Verzeichnis verschoben.

                                          Erläuterung der Schaltflächen

                                          Start Nach Betätigung dieser Schaltfläche überwacht die Importfunktion das
                                          Arbeitsverzeichnis. Wenn neue Importdateien ins Arbeitsverzeichnis gestellt
                                          werden, dann werden diese automatisch geprüft und in die Datenbank impor-
                                          tiert. Die Schaltfläche wechselt zur Darstellung Stopp.

                                          Stopp Nach Betätigung dieser Schaltfläche wird die Inportfunktion beendet.
                                          Wenn neue Importdateien ins Arbeitsverzeichnis gestellt werden, dann blei-
                                          ben diese dort so lange unbearbeitet, bis die Importfunktion wieder gestartet
                                          wird. Die Schaltfläche wechselt zur Darstellung Start.


                                          Ergänzende Informationen
                                           Tutorial, “Optimierungen importieren” auf Seite J-17
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-153
                 Ansicht                                                               Softwarereferenz




                           Fehlermeldungen
                           Ansicht > Fehlermeldungen




                           Abb. J-85    Fehlermeldungen


                           In diesem Dialog wird ein aktuell vorliegender Fehler und alle bisherigen Feh-
                           ler (seit dem letzten Programmstart) angezeigt.

                           Es ist folgender Fehler aufgetreten In diesem Bereich wird ein neu aufge-
                           tretener Fehler angezeigt.

                           Bisherige Fehler In diesem Bereich werden alle bisher aufgetretenen Fehler
                           angezeigt.

                           Fehlerdatei Wenn Sie diese Schaltfläche betätigen, dann wird der Inhalt die-
                           ses Dialogs in einer Fehlerdatei gespeichert.
3.30 / 01-2023




                 J-154                                                         A+W Realtime Optimizer
                 Softwarereferenz                                                       A+W Residual Stock Manager




                                          A+W Residual Stock Manager
                                          Mit dem A+W Residual Stock Manager können Sie Restplatten ohne maschi-
                                          nelle Unterstützung speichern und bearbeiten. Hierfür gibt es eine Webober-
                                          fläche (A+W Planning Web), die über einen Browser von überall geöffnet
                                          werden kann. Die eingelagerten Restplatten stehen anschließend automa-
                                          tisch im A+W Realtime Optimizer zur weiteren Verarbeitung zur Verfügung.


                                          A+W Planning Web
                                          In diesem Modul nehmen Sie die Konfiguration für den A+W Residual Stock
                                          Manager vor.

                                             A+W Planning Web-Konfiguration
                                             Die Standard-Konfiguration wird bei der Installation durch A+W-Mitarbeiter
                                             vorgenommen. Wir erläutern in dieser Dokumentation, wie Sie Lager, Ab-
                                             stellplätze und Gestelle im A+W Planning Web anlegen.


                                          Lager
                                          A+W Planning Web > Lager > Stammdaten




                 Abb. J-86   Stammdaten: Lager


                                          In diesem Bereich werden Ihnen alle in Ihrem Hause angelegten Lager ange-
                                          zeigt. Sie können bestehende Lager ändern, neue Lager hinzufügen oder be-
                                          stehende Lager löschen.

                                          Erläuterung der Felder

                                          ID Eindeutiger numerischer Schlüssel. Dieser Schlüssel muss über alle Lager
                                          hinweg eindeutig sein. Wird ein neues Lager erzeugt, wird die nächste noch
                                          nicht belegte ID vorgeschlagen. Etwaige vorhergehende IDs, die durch das
                                          Löschen eines Lagers wieder frei geworden sind, werden dabei jedoch nicht
                                          berücksichtigt und daher auch nicht vorgeschlagen. Es ist möglich, die ID ma-
                                          nuell zu wählen. Ist die ID bereits vorhanden, wird mit einer entsprechenden
3.30 / 01-2023




                                          Meldung darauf hingewiesen und das Speichern verhindert.

                                          Bezeichnung Hier vergeben Sie einen eindeutigen Namen für Ihr Lager.


                 A+W Realtime Optimizer                                                                          J-155
                 A+W Residual Stock Manager                                                         Softwarereferenz




                                       Erläuterung der Schaltflächen

                                       Bearbeiten Wenn Sie auf diese Schaltfläche klicken, öffnet sich das Register
                                       Abstellplatz. Hier werden Ihnen alle Abstellplätze angezeigt, die für das ent-
                                       sprechende Lager angelegt sind.

                                       Speichern Wenn Sie auf diese Schaltfläche klicken, werden alle vorgenom-
                                       menen Änderungen gespeichert.

                                       Hinzufügen Mit dieser Schaltfläche fügen Sie ein weiteres Lager hinzu.
                                       Wenn Sie auf diese Schaltfläche klicken, wird am Anfang der Tabelle eine Zei-
                                       le eingefügt, in der Sie die entsprechenden Einträge vornehmen können.

                                       Löschen Wenn Sie auf diese Schaltfläche klicken, wird das gewählte Lager
                                       gelöscht. Vorsicht: Es erfolgt keine Sicherheitsabfrage.

                                       Aktualisieren Wenn Sie auf diese Schaltfläche klicken, wird die Anzeige ak-
                                       tualisiert.
                                       Klicken Sie auf die Schaltfläche [< Lager], kehren Sie zurück zur Übersicht der
                                       einzelnen Lager.


                                       Ergänzende Informationen
                                        Tutorial, “Lager” auf Seite J-52
3.30 / 01-2023




                 J-156                                                                      A+W Realtime Optimizer
                 Softwarereferenz                                                            A+W Residual Stock Manager




                                          Abstellplatzinformationen
                                          A+W Planning Web > Lager > Stammdaten > Schaltfläche [Bearbeiten]




                                          Abb. J-87    Bestehenden Abstellplatz bearbeiten


                                          In diesem Dialog werden Ihnen alle Abstellplätze angezeigt, die für das ent-
                                          sprechende Lager angelegt sind.

                                          Erläuterung der Felder

                                          Oben links Hier wird Ihnen angezeigt, wo Sie sich gerade befinden. Im Bei-
                                          spiel oben bedeutet das, Sie befinden sich in den Stammdaten und dort in der
                                          Übersicht der einzelnen Abstellplätze für das Lager Restplattenlager.

                                          ID In diesem Feld wird Ihnen der eindeutige numerische Schlüssel angezeigt.
                                          Dieser Schlüssel muss über alle Lager hinweg eindeutig sein. Wird ein neuer
                                          Abstellplatz erzeugt, wird die nächste noch nicht belegte ID vorgeschlagen.
                                          Etwaige vorhergehende IDs, die durch das Löschen eines Abstellplatzes wie-
                                          der frei geworden sind, werden dabei jedoch nicht berücksichtigt und daher
                                          auch nicht vorgeschlagen. Es ist möglich, die ID manuell zu wählen. Ist die ID
                                          bereits vorhanden, erscheint eine entsprechende Meldung und das Speichern
                                          wird verhindert.

                                          Bezeichnung In diesem Feld wird Ihnen der eindeutige Name zur Identifizie-
                                          rung des Abstellplatzes angezeigt. Sie können den Namen ändern, indem Sie
                                          in das Feld klicken und den bestehenden Namen überschreiben.

                                          Lagertyp In diesem Feld wird Ihnen angezeigt, um welchen Lagertyp es sich
                                          bei dem entsprechenden Abstellplatz handelt. Für jeden Tisch mit der entspre-
                                          chenden Tisch ID sollte ein Lager und ein Lagerplatz mit der Art Lagereingang
                                          angelegt werden, damit manuell neue Restplatten erzeugt und in anderen La-
                                          gerplätzen gespeichert werden können.
                                          Die anderen Lagertypen (Laden, Puffer, Ladestation und Zubringer) sind für
                                          einen Sortjet gedacht und werden nicht im A+W Residual Stock Manager ver-
                                          wendet.

                                          Zuordnungsstatus In diesem Feld können Sie einstellen, ob der Abstellplatz
                                          für Gestelle verwendet werden kann oder gesperrt ist. Eine manuelle Sper-
                                          rung ist beispielsweise dann sinnvoll, wenn die Fläche aufgrund von Waren-
                                          anlieferung blockiert ist. Hier können auch Abstellplätze, die durch das
                                          System gesperrt wurden, wieder freigegeben werden.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                          J-157
                 A+W Residual Stock Manager                                                      Softwarereferenz




                                       Erläuterung der Schaltfläche

                                       Lager Wenn Sie auf diese Schaltfläche klicken, kehren Sie zurück zur Über-
                                       sicht der einzelnen Lager.

                                       Speichern Wenn Sie auf diese Schaltfläche klicken, werden alle vorgenom-
                                       menen Änderungen gespeichert.

                                       Hinzufügen Mit dieser Schaltfläche fügen Sie einen weiteren Abstellplatz
                                       hinzu. Wenn Sie auf diese Schaltfläche klicken, wird am Anfang der Tabelle
                                       eine Zeile eingefügt, in der Sie die entsprechenden Einträge vornehmen kön-
                                       nen.

                                       Löschen Wenn Sie auf diese Schaltfläche klicken, wird der gewählte Abstell-
                                       platz gelöscht. Vorsicht: Es erfolgt keine Sicherheitsabfrage.

                                       Aktualisieren Wenn Sie auf diese Schaltfläche klicken, wird die Anzeige ak-
                                       tualisiert.


                                       Ergänzende Informationen
                                        Tutorial, “Abstellplätze” auf Seite J-53
3.30 / 01-2023




                 J-158                                                                   A+W Realtime Optimizer
                 Softwarereferenz                                                         A+W Residual Stock Manager




                                          Gestelle
                                          A+W Planning Web > Lager > Stammdaten > Abstellplatz > Schaltfläche [Be-
                                          arbeiten]




                                          Abb. J-88    Vorhandene Gestelle


                                          In diesem Dialog werden Ihnen alle Gestelle angezeigt, die für den entspre-
                                          chenden Abstellplatz angelegt sind. Scheiben können ausschließlich auf Ge-
                                          stellen verbucht werden, daher ist es ratsam, für jeden Abstellplatz
                                          mindestens ein Gestell zu konfigurieren.

                                          Erläuterung der Felder

                                          Oben links Hier wird Ihnen angezeigt, wo Sie sich gerade befinden. Im Bei-
                                          spiel oben bedeutet das, Sie befinden sich in den Stammdaten und dort in der
                                          Übersicht der einzelnen Gestelle für den Abstellplatz 101.

                                          ID In diesem Feld wird Ihnen der eindeutige numerische Schlüssel angezeigt.
                                          Dieser Schlüssel muss über alle Abstellplätze hinweg eindeutig sein. Wird ein
                                          neues Gestell erzeugt, wird die nächste noch nicht belegte ID vorgeschlagen.
                                          Etwaige vorhergehende IDs, die durch das Löschen eines Gestells wieder frei
                                          geworden sind, werden dabei jedoch nicht berücksichtigt und daher auch nicht
                                          vorgeschlagen. Es ist möglich, die ID manuell zu wählen. Ist die ID bereits vor-
                                          handen, erscheint eine entsprechende Meldung und das Speichern wird ver-
                                          hindert.

                                          Bezeichnung In diesem Feld wird Ihnen der eindeutige Name zur Identifizie-
                                          rung des Gestells angezeigt. Sie können den Namen ändern, indem Sie in das
                                          Feld klicken und den bestehenden Namen überschreiben.

                                          Zuordnungsstatus In diesem Feld können Sie einstellen, ob das Gestell für
                                          Scheiben verwendet werden kann oder gesperrt ist. Eine manuelle Sperrung
                                          ist beispielsweise dann sinnvoll, wenn die Fläche aufgrund von Warenanliefe-
                                          rung blockiert ist. Hier können auch Gestelle, die durch das System gesperrt
                                          wurden, wieder freigegeben werden.

                                          Eigenschaften In diesem Feld wird Ihnen angezeigt, um welche Gestellart
                                          es sich handelt, z B. Fächerwagen, A-Bock, etc..
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-159
                 A+W Residual Stock Manager                                                       Softwarereferenz




                                       Erläuterung der Schaltfläche

                                       Abstellplatz Wenn Sie auf diese Schaltfläche klicken, kehren Sie zurück zur
                                       Übersicht der einzelnen Abstellplätze.

                                       Speichern Wenn Sie auf diese Schaltfläche klicken, werden alle vorgenom-
                                       menen Änderungen gespeichert.

                                       Hinzufügen Mit dieser Schaltfläche fügen Sie ein weiteres Gestell hinzu.
                                       Wenn Sie auf diese Schaltfläche klicken, wird am Anfang der Tabelle eine Zei-
                                       le eingefügt, in der Sie die entsprechenden Einträge vornehmen können.

                                       Löschen Wenn Sie auf diese Schaltfläche klicken, wird das gewählte Gestell
                                       gelöscht. Vorsicht: Es erfolgt keine Sicherheitsabfrage.

                                       Aktualisieren Wenn Sie auf diese Schaltfläche klicken, wird die Anzeige ak-
                                       tualisiert.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Gestelle” auf Seite J-159
3.30 / 01-2023




                 J-160                                                                    A+W Realtime Optimizer
                 Softwarereferenz                                                        A+W Residual Stock Manager




                                          Gestelleigenschaften
                                          A+W Planning Web > Lager > Stammdaten > Schaltfläche [Gestelleigenschaf-
                                          ten]




                 Abb. J-89   Gestelleigenschaften


                                          In diesem Bereich werden Ihnen die Eigenschaften der unterschiedlichen Ge-
                                          stelltypen angezeigt. Sie können Änderungen vornehmen, aber auch neue
                                          Gestelle anlegen. Um Änderungen an bestehenden Gestellen vorzunehmen,
                                          klicken Sie einfach in das entsprechende Feld.

                                          Erläuterung der Felder

                                          Bezeichnung Eindeutiger Name zur Identifizierung eines Gestelltyp.

                                          Zugangsart Die Zugangsart beschreibt, wie Glas auf- oder abgestapelt wer-
                                          den kann. Es stehen folgende Möglichkeiten zur Verfügung:
                                          • Frei: Wahlfreier Zugriff auf die Gläser (z. B. Fächerwagen)
                                          • First in, First out (FiFo): Es kann nur das zuerst eingelagerte Glas heraus-
                                             genommen werden (z. B. Durchgangsfach)
                                          • Last in, First out (LiFo): Es kann nur das zuletzt eingelagerte Glas heraus-
                                             genommen werden (z. B. A-Bock)

                                          Maximalgewicht In diesem Feld wird Ihnen das Maximalgewicht in kg ange-
                                          zeigt.

                                          Maximale Höhe In diesem Feld wird Ihnen die maximale Höhe des Glases
                                          angezeigt, das auf diesen Gestelltyp gestellt werden kann.

                                          Maximale Breite In diese Feld wird Ihnen die maximale Breite des Glases
                                          angezeigt, das auf diesen Gestelltyp gestellt werden kann. Im Fall von mehre-
                                          ren Stapeln beschreibt dieser Wert die maximale Breite aller Stapel gemein-
                                          sam.

                                          Maximale Tiefe In diesem Feld wird Ihnen die maximale Tiefe des Gestells
                                          angezeigt. Bei einem Glasstapel werden alle Dicken der Gläser eines Stapels
                                          addiert. Bei Fächerwagen wird die maximale Tiefe mit der Breite eines einzel-
                                          nen Fachs gleichgesetzt.

                                          Minimale Höhe In diesem Feld wird Ihnen die minimale Höhe des Glases an-
                                          gezeigt, das auf diese Gestellart gestellt werden darf.
3.30 / 01-2023




                                          Minimale Breite In diesem Feld wird Ihnen die minimale Breite des Glases
                                          angezeigt, das auf diesen Gestelltyp gestellt werden darf.


                 A+W Realtime Optimizer                                                                          J-161
                 A+W Residual Stock Manager                                                         Softwarereferenz




                                       Maximalanzahl der Stapel/Fächer In diesem Feld wird Ihnen die maximal
                                       erlaubte Anzahl an Stapeln auf diesem Gestelltyp angezeigt. Bei einem Fä-
                                       cherwagen ist dies die Anzahl der Fächer. Wird der Wert -1 gesetzt, ist die An-
                                       zahl unbegrenzt, es werden dann ausschließlich die anderen Werte wie
                                       Maximale Höhe, Breite oder Tiefe zur Begrenzung herangezogen.

                                       Segmenttyp In diesem Feld wird Ihnen die Art dieses Gestelltyps angezeigt.
                                       Mögliche Werte sind:
                                       • HarpRack: Fächerwagen
                                       • LRack: L-Gestell

                                          A-Gestell
                                          Zur Konfiguration eines A-Bocks müssen zwei L-Gestelle angelegt wer-
                                          den!

                                       Erläuterung der Schaltfläche

                                       Speichern Wenn Sie auf diese Schaltfläche klicken, werden alle vorgenom-
                                       menen Änderungen gespeichert.

                                       Hinzufügen Mit dieser Schaltfläche fügen Sie eine weitere Gestelleigen-
                                       schaft hinzu. Wenn Sie auf diese Schaltfläche klicken, wird am Anfang der Ta-
                                       belle eine Zeile eingefügt, in der Sie die entsprechenden Einträge vornehmen
                                       können.

                                       Löschen Wenn Sie auf diese Schaltfläche klicken, wird die gewählte Gestell-
                                       eigenschaft gelöscht. Vorsicht: Es erfolgt keine Sicherheitsabfrage.

                                       Aktualisieren Wenn Sie auf diese Schaltfläche klicken, wird die Anzeige ak-
                                       tualisiert.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Gestelleigenschaften” auf Seite J-161
3.30 / 01-2023




                 J-162                                                                       A+W Realtime Optimizer
                 Softwarereferenz                                                            A+W Residual Stock Manager




                                             Glasübersicht
                                             A+W Planning Web > Lager > Übersicht




                 Abb. J-90   Glasübersicht


                                             In diesem Bereich werden Ihnen alle Restblätter angezeigt, die eingelagert
                                             wurden. Die Daten können in der Ansicht editiert werden, z. B. die Größe der
                                             eingelagerten Restscheibe. Über die Filterfunktionen in den Überschriften des
                                             Tabellenkopfes können Sie die Ergebnisse der Anzeige einschränken.

                                             Erläuterung der Felder

                                             Typ In diesem Feld wird Ihnen angezeigt, um welchen Glastyp (Restblatt, La-
                                             gerblatt, Scheibe) es sich handelt. Der Tabellenkopf verfügt rechts außen über
                                             eine Filterfunktion. Klicken Sie auf das Filter-Symbol, öffnet sich ein Bereich,
                                             in dem Sie den gewünschten Wert aus der Kombobox auswählen können. Kli-
                                             cken Sie auf [Filter], wird die Anzeige basierend auf Ihrer Auswahl angepasst.

                                             Abstellplatzinformationen In diesem Feld werden Ihnen die Abstellplatzin-
                                             formationen der eingelagerten Glasscheibe angezeigt. Die Angabe vor der
                                             Klammer Der Tabellenkopf verfügt rechts außen über eine Filterfunktion. Kli-
                                             cken Sie auf das Filter-Symbol, werden Ihnen alle angelegten Abstellplätze
                                             angezeigt. Sie können dann die entsprechende(n) Checkbox(en) anklicken.
                                             Klicken Sie auf [Filter], wird die Anzeige basierend auf Ihrer Auswahl ange-
                                             passt.

                                             Glastyp In diesem Feld wird Ihnen der Glastyp der eingelagerten Glasschei-
                                             be angezeigt. Der Tabellenkopf verfügt rechts außen über eine Filterfunktion.
                                             Klicken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie den Na-
                                             men oder die ID der Glasart eingeben können. Klicken Sie auf [Filter], wird die
                                             Anzeige basierend auf Ihrer Eingabe angepasst.

                                             Etikettennr. Für eingelagerte Scheiben wird Ihnen in diesem Feld die Etikett-
                                             nummer angezeigt. Der Tabellenkopf verfügt rechts außen über eine Filter-
                                             funktion. Klicken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie
3.30 / 01-2023




                                             den Namen oder die ID der Glasart eingeben können. Klicken Sie auf [Filter],
                                             wird die Anzeige basierend auf Ihrer Eingabe angepasst.



                 A+W Realtime Optimizer                                                                               J-163
                 A+W Residual Stock Manager                                                          Softwarereferenz




                                       Breite In diesem Feld wird Ihnen die Breite der eingelagerten Glasscheibe
                                       angezeigt. Der Tabellenkopf verfügt rechts außen über eine Filterfunktion. Kli-
                                       cken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie den Namen
                                       oder die ID der Glasart eingeben können. Klicken Sie auf [Filter], wird die An-
                                       zeige basierend auf Ihrer Eingabe angepasst.verfügt rechts außen über eine
                                       Filterfunktion. Klicken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in
                                       dem Sie den Wert und die Eigenschaft (größer, kleiner, gleich) eingeben kön-
                                       nen. Klicken Sie auf [Filter], wird die Anzeige basierend auf Ihrer Eingabe an-
                                       gepasst.

                                       Höhe In diesem Feld wird Ihnen die Höhe der eingelagerten Glasscheibe an-
                                       gezeigt. Der Tabellenkopf verfügt rechts außen über eine Filterfunktion. Kli-
                                       cken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie den Namen
                                       oder die ID der Glasart eingeben können. Klicken Sie auf [Filter], wird die An-
                                       zeige basierend auf Ihrer Eingabe angepasst.verfügt rechts außen über eine
                                       Filterfunktion. Klicken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in
                                       dem Sie den Wert und die Eigenschaft (größer, kleiner, gleich) eingeben kön-
                                       nen. Klicken Sie auf [Filter], wird die Anzeige basierend auf Ihrer Eingabe an-
                                       gepasst.

                                       Info In diesem Feld können Sie eine zusätzliche Information hinterlegen. Der
                                       Tabellenkopf verfügt rechts außen über eine Filterfunktion. Klicken Sie auf das
                                       Filter-Symbol, öffnet sich ein Bereich, in dem Sie den Namen oder die ID der
                                       Glasart eingeben können. Klicken Sie auf [Filter], wird die Anzeige basierend
                                       auf Ihrer Eingabe angepasst.verfügt rechts außen über eine Filterfunktion. Kli-
                                       cken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie den Wert
                                       und die Eigenschaft (gleich, beinhaltet, Startwert) eingeben können. Klicken
                                       Sie auf [Filter], wird die Anzeige basierend auf Ihrer Eingabe angepasst.

                                       Zuordnungsstatus In diesem Feld können Sie einstellen, ob der Abstellplatz
                                       für Gestelle verwendet werden kann oder gesperrt ist. Eine manuelle Sper-
                                       rung ist beispielsweise dann sinnvoll, wenn die Fläche aufgrund von Waren-
                                       anlieferung blockiert ist. Hier können auch Abstellplätze, die durch das
                                       System gesperrt wurden, wieder freigegeben werden. Der Tabellenkopf ver-
                                       fügt rechts außen über eine Filterfunktion. Klicken Sie auf das Filter-Symbol,
                                       öffnet sich ein Bereich, in dem Sie den Namen oder die ID der Glasart einge-
                                       ben können. Klicken Sie auf [Filter], wird die Anzeige basierend auf Ihrer Ein-
                                       gabe angepasst.verfügt rechts außen über eine Filterfunktion. Klicken Sie auf
                                       das Filter-Symbol, öffnet sich ein Bereich, in dem Sie den gewünschten Wert
                                       aus der Kombobox auswählen können. Klicken Sie auf [Filter], wird die Anzei-
                                       ge basierend auf Ihrer Auswahl angepasst.

                                       Datum In diesem Feld wird Ihnen angezeigt, wann die Scheibe eingelagert
                                       wurde. Der Tabellenkopf verfügt rechts außen über eine Filterfunktion. Klicken
                                       Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie den Namen oder
                                       die ID der Glasart eingeben können. Klicken Sie auf [Filter], wird die Anzeige
                                       basierend auf Ihrer Eingabe angepasst.verfügt rechts außen über eine Filter-
                                       funktion. Klicken Sie auf das Filter-Symbol, öffnet sich ein Bereich, in dem Sie
                                       den Wert und die Eigenschaft (größer, kleiner, gleich) eingeben können. Kli-
3.30 / 01-2023




                                       cken Sie auf [Filter], wird die Anzeige basierend auf Ihrer Eingabe angepasst.




                 J-164                                                                      A+W Realtime Optimizer
                 Softwarereferenz                                                          A+W Residual Stock Manager




                                          Erläuterung der Schaltflächen

                                          Neuen Datensatz hinzufügen Wenn Sie auf diese Schaltfläche klicken, öff-
                                          net sich ein Dialog, in dem Sie die entsprechenden Daten für den Datensatz
                                          eingeben können.

                                          Verwendbare Restblätter hervorheben Wenn Sie auf diese Schaltfläche
                                          klicken, werden alle verwendbaren Restblätter in der Tabelle hervorgehoben.
                                          Die Zugangsart wird bei der Verwendung der Restblätter von Gestellen eben-
                                          falls berücksichtigt:
                                          •   Wenn LiFo ausgewählt ist, wird das zuletzt abgestellte Restblatt verwendet
                                              und in der Anzeige hervorgehoben.
                                          •   Wenn FiFo ausgewählt ist, wird das zuerst abgestellte Restblatt auf einem
                                              Gestell verwendet und in der Anzeige hervorgehoben
                                          •   Wenn Frei ausgewählt ist, besteht wahlfreier Zugriff und alle Restblätter
                                              sind in der Anzeige hervorgehoben.

                                          Bearbeiten Wenn Sie auf diese Schaltfläche klicken, wird der Datensatz zur
                                          Bearbeitung freigegeben und Sie können Änderungen vornehmen.

                                          Löschen Wenn Sie auf diese Schaltfläche klicken, wird der Datensatz ge-
                                          löscht. Vorsicht: Es erfolgt keine Sicherheitsabfrage.

                                          Drucken Wenn Sie auf diese Schaltfläche klicken, wird der Etikettendruck
                                          ausgelöst. Bitte beachten Sie, dass der gewählte Drucker entsprechend ein-
                                          gerichtet ist.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Glasübersicht” auf Seite J-163
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-165
                 A+W Residual Stock Manager                                                       Softwarereferenz




                                       Neuen Datensatz hinzufügen/bearbeiten
                                       A+W Planning Web > Lager > Übersicht > [Neuen Datensatz hinzufügen]
                                       A+W Planning Web > Lager > Übersicht > [Editieren]




                                       Abb. J-91   Datensatz hinzufügen/bearbeiten


                                       In diesem Dialog können Sie bestehende Datensätze editieren oder neue Da-
                                       tensätze anlegen.

                                       Erläuterung der Felder

                                       Lager Wählen Sie aus der Kombobox das entsprechende Lager aus.

                                       Abstellplatzinformationen Wählen Sie aus der Kombobox den entspre-
                                       chenden Abstellplatz aus.

                                       Gestell Wählen Sie aus der Kombobox das entsprechende Gestell aus.

                                       Gruppe Wählen Sie aus der Kombobox die entsprechende Gruppe aus.

                                       Glastyp Wählen Sie aus der Kombobox den entsprechenden Glastyp aus.

                                       Breite/Höhe Geben Sie in diesen Feldern die entsprechenden Abmessun-
                                       gen ein.
3.30 / 01-2023




                                       Info Geben Sie in diesem Feld einen zusätzlichen Text ein, der als Informati-
                                       on dient.




                 J-166                                                                    A+W Realtime Optimizer
                 Softwarereferenz                                                   A+W Residual Stock Manager




                                          Zuordnungsstatus Wählen Sie aus der Kombobox den entsprechenden Zu-
                                          ordnungsstatus aus.

                                          Datum Wählen Sie aus dem Kalender das Datum aus, an dem das Restblatt
                                          eingelagert wurde.


                                          Ergänzende Informationen
                                           Tutorial, “Übersicht” auf Seite J-56
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                  J-167
                 A+W Residual Stock Manager          Softwarereferenz
3.30 / 01-2023




                 J-168                        A+W Realtime Optimizer
A+W Realtime Optimizer         J

                         Partindex
                 Partindex                                             Index A+W Realtime Optimizer




                 Index A+W Realtime Optimizer
                 A                                    – Bruchscheiben J-21
                 A+W Continuous Cutting J-73          – Eilscheiben J-21
                 – Übersicht geplanter Läufe J-73     – Füllaufträge J-21
                 A+W Pattern Viewer J-59              Datenübernahme
                 A+W Residual Stock Manager J-50      – Stand alone-System J-153
                 Ansteuern                            Datenübernahne
                 – Tisch J-129                        – A+W Production J-16
                 Anzeige                              – Arbeitsweise J-15
                 – Bruchscheiben J-138                – Stand alone-System J-17
                 Anzeigen                             Datenverarbeitung
                 – Eilscheibe J-90                    – Tischoptimierung J-29
                 Arbeit                               Defect Optimizer J-80
                 – fortsetzen J-45
                 – unterbrechen J-45                  E
                 Arbeitsweise                         Eilscheibe
                 – Datenübernahne J-15                – anzeigen J-90
                 – Tischansteuerung J-37              – auswählen J-30
                 – Übersicht J-13, J-19, J-27, J-38   – erfassen J-22, J-92
                 Auflösen                             – löschen J-23
                 – Tischoptimierung J-32              – optimieren J-30
                 Ausschalten                          Einschalten
                 – Import J-18                        – Import J-17
                 Auswählen                            Einstellungen
                 – Bruchscheibe J-30                  – Tische J-149
                 – Eilscheibe J-30                    – Tischoptimireung J-151
                 – Glasart J-103                      Erfassen
                 – Job J-82, J-83                     – Bruchscheibe J-23, J-141
                 – Lagerplatte J-113                  – Eilscheibe J-22, J-92
                 – Lauf J-29, J-40, J-125             Erstellen
                 – Optimierung J-103, J-125           – Tischoptimierung J-30, J-82
                                                      Erzeugen
                 B                                    – Schneidcode J-129
                 Bearbeiten
                 – Restblatt J-132                    F
                 Bruch                                Fehlermeldung J-18, J-154
                 – erfassen J-141                     Form-Erfassung J-94
                 Bruchscheibe                         Fortsetzen
                 – auswählen J-30                     – Zuschnitt J-45
                 – erfassen J-23                      Füllauftrag
                 – löschen J-24, J-25                 – verwenden J-32
                 – optimieren J-30
                 – Pool J-138
                                                      G
                                                      Glasart
                 C                                    – auswählen J-103
                 Cluster-Ansicht   J-144              Grundgedanke
3.30 / 01-2023




                                                      – Schneidcodegenerierung J-11
                 D                                    – Zuschnittsoptimierung J-11
                 Datenerfassung


                 A+W Realtime Optimizer                                                      J-171
                 Index A+W Realtime Optimizer                                                       Partindex




                 I                                           – Pausierende Glasarten    J-121
                 Import                                      – prüfen J-43
                 – ausschalten J-18                          – schneiden J-43
                 – Daten J-153
                 – einschalten J-17                          P
                 Importieren                                 Pausierende Glasarten J-121
                 – Lauf J-17                                 PlanEditor J-72
                                                             Platte
                 J                                           – erneut schneiden J-48
                 Job                                         – nicht schneiden J-41
                 – auswählen J-82, J-83                      Produktionsstatus
                 – schneiden J-129                           – zurücksetzen J-48

                 L                                           R
                 Lagerplatte                                 Reihenfolge
                 – auswählen J-31, J-113                     – Los J-43
                 Lauf                                        – Zuschnitt J-43, J-131
                 – auswählen J-29, J-125                     Restblatt
                 – zurücksetzen J-119                        – anzeigen J-43
                 – zuschneiden J-40                          – bearbeiten J-132
                 Läufe                                       – verwenden J-31
                 – Verlinken J-36                            Restelagerplatte
                 Leistungsmerkmale J-12                      – optimieren J-58
                 Leitstand J-37
                 Los                                         S
                 – Reihenfolge J-43                          Scheibe
                 Löschen                                     – erfassen J-22
                 – Bruchscheibe J-24, J-25                   Schneidcode
                 – Eilscheibe J-23                           – erzeugen J-129
                                                             – nicht erstellen J-41
                 M                                           Schneiden
                 Menü                                        – Job J-129
                 – Software J-87                             Software
                 Modellscheibe J-143                         – Menü J-87
                 Module                                      – Übersicht J-87
                 – angeschlossene J-49                       Stammdaten J-17
                 – Defect Optimizer J-80                     Stand alone-System
                 – PlanEditor J-72                           – Datenimport J-153
                                                             Starten
                                                             – Zuschnitt J-129
                 O
                                                             Symbol-Schaltflächen
                 Optimieren
                                                             – Übersicht J-88
                 – Bruchscheibe J-30
                 – Eilscheibe J-30
                 – Glasart wählen J-103                      T
                 – Restelagerplatte J-58                     Tisch
                 – Tischoptimierung J-110                    – ansteuern J-129
                 Optimierung                                 Tische
                 – Aktuell geänderte Einstellungen   J-123   – Einstellungen J-149
3.30 / 01-2023




                 – auswählen J-125                           Tischoptimierung J-29
                 – importieren J-17                          – Anzahl Lagerplatten J-118
                 – Lagerplatte wählen. J-31                  – auflösen J-32



                 J-172                                                                A+W Realtime Optimizer
                 Partindex                               Index A+W Realtime Optimizer




                 – Einstellungen J-151
                 – Ergebnis prüfen J-31
                 – erstellen J-30, J-82
                 – Lagerplatte J-113
                 – Parameter J-110, J-115
                 – Übersicht J-107
                 Tischoptimierungen
                 – verlinken J-34

                 U
                 Übersicht
                 – Arbeitsweise J-13, J-19, J-27, J-38
                 – Software J-87
                 – Symbol-Schaltflächen J-88
                 – Tischoptimierung J-107
                 Überspringen
                 – Zuschnitt J-41
                 Unterbrechen
                 – Zuschnitt J-45

                 V
                 Verlinken J-36
                 – Tischoptimierungen   J-34
                 Verwenden
                 – Füllauftrag J-32
                 – Restblatt J-31

                 W
                 Wiederholen
                 – Lauf J-40
                 – Zuschnitt J-48, J-119

                 X
                 XOPT-ON Plus
                 – Allgemein J-81
                 – Cluster-Ansicht J-144
                 – Import J-81
                 – Optimierung J-81

                 Z
                 Zurücksetzen
                 – Status J-48, J-119
                 Zuschnitt
                 – fortsetzen J-45
                 – Reihenfolge J-43, J-131
                 – starten J-43, J-129
                 – überspringen J-41
                 – unterbrechen J-45
3.30 / 01-2023




                 – wiederholen J-40, J-119
                 Zuschnitttisch J-37



                 A+W Realtime Optimizer                                        J-173
                 Index A+W Realtime Optimizer                                   Partindex
3.30 / 01-2023




                 J-174                          A+W Realtime Optimizer Realtime Optimizer

