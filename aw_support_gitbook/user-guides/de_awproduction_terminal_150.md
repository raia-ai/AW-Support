---
description: "DE AWProduction Terminal 1.50"
---



# DE AWProduction Terminal 1.50

Production Terminal




                            deutsch




                A+ W Production
                                                                                                         Vorspann




                                       Vorspann
                                       In diesem Teil der Dokumentation finden Sie die editorischen Notizen.


                                       Revisionsübersicht
                                       Part                     Beschreibung
                                       Version / Datum

                                       1.50 / 01-2023           Diverse Ergänzungen

                                       1.30 / 01-2016           Nachläufer-Verwaltung ergänzt

                                       1.20 / 09-2014           Terminal Georgian Bars ergänzt

                                       1.10 / 04-2013           Terminal LG und Edit ergänzt

                                       1.00 / 01-2012           Ersterstellung



                                       Editorial
                                       Das Editorial enthält Informationen zu folgenden Themen:
                                       •   Anmerkungen zu diesem Dokument
                                       •   Urheberrechte
                                       •   Warenzeichen
                                       •   Kontaktadressen

                                       Anmerkungen zu diesem Dokument
                                       Diese Veröffentlichung ist ausschließlich für Endanwender des Production
                                       Terminal (Terminal) gedacht.
                                       Diese Dokumentation und die darin beschriebene Software werden nur in Li-
                                       zenz vergeben und dürfen nur gemäß dieser Lizenz verwendet und kopiert
                                       werden. Der Inhalt der Dokumentation dient nur der Information und kann je-
                                       derzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung
                                       von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotz-
                                       dem können Fehler nicht vollständig ausgeschlossen werden. A+W Software
                                       GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei
                                       denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
                                       Dieses Dokument beschreibt die volle Ausbaustufe des Production Terminal.
1.50 / 01-2023




                 Production Terminal                                                                              3
                 Vorspann




                            Urheberrechte
                            © 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                            stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                            Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                            piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                            Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
                            A+W Software GmbH darf die Dokumentation weder elektronisch, noch me-
                            chanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

                            Warenzeichen
                            Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen kön-
                            nen gleichzeitig auch eingetragene Marken oder sonstige gewerbliche
                            Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

                            Kontaktadressen
                            A+W Software GmbH
                            Am Pfahlgraben 4-10
                            D-35415 Pohlheim
                               +49 6404 2051-0
                               +49 6404 2051-877
                            zentrale@a-w.com
                            http://www.a-w.com
1.50 / 01-2023




                 4                                                                   Production Terminal
                                                                                                                                                            Inhalt




                                       Inhalt
                                       Vorspann ................................................................................................................... 3
                                        Revisionsübersicht ................................................................................................. 3
                                        Editorial .................................................................................................................. 3

                                       Tutorial                                                                                                              1-9
                                       Überblick .................................................................................................................. 10
                                         Dokumentation ..................................................................................................... 11
                                           Aufbau des Tutorials ......................................................................................... 11
                                           Darstellungskonventionen ................................................................................. 12
                                       Production Terminal Systeme .................................................................................. 13
                                         Ziele der Leitrechner-Technologie ........................................................................ 15
                                         Bedienung der Leitrechner ................................................................................... 15
                                       Überblick A+W Production Terminal IG ................................................................... 17
                                         Arbeiten mit Terminal IG-In ................................................................................... 18
                                           Modul-Präsentation Terminal IG-In ................................................................... 19
                                           Ablauf von Arbeitsschritten ............................................................................... 24
                                           Weitere Funktionen ........................................................................................... 31
                                         Arbeiten mit Terminal IG-Assembly ...................................................................... 33
                                           Modul-Präsentation Terminal IG-Assembly ....................................................... 34
                                           Ablauf von Arbeitsschritten ............................................................................... 37
                                           Weitere Funktionen ........................................................................................... 38
                                         Arbeiten mit Terminal IG-Out ................................................................................ 40
                                           Modul-Präsentation Terminal IG-Out ................................................................ 41
                                           Ablauf von Arbeitsschritten ............................................................................... 43
                                           Nachläufer-Verwaltung ..................................................................................... 44
                                       Überblick A+W Production Terminal Manual Cutting ............................................... 49
                                         Arbeiten mit Terminal Manual Cutting .................................................................. 50
                                           Modul-Präsentation Terminal Manual Cutting ................................................... 51
                                           Ablauf von Arbeitsschritten ............................................................................... 58
                                           Weitere Funktionen ........................................................................................... 60
                                       Überblick A+W Production Terminal Georgian Bars ................................................ 61
                                         Arbeiten mit Terminal Georgian Bars ................................................................... 62
                                           Modul-Präsentation Terminal Georgian Bars .................................................... 63
                                           Ablauf von Arbeitsschritten ............................................................................... 67
                                           Weitere Funktionen ........................................................................................... 68
                                       Überblick A+W Production Terminal Order .............................................................. 69
                                         Arbeiten mit Terminal Order ................................................................................. 70
                                           Modul-Präsentation Terminal Order .................................................................. 71
                                           Ablauf von Arbeitsschritten ............................................................................... 75
                                           Weitere Funktionen ........................................................................................... 77
                                       Überblick A+W Production Terminal Processing ..................................................... 78
                                         Arbeiten mit Terminal Processing ......................................................................... 79
                                           Modul-Präsentation Terminal Processing ......................................................... 80
                                           Ablauf von Arbeitsschritten ............................................................................... 84
                                           Weitere Funktionen ........................................................................................... 87
                                       Überblick A+W Production Terminal TG .................................................................. 88
                                         Arbeiten mit Terminal TG-In ................................................................................. 89
                                           Modul-Präsentation Terminal TG-In .................................................................. 90
                                           Ablauf von Arbeitsschritten ............................................................................... 93
                                           Weitere Funktionen ........................................................................................... 95
1.50 / 01-2023




                                       Überblick A+W Production Terminal TG-Out ........................................................... 96




                 Production Terminal                                                                                                                              5
                 Inhalt




                           Arbeiten mit Terminal TG-Out ............................................................................... 97
                             Modul-Präsentation Terminal TG-Out ............................................................... 98
                             Ablauf von Arbeitsschritten ............................................................................. 101
                             Weitere Funktionen ......................................................................................... 102
                          Überblick A+W Production Terminal LG ................................................................ 103
                           Arbeiten mit Terminal LG-In ................................................................................ 104
                             Modul-Präsentation Terminal LG-In ................................................................ 105
                             Ablauf von Arbeitsschritten ............................................................................. 107
                             Weitere Funktionen ......................................................................................... 109
                           Arbeiten mit Terminal LG-Assembly .................................................................... 110
                             Modul-Präsentation Terminal LG-Assembly ..................................................... 111
                             Ablauf von Arbeitsschritten ............................................................................. 113
                             Weitere Funktionen ......................................................................................... 114
                          Überblick A+W Production Terminal Edit ................................................................ 115
                           Arbeiten mit Terminal Edit ................................................................................... 116
                             Modul-Präsentation Terminal Edit .................................................................... 117
                             Ablauf von Arbeitsschritten ............................................................................. 121
                             Weitere Funktionen ......................................................................................... 123

                          Softwarereferenz                                                                                               1-125
                          Bedienung der Module ........................................................................................... 126
                           Softwarebegriffe ................................................................................................. 126
                             Schaltflächen .................................................................................................. 126
                             Optionsschalter ............................................................................................... 126
                             Kombobox ....................................................................................................... 126
                             Menüleiste/Menüpunkt .................................................................................... 127
                             Tastaturbefehle ............................................................................................... 127
                           Programm beenden ............................................................................................ 128
                          Übersicht allgemein ............................................................................................... 129
                          Übersicht Terminal IG ............................................................................................ 130
                           Registrierung ...................................................................................................... 131
                           Gehe zu Produktionsnummer ............................................................................. 132
                           Vorschau ............................................................................................................ 133
                           Charge ................................................................................................................ 135
                           Los laden ............................................................................................................ 136
                           Bruch buchen ..................................................................................................... 138
                           Nachläufer laden ................................................................................................ 140
                           Status ................................................................................................................. 142
                           Nachläufer-Verwaltung ....................................................................................... 143
                           Nachläufer-Verwaltung - Bearbeiten .................................................................. 146
                          Übersicht Terminal Manual Cutting ........................................................................ 149
                           Freigabe ............................................................................................................. 150
                           Bruchpool ........................................................................................................... 152
                           Brucherfassung .................................................................................................. 154
                          Übersicht Terminal Georgian Bars ......................................................................... 156
                           Sprossen-Freigabe ............................................................................................. 157
                          Übersicht Terminal Order ....................................................................................... 159
                          Übersicht Terminal Processing .............................................................................. 160
                           Manuelle Eingabe ............................................................................................... 161
                          Übersicht Terminal TG ........................................................................................... 162
                           Manuelle Eingabe ............................................................................................... 163
                           Offene Bearbeitungen ........................................................................................ 164
                          Übersicht Terminal LG ........................................................................................... 166
1.50 / 01-2023




                           Auftrag laden ...................................................................................................... 167
                           Gehe zu Produktionsnummer ............................................................................. 169
                          Übersicht Terminal Edit .......................................................................................... 170
                          Reports .................................................................................................................. 171


                 6                                                                                                    Production Terminal
                                                                                                                                                     Inhalt




                                         Parametereingabe für Report ............................................................................. 172
                                       Die Hilfe verwenden ............................................................................................... 173
                                         Logeinträge für Sitzung ...................................................................................... 174
                                         Sprachauswahl ................................................................................................... 175
                                         Über Production Terminal ................................................................................... 176

                                       Index                                                                                                    1-177
                                       Index Production Terminal ..................................................................................... 179
1.50 / 01-2023




                 Production Terminal                                                                                                                       7
                 Inhalt
1.50 / 01-2023




                 8        Production Terminal
Production Terminal


                      Tutorial
                 Überblick                                                                           Tutorial




                             Überblick
                             Die Schulung zu den A+W Production Terminal-Modulen ist für Mitarbeiter
                             konzipiert, die in der Produktion an den entsprechenden Erfassungsstellen ar-
                             beiten.
                             Wir vermitteln dem Mitarbeiter, wie er mit Hilfe unserer Software seine Arbeits-
                             abläufe effizienter und einfacher ausführen kann und wie er auf Störungen
                             usw. eingeht.

                             Themenblöcke
                             In diesem Tutorial finden Sie folgende Themenblöcke:
                             •   Production Terminal Systeme
                             •   Überblick A+W Production Terminal IG
                             •   Überblick A+W Production Terminal Manual Cutting
                             •   Überblick A+W Production Terminal Order
                             •   Überblick A+W Production Terminal Processing
                             •   Überblick A+W Production Terminal TG

                                 Vorausgesetzte Kenntnisse
                                 EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei der Anwen-
                                 dung der entsprechenden Module vorausgesetzt. Der Mitarbeiter muss
                                 wissen, wie die physischen Arbeitsabläufe und Prozessschritte an der ent-
                                 sprechenden Arbeitsstation aussehen und auszuführen sind.
1.50 / 01-2023




                 10                                                              A+W Production Terminal
                 Tutorial                                                                                        Überblick




                                           Dokumentation
                                           Für die Schulung stehen folgende Unterlagen zur Verfügung:

                                           Handout                 Ausdruck Schulungsunterlage für die Teilnehmer

                                           PDF                     Vollständige Unterlagen
                                                                   Tutorial
                                                                   Softwarereferenz

                                           Online-Hilfe <F1>       Kontextsensitive Dialog-Hilfe der Softwarereferenz


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

                                           Lesehinweis             Der Inhalt einer Lerneinheit baut auf den Kenntnissen
                                                                   auf, die in der vorausgegangenen Einheit vermittelt
                                                                   wurden. Es ist daher sinnvoll, keine Lerneinheiten zu
                                                                   überspringen.
                                                                   Sollten Sie mit einem Thema bereits vertraut sein, lesen
                                                                   Sie mindestens die Zusammenfassung am Beginn der
                                                                   Lerneinheit, um sich die wichtigsten Details zu
                                                                   vergegenwärtigen.
1.50 / 01-2023




                 A+W Production Terminal                                                                                   11
                 Überblick                                                                           Tutorial




                             Darstellungskonventionen
                             Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                             gende Bedeutung:

                             Kursiv                   Sind Zeichenfolgen ausgezeichet, die sich auf Elemente
                                                      der Software beziehen, z. B. der Dialog Muster
                                                      senkrecht/waagerecht.

                             Fett                     Sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                      Tastatur eingeben, z. B. geben Sie den Wert 0 ein.

                             >                        Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                      gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                      Datei > Importieren > Übergabedatei.

                             []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                      z. B, mit [OK] speichern Sie die Daten.

                             <>                       Spitze Klammern bezeichnen Tasten oder
                                                      Tastenkombinationen auf der Tastatur, z. B. mit <F1>
                                                      öffnen Sie die Online-Hilfe.
1.50 / 01-2023




                 12                                                              A+W Production Terminal
                 Tutorial                                                                     Production Terminal Systeme




                                           Production Terminal Systeme
                                           Die A+W Production Terminals sind Softwaremodule des Produktionssteue-
                                           rungssystems A+W Production, mit denen Prozessschritte im Produktionsab-
                                           lauf gesteuert, erfasst, modifiziert, kontrolliert und umgelenkt werden können.
                                           Die A+W Production Terminals visualisieren und steuern einzelne Prozess-
                                           schritte und sind individuell konfigurierbar. Mit den A+W Production Terminals
                                           können online Etiketten und Reports gedruckt und Bruchscheiben mit allen
                                           benötigten Informationen erfasst werden. Die A+W Production Terminals
                                           zeichnen sich durch eine einfache und durchgängige Handhabung aus. Mit
                                           Hilfe dieser intelligenten Systeme sind Sie jederzeit in der Lage, Ihren Kunden
                                           gegenüber Auskunft über den momentanen Status der Produkte zu geben.
                                           Nachfolgend finden Sie die schematische Darstellung einer möglichen A+W
                                           Production Terminal-Landschaft:




                                                                                       Terminal Processing
                                                 Terminal Manual
                                                     Cutting




                                                                   Terminal TG-Out                   Terminal TG-In


                                                                    Terminal LG-Out                          Terminal LG-In




                                                                            Terminal Bender
                                                   Terminal                                            Terminal IG-In
                                                    IG-Out     Terminal IG-Assembly




                 Abb. 1     Überblick Production Terminals
1.50 / 01-2023




                                           Da an jedem Arbeitsplatz in der Produktion andere Informationen erforderlich
                                           sind, gibt es für verschiedene Prozesse und Arbeitsabläufe entsprechend kon-
                                           figurierte Standard-Schirme.



                 A+W Production Terminal                                                                                13
                 Production Terminal Systeme                                                                   Tutorial




                                        Kurze Erläuterung zu den einzelnen Terminals:

                                        Terminal Manual Cutting Visualisiert am Handzuschnitttisch den Arbeits-
                                        plan der zu schneidenden Scheiben.

                                        Terminal Order Kommt überall dort zum Einsatz, wo größere Mengen ge-
                                        bucht werden.

                                        Terminal Processing Ist die Variante des Leitrechners, die an Bearbeitungs-
                                        maschinen zum Einsatz kommt und diese automatisch ansteuert. Das Modul
                                        gibt Ihnen detaillierte Auskunft über die durchzuführenden Bearbeitungen in-
                                        klusive maßstabsgetreuer Produktionszeichnungen.

                                        Terminal IG-In Visualisiert am Einlauf der Isolierglaslinie den Arbeitsplan der
                                        zu produzierenden Scheiben eines Laufes oder eines logischen Produktions-
                                        gestelles/ Fächerwagen in Produktionsreihenfolge.

                                        Terminal IG-Assembly Wird zwischen optischer Scheibenkontrolle nach der
                                        Waschmaschine und vor der Rahmensetzstation installiert und visualisiert die
                                        technischen Daten inklusive der Rahmendaten jeder zu fertigenden Einheit.

                                        Terminal IG-Out Visualisiert am Auslauf der Isolierglaslinie die technischen
                                        und versandorientierten Daten jeder gefertigten Einheit.

                                        Terminal TG-In Ist das Anzeigesystem am Ofeneinlauf. Es zeigt die Bele-
                                        gung des Ofenbettes und wird durch den Bediener gesteuert. Alle Scheiben
                                        werden per Scanner registriert und ihre Geometrie auf Vollständigkeit der Be-
                                        arbeitung geprüft.

                                        Terminal TG-Out Dabei handelt es sich um das Anzeigesystem am Ofen-
                                        auslauf. Es werden alle am Ofeneinlauf registrierte Scheiben, entsprechend
                                        des Durchlauftaktes angezeigt. Der Bediener erhält, wenn definiert, Hinweise
                                        zur weiteren Verwendung oder zu Versandabstellinformationen.

                                        Terminal Edit Ist die Variante des Leitrechners, der in der Regel im Versand-
                                        büro zum Einsatz kommt, um Einheiten, Scheiben oder Gruppen umzubuchen
                                        und Außer-Haus-Gestelle zu verwalten.

                                        Terminal LG-In Visualisiert am Einlauf der VSG-Linie den Arbeitsplan der zu
                                        produzierenden Scheiben eines Laufes oder eines logischen Produktionsge-
                                        stelles/ Fächerwagen in Produktionsreihenfolge.

                                        Terminal LG-Assembly Visualisiert im Reinraum den Arbeitsplan sobald
                                        eine Scheibe oder Einheit am Terminal LG-In gebucht wurde. So ist genug Zeit
                                        zur Verfügung, um Folien zu schneiden.
1.50 / 01-2023




                 14                                                                         A+W Production Terminal
                 Tutorial                                                                 Production Terminal Systeme




                                           Ziele der Leitrechner-Technologie
                                           Im Detail werden mit der gesamten Leitrechner-Technologie folgende Ziele er-
                                           reicht:
                                           •   Geplante und optimierte Jobs oder Lose werden auf die entsprechenden
                                               Arbeitsplätze verteilt.
                                           •   Die Arbeiter an den Maschinen werden mit allen relevanten Informationen
                                               zu den Scheiben (Form, Ausrichtung, Maße, Bearbeitung) grafisch unter-
                                               stützt.
                                           •   Die durchgeführten Arbeiten werden gebucht.
                                           •   Abweichungen von den Vorgaben der Feinplanung werden erfasst.
                                           •   Geplante und tatsächliche Arbeitsweise werden während der Produktion
                                               miteinander abgeglichen.
                                           •   Der Produktionsfortschritt wird angezeigt.
                                           •   Nachläufer (wegen Bruch) werden automatisch generiert.
                                           •   Die Arbeiter an den Maschinen werden mit allen relevanten Informationen
                                               zu den Scheiben (Form, Ausrichtung, Maße, Bearbeitung) unterstützt.
                                           •   Der Produktionsablauf kann manuell nachoptimiert werden.
                                           •   Die gesammelten Daten werden für Auswertungen genutzt.
                                           Die unterschiedlichen Leitrechner-Module unterstützen dabei jeweils einen
                                           Teil dieser Ziele besonders.

                                               Performance Zähler
                                               In den Leitrechnern können zusätzliche Felder eingeblendet werden, wel-
                                               che die produzierte Menge, Fläche und Laufmeter für eine bestimmte Zeit
                                               an einer Erfassungsstelle anzeigen. Bitte kontaktieren Sie diesbezüglich
                                               einen A+W Mitarbeiter.


                                           Bedienung der Leitrechner
                                           Um mit der Leitrechner-Technologie schnell und effektiv zu arbeiten, werden
                                           Barcodes an allen relevanten Stellen eingesetzt. Die entsprechenden Arbeits-
                                           plätze oder Maschinen werden mit Barcode-Scannern ausgerüstet. Der Bar-
                                           code-Scanner ist dann einer Arbeitsstation (Erfassungsstelle) fest
                                           zugeordnet. Mit Barcodes können Produktionsfaktoren, Prozesse oder Zu-
                                           stände identifiziert werden. z. B.:
                                           •   Scheiben (Einzelne oder Gruppen)
                                           •   Gestelle
                                           •   Mitarbeiter
                                           •   Bearbeitungen
                                           •   Brüche
                                           Wird mit einem Scanner z. B. ein Gestell-Barcode gescannt, so bucht die Soft-
                                           ware dieses Gestell z. B. automatisch auf die Bearbeitungsstation.
1.50 / 01-2023




                                           Wird mit dem selben Scanner ein Scheibenbarcode gescannt, bucht die Soft-
                                           ware die Scheibe z. B. auf das angemeldete Gestell.




                 A+W Production Terminal                                                                            15
                 Production Terminal Systeme                                                           Tutorial




                                        Welche Aktionen beim Scannen welches Barcodes automatisch ausgeführt
                                        werden, wird bei der Systemeinrichtung konfiguriert.
1.50 / 01-2023




                 16                                                                   A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal IG




                                           Überblick A+W Production
                                           Terminal IG
                                           In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                           dem A+W Production Terminal IG (Terminal IG) kennen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Arbeiten mit Terminal IG-In
                                           •   Arbeiten mit Terminal IG-Assembly
                                           •   Arbeiten mit Terminal IG-Out
1.50 / 01-2023




                 A+W Production Terminal                                                                            17
                 Überblick A+W Production Terminal IG                                                                  Tutorial




                                        Arbeiten mit Terminal IG-In
                                        Lernziele

                                        •   Die Oberfläche von Terminal IG-In kennenlernen.
                                        •   Die Funktionsweise kennenlernen und verstehen.
                                        •   Arbeitsunterbrechungen korrekt durchführen.
                                        •   Mit unvorhersehbaren Situation (z. B. fehlendes Material) umgehen lernen.


                                        Nutzen

                                        Terminal IG-In hilft Ihnen, die Scheiben einer Einheit in der korrekten Reihenfolge vom
                                        Gestell auf die Linie zu stellen. Um effizient arbeiten zu können, müssen Sie die
                                        Arbeitsweise des Programms verstehen und mit täglich auftretenden Situationen
                                        entsprechend umgehen können.


                                        Definitionen

                                        Barcode                      Ist eine optoelektronisch lesbare Schrift, die aus
                                                                     unterschiedlich breiten, parallelen Strichen und Lücken
                                                                     besteht.

                                        Lauf                         Ein Menge von Positionen, die gemeinsam verplant und
                                                                     produziert werden.

                                        Los                          Eine Menge von Teilen, deren Bearbeitungen
                                                                     gleichzeitig auf derselben Maschine gefertigt werden.

                                        Nachläufer                   Ist eine Scheibe, die aufgrund von Bruch oder einem
                                                                     Mangel erneut geschnitten wurde.

                                        Charge                       Ist eine Gütermenge mit gleichen Eigenschaften. Bsp.:
                                                                     Butyl-Fass.

                                        Bruch                        Eine mangelhafte Scheibe, die nicht verwendet werden
                                                                     kann.

                                        Produktionsnummer            Definiert/visualisiert die Produktionsreihenfolge
                                                                     innerhalb eines Laufes. Bsp. Produktionsnummer 22 ist
                                                                     das 22. zu produzierende ISO.

                                        Scannen                      Unter dem Begriff Scannen versteht man das Lesen
                                                                     einer oder mehrerer Barcodes.

                                        Buchen                       Bei dem Vorgang Buchen werden bestimmte Daten in
                                                                     die Datenbank geschrieben und gespeichert.


                                        Merke

                                        Arbeitsunterbrechungen       Müssen immer protokolliert werden.

                                        Bruchgründe                  Müssen immer dokumentiert werden.
1.50 / 01-2023




                 18                                                                              A+W Production Terminal
                 Tutorial                                                               Überblick A+W Production Terminal IG




                                               Modul-Präsentation Terminal IG-In
                                               Mit Hilfe von Terminal IG-In werden am Linieneingang alle verfügbaren Lose
                                               angezeigt und können ausgewählt werden. Produktionsunterstützende Infor-
                                               mationen zu den Scheiben werden angezeigt. Dazu zählen grafische Darstel-
                                               lungen mit Form und Maßen der Scheiben, Auftrags- und
                                               Kundeninformationen, erforderliches Gas oder Sprossen im Zwischenraum
                                               der Scheiben sowie eine Vorausschau auf nachfolgend zu produzierende Ein-
                                               heiten.
                                               Nachdem Sie Terminal IG-In gestartet haben, präsentiert sich das Modul wie
                                               folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn
                                               Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B                                                                                                          I


                 C                                                                                                          J
                                                                                                                            K

                 D


                                                                                                                            L



                 E




                 F




                 G
                 H

                 A   Menüleiste                               E   Liste der aktuellen Einheit I   Laufnummer/Losnummer
                 B   Produktionsnummer mit Bezeichnung        F   Vorschauliste               J   Sprossenansicht
                 C   Modellanzeige                            G   Infofelder                  K   Verlinkte Dokumente
                 D   Farbliche Darstellung der Einheit        H   Schaltflächen               L   Produktionshinweistexte
                 Abb. 2       Terminal IG-In


                                               Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                               runter finden Sie die aktuelle Produktionsnummer sowie die Bezeichnung (B).
                                               Im Bereich (C) wird Ihnen das Modell und die umschreibenden Maße der
                                               Scheibe angezeigt. In (D) finden Sie die farbliche Darstellung der zu produzie-
1.50 / 01-2023




                                               renden Einheit. Der Bereich (E) zeigt Ihnen die Liste der aktuellen Einheit. Der
                                               Bereich (F) liefert Ihnen eine Vorschau auf die nächste Einheit und im Bereich
                                               (G) befinden sich die Infofelder. Unter (H) befinden sich alle für den weiteren


                 A+W Production Terminal                                                                                        19
                 Überblick A+W Production Terminal IG                                                           Tutorial




                                        Produktionsprozess nötigen Schaltflächen. Der Bereich (I) zeigt Ihnen die
                                        Laufnummer und die Losnummer. Im Bereich (J) werden Ihnen vorhandene
                                        Sprossen angezeigt. Sollte es zu dem Lauf verlinkte Dokumente geben, wer-
                                        den Ihnen diese im Bereich (K) angezeigt. Der Bereich (L) enthält mögliche
                                        Produktionshinweistexte.

                                           Anzeige der Spalten ist frei konfigurierbar
                                           Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                           schirmdarstellung von Ihrer Darstellung abweichen.

                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Im Anschluss finden Sie detaillierte Erläuterungen zu den einzelnen Berei-
                                        chen des oben abgebildeten Dialogs.

                                        Bereich A - Menüleiste
                                        Die Menüleiste beinhaltet die für den Anwender wichtigsten Funktionen. Die
                                        einzelnen Menüs können per Mausklick geöffnet werden.




                                        Bereich B - Produktionsnummer und Bezeichnung
                                        In diesem Bereich wird Ihnen im ersten Feld die aktuelle Produktionsnummer
                                        angezeigt. Dahinter befindet sich die Artikelbezeichung der Einheit.




                                        Bereich C - Modellanzeige
                                        In diesem Bereich wird Ihnen das Modell mit den Abmessungen angezeigt.
1.50 / 01-2023




                 20                                                                         A+W Production Terminal
                 Tutorial                                                             Überblick A+W Production Terminal IG




                                           Bereich D - Farbliche Darstellung der Einheit
                                           In diesem Bereich wird Ihnen die zu produzierende Einheit farblich und in der
                                           richtigen Reihenfolge dargestellt. Eine detaillierte Erläuterung diesbezüglich
                                           finden Sie unter Terminal IG-Assembly.

                                           Bereich E - Liste der aktuellen Einheit
                                           Dieser Bereich zeigt Ihnen die Einheit, die als nächstes zur Produktion an-
                                           steht.




                                           Abb. 3       Ausschnitt aktuelle Einheit


                                           Die obere Reihe der Tabelle (1) zeigt Ihnen die Einheit. Darunter finden Sie die
                                           zur Einheit gehörenden Scheiben in genau der Reihenfolge, wie sie zur Pro-
                                           duktion auf die Linie gestellt werden müssen. Einheit und Scheibe sind an-
                                           hand ihrer Symbole zu unterscheiden.
                                           Folgende Symbole sind möglich:

                                           Symbol       Erläuterung

                                                        Kennzeichnet eine Einheit.

                                                        Kennzeichnet eine Scheibe.


                                           Bei Scheiben, die mit grüner Farbe oder roter Farbe unterlegt sind, handelt es
                                           sich grundsätzlich um sogenannte Nachläufer, d. h. das sind Scheiben, die
                                           noch einmal geschnitten werden müssen. Grüne Scheiben sind bereits nach-
                                           geschnitten, rote Scheiben müssen noch geschnitten werden.




                                           Erläuterung der Tabellenüberschrift

                                           Typ Das Symbol kennzeichnet eine Einheit oder eine Scheibe.

                                           Nr. Zeigt Ihnen die Produktionsnummer innerhalb eines Laufes. Steht in die-
                                           sem Feld eine 1, wird diese Einheit als Erste produziert.

                                           Bock In diesem Feld sehen Sie die Nummer des Gestells, auf dem sich die
                                           Scheibe befindet. Bei Fächerwagen wird auch die Fachnummer mit angege-
1.50 / 01-2023




                                           ben.

                                           Auftrag Hier wird Ihnen die Auftragsnummer der Einheit angezeigt.



                 A+W Production Terminal                                                                                21
                 Überblick A+W Production Terminal IG                                                           Tutorial




                                        Pos. Hier wird Ihnen die Positionsnummer der Einheit innerhalb des Auftrags
                                        angezeigt.

                                        Bezeichnung Hier wird Ihnen die Artikelbezeichnung der Einheit bzw. der je-
                                        weiligen Scheibe angezeigt.

                                        Breite Hier wird die Breite der Scheibe angezeigt. Dieses Maß gibt bei Mo-
                                        dellscheiben die breiteste Stelle an. Die Breite ist das horizontale (waagerech-
                                        te) Maß der Scheibe, wenn sie so steht, wie es für die Produktion erforderlich
                                        ist. Die angegebene Zahl kann in verschiedenen mm- oder inch-Einheiten an-
                                        gezeigt werden (ToolTV.ini).

                                        Höhe Hier wird die Höhe der Scheibe angezeigt. Dieses Maß gibt bei Modell-
                                        scheiben die höchste Stelle an. Die Höhe ist das vertikale (senkrechte) Maß
                                        der Scheibe, wenn sie so steht, wie es für die Produktion erforderlich ist. Die
                                        angegebene Zahl kann in verschiedenen mm- oder inch-Einheiten angezeigt
                                        werden (ToolTV.ini).

                                        Dicke Hier wird die Dicke der Scheibe angezeigt. Die angegebene Zahl kann
                                        in verschiedenen mm- oder inch-Einheiten angezeigt werden (ToolTV.ini).

                                        Etikett Hier wird Ihnen die Etikettnummer der Einheit oder der Scheibe ange-
                                        zeigt.

                                        Bereich F - Vorschauliste
                                        In diesem Bereich können Sie sich einen Überblick darüber verschaffen, wel-
                                        che Einheiten als nächstes zur Produktion anstehen.
                                        Da die Felder dieser Liste identisch sind mit den Feldern der Liste (E), werden
                                        sie an dieser Stelle nicht noch einmal beschrieben.

                                        Bereich G - Infofelder
                                        In diesem Bereich erhalten Sie Informationen zu der angemeldeten Person,
                                        der Charge sowie dem Status der Maschine.




                                        Abb. 4       Ausschnitt Info-Bereich


                                        Im Feld Person [F4] sehen Sie den Namen der Person, die zurzeit angemeldet
                                        ist.
                                        Im Feld Charge [F1] wird Ihnen die Charge angezeigt. Das Feld Status [F3]
                                        zeigt Ihnen den Maschinenstatus an. Folgende Werte sind möglich:
                                        •   Bereit
                                        •   Abgemeldet
                                        •   Pause
1.50 / 01-2023




                                        •   Wartung
                                        •   Rüsten
                                        •   Störung


                 22                                                                         A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal IG




                                           Bereich H - Schaltflächen
                                           Hier finden Sie die für den weiteren Produktionsprozess notwendigen Schalt-
                                           flächen:

                                           Los laden [F2] Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog
                                           Los laden. In diesem Dialog können Sie ein Los zur Produktion auswählen.

                                           Produzieren [F5] Wenn Sie diese Schaltfläche betätigen, wird die Scheibe,
                                           die Sie auf die Linie gestellt haben, zur nächsten Station weiter transportiert
                                           und in den Status produziert gebucht.

                                           Überspringen [F6] Diese Schaltfläche müssen Sie betätigen, wenn die an-
                                           gezeigte Scheibe nicht zur Verfügung steht. Dann überspringen Sie die Schei-
                                           be und die nächste Scheibe wird angezeigt. Es erfolgt keine Buchung.

                                           Bruch [F7] Diese Schaltfläche müssen Sie betätigen, wenn die Scheibe, die
                                           Sie auf die Linie stellen wollen, eine Beschädigung aufweist. Dann kann sie
                                           nicht zur Produktion verwendet werden und wird als Bruch gebucht.

                                           Nachläufer [F8] Wenn Sie diese Schaltfläche betätigen, können Sie einen
                                           Nachläufer laden. Der Dialog Nachläufer laden wird geöffnet.

                                           Bereich I - Laufnummer/Losnummer
                                           In diesem Bereich wird Ihnen links die Laufnummer und rechts die Losnummer
                                           angezeigt. Im Beispiel oben handelt es sich um die Laufnummer 1010 und die
                                           Losnummer 1.

                                           Bereich J - Sprossenansicht
                                           Sollte die Einheit Sprossen enthalten, werden Ihnen diese hier angezeigt.

                                           Bereich K - Verlinkte Dokumente
                                           Sollte es zu dem Los verlinkte Dokumente geben, werden Ihnen diese hier an-
                                           gezeigt.

                                           Bereich L - Produktionshinweistexte
                                           In diesem Bereich werden Ihnen mögliche Hinweistexte (z. B. welcher Ab-
                                           standhalter) für die Produktion angezeigt.

                                              Dialog - Erscheinungsbild
                                              Die Anzeige der Spalten ist konfigurierbar, daher kann Ihre Bildschirmdar-
                                              stellung von der oben gezeigten Darstellung abweichen.


                                           Ergänzende Informationen
                                            Softwarereferenz, “Los laden” auf Seite 136
                                            Softwarereferenz, “Bruch buchen” auf Seite 138
