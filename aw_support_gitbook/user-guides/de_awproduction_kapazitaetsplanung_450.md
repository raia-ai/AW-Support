---
title: "DE AWProduction Kapazitaetsplanung 4.50"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWProduction_Kapazitaetsplanung_4.50"]
version: "1.0"
last_updated: "2025-12-10"
description: "Kapazitätsplanung          E                                deutsch                     A+W Production                                                                                                                  Vorspann                                             Vorspann                                         In diesem Teil der Dokumentation finden Sie editorische Notizen.                                           Revisionsübersicht                                         Part"
source_file: "DE_AWProduction_Kapazitaetsplanung_4.50.pdf"
---


# DE AWProduction Kapazitaetsplanung 4.50

Kapazitätsplanung          E




                           deutsch




                A+W Production
                                                                                                                 Vorspann




                                        Vorspann
                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                        Revisionsübersicht
                                        Part                     Beschreibung
                                        Version / Datum

                                        4.50 / 01-2023           Arbeitsplan exportieren hinzugefügt.

                                        4.00 / 11-2017           Vollständige Überarbeitung.

                                        3.01 / 01-2017           Produkt- und Firmennamen angepasst.

                                        3.00 / 08-2013           Ersterstellung des Tutorials und vollständige
                                                                 Überarbeitung der Softwarereferenz.

                                        2.00 / 04-2008           Überarbeitung.

                                        1.20 / 11-2007           Namensänderung (AWCapacity/Kapazitätsplanung).

                                        1.10 / 2007              Änderung Kapitel Arbeitsplan.

                                        1.00 / 2007              Ersterstellung



                                        Editorial
                                        Das Editorial enthält Informationen zu folgenden Themen:
                                        •   Anmerkungen zu diesem Dokument
                                        •   Urheberrechte
                                        •   Warenzeichen
                                        •   Kontakte

                                        Anmerkungen zu diesem Dokument
                                        Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Produc-
                                        tion gedacht.
                                        Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz
                                        vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden.
                                        Der Inhalt der Dokumentation dient nur der Information und kann jederzeit
                                        ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Tex-
                                        ten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem kön-
                                        nen Fehler nicht vollständig ausgeschlossen werden. Die A+W Software
                                        GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei
                                        denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
                                        Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                    E-3
                 Vorspann




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

                            Kontakte
                            A+W Software GmbH
                            Am Pfahlgraben 4-10
                            D-35415 Pohlheim
                               +49 6404 2051-0
                               +49 6404 2051-877
                            aw.zentrale@a-w.com
                            http://www.a-w.com
4.50 / 01-2023




                 E-4                                                 A+W Production Kapazitätsplanung
                                                                                                                                                                Inhalt




                                        Inhalt
                                        Vorspann ................................................................................................................ E-3
                                          Revisionsübersicht .............................................................................................. E-3
                                          Editorial ............................................................................................................... E-3
                                        Inhalt ....................................................................................................................... E-5

                                        Tutorial                                                                                                                E-9
                                        Überblick ............................................................................................................... E-11
                                          Dokumentation .................................................................................................. E-12
                                            Aufbau des Tutorials ...................................................................................... E-12
                                            Darstellungskonventionen .............................................................................. E-13
                                        Grundlagen ........................................................................................................... E-14
                                          Terminoptimierung ............................................................................................ E-15
                                          Terminfindung ................................................................................................... E-16
                                        Planung und Einlastung ........................................................................................ E-21
                                          Produktionsmonitor ........................................................................................... E-22
                                            Tagesaktuelle Anpassungen der Arbeitsschichten ........................................ E-24
                                            Produktionsmonitor einrichten ....................................................................... E-31
                                          Arbeitsplan exportieren ..................................................................................... E-34
                                          Einlastung und Umlastung ................................................................................ E-35
                                            Aufträge einlasten .......................................................................................... E-36
                                            Umlastungen .................................................................................................. E-37
                                            Bearbeitungen umlasten ................................................................................ E-39
                                            Fehlerhafte Einlastung ................................................................................... E-41
                                            Eingelastete Aufträge nachbearbeiten ........................................................... E-42
                                          Kampagnenplanung .......................................................................................... E-44
                                            Definition der Kampagnen ............................................................................. E-45
                                            Kampagnen in der Terminfindung .................................................................. E-47
                                            Kampagnen anlegen und verwalten .............................................................. E-47
                                            Übungen zu Kampagnen ............................................................................... E-53
                                          Reservierungen ................................................................................................. E-54
                                            Reservierung von Kapazitäten ....................................................................... E-55
                                            Reservierungen anlegen und verwalten ........................................................ E-56
                                            Übungen zu Reservierungen ......................................................................... E-62
                                          Bearbeitungserzeugung .................................................................................... E-63
                                            Bearbeitungserzeugung für die Einlastung .................................................... E-64
                                            Bearbeitungen erzeugen ................................................................................ E-65
                                        Stammdaten der Kapazitätsplanung ..................................................................... E-68
                                          Schichten ........................................................................................................... E-69
                                            Schichtpläne .................................................................................................. E-70
                                            Arbeitsfreie Tage anlegen .............................................................................. E-72
                                            Schichtplan erstellen ...................................................................................... E-75
                                            Schichtregel erstellen ..................................................................................... E-78
                                            Schichtgruppe erstellen ................................................................................. E-83
                                            Übungen ........................................................................................................ E-87
                                          Kostenkalkulation .............................................................................................. E-88
                                            Definition der Kostenkalkulation ..................................................................... E-89
                                            Kosten anlegen und verwalten ....................................................................... E-90
                                            Übungen ........................................................................................................ E-92
                                          Übergangszeiten ............................................................................................... E-93
                                            Übergangszeiten in Schichten oder Stunden ................................................. E-95
4.50 / 01-2023




                                            Definition von Übergangszeiten ..................................................................... E-99
                                            Übergangszeiten anlegen und verwalten ..................................................... E-102
                                            Übungen ...................................................................................................... E-105
                                          Vorgabezeiten ................................................................................................. E-106


                 A+W Production Kapazitätsplanung                                                                                                                 E-5
                 Inhalt




                               Definition der Vorgabezeiten ........................................................................ E-107
                               Struktur von Vorgabezeitformeln ................................................................. E-108
                               Berechnung von Zeitzuschlägen .................................................................. E-111
                               Editor für Formelelemente ........................................................................... E-113
                               Beispiel – Vorgabezeit für die logische Maschine Zuschnitt ........................ E-114
                               Zeitformel-Objekte ....................................................................................... E-117
                               Vorgabezeitformeln anlegen und verwalten ................................................. E-118
                               Zeitformel testen .......................................................................................... E-125
                               Übungen ...................................................................................................... E-131
                             Maschinengruppen .......................................................................................... E-132
                               Definition der Maschinengruppen ................................................................ E-133
                               Maschinengruppen anlegen und verwalten ................................................. E-134
                               Übungen ...................................................................................................... E-137
                             Lastverteilung .................................................................................................. E-138
                               Definition der Lastverteilung ........................................................................ E-139
                               Lastverteilung einrichten und bearbeiten ..................................................... E-140
                               Übungen ...................................................................................................... E-143

                          Softwarereferenz                                                                                              E-145
                          Überblick ............................................................................................................. E-147
                          Einlastung ........................................................................................................... E-148
                            Produktionsmonitor ......................................................................................... E-149
                            Angezeigte Maschinen .................................................................................... E-153
                            Einstellungen ................................................................................................... E-154
                            Bitte wählen Sie einen Auftrag / Lauf aus (Filtern) .......................................... E-157
                              Filter – Aufträge ........................................................................................... E-157
                              Filter – Läufe ................................................................................................ E-158
                              Filter – Eigene Filter ..................................................................................... E-159
                            Neuen Filter erstellen ...................................................................................... E-160
                            Maschine (Name) ............................................................................................ E-161
                            Schichten für Maschine anpassen .................................................................. E-163
                            Schichteigenschaften ...................................................................................... E-164
                            Reservierungsanzeige ..................................................................................... E-166
                            Arbeitsplan aus Produktionsmonitor ................................................................ E-167
                              Arbeitsplan – Details .................................................................................... E-168
                              Arbeitsplan – Übersicht ................................................................................ E-170
                            Einlastung ........................................................................................................ E-171
                            Stücklistenkonfiguration .................................................................................. E-172
                            Aktion .............................................................................................................. E-173
                            Umlastung ....................................................................................................... E-174
                            Maschinenumlastung ...................................................................................... E-178
                            Nachbearbeitung Einlastung ........................................................................... E-179
                            Fehlerhafte Aufträge ........................................................................................ E-182
                            Asynchrone Verarbeitung ................................................................................ E-183
                            Änderung bereits verplanter Aufträge ............................................................. E-184
                            Positionssplit ................................................................................................... E-185
                          Kampagnen und Reservierungen ....................................................................... E-187
                            Kampagnen ..................................................................................................... E-188
                              Kampagnen – Einzeltermine ........................................................................ E-189
                              Kampagnen – Wöchentliche Termine .......................................................... E-191
                            Abgelaufene Reservierungen .......................................................................... E-192
                            Reservierungen ............................................................................................... E-194
                            Reservierung für Maschine ............................................................................. E-197
4.50 / 01-2023




                            Kunde auswählen ............................................................................................ E-198
                            Objekt auswählen ............................................................................................ E-199
                          Bearbeitungen .................................................................................................... E-200
                            Bearbeitungserzeugung .................................................................................. E-201


                 E-6                                                                        A+W Production Kapazitätsplanung
                                                                                                                                                          Inhalt




                                          Existierende Bedingung hinzufügen ................................................................ E-204
                                        Stammdaten für Zeiten ....................................................................................... E-205
                                          Vorgabezeiten ................................................................................................. E-206
                                          Vorgabezeitformel ........................................................................................... E-208
                                          Elemente hinzufügen ....................................................................................... E-212
                                          Tabelle, Vektor (Name) ................................................................................... E-213
                                          Eingabehilfe für Vektoren ................................................................................ E-214
                                          Formel auswählen ........................................................................................... E-216
                                          Erfassung eines Formelelements .................................................................... E-217
                                          Benutzerdefinierte Tabellenelemente .............................................................. E-219
                                          Grenzwert auswählen ...................................................................................... E-220
                                          Zeitformeltest ................................................................................................... E-221
                                          Eigenschaften des Formelobjekts ................................................................... E-223
                                          Formel (Name) ................................................................................................ E-225
                                          Verlauf der Formelauswertung ........................................................................ E-226
                                          Übergangszeiten ............................................................................................. E-227
                                        Stammdaten der Schichten ................................................................................ E-230
                                          Schichten ......................................................................................................... E-231
                                          Schichtkalender ............................................................................................... E-233
                                          Schichtplan ...................................................................................................... E-234
                                          Schichtregel ..................................................................................................... E-236
                                          Schichtgruppe ................................................................................................. E-238
                                          Maschine ......................................................................................................... E-240
                                        Maschinen und Kosten ....................................................................................... E-242
                                          Kostenkalkulation ............................................................................................ E-243
                                          Maschinengruppen .......................................................................................... E-245
                                          Lastverteilung .................................................................................................. E-247

                                        Partindex                                                                                                   E-249
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                                                           E-7
                 Inhalt
4.50 / 01-2023




                 E-8      A+W Production Kapazitätsplanung
Kapazitätsplanung           E

                        Tutorial




                A+W Production
                 Tutorial                                                                                    Überblick




                                        Überblick
                                        Das Tutorial zum Modul Kapazitätsplanung beschäftigt sich mit der Planung
                                        Ihres Produktionsablaufs und der optimalen Nutzung der Kapazität Ihres
                                        Maschinenparks. Ziele der Kapazitätsplanung sind die Liefertermine einzuhal-
                                        ten, den Maschinenpark effizient zu nutzen und flexibel auf unvorhersehbare
                                        Ereignisse reagieren zu können. Eine optimale Kapazitätsplanung stellt immer
                                        einen Kompromiss zwischen größtmöglicher Effizienz und größtmöglicher
                                        Flexibilität dar.
                                        In diesem Tutorial ist beschrieben, wie Sie manuell in die Planung eingreifen
                                        können und wie die Stammdaten für die Kapazitätsplanung eingerichtet wer-
                                        den.
                                        Das Tutorial umfasst folgende Themenblöcke:
                                        •   “Grundlagen” auf Seite E-14
                                        •   “Planung und Einlastung” auf Seite E-21
                                        •   “Stammdaten der Kapazitätsplanung” auf Seite E-68

                                        Vorausgesetzte Kenntnisse
                                        Das Tutorial richtet sich an Mitarbeiter, die in A+W Production die Arbeitsvor-
                                        bereitung verantworten und damit den optimalen Ablauf der Produktion orga-
                                        nisieren. Die Mitarbeiter müssen die Maschinenzuordnung (MZO) und das
                                        Konzept der Stammdaten in A+W Production kennen. Außerdem sind Kennt-
                                        nisse der Grob- und Feinplanung hilfreich.

                                            Stammdaten vor Zugriff schützen
                                            Die Stammdaten von A+W Production und insbesondere von A+W Capa-
                                            city Planner sind hochsensible Daten. Unkontrollierte oder unbeabsichtigte
                                            Eingriffe und Änderungen können die gesamte Produktion stilllegen.
                                            Richten Sie daher die jeweiligen Arbeitsplätze so ein, dass nur die Admi-
                                            nistratoren oder Mitarbeiter mit entsprechenden Funktionen Zugriff auf die
                                            Stammdaten haben.

                                            Datensicherung
                                            Erstellen Sie eine vollständige Datensicherung der Stammdaten bevor Sie
                                            mit der Bearbeitung der Stammdaten beginnen. Das Backup-Tool finden
                                            Sie unter:
                                            C:\Programme (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe.
                                            Verschieben Sie das gespeicherte Backup aus Ihrem User-Verzeichnis in
                                            ein Verzeichnis, auf das auch der Support Zugriff hat.
                                            Besprechen Sie die anstehenden Änderungen vorab mit Ihrem Projektierer
                                            bei der A+W Software GmbH.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-11
                 Überblick                                                                          Tutorial




                             Dokumentation
                             Für das Modul Kapazitätsplanung stehen folgende Dokumente zur Verfügung:

                             Format                  Umfang

                             PDF                     Vollständige Unterlagen
                                                     • Tutorial
                                                     • Softwarereferenz
                                                     • Index

                             Online-Hilfe <F1>       Dialog-Hilfe


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

                             Übungen                 Zu einigen Lerneinheiten finden Sie Übungen mit
                                                     Aufgabenstellungen.
4.50 / 01-2023




                 E-12                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                                       Überblick




                                        Darstellungskonventionen
                                        Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                        gende Bedeutung:

                                        Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                                 Software bezeichnen, z. B. der Dialog
                                                                 Kampagnenplanung.

                                        Fett                      sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                                  Tastatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                                        >                         Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                                  gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                                  Stammdaten > Kapazitätsplanung >
                                                                  Kampagnenplanung > Kampagne hinzufügen.

                                        []                        Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                  z. B.: Mit [OK] speichern Sie die Daten.

                                        <>                        Spitze Klammern bezeichnen Tasten oder
                                                                  Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                                  öffnen Sie die Online-Hilfe.


                                        Lesehinweis
                                        Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der voraus-
                                        gegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinhei-
                                        ten zu überspringen.
                                        Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die
                                        Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten De-
                                        tails zu vergegenwärtigen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                   E-13
                 Grundlagen                                                                          Tutorial




                              Grundlagen
                              A+W Capacity Planner ist so ausgelegt, dass auch für Produkte mit unge-
                              wöhnlich tiefen Stücklisten meist gleich mehrere sichere Pfade von der Start-
                              technologie bis zum Versand gefunden werden. Die Kapazitätsplanung greift
                              dazu auf die Arbeitsgänge zu, die die Scheiben vom Zuschnitt bis zur Auslie-
                              ferung durchlaufen.

                              Stammdaten der Maschinenzuordnung
                              Die Maschinenzuordnung (MZO) stellt die Verbindung zwischen Arbeitsgän-
                              gen und Maschinen dar und bildet die Bewertung nach Vorzugsmaschinen ab.
                              Damit für die zu fertigenden Scheiben gültige Maschinen gefunden werden,
                              müssen die Maschinen präzise beschrieben sein. In der Maschinenzuordnung
                              wird dazu zwischen physikalischen Restriktionen und logischen Maschinen
                              mit zusätzlichen Restriktionen, Kostensätzen und Übergangszeiten unter-
                              schieden.
                              Da die Schritte zum Einrichten der Kapazitätsplanung auf den logischen Ma-
                              schinen beruhen, muss der Maschinenpark vollständig beschrieben sein. Die
                              Informationen dazu finden Sie im Part Maschinenzuordnung.

                              Stammdaten der Kapazitätsplanung
                              Für die Terminbestimmung werden Schichtpläne, Übergangszeiten und Zeiten
                              für die Bearbeitungsdauer benötigt.
                              •   Damit sich zum Test der Daten ein einfaches Bild für die Auslastung ergibt,
                                  empfiehlt es sich, die Bearbeitungsdauern pauschal in Sekunde pro Stück
                                  anzugeben, z. B. 1 - 5 Minuten pro Scheibe je nach Maschine.
                              •   Für die Übergangszeiten soll der optimale und realistische Produktions-
                                  durchlauf beschrieben werden.
                                  Die Angabe der Zeiten in ganzen Schichten sorgt für eine einfache und vor-
                                  hersagbare Terminbestimmung. An Maschinen, die auch unbeaufsichtigt
                                  arbeiten können, kann die Übergangszeit (Verweildauer) in Stunden ange-
                                  geben werden, z. B. Heatsoak, Autoklav oder Aushärten von Silikonversie-
                                  gelungen. Achten Sie bei den Übergängen darauf, dass Sie im Betrieb den
                                  Platz benötigen, um die Glasmenge einer Schicht abzustellen.
                              •   Aus den Zeiten für die Bearbeitungsdauer können die Engpässe für die
                                  Einlastung bestimmt werden.

                              Einlastungsregeln
                              Die Einlastungsregeln werden als Konfigurationsparameter für A+W Capacity
                              Planner festgelegt. Sie beeinflussen das Programmverhalten, die Meldungs-
                              kultur und die möglichen Benutzerreaktionen. Dies betrifft z. B.:
                              •   Dürfen Liefertermine verschoben werden.
                              •   Wann ist der früheste Produktionsbeginn für einen eingelasteten Auftrag.
                              •   Wie werden Angebote eingelastet und müssen sie wieder storniert werden.
4.50 / 01-2023




                              •   Wie werden Eilaufträge durchgeschleust.
                              •   Ab welcher Stückzahl müssen Positionen gesplittet werden.




                 E-14                                                   A+W Production Kapazitätsplanung
                 Tutorial                                                                                            Grundlagen




                                              Terminoptimierung
                                              Die Terminoptimierung beginnt mit dem letzten Betriebsmittel am oder vor
                                              dem Liefertermin: dem Verladen. Mit Blick auf den Produktionsmonitor kann
                                              die Terminoptimierung wie folgt dargestellt werden.


                                                    Mittwoch          Donnerstag          Freitag               Montag

                  Float Zuschnitt

                  Sortierung für Be...

                  Beschichtungsanl.

                  Sortierung für ISO

                                                                                      1
                  Rahmenbieger 1
                                                                                                    0
                  ISO-Linie 2
                                                                                                    0
                  ISO versiegeln
                                                                                                            2
                                                                                                                         0
                  Verpacken
                                                                                                        2
                  Fuhrpark



                                          F                             E                               D   C    B       A
                 A Fuhrpark – Beladung                 C Berechnungsweg 2                 E Konfliktfall
                 B Berechnung mit optimaler            D Übergangszeit in Schichten       F Produktionsbeginn Zuschnitt
                   Übergangszeit
                 Abb. E-1       Einlastungswege mit und ohne Konfliktfall


                                              Ausgehend vom Fahrtermin wird nach Abzug der Kundenhandlingzeit (in Ar-
                                              beitstagen) das Produktionsende festgelegt. Vom Ende der letzten möglichen
                                              Arbeitsschicht (A) aus sucht die Terminierung rückwärts nach dem spätest-
                                              möglichen Produktionsbeginn.
                                              Die Übergangszeiten von einer Bearbeitung zur nächsten werden in Schich-
                                              ten (D) gezählt, wobei 0 die unmittelbar folgende Bearbeitung in derselben
                                              Schicht ist. Gesperrte Schichten, die mit einem X gekennzeichnet sind, wer-
                                              den dabei mitgezählt.
                                              Die Berechnung prüft immer alle möglichen kostengünstigen Wege. Bei Ter-
                                              minkonflikten werden Übergangszeiten beibehalten und es entsteht ein Puffer
4.50 / 01-2023




                                              am Ende der Produktion. Wenn dabei zu lange Lagerungszeiten entstehen,
                                              müssen die Pufferzeiten manuell verteilt werden. Die dabei entstehenden Lö-
                                              sungen sind jedoch wesentlich teurer.


                 A+W Production Kapazitätsplanung                                                                            E-15
                 Grundlagen                                                                                             Tutorial




                                               Der Produktionsmonitor ist in einer separaten Einheit ausführlich beschrieben.
                                                “Produktionsmonitor” auf Seite E-22



                                               Terminfindung
                                               In diesem Kapitel sind technische Hintergrundinformationen für die Terminfin-
                                               dung zusammengefasst.
                                               Die Terminfindung in A+W Capacity Planner wird von der Einlastung und der
                                               interaktiven Umlastung genutzt, um den Stücklisten gültige Bearbeitungster-
                                               mine und -maschinen zuzuweisen.
                                               Die Terminfindung durchläuft fünf Phasen:
                                               •   Analyse der Stückliste.
                                               •   Erstellung der Maschinenwege.
                                               •   Bestimmung möglicher Produktionstermine.
                                               •   Bewertung möglicher Produktionstermine.
                                               •   Auswahl der günstigsten Lösung.

                                               Analyse der Stückliste
                                               Die Stückliste wird in Teileketten zerlegt, das sind Stücklistenabschnitte, deren
                                               erste Bearbeitung keine Vorgängerbearbeitung hat oder die mehrere Stücklis-
                                               tenteile vereinigen. Die einzelnen Teileketten werden unabhängig und parallel
                                               berechnet. Die einzelnen Ergebnisse werden am Schluss der Berechnung zur
                                               endgültigen Stückliste abgestimmt.




                                         ISO                                                    ISO            VSG

                                                                              Teileketten
                                       Rahmen                                                           PVB           Rahmen
                        ESG                            VSG


                                                       PVB
                                         TVG                          TVG                       ESG           TVG    TVG


                        Float



                                         Float                        Float                     Float     Float      Float


                 Abb. E-2       Bildung von Teileketten aus der Stückliste
4.50 / 01-2023




                                               Während die Stückliste für die Terminfindung aufgebaut wird, wird sie gleich-
                                               zeitig auf Plausibilität geprüft. Dabei werden Fehler in der Stückliste erkannt
                                               und gemeldet:



                 E-16                                                                       A+W Production Kapazitätsplanung
                 Tutorial                                                                                               Grundlagen




                                               •   Verwaiste Stücklistenteile und Bearbeitungen werden erkannt und über-
                                                   sprungen. In den Logfiles wird eine Warnung geschrieben.
                                               •   Bearbeitungssequenzen werden geprüft und angepasst. Erzeugende Be-
                                                   arbeitungen erhalten grundsätzlich die Sequenz 100, Bearbeitungen mit
                                                   kleinerer Sequenz werden nach der erzeugenden Bearbeitung angeord-
                                                   net.
                                               •   Fehlende erzeugende Bearbeitungen werden erkannt und gemeldet.
                                               •   Fehlende logische Maschinen werden erkannt und gemeldet.
                                               •   Inkonsistenzen zwischen den Bearbeitungsdaten und MZO-Stammdaten
                                                   werden erkannt.

                                               Erstellung der Maschinenwege
                                               Für die Berechnung der Maschinenwege stehen in A+W Capacity Planner
                                               zwei Features zur Verfügung: Besttechnologie und Automatische Maschinen-
                                               umlastung.
                                               Wenn nur Besttechnologie verwendet wird, gibt es genau einen Maschinen-
                                               weg. Alternative Maschinen werden nicht verwendet.




                 A
                       Zuschnitt   Schleifen       Polieren   Ecken      Bohren      Bohren      Ausschnitt     Vor-        Sieb-
                                                              stoßen                                          spannen       druck
                 B



                                     C               C          D          E          E                                      F
                 A Bearbeitungen                         C Kein Maschinenwechsel              E Kein Maschinenwechsel
                 B Definierte Maschinen                  D Informative Bearbeitung            F Siebdruck + nachfolgender
                                                                                                Siebdruck
                 Abb. E-3      Maschinenweg bei Besttechnologie


                                               Durch Bildung von Bearbeitungsketten auf einer Maschine lassen sich aufei-
                                               nanderfolgende Bearbeitungen zusammenfassen, sofern die Maschinenalter-
                                               nativen dieselben sind. Aufeinanderfolgende Bearbeitungen (C, E) ohne
                                               Maschinenwechsel werden zum selben Termin durchgeführt. Um das zu ver-
                                               hindern, z. B. bei zwei aufeinanderfolgenden Siebdrucken (F), muss eine
                                               Übergangszeit definiert werden, damit der erste Druck trocknen kann, bevor
                                               der zweite aufgetragen wird.
                                               Informative Bearbeitungen (D) werden der Vorgängerbearbeitung zugeordnet.

                                                   Bearbeitungsketten und automatische Umlastung
                                                   Die Einstellungen für Bearbeitungsketten und automatische Umlastung
                                                   werden in den Maschineneigenschaften angegeben. Die Maschinen sind
                                                   im Part Maschinenzuordnung (MZO) beschrieben.
4.50 / 01-2023




                                               Bei der Automatischen Maschinenumlastung werden für jede Bearbeitung in
                                               der Teilekette alle Maschinenalternativen ermittelt und miteinander verbun-



                 A+W Production Kapazitätsplanung                                                                            E-17
                 Grundlagen                                                                                             Tutorial




                                                den. Die Zahl der Maschinenwege kann dabei so groß werden, dass keine Lö-
                                                sung möglich ist. Daher muss die Anzahl der alternativen Maschinen begrenzt
                                                werden.




                        Zuschnitt   Schleifen       Polieren    Ecken     Bohren     Bohren      Ausschnitt     Vor-    Sieb-
                                                                stoßen                                        spannen   druck

                 A


                 B


                 C


                 A Bevorzugte Maschinen                   B Alternative Maschinen             C Manuelle Fertigung
                 Abb. E-4      Automatische Maschinenumlastung


                                                In diesem Beispiel sehen Sie, dass die alternativen Maschinen begrenzt sind:
                                                alle Maschinen, in denen von Hand gearbeitet wird, werden nicht in die Ermitt-
                                                lung der Maschinenwege einbezogen.
                                                Für jede Bearbeitung einer Teilekette wird die Menge gültiger Alternativma-
                                                schinen geladen und mit Übergängen versehen.
                                                •   Für jede Bearbeitung gilt die durch die MZO bestimmte oder durch frühere
                                                    Umlastung festgelegte Maschine. Falls die automatische Umlastung aktiv
                                                    ist und die Bearbeitung noch nicht begonnen wurde, werden zusätzlich Ma-
                                                    schinen mit der Eigenschaft Automatische Umlastung in die Liste mögli-
                                                    cher Alternativen aufgenommen.
                                                •   Aufeinanderfolgende Bearbeitungen ohne Maschinenwechsel werden zum
                                                    selben Termin durchgeführt.
                                                •   Maschinen, die Bearbeitungsketten bilden, können aufeinanderfolgende
                                                    Bearbeitungen zusammenfassen, sofern deren Bearbeitungsalternativen
                                                    identisch sind.
                                                •   Maschinen, die keiner Erfassungsstelle zugeordnet sind, verarbeiten ledig-
                                                    lich informative Bearbeitungen, z. B. Ecken stoßen. Diese Bearbeitungen
                                                    werden der Vorgängerbearbeitung zugeordnet und mit ihr verplant. Die
                                                    erste Bearbeitung einer Teilekette darf darum keine informative Bearbei-
                                                    tung sein.
                                                Alle gefundenen Maschinen werden mit ihren Vorgängermaschinen verbun-
                                                den, sofern die Übergänge erlaubt sind. So entsteht für eine Teilekette die
                                                Menge aller Maschinenwege mit Startpunkten und Endpunkten. Für jeden ein-
                                                zelnen Weg innerhalb der Menge gilt, dass er alle Bearbeitungen der Teileket-
                                                te genau einmal enthalten darf.
4.50 / 01-2023




                 E-18                                                                    A+W Production Kapazitätsplanung
                 Tutorial                                                                                 Grundlagen




                                            Anzahl der Alternativmaschinen klein halten
                                            Für jede Bearbeitung in der Teilekette werden alle Maschinenalternativen
                                            ermittelt und miteinander verbunden. Die Zahl der Maschinenwege kann
                                            dabei so groß werden, dass keine Lösung möglich ist.
                                            Begrenzen Sie daher die Anzahl der Maschinenalternativen. Bilden Sie au-
                                            ßerdem Bearbeitungsketten. Das erhöht die Performance deutlich.

                                        Bestimmung möglicher Produktionstermine
                                        Anhand der Maschinenwege, der Schichtpläne und der Übergänge zwischen
                                        den beteiligten logischen Maschinen werden die möglichen Produktionstermi-
                                        ne für die einzelnen Bearbeitungsschritte bestimmt. Dazu werden auch deren
                                        (virtuelle) Kosten berechnet und die Einlastungsrechte bestimmt, die für die
                                        Nutzung der Übergänge benötigt werden.
                                        Unterhalb der letzten Bearbeitung der Stückliste, unterhalb jeder zusammen-
                                        führender Bearbeitung und unterhalb von Kampagnen, Umlastungszielen und
                                        Datumssperren sind beliebige Übergänge zugelassen.
                                        Dadurch wird gewährleistet, dass gültige Produktionstermine auch dann zur
                                        Verfügung stehen, wenn die Freiheitsgrade der Terminfindung extrem einge-
                                        schränkt sind.
                                        Als Ergebnis steht die Menge aller terminierten Maschinenwege zur Verfü-
                                        gung, sodass die nachfolgende Bewertung die günstigsten Wege ermitteln
                                        kann.

                                        Bewertung möglicher Produktionstermine
                                        Die Menge aller gefundenen Produktionstermine wird komplett abgelaufen
                                        und bewertet. Dabei entstehen Lösungsmengen für Start- und Endtermine der
                                        Maschinenwege und deren (virtuelle) Kosten. Begünstigt werden:
                                        •   Möglichst schneller Produktionsdurchlauf.
                                        •   Vorrangige Verwendung des Übergangstyps Normal.
                                        •   Einlastung auf die bevorzugte Maschine.
                                        •   Pufferzeiten am Ende der Produktion.
                                        •   Verwendung des Übergangstyps Eil am Anfang der Produktion.
                                        Wenn aufgrund von Terminkonflikten, Überlastung, gesperrter Schichten o. ä.
                                        die Produktion vorgezogen werden muss, wird die ganze Bearbeitungskette
                                        vorgezogen.
                                        Als Ergebnis dieses Schrittes steht für jede Teilekette die Menge der günstigs-
                                        ten Lösungen für jeden Fertigstellungstermin der Folgestufe zur Verfügung.

                                        Auswahl der optimalen Lösung
                                        Die Einzellösungen der Teileketten werden mit den Übergangskosten zu den
                                        Folgeschritten so verbunden, dass für die ganze Stückliste das optimale Er-
                                        gebnis entsteht.
                                        Deshalb wird für jeden Starttermin eines VSG oder ISO die Menge der güns-
4.50 / 01-2023




                                        tigsten Lösungen aller Unterteile kombiniert und für jeden Fertigstellungster-
                                        min an die Folgestufe weitergegeben.




                 A+W Production Kapazitätsplanung                                                                E-19
                 Grundlagen                                                                     Tutorial




                              Rückmeldungen ins ERP-System
                              Die berechneten Zeit- und Personalkosten und der Materialverbrauch werden
                              in den Auftrag und die Lagerverwaltung des ERP-Systems gemeldet. In Ver-
                              bindung mit der ERP-Integration werden folgende Daten übermittelt:
                              •   Einlastungszustand.
                              •   Maschinen- und Personalkostenbestimmung.
                              •   Ermittlung des frühest möglichen Liefertermins.
                              •   Abfrage der Fahrtermine der Routenplanung.
                              •   Abfrage der Wareneingangstermine.
                              •   Dateilose Fertigmeldung über Webservices.
                              •   Online-Fortschrittsanzeige aus ERP über Webservices.
4.50 / 01-2023




                 E-20                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                   Planung und Einlastung




                                        Planung und Einlastung
                                        In diesem Themenblock finden Sie Informationen dazu, wie die eingelasteten
                                        Aufträge im Produktionsmonitor angezeigt und bearbeitet werden. Dazu kön-
                                        nen Sie fehlerhafte Einlastungen korrigieren und Produktionszeiten reservie-
                                        ren.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Produktionsmonitor” auf Seite E-22
                                        •   “Einlastung und Umlastung” auf Seite E-35
                                        •   “Kampagnenplanung” auf Seite E-44
                                        •   “Reservierungen” auf Seite E-54
                                        •   “Bearbeitungserzeugung” auf Seite E-63
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-21
                 Planung und Einlastung                                                                          Tutorial




                                            Produktionsmonitor
                                            Der Produktionsmonitor ist der zentrale Kapazitäts- und Auftrags-Leitstand
                                            und der Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlas-
                                            tung.
                                            Im Dialog Produktionsmonitor prüfen und bearbeiten Sie die Planung der Pro-
                                            duktion. Dabei wird die kapazitive Auslastung der Maschinen pro Arbeits-
                                            schicht angezeigt.




                     A                 B        C          D    E           F    G                     H
                 A   Angezeigte Maschinen                             E   Engpass
                 B   Arbeitsschicht pro Datum                         F   Deaktiviert
                 C   Einlastung                                       G   Reserviert für Eilaufträge
                 D   Arbeitsschicht verkürzt                          H   Undefinierte Bearbeitungen
                 Abb. E-5      Produktionsmonitor


                                            In diesem Beispiel sehen Sie, dass für die meisten Maschinen 2 Arbeits-
                                            schichten zur Verfügung stehen. Für einige Maschinen werden 3 Arbeits-
                                            schichten angezeigt und können bebucht werden. Diese Arbeitsschichten
                                            werden über die Stammdaten der Kapazitätsplanung eingerichtet und erzeugt.
4.50 / 01-2023




                                             “Stammdaten der Kapazitätsplanung” auf Seite E-68
                                            Die Aufträge werden unter dem Gesichtspunkt der Terminoptimierung einge-
                                            lastet. Dabei werden die Regeln von A+W Capacity Planner, die Zeiten der Ar-


                 E-22                                                                 A+W Production Kapazitätsplanung
                 Tutorial                                                                       Planung und Einlastung




                                        beitsschichten, die Sperrungen von Schichten, die definierten Engpässe und
                                        die (virtuellen) Kosten berücksichtigt.
                                        Wie die Einlastung im Einzelnen berechnet wird, ist in einer separaten Einheit
                                        beschrieben.
                                         “Terminoptimierung” auf Seite E-15
                                        In der Regel werden die Aufträge aus dem ERP-System automatisch einge-
                                        lastet. Sie werden den Arbeitsgängen (Bearbeitungen) entsprechend auf die
                                        Arbeitsschichten der Maschinen so eingelastet, dass der im Auftrag zugesag-
                                        te Liefertermin eingehalten wird. In besonderen Situationen müssen Sie in die-
                                        se Planung eingreifen:
                                        •   Aufträge auf andere Maschinen oder Termine verschieben.
                                             “Umlastungen” auf Seite E-37
                                             “Bearbeitungen umlasten” auf Seite E-39
                                        •   Fehlende Informationen aus den Aufträgen beheben.
                                             “Fehlerhafte Einlastung” auf Seite E-41
                                             “Eingelastete Aufträge nachbearbeiten” auf Seite E-42
                                             “Bearbeitungen erzeugen” auf Seite E-65
                                        •   Arbeitsschichten sperren, reservieren oder zusätzlich einrichten.
                                             “Kampagnenplanung” auf Seite E-44
                                             “Reservierungen” auf Seite E-54
                                        •   Fehlende Informationen aus den Aufträgen beheben.
                                             “Bearbeitungserzeugung” auf Seite E-63
                                        •   Auslastung tagesaktuell anpassen
                                             “Tagesaktuelle Anpassungen der Arbeitsschichten” auf Seite E-24
                                        •   Außerdem können Sie die farbliche Anzeige der Arbeitsschichten nach Ih-
                                            ren Vorstellungen einrichten.
                                             “Produktionsmonitor einrichten” auf Seite E-31
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-23
                 Planung und Einlastung                                                                          Tutorial




                                          Detailansicht




                 Abb. E-6   Produktionsmonitor – Detailansicht


                                          In der Detailansicht können Sie die Einlastungen einzelner Tage prüfen. Um
                                          die Einlastungen zu bearbeiten, müssen Sie zur Hauptansicht zurückwech-
                                          seln.


                                          Tagesaktuelle Anpassungen der Arbeitsschichten
                                          Die Arbeitsschichten im Produktionsmonitor werden aus den Stammdaten der
                                          Kapazitätsplanung erzeugt. Sie gelten jeweils für die zugeordneten Maschi-
                                          nen an bestimmten Wochentage und in einem definierten Zeitraum. Änderun-
                                          gen an den Stammdaten gelten daher unabhängig von den aktuellen
                                          Planungen.
                                          Sie können die Planung tagesaktuell steuern, indem Sie z. B. einzelne Ar-
                                          beitsschichten für eine Maschine hinzufügen, Maschinen deaktivieren, um sie
                                          von der Einlastung auszuschließen, die Planung entzerren, indem Sie Maschi-
                                          nen oder Arbeitsschichten als Engpass definieren.
                                          Um einzelne Arbeitsschichten auf die aktuellen Bedürfnisse der anfallenden
                                          Aufträge anzupassen, haben Sie folgende Möglichkeiten:
                                          •   “So erstellen Sie eine zusätzliche Arbeitsschicht” auf Seite E-25
                                          •   “So sperren Sie eine Arbeitsschicht vollständig” auf Seite E-26
4.50 / 01-2023




                                          •   “So reservieren Sie eine Arbeitsschicht” auf Seite E-27
                                          •   “So bearbeiten Sie die Arbeitszeit einer Arbeitsschicht” auf Seite E-27
                                          •   “So definieren Sie eine Arbeitsschicht als Engpass” auf Seite E-28


                 E-24                                                               A+W Production Kapazitätsplanung
                 Tutorial                                                                    Planung und Einlastung




                                        •   “So richten Sie die Arbeitsschichten einer Maschine ein” auf Seite E-29
                                        •   “So definieren Sie eine Maschine als Engpassbetriebsmittel” auf
                                            Seite E-30


                                         So erstellen Sie eine zusätzliche Arbeitsschicht

                                            Keine automatische Umlastung
                                            Wenn Sie im Produktionsmonitor eine zusätzliche Schicht einrichten, wer-
                                            den bereits eingelastete Aufträge nicht automatisch umgelastet.

                                        1 Wählen Sie A+W Production > Produktionsmonitor.
                                        2 Öffnen Sie das Kontextmenü zu der Maschine und dem Tag, an dem Sie
                                          die zusätzliche Arbeitsschicht benötigen.




                                        3 Wählen Sie den Eintrag Neue Schicht erstellen.




                                            A                                       B



                                            A Datum der Arbeitsschicht          B Uhrzeit der Arbeitsschicht


                                        4 Wählen Sie die Start- und Endzeit (B).
                                        5 Wählen Sie das Datum (A) der Start- und Endzeit.
                                            Das Enddatum einer Nachtschicht muss auf dem Folgetag liegen.
                                        6 Speichern Sie die Einstellung mit [OK].




                                            Die neue Arbeitsschicht wird im Produktionsmonitor angezeigt.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                               E-25
                 Planung und Einlastung                                                                      Tutorial




                                           So sperren Sie eine Arbeitsschicht vollständig
                                          1 Wählen Sie A+W Production > Produktionsmonitor.

                                                 A


                                                 B


                                             A Markierte Arbeitsschicht            B Kontextmenü
                                             Abb. E-7     Arbeitsschicht – Eigenschaften


                                          2 Markieren Sie die Arbeitsschicht (A), die Sie sperren wollen.
                                          3 Wählen Sie im Kontextmenü (B) Schichteigenschaften.




                                             A                                             B




                                             A Status der Arbeitsschicht           B Auswahl des Status


                                          4 Setzen Sie den Status auf Deaktiviert.
                                          5 Speichern Sie die Einstellung mit [OK].




                                             Die gesperrte Arbeitsschicht wird im Produktionsmonitor mit einem X ge-
                                             kennzeichnet.
4.50 / 01-2023




                 E-26                                                               A+W Production Kapazitätsplanung
                 Tutorial                                                                    Planung und Einlastung




                                         So reservieren Sie eine Arbeitsschicht
                                        1 Öffnen Sie den Dialog Schichteigenschaften wie in der vorausgehenden
                                          Handlungssequenz angezeigt.
                                        2 Setzen Sie den Status auf Aktiv für Eilaufträge.
                                        3 Speichern Sie die Einstellung mit [OK].




                                           Die reservierte Arbeitsschicht wird im Produktionsmonitor mit einem ! ge-
                                           kennzeichnet.


                                         So bearbeiten Sie die Arbeitszeit einer Arbeitsschicht
                                        1 Öffnen Sie den Dialog Schichteigenschaften wie in der vorausgehenden
                                          Handlungssequenz angezeigt.




                                           A                                           B




                                           A Kapazität der Arbeitsschicht       B Angabe der Dauer


                                        2 Tragen Sie die Dauer der Zeit in Stunden und Minuten ein.
                                        3 Speichern Sie die Einstellung mit [OK].




                                           Die Verkürzung der Arbeitsschicht wird im Produktionsmonitor schraffiert
                                           angezeigt.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-27
                 Planung und Einlastung                                                                            Tutorial




                                           So definieren Sie eine Arbeitsschicht als Engpass
                                          1 Öffnen Sie den Dialog Schichteigenschaften wie in der vorausgehenden
                                            Handlungssequenz angezeigt.




                                             A                                              B




                                             A Engpass                              B Änderung der Einstellung


                                          2 Ändern Sie die Einstellung für den Eintrag Engpass (A) auf Ja (B).
                                          3 Speichern Sie die Einstellung mit [OK].
                                             Die Einstellung gilt nur für die aktuelle Arbeitsschicht. Sie verhindert, dass
                                             die Arbeitsschicht über ihre Kapazität hinaus bebucht wird.

                                             Mehrere Arbeitsschichten auf Engpass setzen
                                             Sie können mehrere Arbeitsschichten markieren, indem Sie <Strg> ge-
                                             drückt halten und die Schichten markieren. Bei gedrückter <Strg>-Taste
                                             können Sie auch ein Rechteck über alle Schichten aufziehen, die markiert
                                             werden sollen. Anschließend können Sie alle markierten Schichten ge-
                                             meinsam als Engpass kennzeichnen.
4.50 / 01-2023




                 E-28                                                               A+W Production Kapazitätsplanung
                 Tutorial                                                                  Planung und Einlastung




                                         So richten Sie die Arbeitsschichten einer Maschine ein
                                        1 Öffnen Sie im Produktionsmonitor das Kontextmenü zu der gewünschten
                                          Maschine und wählen Sie Schichteigenschaften.




                                                                                      C


                                           A
                                           B




                                           A Nummer der Schicht                C Wochentage
                                           B Dauer der Arbeitsschicht
                                           Abb. E-8     Wochentage der Maschinenschicht


                                        2 Markieren Sie die Wochentage (C), an denen die Maschine in der Arbeits-
                                          schicht zur Verfügung steht.
                                        3 Geben Sie die Nummer (A) der Schicht an, auf die sich die Änderungen be-
                                          ziehen.
                                        4 Tragen Sie die Dauer (B) ein, in der die Maschine an den markierten Wo-
                                          chentagen zur Verfügung steht.
                                        5 Speichern Sie die Einstellung mit [OK].
                                        6 Aktualisieren Sie ggf. den Produktionsmonitor, damit die Änderungen der
                                          Maschinenschichten angezeigt werden.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-29
                 Planung und Einlastung                                                                           Tutorial




                                           So definieren Sie eine Maschine als Engpassbetriebsmittel
                                          1 Öffnen Sie im Produktionsmonitor das Kontextmenü zu der gewünschten
                                            Maschine und wählen Sie Eigenschaften.




                                             A                                             B




                                             A Engpass                             B Einstellung ändern


                                          2 Ändern Sie die Einstellung für den Eintrag Engpass (A) auf Ja (B).
                                             Die Einstellung gilt nur für die aktuelle Maschine und nur so lange, bis sie
                                             wieder manuell zurückgesetzt wird. Damit kann die Maschine nicht über
                                             ihre Kapazität hinaus bebucht werden.

                                             Enpassbetriebsmittel weit vorn im Prozess definieren
                                             Um die Produktion zu entzerren, müssen Engpassbetriebsmittel möglichst
                                             weit vorne im Produktionsablauf definiert werden. Diese Einstellung sollte
                                             möglichst schon zu Beginn der Inbetriebnahme des Produktionsmonitors
                                             über die Einstellung der angezeigten Maschinen festgelegt werden.

                                              “So zeigen Sie die Maschinen im Produktionsmonitor an” auf Seite E-31
4.50 / 01-2023




                 E-30                                                               A+W Production Kapazitätsplanung
                 Tutorial                                                                    Planung und Einlastung




                                        Produktionsmonitor einrichten
                                        Um die Anzeige auf die Bedürfnisse der Planung anzupassen haben Sie fol-
                                        gende Möglichkeiten:
                                        •   “So zeigen Sie die Maschinen im Produktionsmonitor an” auf Seite E-31
                                        •   “So stellen Sie die Anzeige der Farben ein” auf Seite E-32
                                        •   “So stellen Sie die Anzeigeart für alle Maschinen ein” auf Seite E-33
                                        •   “So stellen Sie die Anzeigeart für eine Maschine ein” auf Seite E-33


                                         So zeigen Sie die Maschinen im Produktionsmonitor an
                                        1 Wählen Sie A+W Production > Produktionsmonitor.
                                        2 Klicken Sie auf [Ausgewählte Maschinen].




                                            A




                                            B




                                            A Angezeigte Maschinen              B Maschinen werden nicht angezeigt
                                            Abb. E-9    Auswahl der Maschinen


                                            In diesem Dialog werden alle Maschinen aus der MZO aufgelistet. Die rote
                                            Schrift kennzeichnet Maschinen, die als Engpassbetriebsmittel definiert
                                            sind. Diese Maschinen können nicht über ihre Kapazität hinaus bebucht
                                            werden.
                                        3 Prüfen Sie, ob die Einstellungen als Engpassbetriebsmittel korrekt sind.
                                            Über das Kontextmenü zu einer Maschine können Sie die Einstellung än-
4.50 / 01-2023




                                            dern.
                                        4 Markieren Sie die Maschinen, die im Produktionsmonitor angezeigt wer-
                                          den sollen.


                 A+W Production Kapazitätsplanung                                                              E-31
                 Planung und Einlastung                                                                          Tutorial




                                          5 Speichern Sie die Einstellung mit [OK].
                                             Der Dialog wird geschlossen.
                                          6 Aktualisieren Sie ggf. den Produktionsmonitor, damit die Änderungen der
                                            Maschinen angezeigt werden.


                                           So stellen Sie die Anzeige der Farben ein
                                          1 Klicken Sie auf [Einstellungen].




                                                                                                  A

                                                                                                  B
                                                                                                  C




                                                                                                  D




                                             A Tage vor Startdatum                 C Angabe der Farbwerte (RGB)
                                             B Auswahl der Farbe                   D Auswahl aus Kombobox
                                             Abb. E-10    Einstellungen des Produktionsmonitors


                                          2 Legen Sie die Einstellungen fest, mit denen die Arbeitsschichten und Ein-
                                            lastungen im Produktionsmonitor angezeigt werden sollen, z. B.:
                                             •   Anzahl der Tage (A), die vor dem Startdatum angezeigt werden.
                                             •   Farbe (B, C), in der die Zeiten angezeigt werden, z. B. belegte Zeiten,
                                                 Reservierungen.
                                             •   Angabe (D), ob bestimmte Informationen angezeigt werden, z. B. die
                                                 Zeit, verplante Arbeitsgänge.
                                          3 Speichern Sie die Einstellungen mit [OK].
4.50 / 01-2023




                                             Der Dialog wird geschlossen.




                 E-32                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                                   Planung und Einlastung




                                        4 Aktualisieren Sie ggf. den Produktionsmonitor, damit die Änderungen der
                                          Maschinen angezeigt werden.


                                         So stellen Sie die Anzeigeart für alle Maschinen ein
                                        1 Klicken Sie auf [Anzeigeart für alle Maschinen ändern].




                                        2 Wählen Sie, mit welchen Werten die Einlastungen im Produktionsmonitor
                                          angezeigt werden sollen.
                                        3 Speichern Sie die Einstellung mit [OK].
                                           Der Dialog wird geschlossen.
                                        4 Aktualisieren Sie die ggf. den Produktionsmonitor, damit die Änderungen
                                          der Maschinen angezeigt werden.


                                         So stellen Sie die Anzeigeart für eine Maschine ein
                                        1 Öffnen Sie im Produktionsmonitor das Kontextmenü zu der gewünschten
                                          Maschine.




                                                                                      B

                                           A




                                           A Logische Maschine                 B Anzeigeart der Maschine


                                        2 Legen Sie fest, ob für die Maschine auch die zugeordneten Logischen Ma-
                                          schinen (A) angezeigt werden.
                                        3 Wählen Sie, mit welchen Werten (B) die Einlastungen der Maschine ange-
                                          zeigt werden sollen.
4.50 / 01-2023




                                        4 Speichern Sie die Einstellung mit [OK].
                                           Der Dialog wird geschlossen.


                 A+W Production Kapazitätsplanung                                                            E-33
                 Planung und Einlastung                                                                        Tutorial




                                          5 Aktualisieren Sie die ggf. den Produktionsmonitor, damit die Änderungen
                                            der Maschinen angezeigt werden.


                                          Arbeitsplan exportieren




                                          Abb. E-11   Arbeitsplan exportieren


                                          Haben Sie im Produktionsmonitor den Arbeitsplan über das Kontextmenü ge-
                                          öffnet, können Sie die Daten in eine CSV-Datei exportieren. Markieren Sie die
                                          gewüschten Einträge und öffnen Sie das Menü Anzeigen. Dort wählen Sie Ex-
                                          portieren aus. Es öffnet sich der Dialog Speichern unter ... Geben Sie einen
                                          entsprechenden Namen ein un klicken Sie auf [Speichern].
4.50 / 01-2023




                 E-34                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                                          Planung und Einlastung




                                       Einlastung und Umlastung
                                        Lernziele

                                        • Was ist die Einlastung und wie werden Aufträge eingelastet?
                                        • Wie können Sie auf Probleme während der Einlastung reagieren?
                                        • Was ist die Umlastung und wie wird umgelastet?


                                        Nutzen

                                        • Mit der Einlastung werden Auftragsdaten und Angebotsdaten, die vom ERP-
                                          System übergeben wurden, aufbereitet und kalkuliert. So werden gültige Termine
                                          errechnet und produktionsrelevante Restriktionen geprüft, um die effiziente
                                          Produktion des Auftrags zu gewährleisten.
                                        • Mit der Umlastung können Sie durchzuführende Bearbeitungen auf andere
                                          Termine und Maschinen buchen.


                                        Merke

                                        Einlastung                 Die Einlastung ist der Prozess der Datenaufbereitung
                                                                   und Kalkulation, nachdem ein Auftrag oder Angebot vom
                                                                   ERP-System übergeben wurde.
                                                                   Die Aufträge oder Angebote werden in der Regel
                                                                   automatisch eingelastet.
                                                                   Sie können eine fehlgeschlagene Einlastung
                                                                   nachbearbeiten.

                                        Engpassbetriebsmittel      Ein Engpassbetriebsmittel kann nicht über seine
                                                                   Kapazität hinaus bebucht werden.

                                        Terminfindung              Die Terminfindung steigt über die Selektion von
                                                                   Bearbeitungen ein.
                                                                   Die Zieltermine sind verbindlich. Sie werden wie
                                                                   Bearbeitungen mit einem einzigen Kampagnentermin
                                                                   behandelt.
                                                                   Liefertermine sind geschützt – Ausnahme: die
                                                                   Bearbeitung Versenden kann verschoben werden.

                                        Bearbeitungssequenzen      Die aufsteigenden Bearbeitungssequenzen geben die
                                                                   Reihenfolge der Bearbeitungen an.

                                        Umlastungsmodus            Möglichkeiten zur Umlastung:
                                                                   •   Ganze Stückliste.
                                                                   •   Nur Vorgängerbearbeitung.
                                                                   •   Nur Nachfolgerbearbeitung
                                                                   •   Einzelne Bearbeitung.
                                                                   Umlastungsmodus und -richtung sind unabhängig.
                                                                   Unbeteiligte Bearbeitungen sind von der Terminfindung
                                                                   ausgenommen.

                                        Aufträge umlasten          • Terminumlastung:
                                                                     Aufträge werden auf andere Termine verschoben.
4.50 / 01-2023




                                                                   • Maschinenumlastung:
                                                                     Aufträge werden auf anderen Maschinen produziert
                                                                     als ursprünglich geplant.



                 A+W Production Kapazitätsplanung                                                                    E-35
                 Planung und Einlastung                                                                          Tutorial




                                          Aufträge einlasten
                                          In der Regel ist in A+W Production die automatische Einlastung der Aufträge
                                          eingerichtet. Der Datenimport läuft als Hintergrundprozess. Sie können den
                                          Prozess der Einlastung über den A+W ServiceMonitor verfolgen. Manuelle
                                          Eingriffe sind nur erforderlich, wenn einzelne Aufträge oder Auftragspositionen
                                          nicht eingelastet werden konnten. Die Bearbeitung dieser Aufträge ist in einer
                                          separaten Einheit beschrieben.
                                           “Fehlerhafte Einlastung” auf Seite E-41
                                          Die eingelasteten Aufträge, die noch nicht weiter verarbeitet sind, können Sie
                                          im Dialog Aufträge prüfen und bearbeiten. Dieses Thema ist im Part Grobpla-
                                          nung beschrieben.
                                          Wenn in A+W Production eine manuelle Einlastung eingerichtet ist, müssen
                                          Sie den Dialog Einlastung verwenden. Nach erfolgreicher Einlastung wird im
                                          Feld Status die aktuelle Uhrzeit angezeigt.




                                          Abb. E-12    Einlastung


                                          Die Einlastung wird in A+W Production so lange berechnet, bis eine Lösung
                                          gefunden ist, die den Einlastungsregeln entspricht. Wenn keine akzeptable
                                          Lösung gefunden wurde, müssen Sie die Einlastung manuell steuern.Dazu
                                          können u. a. große Positionen gesplittet werden. Der Positionssplit ist aus-
                                          führlich im Part Grobplanung beschrieben.

                                             Einstellungen der Datenübergabe
                                             Klären Sie mit dem Kundenservice der A+W Software GmbH, wie die Ein-
                                             stellungen der Datenübergabe vom ERP-System an A+W Production ge-
                                             setzt sind.
4.50 / 01-2023




                 E-36                                                                 A+W Production Kapazitätsplanung
                 Tutorial                                                                   Planung und Einlastung




                                        Umlastungen
                                        Sie können Aufträge umlasten, wenn die Produktion nicht so durchlaufen wer-
                                        den kann, wie es ursprünglich geplant war. Dabei können Sie entweder eine
                                        andere Maschine auswählen oder die Bearbeitung auf einen anderen Termin
                                        verschieben.
                                        •   Die Terminfindung steigt über die Selektion von Bearbeitungen ein.
                                        •   Mit den verschiedenen Umlastungsmodi haben Sie folgende Möglichkeiten
                                            zur Umlastung:
                                            Ganze Stückliste, nur Vorgänger, nur Nachfolger, einzelne Bearbeitung.
                                        •   Die Zieltermine sind verbindlich:
                                            Die Zieltermine werden zugewiesen und verriegelt. Sie werden wie Bear-
                                            beitungen mit einem einzigen Kampagnentermin behandelt.
                                        •   Liefertermine sind geschützt:
                                            Dies gilt nicht für die Bearbeitung Versenden.
                                        •   Umlastungsmodus und -richtung sind unabhängig:
                                            Unbeteiligte Bearbeitungen werden von der Terminfindung ausgenommen.
                                            Wenn durch die Umlastung eine ungültige Bearbeitungsreihenfolge entste-
                                            hen würde, werden alle Nachfolger mit umgelastet, wenn dadurch ein gül-
                                            tiges Ergebnis erreicht wird.
                                            Eine ungültige Umlastung wäre z. B. die Umlastung Nur Vorgänger in Rich-
                                            tung später als die Nachfolger.

                                        Maschinenumlastung
                                        Bei einer Maschinenumlastung wird die Produktion eines Auftrags auf andere
                                        Maschinen verschoben. Das kann z. B. erforderlich sein, wenn eine Maschine
                                        wegen Reparaturen ausfällt.




                                        A
                                                                                       B




                                        A Aktuell eingelastete Maschinen      B Verfügbare Maschinen
                                        Abb. E-13    Maschinenumlastung
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-37
                 Planung und Einlastung                                                                           Tutorial




                                          Bearbeitungsumlastung
                                          Bei der Umlastung eines Produktionstermins wird eine Bearbeitung auf einen
                                          anderen Termin verschoben, damit der Auftrag früher oder später fertig wird.
                                          Das kann z. B. erforderlich sein, wenn sich die Priorität eines Auftrags ändert.




                 A


                                                                                                                         D




                 B




                                                                   C
                 A Bearbeitungen                                       C Umlastungsmodus
                 B Termin- und Maschinenauswahl                        D Vorgaben für die Terminfindung
                 Abb. E-14   Terminumlastung


                                          Sie können eine Bearbeitung (A) auf einen anderen Termin (B) oder auf eine
                                          andere Maschinen umlasten. Dazu können Sie angeben, wie die Übergangs-
                                          zeiten (D) berücksichtigt werden sollen. Die durch eine Umlastung neu be-
                                          rechneten Termine können anschließend gesperrt werden. Damit sind sie vor
                                          einer weiteren Umlastung geschützt.
                                          Bei der Umlastung stehen folgende Modi (C) zur Verfügung:
                                          •    Komplette Stückliste umlasten:
                                               Die komplette Stückliste, zu der die Bearbeitung gehört, wird umgelastet.
                                          •    Nur markierte Bearbeitung:
                                               Nur die markierte Bearbeitung wird umgelastet.
                                          •    Markierte und alle folgenden Bearbeitungen:
4.50 / 01-2023




                                               Die markierte und alle nachfolgenden Bearbeitungen der Scheibe werden
                                               umgelastet.




                 E-38                                                                 A+W Production Kapazitätsplanung
                 Tutorial                                                                        Planung und Einlastung




                                          •       Markierte und alle vorherigen Bearbeitungen:
                                                  Die markierte und alle vorherigen Bearbeitungen der Scheibe werden um-
                                                  gelastet.
                                          •       Unbedingte Terminzuweisung für markierte Bearbeitung:
                                                  Für die markierte Bearbeitung wird die Umlastung zum gewählten Termin
                                                  erzwungen, Maschinenkapazitäten werden dabei nicht berücksichtigt.
                                          Bei allen Modi bleiben Versand- und Liefertermin unverändert, sofern Sie die-
                                          sen nicht explizit umlasten. Wenn Sie die Verschiebung des Liefertermins (D)
                                          zulassen, sollten Sie den neuen Liefertermin auch an das ERP-System zu-
                                          rücksenden.


                                          Bearbeitungen umlasten
                                          In dieser Lerneinheit erfahren Sie, wie Sie die Bearbeitungen auf einen ande-
                                          ren Termin verschieben.


                                           So lasten Sie eine Bearbeitung um
                                          1 Wählen Sie Anzeigen > Aufträge > Kontextmenü auf markierte Aufträge >
                                            Bearbeitungen > Kontextmenü auf markierte Bearbeitungen > Arbeitsplan
                                            > Umlastung.


                                                                                           E




                 A




                 B




                                              C          D
                 A Bearbeitungen                                       C Reservierung
                 B Verfügbare Maschinen für die ausgewählte            D Modus
4.50 / 01-2023




                   Bearbeitung                                         E Zeitraster
                 Abb. E-15   Termin umlasten



                 A+W Production Kapazitätsplanung                                                                 E-39
                 Planung und Einlastung                                                                        Tutorial




                                          2 Wählen Sie die Bearbeitungen (A) aus, die Sie umlasten wollen.
                                             Wenn Sie mehrere Bearbeitungen auswählen, können Sie nur den Termin
                                             verschieben.
                                          3 Wählen Sie die Einstellung für die Einlastung (E):
                                             •   Einlastung erzwingen:
                                                 Mit dieser Einstellung werden die Kapazitätsgrenzen von Engpassbe-
                                                 triebsmitteln nicht berücksichtigt. Daher werden die Arbeitsschichten
                                                 ggf. überbucht.
                                             •   Erlaube Eilraster:
                                                 Zur Umlastung werden die Übergangszeiten vom Typ Eil verwendet.
                                             •   Als Chefauftrag einlasten:
                                                 Die Bearbeitung wird mit den minimalen Übergangszeiten umgelastet.
                                                 Achtung: Dabei können auch die Zeiten von Kampagnen genutzt wer-
                                                 den. Verwenden Sie diese Einstellung nur in Notfällen.
                                          4 Markieren Sie die Schicht, in der die Bearbeitung eingelastet werden soll.




                                          5 Wählen Sie den Modus (D) der Umlastung.
                                             Die Schaltfläche zum Start der Umlastung wird freigeschaltet.
                                          6 Klicken Sie auf [Umlasten], um die Umlastung zu starten.
                                             Die Zeiten werden neu berechnet. Das Ergebnis wird in einem Dialog an-
                                             gezeigt. Wenn die Umlastung nicht erfolgreich war, müssen Sie die Bedin-
                                             gungen ändern und die Umlastung erneut versuchen.
4.50 / 01-2023




                 E-40                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                                         Planung und Einlastung




                                           Fehlerhafte Einlastung
                                           Die Einlastung von Aufträgen kann aus unterschiedlichen Gründen fehlschla-
                                           gen, z. B. in folgenden Fällen:
                                           •   Artikel in Aufträgen sind nicht definiert.
                                           •   Produktionsartikel in Aufträgen sind nicht definiert.
                                           •   Bearbeitungen in Aufträgen sind nicht definiert.
                                           •   Auftragsdaten sind fehlerhaft.
                                           •   Schichtrestriktionen können nicht eingehalten werden.
                                           •   Schichten sind nicht vorhanden, weil z. B. Schichtpläne ausgelaufen sind.
                                           Diese Aufträge können Sie nachbearbeiten und dann die Einlastung wieder-
                                           holen.




                 A




                 B




                 A Fehlerhafte Aufträge                              B Auswahlkriterien für die Anzeige
                 Abb. E-16    Fehlerhafte Einlastungen


                                           Zum Filtern der Aufträge können Sie eine der möglichen Fehlerursachen (B)
                                           auswählen. Die Anzeige der entsprechenden Aufträge (A) wird automatisch
                                           aktualisiert. Pro Auftrag können Sie wählen, wie mit den Aufträgen verfahren
                                           wird. Dazu stehen Ihnen z. B. folgende Optionen zur Verfügung:
                                           •   Erneute Datenübernahme:
                                               Die Auftragsdaten werden erneut und unverändert eingelastet. Dazu müs-
                                               sen Sie Stammdaten korrigieren, z. B. Schichtpläne verlängern, und da-
                                               nach ohne erneute Übergabe der Daten vom ERP-System einlasten.
                                           •   Einlastung erzwingen:
                                               Die Einlastung wird erzwungen. Dabei wird die Kapazität von Engpassbe-
                                               triebsmitteln nicht berücksichtigt. Daher werden die Arbeitsschichten ggf.
4.50 / 01-2023




                                               überbucht.
                                           •   Einlastung ignorieren:
                                               Die Produktionstermine werden ermittelt ohne Rücksicht auf Übergangs-



                 A+W Production Kapazitätsplanung                                                                  E-41
                 Planung und Einlastung                                                                            Tutorial




                                               zeiten, Kapazitätsgrenzen und Kampagnentermine. Alle anderen Aufträge
                                               und deren Liefertermine rücken nach hinten.
                                           •   Löschung der fehlerhaften Aufträge:
                                               Die entsprechenden Aufträge werden gelöscht. Sprechen Sie sich mit Ih-
                                               ren Kollegen aus der Auftragserfassung ab, damit die Aufträge korrigiert
                                               und erneut an A+W Production übergeben werden.
                                           •   Ermittelten Liefertermin bestätigen:
                                               Der von A+W Production vorgeschlagene Liefertermin wird akzeptiert. Der
                                               neue Liefertermin wird an das ERP-System zurückgemeldet.


                                           Eingelastete Aufträge nachbearbeiten
                                           In dieser Lerneinheit erfahren Sie, wie Sie die Aufträge, die nicht eingelastet
                                           werden konnten, manuell nachbearbeiten.


                                            So bearbeiten Sie eine Einlastung nach
                                           1 Wählen Sie Stammdaten > Nachbearbeitung Einlastung.




                 A




                                                                                                         C



                 B




                 A Liste der Aufträge                                  C Anzeigen nach
                 B Auswahlkriterien
                 Abb. E-17    Nachbearbeitung von fehlerhaften Einlastungen


                                           2 Wählen Sie das Filterkriterium (B) für die Anzeige der Aufträge und die Sor-
                                             tierung (C) aus.
                                               Die Liste der Aufträge wird gefiltert.
                                           3 Markieren Sie den Auftrag (A), den Sie bearbeiten wollen.
                                           4 Klicken Sie auf [Bearbeiten].
4.50 / 01-2023




                 E-42                                                                   A+W Production Kapazitätsplanung
                 Tutorial                                                                       Planung und Einlastung




                                           Abhängig vom Filterkriterium haben Sie folgende Möglichkeiten:
                                           •   Wenn Sie Artikel ändern müssen, wird der Dialog für die entsprechen-
                                               den Stammdaten geöffnet. Beheben Sie den Fehler und lasten Sie den
                                               Auftrag erneut ein.
                                           •   Bei den anderen Fehlern wird einer der folgenden Dialoge geöffnet:




                                        Abb. E-18    Fehlerhafte Aufträge und Änderung bereits verplanter Aufträge


                                        5 Wählen Sie die Option, mit der Sie den Fehler beheben können.
                                           Eine Beschreibung der Optionen finden Sie in der Softwarereferenz.
                                            Softwarereferenz, “Fehlerhafte Aufträge” auf Seite E-182
                                            Softwarereferenz, “Asynchrone Verarbeitung” auf Seite E-183
                                            Softwarereferenz, “Änderung bereits verplanter Aufträge” auf Seite E-184
                                        6 Klicken Sie auf [OK], um die Änderungen zu übernehmen.
                                           Der Auftrag wird der gewählten Option entsprechend behandelt.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                    E-43
                 Planung und Einlastung                                                                               Tutorial




                                          Kampagnenplanung
                                          Lernziele

                                          •   Was sind Kampagnen?
                                          •   Wie werden Kampagnen angelegt, bearbeitet oder gelöscht?
                                          •   Was sind Einzeltermine?
                                          •   Was sind Wöchentliche Termine?


                                          Nutzen

                                          • Kampagnen sind Arbeitsgänge, die nur an bestimmten Tagen in bestimmten
                                            Schichten durchgeführt werden, z. B. blauer Siebdruck immer freitags in Schicht 2.


                                          Merke

                                          Kampagnen                   Kampagnen helfen Ihnen, gezielt Aufträge für Kunden
                                                                      oder Objekte abzuarbeiten und termingerecht zu planen.
                                                                      Kampagnen sind feste wiederkehrende Termine für
                                                                      bestimmte Arbeitsgänge, die weitgehend unantastbar
                                                                      sind. Sie können allenfalls durch „Chefaufträge“ oder im
                                                                      Umlastungseditor durch Terminzuweisungen übersteuert
                                                                      werden.

                                          Einzeltermine               Einzeltermine sind Kampagnen, die einmalig
                                                                      durchgeführt werden.

                                          Wöchentliche Termine        Wöchentliche Termine sind Kampagnen, die regelmäßig
                                                                      durchgeführt werden.

                                              Voraussetzung
                                              Um Kampagnen anzulegen, müssen die entsprechenden Arbeitsgänge
                                              und Schichten definiert und der entsprechende Schichtplan aktiv sein.

                                               “Schichten” auf Seite E-69
4.50 / 01-2023




                 E-44                                                                 A+W Production Kapazitätsplanung
                 Tutorial                                                                       Planung und Einlastung




                                          Definition der Kampagnen
                                          Kampagnen dienen vor allem dazu, ein Betriebsmittel richtig einzurichten,
                                          z. B. für Beschichtungen, die lange Rüstzeiten erfordern. Das bedeutet, dass
                                          das Betriebsmittel in unterschiedlichen Modi gefahren wird.
                                          Mit Kampagnen können Sie für bestimmte Arbeitsgänge Kapazitäten einpla-
                                          nen, z. B. für Siebdruck für jeden Wochentag eine andere Farbe. Daraus wür-
                                          den sich z. B. die Kampagnen Blau am Montag oder Grün am Dienstag
                                          ergeben. Der Vorteil dabei ist, dass der Siebdruck jeweils für einen kompletten
                                          Tag nur in einer Farbe betrieben wird und die Reinigungs- und Umrüstarbeiten
                                          minimiert werden.
                                          Kampagnen können aber auch so eingerichtet werden, dass bestimmte Ar-
                                          beitsgänge in einer bestimmten Schicht gemacht werden, z. B. der gesamte
                                          Zuschnitt von Sondergläsern in der ersten Schicht.
                                          Die für eine Kampagne reservierte Zeit kann nur von Chefaufträgen übersteu-
                                          ert werden.




                                                                                                             E


                 A




                 B




                                      C             D
                 A Arbeitsgang der Kampagne                         C Verfügbare Schichten
                 B Tag der Kampagne                                 D Tag der geplanten Kampagne
                                                                    E Aktivierte Kampagne
                 Abb. E-19   Kampagnen
4.50 / 01-2023




                                          Eine Kampagne gilt immer für einen bestimmten Arbeitsgang (A). Sie wird ent-
                                          weder als Einzeltermin oder als wöchentlicher Termin an einem bestimmten


                 A+W Production Kapazitätsplanung                                                                  E-45
                 Planung und Einlastung                                                                              Tutorial




                                          Wochentag (B) festgelegt. Wenn an dem Tag mehrere Schichten (C) zur Ver-
                                          fügung stehen, müssen die jeweiligen Schichten angegeben werden.
                                          Kampagnen werden ausschließlich für Arbeitsgänge erzeugt. Die Maschine,
                                          an der die Bearbeitung stattfindet, spielt dabei keine Rolle.
                                          Dafür dürfen die Arbeitsgänge nicht an eine bestimmte Maschine gebunden
                                          sein.

                                             Beispiel

                                             Wenn zwei unterschiedliche Siebdrucke definiert sind, muss bei der
                                             Einlastung erkannt werden, welcher der beiden Siebdrucke vorliegt. Dabei
                                             spielt es keine Rolle, auf welcher Maschine der Siebdruck gemacht wird.
                                             Ein Arbeitsgang Siebdruck für Kampagne X muss in der MZO also so
                                             eingerichtet werden, dass er nur für Kampagnen verwendet wird. Dieser
                                             Arbeitsgang muss der logischen Maschine zugeordnet sein, auf der die
                                             Kampagnen gefahren werden.
4.50 / 01-2023




                 E-46                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                           Planung und Einlastung




                                        Kampagnen in der Terminfindung
                                        Bei der Terminfindung für Kampagnen werden alle Termine ausgeblendet, für
                                        die der Arbeitsgang nicht zutrifft.


                                                       Montag         Dienstag          Mittwoch      Donnerstag




                                        A



                                                           B    C            D      E
                                        A Ausgeblendete Arbeitsschichten          D Flexible Übergangszeit
                                        B Flexible Übergangszeit                  E Optimale Lösung
                                        C Zweite Kampagne der Stückliste
                                        Abb. E-20     Terminfindung für Kampagnen


                                        In diesem Beispiel sehen Sie, dass die optimale Lösung (E) einen Übergang
                                        von jeweils einer Schicht hat. Wenn die Terminfindung kein Ergebnis findet,
                                        wird geprüft, ob es eine Lösung gibt, wenn Kampagnentermine ignoriert wer-
                                        den. Eine entsprechende Meldung weist im Bedarfsfall darauf hin, dass Kam-
                                        pagnentermine fehlen.
                                        Arbeitsgänge mit Kampagnen erhalten automatisch eine flexible Übergangs-
                                        zeit am Eingang. Wenn in der Stückliste mehrere Kampagnen (C) sind, dann
                                        sucht das System nach früheren Startterminen (B, D), um Konflikte zu vermei-
                                        den.


                                        Kampagnen anlegen und verwalten
                                        In dieser Lerneinheit lernen Sie, wie Sie Kampagnen anlegen, bearbeiten oder
                                        löschen.
                                        Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                        •   “So legen Sie eine Kampagne als Einzeltermin an” auf Seite E-48
                                        •   “So legen Sie eine Kampagne als wöchentlichen Termin an” auf Seite E-50
                                        •   “So bearbeiten Sie eine Kampagne” auf Seite E-52
                                        •   “So löschen Sie eine Kampagne” auf Seite E-53

                                            Voraussetzung
4.50 / 01-2023




                                            Um Kampagnen anzulegen, müssen die entsprechenden Arbeitsgänge
                                            und Schichten definiert und der entsprechende Schichtplan aktiv sein.

                                             “So erstellen Sie einen Schichtplan” auf Seite E-76


                 A+W Production Kapazitätsplanung                                                                    E-47
                 Planung und Einlastung                                                                         Tutorial




                                           So legen Sie eine Kampagne als Einzeltermin an

                                              Voraussetzung
                                              Im Register Einzeltermine werden nur aktivierte Schichtpläne angezeigt.
                                              Aktivieren Sie ggf. die Schichtpläne, die für die Kampagne benötigt wer-
                                              den.

                                          1 Wählen Sie Stammdaten > Kapazitätsplanung > Kampagnenplanung.




                                          A




                                          B




                                          C




                                          A Arbeitsgang                          C Dauer der Kampagne
                                          B Datum der Kampagne
                                          Abb. E-21    Kampagne anlegen


                                          2 Markieren Sie den Arbeitsgang (A) für die Kampagne.
                                              Die Schaltflächen werden freigeschaltet.
                                          3 Klicken Sie auf den Pfeil nach rechts.
                                              Der Arbeitsgang wird im Feld Kampagnen angezeigt.
                                          4 Markieren Sie im Feld Kampagnen die Checkbox des Arbeitsgangs.
                                              Das Register Einzeltermine wird freigeschaltet.
                                          5 Markieren Sie im Kalender das Datum (B) für die Kampagne.
                                              Im Feld Verfügbare Schichten werden die Schichten angezeigt, die für die-
4.50 / 01-2023




                                              ses Datum zur Verfügung stehen.




                 E-48                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                          Planung und Einlastung




                                        6 Markieren Sie die Schicht, in der die Kampagne durchgeführt werden soll.
                                           Wenn die Schichten nicht angezeigt werden, müssen Sie in der entspre-
                                           chenden Schichtregel prüfen, ob die Wochentage markiert sind, an denen
                                           die Schicht zur Verfügung steht.
                                            “So erstellen Sie eine Schichtregel” auf Seite E-79
                                        7 Geben Sie an, wie viele Tage oder Wochen (B) die Kampagne andauern
                                          soll.
                                        8 Klicken Sie auf [+].
                                           Die neue Kampagne wird im Feld Einzeltermine angezeigt. Wenn die Kam-
                                           pagne über mehrere Schichten durchgehen soll, wiederholen Sie die
                                           Schritte 6 - 8 für jede einzelne Schicht.




                                        9 Klicken Sie auf [OK], um die Kampagne zu speichern.
                                           Die Kampagne wird gespeichert und der Dialog wird geschlossen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                   E-49
                 Planung und Einlastung                                                                        Tutorial




                                           So legen Sie eine Kampagne als wöchentlichen Termin an

                                              Voraussetzung
                                              Im Register Wöchentliche Termine werden nur aktivierte Schichtpläne an-
                                              gezeigt. Aktivieren Sie ggf. die Schichtpläne, die für die Kampagne benö-
                                              tigt werden.

                                          1 Wählen Sie Stammdaten > Kapazitätsplanung > Kampagnenplanung.




                                          A




                                          B




                                          C




                                          A Arbeitsgang                          C Dauer der Kampagne
                                          B Datum der Kampagne
                                          Abb. E-22    Kampagnen anlegen


                                          2 Markieren Sie den Arbeitsgang für die Kampagne.
                                              Die Schaltflächen werden freigeschaltet.
                                          3 Klicken Sie auf den Pfeil nach rechts.
                                              Der Arbeitsgang wird im Feld Kampagnen angezeigt.
                                          4 Markieren Sie im Feld Kampagnen die Checkbox des Arbeitsgangs.
                                              Das Register Wöchentliche Termine wird freigeschaltet.
4.50 / 01-2023




                 E-50                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                    Planung und Einlastung




                                        5 Wechseln Sie zum Register Wöchentliche Termine.




                                        A
                                        B




                                        A Kampagnentage                       B Schichten
                                            Abb. E-23   Wöchentliche Kampagnen


                                        6 Markieren Sie im Kalender den Wochentag (A) für die Kampagne.
                                            Im Feld Verfügbare Schichten werden die Schichten angezeigt, die für die-
                                            sen Wochentag zur Verfügung stehen.
                                        7 Markieren Sie die Schicht, in der die Kampagne durchgeführt werden soll.
                                        8 Klicken Sie auf [+].




                                            Die neue Kampagne wird im Feld Wöchentliche Termine angezeigt. Wenn
                                            die Kampagne über mehrere Schichten durchgehen soll, wiederholen Sie
                                            die Schritte 6 - 8 für jede einzelne Schicht.
                                        9 Klicken Sie auf [OK], um die Kampagne zu speichern.
                                            Die Kampagne wird gespeichert und der Dialog wird geschlossen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-51
                 Planung und Einlastung                                                                       Tutorial




                                           So bearbeiten Sie eine Kampagne
                                          1 Wählen Sie Stammdaten > Kapazitätsplanung > Kampagnenplanung.
                                          2 Markieren Sie im Feld Kampagnen die Kampagne, die Sie ändern wollen.
                                             In den Registern Einzeltermine bzw. Wöchentliche Termine werden die
                                             Termine angezeigt, zu denen Kampagnen erstellt sind.




                                             Abb. E-24    Kampagne bearbeiten


                                          3 Markieren Sie den Termin, den Sie ändern wollen.
                                          4 Klicken Sie auf [Löschen].
                                             Der Termin wird gelöscht.
                                          5 Wählen Sie einen neuen Termin oder Wochentag und die Schicht.
                                          6 Klicken Sie auf [+].
                                             Der neue Termin wird angezeigt.
                                          7 Klicken Sie auf [OK], um die Änderungen zu speichern.
                                             Die Änderung wird gespeichert und der Dialog wird geschlossen.
4.50 / 01-2023




                 E-52                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                                    Planung und Einlastung




                                         So deaktivieren Sie eine Kampagne
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Kampagnenplanung.
                                        2 Markieren Sie im Feld Kampagnen die Checkbox der Kampagne, die Sie
                                          deaktivieren wollen.
                                            Die Felder werden gesperrt.
                                        3 Klicken Sie auf [OK], um die Änderungen zu speichern.
                                            Die Änderung wird gespeichert und der Dialog wird geschlossen.
                                            Die Kampagne wird nicht in die Kapazitätsplanung einbezogen. Die Kam-
                                            pagne behält alle ihre Eigenschaften. Damit können Sie Kampagnen kurz-
                                            fristig an und aus schalten.


                                         So löschen Sie eine Kampagne
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Kampagnenplanung.
                                        2 Markieren Sie die Kampagne, die Sie löschen wollen.
                                        3 Klicken Sie auf den Pfeil nach links.
                                            Die Kampagne wird mit allen zugehörigen Terminen gelöscht.
                                        4 Klicken Sie auf [OK], um die Änderungen zu speichern.
                                            Die Änderung wird gespeichert und der Dialog wird geschlossen.


                                        Übungen zu Kampagnen
                                        Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Ver-
                                        fügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung
                                        vollständig sind, können Sie die Planung für eigene Aufträge im Produktions-
                                        monitor testen.
                                        •   Überlegen Sie, welche Arbeitsgänge Ihrer Produktion als Kampagne orga-
                                            nisiert werden sollten.
                                        •   Was ist für diese Arbeitsgänge sinnvoller: eine Kampagne als Einzeltermin
                                            oder eine Kampagne als wöchentlicher Termin?
                                        •   Legen Sie die entsprechenden Kampagnen an.
                                        •   Bearbeiten Sie einzelne Kampagnen.
                                        •   Löschen Sie Termine von Kampagnen.
                                        •   Löschen Sie Kampagnen.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Kampagnen” auf Seite E-188
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-53
                 Planung und Einlastung                                                                             Tutorial




                                          Reservierungen
                                          Lernziele

                                          • Was sind Reservierungen?
                                          • Wie werden Reservierungen angelegt, bearbeitet oder gelöscht?


                                          Nutzen

                                          • Mit Reservierungen können Sie Kapazitäten für Kunden oder Objekte freihalten.


                                          Merke

                                                                     Reservierungen können nur für Engpassbetriebsmittel
                                                                     angelegt werden.

                                                                     Reservierungen werden für Kunden und Objekte
                                                                     eingerichtet.

                                             Voraussetzung
                                             Sie können Reservierungen nur für Maschinen anlegen, die als Engpass-
                                             Betriebsmittel definiert sind.

                                             Reservierungen in Schichten, Tagen oder Wochen
                                             In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstel-
                                             lung unter Stammdaten > Konfiguration > A+W Production > Kapazitätspla-
                                             nung > Art der Reservierung kann die Reservierung aber auch für Tage
                                             oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung än-
                                             dern, gehen die alten Reservierungen verloren.
4.50 / 01-2023




                 E-54                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                        Planung und Einlastung




                                        Reservierung von Kapazitäten
                                        Für einzelne Kunden oder Objekte können Sie Kapazitäten einer bestimmten
                                        Maschine reservieren. In der Regel reservieren Sie die Kapazität über die ge-
                                        samte Woche, so dass Sie unabhängig davon sind, wann der Auftrag eintrifft.
                                        Damit werden Kapazitäten freigehalten, damit die Aufträge ohne Verzug durch
                                        die Engpässe geschleust werden können. Kapazitäten können daher nur für
                                        die Arbeitsgänge und Maschinen reserviert werden, bei denen Engpässe ent-
                                        stehen können und die daher als Engpassbetriebsmittel definiert sind.
                                         “So definieren Sie eine Maschine als Engpassbetriebsmittel” auf Seite E-30.

                                            Reservierungen für einzelne Aufträge
                                            Reservierungen von Zeiten für einzelne Aufträge müssen vom ERP-Sys-
                                            tem erfasst und übertragen werden. Die als Reservierungsauftrag gekenn-
                                            zeichneten und zur Produktion freigegebenen Aufträge reservieren auf
                                            allen für die Produktion benötigten Maschinen entsprechende Zeiten.




                                        A




                                        B




                                        C




                                        A Maschine, für die Kapazitäten          B Detail-Informationen
                                          angezeigt werden                       C Informationen zur Reservierung
                                            Abb. E-25    Reservierungen


                                        Die Kapazitäten einzelner Maschinen (A) werden grafisch dargestellt. Pro Tag
                                        werden alle Schichten angezeigt, die dem ausgewählten Zeitraum entspre-
                                        chen. Dazu stehen jeweils Detail-Informationen (B) zur Verfügung.
                                        Die Reservierungen werden in einer Liste (C) dargestellt, wenn ein Tag mar-
4.50 / 01-2023




                                        kiert ist.
                                        Die Kapazität einer Maschine pro Tag wird durch die Schichten festgelegt, die
                                        für diese Maschine angelegt sind.


                 A+W Production Kapazitätsplanung                                                                       E-55
                 Planung und Einlastung                                                                         Tutorial




                                          Wird ein Auftrag nach A+W Production übertragen, prüft die Software, ob es
                                          für den Kunden oder das Objekt eine Reservierung gibt.
                                          •   Wenn ja, lastet A+W Production den Auftrag in die Reservierung ein, so-
                                              fern bei dieser Reservierung noch Kapazität frei ist.
                                          •   Besteht für den Kunden oder das Objekt noch keine Reservierung, oder bei
                                              der Reservierung sind keine Kapazitäten frei, belegt der Auftrag nicht-re-
                                              servierte Kapazitäten.

                                          Abgelaufene Reservierungen
                                          Sind abgelaufene Reservierungen vorhanden, wird beim Öffnen des Dialogs
                                          Reservierungen zunächst der Dialog Abgelaufene Reservierungen angezeigt.
                                          Abgelaufene Reservierungen könne Sie löschen oder künftige Reservierun-
                                          gen übernehmen, indem Sie das Ablaufdatum ändern.


                                          Reservierungen anlegen und verwalten
                                          In diesem Teil des Tutorials lernen Sie, wie Sie Reservierungen anlegen, be-
                                          arbeiten oder löschen.
                                          Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                          •   “So löschen Sie eine abgelaufene Reservierung” auf Seite E-61
                                          •   “So legen Sie eine Reservierung an” auf Seite E-57
                                          •   “So bearbeiten Sie eine Reservierung” auf Seite E-59
                                          •   “So löschen Sie eine Reservierung” auf Seite E-60

                                              Bedingung
                                              Reservierungen können nur auf Maschinen angelegt werden, die als Eng-
                                              passbetriebsmittel definiert sind.
4.50 / 01-2023




                 E-56                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                                      Planung und Einlastung




                                         So legen Sie eine Reservierung an
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Reservierungen.
                                           Schließen Sie ggf. den Dialog Abgelaufene Reservierungen, um den Dia-
                                           log Reservierungen zu öffnen.
                                            “So löschen Sie eine abgelaufene Reservierung” auf Seite E-61




                                           A
                                           B
                                           C




                                           A Maschine                            C Anzahl der angezeigten Tage
                                           B Starttermin
                                           Abb. E-26    Reservierungen


                                        2 Wählen Sie die Maschine (A), auf der Sie eine Reservierung eintragen wol-
                                          len, z. B. Schleifen.
                                        3 Wählen Sie den Starttermin (B), ab dem die Reservierung gelten soll.
                                        4 Geben Sie die Anzahl der Tage ein (C), die angezeigt werden sollen,
                                          z. B. 5.
                                           Im Bereich Schichtreservierungen werden die Schichten der Tage ange-
                                           zeigt, in denen die gewählte Maschine zur Verfügung steht.
                                        5 Klicken Sie auf [Neu].
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-57
                 Planung und Einlastung                                                                       Tutorial




                                             A

                                             B
                                             C




                                             D



                                             A Kunde                             C Schicht
                                             B Starttermin                       D Prozentuale Reservierung
                                             Abb. E-27   Reservierung anlegen


                                          6 Wählen Sie einen Kunden (A) oder ein Objekt aus.
                                          7 Wählen Sie den Starttermin (B) und die Schicht (C) für die Reservierung
                                            aus.
                                          8 Geben Sie die Reservierung in % (D) an.
                                             Sie können auch in das Feld darüber klicken, um die Reservierung optisch
                                             anzugeben.




                                          9 Klicken Sie auf [OK], um die Reservierung zu speichern.
                                             Der Dialog wird geschlossen. Die Daten werden in den Dialog Reservie-
                                             rungen übernommen.
4.50 / 01-2023




                 E-58                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                                   Planung und Einlastung




                                        10 Markieren Sie im Feld Schichtreservierungen den Tag mit der Reservie-
                                           rung.




                                           Die Reservierungen für die Schicht werden in der Liste der Reservierungen
                                           angezeigt.
                                        11 Klicken Sie auf [OK], um die Änderungen zu übernehmen.
                                           Die Änderungen werden gespeichert und der Dialog wird geschlossen.


                                         So bearbeiten Sie eine Reservierung
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Reservierungen.
                                        2 Wählen Sie die Maschine, auf der Sie eine Reservierung bearbeiten wol-
                                          len, z. B. Schleifen.
                                        3 Wählen Sie den Starttermin, ab dem die Reservierungen gelten.
                                        4 Geben Sie die Anzahl der Tage ein, die angezeigt werden sollen, z. B. 5.
                                           Im Bereich Schichtreservierungen werden die Schichten der gewählten
                                           Tage angezeigt, in denen die gewählte Maschine zur Verfügung steht.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-59
                 Planung und Einlastung                                                                       Tutorial




                                             Abb. E-28   Reservierung bearbeiten


                                          5 Markieren Sie in der Liste der Reservierungen das Feld, das Sie bearbei-
                                            ten wollen.




                                          6 Ändern Sie den Prozentwert der Reservierung.
                                          7 Klicken Sie auf [OK], um die Änderungen zu übernehmen.
                                             Die Änderungen werden gespeichert und der Dialog wird geschlossen.


                                           So löschen Sie eine Reservierung
                                          1 Wählen Sie Stammdaten > Kapazitätsplanung > Reservierungen.
                                          2 Wählen Sie die Maschine, auf der Sie eine Reservierung bearbeiten wol-
                                            len, z. B. Schleifen.
                                          3 Wählen Sie den Starttermin, ab dem die Reservierungen gelten.
                                          4 Geben Sie die Anzahl der Tage ein, die angezeigt werden sollen, z. B. 5.
                                             Im Bereich Schichtreservierungen werden die Schichten der gewählten
4.50 / 01-2023




                                             Tage angezeigt, in denen die gewählte Maschine zur Verfügung steht.




                 E-60                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                                   Planung und Einlastung




                                        5 Markieren Sie die Zeile mit der Reservierung, die gelöscht werden soll.




                                        6 Klicken Sie auf [Löschen].
                                           Die markierte Reservierung wird aus der Liste gelöscht.
                                        7 Klicken Sie auf [OK], um die Änderungen zu übernehmen.
                                           Die Änderungen werden gespeichert und der Dialog wird geschlossen.


                                         So löschen Sie eine abgelaufene Reservierung
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Reservierungen.




                                           Abb. E-29   Abgelaufene Reservierungen


                                        2 Markieren Sie in der Liste die Reservierungen, die Sie löschen wollen.
                                        3 Klicken Sie auf [Löschen].
                                           Die Reservierungen werden gelöscht.
                                        4 Klicken Sie auf [OK], um die Änderungen zu speichern.
                                           Der Dialog Abgelaufene Reservierungen wird geschlossen und der Dialog
                                           Reservierungen wird geöffnet.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-61
                 Planung und Einlastung                                                                         Tutorial




                                          Übungen zu Reservierungen
                                          •   Legen Sie für einen Kunden oder ein Objekt eine Reservierung für mehrere
                                              Tage und Schichten an.
                                          •   Erfassen Sie einen Testauftrag für einen Kunden oder ein Objekt mit einem
                                              Liefertermin am Ende der zwei Wochen.
                                          •   Lasten Sie den Auftrag ein.
                                          •   Prüfen Sie die Ergebnisse.
                                          •   Legen Sie eine neue Reservierung an und erfassen Sie einen neuen Auf-
                                              trag, der die reservierten Kapazitäten übersteigt.
                                          •   Lasten Sie den Auftrag ein und prüfen Sie die Ergebnisse.
                                          •   Bearbeiten Sie Reservierungen.


                                          Ergänzende Informationen
                                           Softwarereferenz, “Reservierungen” auf Seite E-194
4.50 / 01-2023




                 E-62                                                               A+W Production Kapazitätsplanung
                 Tutorial                                                                          Planung und Einlastung




                                       Bearbeitungserzeugung
                                        Lernziele

                                        • Was ist die Bearbeitungserzeugung?
                                        • Wie werden Bearbeitungen erzeugt und in der Stückliste ergänzt?


                                        Nutzen

                                        • Das PPS-System benötigt für die Kalkulation der einzelnen Produktionstermine
                                          und Produktionskosten eine detailliertere Stückliste, in der alle Arbeitsschritte
                                          enthalten sind. Diese werden im Rahmen der Einlastung durch die
                                          Bearbeitungserzeugung erstellt.


                                        Merke

                                        Bearbeitungen               Bearbeitungen definieren den Bedarf bearbeitet zu
                                                                    werden, z. B. Säumen.

                                        Arbeitsgänge                Arbeitsgänge definieren die Art und Weise, wie der
                                                                    Bedarf der Bearbeitung erfüllt werden soll, z. B. eine
                                                                    spezielle Art des Säumens.

                                           Voraussetzung
                                           Die Bearbeitungserzeugung kann nur durch die Zuordnung von Bearbei-
                                           tungsartikeln zu Teiletypen durchgeführt werden. Wie Sie Bearbeitungsty-
                                           pen, Bearbeitungsartikel und Teiletypen anlegen, wird im Part Stammdaten
                                           beschrieben.
                                           Bitte sprechen Sie Änderungen in der Bearbeitungserzeugung mit dem
                                           Kundenservice der A+W Software GmbH ab, da solche Änderungen pro-
                                           duktionsrelevant sind.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                       E-63
                 Planung und Einlastung                                                                          Tutorial




                                          Bearbeitungserzeugung für die Einlastung
                                          Die Stückliste des ERP-Systems enthält das zu fertigende Endprodukt mit sei-
                                          nen Unterteilen und die preisrelevanten Bearbeitungen, z. B. das Säumen der
                                          Kanten. Andere Produktionsschritte sind in dieser Stückliste nur implizit ent-
                                          halten, z. B. der Zuschnitt.
                                          A+W Capacity Planner benötigt für die Kalkulation der einzelnen Produktions-
                                          termine und Produktionskosten eine detailliertere Stückliste mit allen Arbeits-
                                          schritten, für die ein Aufwand an Zeit oder Kosten notwendig ist. Daher werden
                                          im Rahmen der Einlastung produktionsrelevante Arbeitsschritte in der Produk-
                                          tionsstückliste ergänzt. Die Bearbeitungserzeugung stellt damit sicher, dass
                                          für jedes Stücklistenteil beschrieben wird, wie es in der Produktion entsteht.

                                                                                         B




                                          A




                                          A Bearbeitungen mit den zugeordneten B Teiletypen mit zugeordneten
                                            Bearbeitungsartikeln                 Bearbeitungen
                                          Abb. E-30    Bearbeitungserzeugung


                                          Damit die Bearbeitungen für die Teile der Stückliste erzeugt werden können,
                                          müssen diese Bearbeitungen an den entsprechenden Teiletypen erlaubt sein.
                                          Indem Sie die Bearbeitung (A) einem Teiletyp (B) zuordnen, kann die Produk-
                                          tionsstückliste so erzeugt werden, dass alle zeit- und kostenrelevanten Be-
                                          rechnungen durchgeführt werden können.
                                          Daher müssen für die Kapazitätsplanung mindestens für alle Lagerentnah-
                                          men, Bestell- und Zuschnittsteile und für den Zusammenbau von VSG und
4.50 / 01-2023




                                          ISO Bearbeitungen definiert sein.




                 E-64                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                                     Planung und Einlastung




                                        Bearbeitungen erzeugen
                                        In dieser Lerneinheit erfahren Sie, wie Sie die Stückliste um produktionsrele-
                                        vante Bearbeitungsschritte ergänzen.
                                        Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                        •   “So ergänzen Sie eine Bearbeitung” auf Seite E-65
                                        •   “So entfernen Sie eine Bearbeitung aus der Bearbeitungserzeugung” auf
                                            Seite E-66


                                         So ergänzen Sie eine Bearbeitung

                                            Bearbeitungen ergänzen
                                            Bei der Ergänzung von Bearbeitungen sind Änderungen gesetzt, sobald
                                            sie im Dialog eingetragen sind. Sie können nicht rückgängig gemacht wer-
                                            den.
                                            Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH,
                                            wenn Sie Bearbeitungen ändern wollen.

                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung.




                                        Abb. E-31    Bearbeitungsartikel zuordnen
4.50 / 01-2023




                                        2 Markieren Sie im Feld Bearbeitungen den Bearbeitungsartikel, den Sie ei-
                                          nem Teiletyp zuordnen wollen.



                 A+W Production Kapazitätsplanung                                                               E-65
                 Planung und Einlastung                                                                        Tutorial




                                          3 Markieren Sie im Feld Teiletypen einen Teiletyp, dem Sie den Bearbei-
                                            tungsartikel zuordnen wollen.
                                          4 Klicken Sie auf den Pfeil nach rechts.
                                             Der Bearbeitungsartikel wird dem Artikeltyp zugeordnet.
                                          5 Klicken Sie auf [OK], um die Daten zu speichern.
                                             Die Zuordnung wird gespeichert.


                                           So entfernen Sie eine Bearbeitung aus der Bearbeitungserzeugung

                                             Bearbeitungen ergänzen
                                             Bei der Ergänzung von Bearbeitungen sind Änderungen gesetzt, sobald
                                             sie im Dialog eingetragen sind. Diese können nicht rückgängig gemacht
                                             werden.
                                             Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH,
                                             wenn Sie Bearbeitungen ändern wollen.

                                          1 Wählen Sie Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung.




                                          Abb. E-32   Zuordnung entfernen


                                          2 Markieren Sie im Feld Teiletypen den Bearbeitungsartikel, der entfernt wer-
4.50 / 01-2023




                                            den soll.




                 E-66                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                                    Planung und Einlastung




                                        3 Klicken Sie auf den Pfeil nach links.
                                           Die Zuordnung wird vom Artikeltyp entfernt.
                                        4 Klicken Sie auf [OK], um die Daten zu speichern.
                                           Die Änderung wird gespeichert.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-67
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                       Stammdaten der Kapazitäts-
                                       planung
                                       Um mit A+W Capacity Planner arbeiten zu können, müssen die Stammdaten
                                       für die Kapazitätsplanung eingerichtet sein. Diese Stammdaten bilden zusam-
                                       men mit den Stammdaten der Maschinenzuordnung (MZO) und den Stamm-
                                       daten der Artikel die Grundlage für die Einlastung der Aufträge und die
                                       Verplanung durch A+W Capacity Planner.
                                       Bevor Sie die Stammdaten der Kapazitätsplanung einrichten oder bearbeiten,
                                       müssen die Maschinen und Arbeitsgänge vollständig beschrieben sein. Infor-
                                       mationen zu diesem Thema finden Sie im Part Maschinenzuordnung.

                                           Stammdaten vor Zugriff schützen
                                           Die Stammdaten von A+W Production und insbesondere von A+W Capa-
                                           city Planner sind hochsensible Daten. Unkontrollierte oder unbeabsichtigte
                                           Eingriffe und Änderungen können die gesamte Produktion stilllegen.
                                           Richten Sie daher die jeweiligen Arbeitsplätze so ein, dass nur die Admi-
                                           nistratoren oder Mitarbeiter mit entsprechenden Funktionen Zugriff auf die
                                           Stammdaten haben.

                                       In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                       •   “Schichten” auf Seite E-69
                                       •   “Kostenkalkulation” auf Seite E-88
                                       •   “Übergangszeiten” auf Seite E-93
                                       •   “Vorgabezeiten” auf Seite E-106
                                       •   “Maschinengruppen” auf Seite E-132
                                       •   “Lastverteilung” auf Seite E-138

                                           Datensicherung
                                           Erstellen Sie eine vollständige Datensicherung der Stammdaten bevor Sie
                                           mit der Bearbeitung der Stammdaten beginnen. Das Backup-Tool finden
                                           Sie unter:
                                           C:\Programme (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe.
                                           Verschieben Sie das gespeicherte Backup aus Ihrem User-Verzeichnis in
                                           ein Verzeichnis, auf das auch der Support Zugriff hat.
                                           Besprechen Sie die anstehenden Änderung vorab mit Ihrem Projektierer
                                           bei der A+W Software GmbH.
4.50 / 01-2023




                 E-68                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                            Stammdaten der Kapazitätsplanung




                                        Schichten
                                        Lernziele

                                        •   Wozu dient der Kalender?
                                        •   Was sind Schichten?
                                        •   Welche Angaben werden für eine Schicht benötigt?
                                        •   Wie werden Schichten angelegt, bearbeitet oder gelöscht?


                                        Nutzen

                                        • Mit Schichten definieren Sie, in welchem Zeitrahmen an bestimmten Maschinen
                                          gearbeitet wird.


                                        Merke

                                        Kalender                    Mit dem Kalender definieren Sie arbeitsfreie Tage, z. B.
                                                                    gesetzliche Feiertage oder Betriebsferien.

                                        Arbeitsschicht              Arbeitsschichten werden im Produktionsmonitor
                                                                    angezeigt. Eine Arbeitsschicht wird als Schichtplan mit
                                                                    Schichtregeln und Schichtgruppen definiert.

                                        Schichtplan                 Im Schichtplan ist mit Schichtregeln und Schichtgruppen
                                                                    definiert:
                                                                    • In wie vielen Schichten wird gearbeitet.
                                                                    • An welchen Tagen steht die Schicht zur Verfügung.
                                                                    • Für welche Maschinen gelten die Regeln.

                                        Schichtregel                Mit einer Schichtregel definieren Sie Einzelheiten einer
                                                                    Schicht, z. B. die Schichtdauer.
                                                                    Zu jeder Schichtregel kann nur eine Schichtgruppe
                                                                    definiert werden. Alle Schichtregeln eines Schichtplans
                                                                    müssen dieselbe Schichtgruppe haben.

                                        Schichtgruppe               In einer Schichtgruppe sind die Maschinen angegeben,
                                                                    die in der Schicht arbeiten. Alle Schichtregeln einer
                                                                    Schicht müssen dieselben Maschinengruppen haben.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                       E-69
                 Stammdaten der Kapazitätsplanung                                                                 Tutorial




                                         Schichtpläne
                                         Mit Schichtplänen definieren Sie Arbeitsschichten, die im Produktionsmonitor
                                         angezeigt werden. Im Schichtplan legen Sie fest, in welchem Zeitrahmen die
                                         Betriebsmittel in Ihrer Produktion arbeiten. Eine einzelne Arbeitsschicht kann
                                         im Produktionsmonitor geändert oder gelöscht werden, ohne dass die Ände-
                                         rung in den Schichtplan übernommen wird.




                 A
                   B
                 C
                   D                                                                                  E



                                                                                                      F




                 A Kalender                                         D Schichtregel mit zugewiesenen Maschinen
                 B Schichtplan                                      E Schichtplan ist verfügbar
                 C Schichtregel                                     F Daten für den Produktionsmonitor erzeugen
                 Abb. E-33   Schichten


                                         Eine allgemeine Grundlage bildet der Kalender (A), in dem Sie die arbeitsfrei-
                                         en Tage festlegen, z. B. die öffentlichen Feiertage oder Betriebsferien.
                                         Die Schichten definieren Sie in A+W Production durch einen Schichtplan (B)
                                         mit Schichtregeln (C) und Schichtgruppen (D).
                                         •   Mit dem Schichtplan (B) definieren Sie die Rahmenbedingungen. Sie er-
                                             stellen z. B. einen Schichtplan Zwei-Schicht, in dem Sie dann den Zwei-
                                             Schicht-Betrieb definieren. Im Schichtplan Zwei-Schicht legen Sie fest, ob
                                             dieser aktiv ist, ab wann und wie lange er gültig ist und ob Sie den eigenen
                                             Schichtkalender verwenden, oder ob der Schichtkalender aus dem ERP-
                                             System importiert werden soll.
                                         •   Zu jedem Schichtplan gehört mindestens eine Schichtregel (C), mit der Sie
4.50 / 01-2023




                                             festlegen, an welchen Tagen und zu welchen Uhrzeiten gearbeitet wird,
                                             z. B. im Zwei-Schicht-Betrieb von Montag bis Freitag, jeweils von 6 Uhr bis
                                             14 Uhr in der Frühschicht und von 14 Uhr bis 22 Uhr in der Spätschicht.



                 E-70                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                          Stammdaten der Kapazitätsplanung




                                        •   Die Schichtregel gilt für eine Schichtgruppe (D), in der Sie definieren, wel-
                                            che Maschinen in welchen Schichten arbeiten. So können Sie z. B. festle-
                                            gen, dass einer Ihrer Schneidetische immer nur in der Frühschicht aktiv ist,
                                            oder dass das CNC-Center auch samstags in Betrieb ist. Jeder Schichtre-
                                            gel kann nur eine Schichtgruppe hinzugefügt werden. Wenn Sie mehrere
                                            Schichtregeln verwenden, müssen alle dieselbe Schichtgruppe erhalten.
                                            Mit den Schichtregeln können Sie die Planung so einrichten, dass z. B. die
                                            Maschinen, an denen Engpässe entstehen können, in mehreren Schichten
                                            arbeiten, alle anderen aber nur in einer Schicht.
                                        Jeder Schichtplan kann zunächst unabhängig von der Kapazitätsplanung de-
                                        finiert werden. Damit können Sie Schichtpläne anlegen, die Sie nur zu be-
                                        stimmten Zeiten aktivieren (E), z. B. für Sonderschichten.
                                        Außerdem kann jeder Schichtplan nur begrenzt gültig sein. So können Sie
                                        z. B. für ein geplantes Bauprojekt einen Schichtplan anlegen, der nur für die
                                        Zeit gültig ist, in der die Scheiben geliefert werden müssen. Damit werden die-
                                        se Zeiten außerhalb der Gültigkeit nicht in die Planung einbezogen.
                                        Wenn Sie einen Schichtplan anlegen oder ändern, wird die Schicht nur dann
                                        als Arbeitsschicht in den Produktionsmonitor übernommen, wenn sie mit (F)
                                        explizit erzeugt wird. Die neuen Arbeitsschichten werden bei der Einlastung in
                                        A+W Capacity Planner für die neuen Aufträge berücksichtigt, die bereits ein-
                                        gelasteten Aufträge bleiben davon unberührt.
                                        Eine Übersicht über die Arbeitsschichten und deren Auslastung können Sie
                                        sich im Dialog Produktionsmonitor anzeigen lassen.
                                         Softwarereferenz, “Einlastung” auf Seite E-148
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                  E-71
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                       Arbeitsfreie Tage anlegen
                                       In dieser Lerneinheit lernen Sie, wie Sie arbeitsfreie Tage anlegen, bearbeiten
                                       oder löschen.

                                           Kalender einrichten
                                           Sie müssen den Kalender einrichten, bevor Sie Schichtpläne definieren.
                                           Die arbeitsfreien Tage werden nur für neue Schichten berücksichtigt.

                                       Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       •   “So legen Sie arbeitsfreie Tage an” auf Seite E-72
                                       •   “So bearbeiten Sie arbeitsfreie Tage” auf Seite E-73
                                       •   “So löschen Sie arbeitsfreie Tage” auf Seite E-74


                                        So legen Sie arbeitsfreie Tage an
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.

                                                A                                 B




                                       A Kalender markieren                   B Arbeitsfreie Tage
                                       Abb. E-34    Schichtkalender
4.50 / 01-2023




                                       2 Markieren Sie im Feld Schichteditor den Eintrag Kalender (A).



                 E-72                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                        3 Klicken Sie auf [Neu].
                                           Im Bereich Schichtkalender wird eine neue Zeile eingefügt.
                                        4 Tragen Sie in den Feldern Tag und Kommentar die Daten ein, z. B. einen
                                          nationalen Feiertag.
                                        5 Klicken Sie auf [Übernehmen].
                                           Die Daten werden gespeichert. Beim Anlegen von neuen Schichten wer-
                                           den die arbeitsfreien Tage übersprungen.


                                         So bearbeiten Sie arbeitsfreie Tage
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                        2 Markieren Sie im Bereich Schichteditor den Eintrag Kalender.




                                        Abb. E-35   Kalender bearbeiten


                                        3 Markieren Sie im Feld Schichtkalender das Datum, das Sie bearbeiten wol-
                                          len.
                                        4 Ändern Sie die Werte.
                                        5 Klicken Sie auf [Übernehmen].
                                           Die Daten werden gespeichert.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-73
                 Stammdaten der Kapazitätsplanung                                                         Tutorial




                                        So löschen Sie arbeitsfreie Tage
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                       2 Markieren Sie im Bereich Schichteditor den Eintrag Kalender.
                                       3 Markieren Sie im Bereich Kalender in der ersten Spalte den Tag, den Sie
                                         löschen wollen.

                                               A                          B




                                       A Kalender                               B Markierung
                                       Abb. E-36    Arbeitsfreie Tage löschen


                                       4 Klicken Sie auf [Löschen].
                                          Der Tag mit dem Pfeil in der ersten Spalte wird gelöscht.
                                       5 Klicken Sie auf [Übernehmen].
                                          Die Daten werden gespeichert.
4.50 / 01-2023




                 E-74                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                        Schichtplan erstellen
                                        In dieser Lerneinheit lernen Sie, wie Sie Schichtpläne anlegen, bearbeiten
                                        oder löschen.
                                        Eine neue Arbeitsschicht kann erst erzeugt werden, wenn zu dem neuen
                                        Schichtplan mindestens eine Schichtregel und eine Schichtgruppe mit Ma-
                                        schinen angelegt sind.
                                        Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                        •   “So erstellen Sie einen Schichtplan” auf Seite E-76
                                        •   “So bearbeiten Sie einen Schichtplan” auf Seite E-77
                                        •   “So löschen Sie einen Schichtplan” auf Seite E-78

                                            Daten übernehmen
                                            Wenn Sie einen Schichtplan, eine Schichtregel oder eine Schichtgruppe
                                            erstellen oder ändern, müssen Sie auf [Erzeugen] klicken, damit die geän-
                                            derten Schichtdaten im Produktionsmonitor erzeugt wird.
                                            Wenn die geänderte Schicht nicht erzeugt wird, plant A+W Production die
                                            Produktion mit den alten Schichtdaten.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-75
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                        So erstellen Sie einen Schichtplan
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                       2 Markieren Sie im Bereich Schichteditor den Eintrag Kalender.

                                                    A




                                                                                B
                                       A Auswahl Kontextmenü                 B Auswahl Schaltfläche
                                       Abb. E-37    Neuer Schichtplan


                                       3 Öffnen Sie mit einem Rechtsklick auf den Kalender das Kontextmenü (A)
                                         und wählen den Eintrag Neuer Schichtplan.
                                          Alternativ können Sie die Auswahl-Liste (B) auf der Schaltfläche [Neu] öff-
                                          nen und Neuer Schichtplan wählen.
4.50 / 01-2023




                                       4 Tragen Sie im Bereich Schichtplan im Feld Name eine Bezeichnung ein,
                                         z. B. Zwei-Schicht normal.


                 E-76                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                              Stammdaten der Kapazitätsplanung




                                        5 Klicken Sie auf [Übernehmen].
                                           Die Daten werden gespeichert. Der neue Schichtplan wird im Schichteditor
                                           angezeigt.
                                           Als nächstes müssen Sie die Schichtregeln einrichten und die Maschinen
                                           zuordnen. Erst danach wird die Schaltfläche [Erzeugen] freigeschaltet.
                                            “Schichtregel erstellen” auf Seite E-78


                                         So bearbeiten Sie einen Schichtplan
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                        2 Markieren Sie im Bereich Schichteditor den Schichtplan, den Sie bearbei-
                                          ten wollen.




                                        3 Bearbeiten Sie die Werte des Schichtplans.
                                           Ein typischer Anwendungsfall ist die Verlängerung eines Schichtplans.
                                        4 Prüfen Sie, ob die Checkbox Aktiv markiert ist, damit der Schichtplan in der
                                          Kapazitätsplanung verwendet werden kann.
                                        5 Klicken Sie auf [Übernehmen].
                                           Die Daten werden gespeichert.
                                        6 Klicken Sie auf [Erzeugen], damit die Schicht mit den geänderten Daten im
                                          Produktionsmonitor erzeugt wird.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                 E-77
                 Stammdaten der Kapazitätsplanung                                                           Tutorial




                                        So löschen Sie einen Schichtplan

                                           Schichtplan löschen
                                           Wenn Sie einen Schichtplan löschen, werden die zugehörige Schichtregel
                                           und die zugehörige Schichtgruppe mit gelöscht! Im Produktionsmonitor
                                           wird die gelöschte Schicht weiterhin angezeigt. Um sie aus dem Produkti-
                                           onsmonitor zu löschen, müssen Sie erst die eingelasteten Bearbeitungen
                                           umlasten.

                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                       2 Markieren Sie im Bereich Schichteditor den Schichtplan, den Sie löschen
                                         wollen.
                                       3 Klicken Sie auf [Löschen].
                                           Der Schichtplan wird aus dem Schichteditor gelöscht.
                                       4 Klicken Sie auf [Übernehmen].
                                           Die Daten werden gespeichert.


                                       Schichtregel erstellen
                                       In dieser Lerneinheit lernen Sie, wie Sie Schichtregeln anlegen, bearbeiten
                                       oder löschen.
                                       Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       •   “So erstellen Sie eine Schichtregel” auf Seite E-79
                                       •   “So bearbeiten Sie eine Schichtregel” auf Seite E-81
                                       •   “So löschen Sie eine Schichtregel” auf Seite E-82

                                           Daten übernehmen
                                           Wenn Sie einen Schichtplan, eine Schichtregel oder eine Schichtgruppe
                                           erstellen oder ändern, müssen Sie auf [Erzeugen] klicken, damit die geän-
                                           derte Schicht im Produktionsmonitor erzeugt wird.
                                           Wenn die geänderte Schicht nicht erzeugt wird, plant A+W Production die
                                           Produktion mit den alten Schichtdaten.
4.50 / 01-2023




                 E-78                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                         So erstellen Sie eine Schichtregel
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                        2 Markieren Sie den Schichtplan, dem Sie die Schichtregel zuordnen wollen.

                                                      A




                                                                                 B
                                        A Auswahl Kontextmenü                 B Auswahl Schaltfläche
                                        Abb. E-38   Neue Schichtregel


                                        3 Öffnen Sie zu dem Schichtplan das Kontextmenü (A) und wählen den Ein-
                                          trag Neue Schichtregel.
                                           Alternativ können Sie die Auswahl-Liste (B) auf der Schaltfläche [Neu] öff-
                                           nen und Neue Schichtregel wählen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                               E-79
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                                                                           A
                                                                                           B

                                                                                           C




                                                                                           D



                                          A Name der Schichtregel                    C Schichtnummer
                                          B Start- und Enddatum                      D Auswahl Kalender
                                          Abb. E-39    Definition der Schichtregel


                                       4 Geben Sie einen Namen (A) und eine Schichtnummer (C) ein, z. B. Früh-
                                         schicht und Nummer 1.
                                       5 Wählen Sie die Uhrzeit für Schichtbeginn und Schichtende (B), z. B. Be-
                                         ginn 6 Uhr und Ende 14 Uhr.
                                       6 Markieren Sie die Wochentage, an denen in der Schicht gearbeitet werden
                                         soll, z. B. Mo-Fr für eine Fünf-Tage-Arbeitswoche.
                                       7 Wählen Sie, ob Sie den eigenen Kalender verwenden wollen (D), oder ob
                                         der Kalender aus dem ERP-System importiert werden soll, z. B. aus A+W
                                         Enterprise.
                                          Den Gültigkeitszeitraum müssen Sie nur festlegen, wenn Sie eine Sonder-
                                          schicht einrichten.
                                       8 Klicken Sie auf [Übernehmen].
                                          Die Daten werden gespeichert. Der neue Schichtplan wird im Schichteditor
                                          angezeigt.
                                          Als nächstes müssen Sie die Schichtgruppen einrichten und die Maschi-
                                          nen zuordnen. Erst danach wird die Schaltfläche [Erzeugen] freigeschaltet.
                                           “Schichtgruppe erstellen” auf Seite E-83
4.50 / 01-2023




                 E-80                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                         So bearbeiten Sie eine Schichtregel
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                        2 Markieren Sie die Schichtregel, die Sie bearbeiten wollen.




                                                                                      A           B            C
                                        A Gültigkeitszeitraum ändern           B Daten der Schicht speichern
                                                                               C Daten für Planung erzeugen
                                        Abb. E-40    Schichtregel bearbeiten


                                        3 Ändern Sie im Bereich Schichtregel die Werte.
                                           Eine typische Änderung ist, einen Schichtplan zu verlängern. Dazu ändern
                                           Sie den Zeitraum (A). Die Felder für den Zeitraum sind nur freigeschaltet,
                                           wenn mindestens eine Schichtgruppe zugeordnet ist.
                                        4 Klicken Sie auf [Übernehmen] (B).
                                           Die Daten werden gespeichert.
                                        5 Klicken Sie auf [Erzeugen] (C), damit die Schicht mit den geänderten Daten
                                          im Produktionsmonitor erzeugt wird.
                                           Die Arbeitsschicht wird mit den geänderten Daten im Produktionsmonitor
                                           angezeigt.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                  E-81
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                        So löschen Sie eine Schichtregel
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                          Bevor Sie eine Schichtregel löschen, sollten Sie die Gültigkeit einschrän-
                                          ken. Damit werden die Arbeitsschichten im Produktionsmonitor nicht mehr
                                          angezeigt und können nicht mehr bebucht werden.
                                       2 Markieren Sie die Schichtregel, die Sie löschen wollen.




                                                                                           A       B
                                       A Schichtregel löschen                B Schichtregel für Schichtplan löschen
                                       Abb. E-41    Schichtregel löschen


                                       3 Klicken Sie auf [Löschen] (A).
                                          Die Schichtregel wird aus dem Editor gelöscht.
                                       4 Klicken Sie auf [Löschen] (B).
                                          Die Arbeitsschicht wird aus dem Produktionsmonitor gelöscht.

                                          Schicht löschen
                                          Sie können eine Arbeitsschicht im Produktionsmonitor löschen. Dabei wird
                                          nur die einzelne Arbeitsschicht gelöscht. Wenn Sie die Arbeitsschichten lö-
                                          schen wollen, indem Sie die Schichtregel löschen, sollten Sie zunächst die
                                          Arbeitsschichten im Produktionsmonitor prüfen. Unter Umständen müssen
                                          Sie noch eingelastete Aufträge verschieben.
4.50 / 01-2023




                 E-82                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                        Schichtgruppe erstellen
                                        In dieser Lerneinheit lernen Sie, wie Sie Schichtgruppen anlegen, bearbeiten
                                        oder löschen.
                                        Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                        •   “So erstellen Sie eine Schichtgruppe” auf Seite E-83
                                        •   “So bearbeiten Sie eine Schichtgruppe” auf Seite E-86
                                        •   “So löschen Sie eine Schichtgruppe” auf Seite E-87

                                            Daten übernehmen
                                            Wenn Sie einen Schichtplan, eine Schichtregel oder eine Schichtgruppe
                                            erstellen oder ändern, müssen Sie auf [Erzeugen] klicken, damit die geän-
                                            derte Schicht im Produktionsmonitor erzeugt wird.
                                            Wenn die geänderte Schicht nicht erzeugt wird, plant A+W Production die
                                            Produktion mit den alten Schichtdaten.


                                         So erstellen Sie eine Schichtgruppe
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                        2 Markieren Sie im Bereich Schichteditor die Schichtregel, der Sie die
                                          Schichtgruppe zuordnen wollen.

                                                         A




                                                                                  B
4.50 / 01-2023




                                        A Auswahl Kontextmenü                 B Auswahl Schaltfläche
                                        Abb. E-42    Neue Schichtgruppe



                 A+W Production Kapazitätsplanung                                                                E-83
                 Stammdaten der Kapazitätsplanung                                                          Tutorial




                                       3 Öffnen Sie zu der Schichtregel das Kontextmenü (A) und wählen Sie den
                                         Eintrag Neue Schichtgruppe.
                                          Alternativ dazu können Sie die Auswahl-Liste (B) auf der Schaltfläche
                                          [Neu] öffnen und Neue Schichtgruppe wählen.


                                                                                      A




                                                                                      B




                                          A Name der Schichtgruppe              B Schichtgruppe zuweisen
                                          Abb. E-43   Definition der Schichtgruppe


                                       4 Wählen Sie im Feld Name (A) eine Schichtgruppe aus oder tragen Sie ei-
                                         nen Namen ein.
                                          Im Bereich Schichtgruppe bearbeiten werden die verfügbaren Maschinen
                                          gelistet.
                                       5 Klicken Sie auf [Übernehmen], um die Daten zu speichern.
                                       6 Wählen Sie bei allen Maschinen, die Sie der neuen Schichtgruppe zuwei-
                                         sen wollen, in der Spalte Schichtgruppe (B) die Schichtgruppe aus.
4.50 / 01-2023




                 E-84                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                        7 Weisen Sie auf diese Weise jede Maschine einer Schichtgruppe zu.
                                        8 Klicken Sie auf [Übernehmen].
                                           Die Daten werden gespeichert. Die neue Schichtgruppe wird im Schicht-
                                           editor mit allen zugeordneten Maschinen angezeigt.




                                           Nachdem Sie den Schichtplan vollständig definiert haben, können Sie die
                                           Schicht im Produktionsmonitor erzeugen. Dazu gehen Sie folgenderma-
                                           ßen vor:
                                        9 Markieren Sie den neuen Schichtplan im Schichteditor.
                                           Der Bereich Schichtplan wird angezeigt.
                                        10 Markieren Sie die Checkbox Aktiv und tragen Sie das Datum ein, ab dem
                                           der Schichtplan gültig ist.
                                        11 Klicken Sie auf [Erzeugen].
                                           Damit wird die Schicht erzeugt und steht für die Kapazitätsplanung ab dem
                                           Gültigkeitsdatum und ggf. für den angegebenen Zeitraum zur Verfügung.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-85
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                        So bearbeiten Sie eine Schichtgruppe
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                       2 Markieren Sie im Bereich Schichteditor die Schichtgruppe, die Sie bearbei-
                                         ten wollen.




                                       Abb. E-44    Schichtgruppe bearbeiten


                                       3 Ändern Sie im Bereich Schichtgruppe bearbeiten die Daten, z. B.:
                                          •   Maschinen anderen Schichtgruppen zuweisen.
                                              Die Änderung der Zuordnung einer Maschine zu einer Maschinengrup-
                                              pe ist ein typischer Anwendungsfall, um mit einer Maschine in einen an-
                                              deren Schichtbetrieb zu wechseln.
                                          •   Namen einer Schichtgruppe ändern.
                                       4 Klicken Sie auf [Übernehmen], um die Daten zu speichern.
                                          Die Daten werden gespeichert.
                                       5 Markieren Sie die aktuelle Schichtregel.
                                          Der Bereich Schichtregel wird mit den aktuellen Daten angezeigt.
                                       6 Prüfen Sie die Daten und passen Sie ggf. die Einstellungen an, z. B. den
                                         Gültigkeitszeitraum.
                                          Nachdem Sie den Schichtplan bearbeitet haben, können Sie die geänderte
                                          Schicht im Produktionsmonitor erzeugen. Dazu gehen Sie folgenderma-
4.50 / 01-2023




                                          ßen vor:




                 E-86                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                        7 Klicken Sie auf [Erzeugen].
                                            Diesen Schritt müssen Sie für alle Schichten ausführen.


                                         So löschen Sie eine Schichtgruppe
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Schichten.
                                        2 Markieren Sie im Bereich Schichteditor die Schichtgruppe, die Sie löschen
                                          wollen.
                                        3 Klicken Sie auf [Löschen].
                                            Die Schichtgruppe wird gelöscht.
                                        4 Klicken Sie auf [Übernehmen], um die Daten zu speichern.
                                            Die Daten werden gespeichert.


                                        Übungen
                                        Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Ver-
                                        fügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung
                                        vollständig sind, können Sie die Planung für eigene Aufträge im Produktions-
                                        monitor testen.
                                        •   Planen Sie Ihre Produktion auf dem Papier. An welchen Tagen soll in wel-
                                            chen Schichten gearbeitet werden und welche Maschinen werden in wel-
                                            cher Schicht verwendet?
                                        •   Übertragen Sie Ihre Ergebnisse in A+W Production, indem Sie die Schich-
                                            ten definieren.
                                        •   Prüfen Sie Ihre Ergebnisse im Produktionsmonitor.
                                             Softwarereferenz, “Einlastung” auf Seite E-148
                                        •   Ändern Sie für eine Maschine den Schichtplan, z. B. von einem Zwei-
                                            Schicht-Plan in einen Drei-Schicht-Plan.
                                        •   Verlängern Sie einen bestehenden Schichtplan.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Schichten” auf Seite E-231
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-87
                 Stammdaten der Kapazitätsplanung                                                               Tutorial




                                       Kostenkalkulation
                                       Lernziele

                                       • Was ist die Kostenkalkulation in der Kapazitätsplanung?
                                       • Wie werden Kosten für logische Maschinen angelegt, bearbeitet oder gelöscht?
                                       • Welche Daten werden bei der Kostenkalkulation zwischen A+W Production und
                                         dem ERP-System ausgetauscht?


                                       Nutzen

                                       • Mit der Kostenkalkulation kann eine Kostenoptimierung erreicht werden.
                                         Zusammen mit den Übergangszeiten werden bei der Einlastung zunächst die
                                         billigeren Maschinen ausgelastet.
                                       • Durch die Aufschlüsselung und Rückmeldung der Kosten werden folgende Vorteile
                                         ermöglicht:
                                         - Exakte Kostenkalkulation bei Angebots- und Auftragserfassung im ERP-
                                             System.
                                         - Einlastung auf kostengünstigere Betriebsmittel.
                                         - Statistische Auswertungen basierend auf Kosten.


                                       Merke

                                                                  Mit der Kostenkalkulation können Sie Personalkosten,
                                                                  Maschinenkosten und sonstige Kosten ermitteln.

                                                                  Lohn- und Maschinenkosten werden pro Maschine in
                                                                  A+W Capacity Planner hinterlegt.

                                                                  Materialkosten werden im ERP-System hinterlegt und
                                                                  berechnet.
4.50 / 01-2023




                 E-88                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                        Definition der Kostenkalkulation
                                        Für logische Maschinen können Sie die Kosten angeben, die bei der Produk-
                                        tion entstehen. Wird ein Auftrag oder ein Angebot eingelastet, meldet A+W
                                        Production die Kosten an das ERP-System zurück. Damit kann der Auftrags-
                                        erfasser die Produktionskosten anfragen, die bei der Produktion entstehen.
                                        Die Materialkosten werden im ERP-System hinterlegt und berechnet.

                                                      A        B




                                        A Physikalische Maschine                  B Zugeordnete logische Maschine
                                        Abb. E-45     Kostenkalkulation


                                        Sie geben die Kosten pro Stunde und logischer Maschine ein. Damit können
                                        Sie die Kosten einer physikalischen Maschine unterschiedlich gewichten, je
                                        nachdem, welche logische Maschine angesprochen ist. Pro logischer Maschi-
                                        ne geben Sie Maschinenkosten, Lohnkosten und sonstige Kosten separat an.

                                           Beispiel

                                           Auf Ihrer einseitigen Schleifmaschine können unterschiedliche Kantenbear-
                                           beitungen ausgeführt werden, z. B. Schleifen, Polieren und Gehren. Sie wird
                                           insbesondere für Modelle verwendet, wobei die Gehrung auch für Rechtecke
                                           gemacht wird.
                                           Die unterschiedlichen Arbeitsgänge sind nicht nur als unterschiedliche Bear-
                                           beitungen angelegt, sondern auch als unterschiedliche logische Maschinen.
                                           Die Maschinenwerkzeuge für die möglichen Bearbeitungen haben unter-
                                           schiedliche Kosten für die Werkzeugstandzeit und für die Wiederbeschaffung.
                                           Diese Unterschiede bilden Sie über die Kosten der logischen Maschinen ab,
                                           die zu der physikalischen Maschine definiert sind.
                                           Gleichzeitig können Sie die unterschiedlichen Geschwindigkeiten bei der
4.50 / 01-2023




                                           Bearbeitung in verschiedenen Vorgabezeiten berücksichtigen.




                 A+W Production Kapazitätsplanung                                                                     E-89
                 Stammdaten der Kapazitätsplanung                                                              Tutorial




                                       Kosten anlegen und verwalten
                                       In dieser Lerneinheit erfahren Sie, wie Sie Kosten für logische Maschinen an-
                                       legen, bearbeiten oder löschen.
                                       Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       •   “So legen Sie Kosten für eine logische Maschine an” auf Seite E-90
                                       •   “So bearbeiten Sie Kosten für eine logische Maschine” auf Seite E-91
                                       •   “So löschen Sie Kosten für eine logische Maschine” auf Seite E-92


                                        So legen Sie Kosten für eine logische Maschine an
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Kostenkalkulation.
                                           Der Dialog Kostenkalkulation wird geöffnet.
                                       2 Klicken Sie auf [Neu].
                                           In der Liste wird eine Zeile mit der Maschine -1 eingefügt.

                                                       A                          B




                                           A Maschine                             B Kosten
                                           Abb. E-46    Neue Zeile für Kostenkalkulation


                                       3 Klicken Sie doppelt auf das Feld -1 (A).
                                           Der Dialog Bitte wählen Sie eine Maschine aus wird geöffnet.
                                       4 Übernehmen Sie die gewünschte Maschine mit einem Doppelklick.
                                       5 Klicken Sie doppelt auf das leere Feld Log. Maschine.
                                           Der Dialog Bitte wählen Sie eine Technologie aus wird geöffnet. In der Liste
4.50 / 01-2023




                                           sind alle logischen Maschinen aufgeführt, die zur ausgewählten Maschine
                                           definiert sind.




                 E-90                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                        6 Übernehmen Sie die gewünschte logische Maschine mit einem Doppel-
                                          klick.
                                        7 Geben Sie die Lohnkosten pro Stunde für einen Werker ein.
                                           Wenn für den Arbeitsgang zwei Personen erforderlich sind, müssen Sie die
                                           doppelten Kosten eintragen.
                                        8 Wiederholen Sie Schritt 7 für die Felder Maschinenkosten und Sonstige
                                          Kosten (B).
                                           Sie können einen Kommentar eintragen, z. B. um die Lohnkosten zu erklä-
                                           ren.
                                        9 Klicken Sie auf [OK].
                                           Die Daten werden gespeichert und der Dialog wird geschlossen.


                                         So bearbeiten Sie Kosten für eine logische Maschine
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Kostenkalkulation.




                                           Abb. E-47   Kostenkalkulation bearbeiten


                                        2 Ändern Sie den Wert des jeweiligen Felds, z. B. Sonstige Kosten.
                                        3 Wiederholen Sie Schritt 2 für alle Kosten, deren Werte nicht mehr aktuell
                                          sind.
                                        4 Klicken Sie auf [OK].
                                           Die Daten werden gespeichert und der Dialog wird geschlossen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-91
                 Stammdaten der Kapazitätsplanung                                                           Tutorial




                                        So löschen Sie Kosten für eine logische Maschine
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Kostenkalkulation.
                                       2 Markieren Sie die Zeile, die Sie löschen wollen.
                                       3 Klicken Sie auf [Löschen].
                                           Der Eintrag wird aus der Liste gelöscht.
                                           Falls Sie den Eintrag versehentlich gelöscht haben, brechen Sie den Vor-
                                           gang mit [Ende] ab.
                                       4 Klicken Sie auf [OK].
                                           Die Daten werden gespeichert und der Dialog wird geschlossen.


                                       Übungen
                                       Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Ver-
                                       fügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung
                                       vollständig sind, können Sie die Planung für eigene Aufträge im Produktions-
                                       monitor testen.
                                       •   Wählen Sie Ihre Maschine aus und erarbeiten Sie die Kosten für die zuge-
                                           hörigen logischen Maschinen:
                                           Welche Lohnkosten, welche Maschinenkosten und welche sonstigen Kos-
                                           ten fallen jeweils bei der logischen Maschine an.
                                       •   Legen Sie die Kosten für die logische Maschine im Dialog Kostenkalkulati-
                                           on an.
                                       •   Erfassen Sie einen Testauftrag oder ein Testangebot und lasten Sie diese
                                           auf dieser Maschine ein. Prüfen Sie die zurückgemeldeten Preise.
                                       •   Bearbeiten Sie die Kosten der logischen Maschinen im Dialog Kostenkal-
                                           kulation.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Kostenkalkulation” auf Seite E-243
4.50 / 01-2023




                 E-92                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                        Übergangszeiten
                                        Lernziele

                                        • Was sind Übergangszeiten?
                                        • Wie werden Übergangszeiten angelegt, bearbeitet oder gelöscht?


                                        Nutzen

                                        • Übergangszeiten bilden die zeitliche Bewegung der Scheiben durch die Produktion
                                          ab.


                                        Merke

                                        Übergangszeit              Eine Übergangszeit beschreibt die Spanne zwischen
                                                                   den Endzeitpunkten aufeinanderfolgender
                                                                   Bearbeitungen.
                                                                   Wenn zwei aufeinanderfolgende Arbeitsgänge auf
                                                                   derselben Maschine gearbeitet werden, entstehen keine
                                                                   Übergangszeiten, z. B. Bohren und Waschen.
                                                                   Übergangszeiten werden ausschließlich zu logischen
                                                                   Maschinen definiert.

                                        Übergangstyp               Übergangszeiten werden als drei verschiedene Typen
                                                                   definiert: Normal, Eilübergang, minimaler Übergang.

                                        Normaler Übergang          Normale Übergänge beschreiben den optimalen
                                                                   Produktionsablauf, d. h., ohne Ausfälle von Personal
                                                                   oder Maschinen, Bruch usw.

                                        Eilübergang                Eilübergänge bescheiben beschleunigte Durchläufe,
                                                                   z. B., indem die Verweilzeiten verkürzt werden. Diese
                                                                   Übergangszeiten erhöhen jedoch die Kosten.

                                        Minimaler Übergang         Minimale Übergänge sind die teuersten
                                                                   Übergangszeiten.

                                        Übergangszeit 0            Bearbeitungen, die direkt aufeinanderfolgen, haben
                                                                   keine Übergangszeiten, z. B. Rahmenbiegen - ISO-Linie
                                                                   - ISO versiegeln.
                                                                   Bei diesen Bearbeitungen sind alle drei Typen von
                                                                   Übergangszeiten identisch.

                                        Expliziter Übergang        Als expliziten Übergang definieren Sie den Übergang
                                                                   von Maschine x zu Maschine y.

                                        Hierarchische Auswertung   Die hinterlegten Übergangszeiten werden in folgender
                                                                   Reihenfolge ausgewertet:
                                                                   •   Maschine x -> Maschine y.
                                                                   •   Maschine x -> Alle Maschinen.
                                                                   •   Alle Maschinen -> Maschine x.
4.50 / 01-2023




                                                                   •   Alle Maschinen -> Alle Maschinen.




                 A+W Production Kapazitätsplanung                                                                      E-93
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                       Merke

                                       Verweilzeiten        Verweilzeiten bezeichnen Zeiten, die ohne eigentliche
                                                            Bearbeitung verlaufen, z. B. zur Scheibensortierung,
                                                            Wartezeit auf Nachläufer, Trocknungszeiten.
                                                            Notwendige Verweilzeiten können nicht beschleunigt
                                                            werden, z. B. die Zeiten für Heat Soak.
                                                            Verweilzeiten werden mit in die Übergangszeiten
                                                            eingerechnet.

                                       Rüstzeit             Rüstzeiten werden mit in die Übergangszeiten
                                                            eingerechnet.

                                       Kundenhandlingzeit   Damit ist die Zeit gemeint, die zum Verladen der
                                                            verpackten Ware benötigt wird. In der Regel wird dafür
                                                            ein Arbeitstag angesetzt. Für die Beladung eines
                                                            Containers können aber auch mehrere Tage benötigt
                                                            werden.
                                                            Diese Zeit wird nicht in die Terminoptimierung
                                                            eingerechnet und daher auch nicht als Übergangszeit
                                                            definiert. Sie wird im ERP-System in den Stammdaten
                                                            des Kunden hinterlegt.
4.50 / 01-2023




                 E-94                                                       A+W Production Kapazitätsplanung
                 Tutorial                                                               Stammdaten der Kapazitätsplanung




                                             Übergangszeiten in Schichten oder Stunden
                                             Mit Übergangszeiten definieren Sie die Zeit zwischen zwei Bearbeitungen
                                             oder zwei (logischen) Maschinen. Diese Zeiten variieren je nachdem, von wel-
                                             cher Maschine eine Scheibe kommt und zu welcher Maschine sie geht.
                                             Die einfachste Form der Übergangszeit ist die Zeit für den Weg, die eine
                                             Scheibe von einer (logischen) Maschine zur nächsten benötigt, z. B. der
                                             Übergang vom Zuschnitt zur nächsten Bearbeitung. Diese Zeiten werden als
                                             optimale Übergänge mit dem Typ Normal definiert. Wenn der Übergang be-
                                             schleunigt werden kann, wird zusätzlich die Zeit mit dem Typ Eil und/oder Mi-
                                             nimal angelegt.
                                              “Übergangstypen” auf Seite E-100


                                                   Mittwoch         Donnerstag           Freitag           Montag


                  Float Zuschnitt

                  Sortierung für Be...

                  Beschichtungsanl.

                  Sortierung für ISO

                                                                                    1
                  Rahmenbieger 1

                  ISO-Linie 2
                                                                                                   0

                  ISO versiegeln
                                                                                                       2            0
                  Verpacken

                  Fuhrpark



                                                                               A            B                C
                 A Alternative - mit oder ohne        B Übergangszeit innerhalb einer    C Übergang von 2 Schichten
                   Beschichtung                         Schicht
                 Abb. E-48      Rückwärtskalkulation mit normalen Übergangszeiten


                                             In diesem Beispiel sehen Sie den optimalen Ablauf mit den normalen Über-
                                             gangszeiten für eine ISO-Scheibe mit einer beschichteten Scheibe. Wenn in
                                             dem ISO nur eine Scheibe beschichtet (A) wird, teilt sich der Zuschnitt auf
                                             zwei Schichten auf, damit die zu beschichtende Scheibe früher geschnitten
                                             wird. Da Rahmenbieger - ISO-Linie - ISO versiegeln (B) immer direkt hinterei-
4.50 / 01-2023




                                             nander ausgeführt werden, fallen diese Bearbeitungen in derselben Schicht
                                             an.



                 A+W Production Kapazitätsplanung                                                                       E-95
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                       Der Übergang wird jeweils vom Ende einer Schicht aus betrachtet. Der Über-
                                       gang von Verpacken zum Versiegeln (C) ist z. B. mit 2 Schichten angegeben.
                                       Damit bleibt genug Spielraum innerhalb der Schicht, in der die Bearbeitung
                                       anfällt.
                                       Jeder Übergang in eine andere Schicht erzeugt virtuelle Kosten, die um so hö-
                                       her ausfallen, je weiter der Übergang vom optimalen Übergang abweicht. Die
                                       Übergänge müssen also auch unter diesem Gesichtspunkt so optimal wie
                                       möglich gestaltet werden.

                                       Übergangszeiten in Schichten
                                       Maximale Übergangszeiten werden nur für normale Übergänge ausgewertet.
                                       Die anderen Übergänge werden als minimal automatisch aufgefüllt. Falls es
                                       einen Eintrag vom Typ Minimal gibt, sind schnellere Übergänge verboten. Für
                                       Eil-Übergänge genügt die Angabe der Mindestanzahl Schichten.


                                              Mittwoch       Donnerstag        Freitag         Montag




                                                                          A              B         C
                                       A Optimale und maximale                B Eil-Übergangszeit
                                         Übergangszeit                        C Minimale Übergangszeit
                                       Abb. E-49    Übergänge in Schichten


                                       In diesem Beispiel ist die nomale Übergangszeit (A) auf fünf Schichten festge-
                                       legt, die maximal auf sieben erweitert werden können. Der Eil-Übergang (B)
                                       ist mit drei Schichten definiert. Das Programm kann damit automatisch auch
                                       vier Schichten berechnen.
                                       Mit dem minimalen Übergang von genau einer Schicht (C) ist der Übergang in
                                       derselben Schicht automatisch verboten. Der Übergang von zwei Schichten
                                       wird ebenfalls automatisch mit berechnet.
                                       Das bedeutet, dass Sie nur vier Angaben festlegen müssen: Normal mit 5 + 2,
                                       Eil mit 3 Schichten und Minimal mit 1 Schicht. Damit können sieben mögliche
                                       Schichtübergänge berechnet werden.
4.50 / 01-2023




                 E-96                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                         Stammdaten der Kapazitätsplanung




                                        Übergangszeiten in Stunden
                                        Die Übergangszeit in Stunden bezieht sich nicht auf Arbeitszeit, sondern auf
                                        die Kalenderzeit und wird auch so bei den virtuellen Kosten bewertet. Das Pro-
                                        gramm legt die Übergangszeiten in Stunden in aller Regel in die Arbeitszeit.
                                        Bearbeitungstermine beziehen sich immer auf das Schichtende. Bei einer
                                        Übergangszeit von bei 00:00 Stunden gehen die Scheiben unmittelbar auf die
                                        nächste Maschine über, d. h. werden in derselben Schicht weiterbearbeitet.
                                        Wenn Sie die Übergangszeit in Stunden angeben, müssen Sie eine maximale
                                        Zeit angeben. Die Wahl der maximalen Zeit bestimmt, ob Wochenenden in die
                                        Planung einbezogen werden.

                                           Jede Zeitangabe bedeutet einen Wechsel der Schicht
                                           Mit der ersten Minute, die Sie als Übergangszeit in Stunden angeben, wird
                                           in die nächste Schicht gewechselt.


                                               Mittwoch         Donnerstag      Freitag          Montag




                                                    A     B                       C          D
                                        A Übergangszeit = 0                    C Übergangszeit zum nächsten Tag
                                        B Übergangszeit in die nächste Schicht D Übergangszeit zum Wochenende
                                        Abb. E-50       Übergänge in Stunden


                                        Die Schichtzeiten der unterschiedlichen Maschinen können unterschiedlich
                                        lang sein, z. B. kann der ESG-Ofen mit einer Schichtzeit von 6 Std. angege-
                                        ben sein, die ISO-Linie hat dagegen 8 Std.
                                        Wenn Sie mit solchen flatternden Schichtenden arbeiten, darf die Zeit nicht mit
                                        8 Std. angegeben werden. Um diese Problematik zu umgehen, können Sie
                                        einfach 6 Std. (B) angeben.
                                        Von Freitag 22 h bis Montag 14 h brauchen Sie eine Übergangszeit von min-
                                        destens 64 Std (D) für den optimalen Übergang. Nur mit dieser Übergangszeit
                                        lohnt sich das Stehenlassen des Glases über das Wochenende.
                                        An diesem Beispiel sehen Sie, dass die Definition von Übergangszeiten in
                                        Schichten sehr viel einfacher ist als der Übergang in Stunden.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-97
                 Stammdaten der Kapazitätsplanung                                                           Tutorial




                                       Schichtwechsel – Sonderfall
                                       Die Schleifmaschine im folgenden Beispiel arbeit in einer einzigen Schicht.
                                       Außerdem arbeitet sie sehr langsam. Wenn sie am Morgen bestückt wird,
                                       könnten die Scheiben am Schichtende zur nachfolgenden Maschine überge-
                                       hen.
                                       Die Übergangszeiten sind daher mit den folgenden Angaben definiert:
                                       •   Normal = 0 Schicht
                                       •   Max. = 1 Schicht
                                       •   Eil = 1 Schicht
                                       •   Min. = 0 Schicht


                                                                      Montag               Dienstag


                                              Schleifen
                                              Sonderkanten

                                              ESG




                                       Abb. E-51    Schichtwechsel in Bezug auf Maschine


                                       Die Übergangszeit von 1 Schicht bezieht sich auf die Schichten der Schleif-
                                       maschine. Daraus folgt, dass der Übergang in die nächste Schicht unabhän-
                                       gig vom Übergangstyp immer für den folgenden Tag berechnet wird.
                                       In diesem Fall ist es notwendig, die Übergangszeiten für die Schleifmaschine
                                       in Stunden zu definieren:
                                       •   Normal = 0 Std.
                                       •   Max. = 8 Std.
                                       •   Eil = 4 Std.
                                       •   Min. = 4 Std.


                                                                      Montag               Dienstag


                                              Schleifen
                                              Sonderkanten

                                              ESG




                                       Abb. E-52    Übergang in Stunden
4.50 / 01-2023




                                       Als Ergebnis dieser Einstellungen führt der maximale Übergang zum Ende der
                                       nachfolgenden Schicht auf der Folgemaschine. Die Zeiten für den Eilüber-




                 E-98                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                              Stammdaten der Kapazitätsplanung




                                             gang und den minimalen Übergang führen in die Mitte der nachfolgenden
                                             Schicht.


                                             Definition von Übergangszeiten
                                             Für die einzelnen logischen Maschinen legen Sie jeweils Übergangszeiten
                                             von allen Typen mit den entsprechenden Zeitangaben in Schichten an. In Aus-
                                             nahmefällen können Sie auch Zeitdauern mit der Angabe in Stunden verwen-
                                             den, z. B. für Trocknungszeiten.
                                             Daneben gibt es eine Reihe von produktionsbedingten Übergangszeiten, die
                                             nicht beschleunigt werden können, z. B. für Heat Soak oder Trocknungszeiten
                                             nach dem Siebdruck.
                                             Für den Fall, dass ein Übergang nicht zu einem Maschinenwechsel führt und
                                             kein expliziter Übergang zwischen zwei logischen Maschinen definiert ist, wird
                                             ein automatischer Übergang mit Übergangszeit 0 verwendet. Dadurch wird
                                             gewährleistet, dass unnötige Maschinenübergänge auch dann vermieden
                                             werden, wenn keine expliziten Übergänge definiert sind.
                                              “Erstellung der Maschinenwege” auf Seite E-17


                             A                     B                  C          D        E             F




                 A Station, von der die Scheibe kommt                  D Normale Übergangszeit in Stunden
                 B Station, zu der die Scheibe geht                    E Normale Übergangszeit in Schichten
                 C Art des Übergangs                                   F Maximale Übergangszeit in Stunden, Schichten
                 Abb. E-53       Übergangszeiten


                                             Übergangszeiten werden in der Regel in Schichten (E) definiert, können in
                                             Ausnahmefällen aber auch in Stunden (D) angegeben werden. In den Über-
                                             gangszeiten müssen Handlings- und Rüstzeiten berücksichtigt werden.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                    E-99
                 Stammdaten der Kapazitätsplanung                                                                    Tutorial




                                       •   Übergangszeiten in Schichten definieren Sie in ganzen Schichten.
                                       •   Übergangszeiten in Stunden definieren Sie in Blöcken von vier oder acht
                                           Stunden. Das ist den Schichten Ihrer Produktion angepasst und übersicht-
                                           lich. Die Übergangszeiten laufen auch über die arbeitsfreie Zeit, z .B. für
                                           das Aushärten von Silikonversiegelung übers Wochenende.
                                       Die Übergangszeiten werden hierarchisch abgearbeitet. Dabei gilt:
                                       •   Maschine x -> Maschine y beschreibt den expliziten Übergang zwischen
                                           zwei Maschinen.
                                       •   Maschine x -> Alle Maschinen beschreibt den Übergang am Ausgang von
                                           Maschine x.
                                       •   Alle Maschinen -> Maschine x beschreibt den Übergang am Eingang von
                                           Maschine x.
                                       •   Alle Maschinen -> Alle Maschinen beschreibt den allgemeinen Übergang
                                           und wird zuletzt ausgewertet, wenn keine andere Übergangszeit gefunden
                                           wurde.

                                       Übergangstypen
                                       Um die Übergangszeiten korrekt anlegen zu können, müssen Sie den optima-
                                       len Durchlauf Ihrer Produktion kennen. Das bedeutet, dass Sie genau wissen
                                       müssen, wie lange es dauert, bis die nachfolgende Bearbeitung ausgeführt
                                       werden kann. Ausgehend vom normalen (optimalen) Übergang können Sie
                                       dann bestimmen, um welche Zeit ein Übergang verkürzt werden kann.
                                       Die verschiedenen Typen von Übergangszeiten werden folgendermaßen ein-
                                       gesetzt:
                                       •   Im Typ Normal durchlaufen Scheiben die Produktion in der regulären Zeit,
                                           die dafür eingeplant wurde. Diese Zeiten gelten für den optimalen Produk-
                                           tionsablauf, d. h. ohne Ausfälle von Personal oder Maschinen, Bruch usw.
                                       •   Im Typ Eil wird die Produktion einzelner Scheiben beschleunigt, z. B., in-
                                           dem die Verweilzeiten verkürzt werden. Diese Übergangszeiten erhöhen
                                           jedoch die Kosten.
                                       •   Im Typ Minimal werden die sogenannten Chef-Aufträge durch die Produk-
                                           tion geführt. Dabei werden nur die Übergangszeiten berücksichtigt, die un-
                                           abdingbar für die Produktion sind, z. B. Verweilzeiten im VSG-Autoklav,
                                           Trocknung von Verklebungen. Minimale Übergänge sind die teuersten
                                           Übergangszeiten.
                                       •   Mit dem Typ Verboten wird ein Übergang von oder zu einer Maschine ge-
                                           sperrt, z. B. weil innerbetriebliche Transportwege erforderlich sind.

                                           Beispiel

                                           Bei einer Schleif-Bohrstraße kann mit der Einstellung Verboten z. B. erreicht
                                           werden, dass nur solche Scheiben auf die Bohrstation gelangen, die vorher
                                           auf der Schleifstation waren. Dazu würden Sie folgende Übergänge
                                           einrichten:
                                           • Verboten: Alle Maschinen -> Bohrstation
                                           • Normal: Schleifstation -> Bohrstation
4.50 / 01-2023




                 E-100                                                               A+W Production Kapazitätsplanung
                 Tutorial                                                                                   Stammdaten der Kapazitätsplanung




                                        Vorbereitung der Definition von Übergangszeiten
                                        Um die Übergangszeiten für Ihre Produktion zu ermitteln, können Sie zu-
                                        nächst eine Matrix erstellen. Die Matrix hilft, die Übergangszeiten zwischen
                                        den logischen Maschinen zu visualisieren.
                                        Unterscheiden Sie zwischen der Zeit beim Weggang und der Zeit bei Ankunft:
                                        •   Der Weggang nach dem Arbeitsprozess kann z. B. bedeuten, dass eine
                                            Scheibe nach einer Bearbeitung darauf wartet umgepackt zu werden.
                                        •   Die Ankunft am Eingang kann sich z. B. auf Vorarbeiten beziehen.




                                                                                                                       ISO Sprossenbau
                                                                 nach




                                                                                          Heat Soak




                                                                                                                                         ISO Linie
                                                                        Säumen




                                                                                                              Bohren
                                                                                 Bieger



                                                                                                      VSG
                                             von
                                             Wareneingang                 4        4                   4       4          4               4

                                             Zuschnitt                                                         4
                                                                                                                                                     Legende:
                                             Säumen                       0        0                   0                                  0
                                                                                                                                                     • Zahl:
                                             Bieger                                                                                       4
                                                                                                                                                       Übergangszeit in
                                             Heat Soak                                                 8                                  8            Stunden
                                                                                                               8                                     • Grün:
                                             VSG                                                                                          8
                                                                                                                                                       Übergangszeit
                                             Bohren                                                                                       4            bei Weggang
                                                                                                                                          4          • Rot:
                                             ISO Sprossenbau
                                                                                                                                                       Übergangszeit
                                             ISO Linie                                                                                    0            bei Ankunft



                                        Abb. E-54        Beispiel-Matrix für Übergangszeiten


                                        In diesem Beispiel sehen Sie, dass z. B. das Glas im Heat Soak immer acht
                                        Stunden verweilt. Daher beträgt die Übergangszeit vom Heat Soak zu allen
                                        anderen Arbeitsstationen immer 16 Stunden. Die so ermittelten Zeiten Ihrer
                                        Produktion rechnen Sie in Schichten um.
                                        Eine solche Matrix zeigt, dass Sie nur wenige Übergangszeiten zwischen den
                                        Arbeitsstationen definieren müssen. Alle anderen können Sie mit der Einstel-
                                        lung Von allen Maschinen -> Maschine X oder Von Maschine X -> alle anderen
                                        Maschinen definieren.
                                        Die Erstellung der Matrix und das Umsetzen im Dialog führen Sie am besten
                                        gemeinsam mit dem Service der A+W Software GmbH durch.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                                                                E-101
                 Stammdaten der Kapazitätsplanung                                                                Tutorial




                                           Übergangszeiten anlegen und verwalten
                                           In dieser Lerneinheit lernen Sie, wie Sie Übergangszeiten anlegen, bearbeiten
                                           oder löschen. Denken Sie daran, dass in den Übergangszeiten auch Rüstzei-
                                           ten und Handlingszeiten berücksichtigt werden müssen.
                                           Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                           •   “So legen Sie eine Übergangszeit an” auf Seite E-102
                                           •   “So bearbeiten Sie eine Übergangszeit” auf Seite E-104
                                           •   “So löschen Sie eine Übergangszeit” auf Seite E-104

                                               Voraussetzung
                                               Um Übergangszeiten anzulegen, müssen die entsprechenden logischen
                                               Maschinen in der Maschinenzuordnung definiert sein.


                                            So legen Sie eine Übergangszeit an
                                           1 Wählen Sie Stammdaten > Kapazitätsplanung > Übergangszeiten.
                                           2 Klicken Sie auf [Neu].


                     A        B                    C                       D         E                  F




                 A Neue Zeile                                         D Typ der Übergangszeit
                 B Maschine, von der das Teil ausgeht                 E Normale Übergangszeit in Stunden oder Schichten
4.50 / 01-2023




                 C Maschine, zu der das Teil kommt                    F Maximale Übergangszeit in Stunden oder Schichten
                 Abb. E-55    Übergangszeiten einrichten




                 E-102                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                           In der Liste der Maschinen wird oben eine neue Zeile eingefügt.
                                        3 Klicken Sie doppelt in das Feld (B), um den Dialog zur Auswahl der Maschi-
                                          ne zu öffnen.




                                        4 Übernehmen Sie die gewünschte Maschine mit einem Doppelklick.
                                        5 Wiederholen Sie den Schritt für die Maschine (C), zu der Sie den Übergang
                                          festlegen.
                                           Nutzen Sie auch die Möglichkeiten Alle Maschinen auf Maschine X und
                                           Maschine X auf Alle Maschinen.
                                        6 Wählen Sie den Typ (D) für die Übergangszeit aus und tragen Sie die zu-
                                          gehörige Zeit (E) ein.
                                           Verwenden Sie bevorzugt Schichten. In Ausnahmefällen können Sie auch
                                           Zeitdauern verwenden, z. B. Trockungszeiten.
                                        7 Tragen Sie die maximale Übergangszeit (F) ein.
                                           Damit erlauben Sie dem System, die Übergangszeit maximal zu dehnen.
                                           Verwenden Sie auch hier entweder Stunden oder Schichten.

                                           Tipp
                                           Wählen Sie für den Übergang zur letzten Bearbeitung, z. B. Verpacken
                                           oder Versand, die größte Übergangszeit, die möglich ist. Damit haben Sie
                                           in kritischen Situationen größere Flexibilität.

                                        8 Wiederholen Sie die Schritte 2 bis 7 für den nächsten Übergangstyp (D)
                                          derselben Maschinenkombination.
                                        9 Klicken Sie auf [OK], um die Daten zu speichern.
                                           Damit haben Sie die Übergangszeiten in den verschiedenen Übergangs-
                                           typen für einen Übergang angelegt.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-103
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                          So bearbeiten Sie eine Übergangszeit
                                         1 Wählen Sie Stammdaten > Kapazitätsplanung > Übergangszeiten.
                                         2 Korrigieren Sie die Übergangszeiten für die gewünschten Maschinen.
                                             Sie aktivieren die Felder mit einem Doppelklick.
                                         3 Ergänzen Sie ggf. eine Maschinenkombination, indem Sie die Daten für ei-
                                           nen anderen Übergangstyp anlegen.
                                             Folgen Sie dazu der Beschreibung in der Handlungssequenz zum Anlegen
                                             der Übergangszeiten.
                                         4 Klicken Sie auf [OK], um die Änderungen zu speichern.
                                             Damit haben Sie die Übergangszeiten geändert.


                                          So löschen Sie eine Übergangszeit
                                         1 Wählen Sie Stammdaten > Kapazitätsplanung > Übergangszeiten.
                                         2 Markieren Sie in der ersten Spalte die Übergangszeit, die Sie löschen wol-
                                           len.
                                             Die gesamte Zeile der Übergangszeit wird markiert.




                 Abb. E-56   Übergangszeiten löschen


                                         3 Klicken Sie auf [Löschen].
                                             Die Übergangszeit wird aus der Liste gelöscht.
                                             Falls Sie eine Übergangszeit versehentlich aus der Liste gelöscht haben,
                                             klicken Sie auf [Ende].
                                             Wenn Sie die Meldung mit [Nein] bestätigen, wird der Dialog geschlossen,
                                             ohne die Änderung zu speichern. Die Übergangszeit steht wieder in der
4.50 / 01-2023




                                             Liste, wenn Sie den Dialog erneut öffnen.
                                         4 Klicken Sie auf [OK], um den Dialog zu schließen.



                 E-104                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                         Stammdaten der Kapazitätsplanung




                                            Die Änderungen werden in die Datenbank übernommen.


                                        Übungen
                                        Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Ver-
                                        fügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung
                                        vollständig sind, können Sie die Planung für eigene Aufträge im Produktions-
                                        monitor testen.
                                        •   Legen Sie gemeinsam mit dem Trainer eine neue Maschine in der Maschi-
                                            nenzuordnung vollständig an, die Sie deutlich als Test-Maschine für die Ka-
                                            pazitätsplanung kennzeichnen.
                                        •   Definieren Sie die Übergangszeiten für diese Maschine im Eil- und Normal-
                                            raster.
                                        •   Legen Sie Übergangszeiten zwischen zwei Maschinen für alle Typen von
                                            Übergangszeiten an, die für die Übergänge erforderlich sind.
                                        •   Verändern Sie die Übergangszeiten.
                                        •   Prüfen Sie die Ergebnisse mit einem Testauftrag im Produktionsmonitor.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Übergangszeiten” auf Seite E-227
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                               E-105
                 Stammdaten der Kapazitätsplanung                                                                   Tutorial




                                       Vorgabezeiten
                                       Lernziele

                                       •   Was sind Vorgabezeiten?
                                       •   Wie werden Vorgabezeiten angelegt, bearbeitet oder gelöscht?
                                       •   Aus welchen Elementen bestehen Vorgabezeiten?
                                       •   Wie fließen die Elemente in Vorgabezeiten ein?
                                       •   Wie funktioniert der Formeltest?


                                       Nutzen

                                       • Mit Vorgabezeiten definieren Sie, wie lange ein Arbeitsschritt auf einer Maschine
                                         für eine Scheibe dauert. Zusammen mit den Übergangszeiten werden damit die
                                         Zeiten durch die Produktionsstationen berechnet.


                                       Merke

                                       Vorgabezeit =               Mit der Vorgabezeit legen Sie fest, wie lange ein
                                       Bearbeitungsdauer           Arbeitsgang auf einer spezifischen Maschine dauert.
                                                                   Die Bearbeitungsdauer wird anhand von Formeln
                                                                   berechnet.
                                                                   Vorgabezeiten werden in der Maschinenzuordnung
                                                                   (MZO) als Bearbeitungsdauer bezeichnet.

                                       Logische Maschinen          Vorgabezeiten werden zu den logischen Maschinen
                                                                   erstellt.

                                       Vorgabezeiten               Die Vorgabezeiten werden zur Kapazitätsplanung und
                                                                   zur Kostenkalkulation herangezogen.

                                       Formel                      Vorgabezeiten können mit Formeln berechnet werden,
                                                                   um verschiedene Einflussgrößen zu berücksichtigen,
                                                                   z. B. Fläche, Laufmeter, Stückzahl, Dicke.
                                                                   Komplexe Vorgabezeiten hinterlegen Sie als Formel in
                                                                   der Maschinenzuordnung.

                                       Element                     Eine Zeile in einer Vorgabezeitformel, z. B. eine
                                                                   Dickenabhängigkeit, der Zeitanteil für die Fertigung
                                                                   eines Ausschnitts an einem Bearbeitungszentrum oder
                                                                   ein Zeitzuschlag für schwere Scheiben.
                                                                   Elemente können separat erfasst und getestet werden.
                                                                   Es gibt feste Elemente, bedingte Ausdrücke,
                                                                   Schwellenwerte, gewichtete Ausdrücke (freie Elemente)
                                                                   und Vektoren. Als benutzerdefinierte Elemente lassen
                                                                   sich zusätzlich Tabellen und dreidimensionale
                                                                   Abhängigkeiten (Würfel) verarbeiten.
4.50 / 01-2023




                 E-106                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                        Definition der Vorgabezeiten
                                        Mit einer Vorgabezeit definieren Sie, wie die Dauer eines Arbeitsgangs an ei-
                                        ner logischen Maschine berechnet wird. Basis der Berechnung ist dabei z. B.
                                        die jeweilige Fläche oder Kantenlänge in der einzelnen Auftragsposition.




                                        Abb. E-57   Vorgabezeiten


                                        In diesem Dialog sind die logischen Maschinen aufgelistet, über die Bearbei-
                                        tungen gesteuert werden. Vorgabezeiten werden in A+W Production mit Vor-
                                        gabezeitformeln festgelegt. Die Vorgabezeitformeln definieren Sie im Dialog
                                        Vorgabezeitformel.

                                           Vorgabezeiten
                                           Die Vorgabezeiten werden in der Maschinenzuordnung (MZO) als Bearbei-
                                           tungsdauer bezeichnet. Da die Vorgabezeiten an den logischen Maschi-
                                           nen festgemacht werden, können Sie auch in der Maschinenordnung
                                           Formeln für Vorgabezeiten hinterlegen. Sie tun dies im MZO-Editor > Re-
                                           gister Logische Maschine > Feld Bearbeitungsdauer.
                                           Diese Formeln aus der MZO können nicht im Dialog Vorgabezeiten geän-
                                           dert werden.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-107
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                       Struktur von Vorgabezeitformeln
                                       Jede Vorgabezeitformel basiert auf einer Basiszeit, die in Sekunden angege-
                                       ben ist. Vorgabezeitformeln können mit vorgegebenen Elementen definiert
                                       werden. Daneben können Sie auch eigene Elemente erstellen und in der For-
                                       mel verwenden.

                                                    A                                         B         C       D




                                         E
                                       A Elemente der Vorgabezeitformel        D Reihenfolge der Elemente sortieren
                                       B Basiszeit in Sekunden                 E Multiplikator für die
                                       C Auswahl der Rechenoperation             Bearbeitungsmenge

                                       Abb. E-58    Vorgabezeitformel


                                       Mit jeder Zeile ist ein Zeitzuschlag angegeben, der entweder als Formel be-
                                       rechnet oder als Wert aus einer Tabelle ermittelt wird.
                                       Sie können in einer Vorgabezeitformel mehrere unterschiedliche Elemente (A)
                                       verwenden. Dazu wählen Sie jeweils das gewünschte Element aus, geben ei-
                                       nen Wert in Sekunden an und legen fest, wie der Wert in der Rechenoperation
                                       verwendet werden soll (C). Wichtig ist dabei, dass die Reihenfolge (D) korrekt
                                       sortiert ist. Das gilt insbesondere dann, wenn die nächste Rechenoperation
                                       auf dem Zwischenergebnis der vorausgegangenen Operation aufbaut.
                                       Die Basiszeit gilt dabei als Startwert. Alle weiteren Elemente der Formel sind
                                       daher Zuschläge auf den Startwert. Wenn Sie keine Basiszeit eintragen, bau-
                                       en alle Berechnungen auf dem Ergebnis des ersten Eintrags (A) auf.
4.50 / 01-2023




                                       Standardmäßig werden verschiedene Element zur Auswahl angeboten, die
                                       auch durch eigene Definitionen ergänzt werden können:
                                        “Editor für Formelelemente” auf Seite E-113


                 E-108                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                           Beispiel Gas und Modell

                                           Basiszeit                        23 s
                                           Faktor für Größe                 23 * Größenfaktor
                                           Faktor für Gas                   Zwischenergebnis * Gasfaktor
                                           Konstante für Modell             Zwischenergebnis + Modellkonstante


                                        Mit dieser Vorgabezeitformel können Sie Zeiten für Scheiben mit Gasfüllung
                                        und für Modelle berechnen. Wenn Sie aber VSG berechnen wollen, muss die
                                        Formel folgendermaßen aufgebaut werden:

                                           Beispiel VSG, Größe und Gas

                                           Basiszeit                        23 s
                                           Faktor VSG                       + VSG-Faktor
                                           Faktor für Größe                 Zwischenergebnis 1 * Größenfaktor
                                           Faktor für Gas                   Zwischenergebnis 2 + (23 * Gasfaktor)


                                        Feste Elemente
                                        Festen Elementen wird kein Wert zugewiesen, sondern lediglich angegeben,
                                        wie sich die Elemente auf die Vorgabezeitformel auswirken. Zur Berechnung
                                        werden die tatsächlichen Werte des Glases herangezogen. So wird z. B. für
                                        das Feste Element ’Dicke’ bei einer 4.00 mm dicken Scheibe der Wert 4 ermit-
                                        telt. Bei dem Festen Element ’Menge’ wird die Anzahl der Scheiben und bei
                                        einem Festen Element ’Fläche’ wird die Fläche der Scheiben ermittelt.
                                        Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitfor-
                                        meln an, wie der ermittelte Wert in der Vorgabezeitformel verwendet wird.

                                        Faktoren
                                        Mit einem Faktor können Sie einen Zeitzuschlag festlegen, der immer dann
                                        berechnet wird, wenn die Voraussetzung für die Anwendung des Faktors er-
                                        füllt ist.

                                           Beispiel

                                           Mit dem Faktor Wert für ’Große Scheibe’ legen Sie einen Zuschlag auf die
                                           Basiszeit fest, der immer für Übergrößen berechnet wird. Ab wann eine
                                           Scheibe als Übergröße gilt, geben Sie zu dem Faktor an.


                                        Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitfor-
                                        meln an, wie der ermittelte Wert in der Vorgabezeitformel verwendet wird.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                     E-109
                 Stammdaten der Kapazitätsplanung                                                               Tutorial




                                       Vektoren – Tabellen und Würfel
                                       Vektoren ermöglichen eine exakte Planung der Vorgabezeiten in Abhängigkeit
                                       von den Werkstückeigenschaften. Mit Vektoren können Sie die Vorgabezeit
                                       z. B. auf die Glasdicke, die zu bearbeitende Fläche, die Beschaffenheit der
                                       Kanten und das Verhältnis von Breite zu Höhe einer Scheibe abstimmen.




                                       Abb. E-59    Vektor ’Dicke -> Wert’ – Zeitzuschläge abhängig von der Scheibendicke


                                       Unterschiedliche Dicken von Scheiben berücksichtigen Sie z. B. mit dem Vek-
                                       tor ’Dicke  Wert’. Damit legen Sie Zeitzuschläge abhängig von der Dicke ei-
                                       ner Scheibe fest.
                                       Wenn Sie den Wert im Vektor ’Dicke  Wert’ als Tabelle festlegen, können Sie
                                       den Wert des Vektors staffeln, z. B. von 4.00 mm - 5.99 mm Dicke gilt der
                                       Wert 0.1, für 6.00 mm - 7.99 mm der Wert 0.2 usw.
                                       Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitfor-
                                       meln an, wie Vektoren in der Vorgabezeitformel verwendet werden.
4.50 / 01-2023




                 E-110                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                            Stammdaten der Kapazitätsplanung




                                        Eingabehilfe für Vektoren
                                        Vektoren werden im Dialog Vektor (Name) als Tabelle definiert. Diese Tabelle
                                        enthält pro Grenzwert (Staffelstufe) einen Zuschlagswert. Zum Anlegen einer
                                        solchen Tabelle stehen zwei Vorgehensweisen zur Verfügung:
                                        •   Sie geben die Werte einzeln in die Tabelle ein. Dabei legen Sie z. B. meh-
                                            rere Stufen von Dicken, Längen oder Gewichten fest und weisen diesen je-
                                            weils einen Wert zu.
                                        •   Sie lassen sich die Staffelstufen und die gestaffelten Werte berechnen.




                                        Abb. E-60     Eingabehilfe für Vektoren – Resultat


                                            Für diese Berechnung legen Sie einen Anfangs- und einen Endwert fest,
                                            z. B. 4.00 - 20.00 mm für die Dicke. Wenn Sie als Schrittgröße 2.00 mm an-
                                            geben, wird zwischen dem Anfangs- und dem Endwert alle 2.00 mm eine
                                            Stufe eingefügt.
                                            Wenn Sie als Startwert für den Zuschlag 0.1 und als Schrittgröße 0.1 an-
                                            geben, gilt für die erste Stufe der Wert 0.1, für alle weiteren Stufen wird die-
                                            ser Wert jeweils um 0.1 erhöht.
                                            Für die Tabelle ergibt sich daraus: Scheiben mit einer Dicke von 4,00 -
                                            5,99 mm haben den Wert 0.1, von 6.00 mm - 8.00 mm den Wert 0.2 usw.


                                        Berechnung von Zeitzuschlägen
                                        Im einfachsten Fall besteht eine Vorgabezeitformel lediglich aus einer Basis-
                                        zeit. Sie können z. B. für eine logische Maschine eine Basiszeit von
                                        30 Sekunden angeben. Damit ist festgelegt, dass jeder beliebige Arbeitsgang
                                        an dieser logischen Maschine 30 Sekunden dauert.
                                        In der Praxis ist die Dauer eines Arbeitsgangs jedoch von verschiedenen Ein-
4.50 / 01-2023




                                        flüssen abhängig, z. B. von der Dicke einer Scheibe oder von der Kantenlän-
                                        ge, die bearbeitet werden muss. Je dicker eine Scheibe und je länger die zu



                 A+W Production Kapazitätsplanung                                                                    E-111
                 Stammdaten der Kapazitätsplanung                                                                       Tutorial




                                       bearbeitende Kantenlänge, desto mehr Zeit nimmt ein Arbeitsgang in An-
                                       spruch.
                                       Um diese Abhängigkeiten zu berücksichtigen, können Sie Zeitaufschläge fest-
                                       legen. In der Vorgabezeitformel stehen dazu feste Elemente und/oder Vekto-
                                       ren zur Verfügung.
                                       Für die Vorgabezeitformel stehen folgende Elemente zur Wahl:
                                       •   Basiszeit oder Startwert.
                                       •   Zeitzuschlag als festes Element, z. B. die Glasdicke.
                                       •   Zeitzuschlag als fester Wert, z. B. für große Scheiben.
                                       •   Zeitzuschlag als Vektor, z. B. Staffelung nach Gewicht.
                                       •   Zeitzuschlag als Tabelle für Matrix, z. B. Kantenlänge.
                                       Basiszeit und Zeitzuschläge werden in Sekunden angegeben.

                                       Reihenfolge der Berechnungen
                                       Bei der Berechnung müssen Sie die Operatorrangfolge der Mathematik be-
                                       rücksichtigen: Multiplikation und Division werden vor Addition und Subtraktion
                                       gerechnet – es sei denn, Klammern geben die Reihenfolge vor.

                                           Beispiel

                                           1+2*4                    =9                     Multiplikation zuerst

                                           (1 + 2) * 4              = 12                   Klammer zuerst

                                           1 + (2 * 4)              =9

                                           4 * (1 + 2)              = 12

                                           6 + (9 / 3)              =9

                                           (6 + 9) / 3              =5


                                       Zur Berechnung der Zeitzuschläge stehen folgende Einstellungen zur Wahl:

                                       Einstellung           Bedeutung

                                       + Tabelle             Der Wert aus der Tabelle wird zum Zwischenergebnis addiert.

                                       + b * Wert            Die Basiszeit wird mit dem Wert multipliziert. Das Ergebnis der
                                                             Multiplikation wird zum Zwischenergebnis addiert.

                                       + Wert                Der Wert wird zum Zwischenergebnis addiert.

                                       * (1 + Wert)          Der Wert wird zu 1 addiert und das Ergebnis mit dem
                                                             Zwischenergebnis aus der vorausgehenden Zeile multipliziert.

                                       * Vektor              Das Ergebnis der vorausgehenden Zeile wird mit dem Wert
                                                             des Vektors multipliziert.

                                       Tab. E-1          Mögliche Einstellungen für die Vorgabezeitformel
4.50 / 01-2023




                                       Wenn die Berechnung mit der Ermittlung aus einer Formel beginnt, legen Sie
                                       als Startwert 0 fest, z. B. für die Berechnung einer Fläche, bevor der erste
                                       Siebdruck aufgetragen wird.

                 E-112                                                                 A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                        Wenn die Berechnung auf dem Ergebnis der vorausgehenden Zeile basiert,
                                        ist die Reihenfolge der Einträge wichtig.


                                        Editor für Formelelemente
                                        Für die Definition eigener Formelelemente steht ein Editor zur Verfügung, in
                                        dem Sie eigene Formeln anlegen oder eine vordefinierte Formel auswählen
                                        können.



                                        A
                                        B                                                                    E

                                        C                                                                    C
                                                                                                             F
                                        D




                                        A Name des Formelelements                 D Berechnungsfomel
                                        B Auswahl des Typs                        E Eingabeformat
                                        C Beschriftung                            F Unabhängiger Parameter
                                        Abb. E-61    Zeitformelelement erfassen


                                        Dem Formelelement geben Sie einen Namen (A), der in der Auswahl der
                                        Formelelemente angezeigt wird, und eine Beschriftung (C), die im Dialog Vor-
                                        gabezeitformel angezeigt wird. Die zweite Beschriftung wird vor dem Berech-
                                        nungswert angezeigt.
                                        Die unterschiedlichen Elementtypen (B) verwenden Sie für folgende Berech-
                                        nungen:
                                        •   Festes Element:
                                            Ausdrücke ohne Benutzereingabe, z. B. Langkante. Diese Einstellung soll-
                                            ten Sie nicht mehr für neue Definitionen verwenden. Sie ist durch Freies
                                            Element abgelöst worden.
                                        •   Bedingung:
                                            Ausdrücke mit einer Benutzereingabe, die verwendet wird, wenn die Be-
                                            dingung wahr ist.
                                        •   Freies Element:
                                            Ausdrücke, bei denen das Ergebnis mit der Benutzereingabe gewichtet
                                            wird, z. B. Sekunden pro Schleifmeter.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-113
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                       •   Schwellenwert:
                                           Ausdrücke, bei denen der Schwellenwert für die Bedingung einstellbar ist,
                                           ohne die Formeldefinition zu verändern, z. B. Mengenzuschlag ab Benut-
                                           zereingabe.
                                       •   Vektor:
                                           Ausdrücke, bei denen eine Tabelle mit Wertepaaren aus Mindestwerten
                                           und zu verwendenden Koeffizienten gepflegt wird.
                                       Die eigentliche Formeldefinition (D) des Elements können Sie als Formel
                                       schreiben oder eine vordefinierte Formel auswählen und anpassen. Bei Vek-
                                       toren können Sie die Definition nicht ändern, daher ist das Feld ausgeblendet.


                                       Beispiel – Vorgabezeit für die logische Maschine
                                       Zuschnitt
                                       Aus einer Produktionsstatistik haben Sie die Flächenabhängigkeit Ihres Zu-
                                       schnitts ermittelt. Außerdem wissen Sie, dass die Rundbogenmodelle im
                                       Schnitt 20 Sekunden länger dauern und der Tisch 10 % mehr Zeit fürs Rand-
                                       entschichten von ISO-Komponenten benötigt.
                                       Um schnell auf Produktionsveränderungen reagieren zu können, wollen Sie
                                       die komplette Vorgabezeitformel mit einem Steuerparameter auf schneller
                                       oder langsamer einstellen können.




                                       Abb. E-62    Beispiel – Vorgabezeitformel
4.50 / 01-2023




                 E-114                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                              Stammdaten der Kapazitätsplanung




                                        Zeile                     Definition    Erklärung

                                        Basiszeit                 0.95          Der Steuerparameter steht auf 95 % der
                                                                                Vorgabezeit, also auf schneller.

                                        Randentschichtung         * (1 + 0.1)   Der Zuschlag wird nur bei einer
                                                                                beschichteten Scheibe für ISO berechnet.

                                        Zuschnittfläche           * Vektor      Das Ergebniss wird mit den Zeiten für die
                                                                                Scheibenfläche multipliziert.

                                        Rundbogenmodell           + 20          Bei einem Modell mit Rundbogen werden 20
                                                                                Sekunden aufgeschlagen.

                                        Tab. E-2       Beispiel – Bedingungen der Berechnung

                                        Die eigentlichen Zeiten werden in dem Vektor für die Zuschnittsfläche ge-
                                        pflegt, z. B.:

                                         Fläche (qm)         Wert

                                         0.1                 70          bis 0.099 qm werden 70 Sekunden gerechnet

                                         0.5                 45          für 0.1 - 0.499 qm werden 45 Sekunden genrechnet

                                         1.0                 60          für 0.5 - 0.999 qm werden 60 Sekunden gerechnet

                                         2.0                 150         für 1.0 - 1.999 qm werden 150 Sekunden gerechnet

                                         3.0                 210         für 1.999 - 2.999 qm werden 150 Sekunden gerechnet


                                        In diesem Beispiel sehen Sie, dass für die ganz kleinen und für die großen
                                        Scheiben mehr Zeit für den Zuschnitt benötigt wird. Damit entfällt ein weiterer
                                        Größenzuschlag für den Zuschnitt. Für Flächenbearbeitungen kann ein sol-
                                        cher Zuschlag aber durchaus notwendig sein und muss dann an der entspre-
                                        chenden logischen Maschine definiert werden.

                                        Bedingung: Modell mit Rundbogen
                                        Die Bedingung soll nur dann die Benutzereingabe als Ergebnis liefern, wenn
                                        sie wahr ist.

                                           Definition (Beispiel)

                                           IF (($Parts_MODELL_NR >= 60 AND $Parts_MODELL_NR <= 81) OR
                                           ($Parts_MODELL_NR >= 113 AND $Parts_MODELL_NR <= 118) OR
                                           ($Parts_MODELL_NR >= 123 AND $Parts_MODELL_NR <= 125) OR
                                           ($Parts_MODELL_NR >= 133 AND $Parts_MODELL_NR <= 199))
                                           THEN 20 END

                                           Längenangabe in der Formel
                                           Beachten Sie, dass die Längenwerte in einer Formel in µm angegeben
                                           werden müssen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                        E-115
                 Stammdaten der Kapazitätsplanung                                                                 Tutorial




                                          Bedingung: Schwellenwert
                                          Bei mehr als 11 Stück soll die Vorgabezeit 10 % kleiner sein.

                                              Definition (Beispiel)

                                              IF ($Parts_MENGE > 11) THEN - 0.1 END


                                          Bedingung: Vektor für Modellzuschnitt
                                          Vektoren können von Einheiten abhängig sein oder auch nicht lineare Sach-
                                          verhalte darstellen. Falls Ihnen z. B. der einfache Zuschlag für Modelle mit
                                          Rundbögen nicht präzise genug ist, definieren Sie einen Vektor, mit dessen
                                          Hilfe Sie die benötigten Koeffizienten einfach und sehr präzise abfragen kön-
                                          nen.
                                          Im Dialog zur Erfassung eines Formelelements legen Sie dazu ein neues Ele-
                                          ment mit dem Elementtyp Vektor an. Für einen gültigen Vektor wählen Sie eine
                                          Formel für den unabhängigen Parameter, z. B. AWF_ShapeNumber.




                                          A
                                                                        B



                 A Vektor mit unabhängigem Parameter                    B Tabelle für Modellnummern
                 Abb. E-63   Vektor für modellabhängige Zeitzuschläge


                                          Die Tabelle erlaubt die modellabhängige Abstufung der Zuschläge. Der Ein-
                                          trag der linken Spalte gibt immer den Startwert des Gültigkeitsbereichs an. Es
                                          ist gute Praxis, ein Wertepaar für 0 zu definieren, damit der Wertebereich voll-
                                          ständig beschrieben ist.
4.50 / 01-2023




                 E-116                                                                A+W Production Kapazitätsplanung
                 Tutorial                                                         Stammdaten der Kapazitätsplanung




                                        Zeitformel-Objekte
                                        Sie können die Stückliste oder Teile der Stückliste als Formelobjekte abbilden,
                                        um die Kette der Bearbeitungen darzustellen. Diese Darstellung dient dazu,
                                        die Abhängigkeiten der Bearbeitungen in der Vorgabezeitformel zu testen,
                                        z. B. um zu prüfen, wie die Bearbeitung davon abhängt, was in der Gegen-
                                        scheibe gemacht wird. Formelobjekte werden zum Testen von Formeln mit lo-
                                        gischen Mengen verwendet.
                                        Formelobjekte sind immer auf eine bestimmte Vorgabezeitformel bezogen.
                                        Sie können nicht übergreifend verwendet werden. Sie speichern die Formel-
                                        objekte dann, wenn Sie einen Nachweis führen wollen, dass die Formel kor-
                                        rekt angewendet wird.




                                                                                                           E




                                                                                                           D




                                                        A         B                    C
                                        A Gesamtes Objekt speichern             D Markiertes Objekt löschen
                                        B Objekt löschen                        E Objekte
                                        C Objekt hinzufügen
                                        Abb. E-64    Stücklistenbaum aus der Sicht der einzelnen Bearbeitungen


                                        In diesem Beispiel sehen Sie die Bearbeitungsstückliste einer ISO-Scheibe.
                                        Beim Hinzufügen werden die Formelobjekte (E) nummeriert. Mit einem Dop-
                                        pelklick können Sie jedes Formelobjekt öffnen und umbenennen, z. B. das
                                        erste Objekt in ISO. Das ist sinnvoll, um die Struktur zu verdeutlichen. Beim
                                        Hinzufügen (C) wird unter dem markierten Objekt ein neues Objekt angelegt.
                                        Beim Löschen (D) wird das markierte Objekt mit allen Unterebenen gelöscht.

                                           Gespeichertes Objekt zum Testen laden
                                           Ein gespeichertes Formelobjekt kann nur für die Formel verwendet wer-
                                           den, zu der es angelegt wurde, z. B. um die Berechnung nach Änderungen
                                           in der Vorgabezeitformel zu testen. Daher ist es sinnvoll, beim Speichern
4.50 / 01-2023




                                           einen sprechenden Namen zu vergeben.




                 A+W Production Kapazitätsplanung                                                                E-117
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                       Ein Beispiel für ein Formelobjekt finden Sie zum Test der Vorgabezeitformel.
                                        “So testen Sie die Berechnung der Zeitformel” auf Seite E-126


                                       Vorgabezeitformeln anlegen und verwalten
                                       In dieser Lerneinheit erfahren Sie, wie Sie Vorgabezeitformeln anlegen, bear-
                                       beiten oder löschen.
                                       In der ersten Zeile im Dialog Vorgabezeitformeln können Sie Formelelemente
                                       als Vorlagen für alle Maschinen definieren. Wenn Sie für die Maschine 0 eine
                                       Zeitformel definieren, wird diese zwar in der Datenbank gespeichert, die For-
                                       mel wird jedoch nicht verwendet, da der Maschine 0 in der MZO keine Bear-
                                       beitung zugewiesen ist.

                                           Voraussetzung
                                           Vorgabezeitformeln werden zu den logischen Maschinen definiert, die ei-
                                           nen bestimmten Arbeitsgang ausführen. Daher müssen die entsprechen-
                                           den logischen Maschinen in der Maschinenzuordnung definiert sein.

                                       Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       •   “So definieren Sie eine Vorgabezeitformel” auf Seite E-119
                                       •   “So erstellen Sie einen Vektor mit der Eingabehilfe” auf Seite E-122
                                       •   “So löschen Sie eine Vorgabezeitformel” auf Seite E-124

                                           Komplexität von Vorgabezeitformeln
                                           A+W Production bietet die Möglichkeit, Vorgabezeitformeln beliebig kom-
                                           plex zu definieren. Somit lassen sich alle erdenklichen Sonderfälle abde-
                                           cken.
                                           Halten Sie Vorgabezeitformeln so einfach wie möglich. Sollte in Ihrer Pro-
                                           duktion der Einsatz einer komplexen Vorgabezeitformel nötig sein, setzen
                                           Sie sich bitte mit dem Kundenservice der A+W Software GmbH in Verbin-
                                           dung.
4.50 / 01-2023




                 E-118                                                            A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                         So definieren Sie eine Vorgabezeitformel
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten.




                                        Abb. E-65   Vorgabezeiten


                                        2 Markieren Sie die logische Maschine, für die Sie eine Vorgabezeitformel
                                          erstellen wollen.
                                        3 Klicken Sie auf [Bearbeiten].
                                           Der Dialog Vorgabezeitformel wird geöffnet.
                                           Wenn für die logische Maschine bereits in der Maschinenzuordnung eine
                                           Formel zur Bearbeitungsdauer hinterlegt wurde, wird eine Warnmeldung
                                           angezeigt. Wenn Sie den Vorgang fortsetzen, wird die in der Maschinenzu-
                                           ordnung hinterlegte Formel überschrieben.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-119
                 Stammdaten der Kapazitätsplanung                                                                Tutorial




                                                                                              A




                                         B                 C                 D                               E
                                       A Basiszeit                               D Formelelement hinzufügen
                                       B Multiplikator Bearbeitungsmenge         E Vordefinierte Formel hinzufügen
                                       C Aktuelle logische Maschine
                                       Abb. E-66      Vorgabezeitformel


                                       4 Geben Sie die Basiszeit (A) in Sekunden ein.
                                             Sie können entweder eine vordefinierte Formel hinzufügen (E) und die Da-
                                             ten speichern oder eine Formel mit Formelelementen aufbauen. In den fol-
                                             genden Schritten wird der Aufbau mit Formelelementen gezeigt.
                                       5 Klicken Sie auf [Neu] (D), um ein Element auszuwählen.
4.50 / 01-2023




                 E-120                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                        6 Wählen Sie das Element aus, z. B. einen Vektor, und übernehmen Sie die
                                          Auswahl mit [OK].
                                           Das ausgewählte Element wird im Dialog Vorgabezeitformel unter der Ba-
                                           siszeit eingefügt.

                                                                                           A           B




                                        A Werte festlegen                     B Berechnung festlegen
                                        Abb. E-67   Vorgabezeitformel mit neuem Element
4.50 / 01-2023




                                        7 Klicken Sie auf […] (A), um den Dialog zur Eingabe der Werte zu öffnen.




                 A+W Production Kapazitätsplanung                                                          E-121
                 Stammdaten der Kapazitätsplanung                                                                  Tutorial




                                          Wenn Sie einen Vektor anlegen, können Sie die Grenzwerte und die Zeit-
                                          werte manuell oder über die Eingabehilfe eintragen.
                                           “So erstellen Sie einen Vektor mit der Eingabehilfe” auf Seite E-122
                                       8 Wählen Sie den Operator (B) für die Berechnung aus.
                                       9 Wiederholen Sie die Schritte 5 - 8, um weitere Elemente hinzuzufügen.
                                       10 Prüfen Sie die Reihenfolge der Formelelemente.
                                          Die Reihenfolge ist für die Berechnung wichtig, wenn sich der Zuschlag auf
                                          die Zwischensumme des vorausgehenden Elements bezieht.
                                       11 Klicken Sie auf [OK], um die Daten zu übernehmen.
                                          Der Dialog wird geschlossen. Damit haben Sie eine Vorgabezeitformel zu-
                                          sammengestellt. Sie können die Berechnung prüfen und mit einem Formel-
                                          Objekt eine Berechnung mit Beispielgrößen starten.
                                           “Zeitformel testen” auf Seite E-125
                                           “Zeitformel-Objekte” auf Seite E-117


                                        So erstellen Sie einen Vektor mit der Eingabehilfe
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabe-
                                         zeitformel.
                                       2 Geben Sie die Basiszeit in Sekunden ein.
                                       3 Klicken Sie auf [Neu] und wählen Sie ein Element aus, z. B. Vektor ’Dicke
                                         -> Wert’.




                                          Tab. E-3      Vektor ’Dicke -> Wert’


                                       4 Klicken Sie auf [Eingabehilfe].
4.50 / 01-2023




                 E-122                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                           A



                                           B




                                           A Grenzwerte für die Staffelung          B Werte für den Zeitzuschlag
                                           Tab. E-4     Eingabehilfe für Vektoren


                                           Zunächst geben Sie die Grenzwerte für die Staffelung (A) und dann die
                                           Werte für den Faktor (B) ein. Aus diesen Angaben wird die Tabelle erstellt.
                                        5 Geben Sie den Startwert und den Endwert ein, z. B. 4.00 und 20.00.
                                           Diese Werte legen die kleinste und die größte Dicke fest.
                                        6 Geben Sie die Schrittgröße ein, z. B. 2.00.
                                           Dieser Wert legt fest, in welchen Schritten die Grenzwerte für die Staffelung
                                           zwischen dem Startwert und dem Endwert berechnet werden.
                                        7 Geben Sie die den Startwert und die Schrittgröße für den Faktor ein,
                                          z. B 0.1.
                                           Dieser Wert legt fest, um welche Größe der Faktor pro Grenzwert erhöht
                                           wird. Damit haben Sie alle notwendigen Werte eingetragen.
                                        8 Klicken Sie auf [OK], um die Berechnung der Tabelle zu starten.
                                           Der Dialog Eingabehilfe für Vektoren wird geschlossen. Die Tabellen wird
                                           berechnet und in den Dialog ’Vektor-> Dicke’ übernommen.
                                           Sie können die Daten korrigieren und ergänzen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                  E-123
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                       9 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Der Dialog Vektor ’Dicke -> Wert’ wird geschlossen. Die angelegte Staffe-
                                          lung wird in die Vorgabezeitformel übernommen.


                                        So löschen Sie eine Vorgabezeitformel
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabe-
                                         zeitformel.
                                       2 Markieren Sie das Element, das Sie löschen wollen.
                                       3 Klicken Sie auf [Löschen].
                                       4 Wiederholen Sie die Schritte 2 und 3, bis alle Elemente in der Liste entfernt
                                         sind, die nicht mehr benötigt werden.
                                       5 Setzen Sie die Basiszeit auf den Wert Null.
                                       6 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Der Dialog wird geschlossen.
                                          Um eine Vorgabezeitformel insgesamt zu löschen, markieren Sie die Vor-
                                          gabezeit im Dialog Vorgabezeiten und klicken Sie auf [Löschen].
4.50 / 01-2023




                 E-124                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                         Stammdaten der Kapazitätsplanung




                                        Zeitformel testen
                                        Im Dialog Zeitformeltest können Sie Formeln testen und damit die eingegebe-
                                        nen Werte und Berechnungseinstellungen prüfen. Sie können entweder die
                                        Formel testen, die Sie aktuell im Dialog Vorgabezeitformel bearbeiten, oder
                                        Sie laden eine gespeicherte Formel in den Dialog, um diese zu testen.
                                        Der Formeltest gibt ein Ergebnis aus, das die Zeit des jeweiligen Arbeitsgan-
                                        ges in Sekunden angibt.
                                        Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                        •   “So testen Sie die Zeitformel” auf Seite E-125
                                        •   “So testen Sie die Berechnung der Zeitformel” auf Seite E-126
                                        •   “So erstellen Sie eine Kopie der Zeitformelsyntax” auf Seite E-130
                                        Daneben können Sie Formelobjekte definieren, die Sie zum Testen aller For-
                                        meln verwenden können. Dort geben Sie den konkreten Fall an, in dem Sie
                                        die Formel testen wollen, also z. B. die Dicke und die Breite einer Scheibe. Da-
                                        mit haben Sie immer die gleichen Vorgaben für den Test. Diese Funktion ist in
                                        einer separaten Einheit beschrieben.
                                         “Zeitformel-Objekte” auf Seite E-117


                                         So testen Sie die Zeitformel
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabe-
                                          zeitformel.




                                        Abb. E-68    Vorgabezeitformel
4.50 / 01-2023




                                        2 Markieren Sie das Formelelement, das Sie testen wollen:



                 A+W Production Kapazitätsplanung                                                                E-125
                 Stammdaten der Kapazitätsplanung                                                         Tutorial




                                          Wenn Sie die gesamte Vorgabzeitformel testen wollen, müssen Sie das
                                          Element Basic Time markieren. Sie können aber auch jedes Element ein-
                                          zeln testen, indem Sie es markieren und die nachfolgenden Schritte aus-
                                          führen.
                                       3 Klicken Sie auf [Formeltest].




                                                                       A                B
                                          A Testergebnis                      B Auswertung starten
                                          Abb. E-69   Zeitformeltest


                                       4 Klicken Sie auf [Auswerten] (B).
                                          Das Berechnungsergebnis (A) wird angezeigt. Sie können die Formel ggf.
                                          weiter bearbeiten und korrigieren.
                                       5 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Um die Formel mit Scheibendaten zu testen, können Sie für den Test ein
                                          Formelobjekt anlegen und Werte eingeben.


                                        So testen Sie die Berechnung der Zeitformel
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabe-
                                         zeitformel.
                                          Der Dialog Vorgabezeitformel wird geöffnet.
                                       2 Klicken Sie auf [Formeltest].
4.50 / 01-2023




                 E-126                                                        A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                                                                                        A




                                                                                                        B




                                           A Objekt markieren                  B Objekt hinzufügen
                                           Abb. E-70   Zeitformel-Objekt


                                        3 Klicken Sie doppelt auf das Formelobjekt (A), um den Dialog zur Eingabe
                                          der Eigenschaften zu öffnen.

                                                            A                                B
4.50 / 01-2023




                                           A Frei wählbarer Name               B Auswahl des Typs
                                           Abb. E-71   Eigenschaften des Formel-Objekts



                 A+W Production Kapazitätsplanung                                                           E-127
                 Stammdaten der Kapazitätsplanung                                                         Tutorial




                                       4 Geben Sie einen Namen (A) ein und wählen Sie den Typ (B) aus, z. B. Teil.
                                       5 Klicken Sie auf [Hinzufügen].
                                          Die Felder in der Spalte Eigenschaften werden mit den Elementen vorbe-
                                          legt, die in der aktuellen Vorgabezeitformel enthalten sind.




                                          Abb. E-72   Werte für Formelobjekt eingeben


                                       6 Geben Sie zu jeder Eigenschaft die entsprechenden Werte ein, z. B. die
                                         Maße für Höhe und Breite.
                                          Beachten Sie, dass Sie die Maße in Mikrometer μm eingeben müssen.
                                       7 Klicken Sie auf [Schließen], um die Daten zu speichern und den Dialog zu
                                         schließen.
                                          Der Dialog Formeltest wird wieder im Vordergrund angezeigt.
4.50 / 01-2023




                 E-128                                                         A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                           Abb. E-73   Berechnung mit Zeitformel-Objekt


                                        8 Markieren Sie das Formelobjekt, für das die Berechnung gestartet werden
                                          soll.
                                        9 Klicken Sie auf [Formeltest].
                                           Das Ergebnis der Berechnung mit den eingegebenen Werten wird ange-
                                           zeigt. Wenn die Berechnung nicht Ihren Vorstellungen entspricht, können
                                           Sie die berechneten Werte prüfen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-129
                 Stammdaten der Kapazitätsplanung                                                         Tutorial




                                        So erstellen Sie eine Kopie der Zeitformelsyntax
                                       1 Testen Sie die Zeitformel wie in der vorausgehenden Handlungssequenz
                                         angegeben.




                                          A



                                          A Formel anzeigen
                                          Abb. E-74   Zeitformeltest


                                       2 Aktivieren Sie die Checkbox Formel anzeigen (A).




                                          Abb. E-75   Formelsyntax
4.50 / 01-2023




                                          In diesem Dialog können Sie die Syntax der kompletten Formel prüfen. Um
                                          die Syntax mit Unterstützung durch den A+W-Service zu korrigieren, ko-
                                          pieren Sie die Syntax und senden Sie den Text an A+W.



                 E-130                                                        A+W Production Kapazitätsplanung
                 Tutorial                                                         Stammdaten der Kapazitätsplanung




                                        Übungen
                                        •   Wählen Sie eine logische Maschine Ihrer Test-Maschinen und planen Sie
                                            auf dem Papier die Vorgabezeiten für diese logische Maschine:
                                            – Welche Scheiben werden auf der logischen Maschine bearbeitet?
                                            – Welche Faktoren benötigen Sie, um die Vorgabezeiten für diese Schei-
                                               ben zu definieren?
                                            – Wie sollen diese Faktoren in die Vorgabezeitformel einfließen?
                                        •   Stellen Sie die Vorgabezeitformel mit den benötigten Elementen zusam-
                                            men.
                                        •   Erfassen Sie für den Eintrag 0 - Alle Maschinen verschiedene Formelele-
                                            mente, z. B. einen eigenen Vektor, eine Tabelle, einen Schwellenwert.
                                        •   Legen Sie zu einer Formel ein Formelobjekt an und testen Sie die Vorga-
                                            bezeitformel, um zu prüfen, ob das Ergebnis Ihren Erwartungen entspricht.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Vorgabezeiten” auf Seite E-206
                                         Softwarereferenz, “Vorgabezeitformel” auf Seite E-208
                                         Softwarereferenz, “Tabelle, Vektor (Name)” auf Seite E-213
                                         Softwarereferenz, “Eingabehilfe für Vektoren” auf Seite E-214
                                         Softwarereferenz, “Erfassung eines Formelelements” auf Seite E-217
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-131
                 Stammdaten der Kapazitätsplanung                                                                  Tutorial




                                       Maschinengruppen
                                       Lernziele

                                       • Was sind Maschinengruppen in der Kapazitätsplanung?
                                       • Wie werden Maschinengruppen erstellt, bearbeitet oder gelöscht?


                                       Nutzen

                                       • Mit Maschinengruppen fassen Sie Maschinen eines Bereichs zusammen und
                                         steuern über die Mitarbeiteranzahl die Kapazität der Gruppe.


                                       Merke

                                       Maschinengruppen          Mit Maschinengruppen fassen Sie Maschinen von
                                                                 Bereichen zusammen, z. B. Zuschnitt oder
                                                                 Kantenbearbeitung.

                                       Personen                  Sie weisen Maschinengruppen jeweils eine
                                                                 Personenanzahl zu und legen damit die Kapazität der
                                                                 jeweiligen Maschinengruppe fest.

                                       Schichten                 Bei Maschinen einer Maschinengruppe müssen die
                                                                 Schichten übereinstimmen.

                                       Engpassbetriebsmittel     Ein Engpassbetriebsmittel kann nicht über seine
                                                                 Kapazität hinaus bebucht werden.
                                                                 Maschinen werden zu einem Engpassbetriebsmittel,
                                                                 wenn sie einer Maschinengruppe zugewiesen werden.

                                          Voraussetzung
                                          Bei allen Maschinen, die zu einer Maschinengruppe hinzugefügt werden,
                                          müssen die Schichten übereinstimmen. Dies umfasst die Start- und die
                                          Endzeit der Schichten.
4.50 / 01-2023




                 E-132                                                           A+W Production Kapazitätsplanung
                 Tutorial                                                          Stammdaten der Kapazitätsplanung




                                        Definition der Maschinengruppen
                                        Sie können Maschinen zu Gruppen zusammenfassen. Maschinengruppen
                                        sind für Maschinen des gleichen Bereichs sinnvoll. So könnten Sie z. B. eine
                                        Maschinengruppe Zuschnitt erstellen, der Sie alle Maschinen des Zuschnitts
                                        zuordnen. Eine festgelegte Kapazität gilt dann für die gesamte Maschinen-
                                        gruppe, also z. B. für den Zuschnitt.
                                        Sie können nur Maschinen zu einer Gruppe zusammenfassen, deren Schich-
                                        ten übereinstimmen, die also zur gleichen Zeit verfügbar sind. Maschinen, die
                                        Sie zu einer Maschinengruppe hinzufügen, werden automatisch zu einem
                                        Engpassbetriebsmittel.




                                        A                                                                              C




                                        B
                                                                                                                       D




                                        A Maschinengruppe                        C Anzahl der Personen in der Gruppe
                                        B Verfügbare Maschinen                   D Zugeordnete Maschinen
                                        Abb. E-76      Maschinengruppen


                                        Den Maschinengruppen müssen Sie jeweils eine Anzahl von Personen (C) zu-
                                        ordnen. A+W Production geht grundsätzlich davon aus, dass an jeder Maschi-
                                        ne eine Person arbeitet. Wenn Sie die Anzahl der Mitarbeiter in der Gruppe
                                        reduzieren, verringert sich die verfügbare Zeit pro Maschine.

                                            Beispiel

                                            In der Maschinengruppe Zuschnitt mit vier Maschinen werden vier Personen
                                            angenommen.
                                            Wenn die 4 Mitarbeiter 40 Stunden pro Woche arbeiten, sind 4 x 40 = 160
                                            Arbeitsstunden pro Woche verfügbar.
                                            Bei 3 Mitarbeitern sind nur noch 3 x 40 = 120 Arbeitsstunden pro Woche
4.50 / 01-2023




                                            verfügbar.




                 A+W Production Kapazitätsplanung                                                                 E-133
                 Stammdaten der Kapazitätsplanung                                                         Tutorial




                                       Maschinengruppen anlegen und verwalten
                                       In dieser Lerneinheit erfahren Sie, wie Sie Maschinengruppen anlegen, bear-
                                       beiten oder löschen.
                                       Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       •   “So legen Sie eine Maschinengruppe an” auf Seite E-134
                                       •   “So bearbeiten Sie eine Maschinengruppe” auf Seite E-136
                                       •   “So löschen Sie eine Maschinengruppe” auf Seite E-137


                                        So legen Sie eine Maschinengruppe an
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Maschinengruppen.




                                       Abb. E-77    Maschinengruppen


                                       2 Klicken Sie auf [Neu].




                                       3 Geben Sie einen Namen für die Maschinengruppe ein, z. B. Zuschnitt.
                                       4 Klicken Sie auf [OK].
4.50 / 01-2023




                 E-134                                                        A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                           Im Feld Maschinengruppen wird die neue Maschinengruppe angezeigt.
                                        5 Markieren Sie die neue Maschinengruppe.
                                           In der Liste Maschinen für Gruppe … werden alle verfügbaren Maschinen
                                           angezeigt.




                                        6 Markieren Sie die Maschine, die Sie zu der Gruppe hinzufügen wollen,
                                          z. B. 180 Schneidetisch 8.
                                        7 Klicken Sie auf den Pfeil nach rechts und bestätigen Sie die Meldung.
                                           Die Maschine wurde zur Gruppe hinzugefügt.
                                        8 Wiederholen Sie die Schritte 5 bis 7, um weitere Maschinen hinzuzufügen.




                                        9 Klicken Sie im Feld Maschinengruppen doppelt in die Spalte Personen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-135
                 Stammdaten der Kapazitätsplanung                                                            Tutorial




                                       10 Geben Sie die Anzahl der Personen ein, die in dieser Maschinengruppe ar-
                                          beiten.
                                       11 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Der Dialog wird geschlossen. Damit haben Sie die Maschinengruppe an-
                                          gelegt.


                                        So bearbeiten Sie eine Maschinengruppe
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Maschinengruppen.




                                          Abb. E-78    Markierte Maschinengruppe


                                       2 Markieren Sie im Feld Maschinengruppen die Maschinengruppe, die Sie
                                         bearbeiten wollen.
                                          In der Liste Maschinen für Gruppe … werden auf der rechten Seite alle Ma-
                                          schinen angezeigt, die der Gruppe zugeordnet sind. Auf der linken Seite
                                          werden die verfügbaren Maschinen angezeigt.
                                       3 Markieren Sie eine Maschine, die Sie aus der Gruppe entfernen oder zur
                                         Gruppe hinzufügen wollen.
                                       4 Klicken Sie auf den Pfeil nach links oder den Pfeil nach rechts, um eine Ma-
                                         schine aus der Gruppe zu entfernen oder um sie zur Gruppe hinzuzufügen.
                                       5 Wiederholen Sie die Schritte 3 bis 4, um weitere Maschinen aus der Grup-
                                         pe zu entfernen oder zur Gruppe hinzuzufügen.
                                       6 Korrigieren Sie im Feld Maschinengruppen die Anzahl der Personen.
4.50 / 01-2023




                                       7 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Die Änderungen werden gespeichert und der Dialog wird geschlossen.



                 E-136                                                          A+W Production Kapazitätsplanung
                 Tutorial                                                        Stammdaten der Kapazitätsplanung




                                         So löschen Sie eine Maschinengruppe
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Maschinengruppen.
                                        2 Markieren Sie im Feld Maschinengruppen die Maschinengruppe, die Sie
                                          löschen wollen.
                                        3 Klicken Sie auf [Löschen].
                                            Die Maschinengruppe wird aus der Liste entfernt. Damit ändern Sie die
                                            verfügbare Kapazität für die Einlastung.
                                        4 Klicken Sie auf [OK], um die Daten zu speichern.
                                            Die Änderungen werden gespeichert und der Dialog wird geschlossen.


                                        Übungen
                                        Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Ver-
                                        fügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung
                                        vollständig sind, können Sie die Planung für eigene Aufträge im Produktions-
                                        monitor testen.
                                        •   Erarbeiten Sie, welche Maschinen Sie zu Gruppen zusammenfassen wol-
                                            len.
                                        •   Erstellen Sie mindestens eine Maschinengruppe im Dialog Maschinen-
                                            gruppen.
                                        •   Bearbeiten Sie Ihre Maschinengruppe.
                                        •   Löschen Sie eine Ihrer Maschinengruppen.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Maschinengruppen” auf Seite E-245
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-137
                 Stammdaten der Kapazitätsplanung                                                                     Tutorial




                                       Lastverteilung
                                       Lernziele

                                       • Was ist die Lastverteilung in der Kapazitätsplanung?
                                       • Wie wird eine Lastverteilung erstellt, bearbeitet oder gelöscht?


                                       Nutzen

                                       • Die Lastverteilung ist bei Maschinen mit einer Spezialqualifikation sinnvoll. Wenn
                                         diese Qualifikation nicht abgerufen wird, wird die Maschine für die
                                         Standardbearbeitung genutzt.


                                       Merke

                                       Physikalische Maschine      Sie können eine Lastverteilung nur für eine Maschine
                                                                   einrichten, die als Engpassbetriebsmittel definiert ist.
                                                                   Sie können z. B. auf der Maschine 30 % für Modelle
                                                                   freihalten, die aber für Rechtecke verwendet werden
                                                                   dürfen, wenn keine Modelle eingelastet sind.

                                       Logische Maschinen          Die Lastverteilung wird unter den logischen Maschinen
                                                                   vorgenommen, die zu derselben physikalischen
                                                                   Maschine definiert sind. Damit können Sie die
                                                                   Lastverteilung eines CNC-Centers mit z. B. den drei
                                                                   logischen Maschinen Sonderkanten, Ausschnitte und
                                                                   Bohrungen prozentual aufteilen. Diese Lastverteilung
                                                                   wird bei der Einlastung berücksichtigt.

                                       Engpassbetriebsmittel       Ein Engpassbetriebsmittel kann nicht über seine
                                                                   Kapazität hinaus bebucht werden.
4.50 / 01-2023




                 E-138                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                            Stammdaten der Kapazitätsplanung




                                        Definition der Lastverteilung
                                        Die Lastverteilung wird unter den logischen Maschinen festgelegt, die zu
                                        derselben physikalischen Maschine definiert sind. Damit legen Sie den pro-
                                        zentualen Anteil der logischen Maschinen an der Gesamtkapazität der physi-
                                        kalischen Maschine fest.
                                        Lastverteilung nutzen Sie, um zu gewährleisten, dass eine Maschine eine ga-
                                        rantierte Mindestkapazität für Spezialaufgaben freihält, z. B. für den Modellzu-
                                        schnitt. Wenn die freigehaltene Kapazität nicht für Modelle genutzt wird,
                                        können auch Rechtecke bearbeitet werden. Diese Lastverteilung ist nur bei
                                        Maschinen möglich und sinnvoll, die als Engpassbetriebsmittel definiert sind.




                                        A
                                        B

                                        C                                                                                  D




                                        A Physikalische Maschine                   C Logische Maschinen
                                        B Bearbeitung freischalten                 D Anteile an der Gesamtkapazität
                                        Abb. E-79      Lastverteilung


                                        Sie teilen die Kapazität einer Maschine auf, indem Sie den zugehörigen logi-
                                        schen Maschinen (C) prozentuale Anteile (D) zuordnen.

                                            Beispiel

                                            Eine Maschine kann Formen bearbeiten, also Rechtecke und Modelle. Damit
                                            diese Spezialqualifikation nicht von den einfacheren Rechtecken belegt wird,
                                            halten Sie z. B. 30 % für Modelle frei. Diese Lastverteilung wird bei der
                                            Einlastung berücksichtigt.
                                            Wenn diese 30 % aber nicht für Modelle gebraucht werden, können auch
                                            Rechtecke bearbeitet werden.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                     E-139
                 Stammdaten der Kapazitätsplanung                                                             Tutorial




                                       Lastverteilung einrichten und bearbeiten
                                       In dieser Lerneinheit erfahren Sie, wie Sie Lastverteilungen einrichten, bear-
                                       beiten oder löschen.
                                       Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       •   “So richten Sie eine Lastverteilung ein” auf Seite E-140
                                       •   “So bearbeiten Sie eine Lastverteilung” auf Seite E-142
                                       •   “So löschen Sie eine Lastverteilung” auf Seite E-143

                                           Voraussetzung
                                           Sie können eine Lastverteilung nur für eine Maschine einrichten, die als
                                           Engpassbetriebsmittel definiert ist.


                                        So richten Sie eine Lastverteilung ein
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Lastverteilung.




                                           A
                                           B




                                           A Maschine                               B Felder freischalten
                                           Abb. E-80    Lastverteilung definieren


                                       2 Wählen Sie die Maschine (A) aus, deren Kapazität Sie aufteilen wollen.
                                           In der Auswahl-Liste sind nur die Maschinen freigeschaltet, die als Eng-
                                           passbetriebsmittel definiert sind.
4.50 / 01-2023




                 E-140                                                              A+W Production Kapazitätsplanung
                 Tutorial                                                       Stammdaten der Kapazitätsplanung




                                           Abb. E-81    Logische Maschinen


                                           Die zugehörigen logischen Maschinen werden in der Liste angezeigt.
                                        3 Aktivieren Sie die Checkbox Prüfung aktivieren (B), um die Felder freizu-
                                          schalten.
                                           Die Felder der logischen Maschinen werden freigeschaltet. Ist noch keine
                                           Lastverteilung angegeben, steht in der rechten Spalte unbegrenzt.
                                        4 Klicken Sie doppelt in die rechte Spalte.




                                        5 Geben Sie den Prozentwert für die Kapazität ein.
                                        6 Wiederholen Sie die Schritte 4 bis 5, um bei allen logischen Maschinen den
                                          Anteil an der Gesamtkapazität der physikalischen Maschine einzurichten.
                                        7 Deaktivieren Sie die Checkbox Prüfung aktivieren, um versehentliche Än-
                                          derungen zu verhindern.
                                        8 Klicken Sie auf [OK], um die Daten zu speichern und den Dialog Lastver-
                                          teilung zu schließen.
                                           Die Daten werden gespeichert und der Dialog wird geschlossen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-141
                 Stammdaten der Kapazitätsplanung                                                           Tutorial




                                        So bearbeiten Sie eine Lastverteilung
                                       1 Wählen Sie Stammdaten > Kapazitätsplanung > Lastverteilung.




                                          A
                                          B




                                          A Maschine                               B Felder freischalten
                                          Abb. E-82    Lastverteilung definieren


                                       2 Wählen Sie die Maschine (A), deren Lastverteilung Sie bearbeiten wollen.
                                          In der Auswahl-Liste sind nur die Maschinen freigeschaltet, die als Eng-
                                          passbetriebsmittel definiert sind.
                                       3 Aktivieren Sie ggf. die Checkbox Prüfung aktivieren (B).
4.50 / 01-2023




                                          Abb. E-83    Lastverteilung der ausgewählten Maschine




                 E-142                                                             A+W Production Kapazitätsplanung
                 Tutorial                                                           Stammdaten der Kapazitätsplanung




                                        4 Ändern Sie bei allen logischen Maschinen den Prozentwert für die Kapazi-
                                          tät.
                                        5 Deaktivieren Sie ggf. die Checkbox Prüfung aktivieren.
                                        6 Klicken Sie auf [OK], um die Daten zu speichern.
                                            Die Änderungen werden gespeichert und der Dialog wird geschlossen.


                                         So löschen Sie eine Lastverteilung
                                        1 Wählen Sie Stammdaten > Kapazitätsplanung > Lastverteilung.
                                        2 Wählen Sie im Feld Physikalische Maschinen die Maschine, deren Last-
                                          verteilung Sie löschen wollen.
                                            Die zugehörigen logischen Maschinen werden in der Liste angezeigt.
                                        3 Aktivieren Sie die Checkbox Prüfung aktivieren.
                                            Die Felder werden freigeschaltet.
                                        4 Ändern Sie bei allen logischen Maschinen den Prozentwert für die Kapazi-
                                          tät auf 000%.
                                            In den Feldern wird unbegrenzt angezeigt.
                                        5 Deaktivieren Sie ggf. die Checkbox Prüfung aktivieren.
                                        6 Klicken Sie auf [OK], um die Daten zu speichern.
                                            Die Änderungen werden gespeichert und der Dialog wird geschlossen. Da-
                                            mit haben Sie die Lastverteilung für die Maschine gelöscht.


                                        Übungen
                                        Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Ver-
                                        fügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung
                                        vollständig sind, können Sie die Planung für eigene Aufträge im Produktions-
                                        monitor testen.
                                        •   Prüfen Sie, bei welchen Ihrer Maschinen eine Lastverteilung sinnvoll ist.
                                            Legen Sie ggf. zuvor weitere logische Maschinen zu Ihren Test-Maschinen
                                            an.
                                        •   Richten Sie mindestens eine Lastverteilung ein.
                                        •   Bearbeiten Sie eine Lastverteilung.
                                        •   Löschen Sie eine Lastverteilung.


                                        Ergänzende Informationen
                                         Softwarereferenz, “Lastverteilung” auf Seite E-247
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-143
                 Stammdaten der Kapazitätsplanung                            Tutorial
4.50 / 01-2023




                 E-144                              A+W Production Kapazitätsplanung
Kapazitätsplanung                E

                    Softwarereferenz




                A+W Production
                 Softwarereferenz                                                                            Überblick




                                        Überblick
                                        Für die Planung und Organisation der Kapazitäten Ihrer Produktion steht der
                                        Dialog Produktionsmonitor zur Verfügung. In diesem werden die Arbeits-
                                        schichten pro Maschine angezeigt.
                                        Die Aufträge werden positionsweise eingelastet, wobei die Einlastung pro Po-
                                        sition erfolgreich sein muss. Wenn eine Auftragsposition nicht erfolgreich ein-
                                        gelastet werden kann, wird der gesamte Auftrag nicht eingelastet.
                                        Damit die Berechnungen im Produktionsmonitor korrekt ablaufen, müssen die
                                        Stammdaten der Kapazitätsplanung eingerichtet werden. Die Beschreibung
                                        der Dialoge ist zu Themengruppen zusammengefasst. Sie folgt nicht der An-
                                        ordnung der Dialoge in der Softwarereferenz.
                                        In dieser Softwarereferenz finden Sie Informationen zu folgenden Themen:
                                        •   “Einlastung” auf Seite E-148
                                        •   “Kampagnen und Reservierungen” auf Seite E-187
                                        •   “Bearbeitungen” auf Seite E-200
                                        •   “Stammdaten für Zeiten” auf Seite E-205
                                        •   “Stammdaten der Schichten” auf Seite E-230
                                        •   “Maschinen und Kosten” auf Seite E-242
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                               E-147
                 Einlastung                                                                 Softwarereferenz




                              Einlastung
                              Der Produktionsmonitor ist der zentrale Kapazitäts- und Auftrags-Leitstand
                              und der Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlas-
                              tung.
                              In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                              •   “Produktionsmonitor” auf Seite E-149
                              •   “Angezeigte Maschinen” auf Seite E-153
                              •   “Einstellungen” auf Seite E-154
                              •   “Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)” auf Seite E-157
                              •   “Neuen Filter erstellen” auf Seite E-160
                              •   “Maschine (Name)” auf Seite E-161
                              •   “Schichten für Maschine anpassen” auf Seite E-163
                              •   “Schichteigenschaften” auf Seite E-164
                              •   “Reservierungsanzeige” auf Seite E-166
                              •   “Arbeitsplan aus Produktionsmonitor” auf Seite E-167
                              •   “Einlastung” auf Seite E-171
                              •   “Stücklistenkonfiguration” auf Seite E-172
                              •   “Aktion” auf Seite E-173
                              •   “Umlastung” auf Seite E-174
                              •   “Maschinenumlastung” auf Seite E-178
                              •   “Nachbearbeitung Einlastung” auf Seite E-179
                              •   “Fehlerhafte Aufträge” auf Seite E-182
                              •   “Asynchrone Verarbeitung” auf Seite E-183
                              •   “Änderung bereits verplanter Aufträge” auf Seite E-184
                              •   “Positionssplit” auf Seite E-185
4.50 / 01-2023




                 E-148                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                                   Einlastung




                                             Produktionsmonitor
                                             Anzeigen > Produktionsmonitor
                                             Detailanzeige > Kontextmenü > Produktionsmonitor




                 Abb. E-84   Produktionsmonitor


                                             In diesem Dialog werden die aktuelle Planung der Produktion und die kapazi-
                                             tive Auslastung der Maschinen pro Arbeitsschicht angezeigt. Damit ist der
                                             Produktionsmonitor der zentrale Kapazitäts- und Auftrags-Leitstand und der
                                             Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlastung.
                                              Tutorial, “Produktionsmonitor” auf Seite E-22

                                             Schaltflächen

                 Symbol      Funktion                                     Beschreibung

                             Ausgewählte Maschinen                         “Angezeigte Maschinen” auf Seite E-153


                             Einstellungen                                 “Einstellungen” auf Seite E-154


                             Anzeigeart für alle Maschinen ändern         Auswahl der Anzeige für alle Maschinen:
                                                                          •   Zeit
4.50 / 01-2023




                                                                          •   Menge
                                                                          •   Fläche
                                                                          •   Gewicht



                 A+W Production Kapazitätsplanung                                                                      E-149
                 Einlastung                                                                                    Softwarereferenz




                 Symbol       Funktion                                    Beschreibung

                              Anzeige ändern (Schicht, Tag, Woche)        Ändert die Anzeige. Die Maschinenkapazität wird
                                                                          entweder pro Arbeitsschicht, Tag oder Woche
                                                                          angezeigt

                              Ansicht umschalten                          Schaltet die Ansicht um.
                                                                          • Hauptansicht:
                                                                            Alle Schichten im angegebenen Zeitraum werden
                                                                            angezeigt.
                                                                          • Detailansicht:
                                                                            Nur die Schichten des angegebenen Tags werden
                                                                            angezeigt.

                              Vergrößern, Verkleinern                     Vergrößert, verkleinert die Darstellung der
                                                                          Arbeitsschichten.

                              Ansicht aktualisieren                       Aktualisiert die Ansicht.


                              Gegebene Anzahl von Tagen zurück, vor       Verschiebt den angezeigten Zeitraum um die Anzahl
                                                                          der Tage vor oder zurück, die im Feld Tage angegeben
                                                                          ist.

                              Ansicht filtern, Filter entfernen            “Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)”
                                                                            auf Seite E-157


                                              Starttermin Öffnet den Kalender, um den Starttag für die Anzeige der Ar-
                                              beitsschichten auswählen.

                                              Tage Angabe, um wie viele Tage die Anzeige mit den Schaltflächen jeweils
                                              vor- oder zurückgestellt werden soll.

                                              Eingabefeld Filter Eingabe des Filterkriteriums, die Anzeige nach Aufträgen
                                              oder Läufen zu filtern.

                                                  Darstellung
                                                  Die Darstellung kann individuell angepasst werden. Dies betrifft z. B. die
                                                  Farben, ein Zeitraster, Statusinformationen usw.

                                                   “Einstellungen” auf Seite E-154

                                              Arbeitsschichten
                                              Im Produktionsmonitor werden die Arbeitsschichten aller ausgewählten Ma-
                                              schinen angezeigt. Maschinen, die als Engpassbetriebsmittel definiert sind,
                                              werden in roter Schrift angezeigt. Ein Engpassbetriebsmittel kann nicht über seine
                                              Kapazität hinaus bebucht werden.
4.50 / 01-2023




                 E-150                                                                    A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                         Einlastung




                                        Über das Kontextmenü stehen folgende Informationen zur Verfügung:
                                        •   Eigenschaften:
                                            Öffnet einen Dialog, in dem Sie die Anzeige der Maschineneigenschaften
                                            ändern können.
                                             “Maschine (Name)” auf Seite E-161
                                        •   Schichteigenschaften:
                                            Öffnet einen Dialog, in dem Sie Schichtzeiten der Maschine anpassen kön-
                                            nen.
                                             “Schichten für Maschine anpassen” auf Seite E-163
                                        •   Logische Maschinen anzeigen:
                                            Mit diesem Eintrag kann die Darstellung der logischen Maschinen aktiviert
                                            und deaktiviert werden. Bislang musste man dazu den entsprechenden
                                            Schalter im Stammdaten-Dialog ändern. Bei Verwendung des Kontextme-
                                            nüs wird nicht der in den Stammdaten hinterlegte Wert geändert, es wird
                                            nur die Anzeige angepasst, so dass die Änderung nur temporär ist.
                                             “Misc” auf Seite E-162

                                        Status der Planung
                                        Die Farben der Punkte zeigen die Rückstände an:
                                        •   Grün: Keine Rückstände.
                                        •   Gelb: Rückstände, die mit der freien Kapazität noch am aktuellen Tag auf-
                                            geholt werden können.
                                        •   Rot: Rückstände, die nicht mehr am aktuellen Tag aufgeholt werden kön-
                                            nen.

                                        Anzeige der Arbeitsschichten
                                        Im Tooltipp zu einer Arbeitsschicht wird eine Kurzinformation zum Status an-
                                        gezeigt.
                                        Über das Kontextmenü stehen folgende Informationen zur Verfügung:
                                        •   Arbeitsplan:
                                            Öffnet den Dialog Arbeitsplan: Selektion aus A+W Production Monitor mit
                                            dem Überblick über die Läufe und Aufträge der Maschine und Schicht.
                                             “Arbeitsplan aus Produktionsmonitor” auf Seite E-167
                                        •   Löschen:
                                            Löscht eine markierte Arbeitsschicht aus dem Produktionsmonitor.
                                        •   Schichteigenschaften:
                                            Öffnet den Dialog Schichteigenschaften, um die Eigenschaften einer
                                            Schicht zu ändern.
                                             “Schichteigenschaften” auf Seite E-164
                                        •   Reservierungen anzeigen:
                                            Öffnet den Dialog Reservierungsanzeige, um die Reservierungen einer
                                            Schicht zu prüfen.
                                             “Reservierungsanzeige” auf Seite E-166
4.50 / 01-2023




                                        Schraffiert Die Dauer der Arbeitsschicht ist herabgesetzt.

                                        X Die Arbeitsschicht ist deaktiviert.



                 A+W Production Kapazitätsplanung                                                             E-151
                 Einlastung                                                                   Softwarereferenz




                              ! Die Arbeitsschicht ist auf Aktiv für Eilaufträge gesetzt und steht damit nur für
                              Eilaufträge zur Verfügung.

                              ? In der Arbeitsschicht sind undefinierte Bearbeitungen eingelastet.

                              Rahmen Die Arbeitsschicht ist als Engpass definiert.
                               “Schichteigenschaften” auf Seite E-164
4.50 / 01-2023




                 E-152                                                   A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                              Einlastung




                                        Angezeigte Maschinen
                                        Anzeigen > Produktionsmonitor > [Ausgewählte Maschinen]




                                        Abb. E-85    Angezeigte Maschinen


                                        In diesem Dialog wählen Sie die Maschinen aus, die im Dialog Produktions-
                                        monitor angezeigt werden. Dabei können Sie auch die Reihenfolge festlegen.
                                        Maschinen, die als Engpassbetriebsmittel definiert sind, werden in der Liste in
                                        roter Schrift angezeigt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität
                                        hinaus bebucht werden.

                                        Checkbox Angabe, ob eine Maschine im Dialog Produktionsmonitor ange-
                                        zeigt wird.
                                         Die Maschine wird nicht angezeigt.
                                         Die Maschine wird angezeigt.

                                        [Pfeil nach oben], [Pfeil nach unten] Verschiebt die markierte Maschine
                                        um eine Stelle nach oben oder nach unten.

                                        [OK] Speichert und übernimmt die Auswahl und schließt den Dialog.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                  E-153
                 Einlastung                                                                   Softwarereferenz




                              Einstellungen
                              Anzeigen > Produktionsmonitor > [Einstellungen]




                              Abb. E-86    Einstellungen – Felder nach Kategorien angezeigt


                              In diesem Dialog können Sie die Anzeige im Dialog Produktionsmonitor ein-
                              stellen, z. B. ob Maschinengruppen und Rückstände angezeigt werden. Au-
                              ßerdem können Sie die Anzeige der Farben für Arbeitsschichten, Engpässe
                              oder Überlasten festlegen.

                              [Kategorien] Sortiert die Elemente nach Kategorien.

                              [Alphabetisch] Sortiert die Elemente alphabetisch.

                              [Eigenschaften] Zur Zeit nicht genutzt.

                              Andere Einstellungen
                              •   Anzahl an Tagen vor Startdatum:
                                  Angabe, wie viele Tage vor dem aktuellen Startdatum angezeigt werden.
                              •   Behandlung von Maschinengruppen:
                                  Angabe, ob Maschinengruppen angezeigt werden.
4.50 / 01-2023




                              •   Behandlung von Rückständen:
                                  Angabe, ob Rückstände angezeigt werden.




                 E-154                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                       Einlastung




                                        Darstellung
                                        •   Abgearbeitet:
                                            Farbe, in der abgearbeitete Aufträge angezeigt werden.
                                        •   Aktualisierungszeit:
                                            Angabe des Intervalls in Sekunden, in dem die Anzeige im Dialog Produk-
                                            tionsmonitor aktualisiert wird.
                                        •   Ausgewählte Schichten:
                                            Farbe, in der die ausgewählte Arbeitsschicht angezeigt wird.
                                        •   Auslastung in Grafik anzeigen:
                                            Angabe, ob die Auslastung als Text angezeigt wird.
                                        •   Automatische Aktualisierung:
                                            Angabe, ob die Anzeige automatisch aktualisiert wird.
                                        •   Eingelastet:
                                            Farbe, in der eingelastete Aufträge angezeigt werden.
                                        •   Engpass:
                                            Farbe, in der Engpässe angezeigt werden.
                                        •   Engpassfarbe:
                                            Schriftfarbe für Engpassbetriebsmittel.
                                        •   Farbe für Hinweissymbole:
                                            Farbe, in der Hinweissymbole in den Arbeitsschichten angezeigt werden.
                                        •   Freie Reservierungszeit:
                                            Farbe, in der unbebuchte Reservierungen angezeigt werden.
                                        •   Intensität des 3D-Effekts:
                                            Auswahl, in welcher Intensität der 3D-Effekt angezeigt wird.
                                        •   Schicht:
                                            Farbe, in der Arbeitsschichten angezeigt werden.
                                        •   Stunden anzeigen:
                                            Angabe, ob ein Stunden-Raster hinter die Schichten gelegt wird.
                                        •   Überlast:
                                            Farbe, in der eine Überlast angezeigt wird.
                                        •   Verplant:
                                            Farbe, in der verplante Arbeitsschichten angezeigt werden.
                                        •   Verplante Arbeitsgänge:
                                            Farbe, in der verplante Arbeitsgänge angezeigt werden.
                                        •   Zeit anzeigen:
                                            Angabe, ob ein Zeitraster angezeigt wird.
                                        •   Zeitfarbe:
                                            Farbe, in der die Zeit angezeigt wird.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-155
                 Einlastung                                                                Softwarereferenz




                              Detaildarstellung
                              •   Arbeitsgänge mit fertigen Vorprodukten:
                                  Angabe, ob Arbeitsgänge mit fertigen Vorprodukten angezeigt werden.
                              •   Intensität des 3D-Effekts:
                                  Angabe der Intensität des 3D-Effekts für grafische Elemente im Produkti-
                                  onsmonitor.
                              •   Produktionsfreigabe (mengenbasiert):
                                  Farbe, in der mengenbasierte Produktionsfreigaben angezeigt werden.
                              •   Produktionsfreigabe (zeitbasiert):
                                  Farbe, in der zeitbasierte Produktionsfreigaben angezeigt werden.
                              •   Stati anzeigen:
                                  Auswahl, ob neben der Maschine der Status für Rückstände angezeigt
                                  wird.
                              •   Unverplant (mengenbasiert):
                                  Farbe, in der unverplante Arbeitsschichten angezeigt werden. Die Anzeige
                                  ist mengenbasiert.
                              •   Unverplant (zeitbasiert):
                                  Farbe, in der unverplante Arbeitsschichten angezeigt werden. Die Anzeige
                                  ist zeitbasiert.
                              •   Verplant (mengenbasiert):
                                  Farbe, in der verplante Arbeitsschichten angezeigt werden. Die Anzeige ist
                                  mengenbasiert.
                              •   Verplant (zeitbasiert):
                                  Farbe, in der verplante Arbeitsschichten angezeigt werden. Die Anzeige ist
                                  zeitbasiert.
                              •   Vorprodukte fertig (mengenbasiert):
                                  Farbe, in der fertige Vorprodukte angezeigt werden. Die Anzeige ist men-
                                  genbasiert.
                              •   Vorprodukte fertig (zeitbasiert):
                                  Farbe, in der fertige Vorprodukte angezeigt werden. Die Anzeige ist zeitba-
                                  siert.

                              [OK] Speichert und übernimmt die Auswahl und schließt den Dialog.
4.50 / 01-2023




                 E-156                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                          Einlastung




                                        Bitte wählen Sie einen Auftrag / Lauf aus
                                        (Filtern)
                                        Anzeigen > Produktionsmonitor > [Ansicht filtern]
                                        In diesem Dialog können Sie Aufträge, Läufe und selbst erstellte Filter aus-
                                        wählen, nach denen die Ansicht im Produktionsmonitor gefiltert werden soll.
                                        Der Dialog enthält folgende Register:
                                        •   “Filter – Aufträge” auf Seite E-157
                                        •   “Filter – Läufe” auf Seite E-158
                                        •   “Filter – Eigene Filter” auf Seite E-159


                                        Filter – Aufträge
                                        Anzeigen > Produktionsmonitor > [Ansicht filtern] > Aufträge




                                        Abb. E-87     Bitte wählen Sie einen Auftrag/Lauf aus – Aufträge


                                        Im diesem Register sind die definierten Aufträge angezeigt. Sie können je-
                                        weils einen Auftrag auswählen. Die Anzeige im Produktionsmonitor wird auf
                                        den gewählten Auftrag eingeschränkt.

                                        Auftragsnummer Auftragsnummer, nach der gefiltert werden soll.

                                        Kunde Kundenname, nach dem gefiltert werden soll. Die Liste der Aufträge
                                        wird auf den Kunden eingeschränkt.

                                        Anzahl der Sätze Angabe, wie viele Aufträge in der Liste angezeigt werden.

                                        [OK] Speichert die Daten.
4.50 / 01-2023




                                        [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.




                 A+W Production Kapazitätsplanung                                                             E-157
                 Einlastung                                                                  Softwarereferenz




                              Filter – Läufe
                              Anzeigen > Produktionsmonitor > [Ansicht filtern] > Läufe




                              Abb. E-88    Bitte wählen Sie einen Auftrag/Lauf aus – Läufe


                              In diesem Register sind die definierten Läufe angezeigt. Sie können jeweils ei-
                              nen Lauf auswählen. Die Anzeige im Produktionsmonitor wird auf den gewähl-
                              ten Lauf eingeschränkt.

                              Laufnummer Laufnummer, nach der gefiltert werden soll.

                              Laufbeschreibung Laufbeschreibung, nach der gefiltert werden soll. Die Lis-
                              te der Läufe wird auf den Lauf eingeschränkt.

                              Anzahl der Sätze Angabe, wie viele Läufe in der Liste angezeigt werden.

                              [OK] Speichert die Daten.

                              [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-158                                                   A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                              Einlastung




                                        Filter – Eigene Filter
                                        Anzeigen > Produktionsmonitor > [Ansicht filtern] > Eigene Filter




                                        Abb. E-89    Bitte wählen Sie einen Auftrag/Lauf aus – Eigene Filter


                                        In diesem Register werden die selbst definierten Filter angezeigt.

                                        [Neu] Öffnet den Dialog Neuen Filter erstellen, in dem Sie eigene Filter defi-
                                        nieren können.

                                        [OK] Speichert die Daten.

                                        [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                 E-159
                 Einlastung                                                               Softwarereferenz




                              Neuen Filter erstellen
                              Anzeigen > Produktionsmonitor > [Ansicht filtern] > Register Eigene Filter >
                              [Neu]




                              Abb. E-90   Neuen Filter erstellen


                              In diesem Dialog können Sie eigene Filter für die Suche im Produktionsmoni-
                              tor erstellen. Sie erstellen die Filter in der Datenbanksprache SQL.

                                 Eigene Filter erstellen
                                 Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH,
                                 wenn Sie spezielle Filter zur Suche im Produktionsmonitor brauchen.

                              Name Name für den Filter.

                              Beschreibung Beschreibung für den Filter.

                              SQL Definition des Filters in SQL.

                              [OK] Speichert die Daten.

                              [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-160                                                 A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                          Einlastung




                                        Maschine (Name)
                                        Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Eigenschaften




                                        Abb. E-91    Maschine (Name)


                                        In diesem Dialog ändern Sie die Eigenschaften der Maschine im Produktions-
                                        monitor.

                                        [Kategorien] Sortiert die Elemente nach Kategorien.

                                        [Alphabetisch] Sortiert die Elemente alphabetisch.

                                        [Eigenschaften] Zur Zeit nicht genutzt.

                                        Eigenschaften der Maschine
                                        •   ID:
                                            Identifikationsnummer der Maschine.
                                        •   Erfassungsstelle:
                                            Identifikationsnummer der Erfassungsstelle.
                                        •   Name:
                                            Name der Maschine.
                                        •   Engpass:
                                            Auswahl, ob die Maschine ein Engpassbetriebsmittel ist. Engpassbetriebs-
                                            mittel werden im Produktionsmonitor in der Liste der Maschinen in roter
                                            Schrift angezeigt.
                                        •   Anzeigeart:
                                            Auswahl, in welcher Einheit die Schichtinfo den Status Fertig anzeigt. Zur
                                            Auswahl stehen:
                                            – Prozent
                                            – Menge
                                            – Fläche
4.50 / 01-2023




                                            – Gewicht
                                            – Laufmeter
                                            – Bearbeitung


                 A+W Production Kapazitätsplanung                                                              E-161
                 Einlastung                                                              Softwarereferenz




                              •   Gruppe:
                                  Maschinengruppe, zu der die Maschine gehört.
                              •   Leistung pro Anzeigenart ändern:
                                  Angabe der Einheit, in der die Leistung der Maschine angezeigt wird.

                              Misc
                              •   Logische Maschinen anzeigen:
                                  Auswahl, ob im Produktionsmonitor zur markierten Maschine auch die lo-
                                  gischen Maschinen angezeigt werden, z. B. zur Maschine Drilling (Bohr-
                                  maschine).

                              [OK] Speichert die Daten.

                              [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-162                                                A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                        Einlastung




                                        Schichten für Maschine anpassen
                                        Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Schichteigen-
                                        schaften




                                        Abb. E-92   Schichten für Maschine anpassen


                                        In diesem Dialog können Sie die Arbeitsschichten für die jeweilige Maschine
                                        bezogen auf Wochentage anpassen.

                                        Wochentage Angabe, für welche Wochentage die Änderung der Arbeits-
                                        schicht gilt.
                                         Die Arbeitsschicht wird für diesen Wochentag nicht geändert.
                                         Die Arbeitsschicht wird für diesen Wochentag geändert.

                                        Schichtnummer Angabe der Schichtnummer.

                                        Kapazität Angabe der Schichtkapazität an den markierten Wochentagen.

                                        [OK] Speichert die Daten.

                                        [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-163
                 Einlastung                                                                Softwarereferenz




                              Schichteigenschaften
                              Anzeigen > Produktionsmonitor > Anzeige der Schichten > Kontextmenü >
                              Schichteigenschaften




                              Abb. E-93    Schichteigenschaften


                              In diesem Dialog können Sie die Eigenschaften einer Arbeitsschicht bezogen
                              auf eine Maschine anzeigen lassen.

                              [Kategorien] Sortiert die Elemente nach Kategorien.

                              [Alphabetisch] Sortiert die Elemente alphabetisch.

                              [Eigenschaften] Zur Zeit nicht genutzt.

                              Eigenschaften der Schicht
                              •   Datum:
                                  Datum der markierten Arbeitsschicht.
                              •   Schichtnummer:
                                  Nummer der markierten Arbeitsschicht.
                              •   Start, Ende:
                                  Start- und Endezeit aus den Stammdaten der markierten Arbeitsschicht.
                              •   Kapazität:
                                  Zeit in Stunden, die in der Arbeitsschicht zur Verfügung stehen. Sie können
                                  die Kapazität einer Arbeitsschicht ändern. Die verkleinerte Kapazität wird
                                  im Produktionsmonitor schraffiert angezeigt.
                              •   Kommentar:
                                  Bemerkung zu den manuellen Änderungen der aktuellen Arbeitsschicht.
4.50 / 01-2023




                 E-164                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                            Einlastung




                                        •   Status:
                                            Status einer Arbeitsschicht. Im Auswahlmenü wählen Sie unter folgenden
                                            Optionen:
                                            – Aktiv: Die Arbeitsschicht ist für die jeweilige Maschine verfügbar.
                                            – Deaktiviert: Die Arbeitsschicht ist für die jeweilige Maschine nicht ver-
                                               fügbar. Die Schicht wird im Produktionsmonitor mit einem X markiert.
                                                “Anzeige der Arbeitsschichten” auf Seite E-151
                                            – Aktiv für Eilaufträge: Die Arbeitsschicht steht für die jeweilige Maschine
                                              ausschließlich für Eilaufträge zur Verfügung. Die Arbeitsschicht wird im
                                              Produktionsmonitor mit einem ! markiert.
                                        •   Engpass:
                                            Auswahl, ob die Arbeitsschicht ein Engpass ist. Ein Engpassbetriebsmittel
                                            kann nicht über seine Kapazität hinaus bebucht werden.

                                        [OK] Speichert die Daten.

                                        [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-165
                 Einlastung                                                                                Softwarereferenz




                                           Reservierungsanzeige
                                           Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Reservierung an-
                                           zeigen




                 Abb. E-94    Übersicht – Reservierungen


                                           In diesem Dialog werden alle Reservierungen der aktuellen Schicht angezeigt.
                                           Abgelaufene oder abgesagte Reservierungen sollten Sie löschen.
                                            Tutorial, “So löschen Sie eine Reservierung” auf Seite E-60
4.50 / 01-2023




                 E-166                                                                A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                              Einlastung




                                        Arbeitsplan aus Produktionsmonitor
                                        Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan
                                        In diesem Dialog können Sie sich einen Überblick zu einer bestimmten Ar-
                                        beitsschicht verschaffen.
                                        Der Dialog enthält folgende Register:
                                        •   “Arbeitsplan – Details” auf Seite E-168
                                        •   “Arbeitsplan – Übersicht” auf Seite E-170

                                        Kontextmenü
                                        Über das Kontextmenü zu den Läufen können Sie andere Dialoge öffnen, um
                                        sich Details zum gewählten Lauf anzeigen zu lassen.
                                        Über das Kontextmenü zu den Spalten können Sie folgende Einträge wählen:

                                        Eintrag                Funktion

                                        Umsortieren            Spalte aufsteigend oder absteigend sortieren. Wirkt sich
                                                               auf die ersten drei Spalten aus.

                                        Formatieren            Format oder Einheit auswählen, z. B. Datumsformate
                                                               oder Längen-Einheiten.

                                        Einfügen               Öffnet die Auswahl für Spalten, die in den verschiedenen
                                                               Kategorien eingefügt werden können.

                                        Entfernen              Löscht die markierte Spalte.

                                        Definition anzeigen    Öffnet den Dialog Spaltendefinition, in dem Details zur
                                                               jeweiligen Spalte angezeigt werden.


                                        Schaltflächen
                                        Die Funktionen der Schaltflächen sind ausführlich im Part Grobplanung be-
                                        schrieben.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                   E-167
                 Einlastung                                                                              Softwarereferenz




                                            Arbeitsplan – Details
                                            Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan > De-
                                            tails




                 Abb. E-95    Arbeitsplan: Selektion aus Produktionsmonitor – Details


                                            In diesem Register können Sie sich einen Überblick zu den geplanten Läufen
                                            in einer bestimmten Arbeitsschicht verschaffen. Sie können für die markierten
                                            Einträge Glasarten prüfen, Details prüfen und Läufe starten. Diese Funktionen
                                            sind ausführlich im Part Grobplanung beschrieben.

                                            Spalten
                                            Über das Kontextmenü können Sie die Spalten auswählen, um sich die ge-
                                            wünschten Informationen anzeigen zu lassen, z. B.:
                                            •   Lauf:
                                                Angabe des Laufs.
                                            •   Auftrag:
                                                Auftragsnummer.
                                            •   Pos (int Pos):
                                                Nummer der internen Position.
                                            •   Teile-Nr:
                                                Teilenummer.
                                            •   Sequenz:
                                                Sequenznummer der Bearbeitung.
                                            •   Bearbnr:
4.50 / 01-2023




                                                Artikelnummer der Bearbeitung.
                                            •   MZO-Maschine:
                                                Nummer der Maschine, auf der die Bearbeitung durchgeführt wird.


                 E-168                                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                         Einlastung




                                        Summenzeile
                                        In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen,
                                        z. B.:
                                        •   Menge Soll Gesamt:
                                            Gesamtmenge und Menge in den markierten Läufen.
                                        •   Dauer gesamt:
                                            Gesamte Bearbeitungsdauer der markierten Läufe in Stunden.

                                        Filter

                                        [Filter hinzufügen] Fügt einen Filter ein.

                                        Dropdown-Menü Auswahl eines Filters:
                                        • Klick: Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
                                        • Rechtsklick: Öffnet einen Dialog, um den aktuellen Filter zu bearbeiten.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-169
                 Einlastung                                                                                Softwarereferenz




                                           Arbeitsplan – Übersicht
                                           Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan >
                                           Übersicht




                 Abb. E-96    Arbeitsplan: Selektion aus Produktionsmonitor – Übersicht


                                           In diesem Register können Sie sich einen Überblick zu den Bearbeitungsty-
                                           pen verschaffen, die in der gewählten Arbeitsschicht an einer Maschine aus-
                                           geführt werden.
                                           Die Anzeige der Spalten können Sie auf die gleiche Weise einrichten, wie im
                                           Register Details.
4.50 / 01-2023




                 E-170                                                                    A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                          Einlastung




                                        Einlastung
                                        Anzeigen > Einlastung




                                        Abb. E-97    Einlastung


                                        In diesem Dialog prüfen Sie Aufträge, die als XML-Daten aus A+W Business
                                        oder A+W Enterprise importiert werden. Mit Öffnen des Dialogs werden die
                                        Aufträge automatisch importiert. Nach dem Import wird im Feld Status die ak-
                                        tuelle Uhrzeit angezeigt.
                                        Wenn in A+W Production ein automatischer Import der Aufträge eingerichtet
                                        ist, müssen Sie den Dialog Einlastung nicht öffnen. Der Datenimport läuft dann
                                        als Hintergrundprozess. Sie können den Prozess der Einlastung über den
                                        A+W Service Monitor verfolgen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-171
                 Einlastung                                                              Softwarereferenz




                              Stücklistenkonfiguration
                              Stammdaten > Einlastung > Stücklistenkonfiguration




                              Abb. E-98   Stücklistenkonfiguration


                              In diesem Dialog können Sie die Stücklistenkonfiguration analysieren.

                                 Keine Änderungen der Stücklistenkonfiguration
                                 Änderungen im Dialog Stücklistenkonfiguration bedeuten einen tiefen Ein-
                                 griff in die Struktur von A+W Production. Ändern Sie die Stücklistenkonfi-
                                 guration auf keinen Fall. Bei Fragen wenden Sie sich bitte an den
                                 Kundenservice der A+W Software GmbH.
4.50 / 01-2023




                 E-172                                                A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                         Einlastung




                                        Aktion
                                        Stammdaten > Einlastung > Stücklistenkonfiguration > [Neu], [Ändern]




                                        Abb. E-99   Stücklistenkonfiguration – Aktion


                                        In diesem Dialog können Sie die einzelnen Aktionen zur Stücklistenmanipula-
                                        tion analysieren. Jede Aktion besteht aus mindestens einer Bedingung, bei
                                        deren Zutreffen die hinterlegte Funktion ausgeführt wird.

                                           Keine Änderungen der Stücklistenkonfiguration
                                           Änderungen im Dialog Stücklistenkonfiguration bedeuten einen tiefen Ein-
                                           griff in die Struktur von A+W Production. Ändern Sie die Stücklistenkonfi-
                                           guration auf keinen Fall. Bei Fragen wenden Sie sich bitte an den
                                           Kundenservice der A+W Software GmbH.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-173
                 Einlastung                                                                            Softwarereferenz




                                          Umlastung
                                          Anzeige > Produktionsmonitor > Doppelklick auf Schicht > > Kontextmenü >
                                          Arbeitsplan > Umlastung
                                          Anzeige > Aufträge > Kontextmenü > Bearbeitungen > Kontextmenü > Ar-
                                          beitsplan > Umlastung
                                          Anzeige > Läufe > Kontextmenü > Bearbeitungen > Kontextmenü > Arbeits-
                                          plan > Umlastung




                 Abb. E-100   Umlastung


                                          In diesem Dialog können Sie Bearbeitungen aus Aufträgen oder Läufen auf
                                          andere Termine und Maschinen umlasten.
                                           Tutorial, “Umlastungen” auf Seite E-37

                                          1. Wählen Sie umzulastende Bearbeitungen aus
                                          Liste der Bearbeitungen, die umgelastet werden können.
                                          •   Auftrag:
                                              Liste der Bearbeitungen, sortiert nach Datum und Maschinen.
                                          •   Position:
                                              Positions-Nummer der jeweiligen Bearbeitung.
                                          •   Produktionstermin:
4.50 / 01-2023




                                              Bisheriger Termin, an dem die Bearbeitung durchgeführt werden soll.
                                          •   Schicht:
                                              Bisherige Arbeitsschicht, in der die Bearbeitung durchgeführt werden soll.


                 E-174                                                               A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                        Einlastung




                                        •   Geschützt:
                                            Anzeige, ob der Termin geschützt ist.
                                        •   Arbeitsgang:
                                            Arbeitsgang, mit dem die Bearbeitung durchgeführt wird.
                                        •   Logische Maschine:
                                            Logische Maschine, die für die Bearbeitung verwendet wird.
                                        •   Menge:
                                            Teilemenge, die bei der Bearbeitung hergestellt wird.
                                        •   Maschine:
                                            Maschine, auf der die Bearbeitung durchgeführt wird.
                                        •   Teilenummer:
                                            Nummer der Stücklistenkomponente.
                                        •   Sequenz:
                                            Sequenz der Bearbeitung.
                                        •   BearbNr:
                                            Bearbeitungs-Nummer der Bearbeitung.
                                        •   Bestell-Information:
                                            Angabe, ob Bestellteile enthalten sind.

                                        Einlastung erzwingen Sie können die Einlastung auf einen bestimmten Ter-
                                        min erzwingen.
                                         Die Termin-Umlastung wird nicht erzwungen.
                                         Die Termin-Umlastung wird erzwungen. Mit dieser Einstellung werden die
                                        Kapazitätsgrenzen von Engpassbetriebsmitteln nicht berücksichtigt. Daher
                                        werden die Arbeitsschichten ggf. überbucht.

                                        Erlaube Eilraster Sie können für die Umlastung festlegen, dass die Über-
                                        gangszeiten vom Typ Eil verwendet werden.
                                         Die Termin-Umlastung wird mit den normalen Übergangszeiten berechnet.
                                         Die Termin-Umlastung wird mit den Eil-Übergangszeiten berechnet.

                                        Kombobox (Schutz) Auswahl, ob Termine vor Umlastungen geschützt sind.
                                        In der Regel setzen Sie den Schutz nach einer erfolgreichen Umlastung.
                                        • Geschützte Bearbeitungstermine beibehalten:
                                            Geschützte Bearbeitungstermine werden nicht umgelastet.
                                        • Umlastungsziele schützen:
                                            Die nach der Umlastung berechneten neuen Termine werden vor weiteren
                                            Umlastungen geschützt.
                                        • Alle Bearbeitungstermine schützen:
                                            Alle Bearbeitungstermin der markierten Läufe werden geschützt.
                                        • Bearbeitungsschutz aufheben:
                                            Der Schutz für alle Bearbeitungstermine der markierten Läufe wird aufge-
                                            hoben.

                                        Begründung Wenn Sie für die Umlastung auch einen Termin in der Vergan-
                                        genheit zulassen wollen, müssen Sie eine Begründung eingeben. Damit wird
                                        die entsprechende Checkbox freigeschaltet.
4.50 / 01-2023




                                         “Erlaube Zieltermine in der Vergangenheit” auf Seite E-176




                 A+W Production Kapazitätsplanung                                                            E-175
                 Einlastung                                                               Softwarereferenz




                              Tage für automatische Lieferterminverschiebung Angabe, um wie viele
                              Tage der Liefertermin verschoben werden darf.

                                 Umlasten und Versandtermin
                                 Der Versandtermin ist bei der Umlastung geschützt, um die Anforderungen
                                 des ERP-Systems zu erfüllen. Der Versandtermin bleibt bestehen, solange
                                 Sie ihn nicht explizit umlasten.
                                 Halten Sie Rücksprache mit dem Auftragserfasser, falls Sie einen Versand-
                                 termin verändern wollen.

                              Als Chefauftrag umlasten Sie können die Bearbeitung mit oberster Priori-
                              tät umlasten.
                               Die Bearbeitung wird mit der normalen Priorität umgelastet.
                               Die Bearbeitung wird mit oberster Priorität umgelastet. Die Aufträge werden
                              mit den minimalen Übergangszeiten eingelastet. Dabei können auch die Zei-
                              ten von Kampagnen genutzt werden. Verwenden Sie diese Einstellung nur in
                              Notfällen.

                              Ignoriere Wareneingangstermine Manche Bearbeitungen sind davon ab-
                              hängig, dass zugekaufte Teile angeliefert sein müssen, z. B. die Fertigung ei-
                              ner ISO-Scheibe mit einem ESG, das nicht selbst produziert wird.
                               Für die Fertigung wird ein Wareneingang erwartet. Der Wareneingang wird
                              vor der Umlastung geprüft.
                               Der Wareneingang wird vor der Umlastung nicht geprüft.

                              Lieferterminverschiebungen zurückmelden Die Umlastung einer Position
                              kann den Liefertermin betreffen.
                               Bei einer Lieferterminverschiebung für eine Position wird der Liefertermin
                              aus dem Auftragskopf zurückgemeldet.
                               Eine Lieferterminverschiebung einer Position wird an den Auftrag zurück-
                              gemeldet. Der Liefertermin im Auftragskopf wird angepasst. Das ist jedoch nur
                              möglich, wenn die Daten online übertragen werden.

                              Erlaube Zieltermine in der Vergangenheit Sie können bei der Umlastung
                              auch Termine in der Vergangenheit zulassen. Die Checkbox ist nur freige-
                              schaltet, wenn Sie eine Begründung eingegeben haben.
                               Termine werden nicht in die Vergangenheit verschoben.
                               Die Bearbeitung kann auch in die Vergangenheit verschoben werden. Dazu
                              müssen Sie eine Begründung eingeben.
                               “Begründung” auf Seite E-175

                              2. Wählen Sie Datum, Schicht und Maschine aus
                              In diesem Bereich werden die Maschinen und die jeweils zugehörigen Arbeits-
                              schichten pro Arbeitstag angezeigt.

                              [Ansicht aktualisieren] Aktualisiert die Liste.
4.50 / 01-2023




                              [Gegebene Anzahl von Tagen zurück] Verschiebt den Zeitraum der ange-
                              zeigten Arbeitsschichten um die Anzahl der Tage in die Vergangenheit, die im
                              Feld Tage angegeben ist.



                 E-176                                                 A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                        Einlastung




                                        Starttermin Angabe des Starttermins, von dem an der Zeitraum angezeigt
                                        werden soll.

                                        Tage Angabe, um wie viele Tage die Anzeige der Arbeitsschichten mit den
                                        Schaltflächen jeweils vor- oder zurückgestellt werden soll.

                                        [Gegebene Anzahl von Tagen vor] Verschiebt den Zeitraum der angezeig-
                                        ten Arbeitsschichten um die Anzahl der Tage in die Zukunft, die im Feld Tage
                                        angegeben ist.

                                        3. Umlastung ausführen

                                        Zum Start der Umlastung den Modus auswählen Auswahl, in welchem
                                        Modus die Umlastung erfolgt:
                                        • Komplette Stückliste umlasten:
                                          Die komplette Stückliste, zu der die Bearbeitung gehört, wird umgelastet.
                                        • Nur markierte Bearbeitung:
                                          Nur die markierte Bearbeitung wird umgelastet.
                                        • Markierte und alle folgende Bearbeitungen:
                                          Die markierte und alle nachfolgenden Bearbeitungen der Stückliste werden
                                          umgelastet.
                                        • Markierte und alle vorherigen Bearbeitungen:
                                          Die markierte und alle vorherigen Bearbeitungen der Stückliste werden
                                          umgelastet.
                                        • Unbedingte Terminzuweisung für markierte Bearbeitung:
                                          Die markierte Bearbeitung wird auf den ausgewählten Termin der gewähl-
                                          ten Maschine umgelastet. Die Plausibilität wird nicht geprüft und die Ma-
                                          schinenkapazitäten werden dabei nicht berücksichtigt.

                                        [Umlasten] Startet die Umlastung mit den gewählten Parametern. Die
                                        Schaltfläche ist nur freigeschaltet, wenn ein Umlastungsmodus ausgewählt
                                        ist.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-177
                 Einlastung                                                             Softwarereferenz




                              Maschinenumlastung
                              Aufträge > Kontextmenü > Arbeitsplan > Maschinenumlastung
                              Läufe > Kontextmenü > Maschinenumlastung




                              Abb. E-101   Maschinenumlastung


                              In diesem Dialog können Sie Bearbeitungen aus Aufträgen oder Läufen auf
                              andere Logische Maschinen umlasten. Bei der Maschinenumlastung wird die
                              Bearbeitungsdauer nicht neu berechnet. Die Kosten und Einlastungsregeln
                              werden nicht geprüft.
                              Eine Umlastung über diesen Dialog ist daher nur sinnvoll, wenn Sie auf eine
                              identische Logische Maschine umlasten können.

                              Logische Routen Maschinen und logische Maschinen, von denen aus eine
                              Bearbeitung umgelastet werden soll.

                              Umlastungsalternativen Anzeige und Auswahl der möglichen Alternativen
                              zu der markierten logischen Maschine.

                              [Übernehmen] Speichert die Daten.

                              [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-178                                               A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                              Einlastung




                                           Nachbearbeitung Einlastung
                                           Stammdaten > Nachbearbeitung Einlastung




                 Abb. E-102   Nachbearbeitung Einlastung


                                           In diesem Dialog können Sie Aufträge, die nicht erfolgreich eingelastet wur-
                                           den, nachbearbeiten und erneut einlasten.
                                            Tutorial, “Eingelastete Aufträge nachbearbeiten” auf Seite E-42

                                           [Bearbeiten] Öffnet den Dialog Fehlerhafte Aufträge, in dem Sie auf Proble-
                                           me bei der Einlastung reagieren können.
                                            “Fehlerhafte Aufträge” auf Seite E-182

                                           [Aktualisieren] Aktualisiert die Ansicht mit aktuellen Daten.

                                           Übersicht Aufträge
                                           Die Anzeige der Spalten hängt von der Option ab, die im Feld Nachbearbei-
                                           tung von … gewählt ist.
                                           •   Auftrag:
                                               Die Auftragsnummer wird angezeigt, wenn die Option undefinierten Arti-
                                               keln gewählt ist.
                                           •   Artikel-Nr., Artikelbez.:
                                               Nummer und Bezeichnung des Artikels, der nicht definiert ist, werden an-
                                               gezeigt, wenn die Option undefinierten Artikeln oder undefinierten Bearbei-
                                               tungen gewählt ist.
4.50 / 01-2023




                                           •   Produktionsartikelnummer, Produktionsartikel:
                                               Nummer und Bezeichnung des Produktionsartikels, der nicht definiert ist,



                 A+W Production Kapazitätsplanung                                                                  E-179
                 Einlastung                                                              Softwarereferenz




                                  werden angezeigt, wenn die Option undefinierten Produktionsartikel/Di-
                                  cke-Kombinationen gewählt ist.
                              •   Dicke:
                                  Die Dicke im mm wird angezeigt, wenn die Option undefinierten Produkti-
                                  onsartikel/Dicke-Kombinationen gewählt ist.
                              •   Meldung:
                                  Der Text der Rückmeldung wird angezeigt, wenn die Option Rückmel-
                                  dungsprobleme gewählt ist.
                              •   Status:
                                  Der Status der Aufträge wird angezeigt, wenn die Option fehlerhafter Auf-
                                  tragsdaten gewählt ist.
                              •   Anzahl Aufträge:
                                  Die Anzahl der Aufträge mit gleichem Status wird angezeigt, wenn die Op-
                                  tion fehlerhafter Auftragsdaten gewählt ist.
                              •   Zeitstempel der Importdatei:
                                  Datum und Uhrzeit, zu denen der Auftrag eingelastet wurde.
                              •   Pos.:
                                  Die Nummer der Auftragsposition wird angezeigt, wenn die Option Ände-
                                  rungen verplanter Aufträge gewählt ist.
                              •   PosRef.:
                                  Die Referenznummer der Auftragsposition wird angezeigt, wenn die Option
                                  Änderungen verplanter Aufträge gewählt ist.
                              •   Packmittelgruppe:
                                  Die Packmittelgruppe, die dem Lauf zugeordnet ist, wird angezeigt, wenn
                                  die Option Änderungen verplanter Aufträge gewählt ist.
                              •   Anzahl Pos.:
                                  Die Anzahl der zum Lauf gehörenden Positionen wird angezeigt, wenn die
                                  Option Änderungen verplanter Aufträge gewählt ist.
                              •   Änderungstext:
                                  Die Anmerkung aus dem ERP-System wird angezeigt, wenn die Option
                                  Änderungen verplanter Aufträge gewählt ist. Dazu muss die Anmerkung
                                  mit übergeben worden sein.
4.50 / 01-2023




                 E-180                                                 A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                            Einlastung




                                        Nachbearbeitung von
                                        Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Aufträge in
                                        der Liste angezeigt werden sollen. In der Klammer steht jeweils, wie viele Auf-
                                        träge mit dem Kriterium vorhanden sind.
                                        Bei undefinierten Artikeln, Dicken-Kombinationen und/oder Bearbeitungen
                                        können Sie den Auftrag mit einem Doppelklick öffnen und korrigieren.
                                        •   Undefinierten Artikeln (n Aufträge):
                                            Aufträge mit undefinierten Artikeln.
                                        •   Undefinierten Produktionsartikel-/Dicke-Kombinationen (n Aufträge):
                                            Aufträge mit undefinierten Produktionsartikel-Kombinationen und undefi-
                                            nierten Dicke-Kombinationen.
                                        •   Undefinierten Bearbeitungen (n Aufträge):
                                            Aufträge mit undefinierten Bearbeitungen.
                                        •   Rückmeldeproblemen (n Aufträge):
                                            Aufträge mit Rückmeldeproblemen. Rückmeldeprobleme können bei der
                                            Datenübergabe zwischen einem ERP-System und A+W Production entste-
                                            hen.
                                             “Asynchrone Verarbeitung” auf Seite E-183
                                        •   Änderungen verplanter Aufträge (n Aufträge):
                                            Aufträge, die nach der Einlastung geändert wurden.
                                             “Änderung bereits verplanter Aufträge” auf Seite E-184
                                        •   Fehlerhafter Auftragsdaten (n Aufträge):
                                            Aufträge mit fehlerhaften Auftragsdaten.
                                             “Fehlerhafte Aufträge” auf Seite E-182
                                        •   Aufträgen mit Hinweisstatus (n Aufträge):
                                            Aufträge mit einem Hinweisstatus.

                                        Anzeigen nach
                                        Mit der Wahl der Option legen Sie fest, wie die Aufträge in der Liste sortiert
                                        werden.
                                        •   Auftragsnummer:
                                            Sortierung nach Auftragsnummern.
                                        •   Nachbearbeitungsursache:
                                            Sortierung nach Nachbearbeitungsursachen.

                                        Detailanzeige für Läufe und Packmittelgruppen
                                        Das Feld wird angezeigt, wenn die Option Änderungen verplanter Aufträge ge-
                                        wählt ist.
                                        •   Lauf:
                                            Nummer des Laufs.
                                        •   Laufstatus:
                                            Status des Laufs.
                                        •   Packmittelgruppe:
                                            Packmittelgruppe, die dem Lauf zugeordnet ist.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-181
                 Einlastung                                                                   Softwarereferenz




                              Fehlerhafte Aufträge
                              Stammdaten > Nachbearbeitung Einlastung > Option Fehlerhafter Auftragsda-
                              ten > [Bearbeiten]




                              Abb. E-103   Fehlerhafte Aufträge


                              In diesem Dialog können Sie wählen, wie nicht eingelastete Aufträge verarbei-
                              tet werden sollen.
                               Tutorial, “Eingelastete Aufträge nachbearbeiten” auf Seite E-42
                              Dazu können Sie zwischen folgenden Optionen wählen:
                              •   Erneute Datenübernahme:
                                  Markierte Aufträge werden erneut eingelastet. Verwenden Sie diese Option
                                  z. B. bei Fehlern in den Stammdaten, z. B. wenn A+W Production keine Ar-
                                  beitsschicht für den Auftrag gefunden hat.
                                  Wenn Sie den Fehler behoben haben, können Sie den Auftrag einlasten,
                                  ohne eine erneute Datenübertragung vom ERP-System anzufragen.
                              •   Einlastung erzwingen. Die freie Kapazität an Engpassbetriebsmitteln wird
                                  in diesem Fall nicht berücksichtigt.:
                                  Der Auftrag wird erneut eingelastet. Dabei wird die Kapazität der Maschine
                                  nicht berücksichtigt. Daher werden die Arbeitsschichten ggf. überbucht.
                                  Wenn eine Kapazität überschritten ist, kann es zu Terminverschiebungen
                                  bei anderen Aufträgen kommen.
                              •   Einlastung ignorieren. Die Produktionstermine werden ermittelt ohne
                                  Rücksicht auf Übergangszeiten, Kapazitätsgrenzen und Kampagnentermi-
                                  ne. Gültige Arbeitspläne müssen Sie mittels manueller Umlastung erstel-
                                  len.
                              •   Löschung der fehlerhaften Aufträge. Die Aufträge können dann mit diesem
                                  System NICHT verplant werden. Rücksprache mit Auftragserfassung erfor-
                                  derlich!:
                                  Die Aufträge werden aus A+W Production gelöscht. Die Aufträge müssen
4.50 / 01-2023




                                  im ERP-System korrigiert und erneut übertragen werden.
                              •   Ermittelten Liefertermin bestätigen:
                                  Übernahme des neuen Liefertermins, den A+W Production für die gewähl-


                 E-182                                                    A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                               Einlastung




                                            ten Aufträge vorschlägt. Die Aufträge werden zu den neuen Liefertermin-
                                            Bedingungen eingelastet und der ermittelte Liefertermin wird an das ERP-
                                            System zurück gemeldet.
                                            Ändern Sie Liefertermine nur nach Absprache mit der Auftragserfassung.


                                        Asynchrone Verarbeitung
                                        Stammdaten > Nachbearbeitung Einlastung > Option Rückmeldungsproble-
                                        me > [Bearbeiten]




                                        Abb. E-104    Asynchrone Verarbeitung


                                        In diesem Dialog können Sie wählen, wie Aufträge mit Problemen bei der
                                        Rückmeldung verarbeitet werden sollen.
                                        Dazu können Sie zwischen folgenden Optionen wählen:
                                        •   Erneuten Versuch starten:
                                            Markierte Aufträge werden erneut eingelastet. Verwenden Sie diese Option
                                            z. B. bei Fehlern während der Datenübertragung.
                                        •   Position stornieren:
                                            Die Position wird storniert. Der restliche Auftrag wird eingelastet. Bei dieser
                                            Option sollten Sie Rücksprache mit dem Auftraggeber halten, damit die
                                            Daten erneut übertragen werden.
                                        •   Fehler ignorieren:
                                            Die Produktionstermine werden ermittelt. Die Position wird übernommen,
                                            die Rückmeldung wird jedoch nicht geschrieben. Deshalb dürfen Sie diese
                                            Option nur auswählen, wenn Sie absolut sicher sind, dass Sie den Fehler
                                            ignorieren können.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                   E-183
                 Einlastung                                                               Softwarereferenz




                              Änderung bereits verplanter Aufträge
                              Stammdaten > Nachbearbeitung Einlastung > [Bearbeiten]




                              Abb. E-105   Änderung bereits verplanter Aufträge


                              In diesem Dialog können Sie wählen, wie eingelastete Aufträge behandelt
                              werden sollen, zu denen Änderungen übertragen wurden.
                              Dazu können Sie zwischen folgenden Optionen wählen.
                              •   Neue Position erzeugen:
                                  Storno der bisherigen Position und Übernahme der Änderung als neue Po-
                                  sition in den Pool.:
                                  Der Auftrag wird mit einer neuen Positionsnummer erneut eingelastet.
                              •   Erneut versuchen:
                                  Übernahme der Änderung in den Pool. Lösen Sie zuvor die betroffenen
                                  Läufe/PMO-Mastergruppen auf.:
                                  Lösen Sie die betroffenen Läufe zunächst auf und wählen Sie anschlie-
                                  ßend diese Option. Der Auftrag wird erneut eingelastet.
                              •   Änderung ignorieren:
                                  Löschung der Änderung. Die bisherige Position bleibt unverändert.:
                                  Die Änderung wird gelöscht und die ursprünglichen Daten beibehalten.
                              •   (nicht empfohlen):
                                  Übernahme der Änderung in die bisherigen Läufe. Stellen Sie zuvor sicher,
                                  dass die Änderung nicht produktionsrelevant ist.:
                                  Zur Zeit nicht genutzt.

                              [Änderung analysieren] Zur Zeit nicht genutzt.
4.50 / 01-2023




                 E-184                                                   A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                            Einlastung




                                        Positionssplit
                                        Anzeigen > Aufträge > Kontextmenü > Positionen splitten




                                        Abb. E-106   Positionssplit


                                        In diesem Dialog können Sie Positionen aus Aufträgen aufsplitten. Wenn bei
                                        einer großen Position die Bearbeitungsdauer der langsamsten Maschine die
                                        die konfigurierte Schwelle überschreitet, wird diese Position im Rahmen der
                                        Einlastung durch A+W Capacity Planner gesplittet. In der Regel werden die
                                        Positionen automatisch gesplittet, so dass die Terminfindung auch bei großen
                                        Positionen mit optimaler Geschwindigkeit abläuft.
                                        Der Positionssplit ist im Part Grobplanung - Tutorial beschrieben.

                                        Markierte Positionen
                                        In der Liste werden die Positionen angezeigt, die Sie im Dialog Bearbeitungen
                                        ausgewählt haben.
                                        •   Auftrag:
                                            Auftrag, den Sie zum Splitten ausgewählt haben.
                                        •   Pos.:
                                            Nummer der Auftragsposition.
                                        •   UPos.:
                                            Nummer der Unterpositionen im Auftrag.
                                        •   Menge:
                                            Anzahl der Scheiben in der Position.

                                        [Entfernen] Löscht die markierte Position.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                               E-185
                 Einlastung                                                               Softwarereferenz




                              Splitting-Optionen
                              Mit der Wahl der Option legen Sie fest, wie die Positionen geteilt werden:
                              •   Je Position in … Positionen aufteilen:
                                  Angabe, in wie viele neue Positionen aufgeteilt wird. Das Feld zur Angabe
                                  der Anzahl wird freigeschaltet.
                              •   Positionen mit maximal … Scheiben erzeugen:
                                  Angabe, wie viele Scheiben eine neue Position maximal enthalten darf.
                                  Das Feld zur Angabe der Anzahl wird freigeschaltet.
                              •   Je Pos. eine Pos. mit … Scheiben erzeugen:
                                  Angabe der Scheibenanzahl, für die jeweils eine neue Position erzeugt
                                  wird. Das Feld zur Angabe der Anzahl wird freigeschaltet.
                              •   Teilung gemäß PMO Ergebnis:
                                  Angabe, dass die Positionen passend zur Packmitteloptimierung gesplittet
                                  werden.

                              Neue Positionen
                              In der Liste werden die gesplitteten Positionen als Unterpositionen angezeigt.
                              •   Auftrag:
                                  Auftragsnummer.
                              •   Pos.:
                                  Nummer der Auftragsposition.
                              •   UPos.:
                                  Nummer der Unterpositionen im Auftrag.
                              •   Neue Position:
                                  Nummer der neuen Position nach dem Split. Die Nummerierung wird pro
                                  gesplitteter Auftragsposition gezählt.
                              •   Menge:
                                  Anzahl der Scheiben in der neuen Position.

                              [Splitten] Splittet die markierte Position. Die neuen Positionen werden erst
                              gespeichert, wenn sie mit [Übernehmen] bestätigt sind.

                              [Übernehmen] Speichert die neuen Positionen. Diese Aktion kann nicht
                              rückgängig gemacht werden.

                              [Verwerfen] Stellt die ursprüngliche Position wieder her. Anschließend kön-
                              nen Sie die Position mit anderen Vorgaben splitten.

                              [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-186                                                 A+W Production Kapazitätsplanung
                 Softwarereferenz                                                 Kampagnen und Reservierungen




                                        Kampagnen und Reservierun-
                                        gen
                                        Für bestimmte Arbeitsgänge und/oder Aufträge können Sie Kampagnen ein-
                                        richten und Kapazitäten reservieren.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Kampagnen” auf Seite E-188
                                        •   “Abgelaufene Reservierungen” auf Seite E-192
                                        •   “Reservierungen” auf Seite E-194
                                        •   “Reservierung für Maschine” auf Seite E-197
                                        •   “Kunde auswählen” auf Seite E-198
                                        •   “Objekt auswählen” auf Seite E-199
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                         E-187
                 Kampagnen und Reservierungen                                                   Softwarereferenz




                                      Kampagnen
                                      Stammdaten > Kapazitätsplanung > Kampagnenplanung
                                      In diesem Dialog können Sie Kampagnen als Einzeltermine oder wöchentliche
                                      Termine definieren. Mit Kampagnen können Sie für bestimmte Arbeitsgänge
                                      Kapazitäten einplanen, z. B. für Siebdruck für jeden Wochentag eine andere
                                      Farbe.

                                          Voraussetzung
                                          Nur die Bearbeitungen werden in Kampagnenterminen eingelastet, die als
                                          Kampagnen-Bearbeitungen definiert sind.

                                       Tutorial, “Kampagnenplanung” auf Seite E-44
                                      Der Dialog Kampagnen enthält folgende Register:
                                      •   “Kampagnen – Einzeltermine” auf Seite E-189
                                      •   “Kampagnen – Wöchentliche Termine” auf Seite E-191
4.50 / 01-2023




                 E-188                                                         A+W Production Kapazitätsplanung
                 Softwarereferenz                                                      Kampagnen und Reservierungen




                                          Kampagnen – Einzeltermine
                                          Stammdaten > Kapazitätsplanung > Kampagnenplanung > Register Einzelter-
                                          mine




                 Abb. E-107   Kampagnen – Einzeltermine


                                          In diesem Register verwalten Sie Einzelkampagnen. Mit Einzelkampagnen
                                          führen Sie Kampagnen durch, die einmalig anfallen.
                                           Tutorial, “Kampagnenplanung” auf Seite E-44

                                          Arbeitsgang Arbeitsgänge, die Sie in der Maschinenzuordnung erzeugt ha-
                                          ben. Ein Arbeitsgang ist in der Liste hellgrau hinterlegt, wenn er zu einer Kam-
                                          pagne hinzugefügt ist.

                                          Kampagnen Kampagnenfähige Arbeitsgänge, die Sie hinzugefügt haben.
                                          Wenn Sie in der Liste Kampagnen einen Arbeitsgang markieren, werden in
                                          den Registern Einzeltermine oder Wöchentliche Termine die zugehörigen Ter-
                                          mine angezeigt.
                                           Die Kampagne ist nicht aktiv.
                                           Die Kampagne ist aktiv.
4.50 / 01-2023




                                          [Zuordnen] Verschiebt ein markiertes Element auf die andere Seite.




                 A+W Production Kapazitätsplanung                                                                  E-189
                 Kampagnen und Reservierungen                                                    Softwarereferenz




                                      Einzeltermine

                                      Kalender Auswahl eines Datums für eine Kampagne.

                                      Schichten Verfügbare Arbeitsschichten am gewählten Datum.

                                         Anzeige der Schichten
                                         Nur die aktiven Schichtpläne werden angezeigt. Aktivieren Sie ggf. die
                                         Schichtpläne, die für die Kampagne benötigt werden.

                                      Einzeltermine Anzeige der Kampagnen für das markierte Datum.
                                      • Datum:
                                         Termine, zu denen Sie Kampagnen erzeugt haben.
                                      • Schicht:
                                         Arbeitsschicht, in der die jeweilige Kampagne durchgeführt wird.

                                         Kampagnen löschen
                                         Wenn Sie kurzfristig Kampagnen löschen, hat das Auswirkungen auf die
                                         Produktion. Bearbeitungen werden z. B. nicht durchgeführt oder Produkti-
                                         onstermine ändern sich.
                                         Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH,
                                         wenn Sie Kampagnen löschen wollen und zu diesem Zeitpunkt bereits Auf-
                                         träge eingelastet sind.

                                      Hinzufügen für die nächsten Angabe, für welchen Zeitraum die Kampagne
                                      angelegt wird.
                                      Mit der Wahl der Option legen Sie fest, ob die Dauer des Termins in Tagen
                                      oder Wochen angegeben wird.

                                      [Kampagne hinzufügen] Fügt eine Kampagne hinzu. Dazu müssen folgen-
                                      de Elemente markiert sein:
                                      • ein kampagnenfähiger Arbeitsgang
                                      • ein Termin
                                      • eine Schicht

                                      [Löschen] Löscht die markierte Kampagne.

                                      [OK] Speichert die Daten.

                                      [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-190                                                        A+W Production Kapazitätsplanung
                 Softwarereferenz                                                      Kampagnen und Reservierungen




                                          Kampagnen – Wöchentliche Termine
                                          Stammdaten > Kapazitätsplanung > Kampagnenplanung > Register Wöchent-
                                          liche Termine




                 Abb. E-108   Kampagnentage – Wöchentliche Termine


                                          In diesem Register verwalten Sie Serienkampagnen. Mit Serienkampagnen
                                          führen Sie regelmäßig wiederkehrende Kampagnen durch.
                                           Tutorial, “Kampagnen anlegen und verwalten” auf Seite E-47
                                          Eine Beschreibung der Felder im Dialog Kampagnen finden Sie hier:
                                           “Kampagnen – Einzeltermine” auf Seite E-189

                                          Wöchentliche Termine Anzeige der Kampagnen für den markierten Wo-
                                          chentag.
                                          • Wochentag:
                                             Arbeitstage, zu denen Sie Kampagnen erzeugt haben.
                                          • Schicht:
                                             Arbeitsschicht, in der die jeweilige Kampagne durchgeführt wird.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-191
                 Kampagnen und Reservierungen                                                    Softwarereferenz




                                      Abgelaufene Reservierungen
                                      Stammdaten > Kapazitätsplanung > Reservierungen




                                      Abb. E-109   Abgelaufene Reservierungen


                                      In diesem Dialog werden abgelaufene Reservierungen angezeigt. Der Dialog
                                      wird automatisch geöffnet, wenn Sie den Dialog Reservierungen öffnen und
                                      abgelaufene Reservierungen vorhanden sind.

                                      Liste
                                      •   Maschine:
                                          Maschine, auf der Kapazität reserviert wurde.
                                      •   Kunde:
                                          Kunde, für den Kapazität reserviert wurde.
                                      •   Objekt:
                                          Objekt, für das Kapazität reserviert wurde.
                                      •   Woche:
                                          Kalenderwoche, in der Kapazität reserviert wurde.
                                      •   Jahr:
                                          Jahr, für das Kapazität reserviert wurde.
                                      •   Datum:
                                          Datum, an dem die Reservierung beginnt.
                                      •   Schicht:
                                          Arbeitsschicht, für die Kapazität reserviert wurde.
                                      •   Prozent:
                                          Kapazität in Prozent, die auf der Maschine reserviert wurde.
                                      •   Verbraucht:
                                          Angabe in Prozent, wie viel von der Reservierung bereits verbraucht wur-
                                          de.
                                      •   Ablauf:
4.50 / 01-2023




                                          Datum, an dem die Reservierung endet.




                 E-192                                                          A+W Production Kapazitätsplanung
                 Softwarereferenz                                               Kampagnen und Reservierungen




                                        [Löschen] Löscht die markierte Reservierung.

                                        [OK] Speichert die Daten und wechselt zum Fenster Reservierungen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                       E-193
                 Kampagnen und Reservierungen                                                          Softwarereferenz




                                      Reservierungen
                                      Stammdaten > Kapazitätsplanung > Reservierungen




                                      Abb. E-110    Reservierungen


                                      In diesem Dialog verwalten Sie Reservierungen von Maschinenkapazitäten.
                                      Reservierungen sind nur auf den einzelnen Maschinen möglich, die als Eng-
                                      passbetriebsmittel definiert sind. Sie sind zeitlich begrenzt. Ein Engpassbe-
                                      triebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

                                      Die Reservierungen werden entweder für spezifische Kunden oder Bauprojek-
                                      te angelegt.
                                      Im Produktionsmonitor werden die reservierten Zeiten in den jeweiligen Ar-
                                      beitsschichten gekennzeichnet.
                                       Tutorial, “Reservierungen” auf Seite E-54

                                         Reservierungen für einzelne Aufträge
                                         Reservierungen von Zeiten für einzelne Aufträge müssen vom ERP-Sys-
                                         tem erfasst und übertragen werden. Die als Reservierungsauftrag gekenn-
                                         zeichneten und zur Produktion freigegebenen Aufträge reservieren auf
                                         allen für die Produktion benötigten Maschinen entsprechende Zeiten.
4.50 / 01-2023




                 E-194                                                              A+W Production Kapazitätsplanung
                 Softwarereferenz                                                       Kampagnen und Reservierungen




                                        Reservierungen

                                            Reservierungen in Schichten, Tagen oder Wochen
                                            In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstel-
                                            lung unter Stammdaten > Konfiguration > A+W Production > Kapazitätspla-
                                            nung > Art der Reservierung können für die Reservierung aber auch Tage
                                            oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung än-
                                            dern, gehen die alten Reservierungen verloren.

                                        Maschine Auswahl der Maschine, deren Reservierungen angezeigt werden.
                                        In der Auswahl-Liste sind alle Maschinen angezeigt, die als Engpassbetriebs-
                                        mittel definiert sind.

                                        Starttermin Beginn des Reservierungszeitraums. Standardmäßig wird der
                                        aktuelle Kalendertag angezeigt.

                                        Tage Angabe, wie viele Tage in der Vorschau angezeigt werden.

                                        Schichtreservierungen
                                        Im Bereich Schichtreservierungen werden die Reservierungen ab dem ausge-
                                        wählten Datum grafisch dargestellt.

                                        Frei Freie Kapazität der Maschine.

                                        Reserviert Reservierte Kapazität der Maschine.

                                        Benutzt Tatsächlich benutzter Anteil der Reservierung.

                                        Reservierungen pro Kunde
                                        Ist im Bereich Schichtreservierungen ein Tag markiert, wird eine Übersicht mit
                                        allen Reservierungen angezeigt.
                                        •   Kunde:
                                            Kunde, für den Kapazitäten reserviert sind.
                                        •   Objekt:
                                            Objekt, für das Kapazitäten reserviert sind.
                                        •   Reservierung:
                                            Reservierte Maschinen-Kapazitäten in Prozent.
                                        •   Benutzt:
                                            Tatsächlich benutzter Anteil der Reservierung in Prozent.
                                        •   Ablaufdatum:
                                            Datum, an dem die Reservierung endet.
                                        •   Datum:
                                            Datum, an dem die Reservierung erfasst wurde.
                                        •   Schicht:
                                            Arbeitsschicht, für die die Reservierung gilt.
4.50 / 01-2023




                                        [Neu] Öffnet den Dialog zum Reservieren von Maschinen-Kapazitäten.
                                         “Reservierung für Maschine” auf Seite E-197

                                        [Löschen] Löscht die markierte Reservierung.


                 A+W Production Kapazitätsplanung                                                              E-195
                 Kampagnen und Reservierungen                                                     Softwarereferenz




                                      [OK] Speichert die Daten.

                                      [Ende] Bricht die Bearbeitung ab und schließt den Dialog.
4.50 / 01-2023




                 E-196                                                       A+W Production Kapazitätsplanung
                 Softwarereferenz                                                    Kampagnen und Reservierungen




                                        Reservierung für Maschine
                                        Stammdaten > Kapazitätsplanung > Reservierungen > [Neu]




                                        Abb. E-111   Reservierung für Kunde oder Objekt


                                        In diesem Dialog reservieren Sie Maschinen-Kapazitäten für einen bestimm-
                                        ten Kunden oder ein Objekt.

                                           Reservierungen in Schichten, Tagen oder Wochen
                                           In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstel-
                                           lung unter Stammdaten > Konfiguration > A+W Production > Kapazitätspla-
                                           nung > Art der Reservierung können für die Reservierung aber auch Tage
                                           oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung än-
                                           dern, gehen die alten Reservierungen verloren.

                                        Kunde Kunde, für den Maschinen-Kapazität reserviert wird. Die [Lupe] öffnet
                                        den Dialog Kunde auswählen.
                                         “Kunde auswählen” auf Seite E-198

                                        Objekt Objekt, für das Maschinen-Kapazität reserviert wird. Die [Lupe] öffnet
                                        den Dialog Objekt auswählen.
                                         “Objekt auswählen” auf Seite E-199

                                        Datum Beginn des Reservierungszeitraums.

                                        Schicht Arbeitsschicht, in der die Maschine reserviert ist.

                                        Ablaufdatum Ende des Reservierungszeitraums.

                                        Reservierung in % Maschinen-Kapazität in Prozent, die reserviert werden
                                        soll.
                                        Sie können die Reservierung als Betrag eingeben oder indem Sie den Balken
                                        im Feld darüber mit der Maus aufziehen.
4.50 / 01-2023




                                        [OK] Speichert die Daten.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu speichern.


                 A+W Production Kapazitätsplanung                                                             E-197
                 Kampagnen und Reservierungen                                                   Softwarereferenz




                                      Kunde auswählen
                                      Stammdaten > Kapazitätsplanung > Reservierungen > [Neu] > Kunde




                                      Abb. E-112   Kunde auswählen


                                      In diesem Dialog wählen Sie den Kunden, für den Sie Maschinen-Kapazitäten
                                      reservieren wollen.

                                      Übersicht
                                      •   ID:
                                          Kundennummer.
                                      •   Name:
                                          Name des Kunden.
                                      •   Matchcode:
                                          Matchcode, der dem Kunden zugewiesen wurde.

                                      Matchcode Angabe des Matchcodes für die Kundensuche.

                                      Name Angabe des Namens für die Kundensuche.

                                      Anzahl Anzahl der Kunden, die in der Übersicht angezeigt werden.

                                      [Suchen] startet die Suche, wenn Sie im Filterkriterium die Wild Card % ein-
                                      gesetzt haben.

                                      [OK] Übernimmt den markierten Kunden in den Dialog Reservierung für Ma-
                                      schine.

                                      [Schließen] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 E-198                                                        A+W Production Kapazitätsplanung
                 Softwarereferenz                                                  Kampagnen und Reservierungen




                                        Objekt auswählen
                                        Stammdaten > Kapazitätsplanung > Reservierungen > [Neu] > Objekt




                                        Abb. E-113   Objekt auswählen


                                        In diesem Dialog wählen Sie ein Objekt, für das eine Reservierung vorgenom-
                                        men wird.

                                        Übersicht
                                        •   ID:
                                            Identifikationsnummer des Objekts.
                                        •   Beschreibung:
                                            Name des Objekts.

                                        Name Angabe des Namens für die Objektsuche.

                                        Anzahl Anzahl der Objekte, die in der Übersicht angezeigt werden.

                                        [Suchen] startet die Suche, wenn Sie im Filterkriterium die Wild Card % ein-
                                        gesetzt haben.

                                        [OK] Übernimmt das markierte Objekt in den Dialog Reservierung für Ma-
                                        schine.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-199
                 Bearbeitungen                                                               Softwarereferenz




                                 Bearbeitungen
                                 Die Bearbeitungen beschreiben die Arbeitsschritte zur Fertigung der Teile. Die
                                 Bearbeitungserzeugung stellt sicher, dass für jedes Stücklistenteil beschrie-
                                 ben wird, wie es in der Produktion entsteht. Diese Information ist für A+W Ca-
                                 pacity Planner unabdingbar und auch sonst ist es sinnvoll, z.B. auf Papieren
                                 die ganze Entstehung der Produkte zu sehen.
                                 In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                 •   “Bearbeitungserzeugung” auf Seite E-201
                                 •   “Existierende Bedingung hinzufügen” auf Seite E-204
4.50 / 01-2023




                 E-200                                                    A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                        Bearbeitungen




                                          Bearbeitungserzeugung
                                          Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung




                 Abb. E-114   Bearbeitungserzeugung


                                          In diesem Dialog ordnen Sie den Teiletypen jeweils die Bearbeitungsartikel zu,
                                          die in den Stammdaten hinterlegt sind. Diese Zuordnung ist z. B. dann not-
                                          wendig, wenn Ihr ERP-System diese Bearbeitungen nicht übergibt.
                                          Anhand der Zuordnungen können Arbeitsgänge ermittelt werden. Diese Anga-
                                          ben werden für die Produktionsplanung und Kostenermittlung benötigt.
                                          Bei der Bearbeitungserzeugung werden für die Teile der Stückliste den Teile-
                                          typen und den Beschaffungsarten entsprechende Bearbeitungen erzeugt. Die
                                          Bearbeitungen beschreiben die Entstehung der Teile. Damit die Kapazitätspla-
                                          nung arbeiten kann, müssen mindestens für alle Lagerentnahmen, Bestell-
                                          und Zuschnittsteile und Zusammenbaubearbeitungen, wie VSG und ISO, Be-
                                          arbeitungen definiert sein.
                                          Beachten Sie zusätzliche Bearbeitungen wie Verpacken und Versenden, so-
                                          fern dies nicht von Ihrem ERP-System übergeben werden.
                                           Tutorial, “Bearbeitungen erzeugen” auf Seite E-65
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-201
                 Bearbeitungen                                                               Softwarereferenz




                                 Bearbeitungserzeugung

                                 Bearbeitungen Produktionsrelevante Bearbeitungstypen und zugeordnete
                                 Bearbeitungsartikel.

                                 Teiletypen Teiletypen mit zugeordneten Bearbeitungsartikeln.

                                 [Zuordnen] Ordnet einen markierten Bearbeitungsartikel dem markierten
                                 Teiletyp zu.

                                 Details Informationen zum markierten Bearbeitungstyp oder Bearbeitungs-
                                 artikel.
                                 •   Artikelnummer:
                                     Artikelnummer des markierten Bearbeitungsartikels.
                                 •   Bearbeitungstyp:
                                     – Bei markiertem Bearbeitungsartikel: Zugeordneter Bearbeitungstyp.
                                     – Bei markiertem Bearbeitungstyp: ID des Bearbeitungstyps.
                                 •   Beschaffungsart:
                                     Beschaffungsart des Bearbeitungstyps.
                                 •   Klasse:
                                     Bearbeitungsklasse des markierten Bearbeitungsartikels, z. B. Säumen.
                                 •   Name:
                                     Name des markierten Elements.
                                 •   Sequenz/Sequenznummer:
                                     Sequenznummer des markierten Elements. Je höher eine Sequenznum-
                                     mer ist, desto später wird die Bearbeitung am Glas durchgeführt.
                                     – Ist für einen Bearbeitungsartikel eine Sequenz angegeben, wird diese
                                         berücksichtigt.
                                     – Ist für einen Bearbeitungsartikel keine Sequenz angegeben, wird die
                                         Sequenz des Bearbeitungstyps verwendet.
                                     Für alle erzeugenden Bearbeitungen kann die Sequenz 100 gesetzt wer-
                                     den, z. B. für Isolieren, Vorspannen oder Verpacken. Für alle anderen Be-
                                     arbeitungen muss die Sequenz entsprechend aufsteigend sein, z. B. für
                                     Säumen und Bohren.

                                     Sequenz und Sequenznummer
                                     Die Sequenz steuert die Reihenfolge der Bearbeitungen und ist damit pro-
                                     duktionsrelevant.
                                     Wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn
                                     Sie Sequenzen ändern möchten.

                                 •  Teiletyp:
                                    Nummer des Teiletyps, z. B. 2 für Handelsglas.
                                    Der Teiletyp wird durch die A+W Software GmbH festgelegt.
                                 Im Feld darunter wird die Beschreibung zum markierten Element angezeigt.

                                 [Kategorien] Sortiert die Elemente nach Kategorien.
4.50 / 01-2023




                                 [Alphabetisch] Sortiert die Elemente alphabetisch.



                 E-202                                                    A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                  Bearbeitungen




                                        [Eigenschaften] Zur Zeit nicht genutzt.

                                        Bedingungen Formeln, die dem Bearbeitungsartikel zugeordnet sind, der im
                                        Bereich Teiletypen markiert ist.

                                           Formeln und Bedingungen
                                           Formeln beeinflussen die Eigenschaften und planungstechnischen Auswir-
                                           kungen von Bearbeitungstypen und Teiletypen unter Umständen massiv.
                                           Sie müssen verstehen, welche Auswirkungen die hinterlegte Formel hat.
                                           Zum Thema Formeln und Restriktionen in A+W Production gibt es ein se-
                                           parates Handbuch.

                                        [Neu] Öffnet den Dialog Existierende Bedingung hinzufügen, um dem Bear-
                                        beitungsartikel eine Formel zuzuordnen.

                                        [Löschen] Löscht die markierte Formel im Feld Bedingungen.

                                        [OK] Speichert die Daten.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                         E-203
                 Bearbeitungen                                                             Softwarereferenz




                                 Existierende Bedingung hinzufügen
                                 Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung > [Neu Drop-
                                 down-Menü] > Existierende Bedingung hinzufügen, Standardbedingung hin-
                                 zufügen




                                 Abb. E-115   Existierende Bedingung hinzufügen


                                 In diesem Dialog wählen Sie die Bedingung aus, die Sie im Dialog Bearbei-
                                 tungserzeugung einer Bearbeitung zuordnen wollen.

                                 [OK] Übernimmt eine markierte Formel in den Dialog Bearbeitungserzeu-
                                 gung.

                                 [Schließen] Schließt den Dialog, ohne eine Bedingung in den Dialog Bear-
                                 beitungserzeugung zu übernehmen.
4.50 / 01-2023




                 E-204                                                    A+W Production Kapazitätsplanung
                 Softwarereferenz                                                            Stammdaten für Zeiten




                                        Stammdaten für Zeiten
                                        Für alle Bearbeitungen müssen Zeiten hinterlegt werden, aus denen die Dau-
                                        er pro Bearbeitungsposition errechnet werden kann.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Vorgabezeiten” auf Seite E-206
                                        •   “Vorgabezeitformel” auf Seite E-208
                                        •   “Elemente hinzufügen” auf Seite E-212
                                        •   “Tabelle, Vektor (Name)” auf Seite E-213
                                        •   “Eingabehilfe für Vektoren” auf Seite E-214
                                        •   “Formel auswählen” auf Seite E-216
                                        •   “Erfassung eines Formelelements” auf Seite E-217
                                        •   “Benutzerdefinierte Tabellenelemente” auf Seite E-219
                                        •   “Grenzwert auswählen” auf Seite E-220
                                        •   “Zeitformeltest” auf Seite E-221
                                        •   “Eigenschaften des Formelobjekts” auf Seite E-223
                                        •   “Formel (Name)” auf Seite E-225
                                        •   “Verlauf der Formelauswertung” auf Seite E-226
                                        •   “Übergangszeiten” auf Seite E-227
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                          E-205
                 Stammdaten für Zeiten                                                                  Softwarereferenz




                                         Vorgabezeiten
                                         Stammdaten > Kapazitätsplanung > Vorgabezeiten




                                         Abb. E-116   Vorgabezeiten


                                         In diesem Dialog verwalten Sie die Berechnungsformeln für die Bearbeitun-
                                         gen an einer der logischen Maschinen. Mit einer Formel definieren Sie, wie die
                                         Dauer eines Arbeitsgangs berechnet wird. Basis der Berechnung ist z. B. die
                                         jeweilige Fläche oder Kantenlänge in der einzelnen Auftragsposition.
                                          Tutorial, “Vorgabezeiten” auf Seite E-106
                                         Für die Erstellung von Formeln stehen zwei verschiedene Editoren zur Verfü-
                                         gung. Eine ausführliche Beschreibung der Editoren finden Sie im Part Formel-
                                         editor.
                                         In der Zeile 0 – Alle Maschinen können Sie Formelelemente als Vorlagen für
                                         alle Maschinen definieren.

                                         Vorgabezeitformeln
                                         In der Übersicht sind alle in A+W Production definierten Maschinen angezeigt.
                                         Diese Daten werden aus der Maschinenzuordnung eingelesen und können
                                         nicht bearbeitet werden.
                                         •   Nr.:
4.50 / 01-2023




                                             Nummer der logischen Maschine.
                                         •   Log.:
                                             Logische ID der logischen Maschine.


                 E-206                                                                 A+W Production Kapazitätsplanung
                 Softwarereferenz                                                              Stammdaten für Zeiten




                                        •   Maschine:
                                            Name der Maschine.
                                        •   Log. Maschine:
                                            Name der logischen Maschine.
                                        •   Engpass:
                                            Anzeige, ob die Maschine als Engpass definiert ist.
                                        •   Einzel:
                                            Anzeige, ob die Maschine Bearbeitungsketten bildet. Wenn keine Bearbei-
                                            tungsketten gebildet werden sollen, werden die Bearbeitungen einzeln
                                            abgehandelt, d. h. eine nach der anderen in separaten Arbeitsschritten ver-
                                            plant.
                                            Diese Einstellung ist z. B. für Siebdruck, Flächenbearbeitungen usw. wich-
                                            tig.
                                            Für Bohren, Schleifen usw. sollte die Checkbox nicht markiert sein, da für
                                            diese Bearbeitungen Bearbeitungsketten sinnvoll sind.
                                        •   Manuell:
                                            Anzeige, ob die Maschine manuell bedient wird. Manuelle Maschinen wer-
                                            den nicht in die automatische Maschinenumlastung einbezogen. Sie sind
                                            außerdem für den automatischen Positionssplit gesperrt.
                                        •   Typ:
                                            Maschinentyp der zugehörigen Maschine.
                                        •   Id:
                                            Nummer der Logischen Maschine. Diese ID ist für den technischen Sup-
                                            port wichtig.

                                        [Bearbeiten] Öffnet den Dialog Vorgabezeitformel, um die Vorgabezeitfor-
                                        mel zu bearbeiten.
                                         “Vorgabezeitformel” auf Seite E-208

                                            Bereits vorhandene Vorgabezeitformel
                                            Wenn Sie auf Bearbeiten klicken und bereits eine formelbasierte Vorgabe-
                                            zeitformel zugeordnet ist, wird eine Meldung angezeigt. Wenden Sie sich
                                            an den Kundenservice der A+W Software GmbH, wenn Sie die Vorgabe-
                                            zeit ändern wollen.

                                        [Löschen] Löscht den markierten Eintrag.

                                        [Ende] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                               E-207
                 Stammdaten für Zeiten                                                                    Softwarereferenz




                                           Vorgabezeitformel
                                           Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten]




                 Abb. E-117   Vorgabezeitformel – Beispiel der Auswahlmöglichkeiten


                                           In diesem Dialog bearbeiten Sie die Taktzeiten einer logischen Maschine.

                                               Vorgabezeitformel ändern
                                               Ändern oder erstellen Sie Vorgabezeitformeln nur in Rücksprache mit dem
                                               Kundenservice der A+W Software GmbH.

                                               Komplexe Vorgabezeitformeln stellen einen tiefgreifenden Eingriff in A+W
                                               Production dar und sollen nur vom Kundenservice der A+W Software
                                               GmbH vorgenommen werden. Eine Vorgabezeitformel gilt z. B. dann als
                                               komplex, wenn sie zwei und mehr Faktoren/Vektoren enthält.

                                            Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118
4.50 / 01-2023




                 E-208                                                                A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                 Stammdaten für Zeiten




                                        Vorgabezeitformel
                                        Liste der Elemente, die zur Formel gehören.

                                        Basiszeit Angabe der Basiszeit für die Vorgabezeitformel in Sekunden.
                                        Wenn die Berechnung mit der Ermittlung aus einer Formel beginnt, legen Sie
                                        als Startwert 0 fest, z. B. die Berechnung einer Fläche bevor der erste Sieb-
                                        druck aufgetragen wird.
                                        Sie können folgende Zeitzuschläge für die Berechnung definieren:
                                        • Faktor ’Gas‘:
                                            Zuschlag für das Befüllen von ISO mit Gas.
                                        • Faktor ’Sprossen‘:
                                            Zuschlag in Abhängigkeit von der Anzahl der Sprossen.
                                        • Modellfaktor:
                                            Zuschlag in Abhängigkeit vom gewählten Modell.
                                        • Faktor ’Große Scheibe‘, Faktor ’Kleine Scheibe‘:
                                            Zuschlag in Abhängigkeit von der Größe der Scheiben. Dazu geben Sie
                                            auch die Maße der Scheibe an.
                                        • Faktor ’ESG‘:
                                            Zuschlag, mit dem Sie die Handhabung von ESG berücksichtigen.
                                        • Faktor ’VSG‘:
                                            Zuschlag, mit dem Sie die Handhabung von VSG berücksichtigen.
                                        • Faktor ’mindestens Dreifach-ISO‘:
                                            Zuschlag, mit dem Sie die Handhabung von ISO berücksichtigen.
                                        • Beschichtungsfaktor:
                                            Zuschlag, mit dem Sie die Handhabung von beschichteten Scheiben be-
                                            rücksichtigen.
                                        • Vektor ’Gewicht -> Faktor‘:
                                            Zuschlag in Abhängigkeit vom Gewicht der Scheiben.
                                        • Vektor ’Länge -> Faktor‘:
                                            Zuschlag in Abhängigkeit von der zu bearbeitenden Kantenlänge.
                                        • Vektor ’Anzahl -> Faktor‘:
                                            Zuschlag in Abhängigkeit von der Anzahl der zu bearbeitenden Scheiben.
                                        • Vektor ’Dicke -> Faktor‘:
                                            Zuschlag in Abhängigkeit von der Dicke der Scheiben.
                                        • Vektor ’Fläche -> Faktor‘:
                                            Zuschlag in Abhängigkeit von der zu bearbeitenden Fläche.
                                        • Vektor ’Kantenmatrix -> Faktor‘:
                                            Zuschlag in Abhängigkeit von der Kantenmatrix der Scheiben.
                                        • ’Freies‘ Element 1 … 10:
                                            Freie Elemente für weitere Zeitzuschläge.

                                        + Wert, + Vektor, + Tabelle Auswahl der Rechenoperation für einen kon-
                                        stanten Wert, einen Vektor oder eine Tabelle:

                                        Einstellung       Bedeutung
4.50 / 01-2023




                                        + Tabelle         Der Wert aus der Tabelle wird zum Zwischenergebnis addiert.

                                        Tab. E-5      Mögliche Einstellungen für die Vorgabezeitformel




                 A+W Production Kapazitätsplanung                                                                 E-209
                 Stammdaten für Zeiten                                                                      Softwarereferenz




                                         Einstellung        Bedeutung

                                         + b * Wert         Die Basiszeit wird mit dem Wert multipliziert. Das Ergebnis der
                                                            Multiplikation wird zum Zwischenergebnis addiert.

                                         + Wert             Der Wert wird zum Zwischenergebnis addiert.

                                         * (1 + Wert)       Der Wert wird zu 1 addiert und das Ergebnis mit dem
                                                            Zwischenergebnis aus der vorausgehenden Zeile multipliziert.

                                         * Vektor           Das Ergebnis der vorausgehenden Zeile wird mit dem Wert
                                                            des Vektors multipliziert.

                                         Tab. E-5       Mögliche Einstellungen für die Vorgabezeitformel

                                            Berechnungsreihenfolge
                                            Bei der Berechnung müssen Sie die Operatorrangfolge der Mathematik be-
                                            rücksichtigen: Multiplikation und Division werden vor Addition und Subtrak-
                                            tion gerechnet – es sei denn, Klammern geben die Reihenfolge vor.
                                            Außerdem müssen Sie die Reihenfolge der Zeilen beachten, wenn eine
                                            Berechnung auf dem Ergebnis der vorausgehenden Zeile aufbauen soll.

                                         […] Öffnet den Dialog Vektor (Name), in dem Sie die Eigenschaften des Vek-
                                         tors bearbeiten.
                                          “Tabelle, Vektor (Name)” auf Seite E-213

                                         [Verschieben] Verschiebt ein markiertes Element in der Vorgabezeitformel.
                                         Die Reihenfolge der Faktoren ist wichtig, wenn Sie die Option Faktor multipli-
                                         ziert mit Zwischensumme wählen.

                                         Multiplikation des Formelergebnisses mit der Bearbeitungsmenge pro
                                         Teil Sie können das Formelergebnis mit der Bearbeitungsmenge pro Teil
                                         multiplizieren lassen.
                                          Das Formelergebnis wird nicht mit der Bearbeitungsmenge pro Teil multipli-
                                         ziert.
                                          Das Formelergebnis wird mit der Bearbeitungsmenge pro Teil multipliziert.

                                         Eigene Formel
                                         Anzeige der zugewiesenen Formel.

                                         [Lupe] Öffnet den Dialog Formel auswählen, in dem Sie hinterlegte Formeln
                                         auswählen.
                                          “Formel auswählen” auf Seite E-216

                                         [X] Entfernt die Formel aus dem Feld Eigene Formel.

                                         [Formeleditor] Öffnet den Dialog Erfassung eines Formelelements, in dem
                                         Sie eine Formel anlegen können.
                                         Zum Thema Formel-Editor gibt es ein separates Handbuch.
4.50 / 01-2023




                                          “Erfassung eines Formelelements” auf Seite E-217




                 E-210                                                                A+W Production Kapazitätsplanung
                 Softwarereferenz                                                            Stammdaten für Zeiten




                                        Formeltest Öffnet den Dialog Zeitformeltest, mit dem Sie Formeln zur Zeitbe-
                                        rechnung prüfen.
                                         “Zeitformeltest” auf Seite E-221

                                        [Neu] Öffnet den Dialog Elemente hinzufügen, in dem Sie Elemente aus-
                                        wählen können.
                                         “Elemente hinzufügen” auf Seite E-212

                                        [OK] Speichert die Daten.

                                        [Ende] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-211
                 Stammdaten für Zeiten                                                                  Softwarereferenz




                                         Elemente hinzufügen
                                         Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Neu]




                                         Abb. E-118   Elemente hinzufügen


                                         In diesem Dialog können Sie Elemente für Zeitzuschläge in den Dialog Vorga-
                                         bezeitformel übernehmen.
                                          Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118

                                         [Löschen] Löscht den markierten Eintrag.

                                         [OK] Übernimmt den markierten Eintrag in den Dialog Vorgabezeitformel.

                                         [Ende] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 E-212                                                              A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                Stammdaten für Zeiten




                                        Tabelle, Vektor (Name)
                                        Stammdaten > Kapazitätsplanung > Vorgabezeiten > logische Maschine mar-
                                        kieren > [Bearbeiten] > Element einfügen > […]




                                        Abb. E-119   Werterfassung – Tabellarische Erfassung, Matrixdarstellung


                                        In diesem Dialog bearbeiten Sie die Eigenschaften eines Zeitzuschlags. Sie
                                        können die Werte je nach Typ in der tabellarischen Erfassung bearbeiten.
                                         Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118

                                        Spalten Die Anzeige der Spalten hängt von dem Formelelement ab, zu dem
                                        der Dialog geöffnet ist, z. B. Dicke, Gewicht, Höhe und Breite.

                                           Beispiel Dicke

                                           Wenn Sie für die Dicke in der Tabelle die Werte 4,00 mm, 8,00 mm und
                                           10,00 mm angeben, gelten die zugewiesenen Faktoren jeweils für die Dicken
                                           4,00 bis 7,99 mm, 8,00 bis 9,99 mm, usw.


                                        Wert Faktor pro Dicke, Gewicht, Länge, Anzahl, Fläche oder Kantenmatrix.

                                        [Eingabehilfe] Öffnet den Dialog Eingabehilfe für Vektoren.
                                         “Eingabehilfe für Vektoren” auf Seite E-214

                                        [OK] Übernimmt den markierten Eintrag in den Dialog Vorgabezeitformel.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                 E-213
                 Stammdaten für Zeiten                                                                  Softwarereferenz




                                         Eingabehilfe für Vektoren
                                         Stammdaten > Kapazitätsplanung > Vorgabezeiten > logische Maschine mar-
                                         kieren > Bearbeiten > […] > Vektor einfügen > [Eingabehilfe]




                                         Abb. E-120   Eingabehilfe für Vektoren


                                         In diesem Dialog können Sie die Tabelle im Dialog Vektor … automatisch aus-
                                         füllen lassen, indem Sie Werte vorgeben.
                                          Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118

                                         Vorgabewerte
                                         In diesem Bereich geben Sie die Grenzwerte für die Berechnung der Tabelle
                                         ein.

                                         Startwert Startwert, mit dem die Tabelle beginnt.
                                         Der Startwert entspricht der Tabellen-Spalte Dicke, Gewicht, Länge, Anzahl,
                                         Fläche oder Kantenmatrix im Dialog Faktor/Vektor (Name).
                                         Geben Sie zum Beispiel bei dem Vektor ’Länge -> Faktor’ als Startwert die
                                         Länge von 100 mm an, um die Berechnung bei 100 mm zu beginnen.

                                         Endwert Endwert, mit dem die Tabelle schließt.
                                         Der Endwert entspricht der Tabellen-Spalte Dicke, Gewicht, Länge, Anzahl,
                                         Fläche oder Kantenmatrix im Dialog Faktor/Vektor (Name).
                                         Geben Sie zum Beispiel bei dem Vektor ’Länge -> Faktor’ als Endwert die Län-
                                         ge von 2000 mm an, um die Berechnung bei 2000 mm zu beenden.

                                         Schrittgröße Größe, mit der die Grenzwerte zwischen Start- und Endwert
                                         angelegt werden.
                                         Die Schrittgröße entspricht der Tabellen-Spalte Dicke, Gewicht, Länge, An-
                                         zahl, Fläche, oder Kantenmatrix im Dialog Faktor/Vektor (Name).
                                         Geben Sie zum Beispiel bei dem Vektor ’Länge -> Faktor’ als Schrittgröße
4.50 / 01-2023




                                         100 mm an. Damit bekommt der Vektor alle 100 mm einen anderen Wert zu-
                                         geordnet, z. B. 100,00 bis 199,00 mm, 200,00 bis 299,99 mm, usw.




                 E-214                                                              A+W Production Kapazitätsplanung
                 Softwarereferenz                                                           Stammdaten für Zeiten




                                        Werte
                                        In diesem Bereich geben Sie die Werte für die Berechnung der Zeitzuschläge
                                        pro Grenzwert ein.

                                        Startwert Wert, mit dem der Zeitzuschlag für den kleinsten der angegebe-
                                        nen Grenzwerte berechnet wird.
                                        Der Startwert entspricht der Tabellen-Spalte Faktor im Dialog Vektor ….
                                        Geben Sie zum Beispiel bei dem Vektor ’Länge -> Faktor’ als Startwert 1 an.
                                        Damit wird dem Vektor bei einer Länge zwischen 100 mm und 199,99 mm der
                                        Wert 1 zugeordnet.

                                        Schrittgröße Wert, um den der Berechnungswert pro Grenzwert erhöht
                                        wird.
                                        Die Schrittgröße entspricht der Tabellen-Spalte Faktor im Dialog Vektor ….
                                        Geben Sie zum Beispiel bei dem Vektor ’Länge -> Faktor’ als Schrittgröße 2
                                        an. Damit wird der Wert des Vektors alle 100 mm um den Wert 2 erhöht, z. B.
                                        die Werte 1, 3, 5, usw.

                                        [OK] Speichert die Daten.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                           E-215
                 Stammdaten für Zeiten                                                                  Softwarereferenz




                                         Formel auswählen
                                         Stammdaten > Kapazitätsplanung > Vorgabezeiten > Bearbeiten > Eigene
                                         Formel




                                         Abb. E-121   Formel auswählen


                                         In diesem Dialog können Sie definierte Formeln auswählen und im Dialog Vor-
                                         gabezeitformel einfügen.
                                          Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118

                                            Eigene Formeln
                                            Zusätzliche Formeln beeinflussen das Verhalten und die Eigenschaften
                                            von Vorgabezeitformeln unter Umständen massiv.
                                            Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH,
                                            falls Sie eigene Formeln benötigen oder bestehende Formeln ändern wol-
                                            len.

                                         ID Identifikationsnummer der Formel.

                                         Formel Name der Formel.

                                         Beschreibung Beschreibung der Formel.

                                         Sprache Auswahl der Sprache, in der die Formeln geschrieben sind. Wählen
                                         Sie z. B. English, werden nur Formeln angezeigt, die in dieser Sprache defi-
                                         niert sind.

                                         Text Formelsuche über den Namen.

                                         [OK] Speichert die Daten.

                                         [Verwerfen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-216                                                              A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                 Stammdaten für Zeiten




                                        Erfassung eines Formelelements
                                        Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formel-
                                        editor], [Neu]




                                        Abb. E-122    Zeitformel – Element erfassen


                                        In diesem Dialog können Sie ein eigenes Element zur Berechnung einer Zeit-
                                        formel erfassen.
                                         Tutorial, “Editor für Formelelemente” auf Seite E-113

                                        Name Name, der in der Auswahl der Formelelemente angezeigt wird.

                                        Elementtyp Auswahl des Elementtyps.
                                        • Festes Element:
                                           Ausdrücke ohne Benutzereingabe, z. B. Langkante. Diese Einstellung soll-
                                           ten Sie nicht mehr für neue Definitionen verwenden. Sie ist durch Freies
                                           Element abgelöst worden.
                                        • Bedingung:
                                           Ausdrücke mit einer Benutzereingabe, die verwendet wird, wenn die Be-
                                           dingung wahr ist.
                                        • Freies Element:
                                           Ausdrücke, bei denen das Ergebnis mit der Benutzereingabe gewichtet
                                           wird, z. B. Sekunden pro Schleifmeter.
                                        • Schwellenwert:
                                           Ausdrücke, bei denen der Schwellenwert für die Bedingung einstellbar ist,
                                           ohne die Formeldefinition zu verändern, z. B. Mengenzuschlag ab Benut-
                                           zereingabe.
                                        • Vektor:
                                           Ausdrücke, bei denen eine Tabelle mit Wertepaaren aus Mindestwerten
                                           und zu verwendenden Koeffizienten gepflegt wird.

                                        Beschriftung Bezeichnung, die im Dialog Vorgabezeitformel angezeigt
4.50 / 01-2023




                                        wird.

                                        Definition Formel für die Berechnung bei den Elementtypen Festes Element,
                                        Bedingung und Freies Element.


                 A+W Production Kapazitätsplanung                                                               E-217
                 Stammdaten für Zeiten                                                               Softwarereferenz




                                         Eingabeformat Format der Maßeinheit für die Elementtypen Schwellenwert
                                         und Vektor:
                                         • Einheitenlos:
                                            Keine Maßeinheit.
                                         • Dicke, Länge:
                                            Millimeter, inch.
                                         • Fläche:
                                            Quadratmeter, square foot.
                                         Mit der Einstellung wird gewährleistet, dass die Eingaben für die Parameter in
                                         der Einheit interpretiert werden, die in A+W Production konfiguriert ist.

                                         Beschriftung Bezeichnung, die im Dialog Vorgabezeitformel vor dem Be-
                                         rechnungswert angezeigt wird, z. B. sec. bei einem Zeitwert.

                                         Definition Anzeige der Formel für einen unabhängigen Parameter, der bei ei-
                                         nem Vektor oder Schwellenwert ausgewählt ist.
4.50 / 01-2023




                 E-218                                                            A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                 Stammdaten für Zeiten




                                        Benutzerdefinierte Tabellenelemente
                                        Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Neu] >
                                        <Neue Tabelle …>




                                        Abb. E-123   Benutzerdefinierte Tabellenelemente


                                        In diesem Dialog definieren Sie ein neues Tabellenelement für Vorgabezeitfor-
                                        meln.
                                         Tutorial, “Struktur von Vorgabezeitformeln” auf Seite E-108

                                        Eigenschaften

                                        Name Name des Tabellenelements.

                                        Typ Typ des Formelelements.
                                        Für Neue Tabelle stehen folgende Optionen zur Wahl:
                                        • Vektor (eindimensional)
                                        • Tabelle (zweidimensional
                                        • Würfel (dreidimensional)

                                        Wert 1, Wert 2, Wert 3 Öffnet den Dialog Grenzwert auswählen, in dem Sie
                                        einen Wert auswählen. Die Anzahl der Felder ist vom gewählten Tabellentyp
                                        abhängig.
                                         “Grenzwert auswählen” auf Seite E-220

                                        Beschreibung Beschreibung für die Tabellenelemente.

                                        [Löschen] Löscht das markierte Element.

                                        [Speichern] Speichert die Daten.
4.50 / 01-2023




                                        [Neu] Erstellt ein neues Tabellenelement.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu speichern.


                 A+W Production Kapazitätsplanung                                                               E-219
                 Stammdaten für Zeiten                                                              Softwarereferenz




                                         Grenzwert auswählen
                                         Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Neu] >
                                         <Neue Tabelle …> auswählen




                                         Abb. E-124   Grenzwerte für Tabellenelemente


                                         In diesem Dialog können Sie Grenzwerte für ein neues Tabellenelement aus-
                                         wählen. Das Tabellenelement wird für die Formel zur Berechnung von Vorga-
                                         bezeiten eingesetzt.
                                          “Benutzerdefinierte Tabellenelemente” auf Seite E-219

                                         [OK] Übernimmt die Daten.

                                         [Schließen] Schließt den Dialog, ohne die Daten zu übernehmen.
4.50 / 01-2023




                 E-220                                                             A+W Production Kapazitätsplanung
                 Softwarereferenz                                                             Stammdaten für Zeiten




                                        Zeitformeltest
                                        Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formel-
                                        test]




                                        Abb. E-125    Zeitformeltest


                                        In diesem Dialog können Sie Formeln zur Zeitberechnung prüfen lassen. Der
                                        Test betrifft immer das markierte Element im Dialog Vorgabezeitformel. Wenn
                                        die gesamte Vorgabezeitformel getestet werden soll, müssen Sie den Eintrag
                                        Basic Time markieren.
                                         Tutorial, “Zeitformel testen” auf Seite E-125

                                        Formelobjekt

                                        Formelobjekt (Name) Grafische Darstellung der Formelobjekte. Mit einem
                                        Doppelklick öffnen Sie einen Dialog, in dem Sie Werte für den Test eingeben
                                        können, z. B. die Scheibenmaße.
                                         “Eigenschaften des Formelobjekts” auf Seite E-223

                                        [Neu] Speichert ein neues Formelobjekt.

                                        [Laden] Lädt ein gespeichertes Formelobjekt.

                                        [Speichern] Speichert das geänderte Formelobjekt.

                                        [Hinzufügen] Fügt ein Element unter dem markierten Element ein.

                                        [Löschen] Löscht das markierte Element.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-221
                 Stammdaten für Zeiten                                                              Softwarereferenz




                                         Diagnosewerkzeuge

                                         Formel anzeigen Sie können sich die Syntax der Formel anzeigen lassen.
                                          Die Syntax der Formel wird nicht angezeigt.
                                          Öffnet den Dialog (Formelname), in dem die Syntax der Formel angezeigt
                                         wird und kopiert werden kann.
                                          “Formel (Name)” auf Seite E-225

                                         Auswertung protokollieren Sie können ein Protokoll der Formel-Auswer-
                                         tung erstellen lassen.
                                          Es wird kein Protokoll erstellt.
                                          Die Auswertung der Formel wird im Dialog Verlauf der Formelauswertung
                                         angezeigt.
                                          “Verlauf der Formelauswertung” auf Seite E-226

                                         Ergebnis Ergebnis der Zeitberechnung in Sekunden. Ein Pfeil nach oben
                                         oder nach unten zeigt an, ob das Ergebnis der Vorgabezeitformel höher oder
                                         niedriger als die Basiszeit ist.

                                         [Auswerten] Startet die Auswertung der Formel.
                                         Die Auswertung beginnt immer am markierten Formelobjekt. Haben Sie kein
                                         Element ausgewählt, beginnt die Auswertung am Kopfteil.
                                         Das Ergebnis der Auswertung wird im Feld Ergebnis angezeigt. Wenn Sie die
                                         Checkbox Auswertung protokollieren markiert haben, wird der Dialog Verlauf
                                         der Formelauswertung geöffnet.
                                          “Verlauf der Formelauswertung” auf Seite E-226

                                         [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-222                                                             A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                 Stammdaten für Zeiten




                                        Eigenschaften des Formelobjekts
                                        Stammdaten > Kapazitätsplanung > Vorgabezeiten > Bearbeiten > Formeltest
                                        > Doppelklick auf das Formelobjekt




                                        Abb. E-126    Zeitformeltest – Eigenschaften des Formelobjekts


                                        In diesem Dialog geben Sie die Daten für den Formeltest ein, z. B. eine Schei-
                                        be mit der Dicke 4 mm und einer Breite von 2.500 mm. In diesem Dialog wer-
                                        den Längen und Dicken in der Einheit Mikrometer µm angegeben.
                                         Tutorial, “Zeitformel-Objekte” auf Seite E-117

                                        Eigenschaften des Formelobjekts

                                        Name Name des Formelobjekts.

                                        Typ Auswahl der Option Teil oder Bearbeitung.

                                        Übersicht
                                        •   Eigenschaft:
                                            Zugeordnete Eigenschaft. In der Auswahl-Liste stehen alle Faktoren zur
                                            Verfügung, die Sie zur Vorgabezeitformel hinzugefügt haben und deren Ei-
                                            genschaften bearbeitet werden können.
                                        •   Wert:
4.50 / 01-2023




                                            Wert für die jeweilige Testberechnung. Bei Längen- und Dicken-Angaben
                                            in Mikrometer.



                 A+W Production Kapazitätsplanung                                                               E-223
                 Stammdaten für Zeiten                                                             Softwarereferenz




                                         [Hinzufügen] Fügt ein neues Element in der Liste Eigenschaft ein. Die An-
                                         zeige der Eigenschaften ist abhängig von den Elementen, die in die Vorgabe-
                                         zeitformel eingefügt sind.

                                         [Löschen] Löscht das markierte Element.

                                         [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-224                                                          A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                Stammdaten für Zeiten




                                        Formel (Name)
                                        Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formel-
                                        test] > Checkbox Formel anzeigen aktivieren




                                        Abb. E-127   Formel-Syntax


                                        In diesem Dialog wird die Formel in der natürlichen Syntax angezeigt, um Feh-
                                        ler in einer Vorgabezeitformel zu finden.
                                         Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118

                                        [Kopieren] Kopiert die Formel, um sie z. B. in einen Editor einzufügen.

                                        [Schließen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                E-225
                 Stammdaten für Zeiten                                                                  Softwarereferenz




                                         Verlauf der Formelauswertung
                                         Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formel-
                                         test] > Checkbox Auswertung protokollieren aktivieren > [Auswerten]




                                         Abb. E-128   Verlauf der Formelauswertung


                                         In diesem Dialog wird das Protokoll der Formelauswertung angezeigt. Diese
                                         Auswertung wird vom Support der A+W Software GmbH benötigt, um eine
                                         Formelberechnung zu analysieren.
                                          Tutorial, “Vorgabezeitformeln anlegen und verwalten” auf Seite E-118

                                         [Schließen] Schließt den Dialog.
4.50 / 01-2023




                 E-226                                                               A+W Production Kapazitätsplanung
                 Softwarereferenz                                                              Stammdaten für Zeiten




                                          Übergangszeiten
                                          Stammdaten > Kapazitätsplanung > Übergangszeiten




                 Abb. E-129   Übergangszeiten


                                          In diesem Dialog legen Sie Übergangszeiten zwischen (logischen) Maschinen
                                          fest. Sie können Übergangszeiten für den optimalen Übergang und für be-
                                          schleunigte Übergänge definieren. Mit der Angabe von minimalen und maxi-
                                          malen Zeiten legen Sie eine Spanne fest, in der der Übergang stattfinden
                                          kann. Bei der Planung wird immer der Übergang vom Ende einer Schicht aus
                                          betrachtet.
                                           Tutorial, “Übergangszeiten” auf Seite E-93
                                          Die Übergangszeiten werden hierarchisch abgearbeitet.
                                          •     Maschine x -> Maschine y beschreibt den expliziten Übergang zwischen
                                                zwei Maschinen.
                                          •     Maschine x -> Alle Maschinen beschreibt den Übergang am Ausgang von
                                                Maschine x.
                                          •     Alle Maschinen -> Maschine x beschreibt den Übergang am Eingang von
                                                Maschine x.
4.50 / 01-2023




                                          •     Alle Maschinen -> Alle Maschinen beschreibt den allgemeinen Übergang
                                                und wird zuletzt ausgewertet.
                                           Tutorial, “Übergangszeiten” auf Seite E-93



                 A+W Production Kapazitätsplanung                                                             E-227
                 Stammdaten für Zeiten                                                                Softwarereferenz




                                             Übergangszeiten in Schichten
                                             In der Regel werden Übergangszeiten in Schichten definiert. Nur in Aus-
                                             nahmefällen verwenden Sie die Dauer in Stunden und Minuten, z. B. bei
                                             Trocknungszeiten.

                                         Maschinen
                                         •   Maschine 1:
                                             Logische Maschine, von der aus der Übergang stattfindet.
                                             Mit einem Doppelklick in ein Feld öffnen Sie den Dialog zur Auswahl einer
                                             logischen Maschine.
                                         •   Maschine 2:
                                             Logische Maschine, zu der der Übergang stattfindet.
                                             Mit einem Doppelklick in ein Feld öffnen Sie den Dialog zur Auswahl einer
                                             logischen Maschine.
                                         •   Typ:
                                             Art der Übergangszeit:
                                             – Normal:
                                                 Normale Übergangszeit. Sie beschreibt den optimalen Durchgang
                                                 durch die Produktion, d. h. ohne Ausfälle von Personal oder Maschinen,
                                                 Bruch usw.
                                             – Eil:
                                                 Reduzierte Übergangszeit für Eilaufträge, z. B. ohne Verweilzeiten. Mit
                                                 dieser Zeit erhöhen sich die (virtuellen) Kosten. Diese Übergangszeiten
                                                 werden automatisch für Aufträge verwendet, die im ERP-System die
                                                 Priorität Eil haben. Diese Aufträge verwenden auch die für Eilaufträge
                                                 reservierten Arbeitsschichten.
                                             – Minimal:
                                                 Reduzierte Übergangszeit für Chef-Aufträge. Diese Einstellung dürfen
                                                 Sie nur verwenden, wenn eine weitere Reduktion technisch überhaupt
                                                 möglich ist. In der Regel wird diese Einstellung nur verwendet, wenn
                                                 eine Mindestzeit eingehalten werden muss, z. B. nach dem Autoklav.
                                                 Nur die Übergangszeit aus der Spalte Übergangszeit 'h:m' wird verwen-
                                                 det.
                                             – Verboten:
                                                 Maschine 2 darf nicht nach Maschine 1 angesteuert werden. Mit dieser
                                                 Einstellung können Sie z. B. abbilden, dass eine Maschine nicht ohne
                                                 innerbetrieblichen Transport erreichbar ist.
                                         •   Übergangszeit 'h:m':
                                             Minimale Übergangszeit in Stunden und Minuten. Diese Einstellung wird
                                             dann verwendet, wenn die Zeit auch über arbeitsfreie Tage gerechnet wird.
                                             Sie können die minimale Übergangszeit und die maximale Übergangszeit
                                             in gemischten Einheiten angeben, z. B. eine optimale Übergangszeit von
                                             2 Stunden und eine maximale Übergangszeit von 2 Schichten.
                                         •   Schichten:
                                             Minimale Übergangszeit in Schichten.
                                         •   Maximale Übergangszeit 'h:m':
                                             Maximale Übergangszeit in Stunden und Minuten. Hierbei muss ein Wert
4.50 / 01-2023




                                             eingetragen werden, der mindestens ein Wochenende beschreibt, da die
                                             Maschine sonst ggf. am Freitag nicht verwendet wird.




                 E-228                                                             A+W Production Kapazitätsplanung
                 Softwarereferenz                                                            Stammdaten für Zeiten




                                        •   Maximale Schichten:
                                            Maximale Übergangszeit in Schichten. Der Wert der maximalen Über-
                                            gangszeit wird zur minimalen Übergangszeit addiert. So ergibt sich z. B.
                                            aus einer minimalen Übergangszeit von 1 Schicht und einer maximalen
                                            Übergangszeit von 3 Schichten eine Übergangszeit von 1 bis 4 Schichten.
                                            Sie können die minimale Übergangszeit und die maximale Übergangszeit
                                            in gemischten Einheiten angeben, z. B. eine minimale Übergangszeit von
                                            2 Stunden und eine maximale Übergangszeit von 2 Schichten.

                                            Beispiel

                                            Übergangstyp      Schichten       Maximale       Spanne in
                                                                              Schichten      Schichten

                                            Normal                2               2              4
                                                                  2               1              3

                                            Eil                   1                              1

                                            Minimal               1                              1

                                            Tipp
                                            Wählen Sie für den Übergang zur letzten Bearbeitung, z. B. Verpacken
                                            oder Versand, die größte Übergangszeit, die möglich ist. Damit haben Sie
                                            in kritischen Situationen größere Flexibilität.

                                        [Neu] Schaltet eine neue Zeile frei, um eine Übergangszeit zu definieren.

                                        [Löschen] Löscht den markierten Eintrag.

                                        [OK] Übernimmt den markierten Eintrag in den Dialog Vorgabezeitformel.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                             E-229
                 Stammdaten der Schichten                                                          Softwarereferenz




                                       Stammdaten der Schichten
                                       Neben den Vorgabe- und Übergangszeiten können auch Schichten definiert
                                       werden, in denen die Arbeitszeiten in der Produktion pro Tag definiert werden
                                       können.
                                       In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                       •    “Schichten” auf Seite E-231
                                       •    “Schichtkalender” auf Seite E-233
                                       •    “Schichtplan” auf Seite E-234
                                       •    “Schichtregel” auf Seite E-236
                                       •    “Schichtgruppe” auf Seite E-238
                                       •    “Maschine” auf Seite E-240
4.50 / 01-2023




                 E-230                                                          A+W Production Kapazitätsplanung
                 Softwarereferenz                                                            Stammdaten der Schichten




                                          Schichten
                                          Stammdaten > Kapazitätsplanung > Schichten
                                          Zum Dialog Schichten finden Sie folgende Kapitel:
                                          •   “Schichtkalender” auf Seite E-233
                                          •   “Schichtplan” auf Seite E-234
                                          •   “Schichtregel” auf Seite E-236
                                          •   “Schichtgruppe” auf Seite E-238
                                          •   “Maschine” auf Seite E-240




                 Abb. E-130   Schichten


                                          In diesem Dialog verwalten Sie die Schichtpläne.

                                              Schichten ändern
                                              Änderungen an Schichtplänen stellen einen tiefen Eingriff in die Kapazi-
                                              tätsplanung dar. Prüfen Sie im Produktionsmonitor, ob Änderungen korrekt
                                              in Arbeitsschichten umgesetzt sind.
                                              Bereits eingelastete Aufträge werden nicht automatisch umgelastet. Än-
                                              dern Sie Schichtpläne daher so, dass sie erst zu einem Zeitpunkt zur Ver-
                                              fügung stehen, zu dem aktuell noch keine Aufträge eingelastet sind.
                                              Für kurzfristige Änderungen stehen verschiedene Funktionen im Produkti-
                                              onsmonitor zur Verfügung.
4.50 / 01-2023




                                              Bei Fragen wenden Sie sich an den Kundenservice der A+W Software
                                              GmbH.

                                           Tutorial, “Schichten” auf Seite E-69


                 A+W Production Kapazitätsplanung                                                               E-231
                 Stammdaten der Schichten                                                         Softwarereferenz




                                       Schichteditor
                                       Im Bereich Schichteditor werden der Kalender und die Schichtpläne ange-
                                       zeigt. Über das Kontextmenü oder die Schaltflächen können Sie die verschie-
                                       denen Ansichten für die Definition der Schichtpläne öffnen:
                                       •    Schichtkalender
                                       •    Schichtplan
                                       •    Schichtregel
                                       •    Schichtgruppe
                                       •    Maschine

                                       [Neu] Öffnet die Ansicht Schichtkalender, um einen neuen Kalender zu defi-
                                       nieren.

                                       [Löschen] Löscht den markierten Eintrag.

                                       [Übernehmen] Speichert die Daten.

                                       [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-232                                                        A+W Production Kapazitätsplanung
                 Softwarereferenz                                                                   Stammdaten der Schichten




                                           Schichtkalender
                                           Stammdaten > Kapazitätsplanung > Schichten > Kalender




                 Abb. E-131   Schichten – Kalender


                                           In dieser Sicht des Dialogs definieren Sie die arbeitsfreien Tage.
                                            Tutorial, “Arbeitsfreie Tage anlegen” auf Seite E-72

                                           Schichtkalender Angabe der arbeitsfreien Tage, zum Beispiel Feiertage.

                                           Tag Datum des arbeitsfreien Tags.

                                           Kommentar Bezeichnung des arbeitsfreien Tags, zum Beispiel Weihnach-
                                           ten.

                                           [Neu] Fügt im Schichtkalender eine neue Zeile ein, um einen arbeitsfreien
                                           Tag zu definieren.
                                           Über die Auswahl-Liste erstellen Sie einen neuen Schichtplan.

                                           [Löschen] Löscht den markierten Tag aus dem Schichtkalender.

                                           [Übernehmen] Speichert die Daten.

                                           [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                                     E-233
                 Stammdaten der Schichten                                                                Softwarereferenz




                                           Schichtplan
                                           Stammdaten > Kapazitätsplanung > Schichten > Schichtplan




                 Abb. E-132   Schichten, Schichtplan


                                           In dieser Sicht des Dialogs verwalten Sie die Schichtpläne, mit denen Sie die
                                           Arbeitsschichten definieren.
                                            Tutorial, “Schichtplan erstellen” auf Seite E-75

                                           Schichtplan
                                           In diesem Bereich erstellen und verwalten Sie einen Schichtplan, z. B. einen
                                           Zwei-Schicht-Plan oder einen Drei-Schicht-Plan.

                                           ID ID des Schichtplans.

                                           Name Frei wählbarer Name des Schichtplans.

                                           Aktiv Sie können festlegen, ob der Schichtplan für die Planung von wöchent-
                                           lichen Kampagnen verwendet werden kann.
                                            Der Schichtplan steht nicht für Wöchentliche Termine zur Verfügung. Er
                                           kann im Dialog Kampagnen nicht ausgewählt werden.
                                            Der Schichtplan steht für Wöchentliche Termine zur Verfügung.
4.50 / 01-2023




                                           Gültig ab Angabe des Datums, ab dem der Schichtplan gültig ist. Damit kön-
                                           nen Sie den Schichtplan einrichten, ohne dass die Arbeitsschicht sofort zur
                                           Verfügung steht, z. B. für Sonderschichten an einem Wochenende.


                 E-234                                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                         Stammdaten der Schichten




                                        Schichten generieren
                                        Mit der Wahl der Option legen Sie fest, welcher Kalender für den Schichtplan
                                        verwendet wird:
                                        •   Eigenen Kalender verwenden:
                                            Verwendet den Kalender, den Sie im Schichtkalender definiert haben.
                                        •   Kalender aus ERP-System übernehmen:
                                            Importiert einen Kalender aus einem ERP-System, z. B. aus A+W Busi-
                                            ness.

                                        Von …, bis … Angabe des Start- und Enddatums. Arbeitsschichten nach
                                        diesem Schichtplan werden im Produktionsmonitor nur für den angegebenen
                                        Zeitraum erzeugt.

                                        [Erzeugen] Erzeugt im Produktionsmonitor eine Arbeitsschicht mit den neu-
                                        en Daten, die Sie eingegeben haben.
                                        Die Schaltfläche wird erst freigeschaltet, wenn Sie eine Schichtregel und eine
                                        Schichtgruppe mit Maschinen zugewiesen haben.

                                        [Neu] Legt einen neuen Schichtplan an.
                                        Mit der Auswahl-Liste erstellen Sie eine neue Schichtregel.

                                        [Löschen] Löscht einen markierten Schichtplan.

                                        [Übernehmen] Speichert die Daten.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-235
                 Stammdaten der Schichten                                                                Softwarereferenz




                                           Schichtregel
                                           Stammdaten > Kapazitätsplanung > Schichten > Schichtregel




                 Abb. E-133   Schichten – Schichtregel


                                           In dieser Sicht des Dialogs verwalten Sie die Schichtregeln eines Schicht-
                                           plans.
                                            Tutorial, “Schichtregel erstellen” auf Seite E-78

                                           Schichtregel
                                           Schichtregel gelten jeweils für einen einzelnen Schichtplan. Sie können jeder
                                           Schichtregel eine Schichtgruppe zuordnen.

                                           Name Frei wählbaren Namen der Schichtregel, z. B. Frühschicht normal.

                                           Schichtbeginn, Schichtende Angabe der Uhrzeit, zu der die Arbeitsschicht
                                           beginnt und endet.

                                           Kapazität Anzeige der Kapazität der Arbeitsschicht in Stunden. Sie wird aus
                                           dem Schichtbeginn und dem Schichtende berechnet.

                                           Schichtnummer Eingabe der Schichtnummer.
4.50 / 01-2023




                 E-236                                                                  A+W Production Kapazitätsplanung
                 Softwarereferenz                                                         Stammdaten der Schichten




                                        Tage Angabe der Wochentage, an denen die Arbeitsschicht gefahren werden
                                        kann.
                                         Die Arbeitsschicht wird nicht erzeugt.
                                         Die Arbeitsschicht kann im Produktionsmonitor erzeugt werden.

                                        Schichten generieren
                                        Mit der Wahl der Option legen Sie fest, welcher Kalender für den Schichtplan
                                        verwendet wird:
                                        •   Eigenen Kalender verwenden:
                                            Verwendet den Kalender, den Sie im Schichtkalender definiert haben.
                                        •   Kalender aus ERP-System übernehmen:
                                            Importiert einen Kalender aus einem ERP-System, z. B. aus A+W Busi-
                                            ness.

                                        Von …, bis … Angabe des Start- und Enddatums. Arbeitsschichten nach
                                        diesem Schichtplan werden im Produktionsmonitor nur für den angegebenen
                                        Zeitraum erzeugt.

                                        [Löschen] Löscht die markierte Schichtregel mit allen zugeordneten Ma-
                                        schinen. Damit werden die zugehörigen Arbeitsschichten aus dem Produk-
                                        tionsmonitor gelöscht.

                                        [Erzeugen] Erzeugt im Produktionsmonitor Arbeitsschichten mit den neuen
                                        Daten, die Sie eingegeben haben.
                                        Die Schaltfläche wird erst freigeschaltet, wenn Sie eine Schichtgruppe mit Ma-
                                        schinen zugewiesen haben.

                                        [Neu] Erstellt eine neue Schichtregel. Die Auswahl-Liste wird derzeit nicht
                                        verwendet.

                                        [Löschen] Löscht eine markierte Schichtregel.

                                        [Übernehmen] Speichert die Daten.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                              E-237
                 Stammdaten der Schichten                                                               Softwarereferenz




                                           Schichtgruppe
                                           Stammdaten > Kapazitätsplanung > Schichten > Schichtgruppe




                 Abb. E-134   Schichten – Schichtgruppe bearbeiten


                                           In dieser Sicht des Dialogs ordnen Sie einer Schichtgruppe die Erfassungs-
                                           stellen zu. Pro Schichtregel kann jeweils eine Schichtgruppe erstellt werden.
                                            Tutorial, “Schichtgruppe erstellen” auf Seite E-83

                                           Schichtgruppe bearbeiten

                                           Name der Schichtgruppe Name der Schichtgruppe, der die Erfassungsstel-
                                           len zugeordnet sind.

                                           Erfassungsstellennummer Nummer der Erfassungsstelle.

                                           Name Name der Erfassungsstelle.

                                           Schichtgruppe Schichtgruppe, die der Erfassungsstelle für den aktuellen
                                           Schichtplan zugeordnet ist. Sie können eine andere Schichtgruppe auswäh-
                                           len.

                                           [Neu] Erstellt eine neue Schichtgruppe. Jeder Schichtregel kann nur eine
                                           Schichtgruppe zugeordnet werden.
4.50 / 01-2023




                                           [Löschen] Löscht eine markierte Schichtgruppe.



                 E-238                                                                 A+W Production Kapazitätsplanung
                 Softwarereferenz                                                      Stammdaten der Schichten




                                        [Übernehmen] Speichert die Daten.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                        E-239
                 Stammdaten der Schichten                                                              Softwarereferenz




                                          Maschine
                                          Stammdaten > Kapazitätsplanung > Schichten > Schichtgruppe > Maschine




                 Abb. E-135   Schichten – Maschine


                                          In dieser Sicht des Dialogs weisen Sie einer Erfassungsstelle die logischen
                                          Maschinen zu.
                                           Tutorial, “Schichtgruppe erstellen” auf Seite E-83

                                          Erfassungsstelle
                                          Eigenschaften der markierten Erfassungsstelle und die logischen Maschinen,
                                          die der Erfassungsstelle zugeordnet sind.

                                          Nummer ID der Maschine.

                                          Name Name der Maschine.

                                          Barcode Barcode der Maschine.

                                          Maschinen Logische Maschinen, die der Erfassungsstelle zugeordnet sind.
4.50 / 01-2023




                 E-240                                                                A+W Production Kapazitätsplanung
                 Softwarereferenz                                                      Stammdaten der Schichten




                                        [Löschen] Löscht die markierte logische Maschine.

                                        [Übernehmen] Speichert die Daten.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                        E-241
                 Maschinen und Kosten                                                              Softwarereferenz




                                        Maschinen und Kosten
                                        Maschinen können zur Gruppen zusammengefasst werden, um die verfügba-
                                        ren Zeiten besser zu verplanen. Außerdem werden an den Maschinen die
                                        Kosten hinterlegt.
                                        In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                        •   “Kostenkalkulation” auf Seite E-243
                                        •   “Maschinengruppen” auf Seite E-245
                                        •   “Lastverteilung” auf Seite E-247
4.50 / 01-2023




                 E-242                                                            A+W Production Kapazitätsplanung
                 Softwarereferenz                                                             Maschinen und Kosten




                                        Kostenkalkulation
                                        Stammdaten > Kapazitätsplanung > Kostenkalkulation




                                        Abb. E-136    Kostenkalkulation


                                        In diesem Dialog legen Sie Kosten fest, die an logischen Maschinen anfallen.
                                        Wenn Ihre PPS- und ERP-Systeme vollständig eingerichtet sind, werden die
                                        Kosten an das ERP-System zurückgemeldet, z. B. an A+W Enterprise oder
                                        A+W Business.
                                         Tutorial, “Kostenkalkulation” auf Seite E-88

                                        Kosten
                                        In der Übersicht werden alle definierten Maschinen angezeigt.
                                        •   Maschine:
                                            Nummer und Name der physikalischen Maschine, für die Kosten definiert
                                            sind.
                                            Mit einem Doppelklick öffnen Sie einen Dialog zur Auswahl einer Maschi-
                                            ne.
                                        •   Log. Maschine:
                                            Zugeordnete logische Maschine, zu der die Kosten definiert sind.
                                            Mit einem Doppelklick öffnen Sie einen Dialog zur Auswahl einer logischen
                                            Maschine.
                                        •   Lohnkosten:
                                            Lohnkosten der logischen Maschine in der Landeswährung.
4.50 / 01-2023




                                        •   Maschinenkosten:
                                            Maschinenkosten für die logische Maschine in der Landeswährung.



                 A+W Production Kapazitätsplanung                                                             E-243
                 Maschinen und Kosten                                                               Softwarereferenz




                                        •   Sonstige Kosten:
                                            Sonstige Kosten der logischen Maschine in der Landeswährung. Mit die-
                                            sen Kosten können Sie z. B. berücksichtigen, dass an einer Maschine zu-
                                            sätzliche Schutzkleidung notwendig ist und kostentechnisch berücksichtigt
                                            werden muss.
                                        •   Kommentar:
                                            Kommentare zur logischen Maschine.

                                        [Neu] Schaltet eine neue Zeile frei, um weitere Maschinenkosten anzulegen.

                                        [Löschen] Löscht den markierten Eintrag.

                                        [OK] Übernimmt den markierten Eintrag in den Dialog Vorgabezeitformel.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-244                                                           A+W Production Kapazitätsplanung
                 Softwarereferenz                                                            Maschinen und Kosten




                                        Maschinengruppen
                                        Stammdaten > Kapazitätsplanung > Maschinengruppen




                                        Abb. E-137   Maschinengruppen


                                        In diesem Dialog können Sie Maschinen zu Gruppen zusammenfassen und
                                        eine Anzahl von Personen zuordnen. Damit gilt eine festgelegte Kapazität für
                                        die gesamte Maschinengruppe, z. B. für Arbeitsbereiche wie Zuschnitt, ISO
                                        oder Versand.
                                        Das Zusammenfassen zu einer Maschinengruppe funktioniert nur, wenn die
                                        Schichtpläne aller Maschinen in der Gruppe übereinstimmen.
                                        Wenn eine Maschine zu einer Maschinengruppe hinzugefügt wird, wird sie au-
                                        tomatisch zu einem Engpassbetriebsmittel. Die Überlasteinstellungen der lo-
                                        gischen Maschine werden dabei an die Überlasteinstellungen aller logischen
                                        Maschinen in der Gruppe angepasst.
                                         Tutorial, “Maschinengruppen” auf Seite E-132

                                        Maschinengruppen

                                        Gruppe Liste der definierten Maschinengruppen.

                                        Personen Anzahl der Personen, die in der jeweiligen Maschinengruppe tätig
                                        sind.
4.50 / 01-2023




                 A+W Production Kapazitätsplanung                                                            E-245
                 Maschinen und Kosten                                                              Softwarereferenz




                                        Maschinen für Gruppe
                                        Im Feld auf der linken Seite sind die logischen Maschinen angezeigt, die zu
                                        einer markierten Maschinengruppe hinzugefügt werden können. Auf der rech-
                                        ten Seite sind die logischen Maschinen angezeigt, die zur Maschinengruppe
                                        hinzugefügt sind.

                                        [Zuordnen] Verschiebt ein markiertes Element auf die andere Seite.

                                        [Neu] Öffnet einen Dialog, um eine neue Maschinengruppe anzulegen.

                                        [Löschen] Löscht den markierten Eintrag.

                                        [OK] Speichert die Daten.

                                        [Ende] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-246                                                         A+W Production Kapazitätsplanung
                 Softwarereferenz                                                               Maschinen und Kosten




                                        Lastverteilung
                                        Stammdaten > Kapazitätsplanung > Lastverteilung




                                        Abb. E-138    Lastverteilung


                                        In diesem Dialog definieren Sie den prozentualen Anteil der logischen Maschi-
                                        nen an der Kapazität der physikalischen Maschine. Sind zu einer Maschine
                                        zwei logische Maschinen definiert, können Sie die 100 % Last der Maschine
                                        auf die logischen Maschinen aufteilen, z. B. zu jeweils 50 %.
                                        Lastverteilung nutzen Sie, um zu gewährleisten, dass eine Maschine eine ga-
                                        rantierte Mindestkapazität für Spezialaufgaben freihält, z. B. für den Modellzu-
                                        schnitt. Wenn die freigehaltene Kapazität nicht für Modelle genutzt wird,
                                        können auch Rechtecke bearbeitet werden. Diese Lastverteilung ist nur bei
                                        Maschinen möglich und sinnvoll, die als Engpassbetriebsmittel definiert sind.
                                         Tutorial, “Lastverteilung” auf Seite E-138

                                        Lastverteilung

                                        Physikalische Maschinen Auswahl der Maschinen, um die Lastverteilung
                                        zu bearbeiten.

                                        Prüfung aktivieren Die Lastverteilung ist gesperrt, um versehentliche Än-
                                        derungen zu verhindern.
                                         Die Lastverteilung der logischen Maschinen in der Liste kann nicht bearbei-
                                        tet werden.
4.50 / 01-2023




                                         Die Lastverteilung der logischen Maschinen in der Liste kann bearbeitet
                                        werden.




                 A+W Production Kapazitätsplanung                                                                E-247
                 Maschinen und Kosten                                                          Softwarereferenz




                                        [OK] Speichert die Daten.

                                        [Abbrechen] Schließt den Dialog, ohne die Daten zu speichern.
4.50 / 01-2023




                 E-248                                                       A+W Production Kapazitätsplanung
Kapazitätsplanung            E

                       Partindex




                A+W Production
                 Partindex                                                                              Index




                 Index
                 A                                           Berechnungsreihenfolge E-210
                 Abgelaufene Reservierungen E-192            – Vorgabezeitformel E-112
                 Abgelaufene Reservierungen löschen E-61
                 Aktion für Stücklistenkonfiguration E-173   C
                 Alternativmaschinen E-19                    Chefauftrag   E-176
                 Änderung verplanter Aufträge E-184
                 Arbeitsfreie Tage
                                                             E
                 – anlegen E-72
                                                             Eigene Filter (Produktionsmonitor) E-159
                 – bearbeiten E-73
                                                             Eigenschaften Formelobjekt E-223
                 – löschen E-74
                                                             Eingabehilfe für Vektoren E-214
                 Arbeitsplan
                                                             Einlastung E-148, E-171
                 – Exportieren E-34
                                                             – Änderung verplanter Aufträge E-184
                 Arbeitsschicht
                                                             – Asynchrone Verarbeitung E-183
                 – Anpassungen E-24
                                                             – Aufträge einlasten E-36
                 – Engpass E-28
                                                             – Bearbeitungserzeugung E-64
                 – Maschine E-29
                                                             – Fehler E-41, E-179
                 – reservieren E-27
                                                             – Fehlerhafte Aufträge E-182
                 – sperren E-26
                                                             – nachbearbeiten E-42
                 – verlängern, verkürzen E-27
                                                             – Nachbearbeitung Einlastung E-179
                 – zusätzlich einrichten E-25
                                                             – Positionssplit E-185
                 Arbeitsschichten E-22, E-149
                                                             – Stücklistenkonfiguration E-172
                 – Darstellung E-32
                                                             Einlastungsregeln E-14
                 Arbeitsschichten erzeugen E-78
                                                             Einzeltermin (Kampagne) E-189
                 Asynchrone Verarbeitung E-183
                                                             Einzeltermine in Kampagne anlegen E-48
                 Auftrag
                                                             Elemente hinzufügen (Vorgabezeit) E-212
                 – auswählen (Produktionsmonitor) E-157
                                                             Engpass
                 – einlasten E-36
                                                             – Arbeitsschicht E-28
                 – Einlastung nachbearbeiten E-42
                                                             – Maschine E-30
                 – Reservierung E-55
                                                             Exportieren
                 – Umlastung E-37
                                                             – Arbeitsplan E-34
                 Automatische Umlastung E-17

                                                             F
                 B
                                                             Faktoren E-213
                 Bearbeitung
                                                             Faktoren (Vorgabezeitformel) E-109
                 – auflösen E-66
                                                             Fehler
                 – ergänzen E-65
                                                             – Einlastung E-41
                 – erzeugen E-65
                                                             Fehlerhafte Aufträge E-182
                 – Umlastung E-38
                                                             Feste Elemente (Vorgabezeitformel) E-109
                 Bearbeitungen
                                                             Formel auswählen E-216
                 – Positionen splitten E-185
                                                             Formelauswertung E-226
                 – umlasten E-39
                                                             Formelobjekt E-221
                 Bearbeitungsdauer siehe Vorgabezeiten
                 Bearbeitungserzeugung E-64, E-201
                 – Bearbeitung entfernen E-66                K
                 – Bedingung hinzufügen E-204                Kalender
                                                             – arbeitsfreie Tage anlegen E-72
4.50 / 01-2023




                 – Reihenfolge E-202
                 – Sequenz E-202                             – arbeitsfreie Tage bearbeiten E-73
                 Bearbeitungsketten E-17                     – arbeitsfreie Tage löschen E-74
                 Benutzerdefinierte Tabellenelemente E-219   Kampagne


                 A+W Production Kapazitätsplanung                                                   E-251
                 Index                                                                               Partindex




                 – anlegen E-47                               – löschen E-137
                 – bearbeiten E-52                            Maschinengruppen E-245
                 – deaktivieren E-53                          – Definition E-133
                 – Einzeltermin anlegen E-48                  Maschinenschichten E-149
                 – löschen E-53                               Maschinenumlastung E-178
                 – Termin löschen E-52                        Maschinenwege
                 – wöchentlichen Termin anlegen E-50          – Alternativmaschinen E-19
                 Kampagnen E-188                              – Bearbeitungsketten E-17
                 – Einzeltermine E-189                        Matrix für Übergangszeiten E-101
                 – Einzeltermine, Wöchentliche Termine E-45
                 – Kampagnentage E-190                        N
                 – Terminfindung E-47                         Nachbearbeitung Einlastung E-179
                 – Wöchentliche Termine E-191                 – Änderung verplanter Aufträge E-184
                 Kampagnentage E-190                          – Fehlerhafte Aufträge E-182
                 Kapazität reservieren E-55                   Neuen Filter erstellen
                 Kosten E-243                                 (Produktionsmonitor) E-160
                 – anlegen E-90
                 – bearbeiten E-91
                 – löschen E-92                               O
                 Kostenkalkulation E-243                      Objekt auswählen (Reservierung)    E-199
                 – Definition E-89
                 Kunde für Reservierung auswählen E-198       P
                                                              Positionen splitten E-185
                 L                                            Produktionsmonitor E-22, E-149
                 Lastverteilung E-247                         – angezeigte Maschinen E-153
                 – bearbeiten E-142                           – Anpassungen E-24
                 – Definition E-139                           – Anzeige einstellen E-32
                 – einrichten E-140                           – Arbeitsschichten erzeugen E-78
                 – löschen E-143                              – Auftrag auswählen
                 Lauf auswählen (Produktionsmonitor) E-157      (Produktionsmonitor) E-157
                 Logische Maschine                            – Darstellung der Schichten E-154
                 – Kosten anlegen E-90                        – Detailansicht E-24
                 – Schichtgruppe E-240                        – Eigene Filter E-159
                 – Vorgabezeit E-107                          – Einstellungen E-154
                 Logische Maschine siehe auch Maschine        – Lauf auswählen E-157
                                                              – Maschine E-161
                                                              – Maschinen anzeigen E-31
                 M                                            – nach Auftrag filtern E-157
                 Maschine                                     – nach Lauf filtern E-158
                 – Anzeigeart einstellen E-33                 – neuen Filter erstellen E-160
                 – Arbeitsschicht E-29                        – Schichteigenschaften E-164
                 – Engpass E-30                               – Schichten anpassen E-163
                 – Kosten anlegen E-90                        Produktionstermine
                 – Kosten bearbeiten E-91                     – Bewertung E-19
                 – Kosten löschen E-92
                 – Umlastung E-37
                 Maschine siehe auch Logische Maschine        R
                 Maschinen                                    Regeln
                 – Anzeige im Produktionsmonitor E-153        – Terminfindung E-16
                 – im Produktionsmonitor anzeigen E-31        – Terminoptimierung E-15
4.50 / 01-2023




                 Maschinengruppe                              Reservierung
                 – anlegen E-134                              – abgelaufen E-56
                 – bearbeiten E-136                           – abgelaufene Reservierung löschen E-61



                 E-252                                                    A+W Production Kapazitätsplanung
                 Partindex                                                                           Index




                 – abgelaufene Reservierungen E-192          Stücklistenkonfiguration   E-172
                 – anlegen E-57
                 – Auftrag E-55                              T
                 – bearbeiten E-59                           Tabelle (Vorgabezeitformel) E-110
                 – Kapazitäten E-55                          Termine
                 – Konfiguration E-54                        – Kampagne anlegen E-48, E-50
                 – Kunde auswählen E-198                     – Kampagnen E-45
                 – löschen E-60                              Terminfindung E-16
                 – Objekt auswählen E-199                    – Kampagnen E-47
                 – pro Maschine E-195                        – Maschinenwege E-17
                 – pro Schicht E-195                         – Produktionstermine E-19
                 Reservierung für Maschine E-197             – Stückliste E-16
                 Reservierungen E-194                        – Übergangszeiten E-95
                 – pro Kunde E-195                           Terminoptimierung
                 – tageweise, wochenweise E-195              – Regeln E-15

                 S                                           U
                 Schicht                                     Übergang
                 – Sonderfall für Wechsel E-98               – in Stunden oder Schichten E-95
                 Schichteigenschaften E-164                  – Schichten E-96
                 Schichten E-231                             – Stunden E-97
                 – Logische Maschine E-240                   Übergangszeit
                 – Schichtgruppe E-83, E-238                 – anlegen E-102
                 – Schichtkalender E-233                     – bearbeiten E-104
                 – Schichtplan E-77, E-234                   – löschen E-104
                 – Schichtregel E-81, E-236                  – Schichten E-96
                 – Übergangszeit E-228                       – Sonderfall E-98
                 Schichten anpassen E-163                    – Stunden E-97
                 Schichtgruppe E-238                         – Typ E-100
                 – bearbeiten E-86                           Übergangszeiten E-93, E-227
                 – erstellen E-83                            – Definition E-99
                 – löschen E-87                              – Matrix E-101
                 Schichtkalender E-233                       – Schichten E-228
                 Schichtplan E-234                           – Terminfindung E-95
                 – bearbeiten E-77                           Umlastung E-174
                 – erstellen E-76                            – Auftrag E-37
                 – löschen E-78                              – Bearbeitung E-38
                 Schichtpläne E-70                           – Chefauftrag E-174
                 Schichtregel E-236                          – Maschine E-37
                 – bearbeiten E-81                           – Maschinenumlastung E-178
                 – erstellen E-79                            – Termin sperren E-174
                 – löschen E-82                              – Wareneingang E-176
                 Schichtreservierungen E-195
                 Schichtwechsel Sonderfall E-98
                 Schwellenwert (Vorgabezeitformel)   E-116   V
                 Sequenz (Bearbeitungserzeugung)     E-202   Vektoren E-213
                 Stammdaten                                  – Eingabehilfe E-111
                 – Kapazitätsplanung E-14                    – in Vorgabezeitformel anwenden E-122
                 – Maschinenzuordnung E-14                   Vektoren (Vorgabezeitformel) E-110
4.50 / 01-2023




                 – Schutz, Datensicherung E-68               Verlauf der Formelauswertung E-226
                 Stückliste                                  Verweildauer siehe Übergangszeiten
                 – Teileketten E-16                          Vorgabezeiten E-206
                                                             – Definition E-107


                 A+W Production Kapazitätsplanung                                                    E-253
                 Index                                                                 Partindex




                 Vorgabezeitformel E-108, E-208
                 – Bedingung für Modell E-116
                 – Bedingung für Rundbogen E-115
                 – Bedingung für Schwellenwert E-116
                 – Beispiel E-114
                 – Benutzerdefinierte Tabellenelemente E-219
                 – Berechnung testen E-126
                 – Berechnungsreihenfolge E-112, E-210
                 – definieren E-119
                 – Eigenschaften Formelobjekt E-223
                 – Eingabehilfe Vektoren E-111, E-214
                 – Elemente hinzufügen E-212
                 – Faktoren E-109, E-213
                 – Feste Elemente E-109
                 – Formel E-225
                 – Formel anzeigen E-225
                 – Formel auswählen E-216
                 – Formel kopieren E-225
                 – Formeleditor E-113
                 – Formelobjekt E-221
                 – Formelstruktur E-108
                 – Grenzwert für Tabelle E-220
                 – löschen E-124
                 – Syntax kopieren E-130
                 – Tabelle E-110, E-213
                 – testen E-125
                 – Vektor erstellen E-122
                 – Vektoren E-110, E-213
                 – Verlauf der Formelauswertung E-226
                 – Zeitformel testen E-125
                 – Zeitformelelement erfassen E-217
                 – Zeitformel-Objekt E-117
                 – Zeitformeltest E-221
                 – Zeitzuschläge E-111

                 W
                 Wöchentliche Termine (Kampagne)   E-191

                 Z
                 Zeitformel testen E-125
                 Zeitformelelement E-217
                 Zeitformel-Objekt E-117
                 Zeitformeltest E-125, E-221
                 – Eigenschaften Formelobjekt E-223
                 – Formelobjekt E-221
                 Zuschläge auf Vorgabezeit E-111
4.50 / 01-2023




                 E-254                                         A+W Production Kapazitätsplanung

