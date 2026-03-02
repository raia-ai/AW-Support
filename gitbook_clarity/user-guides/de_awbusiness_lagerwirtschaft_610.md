---
description: "DE AWBusiness Lagerwirtschaft 6.10"
---



# DE AWBusiness Lagerwirtschaft 6.10

Lagerwirtschaft            G




                           deutsch




                  A+W Business
                                                                                                                Vorspann




                                          Vorspann
                                          In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                          Revisionsübersicht
                                          Part            Beschreibung
                                          Version/Datum

                                          6.1/04-2020     Neu: Lagerverwaltung > Kritischer Lagerbestand.

                                          6.0/10-2019     Einstellungen Kistenmanagement in separaten Part übertragen
                                                          und aus Part Lagerwirtschaft gelöscht.

                                          5.2/08-2019     Einstellungen zur Inventurlisten und zum Druck von
                                                          Kistenetiketten neu.

                                          5.10/01-2017    Inventur überarbeitet, Dialog Lagerbewertung neu.

                                          5.00/08-2013    Vollständige Überarbeitung der ALFAK-Dokumentation und
                                                          Anpassung auf A+W Business.

                                          4.12/01-2013    Layout an CI 2013 angepasst.

                                          4.11/02-2012    Korrekturen

                                          4.10/11-2010    Aktualisierung und Umstellung auf Doku-Konzept 2010

                                          4.00/08-2009    Vollständige Überarbeitung

                                          3.02/09-2008    Abbildungen und Part-Nummer angepasst.

                                          3.01/08-2008    Rechtschreibkorrekturen

                                          3.00/12-2003    Struktureller Umbau auf Programmstruktur 4.0

                                          2.00/08-2000    Überarbeitung Lager

                                          1.00/03-1998    Ersterstellung



                                          Editorial
                                          Das Editorial enthält Informationen zu folgenden Themen:
                                          •   Anmerkungen zu diesem Dokument
                                          •   Urheberrechte
                                          •   Warenzeichen
                                          •   Kontakte
5.20 / 04-2020




                 A+W Business Fertigung                                                                             G-3
                 Vorspann




                            Anmerkungen zu diesem Dokument
                            Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business
                            gedacht.
                            Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz
                            vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden.
                            Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
                            ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Tex-
                            ten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem kön-
                            nen Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH
                            übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese
                            beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
                            Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

                            Urheberrechte
                            © 2020, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                            stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                            Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen
                            kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner ande-
                            ren Form übertragen werden. Ohne die vorherige schriftliche Genehmigung
                            von A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
                            nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

                            Warenzeichen
                            Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen kön-
                            nen gleichzeitig auch eingetragene Marken oder sonstige gewerbliche
                            Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

                            Kontakte
                            A+W Software GmbH

                            Am Pfahlgraben 4-10

                            D-35415 Pohlheim

                               +49 6404 2051 0

                               +49 6404 2051 877

                            aw.zentrale@a-w.com

                            http://www.a-w.com
5.20 / 04-2020




                 G-4                                                            A+W Business Fertigung
                                                                                                                                                             Inhalt




                                          Inhalt
                                          Vorspann ............................................................................................................... G-3
                                           Revisionsübersicht ............................................................................................. G-3
                                           Editorial .............................................................................................................. G-3

                                          Tutorial                                                                                                           G-9
                                          Übersicht .............................................................................................................. G-11
                                            Dokumentation ................................................................................................. G-12
                                              Aufbau des Tutorials ..................................................................................... G-12
                                              Darstellungskonventionen ............................................................................. G-13
                                            Menü-Übersicht ................................................................................................ G-14
                                          Grundgedanken zum Lager ................................................................................. G-16
                                          Stammdaten ........................................................................................................ G-19
                                            Lager ................................................................................................................ G-20
                                              Lagerdefinition .............................................................................................. G-21
                                              Lagerkategorien ............................................................................................ G-22
                                              Lagerebenen festlegen ................................................................................. G-22
                                              Lagerort definieren ........................................................................................ G-24
                                              Lagerkategorien festlegen ............................................................................ G-27
                                              Übungen ....................................................................................................... G-28
                                            Firmendaten ..................................................................................................... G-29
                                              Lagerführungsmodus und Reservierung ....................................................... G-30
                                              Firmendaten prüfen ....................................................................................... G-31
                                            Status ............................................................................................................... G-34
                                              Statusänderungen durch Zu- und Abgänge .................................................. G-35
                                              Statuszuordnungen prüfen ............................................................................ G-35
                                            Produktdefinition ............................................................................................... G-38
                                              Produkt .......................................................................................................... G-39
                                              Produkte als Lagerartikel .............................................................................. G-40
                                              Lagermaße .................................................................................................... G-42
                                              Produktstammdaten prüfen ........................................................................... G-44
                                              Lagermaß anlegen ........................................................................................ G-48
                                              Übungen ....................................................................................................... G-50
                                            Preise ............................................................................................................... G-51
                                              Einkaufspreis und Durchschnitts-EK ............................................................ G-52
                                              Einstellung für EK-Ermittlung prüfen ............................................................. G-57
                                              Preise prüfen ................................................................................................. G-58
                                              Übungen ....................................................................................................... G-60
                                            Lagerführung auf Stücklistenebene .................................................................. G-61
                                              Reservierung und Buchung für Stücklisten-Komponenten ........................... G-62
                                              Einstellung prüfen ......................................................................................... G-64
                                              Produkte prüfen ............................................................................................ G-65
                                          Lagerwirtschaft .................................................................................................... G-67
                                            Lagerverwaltung ............................................................................................... G-68
                                              Elemente im Dialog Lagerverwaltung ........................................................... G-69
                                              Lagerartikel ................................................................................................... G-70
                                              Lager-Hauptartikel ........................................................................................ G-70
                                              Mindestmengen ............................................................................................ G-71
                                              Preise ............................................................................................................ G-72
                                              Lagerartikel anlegen ..................................................................................... G-74
                                              Übungen ....................................................................................................... G-77
5.20 / 04-2020




                                            Lagerbuchung .................................................................................................. G-78
                                              Lagerbewegungen ........................................................................................ G-79
                                              Buchungsarten .............................................................................................. G-79
                                              Ab- und Zubuchung ...................................................................................... G-80


                 A+W Business Fertigung                                                                                                                        G-5
                 Inhalt




                              Ab- oder Zugang manuell erfassen ............................................................... G-81
                              Lagerort ändern ............................................................................................ G-85
                              Übungen ....................................................................................................... G-87
                            Abfragen ........................................................................................................... G-88
                              Lagerabfrage ................................................................................................. G-89
                              Buchungsjournal anzeigen ............................................................................ G-90
                              Reservierte Lagerartikel drucken .................................................................. G-92
                              Lagerstatistik anzeigen ................................................................................. G-94
                              Übungen ....................................................................................................... G-96
                            Lagerinformationen .......................................................................................... G-97
                              Lagersuche ................................................................................................... G-98
                              Bestand ......................................................................................................... G-98
                              Lagerinfo und zukünftiger Lagerbestand ...................................................... G-99
                              Bestände in der Lagersuche anzeigen ....................................................... G-102
                              Übungen ..................................................................................................... G-106
                            Lagerbestellung (automatisch) ....................................................................... G-107
                              Bestellvorschläge ........................................................................................ G-108
                              Lagerbestellung an den Einkauf übergeben ............................................... G-109
                              Preise vor der Übergabe vergleichen ......................................................... G-114
                              Übungen ..................................................................................................... G-116
                          Lagerartikel in Dokumenten ............................................................................... G-117
                            Auftragserfassung von Lagerartikeln .............................................................. G-118
                              Reservierung und Buchung von Lagerartikeln ............................................ G-119
                              Lagerartikel für Position suchen .................................................................. G-120
                              Buchungen prüfen ....................................................................................... G-124
                              Übungen ..................................................................................................... G-126
                            Manuelle Lagerbestellung .............................................................................. G-127
                              Lagerbestellung manuell erfassen .............................................................. G-128
                              Übungen ..................................................................................................... G-130
                            Produktionsaufträge ....................................................................................... G-131
                              Lagerartikel im Produktionsauftrag ............................................................. G-132
                              Manuelle Erfassung durch Kopieren ........................................................... G-133
                              Einstellungen in der Lieferantenkartei ......................................................... G-134
                              Bestellmenge nach Bestandsprüfung ......................................................... G-135
                              Lagerzugang durch Produktionsauftrag ...................................................... G-140
                          Inventur .............................................................................................................. G-141
                            Periodische Inventur ....................................................................................... G-142
                              Bestandaufnahme ....................................................................................... G-143
                              Inventurliste erstellen .................................................................................. G-145
                              Sollbestand ermitteln .................................................................................. G-150
                              Inventurwerte erfassen ............................................................................... G-152
                              Inventur abschließen ................................................................................... G-154
                              Nachtragsinventur anhängen ...................................................................... G-156
                              Übungen ..................................................................................................... G-157
                            Erstinventur .................................................................................................... G-158
                              Ablauf für die Erstinventur ........................................................................... G-159
                              Erstinventur durchführen ............................................................................. G-160
                          Übungen ............................................................................................................ G-162

                          Softwarereferenz                                                                                             G-163
                          Übersicht ............................................................................................................ G-165
                          Inventur .............................................................................................................. G-166
                            Inventurliste .................................................................................................... G-167
5.20 / 04-2020




                            Listendruck ..................................................................................................... G-171
                            Sollbestand ..................................................................................................... G-173




                 G-6                                                                                         A+W Business Fertigung
                                                                                                                                                             Inhalt




                                          Inventurverwaltung ............................................................................................ G-175
                                            Menüs in der Inventurverwaltung ................................................................... G-175
                                              Menü Optionen ........................................................................................... G-175
                                              Menü Funktionen ........................................................................................ G-176
                                            Verwaltung ..................................................................................................... G-176
                                            Gehe zu Artikel ............................................................................................... G-179
                                            Wertberichtigung ............................................................................................ G-179
                                          Inventurabschluss .............................................................................................. G-180
                                            Menüs im Inventurabschluss .......................................................................... G-180
                                              Menü Optionen ........................................................................................... G-180
                                              Menü Funktionen ........................................................................................ G-180
                                            Abschluss ....................................................................................................... G-181
                                            Inventurliste wählen ........................................................................................ G-183
                                          Lagerverwaltung ................................................................................................ G-184
                                            Menüs in der Lageverwaltung ........................................................................ G-184
                                              Menü Funktionen ........................................................................................ G-184
                                              Menü Optionen ........................................................................................... G-185
                                              Menü Druck ................................................................................................. G-185
                                            Lagerverwaltung ............................................................................................. G-185
                                              Lagerverwaltung – Lagerartikel ................................................................... G-186
                                              Lagerverwaltung – Preise ........................................................................... G-190
                                              Lagerverwaltung – Zusatz ........................................................................... G-193
                                          Lagerbewegung ................................................................................................. G-195
                                            Menü Optionen ............................................................................................... G-195
                                            Lagerbewegung .............................................................................................. G-195
                                              Lagerbewegung – Abgang, Zugang ............................................................ G-196
                                              Lagerbewegung – Umbuchung ................................................................... G-198
                                              Lagerbewegung – Blattanzahl .................................................................... G-199
                                              Lagerbewegung – Aufbruch ........................................................................ G-200
                                            Bemerkung (Lagerbewegung) ........................................................................ G-201
                                          Abfragen ............................................................................................................ G-202
                                            Buchungsjournal ............................................................................................. G-202
                                            Lagerhistorie ................................................................................................... G-204
                                              Lagerhistorie – Auswahl .............................................................................. G-205
                                              Lagerhistorie – Tabelle ............................................................................... G-208
                                            Lagerstatistik .................................................................................................. G-209
                                              Lagerstatistik – Produkte ............................................................................ G-210
                                              Lagerstatistik – Statistik .............................................................................. G-212
                                              Lagerstatistik – FIFO/LIFO .......................................................................... G-214
                                            Reservierte Lagerartikel ................................................................................. G-215
                                          Suche ................................................................................................................. G-217
                                              Lagersuche – Lagersuche .......................................................................... G-217
                                              Lagersuche – Zukünftiger Lagerbestand .................................................... G-218
                                          Lagerbestellung ................................................................................................. G-220
                                            Menüs im Bestellpool ..................................................................................... G-220
                                              Menü Funktionen ........................................................................................ G-220
                                              Menü Optionen ........................................................................................... G-221
                                            Lagerbestellung .............................................................................................. G-223
                                          Lagerbewertung ................................................................................................. G-226
                                            Lagerbewertung ............................................................................................. G-227
                                              Menü Optionen ........................................................................................... G-227
                                              Lagerbewertung – Selektion ....................................................................... G-228
                                              Lagerbewertung – Bewertung ..................................................................... G-230
5.20 / 04-2020




                                          Partindex                                                                                                    G-233
                                          Index Lagerwirtschaft ......................................................................................... G-235




                 A+W Business Fertigung                                                                                                                        G-7
                 Inhalt
5.20 / 04-2020




                 G-8      A+W Business Fertigung
Lagerwirtschaft              G

                         Tutorial




                  A+W Business
                 Tutorial                                                                                      Übersicht




                                          Übersicht
                                          Das Tutorial zum Modul Lagerwirtschaft beschäftigt sich mit den Grundlagen
                                          der Lagerverwaltung in A+W Business. Das Tutorial baut auf den Kenntnissen
                                          zu den Stammdaten, zum Einkauf und zum Verkauf auf.

                                              Funktionen sind von den freigeschalteten Modulen abhängig
                                              Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                              Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                              liert und freigeschaltet sind.

                                              Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                              on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                              GmbH.

                                          Themenblöcke
                                          In diesem Tutorial finden Sie folgende Themenblöcke:
                                          •   Grundgedanken zum Lager
                                          •   Stammdaten
                                          •   Lagerwirtschaft
                                          •   Lagerartikel in Dokumenten
                                          •   Inventur

                                          Vorausgesetzte Kenntnisse
                                          Das Tutorial richtet sich an Teilnehmer, die in A+W Business den Lagerbe-
                                          stand verwalten. Die Teilnehmer müssen das Konzept der Stammdaten, den
                                          Verkauf und den Einkauf in A+W Business kennen.

                                              Kistenverwaltung im Lager
                                              Die Einstellungen zum Kistenmanagement sind in dem separaten Part Kis-
                                              tenmanagement beschrieben.
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-11
                 Übersicht                                                                              Tutorial




                             Dokumentation
                             Für das Modul Lagerwirtschaft stehen folgende Dokumente zur Verfügung:

                             Format                      Umfang

                             Handout                     Ausdruck des Tutorials für die Schulung

                             PDF                         Vollständige Unterlagen
                                                         • Tutorial
                                                         • Softwarereferenz
                                                         • Index

                             Online-Hilfe <F1>           Kontextsensitive Dialog-Hilfe der A+W Business-
                                                         Softwarereferenz und Tutorials.


                             Aufbau des Tutorials
                             Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten.
                             Jede Lerneinheit besteht aus folgenden Komponenten:

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
5.20 / 04-2020




                 G-12                                                                A+W Business Fertigung
                 Tutorial                                                                                        Übersicht




                                          Darstellungskonventionen
                                          Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                          gende Bedeutung:

                                          Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                                   Software bezeichnen, z. B. der Dialog Lagerinfo.

                                          Fett                     sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                                   Tastatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                                          >                        Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                                   kennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                                   Lagerwirtschaft > Inventur > Abschluss.

                                          []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                   z. B.: Mit [OK] speichern Sie die Daten.

                                          <>                       Spitze Klammern bezeichnen Tasten oder
                                                                   Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                                   öffnen Sie die Online-Hilfe.
5.20 / 04-2020




                 A+W Business Fertigung                                                                              G-13
                 Übersicht                                                                                        Tutorial




                                          Menü-Übersicht
                                          In diesem Abschnitt finden Sie eine kurze Übersicht über die Programm-
                                          bereiche, die in den Themenblöcken dieser Schulung angesprochen werden.




                 Abb. G-1    Menü Lagerwirtschaft


                                          Inventur
                                          In diesem Bereich bereiten Sie die Inventur vor, tragen die gezählten Werte
                                          ein und schließen die Inventur ab.
                                          “Menü Lagerwirtschaft” auf Seite G-14
                                           “Inventur” auf Seite G-141
                                           Softwarereferenz, “Inventur” auf Seite G-166

                                          Lagerverwaltung
                                          In diesem Dialog erfassen und pflegen Sie die Daten für Lagerartikel.
                                           “Lagerverwaltung” auf Seite G-68
                                           Softwarereferenz, “Lagerverwaltung” auf Seite G-184

                                          Lagerbewegung
                                          In diesem Dialog buchen Sie Warenzugänge und Warenabgänge, Änderun-
5.20 / 04-2020




                                          gen von Lagerorten und den Aufbruch von Kisten.
                                           “Lagerbuchung” auf Seite G-78
                                           Softwarereferenz, “Lagerbewegung” auf Seite G-195


                 G-14                                                                             A+W Business Fertigung
                 Tutorial                                                                                  Übersicht




                                          Abfragen
                                          In diesem Bereich lassen Sie sich die Lagerhistorie, Auswertungen und Re-
                                          servierungen anzeigen.
                                           “Abfragen” auf Seite G-88
                                           Softwarereferenz, “Abfragen” auf Seite G-202

                                          Suche
                                          In diesem Dialog prüfen Sie die Verfügbarkeit von Produkten in einem be-
                                          stimmten Zeitraum.
                                           “Lagerinformationen” auf Seite G-97
                                           Softwarereferenz, “Suche” auf Seite G-217

                                          Lagerbestellung
                                          In diesem Dialog übergeben Sie Bestellungen zu Lagerartikeln an den Ein-
                                          kauf.
                                           “Lagerbestellung an den Einkauf übergeben” auf Seite G-109
                                           Softwarereferenz, “Lagerbestellung” auf Seite G-220


                                          Ergänzende Informationen
                                           Überblick, “Elemente des Programmfensters” auf Seite A-52
                                           Verkauf, “Dialog Dokumentenverwaltung” auf Seite C-40
5.20 / 04-2020




                 A+W Business Fertigung                                                                        G-15
                 Grundgedanken zum Lager                                                                         Tutorial




                                      Grundgedanken zum Lager
                                      Im Modul Lagerwirtschaft von A+W Business können Sie Bandmaße, Lager-
                                      maße, Restblätter, Kisten, Ganzglastüren, Beschläge, Rahmenteile und Zube-
                                      hör wie Spiegelaufhängungen, Dichtungsbänder usw. verwalten.
                                      Dabei ist es möglich, die Lagerorganisation Ihres Unternehmens im Pro-
                                      gramm abzubilden. Sie definieren Standorte, Gänge, Regale bis hin zu den
                                      einzelnen Fächern und legen fest, welche Stück-, Quadrat- oder Laufmeterar-
                                      tikel sich an welchem Lagerort befinden.



                                                  Auftrag
                                                                                         Bestellartikel

                                                                           Lager



                                                                       Lagerbestand
                                                                                                     Einkauf
                                                       Lagerartikel
                                                                        Reservierung

                                                                         Disposition

                                                                       Unterdeckung                  Lieferant
                                               Lieferschein
                                                                         Abbuchung
                                               Rechnungen
                                                                      Zugangsbuchung             Wareneingang




                                                                       Auswertungen



                                      Abb. G-2      Übersicht über die Lagerwirtschaft


                                      Alle kaufmännischen Vorgänge in A+W Business basieren auf den Stamm-
                                      daten. Nur wenn diese korrekt gepflegt sind, kann die Verwaltung des Lagers
                                      problemlos abgewickelt werden. Zusammen mit dem Verkauf und dem Ein-
                                      kauf ergeben sich folgende Abläufe:
                                      •    Auftrag:
                                           In einem Auftrag fixieren Sie die Bestellung Ihres Kunden. Dabei erfassen
                                           Sie Positionen, die nach den Angaben des Kunden gefertigt werden müs-
                                           sen.
5.20 / 04-2020




                                      •    Übergabe Produktion:
                                           An die Produktion werden die Auftragspositionen übergeben, die gefertigt
                                           werden müssen.
                                           Die benötigten Materialien werden reserviert und beim Druck von Liefer-

                 G-16                                                                         A+W Business Fertigung
                 Tutorial                                                                       Grundgedanken zum Lager




                                              schein oder Rechnung ausgebucht. Gleichzeitig wird der verfügbare La-
                                              gerbestand aktualisiert.
                                          •   Lagerbestellung:
                                              Wenn der Mindestbestand von Lagerartikeln unterschritten wird, müssen
                                              diese Lagerartikel als Lagerbestellung erfasst werden.
                                          •   Lagerzugang:
                                              Mit der Erfassung des Wareneingangs wird der Lagerbestand der Lager-
                                              artikel aktualisiert. Artikel, die nicht als Lagerartikel geführt werden, können
                                              nicht als Lagerbestand geführt werden.
                                          •   Inventur:
                                              Mit der Inventur bereinigen Sie die Bestandszahlen in A+W Business.

                                          Handlungsablauf bei der Lagerverwaltung
                                          Üblicherweise pflegen Sie den Lagerbestand durch folgende Aktivitäten:
                                          •   Stammdaten einrichten
                                          •   Lagerartikel erfassen (Erstinventur)
                                          •   Warenein- und -ausgänge buchen (automatisch, manuell)
                                          •   Abfragen zu Umschlagshäufigkeit, Preisen, Beständen usw.
                                          •   Lagerbestellung erfassen, prüfen, senden
                                          •   Inventur durchführen:
                                              – Inventurliste erstellen, Nachtragsinventur anhängen
                                              – Sollbestand ermitteln
                                              – Zähllisten drucken
                                              – Gezählte Werte erfassen
                                              – Inventur abschließen

                                          Wie soll das Lager geführt werden
                                          Allen Produkten, die im Verkauf erfasst werden, wird ein Kennzeichen zuge-
                                          ordnet, das die Art der Beschaffung festlegt. Gläser, die im Lager geführt wer-
                                          den, haben neben dem Kennzeichen (Beschaffungsart) Lagerentnahme ein
                                          Kennzeichen (Lagerbuchungsart) für die Art, wie ihr Lagerbestand berechnet
                                          wird. Diese beiden Kennzeichen werden in der Themenblock Stammdaten be-
                                          schrieben.
                                          Bevor Sie Ihr Lager in A+W Business einrichten, müssen Sie entscheiden, auf
                                          welcher Basis die Bestände geführt werden sollen: als Fläche (qm) oder in
                                          Stückzahlen. Als dritte Möglichkeit steht die kombinierte Lagerführung zur Ver-
                                          fügung, wobei der maßabhängige Lagermodus mit den Rückmeldungen aus
                                          der Optimierung kombiniert wird, so dass neben den Lagermaßen auch die
                                          zugeschnittenen Bandmaße automatisch ausgebucht werden können.
                                          Diese unterschiedlichen Möglichkeiten wirken sich folgendermaßen aus:
5.20 / 04-2020




                 A+W Business Fertigung                                                                                 G-17
                 Grundgedanken zum Lager                                                                             Tutorial




                 Modus                 Bedeutung, Beispiel                                           Nachteil
                 (Lagerkennzeichen)

                 qm = Fläche:          pro Glas wird die Fläche ermittelt:                           • keine Info über die
                 (nicht maßabhängig)                                                                   Anzahl der
                                       • Float 4 => 10.500 qm
                                                                                                       Lagermaße
                                                                                                     • keine Info darüber,
                                                                                                       wie viele Bandmaße
                                                                                                       verschnitten wurden




                                       • Float 5 => 11.070 qm




                                       • Float 6 => x qm


                 Stück:                pro Bandmaß und Lagermaß wird die Stückzahl ermittelt: • keine Info über
                 (maßabhängig)                                                                  verschnittene Band-
                                        • Float 4
                                                                                                und Lagermaße
                                                                                              • Bandmaße müssen
                                                                                                manuell ausgebucht
                                                                                                werden



                                               3210 / 6000                   900 / 1200     x/x
                                                 3 Stück                      3 Stück     n Stück

                                       • Float 5




                                               3210 / 6000              800 / 1200          x/x
                                                 3 Stück                 3 Stück          n Stück


                 Stück inkl.           Kombination aus maßabhängigen Lagermaßen und                  (Für diesen Modus
                 Rückmeldungen:        Rückmeldungen. Die verschnittenen Bandmaße und die            müssen A+W Optimizer-
                 (kombiniert)          Lagermaße werden automatisch ausgebucht. Bestand              Rückmeldungen möglich
                                       der Stückzahlen wird aktualisiert.                            sein.)

                                       Nach der Entscheidung zum Modus ordnen Sie das entsprechende Lager-
                                       kennzeichen pro Glasprodukt zu und legen in den Firmendaten den Lagerfüh-
5.20 / 04-2020




                                       rungsmodus fest. Diese Einstellungen sind in der Themenblock Stammdaten
                                       detailliert beschrieben.
                                        “Lagerführungsmodus und Reservierung” auf Seite G-30


                 G-18                                                                               A+W Business Fertigung
                 Tutorial                                                                              Stammdaten




                                          Stammdaten
                                          In diesem Themenblock lernen Sie, wie Sie die Stammdaten für die Verwal-
                                          tung des Lagers pflegen.
                                          Dazu gehören folgende Lerneinheiten:
                                          •   “Lager” auf Seite G-20
                                          •   “Firmendaten” auf Seite G-29
                                          •   “Status” auf Seite G-34
                                          •   “Produktdefinition” auf Seite G-38
                                          •   “Preise” auf Seite G-51
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-19
                 Stammdaten                                                                            Tutorial




                              Lager
                              Lernziele

                              • Lagerebenen benennen.
                              • Lagerort definieren.
                              • Lagerkategorien festlegen.


                              Nutzen

                              • Mit Lagerorten können Sie (gleiche) Materialien an unterschiedlichen Orten
                                verwalten.
                              • Auswertungen können sich auf bestimmte Lagerorte oder Lagerartikel beziehen,
                                die an unterschiedlichen Orten gelagert sind.


                              Merke

                              Ebenen                    Vier Differenzierungsebenen bezeichnen z. B.
                                                        unterschiedliche Lagerhäuser, Gänge, Regale und
                                                        Fächer.

                              Lagerorte                 Die Kombinationen der verschiedenen
                                                        Differenzierungsebenen bilden die Lagerorte.

                              Lagerkategorien           Mit Lagerkategorien können Sie die Suche und
                                                        Auswertung auf bestimmte Produkte einschränken, die
                                                        an unterschiedlichen Orten gelagert werden.

                              Voreinstellungen          Keine
5.20 / 04-2020




                 G-20                                                              A+W Business Fertigung
                 Tutorial                                                                                    Stammdaten




                                             Lagerdefinition
                                             Für die Darstellung Ihres Lagers legen Sie folgende Einstellungen fest:
                                             •    Namen der Lagerebenen
                                             •    Lagerebenen
                                             •    Lagerorte
                                             Die Bezeichnung der einzelnen Ebenen können Sie an die Erfordernisse im
                                             Unternehmen anpassen. Diese Möglichkeit sollten Sie auch dann nutzen,
                                             wenn Sie nur mit einer Ebene arbeiten.

                                             Lagerort
                                             Zur Definition von Lagerorten können Sie bis zu vier Differenzierungsebenen
                                             festlegen und damit z. B. Lagerhäuser, Gänge, Regale und Fächer unter-
                                             scheiden. Die Lagerorte werden in der Lagerverwaltung und bei der Inventur
                                             herangezogen.


                                                                      Haus 1




                                                                      Gang A


                                          Regal 1                                         Regal 2


                            Fach 1        Fach 2             Fach 3            Fach 4     Fach 5         Fach 6




                                                                      Gang B


                                          Regal m                                         Regal n



                            Fach           Fach              Fach              Fach        Fach




                 Abb. G-3      Beispiel: Lagerort = Haus 1


                                             Lagerebene
                                             Pro Ebene können Sie verschiedene Namen festlegen, z. B. auf der Ebene 1
5.20 / 04-2020




                                             die Lagerhäuser an unterschiedlichen Standorten, auf Ebene 2 die Gänge A
                                             bis F usw.




                 A+W Business Fertigung                                                                                G-21
                 Stammdaten                                                                          Tutorial




                                  Mindestens einen Lagerort definieren
                                  Sie müssen auch dann einen Lagerort definieren, wenn Sie Ihr Lager nicht
                                  weiter unterteilt haben. In diesem Fall legen Sie nur die Ebene 1 fest und
                                  definieren dann im Lagerort alle weiteren Ebenen als <k.A.>.


                              Lagerkategorien
                              Über Lagerkategorien haben Sie ein weiteres Suchkriterium für die Lagerver-
                              waltung. Wenn Sie z. B. gleiches Material an verschiedenen Lagerorten ver-
                              walten, können Sie die Lagerkategorie dazu verwenden, das Material
                              gemeinsam auszuwerten. Dazu sollten Sie alle Lagerorte definiert haben, an
                              denen das Material tatsächlich vorgehalten wird.
                              Die definierten Lagerkategorien ordnen Sie im Dialog Lagerverwaltung den
                              Produkten zu.


                              Lagerebenen festlegen
                              In dieser Einheit lernen Sie, wie Sie die Lagerebenen an die Erfordernisse in
                              Ihrem Unternehmen anpassen.
                              Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                              •   “So legen Sie Ihre verschiedenen Lagerebenen fest” auf Seite G-22
                              •   “So benennen Sie die Lagerebenen” auf Seite G-24


                               So legen Sie Ihre verschiedenen Lagerebenen fest
                                  Die folgenden Schritte sind für alle Lagerebenen gleich. In diesem Beispiel
                                  wird eine Lagerebene 1 für Fertigprodukte angelegt.
                              1 Wählen Sie im Menü Stammdaten > Lager > Ebene 1.
                                  Der Dialog Ebene 1 wird geöffnet.
                                   Stammdaten, “Ebene 1 bis 4” auf Seite B-736
5.20 / 04-2020




                 G-22                                                              A+W Business Fertigung
                 Tutorial                                                                               Stammdaten




                                          2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                            seln.




                                             Abb. G-4    Zeile für neue Lagerebene


                                          3 Geben Sie eine Bezeichnung für die Lagerebene ein, z. B. Ortsnamen, Zu-
                                            schnitt usw.
                                          4 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert.
                                          5 Wiederholen die Schritte 1 bis 4 für alle Ebenen, die Sie in Ihrem Lager
                                            unterscheiden möchten. Öffnen Sie dazu auch die Dialoge zu den Lager-
                                            ebenen 2 bis 4 und verfahren Sie auf die gleiche Weise.
5.20 / 04-2020




                 A+W Business Fertigung                                                                        G-23
                 Stammdaten                                                                             Tutorial




                               So benennen Sie die Lagerebenen
                              1 Wählen Sie im Menü Stammdaten > Lager > Lagerdefinition.
                                 Der Dialog Lagerdefinition wird geöffnet.
                                  Stammdaten, “Lagerdefinition” auf Seite B-737
                              2 Wählen Sie im Menü Definition > Ebenen.




                                 Abb. G-5     Lagerebenen benennen


                              3 Legen Sie die Namen der Lagerebenen fest, z. B. Lagerhaus für die
                                Ebene 1.
                              4 Klicken Sie auf [OK], um die Namen zu speichern.
                                 Der Dialog wird geschlossen. Die Änderungen werden in den Dialog Lager-
                                 definition übernommen.
                              5 Schließen Sie den Dialog Lagerdefinition oder definieren Sie nun die La-
                                gerorte.


                              Lagerort definieren
                              In dieser Einheit lernen Sie, wie Sie in A+W Business die Lagerorte einrichten.
                              Sie müssen auch dann einen Lagerort definieren, wenn Sie Ihr Lager nicht
                              weiter unterteilt haben. In diesem Fall legen Sie nur die Ebene 1 fest und de-
                              finieren dann für den Lagerort alle weiteren Ebenen als <k.A.>. Beachten Sie,
                              dass auch ein Lagerort mit der Definition <k.A.> für alle Ebenen als Lagerort
                              bebucht werden kann.

                                 Tipp
                                 Sie können bestimmte Materialien von einer Lagerhalle in den Produkti-
                                 onsbereich verlagern. Dazu werden die Lagerorte umgebucht. Für diesen
                                 Fall ist es sinnvoll, Lagerorte so präzise (kleinteilig) wie möglich zu definie-
                                 ren, z. B. bei den Fächern.
5.20 / 04-2020




                 G-24                                                                A+W Business Fertigung
                 Tutorial                                                                                     Stammdaten




                                           So definieren Sie einen Lagerort
                                          1 Wählen Sie im Menü Stammdaten > Lager > Lagerdefinition.




                                          A




                                          B




                                          A Selbst gewählte Bezeichnung der      B Liste der definierten Lagerorte
                                            Ebenen
                                          Abb. G-6      Lagerorte definieren


                                               Stammdaten, “Lagerdefinition” auf Seite B-737
                                              In diesem Modus können Sie die definierten Lagerorte (A) ändern, indem
                                              Sie die Bezeichnungen der Ebenen ändern. Wenn Sie den Erfassungsmo-
                                              dus gewählt haben, werden die Felder der Tabelle gesperrt.
                                          2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                            seln.
5.20 / 04-2020




                 A+W Business Fertigung                                                                              G-25
                 Stammdaten                                                                         Tutorial




                                             A                              B




                              A Auswahl der hinterlegten              B Parameter
                                Lagerebenen
                              Abb. G-7     Felder in der Tabelle gesperrt


                              3 Wählen Sie auf jeder Ebene (A) einen Eintrag aus.
                              4 Legen Sie ggf. einen der Parameter (B) fest, wenn der Lagerort besonders
                                gekennzeichnet werden soll, z. B. als Standardlager.
                                 Wenn Sie als Lagerart den Eintrag Hegla ausgewählt haben, können Sie
                                 den Lagerort für den der Wareneingang der Hegla-Lieferungen festlegen.
                              5 Wählen Sie im Menü Start > Speichern, um den Lagerort zu speichern.
                                 Die Daten werden gespeichert.
                              6 Wiederholen Sie die Schritte 2 bis 5 für alle Lagerorte, die Sie zur Verwal-
                                tung Ihres Lagers benötigen.
5.20 / 04-2020




                 G-26                                                               A+W Business Fertigung
                 Tutorial                                                                                    Stammdaten




                                          Lagerkategorien festlegen
                                          In dieser Einheit lernen Sie, wie Sie die Lagerkategorien festlegen, die Sie den
                                          Lagerartikeln zuordnen wollen.


                                           So legen Sie eine Lagerkategorie fest
                                          1 Wählen Sie im Menü Stammdaten > Lager > Kategorie.




                                             Abb. G-8     Lagerkategorien


                                              Stammdaten, “Lagerkategorien” auf Seite B-739
                                          2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                            seln.
                                          3 Geben Sie für die Lagerkategorie eine ID ein, z. B. Ziffern oder Bezeich-
                                            nungen wie Rohmaterial, Produktion.
                                          4 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                             G-27
                 Stammdaten                                                                        Tutorial




                              Übungen
                              •   Benennen Sie alle vier Lagerebenen um.
                              •   Legen Sie vier unterschiedliche Lagerorte an, von denen mindestens einer
                                  für Rohmaterial vorgesehen ist.


                              Ergänzende Informationen im Part Stammdaten
                               Stammdaten, “Ebene 1 bis 4” auf Seite B-736
                               Stammdaten, “Lagerdefinition” auf Seite B-737
                               Stammdaten, “Lagerkategorien” auf Seite B-739
5.20 / 04-2020




                 G-28                                                            A+W Business Fertigung
                 Tutorial                                                                                      Stammdaten




                                          Firmendaten
                                          Lernziele

                                          • Einstellungen für die Reservierung (Lagerführungsmodus) kennenlernen.
                                          • Einstellungen für die Ermittlung des Einkaufspreises kennenlernen.
                                          • Zeitraum für die Lagervorschau festlegen.


                                          Nutzen

                                          • Reservierungen wirken sich auf den Lagerbestand aus. Der Bestand kann schon
                                            mit der Reservierung aktualisiert werden, so dass reservierte Mengen nicht mehr
                                            frei verfügbar sind.
                                          • In der Lagervorschau werden der aktuelle Bestand und die reservierten Mengen
                                            für einen Zeitraum angezeigt, den Sie selbst festlegen.
                                          • Der Einkaufspreis von Lagerartikeln kann automatisch aktualisiert werden. Dabei
                                            wird entweder der durchschnittliche EK berechnet oder der zuletzt erfasste.


                                          Merke

                                          Lagerführungsmodus         Der Lagerführungsmodus in der Firmentabelle legt fest,
                                                                     wie Reservierungen den Lagerbestand beeinflussen.

                                          Lagerkennzeichen           Das Lagerkennzeichen legt fest, ob die Bestände eines
                                                                     Lagerartikels als Fläche (qm) oder in Stückzahlen
                                                                     gewertet werden.

                                          Reservierung               Zur Fertigung einer Auftragsposition werden die
                                                                     benötigten Mengen reserviert. Die Mengen werden in
                                                                     den Beständen gekennzeichnet oder ausgebucht.

                                          Voreinstellungen           Keine
5.20 / 04-2020




                 A+W Business Fertigung                                                                               G-29
                 Stammdaten                                                                           Tutorial




                              Lagerführungsmodus und Reservierung
                              Wenn im Auftrag ein Produkt mit der Beschaffungsart Lagerentnahme erfasst
                              wird, wird die entsprechende Menge (plus Verschnitt bei Festmaßen) des La-
                              gerartikels als reserviert gekennzeichnet. Die Reservierung kann wahlweise
                              manuell aus dem aktuellen Bestand ausgebucht werden oder automatisch,
                              wenn der Lieferschein oder die Rechnung gedruckt wird.
                              •   Reservierung ohne Bestandsaktualisierung:
                                  Die Menge wird als reserviert gekennzeichnet, vom Bestand jedoch noch
                                  nicht ausgebucht. Die Abbuchung muss manuell durchgeführt werden.
                              •   Reservierung mit Bestandsaktualisierung:
                                  Die reservierte Menge wird mit dem Druck des Lieferscheins oder der
                                  Rechnung aus dem aktuellen Bestand ausgebucht. Dabei bestimmt die
                                  Statuszuordnung, welches Formular die Buchung anstößt.
                              •   Lagerabbuchung vor Formularausdruck durchführen:
                                  Lagerartikel können abgebucht werden, bevor der Formulardruck ausge-
                                  führt wird. Falls bei der Lagerabbuchung ein Problem auftritt, wird der Auf-
                                  trag nicht gedruckt.
                              Diese Einstellungen werden in der Anzeige von Bestandsmengen im Dialog
                              Lagerinfo (Lagervorschau) und bei den automatischen Bestellvorschlägen
                              sichtbar, die beim Erreichen von Mindestmengen angestoßen werden können.
5.20 / 04-2020




                 G-30                                                              A+W Business Fertigung
                 Tutorial                                                                                 Stammdaten




                                           Firmendaten prüfen
                                           In dieser Einheit lernen Sie, wie Sie die Vorgaben zur Bewertung des Lagers
                                           und zum Lagerführungsmodus einstellen.


                                            So prüfen Sie die Einstellungen für das Lager
                                           1 Wählen Sie im Menü Stammdaten > Firma > Firmendaten.
                                               Stammdaten, “Firmendaten” auf Seite B-918
                                           2 Wechseln Sie zum Register Parameter und prüfen Sie die Einstellungen
                                             für die virtuellen Positionsnummern.




                                                                                                              A




                 A Virtuelle Positionsnummern für den Wareneingang von Kisten
                 Abb. G-9     Firmendaten – Parameter


                                              Die virtuelle Positionsnummer wird benötigt, damit der Wareneingang von
                                              Kistenpositionen mit einer Stückzahl > 1 korrekt verbucht werden kann.
                                              Der Wareneingang von Kisten ist im Part Kistenmanagement beschrieben.
                                              Auf das Kennzeichen wird daher in dieser Schulung nur hingewiesen.
                                           3 Wechseln Sie zum Register Lager / EK / EDI.
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-31
                 Stammdaten                                                                                        Tutorial




                 A




                 B




                 C




                 A Einstellungen zur Ermittlung des Einkaufspreises    C Anzahl der Vorschautage für den Dialog Lagerinfo
                 B Einstellung zur Aktualisierung des Lagerbestands
                 Abb. G-10    Firmendaten – Lager / EK / EDI


                                               Die Einstellungen zur Ermittlung des Einkaufspreises lernen Sie in der Ein-
                                               heit Preise kennen.
                                                “Einkaufspreis und Durchschnitts-EK” auf Seite G-52
                                           4 Wählen Sie die Einstellungen für Lagerbestellungen (A) aus:
                                               •   Abstandhalter bei Sprossen mitbestellen:
                                                   Aktivieren Sie diese Checkbox, wenn in einer Stückliste die Abstand-
                                                   halter zusammen mit den Sprossen bestellt werden sollen, deren
                                                   Beschaffungsart auf Bestellung gesetzt ist.
                                               •   ISO als Bestellartikel (Bearb. können Eigenfertigung sein):
                                                   Aktivieren Sie diese Checkbox, wenn die ISO-Einheit ohne die Bearbei-
                                                   tungen bestellt werden soll. Die Bearbeitung wird dann in der eigenen
                                                   Produktion durchgeführt.
                                               •   Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestellung:
                                                   Aktivieren Sie diese Checkbox, wenn in Lagerbestellungen Positionen
                                                   ohne Lagerkennzeichen im Wareneingang in roter Schrift angezeigt
                                                   werden sollen.
5.20 / 04-2020




                 G-32                                                                            A+W Business Fertigung
                 Tutorial                                                                                 Stammdaten




                                          5 Wählen Sie im Bereich Lagerführungsmodus (B) die Funktionen aus, die
                                            bei der Aktualisierung des Lagerbestands berücksichtigt werden sollen.
                                             •   Reservierung ohne Bestandsaktualisierung:
                                                 Aktivieren Sie diese Option, wenn reservierte Mengen nicht aus dem
                                                 aktuellen Bestand ausgebucht werden sollen. Die Abbuchungen müs-
                                                 sen Sie dann zum gegebenen Zeitpunkt manuell durchführen. Bei der
                                                 Auftragserfassung wird der aktuelle Bestand daher nicht angezeigt.
                                             •   Reservierung mit Bestandsaktualisierung:
                                                 Diese Option ist standardmäßig aktiviert, damit reservierte Mengen mit
                                                 dem Druck des Lieferscheins bzw. der Rechnung aus dem aktuellen
                                                 Bestand ausgebucht werden.
                                             •   Lagerführung auf Stücklistenebene:
                                                 Aktivieren Sie diese Checkbox, wenn Produkte im Lager auch dann ge-
                                                 führt werden sollen, wenn sie Bestandteile einer Stückliste sind.
                                             •   Lagerabbuchung vor Formularausdruck durchführen:
                                                 Aktivieren Sie diese Checkbox, wenn Lagerartikel abgebucht werden
                                                 sollen, bevor der Formulardruck ausgeführt wird. Falls bei der Lager-
                                                 abbuchung ein Problem auftritt, wird der Auftrag aus den zu druckenden
                                                 Dokumenten entfernt, also nicht gedruckt.
                                          6 Tragen Sie die Anzahl der Werktage (C) ein.
                                             Die Anzahl der Werktage wird für die Vorschau im Dialog Lagerinfo ausge-
                                             wertet. Sie gibt an, über welchen Zeitraum in die Zukunft die zukünftigen
                                             Lagerbestände angezeigt werden.
                                          7 Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
                                             Die Daten werden gespeichert. Nach Änderungen der Firmendaten sollten
                                             Sie A+W Business neu starten.

                                             Statuszuordnung für Lagerabbuchung
                                             Wenn Sie die Option Lagerabbuchung vor Formulardruck durchführen ak-
                                             tiviert haben, sollten Sie die Statuszuordnung für die Lagerabbuchung prü-
                                             fen. Die Mindest-, Vergabe- und Sperrstatus müssen so organisiert sein,
                                             dass die Lagerabbuchung vor dem Druck ausgeführt werden kann. Wenn
                                             die Statuszuordnung die Umkehrung der Reihenfolge nicht zulässt, wird
                                             unter Umständen die Lagerabbuchung nicht durchgeführt.

                                             Die Statuszuordnungen lernen Sie in der nächsten Einheit kennen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-33
                 Stammdaten                                                                               Tutorial




                              Status
                              Lernziele

                              • Statusänderungen durch Warenzugang und Warenabgang kennenlernen.
                              • Relevante Statuspunkte und -zuordnungen prüfen.


                              Nutzen

                              • Mit der Statuszuordnung schaffen Sie die Voraussetzungen für die automatische
                                Statusumsetzung in Dokumenten und für die Lagerbuchungen.


                              Merke

                              Status                     Der Status legt fest, wann die Bestandswerte aktualisiert
                                                         werden.

                              Voreinstellungen           Keine
5.20 / 04-2020




                 G-34                                                                 A+W Business Fertigung
                 Tutorial                                                                                  Stammdaten




                                          Statusänderungen durch Zu- und Abgänge
                                          Warenab- und Warenzugänge können den Status von Dokumenten verändern
                                          und mit der Statusveränderung zu Bestandsänderungen im Lager führen.
                                          Wenn die Statuspunkte und Statuszuordnungen entsprechend definiert sind,
                                          gilt dies auch für Teillieferungen.
                                          Wenn Sie in den Firmendaten die Option Lagerabbuchung vor Formulardruck
                                          durchführen aktiviert haben, müssen der Mindest-, Vergabe- und Sperrstatus
                                          so organisiert sein, dass die Lagerabbuchung vor dem Druck ausgeführt wer-
                                          den kann. Wenn die Statuszuordnung die Umkehrung der Reihenfolge nicht
                                          zulässt, wird unter Umständen die Lagerabbuchung nicht durchgeführt.


                                          Statuszuordnungen prüfen
                                          In dieser Einheit lernen Sie, wie Sie die Statuszuordnung prüfen und ggf. än-
                                          dern.
                                          Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                          •   “So prüfen Sie die Statusverwaltung” auf Seite G-35
                                          •   “So prüfen Sie die Statuszuordnung” auf Seite G-36


                                           So prüfen Sie die Statusverwaltung
                                          1 Wählen Sie im Menü Stammdaten > Auftrag > Statusverwaltung.




                                              A




                                              B



                                              A Status für Lagereingang             B Status für Lagerabgang
                                              Abb. G-11    Anwenderstatus (Beispiele)


                                               Stammdaten, “Statusverwaltung” auf Seite B-885
                                          2 Prüfen Sie, ob der Anwenderstatus für den Lagereingang und für den La-
                                            gerabgang vorhanden ist. Legen Sie diese ggf. an.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-35
                 Stammdaten                                                                       Tutorial




                              3 Wählen Sie dazu im Menü Start > Neu, um in den Erfassungs-Modus zu
                                wechseln.
                                 Eine neue Zeile wird freigeschaltet.
                              4 Geben Sie die Nummer und die Bezeichnung ein.
                              5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                 Die Daten werden gespeichert.
                              6 Wiederholen Sie die Schritte 3 bis 5, wenn Sie einen weiteren Anwender-
                                status anlegen wollen.
                              7 Prüfen Sie als Nächstes die Statuszuordnungen.


                               So prüfen Sie die Statuszuordnung
                              1 Wählen Sie im Menü Stammdaten > Auftrag > Statuszuordnung.




                                 Abb. G-12    Stammdaten – Statuszuordnung


                                  Stammdaten, “Statuszuordnung” auf Seite B-887
                              2 Prüfen Sie, ob die Statuszuordnungen von Lagereingang und Lagerab-
                                gang für die Dokumententypen Auftrag und Bestellung festgelegt sind:
                                 •   Warenabgang Lager: Status Lieferschein gedruckt oder Rechnung ge-
                                     druckt
                                 •   Wareneingang Lager: Status Wareneingang gebucht
                                 Für Wareneingänge und Teilwareneingänge müssen folgende Zuordnun-
                                 gen festgelegt sein:
                                 •   AB-Lieferant teilweise/Auftrag
5.20 / 04-2020




                                 •   AB-Lieferant komplett/Auftrag
                                 •   Wareneingang teilweise/Auftrag
                                 •   Wareneingang komplett/Auftrag


                 G-36                                                              A+W Business Fertigung
                 Tutorial                                                                             Stammdaten




                                             •   Wareneingang teilweise/Bestellung
                                             •   Wareneingang komplett/Bestellung
                                             •   AB-Lieferant teilweise/Bestellung
                                             •   AB-Lieferant komplett/Bestellung
                                          3 Legen Sie die fehlenden Zuordnungen an und korrigieren Sie die vorhan-
                                            denen ggf.
                                          4 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                        G-37
                 Stammdaten                                                                                  Tutorial




                              Produktdefinition
                              Lernziele

                              •   Unterschied zwischen Lagermaß und Lagerartikel kennenlernen.
                              •   Zusammenspiel von Produkt, Lagerartikel und Lagermaß kennenlernen.
                              •   Produkt und Lagerkennzeichen kennenlernen.
                              •   Einstellungen im Hauptprodukt und in der Stückliste unterscheiden.


                              Nutzen

                              • Wenn Sie die Produkte korrekt anlegen, können die Berechnungen und die
                                Reservierung von Stück und Flächen durchgeführt werden.
                              • Die jeweils aktuelle Anzeige des Bestands inklusive der Reservierungen erleichtert
                                den Einkauf.


                              Merke

                              Produkte                    Die Produkte aus den Stammdaten dienen zur
                                                          Erfassung und Preisfindung in Dokumenten. Sie werden
                                                          nicht automatisch als Lagerbestand geführt, sondern nur
                                                          aufgrund zusätzlicher Einstellungen und Definitionen.

                              Lagerartikel                Alle Produkte, die im Lager mit Bestandsmengen geführt
                                                          werden, müssen auch als Lagerartikel angelegt sein.

                              Bandmaß                     Platte, wie sie vom Hersteller geliefert wird. Aus ihr
                                                          werden die Gläser für den Verkauf zugeschnitten.

                              Lagerplatte                 Tatsächlich im Lager befindliches Glas mit bestimmtem
                                                          Maß, z. B. Float 4 mm in 1200 x 1800 mm oder
                                                          3500 x 5100 mm. Lagerplatten mit definierten Maßen
                                                          werden als auch Lagermaß bezeichnet.
                                                          Lagerplatten können als Ganzes (1200 x 1800)
                                                          verarbeitet werden. Aus ihnen können aber auch Gläser
                                                          zugeschnitten werden, z. B. 600 x 900 aus der Platte
                                                          1200 x 1800 oder aus der Platte 3210 x 5100.

                              Lagermaß (Festmaß)          Die als Lagermaß festgelegten Gläser werden ohne
                                                          Zuschnitt verkauft. Ihnen sind eigene Preistabellen
                                                          (Lagermaßtabelle) zugeordnet. Ein maßabhängiger
                                                          Lagerartikel ist immer auch ein Lagermaß.

                              Lagerkennzeichen            Das Lagerkennzeichen legt fest, ob die Bestände eines
                              (Lagerbuchungsart)          Lagerartikels als Fläche (qm) oder in Stückzahlen
                                                          gewertet werden.

                              Beschaffungsart             Das Kennzeichen legt fest, wie ein Produkt
                                                          standardmäßig beschafft wird, z. B. durch Zuschnitt,
                                                          Lagerentnahme, Produktion, Bestellung.

                              Voreinstellungen            Keine
5.20 / 04-2020




                 G-38                                                                   A+W Business Fertigung
                 Tutorial                                                                                       Stammdaten




                                             Produkt
                                             Produkte werden in den Auftragspositionen mit konkreten Maßen erfasst und
                                             von dort in die Produktion übergeben. In der Produktion werden die Gläser für
                                             die Auftragsposition aus Lagerplatten geschnitten oder aus dem Bestand der
                                             Lagermaße entnommen.
                                             Für die Bestandspflege im Lager ist dabei wichtig, wie viel Material verbraucht
                                             wird. Dieser Verbrauch schließt den Verschnitt mit ein. Die errechnete Fläche
                                             oder Stückzahl wird nach der Auftragserfassung im Lager reserviert.



                    Verkauf                                              Lager (Bestand)

                            Auftrag                      Zuschnitt aus Lagerartikel        Lagerartikel Float 4
                     Position:                           Float 4 (Lagerplatte)             (Lagermaß 400 x 600)

                     • Float 4
                     • 400 x 600 mm




                                                         Verbrauch = Fläche                Verbrauch = Stück
                                                         (Gläser + Verschnitt)




                                                                      Preis

                            Auftrag                      Festmaß (Zuschnitt)               Lagermaß
                                                         Float 4 per qm                    Float 4 400 x 600 per Stück
                     Position:                           Preisliste EK                     Preisliste EK
                     Preisliste VK                       Preistabelle Festmaße             Preistabelle Lagermaße




                 Abb. G-13       Beziehungen zwischen Produkt, Lagermaß und Preis
5.20 / 04-2020




                 A+W Business Fertigung                                                                                  G-39
                 Stammdaten                                                                           Tutorial




                              Beschaffungsart
                              Jedem Produkt ist eine Beschaffungsart zugeordnet, z. B.:
                              •   Lagerentnahme (für Lagerartikel)
                              •   Zuschnitt (für Gläser, die zugeschnitten werden sollen)
                              •   Produktion (für Scheiben, die zusammengesetzt werden, z. B. ISO, VSG)
                              •   Bestellung (für Produkte, die nicht im Lager gehalten werden)
                              Bei der Erstinventur werden die Lagerartikel aufgrund der Beschaffungsart La-
                              gerentnahme und des Lagerkennzeichens (qm oder Stück) automatisch er-
                              stellt.


                              Produkte als Lagerartikel
                              Alle Produkte, die im Lager mit Bestandsmengen geführt werden, müssen
                              auch als Lagerartikel angelegt sein.
                              Die Bestände von Lagerartikeln können im Lager unterschiedlich geführt wer-
                              den, nämlich unter Berücksichtigung der Maße oder der Stückzahlen. Mit dem
                              Kennzeichen zur Lagerbuchungsart legen Sie eine dieser Möglichkeiten fest.
                              Diese Zusammenhänge sind in den Grundgedanken zur Lagerverwaltung dar-
                              gestellt:
                               “Wie soll das Lager geführt werden” auf Seite G-17

                              Lagerbuchungsart (Lagerkennzeichen)
                              Jedem Produkt wird in den Stammdaten eine der folgenden Lagerbuchungs-
                              arten zugeordnet:
                              •   Maßabhängig:
                                  pro Produkt mehrere Lagerartikel (Glas in verschiedenen Abmessungen)
                                  Lagerbuchungsart = Stück
                                  Produkte mit diesem Kennzeichen werden als Stückartikel im Lager ge-
                                  führt. Dies sind in der Regel Gläser mit festen Maßen. Jedes Lagermaß ist
                                  dann ein eigener Stückartikel.
                                  Im Bestand wird die Gesamtfläche dieser Lagermaße nicht bewertet, son-
                                  dern z. B. 6 Stück des Lagermaßes Float 4 in der Größe 600 x 800 mm,
                                  12 Stück Float 4 mit 800 x 1200 mm.
                              •   Nicht maßabhängig:
                                  pro Produkt ein Lagerartikel ohne Maße
                                  Lagerbuchungsart = qm
                                  Produkte mit diesem Kennzeichen werden im Lager in der Mengeneinheit
                                  des Produkts geführt, z. B. Scharniere, Griffe als Stückartikel, Gläser in
                                  Quadratmetern. Die Gesamtfläche eines Glases kann dann aus beliebig
                                  vielen Platten und Resten bestehen. Bandmaße müssen dann manuell
                                  ausgebucht werden.
                              •   Kombiniert:
                                  Lagerbuchung = Stück oder qm
5.20 / 04-2020




                                  Produkte mit diesem Kennzeichen werden sowohl als qm- als auch als
                                  Stückartikel geführt. Diese Einstellung ist nur sinnvoll, wenn die Lagerfüh-
                                  rung Rückmeldungen von A+W Optimizer auswertet. Aus diesen Rückmel-


                 G-40                                                                A+W Business Fertigung
                 Tutorial                                                                                Stammdaten




                                              dungen wird ersichtlich, welche Bandmaße verschnitten wurden. Das
                                              Kennzeichen wird verwendet, um sowohl Bandmaße als auch Lagermaße
                                              im Lager automatisch zu führen.

                                          Lagerbuchungen bei kombinierter Lagerführung
                                          Der kombinierte Lagerführungsmodus erlaubt die Lagerführung für Zu-
                                          schnitts- und für Festmaße sowohl auf Quadratmeter- als auch auf Stück-
                                          basis. Bei einer A+W Optimizer-Rückmeldung ist es dann möglich,
                                          Bandmaße, die verschnitten wurden, aus dem Lager automatisch auszubu-
                                          chen (anstatt nur die qm-Menge).
                                          Für die Reservierung wird ein qm-Lagerartikel mit Abmessung 0 x 0 mm ge-
                                          nutzt, der als eine Art Zwischenspeicher dient:
                                          •   Die Menge wird auf dem qm-Artikel reserviert.
                                          •   Mit der Rückmeldung aus der Produktion wird diese Reservierung stor-
                                              niert.
                                          •   Die Menge wird auf das Bandmaß umgebucht.
                                          •   Mit dem Druck des Lieferscheins wird die Menge ausgebucht. Damit redu-
                                              ziert sich die Stückzahl der Bandmaße. Der verbleibende Rest wird in den
                                              qm-Bestand übernommen.
                                          Ausnahme:
                                          Wird der Lieferschein vor der A+W Optimizer-Rückmeldung gedruckt, so wer-
                                          den zunächst die entsprechenden Quadratmeter ausgebucht (Dummy-Bu-
                                          chung). Wenn danach die A+W Optimizer-Rückmeldung kommt, wird diese
                                          qm-Buchung korrigiert und die entsprechenden Bandmaße ausgebucht. Für
                                          die Dummy-Buchung muss in der Produktverwaltung im Register Fertigung
                                          ggf. eine abweichende Produktnummer im Feld Schlüssel Optimierung ange-
                                          geben werden.
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-41
                 Stammdaten                                                                                         Tutorial




                                              Lagermaße
                                              Gläser mit festen Größen können als Lagermaße und/oder Kisten definiert
                                              werden. Neben den Lagermaßen müssen Sie auch Lagerartikel anlegen. La-
                                              gerartikel werden für die Bestandsführung herangezogen. Wenn Sie ein La-
                                              germaß in den Stammdaten angelegt haben, bietet A+W Business die
                                              Möglichkeit, sofort in die Lagerverwaltung zu wechseln. Wie Sie den Lagerar-
                                              tikel anlegen, lernen Sie im Themenblock Lagerwirtschaft.


                                                                                                  A


                                                                                                  B

                                                                                                  C
                                                                                                                D




                             F            E




                 A Produktverwaltung Lagermaße         C Lagermaße mit verschiedenen    E Zuordnung der Preistabellen
                   (Stammdaten)                          Abmessungen                    F Ermittlung des EK im Lager
                 B Produktnummer, zu der die           D Lagerartikel zu den Lagermaßen
                   Lagermaße gehören                     (Lagerverwaltung)
                 Abb. G-14       Lagermaße (Produktverwaltung) und zugehörige Lagerartikel


                                              Jedem Lagermaß kann eine eigene Preistabelle zugeordnet werden.
                                              Wenn Sie mit dem Lagerkennzeichen maßabhängig arbeiten, müssen Sie für
                                              alle Lagermaße auch Lagerartikel angelegen.

                                                 Lagermaß Kiste im Dialog Lagermaße anlegen
                                                 Das Lagermaß Kiste ist für Lagerbuchungen zwingend erforderlich. Für die
5.20 / 04-2020




                                                 Erfassung einer Kiste als Auftrags- oder Bestellposition muss daher ein La-
                                                 gerartikel/-maß Kiste angelegt sein. Eine ausführliche Beschreibung finden
                                                 Sie im Part Kistenmanagement.


                 G-42                                                                            A+W Business Fertigung
                 Tutorial                                                                                     Stammdaten




                                          Lagermaße vs. Lagerartikel
                                          Lagermaße legen Sie in den Stammdaten für alle Produkte an, die Sie in Ihrem
                                          Lager in festen Größen verwalten, z. B. für das Produkt Float 4 die Größen
                                          600 x 800 mm, 1200 x 1800 mm, 2400 x 2800 mm usw. Diese Lagermaße
                                          dienen jedoch nicht zur Bestandsführung, sondern zur Preisgestaltung.
                                          Allen Lagermaßen können Sie eine eigene Preistabelle zuordnen und so z. B.
                                          Preise mit und ohne Zuschnitt unterscheiden. In der Regel verwenden Sie für
                                          die Lagermaße auch die qm-Preise. Außerdem können Sie auch Lagermaße
                                          anlegen, die nur bestellt werden. Jedem Lagermaß kann eine eigene Waren-
                                          gruppe zugeordnet werden.
                                          Die Lagermaße, die in den Stammdaten angelegt sind, müssen auch in der
                                          Lagerverwaltung anlegt sein, wenn sie auch als Lagerartikel (mit Bestand) ge-
                                          führt werden sollen. Dazu bietet A+W Business den schnellen Wechsel aus
                                          den Stammdaten in die Lagerwirtschaft.


                                                        Stammdaten                             Lagerverwaltung

                                           Produkt              Lagermaß                       Lagerartikel
                                           Float 4 mm
                                                                600 x 800 mm                   600 x 800 mm
                                           Nr. 1004             1200 x 1800 mm                 1200 x 1800 mm
                                                                2400 x 2800 mm                 2400 x 2800 mm


                                          Abb. G-15     Produkt, Lagermaß und Lagerartikel


                                          Sonderfall Lagerentnahme - nicht maßabhängig
                                          Die Lagermaßtabelle (Stammdaten) hat - bis auf einen Sonderfall - keine Ver-
                                          knüpfung zum Lager, sondern wird nur zur Abbildung der preislichen Abwei-
                                          chungen und für statistische Zwecke genutzt.
                                          Der Sonderfall betrifft Lagerartikel mit dem Kennzeichen nicht maßabhängig,
                                          für die ein Lagermaß in der Lagermaßtabelle angelegt wurde.
                                          Für diese nicht maßabhängigen Lagerartikel wird kein Verschnitt reserviert
                                          und es findet keine Übergabe an die Produktion statt, wenn in der Lagermaß-
                                          tabelle der Produkte diese Abmessung vorhanden ist.

                                             Beispiel: Reservierung mit/ohne Verschnitt

                                             Produkt                                         Lagerartikel

                                                                             ohne Lagermaß in      mit Lagermaß in
                                                                             Lagermaßtabelle       Lagermaßtabelle

                                             Float 4 mm                      nicht maßabhängig     nicht maßabhängig
                                                                             500 x 500 mm          500 x 500 mm
                                             Verschnitt 10%
5.20 / 04-2020




                                             Auftragsmenge 500 x 500 mm

                                             Reservierte Menge               0,275 qm              0,25 qm




                 A+W Business Fertigung                                                                                G-43
                 Stammdaten                                                                                       Tutorial




                                           Produktstammdaten prüfen
                                           Die Produkte aus den Stammdaten dienen in Dokumenten als Basis für die Er-
                                           fassung von Positionen. In der Produktion werden die Gläser für die Auftrags-
                                           position aus Lagerplatten geschnitten oder aus dem Bestand der Lagermaße
                                           entnommen.
                                           In dieser Einheit lernen Sie, wie Sie die Produktdaten so einrichten, dass die
                                           Lagerbestände und Preise korrekt berechnet werden.


                                            So prüfen Sie die Stammdaten eines Produkts
                                           1 Wählen Sie im Menü Stammdaten > Produkte > Artikel > Artikel.
                                              Der Dialog Produktverwaltung wird geöffnet.
                                               Stammdaten, “Produktverwaltung” auf Seite B-590
                                           2 Suchen Sie das Produkt, das Sie im Lager führen wollen, und prüfen Sie
                                             die Mengeneinheit.




                                                                                                                    A




                 A Mengeneinheit für die Berechnung von Preisen und Beständen
                 Abb. G-16    Produktverwaltung – Produkt
5.20 / 04-2020




                                              Die Mengeneinheit muss so gewählt sein, dass der Lagerbestand sinnvoll
                                              ermittelt werden kann, z. B. für Scharniere Stück, für Glas qm.



                 G-44                                                                          A+W Business Fertigung
                 Tutorial                                                                                    Stammdaten




                                          3 Wechseln Sie zum Register Preis/Zuschlag und prüfen Sie die Einstellun-
                                            gen.




                                                                                                 A




                                                                                                 B


                                                                                                 C



                                             A Preistabelle für den Einkauf           C Verkaufspreis und Einkaufspreis
                                             B Verschnitt, der bei der Reservierung     ermitteln
                                               berücksichtigt werden muss
                                             Abb. G-17    Produktverwaltung – Preis/Zuschlag


                                             •   Sind die Preistabellen (A), der Verschnitt (B) und die Checkboxen Preis-
                                                 relevant (C) für VK/EK richtig aktiviert.
                                             •   Die Checkboxen Preisrelevant EK muss markiert sein, damit der Ein-
                                                 kaufspreis ermittelt werden kann.
                                          4 Wechseln Sie zum Register Lager/Einkauf und prüfen Sie die Einstellung.
5.20 / 04-2020




                 A+W Business Fertigung                                                                             G-45
                 Stammdaten                                                                             Tutorial




                                                                                  A

                                                                                  B




                                                                                  C

                              A Lagerbuchungsart (Lagerkennzeichen)     C Maximalmaße für die Bestellung der
                              B Verfügbarkeitsprüfung                     Lagerplatte

                              Abb. G-18    Produktverwaltung – Lager/Einkauf


                                 Für Lagerartikel können Sie folgende Lagerbuchungsarten (A) auswählen:
                                 •   Maßabhängig:
                                     Wählen Sie diese Einstellung, wenn Lagermaße als Stückartikel geführt
                                     werden sollen. Die Einstellung ist nur für Glas sinnvoll.
                                     Die Mengeneinheit im Register Produkt setzen Sie trotzdem auf qm, da-
                                     mit die Fläche berechnet wird.
                                 •   Nicht maßabhängig:
                                     Wählen Sie diese Einstellung, für alle Lagerartikel, die in ihrer eigentli-
                                     chen Mengeneinheit geführt werden sollen, z. B. Stückartikel, Beschlä-
                                     ge. Wählen Sie diese Einstellung auch für Gläser, die in qm geführt
                                     werden sollen.
                                 •   Kombiniert:
                                     Wählen Sie diese Einstellung, wenn Sie mit Rückmeldungen von A+W
                                     Optimizer arbeiten. Die Einstellung ist nur für Glas sinnvoll.
                                     Beachten Sie, dass Sie dazu ein Dummy-Lagermaß in qm aber ohne
                                     Maße anlegen müssen.
                                     Die Einstellung ohne wird in diesem Zusammenhang nicht benutzt.
                              5 Legen Sie fest, ob für die Verfügbarkeit (B) des Produkts geprüft werden
                                soll.
                                 Wenn der Lagerartikel nicht in der Lagervorschau berücksichtigt werden
                                 muss, ist eine Verfügbarkeitsprüfung nicht erforderlich.
                              6 Wenn im aktuellen Produkt Stücklisten-Komponenten enthalten sind,
                                wechseln Sie zum Register Stückliste.

                                 Lagerführung auf Stücklistenebene
                                 Wenn Sie in den Firmendaten die Option Lagerführung auf Stücklistenebe-
                                 ne gewählt haben, müssen Sie die Beschaffungsart für die entsprechen-
                                 den Stücklisten-Komponenten setzen.
                                 Diese Form der Lagerführung lernen Sie in der Einheit Lagerführung auf
                                 Stücklistenebene kennen.
5.20 / 04-2020




                 G-46                                                                 A+W Business Fertigung
                 Tutorial                                                                                Stammdaten




                                                                                                               A
                                                                                                               B




                 A Beschaffungsart für die Komponente        B Einkaufspreis ermitteln
                 Abb. G-19   Produktverwaltung – Stücklisten-Komponenten


                                          7 Markieren Sie die jeweilige Stücklisten-Komponente und wählen Sie die
                                            Beschaffungsart (A) aus, wenn diese von der Definition in den Stammdaten
                                            der Komponente abweichen soll.
                                             Wenn die Beschaffungsart für das Hauptprodukt auf Produktion gesetzt ist,
                                             können die Stücklisten-Komponenten gleichzeitig als Lagerartikel geführt
                                             werden. Wenn Sie einen solches Hauptprodukt im Auftrag erfassen, wer-
                                             den in der Lagerinfo alle Stücklisten-Komponenten auf reserviert gesetzt.
                                          8 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                             Die Daten werden gespeichert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-47
                 Stammdaten                                                                                          Tutorial




                                            Lagermaß anlegen
                                            In dieser Einheit lernen Sie, wie Sie die Lagermaße zu den Produkten anle-
                                            gen, um die Preisberechnung differenzieren zu können.


                                             So legen Sie Lagermaße in den Stammdaten an
                                            1 Wählen Sie im Menü Stammdaten > Produkt > Artikel > Lagermaße.
                                                Der Dialog Lagermaße wird geöffnet.
                                                 Stammdaten, “Lagermaße” auf Seite B-637
                                            2 Wählen Sie im Menü Start > Neu und legen Sie das Lagermaß an.




                                                                                                                         A




                                                                                                                         B

                                                                                                                         C




                 A Maße der Platte (Inhalt nur bei Kisten)          B Preistabellen für Verkauf und Einkauf einstellen
                                                                    C Preisermittlung im Lager
                 Abb. G-20    Lagermaß für Preisfindung anlegen


                                                Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerarti-
                                                kel definiert haben sollten, tragen Sie die gleichen Werte für Breite und
                                                Höhe (A) ein.
5.20 / 04-2020




                 G-48                                                                             A+W Business Fertigung
                 Tutorial                                                                                  Stammdaten




                                          3 Sie können zusätzlich folgende abweichende Angaben einstellen:
                                             •   Preisschlüssel für den Verkauf und den Einkauf (B).
                                             •   Bezeichnung und Kurzbezeichnung (Matchcode), um z. B. den Lager-
                                                 artikel besser identifizieren zu können.
                                             •   Beschaffungsart, z. B. bei Lagerartikeln Lagerentnahme.
                                          4 Markieren Sie die Checkbox EK Suche Lager (C), wenn das Lagermaß in
                                            die Preisermittlung einbezogen werden soll.
                                             In der Einheit Preise lernen Sie, welche Einstellungen für die unterschied-
                                             lichen Formen der Berechnung notwendig sind.
                                              “Einkaufspreis und Durchschnitts-EK” auf Seite G-52
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt,
                                             ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
                                          6 Wählen Sie [Ja], wenn das Lagermaß auch als Lagerartikel verwaltet wer-
                                            den soll.
                                             Der Dialog Lagerverwaltung wird geöffnet.
                                             Die Handlungsschritte zum Anlegen eines Lagerartikels sind in einer sepa-
                                             raten Einheit beschrieben.
                                              “Lagerartikel anlegen” auf Seite G-74
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-49
                 Stammdaten                                                                      Tutorial




                              Übungen
                              •   Legen Sie zu einigen Ihrer Produkte Lagermaße an.
                              •   Achten Sie darauf, dass diese Lagermaße auch als Lagerartikel angelegt
                                  sind.


                              Ergänzende Informationen
                               “Lagermaße” auf Seite G-42
                               “Lagerführungsmodus und Reservierung” auf Seite G-30
                               Stammdaten, “Produkt anlegen” auf Seite B-182
                               Stammdaten, “Produktverwaltung” auf Seite B-590
                               Stammdaten, “Lagermaße” auf Seite B-637
                               Stammdaten, “Firmendaten – Lager/EK/EDI” auf Seite B-957
5.20 / 04-2020




                 G-50                                                            A+W Business Fertigung
                 Tutorial                                                                                        Stammdaten




                                          Preise
                                          Lernziele

                                          • Preisdefinitionen für Einkaufspreis prüfen.
                                          • Arten der Preisermittlung für den Einkaufspreis (EK) kennenlernen.


                                          Nutzen

                                          • Die Preisentwicklung von Lagerartikeln kann unter alternativen Möglichkeiten
                                            verfolgt werden: Entweder wird der letzte Einkaufspreis betrachtet oder ein
                                            durchschnittlicher Einkaufspreis.
                                          • In der Lagerverwaltung kann der Durchschnitts-EK jeweils für alle Abmessungen
                                            des Lagerartikels ermittelt werden oder nur für das aktuelle Lagermaß.


                                          Merke

                                          Einkaufspreis              Einkaufspreise werden in den Preisstammdaten auf
                                                                     dieselbe Art wie Verkaufspreise angelegt.

                                          Durchschnitts-EK           Der Durchschnitts-EK wird als Einzelpreis ermittelt. Die
                                                                     Funktion zur Berechnung muss in den Firmendaten
                                                                     aktiviert werden.

                                          Durchschnitts-EK pro       Die Ermittlung des Durchschnitts-EK kann pro Lagermaß
                                          Lagermaß                   ausgeschaltet werden.

                                          Voreinstellungen           Produktverwaltung Lagermaße
                                                                     • Checkbox EK Suche Lager
                                                                     Firmendaten
                                                                     • Register Lager / EK / EDI
5.20 / 04-2020




                 A+W Business Fertigung                                                                                 G-51
                 Stammdaten                                                                                         Tutorial




                                              Einkaufspreis und Durchschnitts-EK
                                              Sie können den Lagerwert eines Lagerartikels auf verschiedene Arten ermit-
                                              teln lassen, nämlich als Durchschnitts-EK oder den letzten EK. Diese Ent-
                                              scheidung haben Sie bereits in den Firmendaten > Register Lager / EK / EDI
                                              getroffen.
                                               “Firmendaten prüfen” auf Seite G-31
                                              Für die Preisermittlung sind u. a. zwei Kennzeichen wichtig, die in den Lager-
                                              maßen und den Lagerartikeln gesetzt werden.




                             A


                                          B


                 A Lagermaße: EK Suche Lager                             B Lagerverwaltung: Einbeziehen in den Gesamt-EK
                 Abb. G-21       Preisermittlung EK


                                              •   Lagermaße:
                                                  Dieses Kennzeichen (A) steuert, ob für dieses Lagermaß die durchschnitt-
                                                  lichen Kosten aus dem Lager ermittelt werden oder nicht.
                                              •   Lagerverwaltung:
                                                  Dieses Kennzeichen (B) steuert, ob der jeweilige Lagerartikel an der Be-
                                                  rechnung des gesamten Durchschnittspreises aller Ausprägungen dieses
                                                  Artikels teilnimmt oder nicht. Die entsprechenden Preise pro Lagerartikel
                                                  und Lagerort werden in den Bereichen Einkaufpreise und Berechnung des
                                                  geschnittenen Preises dargestellt.
                                              Die ausführliche Beschreibung der Preisdarstellung im Dialog Lagerverwal-
5.20 / 04-2020




                                              tung finden Sie in der Softwarereferenz.
                                               Softwarereferenz, “Lagerverwaltung – Preise” auf Seite G-190




                 G-52                                                                               A+W Business Fertigung
                 Tutorial                                                                                      Stammdaten




                                          Durchschnitts-EK
                                          Der Einkaufspreis wird bei jedem Lagerzugang oder bei Preisänderungen in
                                          der Bestellung neu berechnet. Das System speichert diese Informationen für
                                          jeden Lagereingang, um preisliche Änderungen an Bestellungen, die nach
                                          dem Wareneingang durchgeführt werden, wieder in den Durchschnitts-EK
                                          (geschnittener Preis) einrechnen zu können.
                                          Der Durchschnitts-EK wird nach folgender Formel berechnet:
                                          Durchschnitts-EK = ((Lagermenge * Preis) + (Zugangsmenge * Preis des Zu-
                                          ganges)) / (Menge + Zugangsmenge)

                                             Beispiel

                                             Von einem Artikel sind 100 qm zu 10 €/qm im Lager. (Durchschnitts-EK =
                                             10 €/qm). Durch eine Bestellung werden 10 qm zu 15 €/qm zugebucht. Der
                                             Durchschnittspreis wird neu berechnet:
                                             ((100 qm * 10 €) + (10 qm * 15 €)) / (100 qm + 10 qm) = 10,45 € pro qm


                                          Der EK wird so lange aktualisiert, bis für alle Bestellungen eine Rechnungs-
                                          kontrolle durchgeführt wurde oder die Bestellung ins Archiv übergeben wurde.
                                          Danach werden preisliche Änderungen in der Bestellung für die Berechnung
                                          des Durchschnittspreises nicht mehr berücksichtigt. In der Ansicht in der La-
                                          gerverwaltung werden die Bestellungen nicht mehr aufgelistet, sobald sie
                                          (nach der Archivierung) gelöscht wurden.

                                          EK-Ermittlung bei kombiniertem Lagermodus
                                          Wenn Sie mit kombiniert geführten Lagerartikeln arbeiten, wird durch die
                                          Rückmeldung aus der Produktion die auf den 0 x 0-Satz reservierte Menge
                                          gelöscht und die entsprechenden Lagerplatten werden abgebucht.
                                          Wenn Sie aber keine Produktionsrückmeldung haben, werden die Bestände
                                          der qm-Artikel sehr schnell negativ und verfälschen die Kosten.
                                          Daher können Sie in den Firmendaten festlegen, dass kombiniert geführte La-
                                          gerartikel ohne Abmessung bei der Bildung des Durchschnitts-EKs ignoriert
                                          werden. Dann werden nur die durchschnittlichen Kosten der Lagermaße be-
                                          rechnet.
5.20 / 04-2020




                 A+W Business Fertigung                                                                               G-53
                 Stammdaten                                                                                                                                                Tutorial




                                                               Ablaufplan zur Preisermittlung


                                                                                                Start der
                                                                                               Preissuche




                                                                                                Manuelle
                                                                                                                                          ja
                                                                                              Vorgabe des
                                                                                            Preisschlüssels?


                                                                                                                                                           Suche des EK in der
                                                                                                  nein                                                     Tarifzuordnung des
                                                                                                                                                             vorgegebenen
                                                                                                                                                             Preisschlüssels




                                                                                                                                                                  Ende
                                                                                                    In
                                                                             nein                                         ja
                                                                                           Produkt-Lagermaßen
                                                                                               vorhanden?




                                                                                                                                               ja             Suche nach
                                                                                                                                                           Durchschnittspreis
                                                                                                                                                                aktiv?




                                               ja             Produktausprägung                                                                                    nein
                                                            exakt in Lagerverwaltung
                                                                   vorhanden?



                                                                      nein

                      Selektion des
                  durchschnittlichen EK                      Bilden des gewichteten
                  aus dem Lagerartikel                   durchschnittlichen Preises über
                                                              all die Lagerprodukte,
                                                          in denen das entsprechende
                                                            Kennzeichen aktiviert ist.                                                                       Abweichender
                                                                                                                                                    nein
                                                                                                                                                            Preisschlüssel für
                                                                                                                                                             EK hinterlegt?




                                                                                                                                                                    ja


                                          Ist der ermittelte                                                    nein
                                              Preis > 0?




                                                    ja                                                                  Suche des EK                       Suche des EK in der
                                                                                                                       in der Standard-                    Tarifzuordnung des
                                                                                                                        Tarifzuordnung                       vorgegebenen
                                                                                                                                                             Preisschlüssels




                                                Ende                                                                                           Ende
5.20 / 04-2020




                 Abb. G-22          Ablaufplan zur Preisermittlung




                 G-54                                                                                                                          A+W Business Fertigung
                 Tutorial                                                                                     Stammdaten




                                          Erläuterung zum Ablaufplan – Preisberechnung
                                          Die Preisberechnung sucht zunächst in den Produkt-Lagermaßen, ob der Ar-
                                          tikel in genau der angegebenen Ausprägung vorhanden ist.
                                          •   Wenn ja, wird abhängig vom dortigen Kennzeichen der Durchschnittspreis
                                              des Lagerartikels ermittelt oder nicht. Ist das Kennzeichen nicht aktiv, wird
                                              der Preis im Standard-Tarif für den Einkauf gesucht. Ist ein abweichender
                                              EK-Schlüssel hinterlegt, hat dieser Vorrang vor dem Standard-Tarif.
                                          •   Wenn der Artikel nicht in den Produkt-Lagermaßen vorhanden ist, wird mit
                                              der Suche des Durchschnittspreises im Lager fortgefahren.

                                          Durchschnittspreis
                                          Bei der Ermittlung des Durchschnittspreises werden folgende Stufen durch-
                                          laufen:
                                          •   Wenn der Durchschnittspreis aus dem Lager ermittelt wird, so wird zu-
                                              nächst der genaue Lagerartikel gesucht. Wenn der Artikel vorhanden ist,
                                              wird der dort hinterlegte Preis verwendet.
                                          •   Wenn der Artikel nicht vorhanden ist, wird das gewichtete Mittel über alle
                                              Produkte mit dieser Artikelnummer und mit einem aktiven Kennzeichen er-
                                              mittelt.
                                          •   Wenn der ermittelte Preis 0 ist, so wird der Preis aus der Standard-Tarifzu-
                                              ordnung des EK gesucht.
                                          •   Wurde in der Auftragserfassung der Preisschlüssel manuell vorgegeben,
                                              so wird der Preis nur aus der Tarifzuordnung des gewählten Preisschlüs-
                                              sels ermittelt, ohne Durchschnittspreissuche.
                                          Die Kennzeichen haben auf die Rückschreibung der Kosten in den jeweiligen
                                          Lagerartikel keinen Einfluss.
                                          Nachfolgend sind einige Beispiele zum Ablauf der Preissuche dargestellt.

                                              Produkt-Lagermaße

                                              Artikel   Abmessung      Durchschnittspreis    abw. Preis-
                                                                       ermitteln             Schlüssel

                                              1004      3210 x 6000    ja                    Lagermaße
                                              1004      3210 x 3000    nein                  <k.A.>
                                              1004      3210 x 2000    nein                  Lagermaße


                                              Lagerverwaltung

                                              Artikel   Abmessung      Ermittlung Gesamt-    Bestand   Durchschnittspreis
                                                                       Durchschnittspreis

                                              1004      3210 x 6000    ja                    100 Stk   1,25 €/qm
                                              1004      2000 x 2000    ja                    40 Stk    1,84 €/qm
                                              1004      1500 x 3000    nein                  45 Stk    1,99 €/qm
5.20 / 04-2020




                 A+W Business Fertigung                                                                              G-55
                 Stammdaten                                                                        Tutorial




                              Preise laut Tarifzuordnung in der Preisverwaltung

                              Preisschlüssel          Preis

                              Standard                1,50 €/qm
                              Lagermaße               1,00 €/qm


                              Auftrag mit den ermittelten Einkaufspreisen

                              Pos.       Artikel      Abmessung             Vorgabe des       EK
                                                                            Preisschlüssels

                              1          1004         3210 x 6000           nein              1,25 €/qm
                              2          1004         2000 x 2000           nein              1,44 €/qm
                              3          1004         3210 x 3000           nein              1,50 €/qm
                              4          1004         3210 x 2000           nein              1,00 €/qm
                              5          1004         1250 x 1433           nein              1,30 €/qm
                              6          1004         3210 x 6000           ja (Lagermaße)    1,00 €/qm
5.20 / 04-2020




                 G-56                                                              A+W Business Fertigung
                 Tutorial                                                                                     Stammdaten




                                            Einstellung für EK-Ermittlung prüfen
                                            In den Firmendaten haben Sie bereits den Lagerführungsmodus eingestellt.
                                            Dazu aktivieren Sie jetzt zunächst die Ermittlung des Einkaufspreises und
                                            wählen dann die Art der Ermittlung.


                                             So prüfen Sie die Einstellungen für den Einkaufspreis
                                            1 Wählen Sie im Menü Stammdaten > Firma > Firmendaten.
                                                Stammdaten, “Firmendaten” auf Seite B-918
                                            2 Wechseln Sie zum Register Lager / EK / EDI.




                 A
                 B
                 C




                 A Ermittlung des Einkaufspreises aktivieren          C Zusatzfunktion für den kombinierten
                 B Art der Ermittlung des EK                            Lagerführungsmodus

                 Abb. G-23    Firmendaten – Lager / EK / EDI
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-57
                 Stammdaten                                                                          Tutorial




                              3 Aktivieren Sie die Checkbox Einkaufspreis ermitteln (A), um die Optionen
                                freizuschalten:
                                  •   Durchschnitts EK:
                                      Bei jeder Lagerzubuchung wird der Durchschnitts-EK neu berechnet.
                                  •   Letzter EK:
                                      Jeweils der letzte EK, der im Lager bei einem Wareneingang oder bei
                                      der Rechnungskontrolle gebucht wurde, wird zur Lagerbewertung her-
                                      angezogen.
                                  •   Kombiniert geführte Lagerartikel ohne Abmessung ignorieren:
                                      Aktivieren Sie diese Checkbox, wenn die Bestände von kombiniert ge-
                                      führten Lagerartikeln ohne Abmessung bei der Bestimmung des durch-
                                      schnittlichen EKs nicht berücksichtigt werden sollen.
                              4 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                  Die Daten werden gespeichert.


                              Preise prüfen
                              In dieser Einheit lernen Sie, wie Sie die Preise für den Einkauf festlegen.
                              Damit der Durchschnitts-EK ermittelt werden kann, müssen folgende Bedin-
                              gungen erfüllt sein:
                              •   Das Produkt muss als Lagerartikel angelegt sein.
                              •   Das Kennzeichen für den EK muss in den Firmendaten gesetzt sein.
                              In der Regel legen Sie nur einen Preisschlüssel für den EK an, Sie können je-
                              doch auch mehrere EK-Preisschlüssel nutzen. Alle Preisschlüssel für den EK
                              müssen anschließend als Tarifkombination definiert werden. Bei mehreren
                              Preisschlüsseln für den EK sollte eine Standard-Preisliste definiert sein. Sie
                              können auch einen Preis anlegen. Dieser wird bei der Berechnung des Durch-
                              schnittspreises nicht überschrieben. Der Durchschnitts-EK wird in der Lager-
                              verwaltung in gesonderten Feldern angezeigt.
5.20 / 04-2020




                 G-58                                                              A+W Business Fertigung
                 Tutorial                                                                                  Stammdaten




                                           So prüfen Sie die Stammdaten Ihrer Preislisten
                                          1 Wählen Sie im Menü Stammdaten > Preise und prüfen Sie die Einstellun-
                                            gen in den Dialogen Jahrgang, Schlüssel und Tarif.
                                              Sie brauchen nur die Einträge zu prüfen, die für Preise (und sonstige Ei-
                                              genkalkulationen) für Lagermaße und Kisten verwendet werden.
                                          2 Wählen Sie im Menü Stammdaten > Preise > Preise.




                    Abb. G-24   EK-Preistabellen


                                               Stammdaten, “Preise” auf Seite B-714
                                          3 Prüfen Sie, ob alle EK- und VK-Preise definiert und auf dem aktuellen
                                            Stand sind, und ergänzen oder korrigieren Sie diese ggf.
                                          4 Wechseln Sie zu dem Register, in dem der Preis definiert ist, und prüfen
                                            Sie, ob der EK-Preis korrekt eingetragen ist, oder korrigieren Sie diesen
                                            ggf.




                    Abb. G-25   Definierte Einkaufspreise


                                          5 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                              Die Daten werden gespeichert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-59
                 Stammdaten                                                                         Tutorial




                              Übungen
                              •   Prüfen Sie, ob den Lagermaßen die korrekten Preislisten zugeordnet sind.
                              •   Legen Sie eine neue Preisliste mit einem EK-Einzelpreis für einen Lager-
                                  artikel an.


                              Ergänzende Informationen
                               Softwarereferenz, “Reservierte Lagerartikel” auf Seite G-215
                               Softwarereferenz, “Einkaufspreise” auf Seite G-190
                               Stammdaten, “Status zuordnen” auf Seite B-427
                               Stammdaten, “Einzelpreise anlegen” auf Seite B-236
                               Stammdaten, “Preise” auf Seite B-714
                               Stammdaten, “Tarife” auf Seite B-664
                               Stammdaten, “Einkaufspreis ermitteln” auf Seite B-957
                               Stammdaten, “Lagerführungsmodus” auf Seite B-960
5.20 / 04-2020




                 G-60                                                                A+W Business Fertigung
                 Tutorial                                                                                      Stammdaten




                                          Lagerführung auf Stücklistenebene
                                          Lernziele

                                          • Zusammenhang der Beschaffungsart auf den Ebenen des Hauptprodukts und der
                                            Stücklisten-Komponenten kennenlernen.
                                          • Einstellungen in den Firmendaten prüfen.


                                          Nutzen

                                          • Stücklisten-Komponenten, die für die Produktion benötigt werden, können als
                                            Lagerartikel geführt werden.


                                          Merke

                                          Ebene: Hauptartikel        Wenn der Hauptartikel bereits als Lagerartikel definiert
                                                                     ist, sind automatisch alle Stücklisten-Komponenten auch
                                                                     als Lagerartikel definiert.

                                          Ebene: Stückliste          Jede Stücklisten-Komponente kann auch dann als
                                                                     Lagerartikel definiert werden, wenn das Hauptprodukt
                                                                     die Beschaffungsart Produktion hat.

                                          Voreinstellungen           Stammdaten:
                                                                     • Produktverwaltung
                                                                     • Lieferantenkartei
                                                                     Firmendaten:
                                                                     • Register Parameter
                                                                     • Register Lager / EK / EDI
5.20 / 04-2020




                 A+W Business Fertigung                                                                                G-61
                 Stammdaten                                                                                         Tutorial




                                            Reservierung und Buchung für Stücklisten-Kompo-
                                            nenten
                                            Lagerartikel können sowohl Hauptprodukte als auch Stücklisten-Komponen-
                                            ten sein. So können Sie beispielsweise bei einer Fertigtür, die Sie inkl. Be-
                                            schlägen verkaufen, das Glas als Eigenfertigung anlegen und die Beschläge
                                            als Lagerartikel führen.
                                            Wenn der Hauptartikel bereits als Lagerartikel definiert ist, sind automatisch
                                            alle Stücklisten-Komponenten auch als Lagerartikel definiert.




                                                                                                                A




                                                                                                                             B




                 A Beschaffungsart Hauptprodukt                          B Beschaffungsart Stücklisten-Komponente
                 Abb. G-26    Einstellung der Beschaffungsart bei Hauptprodukt mit Stückliste
5.20 / 04-2020




                                            Wenn Sie einen solchen Stücklistenartikel im Auftrag erfassen, wird jede Kom-
                                            ponente, die als Lagerartikel definiert wurde, in der Lagersuche angezeigt.



                 G-62                                                                            A+W Business Fertigung
                 Tutorial                                                                                   Stammdaten




                                            Wenn Sie dieses Hauptprodukt im Dialog Lagerinfo prüfen, werden alle Stück-
                                            listen-Komponenten mit angezeigt.




                 A




                                        B




                 A Auftragsposition                                 B Lagerinfo – Stücklisten-Komponenten
                 Abb. G-27    Auftragserfassung und Lagerinfo


                                            Nachdem Sie den Auftrag gespeichert haben, werden alle Stücklisten-Kompo-
                                            nenten reserviert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-63
                 Stammdaten                                                                           Tutorial




                              Abb. G-28   Reservierte Stücklisten-Komponenten


                              Wenn eine übergeordnete Komponente mit 2 Stück in der Stückliste geführt
                              wird, so wird die im Lager zu verbuchende Menge der untergeordneten Kom-
                              ponenten (Kinder) mit 2 multipliziert.


                              Einstellung prüfen
                              In den Firmendaten muss die Option Lagerführung auf Stücklistenebene akti-
                              viert sein.




                              Abb. G-29   Firmendaten – Lager / EK / EDI: Einstellungen zur Lagerführung von
                                          Stücklisten
5.20 / 04-2020




                 G-64                                                              A+W Business Fertigung
                 Tutorial                                                                                     Stammdaten




                                          Produkte prüfen
                                          In dieser Einheit lernen Sie, wie Sie die Beschaffungsart für die Stücklisten-
                                          Komponenten in der Produktverwaltung prüfen.


                                           So richten Sie Ihre Stücklisten für die Lagerführung ein
                                          1 Wählen Sie im Menü Stammdaten > Produkte > Artikel > Artikel.
                                             Der Dialog Produktverwaltung wird geöffnet.
                                              Stammdaten, “Produktverwaltung – Stückliste” auf Seite B-616
                                          2 Suchen Sie das Produkt, das Sie im Lager mit Stücklisten führen wollen.
                                          3 Wechseln Sie zum Register Stückliste.




                                                                                                                  A

                                                                                                                  B




                 A Beschaffungsart für die Komponente         B Einkaufspreis ermitteln
                 Abb. G-30   Produktverwaltung – Stücklisten-Komponenten


                                          4 Markieren Sie die jeweilige Stücklisten-Komponente und wählen Sie die
                                            Beschaffungsart aus, wenn diese von der Definition in den Stammdaten
                                            der Komponente abweichen soll.
                                             Wenn die Beschaffungsart für das Hauptprodukt auf Lagerentnahme ge-
5.20 / 04-2020




                                             setzt ist, gilt dies für alle Stücklisten-Komponenten.
                                             Wenn die Beschaffungsart für das Hauptprodukt auf Produktion gesetzt ist,
                                             können die Stücklisten-Komponenten gleichzeitig als Lagerartikel geführt



                 A+W Business Fertigung                                                                               G-65
                 Stammdaten                                                                        Tutorial




                                 werden. Wenn Sie einen solches Hauptprodukt im Auftrag erfassen, wer-
                                 den in der Lagerinfo alle Stücklisten-Komponenten auf reserviert gesetzt.
                              5 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                 Die Daten werden gespeichert.
                              6 Wiederholen Sie die Schritte für alle in Frage kommenden Produkte.
5.20 / 04-2020




                 G-66                                                            A+W Business Fertigung
                 Tutorial                                                                             Lagerwirtschaft




                                          Lagerwirtschaft
                                          In diesem Themenblock lernen Sie, wie Sie die Lagerartikel erfassen und ver-
                                          walten.
                                          Dazu gehören folgende Lerneinheiten:
                                          •   “Lagerverwaltung” auf Seite G-68
                                          •   “Lagerbuchung” auf Seite G-78
                                          •   “Abfragen” auf Seite G-88
                                          •   “Lagerinformationen” auf Seite G-97
                                          •   “Lagerbestellung (automatisch)” auf Seite G-107
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-67
                 Lagerwirtschaft                                                                              Tutorial




                                   Lagerverwaltung
                                   Lernziele

                                   • Dialog Lagerverwaltung kennenlernen.
                                   • Lagerartikel anlegen.


                                   Nutzen

                                   • Mit Lagerartikeln können Sie den Lagerbestand erfassen und pflegen.
                                   • Die Bestände von Lagerartikeln werden mit der Buchung von Warenab- und
                                     Warenzugänge aktualisiert.
                                   • Über die Lagerartikel erhalten Sie die aktuelle Berechnung des Bestands inklusive
                                     der Reservierungen und der Bestellungen.


                                   Merke

                                   Bestand berechnen           Nur wenn Sie die Lagerartikel anlegen, kann die
                                                               Berechnung von Stückzahlen und Flächen korrekt
                                                               durchgeführt werden.

                                   Lagerartikel               Im Lager können nur Bestände von Lagerartikeln
                                                              verwaltetet werden.
                                                               Die Produkte aus den Stammdaten werden nicht
                                                               automatisch als Lagerbestand geführt.

                                   Wareneingang, -ausgang      Der Wareneingang und Warenausgang kann nur für
                                                               Lagerartikel gebucht werden.

                                   Voreinstellungen            Stammdaten:
                                                               • Lagerorte
                                                               • Produkte
                                                               • Lagermaße
5.20 / 04-2020




                 G-68                                                                      A+W Business Fertigung
                 Tutorial                                                                                    Lagerwirtschaft




                                            Elemente im Dialog Lagerverwaltung
                                            Jeder Lagerartikel kann in verschiedenen Ausprägungen angelegt werden,
                                            z. B. Float 5 mm in mehreren Abmessungen.


                                              J                  I




                 A

                                                                                                                        H
                 B

                 C


                 D

                 E
                                                                                                                        G




                                                      F
                 A   Produktnummer                                   F   Bestandsprüfung für Lagervorschau
                 B   Maße des Lagerartikels                          G   Definierte Lagerartikel
                 C   Standard-Lagerort                               H   Hauptartikel
                 D   Lagerkategorie                                  I   Blattzahl bei Kisten
                 E   Kennzeichen Lager-Hauptartikel                  J   Lagerort (4 Ebenen)
                 Abb. G-31    Definition des Lagerartikels


                                            Wenn die Bestände nicht pro Lagerort (F) geprüft werden, muss ein Hauptar-
                                            tikel (E, H) zugeordnet werden, um die verfügbaren Quadratmeter des Glases
                                            zu ermitteln.
                                            Bestandsmengen können pro Lagerort (J) gepflegt werden. Die definierten
                                            Lagerorte werden dazu den Lagerartikeln zugeordnet. Wenn ein Lagerartikel
                                            an verschiedenen Lagerorten vorgehalten wird, muss ein Standard-
                                            Lagerort (C) festgelegt werden.
                                            Zu- und Abgänge werden automatisch am Standard-Lagerort verbucht, kön-
5.20 / 04-2020




                                            nen aber manuell geändert werden.




                 A+W Business Fertigung                                                                               G-69
                 Lagerwirtschaft                                                                              Tutorial




                                   Lagerartikel
                                   Die Produkte aus den Stammdaten werden nicht automatisch im Lager ge-
                                   führt. Damit ist gesichert, dass in der Bestandsführung nur die Artikel verwaltet
                                   werden, für die Lagerbestände vorgehalten werden. Andere Artikel, die nur
                                   kurzzeitig im Lager für die Produktion eines Auftrags gelagert sind, brauchen
                                   nicht als Lagerbestand gepflegt zu werden.
                                   Zu jedem (Glas-)Produkt gehören auch ein Lagermaß und ein Lagerartikel.
                                   Die Zusammenhänge haben Sie bereits in der Lerneinheit Produkt kennenge-
                                   lernt.


                                   Lager-Hauptartikel
                                   Sie können in der Lagerverwaltung mehrere Lagermaße miteinander verknüp-
                                   fen, indem Sie einen Lager-Hauptartikel angeben. Die Bestandsprüfung (für
                                   die Lagervorschau im Dialog Lagerinfo) wird dann nur für den Lager-Haupt-
                                   artikel durchgeführt und nur für diesen müssen Sie einen Mindestbestand hin-
                                   terlegen.

                                      Beispiel

                                      Der Artikel 1004 ist mit folgenden Abmessungen angelegt:
                                      0 x 0, 500 x 600, 1200 x 1800, 3210 x 4000 und 3210 x 5000.
                                      Für die Maße 3210 x 4000 und 3210 x 5000 ist als Lager-Hauptartikel jeweils
                                      der Artikel 0 x 0 angegeben. Für diesen ist der Mindestbestand mit
                                      19.000,00 qm festgelegt.
                                      Die Bestände der Maße 3210 x 4000 und 3210 x 5000 werden gemeinsam
                                      gegen den Mindestbestand 19.000,00 qm geprüft.
                                      Für die Maße 500 x 600 und 1200 x 1800 sind jeweils eigene
                                      Mindestbestände festgelegt, die zur Prüfung herangezogen werden.


                                   Wenn Sie die Lagerartikel bereits mit jeweils einem Mindestbestand angelegt
                                   haben, können Sie diese später dennoch einem Hauptartikel zuordnen. Bei
                                   der Ermittlung des Mindestbestands wird nur die Einstellung am Hauptartikel
                                   geprüft, die Mindestbestände an den Lagerartikeln werden ignoriert.
5.20 / 04-2020




                 G-70                                                                     A+W Business Fertigung
                 Tutorial                                                                              Lagerwirtschaft




                                          Mindestmengen
                                          Wenn der Lagerbestand eines Artikels eine bestimmte Mindestmenge (unter
                                          Berücksichtigung der Aufträge und Bestellungen) unterschreitet, muss recht-
                                          zeitig nachbestellt werden, um die Produktion nicht zu behindern. In
                                          A+W Business können Sie einen Schwellenwert für den Mindestbestand und
                                          einen Wert für den kritischen Lagerbestand angeben. Dieser wird für jeden Ar-
                                          tikel gesondert festgelegt.
                                          Der Mindestbestand ist also eine Kenngröße, die nicht unterschritten werden
                                          sollte, und zwar weder real noch im Rahmen von Reservierungen.
                                          Mit Hilfe des definierten Mindestbestands erzeugt das Lager automatisch Be-
                                          stellvorschläge. Diese müssen manuell freigegeben werden. Die automati-
                                          schen Bestellvorschläge verwenden als Grundlage zur Berechnung der zu
                                          bestellenden Mengen folgende Kennzahlen:
                                          •   Bestellte Menge
                                          •   Reservierung
                                          •   Mindestbestand
                                          •   Standardbestellmenge
                                          •   Aktueller Bestand
                                          Um den Artikel exakt zu bestimmen, werden u. a. Breite und Höhe ausgewer-
                                          tet.
                                          Die Berechnung der Bestellmenge lernen Sie in einer gesonderten Einheit
                                          kennen.
                                           “Bestellmenge nach Bestandsprüfung” auf Seite G-135
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-71
                 Lagerwirtschaft                                                                                       Tutorial




                                            Preise
                                            Die Preise eines Lagerartikels werden als durchschnittliche Bezugspreise
                                            (EK-Preise) dargestellt, sofern diese Funktion in den Firmendaten aktiviert ist.
                                            Die Anzeige der Durchschnittspreise wird bei der Archivierung und bei der
                                            Rechnungskontrolle für den jeweiligen Lagerartikel aktualisiert.
                                            A+W Business geht davon aus, dass nach diesen Vorgängen die Preise nicht
                                            mehr geändert werden. Wenn Sie die Preise dennoch nach einem der Vorgän-
                                            ge ändern, fließen diese Änderungen nicht in die Berechnung des Durch-
                                            schnittspreises ein.


                                                          E




                 A


                 B




                 C
                 D

                 A Anzeigemodus (z. B. für Scheiben mit              D Durchschnittspreis pro Artikel oder über alle
                   unterschiedlichen Lagermaßen)                       Abmessungen, wenn C aktiviert ist
                 B Durchschnittspreise im Einkauf                    E Lagerwerte des markierten Artikels
                 C Einbeziehung in den Gesamt-EK
                 Abb. G-32    Durchschnittspreise für Lagerartikel


                                            Sie können festlegen, ob ein Artikel in die Berechnung des Durchschnittsprei-
                                            ses über alle Abmessungen einbezogen werden soll. Nur wenn Sie die Check-
                                            box Einbeziehen in Gesamt-EK (C) markiert haben, werden die Preise für den
                                            aktuellen Artikel in die Berechnung einbezogen.
                                            Mit der Wahl des Modus (A) bestimmen Sie die Ansicht der Preisdarstellung:
5.20 / 04-2020




                                            •   Nur dieser Artikel:
                                                Bei der Berechnung wird nur der angezeigte Artikel in der gewählten Ab-
                                                messung berücksichtigt. Die EK-Historie des aktuellen Artikels wird ange-
                                                zeigt.


                 G-72                                                                                A+W Business Fertigung
                 Tutorial                                                                               Lagerwirtschaft




                                          •   Alle Abmessungen:
                                              Bei der Berechnung werden alle Abmessungen des angezeigten Glases
                                              berücksichtigt. Die EK-Historie aller Abmessungen des Artikels wird ange-
                                              zeigt.
                                          Der Durchschnitts-EK wird für jeden Datensatz errechnet, außer für Warenab-
                                          gänge. Warenabgänge reduzieren lediglich den Bestand. Die angezeigte Liste
                                          der Neuberechnungen (B) wird durch die Archivierung und durch die Rech-
                                          nungskontrolle reduziert. Damit bleibt die Anzeige übersichtlicher.
                                          Der erste Datensatz zeigt den Anfangsbestand und den ursprünglichen Preis.
                                          Darunter werden Zu- und Abgänge (negatives Vorzeichen) aufgeführt. Beim
                                          Zugang durch eine Lagerbestellung sind außerdem die Bestellnummer und
                                          die Bestellposition angezeigt.
                                          Der Durchschnitts-EK wird bei der Erfassung oder Änderungen von Bestellun-
                                          gen aktualisiert. Er wird unter Berücksichtigung der gesamten Menge ermit-
                                          telt.

                                              Beispiel:

                                               100 Stück        auf Lager          à 15,00 €                  1500,00 €

                                                40 Stück        neue Einbuchung    à 18,00 €        +          720,00 €

                                                                                                    =        2200,00 €
                                                                                                             ========
                                               2200,00/140 Stück = 15,86 €



                                          In die Berechnung fließen auch automatische Zuschläge ein, die in Bestellun-
                                          gen aufgeführt sind, z. B. Energie- oder Transportzuschlag.

                                          Verteilung von Zuschlägen
                                          Kosten, die durch eine Lagerbestellung im Lager entstanden sind, werden im
                                          EK anteilig auf alle Artikel der Bestellung aufgeschlagen. Solche Kosten kön-
                                          nen beispielsweise Frachtkosten, Energiezuschlag oder beliebige sonstige
                                          Kosten sein, die für die Beschaffung der Lagerware eine Rolle spielen.
                                          Diese Rückverteilung ist abhängig von der Preiseinheit des Zuschlages. Ist
                                          die Preiseinheit kg, so wird der Zuschlag auf Grundlage der Positionsgewichte
                                          rückverteilt. Bei allen anderen Preiseinheiten wird nach dem Preis der Positi-
                                          onen gewichtet.
                                          Da jede Änderung an einer der Positionen Einfluss auf die Rückverteilung aller
                                          anderer Positionen hat, erfolgt diese Rückverteilung für das komplette Doku-
                                          ment immer nach einer Positionsänderung, also nach Abschluss der Eingabe
                                          in der Positionserfassung.
                                          Änderungen an solchen Positionen aktualisieren den EK nur so lange, bis die
                                          Rechnungskontrolle durchgeführt wurde.
                                          Die Fußzuschläge haben Sie in der Schulung zum Einkauf kennengelernt.
5.20 / 04-2020




                                           Einkauf, “Fußzuschläge/-rabatte” auf Seite D-157




                 A+W Business Fertigung                                                                           G-73
                 Lagerwirtschaft                                                                              Tutorial




                                   Lagerartikel anlegen
                                   In dieser Einheit lernen Sie, wie Sie die benötigten Lagerartikel anlegen. Dabei
                                   müssen Sie mindestens folgende Einstellungen festlegen, um das Lager ver-
                                   walten zu können:
                                   •   Artikelnummer und Bezeichnung
                                   •   Maße bei Lagermaßen
                                   •   Lagerort und Standard-Lagerort (Default-Lagerort)
                                   •   Bestände

                                       Inbetriebnahme des Lagers
                                       Wenn noch gar keine Lagerartikel angelegt sind, können Sie sich diese
                                       Aufgabe durch die sogenannte Erstinventur erleichtern. Diesen Ablauf ler-
                                       nen Sie in einer gesonderten Einheit kennen.


                                    So legen Sie einen Lagerartikel an
                                   1 Wählen Sie im Menü Lagerwirtschaft > Lagerverwaltung.
                                       Der Dialog Lagerverwaltung wird geöffnet.
                                        Softwarereferenz, “Lagerverwaltung – Lagerartikel” auf Seite G-186
                                   2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                     seln.
                                       Wenn Sie den Dialog Lagerverwaltung aus den Stammdaten heraus geöff-
                                       net haben, entfällt dieser Schritt. Die Felder für Artikel und Maße sind dann
                                       bereits gefüllt.
5.20 / 04-2020




                 G-74                                                                     A+W Business Fertigung
                 Tutorial                                                                                  Lagerwirtschaft




                 A


                 B

                 C




                 D




                 E




                                                   F
                 A Nummer des Lagerartikels                           D Hauptartikel
                 B Maße                                               E Bestände
                 C Lagerort                                           F Bestandsprüfung
                 Abb. G-33   Felder für neuen Lagerartikel freigeschaltet


                                           3 Geben Sie die Nummer (A) und ggf. die Maße (B) ein.
                                           4 Wählen Sie einen Lagerort aus (C).
                                               Wenn Sie keinen Lagerort auswählen, wird der Lagerort <k.A.> eingetra-
                                               gen. In der Lagerwirtschaft wird dieser wie die definierten Lagerorte behan-
                                               delt, z. B. bei der Inventur und bei Abfragen.
                                               Wenn Sie einen Lagerartikel an mehreren Lagerorten verwalten, müssen
                                               Sie einen dieser Lagerorte als Standard festlegen.
                                           5 Markieren Sie dazu die Checkbox Default-Lagerort.
                                           6 Wählen Sie im Feld Hauptartikel (D) den Artikel aus, für den Sie einen Min-
                                             destbestand für die Bestandsprüfung hinterlegen wollen.
                                               Wenn Sie für den neuen Lagerartikel einen eigenen Mindestbestand ange-
                                               ben wollen, müssen Sie die Maße des neuen Artikels auswählen. Die neu-
                                               en Maße werden jedoch erst angezeigt, nachdem Sie den neuen Artikel
                                               gespeichert haben. Wählen Sie also zunächst irgendein Maß aus und än-
                                               dern Sie dieses, nachdem Sie den Artikel gespeichert haben.
5.20 / 04-2020




                                           7 Aktivieren Sie die Checkbox Bestandsprüfung pro Lagerort (F), wenn für
                                             den Lagerartikel alle Lagerorte bei der Bestandsprüfung getrennt bewertet
                                             werden sollen.


                 A+W Business Fertigung                                                                              G-75
                 Lagerwirtschaft                                                                       Tutorial




                                   8 Geben Sie ggf. im Bereich Bestände (E) die Werte für die Mengen ein.
                                      Beachten Sie, dass der Mindestbestand entsprechend groß angegeben
                                      werden muss, wenn Sie für mehrere Maße denselben Hauptartikel ange-
                                      geben haben.
                                      Die Checkboxen sind nur im Auswahlmodus freigeschaltet. Sie dienen da-
                                      zu, die Suche nach Lagerartikeln zu filtern.
                                      Damit sind die Mindestangaben für den Lagerartikel hinterlegt.
                                   9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                      Die Daten werden gespeichert. Gleichzeitig wird ein Dummy-Lagerartikel
                                      ohne Maße für den kombinierten Lagerführungsmodus angelegt.
                                      Damit sind alle notwendigen Informationen hinterlegt, die A+W Business
                                      braucht, um Reservierungen und Buchungen durchzuführen. Der neue La-
                                      gerartikel kann nun bebucht werden.
5.20 / 04-2020




                 G-76                                                                A+W Business Fertigung
                 Tutorial                                                                               Lagerwirtschaft




                                          Übungen
                                          Legen Sie folgend Lagerartikel an und weisen Sie die korrekte Preisliste zu:
                                          •   Lagerartikel, der in Stück auf Lager geführt wird.
                                          •   Lagerartikel Handgriff, der in seiner eigenen Mengeneinheit auf Lager ge-
                                              führt wird.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Verwaltung” auf Seite G-176
                                           Einkauf, “Dokument Bestellung” auf Seite D-45
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-77
                 Lagerwirtschaft                                                                           Tutorial




                                   Lagerbuchung
                                   Lernziele

                                   • Buchungsarten für Lagerartikel kennenlernen.
                                   • Automatische Lagerbuchungen kennenlernen.
                                   • Lagerbuchungen manuell auslösen.


                                   Nutzen

                                   • Bei Bestellungen von Lagerartikeln wird der Wareneingang automatisch im Lager
                                     verbucht, bei Auftragspositionen der Warenausgang.
                                   • Sie können den Lagerbestand an einzelnen Lagerorten korrigieren, indem Sie
                                     Lagerartikel umbuchen.


                                   Merke

                                   Automatische Buchung      • Automatische Zugangsbuchungen werden ausgelöst,
                                                               wenn beim Wareneingang der Status in der
                                                               Bestellung umgesetzt wird.
                                                             • Automatische Abgangsbuchungen werden ausgelöst,
                                                               wenn in einem Auftrag der Status durch den Druck
                                                               umgesetzt wird.

                                   Buchungsarten             Die Buchungsarten für Lagerbuchungen sind fest im
                                                             System hinterlegt.

                                   Manuelle Buchungen        Manuell können z. B. folgende Buchungen ausgelöst
                                                             werden:
                                                             • Zu- und Abgang von Waren
                                                             • Lagerort ändern

                                   Voreinstellungen          Stammdaten:
                                                             • Statuszuordnungen
                                                             Firmendaten:
                                                             • Register Lager / EK / EDI
5.20 / 04-2020




                 G-78                                                                      A+W Business Fertigung
                 Tutorial                                                                             Lagerwirtschaft




                                          Lagerbewegungen
                                          Die Lagerwirtschaft übernimmt Führung, Pflege und Kontrolle von Lagerbe-
                                          ständen. Zusätzlich steht der Dialog Lagerverwaltung für den manuellen Ein-
                                          gang, den manuellen Ausgang und zur Umbuchung von Lagerorten zur
                                          Verfügung.




                                          Abb. G-34   Lagerverwaltung für manuelle Lagerbuchungen


                                          Alle Lagerbewegungen werden in einem Protokoll festgehalten, so dass Sie
                                          alle Vorgänge zurückverfolgen können.
                                          Lagerbewegungen werden durch Aufträge, Bestellungen und Wareneingänge
                                          automatisch gebucht.

                                          Scannen
                                          In Verbindung mit AWPort können Lagerbuchungen auch über Barcodes er-
                                          fasst werden. Dazu gehören nicht nur die Wareneingänge und Warenausgän-
                                          ge, sondern auch Umbuchungen.
                                          Weitere Informationen zum Barcode und den Formaten entnehmen Sie bitte
                                          der Dokumentation zu AWPort.


                                          Buchungsarten
                                          Die Buchungsarten für Lagerbuchungen sind fest im System hinterlegt und
                                          können nicht bearbeitet werden. Bei jeder Buchung eines Lagerartikels wird
                                          eine entsprechende Buchungsart zugewiesen. Anhand der Buchungsart kön-
5.20 / 04-2020




                                          nen Auswertungen erstellt werden, die den Überblick über den Lagerbestand
                                          oder die Art der Lagerbewegungen verfeinern, z. B. über bestellte und reser-
                                          vierte Mengen.


                 A+W Business Fertigung                                                                         G-79
                 Lagerwirtschaft                                                                            Tutorial




                                   Folgende Buchungsarten stehen zur Verfügung:
                                   •   Reserviert:
                                       Ein Artikel ist durch einen Auftrag so lange reserviert, bis der Lieferschein
                                       oder die Rechnung gedruckt wurde.
                                   •   Ausgeliefert:
                                       Ein Artikel wird als ausgeliefert gekennzeichnet, wenn der Lieferschein
                                       oder die Rechnung gedruckt wurde.
                                   •   Verschnittenes LM:
                                       Diese Buchungsart wird von Rückmeldung des der A+W Optimizers ver-
                                       wendet, wenn eine Position aus einem Lagermaß zugeschnitten wurde.
                                       Die Anzahl der Lagerplatten wird ausgewertet.
                                   •   Bestellt:
                                       Das Kennzeichen wird durch eine Lagerbestellung gesetzt.
                                   •   Empfangen:
                                       Ein Artikel gilt dann als geliefert und empfangen, wenn er im Wareneingang
                                       verbucht wurde.
                                   •   Lagereingang manuell, Lagerausgang manuell:
                                       Die manuell gebuchten Lagerzu- oder Lagerabgänge sind durch eigene
                                       Buchungsarten gekennzeichnet.
                                   •   Lagerumbuchung:
                                       Lagerumbuchungen werden manuell ausgelöst.
                                   •   Neuanlage:
                                       Die Daten für neue Lagerartikel können im Rahmen einer Inventur oder
                                       manuell angelegt worden sein. Berücksichtigt werden alle neuen Artikel ab
                                       der letzten Archivierung.
                                   •   Korrektur:
                                       Im Rahmen einer Inventur können die Bestände von Lagerartikeln berich-
                                       tigt werden. Berücksichtigt werden alle Korrekturen ab der letzten Archivie-
                                       rung.
                                   •   Aus Lager gelöscht:
                                       Interne Buchungsart


                                   Ab- und Zubuchung
                                   Lagerartikel werden je nach dem definierten Status abgebucht, wenn der Lie-
                                   ferschein oder die Rechnung für einen Auftrag gedruckt wird. Bis zu diesem
                                   Zeitpunkt sind die Lagerartikel lediglich reserviert.
                                   Ob eine Reservierung den Bestand aktualisiert oder nicht, hängt vom Lager-
                                   führungsmodus ab, den Sie in den Firmendaten gewählt haben.
                                    “Lagerführungsmodus und Reservierung” auf Seite G-30
                                   Durch den Wareneingang im Einkauf werden Lagerartikel aus Lagerbestellun-
                                   gen automatisch hinzugebucht.
                                   Beim Wareneingang aus Lagerbestellungen können auch Waren erfasst wer-
                                   den, die nicht als Lagerartikel angelegt sind. Diese werden jedoch nicht mit
                                   Bestandsmengen gepflegt. Für diese Produkte werden keine Lagerbuchun-
5.20 / 04-2020




                                   gen durchgeführt.




                 G-80                                                                    A+W Business Fertigung
                 Tutorial                                                                                Lagerwirtschaft




                                              Lagerbuchungen für Kisten
                                              Kisten werden in der Regel über Identnummern (ID) verbucht. Eine aus-
                                              führliche Beschreibung finden Sie im Part Kistenmanagement.


                                          Ab- oder Zugang manuell erfassen
                                          In dieser Einheit lernen Sie, wie Sie einen Abgang oder Zugang von Lager-
                                          artikeln manuell buchen.
                                          Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                          •   “So buchen Sie einen Warenzugang manuell” auf Seite G-81
                                          •   “So buchen Sie einen Warenabgang manuell” auf Seite G-84


                                           So buchen Sie einen Warenzugang manuell
                                          1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung.
                                              Der Dialog Lagerbewegung wird angezeigt.
                                               Softwarereferenz, “Lagerbewegung – Abgang, Zugang” auf Seite G-196
                                          2 Wechseln Sie ggf. zum Register Zugang.




                                              Abb. G-35   Lagerartikel suchen


                                          3 Geben Sie im Feld Produkt die Produktnummer ein und wählen Sie im
                                            Menü Start > Suchen.
                                              Im Bereich Lagerorte werden alle Lagerartikel aufgeführt, die dem Such-
5.20 / 04-2020




                                              kriterium entsprechen.




                 A+W Business Fertigung                                                                              G-81
                 Lagerwirtschaft                                                                         Tutorial




                                                                                                           B




                                   A




                                   A Artikel markieren                     B Zugangsmenge
                                   Abb. G-36    Lagerbewegung – Zugang


                                   4 Markieren Sie den gewünschten Lagerartikel (A).
                                       Im Bereich Bestandsveränderung werden die Felder mit den aktuellen
                                       Werten gefüllt.
                                   5 Tragen Sie die Zugangsmenge (B) und/oder den neuen Bewertungspreis
                                     ein.
                                   6 Ändern Sie ggf. das Buchungsdatum.
                                   7 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                       Die Daten werden gespeichert und der Bestand wird aktualisiert.
                                       Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird der Di-
                                       alog Lagerhistorie geöffnet, wenn Sie den Dialog Lagerbewegung schlie-
                                       ßen.
5.20 / 04-2020




                 G-82                                                                 A+W Business Fertigung
                 Tutorial                                                                           Lagerwirtschaft




                 Abb. G-37   Lagerhistorie


                                             Sie können dann alle Lagerbewegungen als Protokoll drucken.




                                                                                         A



                                                                                         B




                 A Legende                       B Buchungsdetails der manuellen Zugangsbuchung
                 Abb. G-38   Protokoll der Zugangsbuchung
5.20 / 04-2020




                 A+W Business Fertigung                                                                      G-83
                 Lagerwirtschaft                                                                       Tutorial




                                    So buchen Sie einen Warenabgang manuell
                                   1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung > Register Ab-
                                     gang.
                                   2 Geben Sie im Feld Produkt die Produktnummer ein und wählen Sie im
                                     Menü Start > Suchen.
                                     Im Bereich Lagerorte werden alle Lagerartikel aufgeführt, die dem Suchkri-
                                     terium entsprechen.
                                   3 Markieren Sie den gewünschten Lagerartikel.
                                     Im Bereich Bestandsveränderungen werden die Felder mit den aktuellen
                                     Werten gefüllt.




                                     Abb. G-39   Manueller Lagerabgang


                                   4 Tragen Sie die Menge ein, die aus dem Bestand ausgebucht werden soll.
                                   5 Ändern Sie ggf. das Buchungsdatum.
                                   6 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                     Die Daten werden gespeichert und der Bestand wird aktualisiert.
5.20 / 04-2020




                 G-84                                                                A+W Business Fertigung
                 Tutorial                                                                               Lagerwirtschaft




                                          Lagerort ändern
                                          In dieser Einheit lernen Sie, wie Sie einen Lagerartikel von einem Lagerort zu
                                          einem anderen verschieben, z. B. aus der Lagerhalle in den Produktions-
                                          bereich. Diese Bewegung wird durch eine Umbuchung erfasst. Dadurch wer-
                                          den die Lagerartikel beim alten Lagerort als Abgang und beim neuen als
                                          Zugang verbucht.

                                             Lagerort für einen Teil des Bestands ändern
                                             Mit dem Umbuchen eines Lagerorts im Register Umbuchen wird immer der
                                             gesamte Bestand eines Lagerortes an einen anderen Lagerort umgebucht.
                                             Wenn Sie nur einen Teil der gelagerten Menge umbuchen wollen, müssen
                                             Sie diesen Teil am alten Lagerort ausbuchen und anschließend am neuen
                                             Lagerort zubuchen.


                                           So buchen Sie einen Lagerort um
                                          1 Wählen Sie im Menü Lagerwirtschaft > Lagerbewegung.
                                             Der Dialog Lagerbewegung wird angezeigt.
                                              Softwarereferenz, “Lagerbewegung” auf Seite G-195
                                          2 Wechseln Sie zum Register Umbuchung.
                                          3 Geben Sie im Feld Produkt die Produktnummer oder die ID ein.
                                          4 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-85
                 Lagerwirtschaft                                                                       Tutorial




                                                                         A                    B




                                      A Aktueller Lagerort                   B Neuen Lagerort wählen
                                      Abb. G-40    Lagerbewegung – Umbuchung


                                      Im Bereich Lagerorte (A) werden alle Lagerartikel aufgeführt, die dem
                                      Suchkriterium entsprechen.
                                   5 Markieren Sie den gewünschten Lagerartikel.
                                   6 Wählen Sie im Bereich Lagerort (B) den neuen Lagerort aus.
                                   7 Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
                                      Die Daten werden gespeichert. Der Lagerartikel wird am alten Lagerort
                                      aus- und am neuen zugebucht.
5.20 / 04-2020




                 G-86                                                                 A+W Business Fertigung
                 Tutorial                                                                                 Lagerwirtschaft




                                          Übungen
                                          •   Buchen Sie einen Lagerort um. Beachten Sie dabei, dass alle Lagerartikel
                                              umgebucht werden.
                                          •   Verbuchen Sie einen Lagerzugang manuell. Wenn Sie keine offene Lager-
                                              bestellung haben, holen Sie diese Übung in der Einheit Lagerbestellung
                                              nach.


                                          Ergänzende Informationen
                                           “Lagerdefinition” auf Seite G-21
                                           Softwarereferenz, “Buchungsart” auf Seite G-203
                                           Einkauf, “Kistengeschäft” auf Seite D-136
                                           Einkauf, “Wareneingang von Kisten erfassen” auf Seite D-138
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-87
                 Lagerwirtschaft                                                                             Tutorial




                                   Abfragen
                                   Lernziele

                                   • Lagerbestand prüfen.
                                   • Lagerbewegungen verfolgen.
                                   • Lagerentwicklung prüfen.


                                   Nutzen

                                   • Sie können sich mit den Abfragen (außerhalb der Inventur) einen schnellen
                                     Überblick über die Bestände verschaffen.
                                   • Sie können Ladenhüter und Renner identifizieren und die Lagerverwaltung
                                     entsprechend anpassen.


                                   Merke

                                   Buchungsjournal            Im Buchungsjournal werden alle automatisch
                                                              durchgeführten Buchungen angezeigt, die sich aus
                                                              Dokumenten ergeben.

                                   Lagerhistorie              In der Lagerhistorie werden alle Lager-Buchungsarten
                                                              ausgewertet.

                                   Lagerstatistik             Über die Lagerstatistik können Sie verschiedene
                                                              Kennzahlen nach definierten Zeiträumen betrachten.

                                   Voreinstellungen           Keine
5.20 / 04-2020




                 G-88                                                                    A+W Business Fertigung
                 Tutorial                                                                              Lagerwirtschaft




                                          Lagerabfrage
                                          Mit verschiedenen Abfragen können Sie sich einen Überblick über die Bu-
                                          chungen, den Gesamtwert des Lagerbestands, statistische Auswertungen
                                          und eine Übersicht über Reservierungen anzeigen lassen.
                                          Damit kann auch nachverfolgt werden, welche Daten von wem geändert wur-
                                          den.

                                          Buchungsjournal
                                          Das Buchungsjournal enthält Auswertungen zu den Lagerbuchungen, die aus
                                          Aufträgen und Bestellungen rühren. Sie können sich z. B. die Lagerbuchun-
                                          gen pro Produkt anzeigen lassen.

                                          Lagerhistorie
                                          Über die Historie können Sie sich einen Überblick über das Tagesgeschehen
                                          im Lager pro Produkt verschaffen.

                                          Lagerstatistik
                                          Die Lagerstatistik gibt Ihnen Aufschluss darüber, welche Ihrer Lagerartikel
                                          Renner und welche Ladenhüter sind. Damit haben Sie ein Kriterium, ob Artikel
                                          in das Lager auf- bzw. herausgenommen werden sollten.
                                          Die Entwicklung einzelner Lagerartikel kann über einen gewählten Zeitraum
                                          betrachtet werden, z. B. über ein ganzes Jahr oder nur über einen Monat.
                                          Die Auswertungen zeigen Anfangs- bzw. Endbestände und Zu- bzw. Abgänge
                                          Ihrer Lagerartikel pro Monat. Damit können Sie sich über die Umschlagshäu-
                                          figkeit, die durchschnittliche Lagerdauer und den durchschnittlichen Lagerbe-
                                          stand Ihrer Lagerartikel informieren.

                                          Lagerbewertung
                                          Der aktuelle Lagerwert des gesamten Lagers kann jederzeit und außerhalb
                                          der Inventur abgefragt werden.
                                          Daneben werden in der Lagerverwaltung zu jedem einzelnen Lagerartikel der
                                          höchste, niedrigste und Durchschnitts-EK und der zugehörige Lagerwert an-
                                          gezeigt.

                                          Reservierte Lagerartikel
                                          Lagerartikel, die durch Aufträge reserviert sind, können pro Nummernverwal-
                                          ter aufgelistet werden. In der Ausgabe werden die reservierten Lagerartikel
                                          pro Artikelnummer und Lagerort dargestellt.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-89
                 Lagerwirtschaft                                                                         Tutorial




                                   Buchungsjournal anzeigen
                                   In dieser Einheit lernen Sie, wie Sie welche Kriterien im Buchungsjournal und/
                                   oder in der Lagerhistorie einsetzen können. Diese beiden Dialoge sind analog
                                   aufgebaut, geben aber unterschiedliche Sachverhalte wieder:
                                   •   Im Buchungsjournal werden alle automatisch durchgeführten Buchungen
                                       angezeigt. Aufträge können nur so lange herangezogen werden, wie sie
                                       nicht archiviert und gelöscht sind.
                                   •   In der Lagerhistorie werden alle manuellen und automatischen Buchun-
                                       gen, Neuanlagen, Umbuchungen und Korrekturen aus der Inventur ange-
                                       zeigt.
                                   In dieser Anleitung werden die beiden Dialoge am Beispiel Buchungsjournal
                                   beschrieben.


                                    So lassen Sie sich Reservierungen anzeigen
                                   1 Wählen Sie im Menü Lagerwirtschaft > Abfragen > Buchungsjournal.

                                                     A        B                          C         D




                                   A Buchungsart                           C Artikel
                                   B Abfragezeitraum                       D Artikelauswahl
                                   Abb. G-41    Buchungsjournal


                                        Softwarereferenz, “Buchungsjournal” auf Seite G-202
                                       Sie können die Anzeige der Buchungen mit verschiedenen Filtern ein-
                                       schränken, z. B. auf einen Artikel.
5.20 / 04-2020




                 G-90                                                                   A+W Business Fertigung
                 Tutorial                                                                                    Lagerwirtschaft




                                          2 Wählen Sie im Feld Buchungsart (A) den Eintrag reserviert aus.
                                             Wenn Sie das Feld frei lassen, werden alle Buchungen angezeigt.
                                          3 Grenzen Sie die Anzeige ggf. weiter ein, z. B. auf einen Artikel (C, D) und
                                            einen Zeitraum (B).
                                          4 Wählen Sie im Menü Start > Ausführen, um das Buchungsjournal zu erzeu-
                                            gen.




                                          Abb. G-42    Buchungsjournal – Ergebnis


                                             Die Reservierungen werden in der Übersicht aufgelistet. Wenn Sie die An-
                                             zeige nicht weiter eingeschränkt haben, werden alle Aufträge und Bestel-
                                             lungen berücksichtigt, die noch nicht archiviert sind.
                                             Auf die gleiche Weise können Sie sich jede einzelne Buchungsart auswer-
                                             ten lassen.
                                              Softwarereferenz, “Buchungsjournal” auf Seite G-202
                                              Softwarereferenz, “Lagerhistorie – Tabelle” auf Seite G-208
5.20 / 04-2020




                 A+W Business Fertigung                                                                               G-91
                 Lagerwirtschaft                                                                          Tutorial




                                   Reservierte Lagerartikel drucken
                                   Reservierungen werden in den Dialogen Buchungsjournal, Lagerhistorie und
                                   Lagerinfo angezeigt. Im Dialog Reservierte Lagerartikel erhalten Sie eine
                                   schnelle Übersicht über die Reservierungen aus Aufträgen in einem Num-
                                   mernverwalter. In dieser Einheit lernen Sie, wie Sie sich eine Liste dieser re-
                                   servierten Lagerartikel ausdrucken lassen.


                                    So drucken Sie sich die Liste der reservierten Lagerartikel
                                   1 Wählen Sie im Menü Lagerwirtschaft > Abfragen > Reservierte Lagerarti-
                                     kel.
                                      Der Dialog Reservierungen wird geöffnet.
                                       Softwarereferenz, “Reservierte Lagerartikel” auf Seite G-215
                                   2 Wählen Sie den Nummernverwalter aus, in dem die aktuellen Aufträge ge-
                                     sammelt sind.




                                      Abb. G-43    Reservierte Lagerartikel


                                      Die Aufträge werden im Bereich Tabelle aufgelistet. Sie können die Liste
                                      aus der Bildschirmanzeige heraus drucken. Über Menü Druck > Drucker
                                      können Sie die Liste direkt drucken.
                                   3 Wählen Sie im Menü Druck > Bildschirm, um sich die Liste auf den Bild-
                                     schirm anzeigen zu lassen.
5.20 / 04-2020




                 G-92                                                                    A+W Business Fertigung
                 Tutorial                                                                                Lagerwirtschaft




                                          4 Wählen Sie aus, wo der Druck umgebrochen werden soll.
                                          5 Klicken Sie auf [OK], um die Einstellungen zu übernehmen.
                                             Der Dialog Druck - Lagerprotokoll wird geöffnet.
                                             Wenn Sie die Ausgabe auf dem Bildschirm gewählt haben, wird die Liste
                                             der reservierten Lagerartikel angezeigt.




                                             Abb. G-44   Reservierte Lagerartikel – Ausgabe auf dem Bildschirm


                                             Die reservierten Lagerartikel werden pro Artikelnummer und Lagerort auf-
                                             gelistet. Bei mehreren Lagerorten wird die Gesamtsumme angezeigt.
                                             Mit den Schaltflächen können Sie vor- und zurückblättern, wenn die Liste
                                             mehr als eine Seite hat.
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-93
                 Lagerwirtschaft                                                                                    Tutorial




                                             Lagerstatistik anzeigen
                                             In dieser Einheit lernen Sie, wie Sie sich in der Lagerstatistik verschiedene
                                             Lagerkennzahlen eines Produkts anzeigen lassen können.


                                              So lassen Sie sich die Statistik zu Lagerbeständen anzeigen
                                             1 Wählen Sie im Menü Lagerwirtschaft > Abfragen > Lagerstatistik.
                                                Der Dialog Statistik wird geöffnet.
                                                 Softwarereferenz, “Lagerstatistik – Produkte” auf Seite G-210
                                                Sie können die Anzeige auf ein Produkt und/oder einen Zeitraum ein-
                                                schränken. Wenn Sie keine Auswahl treffen, werden alle Produkte ange-
                                                zeigt.




                    Abb. G-45      Lagerstatistik – Produktauswahl


                                             2 Wählen Sie im Menü Start > Ausführen, um die Auswertung zu erstellen.
                                                Die Produkte werden den Filtereinstellungen entsprechend aufgelistet.
5.20 / 04-2020




                 G-94                                                                               A+W Business Fertigung
                 Tutorial                                                                               Lagerwirtschaft




                                           3 Markieren Sie einen Eintrag und wechseln Sie zum Register Statistik, um
                                             die Details auszuwerten.




                    Abb. G-46   Lagerstatistik – Statistik


                                               Die Werte zum ausgewählten Produkt werden aufgelistet, z. B. die Bestän-
                                               de und Zu- und Abgänge pro Monat, die Umschlagshäufigkeit und Lager-
                                               dauer. In der Summenzeile werden die summierten Werte des angezeigten
                                               Zeitraums angezeigt.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-95
                 Lagerwirtschaft                                                                         Tutorial




                                   Übungen
                                   •   Prüfen Sie im Buchungsjournal die Reservierungen für das Float 4 mm.
                                   •   Drucken Sie die Reservierungen eines Float 5 mm für den nächsten Monat
                                       aus.


                                   Ergänzende Informationen
                                    Softwarereferenz, “Buchungsjournal” auf Seite G-202
                                    Softwarereferenz, “Lagerhistorie” auf Seite G-204
                                    Softwarereferenz, “Lagerstatistik” auf Seite G-209
                                    Softwarereferenz, “Reservierte Lagerartikel” auf Seite G-215
5.20 / 04-2020




                 G-96                                                                     A+W Business Fertigung
                 Tutorial                                                                                     Lagerwirtschaft




                                          Lagerinformationen
                                          Lernziele

                                          • Dialog Lagersuche kennenlernen.
                                          • Änderungen im Bestand und bei den Reservierungen erkennen.


                                          Nutzen

                                          • Mit dem Überblick über die zukünftigen Lagerbestände und Reservierungen
                                            erhalten Sie ein weiteres Mittel zur Pflege der Bestände.
                                          • Sie können erkennen, wann weitere Bestellungen erfasst werden müssen, damit
                                            die Produktion nicht unterbrochen wird.


                                          Merke

                                          Lagerbestand              Der Lagerbestand wird beim Wareneingang von
                                                                    Lagerartikeln und nach der Abbuchung aktualisiert.
                                                                    Die Abbuchung wird angestoßen, wenn der Lieferschein
                                                                    oder die Rechnung zu einem Auftrag gedruckt wird.

                                          Voreinstellungen          Stammdaten
                                                                    • Lieferantenkartei:
                                                                      Lieferzeit Tage (Wiederbeschaffungszeit)
                                                                    • Statuszuordnung
                                                                    Firmendaten
                                                                    • Register Lager / EK / EDI > Lagervorschau
                                                                    Lagerverwaltung
                                                                    • Register Lager-Artikel > Hauptartikel
5.20 / 04-2020




                 A+W Business Fertigung                                                                                G-97
                 Lagerwirtschaft                                                                                  Tutorial




                                           Lagersuche
                                           Im Dialog Lagersuche können Sie sich alle Lagerartikel pro Lagerort und Ab-
                                           messung anzeigen lassen. Diesen Dialog können Sie auch bei der Positions-
                                           erfassung öffnen. Die Lagersuche ist dann bereits auf einen Lagerartikel
                                           eingeschränkt.




                 A




                        B                      C                          D
                 A Filter zum Einstellen der Suche C Wird als Lagermaß geführt, ist D Bestellartikel, die nicht auf Lager
                 B Wird als Lagerartikel geführt und aber kein Lagerartikel auf Lager, geführt werden, z. B. Lagermaße mit
                   entsprechend gebucht              z. B. Bandmaße bei qm-Lager       der Beschaffungsart Bestellung

                 Abb. G-47    Lagerinfo – Lagersuche


                                           Bestand
                                           Die Berechnung des Bestands ist abhängig von dem Modus, in dem Sie das
                                           Lager führen. Diese Zusammenhänge haben Sie ganz am Anfang der Schu-
                                           lung kennengelernt.
                                            “Wie soll das Lager geführt werden” auf Seite G-17
                                           Bei der Berechnung von qm-Artikeln wird neben der Reservierung auch der
                                           Verschnitt berücksichtigt. Wenn Sie einem oder mehreren Artikeln einen
                                           Hauptartikel zugeordnet haben, wird der Bestand nicht mehr für die einzelnen
5.20 / 04-2020




                                           Artikel angezeigt.
                                           Bei der Erfassung eines Auftrags wird die Stückzahl oder die Anzahl der Qua-
                                           dratmeter (qm-Zahl) der Lagerartikel automatisch für den Kundenauftrag re-


                 G-98                                                                             A+W Business Fertigung
                 Tutorial                                                                                   Lagerwirtschaft




                                          serviert. Die Lagerabbuchung erfolgt dann automatisch bei Lieferschein- oder
                                          Rechnungsdruck.


                                          Lagerinfo und zukünftiger Lagerbestand
                                          Eine detaillierte Ansicht im Dialog Lagerinfo gibt Auskunft über Liefertermin,
                                          Menge, Reservierungen usw. Dabei werden die verfügbaren Lagermaße einer
                                          Größe pro Lagerort angezeigt.




                 A




                 B




                 C




                 A Ausgewählter Lagerartikel                            C Lagerartikel, die mit dem Hauptartikel verknüpft
                 B Vorschau                                               sind

                 Abb. G-48   Lagerinfo – Zukünftiger Lagerbestand


                                          Der zukünftige Lagerbestand wird in drei Listen dargestellt:
                                          •    In der ersten Liste (A) ist der ausgewählte Lagerartikel aufgeführt. Wenn
                                               dies ein Lagerhauptprodukt ist, werden in der dritten Liste die verknüpften
                                               Lagerartikel aufgeführt.
                                          •    In der zweiten Liste (B) finden Sie die Vorschau auf die nächsten Tage. Die
                                               Anzahl der Tage können Sie in den Firmendaten festlegen.
                                          •    In der dritten Liste (C) sind die Lagermaße aufgeführt, die mit dem Haupt-
                                               lagerartikel verknüpft sind.
                                               Dazu kann auch der kritische Lagerbestand angezeigt werden.
5.20 / 04-2020




                                          Mit farblichen Markierungen werden Probleme für die erfassten Aufträge an-
                                          gezeigt:



                 A+W Business Fertigung                                                                                G-99
                 Lagerwirtschaft                                                                                  Tutorial




                                           •   Rot: Termine können nicht eingehalten werden.
                                           •   Gelb: Die Wiederbeschaffungszeit reicht aus.


                         A    B           C




                       I                             H           G           F        E                  D
                 A   Ausgewählter Lagerartikel                       F Offene Bestellungen zum jeweiligen Datum
                 B   Angezeigter Zeitraum                              (Liefertermin)
                 C   Lagerort                                        G Reservierung zum Datum
                 D   Mindestbestand aus der Lagerverwaltung          H Bestand zum Datum
                 E   Errechneter Endbestand = H - G + F              I Abmessung des Lagerartikels

                 Abb. G-49    Anzeige des zukünftigen Bestands


                                           Offene Bestellmengen (F) zu einem Lagerartikel werden angezeigt, bis der
                                           Wareneingang verbucht wurde. Danach wird der aktuelle Bestand der gelie-
                                           ferten Menge aktualisiert.

                                           Wiederbeschaffungszeit
                                           Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferan-
                                           tenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferan-
                                           ten, die in der Tourenverwaltung hinterlegt sind.
5.20 / 04-2020




                                           Wenn Sie eine Auftragsposition erfassen, können Sie den zukünftigen Lager-
                                           bestand abfragen. Wenn der Mindestbestand (D) zu einem bestimmten Termin
                                           unterschritten wird, können zwei Fälle eintreten:



                 G-100                                                                          A+W Business Fertigung
                 Tutorial                                                                               Lagerwirtschaft




                                          •   Die Wiederbeschaffungszeit für den Artikel reicht aus, um die Ware bis zu
                                              dem Termin nachzubestellen. In der Lagervorschau werden die entspre-
                                              chenden Zeilen gelb markiert.
                                          •   Die Wiederbeschaffungszeit reicht nicht aus. In der Lagervorschau werden
                                              die entsprechenden Zeilen rot markiert.
                                          Bei der Erfassung eines Dokuments können Sie dann den Lieferanten und/
                                          oder den Liefertermin ändern. In der Einheit Auftragserfassung von Lagerarti-
                                          keln ist dies ausführlich beschrieben.
                                           “Lagerartikel für Position suchen” auf Seite G-120

                                          Einstellungen zu Lagerverfügbarkeit und Wiederbeschaffungszeit
                                          Zur Berechnung der zukünftigen Bestände werden vom aktuellen Bestand alle
                                          Reservierungen pro Tag abgezogen und bestellte Mengen addiert. Daraus er-
                                          gibt sich der voraussichtliche Lagerbestand abhängig vom Tagesdatum.
                                          Um die Performance zu erhöhen, können Sie die Anzeige im Dialog Lagerinfo
                                          durch folgende Einstellungen einschränken:
                                          •   Im Dialog Produktverwaltung > Register Lager/Einkauf > Checkbox keine
                                              Verfügbarkeitsprüfung können Sie bestimmte Artikel aus der Lagervor-
                                              schau und der Verfügbarkeitsprüfung herausnehmen, indem Sie die Ver-
                                              fügbarkeitsprüfung für diese Artikel ausschalten.
                                          •   Im Dialog Firmendaten können Sie einstellen, über welchen Zeitraum die
                                              Vorschau dargestellt werden soll. In der Regel reichen zwei bis vier Wo-
                                              chen aus. Wenn Sie eine Null eintragen, wird die Vorschau für 14 Tage an-
                                              gezeigt.
                                          •   Im Dialog Lagerverwaltung können Sie mehrere Lagermaße miteinander
                                              verknüpfen. Damit wird erreicht, dass Sie nur für den Hauptartikel einen
                                              Mindestbestand hinterlegen müssen, gegen den die Bestandsprüfung
                                              durchgeführt wird. Diese Funktion haben Sie bereits in der Einheit Lager-
                                              verwaltung kennengelernt.
                                               “Lager-Hauptartikel” auf Seite G-70

                                          Buchungstermine
                                          Um eine konkrete Aussage über den Lagerbestand zu einem bestimmten Ter-
                                          min treffen zu können, müssen alle Wareneingänge und Warenausgänge mit
                                          einem voraussichtlichen Buchungsdatum versehen werden.
                                          Die voraussichtlichen Buchungstermine werden bei der Erfassung der Positi-
                                          onen wie folgt festgelegt:
                                          •   Stücklistenelemente und Produkte mit der Beschaffungsart Lagerentnah-
                                              me, die zugeschnitten werden müssen, werden zum Datum des Produkti-
                                              onsstarts eingetragen.
                                          •   Für alle anderen Lagerartikel wird als Buchungsdatum das Lieferdatum
                                              aus dem Dokument verwendet.
                                          Wenn der Auftrag anschließend in AWCapacity Planning eingelastet wird, so
                                          werden diese voraussichtlichen Termine durch die berechneten, tatsächlichen
5.20 / 04-2020




                                          Termine ersetzt.




                 A+W Business Fertigung                                                                         G-101
                 Lagerwirtschaft                                                                                  Tutorial




                                             Bestände in der Lagersuche anzeigen
                                             Lagerbestände werden durch die Buchungen von Warenein- und -ausgängen
                                             aktualisiert. Das Lager ist eng gekoppelt mit den Dokumenten für den Verkauf
                                             und den Einkauf. Beim Erfassen von Dokumenten kann der aktuelle Lager-
                                             bestand daher über die Lagerinfo jederzeit erfragt werden.
                                             Der aktuelle Lagerbestand wird auch bei der Erfassung von Angeboten, Auf-
                                             trägen und bei der Bestellung angezeigt. Dabei werden sowohl die Bestellun-
                                             gen als auch die Reservierungen berücksichtigt.
                                             In dieser Einheit lernen Sie, wie Sie sich die Bestände und Reservierungen
                                             von Lagerartikeln anzeigen lassen.

                                                 Dialog Lagersuche öffnen
                                                 Der Dialog Lagersuche steht auch über das Modul Dokumente zur Verfü-
                                                 gung. Damit kann schon bei der Erfassung eines Auftrags geprüft werden,
                                                 ob die gewünschten Produkte in ausreichender Menge verfügbar sind.


                                              So lassen Sie die Bestände von Lagerartikeln anzeigen
                                             1 Wählen Sie im Menü Lagerwirtschaft > Suche.




                    A




                    B




                    A Produkt – Lagerartikel                                 B Filter
5.20 / 04-2020




                    Abb. G-50      Filter für die Suche nach Lagerartikeln


                                                  Softwarereferenz, “Suche” auf Seite G-217



                 G-102                                                                          A+W Business Fertigung
                 Tutorial                                                                            Lagerwirtschaft




                                          2 Schränken Sie die Suche ein, indem Sie z. B. ein Produkt (A) auswählen.
                                          3 Wählen Sie im Bereich Filteroptionen (B) aus, welche Lagerartikel ange-
                                            zeigt werden sollen.
                                             Wenn Sie die Einstellung Lagerware deaktivieren, werden nur die Lager-
                                             maße angezeigt, die im Dialog Produktverwaltung Lagermaße angelegt
                                             sind, unabhängig davon, ob es sich um echte Lagerartikel handelt, das
                                             heißt, Lagerartikel aus der Lagerverwaltung.
                                          4 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.
                                             Die Trefferliste wird in der Übersicht angezeigt.




                    Abb. G-51   Ergebnis der Suche


                                             In diesem Beispiel wurde nach dem Produkt Float 5 mm gesucht.
                                          5 Wenn Sie sich die korrespondierenden Dokumente anzeigen lassen möch-
                                            ten, markieren Sie eine Zeile und öffnen das Kontextmenü (rechte Maus-
                                            taste).
                                          6 Klicken Sie auf korrespondierende Dokumente.
5.20 / 04-2020




                 A+W Business Fertigung                                                                      G-103
                 Lagerwirtschaft                                                                                Tutorial




                                                Abb. G-52     Korrespondierende Dokumente


                                                In diesem Dialog werden alle Aufträge und Bestellungen angezeigt, in de-
                                                nen das Produkt erfasst wurde.
                                             7 Klicken Sie auf [Ende], um den Dialog zu schließen.
                                                Der Dialog Lagersuche wird wieder angezeigt.
                                             8 Wenn Sie die nächsten Warenabgänge und -zugänge zu einem Produkt
                                               oder den zukünftigen Lagerbestand anschauen möchten, markieren Sie
                                               das Produkt und wechseln zum Register Zukünftiger Lagerbestand.
5.20 / 04-2020




                    Abb. G-53      Zukünftiger Lagerbestand




                 G-104                                                                         A+W Business Fertigung
                 Tutorial                                                                           Lagerwirtschaft




                                          Der zukünftige Lagerbestand wird für den Zeitraum in der Zukunft ange-
                                          zeigt, den Sie in den Firmendaten für die Vorschau eingetragen haben. Die
                                          Sonn- und Feiertage werden mit angezeigt, jedoch nicht mitgezählt.
5.20 / 04-2020




                 A+W Business Fertigung                                                                     G-105
                 Lagerwirtschaft                                                                        Tutorial




                                   Übungen
                                   •   Prüfen Sie den Bestand und die Reservierungen für Float 4 mm.
                                       Notieren Sie sich die einzelnen Werte aus dem Register Zukünftiger Lager-
                                       bestand. In der nächsten Einheit werden Sie eine Bestellung erfassen und
                                       anschließend prüfen, wie sich die Werte geändert haben.


                                   Ergänzende Informationen
                                    Softwarereferenz, “Suche” auf Seite G-217
5.20 / 04-2020




                 G-106                                                                A+W Business Fertigung
                 Tutorial                                                                                    Lagerwirtschaft




                                          Lagerbestellung (automatisch)
                                          Lernziele

                                          •   Dialog Lagerbestellung kennenlernen.
                                          •   Automatische Lagerbestellung kennenlernen.
                                          •   Automatisch ausgelöste Bestellvorschläge an den Einkauf übergeben.
                                          •   Änderung der angezeigten Werte im zukünftigen Lagerbestand prüfen.


                                          Nutzen

                                          • Mit Bestellungen ergänzen Sie die Lagerbestände auf den gewünschten
                                            Sollbestand oder den Reservierungen entsprechend.
                                          • Wenn der Mindestbestand unterschritten wird, wird automatisch ein
                                            Bestellvorschlag erzeugt. Diesen können Sie im Dialog Lagerbestellung prüfen
                                            und dann an den Einkauf übergeben.


                                          Merke

                                          Lagerbestellung manuell     Lagerbestellungen werden im Modul Dokumente erfasst
                                          erfassen                    und bearbeitet.
                                                                      Dieser Vorgang ist im Part Einkauf beschrieben.

                                          Bestellvorschläge           Automatische Bestellvorschläge werden ausgelöst,
                                                                      wenn die definierte Mindestmenge unterschritten wird.
                                                                      Dabei werden Reservierungen und offene Bestellungen
                                                                      berücksichtigt.
                                                                      Die Bestellvorschläge werden automatisch erzeugt und
                                                                      manuell an den Einkauf übergeben. Erst durch die
                                                                      Übergabe wird eine Bestellung erzeugt, die an den
                                                                      Lieferanten gesendet werden kann.

                                          Voreinstellungen            Stammdaten:
                                                                      • Produktverwaltung
                                                                      • Lieferantenkartei
                                                                      Firmendaten:
                                                                      • Register Parameter
                                                                      • Register Lager / EK / EDI
                                                                      Lagerverwaltung
                                                                      • Mindestbestand
                                                                      • Bestellmenge
5.20 / 04-2020




                 A+W Business Fertigung                                                                                 G-107
                 Lagerwirtschaft                                                                              Tutorial




                                         Bestellvorschläge
                                         In der Regel werden Bestellungen aus der Lagerwirtschaft heraus erzeugt, um
                                         die Bestände auf dem gewünschten Niveau zu halten.




                 A
                 B




                 A Mindestbestand                                  B Menge für Bestellvorschlag
                 Abb. G-54   Lagerverwaltung – Bestandszahlen


                                         Wenn Sie im Dialog Lagerverwaltung Mindestmengen (A) für einen Lagerarti-
                                         kel hinterlegt haben, werden Bestellvorschläge automatisch mit der hinterleg-
                                         ten Bestellmenge (B) erzeugt. Sie können diese vor der Übergabe an den
                                         Einkauf prüfen und ggf. den Lieferanten und den Termin ändern. Mit der Über-
                                         gabe an den Einkauf wird aus dem Vorschlag eine Lagerbestellung erzeugt.
                                         Lagerbestellungen können auch manuell über die Dokumentenverwaltung er-
                                         zeugt werden. Die manuelle Lagerbestellung lernen Sie in einer separaten
                                         Einheit kennen.
                                          “Manuelle Lagerbestellung” auf Seite G-127
5.20 / 04-2020




                 G-108                                                                      A+W Business Fertigung
                 Tutorial                                                                                Lagerwirtschaft




                                          Lagerbestellung an den Einkauf übergeben
                                          Automatisch erzeugte Bestellvorschläge werden im Dialog Lagerbestellung –
                                          Bestellpool angezeigt. Sie können den Lieferanten und den Termin ändern.
                                          Mit der Übergabe an den Einkauf erzeugen Sie die Bestellung. Diese muss
                                          dann an den Lieferanten gesendet werden.
                                          Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im
                                          Bestellpool die Liefertermine und Preise vergleichen und einen anderen Lie-
                                          feranten auswählen.
                                          In dieser Einheit lernen Sie, wie Sie einen Bestellvorschlag an den Einkauf
                                          übergeben.

                                              Dialog Lagerbestellung
                                              Der Dialog Lagerbestellung – Bestellpool ist nahezu identisch wie der Dia-
                                              log Bestellübergabe aufgebaut, den Sie aus der Schulung zum Einkauf
                                              kennen. Es handelt sich jedoch um verschiedene Dialoge. Sie werden da-
                                              her für jeden Bestellvorschlag genau einen Eintrag finden, zu dem es keine
                                              referenzierten Dokumente gibt.

                                          Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                          •   “So übergeben Sie die Bestellvorschläge an den Einkauf” auf Seite G-109
                                          •   “So ändern Sie den Lieferanten und den Liefertermin” auf Seite G-112


                                           So übergeben Sie die Bestellvorschläge an den Einkauf
                                          1 Wählen Sie im Menü Lagerwirtschaft > Lagerbestellung.
                                              Der Dialog Lagerbestellung wird geöffnet.
                                               Softwarereferenz, “Lagerbestellung” auf Seite G-220
                                              Wenn Sie die Bestellvorschläge nicht für das gesamte Lager anzeigen las-
                                              sen wollen, können Sie die Anzeige auf bestimmte Lagerorte einschrän-
                                              ken.
                                          2 Stellen Sie zur Einschränkung der Anzeige in den Feldern Warenhaus,
                                            Gang, Regal und Fach den gewünschten Lagerort ein.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-109
                 Lagerwirtschaft                                                                                  Tutorial




                    Abb. G-55      Lagerbestellung


                                                In diesem Beispiel wird kein Lagerort ausgewählt, damit der Bestand aller
                                                Lagerorte aufgelistet wird.
                                            3 Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.
                                                Die Vorschläge werden eingelesen und in der Übersicht aufgelistet.
5.20 / 04-2020




                 G-110                                                                          A+W Business Fertigung
                 Tutorial                                                                             Lagerwirtschaft




                    Abb. G-56   Lagerbestellung – Bestellvorschläge


                                          4 Markieren Sie die Bestellvorschläge, die Sie an den Einkauf übergeben
                                            möchten.

                                             Einträge gemeinsam markieren
                                             Sie können Bestellvorschläge gemeinsam markieren, indem Sie über das
                                             Menü Funktionen den Dialog Markierungsoptionen öffnen. Wenn Sie in
                                             diesem Dialog z. B. ein gestimmtes Produkt angeben, werden alle Bestell-
                                             vorschläge zu diesem Produkt mit einem Kreuz im Zeilenkopf markiert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-111
                 Lagerwirtschaft                                                                                  Tutorial




                    Abb. G-57      Markierte Bestellvorschläge


                                                Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge
                                                sind markiert, die mit einem X gekennzeichnet sind.
                                             5 Wählen Sie im Menü Start > Ausführen, um die Übergabe an den Einkauf
                                               zu starten.
                                                Bestätigen Sie die Meldung zur Anzahl der übergebenen Vorschläge.
                                                Die Bestellungen werden erzeugt und die übergebenen Vorschläge wer-
                                                den aus der Liste gelöscht.


                                              So ändern Sie den Lieferanten und den Liefertermin
                                             1 Lesen Sie im Dialog Lagerbestellung die Bestellvorschläge ein, wie oben
                                               beschrieben.
                                             2 Markieren Sie den Vorschlag, zu dem Sie den Lieferanten und/oder Liefer-
                                               termin ändern wollen.
                                                Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge
                                                sind markiert, die mit einem X gekennzeichnet sind.
5.20 / 04-2020




                 G-112                                                                          A+W Business Fertigung
                 Tutorial                                                                            Lagerwirtschaft




                    Abb. G-58   Vorschlag, dem ein anderer Lieferant zugeordnet werden soll


                                          3 Wählen Sie im Menü Funktionen > Lieferant/Liefertermine ändern.




                                             Abb. G-59     Liefertermin ändern


                                          4 Tragen Sie einen anderen Lieferanten und/oder Liefertermin ein.
                                          5 Klicken Sie auf [OK], um die Änderung zu übernehmen.
                                             Der Dialog Lieferant und Liefertermin ändern wird geschlossen. In der
                                             Übersicht wird der Vorschlag mit dem neuen Lieferanten und/oder Liefer-
5.20 / 04-2020




                                             termin angezeigt.
                                             Sie können den Bestellvorschlag jetzt an den Einkauf übergeben.



                 A+W Business Fertigung                                                                        G-113
                 Lagerwirtschaft                                                                                    Tutorial




                                             Preise vor der Übergabe vergleichen
                                             Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie die
                                             Preise vor der Übergabe vergleichen und einen anderen Lieferanten auswäh-
                                             len. In dieser Einheit lernen Sie, wie Sie die Preise vergleichen und den güns-
                                             tigsten oder schnellsten Lieferanten auswählen können.


                                              So vergleichen Sie die Preise in einem Bestellvorschlag
                                             1 Wählen Sie im Menü Lagerwirtschaft > Lagerbestellung.
                                                 Der Dialog Lagerbestellung wird geöffnet.
                                                  Softwarereferenz, “Lagerbestellung” auf Seite G-220
                                             2 Wählen Sie in den Feldern Warenhaus, Gang, Regal und Fach den ge-
                                               wünschten Lagerort ein.
                                             3 Wählen Sie im Menü Start > Ausführen, um die Bestellvorschläge einzule-
                                               sen.
                                                 Die Vorschläge werden eingelesen und in der Übersicht aufgelistet.
                                             4 Markieren Sie den Vorschlag, zu dem Sie die Preise der Lieferanten ver-
                                               gleichen wollen.
                                                 Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge
                                                 sind markiert, die mit einem X gekennzeichnet sind.
5.20 / 04-2020




                    Abb. G-60      Position, zu der die Preise verglichen werden sollen


                 G-114                                                                             A+W Business Fertigung
                 Tutorial                                                                                    Lagerwirtschaft




                                          5 Wählen Sie im Menü Funktionen > Lieferantenpreise.

                                                           A       B         C          D




                                                                         H

                                                       E
                                                       F
                                                       G

                                          A Standard-Lieferant (Textfarbe rot)  E    Textfarbe rot: Standard-Lieferant
                                          B Checkbox des Standard-Lieferanten F      Textfarbe grün: preisgünstigster Lieferant
                                            (abgewählt)                         G    Textfarbe blau: Standard-Lieferant ist am
                                          C Ausgewählter Lieferant für aktuelle      preisgünstigsten
                                            Bestellung                          H    !!! bei allen Textfarben: Liefertermin
                                          D Checkbox zur Auswahl des                 möglicherweise zu spät für rechtzeitige
                                            Lieferanten (markiert)                   Produktion und Auslieferung an Kunden
                                          Abb. G-61    Lieferanten für markierte Position ändern


                                          6 Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung
                                            der Position gesendet werden soll.
                                          7 Klicken Sie auf [OK], um die Änderung zu übernehmen.
                                             Der Dialog Preisvergleich wird geschlossen. In der Übersicht wird der Vor-
                                             schlag mit dem neuen Lieferanten und/oder Liefertermin angezeigt.
                                             Sie können den Bestellvorschlag jetzt an den Einkauf übergeben.
                                              “So übergeben Sie die Bestellvorschläge an den Einkauf” auf Seite G-109
5.20 / 04-2020




                 A+W Business Fertigung                                                                                G-115
                 Lagerwirtschaft                                                                        Tutorial




                                   Übungen
                                   •   Richten Sie die Mindest- und die Bestellmenge eines Lagerartikels so ein,
                                       dass ein automatischer Bestellvorschlag erzeugt wird. Wählen Sie dazu
                                       den Lagerartikel aus, für den Sie in der vorigen Übung die Werte aus dem
                                       zukünftigen Lagerbestand notiert haben.
                                   •   Prüfen Sie einen Bestellvorschlag und ändern Sie den Lieferanten oder der
                                       Liefertermin. Wenn keine alternativen Lieferanten angezeigt werden, müs-
                                       sen Sie die Lieferantenkartei in den Stammdaten prüfen und anpassen.
                                   •   Übergeben Sie die Bestellvorschläge an den Einkauf.
                                   •   Prüfen Sie im Dialog Lagersuche, wie sich die Werte geändert haben.


                                   Ergänzende Informationen im Part Verkauf
                                    Verkauf, “Auftragskopf” auf Seite C-39
                                    Verkauf, “Bestellkennzeichen ändern” auf Seite C-310
                                    Einkauf, “Lieferantenkartei anpassen” auf Seite D-33
                                    Einkauf, “Dokument Bestellung” auf Seite D-45
                                    Einkauf, “Wareneingang erfassen” auf Seite D-127
                                    Einkauf, “Kistengeschäft” auf Seite D-136
5.20 / 04-2020




                 G-116                                                                  A+W Business Fertigung
                 Tutorial                                                                  Lagerartikel in Dokumenten




                                          Lagerartikel in Dokumenten
                                          In diesem Themenblock lernen Sie, wie Aufträge und manuelle Bestellungen
                                          auf die Lagerwirtschaft zugreifen.
                                          Dazu gehören folgende Lerneinheiten:
                                          •   “Auftragserfassung von Lagerartikeln” auf Seite G-118
                                          •   “Manuelle Lagerbestellung” auf Seite G-127
                                          •   “Produktionsaufträge” auf Seite G-131
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-117
                 Lagerartikel in Dokumenten                                                                          Tutorial




                                         Auftragserfassung von Lagerartikeln
                                         Lernziele

                                         • Nach Lagerartikeln für die Positionserfassung suchen.
                                         • Reservierung prüfen.
                                         • Änderungen im Lagerbestand nach Änderungen im Auftrag prüfen.


                                         Nutzen

                                         • Bei der Erfassung von Positionen kann die Verfügbarkeit eines Produktes geprüft
                                           werden. Bei Engpässen können der Lieferant oder der Liefertermin direkt im
                                           Dokument geändert werden.


                                         Merke

                                         Positionserfassung         Lagerartikel werden in der Positionserfassung über die
                                                                    Lagersuche [F3] ausgewählt.

                                         Reservierung               Ein im Auftrag erfasster Lagerartikel wird im Lager als
                                                                    reserviert gekennzeichnet.

                                         Voreinstellungen           Stammdaten:
                                                                    • Produktverwaltung
                                                                    • Lieferantenkartei
                                                                    Firmendaten:
                                                                    • Register Parameter
                                                                    • Register Lager / EK / EDI
5.20 / 04-2020




                 G-118                                                                            A+W Business Fertigung
                 Tutorial                                                                     Lagerartikel in Dokumenten




                                          Reservierung und Buchung von Lagerartikeln
                                          Bei der Auftragserfassung wird die Stückzahl oder die Anzahl der Quadrat-
                                          meter (qm-Zahl) der Lagerartikel für den Kundenauftrag reserviert. Die Lager-
                                          abbuchung erfolgt dann automatisch bei Lieferschein- oder Rechnungsdruck.
                                          Über die verkauften und bestellten Mengen errechnet A+W Business die ak-
                                          tuellen Bestände.

                                          Lagerbestand nach Änderung im Auftrag
                                          Was passiert mit dem Lagerbestand, wenn Aufträge geändert werden, für die
                                          bereits ein Warenabgang gebucht wurde? In den folgenden Beispielen wird
                                          der Warenabgang beim Druck des Lieferscheins gebucht.

                                             Änderung im Auftrag      Folge im Auftrag        Lagerbuchung

                                             Auftragskopf ändern,     Status bleibt           Bei erneutem Erst-Druck des
                                             keine Änderung der       unverändert.            Lieferscheins wird kein neuer
                                             Positionen                                       Warenabgang im Lager
                                                                                              gebucht.

                                             Position nachträglich    Status ist bereits 72 und Abfrage, ob der Lagerbestand
                                             löschen                  bleibt unverändert.       korrigiert werden soll.

                                             Position nachträglich                            Abfrage, ob der Lagerbestand
                                             hinzufügen                                       korrigiert werden soll.

                                             Stückzahl nachträglich                           Lagermenge wird automatisch
                                             ändern                                           ohne weiteren Hinweis
                                                                                              korrigiert.


                                          In den nächsten Einheiten lernen Sie, wie Sie einen Lagerartikel in einem Do-
                                          kument erfassen und die Buchung prüfen können.
5.20 / 04-2020




                 A+W Business Fertigung                                                                              G-119
                 Lagerartikel in Dokumenten                                                                         Tutorial




                                         Lagerartikel für Position suchen
                                         In dieser Einheit lernen Sie, wie Sie eine Position erfassen und dabei die Ver-
                                         fügbarkeit des gewünschten Produktes prüfen. Sie öffnen dazu den Dialog La-
                                         gersuche, den Sie bereits in der vorigen Einheit kennengelernt haben.

                                              Lagersuche beim Erfassen einer Bestellung
                                              Die Auswahl eines Lagerartikels über den Dialog Lagersuche können Sie
                                              auch beim Erfassen einer manuellen Lagerbestellung anwenden. Die ma-
                                              nuelle Lagerbestellung ist in der gleichnamigen Einheit beschrieben.

                                               “Manuelle Lagerbestellung” auf Seite G-127


                                          So erfassen Sie einen Lagerartikel als Position
                                         1 Wählen Sie im Menü Dokumente > Auftrag > Auftrag und erfassen Sie ei-
                                           nen Auftragskopf.
                                         2 Wechseln Sie zur Positionserfassung und geben Sie in der Erfassungszei-
                                           le die Produktnummer ein.
                                         3 Wählen Sie im Menü Start > Lagersuche, um den Dialog Lagerinfo zu öff-
                                           nen.
                                              Die Auswahl im Dialog Lagerinfo ist bereits auf den Artikel eingeschränkt,
                                              den Sie in der Position erfasst haben. Sie müssen die Anzeige nun weiter
                                              filtern, indem Sie z. B. die Einstellungen auf Lagermaße und Bestände
                                              über null einschränken.


                                              A                                                         B



                                              A Anzeige von Lagermaßen an- oder       B Nur Lagerartikel mit Bestandsmenge
                                                abschalten                              größer 0 anzeigen
                                              Abb. G-62    Filter für die Suche nach Lagerartikeln
5.20 / 04-2020




                 G-120                                                                               A+W Business Fertigung
                 Tutorial                                                                   Lagerartikel in Dokumenten




                                          4 Wechseln Sie zum Register Zukünftiger Lagerbestand, um zu prüfen, ob
                                            die Produktionstermine gefährdet sind.
                                             Die Anzeige des zukünftigen Lagerbestands im Dialog Lagerinfo haben Sie
                                             bereits in der Einheit Lagerinfo kennengelernt.
                                              “Anzeige des zukünftigen Bestands” auf Seite G-100




                    Abb. G-63   Zukünftiger Lagerbestand


                                             Falls die Wiederbeschaffungszeit zu knapp ist, können Sie das Produkt
                                             dennoch erfassen und anschließend prüfen, ob ein anderer Lieferant ver-
                                             fügbar ist oder ob Sie den Liefertermin ändern müssen.
                                          5 Wechseln Sie zurück zum Register Lagersuche und klicken Sie doppelt auf
                                            den Lagerartikel, den Sie in die Positionserfassung übernehmen wollen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                        G-121
                 Lagerartikel in Dokumenten                                                                    Tutorial




                    Abb. G-64   Lagerartikel auswählen


                                              Der Dialog Lagerinfo wird geschlossen und die Daten in der Positionser-
                                              fassung werden aktualisiert.
                                          6 Erfassen Sie alle Positionsdaten und kehren Sie zurück zum Dokumenten-
                                            kopf.
                                              Wenn die Wiederbeschaffungszeiten nicht ausreichen, können Sie sich die
                                              betroffenen Artikel im Dialog Liefertermin ändern anzeigen lassen.
                                          7 Klicken Sie auf die Symbolschaltfläche neben dem Versandtag, um den Di-
                                            alog zu öffnen.
5.20 / 04-2020




                 G-122                                                                       A+W Business Fertigung
                 Tutorial                                                                     Lagerartikel in Dokumenten




                                                                                                                   A




                                                                                                                   B




                                                                                                                   C




                 A Liefertermin prüfen                                 C Übersicht über die möglichen Lieferanten und
                 B Produkte mit zu geringem Lagerbestand                 Liefertermine zum markierten Produkt

                 Abb. G-65   Liefertermin im Auftrag prüfen


                                              Alternative Lieferanten aus der Lieferantenkartei werden mit der hinterleg-
                                              ten Wiederbeschaffungszeit und dem entsprechenden Termin angezeigt.
                                              Mit einem Doppelklick auf den Artikel in der oberen Liste (B) öffnen Sie den
                                              Dialog Lagerinfo mit den Details zu den Artikeln.
                                           8 Wenn der geplante Liefertermin gefährdet ist, haben Sie folgende Möglich-
                                             keiten:
                                              •   Wechseln Sie den Lieferanten für die fragliche Position oder für den ge-
                                                  samten Auftrag.
                                              •   Ändern Sie den Liefertermin und benachrichtigen Sie den Kunden.
                                                  Diese Handlungsschritte sind im Tutorial zum Verkauf ausführlich be-
                                                  schrieben.
5.20 / 04-2020




                                           9 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                              Die Daten werden gespeichert. Sie können jetzt die Reservierung der La-
                                              gerartikel prüfen.


                 A+W Business Fertigung                                                                            G-123
                 Lagerartikel in Dokumenten                                                                    Tutorial




                                         Buchungen prüfen
                                         In dieser Einheit lernen Sie, wie Sie die Buchungen der Lagerartikel prüfen
                                         können. Die Position wird nach dem Speichern reserviert. Der Warenabgang
                                         wird in der Regel mit dem Druck des Lieferscheins gebucht. Dieser Druck ist
                                         von den Einstellungen in der Statusverwaltung abhängig.
                                          “Statusänderungen durch Zu- und Abgänge” auf Seite G-35


                                          So prüfen Sie die Buchungen
                                         1 Öffnen Sie den Dialog Buchungsjournal, wie in der Einheit Abfragen be-
                                           schrieben.
                                               “Buchungsjournal anzeigen” auf Seite G-90
                                         2 Schränken Sie die Auswahl auf den Auftrag ein, zu dem Sie die Reservie-
                                           rung prüfen wollen.
                                              In der Übersicht werden alle Auftragspositionen mit dem aktuellen Bu-
                                              chungstyp aufgelistet.




                                         Abb. G-66     Buchung – reserviert


                                              Im Buchungsjournal wird die Buchungsart reserviert nur so lange ange-
                                              zeigt, bis der Warenabgang gebucht wurde.
5.20 / 04-2020




                 G-124                                                                       A+W Business Fertigung
                 Tutorial                                                                Lagerartikel in Dokumenten




                                             Nach dem Warenabgang werden die Auftragspositionen als ausgeliefert
                                             gekennzeichnet.




                                          Abb. G-67      Buchung – ausgeliefert


                                             In der Auftragshistorie werden die einzelnen Statusänderungen anhand
                                             des Drucks und der Lagerbuchungen dargestellt.
5.20 / 04-2020




                                             Abb. G-68      Auftragshistorie




                 A+W Business Fertigung                                                                     G-125
                 Lagerartikel in Dokumenten                                                                    Tutorial




                                         Übungen
                                         •    Erfassen Sie einen Auftrag mit vorhandenen Lagerprodukten und prüfen
                                              Sie die Einträge im Buchungsjournal:
                                              – Nach der Erfassung des Auftrags.
                                              – Nach dem Druck des Lieferscheins. Welche Änderungen sehen Sie?
                                         •    Erfassen Sie einen Auftrag und prüfen Sie dabei den Lagerbestand und die
                                              Reservierungen.
                                         •    Erstellen Sie eine Rechnung zu dem Auftrag und prüfen Sie die Lager-
                                              reservierungen erneut.
5.20 / 04-2020




                 G-126                                                                       A+W Business Fertigung
                 Tutorial                                                                     Lagerartikel in Dokumenten




                                          Manuelle Lagerbestellung
                                          Lernziele

                                          • Besonderheiten der Lagerbestellung in der Dokumentenverwaltung kennenlernen.


                                          Nutzen

                                          • Mit manuellen Lagerbestellungen ergänzen Sie Lagerbestände, z. B. für
                                            Großaufträge, zu denen die automatische Nachbestellung nicht ausreicht.


                                          Merke

                                          Dokumententyp              Das Dokument Lagerbestellung ist ein eigener
                                                                     Dokumententyp. Nur bei Bestellungen aus einer
                                                                     Lagerbestellung kann der Wareneingang auf das Lager
                                                                     gebucht werden.

                                          Voreinstellungen           Stammdaten:
                                                                     • Produktverwaltung
                                                                     • Lieferantenkartei
                                                                     Firmendaten:
                                                                     • Register Parameter
                                                                     • Register Lager / EK / EDI
5.20 / 04-2020




                 A+W Business Fertigung                                                                               G-127
                 Lagerartikel in Dokumenten                                                                       Tutorial




                                          Lagerbestellung manuell erfassen
                                          Bestellungen von Lagerartikeln können automatisch ausgelöst oder manuell
                                          erfasst werden. Die automatischen Bestellvorschläge haben Sie bereits in der
                                          Einheit zur automatischen Lagerbestellung kennengelernt.
                                           “Lagerbestellung (automatisch)” auf Seite G-107
                                          In dieser Einheit lernen Sie, wie Sie eine Lagerbestellung manuell erfassen.
                                          Die Erfassung von Dokumenten ist ausführlich in den Parts Verkauf und Ein-
                                          kauf beschrieben. Die folgende Handlungsanleitung konzentriert sich daher
                                          auf die wichtigsten Schritte.


                                           So erfassen Sie eine Lagerbestellung manuell
                                          1 Wählen Sie im Menü Dokumente > Bestellung > Bestellung.
                                               Der Dialog Dokumentenverwaltung wird geöffnet.
                                                Verkauf, “Dokument – Kopfdaten” auf Seite C-417
                                          2 Erfassen Sie den Dokumentenkopf. Tragen Sie mindestens den Lieferan-
                                            ten und das Lieferdatum ein.


                                                                                                                       A




                                                                                                                       B




                 A Dokumententyp                                     B Einstellen des Dokumententyps
5.20 / 04-2020




                 Abb. G-69   Lagerbestellung




                 G-128                                                                             A+W Business Fertigung
                 Tutorial                                                                    Lagerartikel in Dokumenten




                                          3 Wählen Sie im Feld Typ (B) den Eintrag Lagerbestellung.
                                             Wenn Sie einen anderen Dokumententyp einstellen, wird der Warenein-
                                             gang nicht automatisch in den Lagerbestand gebucht.
                                          4 Erfassen Sie die Position(en).

                                             Positionen ohne Lagerkennzeichen
                                             Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lager-
                                             artikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie
                                             können in den Stammdaten Firma > Firmendaten > Register Lager / EK /
                                             EDI jedoch die entsprechende Option aktivieren.

                                              “Firmendaten – Lager / EK / EDI” auf Seite G-32
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert.
                                          6 Drucken und versenden Sie die Bestellung.
                                             Dieser Vorgang ist im Part Verkauf beschrieben.
                                              Tutorial, “Auftragskopf” auf Seite C-39
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-129
                 Lagerartikel in Dokumenten                                                                  Tutorial




                                         Übungen
                                         •    Prüfen Sie die Lagerbestände für einen Lagerartikel.
                                         •    Erfassen Sie eine Lagerbestellung manuell und prüfen Sie im Dialog
                                              Lagerinfo die entsprechenden Werte erneut.
5.20 / 04-2020




                 G-130                                                                      A+W Business Fertigung
                 Tutorial                                                                      Lagerartikel in Dokumenten




                                          Produktionsaufträge
                                          Lernziele

                                          • Produktionsauftrag kennenlernen.
                                          • Manuelle und automatische Erstellung von Produktionsaufträgen kennenlernen.


                                          Nutzen

                                          • Produktionsaufträge werden verwendet, um den eigenen Lagerbestand
                                            aufzufüllen.
                                          • Produktionsaufträge können bei Unterdeckung des Mindestbestands automatisch
                                            erzeugt werden, wenn in der Lieferantenkartei die Umleitung auf einen internen
                                            Kunden aktiviert ist.


                                          Merke

                                          Beschaffungsart            Alle Artikel, die in einem Produktionsauftrag erfasst
                                                                     werden, müssen die Beschaffungsart Produktion haben.

                                          Buchungsart                Im Gegensatz zu normalen Aufträgen werden die
                                                                     erfassten Positionen nicht im Lager reserviert, sondern
                                                                     als bestellt markiert.

                                          Lagerzugang                Der Lagerzugang aus Produktionsaufträgen kann
                                                                     manuell oder automatisch gebucht werden:
                                                                     • Manuelle Statusumsetzung im Modul Fertigung.
                                                                     • Automatische Status-Rückmeldungen aus der
                                                                       Produktion.

                                          Voreinstellungen           Lagerverwaltung:
                                                                     • Mindestbestand
                                                                     • Bestellmenge
                                                                     Stammdaten:
                                                                     • Produktverwaltung
                                                                     • Partnerverwaltung (interner Kunde)
                                                                     • Lieferantenkartei (Umleitung auf internen Kunden)
                                                                     Firmendaten:
                                                                     • Register Parameter
                                                                     • Register Lager / EK / EDI > Erfassungsstelle
5.20 / 04-2020




                 A+W Business Fertigung                                                                               G-131
                 Lagerartikel in Dokumenten                                                                     Tutorial




                                         Lagerartikel im Produktionsauftrag
                                         Produktionsaufträge werden verwendet, um den eigenen Lagerbestand auf-
                                         zufüllen. Alle Artikel, die in einem solchen Auftrag erfasst werden, werden au-
                                         tomatisch auf die Beschaffungsart Produktion umgesetzt. Im Gegensatz zu
                                         Kunden-Aufträgen werden die Positionen nicht im Lager reserviert, sondern
                                         als bestellt markiert.




                                         Abb. G-70    Positionserfassung – Beschaffungsart Produktion


                                         Ein Produktionsauftrag unterscheidet sich nur durch den Dokumententyp von
                                         anderen Aufträgen:




                                         Abb. G-71    Auftragserfassung – Dokumententyp Produktionsauftrag


                                         Produktionsaufträge können auf unterschiedliche Weise erfasst werden:
                                         •    Manuelle Erfassung eines neuen Dokumentes.
                                         •    Kopieren eines gespeicherten (Dummy-)Auftrags.
                                         •    Automatische Erstellung durch Unterdeckung des Lagerbestands.
5.20 / 04-2020




                 G-132                                                                        A+W Business Fertigung
                 Tutorial                                                                     Lagerartikel in Dokumenten




                                           Manuelle Erfassung durch Kopieren
                                           Wenn Sie regelmäßig Produktionsaufträge erfassen, können Sie den zuvor er-
                                           fassten Auftrag kopieren und sich so die Arbeit erleichtern.
                                           •   Vor dem Kopieren müssen Sie den Dokumententyp des Ziel-Dokuments
                                               auf Produktionsauftrag einstellen.
                                           •   Wenn nur bestimmte Positionen aus dem Auftrag übernommen werden
                                               sollen, können Sie diese auswählen.
                                           •   Im neuen Dokument können Sie die Daten anpassen.




                 A


                                                                                                                      B




                 A Kopieren von Auftrag nach Auftrag                         B Dokumententyp des Ziel-Auftrags
                 Abb. G-72    Produktionsauftrag durch Kopieren erstellen


                                           Eine ausführliche Beschreibung der Funktion Dokumente kopieren finden Sie
                                           im Part Verkauf.
                                            Verkauf, “Neuer Auftrag durch Kopieren” auf Seite C-245
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-133
                 Lagerartikel in Dokumenten                                                                       Tutorial




                                            Einstellungen in der Lieferantenkartei
                                            Wenn im Dialog Lagerverwaltung ein Mindestbestand und eine (Standard-)
                                            Bestellmenge für den Lagerartikel hinterlegt sind, kann das System automati-
                                            sche Bestellvorschläge generieren. Diese werden im Dialog Lagerbestellung
                                            aufgelistet.
                                            Normalerweise werden auf diesem Weg Bestellungen vom Typ Lagerbestel-
                                            lung generiert. Wenn jedoch in der Lieferantenkartei statt eines Standard-Lie-
                                            feranten ein interner Kunde hinterlegt ist, können Produktionsaufträge
                                            automatisch erzeugt werden.




                 A




                 B




                                     C
                 A Produkt, für das Produktionsaufträge erzeugt        B Umleitung auf internen Kunden
                   werden sollen                                       C Auswahl des Kunden
                 Abb. G-73    Interner Kunde für Produktionsaufträge


                                            In der Lieferantenkartei wird ein interner Kunde eingetragen, für den der Pro-
                                            duktionsauftrag automatisch erfasst wird. Die Option Interner Kunde kann auf
                                            der Ebene der Warengruppen oder der Produkte aktiviert werden. Dabei ha-
                                            ben die Einstellungen für Produkte Vorrang vor denen für Warengruppen.
5.20 / 04-2020




                 G-134                                                                            A+W Business Fertigung
                 Tutorial                                                                              Lagerartikel in Dokumenten




                                          Bestellmenge nach Bestandsprüfung
                                          Das Programm prüft, ob die aktuellen Lagerbestände zuzüglich der bereits be-
                                          stellten Mengen und abzüglich der reservierten Mengen den Mindestbestand
                                          unterschreiten.
                                          Wenn dies der Fall ist, wird als Vorschlag ein Vielfaches der (Standard-) Be-
                                          stellmenge angezeigt.

                                          Manuelle und automatische Lagerbestellung


                                                                               Lagerbestellung
                                                                                  Lagerort




                                                                                Mindestbestand
                                                                                unterschritten?



                                                                                       ja




                                                                                  Standard-
                                                                                Bestellmenge?



                                                                                       ja




                                                                                  Suche in der
                                                                               Lieferanten-Kartei




                                                               Standard-                             Interner
                                                               Lieferant?                             Kunde



                                                                   ja                                   ja




                                                            Bestellvorschlag                     Produktionsauftrag
                                                            Lagerbestellung                    Dokumentenverwaltung
5.20 / 04-2020




                                          Abb. G-74    Lagerbestellung vs. Produktionsauftrag




                 A+W Business Fertigung                                                                                   G-135
                 Lagerartikel in Dokumenten                                                                          Tutorial




                                         In diesem Ablaufplan ist dargestellt, wie A+W Business auf die unterschiedli-
                                         chen Voreinstellungen in der Lieferantenkartei reagiert.

                                         Bestellmenge
                                         Der Multiplikator wird so berechnet, dass durch den Vorschlag der Mindestbe-
                                         stand überschritten wird.




                                         Abb. G-75       Mengenangaben für Lagerartikel (Dialog Lagerverwaltung)


                                              Beispiel

                                              Das ESG mit der Produktnummer 4008 wird als Lagerartikel geführt.
                                              Aktueller Lagerbestand: 10 Stk.
                                              Mindestbestand: 30 Stk.
                                              Bestellmenge: 5 Stk.
                                              Die Bestellmenge für das ESG 4008 wird folgendermaßen berechnet:
                                              Differenz zwischen aktuellem Bestand und Mindestbestand: 20 Stk. In dieser
                                              Differenz ist die Bestellmenge 5 Stk. vier mal enthalten.
                                              Bestellmenge: 4 x 5 = 20 Stk.
                                              Aktueller Bestand plus bestellte Menge: 10 + 20 = 30 Stk.


                                         Die errechnete Menge wird in den Bestellvorschlag übernommen. Sie kann im
                                         Dialog Lagerbestellung angepasst werden.
5.20 / 04-2020




                 G-136                                                                             A+W Business Fertigung
                 Tutorial                                                                    Lagerartikel in Dokumenten




                 A




                 B




                 A Einschränkung auf Lagerort                       B Bestellvorschlag für Produktionsauftrag
                 Abb. G-76   Lagerbestellung – Bestellvorschläge


                                          Wie Sie die Bestellungen bearbeiten und übergeben, haben Sie in der Einheit
                                          Lagerbestellung kennengelernt.
                                           “Lagerbestellung an den Einkauf übergeben” auf Seite G-109
                                          Der Produktionsauftrag wird erst durch die Übergabe erzeugt und in dem Auf-
                                          tragsnummernverwalter angelegt, der zuletzt aktiviert war.
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-137
                 Lagerartikel in Dokumenten                                                                Tutorial




                 A




                 A Automatisch erzeugter Produktionsauftrag
                 Abb. G-77    Produktionsauftrag im Nummernverwalter für Aufträge


                                           Der Produktionsauftrag kann nun als Dokument geöffnet werden.
5.20 / 04-2020




                 G-138                                                                     A+W Business Fertigung
                 Tutorial                                                                   Lagerartikel in Dokumenten




                                                                                    A




                                                       B
                 A Auftragskopf – Produktionsauftrag                    B Bestellte Menge
                 Abb. G-78    Dokument Produktionsauftrag


                                           Der Produktionsauftrag kann bearbeitet und an die Produktion weitergeleitet
                                           werden.
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-139
                 Lagerartikel in Dokumenten                                                                       Tutorial




                                         Lagerzugang durch Produktionsauftrag
                                         In den Firmendaten müssen Sie ist im Register Lager / EK / EDI den Grenz-
                                         status für die Erfassungsstellen einstellen, ab dem ein Auftrag als produziert
                                         gilt. Als Grenzstatus gilt der für die gewählte Erfassungsstelle hinterlegte Sta-
                                         tus.




                                         Abb. G-79    Firmendaten – Lager / EK / EDI: Erfassungsstelle für Statusumsetzung


                                         Den Lagerzugang aus einem Produktionsauftrag können Sie auf zwei Arten
                                         erfassen:
                                         •  Sobald durch eine Produktionsrückmeldung der Status des Produktions-
                                            auftrages über diesen Status hinaus steigt, wird der Lagerzugang automa-
                                            tisch verbucht.
                                         • Wenn Sie nicht mit Produktionsrückmeldungen arbeiten, können Sie den
                                            Zugang über die manuelle Statusmeldung im Modul Fertigung erfassen.
                                            Wenn Sie den Produktionsauftrag dort auf einen Status setzen, der über
                                            dem o. g. Grenzstatus liegt, werden der Lagerabgang der verbrauchten
                                            Materialien und der Lagerzugang der gefertigten Lagerartikel automatisch
                                            gebucht.
                                         Wenn kein abweichender Lagerort definiert wurde, werden die Auftragsmen-
                                         gen dem Standard-Lagerort zugeordnet.
                                         Die Verbuchung von Produktionsaufträgen wird im Part Fertigung ausführlich
                                         behandelt.


                                         Ergänzende Informationen
                                          Stammdaten, “Firmendaten – Lager/EK/EDI” auf Seite B-957
                                          Verkauf, “Auftragskopf” auf Seite C-39
                                          Verkauf, “Bestellkennzeichen ändern” auf Seite C-310
                                          Fertigung, “Produktionsaufträge” auf Seite E-130
5.20 / 04-2020




                 G-140                                                                         A+W Business Fertigung
                 Tutorial                                                                                  Inventur




                                          Inventur
                                          In diesem Themenblock lernen Sie, wie Sie die Bestandszahlen Ihres Lagers
                                          in A+W Business durch eine Inventur bereinigen.
                                          Dazu gehören folgende Lerneinheiten:
                                          •   “Periodische Inventur” auf Seite G-142
                                          •   “Erstinventur” auf Seite G-158
5.20 / 04-2020




                 A+W Business Fertigung                                                                     G-141
                 Inventur                                                                                 Tutorial




                            Periodische Inventur
                            Lernziele

                            • Inventurablauf kennenlernen.
                            • Dialoge für die Inventur kennenlernen.
                            • Inventur durchführen.


                            Nutzen

                            • Mit der Inventur können Sie die Bestandszahlen in A+W Business bereinigen.
                            • Bei großen Lagerorten können Sie die Inventur so organisieren, dass der normale
                              Geschäftsbetrieb möglichst wenig behindert wird.


                            Merke

                            Keine Bestandsänderung      Am Zähltag dürfen keine Aufträge, Bestellungen und
                            während der Inventur        Wareneingänge erfasst werden, Ware darf nicht aus
                                                        dem Lager entnommen oder in es hineingestellt werden.
                                                        Der Sollbestand sollte am Zähltag ermittelt werden.

                            Verlauf der Inventur        Die Inventur wird in folgenden Schritten durchgeführt:
                                                        •   Inventurliste erstellen
                                                        •   Sollbestand ermitteln
                                                        •   Inventurwerte erfassen
                                                        •   Inventur abschließen

                            Inventur splitten           Bei großen Lagerorten ist es sinnvoll, die Inventur in
                                                        kleineren Einheiten durchzuführen.

                            Kisten gesondert            Für Kisten wird eine eigene Inventurliste erstellt. Die
                            inventarisieren             vorhandenen Kisten werden dann einzeln per Scanner
                                                        erfasst.

                            Keine Änderungen an den     Sobald die Inventurliste erstellt ist, werden in der
                            Stammdaten der Produkte     Produktverwaltung (Stammdaten) alle Produkte
                                                        gekennzeichnet, die in der Inventurliste aufgeführt sind.
                                                        Die Beschaffungsart und das Lagerkennzeichen in
                                                        diesen Produkten sind dann gesperrt.
                                                        Die Kennzeichnung wird gelöscht, sobald die Inventur
                                                        abgeschlossen ist.

                            Inventurliste ergänzen      Ergänzungen dürfen nur vor Ermittlung des Sollbestands
                                                        eingefügt werden.

                            Sollbestand in der Zählliste Wenn in der Zählliste der Sollbestand gedruckt werden
                                                         soll, müssen Sie den Sollbestand vor dem Druck
                                                         ermitteln.

                            Inventurabschluss pro       Der Inventurabschluss kann nur einmal pro Inventurliste
                            Inventurliste               durchgeführt werden.
5.20 / 04-2020




                            Voreinstellungen            Keine




                 G-142                                                                A+W Business Fertigung
                 Tutorial                                                                                        Inventur




                                          Bestandaufnahme
                                          In jedem Geschäftsjahr muss mindestens einmal durch körperliche Bestands-
                                          aufnahme geprüft werden, ob der jeweilige Buch- bzw. Sollbestand in der
                                          A+W Business-Lagerwirtschaft mit dem tatsächlich vorhandenen Bestand
                                          (Istbestand) übereinstimmt. Für diese gesetzlich vorgeschriebene Jahresin-
                                          ventur werden Inventurlisten erstellt, anhand derer die Bestände gezählt und
                                          erfasst werden können. Die Inventur stellt den Bestand des Vorratsvermögens
                                          nach Art, Menge und Wert fest.
                                          Grundlage jeder Inventur ist die Inventurliste, die sich auf ausgewählte Lager-
                                          artikel und/oder Lagerorte beziehen kann. Auf diese Weise kann die Inventur
                                          in mehreren Etappen durchgeführt werden und behindert so das Tagesge-
                                          schäft weniger.
                                          Bei der Inventur erhalten Sie von A+W Business Inventurlisten und Sollbe-
                                          stände. Die Inventur können Sie nach konventionellen Methoden durchführen
                                          oder für Kisten auch mit Hilfe der Barcode-Lesung.
                                          Die Inventur wird mit dem Inventurabschluss beendet. Erst damit werden die
                                          Bestandsmengen in A+W Business aktualisiert.

                                          Istbestand
                                          Die Istbestände werden anhand von Zähllisten eingegeben. Dabei können
                                          neue Lagerartikel angelegt werden. Während der Inventur sind die Lagerarti-
                                          kel für die Dokumentenerfassung nicht gesperrt, wenn sie sich in der Inventur-
                                          liste befinden. Daher sollten am Zähltag keine Aufträge, Bestellungen und
                                          Wareneingänge erfasst werden.

                                          Sollbestand
                                          Der Sollbestand muss spätestens am Tag der Zählung ermittelt werden. Damit
                                          haben Sie die Möglichkeit, die Inventurliste zu einem früheren Zeitpunkt zu er-
                                          stellen, als die Zählung und die Erfassung der gezählten Mengen und den In-
                                          venturabschluss.

                                             Beispiel

                                             Aktion                   Datum                 Bestand     Sollbestand

                                             Inventurliste erstellt   15.12.                                   100

                                             Zählung Istbestand       31.12.                      80           100

                                             Verkauf                  01.01. bis                 -30           -30
                                             Einkauf                  14.01.                     +10           +10

                                                                      15.01.            Tatsächlicher           80
                                                                                       Istbestand 60

                                             Inventurabschluss                       Sollbestand neu:           60
5.20 / 04-2020




                                          Mit dem Inventurabschluss wird der Istbestand als neuer Sollbestand im Sys-
                                          tem gespeichert.




                 A+W Business Fertigung                                                                           G-143
                 Inventur                                                                         Tutorial




                            Der Sollbestand kann wahlweise in den Zähllisten gedruckt werden. Wenn Sie
                            den Sollbestand nicht drucken, können Sie "gezählte" Mengen, die aufgrund
                            des Sollbestandes geschätzt wurden, nahezu ausschließen.

                            qm-Artikel
                            Werden für einen qm-Artikel einzelne Blätter in bestimmten Abmessungen ge-
                            zählt, so können diese als Stückartikel erfasst werden. Beim Inventurab-
                            schluss werden diese dann in qm umgewandelt und als solche in das Lager
                            gebucht (in Ausdrucken des Inventurabschlusses stehen allerdings die ge-
                            zählten Stückzahlen).

                            Inventarisieren einer Kiste
                            Zum Inventarisieren der Kiste, also um sie in einer Inventurliste zu erfassen,
                            wird zunächst eine Inventurliste erstellt und dafür der Sollbestand ermittelt.
                            Danach werden die Identnummer der Kiste, der Lagerort und ggf. eine abwei-
                            chende Blattanzahl gescannt oder manuell eingegeben. Der Scanvorgang
                            fügt diese Kiste immer der aktuellsten Inventurliste hinzu. Anschließend wird
                            ggf. in der Inventurverwaltung noch der restliche Lagerbestand erfasst und am
                            Ende der Inventurabschluss gebucht.

                            Beispiel für eine Zählliste




                            Abb. G-80    Zählliste mit Feldern für die gezählten Mengen


                            Die gezählten Mengen werden in der Zählliste eingetragen und später in der
5.20 / 04-2020




                            Inventurverwaltung erfasst.
                             “Inventurwerte erfassen” auf Seite G-152




                 G-144                                                             A+W Business Fertigung
                 Tutorial                                                                                         Inventur




                                          Inventurliste erstellen
                                          Für die Inventur werden Listen benötigt, in denen die manuellen Zählmengen
                                          festgehalten werden. Diese Listen können nach verschiedenen Kriterien aus-
                                          geführt und gedruckt werden.
                                          Wenn beim Druck festgestellt wird, dass bestimmte Artikel auf der Liste fehlen,
                                          kann eine Nachtragsinventur angehängt werden. Damit müssen nicht alle Lis-
                                          ten neu gedruckt werden.

                                              Keine Änderungen an den Stammdaten der Produkte
                                              Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung alle
                                              Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Be-
                                              schaffungsart und das Lagerkennzeichen in diesen Produkten sind dann
                                              gesperrt.
                                              Wenn die Inventur abgeschlossen ist, wird die Kennzeichnung gelöscht
                                              und die Daten können wieder bearbeitet werden.

                                          In dieser Einheit lernen Sie, wie Sie Inventurlisten erstellen und wieder öffnen.
                                          Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                                          •   “So beginnen Sie eine Inventur” auf Seite G-146
                                          •   “So drucken Sie die Zähllisten” auf Seite G-148
                                          •   “So laden Sie eine gespeicherte Inventurliste” auf Seite G-149
                                          •   “So ergänzen Sie eine Inventurliste vor dem Zählen” auf Seite G-149
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-145
                 Inventur                                                                              Tutorial




                             So beginnen Sie eine Inventur
                            1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Inventurliste.
                               Der Dialog Inventurliste wird geöffnet.
                                Softwarereferenz, “Inventurliste” auf Seite G-167
                            2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                              seln.

                             A           B                     C




                                                                                                             D


                                                                                                             E




                            A Alle Artikel oder Folge von                C Eingrenzungen
                              Artikelnummern                             D Lagerbewertung
                            B Datum der Inventur                         E Sortierung der Liste
                            Abb. G-81    Felder für neue Inventurliste freigeschaltet


                               Als Name wird für die Inventur ein Datum (B) verwendet. Standardmäßig
                               wird das aktuelle Tagesdatum vorgeschlagen. Sie können jedes beliebige
                               andere Datum eintragen oder auswählen.
                            3 Wählen Sie die Artikel (A) für die Inventur aus:
                               •   Alle Artikel:
                                   Sie können die Inventur für alle Artikel durchführen, die als Produkte in
                                   den Stammdaten erfasst sind. In diesem Fall sind die Felder für die Ar-
                                   tikelnummern gesperrt.
                                   Bei der Erstinventur aktivieren Sie diese Option, bei allen anderen In-
                                   venturen können Sie die Inventurlisten auf bestimmte Artikel beschrän-
                                   ken.
5.20 / 04-2020




                               •   Artikelnummer:
                                   Sie können die Inventurliste auf eine Folge von Artikelnummern ein-




                 G-146                                                                  A+W Business Fertigung
                 Tutorial                                                                                       Inventur




                                                 schränken. Die Felder sind gesperrt, wenn Sie die Option Alle Artikel
                                                 markiert haben.
                                          4 Schränken Sie die Liste ggf. weiter ein (C):
                                             •   Nur Produkte mit Lagerbestand > 0:
                                                 Sie können die Inventur auf die Lagerartikel mit Bestand einschränken.
                                                 Wenn Sie die Checkbox nicht markieren, wird der komplette Produkt-
                                                 stamm in die Inventurliste aufgenommen, sofern die Auswahl nicht
                                                 durch andere Kriterien eingeschränkt wird.
                                             •   Nur Produkte mit zugeordnetem Lagerprodukt:
                                                 Sie können die Inventur auf die Lagerartikel aus der Lagerverwaltung
                                                 einschränken. Wenn Sie die Checkbox nicht markieren, wird der kom-
                                                 plette Produktstamm inklusive Lagermaßtabelle in die Inventurliste auf-
                                                 genommen, sofern die Auswahl nicht durch andere Kriterien
                                                 eingeschränkt wird.
                                             •   Nur Produkte mit Lagerführung in dem Produkt:
                                                 Sie können die Inventur auf die Produkte mit der Beschaffungsart Lage-
                                                 rentnahme einschränken.
                                             •   Keine Kisten mit Identnummer und Bestand = 0:
                                                 Im Lagerbestand können sich Kisten befinden, die bereits ausgeliefert
                                                 sind, aber nicht gelöscht wurden. Deren Bestand wird korrekt mit 0 an-
                                                 gezeigt. Diese Kisten können Sie ausblenden, da zu ihnen keine Menge
                                                 erfasst werden wird.
                                             •   Nur für bestimmten Lagerort:
                                                 Mit dieser Einstellung werden die Felder für die Auswahl des Lagerorts
                                                 freigeschaltet.
                                                 Wenn Sie die Inventur nur für bestimmte Lagerorte durchführen möch-
                                                 ten, können Sie für diese je eine eigene Inventurliste erstellen. Beach-
                                                 ten Sie dabei, dass Artikel auch auf den Lagerort <k.A.> gebucht sein
                                                 können.
                                                 Wenn Sie eine gesamte Inventur durchführen wollen, können Sie die In-
                                                 venturliste auch im Druck nach Lagerorten splitten.
                                          5 Wählen Sie die Art der Lagerbewertung (D) aus.
                                             Wenn Sie in den Firmendaten die Optionen für die EK-Berechnung aktiviert
                                             haben, können Sie die Lagerbewertung folgendermaßen berechnen las-
                                             sen:
                                             •   EK-Preisliste:
                                                 Die Einzelpreise der Produkte aus der EK-Tarifzuordnung werden her-
                                                 angezogen.
                                             •   Niedrigster EK:
                                                 Für alle Artikel wird jeweils der niedrigste Wert herangezogen.
                                             •   Geschnittener EK:
                                                 Für alle Artikel wird jeweils der Durchschnitts-EK herangezogen. Dazu
                                                 muss in den Firmendaten die Option Durchschnitts-EK aktiviert sein.
                                          6 Wählen Sie die Art der Sortierung (E) aus.
                                             Die Sortierung der Artikel auf der Inventurliste sollte sich nach den ausge-
5.20 / 04-2020




                                             wählten Kriterien richten. Die Option Abmessung ist z. B. für Lagermaße
                                             sinnvoll.
                                          7 Wählen Sie im Menü Start > Speichern, um die Inventurliste zu erstellen.


                 A+W Business Fertigung                                                                          G-147
                 Inventur                                                                              Tutorial




                               Die Inventurliste wird in der Übersicht angezeigt. Sie können jetzt die Zähl-
                               listen drucken und/oder den Sollbestand ermitteln.

                               Keine Änderungen an den Stammdaten der Produkte
                               Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung
                               (Stammdaten) alle Produkte gekennzeichnet, die in der Inventurliste aufge-
                               führt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Pro-
                               dukten sind dann gesperrt. Sobald die Inventur abgeschlossen ist, wird die
                               Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.


                             So drucken Sie die Zähllisten
                               Wenn in der Zählliste der Sollbestand gedruckt werden soll, müssen Sie
                               vor dem Druck den Sollbestand ermitteln.
                                “So ermitteln Sie den Sollbestand zu einer Inventurliste” auf Seite G-151
                            1 Wählen Sie im Menü Lagerwirtschaft > Inventur und wählen Sie das Datum
                              der Inventurliste aus.
                            2 Wählen Sie im Menü Start > Suchen, um die Inventurliste zu laden.
                               Diese Schritte entfallen, wenn Sie die Zählliste sofort nach dem Erstellen
                               der Inventurliste drucken.
                            3 Wählen Sie im Menü Druck > Drucker.
                               Wenn Sie das Ergebnis zunächst am Bildschirm prüfen möchten, wählen
                               Sie Bildschirm. Sie können dann den Druck starten, wenn Sie mit dem Er-
                               gebnis zufrieden sind. Die folgenden Schritte sind für beide Einstellungen
                               gleich.



                               A

                               B


                               C




                               A Seitenumbruch                         C Sortierung
                               B Artikel, die gedruckt werden sollen
5.20 / 04-2020




                               Abb. G-82     Inventur – Zählliste drucken


                                Softwarereferenz, “Listendruck” auf Seite G-171


                 G-148                                                              A+W Business Fertigung
                 Tutorial                                                                                        Inventur




                                             Drucken Sie die Zähllisten so aus, dass sie den Aufgaben Ihrer Inventur-
                                             Mitarbeiter entsprechen.
                                          4 Bestimmen Sie, an welcher Stelle eine neue Seite (A) gedruckt werden
                                            soll.
                                             Wenn Sie keine unterschiedlichen Lagerorte angelegt haben, entfällt diese
                                             Einstellung. Wenn Sie die Zählbereiche nach Lagerorten verteilt haben,
                                             machen Sie den Seitenumbruch nach den entsprechenden Lagerorten.
                                             Für den Druck müssen Sie mindestens Lagerhaus (Ebene 1) markieren.
                                          5 Legen Sie fest, welche Lagerware (B) in der Liste gedruckt werden soll.
                                             Wenn an den angegebenen Lagerorten unterschiedliche Lagerartikel
                                             vorkommen, können Sie nach Fertigprodukten oder Rohmaterial unter-
                                             scheiden. Fertigprodukte sind alle Lagerartikel, die nicht im Lager für Roh-
                                             material gelagert sind.
                                             Die Zuordnung der Eigenschaften Fertigprodukte und Rohmaterial haben
                                             Sie in der Lagerdefinition getroffen.
                                              “Lagerort definieren” auf Seite G-24
                                          6 Wählen Sie die Sortierung (C) der Artikel auf der Zählliste so, dass sie sich
                                            nach den ausgewählten Kriterien richten. Die Option Artikel ist z. B. dann
                                            sinnvoll, wenn Sie das Lager nach Produkten aufgebaut haben.
                                          7 Klicken Sie auf [OK], um den Druck zu starten.
                                             Die Liste wird gedruckt und kann nun zur Zählung verwendet werden.


                                           So laden Sie eine gespeicherte Inventurliste
                                          1 Wählen Sie im Menü Lagerwirtschaft > Inventur.
                                          2 Wählen Sie im Feld Inventurdatum das Datum aus, unter dem die Inven-
                                            turliste gespeichert wurde.
                                          3 Wählen Sie im Menü Start > Suchen, um die Inventurliste zu laden.
                                             Die Inventurliste wird angezeigt.


                                           So ergänzen Sie eine Inventurliste vor dem Zählen
                                             Wenn Sie den Sollbestand zu einer Inventurliste bereits ermittelt haben,
                                             können Sie die Liste nicht mehr ergänzen. Beenden Sie in diesem Fall die
                                             Inventur und erfassen Sie die fehlenden Artikel in einer neuen Inventurliste.
                                          1 Wählen Sie im Menü Lagerwirtschaft > Inventur.
                                          2 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                            seln.
                                             Die Felder werden freigeschaltet.
                                          3 Wählen Sie die Inventurliste aus, zu der Sie weitere Artikel hinzufügen
                                            möchten.
5.20 / 04-2020




                                          4 Wählen Sie die Lagerartikel und/oder Standorte aus.
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.


                 A+W Business Fertigung                                                                           G-149
                 Inventur                                                                          Tutorial




                               Eine Abfrage wird angezeigt, in der Sie den Vorgang abbrechen oder zu
                               Ende führen können.
                            6 Wählen Sie:
                               •   [Ja]: Die bestehende Liste wird angezeigt und die neuen Artikel werden
                                   am Ende hinzugefügt.
                               •   [Nein] oder [Abbrechen]: Die Abfrage wird geschlossen. Sie können das
                                   Datum und weitere Kriterien ändern und damit eine neue Inventurliste
                                   erstellen.


                            Sollbestand ermitteln
                            Der Sollbestand muss für jede Inventurliste durchgeführt werden. Er gibt die
                            Mengen an, die sich laut System im Lager befinden müssen. Wenn der Soll-
                            bestand mit in den Zähllisten gedruckt werden soll, muss er vor dem Druck der
                            Liste ermittelt werden.

                               Keine Lagerbuchungen am Zähltag
                               Nachdem der Sollbestand ermittelt wurde, müssen die Bestände gezählt
                               werden. Am Tag der Zählung dürfen keine Lagerartikel entnommen und
                               keine Lagerbewegungen gebucht werden, bis die Zählung abgeschlossen
                               ist. Dies betrifft alle manuellen oder automatischen Lagerab-/zugänge und
                               alle Wareneingänge für Lagerbestellungen. A+W Business wird nicht auto-
                               matisch für Buchungen gesperrt.

                            In dieser Einheit lernen Sie, wie Sie den Sollbestand für eine gespeicherte In-
                            venturliste ermitteln.
5.20 / 04-2020




                 G-150                                                          A+W Business Fertigung
                 Tutorial                                                                                      Inventur




                                           So ermitteln Sie den Sollbestand zu einer Inventurliste
                                          1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Sollbestand.
                                             Der Dialog Sollbestand wird geöffnet.
                                              Softwarereferenz, “Sollbestand” auf Seite G-173
                                          2 Laden Sie die Inventurliste, zu der der Sollbestand ermittelt werden soll.




                                             Abb. G-83    Sollbestand ermitteln


                                          3 Wählen Sie im Menü Start > Ausführen, um den Sollbestand zu ermitteln
                                            und bestätigen Sie die Abfrage mit [Ja].
                                             Der Sollbestand wird in der Spalte Soll eingetragen. Sie können den Soll-
                                             bestand nur einmal pro Inventurliste ermitteln. Wenn Sie die Funktion
                                             mehrfach ausführen, wird das Ergebnis nicht aktualisiert.
                                             Wenn der Sollbestand mit in die Zählliste gedruckt werden soll, können Sie
                                             jetzt den Druck starten.
                                             Sie können jetzt die Zählung beginnen und anschließend die gezählten
                                             Mengen erfassen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-151
                 Inventur                                                                         Tutorial




                            Inventurwerte erfassen
                            Wenn die Zählmengen in die gedruckten Zähllisten eingetragen sind, können
                            Sie die Werte im Dialog Inventurverwaltung eingeben.
                            In dieser Einheit lernen Sie, wie Sie die gezählten Mengen in A+W Business
                            erfassen und ggf. einen neuen Lagerartikel anlegen.
                            Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
                            •   “So erfassen Sie die gezählten Mengen” auf Seite G-152
                            •   “So erfassen Sie einen neuen Lagerartikel während der Inventur” auf
                                Seite G-153


                             So erfassen Sie die gezählten Mengen
                            1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Verwaltung.
                                Der Dialog Verwaltung wird geöffnet.
                                 Softwarereferenz, “Verwaltung” auf Seite G-176
                            2 Laden Sie die Inventurliste.
                                In der Tabelle werden die Belege in derselben Reihenfolge angezeigt, wie
                                in der gedruckten Liste.
                                Über das Menü Sortierung kann eine andere Reihenfolge ausgewählt wer-
                                den, wenn dadurch die Erfassung der gezählten Werte einfacher wird.




                                                                                                       A




                                                                                                       B




                            A Gezählte Menge eingeben               B Liste der Belege
                            Abb. G-84     Inventur – Zählmengen erfassen
5.20 / 04-2020




                            3 Tragen Sie die Menge (A) der ersten Position im Feld Menge ein und be-
                              stätigen Sie mit <Enter>.



                 G-152                                                             A+W Business Fertigung
                 Tutorial                                                                                     Inventur




                                             Die Markierung wechselt danach automatisch in die nächste Zeile, so dass
                                             Sie sofort die nächste Menge eintragen können.
                                          4 Markieren Sie ggf. eine Zeile, wenn Sie die Mengen in einer anderen Rei-
                                            henfolge erfassen möchten.

                                             Menge und Lagerort für mehrere Artikel
                                             Sie können mehrere Belege markieren und für alle gemeinsam über das
                                             Menü Funktionen die Menge auf null setzen oder den Lagerort ändern.

                                          5 Ändern Sie ggf. den Lagerort, den Inventurpreis und die Kategorie, die für
                                            die Bewertung des Lagers herangezogen werden.
                                             Geänderte Inventurpreise werden nach dem Abschluss der Inventur nicht
                                             in die EK-Preistabelle zurückgeschrieben und fließen nicht in die Berech-
                                             nung des Durchschnitts-EKs ein.
                                          6 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Daten werden gespeichert. Wenn Sie die Daten noch nicht vollständig
                                             erfasst haben, können Sie die Eingabe zu einem späteren Zeitpunkt fort-
                                             setzen. Beginnen Sie dann mit Schritt 1.
                                             Wenn Sie alle Mengen erfasst haben, können Sie die Inventur abschlie-
                                             ßen.


                                           So erfassen Sie einen neuen Lagerartikel während der Inventur
                                          1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Verwaltung und wählen
                                            Sie die aktuelle Inventur aus.
                                          2 Markieren Sie den Beleg, zu dem Sie einen neuen Lagerartikel anlegen
                                            möchten.
                                          3 Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wech-
                                            seln.
                                             Alle Daten des ursprünglichen Lagerartikels werden damit kopiert, so dass
                                             Sie im neuen Lagerartikel nur die abweichenden Daten bearbeiten müs-
                                             sen.
                                          4 Tragen Sie die Breite, Höhe, den Lagerort usw. ein.
                                          5 Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
                                             Die Liste wird um den neuen Lagerartikel erweitert.
5.20 / 04-2020




                 A+W Business Fertigung                                                                        G-153
                 Inventur                                                                           Tutorial




                            Inventur abschließen
                            Die Inventur wird abgeschlossen, indem die Zählergebnisse verbucht und die
                            Bestände im Lager aktualisiert werden.
                            Der Inventurabschluss kann nur einmal pro Inventurliste durchgeführt werden.
                            Wenn Sie nach dem Abschluss Fehler in den gezählten oder erfassten Werten
                            feststellen, müssen Sie die Mengen im Dialog Lagerverwaltung korrigieren
                            oder für den entsprechenden Artikel eine neue Inventurliste erstellen und ab-
                            schließen.
                            In dieser Einheit lernen Sie, wie Sie die Inventur zu einer Inventurliste ab-
                            schließen.
                            Zu diesem Thema gibt es folgende Handlungsanleitungen:
                            •   “So schließen Sie die Inventur ab” auf Seite G-154
                            •   “So löschen Sie eine Inventurliste nach dem Inventurabschluss” auf
                                Seite G-155


                             So schließen Sie die Inventur ab
                            1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Abschluss.
                                Der Dialog Abschluss wird geöffnet.
                                 Softwarereferenz, “Abschluss” auf Seite G-181
                            2 Laden Sie die Inventur, die Sie abschließen möchten.




                                Abb. G-85    Inventur – Abschluss
5.20 / 04-2020




                                In der Übersicht wird die Inventurliste mit den eingegebenen Mengen an-
                                gezeigt.



                 G-154                                                            A+W Business Fertigung
                 Tutorial                                                                                       Inventur




                                          3 Prüfen Sie im Menü Optionen, ob der Bestand ohne oder mit Abfrage auf
                                            Null gesetzt werden soll, wenn keine Mengen erfasst sind.
                                          4 Wählen Sie ggf. den AV-Bereich aus, auf den die Inventur eingeschränkt
                                            wurde.
                                          5 Wählen Sie im Menü Start > Ausführen und bestätigen Sie die Abfrage mit
                                            [Ja], um die Inventur abzuschließen.
                                             Die Daten werden gespeichert und die Bestandswerte und Preise für die
                                             Lagerbewertung werden aktualisiert. Die verbuchten Belege werden aus
                                             der Liste gelöscht. Die Sperrungen in den Produktstammdaten werden auf-
                                             gehoben.
                                             Belege, die nicht verbucht werden konnten, bleiben in der Liste enthalten.
                                             Sie können die fehlenden Werte im Dialog Verwaltung ergänzen.
                                             Wenn alle Belege verbucht werden konnten, wird die gesamte Inventurliste
                                             aus dem Inventurabschluss gelöscht.

                                             Fehler bei der Inventur
                                             Wenn bei der Inventur Fehler aufgetreten sind und einzelne Belege nicht
                                             aus der Inventurliste gelöscht werden, können Sie im Logbuch nach der
                                             Ursache forschen. Öffnen Sie das Logbuch über System > Logbuch.


                                           So löschen Sie eine Inventurliste nach dem Inventurabschluss

                                             Keine einzelnen Belege löschen
                                             Sie können nach dem Inventurabschluss keine einzelnen Belege aus der
                                             Liste löschen.

                                          1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Inventurliste.
                                          2 Laden Sie die Inventurliste, die Sie abgeschlossen haben.
                                          3 Wählen Sie im Menü Start > Löschen und bestätigen Sie die Abfrage mit
                                            [Ja].
                                             Die Inventurliste wird gelöscht. Wenn Sie weitere Inventurlisten erzeugt ha-
                                             ben, wird die nächste Liste geladen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-155
                 Inventur                                                                           Tutorial




                            Nachtragsinventur anhängen
                            Sie können zwei getrennte Inventuren für den Druck im Inventurabschluss zu-
                            sammenfassen. Dazu müssen beide Inventuren abgeschlossen (also ver-
                            bucht) sein.
                            Wie Sie eine Inventurliste um weitere Lagerartikel ergänzen, ist im Kapitel In-
                            venturliste erstellen beschrieben.
                             “So ergänzen Sie eine Inventurliste vor dem Zählen” auf Seite G-149
                            In dieser Einheit lernen Sie, wie Sie eine Nachtragsinventur an eine Haupt-
                            inventur anhängen.


                             So hängen Sie eine Nachtragsinventur an
                            1 Wählen Sie im Menü Lagerwirtschaft > Inventur > Abschluss.
                               Der Dialog Abschluss wird geöffnet.
                            2 Wählen Sie in Feld Inventurdatum die Hauptinventur aus.
                            3 Wählen Sie im Menü Funktionen > Nachtragsinventur anhängen.




                               Abb. G-86     Nachtragsinventur auswählen


                            4 Wählen Sie das Datum der Nachtragsinventur aus und übernehmen Sie
                              diese mit [OK].
                               Die Liste der Hauptinventur wird um die Positionen der Nachtragsinventur
                               erweitert. Die Liste der Nachtragsinventur wird aus dem Dialog Inventurlis-
                               te gelöscht.
5.20 / 04-2020




                 G-156                                                            A+W Business Fertigung
                 Tutorial                                                                                         Inventur




                                          Übungen
                                          •   Erstellen Sie eine Inventurliste für eine Folge von 5 Artikeln.
                                          •   Ergänzen Sie die Inventurliste um zwei Artikel.
                                          •   Ermitteln Sie den Sollbestand für die gesamte Inventurliste.
                                          •   Tragen Sie die Zählwerte ein.
                                          •   Schließen Sie die Inventur ab.
                                          •   Erstellen Sie eine weitere Inventurliste mit drei Artikeln. Hängen Sie diese
                                              als Nachtragsinventur an die erste Inventur an.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Inventurliste” auf Seite G-167
                                           Softwarereferenz, “Listendruck” auf Seite G-171
                                           Softwarereferenz, “Sollbestand” auf Seite G-173
                                           Softwarereferenz, “Verwaltung” auf Seite G-176
                                           Softwarereferenz, “Abschluss” auf Seite G-181
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-157
                 Inventur                                                                                Tutorial




                            Erstinventur
                            Lernziele

                            • Funktion der Erstinventur kennenlernen.


                            Nutzen

                            • Mit der Erstinventur können Sie Ihr Lager mit den Lagerartikeln und den aktuellen
                              Beständen in Betrieb nehmen.


                            Merke

                            Erstinventur mit            Bevor Sie mit der Erstinventur beginnen, sollten Sie sich
                            Unterstützung               mit der A+W Software GmbH in Verbindung setzen. Ihre
                                                        Ansprechpartner werden Sie dann bei der Durchführung
                                                        unterstützen.

                            Keine Auftragsbearbeitung Da während der Erstinventur keine Aufträge bearbeitet
                                                      werden dürfen, sollten Sie die Erstinventur außerhalb
                                                      des normalen Tagesgeschäfts durchführen, z. B. an
                                                      einem Wochenende.

                            Voraussetzung               Sie müssen den Ablauf der periodischen Inventur
                                                        kennen, bevor Sie eine Erstinventur beginnen. Lesen
                                                        Sie daher die Lerneinheit Periodische Inventur
                                                        aufmerksam durch.

                            Voreinstellungen            Keine
5.20 / 04-2020




                 G-158                                                               A+W Business Fertigung
                 Tutorial                                                                                        Inventur




                                          Ablauf für die Erstinventur
                                          •   Lagerinitialisierung: Das Lager wird gelöscht (Modul Utilities).
                                              Ab jetzt dürfen keine neuen Aufträge erfasst und die alten nicht bearbeitet
                                              werden.
                                          •   Inventurliste erstellen.
                                          •   Sollbestand ermitteln.
                                          •   Lagerverwaltung: Alle Bestände auf 0 setzen und den Standard-Lagerort
                                              für alle Lagerartikel festlegen.
                                          •   Inventur abschließen.
                                          •   Lagerinitialisierung (Modul Utilities).
                                              Bis jetzt haben Sie alle echten Lagerartikel erfasst und deren Bestand auf
                                              0 gesetzt. Alle alten (falschen) Werte, z. B. Testprodukte und Bestandszah-
                                              len zum Testen von Funktionen, sind gelöscht.
                                              Die Werte für Bestellungen und Reservierungen werden geprüft und ggf.
                                              berichtigt.
                                          •   Vollständige Inventur durchführen:
                                              – Neue Inventurliste erstellen.
                                              – Zählliste drucken.
                                              – Sollbestand ermitteln.
                                              – Mengen der Lagerartikel zählen.
                                                 Während der Zählphase keine Ab- und Zugänge im Lager buchen.
                                              – Gezählte Werte erfassen.
                                              – Inventur abschließen.
                                          •   Lagerinitialisierung (Modul Utilities).
                                              Die Werte für Bestellungen und Reservierungen werden erneut geprüft und
                                              auf die Lagerartikel umgesetzt.
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-159
                 Inventur                                                                                          Tutorial




                                           Erstinventur durchführen
                                           Die Erstinventur wird durchgeführt, bevor Sie zum ersten Mal mit der
                                           A+W Business-Lagerwirtschaft arbeiten. Sie dient dazu, das Lager mit den
                                           Lagerartikeln und deren Anfangsbeständen in Betrieb zu nehmen.

                                               Ablauf der normalen Inventur sollte bekannt sein
                                               Bevor Sie mit den nachfolgend beschriebenen Handlungsabläufen begin-
                                               nen, sollten Sie sich die Beschreibungen der normalen Inventur durchle-
                                               sen. Die Beschreibung der Erstinventur setzt diese Kenntnis voraus.


                                            So führen Sie eine Erstinventur durch

                                               Vor der Erstinventur Kontakt mit dem Service aufnehmen
                                               Bevor Sie mit der Erstinventur beginnen, sollten Sie sich mit der A+W Soft-
                                               ware GmbH in Verbindung setzen. Ihre Ansprechpartner werden Sie dann
                                               bei der Durchführung unterstützen.

                                           1 Starten Sie das Modul Utilities.
                                           2 Wählen Sie im Menü System > Lagerinitialisierung.




                    Abb. G-87   Utilities – Lagerinitialisierung
5.20 / 04-2020




                                           3 Wählen Sie im Menü Funktionen > Lager löschen.
                                               Ab jetzt dürfen keine neuen Aufträge erfasst und keine alten Aufträge be-
                                               arbeitet werden, bis Sie die Lagerinitialisierung erneut durchgeführt haben.


                 G-160                                                                          A+W Business Fertigung
                 Tutorial                                                                                          Inventur




                                             Wenn doch im Dialog Dokumentenverwaltung gearbeitet wird, wird der La-
                                             gerort k.A. in der Lagerverwaltung wieder angelegt und allen Lagerartikeln
                                             zugeordnet.
                                          4 Führen Sie jetzt die Inventur in folgenden Schritten durch:
                                             •   Inventurliste erstellen.
                                                 Wählen Sie im Dialog Inventurliste folgende Kriterien:
                                                 – Nur für Lagerartikel:
                                                    Mit der Einstellung alle Artikel würden z. B. auch die Bestellartikel in
                                                    die Liste aufgenommen.
                                                 – Alle Lagerorte.
                                             •   Sollbestand ermitteln.
                                             •   Inventurwerte erfassen.
                                                 Setzen Sie im Dialog Lagerwirtschaft > Verwaltung die Mengen aller ge-
                                                 zählten Artikel auf 0.
                                                 Dieser Vorgang ist in der Handlungsanleitung zum Erfassen der gezähl-
                                                 ten Mengen in der Anmerkung zu Schritt 4 und in Schritt 5 beschrieben.
                                             •   Inventur abschließen.
                                          5 Wechseln Sie wieder zum Dialog Lagerinitialisierung.
                                          6 Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten.
                                          7 Führen Sie mit einer neuen Inventurliste eine vollständige Inventur durch:
                                             •   “So beginnen Sie eine Inventur” auf Seite G-146
                                             •   “So drucken Sie die Zähllisten” auf Seite G-148
                                             •   “So ermitteln Sie den Sollbestand zu einer Inventurliste” auf
                                                 Seite G-151
                                             Achten Sie darauf, dass während der Zählphase keine Ab- oder Zugänge
                                             im Lager gebucht werden. Dies betrifft auch das Erfassen von Warenein-
                                             gängen.
                                          8 Tragen Sie die gezählten Mengen und die korrekten Lagerorte ein und
                                            schließen Sie die Inventur ab:
                                             •   “So erfassen Sie die gezählten Mengen” auf Seite G-152
                                             •   “So schließen Sie die Inventur ab” auf Seite G-154
                                          9 Öffnen Sie den Dialog Lagerinitialisierung, wie in Schritt 1 und 2 beschrie-
                                            ben.
                                          10 Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten.
                                             Ab jetzt stimmen die Bestände im Lager und die Lagerorte.
5.20 / 04-2020




                 A+W Business Fertigung                                                                              G-161
                 Übungen                                                                       Tutorial




                           Übungen
                           Beantworten Sie die folgenden Fragen, indem Sie die entsprechenden Ein-
                           stellungen erklären.
                           •   Wann berücksichtigt das Lager Rückmeldungen aus der Produktion, z. B.
                               von A+W Production?
                           •   Wo hinterlegt man, ob die Ausbuchung von reservierten Lagerprodukten
                               nach Lieferscheindruck oder nach Rechnungsdruck erfolgt?
                           •   Was müssen Sie tun, um Lagerprodukte, die als Stücklisten-Komponenten
                               in einer Position stehen, im Lager automatisch zu verbuchen?
                           •   Was ist der Unterschied zwischen der Definition von Lagermaßen im Dia-
                               log Stammdaten > Produkte > Artikel > Lagermaße und im Dialog Lager-
                               wirtschaft > Lagerverwaltung?
                           •   Was wird in den ersten beiden Registern im Dialog Lagerwirtschaft > La-
                               gerverwaltung angezeigt. Beschreiben Sie die Unterschiede!
                           •   Was ist der Unterschied zwischen dem Buchungsjournal und der Lager-
                               historie?
                           •   Wozu dient der Dialog Lagerwirtschaft > Lagerbestellung?
                           •   Was ist der Unterschied zwischen einer manuellen und einer automati-
                               schen Lagerbestellung?
5.20 / 04-2020




                 G-162                                                       A+W Business Fertigung
Lagerwirtschaft               G

                  Softwarereferenz




                  A+W Business
                 Softwarereferenz                                                                         Übersicht




                                          Übersicht
                                          Im Modul Lagerwirtschaft werden alle Daten zum Lager gepflegt und ausge-
                                          wertet. Außerdem führen Sie in diesem Modul die Inventur durch und buchen
                                          Lagerbewegungen.
                                          In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                          •   “Inventur” auf Seite G-166
                                          •   “Lagerverwaltung” auf Seite G-184
                                          •   “Lagerbewegung” auf Seite G-195
                                          •   “Abfragen” auf Seite G-202
                                          •   “Suche” auf Seite G-217
                                          •   “Lagerbestellung” auf Seite G-220
                                          •   “Lagerbewertung” auf Seite G-226
5.20 / 04-2020




                 A+W Business Fertigung                                                                      G-165
                 Inventur                                                                 Softwarereferenz




                            Inventur
                            Lagerwirtschaft > Inventur
                            Über die Dialoge aus dem Menü Inventur führen Sie die Inventur in einzelnen
                            Schritten durch: Sie erstellen eine Inventurliste, ermitteln den Sollbestand, er-
                            fassen die gezählten Mengen und schließen die Inventur ab.
                            Im Menü Inventur finden Sie sich folgende Programmpunkte:
                            •   Inventurliste
                            •   Sollbestand
                            •   Inventurverwaltung
                            •   Inventurabschluss

                            Ergänzende Informationen
                             Tutorial, “Periodische Inventur” auf Seite G-142
                             Tutorial, “Erstinventur” auf Seite G-158
5.20 / 04-2020




                 G-166                                                            A+W Business Fertigung
                 Softwarereferenz                                                                               Inventur




                                          Inventurliste
                                          Lagerwirtschaft > Inventur > Inventurliste

                                          Menü Funktionen
                                          Mit der Funktion Lager bereinigen wird die alte Inventurliste gelöscht. Gleich-
                                          zeitig werden alle Produkte aus den Lager-Stammdaten gelöscht, die kein La-
                                          gerkennzeichen haben oder die unsinnig sind, z. B. ein Produkt, das keine
                                          Referenz auf einen Lagerort hat.

                                             Der Vorgang kann erhebliche Zeit in Anspruch nehmen
                                             Je nach Größe der Datenbank und Rechnerleistung kann die Bereinigung
                                             des Lagers über einen längeren Zeitraum laufen. Dies können auch meh-
                                             rere Stunden sein. In dieser Zeit kann mit A+W Business nicht gearbeitet
                                             werden.




                                          Abb. G-88     Inventurliste


                                          Die Inventurliste bildet die Basis für den Inventurvorgang. Dazu wählen Sie die
                                          Kriterien aus, nach denen die Liste erstellt werden soll. Da während des Zähl-
                                          vorgangs keine Lagerveränderungen ausgeführt werden dürfen, ist es bei gro-
                                          ßen Lagern sinnvoll, die Inventur in kleineren Einheiten durchzuführen, z. B.
                                          nach Lagerorten.
                                           Tutorial, “Inventurliste erstellen” auf Seite G-145
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-167
                 Inventur                                                                   Softwarereferenz




                               Keine Änderungen an den Stammdaten der Produkte
                               Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung
                               (Stammdaten) alle Produkte gekennzeichnet, die in der Inventurliste aufge-
                               führt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Pro-
                               dukten sind dann gesperrt. Sobald die Inventur abgeschlossen ist, wird die
                               Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.

                            Wenn die Inventurliste erstellt ist, kann der Sollbestand für die Artikel ermittelt
                            werden, die auf der Inventurliste aufgeführt sind.
                             Tutorial, “Inventur” auf Seite G-141

                               Inventurliste löschen
                               Wenn eine Inventur vollständig durchgeführt und abgeschlossen ist, sollten
                               Sie die zugehörige Inventurliste löschen. Sie können jedoch auch jede be-
                               liebige Inventurliste zu jedem Zeitpunkt wieder löschen. Das Kennzeichen
                               Artikel steht auf der Inventurliste im Auftrag und die Sperrung der Produkt-
                               stammdaten werden dann aufgehoben.

                            Parameter
                            Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie eine neue In-
                            venturliste erstellen. Im Auswahlmodus können Sie eine Inventurliste über das
                            Datum anzeigen lassen.

                            Inventurdatum Die Inventurliste wird zu einem bestimmten Datum erstellt.
                            Alle weiteren Inventurvorgänge beziehen sich immer auf das Inventurdatum.
                            Das aktuelle Tagesdatum wird automatisch angezeigt. Es kann mit dem ge-
                            wünschten Datum überschrieben werden, z. B., wenn Sie die Vorbereitungen
                            zu einer Inventur treffen, die zu einem späteren Zeitpunkt durchgeführt wer-
                            den soll.

                            Alle Artikel Sie können die Inventur für alle Artikel durchführen, die als Pro-
                            dukte in den Stammdaten erfasst sind.

                            Artikelnummer von … bis Sie können die Inventurliste für einen bestimm-
                            ten Bereich von Artikelnummern erstellen, indem Sie die entsprechenden
                            Nummern eingeben. Diese Felder sind gesperrt, wenn die Checkbox Alle Ar-
                            tikel markiert ist.

                            Lagerbewertung
                            Mit der Wahl einer Option legen Sie fest, wie der Lagerwert zur Inventur ermit-
                            telt werden soll. Der entsprechende Wert wird in der Spalte EK/PE in der In-
                            venturliste angezeigt. Der Wert kann auf der Zählliste gedruckt werden.
                            • EK-Preisliste:
                                Die Einzelpreise der Produkte aus der EK-Tarifzuordnung werden zur La-
                                gerbewertung herangezogen.
                            • Niedrigster EK:
                                Für alle Artikel wird jeweils der niedrigste Wert zur Lagerbewertung heran-
5.20 / 04-2020




                                gezogen.
                            • Geschnittener EK:
                                Für alle Artikel wird jeweils der Durchschnitts-EK zur Lagerbewertung her-


                 G-168                                                             A+W Business Fertigung
                 Softwarereferenz                                                                                  Inventur




                                             angezogen. Dazu muss in den Firmendaten die Option Durchschnitts-EK
                                             aktiviert sein.
                                              Stammdaten, “Durchschnitts EK: Der Durchschnittspreis für den Einkauf wird in
                                               folgenden Fällen neu berechnet:” auf Seite B-957

                                          Nur Produkte mit Lagerbestand > 0 Sie können die Inventur auf die Lager-
                                          artikel mit Bestand einschränken.
                                          ☐ Der komplette Produktstamm inklusive Lagermaßtabelle wird in die Inven-
                                          turliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien einge-
                                          schränkt wird.
                                          ☑ Nur die Lagerartikel werden in die Inventurliste übernommen, zu denen ein
                                          Bestand vorhanden ist.
                                          Die Checkboxen Nur Produkte mit Lagerführung in dem Produkt und Keine
                                          Kisten mit Identnummer und Bestand = 0 werden markiert und gesperrt.

                                          Nur Produkte mit zugeordnetem Lagerprodukt Sie können die Inventur
                                          auf Lagerartikel einschränken.
                                          ☐ Der komplette Produktstamm inklusive Lagermaßtabelle wird in die Inven-
                                          turliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien einge-
                                          schränkt wird.
                                          ☑ Nur die Lagerartikel werden in die Inventurliste übernommen, die in der La-
                                          gerverwaltung angelegt sind.

                                          Nur Produkte mit Lagerführung in dem Produkt Sie können die Inventur
                                          auf die Produkte mit einem Lagerkennzeichen einschränken.
                                          ☐ Der komplette Produktstamm inklusive Lagermaßtabelle wird in die Inven-
                                          turliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien einge-
                                          schränkt wird.
                                          ☑ Nur Artikel mit der Beschaffungsart Lagerentnahme werden in die Inventur-
                                          liste aufgenommen.
                                          Die Checkbox ist markiert und gesperrt, wenn die Checkbox Nur Produkte mit
                                          Lagerbestand > 0 markiert ist.

                                          Keine Kisten mit Identnummer und Bestand = 0 Im Lagerbestand kön-
                                          nen sich Kisten befinden, die bereits ausgeliefert sind, aber nicht gelöscht wur-
                                          den. Deren Bestand wird korrekt mit 0 angezeigt.
                                          ☐ Alle Kisten werden in der Inventurliste aufgeführt.
                                          ☑ Kisten mit einer ID und einem Bestand = 0 werden nicht in der Inventurliste
                                          aufgeführt.
                                          Die Checkbox ist markiert und gesperrt, wenn die Checkbox Nur Produkte mit
                                          Lagerbestand > 0 markiert ist.

                                          Nur für bestimmten Lagerort Sie können die Inventur auf einen Lagerort
                                          einschränken.
                                          ☐ Die Inventur wird für alle Lagerorte durchgeführt. Sie wird nicht auf einen
                                          Lagerort eingeschränkt.
                                          ☑ Die Inventur wird für einen Lagerort durchgeführt. Zur Bestimmung des La-
                                          gerorts werden die Komboboxen Warenlager, Gang, Regal und Fach (Ebene
5.20 / 04-2020




                                          1 bis 4) freigeschaltet. Diese Einstellung ist nur dann sinnvoll, wenn die Be-
                                          stände Ihrer Lagerorte in unterschiedlichen Zeiträumen überprüft werden.



                 A+W Business Fertigung                                                                              G-169
                 Inventur                                                                   Softwarereferenz




                                Lagerort <k.A.>
                                Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                <k.A.> erhalten und können bebucht werden.

                            Warenhaus, Regal, Gang, Fach Sie können die Inventurliste auf einen La-
                            gerort einschränken. Die Felder sind nur freigeschaltet, wenn die Checkbox
                            Nur für bestimmten Lagerort markiert ist.

                            Sortierung
                            Mit der Wahl der Option legen Sie die Sortierung der Inventurliste fest. Stan-
                            dardmäßig ist die Option Artikel aktiviert.

                            Übersicht
                            In der Übersicht sind alle Artikel aufgelistet, die in der Inventur gezählt und be-
                            wertet werden sollen.
                            •   Beleg Nr.:
                                Laufende Nummer in der Inventurliste.
                            •   Art. Nr.:
                                Produktnummer aus den Stammdaten.
                            •   Bezeichnung:
                                Produktbezeichnung aus den Stammdaten.
                            •   Farbe:
                                Die Farbe wird nur angegeben, wenn das Produkt mit Varianten/Farben
                                angelegt ist.
                            •   Breite, Höhe:
                                Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder
                                Kiste mit festen Größen angelegt ist. Bei allen nicht maßabhängigen Pro-
                                dukten wird der Wert 0 angezeigt.
                            •   EK / PE:
                                Einkaufspreis (EK) pro Preiseinheit. Je nach Einstellung ist das der nied-
                                rigste oder der Durchschnitts-EK.
                            •   PE:
                                Preiseinheit für den EK.
                            •   EK / Blatt:
                                Der EK-Preis pro Blatt wird nur bei Lagermaßen angezeigt. Er wird errech-
                                net aus dem EK/PE und der tatsächlichen Größe der Platte. Wenn ein
                                Stückpreis hinterlegt ist, sind die Werte in den Spalten EK/PE und EK/Blatt
                                identisch.
                            •   Soll:
                                Der Sollbestand gibt an, welche Menge in A+W Business den durchgeführ-
                                ten Buchungen gemäß gespeichert ist. Er wird erst angezeigt, wenn der
                                Sollbestand ermittelt wurde.
                                 “Sollbestand” auf Seite G-173
                            •   ME:
                                Mengeneinheit, mit der das Produkt im Lager geführt wird.
5.20 / 04-2020




                 G-170                                                             A+W Business Fertigung
                 Softwarereferenz                                                                                  Inventur




                                          Listendruck
                                          Lagerwirtschaft > Inventur > Inventurliste > Menü Druck




                                          Abb. G-89     Druck – Inventurliste


                                          In diesem Dialog können Sie einstellen, wie die Zähllisten gedruckt werden
                                          sollen. Damit können Sie die Blätter für die manuelle Erfassung der Bestände
                                          Ihrem Lager und den Inventur-Aufgaben Ihrer Mitarbeiter entsprechend ge-
                                          stalten.
                                           Tutorial, “So drucken Sie die Zähllisten” auf Seite G-148

                                             Sollbestand in der Zählliste
                                             Der Sollbestand kann nur in der Zählliste gedruckt werden, wenn er vor
                                             dem Druck ermittelt wurde.

                                              “Sollbestand” auf Seite G-173

                                          Seitenumbruch nach Wechsel von

                                          Lagerhaus, Lagergang, Lagerregal, Lagerfach Wenn Sie die Zählliste
                                          nach dem Lagerort sortieren, können Sie zusätzlich angeben, nach welchen
                                          Lagerebenen ein Seitenumbruch erfolgen soll.
                                          Die Einstellung ist sinnvoll, wenn Sie die Zählliste nach Lagerorten sortiert dru-
                                          cken. Sie können damit für jede Ebene ein eigenes Blatt drucken.
                                           “Sortiert nach” auf Seite G-172

                                          Parameter
                                          Mit der Wahl der Option legen Sie fest, welche Produkte in der Zählliste auf-
5.20 / 04-2020




                                          geführt werden sollen.
                                          Die Optionen Fertigprodukte und Rohmaterial beziehen sich auf das Kennzei-
                                          chen Rohmaterial aus der Lagerdefinition. Wenn das Kennzeichen Rohmate-


                 A+W Business Fertigung                                                                             G-171
                 Inventur                                                                Softwarereferenz




                            rial nicht gesetzt ist, wertet das System den entsprechenden Lagerort
                            automatisch als Lagerort für Fertigprodukte.
                             Stammdaten, “Lagerdefinition” auf Seite B-737
                            •   Alle Artikel:
                                Alle Artikel der Inventurliste werden in der Zählliste gedruckt.
                            •   Fertigprodukte:
                                Nur die Artikel der Inventurliste werden gedruckt, deren Lagerort nicht für
                                Rohmaterial bestimmt ist.
                            •   Rohmaterial:
                                Nur die Produkte der Inventurliste werden gedruckt, die sich an einem La-
                                gerort für Rohmaterial befinden.
                            •   Preise drucken:
                                Die Zählliste kann wahlweise mit oder ohne die Preise gedruckt werden.
                            •   Sollbestand drucken:
                                Der Sollbestand kann nur auf den Zähllisten gedruckt werden, wenn die
                                Sollbestandsermittlung ausgeführt wurde.

                            Sortiert nach Mit der Wahl der Option legen Sie fest, wie die Artikel auf der
                            Zählliste sortiert werden sollen:
                            • Artikel:
                              Die Liste wird nach Produktnummern sortiert.
                            • Abmessung:
                              Wenn die Zählliste Lagermaße enthält, werden die Einträge nach Breite/
                              Höhe sortiert gedruckt.
                            • Lagerort:
                              Wenn die Artikel der Zählliste an verschiedenen Lagerorten gehalten wer-
                              den, ist die Sortierung nach Lagerorten sinnvoll. Zusätzlich können Sie Sei-
                              tenumbrüche festlegen.
                                 “Seitenumbruch nach Wechsel von” auf Seite G-171

                            Lagerorte drucken
                            In der Übersicht werden alle Lagerorte aufgeführt, die in den Stammdaten de-
                            finiert oder für die Inventurliste ausgewählt wurden. Sie können bestimmen,
                            ob die Lagerorte in der Zählliste gedruckt werden sollen. Wenn Sie Lagerorte
                            mit drucken möchten, müssen Sie mindestens einen auswählen.

                                Lagerort <k.A.>
                                Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                <k.A.> erhalten und können bebucht werden.
5.20 / 04-2020




                 G-172                                                          A+W Business Fertigung
                 Softwarereferenz                                                                                 Inventur




                                          Sollbestand
                                          Lagerwirtschaft > Inventur > Sollbestand




                                          Abb. G-90     Sollbestand


                                          Der Sollbestand entspricht dem Bestand, der vom System durch automatische
                                          oder manuelle Buchungen ermittelt wird. Er wird jeweils für eine bestimmte In-
                                          venturliste und alle Artikel ermittelt, die in der gewählten Inventurliste aufge-
                                          führt sind.
                                           Tutorial, “Sollbestand ermitteln” auf Seite G-150

                                             Keine Lagerveränderungen am Zähltag
                                             Nachdem der Sollbestand ermittelt wurde, müssen die Bestände gezählt
                                             werden. Am Tag der Zählung dürfen keine Lagerartikel entnommen und
                                             keine Lagerbewegungen gebucht werden, bis die Zählung abgeschlossen
                                             ist. A+W Business wird nicht automatisch für Buchungen gesperrt.

                                          Parameter

                                          Inv. Datum In der Kombobox werden alle Inventurlisten aufgeführt, die noch
                                          im System gespeichert sind. Aus dem Datum ist nicht ersichtlich, ob die Inven-
                                          tur abgeschlossen ist.
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-173
                 Inventur                                                               Softwarereferenz




                            Liste
                            •   Beleg Nr.:
                                Laufende Nummer in der Inventurliste.
                            •   Art. Nr.:
                                Produktnummer aus den Stammdaten.
                            •   Bezeichnung:
                                Produktbezeichnung aus den Stammdaten.
                            •   Ident:
                                Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                            •   Inhalt:
                                Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten
                                die Anzahl der Blätter.
                            •   Breite, Höhe:
                                Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder
                                Kiste angelegt ist.
                            •   Farbe:
                                Die Farbe wird nur angegeben, wenn das Produkt als Variante angelegt ist.
                            •   Lagerort:
                                Lagerort in der Reihenfolge von Ebene 1 bis 4.
                            •   EK / PE:
                                Einkaufspreis (EK) pro Preiseinheit. Je nach Einstellung ist das der nied-
                                rigste oder der Durchschnitts-EK.
                            •   PE:
                                Preiseinheit für den EK.
                            •   Kat.:
                                Diese Funktion wird nur kundenspezifisch verwendet.
                            •   Soll:
                                Bestand, der laut System vorhanden sein sollte. Die Werte werden erst an-
                                gezeigt, wenn der Sollbestand ermittelt wurde.
                            •   ME:
                                Mengeneinheit, mit der das Produkt im Lager geführt wird.
5.20 / 04-2020




                 G-174                                                          A+W Business Fertigung
                 Softwarereferenz                                                                       Inventurverwaltung




                                          Inventurverwaltung
                                          Lagerwirtschaft > Inventur > Verwaltung
                                          Sie geben die gezählten Mengen im Dialog Verwaltung ein. Lagerbuchungen
                                          können direkt nach dem Zählen wieder durchgeführt werden.
                                          In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                          •   “Menüs in der Inventurverwaltung” auf Seite G-175
                                          •   “Verwaltung” auf Seite G-176
                                          •   “Gehe zu Artikel” auf Seite G-179


                                          Menüs in der Inventurverwaltung
                                          Lagerwirtschaft > Inventur > Verwaltung
                                          Über die Menüs der Inventurverwaltung können Sie die Standardeinstellung
                                          des Dialoges bestimmen und andere Dialoge öffnen, ohne die Inventurverwal-
                                          tung zu schließen.
                                          In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                          •   “Menü Optionen” auf Seite G-175
                                          •   “Menü Funktionen” auf Seite G-176


                                          Menü Optionen
                                          Lagerwirtschaft > Inventur > Verwaltung

                                          Gruppe Lagermaße
                                          •   Fläche der Lagermaße automatisch berechnen:
                                              Die Fläche der gezählten Lagerplatten wird automatisch in Quadratmetern
                                              angezeigt.

                                          Gruppe Sortierung
                                          •   Artikel / Lagerort / Abmessung:
                                              Die Liste ist nach Artikeln sortiert. Diese Sortierung ist sinnvoll, wenn glei-
                                              che Artikel an mehreren Lagerorten untergebracht sind.
                                          •   Abmessung / Artikel / Lagerort:
                                              Die Liste ist nach den Größen der Lagermaße sortiert. Diese Sortierung ist
                                              sinnvoll, wenn Sie die Lagermaße in eigenen Zähllisten erfasst haben.
                                          •   Lagerort / Artikel / Abmessung:
                                              Die Liste wird nach Lagerorten sortiert. Diese Sortierung ist sinnvoll, wenn
                                              Sie auch die Zähllisten nach Lagerorten sortiert haben.
                                          •   Beleg Nr.:
                                              Belegnummer aus der Inventurliste
5.20 / 04-2020




                 A+W Business Fertigung                                                                              G-175
                 Inventurverwaltung                                                                 Softwarereferenz




                                      Menü Funktionen
                                      Lagerwirtschaft > Inventur > Verwaltung
                                      Folgende Einträge werden angezeigt:
                                      •   Gehe zu Artikel:
                                          Öffnet den Dialog Gehe zu Artikel.
                                           “Gehe zu Artikel” auf Seite G-179
                                      •   Menge für markierte Artikel auf Null setzen:
                                          Die Menge wird auf null gesetzt. Diese Funktion ist sinnvoll, wenn Sie meh-
                                          rere Belege markieren. Sie brauchen dann nicht jeden einzelnen auf null
                                          zu setzen.
                                      •   Lagerort für markierte Artikel setzen:
                                          Der Lagerort wird für alle markierten Belege umgesetzt.


                                      Verwaltung
                                      Lagerwirtschaft > Inventur > Verwaltung




                                      Abb. G-91     Inventurverwaltung


                                      In diesem Dialog erfassen Sie die gezählten Mengen. Die Liste zeigt die Ein-
                                      träge, die Sie mit der Inventurliste ausgewählt haben. Lagerbuchungen kön-
                                      nen direkt nach dem Zählen wieder durchgeführt werden.
                                       Tutorial, “Inventurwerte erfassen” auf Seite G-152
5.20 / 04-2020




                 G-176                                                                       A+W Business Fertigung
                 Softwarereferenz                                                                     Inventurverwaltung




                                             Kiste inventarisieren
                                             Wenn für die Inventurliste der Sollbestand ermittelt wurde, können Kisten
                                             auch per Scanner erfasst und in die Inventurliste aufgenommen werden.
                                             Dazu müssen die Kisten-ID, der Lagerort und ggf. eine abweichende Blatt-
                                             anzahl gescannt werden.

                                          Eingabemaske

                                          Inventurdatum Angabe des Datums der Inventurliste.

                                          Artikelnummer Nummer des Artikels, dessen Menge erfasst werden soll.

                                          Breite, Höhe Die Maße werden nur bei Lagerplatten und Kisten eingetra-
                                          gen. Für alle anderen Artikel steht in den beiden Feldern eine Null (0).

                                          Kategorie Diese Funktion wird nur kundenspezifisch verwendet, um Katego-
                                          rien für die Wertberichtigung des Lagers zu verwenden.

                                          Inv. Preis Für die Lagerbewertung kann ein Inventurpreis manuell eingetra-
                                          gen werden. Dieser Preis wird nach dem Abschluss der Inventur nicht in die
                                          EK-Preistabelle zurückgeschrieben und fließt nicht in die Berechnung des
                                          Durchschnitts-EKs ein.
                                          Wenn kein Inventurpreis eingetragen wird, gilt der niedrigste oder der Durch-
                                          schnitts-EK je nach Einstellung in der Inventurliste.

                                          Inhalt Anzeige der Stückzahl bei Kisten. Wenn Kisten als Einheit gezählt
                                          wurden, darf die Kiste nicht aufgelöst sein, d. h., es dürfen keine Platten ent-
                                          nommen sein.

                                          Bezeichnung Artikelbezeichnung aus den Produktstammdaten.

                                          Farbe Bei Artikeln mit Farbzuweisungen (Variante) kann die Stückzahl pro
                                          Farbe eingetragen werden.

                                          Ident Kisten-ID (manuelle Buchung oder aus dem Wareneingang).

                                          Lagerort Lagerort des gezählten Artikels.

                                             Lagerort <k.A.>
                                             Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                             <k.A.> erhalten und können bebucht werden.

                                          Menge In diesem Feld erfassen Sie die gezählte Menge aus der Zählliste. Sie
                                          können die Mengen erst eingeben, nachdem Sie den Sollbestand ermittelt ha-
                                          ben.
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-177
                 Inventurverwaltung                                                                   Softwarereferenz




                                      Tabelle
                                      In der Übersicht sind alle Artikel aufgelistet, die in der Inventur gezählt und be-
                                      wertet werden sollen.
                                      •   Beleg Nr.:
                                          Laufende Nummer in der Inventurliste.
                                      •   Art. Nr.:
                                          Produktnummer aus den Stammdaten.
                                      •   Bezeichnung:
                                          Produktbezeichnung aus den Stammdaten.
                                      •   Inhalt:
                                          Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten
                                          die Anzahl der Blätter.
                                      •   Ident:
                                          Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                      •   Breite, Höhe:
                                          Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder
                                          Kiste angelegt ist.
                                      •   Lagerort:
                                          Lagerort in der Reihenfolge von Ebene 1 bis 4.
                                      •   EK / PE:
                                          Einkaufspreis (EK) pro Preiseinheit. Je nach Einstellung ist das der nied-
                                          rigste oder der Durchschnitts-EK.
                                      •   PE:
                                          Preiseinheit für den EK.
                                      •   Kategorie:
                                          Diese Funktion wird nur kundenspezifisch verwendet.
                                      •   Menge:
                                          Wert, der als gezählte Menge eingegeben wurde.
                                      •   ME:
                                          Mengeneinheit, mit der das Produkt im Lager geführt wird.
5.20 / 04-2020




                 G-178                                                                       A+W Business Fertigung
                 Softwarereferenz                                                                  Inventurverwaltung




                                          Gehe zu Artikel
                                          Lagerwirtschaft > Inventur > Verwaltung > Menü Funktionen > Gehe zu Arti-
                                          kel…




                                          Abb. G-92    Gehe zu Artikel


                                          In diesem Dialog können Sie die Markierung auf den ersten Beleg zum ange-
                                          gebenen Artikel setzen.

                                          Artikel Nummer des Lagerartikels, zu dem Sie in der Liste springen möchten.


                                          Wertberichtigung
                                          Lagerwirtschaft > Inventur > Verwaltung > Feld Kategorie > Symbol Ordner




                                          Abb. G-93    Wertberichtigung


                                          In diesem Dialog hinterlegen Sie Kategorien und Prozentwerte für die Berich-
                                          tigung des Lagerwerts.
                                          Der Dialog ist nur kundenspezifisch freigeschaltet.
5.20 / 04-2020




                 A+W Business Fertigung                                                                        G-179
                 Inventurabschluss                                                                 Softwarereferenz




                                     Inventurabschluss
                                     Lagerwirtschaft > Inventur > Abschluss
                                     Mit dem Inventurabschluss beenden Sie die Inventur. Lagerbuchungen kön-
                                     nen direkt nach dem Zählen wieder durchgeführt werden.
                                     In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                     •   “Menüs im Inventurabschluss” auf Seite G-180
                                     •   “Abschluss” auf Seite G-181


                                     Menüs im Inventurabschluss
                                     Lagerwirtschaft > Inventur > Abschluss
                                     Über die Menüs können Sie die Standardeinstellung bestimmen und andere
                                     Dialoge öffnen, ohne den Dialog zu schließen.
                                     In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                     •   “Menü Optionen” auf Seite G-180
                                     •   “Menü Funktionen” auf Seite G-180


                                     Menü Optionen
                                     Lagerwirtschaft > Inventur > Abschluss
                                     Folgende Einträge werden angezeigt:
                                     •   Artikel mit Bestand = 0 nicht drucken:
                                         Nur Artikel, deren Bestand größer als 0 ist, werden gedruckt. Diese Einstel-
                                         lung ist sinnvoll, wenn es sehr viele Artikel ohne Bestandszahlen gibt. Die
                                         gedruckte Liste wird dann übersichtlicher.
                                     •   Bei nicht gezählten Artikeln nachfragen, ob Bestand auf 0 gesetzt werden
                                         soll:
                                         Mit dieser Funktion legen Sie fest, dass die Menge von Artikel, zu denen
                                         kein Bestand erfasst wurde, erst dann auf 0 gesetzt wird, wenn Sie dies pro
                                         Artikel bestätigt haben.


                                     Menü Funktionen
                                     Lagerwirtschaft > Inventur > Abschluss
                                     Folgende Einträge werden angezeigt:
                                     •   Nachtragsinventur anhängen:
                                         Öffnet den Dialog Inventurliste wählen, um zwei verschiedene Inventuren
                                         in einer gemeinsamen Liste zu drucken und auszuwerten.
                                          “Inventurliste wählen” auf Seite G-183
5.20 / 04-2020




                 G-180                                                                    A+W Business Fertigung
                 Softwarereferenz                                                                     Inventurabschluss




                                          Abschluss
                                          Lagerwirtschaft > Inventur > Abschluss




                                          Abb. G-94    Inventurabschluss


                                          In diesem Dialog schließen Sie die Inventur pro Inventurliste einzeln ab. Damit
                                          werden die erfassten Werte in die Lagerbestände (Bestandslisten) übernom-
                                          men. Ab- und Zugänge, die in der Zwischenzeit erfasst wurden, werden dabei
                                          berücksichtigt. Neue Lagerartikel aus der Inventur werden automatisch in die
                                          Lagerverwaltung übernommen.
                                           Tutorial, “Inventur abschließen” auf Seite G-154

                                             Pro Inventurliste nur ein Abschluss
                                             Der Inventurabschluss kann nur einmal pro Inventurliste ausgeführt wer-
                                             den. Eingabefehler können nach dem Abschluss nur in der Lagerverwal-
                                             tung korrigiert werden. Alternativ dazu kann eine neue Inventurliste mit den
                                             fehlerhaft erfassten Artikeln erstellt werden.
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-181
                 Inventurabschluss                                                              Softwarereferenz




                                     Einbuchung

                                     Inventurdatum Datum der Inventur, die abgeschlossen werden soll.

                                     Verbuchung nach Beschaffungsart aus AV-Bereich Wenn Sie mit AV-Be-
                                     reichen arbeiten, können die Bestände einem bestimmten AV-Bereich zuge-
                                     ordnet sein, z. B. für die Produktion von VSG. Das Feld zur Auswahl des AV-
                                     Bereichs ist nur freigeschaltet, wenn Sie die Checkbox markiert haben.
                                     ☐ Die gezählten Bestände werden dem Standard-Lagerort zugeordnet.
                                     ☑ Die Bestände sollen einem AV-Bereich zugeordnet werden.
                                      Stammdaten, “AV-Bereiche” auf Seite B-1019

                                     Beleg Nr. von … bis Anzeige der ersten und letzten Belegnummer der ge-
                                     ladenen Inventurliste.

                                     Übersicht
                                     •   Beleg Nr.:
                                         Laufende Nummer in der Inventurliste.
                                     •   Art. Nr.:
                                         Produktnummer aus den Stammdaten.
                                     •   Bezeichnung:
                                         Produktbezeichnung aus den Stammdaten.
                                     •   Inhalt:
                                         Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten
                                         die Anzahl der Blätter.
                                     •   Ident:
                                         Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                     •   Breite, Höhe:
                                         Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder
                                         Kiste angelegt ist.
                                     •   Lagerort:
                                         Lagerort in der Reihenfolge von Ebene 1 bis 4.
                                     •   Menge:
                                         Wert, der als gezählte Menge eingegeben wurde.
                                     •   ME:
                                         Mengeneinheit, mit der das Produkt im Lager geführt wird.
                                     •   Status:
                                         Ein Status wird nur angezeigt, wenn der Beleg nicht verbucht werden konn-
                                         te. Über das Logbuch können Sie nach den möglichen Ursachen suchen.
5.20 / 04-2020




                 G-182                                                                  A+W Business Fertigung
                 Softwarereferenz                                                                       Inventurabschluss




                                          Inventurliste wählen
                                          Lagerwirtschaft > Inventur > Abschluss > Menü Funktionen > Nachtragsinven-
                                          tur anhängen




                                          Abb. G-95    Nachtragsinventur anhängen


                                          Eine Nachtragsinventur kann nur angehängt werden, wenn beide Inventuren
                                          abgeschlossen sind. Die beiden Inventuren können dann auf einer gemeinsa-
                                          men Liste gedruckt und ausgewertet werden.
                                           Tutorial, “So hängen Sie eine Nachtragsinventur an” auf Seite G-156
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-183
                 Lagerverwaltung                                                                Softwarereferenz




                                   Lagerverwaltung
                                   Lagerwirtschaft > Lagerverwaltung
                                   Im Dialog Lagerverwaltung können Sie sich alle Artikel anzeigen lassen, die
                                   im Lager verwaltet werden.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menüs in der Lageverwaltung” auf Seite G-184
                                   •   “Lagerverwaltung” auf Seite G-185


                                   Menüs in der Lageverwaltung
                                   Lagerwirtschaft > Lagerverwaltung
                                   Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen
                                   und andere Dialoge öffnen, ohne den Dialog zu schließen.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menü Funktionen” auf Seite G-184
                                   •   “Menü Optionen” auf Seite G-185
                                   •   “Menü Druck” auf Seite G-185


                                   Menü Funktionen
                                   Lagerwirtschaft > Lagerverwaltung > Menü Funktionen
                                   Über dieses Menü können Sie andere Dialoge öffnen, ohne die Lagerverwal-
                                   tung zu schließen.
                                   Folgende Einträge werden angezeigt:
                                   •   Lagerhistorie:
                                       Öffnet den Dialog Lagerhistorie mit dem Protokoll der Vorgänge, die in der
                                       Lagerverwaltung gebucht wurden.
                                        “Lagerhistorie” auf Seite G-204
                                   •   Buchungsjournal:
                                       Öffnet den Dialog Buchungsjournal mit dem Protokoll der Lagerbuchungen
                                       aus Aufträgen und Bestellungen.
                                        “Buchungsjournal” auf Seite G-202
5.20 / 04-2020




                 G-184                                                                 A+W Business Fertigung
                 Softwarereferenz                                                                       Lagerverwaltung




                                          Menü Optionen
                                          Lagerwirtschaft > Lagerverwaltung > Menü Optionen
                                          Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                          men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                          wird nicht zurückgesetzt, wenn Sie den Dialog schließen.
                                          Folgende Einträge werden angezeigt:
                                          •   Artikel mit Bestand = 0 nicht drucken:
                                              Nur Artikel, deren Bestand größer als 0 ist, werden gedruckt. Diese Einstel-
                                              lung ist sinnvoll, wenn es sehr viele Kisten mit einer ID aber ohne Bestand
                                              gibt. Diese sind dann in der Regel als Kiste ausgeliefert worden und aus
                                              dem Bestand gelöscht. Die Einstellung gilt nur für den Druck, im Dialog
                                              werden alle Artikel angezeigt.
                                          •   Identnummer automatisch vergeben:
                                              Die ID der Kiste kann auch automatisch vergeben werden, wenn sie ma-
                                              nuell als Bestand gebucht wird.


                                          Menü Druck
                                          Lagerwirtschaft > Lagerverwaltung > Menü Druck
                                          Über dieses Menü können Sie den Druck von Etiketten starten.
                                          Folgende Einträge werden angezeigt:
                                          •   Kistenetiketten:
                                              Nur Etiketten für Kisten werden gedruckt. Dazu muss der Druckpunkt 973
                                              angelegt und in der Formularverwaltung der Report boxlabel.qrp zugewie-
                                              sen sein.
                                          •   Standard:
                                              Etiketten für die Lagerartikel werden gedruckt.


                                          Lagerverwaltung
                                          Lagerwirtschaft > Lagerverwaltung
                                          Im Dialog Lagerverwaltung werden die Lagerartikel erfasst, die im Lager mit
                                          Beständen gehalten werden.
                                          Lagermaße werden in A+W Business auch in der Produktverwaltung gepflegt.
                                          Sie dienen dort dazu, Preisschlüssel, Warengruppen, usw. zuzuordnen.
                                          Im Dialog Lagerverwaltung finden Sie folgende Register:
                                          •   Lagerverwaltung – Lagerartikel
                                          •   Lagerverwaltung – Preise
                                          •   Lagerverwaltung – Zusatz
5.20 / 04-2020




                 A+W Business Fertigung                                                                           G-185
                 Lagerverwaltung                                                                            Softwarereferenz




                                              Lagerverwaltung auf der Ebene der Stücklisten
                                              Sie können im Lager auch Produkte verwalten, die als Stücklisten-Kompo-
                                              nenten in anderen Produkten enthalten sind. Dazu muss in den Firmenda-
                                              ten die Checkbox Lagerführung auf Stücklistenebene aktiviert sein.

                                               Tutorial, “Lagerführung auf Stücklistenebene” auf Seite G-61
                                               Stammdaten, “Lagerführung auf Stücklistenebene” auf Seite B-960


                                          Lagerverwaltung – Lagerartikel
                                          Lagerwirtschaft > Lagerverwaltung > Register Lager-Artikel




                 Abb. G-96   Lagerverwaltung – Lagerartikel


                                          In diesem Register können Sie die Artikel prüfen, die im Lager verwaltet wer-
                                          den. Der angezeigte Bestand wird mit jeder Lagerbuchung aktualisiert. Sie
                                          können neue Artikel hinzufügen und die verschiedenen Mengen korrigieren.
                                          Für das Bestellwesen legen Sie außerdem Mindest- und Bestellmengen fest.
                                           Tutorial, “So legen Sie einen Lagerartikel an” auf Seite G-74

                                          Identifikation

                                          Artikel Produktnummer aus den Stammdaten. Wenn Sie einen neuen La-
5.20 / 04-2020




                                          gerartikel erfassen möchten, müssen Sie ihn zuerst in den Stammdaten anle-
                                          gen.




                 G-186                                                                            A+W Business Fertigung
                 Softwarereferenz                                                                         Lagerverwaltung




                                          Lager-ID Identnummer, die beim Wareneingang vergeben wurde.

                                          Bezeichnung Produktbezeichnungen aus den Stammdaten.

                                          Breite x Höhe / Inhalt Maße des Lagerartikels in mm (nur Lagermaße) und
                                          Inhalt der Kiste. Bei Kisten tragen Sie ein, wie viele Blätter die Kiste enthält.
                                          Für alle anderen Lagerartikel steht automatisch eine 1.

                                          Variante Wenn zu einem Artikel Varianten angelegt sind, so wird die Farbe
                                          angezeigt.

                                          Default-Lagerort Wenn Sie Lagerorte definiert haben, werden diese zur
                                          Auswahl angeboten.
                                          Wenn Sie einen Lagerartikel an mehreren Lagerorten halten, kann ein Stan-
                                          dard-Lagerort festgelegt werden.
                                          ☐ Der angezeigte Lagerort ist für den Lagerartikel nicht als Standard festge-
                                          legt.
                                          ☑ Der angezeigte Lagerort ist für den Lagerartikel als Standard-Lagerort fest-
                                          gelegt.
                                           Stammdaten, “Lagerdefinition” auf Seite B-737

                                             Lagerort <k.A.>
                                             Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                             <k.A.> erhalten und können bebucht werden.

                                          Ident. Die Kisten-ID, die beim Wareneingang oder manuell vergeben wurde.
                                          Die ID wird nur angezeigt, wenn Sie in der Übersicht der Lagerartikel eine Kis-
                                          te markiert haben.

                                          Details

                                          Kategorie Wenn Sie in den Stammdaten Lagerkategorien definiert haben,
                                          können Sie dieses Feld als Suchkriterium verwenden. Beim Anlegen neuer
                                          Lagerartikel können Sie eine Kategorie zuordnen.

                                          Lief.-Ident Die Kisten-ID des Lieferanten wird nur angezeigt, wenn Sie im
                                          Bereich Lagerartikel eine Kiste markiert haben.

                                          Hauptartikel Lagerartikel mit mehreren Maßen können Sie miteinander ver-
                                          knüpfen, indem Sie einen Hauptartikel angeben. Die Bestandsprüfung (für die
                                          Lagervorschau im Dialog Lagerinfo) wird dann nur für den Hauptartikel durch-
                                          geführt und nur für diesen müssen Sie einen Mindestbestand hinterlegen.
                                          Wenn bei den zugeordneten Lagerartikeln ebenfalls Mindestbestände festge-
                                          legt sind, werden diese bei der Prüfung ignoriert.
                                           Tutorial, “Lager-Hauptartikel” auf Seite G-70

                                          Produktionslauf / Datum Zur Zeit nicht genutzt.
5.20 / 04-2020




                                          Datum Datum, an dem der Lagerartikel zuletzt geändert wurde.




                 A+W Business Fertigung                                                                             G-187
                 Lagerverwaltung                                                               Softwarereferenz




                                   In Produktion In Verbindung mit A+W Production können Sie festlegen, ob
                                   der Lagerartikel der Produktion zugeordnet ist.
                                   ☐ Der Lagerartikel ist frei verfügbar.
                                   ☑ Der Lagerartikel ist der Produktion zugeordnet (nur Info).

                                   Bestände

                                   Lagerbestand Anzeige des aktuellen Bestands. Der Bestand wird bei jeder
                                   Ab- oder Zubuchung aktualisiert. Für Kisten mit einer ID wird jeweils der Be-
                                   stand 1 angezeigt.
                                   Wenn Sie den Lagerartikel neu angelegt haben, ist das Feld freigeschaltet und
                                   Sie können den Anfangsbestand eintragen.

                                   Bestand > 0 Diese Checkbox ist nur im Auswahlmodus freigeschaltet. Sie
                                   können damit als Suchkriterium festlegen, ob Artikel ohne Bestandsmenge
                                   angezeigt werden.
                                   ☐ Im Suchergebnis werden auch Artikel angezeigt, deren aktueller Bestand 0
                                   ist.
                                   ☑ Im Suchergebnis werden nur Artikel angezeigt, deren aktueller Bestand
                                   mindestens 1 ist.

                                   Mindestbestand Der Mindestbestand bildet die Grundlage für automatische
                                   Bestellvorschläge. Sie werden erzeugt, wenn der Lagerbestand den Mindest-
                                   bestand unterschreitet. Dabei werden die Reservierungen und die Bestellun-
                                   gen mitberücksichtigt. Diese automatischen Bestellvorschläge können Sie im
                                   Dialog Lagerbestellung prüfen und an den Einkauf übergeben.
                                    “Lagerbestellung” auf Seite G-220

                                   Mindestbestand > 0 Diese Checkbox ist nur im Auswahlmodus freigeschal-
                                   tet. Sie können damit als Suchkriterium festlegen, ob der Mindestbestand grö-
                                   ßer als 0 sein muss.
                                   ☐ Im Suchergebnis werden alle Artikel angezeigt.
                                   ☑ Im Suchergebnis werden nur Artikel angezeigt, deren Mindestbestand grö-
                                   ßer als Null ist.

                                   Bestellmenge Dieser Wert gibt an, welche Menge standardmäßig bestellt
                                   wird. Bei der automatischen Lagerbestellung wird der Wert übernommen.

                                   Bestand < Mindestbestand Diese Checkbox ist nur im Auswahlmodus frei-
                                   geschaltet. Sie können damit als Suchkriterium festlegen, ob der Bestand un-
                                   ter dem Mindestbestand liegen soll.
                                   ☐ Im Suchergebnis werden alle Artikel angezeigt.
                                   ☑ Im Suchergebnis werden nur Artikel angezeigt, deren aktueller Bestand
                                   kleiner als der Mindestbestand ist.

                                   Maximalbestand Mit der Eingabe von Maximalmengen pro Lagerartikel
                                   kann verhindert werden, dass das Lager überfüllt ist. Der eingetragene Wert
                                   dient nur der manuellen Kontrolle.
5.20 / 04-2020




                                   Sollbestand Zur Zeit nicht genutzt.



                 G-188                                                                A+W Business Fertigung
                 Softwarereferenz                                                                      Lagerverwaltung




                                          Bestandsprüfung pro Lagerort Wenn Sie den Bestand pro Lagerort pfle-
                                          gen, können Sie die den Bestand pro Lager prüfen.
                                          ☐ Der Bestand wird für alle Lagerorte gemeinsam geprüft.
                                          ☑ Der Bestand wird pro Lagerort geprüft.

                                          Kritischer Lagerbestand Für jeden Lagerartikel können Sie die Menge an-
                                          geben, ab der eine Bestellung zwingend erforderlich ist.
                                          Damit der eingetragene Wert geprüft wird, muss die Option Bestandsprüfung
                                          pro Lagerort aktiviert sein.
                                          In der Lagerwirtschaft wird das Datum berechnet, an dem der Bestand eines
                                          Lagerartikels unter diese kritische Menge fällt. Das Datum, an dem ein Lager-
                                          artikel die kritische Menge erreicht, wird im Bestellpool.
                                           Verkauf, “Bestellübergabe – Bestellpool” auf Seite C-659

                                          Lagerartikel
                                          In den Übersichten werden die Lagerartikel angezeigt, die den Suchkriterien
                                          entsprechen. Die obere Liste zeigt die Lagerartikel insgesamt an. Wenn Sie
                                          einen Eintrag markieren, werden in der unteren Liste die Artikel pro Lagerort
                                          angezeigt. Wenn Checkbox Bestand > 0 aktiviert ist, werden nur Lagerorte
                                          aufgelistet, deren Bestand größer als 0 ist.
                                          Folgende Spalten werden angezeigt:
                                          •   Artikel, Variante:
                                              Artikelnummer, Bezeichnung und Farbe aus der Lagerverwaltung.
                                          •   Breite, Höhe:
                                              Maße aus der Lagerverwaltung.
                                          •   Inhalt:
                                              Anzahl der Blätter in einer Kiste.
                                          •   Ges. Bestand:
                                              Bestand des Lagerartikels aller Lagerorte.
                                          •   Min. Bestand:
                                              Menge des festgelegten Mindestbestands.
                                          •   Best. Menge:
                                              Festgelegte Bestellmenge.

                                          Lagerorte
                                          •   Ident:
                                              Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                          •   Lagerort:
                                              Lagerort in der Reihenfolge von Ebene 1 bis 4.
                                          •   Lagerbestand:
                                              Aktueller Bestand am Lagerort.
                                          •   Lief.-Ident:
                                              Kisten-ID des Lieferanten (nur wenn diese im Wareneingang miterfasst
                                              wurde).
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-189
                 Lagerverwaltung                                                                          Softwarereferenz




                                          Lagerverwaltung – Preise
                                          Lagerwirtschaft > Lagerverwaltung > Register Preise




                 Abb. G-97   Lagerverwaltung – Preise


                                          In diesem Register werden die aktuellen Preise eines Lagerartikels angezeigt.
                                          Bei der Aktualisierung werden Aufträge, Bestellungen und Lagerumbuchun-
                                          gen berücksichtigt.
                                           Tutorial, “Preise” auf Seite G-51

                                             Voraussetzung
                                             Der durchschnittliche Einkaufspreis (Durchschnitts-EK) wird nur dann be-
                                             rechnet und angezeigt, wenn in den Firmendaten die Checkbox Einkaufs-
                                             preis ermitteln und die Option Durchschnitts EK aktiviert sind.

                                              Stammdaten, “Durchschnitts EK: Der Durchschnittspreis für den Einkauf wird in
                                               folgenden Fällen neu berechnet:” auf Seite B-957
                                          Die Felder in den Übersichten sind ausführlich zum Register Lagerartikel be-
                                          schrieben.
                                           “Lagerverwaltung – Lagerartikel” auf Seite G-186

                                          Einkaufspreise
5.20 / 04-2020




                                          Niedrigster Preis Der niedrigste Preis, zu dem der Artikel eingekauft wurde.

                                          Höchstpreis Der höchste Preis, zu dem der Artikel eingekauft wurde.



                 G-190                                                                          A+W Business Fertigung
                 Softwarereferenz                                                                      Lagerverwaltung




                                          Letzter Preis Der jüngste Preis, zu dem der Artikel eingekauft wurde.

                                          Lagerwert In dieser Spalte werden die aktuellen Lagerwerte angezeigt. Sie
                                          ergeben sich aus dem jeweiligen Preis und der Menge.

                                          Berechnung des geschnittenen Preises (Durchschnitts-EK)
                                          Mit der Wahl der Option bestimmen Sie, welche Lagermaße in dieser Über-
                                          sicht bei der Berechnung berücksichtigt werden. Die Einstellung ist nur bei
                                          Scheiben mit unterschiedlichen Lagermaßen sinnvoll.
                                          •   Nur dieser Artikel:
                                              Bei der Berechnung wird nur der angezeigte Artikel in der gewählten Ab-
                                              messung berücksichtigt. Die EK-Historie des aktuellen Artikels wird ange-
                                              zeigt.
                                          •   Alle Abmessungen:
                                              Bei der Berechnung werden alle Abmessungen des angezeigten Glases
                                              berücksichtigt. Die EK-Historie aller Abmessungen des Artikels wird ange-
                                              zeigt.
                                          Der Durchschnitts-EK wird für jeden Wareneingang errechnet, unabhängig
                                          davon, wie er gebucht wurde. Warenabgänge reduzieren lediglich den Be-
                                          stand. Die Liste wird durch die Archivierung und durch die Rechnungskontrolle
                                          reduziert.
                                          Der erste Datensatz zeigt den Anfangsbestand und den ursprünglichen Preis.
                                          Darunter werden Zu- und Abgänge (negatives Vorzeichen) aufgeführt. Beim
                                          Zugang durch eine Lagerbestellung sind außerdem die Bestellnummer und
                                          die Bestellposition angezeigt.
                                          Der Durchschnitts-EK wird bei der Erfassung oder Änderungen von Bestellun-
                                          gen aktualisiert. Er wird unter Berücksichtigung der gesamten Menge ermit-
                                          telt.

                                              Beispiel:

                                              100 Stück      auf Lager             à 15,00 €               1500,00 €

                                               40 Stück      neue Einbuchung       à 18,00 €       +        720,00 €

                                                                                                   =      2200,00 €
                                                                                                          ========
                                              2200,00/140 Stück = 15,86 €



                                          In die Berechnung fließen auch automatische Zuschläge ein, die in Bestellun-
                                          gen aufgeführt sind, z. B. Energie- oder Transportzuschlag.
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-191
                 Lagerverwaltung                                                               Softwarereferenz




                                   Übersicht Die jeweiligen Durchschnittspreise werden als Historie darge-
                                   stellt. Auf diese Weise können Sie die Preisentwicklung leicht nachverfolgen.
                                   Angezeigt werden:
                                   •   Datum:
                                       Datum der letzten Aktualisierung.
                                   •   Menge [ME]:
                                       Ab- oder zugebuchte Menge und Mengeneinheit.
                                   •   Preis/[PE]:
                                       EK-Preis pro Preiseinheit zum Zeitpunkt der Buchung.
                                   •   Bestand [ME]:
                                       Bestand zum anzeigten Datum. Wenn der Durchschnitts-EK für alle Ab-
                                       messungen angezeigt wird, wird der Bestand immer in qm angezeigt.
                                   •   Geschnittener Preis / [PE]:
                                       Durchschnittspreis pro Preiseinheit zum Zeitpunkt der Buchung.
                                   •   Bestellung / Pos.:
                                       Nummer der Bestellung und der Bestellposition.
                                   •   Lagerwert:
                                       Lagerwert zum angezeigten Datum (Berechnung: EK-Preis * Bestand).
                                   •   Typ:
                                       Art von Buchung, die den jeweiligen Eintrag verursacht hat.

                                   Einbeziehen in Gesamt-EK Sie können festlegen, ob der Artikel in die Be-
                                   rechnung des gesamten Durchschnittspreises aller Ausprägungen dieses Ar-
                                   tikels einbezogen werden soll.
                                   ☐ Der Artikel wird bei der Berechnung des Durchschnittspreises nicht berück-
                                   sichtigt.
                                   ☑ Der Artikel wird in die Berechnung mit einbezogen.

                                   Geschnittener Preis Aktueller Durchschnittspreis. Je nach der Option zur
                                   Berechnung des Durchschnitts-EKs gilt die Anzeige für den aktuellen Artikel
                                   oder für alle Abmessungen des Artikels.

                                       Aktualisierung der Anzeige
                                       Die Anzeige der Durchschnittspreise wird bei der Archivierung und bei der
                                       Rechnungskontrolle für den jeweiligen Lagerartikel aktualisiert. Damit
                                       bleibt die Anzeige übersichtlicher.
                                       A+W Business geht davon aus, dass nach diesen Vorgängen die Preise
                                       nicht mehr geändert werden. Wenn Sie die Preise dennoch nach einem der
                                       Vorgänge ändern, fließen diese Änderungen nicht in die Berechnung des
                                       Durchschnittspreises ein.
5.20 / 04-2020




                 G-192                                                                A+W Business Fertigung
                 Softwarereferenz                                                                    Lagerverwaltung




                                          Lagerverwaltung – Zusatz
                                          Lagerwirtschaft > Lagerverwaltung > Register Zusatz




                 Abb. G-98   Lagerverwaltung – Tabelle


                                          In diesem Register werden Reservierungen zu dem markierten Lagerartikel
                                          angezeigt.
                                          Die Felder in den Übersichten sind ausführlich zum Register Lagerartikel be-
                                          schrieben.
                                           “Lagerverwaltung – Lagerartikel” auf Seite G-186

                                          Reservierung
                                          Die Felder in diesem Bereich sind kundenspezifisch freigeschaltet.

                                          Kunde Nummer und Name des Kunden, für den der markierte Lagerartikel
                                          reserviert ist.

                                          Voll gesperrt Zur Zeit nicht genutzt.

                                          Exklusive Reservierungen Zur Zeit nicht genutzt.

                                          Lieferant
5.20 / 04-2020




                                          Lieferant Nummer und Name des Lieferanten, bei dem der Lagerartikel be-
                                          stellt wird.




                 A+W Business Fertigung                                                                        G-193
                 Lagerverwaltung                                                               Softwarereferenz




                                   Bemerkung

                                   Produktbezogen, Lagerortbezogen Sie können zu jedem Lagerartikel und
                                   zu jedem Lagerort weitere Angaben eintragen, z. B. wann und von welchem
                                   Lieferanten die Gläser/Kisten geliefert wurden, um die älteren Lieferungen zu-
                                   erst zu verwerten.
5.20 / 04-2020




                 G-194                                                                 A+W Business Fertigung
                 Softwarereferenz                                                                    Lagerbewegung




                                          Lagerbewegung
                                          Lagerwirtschaft > Lagerbewegung
                                          Sie können Ab- und Zugänge von Lagerartikeln manuell buchen, Bestands-
                                          zahlen korrigieren, Lagerorte umbuchen und Kisten auflösen.
                                          In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                          •   “Menü Optionen” auf Seite G-195
                                          •   “Lagerbewegung” auf Seite G-195


                                          Menü Optionen
                                          Lagerwirtschaft > Lagerbewegung
                                          Folgende Einträge werden angezeigt:
                                          •   Protokoll beim Beenden:
                                              Beim Beenden des Dialogs wird automatisch die Lagerhistorie angezeigt.
                                               “Lagerhistorie” auf Seite G-204
                                          •   Bestand > 0:
                                              Nur Lagerartikel mit einem Bestand größer 0 werden angezeigt.


                                          Lagerbewegung
                                          Lagerwirtschaft > Lagerbewegung
                                          Zu- und Abgänge der Lagerartikel werden automatisch gebucht: bei Waren-
                                          eingängen durch Lieferung, bei Warenabgängen durch Aufträge. Im Dialog
                                          Lagerbewegung können Sie Zu- oder Abgänge manuell buchen, z. B. um Be-
                                          standsmengen zu korrigieren.
                                          Im Dialog Lagerbewegung finden Sie folgende Register:
                                          •   Lagerbewegung – Abgang, Zugang
                                          •   Lagerbewegung – Umbuchung
                                          •   Lagerbewegung – Blattanzahl
                                          •   Lagerbewegung – Aufbruch
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-195
                 Lagerbewegung                                                            Softwarereferenz




                                 Lagerbewegung – Abgang, Zugang
                                 Lagerwirtschaft > Lagerbewegung > Register Abgang, Register Zugang




                                 Abb. G-99    Lagerbewegung – Abgang, Zugang


                                 In den Registern Abgang und Zugang können Sie manuell Ab- und Zugänge
                                 buchen. Sie können einen bestimmten Lagerartikel auswählen und die ent-
                                 sprechenden Daten eingeben. Wenn Sie sich alle Lagerartikel anzeigen las-
                                 sen, können Sie den gewünschten Artikel in der Liste Lagerorte markieren.
                                 Die Felder im Bereich Bestandsveränderung werden dann freigeschaltet.
                                  Tutorial, “Ab- und Zubuchung” auf Seite G-80
                                 Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird automa-
                                 tisch die Lagerhistorie mit dem Register Tabelle angezeigt, wenn Sie den
                                 Dialog schließen.
                                  “Lagerhistorie – Tabelle” auf Seite G-208

                                    Zugang von Kisten manuell erfassen
                                    Da jede Kiste mit einer eigenen ID geführt wird, können Sie Zugänge von
                                    Kisten nur über den Wareneingang oder in der Lagerverwaltung erfassen.
                                    Eine Beschreibung dazu finden Sie im Part Kistenmanagement.
5.20 / 04-2020




                 G-196                                                            A+W Business Fertigung
                 Softwarereferenz                                                                    Lagerbewegung




                                          Lagerprodukt

                                          Produkt Nummer und Bezeichnung des Lagerartikels.

                                          Ident Nr. Über die Identifikationsnummer können Sie nur Lagerabgänge ver-
                                          buchen. Zugänge von Kisten müssen Sie in der Lagerverwaltung definieren,
                                          damit Sie eine neue ID eintragen können.

                                          Inhalt Wenn Sie eine Kiste ausgewählt haben, wird deren Inhalt angezeigt.
                                          Wenn eine Kiste mit Identnummer ausgeliefert oder geöffnet werden soll, die
                                          bereits einem Auftrag zugeordnet ist, wird eine Meldung angezeigt. Dadurch
                                          wird verhindert, dass durch den anschließenden Druck des Lieferscheins oder
                                          der Rechnung ein negativer Bestand entsteht.

                                          Lagerort Lagerort, der dem Lagerartikel zugeordnet wurde.

                                              Lagerort <k.A.>
                                              Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                              <k.A.> erhalten und können bebucht werden.

                                          Durchschnitts EK Der Durchschnitts-EK wird nur angezeigt, wenn die
                                          Funktion in den Stammdaten aktiviert ist.
                                           Stammdaten, “Einkaufspreis ermitteln” auf Seite B-957

                                          Bestandsveränderung

                                          Menge Eingabe die Menge in Stück, die ab- oder zugebucht werden soll.
                                          Wenn Sie mit einer manuellen Abbuchung den Mindestbestand unterschrei-
                                          ten, wird eine Warnmeldung angezeigt.

                                          Breite / Höhe Diese Felder werden nur bei Lagermaßen mit der Mengenein-
                                          heit qm gefüllt.

                                          Bewertungspreis Eingabe des EK-Preises, zu dem der Warenzugang ge-
                                          liefert wurde.

                                          Buchungsdatum Das aktuelle Tagesdatum wird automatisch angezeigt. Es
                                          kann überschrieben werden.

                                          Bemerkung Sie können eine Bemerkung eingetragen oder aus der Kombo-
                                          box auswählen. Die Bemerkung wird in der Lagerhistorie angezeigt.
                                           “Lagerhistorie – Tabelle” auf Seite G-208
                                          Über die Schaltfläche können Sie der Liste eine neue Bemerkung hinzufügen.
                                           “Bemerkung (Lagerbewegung)” auf Seite G-201

                                          Lagerorte
                                          •   Farbe:
                                              Die Farbe wird nur bei Varianten angezeigt.
5.20 / 04-2020




                                          •   Breite, Höhe:
                                              Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder
                                              Kiste angelegt ist.


                 A+W Business Fertigung                                                                       G-197
                 Lagerbewegung                                                                  Softwarereferenz




                                 •   Inhalt:
                                     Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten
                                     die Anzahl der Blätter.
                                 •   Lagerort:
                                     Lagerort in der Reihenfolge von Ebene 1 bis 4.
                                 •   Ident Nr.:
                                     Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                 •   Bestand:
                                     Aktueller Bestand
                                 •   ME:
                                     Mengeneinheit, mit der das Produkt im Lager geführt wird.
                                 •   Lief-Ident:
                                     Kisten-ID des Lieferanten.


                                 Lagerbewegung – Umbuchung
                                 Lagerwirtschaft > Lagerbewegung > Register Umbuchung




                                 Abb. G-100   Lagerbewegung – Umbuchung


                                 In diesem Register buchen Sie Lagerartikel an einen anderen Lagerort. Beim
                                 Umbuchen eines Lagerorts wird immer der gesamte Bestand eines Lagerortes
                                 an einen anderen Lagerort umgebucht.
                                  Tutorial, “So buchen Sie einen Lagerort um” auf Seite G-85
                                 Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register
                                 Abgang beschrieben.
5.20 / 04-2020




                                  “Lagerbewegung – Abgang, Zugang” auf Seite G-196




                 G-198                                                                 A+W Business Fertigung
                 Softwarereferenz                                                                          Lagerbewegung




                                          Lagerort

                                          Lagerort Anzeige des aktuellen Lagerorts. Sie können einen anderen Lager-
                                          ort zuweisen. In der Kombobox werden alle hinterlegten Lagerorte aufgelistet.

                                             Lagerort <k.A.>
                                             Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                             <k.A.> erhalten und können bebucht werden.


                                          Lagerbewegung – Blattanzahl
                                          Lagerwirtschaft > Lagerbewegung > Register Blattanzahl




                                          Abb. G-101   Lagerbewegung – Blattanzahl


                                          In diesem Register korrigieren Sie den Inhalt von Kisten.
                                           Kistenmanagement, “Kisteninhalt korrigieren (Blattanzahl)” auf Seite K-66
                                          Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register
                                          Abgang beschrieben.
                                           “Lagerbewegung – Abgang, Zugang” auf Seite G-196

                                          Inhaltsänderung

                                          Inhalt Nur wenn Sie eine Kiste mit ID ausgewählt haben, wird die Anzahl der
                                          Blätter angezeigt, die in der Kiste vorhanden sein sollten. Diesen Wert können
                                          Sie korrigieren.
5.20 / 04-2020




                 A+W Business Fertigung                                                                                 G-199
                 Lagerbewegung                                                                 Softwarereferenz




                                 Lagerbewegung – Aufbruch
                                 Lagerwirtschaft > Lagerbewegung > Register Aufbruch




                                 Abb. G-102   Lagerbewegung – Aufbruch


                                 In diesem Register lösen Sie Kisten auf, damit die einzelnen Blätter für die
                                 Produktion zur Verfügung stehen. Bei diesem Vorgang wird die Kiste aus dem
                                 Bestand ausgebucht und die Anzahl der Blätter werden dem Bestand des La-
                                 germaßes zugebucht.
                                  Kistenmanagement, “Kisten aufbrechen (auflösen)” auf Seite K-67

                                    Kisteninhalt an einen anderen Lagerort buchen
                                    Wenn Sie eine Kiste aufbrechen, wird der Inhalt an denselben Lagerort ge-
                                    bucht, an dem die Kiste steht. Wenn Sie den Inhalt umbuchen wollen, müs-
                                    sen Sie diesen am alten Lagerort ausbuchen und anschließend am neuen
                                    Lagerort zubuchen.

                                 Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register
                                 Abgang beschrieben.
                                  “Lagerbewegung – Abgang, Zugang” auf Seite G-196

                                 Kistenaufbruch
                                 Wenn eine Kiste mit Identnummer ausgeliefert oder geöffnet werden soll, die
                                 bereits einem Auftrag zugeordnet ist, wird eine Meldung angezeigt. Dadurch
                                 wird verhindert, dass durch den anschließenden Druck des Lieferscheins oder
5.20 / 04-2020




                                 der Rechnung ein negativer Bestand entsteht.

                                 Anzahl Kisten Anzahl der Kisten, die aufgebrochen werden sollen.



                 G-200                                                                A+W Business Fertigung
                 Softwarereferenz                                                                   Lagerbewegung




                                          Abweichender Inhalt Nur wenn Sie eine Kiste ausgewählt haben, wird die
                                          Anzahl der Blätter angezeigt. Sie können diesen Wert korrigieren.


                                          Bemerkung (Lagerbewegung)
                                          Lagerwirtschaft > Lagerbewegung > [Bemerkung]




                                          Abb. G-103   Bemerkung zur Lagerbewegung


                                          In diesem Dialog hinterlegen Sie Bemerkungen, die im Dialog Lagerbewe-
                                          gung zur Auswahl angeboten werden. Wenn Sie die erste Zeile leer lassen,
                                          können Sie eine zugewiesene Bemerkung auch wieder entfernen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                     G-201
                 Abfragen                                                                                Softwarereferenz




                                          Abfragen
                                          Lagerwirtschaft > Abfragen
                                          Über die verschiedenen Abfragen können Sie sich einen schnellen Überblick
                                          über Bestände, Bewegungen und Werte in Ihren Lägern verschaffen.
                                          In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                          •     “Buchungsjournal” auf Seite G-202
                                          •     “Lagerhistorie” auf Seite G-204
                                          •     “Lagerstatistik” auf Seite G-209
                                          •     “Reservierte Lagerartikel” auf Seite G-215


                                          Buchungsjournal
                                          Lagerwirtschaft > Abfragen > Buchungsjournal




                 Abb. G-104   Buchungsjournal


                                          In diesem Dialog wählen Sie die Kriterien für die Abfrage aus. Im Buchungs-
                                          journal werden alle automatischen Auftrags- bzw. Bestellvorgänge protokol-
                                          liert, die das Lager betreffen, z. B. Reservierungen, Bestellungen, Zu- und
                                          Abgänge.
                                           Tutorial, “Buchungsjournal anzeigen” auf Seite G-90
5.20 / 04-2020




                 G-202                                                                            A+W Business Fertigung
                 Softwarereferenz                                                                                Abfragen




                                          Auswahl

                                          Buchungsart Sie können das Lager nach folgenden Buchungsarten durch-
                                          suchen:
                                          • (Keine Angabe):
                                             Wenn Sie keine Buchungsart angeben, werden alle Artikel angezeigt.
                                          • Reserviert:
                                             Nur die reservierten Artikel werden angezeigt. Ein Artikel ist so lange reser-
                                             viert, bis der Lieferschein oder die Rechnung gedruckt wurde.
                                          • Ausgeliefert:
                                             Nur die ausgelieferten Lagerartikel werden angezeigt. Ein Artikel wird als
                                             ausgeliefert gekennzeichnet, wenn der Lieferschein oder die Rechnung
                                             gedruckt wurde.
                                          • Bestellt:
                                             Nur die bestellten Lagerartikel werden angezeigt. Das Kennzeichen wird
                                             durch eine Lagerbestellung gesetzt.
                                          • Empfangen:
                                             Nur die gelieferten Lagerartikel werden angezeigt. Ein Artikel gilt dann als
                                             geliefert und empfangen, wenn er im Wareneingang verbucht wurde.

                                          Buchungszeitpunkt von … bis Sie können die Suche auf ein Datum oder
                                          einen Zeitraum einschränken, in dem die Artikel im Lager gebucht wurden.
                                          Achten Sie bei der Auswahl des Datums auf die Angabe der Uhrzeit, zu der
                                          die Buchung durchgeführt wurde.
                                          Wenn Sie die Anzeige nicht weiter eingeschränkt haben, werden alle Buchun-
                                          gen im angegebenen Zeitraum angezeigt.

                                          Lagerort Sie können die Suche auf einen Lagerort einschränken.

                                             Lagerort <k.A.>
                                             Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                             <k.A.> erhalten und können bebucht werden.

                                          Ident-Nr. Sie können die Suche auf eine Kisten-ID einschränken.

                                          Auswahl nach Mit der Wahl der Option legen Sie fest, auf was sich die Su-
                                          che beziehen soll:
                                          • Artikel:
                                             Sie können nach einem oder mehreren Artikeln suchen. Die Eingabe in
                                             den Feldern Nummer von und bis bezieht sich auf die Produktnummern.
                                             Wenn Sie keine Buchungsart gewählt haben, werden alle Buchungsarten
                                             aufgelistet.
                                          • Auftrag:
                                             Sie können nach Artikeln suchen, die in Aufträgen enthalten sind. Die Ein-
                                             gabe in den Feldern Nummer von und bis bezieht sich auf die Auftrags-
                                             nummern.

                                          Nummer von, bis Die Suche kann auf eine Nummer oder eine Folge von
5.20 / 04-2020




                                          Nummern eingeschränkt werden.




                 A+W Business Fertigung                                                                            G-203
                 Abfragen                                                               Softwarereferenz




                            Tabelle
                            In der Übersicht wird das Ergebnis der Suche angezeigt.
                            •   Buch. Typ:
                                Buchungsart, in der das Produkt gebucht wurde.
                            •   Auftr. Nr./Bestell. Nr.:
                                Nummer des Auftrags oder der Bestellung, aus denen die Buchung er-
                                zeugt wurde.
                            •   Pos.Nr.:
                                Nummer der Auftrags- oder Bestellposition.
                            •   Menge:
                                Menge der Position.
                            •   Produkt, Bezeichnung:
                                Nummer und Bezeichnung aus den Stammdaten.
                            •   Farbe:
                                Nur bei Varianten wird eine Farbe angezeigt.
                            •   Breite, Höhe:
                                Maße der Position.
                            •   Ident-Nr.:
                                Kisten-ID (manuelle Buchung oder aus dem Wareneingang). Wenn der
                                Eintrag keine Kiste darstellt, wird eine Null angezeigt.
                            •   Lief.-Ident:
                                Kisten-ID des Lieferanten.
                            •   Lagerort:
                                Ort, bei dem das Produkt ab- oder zugebucht wurde.
                            •   Buch. Datum:
                                Datum des Wareneingangs.
                            •   EK:
                                Einkaufspreis der Position. Jede Änderung des EK im Wareneingang, bei
                                der Kontrolle der Lieferanten-AB oder der Rechnung wird in die Bestellung
                                zurückgeschrieben.


                            Lagerhistorie
                            Lagerwirtschaft > Abfragen > Lagerhistorie
                            In der Lagerhistorie werden alle Vorgänge protokolliert, die das Lager betref-
                            fen. Das sind neben den Buchungsarten z. B. auch die verschnittenen Lager-
                            platten, Korrekturen, neue Artikel.
                            Im Dialog Lagerhistorie finden Sie folgende Register:
                            •   Lagerhistorie – Auswahl
                            •   Lagerhistorie – Tabelle
5.20 / 04-2020




                 G-204                                                          A+W Business Fertigung
                 Softwarereferenz                                                                                  Abfragen




                                           Lagerhistorie – Auswahl
                                           Lagerwirtschaft > Abfragen > Lagerhistorie > Register Auswahl




                 Abb. G-105   Lagerhistorie – Auswahl


                                           In diesem Register wählen Sie die Kriterien für die Abfrage aus. Das Ergebnis
                                           wird automatisch im Register Tabelle angezeigt.
                                            Tutorial, “Buchungsjournal anzeigen” auf Seite G-90

                                           Buchungsart
                                           Sie können das Lager nach folgenden Buchungsarten durchsuchen:
                                           •   (Keine Angabe):
                                               Wenn Sie keine Buchungsart angeben, werden alle Artikel angezeigt.
                                           •   Reserviert:
                                               Nur die reservierten Artikel werden angezeigt. Ein Artikel ist so lange reser-
                                               viert, bis der Lieferschein oder die Rechnung gedruckt wurde.
                                           •   Ausgeliefert:
                                               Nur die ausgelieferten Lagerartikel werden angezeigt. Ein Artikel wird als
                                               ausgeliefert gekennzeichnet, wenn der Lieferschein oder die Rechnung
                                               gedruckt wurde.
                                           •   Verschnittenes LM:
                                               Diese Buchungsart wird von der A+W Optimizer-Rückmeldung verwendet,
                                               wenn eine Position aus einem Lagermaß zugeschnitten wurde. Die Anzahl
5.20 / 04-2020




                                               der Lagerplatten wird ausgewertet.




                 A+W Business Fertigung                                                                              G-205
                 Abfragen                                                                 Softwarereferenz




                            •   Bestellt:
                                Nur die bestellten Lagerartikel werden angezeigt. Das Kennzeichen wird
                                durch eine Lagerbestellung gesetzt.
                            •   Empfangen:
                                Nur die gelieferten Lagerartikel werden angezeigt. Ein Artikel gilt dann als
                                geliefert und empfangen, wenn er im Wareneingang verbucht wurde.
                            •   Lagereingang/Lagerausgang manuell:
                                Nur manuell gebuchte Lagerzu- oder Lagerabgänge werden angezeigt.
                            •   Lagerumbuchung:
                                Nur Lagerumbuchungen werden angezeigt.
                            •   Neuanlage:
                                Nur die Artikel werden angezeigt, die neu ins Lager aufgenommen wurden.
                                Die Daten können im Rahmen einer Inventur oder manuell angelegt wor-
                                den sein. Berücksichtigt werden alle neuen Artikel ab der letzten Archivie-
                                rung.
                            •   Korrektur:
                                Nur die Artikel werden angezeigt, deren Bestände bei der Inventur bearbei-
                                tet wurden. Berücksichtigt werden alle Korrekturen ab der letzten Archivie-
                                rung.
                            •   Umbuchung auf Papierkorb, Rückbuchung vom Papierkorb, Aus Lager ge-
                                löscht:
                                Interne Buchungsarten.

                            Programm
                            Sie können die Suche auf Artikel einschränken, die in einem bestimmten Dia-
                            log der Lagerwirtschaft bearbeitet wurden, z. B. Lagerumbuchungen.

                            Bemerkungstext
                            Sie können die Suche auf die Artikel einschränken, zu denen eine bestimmte
                            Bemerkung hinterlegt ist. Die Bemerkung wird unter dem Eingabefeld ange-
                            zeigt.

                            Artikel/Auftragsnummer
                            Mit der Wahl der Option schränken Sie die Suche auf bestimmte Artikel oder
                            Aufträge ein:
                            •   Nach Artikel von … bis:
                                Sie können einen oder mehrere Artikel auswählen.
                            •   Nach Dokumentennummer von … bis:
                                Sie können einen oder mehrere Aufträge oder Bestellungen auswählen.

                                Tagesaktivitäten anzeigen
                                Wenn Sie in beiden Feldern dieselbe Artikel- bzw. Auftragsnummer eintra-
                                gen, werden alle Aktivitäten angezeigt, die in einem bestimmten Zeitraum
                                zu einem Artikel oder Auftrag gebucht wurden. Geben Sie dazu auch den
                                Buchungszeitpunkt mit der Uhrzeit an.
5.20 / 04-2020




                 G-206                                                           A+W Business Fertigung
                 Softwarereferenz                                                                                Abfragen




                                          Lager-ID/Serial-Nr.

                                          Lager-ID von … bis Sie können eine oder mehrere Lager-IDs auswählen.

                                          Ident-Nr. / Lief.-Ident von … bis Sie können eine oder mehrere IDs aus-
                                          wählen. Die Ident-Nr. bezieht sich auf die Kiste, die Lief.-Ident auf die Kisten-
                                          ID des Lieferanten.

                                          Lagerorte
                                          Sie können die Suche auf Lagerartikel einschränken, die von einem bestimm-
                                          ten Lagerort an einen anderen Lagerort umgebucht wurden.

                                          Von Lagerort Nur die Artikel werden angezeigt, die vom gewählten Lagerort
                                          abgebucht und einem ausgewählten Lagerort zugebucht wurden.

                                          Nach Lagerort Nur die Artikel werden angezeigt, die am gewählten Lagerort
                                          zugebucht und von einem ausgewählten Lagerort abgebucht wurden.

                                          Mitarbeiter/Buchungsdatum

                                          Mitarbeiter Sie können die Suche auf Artikel einschränken, die vom gewähl-
                                          ten Mitarbeiter bearbeitet wurden.

                                          Buchungszeitpunkt von … bis Sie können die Suche auf einen Buchungs-
                                          zeitraum einschränken. Achten Sie bei der Eingabe darauf, dass die Uhrzeit
                                          mit angegeben werden muss.
5.20 / 04-2020




                 A+W Business Fertigung                                                                            G-207
                 Abfragen                                                                              Softwarereferenz




                                            Lagerhistorie – Tabelle
                                            Lagerwirtschaft > Abfragen > Lagerhistorie > Register Tabelle




                 Abb. G-106   Lagerhistorie – Tabelle


                                            In diesem Register wird das Ergebnis der Abfrage angezeigt.

                                            Tabelle
                                            •   Buch. Typ:
                                                Buchungsart, in der das Produkt gebucht wurde.
                                            •   Auftr./Bestell., Pos.:
                                                Nummer des Auftrags/der Bestellung und der Position, aus denen die Bu-
                                                chung erzeugt wurde.
                                            •   Menge:
                                                Menge der Position.
                                            •   Ident, Lief.-Ident:
                                                Kisten-ID (manuelle Buchung oder aus dem Wareneingang) und Kisten-ID
                                                des Lieferanten.
                                            •   Produkt, Bezeichnung:
                                                Nummer und Bezeichnung aus den Stammdaten.
                                            •   Farbe:
                                                Nur bei Varianten wird eine Farbe angezeigt.
                                            •   Breite, Höhe:
5.20 / 04-2020




                                                Maße der Position.
                                            •   Inhalt:
                                                Anzahl der Blätter bei Kisten.



                 G-208                                                                        A+W Business Fertigung
                 Softwarereferenz                                                                           Abfragen




                                          •   EK / PE:
                                              Einkaufspreis pro Preiseinheit.
                                          •   Gesamt EK:
                                              Einkaufspreis der Position.
                                          •   PE:
                                              Preiseinheit des Gesamt-EK.
                                          •   ME:
                                              Mengeneinheit der Position.
                                          •   Buch. Datum:
                                              Datum und Uhrzeit der Buchung.
                                          •   Ausf. Datum:
                                              Datum und Uhrzeit, zu denen der Vorgang gebucht wurde.
                                          •   Von Lagerort, Nach Lagerort:
                                              Alter und neuer Lagerort bei Umbuchungen.
                                          •   Mitarbeiter, Programm:
                                              Name des Mitarbeiters, der den Vorgang gebucht hat, und Name des
                                              Dialogs, in dem die Buchung durchgeführt wurde.
                                          •   Bemerkung:
                                              Bei bestimmten Buchungsarten wird eine Bemerkung angezeigt, z. B.
                                              welche Korrektur bei der Inventur vorgenommen wurde.


                                          Lagerstatistik
                                          Lagerwirtschaft > Abfragen > Lagerstatistik
                                          Die Lagerstatistik gibt Ihnen Aufschluss darüber, welche Ihrer Lagerartikel
                                          Renner und welche Ladenhüter sind. Die Auswertungen zeigen Anfangs- bzw.
                                          Endbestände und Zu- bzw. Abgänge Ihrer Lagerartikel pro Monat. Damit kön-
                                          nen Sie sich über die Umschlagshäufigkeit, die durchschnittliche Lagerdauer
                                          und den durchschnittlichen Lagerbestand Ihrer Produkte informieren.
                                          Im Dialog Lagerstatistik finden Sie folgende Register:
                                          •   Lagerstatistik – Produkte
                                          •   Lagerstatistik – Statistik
                                          •   Lagerstatistik – FIFO/LIFO
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-209
                 Abfragen                                                                                    Softwarereferenz




                                            Lagerstatistik – Produkte
                                            Lagerwirtschaft > Abfragen > Lagerstatistik > Register Produkte




                 Abb. G-107   Lagerstatistik – Produkte


                                            In diesem Register legen Sie die Kriterien für die statistische Auswertung fest.
                                            Wenn Sie einen Eintrag in der Trefferliste markieren, werden die zugehörigen
                                            Details im Register Statistik angezeigt.
                                             Tutorial, “So lassen Sie sich die Statistik zu Lagerbeständen anzeigen” auf
                                              Seite G-94

                                            Auswahl

                                            Jahr Auswahl des Jahres, aus dem die Daten ausgewertet werden sollen.
                                            Damit können Sie einen bestimmten Zeitraum mit demselben Zeitraum des
                                            Vorjahres vergleichen.

                                            Monat von … bis Die Auswahl der Monate bezieht sich immer auf das ein-
                                            gestellte Jahr. Wenn Sie mehr als ein Jahr auswerten möchten, müssen Sie
                                            die Auswertung splitten. Wenn Sie eine Auswertung über den Jahreswechsel
                                            hinaus benötigen, müssen Sie zwei Auswertungen nacheinander durchfüh-
                                            ren.

                                            Produkt von … bis Auswahl eines Produkts oder einer Folge von Produk-
                                            ten. Zu jeder Produktnummer werden alle zugehörigen Lagerartikel ausge-
5.20 / 04-2020




                                            wertet, z. B. zum Produkt Float 4 mm alle Lagermaße, Kisten, Lagerorte usw.




                 G-210                                                                              A+W Business Fertigung
                 Softwarereferenz                                                                             Abfragen




                                          Übersicht
                                          In der Übersicht werden alle Lagerartikel aufgelistet, die den Suchkriterien
                                          entsprechen. Wenn Sie einen Eintrag der Trefferliste markieren, werden die
                                          zugehörigen Details im Register Statistik angezeigt.
                                          •   Produkt:
                                              Produktnummer aus den Stammdaten.
                                          •   Bezeichnung:
                                              Bezeichnung aus den Stammdaten.
                                          •   Breite, Höhe:
                                              Maße für die hinterlegten Lagermaße.
                                          •   Inhalt:
                                              Anzahl der Blätter einer Kiste.
                                          •   Ident:
                                              Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
                                          •   Farbe:
                                              Nur bei Varianten, die auf Lager gehalten werden.
                                          •   Lagerort:
                                              Lagerort des Lagerartikels.

                                              Lagerort <k.A.>
                                              Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte
                                              <k.A.> erhalten und können bebucht werden.
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-211
                 Abfragen                                                                                 Softwarereferenz




                                             Lagerstatistik – Statistik
                                             Lagerwirtschaft > Abfragen > Lagerstatistik > Register Statistik




                 Abb. G-108   Lagerstatistik – Statistik


                                             In diesem Register werden Details für den Eintrag angezeigt, der in der Tref-
                                             ferliste im Register Produkte markiert ist.

                                             Lagerartikel
                                             In diesem Bereich werden die Daten des markierten Lagerartikels angezeigt.

                                             Produkt Produktnummer und Bezeichnung aus den Stammdaten.

                                             Breite / Höhe Maße für die hinterlegten Lagermaße.

                                             Lagerort Lagerort des Lagerartikels.

                                             EK Durchschnitts-EK und Mengeneinheit.

                                             Inhalt Anzahl der Blätter einer Kiste.
5.20 / 04-2020




                 G-212                                                                           A+W Business Fertigung
                 Softwarereferenz                                                                              Abfragen




                                          Übersicht
                                          In der Übersicht werden die statistischen Werte für den Lagerartikel pro Monat
                                          angezeigt.
                                          •   Monat:
                                              Je nach Auswahl werden einzelne Monate oder das gesamte Jahr darge-
                                              stellt.
                                          •   Anf.-bestand:
                                              Als Anfangsbestand wird der Endbestand des Vormonats herangezogen.
                                          •   Zugang:
                                              Summe aller Zugänge innerhalb des Monats.
                                              Bei den Zugängen handelt es sich u. a. um neu angelegte Lagerartikel, um
                                              manuelle Zubuchungen in der Lagerbewegung und/oder Wareneingänge
                                              aus dem Einkauf.
                                          •   Abgang:
                                              Summe aller Abgänge innerhalb des Monats.
                                              Abgänge werden entweder bei Lieferschein- und/oder Rechnungsdruck
                                              automatisch gebucht oder als manuelle Lagerbewegung.
                                          •   Endbestand:
                                              Berechnung: Anfangsbestand + Zugang - Abgang (innerhalb des Monats).
                                          •   Umschlagshäufigkeit:
                                              Berechnung: Lagerabgang ÷ durchschnittlicher Lagerbestand
                                              Je höher der Wert, desto geringer ist die Verweildauer der Produkte im La-
                                              ger.
                                          •   Durchschnittliche Lagerdauer (in Tagen):
                                              Berechnung: Tage der Abrechnungsperiode ÷ Umschlagshäufigkeit
                                              Anzahl der Tage, die benötigt werden, um beim derzeitigen Abgang den
                                              aktuellen Endbestand abzubauen.
                                          •   Durchschnittlicher Lagerbestand:
                                              Berechnung: (Anfangsbestand + Endbestand) ÷ 2.
                                          •   Anfangswert/Zugangswert/Abgangswert/Endwert:
                                              Die Lagerwerte werden auf der Basis des Einkaufspreises ermittelt.
                                          •   Summe Lagerbestand:
                                              Berechnung: = (Anfangsbestand + (n * Endbestand)) / (n + 1), n = Anzahl
                                              der Monate.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-213
                 Abfragen                                                                              Softwarereferenz




                                           Lagerstatistik – FIFO/LIFO
                                           Lagerwirtschaft > Abfragen > Lagerstatistik > Register FIFO/LIFO




                 Abb. G-109   Lagerstatistik – FIFO/LIFO


                                           In diesem Register werden die im Lager geführten Artikel nach dem FIFO und/
                                           oder LIFO Verfahren bewertet angezeigt. Die gewünschte Anzeige wählen Sie
                                           im Menü Optionen > Berechnung.
                                           Die Daten werden erst angezeigt, wenn Sie im Dialog Lagerbewertung eine
                                           Berechnung der Lagerwerte gestartet haben.
                                            “Lagerbewertung” auf Seite G-227

                                           Übersicht
                                           In der Übersicht werden die statistischen Werte für den Lagerartikel pro Monat
                                           angezeigt.
                                           •   Datum:
                                               Datum der Bewertung oder der Inventur.
                                           •   Zugang:
                                               Summe aller Zugänge im ausgewählten Bewertungszeitraum.
                                           •   ME:
                                               Mengeneinheit des Lagerartikels.
                                           •   Preis, PE:
5.20 / 04-2020




                                               Preis und Preiseinheit
                                           •   Restmenge FIFO:
                                               Verbleibende Menge nach der Berechnung.



                 G-214                                                                         A+W Business Fertigung
                 Softwarereferenz                                                                                      Abfragen




                                          •   Preis FIFO:
                                              Preis der verbleibenden Menge nach der FIFO-Berechnung.
                                          •   Restmenge LIFO:
                                              Verbleibende Menge nach der Berechnung.
                                          •   Preis LIFO:
                                              Preis der verbleibenden Menge nach der LIFO-Berechnung.
                                          Ein Berechnungsbeispiel finden Sie im Abschnitt Lagerbewertung:
                                           “Lagerbewertung” auf Seite G-226



                                          Reservierte Lagerartikel
                                          Lagerwirtschaft > Abfragen > Reservierte Lagerartikel




                                          Abb. G-110    Reservierte Lagerartikel


                                          Über diesen Dialog können Sie sich die Aufträge eines Nummernverwalters
                                          anzeigen lassen, um zu prüfen, welche Lagerartikel reserviert sind. Die reser-
                                          vierten Artikel werden im Ausdruck aufgeführt.
                                           Tutorial, “Lagerführungsmodus und Reservierung” auf Seite G-30
                                           Tutorial, “So drucken Sie sich die Liste der reservierten Lagerartikel” auf Seite G-92

                                          Auswahl

                                          Mitarbeiter Name des angemeldeten Mitarbeiters.
5.20 / 04-2020




                                          Nummernverwalter Auswahl des Nummernverwalters, dessen Aufträge
                                          ausgewertet werden sollen.



                 A+W Business Fertigung                                                                                   G-215
                 Abfragen                                                                  Softwarereferenz




                            Tabelle
                            •   Nummer:
                                Auftragsnummer.
                            •   Nummer Kunde/Lief.:
                                Kundennummer.
                            •   Kunde/Lieferant:
                                Name des Kunden oder Lieferanten.
                            •   Status:
                                Status des Auftrags.
                            •   Datum Erfassung:
                                Datum, an dem der Auftrag erfasst wurde.
                            •   Datum Lieferung:
                                Datum, zu dem der Auftrag geliefert werden soll.
                            •   Datum AB:
                                Datum der Auftragsbestätigung durch den Lieferanten.
                            •   Sperr-KZ:
                                Sperrkennzeichen aus dem Auftrag.

                            Gedruckte Liste




                            Abb. G-111   Reservierte Lagerartikel – Ausgabe auf dem Bildschirm


                            Die reservierten Lagerartikel werden pro Artikelnummer und Lagerort aufge-
                            listet. Bei mehreren Lagerorten wird die Gesamtsumme angezeigt.
5.20 / 04-2020




                 G-216                                                            A+W Business Fertigung
                 Softwarereferenz                                                                             Suche




                                          Suche
                                          Lagerwirtschaft > Suche
                                          Sie können den Lagerbestand nach einzelnen Lagerartikeln oder nach Waren-
                                          gruppen abfragen.

                                              Filter setzen
                                              Wenn keine Filter gesetzt sind, werden keine Daten angezeigt.

                                          Der Dialog ist ausführlich im Part Verkauf beschrieben.
                                           Verkauf, “Lagerinfo” auf Seite C-741
                                          Im Dialog Lagersuche finden Sie folgende Register:
                                          •   Lagersuche – Lagersuche
                                          •   Lagersuche – Zukünftiger Lagerbestand


                                          Lagersuche – Lagersuche
                                          Lagerwirtschaft > Suche > Register Lagersuche




                 Abb. G-112   Lagersuche – Lagersuche
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-217
                 Suche                                                                                     Softwarereferenz




                                           In diesem Register können Sie sich die aktuellen Bestände, die reservierten
                                           Mengen und die zukünftigen Bestände zu Lagerartikeln anzeigen lassen.
                                            Tutorial, “Lagerführungsmodus und Reservierung” auf Seite G-30
                                            Tutorial, “Bestände in der Lagersuche anzeigen” auf Seite G-102


                                           Lagersuche – Zukünftiger Lagerbestand
                                           Lagerwirtschaft > Suche > Register Zukünftiger Lagerbestand




                 Abb. G-113   Lagersuche – Zukünftiger Lagerbestand


                                           In diesem Register können Sie prüfen, ob die Wiederbeschaffungszeiten für
                                           ein bestimmtes Produkt ausreichen, um einen Auftrag termingerecht auslie-
                                           fern zu können. Die Farbe Rot zeigt an, dass die Termine nicht eingehalten
                                           werden können. Gelb zeigt an, dass die Wiederbeschaffungszeit ausreicht,
                                           sofern die Bestellungen termingerecht eintreffen.
                                            Tutorial, “Lagerinfo und zukünftiger Lagerbestand” auf Seite G-99
                                           Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferan-
                                           tenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferan-
                                           ten, die in der Tourenverwaltung hinterlegt sind.
5.20 / 04-2020




                 G-218                                                                            A+W Business Fertigung
                 Softwarereferenz                                                                             Suche




                                          Um die Performance zu erhöhen, können Sie die Anzeige der Vorschau durch
                                          folgende Einstellungen einschränken:
                                          •   Im Dialog Produktverwaltung > Register Lager/Einkauf > Checkbox keine
                                              Verfügbarkeitsprüfung können Sie bestimmte Artikel aus der Lagervor-
                                              schau und der Verfügbarkeitsprüfung herausnehmen, indem Sie die Ver-
                                              fügbarkeitsprüfung für diese Artikel ausschalten.
                                          •   Im Dialog Firmendaten können Sie einstellen, über welchen Zeitraum die
                                              Vorschau dargestellt werden soll.
                                               Tutorial, “Einstellung prüfen” auf Seite G-64
                                          •   Im Dialog Lagerverwaltung können Sie mehrere Lagermaße miteinander
                                              verknüpfen, damit die Bestandsprüfung nur für den definierten Lager-
                                              Hauptartikel durchgeführt wird.
                                               “Hauptartikel” auf Seite G-187
5.20 / 04-2020




                 A+W Business Fertigung                                                                      G-219
                 Lagerbestellung                                                                 Softwarereferenz




                                   Lagerbestellung
                                   Lagerwirtschaft > Lagerbestellung
                                   In diesem Dialog können Sie alle vorgeschlagenen Lagerbestellungen prüfen
                                   und an den Einkauf übergeben.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menüs im Bestellpool” auf Seite G-220
                                   •   “Lagerbestellung” auf Seite G-223


                                   Menüs im Bestellpool
                                   Über die Menüs können Sie automatisch die Datumsfelder aktualisieren las-
                                   sen und zusätzlich andere Dialoge öffnen.
                                   In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                   •   “Menü Funktionen” auf Seite G-220
                                   •   “Menü Optionen” auf Seite G-221


                                   Menü Funktionen
                                   Lagerwirtschaft > Lagerbestellung > Menü Funktionen
                                   Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellüber-
                                   gabe zu schließen. Folgende Einträge werden angezeigt:
                                   •   Lieferant/Liefertermine ändern:
                                       Öffnet den Dialog Lieferant und Liefertermine ändern.
                                        “Lieferant und Liefertermin ändern” auf Seite C-662
                                   •   Markierungsoptionen:
                                       Öffnet den Dialog Markierungsoptionen.
                                        “Markierungsoptionen” auf Seite C-663
                                   •   Lieferantenpreise:
                                       Öffnet den Dialog Preisvergleich.
                                        “Preisvergleich” auf Seite C-664
5.20 / 04-2020




                 G-220                                                                    A+W Business Fertigung
                 Softwarereferenz                                                                      Lagerbestellung




                                          Menü Optionen
                                          Lagerwirtschaft > Lagerbestellung > Menü Optionen
                                          Über dieses Menü können Sie die Standardeinstellung des Dialoges bestim-
                                          men. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung
                                          wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

                                              Aktivierte Optionen nach dem Öffnen des Dialogs
                                              Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen
                                              des Dialogs wirksam werden.
                                              Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich
                                              das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt
                                              von der Leistungsfähigkeit des Rechners ab.
                                              Die folgenden Beschreibungen stellen die aktivierte Option dar.

                                          Gruppe Übergabe
                                          •   Auftragsbezogene Übergabe:
                                              Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht
                                              aktiviert ist, können Sammelbestellungen erzeugt werden.
                                          •   Bestellnummer = Auftragsnummer:
                                              Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene
                                              Übergabe aktiviert ist.
                                          •   Bestellpool pro Mitarbeiter:
                                              Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

                                          Gruppe Liefertermin
                                          •   Lieferterminprüfung:
                                              Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin,
                                              der nicht an einem Tourentag liegt, wird eine entsprechende Meldung an-
                                              gezeigt.
                                          •   Lieferantentour berücksichtigen:
                                              Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tou-
                                              rentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen
                                              die Lieferantentouren in den Stammdaten hinterlegt werden.
                                               Stammdaten, “Touren” auf Seite B-862
                                          •   Vorlauftage mit Kombiwarengruppe ermitteln:
                                              Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese
                                              zur Berechnung des Liefertermins herangezogen werden.
                                               Stammdaten, “Vorlauftage” auf Seite B-568
5.20 / 04-2020




                 A+W Business Fertigung                                                                         G-221
                 Lagerbestellung                                                               Softwarereferenz




                                   Gruppe Produktbezeichnung
                                   •   Produktbezeichnungen aus Lieferantenkartei:
                                       Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei
                                       übernommen.
                                   •   Produktbezeichnungen aus Basisdaten (interne Best.):
                                       Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus
                                       den Produktstammdaten übernommen.

                                   Gruppe Sonstige
                                   •   Keine Kostenrückschreibung:
                                       Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
                                   •   Maßzuschläge berücksichtigen:
                                       Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.
                                   •   Druckkennzeichen für Bearbeitungen immer setzen:
                                       In der Bestellung sollen Bearbeitungen immer gedruckt werden. Wenn die
                                       Option deaktiviert ist, werden die Druckkennzeichen unverändert aus dem
                                       Auftrag in die Bestellung übernommen.
                                   •   Statistikwarengruppe aus dem Auftrag:
                                       Die Angabe zur Statistikwarengruppe wird aus dem Auftrag übernommen,
                                       wenn für Auftrag und Bestellung unterschiedliche Statistikwarengruppen
                                       definiert sind.
                                   •   Geschäftsart aus dem Auftrag:
                                       Die Geschäftsart wird aus dem Auftrag übernommen, wenn für Auftrag und
                                       Bestellung unterschiedliche Geschäftsarten definiert sind.
                                   •   AV-Bereich aus dem Auftrag:
                                       Der AV-Bereich wird aus dem Auftrag übernommen, wenn für Auftrag und
                                       Bestellung unterschiedliche AV-Bereiche definiert sind.
                                   •   Fachberater = Erfasser bei Neuanlage:
                                       In der Bestellung wird automatisch der Name des Mitarbeiters eingetragen,
                                       der sich in A+W Business angemeldet hat.
                                   •   Statusänderung erfragen:
                                       Die Abfrage zur Änderung des Status wird angezeigt.
                                   •   Wiederholte Übergabe nur bis Sperrstatus:
                                       Bestellungen können mehrfach übergeben werden, allerdings nur, bis der
                                       Sperrstatus erreicht ist.

                                   Gruppe Erweitert
                                   •   Einstellungen:
                                       Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von
                                       Texten und Dateianhängen festzulegen.
5.20 / 04-2020




                 G-222                                                                A+W Business Fertigung
                 Softwarereferenz                                                                            Lagerbestellung




                                           Lagerbestellung
                                           Lagerwirtschaft > Lagerbestellung




                 Abb. G-114   Lagerbestellung


                                           In diesem Dialog können Sie alle vorgeschlagenen Bestellungen für Artikel se-
                                           hen, deren Mindestbestand unterschritten wurde. Die Bestellmenge wird nach
                                           der Menge berechnet, die im Dialog Lagerverwaltung festgelegt ist.
                                           Mit der Übergabe werden die Bestellungen angelegt und können gedruckt und
                                           versendet werden.
                                            Tutorial, “Lagerbestellung (automatisch)” auf Seite G-107
                                            Tutorial, “Bestellmenge nach Bestandsprüfung” auf Seite G-135

                                           Lagerort

                                           Warenhaus, Gang, Regal, Fach Sie können die Anzeige auf einzelne La-
                                           gerorte einschränken. Bedenken Sie dabei, dass auch auf den Lagerort
                                           <k.A.> Lagerartikel gebucht sein können. Wenn Sie die Auswahl nicht ein-
                                           schränken, werden Bestellvorschläge zu allen Artikeln angezeigt, deren Min-
                                           destbestand unterschritten ist.
5.20 / 04-2020




                                           Die Bezeichnung der Lagerorte kann in den Stammdaten geändert werden.
                                            Tutorial, “Lagerebenen festlegen” auf Seite G-22




                 A+W Business Fertigung                                                                              G-223
                 Lagerbestellung                                                                    Softwarereferenz




                                   Übersicht
                                   In der Übersicht werden die Daten zu den Bestellvorschlägen angezeigt. Sie
                                   können einen anderen Lieferanten auswählen und sich einen Preisvergleich
                                   anzeigen lassen.
                                   •   Lieferant:
                                       Der Lieferant wird aus der Lieferantenkartei übernommen. Wenn kein Lie-
                                       ferant eingetragen ist oder wenn Ihnen Lieferschwierigkeiten Ihres Stan-
                                       dard-Lieferanten bekannt sind, können Sie den Namen ändern.
                                   •   Artikel/Farbe:
                                       Nummer und ggf. Variante des Produkts, das bestellt werden soll.
                                   •   Ident-Nr.:
                                       Kisten-ID (manuelle Buchung oder aus dem Wareneingang)
                                   •   Lagerort:
                                       Lagerort, an dem der Bestand des Lagerartikels unterschritten ist.
                                   •   Menge:
                                       Menge, die bestellt werden soll. Die Standard-Bestellmenge wird so oft
                                       multipliziert, bis der Mindestbestand überschritten ist. Sie können den Wert
                                       direkt in der Übersicht überschreiben.
                                   •   Breite, Höhe:
                                       Maße der Scheibe, die bestellt werden soll.
                                   •   Inhalt:
                                       Der Inhalt wird nur bei Kisten angezeigt.
                                   •   Anlief.-Lief.:
                                       Der Liefertermin des Lieferanten wird aus den Angaben in der Lieferanten-
                                       kartei errechnet. Wenn Ihnen Lieferschwierigkeiten Ihres Standard-Liefe-
                                       ranten bekannt sind, können Sie den Termin ändern.
                                    Verkauf, “Lieferant und Liefertermin ändern” auf Seite C-662
                                    Verkauf, “Preisvergleich” auf Seite C-664

                                   Position für Die Bestellvorschläge sind in unterschiedlichen Farben darge-
                                   stellt:
                                   • Rot: interner Auftrag:
                                      Interne Aufträge sind Produktionsaufträge, die erzeugt werden, um den La-
                                      gerbestand aufzufüllen. Der Vorschlag wird automatisch erzeugt, wenn in
                                      der Lieferantenkartei für das Produkt die entsprechende Option aktiviert ist.
                                   • Blau: Anfrage:
                                      Bestellanfragen an einen Lieferanten, um z. B. Preise und Liefertermine zu
                                      erfragen.
                                   • Grün: Liefertermin für Auftr./Best. gefährdet:
                                      Als Liefertermin wird automatisch das aktuelle Tagesdatum eingesetzt. Da-
                                      mit ist die Lieferung i. d. R. nicht termingerecht möglich. Wenn Sie das Da-
                                      tum ändern, wechselt die Schriftfarbe für den Eintrag zu Schwarz.
5.20 / 04-2020




                 G-224                                                                    A+W Business Fertigung
                 Softwarereferenz                                                                  Lagerbestellung




                                          Ziel-Nummernverwalter

                                          Mitarbeiter Name des Mitarbeiters, der sich in A+W Business angemeldet
                                          hat oder der den Nummernverwalter eingerichtet hat. Wenn Sie einen neuen
                                          Nummernverwalter anlegen, können Sie diesen einem bestimmten Mitarbeiter
                                          zuweisen.

                                          Name Name des Nummernverwalters, in den die Bestellungen übergeben
                                          werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Num-
                                          mernverwalter angelegt.

                                          Ziel-Nummernkreis

                                          Mandant Wenn Sie für Ihre Mandanten gesonderte Nummernkreise einge-
                                          richtet haben, können Sie den gewünschten Mandanten auswählen.

                                          AV-Bereich Wenn Sie mit AV-Bereichen arbeiten, können Sie die Bestellung
                                          einem bestimmten AV-Bereich zuordnen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                    G-225
                 Lagerbewertung                                                                        Softwarereferenz




                                  Lagerbewertung
                                  Bei der Lagerbewertung werden die Lagerbestände nach dem periodischen
                                  Verfahren bewertet. Dazu werden die Lagerabgänge der gesamten Periode
                                  zunächst summiert. Anschließend werden die Lagerabgänge von den Waren-
                                  eingängen abgezogen. Dieser Vorgang hängt vom gewählten Verfahren ab:
                                  •       LIFO: Die zuletzt eingegangenen Artikel werden zuerst abgezogen.
                                  •       FIFO: Die zuerst eingegangenen Artikel werden zuerst abgezogen.
                                          Der Lagerwert wird jeweils aus der nicht verbrauchten Menge berechnet.
                                          Dabei wird der Zeitraum von der letzten Lagerbewertung bis zum Auswer-
                                          tungszeitpunkt berücksichtigt.

                                  Beispiel

                                      Lager        Artikel      Datum       Wert in €    Menge           Wert
                                                                                         (Nach LIFO)

                                      1            111          1.5.2016    8,50         15 (15)         15*8,50

                                      1            111          4.5.2016    8,70         20 (10)         15*8,50
                                                                                                         +20*8,70

                                      1            111          5.5.2016    8,20         10 (0)          15*8,50
                                                                                                         +20*8,70
                                                                                                         +10*8,20

                                                                    Der LIFO Wert beträgt (15*8,50+10*8,70) / 25 = 8,58

                                      Lager        Artikel      Datum       Wert in €    Menge           Wert
                                                                                         (Nach FIFO)

                                      1            111          1.5.2016    8,50         15 (15)         15*8,50

                                      1            111          4.5.2016    8,70         20 (10)         15*8,50
                                                                                                         +20*8,70

                                      1            111          5.5.2016    8,20         10 (0)          15*8,50
                                                                                                         +20*8,70
                                                                                                         +10*8,20

                                                                    Der FIFO Wert beträgt (15*8,70+10*8,20) / 25 = 8,50

                                  Tab. G-1          Berechnungsbeispiele

                                          Lagerartikel mit ID
                                          Lagerartikel mit Identnummern können nicht nach FIFO/LIFO bewertet
                                          werden, da diese eindeutig identifizierbar sind. Von diesen Lagerartikeln ist
                                          entweder 1 oder kein Stück vorhanden. Daher gibt es keine Entnahmerei-
                                          henfolge.

                                  Bei der Erstbewertung darf der Lagerbestand nicht negativ sein. Die Erstbe-
5.20 / 04-2020




                                  wertung kann nur nach durchschnittlichem EK oder manuellem Wert erfolgen.
                                  Ab dem Zeitpunkt der Erstbewertung kann dann mit dem FIFO oder LIFO Ver-
                                  fahren gerechnet werden.



                 G-226                                                                      A+W Business Fertigung
                 Softwarereferenz                                                                   Lagerbewertung




                                          Lagerbewertung
                                          Lagerwirtschaft > Lagerbewertung > Selektion
                                          In diesem Dialog starten Sie die Berechnung des Lagerwerts.
                                          Im Dialog Lagerbewertung finden Sie folgende Register:
                                          •   Lagerbewertung – Selektion
                                          •   Lagerbewertung – Bewertung


                                          Menü Optionen
                                          Lagerwirtschaft > Lagerbewertung
                                          Folgende Einträge werden angezeigt:
                                          •   Erstbewertung nach:
                                              Für die Erstbewertung des Lagerbestands können Sie eines der folgenden
                                              Verfahren auswählen:
                                              – FIFO, LIFO
                                              – Durch. EK
                                              – Manuell
5.20 / 04-2020




                 A+W Business Fertigung                                                                      G-227
                 Lagerbewertung                                                                        Softwarereferenz




                                           Lagerbewertung – Selektion
                                           Lagerwirtschaft > Lagerbewertung > Selektion




                 Abb. G-115   Lagerbewertung – Selektion


                                           In diesem Register stellen Sie die Kriterien ein, nach denen der Lagerwert be-
                                           rechnet werden soll. Zusätzlich können Sie in den Firmendaten festlegen, wie
                                           der EK berechnet werden soll.
                                            “Inventurliste” auf Seite G-167

                                           Auswahl

                                           Nicht bewertet seit Angabe des letzten Bewertungsdatums. Sie können ein
                                           beliebiges Datum in der Vergangenheit wählen. Damit werden nur die Produk-
                                           te bewertet, deren letzte Bewertung vor diesem Datum liegt.
                                           Der Bewertungszeitraum liege zwischen diesem Datum und dem Datum, das
                                           Sie im Feld Bewertung eintragen.

                                           Produkt von … bis Auswahl der Produkte, die bewertet werden sollen.

                                           Produktart Auswahl der Produktart, deren Produkte bewertet werden sollen.

                                           Stat. Warengruppe Auswahl der Statistik-Warengruppe, die dem Produkt
                                           zugewiesen ist.
5.20 / 04-2020




                                           Warenhaus, Gang, Regal, Fach Auswahl des Lagerorts, dessen Produkte
                                           bewertet werden sollen.




                 G-228                                                                         A+W Business Fertigung
                 Softwarereferenz                                                                    Lagerbewertung




                                          Nur gültige Bestände (Bestand nicht negativ) Sie können Produkte von
                                          der Bewertung ausschließen, deren Bestand aufgrund von Reservierungen
                                          negativ ist.
                                          ☐ Alle Produkte werden bewertet, die den Auswahlkriterien in den Feldern
                                          Produkt und Produktart entsprechen.
                                          ☑ Nur die Produkte werden bewertet, deren Bestand nicht negativ ist. Darin
                                          sind auch Produkte enthalten, deren Bestand = 0 ist.

                                          Kein Glas mit Abmessungen (0x0) Für die kombinierte Lagerführung wer-
                                          den Produkte mit den Abmessungen 0x0 angelegt, auf die reservierte Mengen
                                          bis zum Abbuchen der verbrauchten Lagerplatten gebucht werden.
                                          ☐ Alle Produkte werden bewertet, die den Auswahlkriterien in den Feldern
                                          Produkt und Produktart entsprechen.
                                          ☑ Produkte mit den Abmessungen 0x0 werden nicht bewertet.

                                          Bewertung Angabe des Datums, zu dem die Lagerwertung berechnet wer-
                                          den soll. Damit können Sie eine Lagerbewertung in der Vergangenheit durch-
                                          zuführen. Die Lagerbestände werden zu diesem Datum berechnet.
5.20 / 04-2020




                 A+W Business Fertigung                                                                       G-229
                 Lagerbewertung                                                                      Softwarereferenz




                                          Lagerbewertung – Bewertung
                                          Lagerwirtschaft > Lagerbewertung > Bewertung




                 Abb. G-116   Lagerbewertung – Bewertung


                                          In diesem Register werden zunächst die Artikel angezeigt, die den Auswahl-
                                          kriterien entsprechen. Wenn Sie die Bewertung über eine der Schaltflächen
                                          gestartet haben, werden die berechneten Werte angezeigt.
                                          Diese Werte werden auch in der Lagerstatistik angezeigt:
                                           “Lagerstatistik – FIFO/LIFO” auf Seite G-214
                                          Die Werte können gespeichert werden. Vor dem Speichern werden alle einge-
                                          stellten Bewertungen nochmal auf ihre Konsistenz geprüft. Wenn hierbei ein
                                          Fehler festgestellt wird, wird dieser angezeigt und keiner der Sätze gespei-
                                          chert. Sie müssen den Fehler bereinigen, um anschließend die Datensätze
                                          speichern zu können.
                                          Wenn Sie die Daten gespeichert haben, können Sie die Bewertung nicht mehr
                                          ändern.

                                          Bewertung

                                          Alle selektieren Sie können aus der Liste einzelne Produkte auswählen. Mit
                                          der Mehrfachauswahl können Sie beliebig viele Produkte markieren. Über die
                                          Schaltflächen können Sie alle Produkte auswählen oder die Auswahl vollstän-
                                          dig aufheben.
5.20 / 04-2020




                                          [LIFO berechnen] startet die Bewertung der markierten Produkte nach dem
                                          LIFO-Verfahren.


                 G-230                                                                      A+W Business Fertigung
                 Softwarereferenz                                                                       Lagerbewertung




                                          [FIFO berechnen] startet die Bewertung der markierten Produkte nach dem
                                          FIFO-Verfahren.

                                          [Beide berechnen] startet die Bewertung der markierten Produkte nach
                                          dem beiden Verfahren.

                                          Bewertungsart ändern Auswahl der Bewertungsart. Die Änderung der Be-
                                          wertungsart wirkt sich nur auf die markierten Einträge aus.

                                          Übersicht
                                          Folgende Spalten können angezeigt werden:
                                          •   Produkt, Bezeichnung:
                                              Nummer und Bezeichnung des Produkts.
                                          •   Breite, Höhe:
                                              Maße der Scheibe.
                                          •   Inhalt:
                                              Inhalt eine Kiste.
                                          •   Farbe:
                                              Farbvariante des Glases.
                                          •   Lagerort:
                                              Vollständiger Lagerort.
                                          •   PE:
                                              Preiseinheit des Produkts.
                                          •   Lagerbestand:
                                              Aktueller Lagerbestand ohne Reservierungen.
                                          •   ME:
                                              Mengeneinheit, in der das Produkt im Lager geführt wird.
                                          •   Bewertung:
                                              Art der Bewertung:
                                              – Keine:
                                                  Der Bestand dieses Produkts wurde nicht berechnet.
                                              – LIFO, FIFO:
                                                  Der Lagerwert ist als LIFO-, FIFO-Wert berechnet.
                                              – Durch. EK:
                                                  Der Lagerwert ist ein durchschnittlicher EK-Wert.
                                              – Manuell:
                                                  Der Lagerwert ist manuell eingetragen.
                                          •   FIFO, LIFO:
                                              Berechneter Lagerwert des Produkts.
                                          •   Durch. EK:
                                              Durchschnittlicher Einkaufspreis. Dieser Preis wird nur berechnet, wenn in
                                              den Firmendaten die entsprechende Option aktiviert ist.
                                          •   Manuell:
                                              Der Wert der manuellen Eingabe wird als Lagerwert eingetragen.
5.20 / 04-2020




                 A+W Business Fertigung                                                                          G-231
                 Lagerbewertung                                                              Softwarereferenz




                                  •   Bemerkung FIFO/LIFO:
                                      Anzeige des Status nach der Bewertung:
                                      – OK:
                                         Der Bestand dieses Produkts wurde berechnet. Dieser Status ist bei der
                                         Erstbewertung nicht möglich.
                                      – Bestand ist negativ!:
                                         Der Bestand dieses Produkts kann nicht berechnet werden, weil der Be-
                                         stand negative Werte enthält.
                                      – Es wurde kein Anfangssatz gefunden:
                                         Der Bestand dieses Produkts kann nur nach durchschnittlichen EK oder
                                         manuell bewertet werden.
                                      – Menge muss größer 0 sein:
                                         Der Bestand dieses Produkts kann nicht berechnet werden, weil kein
                                         Bestand vorhanden ist.
                                  •   Letzte Bewertung:
                                      Datum der letzten Lagerbewertung.
                                  •   Bewertung:
                                      Wert der letzten Bewertung.
5.20 / 04-2020




                 G-232                                                               A+W Business Fertigung
Lagerwirtschaft             G

                       Partindex




                  A+W Business
                 Partindex                                                            Index Lagerwirtschaft




                 Index Lagerwirtschaft
                 A                                           E
                 Abfragen G-202                              Einkaufspreis G-58
                 Aufbruch einer Kiste G-200                  EK-Preis
                 Auftrag                                     – durchschnittlicher EK G-53
                 – intern G-134                              – Einstellungen prüfen G-57
                 – Lagerartikel erfassen G-120               – kombinierter Lagermodus G-53
                 – Produktionsauftrag G-132                  Erstinventur G-158
                 Auftragsposition
                 – Buchung prüfen G-124                      F
                 Auswahl                                     Firmendaten
                 – Lagerhistorie G-205                       – Einstellungen G-31
                                                             – EK-Berechnung aktivieren G-57
                 B                                           – Lagerführungsmodus aktivieren G-33
                 Bemerkung zur Lagerbewegung G-201           Funktionen
                 Berechnung                                  – Inventurabschluss (Menü) G-180
                 – Ablauf EK-Preisberechnung G-54            – Inventurverwaltung (Menü) G-176
                 – Verschnitt G-43
                 Beschaffungsart G-40                        H
                 Bestellübergabe                             Historie
                 – Menü Funktionen G-220                     – Lager G-204
                 – Menü Optionen G-221                       – Lagerwirtschaft G-89
                 Bestellung
                 – an Einkauf übergeben G-109
                 – automatisch G-108                         I
                 – Bestellmenge nach Bestandsprüfung G-135   Inventur G-166
                 – Bestellvorschlag übergeben G-109          – abschließen G-154
                 – Lager G-220                               – Abschluss G-180
                 – Lieferanten ändern G-112                  – Artikel erfassen G-153
                 – Mindestmenge und Bestellmenge G-108       – Bestand auf Null setzen G-153
                 – Preisvergleich G-114                      – Gehe zu Artikel G-179
                 – Termin ändern G-112                       – gezählte Mengen eingeben G-152
                 – Vorschlag G-108                           – Inventurliste erstellen G-146
                 Bewertung                                   – Inventurliste löschen G-155
                 – FIFO/LIFO G-230                           – Istbestand, Sollbestand G-143
                 Blattanzahl einer Kiste G-199               – Kiste G-144
                 Buchung                                     – Lagerbewertung G-168
                 – für Auftragsposition prüfen G-124         – Listendruck G-171
                 Buchungsart                                 – Nachtragsinventur G-183
                 – für Lagerbuchung G-46                     – Produktstammdaten G-148
                 – Lager G-79                                – qm-Artikel G-144
                 Buchungsjournal G-202                       – Sollbestand G-173
                 – für Lager erstellen G-90                  – Sollbestand ermitteln G-151
                 – Lagerwirtschaft G-89                      – Verwaltung G-175
                                                             – Wertberichtigung G-144, G-179
                                                             – Zählliste drucken G-148
                 D                                           – Zählwerte erfassen G-152
5.20 / 04-2020




                 Darstellungskonventionen G-13               Inventurabschluss G-154, G-181
                 Durchschnitts-EK G-53                       Inventurliste G-167
                 Durchschnittspreis (Lager) G-55


                 A+W Business Fertigung                                                             G-235
                 Index Lagerwirtschaft                                                       Partindex




                 – drucken G-148                         – Mindestmenge G-71
                 – ergänzen G-149                        – Wiederbeschaffungszeit G-100
                 – erstellen G-146                       Lagerbestellung
                 – laden G-149                           – Bestellpool G-220
                 – löschen G-155                         – manuell erfassen G-128
                 – Nachtragsinventur anhängen    G-156   – Prüfung bei automatischer Bestellung G-135
                 Inventurverwaltung G-176                – Zuschläge G-73
                 – Funktionen G-176                      Lagerbestellung nach Bestandsprüfung G-135
                 – Gehe zu Artikel G-179                 Lagerbewegung G-195
                 – Optionen G-175                        – Abgang, Zugang G-196
                 – Sortierung G-175                      – Aufbruch G-200
                 – Wertberichtigung G-179                – Bemerkung G-201
                 Istbestand G-143                        – Blattanzahl G-199
                                                         – manuell G-79
                 J                                       – Optionen (Menü) G-195
                 Journal                                 – Statistik G-94
                 – für Lagerbuchung anzeigen    G-90     – Umbuchung G-198
                                                         Lagerbewertung
                                                         – Berechnungsbeispiele G-226
                 K                                       – Bewertung G-230
                 Kiste                                   – Inventur G-168
                 – auflösen   G-200                      – Selection G-228
                                                         Lagerbuchung
                 L                                       – Ab- und Zugang G-80
                 Lager                                   – Ab-/Zugang manuell buchen G-81, G-84
                 – aktuellen Bestand anzeigen G-102      – Anwenderstatus G-35
                 – Definition G-21                       – bei Stückliste G-62
                 – Ebene benennen G-24                   – Buchungsart G-79
                 – Ebene definieren G-22                 – Buchungsart auswählen G-46
                 – Erstinventur G-158                    – Erfassungsstelle G-140
                 – Lagerkategorie definieren G-27        – Journal anzeigen G-90
                 – Lagerort definieren G-25              – Journal erstellen G-90
                 – Orte G-21                             – kombinierte Lagerführung G-41
                 – Produktstammdaten prüfen G-44         – Lagerort ändern G-85
                 – Stammdaten Preise prüfen G-58         – manuell G-79, G-80
                 – Vorschau auf Bestand G-99             – reservierte Lagerartikel drucken G-92
                 Lagerabfrage G-89                       – Statistik anzeigen G-94
                 Lagerabgang G-196                       – Statuszuordnung G-36
                 Lagerartikel G-70, G-215                Lagerbuchungsart G-40
                 – bei Inventur erfassen G-153           Lagerführung
                 – Hauptartikel G-70                     – auf Stücklisten-Ebene G-62
                 – im Auftrag G-119                      – kombiniert G-41
                 – in Lagerverwaltung anlegen G-74       – Lagerkennzeichen G-40
                 – Lagermaß G-43, G-48                   – Lagerort G-17
                 – Lagerort umbuchen G-85                – Stückliste einrichten G-65
                 – Produktionsauftrag G-132              Lagerführungsmodus G-30
                 – reserviert G-215                      – EK-Ermittlung G-53
                 – Reservierung drucken G-92             – in Firmendaten aktivieren G-33
                 Lagerbesand                             Lagerhistorie G-204
5.20 / 04-2020




                 – zukünftiger Bestand G-99              – Auswahl G-205
                 Lagerbestand                            – Tabelle G-208
                 – anzeigen G-102                        Lagerkennzeichen G-40
                 – Aufnahme in Inventur G-143


                 G-236                                                         A+W Business Fertigung
                 Partindex                                                            Index Lagerwirtschaft




                 Lagermaß                                   O
                 – in Stammdaten anlegen G-48               Optionen
                 – Lagerartikel G-43, G-48                  – Inventurabschluss (Menü) G-180
                 – Produktverwaltung G-42                   – Inventurverwaltung (Menü) G-175
                 – Stammdaten, Lagerverwaltung G-43         – Lagerbewegung G-195
                 Lagerort
                 – Artikel umbuchen G-85
                                                            P
                 – Bestand G-17
                                                            Preis
                 Lagerstatistik G-209
                                                            – in Bestellvorschlag vergleichen G-114
                 – Produkte G-210
                                                            Preise
                 – Statistik G-212, G-214
                                                            – Lagerverwaltung G-190
                 Lagerverwaltung G-185
                                                            Preislisten
                 – Grundgedanken G-16
                                                            – für EK-Berechnung G-59
                 – Handlungsablauf G-17
                                                            Produkt
                 – Lagerartikel G-186
                                                            – Lagerartikel G-40
                 – Lagerartikel anlegen G-74
                                                            – Lagermaß anlegen G-48
                 – Lagerbestellung manuell erfassen G-128
                                                            – Lagerstatistik G-210
                 – Lager-Hauptartikel G-70
                                                            – Stammdaten für Lager prüfen G-44
                 – Preise G-190
                                                            Produktionsauftrag
                 – Preisentwicklung G-72
                                                            – Lagerzugang G-140
                 – Zusatz G-193
                                                            – Lieferantenkartei G-134
                 Lagerwert
                 – EK-Bewertung G-52
                 Lagerwirtschaft G-165                      R
                 – Buchungsjournal G-89                     Reservierte Lagerartikel drucken G-92
                 – EK-Berechnung aktivieren G-57            Reservierung
                 – Historie G-89                            – für Stückliste G-62
                 – Lagerwert G-89                           – im Lagerjournal anzeigen G-90
                 – Menü-Übersicht G-14                      – Lagerartikel G-215
                 – Statistik G-89                           – Verschnitt G-43
                 Lagerzugang G-196                          Reservierungen G-30
                 – durch Produktionsauftrag G-140
                 Lieferant                                  S
                 – in Bestellung ändern G-112               Sollbestand G-143, G-173
                 Lieferantenkartei                          Sollbestand ermitteln G-151
                 – interner Kunde G-134                     Sortierung
                 – Produktionsauftrag G-134                 – Inventurverwaltung G-175
                                                            Sperre der Produktstammdaten G-148
                 M                                          Stammdaten
                 Menü                                       – Anwenderstatus für Lagerbuchung G-35
                 – Funktionen (Bestellübergabe) G-220       – Lagerebene benennen G-24
                 – Optionen (Bestellübergabe) G-221         – Lagerebene definieren G-22
                 Mindestmenge                               – Lagerkategorie definieren G-27
                 – Lagerbestand G-71                        – Lagermaß anlegen G-48
                                                            – Lagerort definieren G-25
                                                            – Preisdaten für Lagerware G-58
                 N
                                                            – Preislisten für EK-Berechnung prüfen G-59
                 Nachtragsinventur anhängen   G-156
                                                            – Produkt prüfen G-44
                                                            – Statuszuordnung für Lagerbuchung G-36
5.20 / 04-2020




                                                            Statistik
                                                            – für Lagerbewegung anzeigen G-94
                                                            – Lager G-209
                                                            – Lagerwirtschaft G-89


                 A+W Business Fertigung                                                               G-237
                 Index Lagerwirtschaft                                    Partindex




                 Status
                 – Lagerbuchung G-33
                 – Zuordnungen für Lagerbuchung G-35
                 Stückliste
                 – für Lagerführung einrichten G-65
                 Suche (Lagerinfo) G-217

                 U
                 Umbuchung von Lagerartikeln    G-198

                 V
                 Verschnitt   G-43

                 W
                 Wareneingang
                 – Lagerbuchung G-80
                 Wertberichtigung
                 – Inventur G-144

                 Z
                 Zählliste G-171
                 Zählliste drucken G-148
                 Zählwerte erfassen G-152
                 Zusatz
                 – Lagerverwaltung G-193
                 Zuschlag
                 – Verteilung in Lagerbestellungen   G-73
5.20 / 04-2020




                 G-238                                      A+W Business Fertigung