1.50 / 01-2023




                                            Softwarereferenz, “Nachläufer laden” auf Seite 140




                 A+W Production Terminal                                                                               23
                 Überblick A+W Production Terminal IG                                                       Tutorial




                                        Ablauf von Arbeitsschritten
                                        Die Vorgehensweise zum Arbeiten in Terminal IG-In ist:
                                        •   Starten Sie das Modul Terminal IG-In.
                                        •   Melden Sie sich an (<Name>).
                                        •   Laden Sie ein Los.
                                        •   Produzieren Sie die Scheibe.
                                        Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                        protokollieren. Gründe für eine Unterbrechung können sein:
                                        •   Wartung der Maschine.
                                        •   Störung der Maschine.
                                        •   Pausenzeiten.
                                        Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                        weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                        Mängel können sein:
                                        •   Bruch
                                        •   Kratzer
                                        •   Falsches Maß
                                        •   Riss


                                         So melden Sie sich an
                                        1 Starten Sie Terminal IG-In.
                                        2 Öffnen Sie im Menü Datei den Menüpunkt Ummelden oder betätigen Sie
                                          die Funktionstaste [F4]. Der Dialog ToolTV Anmeldung wird geöffnet.




                                        3 Tippen Sie in das Feld Anwender Ihren Namen (z. B. Schmidt).
                                        4 Betätigen Sie die Schaltfläche [OK].
                                        5 Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Haupt-
                                          fenster.

                                            Namen scannen
                                            Arbeiten Sie mit einem Scanner, können Sie direkt im Hauptfenster scan-
                                            nen und brauchen nicht den Dialog ToolTV Anmeldung öffnen.
1.50 / 01-2023




                 24                                                                       A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal IG




                                           Ein Los laden
                                           Wenn Sie das Modul starten, ist der Dialog leer. Um mit Ihrer Arbeit beginnen
                                           zu können, müssen Sie zunächst ein Los laden.


                                            So laden Sie ein Los
                                           1 Betätigen Sie die Schaltfläche [Los laden].
                                           2 Der Dialog Los laden wird geöffnet.




                                           3 Terminal IG-In merkt sich den zuletzt bearbeiteten Lauf. Um alle Läufe se-
                                             hen zu können, müssen Sie deshalb den Filter löschen. Betätigen Sie die
                                             Schaltfläche [Alle anzeigen].
                                           4 Wählen Sie aus der linken Liste den Lauf, den Sie als nächstes fertigen
                                             möchten. Wenn Sie den Lauf markiert haben, sehen Sie in der rechten Lis-
                                             te den Inhalt.
                                           5 Betätigen Sie die Schaltfläche [Laden].
                                           6 Der Dialog wird geschlossen und das gewählte Los wird geladen. Sie be-
                                             finden sich jetzt wieder im Hauptfenster.


                                            So produzieren Sie eine Scheibe
                                           1 Stellen Sie die Scheibe vom Gestell auf die Linie und betätigen Sie die
                                             Schaltfläche [Produzieren].
                                           2 Die Scheibe wird zur nächsten Station weiter transportiert.
1.50 / 01-2023




                 A+W Production Terminal                                                                               25
                 Überblick A+W Production Terminal IG                                                         Tutorial




                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Eine solche Unterbrechung muss immer protokol-
                                        liert werden.
                                        Gründe für eine Unterbrechung können sein:
                                        •   Wartung der Maschine
                                        •   Störung der Maschine
                                        •   Pausenzeiten
                                        •   Rüstzeiten

                                            Automatisches Abmelden
                                            Die A+W Production Terminal Stationen können so konfiguriert werden,
                                            dass sie sich nach einer gewissen Zeit der Inaktivität automatisch abmel-
                                            den.


                                         So ändern Sie den Maschinenstatus
                                        1 Wählen Sie im Menü Maschine > Maschinenstatus. Oder betätigen Sie die
                                          Schaltfläche [F3].
                                        2 Es öffnet sich der Dialog Status.




                                        3 Wählen Sie aus der Liste den Grund aus.
                                        4 Betätigen Sie die Schaltfläche [OK].
                                        5 Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Haupt-
                                          fenster. Im Bereich Status wird der gewählte Status angezeigt.

                                            Status auf Bereit setzen
                                            Vergessen Sie nicht, nach der Arbeitsunterbrechung die Maschine wieder
                                            in den Zustand Bereit zu setzen! Sonst können Sie nicht weiterarbeiten.
1.50 / 01-2023




                 26                                                                        A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal IG




                                           Ergänzende Informationen
                                            Softwarereferenz, “Status” auf Seite 142
1.50 / 01-2023




                 A+W Production Terminal                                                                            27
                 Überblick A+W Production Terminal IG                                                          Tutorial




                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass Sie die vom Modul vorgeschla-
                                        gene Scheibe nicht fertigen können, da sie einen Mangel aufweist. Dann ist es
                                        nötig, die Scheibe entsprechend zu kennzeichnen. Gründe für Mängel können
                                        sein:
                                        •   Bruch
                                        •   Mangel (Qualitätssicherungsgrund)
                                        •   Kratzer
                                        •   Falsches Maß
                                        •   Falsche Glasart
                                        •   Risse
                                        Für Bruch, Kratzer und Risse werden Nachläufer automatisch erstellt. D. h.,
                                        wenn irgendwo in der Produktion ein Bruch entsteht und dieser gescannt wird,
                                        kommen die entsprechenden Scheiben automatisch in einen sogenannten
                                        Bruchpool und werden so schnell wie möglich nachgeschnitten. Bei den Fäl-
                                        len Falsches Maß und Falsche Glasart ist jedoch ein erneutes Schneiden nicht
                                        erwünscht. Deshalb werden bei diesen beiden Bruchgründen keine Nachläu-
                                        fer erzeugt.
                                        Bei einem Mangel hat der Vorgesetzte zu entscheiden, ob dieser bleiben bzw.
                                        entfernt werden kann oder nicht. Beispiel: Es befindet sich ein Kratzer auf der
                                        Scheibe, der aber weg poliert werden kann. Aufgrund dieser Markierung kön-
                                        nen Sie Reports erstellen, die Ihnen zur Qualitätsauswertung dienen.


                                         So verfahren Sie mit beschädigten Scheiben
                                        1 Markieren Sie die entsprechende Scheibe.
                                        2 Betätigen Sie die Schaltfläche [Bruch].
                                        3 Der Dialog Zustand wird geöffnet.




                                        4 Wählen Sie aus der Liste den entsprechenden Grund aus.
1.50 / 01-2023




                                        5 Betätigen Sie die Schaltfläche [OK].




                 28                                                                         A+W Production Terminal
                 Tutorial                                                        Überblick A+W Production Terminal IG




                                           6 Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Haupt-
                                             fenster.

                                              Automatische Nachläufer
                                              Für einige Bruchtypen werden Nachläufer automatisch generiert. Dies wird
                                              bei der Konfiguration entsprechend eingestellt. Der Mitarbeiter an der Ma-
                                              schine muss mit diesen Modalitäten vertraut sein.

                                           Eine andere Produktionsnummer laden
                                           Es kann vorkommen, dass Sie die von Terminal IG-In vorgeschlagene Produk-
                                           tionsnummer nicht fertigen können oder aber eine andere Produktionsnum-
                                           mer der Aktuellen vorziehen sollen. Um in der Vorschauliste nicht umständlich
                                           nach unten scrollen zu müssen, können Sie die gewünschte Produktionsnum-
                                           mer direkt laden.


                                            So laden Sie eine Produktionsnummer
                                           1 Wählen Sie im Menü Datei > Springe zu ProdNr.
                                           2 Der Dialog Gehe zu Produktionsnummer wird geöffnet.




                                           3 Wählen Sie im Feld Neue Produktionsnummer über die Pfeiltasten die ge-
                                             wünschte Produktionsnummer aus.
                                           4 Betätigen Sie die Schaltfläche [OK].
                                           5 Der Dialog wird geschlossen und die gewählte Produktionsnummer wird
                                             geladen. Sie befinden sich jetzt wieder im Hauptfenster.
1.50 / 01-2023




                 A+W Production Terminal                                                                            29
                 Überblick A+W Production Terminal IG                                                           Tutorial




                                        Einen Nachläufer laden
                                        Befinden sich für die aktuell zu fertigende Produktionsnummer noch Nachläu-
                                        fer in der Produktion, können diese über den Dialog Nachläufer einfügen ge-
                                        laden oder gescannt werden.


                                         So laden Sie Nachläufer
                                        1 Betätigen Sie die Schaltfläche [Nachläufer].
                                        2 Es öffnet sich der Dialog Einfügen.




                                        3 Geben Sie im Feld Barcode die entsprechende Etikettnummer der ISO-
                                          Einheit manuell oder scannen Sie diese.
                                        4 Betätigen Sie die Schaltfläche [Übernehmen].
                                        5 Die zugehörigen Daten werden im Feld darunter angezeigt.
                                        6 Betätigen Sie die Schaltfläche [Laden].
                                        7 Der Dialog wird geschlossen und der Nachläufer wird geladen. Sie befin-
                                          den sich jetzt wieder im Hauptfenster.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Nachläufer laden” auf Seite 140
1.50 / 01-2023




                 30                                                                            A+W Production Terminal
                 Tutorial                                                        Überblick A+W Production Terminal IG




                                           Weitere Funktionen
                                           Zu den weiteren Funktionen zählen:
                                           •   Listen (Reports)
                                           •   Log-Einträge
                                           •   Unterschiedliche Programm-Sprachen

                                           Listen (Reports) generieren
                                           Die Listen (Reports) sind im gleichnamigen Menü zu finden. Sie werden von
                                           A+W für jeden Kunden individuell erstellt und den jeweiligen Anforderungen
                                           angepasst. Wir zeigen Ihnen im Anschluss den Report einer Auftragsüber-
                                           sicht.


                                            So drucken Sie eine Auftragsübersicht
                                           1 Wählen Sie im Menü Listen > Auftragsübersicht.
                                           2 Der Dialog Parametereingabe für Report wird geöffnet.
                                           3 Geben Sie im Bereich Geben Sie einen Wert ein die gewünschte Auftrags-
                                             nummer an.
                                           4 Betätigen Sie die Schaltfläche [OK].
                                           5 Der Dialog wird geschlossen und der Report wird angezeigt:




                                           Log-Einträge exportieren
                                           Sie können die Logeinträge in Form einer Text-Datei exportieren. Im Falle ei-
                                           nes Fehlers kann es von Vorteil sein, diese Text-Datei zu Analysezwecken zu
                                           A+W zu schicken.


                                            So exportieren Sie Log-Einträge
                                           1 Wählen Sie im Menü ? > Aktuelle Log-Einträge.
                                           2 Der Dialog Log-Einträge für diese Sitzung wird geöffnet.
                                           3 Betätigen Sie die Schaltfläche [Exportieren].
1.50 / 01-2023




                                           4 Es öffnet sich der Dialog Speichern unter … .




                 A+W Production Terminal                                                                             31
                 Überblick A+W Production Terminal IG                                                          Tutorial




                                        5 Vergeben Sie einen Namen für die Datei und wählen Sie den entsprechen-
                                          den Speicherort aus.
                                        6 Betätigen Sie die Schaltfläche [Speichern].
                                        7 Der Dialog wird geschlossen und die Datei ist gespeichert.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174

                                        Programmsprache wählen
                                        Das Modul kann in verschiedenen Sprachen betrieben werden. Die Sprache
                                        kann während der Laufzeit umgestellt werden. Ein Neustart ist nicht erforder-
                                        lich.


                                         So wählen Sie eine andere Sprache aus
                                        1 Wählen Sie im Menü ? > Sprache ändern.
                                        2 Der Dialog Sprache ändern wird geöffnet.
                                        3 Wählen Sie aus der Kombobox Sprache die gewünschte Sprache aus.
                                        4 Schließen Sie den Dialog über die Schaltfläche [OK]. Das Modul präsen-
                                          tiert sich in der gewünschten Sprache.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Sprachauswahl” auf Seite 175
1.50 / 01-2023




                 32                                                                           A+W Production Terminal
                 Tutorial                                                             Überblick A+W Production Terminal IG




                                           Arbeiten mit Terminal IG-Assembly
                                           Lernziele

                                           •   Oberfläche von Terminal IG-Assembly kennenlernen.
                                           •   Die Funktionsweise kennenlernen und verstehen.
                                           •   Arbeitsunterbrechungen korrekt durchführen.
                                           •   Mit unvorhersehbaren Situation (z. B. fehlendes Material) umgehen lernen.
                                           •   Chargen definieren.


                                           Nutzen

                                           Terminal IG-Assembly unterstützt Sie an dieser Stelle erheblich bei Ihrer Arbeit. Es
                                           zeigt Ihnen optisch den Scheibenaufbau sowie das zu verwendende Gas und den
                                           entsprechenden Rahmen. Alle relevanten Informationen sind auf einen Blick
                                           ersichtlich und müssen nicht nachgeschlagen (Papier) werden.


                                           Definitionen

                                           Produktionshinweistexte      Werden Ihnen in einem eigenen Bereich angezeigt.

                                           Rahmen                       Abstandhalter, der sich zwischen den einzelnen
                                                                        Glasscheiben befindet.

                                           Gas                          Der Scheibenzwischenraum wird mit Gas gefüllt.


                                           Merke

                                           Aktualisieren                Über diese Schaltfläche aktualisieren Sie die Anzeige.

                                           Farbliche Darstellung der    Lässt Sie den Aufbau der Einheit auf einen Blick
                                           Einheit                      erkennen.
1.50 / 01-2023




                 A+W Production Terminal                                                                                      33
                 Überblick A+W Production Terminal IG                                                                   Tutorial




                                           Modul-Präsentation Terminal IG-Assembly
                                           Terminal IG-Assembly befindet sich im Anschluss von Terminal IG-In. Es wird
                                           zwischen der optischer Scheibenkontrolle nach der Waschmaschine und vor
                                           der Rahmensetzstation installiert und visualisiert die technischen Daten inklu-
                                           sive der Rahmendaten jeder zu fertigenden Einheit. Diese ist die letzte und
                                           sinnvolle Station, an der Sie ISO-Unterteile als Bruch buchen können.
                                           Nachdem Sie Terminal IG-Assembly gestartet haben, präsentiert sich das Mo-
                                           dul wie folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten.
                                           Wenn Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B                                                                                                         I


                 C                                                                                                         J
                                                                                                                           K

                 D


                                                                                                                           L



                 E




                 F




                 G
                 H

                 A    Menüleiste                          E   Liste der aktuellen Einheit I   Laufnummer/Losnummer
                 B    Produktionsnummer und Bezeichnung   F   Vorschauliste               J   Sprossenansicht
                 C    Modellanzeige                       G   Infofelder                  K   Verlinkte Dokumente
                 D    Farbliche Darstellung der Einheit   H   Meldungsfenster und         L   Produktionshinweistexte
                                                              Schaltflächen
                 Abb. 5        Terminal IG-Assembly


                                           Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                           runter finden Sie die aktuelle Produktionsnummer sowie die Bezeichnung (B).
                                           Im Bereich (C) wird Ihnen das Modell und die umschreibenden Maße der
                                           Scheibe angezeigt. In (D) finden Sie die farbliche Darstellung der zu produzie-
                                           renden Einheit. Der Bereich (E) zeigt Ihnen die Liste der aktuellen Einheit. Der
1.50 / 01-2023




                                           Bereich (F) liefert Ihnen eine Vorschau auf die nächste Einheit und im Bereich
                                           (G) befinden sich die Infofelder. Unter (H) befinden sich alle für den weiteren
                                           Produktionsprozess nötigen Schaltflächen. Der Bereich (I) zeigt Ihnen die



                 34                                                                               A+W Production Terminal
                 Tutorial                                                            Überblick A+W Production Terminal IG




                                           Laufnummer und die Losnummer. Im Bereich (J) werden Ihnen vorhandene
                                           Sprossen angezeigt. Sollte es zu dem Lauf verlinkte Dokumente geben, wer-
                                           den Ihnen diese im Bereich (K) angezeigt. Der Bereich (L) enthält mögliche
                                           Produktionshinweistexte.

                                               Anzeige der Spalten ist frei konfigurierbar
                                               Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                               schirmdarstellung von Ihrer Darstellung abweichen.

                                           Detaillierte Erläuterung zu den einzelnen Bereichen
                                           Außer dem Bereich (D) sind alle Bereiche von Terminal IG-Assembly identisch
                                           mit den Bereichen von Terminal IG-In und werden deshalb an dieser Stelle
                                           nicht noch einmal beschrieben.
                                            Tutorial, “Detaillierte Erläuterung zu den einzelnen Bereichen” auf Seite 20

                                           Bereich D - Farbliche Darstellung der Einheit
                                           In diesem Bereich wird Ihnen die zu produzierende Einheit farblich und in der
                                           richtigen Reihenfolge dargestellt. Im Anschluss folgt eine detaillierte Erläute-
                                           rung zur Darstellung der Einheit:

                                                                                              D
                                           A



                                           B


                                                                                             E
                                           C



                                           A Außenseite (Sonne)                      D Beschichtung
                                           B Äußere Scheibe                          E Innere Scheibe
                                           C Scheibenzwischenraum


                                           Für Scheiben gibt es folgende Darstellungen:

                                           Symbol        Erläuterung

                                                         Kennzeichnet eine Float-Scheibe.



                                                         Kennzeichnet eine ESG-Scheibe.



                                           Tab. 1        Symbole und ihre Bedeutung
1.50 / 01-2023




                 A+W Production Terminal                                                                                    35
                 Überblick A+W Production Terminal IG                                                           Tutorial




                                        Symbol        Erläuterung

                                                      Kennzeichnet eine VSG-Scheibe.



                                                      Kennzeichnet eine beschichtete Float-
                                                      Scheibe.


                                                      Kennzeichnet ein Ornament-Glas.



                                        Tab. 1        Symbole und ihre Bedeutung

                                        Für den Scheibenzwischenraum gibt es folgende Darstellungen:

                                        Symbol        Erläuterung

                                                      Kein Gas




                                                      Gas: Argon




                                                      Gas: Krypton




                                                      Sprossen



                                        Tab. 2        Symbole und ihre Bedeutung


                                        Ergänzende Informationen
                                         Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19
1.50 / 01-2023




                 36                                                                            A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal IG




                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal IG-Assembly ist:
                                           •   Starten Sie das Modul Terminal IG-Assembly.
                                           •   Melden Sie sich an (<Name>).
                                           •   Definieren Sie eine Charge (optional)
                                           •   Produzieren Sie die Einheit.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine
                                           •   Störung der Maschine
                                           •   Pausenzeiten
                                           Sollte eine Scheibe, die Sie gerade auf die Linie stellen wollen eine Beschädi-
                                           gung aufweisen, müssen Sie den entsprechenden Grund ebenfalls buchen.
                                           Gründe für Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Falsches Maß
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So definieren Sie Chargen
                                               Unter einer Charge versteht man eine Gütermenge mit gleichen Eigen-
                                               schaften. An dieser Erfassungsstation könnte dies z. B. ein Butyl-Fass
                                               sein.
                                           1 Öffnen Sie im Menü Datei den Menüpunkt Charge oder betätigen Sie die
                                             Funktionstaste [F1]. Der Dialog Manuelle Eingabe wird geöffnet.




                                           2 Geben Sie im Feld Charge die gewünschte Bezeichnung ein.
                                           3 Betätigen Sie die Schaltfläche [OK].
                                           4 Der Dialog wird geschlossen und Sie befinden sich jetzt wieder im Haupt-
1.50 / 01-2023




                                             fenster. Im Bereich Charge wird die eingegebene Charge angezeigt.




                 A+W Production Terminal                                                                              37
                 Überblick A+W Production Terminal IG                                                         Tutorial




                                         So produzieren Sie die Einheit
                                        1 Nehmen Sie den erforderlichen Rahmen und stellen Sie ihn auf die Linie.
                                        2 Anschließend betätigen Sie die Schaltfläche [Produzieren [F5]].
                                        3 Die Einheit wird zusammengebaut und weiter transportiert.

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                        befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                        Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                        Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                        In ausführlich beschrieben.
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28

                                        Eine Einheit überspringen
                                        Es kann vorkommen, dass Sie die nächste zur Produktion anstehende Einheit
                                        nicht fertigen können. Ein Grund dafür ist z. B. ein fehlender Rahmen. In die-
                                        sem Fall werden die Scheiben (in der Regel) auf der Linie belassen und ein-
                                        fach weiter transportiert.


                                         So überspringen Sie eine Einheit
                                        1 Markieren Sie die entsprechende Einheit.
                                        2 Betätigen Sie die Schaltfläche [Überspringen [F6]].


                                        Weitere Funktionen
                                        Zu den weiteren Funktionen zählen:
                                        •   Listen (Reports)
                                        •   Log-Einträge
                                        •   Unterschiedliche Programm-Sprachen
                                        Da in diesem Bereich die Felder von Terminal IG-Assembly identisch sind mit
                                        den Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal
                                        beschrieben.
1.50 / 01-2023




                                         Tutorial, “Weitere Funktionen” auf Seite 31




                 38                                                                          A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal IG




                                           Ergänzende Informationen
                                            Tutorial, “Den Zustand der Maschine ändern” auf Seite 26
                                            Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28
                                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                                            Tutorial, “Log-Einträge exportieren” auf Seite 31
                                            Tutorial, “Programmsprache wählen” auf Seite 32
                                            Softwarereferenz, “Status” auf Seite 142
                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
1.50 / 01-2023




                 A+W Production Terminal                                                                            39
                 Überblick A+W Production Terminal IG                                                                 Tutorial




                                        Arbeiten mit Terminal IG-Out
                                        Lernziele

                                        •   Oberfläche von Terminal IG-Out kennenlernen.
                                        •   Die Funktionsweise kennenlernen und verstehen.
                                        •   Ein Gestell anmelden.
                                        •   Mit unvorhersehbaren Situation (z. B. fehlendes Material) umgehen lernen.


                                        Nutzen

                                        Terminal IG-Out hilft Ihnen beim korrekten Abstellen der Einheiten. Unter Verwendung
                                        unterschiedlicher Farben sehen Sie, welche Einheit auf welches Gestell gehört. Das
                                        spart Zeit, da Sie nichts nachschlagen müssen.


                                        Definitionen

                                        Gestell-Farbcode             Einheiten mit der gleichen Farbe kommen auf ein
                                                                     Gestell.

                                        Packmittelgruppe             Eine Packmittelgruppeist eine individuelle Gruppierung
                                                                     von Einheiten, meistens nach Versandkriterien.


                                        Merke

                                        Gestell anmelden             Bevor Sie mit der Arbeit beginnen, müssen Sie ein
                                                                     Gestell anmelden.

                                        Beginn eines Gestells        Ist das Gestell leer, vergessen Sie nicht, die Checkbox
                                                                     zu aktivieren.

                                        Erst abstellen, dann         Buchen Sie die Einheit erst, wenn sie auf dem Gestell
                                        buchen                       steht!
1.50 / 01-2023




                 40                                                                              A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal IG




                                           Modul-Präsentation Terminal IG-Out
                                           Terminal IG-Out befindet sich im Anschluss von Terminal IG-Assembly. Es vi-
                                           sualisiert am Isolierglaslinienauslauf die versandorientierten Daten jeder ge-
                                           fertigten Einheit.
                                           Nachdem Sie Terminal IG-Out gestartet haben, präsentiert sich das Modul wie
                                           folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn
                                           Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B                                                                                                    I
                 C
                                                                                                                      J
                 D

                                                                                                                      K
                                                                                                                      L


                                                                                                                      M
                 E




                 F




                 G

                                                                                                                      N
                 H

                 A   Menüleiste                           G Infofelder                K   Packmittelgruppe
                 B   Produktionsnummer und Bezeichnung    H Meldungsfenster           L   Anzahl/Gewicht
                 C   Abmessungen der Einheit              I Gestell-Farbcode/         M   Modellanzeige
                 D   Auftragsdaten                          Kennzeichen: Gestell leer N   Schaltflächen
                 E   Verlinkte Dokumente                  J Angemeldetes o.
                 F   Liste der Einheiten auf der Linie      vorgeschlagenes Gestell

                 Abb. 6       Terminal IG-Out


                                           Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                           runter finden Sie die aktuelle Produktionsnummer sowie die Bezeichnung (B).
                                           Im Bereich (C) finden Sie Abmessungen der Einheit. In (D) befinden sich die
                                           Auftragsdaten. Der Bereich (E) zeigt Ihnen die verlinkten Dokumente. Der Be-
                                           reich (F) zeigt Ihnen die ISO-Einheiten, wie sie an der vorherigen Station (Ter-
                                           minal IG-Assembly) zusammengebaut wurden und im Bereich (G) befinden
1.50 / 01-2023




                                           sich die Infofelder. Unter (H) befindet sich das Meldungsfenster. Der Bereich
                                           (I) zeigt Ihnen den Gestell-Farbcode sowie das Kennzeichen für ein leeres Ge-
                                           stell. Im Bereich (J) wird Ihnen das angemeldete bzw. vorgeschlagene Gestell


                 A+W Production Terminal                                                                                  41
                 Überblick A+W Production Terminal IG                                                            Tutorial




                                        angezeigt. Der Bereich (K) zeigt Ihnen die Packmittelgruppe. Im Bereich (L)
                                        finden Sie das Stückgewicht bzw. das Gesamtgewicht (Gestell). Bitte beach-
                                        ten Sie, dass das Gestellgewicht (Leergewicht) in den Stammdaten von A+W
                                        Production gepflegt sein muss. Im Bereich (M) finden Sie die Modellanzeige
                                        und im Bereich (N) befinden sich die Schaltflächen.

                                           Anzeige der Spalten ist frei konfigurierbar
                           I




                                           Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                           schirmdarstellung von Ihrer Darstellung abweichen.

                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Die Bereiche (A), (B), (E), (F), (G), (H), (M) und (N) von Terminal IG-Out sind
                                        identisch sind mit den Bereichen von Terminal IG-In und werden an dieser
                                        Stelle nicht noch einmal beschrieben.

                                        Bereich I - Gestell-Farbcode
                                        In diesem farblich hervorgehobenen Feld wird der Name des angemeldeten
                                        Gestells angezeigt. Der farbige Rahmen blinkt, wenn kein Gestell angemeldet
                                        ist. Es soll das Gestell angemeldet werden, auf das die aktuelle Einheit gestellt
                                        wird.
                                        Die Verwendung von Farben kann an bestimmte Bedingungen geknüpft wer-
                                        den. So kann festgelegt werden, dass eine Gruppe von Einheiten, die auf ein
                                        oder mehreren Gestellen zusammengehalten werden sollen, mit der gleichen
                                        Farbe im Bereich (F) angezeigt werden. Ein Wechsel der Farbe bedeutet
                                        gleichzeitig Wechsel des Gestells.

                                        Bereich J - Angemeldetes oder vorgeschlagenes Gestell
                                        In diesem Bereich sehen Sie, welches Gestell angemeldet ist. Der Name des
                                        Gestells ist eindeutig. Es existiert kein weiteres Gestell mit diesem Namen.
                                        Der Name kann alphabetisch, numerisch oder auch alphanumerisch sein.

                                        Bereich K - Kennzeichen, Gestell leer
                                        Haben Sie ein leeres Gestell, aktivieren Sie nach der Anmeldung des Gestells
                                        noch diese Checkbox. Damit stellen Sie sicher, dass sich auf dem Gestell kei-
                                        ne gebuchten Scheiben mehr befinden.
                                        Arbeiten Sie mit einem Scanner, können Sie auch den Barcode Beginn scan-
                                        nen.

                                           Gestell mit Einheiten
                                           Befinden sich auf dem Gestell bereits Einheiten, dürfen Sie die Checkbox
                                           nicht aktivieren. Sonst löschen Sie die Einheiten, die sich bereits auf dem
                                           Gestell befinden.

                                        Bereich L - Packmittelgruppe
                                        In diesem Bereich wird Ihnen die Packmittelgruppe angezeigt. Bei einer Pack-
                                        mittelgruppe handelt es sich um eine Gruppe mit zusammengehörenden Ein-
1.50 / 01-2023




                                        heiten.




                 42                                                                          A+W Production Terminal
                 Tutorial                                                            Überblick A+W Production Terminal IG




                                           Ergänzende Informationen
                                            Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19


                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal IG-Out ist:
                                           •   Starten Sie das Modul Terminal IG-Out.
                                           •   Melden Sie sich an (<Name>).
                                           •   Melden Sie ein Gestell an.
                                           •   Stellen Sie die Einheit auf das Gestell.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Scheibe, die Sie gerade von der Linie nehmen wollen, eine Be-
                                           schädigung aufweisen, müssen Sie den entsprechenden Grund ebenfalls bu-
                                           chen. Gründe für Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So melden Sie ein Gestell an
                                           1 Scannen Sie die Gestellnummer des physikalischen Gestells.
                                           2 Haben Sie ein leeres Gestell, aktivieren Sie nach der Anmeldung des Ge-
                                             stells die Checkbox Beginn (F11). Arbeiten Sie mit einem Scanner, können
                                             Sie auch den Barcode Beginn scannen.


                                            So produzieren Sie die Einheit
                                           1 Nehmen Sie die Einheit von der Linie und stellen Sie sie auf das Gestell.
                                           2 Anschließend betätigen Sie die Schaltfläche [Produzieren [F5]].

                                               Erst abstellen, dann buchen
                                               Stellen Sie bitte erst die Einheit auf das Gestell und betätigen anschließend
                                               die Schaltfläche [Produzieren[F5]].
1.50 / 01-2023




                 A+W Production Terminal                                                                                 43
                 Überblick A+W Production Terminal IG                                                           Tutorial




                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                        befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                        Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                        Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                        In ausführlich beschrieben.
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28


                                        Nachläufer-Verwaltung
                                        In der Produktion kann es vorkommen, dass Komponenten nicht komplett ka-
                                        putt sind, sondern zum Teil noch zu verwenden sind. Das könnte z. B. bei ei-
                                        nem zusammengebauten ISO der Fall sein, wenn nur eine Scheibe kaputt ist
                                        bzw. Beschädigungen aufweist und die andere (teure) Scheibe wiederverwen-
                                        det werden kann. Darüber hinaus kann es vorkommen, dass bei einem Ein-
                                        fachglas Bearbeitungen wiederholt werden müssen (z. B. eine Beschichtung
                                        muss abgewaschen und die Scheibe muss neu beschichtet werden). Da in
                                        den beiden genannten Fällen das Produkt nicht komplett kaputt ist, spricht
                                        man hier von einem Teilebruch.
                                        In der Nachläufer-Verwaltung kann man für solche Teilebrüche entscheiden,
                                        welche Teile wiederzuverwenden sind, welche Bearbeitungen zu wiederholen
                                        sind und wie die defekten Teile erneut in die Produktion eingesteuert werden
                                        sollen.
                                        Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                        •   Wiederverwendung
                                        •   AV-Nachläufer
                                        •   Direkte Nachfertigung

                                        Wiederverwendung
1.50 / 01-2023




                                        Kann der Fehler an der bruchgebuchten Scheibe / Einheit behoben werden,
                                        so dass die Scheibe / Einheit nicht neu produziert werden muss, wählen Sie
                                        die Option [Wiederverwendung]. Über die Schaltfläche [F3] öffnet sich der Di-
                                        alog Bearbeiten. Dort können Sie festlegen, auf welche Erfassungsstelle die


                 44                                                                            A+W Production Terminal
                 Tutorial                                                         Überblick A+W Production Terminal IG




                                           Scheibe / Einheit gebucht werden soll, so dass man sie später in der Produk-
                                           tion leichter findet. In diesem Dialog können Sie auch festlegen, welche Bear-
                                           beitungen wiederholt werden sollen.
1.50 / 01-2023




                 A+W Production Terminal                                                                             45
                 Überblick A+W Production Terminal IG                                                         Tutorial




                                        AV-Nachläufer
                                        Befinden sich an der defekten Einheit komplexe Bearbeitungen, kann es hilf-
                                        reich sein, diese komplett neu zu verplanen. In diesem Fall verwenden Sie die
                                        Option [AV-Nachläufer]. Damit können Sie eine komplett neue Position im Auf-
                                        tragspool erzeugen. Die alte Produktionsposition wird mengenmäßig entspre-
                                        chend reduziert, sodass die Gesamtmenge der Auftragsposition wieder
                                        stimmt.
                                        Direkte Nachfertigung
                                        Wenn Sie die Scheibe ohne neue Planung erneut zuschneiden, wählen Sie
                                        die Option [Direkte Nachfertigung]. Damit wird die Scheibe in den Bruchpool
                                        des A+W Realtime Optimizers gebucht, so dass sie direkt nachgeschnitten
                                        werden kann.

                                        Arbeitsablauf




                                        Abb. 7       Nachläufer-Verwaltung


                                        Der Dialog zeigt Ihnen die als Teilebruch gemeldeten Scheiben / Einheiten.
                                        Eine Nachläuferposition hat beim Buchen von Bruch den Zustand Teilebruch
                                        zugewiesen bekommen (im A+W Standard mit Zustand 40 und Erfassungs-
                                        stelle 40).
                                        Im oberen Bereich werden Ihnen die Einheiten angezeigt, die sich im Zustand
                                        Teilebruch befinden. Klicken Sie im oberen Bereich eine Einheit an, wird Ihnen
                                        im Bereich Details die gesamte Stückliste der Einheit angezeigt.
1.50 / 01-2023




                                        Markieren Sie im oberen Bereich die Einheit und wählen Sie dann für die Ein-
                                        heit mittels der Schaltflächen [Wiederverwendung], [AV-Nachläufer] und [Di-
                                        rekte Nachfertigung], wie mit der Einheit zu verfahren ist. Alle Unterteile
                                        bekommen automatisch ebenfalls diese Art der Verwendung zugewiesen.


                 46                                                                        A+W Production Terminal
                 Tutorial                                                        Überblick A+W Production Terminal IG




                                           Gibt es Bestandteile der Einheit, die weiter- bzw. wiederverwendet werden
                                           können, markieren Sie diese in der Tabelle und klicken anschließend auf [Be-
                                           arbeiten].




                                           Abb. 8      Nachläufer-Verwaltung, Bearbeiten


                                           Es öffnet sich für dieses Teil der Dialog Bearbeiten. Ändern Sie die Beschaf-
                                           fungsart in Wiederverwendung und geben Sie im Feld Erfassungsstelle an, wo
                                           es hingebucht werden soll. Dort wartet das Teil auf die Nachläufer, um dann
                                           gemeinsam zu einer neuen Einheit produziert zu werden.
                                           Den Dialog Bearbeiten schließen Sie über die Schaltfläche [OK]. Sie befinden
                                           sich dann wieder in der Nachläufer-Verwaltung und das soeben bearbeitete
                                           Teil hat jetzt eine grüne Flagge. Die Felder Beschaffungsart, ES und Name
                                           wurden entsprechend angepasst.
                                           Unterteile, welche nicht wiederverwendet werden können, werden durch den
                                           Status Bruch zur Nachproduktion vorgesehen. Diese sind später, nach Spei-
                                           chern und Schließen des Dialogs Nachläufer-Verwaltung, als neue Einträge in
                                           den entsprechenden Pool-Anzeigen sichtbar.


                                            So erzeugen Sie einen Teilebruch
                                           1 Markieren Sie im A+W Production Terminal die entsprechende Einheit.
                                           2 Betätigen Sie die Schaltfläche [Bruch].
                                           3 Der Dialog Zustand wird geöffnet.
                                           4 Wählen Sie aus der Liste den Bruchgrund Teilebruch aus.
                                           5 Betätigen Sie die Schaltfläche [OK].
1.50 / 01-2023




                 A+W Production Terminal                                                                             47
                 Überblick A+W Production Terminal IG                                                            Tutorial




                                         So arbeiten Sie mit der Nachläufer-Verwaltung
                                        6 Öffnen Sie im Menü Extras den Menüpunkt Nachläufer-Verwaltung. Es öff-
                                          net sich der gleichnamige Dialog, der alle Einheiten enthält, die sich im Zu-
                                          stand Teilebruch befinden.
                                        7 Über die Schaltflächen [Wiederverwendung], [AV-Nachläufer] und [Direkte
                                          Nachfertigung] steuern Sie, wie mit der Einheit bzw. den einzelnen Be-
                                          standteilen zu verfahren ist.
                                        8 Falls es Bestandteile gibt, die noch zu verwenden sind, markieren Sie die-
                                          se im unteren Bereich und klicken Sie auf die Schaltfläche [Bearbeiten].
                                          Nun können Sie das Teil zur Wiederverwendung kennzeichnen und eine
                                          Erfassungsstelle auswählen, auf die das Teil entsprechend gebucht wer-
                                          den soll.
                                        9 Den Dialog verlassen Sie über die Schaltfläche [Schließen].
                                        Eine detaillierte Erläuterung der einzelnen Felder und Schaltflächen finden Sie
                                        in der Softwarereferenz.


                                        Ergänzende Informationen
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28
                                         Tutorial, “Listen (Reports) generieren” auf Seite 31
                                         Tutorial, “Log-Einträge exportieren” auf Seite 31
                                         Tutorial, “Programmsprache wählen” auf Seite 32
                                         Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
                                         Softwarereferenz, “Nachläufer-Verwaltung” auf Seite 143
                                         Softwarereferenz, “Nachläufer-Verwaltung - Bearbeiten” auf Seite 146
1.50 / 01-2023




                 48                                                                          A+W Production Terminal
                 Tutorial                                           Überblick A+W Production Terminal Manual Cutting




                                           Überblick A+W Production
                                           Terminal Manual Cutting
                                           In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                           dem A+W Production Terminal Manual Cutting (Terminal Manual Cutting) ken-
                                           nen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Arbeiten mit Terminal Manual Cutting
1.50 / 01-2023




                 A+W Production Terminal                                                                         49
                 Überblick A+W Production Terminal Manual Cutting                                                     Tutorial




                                        Arbeiten mit Terminal Manual Cutting
                                        Lernziele

                                        •   Oberfläche von Terminal Manual Cutting kennenlernen.
                                        •   Die Funktionsweise kennenlernen und verstehen.
                                        •   Läufe freigeben.
                                        •   Mit dem Bruchpool arbeiten.
                                        •   Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                        Nutzen

                                        Mit Terminal Manual Cutting haben Sie unter Anderem die Möglichkeit, defekte
                                        Scheiben unverzüglich nachschneiden zu können. Das spart Zeit und Geld.


                                        Definitionen

                                        Bruchpool                   Mit dem Bruchpool können Sie auf zu Bruch gegangene
                                                                    Scheiben schnell reagieren.

                                        LM                          Lagermaß

                                        Werte                       Im Bereich der Modellskizze gibt es folgende Werte:
                                                                    W=Breite
                                                                    H=Höhe
                                                                    T1,T2, … = Bruchrand
                                                                    <->=Spiegelkennzeichen
                                                                    @=Drehkennzeichen


                                        Merke

                                        Anzeige                     Die Anzeige aktualisiert sich automatisch.

                                        Filterfunktionen            Mit Hilfe der Filterfunktionen können Sie die Inhalte
                                                                    derAnzeige einschränken.
1.50 / 01-2023




                 50                                                                             A+W Production Terminal
                 Tutorial                                               Überblick A+W Production Terminal Manual Cutting




                                             Modul-Präsentation Terminal Manual Cutting
                                             Terminal Manual Cutting zeigt Ihnen alle freigegebenen Läufe bzw. Lose für
                                             einen bestimmten Zuschnitttisch. Bei dem Zuschnitttisch handelt es sich in der
                                             Regel um einen Handzuschnitttisch. Sofern Sie keinen Maschinencode am
                                             Tisch erzeugen müssen, kann das Terminal Manual Cutting auch an einem an-
                                             deren Tisch installiert sein.
                                             Nachdem Sie Terminal Manual Cutting gestartet haben, präsentiert sich das
                                             Modul wie folgt. Es werden die Daten angezeigt, die Sie über die Filterfunktion
                                             (s.u.) bestimmt haben:


                 A


                 B




                 C



                 D

                 E                                                                                                       F




                 A Menüleiste                               D Infofelder
                 B Arbeitsvorrat unter Berücksichtigung der E Meldungsfenster
                   Filter                                   F Schaltflächen
                 C Filterfunktionen
                 Abb. 9         Terminal Manual Cutting


                                             Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                             runter finden Sie den Arbeitsvorrat (B). Im Bereich (C) befinden sich die Filter-
                                             funktionen. Im Bereich (D) befinden sich die Infofelder. Unter (E) befindet sich
                                             das Meldungsfenster und unter (F) die Schaltflächen.

                                                Anzeige der Spalten ist frei konfigurierbar
                            I
1.50 / 01-2023




                                                Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                                schirmdarstellung von Ihrer Darstellung abweichen.




                 A+W Production Terminal                                                                                  51
                 Überblick A+W Production Terminal Manual Cutting                                             Tutorial




                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Die Bereiche (A), (D) und (E) von Terminal Manual Cutting sind identisch sind
                                        mit den Bereichen von Terminal IG-In und werden an dieser Stelle nicht noch
                                        einmal beschrieben.

                                        Bereich B - Arbeitsvorrat
                                        Dieser Bereich zeigt Ihnen alle freigegebenen Läufe bzw. Lose für den ent-
                                        sprechenden Tisch. Die Inhalte der Anzeige sind abhängig von den Filtern
                                        (Bereich C).
                                        Im Feld Lauf wird Ihnen die Laufnummer angezeigt. Das Feld Los zeigt Ihnen
                                        die Losnummer innerhalb des Laufes. Im Feld Bezeichnung sehen Sie die
                                        Glasbezeichnung. Das Feld LM zeigt Ihnen das Lagermaß. Wird Terminal Ma-
                                        nual Cutting an einem Handzuschnitttisch eingesetzt, steht im Feld LM eine -
                                        1. Das liegt daran, dass Handzuschnitt-Scheiben nicht optimiert wurden und
                                        somit kein Lagermaß vorhanden ist. Im Feld Termin sehen Sie den Produkti-
                                        onstermin. Das Feld Dicke zeigt Ihnen die Dicke der Glasart. Im Feld Stück
                                        wird Ihnen die Stückzahl angezeigt und im Feld Modelle die Modell-Nummer.
                                        Im Feld Maschine sehen Sie, auf welchem Tisch die Glasart geschnitten wer-
                                        den soll. Im Feld Text finden Sie eventuelle Beschreibungen.

                                        Bereich C - Filterfunktionen
                                        Im Bereich Filter finden Sie vier Komboboxen, mit deren Hilfe Sie den Inhalt
                                        der Anzeige einschränken können. In der rechten, oberen Kombobox ist stan-
                                        dardmäßig der Tisch ausgewählt, für den Terminal Manual Cutting vorgese-
                                        hen ist. Sie können jederzeit einen anderen Tisch auswählen, betätigen Sie
                                        anschließend die Schaltfläche [Aktualisieren] und die Anzeige wird der neuen
                                        Filterfunktion angepasst. Die Kombobox darunter steht standardmäßig auf
                                        Nicht fertig. Das bedeutet, es werden nur Glasarten angezeigt, die noch nicht
                                        freigegeben sind. Sollten Sie versehentlich einen Lauf freigegeben haben und
                                        sich dieser nicht mehr in der Anzeige befinden, können Sie die linke, untere
                                        Kombobox öffnen und Eintrag fertig wählen. Um die Anzeige zu aktualisieren,
                                        betätigen Sie die Schaltfläche [Aktualisieren].
                                        Über die Kombobox Filter 2 können Sie sich einzelne Läufe anzeigen lassen.
                                        Wählen Sie Lauf und geben Sie im Feld dahinter die entsprechende Laufnum-
                                        mer an. Sie können sich auch Läufe von bis anzeigen lassen. Dann wählen
                                        Sie aus der Kombobox Lauf von … bis … und geben im ersten Feld dahinter
                                        die Laufnummer ein, mit der begonnen werden soll und im zweiten Feld die
                                        Laufnummer, mit der geendet werden soll. Anschließend betätigen Sie die
                                        Schaltfläche [Aktualisieren].

                                           Filter löschen
                                           Zum Löschen der Filter öffnen Sie die Kombobox und wählen den Eintrag
                                           ---. Vergessen Sie nicht, die Schaltfläche [Aktualisieren] zu betätigen.
1.50 / 01-2023




                 52                                                                        A+W Production Terminal
                 Tutorial                                              Überblick A+W Production Terminal Manual Cutting




                                           Bereich F - Schaltflächen
                                           In diesem Bereich befindet sich drei Schaltflächen.
                                           Mit der Schaltfläche [Freigabe] geben Sie den bzw. die ausgewählten Läufe
                                           frei. Die Schaltfläche [Aktualisieren] dient dem Aktualisieren der Anzeige. Un-
                                           terhalb der Schaltfläche befindet sich ein Fortschrittsbalken. Terminal Manual
                                           Cutting kann so eingestellt werden, dass sich die Anzeige alle 60 Sekunden
                                           aktualisiert. An dem Balken können Sie dann den Fortschritt erkennen. Die
                                           Schaltfläche [Bruchpool] öffnet den Bruchpool.


                                           Ergänzende Informationen
                                            Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19

                                           Einen Lauf freigeben
                                           Nachdem Sie im Hauptfenster die entsprechende Auswahl zum Buchen ge-
                                           troffen haben, betätigen Sie die Schaltfläche [Freigabe]. Es öffnet sich der Di-
                                           alog Freigabe. In diesem Dialog sind jetzt alle Scheiben einzeln aufgelistet,
                                           d. h. wenn Sie im Hauptfenster einen Lauf mit 64 Scheiben markiert haben,
                                           finden Sie im Dialog Freigabe diese 64 Scheiben einzeln aufgelistet.



                   A




                   B                                                                                                  E
                   C




                                                                                                                      F
                   D


                 A Auswahl                                 C SN-Zeichnung                E Gestell
                 B Modellanzeige                           D Selektiert von Gesamt       F Schaltflächen
                 Abb. 10    Freigabe


                                           Bereich A - Auswahl
                                           Im Feld Lauf wird Ihnen die Laufnummer angezeigt. Das Feld Los zeigt Ihnen
                                           die Losnummer innerhalb des Laufes. Im Feld Glasart sehen Sie die Glasbe-
                                           zeichnung. Das Feld Barcode zeigt Ihnen die Etikettnummer. Im Feld Bock se-
                                           hen Sie die Gestellnummer und im Feld Fach die entsprechende
                                           Fachnummer. Im Feld Pr.-Nr. wird Ihnen die Menge angezeigt, die produziert
1.50 / 01-2023




                                           werden soll. Das Feld Modell zeigt Ihnen die Modellnummer. Im Feld ZS-Brei-
                                           te wird Ihnen die Breite angezeigt und im Feld ZS-Höhe die Höhe. Im Feld Auf-
                                           trag sehen Sie die Auftragsnummer und im Feld Pos die Positionsnummer.


                 A+W Production Terminal                                                                                  53
                 Überblick A+W Production Terminal Manual Cutting                                                 Tutorial




                                        Bereich B - Modellanzeige
                                        In diesem Bereich befindet sich die Modellanzeige.

                                        Bereich C - Modellskizze
                                        In diesem Bereich sehen Sie die Modellskizze.
                                        Die Tabelle daneben zeigt Ihnen die entsprechenden Werte. Folgende Werte
                                        sind möglich:
                                        • W = Breite
                                        • H = Höhe
                                        • T1, T2, … = Bruchrand
                                        • <-> = Spiegelkennzeichen
                                        • @ = Drehkennzeichen

                                        Bereich E - Gestell
                                        In diesem Bereich befinden sich die Daten zum Gestell. Sie können die Ge-
                                        stellnummer eingeben oder aber scannen. Wenn das Gestell leer ist, aktivie-
                                        ren Sie die Checkbox Beginn.
                                        Im Feld Charge können Sie eine Chargenbezeichnung hinterlegen.

                                        Bereich D - Selektiert von Gesamt
                                        In diesem Bereich sehen Sie, wie viele Scheiben Sie in der Tabelle markiert
                                        haben und die Gesamtstückzahl. Bsp.: 1/64 bedeutet, dass 64 Scheiben in der
                                        Tabelle angezeigt werden und Sie 1 Scheibe davon markiert haben.

                                        Bereich F - Schaltflächen
                                        Wenn Sie die Schaltfläche [Produzieren] betätigen, wird die bzw. werden die
                                        markierten Scheiben gebucht. Über die Schaltfläche [Eti Druck] wird für die
                                        bzw. werden für die markierten Scheiben die Etiketten gedruckt. Über die
                                        Schaltfläche [Bruch] buchen Sie markierte Scheiben als Bruch und mit [Abbre-
                                        chen] wird der Dialog geschlossen.


                                        Ergänzende Informationen
                                         Tutorial, “Ablauf von Arbeitsschritten” auf Seite 58
                                         Softwarereferenz, “Freigabe” auf Seite 150
1.50 / 01-2023




                 54                                                                              A+W Production Terminal
                 Tutorial                                            Überblick A+W Production Terminal Manual Cutting




                                            Mit dem Bruchpool arbeiten
                                            Mit diesem Instrument haben Sie die Möglichkeit, auf zu Bruch gegangene
                                            Scheiben schnell reagieren zu können. Wird irgendwo in der Produktion eine
                                            Scheibe als Bruch gescannt, öffnet sich der Dialog Bruchpool automatisch.
                                            Die zu Bruch gegangene Scheibe ist dann im Bruchpool enthalten und kann
                                            sofort nachgeschnitten werden (ohne über die Haupttische oder den automa-
                                            tischen Zuschnitt zu laufen).



                            A




                            B
                            C




                            D


                 A Inhalt Bruchpool                       C Modellskizze
                 B Modellanzeige                          D Schaltflächen
                 Abb. 11        Bruchpool


                                            Bereich A - Inhalt
                                            Im Feld Artikel wird Ihnen die Artikelnummer angezeigt. Das Feld Bezeich-
                                            nung zeigt Ihnen die Glasbezeichnung. Das Feld Dicke zeigt Ihnen die Glas-
                                            dicke. Das Feld Breite zeigt Ihnen die Breite der Scheibe und das Feld Höhe
                                            zeigt Ihnen die Höhe der Scheibe. Im Feld Lauf sehen Sie die Laufnummer.
                                            Das Feld Kunde zeigt Ihnen den Namen des Kunden. Im Feld Auftrag sehen
                                            Sie die Auftragsnummer und im Feld Pos die Positionsnummer. Das Feld Eti-
                                            kett zeigt Ihnen die Etikettnummer. Das Feld Modell zeigt Ihnen die Modell-
                                            nummer und im Feld Bock sehen Sie die Gestellnummer. Das Feld
                                            Liefertermin zeigt Ihnen das Lieferdatum.

                                            Bereich B - Modellanzeige
1.50 / 01-2023




                                            In diesem Bereich befindet sich die Modellanzeige.




                 A+W Production Terminal                                                                           55
                 Überblick A+W Production Terminal Manual Cutting                                                 Tutorial




                                        Bereich C - Modellskizze
                                        In diesem Bereich sehen Sie die Modellskizze.
                                        Die Tabelle daneben zeigt Ihnen die entsprechenden Werte. Folgende Werte
                                        sind möglich:
                                        • W = Breite
                                        • H = Höhe
                                        • T1, T2, … = Bruchrand
                                        • <-> = Spiegelkennzeichen
                                        • @ = Drehkennzeichen

                                        Bereich D - Schaltflächen
                                        Wenn Sie die Schaltfläche [Aktualisieren] betätigen, wird die Anzeige aktuali-
                                        siert. Über die Schaltfläche [Hinzufügen] können Sie selber dem Bruchpool
                                        eine Scheibe hinzufügen. Es öffnet sich der Dialog Brucherfassung. Über die
                                        Schaltfläche [Löschen] können Sie eine markierte Scheibe löschen. Die
                                        Schaltflächen [Drucken] und [Drucken2] werden vor Ort angepasst und dienen
                                        dem Drucken (Etiketten, Reports). Betätigen Sie die Schaltfläche [BDE bu-
                                        chen], wird die markierte Scheibe gebucht. Mit [Abbrechen] wird der Dialog
                                        geschlossen.


                                        Ergänzende Informationen
                                         Tutorial, “Ablauf von Arbeitsschritten” auf Seite 58
                                         Softwarereferenz, “Bruchpool” auf Seite 152
1.50 / 01-2023




                 56                                                                              A+W Production Terminal
                 Tutorial                                              Überblick A+W Production Terminal Manual Cutting




                                           Dem Bruchpool eine Scheibe manuell zufügen
                                           Über die Brucherfassung können Sie Brüche manuell dem Bruchpool hinzufü-
                                           gen.




                                           Abb. 12       Brucherfassung


                                           Erläuterung der Felder im Bereich Kunde
                                           Im Feld Auftrag geben Sie die entsprechende Auftragsnummer ein und im
                                           Feld Position die dazugehörige Positionsnummer.

                                           Erläuterung der Felder im Bereich Teile
                                           Im Feld Auftrag wird Ihnen die Auftragsnummer angezeigt und im Feld Positi-
                                           on die dazugehörige Positionsnummer. Im Feld TeileNr. sehen Sie die Teile-
                                           nummer und im Feld Glasart die Glasbezeichnung. Die Felder Breite und
                                           Höhe zeigen Ihnen die Abmessungen der Scheibe.

                                           Erläuterung der Felder im Bereich Bruchgrund
                                           Die Kombobox enthält alle möglichen Bruchgründe. Wählen Sie den entspre-
                                           chenden Bruchgrund aus.

                                           Erläuterung der Felder im Bereich Barcodes
                                           Im Feld Etikett wird Ihnen die Etikettnummer angezeigt und im Feld ES die Er-
                                           fassungsstelle. Im Feld Gestell sehen Sie die Gestellnummer.


                                           Ergänzende Informationen
1.50 / 01-2023




                                            Tutorial, “Ablauf von Arbeitsschritten” auf Seite 58
                                            Softwarereferenz, “Brucherfassung” auf Seite 154




                 A+W Production Terminal                                                                            57
                 Überblick A+W Production Terminal Manual Cutting                                              Tutorial




                                        Ablauf von Arbeitsschritten
                                        Die Vorgehensweise zum Arbeiten in Terminal Manual Cutting ist:
                                        •   Starten Sie das Modul Terminal Manual Cutting.
                                        •   Melden Sie sich an (<Name>).
                                        •   Wählen Sie den Lauf aus, der freigegeben werden soll.
                                        •   Geben Sie den Lauf frei.
                                        •   Weisen Sie ein Gestell zu.
                                        •   Buchen Sie den Lauf.
                                        •   Bruchpool: Fügen Sie einen Bruch manuell zu (optional).
                                        •   Bruchpool: Löschen Sie eine Scheibe (optional).
                                        Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                        protokollieren. Gründe für eine Unterbrechung können sein:
                                        •   Wartung der Maschine.
                                        •   Störung der Maschine.
                                        •   Pausenzeiten.
                                        Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                        weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                        Mängel können sein:
                                        •   Bruch
                                        •   Kratzer
                                        •   Riss

                                        Anmelden an der Arbeitsstation
                                        Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                        Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                         Tutorial, “So melden Sie sich an” auf Seite 24


                                         So wählen Sie einen Lauf aus
                                        1 Wählen Sie den gewünschten Lauf aus.




                                        2 Anschließend betätigen Sie die Schaltfläche [Freigabe [F5]]. Es öffnet sich
                                          der Dialog Freigabe.
                                        3 In diesem Dialog sind jetzt alle Scheiben einzeln aufgelistet, d. h. wenn Sie
                                          im Hauptfenster einen Lauf mit 64 Scheiben markiert haben, finden Sie im
                                          Dialog Freigabe diese 64 Scheiben einzeln aufgelistet. Die Scheiben sind
                                          standardmäßig alle ausgewählt.
                                        4 Sie können jetzt entweder alle Scheiben der Anzeige buchen oder einzelne
1.50 / 01-2023




                                          durch anklicken.
                                        5 Geben Sie im Feld Gestell die Gestell-Nr. ein oder scannen Sie diese. Falls
                                          es sich um ein leeres Gestell handelt, aktivieren Sie die Checkbox Beginn.


                 58                                                                         A+W Production Terminal
                 Tutorial                                           Überblick A+W Production Terminal Manual Cutting




                                           6 Zum Buchen betätigen Sie die Schaltfläche [Produzieren].


                                            So buchen Sie die ausgewählte(n) Scheibe(n)
                                           1 Wählen Sie die gewünschte Scheibe aus.




                                           2 Geben Sie im Feld Gestell die Gestell-Nr. ein oder scannen Sie diese. Falls
                                             es sich um ein leeres Gestell handelt, aktivieren Sie die Checkbox Beginn.
                                             Arbeiten Sie mit einem Scanner, können Sie auch den Barcode Beginn
                                             scannen.
                                           3 Geben Sie eine Chargenbezeichnung ein (optional).
                                           4 Zum Buchen betätigen Sie die Schaltfläche [Produzieren].


                                            So fügen Sie einen Bruch manuell hinzu
                                           1 Öffnen Sie die Brucherfassung.
                                           2 Geben Sie im Feld Auftrag die entsprechende Auftragsnummer ein.
                                           3 Geben Sie im Feld Position die entsprechende Positionsnummer ein. Im
                                             Bereich Teile werden Ihnen die zu der Auftrags- und Positionsnummer ge-
                                             hörenden Teile angezeigt.
                                           4 Öffnen Sie im Bereich Bruchgrund die Kombobox.
                                           5 Wählen Sie den Bruchgrund aus, z. B. Kratzer.
                                           6 Wählen Sie im Bereich Barcodes die Scheibe aus, die Sie hinzufügen
                                             möchten.
                                           7 Betätigen Sie die Schaltfläche [Speichern].
                                           8 Der Dialog wird geschlossen. Sie befinden sich im Dialog Bruchpool, der
                                             die soeben gebuchte Scheibe enthält.


                                            So löschen Sie eine Scheibe aus dem Bruchpool
                                           1 Öffnen Sie den Bruchpool.
                                           2 Wählen Sie die gewünschte Scheibe aus.




                                           3 Betätigen Sie die Schaltfläche [Löschen].
                                           4 Die Scheibe wird gelöscht. Der Dialog bleibt geöffnet.
1.50 / 01-2023




                 A+W Production Terminal                                                                             59
                 Überblick A+W Production Terminal Manual Cutting                                                 Tutorial




                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                        befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                        Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                        Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                        In ausführlich beschrieben.
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28


                                        Weitere Funktionen
                                        Zu den weiteren Funktionen zählen:
                                        •   Listen (Reports)
                                        •   Log-Einträge
                                        •   Unterschiedliche Programm-Sprachen
                                        Da in diesem Bereich die Felder von Terminal Manual Cutting identisch sind
                                        mit den Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch ein-
                                        mal beschrieben.


                                        Ergänzende Informationen
                                         Tutorial, “Listen (Reports) generieren” auf Seite 31
                                         Tutorial, “Log-Einträge exportieren” auf Seite 31
                                         Tutorial, “Programmsprache wählen” auf Seite 32
                                         Softwarereferenz, “Freigabe” auf Seite 150
                                         Softwarereferenz, “Bruchpool” auf Seite 152
                                         Softwarereferenz, “Brucherfassung” auf Seite 154
1.50 / 01-2023




                 60                                                                              A+W Production Terminal
                 Tutorial                                            Überblick A+W Production Terminal Georgian Bars




                                           Überblick A+W Production
                                           Terminal Georgian Bars
                                           In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                           dem A+W Production Terminal Georgian Bars kennen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Arbeiten mit Terminal Georgian Bars
1.50 / 01-2023




                 A+W Production Terminal                                                                         61
                 Überblick A+W Production Terminal Georgian Bars                                                      Tutorial




                                        Arbeiten mit Terminal Georgian Bars
                                        Lernziele

                                        •   Oberfläche von Terminal Georgian Bars kennenlernen.
                                        •   Die Funktionsweise kennenlernen und verstehen.
                                        •   Läufe freigeben.
                                        •   Mit dem Bruchpool arbeiten.
                                        •   Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                        Nutzen

                                        Mit Terminal Georgian Bars können Sie sich das zu produzierende Sprossenbild am
                                        Monitor anzeigen lassen. Nachdem die Sprossen produziert wurden, kann das ISO
                                        produziert werden. Durch die Vernetzung der einzelnen Terminals ist ein Nachfragen
                                        an der entsprechenden Produktionsstelle nicht mehr nötig.


                                        Definitionen

                                        Pos                         Auftragsposition

                                        PPos                        Produktionsposition


                                        Merke

                                        Drucken                     Sie können sich das Sprossenbild am Arbeitsplatz
                                                                    ausdrucken lassen.

                                        Filterfunktionen            Mit Hilfe der Filterfunktionen können Sie die Inhalte der
                                                                    Anzeige einschränken.
1.50 / 01-2023




                 62                                                                             A+W Production Terminal
                 Tutorial                                               Überblick A+W Production Terminal Georgian Bars




                                             Modul-Präsentation Terminal Georgian Bars
                                             Terminal Georgian Bars zeigt Ihnen alle freigegebenen Läufe bzw. Lose, die
                                             Sprossen enthalten.
                                             Nachdem Sie Terminal Georgian Bars gestartet haben, präsentiert sich das
                                             Modul wie folgt. Es werden die Daten angezeigt, die Sie über die Filterfunktion
                                             (s.u.) bestimmt haben:


                 A


                 B




                 C



                 D

                 E                                                                                                       F




                 A Menüleiste                               D Infofelder
                 B Arbeitsvorrat unter Berücksichtigung der E Meldungsfenster
                   Filter                                   F Schaltflächen
                 C Filterfunktionen
                 Abb. 13        Terminal Georgian Bars


                                             Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                             runter finden Sie den Arbeitsvorrat (B). Im Bereich (C) befinden sich die Filter-
                                             funktionen. Im Bereich (D) befinden sich die Infofelder. Unter (E) befindet sich
                                             das Meldungsfenster und unter (F) die Schaltflächen.

                                                Anzeige der Spalten ist frei konfigurierbar
                            I




                                                Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                                schirmdarstellung von Ihrer Darstellung abweichen.
1.50 / 01-2023




                 A+W Production Terminal                                                                                  63
                 Überblick A+W Production Terminal Georgian Bars                                               Tutorial




                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Die Bereiche (A), (D) und (E) von Terminal Georgian Bars sind identisch sind
                                        mit den Bereichen von Terminal IG-In und werden an dieser Stelle nicht noch
                                        einmal beschrieben.

                                        Bereich B - Arbeitsvorrat
                                        Dieser Bereich zeigt Ihnen alle freigegebenen Läufe bzw. Lose, die Sprossen
                                        enthalten. Die Inhalte der Anzeige sind abhängig von den Filtern (Bereich C).
                                        Im Feld Lauf wird Ihnen die Laufnummer angezeigt. Das Feld Bezeichnung
                                        zeigt Ihnen, um welche Sprosse es sich handelt. Im Feld Termin sehen Sie den
                                        Produktionstermin. Das Feld Dicke zeigt Ihnen die Dicke der Sprosse. Im Feld
                                        Stück wird Ihnen die Stückzahl angezeigt und im Feld Modelle die Modell-
                                        Nummer. Im Feld Maschine sehen Sie, wo die Sprosse geschnitten werden
                                        soll. Im Feld Text finden Sie eventuelle Beschreibungen.

                                        Bereich C - Filterfunktionen
                                        Im Bereich Filter finden Sie vier Komboboxen, mit deren Hilfe Sie den Inhalt
                                        der Anzeige einschränken können. In der rechten, oberen Kombobox ist stan-
                                        dardmäßig der Platz ausgewählt, für den Terminal Georgian Bars vorgesehen
                                        ist. Sie können jederzeit einen anderen Platz auswählen, betätigen Sie an-
                                        schließend die Schaltfläche [Aktualisieren] und die Anzeige wird der neuen Fil-
                                        terfunktion angepasst. Die Kombobox darunter steht standardmäßig auf Nicht
                                        fertig. Das bedeutet, es werden nur Sprossen angezeigt, die noch nicht freige-
                                        geben sind. Sollten Sie versehentlich einen Lauf freigegeben haben und sich
                                        dieser nicht mehr in der Anzeige befinden, können Sie die linke, untere Kom-
                                        bobox öffnen und Eintrag fertig wählen. Um die Anzeige zu aktualisieren, be-
                                        tätigen Sie die Schaltfläche [Aktualisieren].
                                        Über die Kombobox Filter 2 können Sie sich einzelne Läufe anzeigen lassen.
                                        Wählen Sie Lauf und geben Sie im Feld dahinter die entsprechende Laufnum-
                                        mer an. Sie können sich auch Läufe von bis anzeigen lassen. Dann wählen
                                        Sie aus der Kombobox Lauf von … bis … und geben im ersten Feld dahinter
                                        die Laufnummer ein, mit der begonnen werden soll und im zweiten Feld die
                                        Laufnummer, mit der geendet werden soll. Anschließend betätigen Sie die
                                        Schaltfläche [Aktualisieren].

                                           Filter löschen
                                           Zum Löschen der Filter öffnen Sie die Kombobox und wählen den Eintrag
                                           ---. Vergessen Sie nicht, die Schaltfläche [Aktualisieren] zu betätigen.
1.50 / 01-2023




                 64                                                                         A+W Production Terminal
                 Tutorial                                              Überblick A+W Production Terminal Georgian Bars




                                           Bereich F - Schaltflächen
                                           In diesem Bereich befindet sich zwei Schaltflächen.
                                           Mit der Schaltfläche [Freigabe] geben Sie den bzw. die ausgewählten Läufe
                                           frei. Die Schaltfläche [Aktualisieren] dient dem Aktualisieren der Anzeige. Un-
                                           terhalb der Schaltfläche befindet sich ein Fortschrittsbalken. Terminal Georgi-
                                           an Bars kann so eingestellt werden, dass sich die Anzeige alle 60 Sekunden
                                           aktualisiert. An dem Balken können Sie dann den Fortschritt erkennen.


                                           Ergänzende Informationen
                                            Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19

                                           Einen Lauf freigeben
                                           Nachdem Sie im Hauptfenster die entsprechende Auswahl zum Buchen ge-
                                           troffen haben, betätigen Sie die Schaltfläche [Freigabe]. Es öffnet sich der Di-
                                           alog Sprossen-Freigabe. In diesem Dialog sind jetzt alle Sprossen einzeln
                                           aufgelistet, d. h. wenn Sie im Hauptfenster einen Lauf mit 64 Sprossen mar-
                                           kiert haben, finden Sie im Dialog Freigabe diese 64 Sprossen einzeln aufge-
                                           listet. Nachdem sich der Dialog geöffnet hat, sind alle Sprossen markiert. Um
                                           sich ein einzelnes Sprossenbild anzeigen zu lassen, müssen Sie die entspre-
                                           chende Position auswählen.




                 A




                                                                                                                    D




                 B

                                                                                                                    E
                 C

                 A Auswahl                                 C Selektiert von Gesamt       E Schaltflächen
                 B Gestell                                 D Sprossenbild
1.50 / 01-2023




                 Abb. 14     Sprossen-Freigabe




                 A+W Production Terminal                                                                                65
                 Überblick A+W Production Terminal Georgian Bars                                                  Tutorial




                                        Bereich A - Auswahl
                                        Im Feld Lauf wird Ihnen die Laufnummer angezeigt. Das Feld Etikett zeigt Ih-
                                        nen die Etikettnummer. Im Feld Bezeichnung sehen Sie die Sprossenbezeich-
                                        nung. Das Feld Auftrag zeigt Ihnen die Auftragsnummer. Im Feld Pos sehen
                                        Sie die Auftragspositionsnummer und im Feld PPos die entsprechende Pro-
                                        duktionsposition. Das Feld Termin zeigt Ihnen die Produktionstermin.

                                        Bereich B - Gestell (Verwendung: optional)
                                        In diesem Bereich befinden sich die Daten zum Gestell. Sie können die Ge-
                                        stellnummer eingeben oder aber scannen. Wenn das Gestell leer ist, aktivie-
                                        ren Sie die Checkbox Beginn.
                                        Im Feld Charge können Sie eine Chargenbezeichnung hinterlegen.

                                        Bereich C - Selektiert von Gesamt
                                        In diesem Bereich sehen Sie, wie viele Sprossen Sie in der Tabelle markiert
                                        haben und die Gesamtstückzahl. Bsp.: 1/64 bedeutet, dass 64 Sprossen in der
                                        Tabelle angezeigt werden und Sie 1 Sprosse davon markiert haben.

                                        Bereich D - Sprossenbild
                                        In diesem Bereich sehen Sie, wie die Scheibe später mit den verbauten Spros-
                                        sen aussehen wird.

                                        Bereich E - Schaltflächen
                                        Wenn Sie die Schaltfläche [Produzieren] betätigen, wird die bzw. werden die
                                        markierten Sprosse gebucht. Über die Schaltfläche [Drucken] können Sie das
                                        Sprossenbild an einem lokalen Drucker ausgeben. Über die Schaltfläche
                                        [Bruch] buchen Sie markierte Sprosse als Bruch und mit [Abbrechen] wird der
                                        Dialog geschlossen.


                                        Ergänzende Informationen
                                         Tutorial, “Ablauf von Arbeitsschritten” auf Seite 58
                                         Softwarereferenz, “Freigabe” auf Seite 150
1.50 / 01-2023




                 66                                                                              A+W Production Terminal
                 Tutorial                                              Überblick A+W Production Terminal Georgian Bars




                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal Georgian Bars ist:
                                           •   Starten Sie das Modul Terminal Georgian Bars.
                                           •   Melden Sie sich an (<Name>).
                                           •   Wählen Sie den Lauf aus, der freigegeben werden soll.
                                           •   Geben Sie den Lauf frei.
                                           •   Weisen Sie ein Gestell zu.
                                           •   Buchen Sie den Lauf.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Sprosse, die Sie gerade buchen wollen, eine Beschädigung auf-
                                           weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                           Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So wählen Sie einen Lauf aus
                                           1 Wählen Sie den gewünschten Lauf aus.




                                           2 Anschließend betätigen Sie die Schaltfläche [Freigabe [F5]]. Es öffnet sich
                                             der Dialog Sprossen-Freigabe.
                                           3 In diesem Dialog sind jetzt alle Sprossen einzeln aufgelistet, d. h. wenn Sie
                                             im Hauptfenster einen Lauf mit 64 Sprossen markiert haben, finden Sie im
                                             Dialog Sprossen-Freigabe diese 64 Sprossen einzeln aufgelistet. Die
                                             Sprossen sind standardmäßig alle ausgewählt.
                                           4 Sie können jetzt entweder alle Sprossen der Anzeige buchen oder einzelne
                                             durch anklicken.
                                           5 Optional: Geben Sie im Feld Gestell die Gestell-Nr. ein oder scannen Sie
1.50 / 01-2023




                                             diese. Falls es sich um ein leeres Gestell handelt, aktivieren Sie die Check-
                                             box Beginn.
                                           6 Zum Buchen betätigen Sie die Schaltfläche [Produzieren].


                 A+W Production Terminal                                                                               67
                 Überblick A+W Production Terminal Georgian Bars                                                Tutorial




                                         So buchen Sie die ausgewählte(n) Sprosse(n)
                                        1 Wählen Sie die gewünschte Sprosse aus.




                                        2 Geben Sie im Feld Gestell die Gestell-Nr. ein oder scannen Sie diese. Falls
                                          es sich um ein leeres Gestell handelt, aktivieren Sie die Checkbox Beginn.
                                          Arbeiten Sie mit einem Scanner, können Sie auch den Barcode Beginn
                                          scannen.
                                        3 Geben Sie eine Chargenbezeichnung ein (optional).
                                        4 Zum Buchen betätigen Sie die Schaltfläche [Produzieren].

                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26


                                        Weitere Funktionen
                                        Zu den weiteren Funktionen zählen:
                                        •   Listen (Reports)
                                        •   Log-Einträge
                                        •   Unterschiedliche Programm-Sprachen
                                        Da in diesem Bereich die Felder von Terminal Manual Cutting identisch sind
                                        mit den Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch ein-
                                        mal beschrieben.


                                        Ergänzende Informationen
                                         Tutorial, “Listen (Reports) generieren” auf Seite 31
                                         Tutorial, “Log-Einträge exportieren” auf Seite 31
                                         Tutorial, “Programmsprache wählen” auf Seite 32
1.50 / 01-2023




                                         Softwarereferenz, “Sprossen-Freigabe” auf Seite 157




                 68                                                                            A+W Production Terminal
                 Tutorial                                                   Überblick A+W Production Terminal Order




                                           Überblick A+W Production
                                           Terminal Order
                                           In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                           dem A+W Production Terminal Order (Terminal Order) kennen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Arbeiten mit Terminal Order
                                           •   Modul-Präsentation Terminal Order
                                           •   Ablauf von Arbeitsschritten
                                           •   Weitere Funktionen
1.50 / 01-2023




                 A+W Production Terminal                                                                        69
                 Überblick A+W Production Terminal Order                                                               Tutorial




                                        Arbeiten mit Terminal Order
                                        Lernziele

                                        •   Oberfläche von Terminal Order kennenlernen.
                                        •   Die Funktionsweise kennenlernen und verstehen.
                                        •   Aufträge und Positionen laden.
                                        •   Die richtigen Teile (Oberteil/Unterteil) wählen.
                                        •   Mengen korrekt buchen.
                                        •   Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                        Nutzen

                                        Mit Terminal Order können Sie größere Mengen auf einmal laden und buchen. Das
                                        spart Zeit und minimiert Fehler.


                                        Definitionen

                                        Oberteil                    Oberteile sind übergeordnete Teile. Sie tragen die
                                                                    Teilenummer 0, z. B. ISO.

                                        Unterteil                   Unterteile sind untergeordnete Teile. Sie tragen die
                                                                    Teilenummern 1, 2, usw. z. B. Float.


                                        Merke

                                        Richtiges Teil auswählen    Denken Sie beim Buchen der Teile daran, das richtige
                                                                    Teil auszuwählen.

                                        Erfassungsstellen ohne      Teile können auch auf Erfassungsstellen gebucht
                                        Bearbeitungen               werden, die keine Bearbeitung haben, z. B. Sortieren.

                                        Reset                       Über diese Schaltfläche leeren Sie die Anzeige.

                                        Symbol Grüner Hacken        Die Bearbeitung wurde bereits gemacht.

                                        Symbol Rotes X              Die Bearbeitung ist noch offen, kann aber an der
                                                                    angemeldeten Maschine nicht gemacht werden.
1.50 / 01-2023




                 70                                                                             A+W Production Terminal
                 Tutorial                                                         Überblick A+W Production Terminal Order




                                           Modul-Präsentation Terminal Order
                                           Mit Terminal Order haben Sie die Möglichkeit größere Mengen zu verbuchen.
                                           Bearbeitungen, die mit der jeweiligen Erfassungsstelle verknüpft sind, werden
                                           dabei mit gebucht.
                                           Nachdem Sie Terminal Order gestartet haben, präsentiert sich das Modul wie
                                           folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn
                                           Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B                                                                                                      H

                 C




                 D




                 E                                                                                                      I




                 F


                 G                                                                                                      J



                 A   Menüleiste                           F   Infofelder
                 B   Suchfelder                           G   Meldungsfenster
                 C   Filterfunktion                       H   Modellvorschau
                 D   Mengenübersicht/Buchungsbereich      I   Bearbeitungsliste
                 E   Vorschauliste                        J   Schaltflächen
                 Abb. 15      Terminal Order


                                           Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                           runter finden Sie die Suchfelder für die Auftragsposition (B). Im Bereich (C) fin-
                                           den Sie die Filterfunktionen. In (D) sehen Sie, wie viele Einheiten noch offen
                                           sind sowie die Gesamtstückzahl. Der Bereich (E) zeigt Ihnen eine Übersicht
                                           zu allen Auftragspositionen. Im Bereich (F) befinden sich die Infofelder. Unter
                                           (G) befindet sich das Meldungsfenster. Der Bereich (H) zeigt Ihnen Modellvor-
                                           schau und im Bereich (I) befindet sich die Bearbeitungsliste. Unter (J) finden
1.50 / 01-2023




                                           Sie die Schaltflächen.




                 A+W Production Terminal                                                                                    71
                 Überblick A+W Production Terminal Order                                                         Tutorial




                                            Anzeige der Spalten ist frei konfigurierbar
                           I




                                            Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                            schirmdarstellung von Ihrer Darstellung abweichen.

                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Die Bereiche (A), (F), (G), und (J) von Terminal Order sind identisch sind mit
                                        den Bereichen von Terminal IG-In und werden an dieser Stelle nicht noch ein-
                                        mal beschrieben.

                                        Bereich B - Suchfelder
                                        Dieser Bereich dient zur Auswahl der Auftragsposition. Es stehen Ihnen drei
                                        Möglichkeiten zur Verfügung.
                                        •   Geben Sie die Auftrags- und/oder Positionsnummer im Bereich Auftrags-
                                            daten ein. Gibt es nur eine Position in dem Auftrag, genügt die Eingabe der
                                            Auftragsnummer. Anschließend betätigen Sie die Schaltfläche [Enter] oder
                                            die Schaltfläche [Suchen]. Die Daten werden geladen.
                                        •   Scannen des Barcodes. Die Daten werden geladen.
                                        •   Eintippen des Barcodes in das Feld Etikett. Anschließend betätigen Sie die
                                            Schaltfläche [Enter] oder die Schaltfläche [Suchen]. Die Daten werden ge-
                                            laden.

                                        Bereich C - Filter
                                        Um eine Scheibe auf eine Erfassungsstelle zu buchen, müssen Sie die Erfas-
                                        sungsstelle zunächst anmelden. Dazu öffnen Sie die Kombobox Erf.-Stelle
                                        und wählen die gewünschte Erfassungsstelle aus.
                                        Im Feld Bearbeitungen sehen Sie die Bearbeitungstypen, die der ausgewähl-
                                        ten Erfassungsstelle zugeordnet sind. Ein Buchen auf die Erfassungsstelle
                                        bedeutet auch ein Buchen der entsprechenden Bearbeitung.
                                        Darüber hinaus hat der Bereich Filter Einfluss auf die Vorschauliste. Je nach-
                                        dem, welche Erfassungsstelle Sie wählen und in Abhängigkeit der aktivierten
                                        oder deaktivierten Checkboxen im Bereich Teile/Bearbeitungen, ändert sich
                                        der Inhalt der Vorschauliste.
                                        Beispiel: Auftragsposition mit 3 ISO-Einheiten, Erfassungsstelle: ISO-Linie.
                                        Angezeigt werden die 3 ISO-Einheiten.
1.50 / 01-2023




                 72                                                                          A+W Production Terminal
                 Tutorial                                                      Überblick A+W Production Terminal Order




                                           Wir ändern die Erfassungsstelle: Zuschnitt. Angezeigt werden alle Unterteile
                                           der ISO-Einheiten.




                                               Richtige Teile auswählen
                                               Achten Sie beim Buchen der Positionen darauf, das richtige Teil (Oberteil/
                                               Unterteil) auszuwählen. Die jeweiligen Teile sind bereits den entsprechen-
                                               den Erfassungsstellen angepasst. Dennoch kann es vorkommen, dass Sie
                                               die per Standard definierten Bearbeitungen so nicht buchen können. Bei-
                                               spiel: Zuschnitt, unterschiedliche Glasarten.

                                           Bereich D - Mengenübersicht/Buchungsbereich
                                           Auftragspositionen können auf zwei unterschiedliche Arten gewählt werden.
                                           •   Markieren Sie in der Tabelle Übersicht die gewünschte(n) Position(en) mit
                                               einemDoppelklick. Die Anzahl im Feld Buchen wird entsprechend ange-
                                               passt.
                                           •   Geben Sie im Feld Buchen die anzahl der Positionen an, die gebucht wer-
                                               den sollen. Nachdem Sie die Schaltfläche [Enter] betätigt haben, weden in
                                               der Tabelle Übersicht die Auftragspositionen von oben nach unten ausge-
                                               wählt.
                                           Im Feld Offen/Fertig sehen Sie, wie viele offene Bearbeitungen existieren. 3/
                                           0 bedeutet, es sind insgesamt 3 Gläser mit offenen Bearbeitungen (oder Glä-
                                           ser, die noch nicht auf dieser Erfassungsstelle sind) und davon sind 0 ge-
                                           macht.

                                               Erfassungsstellen ohne Bearbeitungen
                                               Bei Erfassungsstellen ohne Bearbeitungen (z. B. Sortieren) hat das Feld
                                               keinen Eintrag. Dennoch können Sie die Scheiben auf eine solche Erfas-
                                               sungsstelle buchen.

                                           Im Feld Gestell können Sie (optional) den Gestellnamen eingeben oder den
                                           Barcode scannen. Die Scheiben werden dann auf das eingegebene Gestell
                                           gebucht. Haben Sie ein leeres Gestell, aktivieren Sie noch die Checkbox Be-
                                           ginn. Damit stellen Sie sicher, dass sich auf dem Gestell keine gebuchten
                                           Scheiben mehr befinden. Arbeiten Sie mit einem Scanner, können Sie auch
                                           den Barcode Beginn scannen und dann das Gestell.
1.50 / 01-2023




                 A+W Production Terminal                                                                             73
                 Überblick A+W Production Terminal Order                                                        Tutorial




                                        Bereich E - Vorschauliste
                                        In diesem Bereich erhalten Sie eine Übersicht zu allen Auftragspositionen, die
                                        noch nicht gebucht wurden.
                                        Das Feld Stk zeigt Ihnen die Stückzahl. Im Feld Etikett sehen Sie die Etikett-
                                        Nummer. Im Feld Auftrag wird Ihnen die Auftrags-Nummer und im Feld Pos.
                                        die Positionsnummer angezeigt. Die Felder Breite und Höhe zeigen Ihnen die
                                        Scheiben-Abmessungen der Position und das Feld Glasart zeigt Ihnen die
                                        Glasart. Im Feld Kunde sehen Sie, wer der Besteller ist. Das Feld Erfassungs-
                                        stelle zeigt Ihnen, an welcher Erfassungsstelle sich die Scheibe befindet. Ist
                                        das Feld leer, wurde die Scheibe noch keiner Erfassungsstelle zugeordnet. Im
                                        Feld Gestell sehen Sie, auf welchem Gestell sich die Scheibe befindet. Ist das
                                        Feld leer, wurde noch kein Gestell zugeordnet. Im Feld Prod.-Termin sehen
                                        Sie das Produktionsdatum und im Feld Teil die Teile-Nr.

                                        Bereich H - Modellvorschau mit Zoom-Funktion
                                        In diesem Bereich befindet sich die Modellvorschau der aktuell gewählten
                                        Scheiben.
                                        Über die Schaltfläche [Zoom] haben Sie die Möglichkeit, die Modellvorschau
                                        zu vergrößern. Wenn Sie die Schaltfläche betätigen, öffnet sich der Dialog
                                        SNLive mit dem vergrößerten Modell.
                                        Am linken, unteren Bildschirmrand befindet sich die Symbol-Schaltfläche für
                                        den Drucker. Betätigen Sie die Schaltfläche, öffnet sich der Dialog zum Dru-
                                        cken.
                                        Den Dialog SNLive verlassen Sie über die Schaltfläche [Schließen].

                                        Bereich I - Bearbeitungsliste
                                        In diesem Bereich erhalten Sie eine Übersicht zu den offenen Bearbeitungen.
                                        Eine grün hinterlegte Bearbeitung bedeutet, dass die Bearbeitung an dieser
                                        Maschine möglich ist. Hat die Bearbeitung einen grünen Haken, ist sie bereits
                                        gemacht. Ein rotes X bedeutet, dass die Bearbeitung noch zu machen ist, an
                                        der angemeldeten Maschine jedoch nicht möglich ist.


                                        Ergänzende Informationen
                                         Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19
1.50 / 01-2023




                 74                                                                            A+W Production Terminal
                 Tutorial                                                        Überblick A+W Production Terminal Order




                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten im Terminal Order ist:
                                           •   Starten Sie das Modul Terminal Order.
                                           •   Melden Sie sich an (<Name>).
                                           •   Geben Sie die Auftragsnummer ein oder scannen Sie diese.
                                           •   Geben Sie die Positionsnummer ein oder scannen Sie diese.
                                           •   Wählen Sie die Ziel-Erfassungsstelle aus.
                                           •   Weisen Sie ein Gestell zu (optional).
                                           •   Buchen Sie die Auftragsposition(en).
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                           weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                           Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So melden Sie eine Erfassungsstelle an
                                               Um eine Scheibe auf eine Erfassungsstelle zu buchen, müssen Sie die Er-
                                               fassungsstelle zunächst anmelden.




                                           1 Scannen Sie den entsprechenden Barcode oder öffnen Sie die Kombobox
                                             Erf.-Stelle.
                                           2 Wählen Sie die gewünschte Erfassungsstelle aus. Die der Erfassungsstel-
                                             le zugeordneten Bearbeitungstypen werden im Bereich Bearbeitungen an-
1.50 / 01-2023




                                             gezeigt. Arbeiten Sie mit einem Scanner, ist dieser Schritt nicht notwendig,
                                             die Daten werden nach dem Scannen der Erfassungsstelle automatisch
                                             geladen.


                 A+W Production Terminal                                                                             75
                 Überblick A+W Production Terminal Order                                                        Tutorial




                                         So melden Sie ein Gestell an
                                        1 Geben Sie die Gestellnummer des physikalischen Gestells ein oder scan-
                                          nen Sie den Barcode.
                                        2 Haben Sie ein leeres Gestell, aktivieren Sie nach der Anmeldung des Ge-
                                          stells die Checkbox Gestell leeren. Arbeiten Sie mit einem Scanner, kön-
                                          nen Sie auch den Barcode Beginn scannen.


                                         So produzieren Sie die Einheit/Scheibe
                                        1 Geben Sie die Auftragsnummer ein oder scannen Sie diese.
                                        2 Geben Sie die gewünschte(n) Auftragsposition(en) ein. Der Auftrag wird
                                          geladen und in der Vorschauliste angezeigt.
                                        3 Wählen Sie die gewünschte Erfassungsstelle aus oder scannen Sie diese.
                                        4 Geben Sie die Gestell-Nummer ein (optional).
                                        5 Aktivieren Sie die Checkbox Beginn [F11].
                                        6 Geben Sie die Charge ein (optional).
                                        7 Geben Sie im Feld Buchen die gewünschte Menge ein oder markieren Sie
                                          in der Vorschauliste die entsprechenden Positionen mit einem Doppelklick.
                                        8 Anschließend betätigen Sie die Schaltfläche [Produzieren [F5]].


                                         So leeren Sie die Anzeige
                                        1 Sie können die Anzeige zu jeder Zeit leeren.
                                        2 Betätigen Sie die Schaltfläche [Reset].
                                        3 Die Anzeige wird geleert.

                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26
1.50 / 01-2023




                 76                                                                            A+W Production Terminal
                 Tutorial                                                      Überblick A+W Production Terminal Order




                                           Umgang mit beschädigten Scheiben
                                           Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                           befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                           Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                           Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                           In ausführlich beschrieben.
                                            Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28


                                           Weitere Funktionen
                                           Zu den weiteren Funktionen zählen:
                                           •   Listen (Reports)
                                           •   Log-Einträge
                                           •   Unterschiedliche Programm-Sprachen
                                           Da in diesem Bereich die Felder von Terminal Order identisch sind mit den Fel-
                                           dern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                           schrieben.


                                           Ergänzende Informationen
                                            Tutorial, “Den Zustand der Maschine ändern” auf Seite 26
                                            Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28
                                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                                            Tutorial, “Log-Einträge exportieren” auf Seite 31
                                            Tutorial, “Programmsprache wählen” auf Seite 32
                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
1.50 / 01-2023




                 A+W Production Terminal                                                                             77
                 Überblick A+W Production Terminal Processing                                           Tutorial




                                        Überblick A+W Production
                                        Terminal Processing
                                        In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                        dem A+W Production Terminal Processing (Terminal Order) kennen.
                                        Der Themenblock beinhaltet folgende Schulungseinheiten:
                                        •   Arbeiten mit Terminal Processing
                                        •   Modul-Präsentation Terminal Processing
                                        •   Ablauf von Arbeitsschritten
                                        •   Weitere Funktionen
1.50 / 01-2023




                 78                                                                    A+W Production Terminal
                 Tutorial                                                   Überblick A+W Production Terminal Processing




                                           Arbeiten mit Terminal Processing
                                           Lernziele

                                           •   Oberfläche von Terminal Processing kennenlernen.
                                           •   Die Funktionsweise kennenlernen und verstehen.
                                           •   Den Arbeitsablauf kennenlernen.
                                           •   Eine Scheibe bearbeiten.
                                           •   Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                           Nutzen

                                           Das Arbeiten mit Terminal Processing ist nur dann effizient möglich, wenn Sie die
                                           Arbeitsweise des Programms verstehen und mit täglich auftretenden Situationen
                                           entsprechend umgehen können.


                                           Definitionen

                                           Code                        Maschinencode. Ist eine Sammlung von Befehlen, die
                                                                       von einer Maschine ausgeführt werden können.

                                           SN Ansicht                  Über die Kombobox können Sie sich die Scheibe in den
                                                                       verschiedenen SN Ansichten anzeigen lassen.

                                           Ausgang                     Kennzeichnet die Erfassungsstelle, auf die die Scheibe
                                                                       beim Produzieren gebucht wird.


                                           Merke

                                           Maschine anmelden           Bevor Sie mit der Arbeit beginnen, müssen Sie die
                                                                       Maschine anmelden.

                                           Anzeige leeren              Über diese Schaltfläche leeren Sie die Anzeige.
1.50 / 01-2023




                 A+W Production Terminal                                                                                       79
                 Überblick A+W Production Terminal Processing                                                           Tutorial




                                             Modul-Präsentation Terminal Processing
                                             Terminal Processing ist ein Leitrechner, der an Bearbeitungsmaschinen zum
                                             Einsatz kommt. Terminal Processing gibt Ihnen detaillierte Auskunft über die
                                             durchzuführenden Bearbeitungen inklusive maßstabgetreuer Produktions-
                                             zeichnungen.
                                             Nachdem Sie Terminal Processing gestartet haben, präsentiert sich das Mo-
                                             dul wie folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten.
                                             Wenn Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B
                                                                                                                           K

                 C



                 D
                 E


                                                                                                                           L

                 F                                                                                                         M

                 G

                 H

                 I

                 J

                 A    Menüleiste                            E   Auftragsdaten             I   Infofelder
                 B    Etikett- und Gestellnummer            F   Vorschau                  J   Schaltflächen
                 C    Info zur Scheibe                      G   Verlinkte Dokumente       K   SN Zeichnung
                 D    Info zum fertigen Produkt             H   Meldungsfenster           L   SN Ansicht
                                                                                          M   Liste der Bearbeitungen
                 Abb. 16        Terminal Processing


                                             Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                             runter finden Sie die Etikett- sowie die Gestellnummer der Scheibe (B). Im Be-
                                             reich (C) finden Sie die Informationen zur Scheibe und in (D) die Informationen
                                             zum fertigen Produkt. Der Bereich (E) zeigt Ihnen eine Übersicht zu den Auf-
                                             tragsdaten. Im Bereich (F) befindet sich die Vorschau. Unter (G) finden Sie die
                                             verlinkten Dokumente. Im Bereich (H) befindet sich das Meldungsfenster. Un-
                                             ter (I) finden Sie die Infofelder und unter (J) die Schaltflächen. Im Bereich (K)
1.50 / 01-2023




                                             befindet sich die SN Zeichnung inkl. Vermaßung und unter (L) die SN Ansicht.
                                             Unter (L) sehen Sie die Liste der Bearbeitungen.



                 80                                                                                A+W Production Terminal
                 Tutorial                                                Überblick A+W Production Terminal Processing




                                              Anzeige der Spalten ist frei konfigurierbar
                            I




                                              Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                              schirmdarstellung von Ihrer Darstellung abweichen.

                                           Detaillierte Erläuterung zu den einzelnen Bereichen
                                           Die Bereiche (A), (G), (H), und (I) von Terminal Processing sind identisch sind
                                           mit den Bereichen von Terminal IG-In und werden an dieser Stelle nicht noch
                                           einmal beschrieben.

                                           Bereich B - Etikett- und Gestellnummer
                                           Im Feld Etikett wird Ihnen die Etikettnummer der Scheibe angezeigt. Die Ein-
                                           gabe der Nummer kann per Tastatur oder Barcodescanner erfolgen.
                                           Im Feld dahinter können Sie (optional) den Gestellnamen oder -barcode ein-
                                           geben. Die Scheiben werden dann auf das eingegebene Gestell gebucht. Ha-
                                           ben Sie ein leeres Gestell, aktivieren Sie die Checkbox Gestell leeren. Damit
                                           stellen Sie sicher, dass sich auf dem Gestell keine gebuchten Scheiben mehr
                                           befinden. Arbeiten Sie mit einem Scanner, können Sie auch den Barcode Be-
                                           ginn scannen.

                                           Bereich C - Info zur Scheibe




                                           Im oberen Feld wird Ihnen die Glasart der Scheibe je Position angezeigt (z. B.
                                           Float 4 mm). Darunter finden Sie die Abmessungen der Scheibe.

                                           Bereich D - Info zum fertigen Produkt




                                           Dieser Bereich zeigt Ihnen die Produktbezeichnung des fertigen Produktes
                                           an.

                                           Bereich E - Auftragsdaten
1.50 / 01-2023




                                           Im Feld Auftrag wird Ihnen die Auftragsnummer angezeigt, zu dem die Schei-
                                           be gehört. Das Feld Pos. zeigt die Position des Kundenauftrags. Im Feld Men-
                                           ge wird die vom Kunden bestellte Menge Scheiben je Position angezeigt.



                 A+W Production Terminal                                                                               81
                 Überblick A+W Production Terminal Processing                                                   Tutorial




                                        Im Feld Lief. Term. sehen Sie den Liefertermin. Das Feld Kunde zeigt Ihnen
                                        den Namen des Kunden.




                                        Mit der Kombobox Ausgang können Sie wählen, auf welche Erfassungsstelle
                                        die Scheiben beim Produzieren gebucht werden. Bitte denken Sie daran, die
                                        ausgewählte Erfassungsstelle anzumelden.
                                        Im Feld Code sehen Sie den der Erfassungsstelle zugeordneten Treiber, der
                                        automatisch geladen wird. Sollte kein Treiber zugeordnet sein, können Sie
                                        diesen durch Öffnen der Kombobox Code auswählen.

                                        Bereich F - Vorschau
                                        Diese Liste zeigt alle zum Produzieren anstehenden Scheiben. So können Sie
                                        sich einen Vorrat von Scheiben in die Anzeige laden und dann produzieren.
                                        Die erste Scheibe ist immer die aktuell angezeigte Scheibe.

                                        Bereich G - Arbeitsvorrat
                                        Diese Liste zeigt alle zum Produzieren anstehenden Scheiben. So können Sie
                                        sich einen Vorrat von Scheiben in die Anzeige laden und dann produzieren.
                                        Die erste Scheibe ist immer die aktuell angezeigte Scheibe.

                                        Bereich J - Schaltflächen
                                        Die Schaltflächen [Produzieren], [Überspringen] und [Bruch melden] sind
                                        identisch sind mit den Schaltflächen von Terminal IG-In und werden an dieser
                                        Stelle nicht noch einmal beschrieben.
                                        Die Schaltfläche [Anzeige leeren] ist identisch mit der Schaltfläche [Reset] von
                                        Terminal Order und wird an dieser Stelle nicht noch einmal beschrieben.
                                        Mit der Schaltfläche [Code] wird der Treiber aufgerufen, um die Scheibe zu be-
                                        arbeiten. Die Scheibe bleibt danach in der Anzeige. Nachdem Sie die Schalt-
                                        fläche [Produzieren] betätigt haben, erfolgt die Buchung auf den Ausgang und
                                        die Scheibe verschwindet aus der Anzeige.

                                        Bereich K - SN Zeichnung
                                        Hier wird Ihnen die Auftragsposition als vermaßte Zeichnung dargestellt.
                                        Ein Klick auf die Zeichnung öffnet diese im Vollbildmodus. Um den Vollbildmo-
                                        dus zu schließen, betätigen Sie die Schaltfläche [Schließen] am rechten, un-
                                        teren Bildschirmrand.
1.50 / 01-2023




                 82                                                                          A+W Production Terminal
                 Tutorial                                                  Überblick A+W Production Terminal Processing




                                           Bereich L - SN Ansicht
                                           Mit dieser Kombobox haben Sie die Möglichkeit, sich die unterschiedlichen
                                           SN Ansichten anzeigen zu lassen. Nachdem Sie die gewünschte Ansicht aus-
                                           gewählt haben, wird die Anzeige aktualisiert.
                                           Über die Schaltfläche [SN Druck] können Sie die Grafik drucken.

                                           Bereich M - Liste der Bearbeitungen
                                           In diesem Bereich wird die Liste der Bearbeitungsschritte eingeblendet, die
                                           die im Dialog angezeigte Auftragsposition bereits durchlaufen hat oder noch
                                           durchlaufen muss. Ein grünes Häkchen markiert die erfolgreich durchgeführ-
                                           ten Arbeiten, ein fehlendes Häkchen kennzeichnet die noch auszuführenden
                                           Arbeiten.


                                           Ergänzende Informationen
                                            Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19
1.50 / 01-2023




                 A+W Production Terminal                                                                            83
                 Überblick A+W Production Terminal Processing                                                 Tutorial




                                        Ablauf von Arbeitsschritten
                                        Die Vorgehensweise zum Arbeiten in Terminal Processing ist:
                                        •   Starten Sie das Modul Terminal Processing.
                                        •   Melden Sie sich an (<Name>).
                                        •   Scannen Sie ein Etikett oder geben Sie die Etikettnummer ein.
                                        •   Wählen Sie die Erfassungsstelle aus.
                                        •   Wählen Sie den entsprechenden Treiber aus (falls er nicht zugeordnet ist).
                                        •   Erzeugen Sie den Maschinencode.
                                        •   Buchen Sie die Etikettnummer.
                                        •   Laden Sie ein weiteres Etikett.
                                        Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                        protokollieren. Gründe für eine Unterbrechung können sein:
                                        •   Wartung der Maschine.
                                        •   Störung der Maschine.
                                        •   Pausenzeiten.
                                        Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                        weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                        Mängel können sein:
                                        •   Bruch
                                        •   Kratzer
                                        •   Riss

                                        Anmelden an der Arbeitsstation
                                        Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                        Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                         Tutorial, “So melden Sie sich an” auf Seite 24


                                         So scannen Sie ein Etikett
                                        1 Geben Sie im Feld Etikett die gewünschte Etikettnummer ein oder scannen
                                          Sie das Etikett.
                                        2 Die Daten werden geladen.

                                            Weitere Scheiben laden
                                            Zum Laden einer weiteren Scheibe öffnen Sie im Menü Extras den Menü-
                                            punkt Barcode. Es öffnet sich der Dialog Manuelle Eingabe. Geben Sie im
                                            Feld Barcode die gewünschte Etikettnummer ein oder scannen Sie den
                                            Barcode und betätigen Sie die Schaltfläche [OK]. Die geladene Scheibe
                                            wird in der Übersicht am Ende der Tabelle angezeigt.
1.50 / 01-2023




                 84                                                                        A+W Production Terminal
                 Tutorial                                                Überblick A+W Production Terminal Processing




                                            So melden Sie eine Erfassungsstelle an
                                           1 Scannen Sie den entsprechenden Barcode oder öffnen Sie die Kombobox
                                             Erf.-Stelle.
                                           2 Wählen Sie die gewünschte Erfassungsstelle aus. Die der Erfassungsstel-
                                             le zugeordneten Bearbeitungstypen werden im Bereich Bearbeitungen an-
                                             gezeigt. Arbeiten Sie mit einem Scanner, ist dieser Schritt nicht notwendig,
                                             die Daten werden nach dem Scannen der Erfassungsstelle automatisch
                                             geladen.


                                            So melden Sie ein Gestell an
                                           1 Geben Sie die Gestellnummer des physikalischen Gestells ein oder scan-
                                             nen Sie den Barcode.
                                           2 Haben Sie ein leeres Gestell, aktivieren Sie nach der Anmeldung des Ge-
                                             stells die Checkbox Gestell leeren. Arbeiten Sie mit einem Scanner, kön-
                                             nen Sie auch den Barcode Beginn scannen.


                                            So erzeugen Sie Maschinencode
                                           1 Geben Sie die Etikettnummer ein, für die der Maschinencode erzeugt wer-
                                             den soll.
                                           2 Geben Sie die Gestell-Nummer ein (optional).
                                           3 Haben Sie ein leeres Gestell, aktivieren Sie nach der Anmeldung des Ge-
                                             stells die Checkbox Gestell leeren. Arbeiten Sie mit einem Scanner, kön-
                                             nen Sie auch den Barcode Beginn scannen.
                                           4 Wählen Sie die gewünschte Erfassungsstelle aus.
                                           5 Falls der Treiber nicht automatisch geladen wird, können Sie ihn über die
                                             Kombobox Code auswählen.
                                           6 Betätigen Sie die Schaltfläche [Code].
                                           7 Der Treiber wird aufgerufen und der Maschinencode wird erzeugt. Die
                                             Scheibe wird auf den Erfassungsstellen-Eingang gebucht.
1.50 / 01-2023




                 A+W Production Terminal                                                                             85
                 Überblick A+W Production Terminal Processing                                                   Tutorial




                                         So produzieren Sie eine Scheibe
                                        1 Geben Sie die Gestell-Nummer ein (optional).
                                        2 Haben Sie ein leeres Gestell, aktivieren Sie nach der Anmeldung des Ge-
                                          stells die Checkbox Gestell leeren. Arbeiten Sie mit einem Scanner, kön-
                                          nen Sie auch den Barcode Beginn scannen.
                                        3 Geben Sie die Charge ein (optional).
                                        4 Wählen Sie die gewünschte Erfassungsstelle aus.
                                        5 Falls der Treiber nicht automatisch geladen wird, können Sie ihn über die
                                          Kombobox Code auswählen.
                                        6 Betätigen Sie die Schaltfläche [Code].
                                        7 Der Treiber wird aufgerufen und der Maschinencode wird erzeugt. Die
                                          Scheibe wird auf den Erfassungsstellen-Eingang gebucht.
                                        8 Führen Sie die Bearbeitung durch.
                                        9 Anschließend betätigen Sie die Schaltfläche [Produzieren [F5]].
                                        10 Die Scheibe wird auf das entsprechende Gestell und den Erfassungsstel-
                                           len-Ausgang gebucht. Die zeitliche Differenz zwischen dem Erfassungs-
                                           stellen-Eingang und -Ausgang ist dann die Dauer der Bearbeitung.

                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                        befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                        Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                        Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                        In ausführlich beschrieben.
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28
1.50 / 01-2023




                 86                                                                            A+W Production Terminal
                 Tutorial                                                  Überblick A+W Production Terminal Processing




                                           Weitere Funktionen
                                           Zu den weiteren Funktionen zählen:
                                           •   Listen (Reports)
                                           •   Log-Einträge
                                           •   Unterschiedliche Programm-Sprachen
                                           Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den
                                           Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                           schrieben.


                                           Ergänzende Informationen
                                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                                            Tutorial, “Log-Einträge exportieren” auf Seite 31
                                            Tutorial, “Programmsprache wählen” auf Seite 32
                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
1.50 / 01-2023




                 A+W Production Terminal                                                                            87
                 Überblick A+W Production Terminal TG                                                   Tutorial




                                        Überblick A+W Production
                                        Terminal TG
                                        In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                        dem A+W Production Terminal TG (Terminal TG) kennen.
                                        Der Themenblock beinhaltet folgende Schulungseinheiten:
                                        •   Arbeiten mit Terminal TG-In
                                        •   Ablauf von Arbeitsschritten
                                        •   Weitere Funktionen
1.50 / 01-2023




                 88                                                                    A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal TG




                                           Arbeiten mit Terminal TG-In
                                           Lernziele

                                           •   Oberfläche von Terminal TG-In kennenlernen.
                                           •   Die Funktionsweise kennenlernen und verstehen.
                                           •   Ofenbetten befüllen.
                                           •   Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                           Nutzen

                                           Terminal TG-In unterstützt Sie am Ofeneingang durch die grafische Darstellung der
                                           Ofenbettbelegung. Das führt zu einer optimalen Auslastung der Öfen und spart Geld.


                                           Definitionen

                                           Rotieren                    Drehen von Scheiben.


                                           Merke

                                           Bedienung über Scanner      Terminal TG-In wird überwiegend mit dem Scanner
                                                                       bedient. Zur Bedienung mit einer Maus finden Sie die
                                                                       Hinweise an den entsprechenden Stellen.

                                           Ofenbetten                  Es stehen 15 Ofenbetten zur Verfügung, die nummeriert
                                                                       sind. Beispiel: 01 ist das erste Ofenbett, 08 das Achte.

                                           <F11>                       Haben Sie nicht zwei Monitore zur Verfügung, können
                                                                       Sie mit <F11> von der einen in die andere Ansicht
                                                                       wechseln (Hauptfenster/Ofenbett).

                                           Warnfenster                 Das Warnfenster erscheint automatisch, wenn es vor
                                                                       dem Härten noch offenen Bearbeitungen gibt.

                                           Scheiben drehen und         Scheiben können auf dem Ofenbett auch mit der Maus
                                           verschieben                 gedreht und in die nächste Zeile verschoben werden.
1.50 / 01-2023




                 A+W Production Terminal                                                                                      89
                 Überblick A+W Production Terminal TG                                                                Tutorial




                                              Modul-Präsentation Terminal TG-In
                                              Terminal TG-In ist ein Leitrechner, der am Eingang des ESG-Ofens zum Ein-
                                              satz kommt. Mit seiner Hilfe werden am Ofeneingang alle Scheiben erfasst,
                                              die in den Durchlauf- oder Chargenofen eingebracht werden. Produktionsun-
                                              terstützende Informationen zu den gewählten Scheiben werden angezeigt.
                                              Dazu zählen z. B. grafische Darstellungen mit Form und Maße der Scheiben
                                              sowie Auftrags- und Kundeninformationen.
                                              Terminal TG-In besteht aus zwei Dialogen: Dem Terminal TG-In (Hauptfens-
                                              ter) und dem Ofenbett. Die beiden Dialoge sind für einen Zwei-Monitor-Betrieb
                                              ausgelegt. Verfügen Sie nicht über zwei Monitore, können Sie mit <F11> zwi-
                                              schen den beiden Dialogen wechseln.
                                              Nachdem Sie Terminal TG-In gestartet haben, präsentiert sich das Modul wie
                                              folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn
                                              Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B




                 C                                                                                                      H
                                                                                                                        I
                 D


                 E
                 F

                 G                                                                                                      J



                 A    Menüleiste                             E   Etikettendruck          I   Modellvorschau SN
                 B    Liste in Beladereihenfolge             F   Infofelder              J   Schaltflächen
                 C    Bettbezeichnung                        G   Meldungsfenster
                 D    Verlinkte Dokumente                    H   Modellanzeige
                 Abb. 17        Terminal TG-In


                                              Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                              runter finden Sie die Liste in Beladereihenfolge (B). Im Bereich (C) finden Sie
1.50 / 01-2023




                                              die Informationen zum Ofenbett und in (D) die verlinkten Dokumente. Der Be-
                                              reich (E) steuert den Etikettendruck. Im Bereich (F) befinden sich die Infofel-
                                              der. Unter (G) befindet sich das Meldungsfenster. Unter (H) finden Sie die


                 90                                                                               A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal TG




                                           Modellanzeige und unter (I) die Modellvorschau. Die Schaltflächen befinden
                                           sich im Bereich (J).

                                              Anzeige der Spalten ist frei konfigurierbar
                                              Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                              schirmdarstellung von Ihrer Darstellung abweichen.

                                           Detaillierte Erläuterung zu den einzelnen Bereichen
                                           Die Bereiche (A), (D), (F), (G), (H) und (J) von Terminal TG-In sind identisch
                                           sind mit den Bereichen von Terminal IG-In und werden an dieser Stelle nicht
                                           noch einmal beschrieben.
                                            Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19

                                              Neue Charge eingeben
                                              Das Terminal IG-I kann so konfiguriert werden, dass automatisch eine
                                              neue Chargenbezeichnung vorgeschlagen wird, wenn sich zum Beispiel
                                              die Glasdicke oder eine beliebige andere Eigenschaft der aufgelegten
                                              Scheiben ändert. Zusätzlich kann eine Zeitspanne konfiguriert werden,
                                              nach deren Ablauf auch bei gleicher Eigenschaft eine neue Chargenbe-
                                              zeichnung vorgeschlagen wird.

                                           Das Feld (I) von Terminal TG-In ist identisch mit dem Feld von Terminal Order
                                           und wird an dieser Stelle nicht noch einmal beschrieben. In Terminal TG-In
                                           dient die Modellvorschau zur Anzeige der ESG-Stempel-Position.
                                            Tutorial, “Modul-Präsentation Terminal Order” auf Seite 71

                                           Bereich B - Liste in Beladereihenfolge
                                           Die Liste zeigt Ihnen die Beladung des Ofenbettes in der Reihenfolge, wie Sie
                                           die Scheiben gescannt haben.
                                           Im Feld Etikett wird Ihnen die Etikettnummer der Scheibe angezeigt. Dahinter
                                           sehen Sie im Feld Auftrag die Auftragsnummer und im Feld Pos die entspre-
                                           chende Positionsnummer. Die Felder Breite, Höhe und Dicke zeigen Ihnen die
                                           Abmessungen der Scheibe. Im Feld Glasart sehen Sie die Glasbezeichnung
                                           und im Feld Produkt das fertige Produkt.

                                           Bereich C - Bettbezeichnung




                                           Im diesem Bereich wird Ihnen die Bettbezeichnung angezeigt.
                                           O1 bedeutet, dass es sich um den Ofen 1 handelt. 04 bedeutet, dass es sich
                                           um das vierte Ofenbett handelt.
1.50 / 01-2023




                 A+W Production Terminal                                                                               91
                 Überblick A+W Production Terminal TG                                                        Tutorial




                                        Bereich E - Etikettendruck




                                        Zum Drucken von Etiketten aktivieren Sie die Checkbox Etiketten an und wäh-
                                        len aus der dahinter liegenden Kombobox den entsprechenden Drucker aus.
                                        Es wird dann für jede Scheibe auf dem Ofenbett in Beladereihenfolge ein Eti-
                                        kett gedruckt.




                                        Abb. 18     Ofenbett Terminal TG-In


                                        Das Ofenbett wird in der Originalgröße dargestellt. Die entsprechenden Ein-
                                        stellungen werden im Programm hinterlegt. Die Scheiben werden so platziert,
                                        dass sowohl zum Rand hin als auch zwischen den einzelnen Scheiben ein ge-
                                        wisser Zwischenraum bleibt.
                                        Das Ofenbett wird immer von links nach rechts beladen. Ist eine Reihe voll,
                                        wird die Nächste angefangen.

                                        Scheiben auf dem Ofenbett verschieben oder drehen
                                        Es kann unter Umständen vorkommen, dass Sie Scheiben auf dem Ofenbett
                                        verschieben oder drehen müssen. Dazu markieren Sie die Scheibe und scan-
                                        nen den Barcode Zeilenumbruch, wenn die markierte Scheibe in die nächste
                                        Zeile geschoben werden soll. Möchten Sie die Scheibe drehen, scannen Sie
                                        den Barcode Rotieren. Dann wird die Scheibe bei jedem Scannen um 90° im
                                        Uhrzeigersinn gedreht. Arbeiten Sie mit einer Maus (anstelle eines Scanners)
                                        markieren Sie die Scheibe, drücken die linke Maustaste und halten Sie diese
1.50 / 01-2023




                                        gedrückt. Dann verschieben Sie die Scheibe an die gewünschte Stelle und
                                        lassen die linke Maustaste los. Zum Drehen der Scheibe betätigen Sie die
                                        rechte Maustaste. Pro Tastenklick wird die Scheibe um 90° Grad gedreht.


                 92                                                                       A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal TG




                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal TG-In ist:
                                           •   Starten Sie das Modul Terminal TG-In.
                                           •   Melden Sie sich an (<Name>).
                                           •   Scannen Sie ein Etikett oder geben Sie die Etikettnummer ein.
                                           •   Füllen Sie das Ofenbett.
                                           •   Drucken Sie die Etiketten.
                                           •   Produzieren Sie das Ofenbett.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                           weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                           Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So scannen Sie ein Etikett
                                           1 Scannen Sie im Hauptfenster das gewünschte Etikett.
                                           2 Die entsprechenden Daten werden geladen und in der Tabelle angezeigt.

                                               Arbeiten ohne Scanner
                                               Arbeiten Sie ohne Scanner, öffnen Sie im Menü Extras den Menüpunkt
                                               Barcode. Es öffnet sich der Dialog Manuelle Eingabe. Geben Sie im Feld
                                               Barcode die gewünschte Etikettnummer ein und betätigen Sie die Schalt-
                                               fläche [OK]. Die geladene Scheibe wird in der Übersicht angezeigt.


                                            So verfahren Sie mit offenen Bearbeitungen
                                           1 Scannen Sie im Hauptfenster das gewünschte Etikett.
                                           2 Der Dialog Offene Bearbeitungen öffnet sich automatisch.
                                           3 Prüfen Sie, ob die Bearbeitung wirklich fehlt oder ob sie nur vergessen wur-
                                             de zu buchen.
1.50 / 01-2023




                                           4 Fehlt die Bearbeitung, betätigen Sie die Schaltfläche [Schließen]. Der Dia-
                                             log wird geschlossen. Die Scheibe muss noch bearbeitet werden.



                 A+W Production Terminal                                                                             93
                 Überblick A+W Production Terminal TG                                                        Tutorial




                                        5 Wurde die Bearbeitung gemacht, betätigen Sie die Schaltfläche [Trotzdem
                                          laden]. Der Dialog wird geschlossen. Die Daten werden geladen.


                                         So verschieben Sie eine Scheibe auf dem Ofenbett
                                           Möchten Sie eine bereits platzierte Scheibe lieber in der nächsten Reihe
                                           haben, können Sie die Scheibe manuell verschieben.
                                        1 Markieren Sie die Scheibe, die verschoben werden soll.
                                        2 Scannen Sie den Barcode Zeilenumbruch.
                                        3 Die Scheibe wird in die nächste Zeile verschoben.

                                           Arbeiten ohne Scanner
                                           Arbeiten Sie ohne Scanner, markieren Sie die Scheibe, betätigen die linke
                                           Maustaste und halten Sie diese gedrückt. Verschieben Sie die Scheibe an
                                           die gewünschte Position und lassen Sie die Maustaste los.


                                         So drehen Sie eine Scheibe auf dem Ofenbett
                                           Möchten Sie eine bereits platzierte Scheibe drehen, können Sie dies eben-
                                           falls manuell tun.
                                        1 Markieren Sie die Scheibe, die gedreht werden soll.
                                        2 Scannen Sie den Barcode Rotieren.
                                        3 Mit jedem Scannen wird die Scheibe um 90° im Uhrzeigersinn gedreht.
                                        4 Wiederholen Sie den Vorgang so oft, bis sich die Scheibe in der gewünsch-
                                          ten Position befindet.

                                           Arbeiten ohne Scanner
                                           Arbeiten Sie ohne Scanner, markieren Sie die Scheibe und betätigen die
                                           rechte Maustaste. Pro Tastenklick wird die Scheibe um 90° gedreht.


                                         So produzieren Sie das Ofenbett
                                        1 Füllen Sie das Ofenbett.
                                        2 Scannen Sie den Barcode Bett produzieren.
                                        3 Die Scheibe wird auf den Erfassungsstellen-Ausgang gebucht. Die zeitli-
                                          che Differenz zwischen dem Erfassungsstellen-Eingang und -Ausgang ist
                                          dann die Dauer der Bearbeitung.
                                        4 Falls nötig, drucken Sie die entsprechenden Etiketten.
                                        5 Das nächste freie Ofenbett wird automatisch geladen (Feld Bett).
1.50 / 01-2023




                 94                                                                       A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal TG




                                           Chargen erfassen
                                           Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                           schrieben.
                                            Tutorial, “So definieren Sie Chargen” auf Seite 37

                                           Den Zustand der Maschine ändern
                                           Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                           terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                           Maschine oder auch Pausenzeiten.
                                           Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                           ausführlich beschrieben.
                                            Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                           Umgang mit beschädigten Scheiben
                                           Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                           befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                           Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                           Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                           In ausführlich beschrieben.
                                            Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28


                                           Weitere Funktionen
                                           Zu den weiteren Funktionen zählen:
                                           •   Listen (Reports)
                                           •   Log-Einträge
                                           •   Unterschiedliche Programm-Sprachen
                                           Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den
                                           Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                           schrieben.


                                           Ergänzende Informationen
                                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                                            Tutorial, “Log-Einträge exportieren” auf Seite 31
                                            Tutorial, “Programmsprache wählen” auf Seite 32
                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
1.50 / 01-2023




                 A+W Production Terminal                                                                             95
                 Überblick A+W Production Terminal TG-Out                                               Tutorial




                                        Überblick A+W Production
                                        Terminal TG-Out
                                        In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                        dem A+W Production Terminal TG-Out (Terminal TG-Out) kennen.
                                        Der Themenblock beinhaltet folgende Schulungseinheiten:
                                        •   Arbeiten mit Terminal TG-Out
                                        •   Ablauf von Arbeitsschritten
                                        •   Ablauf von Arbeitsschritten
                                        •   Weitere Funktionen
1.50 / 01-2023




                 96                                                                    A+W Production Terminal
                 Tutorial                                                       Überblick A+W Production Terminal TG-Out




                                           Arbeiten mit Terminal TG-Out
                                           Lernziele

                                           •   Oberfläche von Terminal TG-Out kennenlernen.
                                           •   Die Funktionsweise kennenlernen und verstehen.
                                           •   Ofenbetten abräumen.
                                           •   Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                           Nutzen

                                           Durch die Anzeige der Packmittelgruppen stellen Sie die Scheiben gleich auf die
                                           entsprechenden Gestelle für den weiteren Produktionsprozess. Das erspart Ihnen ein
                                           Umsortieren und somit Zeit.


                                           Definitionen

                                           Muster                      Grafische Darstellung des Ofenbettes.

                                           Fehlergestell               Scheiben, die nicht gebucht wurden, landen
                                                                       automatisch auf sog. Fehlergestellen.


                                           Merke

                                           Lücken auf dem Ofenbett     Haben Sie eine Scheibe gescannt, verschwindet diese
                                                                       vom Ofenbett und es entsteht eine Lücke.

                                           Mehrere Scanner             In Terminal TG-Out können Sie mit bis zu drei Scannern
                                           verwenden                   arbeiten.

                                           Bett produzieren            Über diese Schaltfläche haben Sie die Möglichkeit, das
                                                                       komplette Ofenbett auf einmal zu buchen.

                                           Packmittelgruppe            Packmittelgruppen werden auch hier mit
                                                                       unterschiedlichen Farben dargestellt.
1.50 / 01-2023




                 A+W Production Terminal                                                                                   97
                 Überblick A+W Production Terminal TG-Out                                                            Tutorial




                                            Modul-Präsentation Terminal TG-Out
                                            Terminal TG-Out ist ein Leitrechner, der am Ausgang des ESG-Ofens zum
                                            Einsatz kommt. Terminal TG-Out besteht aus zwei Dialogen: Dem Terminal
                                            TG-Out (Hauptfenster) und dem Ofenbett. Die beiden Dialoge sind für einen
                                            Zwei-Monitor-Betrieb ausgelegt. Verfügen Sie nicht über zwei Monitore, kön-
                                            nen Sie mit <F11> zwischen den beiden Dialogen wechseln.
                                            Nachdem Sie Terminal TG-Out gestartet haben, präsentiert sich das Modul
                                            wie folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten.
                                            Wenn Sie das Modul starten, ist das Hauptfenster leer:


                 A
                 B




                 C                                                                                                      H
                 D
                 E                                                                                                      I

                 F

                 G


                 A Menüleiste                               D Gestellnummer              G Schaltflächen
                 B Liste in Abladereihenfolge               E Meldungsfenster            H Verlinkte Dokumente
                 C Bettbezeichnung                          F Infofelder                 I Modellanzeige SN
                 Abb. 19      Terminal TG-Out


                                            Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                            runter finden Sie die Liste in Abladereihenfolge (B). Im Bereich (C) finden Sie
                                            die Informationen zum Ofenbett und in (D) die Gestellnummer. Der Bereich (E)
                                            beinhaltet das Meldungsfenster. Im Bereich (F) befinden sich die Infofelder.
                                            Unter (G) befinden sich die Schaltflächen. Unter (H) finden Sie die verlinkten
                                            Dokumente und unter (I) die Modellanzeige.

                                                Anzeige der Spalten ist frei konfigurierbar
1.50 / 01-2023




                                                Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                                schirmdarstellung von Ihrer Darstellung abweichen.



                 98                                                                              A+W Production Terminal
                 Tutorial                                                       Überblick A+W Production Terminal TG-Out




                                           Detaillierte Erläuterung zu den einzelnen Bereichen
                                           Die Bereiche (A), (D), (E), (F), (H) und (I) von Terminal TG-In sind identisch
                                           sind mit den Bereichen von Terminal IG-In und werden an dieser Stelle nicht
                                           noch einmal beschrieben.
                                            Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19
                                           Das Feld (C) von Terminal TG-Out ist identisch mit dem Feld von Terminal TG-
                                           In und wird an dieser Stelle nicht noch einmal beschrieben.
                                            Tutorial, “Bereich C - Bettbezeichnung” auf Seite 91

                                           Bereich B - Liste in Abladereihenfolge
                                           Die Liste zeigt Ihnen die Abladung des Ofenbettes in der Reihenfolge, wie die
                                           Scheiben durch den Ofen kommen.
                                           Im Feld Etikett wird Ihnen die Etikettnummer der Scheibe angezeigt. Dahinter
                                           sehen Sie im Feld Auftrag die Auftragsnummer und im Feld Pos die entspre-
                                           chende Positionsnummer. Die Felder Breite, Höhe und Dicke zeigen Ihnen die
                                           Abmessungen der Scheibe. Im Feld Glasart sehen Sie die Glasbezeichnung
                                           und im Feld Modell die Modellnummer. Im Bereich Nächste ES sehen Sie,
                                           welche Station als nächstes ansteht.
                                           Die farbliche Unterlegung des Feldes kennzeichnet die jeweilige Packmittel-
                                           gruppe. Scheiben aus dieser Liste, die die gleiche Farbe haben wie das Feld
                                           Gestellnummer, gehöhren auf ein Gestell. Ein Wechsel der Farbe bedeutet
                                           gleichzeitig Wechsel des Gestells.

                                              Farbe der Packmittelgruppe auch auf Ofenbett
                                              Der farbliche Rahmen der Scheibe auf dem Ofenbett kennzeichnet eben-
                                              falls die jeweilige Packmittelgruppe.

                                           Bereich G - Schaltflächen
                                           Die Schaltflächen [Produzieren], [Abbrechen] und [Bruch] sind identisch sind
                                           mit den Schaltflächen von Terminal IG-In und werden an dieser Stelle nicht
                                           noch einmal beschrieben.
                                            Tutorial, “Bereich H - Schaltflächen” auf Seite 23
                                           Möchten Sie das komplette Ofenbett auf einmal buchen, betätigen Sie die
                                           Schaltfläche [Bett produzieren].
1.50 / 01-2023




                 A+W Production Terminal                                                                              99
                 Überblick A+W Production Terminal TG-Out                                                      Tutorial




                                        Abb. 20      Ofenbett Terminal TG-Out


                                        Das Ofenbett wird in der Originalgröße dargestellt. Die entsprechenden Ein-
                                        stellungen werden im Programm hinterlegt. Die Anordnung der Scheiben ist
                                        so, wie sie am Terminal TG-In auf das Ofenbett gelegt wurden.
                                        Am unteren, linken Bildschirmrand sehen Sie die Bettbezeichnung (O107). O1
                                        bedeutet, dass es sich um den Ofen 1 handelt. 07 bedeutet, dass es sich um
                                        das siebente Ofenbett handelt.
                                        Daneben befinden sich die Felder für die unterschiedlichen Scanner. Terminal
                                        TG-Out können Sie mit bis zu drei Scannern bedienen, d. h., es können bis zu
                                        drei Mitarbeiter am Ofenausgang die Scheiben vom Ofenbett nehmen und auf
                                        die entsprechenden Gestelle verteilen.
                                        Im ersten Schritt scannen Sie die Gestellnummer, auf die die Scheibe gestellt
                                        wird. Dann nehmen Sie die Scheibe vom Bett und scannen sie.
                                        Haben Sie eine Scheibe gescannt, verschwindet die Scheibe vom Ofenbett,
                                        das eigentliche Muster bleibt jedoch erhalten. D. h., die Lücken, die durch das
                                        Scannen der Scheiben entstehen bleiben, die Scheiben werden nicht zusam-
                                        mengerückt.
1.50 / 01-2023




                 100                                                                        A+W Production Terminal
                 Tutorial                                                      Überblick A+W Production Terminal TG-Out




                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal TG-Out ist:
                                           •   Starten Sie das Modul Terminal TG-Out.
                                           •   Melden Sie sich an (<Name>).
                                           •   Melden Sie ein Gestell an.
                                           •   Nehmen Sie die Scheibe vom Ofenbett und stellen Sie sie auf das Gestell.
                                           •   Buchen Sie die Scheibe.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                           weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                           Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So arbeiten Sie mit mehreren Personen, um das Ofenbett zu leeren
                                               Am Ofenausgang haben Sie die Möglichkeit, mit bis zu drei Scannern zu
                                               arbeiten.
                                           1 Scannen Sie die Gestellnummer, auf die die Scheibe gestellt werden soll.
                                           2 Scannen Sie Ihren Namen.
                                           3 Stellen Sie die Scheibe auf das Gestell.
                                           4 Buchen Sie die Scheibe.


                                            So buchen Sie das gesamte Ofenbett
                                               Unter Umständen kann es vorkommen, dass Sie das gesamte Ofenbett auf
                                               einmal buchen müssen. Das ist z. B. der Fall, wenn Sie mehr Mitarbeiter
                                               zum Abräumen des Ofenbettes benötigen, als Ihnen zur Verfügung stehen.
                                           5 Betätigen Sie die Schaltfläche [Bett produzieren]. Das gesamte Bett wird
                                             herausgefahren.
                                           6 Räumen Sie das Ofenbett ab.
1.50 / 01-2023




                                           7 Buchen Sie die Scheiben (wenn Sie die Zeit dafür haben).




                 A+W Production Terminal                                                                          101
                 Überblick A+W Production Terminal TG-Out                                                       Tutorial




                                            Gesamtes Ofenbett buchen
                                            In der Praxis wird diese Schaltfläche überwiegend dann verwendet, wenn
                                            das Abräumen so schnell gehen muss, dass es mit dem zur Verfügung ste-
                                            henden Personal nicht machbar ist. Damit die Scheiben nicht auf Fehler-
                                            gestellen landen, können sie mit einem Klick gebucht werden. Bitte
                                            beachten Sie, dass in diesem Fall keine Gestellzuweisung stattfindet.

                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37

                                        Den Zustand der Maschine ändern
                                        Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                        terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                        Maschine oder auch Pausenzeiten.
                                        Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                        ausführlich beschrieben.
                                         Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                        befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                        Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                        Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                        In ausführlich beschrieben.
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28


                                        Weitere Funktionen
                                        Zu den weiteren Funktionen zählen:
                                        •   Listen (Reports)
                                        •   Log-Einträge
                                        •   Unterschiedliche Programm-Sprachen
                                        Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den
                                        Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                        schrieben.


                                        Ergänzende Informationen
                                         Tutorial, “Listen (Reports) generieren” auf Seite 31
                                         Tutorial, “Log-Einträge exportieren” auf Seite 31
                                         Tutorial, “Programmsprache wählen” auf Seite 32
1.50 / 01-2023




                                         Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174




                 102                                                                           A+W Production Terminal
                 Tutorial                                                      Überblick A+W Production Terminal LG




                                           Überblick A+W Production
                                           Terminal LG
                                           In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                           dem A+W Production Terminal LG (Terminal LG) kennen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Arbeiten mit Terminal LG-In
                                           •   Arbeiten mit Terminal LG-Assembly
1.50 / 01-2023




                 A+W Production Terminal                                                                      103
                 Überblick A+W Production Terminal LG                                                                Tutorial




                                        Arbeiten mit Terminal LG-In
                                        Lernziele

                                        • Oberfläche von Terminal LG-In kennenlernen.
                                        • Die Funktionsweise kennenlernen und verstehen.
                                        • Mit unvorhersehbaren Situation (z. B. Bruch) umgehen lernen.


                                        Nutzen

                                        Terminal LG-In unterstützt Sie am Linieneingang durch die grafische Darstellung des
                                        Scheibenaufbaus inklusive der Folien. Was an diesem Terminal gebucht wird, wird
                                        sofort im Terminal LG-Assembly angezeigt.


                                        Definitionen

                                        Wenden                      Mit Hilfe dieser Checkbox wird der Scheibenaufbau
                                                                    umgekehrt und auch so im Reinraum angezeigt.


                                        Merke

                                        VSG produzieren             Mit dieser Schaltfläche produzieren Sie die Einheit.

                                        Produzieren                 Mit dieser Schaltfläche laden Sie die Scheibe.

                                        Laden                       Diese Schaltfläche greift auf die zuletzt angewandte
                                                                    Methode zurück - Auftrag oder Los laden.
1.50 / 01-2023




                 104                                                                            A+W Production Terminal
                 Tutorial                                                         Überblick A+W Production Terminal LG




                                           Modul-Präsentation Terminal LG-In
                                           Terminal LG-In ist ein Leitrechner, der am Eingang der VSG-Linie zum Einsatz
                                           kommt. Mit seiner Hilfe werden alle Scheiben erfasst, die in die Linie einge-
                                           bracht werden. Produktionsunterstützende Informationen zu den gewählten
                                           Scheiben werden angezeigt.
                                           Dazu zählen z. B. grafische Darstellungen mit Form und Maße der Scheiben,
                                           Folien sowie Auftrags- und Kundeninformationen.
                                           Nachdem Sie Terminal LG-In gestartet haben, präsentiert sich das Modul wie
                                           folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn
                                           Sie das Modul starten, ist das Hauptfenster leer:



                 A
                 B
                                                                                                                       G
                 C




                                                                                                                       H

                 D




                 E                                                                                                     I
                                                                                                                       J
                 F
                                                                                                                       K



                 A   Menüleiste                           E   Verlinkte Dokumente       I Modellvorschau SN
                 B   Produktionsnummer mit Bezeichnung    F   Infofelder                J Checkbox zum Wenden
                 C   Liste der aktuellen Einheit          G   Modellanzeige             K Schaltflächen
                 D   Vorschauliste                        H   Farbliche Darstellung der
                                                              Einheit
                 Abb. 21      Terminal LG-In


                                           Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                           runter finden Sie die aktuelle Produktionsnummer sowie die Bezeichnung (B).
                                           Im Bereich (C) finden Sie die Liste der aktuellen Einheit und in (D) die Vor-
                                           schau auf die nächsten Einheiten. Unter (E) finden Sie die verlinkten Doku-
1.50 / 01-2023




                                           mente. Im Bereich (F) befinden sich die Infofelder. Im Bereich (G) wird Ihnen
                                           das Modell und die umschreibenden Maße der Scheibe angezeigt. Unter (H)
                                           finden Sie die farbliche Darstellung der zu produzierenden Einheit, unter (I) die



                 A+W Production Terminal                                                                               105
                 Überblick A+W Production Terminal LG                                                           Tutorial




                                        Modellvorschau SN und unter (J) die Checkbox zum Wenden des Aufbaus.
                                        Die Schaltflächen befinden sich im Bereich (K).

                                           Anzeige der Spalten ist frei konfigurierbar
                                           Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                           schirmdarstellung von Ihrer Darstellung abweichen.

                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Die Bereiche (A), (B), (C), (D), (F), (G) und (H) von Terminal LG-In sind iden-
                                        tisch sind mit den Bereichen von Terminal IG-In und werden an dieser Stelle
                                        nicht noch einmal beschrieben.
                                         Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19
                                        Das Feld (E) von Terminal LG-In ist identisch mit dem Feld von Terminal Pro-
                                        cessing und wird an dieser Stelle nicht noch einmal beschrieben.
                                         Tutorial, “Modul-Präsentation Terminal Processing” auf Seite 80
                                        Das Feld (I) von Terminal LG-In ist identisch mit dem Feld von Terminal Pro-
                                        cessing und wird an dieser Stelle nicht noch einmal beschrieben.
                                         Tutorial, “Modul-Präsentation Terminal TG-In” auf Seite 90

                                        Bereich J - Checkbox Wenden
                                        Diese Checkbox dient dem manuellen Wenden der Einheit.




                                        A Aufbau ohne Wenden                      B Aufbau mit Wenden


                                           Arbeiten mit Scannern
                                           Arbeiten Sie mit einem Scanner, ist das manuelle Wenden der Enheit nicht
                                           nötig, da der Scheibenaufbau anhand der Etikettnummer erkannt wird.
1.50 / 01-2023




                 106                                                                           A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal LG




                                           Bereich K - Schaltflächen
                                           Die Schaltfläche Laden [F2] steht in Zusammenhang mit den Menüeinträgen
                                           Auftrag laden und Lauf laden. Sie greift auf die zuletzt verwendete Methode
                                           zurück. Das bedeutet, haben Sie über das Menü einen Auftrag geladen, öffnet
                                           sich der Dialog Auftrag laden, wenn Sie das nächste Mal die Schaltfläche La-
                                           den [F2] betätigen. Haben Sie zuletzt einen Lauf über das Menü geladen, öff-
                                           net sich der Dialog Los laden, wenn Sie das nächste Mal die Schaltfläche
                                           Laden [F2] betätigen. Damit weisen Sie der Schaltfläche quasi die Funktion für
                                           das Arbeiten zu: Auftrag laden oder Los laden.
                                           Über die Schaltfläche [VSG produzieren] produzieren Sie die komplette Ein-
                                           heit. Die Einheit verschwindet aus der Anzeige und die nächste Einheit wird
                                           angezeigt.
                                           Betätigen Sie die Schaltfläche Produzieren [F5], wird die einzelne Scheibe
                                           produziert. In der Liste hat die Scheibe anschließend einen grünen Haken.


                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal LG-In ist:
                                           •   Starten Sie das Modul Terminal LG-In.
                                           •   Melden Sie sich an (<Name>).
                                           •   Scannen Sie ein Etikett ein oder laden Sie einen Auftrag oder einen Lauf.
                                           •   Produzieren Sie die Scheibe bzw. die Einheit.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                           weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                           Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24
1.50 / 01-2023




                 A+W Production Terminal                                                                            107
                 Überblick A+W Production Terminal LG                                                           Tutorial




                                         So scannen Sie ein Etikett
                                        1 Scannen Sie im Hauptfenster das gewünschte Etikett.
                                        2 Die entsprechenden Daten werden geladen und in der Tabelle angezeigt.

                                           Arbeiten ohne Scanner
                                           Arbeiten Sie ohne Scanner, öffnen Sie im Menü Datei den Menüpunkt Auf-
                                           trag laden oder Lauf laden. Es öffnet sich der Dialog Auftrag laden/Los la-
                                           den. Wählen Sie aus der Liste den gewünschten Auftrag bzw. den
                                           gewünschten Lauf aus und betätigen Sie die Schaltfläche Laden [F5]. Die
                                           geladene Scheibe wird in der Übersicht angezeigt.


                                         So laden Sie einen Auftrag
                                        1 Wählen Sie im Menü Datei den Menüpunkt Auftrag laden.
                                        2 Der Dialog Auftrag laden wird geöffnet.
                                        3 Wählen Sie den gewünschten Auftrag aus.
                                        4 Betätigen Sie die Schaltfläche [Laden].
                                        5 Der Dialog wird geschlossen und der gewählte Auftrag wird geladen. Sie
                                          befinden sich jetzt wieder im Hauptfenster.

                                        Ein Los laden
                                        Das Laden eines Loses ist immer gleich. Die Vorgehensweise ist im Bereich
                                        von Terminal IG-In ausführlich beschrieben.
                                         Tutorial, “So laden Sie ein Los” auf Seite 25

                                           Schaltfläche Laden [F2]
                                           Die Schaltfläche Laden [F2] greift auf die zuletzt verwendete Methode (Auf-
                                           trag oder Lauf) zurück. Das bedeutet, haben Sie über das Menü einen Auf-
                                           trag geladen, öffnet sich der Dialog Auftrag laden, wenn Sie das nächste
                                           Mal die Schaltfläche Laden [F2] betätigen. Haben Sie zuletzt einen Lauf
                                           über das Menü geladen, öffnet sich der Dialog Los laden, wenn Sie das
                                           nächste Mal die Schaltfläche Laden [F2] betätigen. Damit weisen Sie der
                                           Schaltfläche quasi die Funktion für das Arbeiten zu: Auftrag laden oder Los
                                           laden.


                                         So überspringen Sie eine Einheit
                                        1 Scannen Sie im Hauptfenster das gewünschte Etikett.
                                        2 Betätigen Sie die Schaltfläche [Abbrechen F6].
                                        3 Die Einheit verschwindet aus der Anzeige und die nächste wird geladen.

                                        Chargen erfassen
                                        Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
1.50 / 01-2023




                                        schrieben.
                                         Tutorial, “So definieren Sie Chargen” auf Seite 37




                 108                                                                           A+W Production Terminal
                 Tutorial                                                         Überblick A+W Production Terminal LG




                                           Den Zustand der Maschine ändern
                                           Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                           terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                           Maschine oder auch Pausenzeiten.
                                           Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                           ausführlich beschrieben.
                                            Tutorial, “Den Zustand der Maschine ändern” auf Seite 26

                                           Beschädigte Scheiben ersetzen
                                           Es kann vorkommen, dass eine Scheibe einer Einheit eine Beschädigung auf-
                                           weist. Haben Sie bereits gute Scheiben der betroffenen Einheit gebucht, kön-
                                           nen Sie die beschädigte Scheibe durch die nächst folgende passende
                                           Scheibe ersetzen. Diese Prozedur erfolgt entweder automatisch oder Sie kön-
                                           nen den Barcode der Scheibe, die die kaputte Scheibe ersetzt, scannen.
                                           Der Ablauf ist wie folgt:
                                           •   1. Scheibe, die in Ordnung ist, buchen.
                                           •   2. Scheibe, die in Ordnung ist, buchen.
                                           •   3. Scheibe hat einen Mangel. Die Scheibe über die Schaltfläche [Bruch]
                                               buchen.
                                           •   Die Scheibe bleibt weiterhin in der Anzeige und wird entsprechend gekenn-
                                               zeichnet.
                                           •   Die Barcodenummer der zu Bruch gemeldeten Scheibe wird durch die
                                               nächste in der Sequenz der Position ersetzt.
                                           •   Sie können auch die nächste Scheibe scannen, dann wird die Barcode-
                                               nummer der zu Bruch gemeldeten Scheibe durch die gescannte Barcode-
                                               Nummer ersetzt.


                                           Weitere Funktionen
                                           Zu den weiteren Funktionen zählen:
                                           •   Gehe zu Produktionsnummer
                                           •   Listen (Reports)
                                           •   Log-Einträge
                                           •   Unterschiedliche Programm-Sprachen
                                           Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den
                                           Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                           schrieben.


                                           Ergänzende Informationen
                                            Softwarereferenz, “Gehe zu Produktionsnummer” auf Seite 169
                                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                                            Tutorial, “Log-Einträge exportieren” auf Seite 31
                                            Tutorial, “Programmsprache wählen” auf Seite 32
1.50 / 01-2023




                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174




                 A+W Production Terminal                                                                           109
                 Überblick A+W Production Terminal LG                                                               Tutorial




                                        Arbeiten mit Terminal LG-Assembly
                                        Lernziele

                                        • Oberfläche von Terminal LG-Assembly kennenlernen.
                                        • Die Funktionsweise kennenlernen und verstehen.


                                        Nutzen

                                        Terminal LG-Assembly unterstützt Sie im Reinraum durch die grafische Darstellung
                                        des Scheibenaufbaus inklusive der Folien. Sobald die Scheibe im Terminal LG-In
                                        gebuch wurde, ist sie im Terminal LG-Assembly sichtbar. Somit steht ausreichend Zeit
                                        zum Schneiden der Folien zur Verfügung.


                                        Merke

                                        Scheibenaufbau              Die Scheiben kommen in der Reihenfolgen, wie sie auf
                                                                    der Grafik zu sehen ist.

                                        Gestelle                    Bei den Gestellen für Terminal LG-Assembly handelt es
                                                                    sich um spezielle Autoklavengestelle.
1.50 / 01-2023




                 110                                                                           A+W Production Terminal
                 Tutorial                                                         Überblick A+W Production Terminal LG




                                           Modul-Präsentation Terminal LG-Assembly
                                           Terminal LG-Assembly ist ein Leitrechner, der im Reinraum die Plausibilität
                                           der Scheibenreihenfolge prüft und die fertige Einheit bucht. Die Arbeitsmenge
                                           sind die am Linieneingang (LG-IN) gelesenen Scheibenbarcodes. Die Einhei-
                                           ten werden hier ebenfalls mit ihren Detaildaten dargestellt.
                                           Dazu zählen z. B. grafische Darstellungen mit Form und Maße der Scheiben,
                                           Folien sowie Auftrags- und Kundeninformationen.
                                           Nachdem Sie Terminal LG-Assembly gestartet haben, präsentiert sich das
                                           Modul wie folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Da-
                                           ten:



                 A
                 B
                                                                                                                        H
                 C




                                                                                                                        I



                 D




                 E                                                                                                      J


                 F
                 G                                                                                                      K


                 A   Menüleiste                           E   Etikettendruck            I Farbliche Darstellung der Einheit
                 B   Produktionsnummer mit Bezeichnung    F   Infofelder                J Gestellnummer
                 C   Liste der aktuellen Einheit          G   Meldungsfenster           K Schaltflächen
                 D   Verlinkte Dokumente                  H   Modellvorschau SN
                 Abb. 22      Terminal LG-Assembly


                                           Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                           runter finden Sie die aktuelle Produktionsnummer sowie die Bezeichnung (B).
                                           Im Bereich (C) finden Sie die Liste der aktuellen Einheit und in (D) die verlink-
                                           ten Dokumente. Der Bereich (E) steuert den Etikettendruck. Im Bereich (F) be-
                                           finden sich die Infofelder. Unter (G) befindet sich das Meldungsfenster. Unter
1.50 / 01-2023




                                           (H) finden Sie die Modellvorschau SN, unter (I) finden Sie die farbliche Dar-
                                           stellung der zu produzierenden Einheit. Im Bereich (J) finden Sie die Gestell-
                                           nummer. Die Schaltflächen befinden sich im Bereich (K).



                 A+W Production Terminal                                                                                111
                 Überblick A+W Production Terminal LG                                                            Tutorial




                                           Anzeige der Spalten ist frei konfigurierbar
                                           Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                           schirmdarstellung von Ihrer Darstellung abweichen.

                                        Detaillierte Erläuterung zu den einzelnen Bereichen
                                        Die Bereiche (A), (B), (C), (D), (F), (G), (H) und (K) von Terminal LG-Assembly
                                        sind identisch sind mit den Bereichen von Terminal IG-In und werden an dieser
                                        Stelle nicht noch einmal beschrieben.
                                         Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19
                                        Im Bereich (C) sind folgende Symbole möglich:

                                        Symbol        Erläuterung

                                                      Kennzeichnet eine gebuchte Scheibe.

                                                      Kennzeichnet eine Scheibe, die im LG-In
                                                      als Bruch gemeldet wurde.

                                                      Kennzeichnet eine Scheibe, die im LG-In
                                                      übersprungen wurde.

                                                      Kennzeichnet Folien oder Scheiben, die
                                                      noch kommen werden.


                                        Das Feld (E) von Terminal LG-Assembly ist identisch mit dem Feld von Termi-
                                        nal TG-In und wird an dieser Stelle nicht noch einmal beschrieben.
                                         Tutorial, “Modul-Präsentation Terminal TG-In” auf Seite 90
                                        Das Feld (I) von Terminal LG-Assembly ist identisch mit dem Bereich von Ter-
                                        minal LG-In und wird an dieser Stelle nicht noch einmal beschrieben.
                                         Tutorial, “Modul-Präsentation Terminal LG-In” auf Seite 105

                                        Bereich J - Gestellnummer
                                        Das Feld Gestellnummer steht in Zusammenhang mit der Schaltfläche [Aus-
                                        gang F9] und kennzeichnet das Gestell, das in den Autoklaven geschoben
                                        wird. Mit jedem Betätigen der Schaltfläche [Ausgang F9], wird die Gestellnum-
                                        mer hochgezählt, bis die maximale Anzahl an Autoklavengestellen in Ihrem
                                        Hause erreicht ist.
1.50 / 01-2023




                 112                                                                            A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal LG




                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal LG-Assembly ist:
                                           •   Starten Sie das Modul Terminal LG-Assembly.
                                           •   Melden Sie sich an (<Name>).
                                           •   Wählen Sie ein Gestell für den Autoklaven aus.
                                           •   Buchen Sie die Einheit.
                                           Wann immer Sie Ihre Arbeit an der Maschine unterbrechen, müssen Sie dies
                                           protokollieren. Gründe für eine Unterbrechung können sein:
                                           •   Wartung der Maschine.
                                           •   Störung der Maschine.
                                           •   Pausenzeiten.
                                           Sollte eine Scheibe, die Sie gerade buchen wollen, eine Beschädigung auf-
                                           weisen, müssen Sie den entsprechenden Grund ebenfalls buchen. Gründe für
                                           Mängel können sein:
                                           •   Bruch
                                           •   Kratzer
                                           •   Riss

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So überspringen Sie eine Einheit
                                           1 Betätigen Sie die Schaltfläche [Abbrechen F6].
                                           2 Die Einheit verschwindet aus der Anzeige und die nächste wird geladen

                                           Chargen erfassen
                                           Wie man Chargen erfasst, ist im Bereich von Terminal IG-In ausführlich be-
                                           schrieben.
                                            Tutorial, “So definieren Sie Chargen” auf Seite 37

                                           Den Zustand der Maschine ändern
                                           Während des Produktionsbetriebes kann es vorkommen, dass die Arbeit un-
                                           terbrochen werden muss. Gründe dafür sind z. B. Wartungsarbeiten an der
                                           Maschine oder auch Pausenzeiten.
                                           Wie man den Zustand der Maschine ändert, ist im Bereich von Terminal IG-In
                                           ausführlich beschrieben.
                                            Tutorial, “Den Zustand der Maschine ändern” auf Seite 26
1.50 / 01-2023




                 A+W Production Terminal                                                                            113
                 Überblick A+W Production Terminal LG                                                          Tutorial




                                        Umgang mit beschädigten Scheiben
                                        Unter Umständen kann es vorkommen, dass sich auf der Linie eine Scheibe
                                        befindet, die Sie aber nicht verwenden können, da sie einen Mangel aufweist.
                                        Dann ist es nötig, die Scheibe entsprechend zu kennzeichnen.
                                        Wie Sie mit beschädigten Scheiben verfahren, ist im Bereich von Terminal IG-
                                        In ausführlich beschrieben.
                                         Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28


                                        Weitere Funktionen
                                        Zu den weiteren Funktionen zählen:
                                        •   Listen (Reports)
                                        •   Log-Einträge
                                        •   Unterschiedliche Programm-Sprachen
                                        Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den
                                        Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                        schrieben.


                                        Ergänzende Informationen
                                         Tutorial, “Listen (Reports) generieren” auf Seite 31
                                         Tutorial, “Log-Einträge exportieren” auf Seite 31
                                         Tutorial, “Programmsprache wählen” auf Seite 32
                                         Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
1.50 / 01-2023




                 114                                                                          A+W Production Terminal
                 Tutorial                                                    Überblick A+W Production Terminal Edit




                                           Überblick A+W Production
                                           Terminal Edit
                                           In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit
                                           dem A+W Production Terminal Edit (Terminal Edit) kennen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Arbeiten mit Terminal Edit
1.50 / 01-2023




                 A+W Production Terminal                                                                      115
                 Überblick A+W Production Terminal Edit                                                             Tutorial




                                         Arbeiten mit Terminal Edit
                                         Lernziele

                                         • Oberfläche von Terminal Edit kennenlernen.
                                         • Die Funktionsweise kennenlernen und verstehen.


                                         Nutzen

                                         Terminal Edit unterstützt Sie im Versandbereich beim Buchen von größeren Mengen.
                                         Das spart Zeit und Geld.


                                         Definitionen

                                         Quelldaten                Bei den Quelldaten handelt es sich um die Daten, die
                                                                   Sie umgebucht werden sollen.

                                         Zieldaten                 Zieldaten sind die Daten, wo die Quelldaten hingebucht
                                                                   werden.

                                         Kopfteile                 Kopfteil einer Stückliste (z. B. ISO).

                                         Unterteile                Unterteile einer Stückliste (z. B. Float 4 mm)

                                         ES-Typ                    Abkürzung für Erfassungsstellen-Typ.

                                         Erf.-Stelle               Abkürzung für Erfassungsstelle

                                         Zust. Typ                 Abkürzung für Zustand-Typ
1.50 / 01-2023




                 116                                                                             A+W Production Terminal
                 Tutorial                                                           Überblick A+W Production Terminal Edit




                                              Modul-Präsentation Terminal Edit
                                              Im Produktionsalltag kommt es vor, dass Bearbeitungen durchgeführt werden,
                                              ohne dass diese gebucht werden, oder dass falsche Buchungen durchgeführt
                                              werden. An dieser Station können solche Umbuchungen durchgeführt wer-
                                              den.
                                              Es besteht die Möglichkeit, Einheiten, Scheiben oder Gruppen auf Gestelle
                                              und auf Erfassungsstellen umzubuchen. Gestelle können auch auf andere Er-
                                              fassungsstellen gebucht werden. Terminal Edit bietet darüber hinaus die Mög-
                                              lichkeit, außer-Haus-Gestelle zu verwalten.
                                              Nachdem Sie Terminal Edit gestartet haben, präsentiert sich das Modul wie
                                              folgt. Zum besseren Verständnis zeigt das folgende Bild bereits Daten. Wenn
                                              Sie das Modul starten, ist das Hauptfenster leer:



                 A
                 B                                                                                                        H



                 C



                 D
                                                                                                                         I

                                                                                                                         J




                 E                                                                                                       K

                 F
                                                                                                                         L
                 G

                 A   Menüleiste                              E Schaltflächen für          I Zur Verfügung stehenden
                 B   Quelldaten                                Quellbereich                 Zieldaten
                 C   Filterfunktion                          F Infofelder                 J Schaltflächen zum Verschieben
                 D   Zur Verfügung stehenden Quelldaten      G Meldungsfelder             K Schaltflächen für Zieldatenbereich
                                                             H Zieldaten                  L Schaltflächen allgemein
                 Abb. 23      Terminal Edit


                                              Im oberen Bereich befindet sich von links nach rechts die Menüleiste (A). Da-
                                              runter finden Sie den Bereich zum Selektieren der Quelldaten (B) sowie die
1.50 / 01-2023




                                              Filterfunktion (C). Im Bereich (D) finden Sie die geladenen Quelldaten und in
                                              (E) die Schaltflächen für die Quelldaten. Im Bereich (F) befinden sich die Info-
                                              felder und im Bereich (G) das Meldungsfenster. Der Bereich (H) dient zum Se-


                 A+W Production Terminal                                                                                 117
                 Überblick A+W Production Terminal Edit                                                           Tutorial




                                         lektieren der Zieldaten. Unter (I) finden Sie die geladenen Zieldaten und unter
                                         (J) die Schaltflächen zum Verschieben der Daten. Unter (K) befinden Sie die
                                         Schaltflächen für die Zieldaten und unter (L) die allgemeinen Schaltflächen.

                                             Anzeige der Spalten ist frei konfigurierbar
                                             Die Anzeige der Spalten ist fei konfigurierbar. Daher kann die gezeigte Bild-
                                             schirmdarstellung von Ihrer Darstellung abweichen.

                                         Detaillierte Erläuterung zu den einzelnen Bereichen
                                         Die Bereiche (A), (F) und (G) von Terminal Edit sind identisch sind mit den Be-
                                         reichen von Terminal IG-In und werden an dieser Stelle nicht noch einmal be-
                                         schrieben.
                                          Tutorial, “Modul-Präsentation Terminal IG-In” auf Seite 19

                                         Bereich B und E - Quelldaten und Schaltflächen
                                         Hier stehen Ihnen zum Laden der Quelldaten verschiedene Möglichkeiten zur
                                         Verfügung. Sie können für folgende Bereiche Quelldaten laden:
                                         •   Erfassungsstellen-Typ (Gruppe von Erfassungsstellen, z. B. Produktions-
                                             bereich).
                                         •   Erfassungsstellen (Tische, Handzuschnitt, Wareneingang, etc.).
                                         •   Gestelle (vorhandenen Gestelle).
                                         •   Auftrag (vorhandene Aufträge).
                                         •   Etikett (vorhandene Etikett-Nummern).
                                         •   Lauf (vorhandene Läufe).
                                         Wählen Sie aus den entsprechenden Bereichen über die Komboboxen die ge-
                                         wünschten Einträge, z. B. den Eintrag Außer Haus im Bereich Erfassungsstel-
                                         le. Um die Daten zu laden, betätigen Sie die Schaltfläche [Hinzufügen].

                                         Bereich C - Filterfunktion
                                         Über diese beiden Checkboxen haben Sie die Möglichkeit, die angezeigten
                                         Daten einzuschränken. Sie können sich alle Teile (der Stückliste), nur die
                                         Kopfteile (der Stückliste) oder auch nur die Unterteile (der Stückliste) anzeigen
                                         lassen. Neben den beiden Checkboxen befindet sich eine Kombobox, die fest
                                         definierte Typen enthält. Sie können die Anzeige dadurch nochmal einschrän-
                                         ken. Bsp.: Sie möchten nur die Unterteile eines ISOs angezeigt bekommen.
                                         Aktivieren Sie die Checkbox Unterteile und wählen Sie aus der Kombobox den
                                         Eintrag ISO.

                                         Bereich D - Anzeige der Quelldaten
                                         Nachdem im Bereich Quelle die entsprechende Auswahl getroffen haben, be-
                                         tätigen Sie die Schaltfläche [Hinzufügen]. Anschließend werden die Daten in
                                         diesem Bereich angezeigt.
1.50 / 01-2023




                 118                                                                            A+W Production Terminal
                 Tutorial                                                       Überblick A+W Production Terminal Edit




                                           A                                               E
                                           B                                               F
                                           C
                                           D




                                           A Gruppierungsbereich                  D Tabellenkopf
                                           B Gruppierungen und Sortierungen       E Felder für Tabellenkopf
                                           C Tabellenkopf                         F Schaltfläche zum Auf- und Zuklappen
                                                                                    der Gruppeninhalte


                                           Im Bereich (A) haben Sie die Möglichkeit, die geladenen Daten zu gruppieren
                                           und innerhalb der Gruppierung zu sortieren. Eine Gruppierung erstellen Sie,
                                           indem Sie im Tabellenkopf das gewünschte Feld (z. B. Glasart) anklicken und
                                           die Maustaste gedrückt halten. Schieben Sie das Feld, mit gedrückter Maus-
                                           taste, in den Gruppierungsbereich und lassen Sie die Maustaste los. Ihr Tabel-
                                           lenkopf sieht jetzt so aus:




                                           Um innerhalb der Gruppierung noch eine Sortierung hinzuzufügen, gehen Sie
                                           genauso vor. Sie klicken mit der Maus im Tabellenkopf das gewünschte Feld
                                           (z.B. Gestell alt) an und ziehen es mit gedrückter Maustaste nach oben in den
                                           Gruppierungsbereich. Ihr Tabellenkopf sieht jetzt so aus:




                                           Betätigen Sie die Symbol-Schaltfläche Spalten, öffnet sich folgender Auswahl-
                                           Dialog:
1.50 / 01-2023




                                           Sie können mit der Maus die einzelnen Felder anklicken und mit gehaltener
                                           Maustaste das Feld an die gewünschte Stelle im Tabellenkopf zielen. An der
                                           entsprechenden Stelle angekommen, lassen Sie die Maustaste los.


                 A+W Production Terminal                                                                            119
                 Überblick A+W Production Terminal Edit                                                      Tutorial




                                         Über die Symbol-Schaltflächen Plus und Minus können Sie die Gruppierungs-
                                         inhalte auf- und zuklappen.
                                         Beispiel einer zugeklappten Sortierung:




                                         Beispiel einer aufgeklappten Sortierung:




                                         Bereich H und K - Zieldaten und Schaltflächen
                                         Hier stehen Ihnen zum Laden der Zieldaten verschiedene Möglichkeiten zur
                                         Verfügung. Sie können für folgende Bereiche Zieldaten laden:
                                         •   Erfassungsstellen-Typ, Erfassungsstellen und Gestelle sind identisch mit
                                             den Feldern im Bereich Quelle.
                                         •   Zustand Typ (Gruppe von Zuständen, z. B. Beginn, Mangel, Maschinensta-
                                             tus, etc.).
                                         •   Zustand (mögliche Zustände, z. B. Kratzer, Bereit).
                                         Wählen Sie aus den entsprechenden Bereichen über die Komboboxen die ge-
                                         wünschten Einträge, z. B. den Eintrag Außer Haus im Bereich Erfassungsstel-
                                         le. Um die Daten zu laden, betätigen Sie die Schaltfläche [Hinzufügen].

                                         Bereich I - Anzeige der Zieldaten
                                         Nachdem im Bereich Ziel die entsprechende Auswahl getroffen haben, betä-
                                         tigen Sie die Schaltfläche [Hinzufügen]. Anschließend werden die Daten in
                                         diesem Bereich angezeigt.
                                         Der Tabellenkopf in diesem Bereich ist identisch mit dem Tabellenkopf im Be-
                                         reich Quelldaten und wird an dieser Stelle nicht noch einmal erläutert.
1.50 / 01-2023




                 120                                                                       A+W Production Terminal
                 Tutorial                                                          Überblick A+W Production Terminal Edit




                                           Bereich J - Schaltflächen zum Verschieben der Daten
                                           Mit diesen Schaltflächen können Sie die Daten aus dem Quellbereich in den
                                           Zielbereich verschieben oder auch umgekehrt.

                                           Bereich L - Schaltflächen
                                           Die Schaltfläche Aktualisieren [F2] dient dem Auffrischen der Anzeige.
                                           Über die Schaltfläche [Reset] leeren Sie die Anzeige.
                                           Betätigen Sie die Schaltfläche Übernehmen [F5], werden die Daten von der
                                           Quelle auf das Ziel gebucht.


                                           Ablauf von Arbeitsschritten
                                           Die Vorgehensweise zum Arbeiten in Terminal Edit ist:
                                           •   Starten Sie das Modul Terminal Edit.
                                           •   Melden Sie sich an (<Name>).
                                           •   Laden Sie die Quelldaten.
                                           •   Bei Erfassungsstellen wählen Sie das Gestell aus.
                                           •   Wählen Sie den Zielbereich aus.
                                           •   Buchen Sie die Daten vom Quellbereich auf den Zielbereich.

                                           Anmelden an der Arbeitsstation
                                           Die Anmeldung an den unterschiedlichen Arbeitsstationen ist immer gleich.
                                           Sie ist im Bereich von Terminal IG-In ausführlich beschrieben.
                                            Tutorial, “So melden Sie sich an” auf Seite 24


                                            So laden Sie eine Erfassungsstelle
                                           1 Öffnen Sie im Feld Erf.-Stelle die Kombobox und wählen Sie die entspre-
                                             chende Erfassungsstelle aus. Alternativ dazu können Sie auch die erste
                                             Ziffer der Erfassungsstelle tippen. Es werden anschließend alle Erfas-
                                             sungsstellen angezeigt, die mit dieser Ziffer beginnen.
                                           2 Wählen Sie die entsprechende Erfassungsstelle aus.
                                           3 Betätigen Sie die Schaltfläche [Hinzufügen].
                                           4 Die Daten werden geladen.


                                            So laden Sie ein Gestell
                                           1 Öffnen Sie im Feld Gestell die Kombobox und wählen Sie das entspre-
                                             chende Gestell aus. Alternativ dazu können Sie auch die erste Ziffer des
                                             Gestells tippen. Es werden anschließend alle Gestelle angezeigt, die mit
                                             dieser Ziffer beginnen.
                                           2 Wählen Sie das entsprechende Gestell aus.
1.50 / 01-2023




                                           3 Betätigen Sie die Schaltfläche [Hinzufügen].
                                           4 Die Daten werden geladen.



                 A+W Production Terminal                                                                            121
                 Überblick A+W Production Terminal Edit                                                    Tutorial




                                          So laden Sie einen Auftrag, einen Lauf oder ein Etikett
                                         1 Entscheiden Sie, ob Sie eine Auftragsnummer, eine Laufnummer oder eine
                                           Etikettnummer laden wollen und wählen Sie in der Kombobox den entspre-
                                           chenden Eintrag Auftrag, Lauf oder Etikett.
                                         2 Geben Sie im Feld darunter die entsprechende Nummer ein.
                                         3 Betätigen Sie die Schaltfläche [Hinzufügen].
                                         4 Die Daten werden geladen.


                                          So buchen Sie einen LKW außer Haus
                                         1 Öffnen Sie im Bereich Quelle die Kombobox Erf.-Stelle oder ES-Typ. Wäh-
                                           len Sie den Eintrag LKW.
                                         2 Betätigen Sie die Schaltfläche [Hinzufügen]. Die Daten werden geladen.
                                         3 Öffnen Sie im Bereich Ziel die Kombobox Zustand. Wählen Sie den Eintrag
                                           Ausgeliefert.
                                         4 Betätigen Sie die Schaltfläche [Hinzufügen]. Die Daten werden geladen.
                                         5 Wählen Sie im Bereich Quelle aus der Liste den LKW aus, den Sie umbu-
                                           chen möchten. Sie können auch alle LKWs auswählen und mit einem Klick
                                           umbuchen.
                                         6 Betätigen Sie die Schaltfläche zum Verschieben.
                                         7 Die Daten werden vom Quell- in den Zielbereich verschoben.
                                         8 Betätigen Sie die Schaltfläche [Übernehmen]. Die Daten werden gebucht.

                                            Daten versehentlich oder falsch gebucht
                                            Sollten Sie Daten versehentlich gebucht haben, können Sie auf die oben
                                            beschriebene Art und Weise die Daten aus dem Zielbereich wieder in den
                                            Quellbereich verschieben.
1.50 / 01-2023




                 122                                                                      A+W Production Terminal
                 Tutorial                                                         Überblick A+W Production Terminal Edit




                                            So passen Sie den Tabellenkopf im Bereich der Quelldaten an
                                           Das Erscheinungsbild von Terminal Edit wird bei der Installation konfiguriert.
                                           Sollten Sie im Laufe der Zeit feststellen, dass Sie gerne zusätzliche Felder an-
                                           gezeigt bekommen möchten, oder auch vorhandene Felder überflüssig ge-
                                           worden sind, gehen Sie wie folgt vor.
                                           1 Wählen Sie die Erf.-Stelle oder das Gestell aus.
                                           2 Betätigen Sie die Schaltfläche [Hinzufügen]. Die Daten werden geladen.
                                           3 Der Dialog Auftrag laden wird geöffnet.
                                           4 Wählen Sie den gewünschten Auftrag aus.
                                           5 Betätigen Sie die Schaltfläche [Laden].
                                           6 Der Dialog wird geschlossen und der gewählte Auftrag wird geladen. Sie
                                             befinden sich jetzt wieder im Hauptfenster.


                                           Weitere Funktionen
                                           Zu den weiteren Funktionen zählen:
                                           •   Listen (Reports)
                                           •   Log-Einträge
                                           •   Unterschiedliche Programm-Sprachen
                                           Da in diesem Bereich die Felder von Terminal IG-Out identisch sind mit den
                                           Feldern von Terminal IG-In, werden sie an dieser Stelle nicht noch einmal be-
                                           schrieben.


                                           Ergänzende Informationen
                                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                                            Tutorial, “Log-Einträge exportieren” auf Seite 31
                                            Tutorial, “Programmsprache wählen” auf Seite 32
                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
1.50 / 01-2023




                 A+W Production Terminal                                                                              123
                 Überblick A+W Production Terminal Edit                    Tutorial
1.50 / 01-2023




                 124                                      A+W Production Terminal
Production Terminal


                      Softwarereferenz
                 Bedienung der Module                                                              Softwarereferenz




                                        Bedienung der Module
                                        Die Module starten Sie entweder über einen Desktop-Shortcut, oder über den
                                        entsprechenden Eintrag im Menü Start > Programme (unter Windows).
                                        Im Anschluss finden Sie Erläuterungen zu den in der Dokumentation verwen-
                                        deten Begriffe und wie Sie das Programm beenden.
                                        •   Softwarebegriffe
                                        •   Programm beenden


                                        Softwarebegriffe
                                        In diesem Abschnitt wird Ihnen der allgemeine Umgang mit den Menüs und
                                        den Dialogen vorgestellt.
                                        Nachfolgend erhalten Sie Informationen zu:
                                        •   Schaltflächen
                                        •   Optionsschalter
                                        •   Kombobox
                                        •   Menüleiste/Menüpunkt
                                        •   Tastaturbefehle


                                        Schaltflächen




                                        Optionsschalter




                                        In einem Rahmen mit Optionsschaltern kann immer nur eine Option ange-
                                        wählt werden! In der Abbildung oben ist die Option Senkrecht angewählt. Kli-
                                        cken Sie z. B. nun die Option Waagerecht an, wird automatisch die Option
                                        Senkrecht abgewählt.


                                        Kombobox
1.50 / 01-2023




                 126                                                                           Production Terminal
                 Softwarereferenz                                                               Bedienung der Module




                                       Wenn Sie in einer Kombobox auf den Pfeil rechts klicken, öffnet sich eine Aus-
                                       wahlliste. Wählen Sie aus dieser Liste den gewünschten Eintrag durch Ankli-
                                       cken aus. Ihre Auswahl wird in der Anzeige dargestellt.


                                       Menüleiste/Menüpunkt




                                       Auch Pull-Down-Menü-Leiste genannt. Wenn Sie z. B. eine Fassadenanlage
                                       erstellen möchten, klicken Sie mit der Maus auf den Menüeintrag Makros, das
                                       entsprechende Pull– Down– Menü öffnet sich (siehe Abbildung oben) und hier
                                       auf den Menüeintrag Fassadenanlage.


                                       Tastaturbefehle
                                       Tastaturbefehle sind Tasten oder Tastenkombinationen, mit denen ein Befehl
                                       aufgerufen bzw. eine Funktion ausgeführt wird. Tastaturbefehle helfen dem
                                       geübten Benutzer schnell zum gewünschten Ergebnis zu gelangen. Nachfol-
                                       gend erhalten Sie einen Überblick über die wichtigsten Tastaturbefehle und
                                       Funktionstasten:

                                       Tastaturbefehl           Erläuterung

                                       [F1]                      Mit dieser Funktionstaste erfassen Sie eine Charge.
                                                                 Der Dialog Manuelle Eingabe wird geöffnet.

                                       [F2]                      Wenn Sie diese Funktionstaste betätigen, können Sie
                                                                 ein neues Los laden. Der Dialog Lade Los wird
                                                                 geöffnet.

                                       [F3]                      Mit dieser Funktionstaste bringen Sie die Maschine in
                                                                 einen anderen Zustand. Der Dialog Status wird
                                                                 geöffnet.

                                       [F4]                      Mit dieser Funktionstaste melden Sie eine Person an
                                                                 der Maschine an. Der Dialog ToolTV Anmeldung wird
                                                                 geöffnet.
                                                                 Sie können mit dieser Taste auch zwischen mehreren
                                                                 Schirmen umschalten.

                                       [F5]                      Wenn Sie diese Funktionstaste betätigen, wird die
                                                                 aktuelle Einheit in den Status produziert gebucht.

                                       [F6]                      Wenn Sie diese Funktionstaste betätigen, wird die
                                                                 aktuelle Einheit übersprungen und die nächsten Einheit
                                                                 zur Produktion angezeigt. Es erfolgt keine Buchung.
1.50 / 01-2023




                                       [F7]                      Wenn Sie diese Funktionstaste betätigen, wird die
                                                                 aktuelle Scheibe zu Bruch gebucht. Der Dialog Zustand
                                                                 wird geöffnet.



                 Production Terminal                                                                                   127
                 Bedienung der Module                                                                  Softwarereferenz




                                        Tastaturbefehl            Erläuterung

                                        [F8]                      Wenn Sie diese Funktionstaste betätigen, können Sie
                                                                  einen Nachläufer laden. Der Dialog Nachläufer laden
                                                                  wird geöffnet.

                                        [F11]                     Mit dieser Funktionstaste können Sie eine andere
                                                                  Produktionsnummer laden. Der Dialog Gehe zu
                                                                  Produktionsnummer wird geöffnet.

                                        [F12]                     Mit dieser Funktionstaste starten Sie die Vorschau. Der
                                                                  Dialog Vorschau wird geöffnet.

                                            Aktive bzw. inaktive Schaltflächen
                                            In den verschiedenen Programmdialogen finden Sie aktive und inaktive
                                            Schaltflächen vor. Die Schaltflächen werden abhängig von den Eingaben
                                            aktiv oder inaktiv!


                                        Programm beenden
                                        Es bestehen verschiedene Möglichkeiten das Programm zu beenden.
                                        •   Mausklick auf die Schaltfläche [Schließen] in der rechten oberen Pro-
                                            gramm-Fensterecke beendet das Programm.
                                        •   Über das Menü Datei > Beenden.

                                            Hinweis zum Beenden
                                            Wurden Daten geändert bzw. neue Daten erfasst, die noch nicht gesichert
                                            wurden, erscheint ein entsprechender Hinweis. Wählen Sie [Ja] um den Di-
                                            alog Datei speichern unter … zu aktivieren. Sie können hier die Datei bzw.
                                            Ihre Änderungen speichern. Anschließend wird das Programm beendet.
                                            Wählen Sie [Nein] um das Programm ohne Speichern der Datei bzw. der
                                            Änderungen zu beenden. Wählen Sie [Abbrechen] um den Vorgang Been-
                                            den abzubrechen und mit dem Programm weiter zu arbeiten.
1.50 / 01-2023




                 128                                                                                Production Terminal
                 Softwarereferenz                                                             Übersicht allgemein




                                       Übersicht allgemein
                                       In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                       •   Übersicht Terminal IG
                                       •   Übersicht Terminal Manual Cutting
                                       •   Übersicht Terminal Order
                                       •   Übersicht Terminal Processing
                                       •   Übersicht Terminal TG
                                       •   Reports
                                       •   Die Hilfe verwenden

                                           Dialoge können von unterschiedlichen Stellen aus geöffnet werden
                                           Bitte beachten Sie, dass Dialoge und Funktionen auf verschiedenen We-
                                           gen geöffnet werden können. In dieser Anleitung werden die entsprechen-
                                           den Dialoge nur einmal beschrieben.
1.50 / 01-2023




                 Production Terminal                                                                           129
                 Übersicht Terminal IG                                                                     Softwarereferenz




                                         Übersicht Terminal IG
                                         Terminal IG kommt an der Isolierglas-Linie zum Einsatz und zeigt Ihnen alle
                                         verfügbaren Lose inklusive produktionsunterstützender Informationen.
                                         Die Module Terminal IG-In, Terminal IG-Assembly und Terminal IG-Out haben
                                         die gleichen Menüs:
                                         •   Menü Datei
                                         •   Menü Listen
                                         •   Menü Maschine
                                         •   Menü Extras (für A+W-Mitarbeiter)
                                         •   Menü ?
                                         In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                         •   Menü Datei, Menü-Eintrag Ummelden:
                                             Mit diesen Menüpunkt melden Sie sich am Terminal an.
                                              Softwarereferenz, “Registrierung” auf Seite 131
                                         •   Menü Datei, Menü-Eintrag Springe zu ProdNr. [F11]:
                                             Mit diesem Menüpunkt können Sie direkt zu einer anderen Produktions-
                                             nummer springen.
                                              Softwarereferenz, “Gehe zu Produktionsnummer” auf Seite 132
                                         •   Menü Datei, Menü-Eintrag Vorschau-Dialog [F12:
                                             Mit diesem Menüpunkt öffnen Sie die Dialog Vorschau.
                                              Softwarereferenz, “Vorschau” auf Seite 133
                                         •   Menü Datei, Menü-Eintrag Charge [F1]:
                                             Wählen Sie diesen Menüpunkt um Chargen zuzuweisen.
                                              Softwarereferenz, “Charge” auf Seite 135
                                         •   Menü Listen, Menü-Eintrag Auftragsübersicht:
                                             Mit diesen Menüpunkt drucken Sie den Report Auftragsübersicht.
                                              Softwarereferenz, “Parametereingabe für Report” auf Seite 172
                                         •   Menü Maschine, Menü-Eintrag Maschinenstatus Dialog [F3]:
                                             Wählen Sie diesen Menüpunkt um Arbeitsunterbrechungen zu buchen.
                                              Softwarereferenz, “Status” auf Seite 142
                                         •   Benutzer Hilfe:
                                             Über diesen Menüpunkt starten Sie die Kurzbeschreibungen.
                                         •   Aktuelle Logeinträge:
                                             Über diesen Menüpunkt starten Sie die Log-Datei. Diese Datei enthält die
                                             Log-Einträge für die jeweilige Sitzung.
                                              Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
                                         •   Sprache ändern:
                                             Über diesen Menüpunkt können Sie die Modulsprache ändern. Es öffnet
                                             sich der Dialog Sprache ändern.
                                              Softwarereferenz, “Sprachauswahl” auf Seite 175
                                         •   Informationen:
                                             Über diesen Menüpunkt können Sie sich weitere Informationen zu den Mo-
                                             dulen anzeigen lassen. Es öffnet sich der Dialog Version Infos.
1.50 / 01-2023




                                              Softwarereferenz, “Über Production Terminal” auf Seite 176




                 130                                                                                  Production Terminal
                 Softwarereferenz                                                             Übersicht Terminal IG




                                       Registrierung
                                       Datei > Ummelden
                                       oder über die Funktionstaste
                                       F4




                                       Abb. 24       Anmelden


                                       Dieser Dialog hat zwei Funktionen. Er erscheint automatisch, wenn Sie das
                                       Programm starten. Dann geben Sie im Feld Anwender Ihren Namen ein. Das
                                       entsprechende Terminal-Modul wird gestartet. Wenn bereits ein Terminal-Mo-
                                       dul läuft, können Sie mit diesem Dialog dann einen anderen Benutzer anmel-
                                       den (z. B. Wechsel eines Mitarbeiters).

                                            Namen scannen
                                            Wenn Sie mit einem Scanner arbeiten, können Sie direkt im Hauptfenster
                                            unter Person Ihren Namen scannen und brauchen nicht den Dialog ToolTV
                                            Registrierung öffnen.

                                       Erläuterung der Felder

                                       Anwender Wählen Sie aus der Kombobox den entsprechenden Anwender
                                       aus.
                                       Technische Info: Pflichtfeld, Auswahl

                                       ToolTV Wählen Sie aus der Kombobox den Leitrechner aus, an dem Sie sich
                                       anmelden möchten.
                                       Technische Info: Pflichtfeld, Auswahl

                                       Erläuterung der Schaltflächen

                                       OK Haben Sie in den Feldern Anwender und ToolTV die gewünschten Aus-
                                       wahlen getroffen, wird durch das Betätigen der Schaltfläche [OK] der entspre-
                                       chende Leitrechner geöffnet. In diesem Beispiel wird Terminal IG-In geöffnet.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen.


                                       Ergänzende Informationen
1.50 / 01-2023




                                        Tutorial, “So melden Sie sich an” auf Seite 24




                 Production Terminal                                                                           131
                 Übersicht Terminal IG                                                                    Softwarereferenz




                                         Gehe zu Produktionsnummer
                                         Datei > Springe zu ProdNr.
                                         oder über die Funktionstaste
                                         F11




                                         Abb. 25      Gehe zu Produktionsnummer


                                         Mit diesem Dialog können Sie eine andere Produktionsnummer laden. Die
                                         Produktionsnummer bestimmt die Reihenfolge der zu produzierenden Einhei-
                                         ten. So können Sie z. B. direkt von der Produktionsnummer 3 auf die Produk-
                                         tionsnummer 15 springen ohne mehrfach die Schaltfläche [Überspringen]
                                         betätigen zu müssen. Das kann der Fall sein, wenn noch Nachläufer unter-
                                         wegs sind.

                                         Erläuterung der Felder

                                         Produktionsnummer Wählen Sie über die Pfeiltasten die Produktionsnum-
                                         mer aus, die als nächstes produziert werden soll.

                                         Erläuterung der Schaltflächen

                                         OK Wenn Sie diese Schaltfläche betätigen, wird die gewählte Produktions-
                                         nummer übernommen.

                                         Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                         schlossen. Die gewählte Produktionsnummer wird nicht übernommen.


                                         Ergänzende Informationen
                                          Tutorial, “Eine andere Produktionsnummer laden” auf Seite 29
1.50 / 01-2023




                 132                                                                                Production Terminal
                 Softwarereferenz                                                             Übersicht Terminal IG




                                       Vorschau
                                       Datei > Vorschau-Dialog
                                       oder über die Funktionstaste
                                       F12




                                       Abb. 26     Vorschau


                                       Dieser Dialog zeigt Ihnen die Arbeitsmenge für die jeweilige Erfassungsstelle
                                       und den heutigen Tag. Über die Radiotasten haben Sie die Möglichkeit, die
                                       Anzeige einzuschränken.

                                       Erläuterung der Felder

                                       Erfassungsstelle In diesem Feld wird Ihnen die Erfassungsstelle angezeigt,
                                       auf die sich die Vorschau bezieht.

                                       Alle Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben an-
                                       gezeigt.

                                       Verfügbare Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die
                                       Scheiben angezeigt, die zurzeit verfügbar sind.

                                       Geplante Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben
                                       angezeigt, die geplant sind.
1.50 / 01-2023




                                       Mögliche Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Schei-
                                       ben angezeigt, deren Bearbeitung möglich ist.



                 Production Terminal                                                                            133
                 Übersicht Terminal IG                                                            Softwarereferenz




                                         Erläuterung der Schaltflächen

                                         Schließen Wenn Sie diese Schaltfläche oder die Funktionstaste [F5] betäti-
                                         gen, wird der Dialog geschlossen.
1.50 / 01-2023




                 134                                                                           Production Terminal
                 Softwarereferenz                                                             Übersicht Terminal IG




                                       Charge
                                       Datei > Charge
                                       oder über die Funktionstaste
                                       F1




                                       Abb. 27      Charge


                                       Mit diesem Dialog können Sie Chargen zuweisen. Chargen dienen der Quali-
                                       tätssicherung und -überwachung. Für Terminal IG-Assembly wäre z. B. an der
                                       Visitierstation ein Butyl-Fass eine denkbare Charge.

                                       Erläuterung der Felder

                                       Charge Geben Sie in diesem Feld die gewünschte Chargen-Bezeichnung
                                       ein. Alphanumerische Werte sind möglich.

                                       Erläuterung der Schaltflächen

                                       OK Wenn Sie diese Schaltfläche betätigen, wird die eingegebene Charge
                                       übernommen.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen. Die eingegebene Charge wird nicht übernommen.


                                       Ergänzende Informationen
                                        Tutorial, “So definieren Sie Chargen” auf Seite 37
1.50 / 01-2023




                 Production Terminal                                                                          135
                 Übersicht Terminal IG                                                                   Softwarereferenz




                                         Los laden
                                         ToolTV IG-In > [Los laden]
                                         oder über die Funktionstaste
                                         F2




                                         Abb. 28        Los laden


                                         In diesem Dialog werden Ihnen die zur Bearbeitung anstehenden Läufe inklu-
                                         sive aller enthaltenen Lose angezeigt. Der Dialog ist in zwei Fenster unterteilt.
                                         Im linken Fenster befindet sich die Übersicht aller anstehenden Läufe. Wählen
                                         Sie einen Lauf aus, sehen Sie im rechten Fenster, welche Einheiten zu diesem
                                         Lauf gehören und auf welcher Gestell-Nummer sie sich befinden. Sollten Sie
                                         nicht alle aufgeführten Gestell-Nummern für den Lauf im Zugriff haben, kön-
                                         nen Sie auch nur die vorhandenen Gestell-Nummern laden.

                                              Filter löschen
                                              Terminal IG-In merkt sich den zuletzt bearbeiteten Lauf. Um alle Läufe se-
                                              hen zu können, müssen Sie deshalb den Filter löschen. Zum Löschen des
                                              Filters betätigen Sie die Schaltfläche [Alle anzeigen]. Sie erhalten dann die
                                              vollständige Laufliste.
1.50 / 01-2023




                 136                                                                                 Production Terminal
                 Softwarereferenz                                                              Übersicht Terminal IG




                                       Erläuterung der Felder

                                       Lauf In dieser Spalte werden alle Läufe angezeigt, die zur Produktion an der
                                       angemeldeten Maschine anstehen.

                                       Los In dieser Spalte wird die Losnummer der im Lauf enthaltenen Lose ange-
                                       zeigt.

                                       Stk In dieser Spalte sehen Sie, wie viele Einheiten zu produzieren sind. Eine
                                       Einheit besteht aus mindestens zwei Scheiben.

                                       Text In dieser Spalte wird Ihnen die Glasbezeichnung angezeigt. Die Glasbe-
                                       zeichnung kommt aus den Stammdaten.

                                       Sperre Sollten Scheiben eines Laufes bereits von einer anderen Maschine
                                       bearbeitet werden, sehen Sie in dieser Spalte den Namen der Maschine. Die-
                                       se Scheiben sind dann zur Bearbeitung an Ihrer Maschine gesperrt.

                                       Gestell In dieser Spalte sehen Sie, auf welchem logischen Gestell (Gestell-
                                       Nummer) sich die Scheiben befinden.

                                       Glasart In dieser Spalte wird Ihnen die Glasbezeichnung angezeigt.

                                       Teile In dieser Spalte wird Ihnen die Anzahl der Scheiben angezeigt.

                                       Erläuterung der Schaltflächen

                                       Alle anzeigen Wenn Sie diese Schaltfläche betätigen, löschen Sie den Filter
                                       zur Anzeige der Läufe. Es werden dann alle anstehenden Läufe angezeigt.

                                       Lauf entfernen Diese Schaltfläche entfernt alte, überflüssige Läufe, die nicht
                                       mehr produziert werden müssen.

                                       Aktualisieren Wenn Sie diese Schaltfläche betätigen, wird der Dialog aktua-
                                       lisiert.

                                       Laden Wenn Sie diese Schaltfläche betätigen, wird der gewählte Lauf gela-
                                       den.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen. Es wird kein Lauf geladen.


                                       Ergänzende Informationen
                                        Tutorial, “Ein Los laden” auf Seite 25
1.50 / 01-2023




                 Production Terminal                                                                            137
                 Übersicht Terminal IG                                                                Softwarereferenz




                                         Bruch buchen
                                         ToolTV IG-In > Einheit markieren > [Bruch]
                                         oder über die Funktionstaste
                                         F7




                                         Abb. 29       Bruch buchen


                                         Mit diesem Dialog wird die markierte Scheibe auf Bruch gesetzt. Wenn mit au-
                                         tomatischen Nachläufern gearbeitet wird, dann werden für alle Teile der Ein-
                                         heit entsprechende Nachläufer angestoßen.

                                         Erläuterung der Felder

                                         Einheit Barcodenummer der Einheit, für die Bruch gemeldet werden soll.

                                         Bruchgründe Liste der auswählbaren Bruchgründe. Die verfügbaren Bruch-
                                         gründe müssen bei der Konfiguration des Systems definiert werden. Mögliche
                                         Gründe können sein:
                                         • Bruch
                                         • Mangel
                                         • Kratzer
                                         • Maß falsch
                                         • Falsche Glasart
                                         • MA-Kratzer
                                         • Teilebruch

                                              Automatische Nachläufer
1.50 / 01-2023




                                              Für einige Bruchtypen werden Nachläufer automatisch generiert. Dies wird
                                              bei der Konfiguration entsprechend eingestellt. Der Mitarbeiter an der Ma-
                                              schine muss mit diesen Modalitäten vertraut sein.


                 138                                                                               Production Terminal
                 Softwarereferenz                                                                 Übersicht Terminal IG




                                       Erläuterung der Schaltflächen

                                       OK Wenn Sie diese Schaltfläche betätigen, wird der gewählte Bruchgrund
                                       übernommen.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen. Der zugewiesene Bruchgrund wird nicht übernommen.


                                       Ergänzende Informationen
                                        Tutorial, “Umgang mit beschädigten Scheiben” auf Seite 28
                                        Tutorial, “So verfahren Sie mit beschädigten Scheiben” auf Seite 28
1.50 / 01-2023




                 Production Terminal                                                                              139
                 Übersicht Terminal IG                                                            Softwarereferenz




                                         Nachläufer laden
                                         ToolTV IG-In > [Nachläufer]
                                         oder über die Funktionstaste
                                         F8




                                         Abb. 30     Nachläufer laden


                                         In diesem Dialog können Sie Nachläufer laden. Geben Sie zunächst die Eti-
                                         kettnummer manuell oder via Scanner ein. Sie können auch mehrere Etikett-
                                         nummern hinter einander eingeben.

                                         Erläuterung der Felder

                                         Barcode In diesem Feld geben Sie die Etikettnummer des Nachläufers ein
                                         oder scannen ein Etikett.

                                         Übernehmen [F2] Nachdem Sie die Etikettnummer eingegeben oder ge-
                                         scannt haben, betätigen Sie diese Schaltfläche. Die entsprechenden Daten
                                         werden im Feld darunter angezeigt.

                                         Auftrag In diesem Feld sehen Sie die Auftragsnummer für den Nachläufer.

                                         Pos In diesem Feld sehen Sie die Positionsnummer für den Nachläufer.

                                         Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.
1.50 / 01-2023




                 140                                                                           Production Terminal
                 Softwarereferenz                                                           Übersicht Terminal IG




                                       Erläuterung der Schaltflächen

                                       Laden Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlossen
                                       und der gewählte Nachläufer wird geladen.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen. Der Nachläufer wird nicht geladen.


                                       Ergänzende Informationen
                                        Tutorial, “So laden Sie Nachläufer” auf Seite 30
                                        Tutorial, “Einen Nachläufer laden” auf Seite 30
1.50 / 01-2023




                 Production Terminal                                                                          141
                 Übersicht Terminal IG                                                                  Softwarereferenz




                                         Status
                                         Maschine > Maschinenstatus




                                         Abb. 31      Status


                                         Die Grundlage für aussagekräftige Auswertungen der Maschinendaten ist
                                         eine korrekte Zustandserfassung dieser Maschinen.
                                         Tritt an der Maschine ein Fehler auf, fehlt Personal, müssen Wartungsarbeiten
                                         durchgeführt oder kann der Produktivbetrieb wieder aufgenommen werden,
                                         so muss dieser neue Zustand jeweils dokumentiert werden.

                                         Erläuterung der Felder

                                         Nr. In diesem Feld werden Ihnen die Zustandsnummer angezeigt. Die mögli-
                                         chen Zustände müssen konfiguriert werden.

                                         Name In diesem Feld werden Ihnen die Zustandsnamen angezeigt. Die mög-
                                         lichen Zustände müssen konfiguriert werden.


                                         Ergänzende Informationen
                                          Tutorial, “So ändern Sie den Maschinenstatus” auf Seite 26
1.50 / 01-2023




                 142                                                                                Production Terminal
                 Softwarereferenz                                                           Übersicht Terminal IG




                                       Nachläufer-Verwaltung
                                       Extras > Nachläufer-Verwaltung




                                       Abb. 32     Nachläufer-Verwaltung


                                       In diesem Dialog werden Ihnen die Nachläuferpositionen angezeigt, für die
                                       noch entschieden werden muss, wie sie wieder in die Produktion eingesteuert
                                       werden sollen und welche Teile ggf. wiederzuverwenden sind. Für eine solche
                                       Nachläuferposition wurde eine Zustandsbuchung vom Typ Teilebruch erzeugt.

                                       Erläuterung der Felder im Bereich Übersicht

                                       BT In diesem Feld wird Ihnen angezeigt, ob es sich bei dem Teil um ein Be-
                                       stellteil handelt. In diesem Fall erscheint in dem Feld ein blauer Punkt.

                                       Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                       Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                                       Pos. In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

                                       PPos. In diesem Feld wird Ihnen die Produktionspositionsnummer angezeigt.

                                       Teil In diesem Feld wird Ihnen die Teilenummer angezeigt.

                                       Bezeichnung In diesem Feld wird Ihnen die Teilebezeichnung angezeigt.
1.50 / 01-2023




                                       Name In diesem Feld wird Ihnen der Bruchgrund angezeigt.



                 Production Terminal                                                                         143
                 Übersicht Terminal IG                                                                 Softwarereferenz




                                         Buchungszeit In diesem Feld wird Ihnen angezeigt, wann die Buchung statt-
                                         gefunden hat.

                                         Erfassungsstelle In diesem Feld wird Ihnen die Erfassungsstelle angezeigt,
                                         an der der Bruch entstanden ist.

                                         Info In diesem Feld wird Ihnen der Info-Text angezeigt, der erfasst wurde.

                                         Mitarbeiter In diesem Feld wird Ihnen der Mitarbeiter angezeigt, der den
                                         Bruch gebucht hat.

                                         Erläuterung der Schaltflächen

                                         Umbuchen Wenn Sie diese Schaltfläche betätigen, können Sie der Scheibe
                                         einen anderen Bruchgrund zuweisen und eine zusätzliche Information erfas-
                                         sen.

                                         Wiederverwendung Wenn Sie diese Schaltfläche betätigen, kann das kom-
                                         plette Teil noch weiter verwendet werden. D. h., das Teil erhält die Beschaf-
                                         fungsart Wiederverwenden und verschwindet aus der Anzeige.

                                         AV-Nachläufer Wenn Sie diese Schaltfläche betätigen, wird für das Teil eine
                                         komplett neue Produktionsposition im Auftragspool mit den ursprünglichen
                                         Beschaffungsarten erzeugt. Die alte Produktionsposition wird mengenmäßig
                                         entsprechend reduziert, sodass die Gesamtmenge der Auftragsposition wie-
                                         der stimmt.

                                         Direkte Nachfertigung Wenn Sie diese Schaltfläche betätigen, wird für das
                                         Teil eine direkte Nachfertigung ausgelöst. D. h. es wird für das Teil ein Eintrag
                                         im Bruchpool (globales Bruchmanagement) erzeugt, so dass die Scheibe au-
                                         tomatisch nachgeschnitten werden kann.

                                         Erläuterung der Kombobox

                                         Filter Über diese Kombobox haben Sie die Möglichkeit, die angezeigten Da-
                                         ten nach einzelnen Zuständen in der Nachläufer-Verwaltung zu filtern.

                                         Erläuterung der Felder im Bereich Details
                                         Selektieren Sie im Bereich Übersicht eine Scheibe, wird Ihnen hier die gesam-
                                         te Stückliste unterhalb der Position angezeigt. Dadurch können Sie auch für
                                         die zugehörigen Teile eine Entscheidung treffen, wie mit ihnen zu verfahren
                                         ist.

                                         Bearbeitet In diesem Feld wird Ihnen angezeigt, ob es sich bei dem Teil um
                                         ein Bestellteil handelt. In diesem Fall erscheint in dem Feld ein blauer Punkt.

                                         BT In diesem Feld wird Ihnen angezeigt, ob es sich bei dem Teil um ein Be-
                                         stellteil handelt. In diesem Fall erscheint in dem Feld ein blauer Punkt.
1.50 / 01-2023




                                         Beschaffungsart In diesem Feld wird Ihnen die Beschaffungsart angezeigt.




                 144                                                                                Production Terminal
                 Softwarereferenz                                                                Übersicht Terminal IG




                                       AV-Nachläufer Wenn diese Checkbox aktiviert ist, wird eine neue Produkti-
                                       onsposition im Auftragspool erzeugt.

                                       ES In diesem Feld wird Ihnen die Erfassungsstelle angezeigt, auf die die
                                       Scheibe gebucht werden soll.

                                       Gestell In diesem Feld wird Ihnen der Name des Gestells angezeigt, auf den
                                       die Scheibe gebucht werden soll.

                                       Name In diesem Feld wird Ihnen der Bruchgrund angezeigt.

                                       Fehlerort In diesem Feld wird Ihnen der Fehlerort angezeigt, wenn dieser
                                       ausgewählt wurde.

                                       Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                       Teil In diesem Feld wird Ihnen die Teilenummer angezeigt.

                                       Bezeichnung In diesem Feld wird Ihnen die Teilebezeichnung angezeigt.

                                       Lauf In diesem Feld wird Ihnen die Laufnummer angezeigt.

                                       Prod.-Termin In diesem Feld wird Ihnen der Produktionstermin angezeigt.

                                       Erläuterung der Schaltflächen

                                       Aktualisieren Wenn Sie diese Schaltfläche betätigen, wird der Bildschirm
                                       aufgefrischt. Es ist auch möglich, in den Parametern eine Zeit einzustellen,
                                       nach der der Bildschirm automatisch aufgefrischt wird.

                                       Bearbeiten Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog Be-
                                       arbeiten, für das Stücklistenelement, das Sie im Bereich Details ausgewählt
                                       haben.

                                       Zurück Wenn Sie diese Schaltfläche betätigen, wird die zuletzt durchgeführ-
                                       te Aktion rückgängig gemacht.

                                       Alles zurück Wenn Sie diese Schaltfläche betätigen, werden alle Aktionen,
                                       die Sie an dem Teil vorgenommen haben, rückgängig gemacht.

                                       Speichern Wenn Sie diese Schaltfläche betätigen, wird die eigentliche Bu-
                                       chung gemäß den vorgenommenen Einstellungen ausgeführt. D. h., so lange,
                                       wie Sie diese Schaltfläche noch nicht gedrückt haben, wurde nichts in die Da-
                                       tenbank geschrieben und Sie können noch Aktionen rückgängig machen.

                                       Schließen Wenn Sie diese Schaltfläche betätigen, wird der Dialog beendet.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Nachläufer-Verwaltung - Bearbeiten” auf Seite 146
1.50 / 01-2023




                                        Tutorial, “Nachläufer-Verwaltung” auf Seite 44




                 Production Terminal                                                                             145
                 Übersicht Terminal IG                                                               Softwarereferenz




                                         Nachläufer-Verwaltung - Bearbeiten
                                         Extras > Nachläufer-Verwaltung > [Bearbeiten]




                                         Abb. 33     Nachläufer-Verwaltung - Bearbeiten


                                         In diesem Dialog können Sie die genauen Einstellungen für jedes einzelne Teil
                                         vornehmen.

                                         Erläuterung der Felder

                                         Beschaffungsart In diesem Feld können Sie über die Kombobox die Be-
                                         schaffungsart des gewählten Teils ändern. Sie können zwischen der ursprüng-
                                         lichen Beschaffungsart und Beschaffungsart Wiederverwendung wählen.
                                         Wählen Sie Wiederverwendung, dann werden die darunter liegenden Felder
                                         Erfassungsstelle und Gestell zur Bearbeitung freigegeben.

                                         Erfassungsstelle Wenn das Teil wieder verwendet werden kann, wählen Sie
                                         hier den Ort, wo Sie das Teil bis zur Wiederverwendung abstellen. Diese In-
                                         formation kann in den Production Terminals angezeigt werden.

                                         Gestell Wenn das Teil wieder verwendet werden kann, können Sie hier zu-
                                         sätzlich zur Erfassungsstelle noch das Gestell angeben, auf dem das wieder
                                         verwendbare Teil steht. Diese Information wird z. B. bei der Nachproduktion
                                         des gesamten ISOs am A+W Production Terminal IG-In anstelle der logischen
                                         Gestellnummer angezeigt.
1.50 / 01-2023




                 146                                                                             Production Terminal
                 Softwarereferenz                                                              Übersicht Terminal IG




                                       Fehlergrund Wenn das Teil nicht wieder verwendet werden kann und die Be-
                                       schaffungsart Produktion gewählt wurde, dann können Sie hier den wirklichen
                                       Bruchgrund auswählen. Dieser kann dann später für statistische Auswertun-
                                       gen genutzt werden.

                                       Fehlerort Zusätzlich zum Bruchgrund können Sie hier noch einen Fehlerort
                                       angeben. Dieser ist, unabhängig von der Erfassungsstelle, an der der Bruch
                                       passiert ist, wählbar.

                                       AV-Nachläufer Wenn Sie diese Checkbox aktivieren, wird eine neue Produk-
                                       tionsposition im Auftragspool erzeugt.

                                       Erläuterung der Felder im Bereich Bearbeitungen
                                       In diesem Bereich werden alle Bearbeitungen angezeigt, die an der betroffe-
                                       nen Scheibe schon gebucht wurden.

                                       Wiederholen Durch setzen der Haken in dieser Spalte, werden die Bearbei-
                                       tungen so zurückgesetzt, dass man sie erneut buchen kann.

                                       Artikel In diesem Feld wird Ihnen die Artikelnummer angezeigt.

                                       BearbNr In diesem Feld wird Ihnen die Bearbeitungsnummer angezeigt.

                                       Bearbeitung In diesem Feld wird Ihnen der Name der Bearbeitung ange-
                                       zeigt.

                                       Erläuterung der Felder im Bereich Mögliche Teile
                                       In diesem Bereich werden Ihnen alle Teile angezeigt, die für das ausgewählte
                                       Teil in Frage kommen. D. h., Sie müssen aus dieser Liste eine Etikettnummer
                                       auswählen, die mit dem Nachläufer als Gegenscheibe zusammen laufen soll.
                                       Idealerweise verwendet man hier eine Etikettnummer, die sich noch nicht in
                                       der Produktion befindet. Ist dies nicht möglich, muss die ausgewählte Etikett-
                                       nummer aus der Produktion entfernt werden, damit eine versehentliche Ver-
                                       wendung dieser Etikettnummer vermieden wird. Die Zuweisung einer
                                       Etikettnummer ist nur erforderlich, wenn die Teile nicht vorher schon zusam-
                                       mengebaut waren, in diesem Fall sind bereits eindeutige Etikettnummern zu-
                                       gewiesen.

                                       Auswählen Durch setzen der Haken in dieser Spalte, werden genau diese
                                       Bearbeitungen in den Tabellen so zurückgesetzt, dass man sie erneut buchen
                                       kann.

                                       Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                       Erfassungsstelle In diesem Feld wird Ihnen die Erfassungsstelle angezeigt.

                                       Gestell In diesem Feld wird Ihnen der Gestellname angezeigt.
1.50 / 01-2023




                                       Lauf In diesem Feld wird Ihnen die Laufnummer angezeigt.




                 Production Terminal                                                                            147
                 Übersicht Terminal IG                                                                  Softwarereferenz




                                         Letzte Buchung In diesem Feld wird Ihnen angezeigt, wann die letzte Bu-
                                         chung durchgeführt wurde.

                                         Status In diesem Feld wird Ihnen der Status angezeigt.

                                         Bezeichnung In diesem Feld wird Ihnen die Artikelbezeichnung angezeigt.


                                         Ergänzende Informationen
                                          Softwarereferenz, “Nachläufer-Verwaltung” auf Seite 143
                                          Tutorial, “Nachläufer-Verwaltung” auf Seite 44
1.50 / 01-2023




                 148                                                                                 Production Terminal
                 Softwarereferenz                                                  Übersicht Terminal Manual Cutting




                                       Übersicht Terminal Manual
                                       Cutting
                                       Terminal Manual Cutting zeigt Ihnen alle freigegebenen Läufe bzw. Lose für
                                       einen bestimmten Zuschnitttisch. Bei dem Zuschnitttisch handelt es sich in der
                                       Regel um einen Handzuschnitttisch. Sofern Sie keinen Maschinencode am
                                       Tisch erzeugen müssen, kann das Terminal Manual Cutting auch an einem
                                       anderen Tisch installiert sein.
                                       Die Menüs von Terminal Manual Cutting sind identisch mit den Menüs von Ter-
                                       minal IG-In und werden an dieser Stelle nicht noch einmal beschrieben.
                                        “Übersicht Terminal IG” auf Seite 1-130
1.50 / 01-2023




                 Production Terminal                                                                            149
                 Übersicht Terminal Manual Cutting                                                  Softwarereferenz




                                         Freigabe
                                         JobTV Handzuschnitt > Lauf markieren > Schaltfläche [Freigabe]



                  A




                  B                                                                                              E
                  C




                                                                                                                 F
                  D


                 A Auswahl                             C Modell-Skizze            E Gestell
                 B Modellanzeige                       D Selektiert von Gesamt    F Schaltflächen
                 Abb. 34     Freigabe


                                         Dieser Dialog zeigt Ihnen die Scheiben an, die Sie zuvor im Terminal Manual
                                         Cutting ausgewählt haben. Sie können alle Scheiben auf einmal buchen oder
                                         aber einzelnen Scheiben. Wenn der Dialog geöffnet wird, sind standardmäßig
                                         alle Scheiben selektiert. Um eine einzelne Scheibe zu buchen, markieren Sie
                                         diese in der Tabelle.

                                         Erläuterung der Felder im Bereich A

                                         Lauf In diesem Feld wird Ihnen die Laufnummer angezeigt.

                                         Los In diesem Feld wird Ihnen die Losnummer angezeigt.

                                         Glasart In diesem Feld wird Ihnen die Glasart angezeigt.

                                         Barcode In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                         Bock In diesem Feld wird Ihnen die Gestellnummer angezeigt.

                                         Fach In diesem Feld wird Ihnen die Fachnummer angezeigt.

                                         Pr.-Nr. In diesem Feld wird Ihnen die Produktionsnummer angezeigt.

                                         Modell In diesem Feld wird Ihnen die Modellnummer angezeigt.
1.50 / 01-2023




                                         ZS-Breite In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.




                 150                                                                            Production Terminal
                 Softwarereferenz                                                   Übersicht Terminal Manual Cutting




                                       ZS-Höhe In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.

                                       Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                                       Pos. In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

                                       Erläuterung der Felder im Bereich B
                                       In diesem Bereich befindet sich die Modellanzeige.

                                       Erläuterung der Felder im Bereich C
                                       In diesem Bereich sehen Sie die Modellskizze.
                                       Die Tabelle daneben zeigt Ihnen die entsprechenden Werte. Folgende Werte
                                       sind möglich:
                                       • W = Breite
                                       • H = Höhe
                                       • T1, T2, … = Bruchrand
                                       • <-> = Spiegelkennzeichen
                                       • @ = Drehkennzeichen

                                       Erläuterung der Felder im Bereich D
                                       In diesem Bereich sehen Sie, wie viele Scheiben Sie in der Tabelle markiert
                                       haben und die Gesamtstückzahl. Bsp.: 1/64 bedeutet, dass 64 Scheiben in der
                                       Tabelle angezeigt werden und Sie 1 Scheibe davon markiert haben.

                                       Erläuterung der Felder im Bereich E
                                       In diesem Bereich befinden sich die Daten zum Gestell. Sie können die Ge-
                                       stellnummer eingeben oder aber scannen. Wenn das Gestell leer ist, aktivie-
                                       ren Sie die Checkbox Beginn.

                                       Erläuterung der Schaltflächen

                                       Produzieren Wenn Sie diese Schaltfläche betätigen, wird die markierte
                                       Scheibe gebucht.

                                       Eti Druck Wenn Sie diese Schaltfläche betätigen, wird für die markierte
                                       Scheibe ein Etikett gedruckt.

                                       Bruch Wenn Sie diese Schaltfläche betätigen, wird die markierte Scheibe als
                                       Bruch gebucht.


                                       Ergänzende Informationen
                                        Tutorial, “Arbeiten mit Terminal Manual Cutting” auf Seite 50
                                        Tutorial, “So buchen Sie die ausgewählte(n) Scheibe(n)” auf Seite 59
1.50 / 01-2023




                 Production Terminal                                                                             151
                 Übersicht Terminal Manual Cutting                                                  Softwarereferenz




                                         Bruchpool
                                         JobTV Handzuschnitt > Schaltfläche [Bruchpool]



                 A




                 B                                                                                            E
                 C




                                                                                                              F
                 D




                 A Auswahl                             C Modell-Skizze            E Gestell
                 B Modellanzeige                       D Selektiert von Gesamt    F Schaltflächen
                 Abb. 35     Bruchpool


                                         Mit diesem Instrument haben Sie die Möglichkeit, auf zu Bruch gegangene
                                         Scheiben schnell reagieren zu können. Wird irgendwo in der Produktion eine
                                         Scheibe als Bruch gescannt, öffnet sich der Dialog Bruchpool automatisch.
                                         Die zu Bruch gegangene Scheibe ist dann im Bruchpool enthalten und kann
                                         sofort nachgeschnitten werden (ohne über die Hauttische zu laufen).

                                         Erläuterung der Felder im Bereich A

                                         Artikel In diesem Feld wird Ihnen die Artikelnummer angezeigt.

                                         Bezeichnung In diesem Feld wird Ihnen die Glasart angezeigt.

                                         Glasart In diesem Feld wird Ihnen die Glasart angezeigt.

                                         Dicke In diesem Feld wird Ihnen die Dicke der Scheibe angezeigt.

                                         Breite In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.
1.50 / 01-2023




                                         Höhe In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.



                 152                                                                            Production Terminal
                 Softwarereferenz                                                   Übersicht Terminal Manual Cutting




                                       Lauf In diesem Feld wird Ihnen die Laufnummer angezeigt.

                                       Kunde In diesem Feld wird Ihnen der Kundenname angezeigt.

                                       Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                                       Pos. In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

                                       Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                       Modell In diesem Feld wird Ihnen die Modellnummer angezeigt.

                                       Bock In diesem Feld wird Ihnen die Gestellnummer angezeigt.

                                       Liefertermin In diesem Feld wird Ihnen der Liefertermin angezeigt.

                                       Erläuterung der Schaltflächen

                                       Aktualisieren Wenn Sie diese Schaltfläche betätigen, wird die Anzeige aktu-
                                       alisiert.

                                       Hinzufügen Wenn Sie diese Schaltfläche betätigen, wird der Dialog Brucher-
                                       fassung geöffnet.

                                       Löschen Wenn Sie diese Schaltfläche betätigen, wird die markierte Scheibe
                                       gelöscht.

                                       Drucken/Drucken2 Diese Schaltflächen werden vor Ort angepasst und die-
                                       nen dem Drucken von Etiketten oder Reports.

                                       BDE buchen Wenn Sie diese Schaltfläche betätigen, wird die markierte
                                       Scheibe gebucht.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen.

                                          Automatische Aktualisierung
                                          Der Bruchpoool aktualisiert sich automatisch alle x Sekunden. Dieser Wert
                                          ist einstellbar.


                                       Ergänzende Informationen
                                        Tutorial, “Arbeiten mit Terminal Manual Cutting” auf Seite 50
                                        Tutorial, “So buchen Sie die ausgewählte(n) Scheibe(n)” auf Seite 59
1.50 / 01-2023




                 Production Terminal                                                                            153
                 Übersicht Terminal Manual Cutting                                                  Softwarereferenz




                                         Brucherfassung
                                         JobTV Handzuschnitt > Schaltfläche [Bruchpool] > Schaltfläche [Hinzufügen]




                                         Abb. 36     Brucherfassung


                                         Mit dem Dialog Brucherfassung besteht die Möglichkeit, Brüche manuell dem
                                         Bruchpool hinzuzufügen.

                                         Erläuterung der Felder im Bereich Kunde

                                         Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                                         Position In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

                                         Erläuterung der Felder im Bereich Teile

                                         Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.

                                         Pos In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

                                         Teilenummer In diesem Feld wird Ihnen die Teilenummer angezeigt.

                                         Glasart In diesem Feld wird Ihnen die Glasart angezeigt.

                                         Breite In diesem Feld wird Ihnen die Breite der Scheibe angezeigt.

                                         Höhe In diesem Feld wird Ihnen die Höhe der Scheibe angezeigt.
1.50 / 01-2023




                 154                                                                            Production Terminal
                 Softwarereferenz                                                    Übersicht Terminal Manual Cutting




                                       Erläuterung der Felder im Bereich Bruchgrund
                                       Wählen Sie aus der Kombobox den entsprechenden Bruchgrund aus.

                                       Erläuterung der Felder im Bereich Barcodes

                                       Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                       ES In diesem Feld wird Ihnen die Erfassungsstelle angezeigt.

                                       Gestell In diesem Feld wird Ihnen die Gestellnummer angezeigt.


                                       Ergänzende Informationen
                                        Tutorial, “Arbeiten mit Terminal Manual Cutting” auf Seite 50
                                        Tutorial, “So fügen Sie einen Bruch manuell hinzu” auf Seite 59
1.50 / 01-2023




                 Production Terminal                                                                             155
                 Übersicht Terminal Georgian Bars                                                  Softwarereferenz




                                         Übersicht Terminal Georgian
                                         Bars
                                         Terminal Georgian Bars zeigt Ihnen alle freigegebenen Läufe bzw. Lose für
                                         den Sprossenbau.
                                         Die Menüs von Terminal Georgian Bars sind identisch mit den Menüs von Ter-
                                         minal IG-In und werden an dieser Stelle nicht noch einmal beschrieben.
                                          “Übersicht Terminal IG” auf Seite 1-130
1.50 / 01-2023




                 156                                                                           Production Terminal
                 Softwarereferenz                                                   Übersicht Terminal Georgian Bars




                                         Sprossen-Freigabe
                                         Terminal Georgian Bars > Lauf markieren > Schaltfläche [Freigabe]




                 A




                                                                                                                D




                 B

                                                                                                                E
                 C

                 A Auswahl                              C Selektiert von Gesamt     E Schaltflächen
                 B Gestell                              D Sprossenbild
                 Abb. 37     Sprossen-Freigabe


                                         Dieser Dialog zeigt Ihnen die Sprossen an, die Sie zuvor im Terminal Georgain
                                         Bars ausgewählt haben. Sie können alle Sprossen auf einmal buchen oder
                                         aber einzelne Sprossen. Wenn der Dialog geöffnet wird, sind standardmäßig
                                         alle Sprossen selektiert. Um eine einzelne Sprossen zu buchen, markieren Sie
                                         diese in der Tabelle.

                                         Erläuterung der Felder im Bereich A

                                         Lauf In diesem Feld wird Ihnen die Laufnummer angezeigt.

                                         Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                         Bezeichnung In diesem Feld wird Ihnen die Sprossenbezeichnung ange-
                                         zeigt.

                                         Auftrag In diesem Feld wird Ihnen die Auftragsnummer angezeigt.
1.50 / 01-2023




                                         Pos. In diesem Feld wird Ihnen die Auftragspositionsnummer angezeigt.

                                         PPos. In diesem Feld wird Ihnen die Produktionspositionsnummer angezeigt.


                 Production Terminal                                                                                157
                 Übersicht Terminal Georgian Bars                                                        Softwarereferenz




                                         Termin In diesem Feld wird Ihnen die Produktionstermin angezeigt.

                                         Modell In diesem Feld wird Ihnen die Modellnummer angezeigt.

                                         Breite In diesem Feld wird Ihnen die Breite des Modells (umschreibendes
                                         Rechteck) angezeigt.

                                         Höhe In diesem Feld wird Ihnen die Höhe des Modells (umschreibendes
                                         Rechteck) angezeigt.

                                         Erläuterung der Felder im BereichB
                                         In diesem Bereich befinden sich die Daten zum Gestell. Sie können die Ge-
                                         stellnummer eingeben oder aber scannen. Wenn das Gestell leer ist, aktivie-
                                         ren Sie die Checkbox Beginn.

                                         Erläuterung der Felder im Bereich C
                                         In diesem Bereich sehen Sie, wie viele Sprossen Sie in der Tabelle markiert
                                         haben und die Gesamtstückzahl. Bsp.: 1/64 bedeutet, dass 64 Sprossen in der
                                         Tabelle angezeigt werden und Sie 1 Sprosse davon markiert haben.

                                         Erläuterung der Felder im Bereich D
                                         In diesem Bereich befindet sich die Anzeige des Sprossenbildes.

                                         Erläuterung der Schaltflächen

                                         Produzieren Wenn Sie diese Schaltfläche betätigen, wird die markierte
                                         Sprosse gebucht.

                                         Drucken Wenn Sie diese Schaltfläche betätigen, können Sie das Sprossen-
                                         bild auf einem lokalen Drucker ausdrucken.

                                         Bruch Wenn Sie diese Schaltfläche betätigen, wird die markierte Sprosse als
                                         Bruch gebucht.


                                         Ergänzende Informationen
                                          Tutorial, “Arbeiten mit Terminal Georgian Bars” auf Seite 62
                                          Tutorial, “So buchen Sie die ausgewählte(n) Sprosse(n)” auf Seite 68
1.50 / 01-2023




                 158                                                                                 Production Terminal
                 Softwarereferenz                                                          Übersicht Terminal Order




                                       Übersicht Terminal Order
                                       Mit Terminal Order haben Sie die Möglichkeit größere Mengen zu verbuchen.
                                       Bearbeitungen, die mit der jeweiligen Erfassungsstelle verknüpft sind, werden
                                       dabei mit gebucht.
                                       Die Menüs von Terminal Order sind identisch mit den Menüs von Terminal IG
                                       und werden an dieser Stelle nicht noch einmal beschrieben.
                                        “Übersicht Terminal IG” auf Seite 1-130
1.50 / 01-2023




                 Production Terminal                                                                            159
                 Übersicht Terminal Processing                                                      Softwarereferenz




                                         Übersicht Terminal Proces-
                                         sing
                                         Terminal Processing ist ein Leitrechner, der an Bearbeitungsmaschinen zum
                                         Einsatz kommt. Terminal Processing gibt Ihnen detaillierte Auskunft über die
                                         durchzuführenden Bearbeitungen inklusive maßstabgetreuer Produktions-
                                         zeichnungen.
                                         Die Menüs von Terminal Processing sind identisch mit den Menüs von Termi-
                                         nal IG und werden an dieser Stelle nicht noch einmal beschrieben.
                                          “Übersicht Terminal IG” auf Seite 1-130
1.50 / 01-2023




                 160                                                                             Production Terminal
                 Softwarereferenz                                                         Übersicht Terminal Processing




                                       Manuelle Eingabe
                                       Extras > Barcode




                                       Abb. 38       Manuelle Eingabe


                                       Mit diesem Dialog haben Sie die Möglichkeit, eine weitere Scheibe zu laden.
                                       Geben Sie im Feld Barcode die gewünschte Etikett-Nummer ein oder scannen
                                       Sie den Barcode. Anschließend betätigen Sie die Schaltfläche [OK].
                                       Der Dialog wird geschlossen. Sie sind jetzt wieder im Hauptfenster. Die gela-
                                       dene Scheibe wird am Ende der Übersicht angezeigt.


                                       Ergänzende Informationen
                                        Tutorial, “Arbeiten mit Terminal Processing” auf Seite 79
                                        Tutorial, “So scannen Sie ein Etikett” auf Seite 84
1.50 / 01-2023




                 Production Terminal                                                                              161
                 Übersicht Terminal TG                                                             Softwarereferenz




                                         Übersicht Terminal TG
                                         Terminal TG kommt an ESG-Öfen zum Einsatz und unterstützt Sie dort bei der
                                         Be- und Entladung der Ofenbetten.
                                         Die Module Terminal TG-In und Terminal TG-Out haben die gleichen Menüs
                                         wie Terminal IG und werden an dieser Stelle nicht noch einmal beschrieben.
                                          “Übersicht Terminal IG” auf Seite 1-130
1.50 / 01-2023




                 162                                                                           Production Terminal
                 Softwarereferenz                                                               Übersicht Terminal TG




                                       Manuelle Eingabe
                                       ToolTV TG-In > Extras > Barcode




                                       Abb. 39       Manuelle Eingabe


                                       Mit diesem Dialog haben Sie die Möglichkeit, eine weitere Scheibe zu laden.
                                       Geben Sie im Feld Barcode die entsprechende Etikett-Nummer ein und betä-
                                       tigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen und die Etikett-
                                       Nummer wird geladen.


                                       Ergänzende Informationen
                                        Tutorial, “Arbeiten mit Terminal TG-In” auf Seite 89
                                        Tutorial, “So scannen Sie ein Etikett” auf Seite 93
1.50 / 01-2023




                 Production Terminal                                                                            163
                 Übersicht Terminal TG                                                             Softwarereferenz




                                         Offene Bearbeitungen
                                         ToolTV TG-In > Etikettnummer laden




                                         Abb. 40     Brucherfassung


                                         Dieser Dialog erscheint automatisch, wenn es vor dem Härten noch offene Be-
                                         arbeitungen gibt. Dann werden Ihnen diese offenen Bearbeitungen angezeigt
                                         und Sie können entscheiden, wie mit der Scheibe weiter verfahren werden
                                         soll.

                                         Erläuterung der Felder

                                         Etikett In diesem Feld wird Ihnen die Etikettnummer angezeigt.

                                         Auftrag/Pos. In diesem Feld wird Ihnen die Auftrags- sowie die Positions-
                                         nummer angezeigt.

                                         Erläuterung der Tabelle

                                         Fertig In diesem Feld sehen Sie, welche Bearbeitungen noch offen sind.
                                         Mögliche Werte:
                                         • Rotes X: Die Bearbeitung ist noch offen.
                                         • Grüner Hacken: Die Bearbeitung ist gemacht.

                                         Termin In diesem Feld sehen Sie, wann die Bearbeitung durchgeführt wird.

                                         Bearbeitung In diesem Feld wird Ihnen die Bearbeitung angezeigt.
1.50 / 01-2023




                 164                                                                            Production Terminal
                 Softwarereferenz                                                                 Übersicht Terminal TG




                                       Erläuterung der Schaltflächen

                                       Trotzdem laden Diese Schaltfläche müssen Sie verwenden, wenn die Bear-
                                       beitung durchgeführt wurde, jedoch nicht gebucht wurde. Der Dialog wird ge-
                                       schlossen. Sie befinden sich jetzt wieder im Hauptfenster. Die geladene
                                       Scheibe wird in der Übersicht angezeigt.

                                       Schließen Diese Schaltfläche müssen Sie verwenden, wenn die Bearbeitung
                                       wirklich fehlt. Dann wird der Dialog geschlossen, die Scheibe muss noch be-
                                       arbeitet werden.


                                       Ergänzende Informationen
                                        Tutorial, “Arbeiten mit Terminal TG-In” auf Seite 89
                                        Tutorial, “Arbeiten mit Terminal TG-Out” auf Seite 97
                                        Tutorial, “So verfahren Sie mit offenen Bearbeitungen” auf Seite 93
1.50 / 01-2023




                 Production Terminal                                                                              165
                 Übersicht Terminal LG                                                              Softwarereferenz




                                         Übersicht Terminal LG
                                         Terminal LG kommt an der VSG-Linie zum Einsatz und zeigt Ihnen alle verfüg-
                                         baren Lose inklusive produktionsunterstützender Informationen.
                                         Die Module Terminal LG-In und Terminal LG-Assembly haben die gleichen
                                         Menüs wie Terminal IG und werden an dieser Stelle nicht noch einmal be-
                                         schrieben.
                                          “Übersicht Terminal IG” auf Seite 1-130
                                         In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                         •   Menü Datei, Menü-Eintrag Auftrag laden:
                                             Mit diesen Menüpunkt laden Sie einen speziellen Auftrag.
                                              Softwarereferenz, “Registrierung” auf Seite 131
1.50 / 01-2023




                 166                                                                             Production Terminal
                 Softwarereferenz                                                           Übersicht Terminal LG




                                       Auftrag laden
                                       Terminal LG-In > Datei > Auftrag laden




                                       Abb. 41     Auftrag laden


                                       Mit diesem Dialog haben Sie die Möglichkeit, einen bestimmten Auftrag zu la-
                                       den.Über die Radiotasten haben Sie die Möglichkeit, die Anzeige einzu-
                                       schränken.

                                       Erläuterung der Felder

                                       Alle Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben an-
                                       gezeigt.

                                       Verfügbare Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die
                                       Scheiben angezeigt, die zurzeit verfügbar sind.

                                       Geplante Wenn Sie diese Radiotaste aktivieren, werden Ihnen alle Scheiben
                                       angezeigt, die geplant sind.

                                       Mögliche Wenn Sie diese Radiotaste aktivieren, werden Ihnen nur die Schei-
                                       ben angezeigt, deren Bearbeitung möglich ist.

                                       Auftrag In diesem Feld wird Ihnen die Auftrags-Nummer angezeigt.

                                       Pos In diesem Feld wird Ihnen die Positions-Nummer angezeigt.
1.50 / 01-2023




                                       Teil In diesem Feld wird Ihnen die Teile-Nummer angezeigt.

                                       Bezeichnung In diesem Feld wird Ihnen die Teile-Bezeichnung angezeigt.



                 Production Terminal                                                                          167
                 Übersicht Terminal LG                                                                   Softwarereferenz




                                         Lauf In diesem Feld wird Ihnen die Lauf-Nummer angezeigt.

                                         Menge In diesem Feld wird Ihnen die zu produzierende Menge angezeigt.
                                         Die Tabelle darunter enthält detaillierte Informationen zu dem Auftrag, den Sie
                                         oben ausgewählt haben.

                                         Erläuterung der Schaltflächen

                                         Laden Wenn Sie diese Schaltfläche oder die Funktionstaste [F5] betätigen,
                                         wird die Auswahl übernommen.

                                         Abbrechen Wenn Sie diese Schaltfläche oder die Funktionstaste [F6] betäti-
                                         gen, wird der Dialog geschlossen.


                                         Ergänzende Informationen
                                          Tutorial, “Arbeiten mit Terminal LG-In” auf Seite 104
                                          Tutorial, “Arbeiten mit Terminal LG-Assembly” auf Seite 110
1.50 / 01-2023




                 168                                                                                 Production Terminal
                 Softwarereferenz                                                               Übersicht Terminal LG




                                       Gehe zu Produktionsnummer
                                       Datei > Springe zu ProdNr.
                                       oder über die Funktionstaste
                                       F11




                                       Abb. 42      Gehe zu Produktionsnummer


                                       Mit diesem Dialog können Sie eine andere Produktionsnummer laden. Die
                                       Produktionsnummer bestimmt die Reihenfolge der zu produzierenden Einhei-
                                       ten. So können Sie z. B. direkt von der Produktionsnummer 3 auf die Produk-
                                       tionsnummer 15 springen ohne mehrfach die Schaltfläche [Überspringen]
                                       betätigen zu müssen.

                                       Erläuterung der Felder

                                       Produktionsnummer Wählen Sie über die Pfeiltasten die Produktionsnum-
                                       mer aus, die als nächstes produziert werden soll.

                                       Erläuterung der Schaltflächen

                                       OK Wenn Sie diese Schaltfläche betätigen, wird die gewählte Produktions-
                                       nummer übernommen.

                                       Abbrechen Wenn Sie diese Schaltfläche betätigen, wird der Dialog ge-
                                       schlossen. Die gewählte Produktionsnummer wird nicht übernommen.


                                       Ergänzende Informationen
                                        Tutorial, “Eine andere Produktionsnummer laden” auf Seite 29
1.50 / 01-2023




                 Production Terminal                                                                            169
                 Übersicht Terminal Edit                                                              Softwarereferenz




                                           Übersicht Terminal Edit
                                           Terminal Edit bietet die Möglichkeit, fehlende oder falsche Buchungen zu kor-
                                           rigieren und größere Mengen auf einmal zu buchen.
                                           Das Modul hat die gleichen Menüs wie Terminal IG und werden an dieser Stel-
                                           le nicht noch einmal beschrieben.
                                            “Übersicht Terminal IG” auf Seite 1-130
1.50 / 01-2023




                 170                                                                               Production Terminal
                 Softwarereferenz                                                                            Reports




                                       Reports
                                       Menü Listen öffnen
                                       Im Menü Listen befindet sich die auf Kundenwunsch erstellten Reports. In un-
                                       serem Beispiel finden Sie dort den Menüpunkt:
                                       •   Auftragsübersicht:
                                           Über diesen Menüpunkt starten Sie den Report für die Auftragsübersicht.
                                            Softwarereferenz, “Parametereingabe für Report” auf Seite 172
1.50 / 01-2023




                 Production Terminal                                                                            171
                 Reports                                                                      Softwarereferenz




                           Parametereingabe für Report
                           Listen > Auftragsübersicht




                           Abb. 43       Parametereingabe für Report


                           Der Dialog oben zeigt die Parametereingabe für eine Auftragsübersicht. In
                           Terminal gibt es viele unterschiedliche Listen (Reports). Sie werden von A+W
                           für jeden Kunden individuell erstellt und den jeweiligen Anforderungen ange-
                           passt.




                           Abb. 44       Beispielreport Auftragsübersicht


                           Ergänzende Informationen
                            Tutorial, “Listen (Reports) generieren” auf Seite 31
                            Tutorial, “So drucken Sie eine Auftragsübersicht” auf Seite 31
1.50 / 01-2023




                 172                                                                    Production Terminal
                 Softwarereferenz                                                                   Die Hilfe verwenden




                                       Die Hilfe verwenden
                                       Menü ? öffnen
                                       Im Menü ? befinden sich folgende Menüpunkte:
                                       •   Benutzer-Hilfe:
                                           Über diesen Menüpunkt starten Sie die Kurzbeschreibungen.
                                       •   Aktuelle Logeinträge:
                                           Über diesen Menüpunkt starten Sie die Log-Datei. Diese Datei enthält die
                                           Log-Einträge für die jeweilige Sitzung.
                                            Softwarereferenz, “Logeinträge für Sitzung” auf Seite 174
                                       •   Sprache ändern:
                                           Über diesen Menüpunkt können Sie die Modulsprache ändern. Es öffnet
                                           sich der Dialog Sprache ändern.
                                            Softwarereferenz, “Sprachauswahl” auf Seite 175
                                       •   Informationen:
                                           Über diesen Menüpunkt erhalten Sie weitere Informationen zum jeweiligen
                                           Modul.
                                            Softwarereferenz, “Über Production Terminal” auf Seite 176
1.50 / 01-2023




                 Production Terminal                                                                              173
                 Die Hilfe verwenden                                                                   Softwarereferenz




                                       Logeinträge für Sitzung
                                       ? > Aktuelle Logeinträge




                                       Abb. 45       Logeinträge


                                       In diesem Dialog werden Ihnen Details zu der jeweiligen Sitzung angezeigt.
                                       Sie können die Logeinträge in Form einer Text-Datei exportieren. Im Falle ei-
                                       nes Fehlers kann es von Vorteil sein, diese Text-Datei zu Analysezwecken zu
                                       A+W zu schicken.

                                       Erläuterung der Schaltflächen

                                       Aktualisieren Wenn Sie diese Schaltfläche betätigen, aktualisieren Sie die
                                       Anzeige.

                                       Exportieren Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog
                                       Speichern unter … . Sie können die Logeinträge dann als Text-Datei spei-
                                       chern.

                                       Schließen Wenn Sie diese Schaltfläche betätigen, wird der Dialog geschlos-
                                       sen.


                                       Ergänzende Informationen
                                        Tutorial, “So exportieren Sie Log-Einträge” auf Seite 31
1.50 / 01-2023




                 174                                                                                Production Terminal
                 Softwarereferenz                                                                  Die Hilfe verwenden




                                       Sprachauswahl
                                       ? > Sprache ändern




                                       Abb. 46      Sprache ändern


                                       In diesem Dialog wählen Sie die Sprache für das jeweilige Terminal aus. Nach-
                                       dem Sie den Dialog mit der Schaltfläche [OK] verlassen haben, stellt Terminal
                                       die Sprache um.

                                       Erläuterung der Felder

                                       Sprache Wählen Sie aus der Kombobox die gewünschte Sprache aus und
                                       betätigen Sie die Schaltfläche [OK]. Die Sprache wird automatisch umgestellt.
                                       Es ist kein Neustart erforderlich.

                                       Ersatz-Sprache Wählen Sie aus der Kombobox die gewünschte Ersatz-
                                       Sprache aus. Die Ersatz-Sprache kommt dann zum Einsatz, wenn z. B. die
                                       Übersetzung für einen Eintrag fehlt.


                                       Ergänzende Informationen
                                        Tutorial, “So wählen Sie eine andere Sprache aus” auf Seite 32
1.50 / 01-2023




                 Production Terminal                                                                             175
                 Die Hilfe verwenden                                                            Softwarereferenz




                                       Über Production Terminal
                                       ? > Information




                                       Abb. 47     Über ToolTV


                                       In diesem Dialog erhalten Sie weitere Informationen zu den einzelnen Modu-
                                       len, z. B. Version und Release-Stand.
1.50 / 01-2023




                 176                                                                         Production Terminal
Production Terminal


                      Index
                 Index                                                              Index Production Terminal




                 Index Production Terminal
                                                            L
                                                            Laufnummer/Losnummer
                 A                                          – Terminal IG 1-23
                 Abladereihenfolge (Terminal TG-In) 1-99    Liste aktuelle Einheit
                 Ablauf von Arbeitsschritten                – Terminal IG-In 1-21
                 – Terminal Edit 1-121                      Logeinträge exportieren 1-130
                 – Terminal IG-Assembly 1-37                Los laden
                 – Terminal IG-Out 1-43                     – Terminal IG-In 1-25
                 – Terminal LG-Assembly 1-113
                 – Terminal LG-In 1-107                     M
                 – Terminal Manual Cutting 1-58, 1-67       Maschinen
                 – Terminal Order 1-75                      – Maschinenstatus-Dialog 1-130
                 – Terminal Processing 1-84                 Maschinenzustand 1-26
                 – Terminal TG-In 1-93                      Menü Datei
                 – Terminal TG-Out 1-101                    – Auftrag laden 1-166
                 Andere Produktionsnummer laden 1-29        – Charge 1-130
                 Anmelden                                   – Springe zu ProdNr. 1-130
                 – Terminal IG-In 1-24                      – Ummelden 1-130
                                                            – Vorschau-Dialog 1-130
                 B                                          Menüleiste 1-20
                 Beschädigte Scheiben         1-28          Modellanzeige 1-20

                 D                                          N
                 Drucken                                    Nachläufer laden
                 – Auftragsübersicht        1-31            – Terminal IG-In 1-30

                 E                                          O
                 Exportieren                                Oberläche 1-19
                 – Log-Einträge      1-31                   Offene Bearbeitung Terminal TG-In     1-93

                 F                                          P
                 Farbliche Darstellung der Einheit   1-35   Produktionshinweistexte Terminal IG     1-23
                                                            Programmsprache ändern 1-32
                 G
                 Gesamtes Ofenbett buchen (Terminal TG-     S
                 Out) 1-101                                 Schaltflächen allgemein
                                                            – Bruch 1-23
                                                            – Produzieren 1-23
                 H
                                                            Schaltflächen Terminal IG
                 Hilfe starten   1-130
                                                            – Überspringen 1-23
                                                            Schaltflächen Terminal IG-In
                 I                                          – Los Laden 1-23
                 Infofelder   1-22                          Schaltflächen Terminal TG-Out    1-99
                                                            Schaltflächen ToolTV IG-In
                 K                                          – Nachläufer 1-23
1.50 / 01-2023




                 Kontaktadressen      1-4                   Scheibe produzieren
                                                            – Terminal IG-In 1-25
                                                            Sprache ändern 1-130


                 Production Terminal                                                                       179
                 Index Production Terminal                             Index




                 Sprossenansicht Terminal IG   1-23

                 T
                 Terminal Edit
                 – Arbeitsschritte 1-121
                 Terminal IG
                 – Laufnummer/Losnummer 1-23
                 – Produktionshinweistexte 1-23
                 – Produktionsnummer/Bezeichnung 1-20
                 – Sprossenansicht 1-23
                 Terminal IG-In 1-19
                 – Andere Produktionsnummer laden 1-29
                 – Anmelden 1-24
                 – Arbeitsschritte 1-24
                 – Liste der aktuellen Einheit 1-21
                 – Los laden 1-25
                 – Nachläufer laden 1-30
                 – Oberfläche 1-19
                 – Scheibe produzieren 1-25
                 – Vorschauliste 1-22
                 Terminal IG-Out
                 – Arbeitsschritte 1-43
                 Terminal LG-Assembly
                 – Arbeitsschritte 1-113
                 Terminal LG-In
                 – Arbeitsschritte 1-107
                 Terminal Order
                 – Arbeitsschritte 1-75
                 Terminal Processing
                 – Arbeitsschritte 1-84
                 Terminal TG-In
                 – Arbeitsschritte 1-93
                 – Liste Abladereihenfolge 1-99
                 – Offene Bearbeitung 1-93
                 Terminal TG-Out
                 – Arbeitsschritte 1-101
                 – Gesamtes Ofenbett buchen 1-101

                 U
                 Umgang mit
                 – beschädigten Scheiben 1-28
                 – Maschinenzuständen 1-26
                 Urheberrechte 1-4

                 V
                 Verlinkte Dokumente 1-23
                 Vorausgesetzte Kenntnisse 1-10
                 Vorschauliste 1-22
1.50 / 01-2023




                 W
                 Warenzeichen    1-4



                 180                                     Production Terminal
                 Index                 Index Production Terminal
1.50 / 01-2023




                 Production Terminal                       181
                 Index Production Terminal                 Index
1.50 / 01-2023




                 182                         Production Terminal

