---
description: "DE AWProduction MZO 2.10"
---



# DE AWProduction MZO 2.10

Maschinenzuordnung       D




                         deutsch




              A+W Production
                                                                                                            Vorspann




                                      Vorspann
                                      In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                      Revisionsübersicht
                                      Maschinenzuordnung       Beschreibung
                                      Version / Datum

                                      2.10 / 11-2018           Kapitel zu Maschinentyp neu.
                                                               Screenshots aktualisiert.

                                      2.02 / 01-2017           Produkt- und Firmennamen angepasst.

                                      2.01 / 01-2013           Layout an CI 2013 angepasst.

                                      2.00 / 09-2012           Neuerstellung Tutorial, Überarbeitung Softwarereferenz

                                      1.00 / 01-2003           Ersterstellung



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
                                      ohne Vorankündigung geändert werden.
                                      Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter
                                      Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausge-
                                      schlossen werden. Die A+W Software GmbH übernimmt keine Haftung für
                                      Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem
                                      oder grobfahrlässigem Handeln.
                                      Die Beschreibungen in dieser Dokumentation beruhen auf der vollen
                                      Ausbau-stufe von A+W Production.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                               D-3
                 Vorspann




                            Urheberrechte
                            © 2018, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
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

                            Am Pfahlgraben

                            D-35415 Pohlheim

                               +49 6404 2051 0

                               +49 6404 2051 877

                            aw.zentrale@a-w.com

                            http://www.a-w.com
2.10 / 11-2018




                 D-4                                             A+W Production Maschinenzuordnung
                                                                                                                                                           Inhalt




                                      Inhalt
                                      Vorspann ................................................................................................................ D-3
                                       Revisionsübersicht .............................................................................................. D-3
                                       Editorial ............................................................................................................... D-3

                                      Tutorial                                                                                                             D-7
                                      Überblick ................................................................................................................. D-9
                                        Dokumentation .................................................................................................. D-10
                                          Aufbau des Tutorials ...................................................................................... D-10
                                          Darstellungskonventionen .............................................................................. D-11
                                      Grundlagen ........................................................................................................... D-12
                                      Maschinenzuordnung ........................................................................................... D-14
                                        Maschinen ......................................................................................................... D-15
                                          Maschinen in der Maschinenzuordnung ........................................................ D-16
                                          Maschinen anlegen und verwalten ................................................................ D-22
                                          Restriktionen von Maschinen anlegen und bearbeiten .................................. D-26
                                          Übungen zu Maschinen ................................................................................. D-32
                                        Logische Maschinen .......................................................................................... D-33
                                          Logische Maschinen in der Maschinenzuordnung ......................................... D-34
                                          Logische Maschinen anlegen und verwalten ................................................. D-36
                                          Übungen zu logischen Maschinen ................................................................. D-39
                                        Arbeitsgänge ..................................................................................................... D-40
                                          Arbeitsgänge in der Maschinenzuordnung .................................................... D-41
                                          Arbeitsgänge anlegen und verwalten ............................................................. D-48
                                          Übungen zu Arbeitsgängen ........................................................................... D-50
                                        Arbeitsgangzuordnung ...................................................................................... D-51
                                          Angepasste Arbeitsgangzuordnung ............................................................... D-52
                                          Arbeitsgänge und logische Maschinen zuordnen .......................................... D-58
                                          Übungen zur Arbeitsgangzuordnung ............................................................. D-62
                                        Bedingungen, Formeln, Restriktionen ............................................................... D-63
                                          Bedingungen und Formeln in der Maschinenzuordnung ............................... D-64
                                          Bedingung auswählen .................................................................................... D-65
                                          Formel zur Bearbeitungsdauer einer logischen Maschine auswählen ........... D-66
                                          Übungen zum Auswählen von Bedingungen ................................................. D-68
                                        Bearbeitungstypen und Bearbeitungsartikel ...................................................... D-69
                                          Bearbeitungstypen in der Maschinenzuordnung ............................................ D-70
                                          Bearbeitungsartikel in der Maschinenzuordnung ........................................... D-71
                                          Bearbeitungstypen anlegen und verwalten .................................................... D-73
                                          Bearbeitungsartikel anlegen und verwalten ................................................... D-76
                                          Übungen zur Maschinenzuordnung ............................................................... D-80
                                      Schaltflächen in der Maschinenzuordnung ........................................................... D-81

                                      Softwarereferenz                                                                                                  D-83
                                      Maschinenzuordnung ........................................................................................... D-85
                                       MZO-Editor ........................................................................................................ D-86
                                         MZO-Editor – Maschinen ............................................................................... D-87
                                         MZO-Editor – Logische Maschinen ................................................................ D-88
                                         MZO-Editor – Arbeitsgänge ........................................................................... D-90
                                         MZO-Editor – Arbeitsgangzuordnung ............................................................ D-91
                                         MZO-Editor – Maschinentypen ...................................................................... D-92
2.10 / 11-2018




                                       Neue Maschine ................................................................................................. D-94
                                       Maschine ........................................................................................................... D-95
                                       Abmessungsrestriktionen ................................................................................ D-100
                                       SZR Restriktionen ........................................................................................... D-101


                 A+W Production Maschinenzuordnung                                                                                                           D-5
                 Inhalt




                            Bedingung auswählen ..................................................................................... D-102
                            Neue logische Maschine ................................................................................. D-103
                            Logische Maschine .......................................................................................... D-104
                            Formel-Auswahl .............................................................................................. D-106
                            Neuer Arbeitsgang .......................................................................................... D-107
                            Arbeitsgang ..................................................................................................... D-108
                            Neuer Maschinentyp ....................................................................................... D-110
                            Maschinentyp .................................................................................................. D-111
                          Formeln in der Maschinenzuordnung ................................................................. D-113
                            Auswahl Bedingungen ..................................................................................... D-114
                            Bedingungseditor (grafische Variante) ............................................................ D-115
                            Neue Bedingung .............................................................................................. D-117
                            Info (zur neuen Bedingung) ............................................................................. D-117
                            Auswahl Menge ............................................................................................... D-118
                            Bedingungseditor (Text-Variante) ................................................................... D-119
                            Formel-Editor ................................................................................................... D-120
                          Bearbeitungen in der Maschinenzuordnung ....................................................... D-122
                            Bearbeitungstypen .......................................................................................... D-123
                            Bearbeitungsartikel .......................................................................................... D-125
                            Spalten anpassen ............................................................................................ D-128
                            Spaltendefinition .............................................................................................. D-129

                          Partindex                                                                                                 D-131
2.10 / 11-2018




                 D-6                                                                A+W Production Maschinenzuordnung
Maschinenzuordnung        D

                      Tutorial




              A+W Production
                 Tutorial                                                                                 Überblick




                                      Überblick
                                      Das Tutorial zum Modul Maschinenzuordnung (MZO) beschäftigt sich mit der
                                      Zuweisung von Bearbeitungen zu Maschinen in A+W Production. Die Maschi-
                                      nenzuordnung weist die anstehenden Bearbeitungen den einzelnen Maschi-
                                      nen zu und berücksichtigt dabei Maschinenrestriktionen und Vorgaben zur
                                      Produktionssteuerung. Mit Prüfprogrammen von Maschinenherstellern kann
                                      in A+W Production geprüft werden, ob die Arbeitsgänge plausibel sind.

                                         Funktionen sind von den freigeschalteten Modulen abhängig
                                         Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                         Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                         liert und freigeschaltet sind.
                                         Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                         on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                         GmbH.

                                      Vorausgesetzte Kenntnisse
                                      Das Tutorial richtet sich an Teilnehmer, die in A+W Production die Arbeitsvor-
                                      bereitung verantworten und damit den optimalen Ablauf der Produktion orga-
                                      nisieren. Die Teilnehmer müssen das Konzept der Stammdaten in A+W
                                      Production kennen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                             D-9
                 Überblick                                                                          Tutorial




                             Dokumentation
                             Für das Modul Maschinenzuordnung stehen folgende Dokumente zur Verfü-
                             gung:

                             PDF                     Vollständige Unterlagen
                                                     • Tutorial
                                                     • Softwarereferenz
                                                     • Index

                             Online-Hilfe <F1>       Kontextsensitive Dialog-Hilfe


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
2.10 / 11-2018




                 D-10                                            A+W Production Maschinenzuordnung
                 Tutorial                                                                                     Überblick




                                      Darstellungskonventionen
                                      Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                      gende Bedeutung:

                                      Kursiv                   sind Zeichenfolgen ausgezeichnet, die Elemente der
                                                               Software bezeichnen, z. B. der Dialog Neue Maschine.

                                      Fett                      sind Zeichenfolgen ausgezeichnet, die Sie über die
                                                                Tastatur eingeben, z. B.: Geben Sie den Wert 0 ein.

                                      >                         Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                                gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                                Stammdaten > MZO > MZO-Editor > Maschinen > Neu.

                                      []                        Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                z. B.: Mit [OK] speichern Sie die Daten.

                                      <>                       Spitze Klammern bezeichnen Tasten oder
                                                               Tastenkombinationen auf der Tastatur, z. B.: Mit <F1>
                                                               öffnen Sie die Online-Hilfe.


                                      Lesehinweis
                                      Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der voraus-
                                      gegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinhei-
                                      ten zu überspringen.
                                      Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die
                                      Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten De-
                                      tails zu vergegenwärtigen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                D-11
                 Grundlagen                                                                                                  Tutorial




                                              Grundlagen
                                              Die Maschinenzuordnung stellt die Bezüge zwischen Arbeitsgängen und Ma-
                                              schinen dar. Auf Basis der Maschinen und der Arbeitsgänge kann die Kapazi-
                                              tätsplanung die Aufträge optimal einlasten.
                                              Zum Einrichten der Stamdaten müssen folgende Fragen behandelt werden:
                                              •     Welche Aufgabe muss durch die Bearbeitung an einer Scheibe eines Auf-
                                                    trags erfüllt werden: Was ist zu tun.
                                              •     Welche verwendende Methode wird verwdnet: Wie wird das gemacht.
                                              •     Welches Arbeitsmittel wird verwendet: Wo wird die Bearbeitung ausge-
                                                    führt.
                                              •     Welche Rangfolge und Restriktionen müssen beachtet werden: Warum
                                                    oder Wann wird in die Maschine verwendet.



                            Restriktionen, Formeln,
                             z. B. minimale Dicke
                                      2 mm


                             Eigenschaften, z. B.                                                     Bearbeitungsartikel,
                            Erfassungsstelle 180,                                                     z. B. Floatzuschnitt
                               Kostenstelle 25



                                Maschinentyp,                        Formeln,                          Bearbeitungstyp,
                                z. B. Zuschnitt                   z. B. Ist Modell                      z. B. Zuschnitt



                                                                logische Maschine,
                                  Maschine,                                                               Arbeitsgang,
                                                                   z. B. logischer
                             z. B. Schneidtisch 8                                                      z. B. Zuschnitt für
                                                                  Schneidtisch 8
                                                                                                           Isolierglas




                                                                                     Arbeitsgangzuordnung




                                                                                     A+W Production gibt
                                                                                           den


                 Abb. D-1      Bestandteile in der Maschinenzuordnung.
2.10 / 11-2018




                                              In dieser schematischen Darstellung sehen Sie, welche Bestandteile zur Ma-
                                              schinenzuordnung gehören und wie sie miteinander verknüpft sind.



                 D-12                                                                  A+W Production Maschinenzuordnung
                 Tutorial                                                                                Grundlagen




                                      Maschinen werden durch einen Maschinentyp, Eigenschaften und Restriktio-
                                      nen definiert. Zum Beispiel ist dem Schneidtisch 8 der Maschinentyp Zuschnitt
                                      zugewiesen.
                                      Zu den Eigenschaften von Schneidtisch 8 gehört, dass er der Kostenstelle 25
                                      und der Erfassungsstelle 180 zugewiesen ist. Die logische Maschine zu
                                      Schneidtisch 8 heißt logischer Schneidtisch 8. Ihr ist die Formel Ist Modell zu-
                                      gewiesen.

                                      Beschreibung der Arbeitsgänge
                                      Mithilfe der Arbeitsgänge werden die Materialströme in der Produktion aufge-
                                      teilt und lassen sich separat behandeln. Arbeitsgänge müssen daher zualler-
                                      erst betrachtet werden.
                                      Bei der Einrichtung der Arbeitsgänge werden um folgende Fragen berücksich-
                                      tigt:
                                      •   Welche Bearbeitung können zusammengefasst werden und welche dürfen
                                          nicht zusammengefasst werden?
                                      •   Gibt es zusätzliche Bearbeitungen die ausgeführt werden, aber nicht in der
                                          Stückliste erscheinen?
                                      •   Gibt es ggf. verschiedene Materialströme, z. B. Serienscheiben, Badspie-
                                          gel, Wohnmobilscheiben, die ganz eigene Wege durch die Produktion ge-
                                          hen und daher früh unterschieden werden sollen?
                                      •   Gibt es ggf. Arbeitsgänge, die gar nicht hier gefertigt werden, z. B. Sand-
                                          strahlen am anderen Ende der Stadt?

                                      Beschreibung der Maschinen
                                      In dem die Maschinen präzise beschrieben werden, wird gewährleistet, dass
                                      zu fertigende Scheiben gültige Maschinen finden. Dabei wird zwischen physi-
                                      kalischen Restriktionen und logischen Maschinen mit zusätzlichen Restriktio-
                                      nen, Kostensätzen und Übergangszeiten unterschieden.
                                      Zur Liste der Maschinen kommen Orte, die zwar keine Maschinen im her-
                                      kömmlichen Sinne sind, die aber für die Produktion relevant sind, z. B. Lager,
                                      Wareneingang, Versandlager, Verladerampe, zusätzliche Produktionsorte.

                                      Beschreibung der logischen Maschine
                                      Logische Maschinen werden verwendet, um in der Kapazitätsplanung unter-
                                      schiedliche Übergangszeiten, Kostensätze oder Bearbeitungsdauern auszu-
                                      drücken. Als Leitfaden bietet sich an, eigene logische Maschinen einzurichten,
                                      wenn eine Maschine in verschiedenen Betriebsarten verwendet werden kann.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                              D-13
                 Maschinenzuordnung                                                                     Tutorial




                                      Maschinenzuordnung
                                      In diesem Kapitel erfahren Sie, welche Bereiche von A+W Production zur Ma-
                                      schinenzuordnung (MZO) gehören und wie Sie Maschinen zuordnen.
                                      Mithilfe des MZO-Editors verwalten Sie Maschinen, logische Maschinen und
                                      Arbeitsgänge, deren Zuordnung und Eigenschaften.
                                      Zur Maschinenzuordnung gehören folgende Kapitel:
                                      •   “Maschinen” auf Seite D-15
                                      •   “Logische Maschinen” auf Seite D-33
                                      •   “Arbeitsgänge” auf Seite D-40
                                      •   “Arbeitsgangzuordnung” auf Seite D-51
                                      •   “Bedingungen, Formeln, Restriktionen” auf Seite D-63
                                      •   “Bearbeitungstypen und Bearbeitungsartikel” auf Seite D-69
                                      In den folgenden Lerneinheiten lernen Sie zunächst Maschinen, logische Ma-
                                      schinen, Arbeitsgänge und die Arbeitsgangzuordnung kennen. Diese Kennt-
                                      nisse werden anschließend durch die Themen Bearbeitungstypen und
                                      Formelauswahl vertieft.
2.10 / 11-2018




                 D-14                                                     A+W Production Maschinenzuordnung
                 Tutorial                                                                       Maschinenzuordnung




                                      Maschinen
                                      Lernziele

                                      • Was sind Maschinen in A+W Production und speziell in der Maschinenzuordnung.
                                      • Wie werden Maschinen verwaltet, neu angelegt, bearbeitet oder gelöscht.
                                      • Wie werden Namen und Nummern sinnvoll vergeben.


                                      Nutzen

                                      • Mit Maschinen wird der physikalische Maschinenpark abgebildet. Somit bilden
                                        Maschinen die Basis, um die Produktion zu steuern.


                                      Merke

                                      Maschinen                  Maschinen bilden die physikalischen Maschinen im
                                                                 Maschinenpark ab.
                                                                 Namen und Nummern werden in A+W Production
                                                                 systematisch vergeben.

                                      Maschinentypen             Die Maschinentypen sind in A+W Production bereits
                                                                 definiert und werden Maschinen zugewiesen. Mit
                                                                 Maschinentypen wird definiert, um welchen Typ einer
                                                                 Maschine es sich handelt, zum Beispiel Zuschnitt,
                                                                 Rahmenbieger oder Sonstige.

                                      Verknüpfungen              UND-/ODER-Verknüpfungen sind die Operatoren, mit
                                                                 denen in A+W Production Restriktionen, Bedingungen
                                                                 und Formeln verknüpft werden.

                                      Schnitte                   Z- und W-Schnitte sind aufwendigere Schnitte, denen
                                                                 ein zusätzlicher Kostenfaktor Kosten pro Z-Schnitt
                                                                 zugewiesen werden kann.

                                         Voraussetzung
                                         Um eine Maschine in A+W Production anlegen zu können, muss der pas-
                                         sende Maschinentyp definiert sein. Der Maschinentyp wird im Dialog Neue
                                         Maschine ausgewählt.
                                         Ist im Dialog Neue Maschine der entsprechende Maschinentyp nicht ver-
                                         fügbar, wenden Sie sich bitte an die A+W Software GmbH.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                               D-15
                 Maschinenzuordnung                                                                       Tutorial




                                      Maschinen in der Maschinenzuordnung
                                      In dieser Einheit lernen Sie, wie Sie Ihren Maschinenpark in A+W Production
                                      abbilden und welche Eigenschaften den Maschinen zugeordnet werden.




                                      Abb. D-2    MZO-Editor – Maschinen


                                      Im Register Maschinen sind alle physikalischen Maschinen gelistet. Das Re-
                                      gister Maschinen bildet somit Ihren realen Maschinenpark ab.
                                      Jede Maschineist durch eine ID eindeutig identifizierbar. Zu jeder Maschine
                                      heört eine Erfassungsstelle für die Erfassung der Betriebsdaten (BDE). Sie
                                      ordnen jeder Maschine einen Maschinentyp zu, der festlegt, um welchen tech-
                                      nischen Typ es sich handelt, zum Beispiel Zuschnitt, CNC-Center oder Spros-
                                      senbau. Die Maschinentypen sind fest definiert und können nicht geändert
                                      werden. A+W Production legt zu jeder Maschine automatisch eine logische
                                      Maschine an.
                                      Sie müssen also zu jeder real existierenden Maschine im Maschinenpark eine
                                      Maschine in A+W Production anlegen und die Eigenschaften definieren.
2.10 / 11-2018




                 D-16                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                   Maschinenzuordnung




                                                 Maschinenpark                      Abbildung in
                                                                                   A+W Production

                                                  Schneidtisch 1,
                                                  Maschinentyp                      Schneidtisch 1
                                                    Zuschnitt


                                                  Schneidtisch 2,
                                                  Maschinentyp                       Schneidtisch 2
                                                    Zuschnitt


                                                 CNC-Maschine 1,
                                                  Maschinentyp                     CNC-Maschine 1
                                                   CNC-Center


                                                 CNC-Maschine 2,
                                                  Maschinentyp                     CNC-Maschine 2
                                                   CNC-Center


                                                 Bohrmaschine 1,
                                                  Maschinentyp                      Bohrmaschine 1
                                                   Bohrungen


                                                 Bohrmaschine 2



                                      Abb. D-3      Maschinen in A+W Production


                                      In diesem Beispiel ist zur Bohrmaschine 2 keine Maschine in A+W Production
                                      angelegt. Damit ist die Maschine der Software nicht bekannt und kann auch
                                      nicht angesteuert werden.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-17
                 Maschinenzuordnung                                                                          Tutorial




                                      Maschineneigenschaften
                                      Für jede in A+W Production angelegte Maschine müssen die folgenden Ei-
                                      genschaften der Maschine festgelegt werden.
                                      •   Handbetrieb:
                                          Kennzeichen für Maschinen, die nicht über automatische Ladeeinrichtun-
                                          gen verfügen. Dieses Kennzeichnen verhindert u.a. dass anhand der ma-
                                          nuellen Bearbeitungsdauer gesplittet wird oder dass Positionen
                                          automatisch auf Handzuschnittstische eingelastet werden.
                                      •   Einzelbearbeitung:
                                          Kennzeichen für Maschinen, deren Bearbeitungen nicht zusammengefasst
                                          werden dürfen, z. B.
                                          – Bohrungen = 0: für zwei Bohrungen auf derselben Maschine werden
                                              nicht zwei Termine ermittelt.
                                          – Siebdrucke oder Beschichtungen = 1: für zwei Beschichtungen werden
                                              nicht zwei verschiedene Termine ermittelt, auch wenn sie auf derselben
                                              Maschinen gemacht werden.
                                      •   Mindestgröße:
                                          Mindestabmessungen für eine Scheibe, die auf der Maschine gefertigt wer-
                                          den kann, ohne z. B. durch die Rollen zu fallen.
                                          Wenn Sie zu kleine Scheiben auf eine größere Scheibe legen können, z. B.
                                          um sie zu bedrucken, legen Sie die Größenrestriktion nicht an der Maschi-
                                          ne fest, sondern an den logischen Maschinen, z. B. als Siebdruck mit Trä-
                                          gerscheibe.
                                      •   Maximalgröße:
                                          Maximale Abmessungen für eine Scheibe, die der Maschine gefertigt wer-
                                          den kann, weil sie die Breite der Führungsschienen, die Ofenbreite oder
                                          die Deckenhöhe überschreitet.
                                          Wenn Sie größere Scheiben fertigen können, indem Sie z. B. am Bearbei-
                                          tungszentrum die Seitenwände abschrauben und Spritzschutz aufstellen,
                                          legen Sie die Größenrestriktion nicht an der Maschine fest, sondern an den
                                          logischen Maschinen, z.B: als Bearbeitungszentrum für Übergrößen.
                                      •   Dicken:
                                          Dickenbereich, in dem die Maschine arbeiten kann. Anderen Dicken kön-
                                          nen nicht auf der Maschine bearbeitet werdn, z. B. weil 3 mm nicht zuver-
                                          lässig unterstützt werden und für 15 mm die Führungen zu schmal sind.
                                          Wenn eine 15 mm Scheibe gefertigt werden kann, indem Sie die Maschine
                                          umbauen, legen Sie die Größenrestriktion nicht an der Maschine fest, son-
                                          dern an den logischen Maschinen, z. B. Schleifmaschine für Dickgläser.
                                      •   Modelle:
                                          Angabe, ob die Maschine ausschließlich Rechtecke, ausschließlich Model-
                                          le oder beides fertigen kann. Berücksichtigen Sie ggf. dass Freiformen
                                          oder Rundbögen nicht gefertigt werden können, z. B. bei VSG-Zuschnitt.
                                      •   Gewicht:
                                          Maximalgewicht einer Scheibe, für das die Maschine zugelassen ist. Um
                                          auszudrücken, dass die Maschine das Gewicht zwar verarbeiten kann,
                                          hierfür aber ein zweiter Mitarbeiter zum Handling bereitstehen muss, ge-
                                          ben Sie die Restriktion bei den logischen Maschinen an, z .B. Einseiter mit
2.10 / 11-2018




                                          zwei Personen.




                 D-18                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                         Maschinenzuordnung




                                          Maschine löschen
                                          Das Löschen einer Maschine kann Auswirkungen auf die Produktion ha-
                                          ben. Vergewissern Sie sich, dass die Maschine in der Produktion nicht
                                          mehr verwendet wird, bevor Sie sie löschen.

                                      Namen, IDs und Nummern vergeben
                                      Vergeben Sie für Maschinen des gleichen Typs IDs im gleichen Hunderter-Be-
                                      reich, zum Beispiel für alle Schneidtische IDs zwischen 100 und 199. Damit
                                      sind in der Liste Schneidtische sofort erkennbar. Wenn Sie keine eigenen
                                      Nummernkreise für Betriebsmittel haben, orientieren Sie sich am Nummerie-
                                      rungsschema der Betriebsdatenerfassung.
                                      Vergeben Sie für Maschinen des gleichen Typs gleiche Namen und numme-
                                      rieren Sie diese durch, z. B. bekommt der achte Schneidtisch im Maschinen-
                                      park den Namen Schneidtisch 8.

                                      Maschinenrestriktionen
                                      Maschinen können bauartbedingt verschiedene Restriktionen haben, z. B.
                                      können sie nur Scheiben bis zu einer bestimmten Größe bearbeiten. Die Re-
                                      striktionen der einzelnen Maschinen können Sie im Dialog Maschine ange-
                                      ben.
                                      Die verfügbaren Restriktionen im Dialog Maschine sind:
                                      •   Minimale Dicke
                                      •   Maximale Dicke
                                      •   Modelle
                                      •   Beschichtete Gläser
                                      •   Strukturgläser
                                      •   Stufen ISO
                                      •   Abmessungen
                                      •   SZR
                                      Haben Sie eine Maschine, die weitere Restriktionen aufweist, müssen die Re-
                                      striktionen mit zusätzlichen Bedingungen formuliert werden. Diese Bedingun-
                                      gen können auch Formeln enthalten.
                                       “Bedingungen und Formeln in der Maschinenzuordnung” auf Seite D-64
                                      Im Folgenden sind Beispiele zu den verfügbaren Restriktionen im Dialog Ma-
                                      schine aufgelistet.

                                          Beispiel: Restriktionen Dicke

                                          Sie können die Restriktion Dicke folgendermaßen einstellen:
                                          • Wenn die Maschine nur Scheiben ab einer Dicke von 8 mm bearbeiten
                                            kann, geben Sie die Restriktion minimale Dicke 8 mm ein.
                                          • Wenn die Maschine nur Scheiben bis zu einer Dicke von 15 mm
                                            bearbeiten kann, geben Sie die Restriktion maximale Dicke 15 mm ein.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                 D-19
                 Maschinenzuordnung                                                                               Tutorial




                                         Beispiel: Restriktion Modelle

                                         Sie können die Restriktion Modelle folgendermaßen einstellen:
                                         • Keine Restriktion: die Maschine kann Modelle und Rechtecke bearbeiten,
                                           z. B. bei einem modernen Zuschnitttisch.
                                         • Die Maschine kann nur Modelle bearbeiten, z. B. um zu verhindern, dass
                                           rechteckige Scheiben zum Schleifen auf ein CNC-Center gelangen.
                                         • Die Maschine kann keine Modelle, also nur Rechtecke, bearbeiten, z. B.
                                           bei einer Schleif-Bohrstraße.


                                         Beispiel: Restriktion Beschichtete Gläser

                                         Sie können die Restriktion Beschichtete Gläser folgendermaßen einstellen:
                                         • Keine Restriktion: die Maschine kann beschichtete und unbeschichtete
                                           Gläser bearbeiten.
                                         • Die Maschine kann nur beschichtete Gläser bearbeiten.
                                         • Die Maschine kann nur unbeschichtete Gläser bearbeiten.


                                         Beispiel: Restriktion Strukturgläser

                                         Sie können die Restriktion Strukturgläser folgendermaßen einstellen:
                                         • Keine Restriktion: die Maschine kann Strukturgläser und Gläser ohne
                                           Struktur bearbeiten.
                                         • Die Maschine kann nur Strukturgläser bearbeiten.
                                         • Die Maschine kann nur Gläser ohne Struktur bearbeiten.


                                         Beispiel: Restriktion Stufen-ISO

                                         Sie können die Restriktion Stufen-ISO folgendermaßen einstellen:
                                         • Keine Restriktion: die Maschine kann Stufen-ISO und Normal-ISO
                                           fertigen.
                                         • Die Maschine kann nur Stufen-ISO bearbeiten.
                                         • Die Maschine kann nur Normal-ISO bearbeiten.


                                      Abmessungsrestriktionen und Scheibenformat
                                      Sie können bei einer Maschine minimale und maximale Größen der zu bear-
                                      beitenden Scheiben definieren. Orientieren Sie sich bei der Angabe der Werte
                                      an der Laufrichtung der Maschine. Die Werte Breite und Höhe dienen lediglich
                                      der Anschauung, Sie können auch Scheiben verarbeiten, deren Breite und
                                      Höhe vertauscht sind. Die Scheibe muss dann u. U. per Hand an der Maschi-
                                      ne gedreht werden.

                                      SZR-Restriktionen
                                      Hier legen Sie fest, ob die Maschine einfaches ISO mit einem SZR oder mehr-
                                      faches ISO mit zwei SZRs fertigen kann. Für jeden SZR kann ein Mindest- und
                                      ein Maximalwert eingegeben werden.
2.10 / 11-2018




                 D-20                                                         A+W Production Maschinenzuordnung
                 Tutorial                                                                   Maschinenzuordnung




                                      UND-/ODER-Verknüpfungen
                                      Wenn Sie die Restriktionen einer Maschine angeben, dann müssen Sie diese
                                      als logische Verknüpfungen (UND/ODER, AND/OR) angeben. Diese sind
                                      Grundverknüpfungen der booleschen Algebra, mit der sich logische Zusam-
                                      menhänge zeigen lassen.
                                      •   UND-Verknüpfung: Wenn zwei (oder mehr) Aussagen zutreffen, ist eine
                                          Aussage wahr.
                                          Beispiel: Auf einer Maschine können nur Scheiben bearbeitet werden, die
                                          breiter als 150 mm und höher als 200 mm sind. Daraus ergibt sich:
                                          Breite >= 150 mm UND Höhe >= 200 mm.
                                      •   ODER-Verknüpfung: Wenn die eine oder die andere Aussage zutrifft, ist
                                          eine Aussage wahr.
                                          Beispiel: Auf einer Maschine können nur Scheiben bearbeitet werden, die
                                          breiter als 150 mm oder kürzer als 3500 mm sind. Daraus ergibt sich:
                                          Breite >= 150 mm ODER Länge <= 3500 mm.

                                      Komponenten-ID
                                      Die Komponenten-ID wird nur bei den Maschinentypen Linie, Zuschnitt und
                                      Bieger verwendet. Mit der Komponenten-ID kann zwischen Linien, Tischen
                                      oder Biegern unterschieden werden, wenn es mehrere des gleichen Typs gibt.
                                      So könnten zum Beispiel die Tische 1, 2 und 3 die Komponenten-IDs TB1,
                                      TB2 und TB3 bekommen.
                                      Die Komponenten-ID steuert, in welchem Format die NC-Codeausgabe er-
                                      folgt.

                                      Zusätzliche Bedingungen
                                      Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaften
                                      von Maschinen unter Umständen massiv.
                                      Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche Aus-
                                      wirkungen diese hat.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-21
                 Maschinenzuordnung                                                                        Tutorial




                                      Maschinen anlegen und verwalten
                                      In dieser Lerneinheit lernen Sie, wie Sie neue Maschinen anlegen, bearbeiten
                                      oder löschen.
                                      Wenn Sie eine Maschine anlegen, müssen Sie anschließend die Maschinen-
                                      daten bearbeiten.
                                      Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                      •   “So legen Sie eine Maschine an” auf Seite D-22
                                      •   “So geben Sie die Eigenschaften einer Maschine ein” auf Seite D-23
                                      •   “So löschen Sie eine Maschine” auf Seite D-25

                                          Voraussetzung
                                          Um eine neue Maschine anzulegen, muss ein passender Maschinentyp
                                          angelegt sein, z. B. Zuschnitt, CNC-Center, Rahmenbieger, Sonstiges.
                                          Der Katalog der Maschinentypen ist in A+W Production fest vorgegeben.
                                          Er steht in der Kombobox zur Verfügung, wenn Sie eine neue Maschine an-
                                          legen.


                                       So legen Sie eine Maschine an
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen > [Neu].




                                      2 Geben Sie eine ID aus dem Nummernbereich ein, den Sie für diesen Ma-
                                        schinentyp vorgesehen haben, zum Beispiel 180.
                                      3 Geben Sie einen Namen ein, der die Maschine eindeutig beschreibt, zum
                                        Beispiel Schneidtisch 8.
                                      4 Wählen Sie den zugehörigen Maschinentyp, zum Beispiel Zuschnitt.
                                      5 Geben Sie eine Komponenten-ID ein, zum Beispiel TB8.
                                          Sie müssen bei den Maschinentypen Linien, Tische oder Bieger eine Kom-
                                          ponenten-ID eingeben. Damit können Sie zwischen den Maschinen unter-
                                          scheiden, wenn es mehrere davon gibt.
2.10 / 11-2018




                 D-22                                                     A+W Production Maschinenzuordnung
                 Tutorial                                                                  Maschinenzuordnung




                                         Abb. D-4    Beispiel für eine neue Maschine


                                      6 Klicken Sie auf [OK], um die Daten zu speichern.
                                         Damit haben Sie eine neue Maschine angelegt. Sie wird in der Liste der
                                         Maschinen im Dialog MZO-Editor aufgeführt.
                                         Um die Maschine vollständig zu beschreiben, müssen Sie die Eigenschaf-
                                         ten und Zuordnungen festlegen.


                                       So geben Sie die Eigenschaften einer Maschine ein
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen.
2.10 / 11-2018




                                         Abb. D-5    MZO-Editor – Maschinen




                 A+W Production Maschinenzuordnung                                                         D-23
                 Maschinenzuordnung                                                                              Tutorial




                                      2 Markieren Sie die Maschine, die Sie bearbeiten wollen.
                                      3 Klicken Sie auf [Bearbeiten].




                                         A

                                                                                          B




                                         A Allgemeine Eigenschaften            B Kombobox
                                         Abb. D-6     Maschine


                                      4 Ergänzen Sie die Allgemeinen Eigenschaften (A).
                                         Wenn Sie in ein Feld klicken, können Sie die Daten aus der Kombobox (B)
                                         wählen.
                                         Die Restriktionen unteren Teil des Dialogs können Sie später bestimmen.
                                      5 Bestätigen Sie mit [OK].
                                         Damit haben Sie die Stammdaten der Maschine angegeben.
                                         Die Maschinen-Restriktionen lernen Sie in einer separaten Einheit kennen.
                                          “Restriktionen von Maschinen anlegen und bearbeiten” auf Seite D-26
2.10 / 11-2018




                 D-24                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                  Maschinenzuordnung




                                       So löschen Sie eine Maschine

                                         Maschinen löschen
                                         Das Löschen von Maschinen in A+W Production kann Auswirkungen auf
                                         die Produktion haben. Vergewissern Sie sich, dass die Maschinen nicht
                                         verwendet werden, bevor Sie sie löschen.

                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen.
                                      2 Markieren Sie die Maschine, die Sie löschen möchten.
                                      3 Klicken Sie auf [Löschen].
                                         Eine Sicherheitsabfrage wird angezeigt.
                                      4 Bestätigen Sie die Sicherheitsabfrage mit [Yes], wenn Sie die Maschine
                                        endgültig löschen möchten.
                                         Die Maschinendaten werden gelöscht.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                        D-25
                 Maschinenzuordnung                                                                         Tutorial




                                      Restriktionen von Maschinen anlegen und bearbei-
                                      ten
                                      In dieser Lerneinheit lernen Sie, die Restriktionen einer Maschine festlegen.
                                      Dazu gibt es folgende Handlungsanleitungen:
                                      •   “So bearbeiten Sie die Restriktionen zur Dicke” auf Seite D-26
                                      •   “So bearbeiten Sie die Restriktionen für Modelle, beschichtete Gläser,
                                          Strukturgläser und Stufen-ISO” auf Seite D-28
                                      •   “So bearbeiten Sie Restriktionen für Abmessungen und SZR” auf
                                          Seite D-30
                                      •   “So entfernen Sie die Restriktionen Abmessungen und SZR” auf
                                          Seite D-31

                                          Restriktionen und Zusätzliche Bedingung gleichzeitig
                                          Wenn Restriktionen aktiviert sind und gleichzeitig eine Formel ausgewählt
                                          ist, kann dies zu einem Konflikt führen.
                                          Restriktionen können sich gegenseitig aufheben.

                                          Für Rückfragen wenden Sie sich bitte an den Support der A+W Software
                                          GmbH.


                                       So bearbeiten Sie die Restriktionen zur Dicke
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen.
2.10 / 11-2018




                                          Abb. D-7    MZO-Editor – Maschinen



                 D-26                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                      Maschinenzuordnung




                                      2 Markieren Sie die Maschine, die Sie bearbeiten wollen.
                                      3 Klicken Sie auf [Bearbeiten].




                                         A                                                B




                                         A Aktivieren der Restriktion           B Eingabefeld öffnen.
                                         Abb. D-8     Restriktion – Dicke bearbeiten


                                      4 Klicken Sie doppelt auf […] (B).




                                      5 Klicken Sie auf den [Pfeil], um den Wert für die minimale Dicke einzugeben.
2.10 / 11-2018




                                      6 Geben Sie den Wert der minimalen Dicke in Millimetern ein.


                 A+W Production Maschinenzuordnung                                                           D-27
                 Maschinenzuordnung                                                                            Tutorial




                                      7 Klicken Sie auf [OK], um den Wert zu speichern.
                                         Damit haben Sie den Wert der minimalen Dicke der Maschine geändert.
                                      8 Wiederholen Sie die Schritte 4 bis 7, um die Restriktionen für die maximale
                                        Dicke zu bearbeiten.


                                       So bearbeiten Sie die Restriktionen für Modelle, beschichtete Gläser,
                                        Strukturgläser und Stufen-ISO
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen.
                                      2 Markieren Sie die Maschine, die Sie bearbeiten wollen.
                                      3 Klicken Sie auf [Bearbeiten].




                                         A                                                 B




                                         A Aktivieren der Restriktion Modelle     B Weitere Checkbox öffnen.
                                         Abb. D-9     Restriktion – Modelle bearbeiten


                                      4 Klicken Sie doppelt auf […] hinter Modelle.
                                         Ein [Pfeil] wird angezeigt.
2.10 / 11-2018




                 D-28                                                           A+W Production Maschinenzuordnung
                 Tutorial                                                                      Maschinenzuordnung




                                      5 Klicken Sie auf den [Pfeil] (B), um Modelle zu aktivieren.



                                         A                                          B

                                                     C
                                                                                               D


                                                                  E
                                                                                                           F


                                         A und B         Keine Restriktion. Die Maschine kann Rechtecke und Modelle
                                                         bearbeiten.
                                         C und D         Die Maschine kann nur Rechtecke bearbeiten.
                                         E und F         Die Maschine kann nur Modelle bearbeiten.
                                         Abb. D-10    Restriktion Modelle – Kombinationen der Checkboxen


                                      6 Wählen Sie die gewünschte Kombination der Checkboxen, um die Restrik-
                                        tion festzulegen:
                                         •   Keine Einschränkung (A, B)
                                         •   Keine Modelle (C, D)
                                         •   Keine Rechtecke (E, F)
                                      7 Klicken Sie auf [OK], um die Restriktion für Modelle zu speichern.
                                         Damit haben Sie die Restriktion Modelle für die Maschine bearbeitet.
                                      8 Bearbeiten Sie auf die gleiche Weise die Restriktionen für beschichtete
                                        Gläser, Strukturgläser und Stufen-ISO.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                              D-29
                 Maschinenzuordnung                                                                      Tutorial




                                       So bearbeiten Sie Restriktionen für Abmessungen und SZR

                                          Restriktionen werden unwiderruflich gelöscht
                                          Abmessungsrestriktionen unwiderruflich und ohne Sicherheitsabfrage ge-
                                          löscht, wenn Sie auf das [Kreuz] klicken.

                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen.
                                      2 Markieren Sie die Maschine, die Sie bearbeiten wollen.
                                      3 Klicken Sie auf [Bearbeiten].

                                      s




                                                                                    A




                                          A Bearbeiten
                                          Abb. D-11   Restriktion – Abmessungen bearbeiten
2.10 / 11-2018




                 D-30                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                  Maschinenzuordnung




                                      4 Klicken Sie im Feld Abmessungen auf das [Stift-Symbol], um den Dialog
                                        Abmessungsrestriktionen zu öffnen.




                                      5 Aktivieren Sie die Checkboxen der Eingabefelder, die Sie bearbeiten
                                        möchten.
                                      6 Geben Sie die Werte in die Eingabefelder ein.
                                      7 Klicken Sie auf [OK], um die Änderungen der Abmessungsrestriktionen zu
                                        speichern.
                                         Damit haben Sie die Restriktion Abmessungen für die Maschine geändert.
                                         Die Restriktion wird im Feld Abmessungen als UND-/ODER-Verknüpfun-
                                         gen angezeigt.




                                      8 Bearbeiten Sie auf die gleiche Weise die Restriktionen für den SZR.


                                       So entfernen Sie die Restriktionen Abmessungen und SZR

                                         Abmessungsrestriktionen löschen
                                         Abmessungsrestriktionen unwiderruflich und ohne Sicherheitsabfrage ge-
                                         löscht, wenn Sie auf das [Kreuz] klicken.

                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Maschinen.
                                      2 Markieren Sie die Maschine, die Sie bearbeiten wollen.
                                      3 Klicken Sie auf [Bearbeiten].
                                         Der Dialog Maschine wird geöffnet.
                                      4 Klicken Sie im Bereich Abmessungen, auf [X], um Restriktion zu entfernen.
                                         Damit haben Sie die Restriktionen Abmessungen für die Maschine ge-
                                         löscht.
                                      5 Klicken Sie auf [OK], um die Änderungen zu speichern.
                                      6 Entfernen Sie auf die gleiche Weise die SZR-Restriktionen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                            D-31
                 Maschinenzuordnung                                                                       Tutorial




                                      Übungen zu Maschinen
                                      Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
                                      •   Bilden Sie auf Papier den Maschinenpark Ihres Betriebes ab.
                                      •   Notieren Sie, welche Maschine in welchen Maschinentyp fällt.
                                      •   Vergeben Sie für die Maschinen systematisch IDs (Nummernkreise).
                                      •   Notieren Sie, welche Eigenschaften für die Maschinen gelten und ob es
                                          Restriktionen gibt:
                                          – Gibt es Restriktionen, wie zum Beispiel minimale Dicke, maximale Di-
                                              cke oder Abmessungsrestriktionen.
                                          – Kann die Maschine ISO oder 3-fach-ISO bearbeiten? Wo müssen Sie
                                              diese Eingaben vornehmen?
                                      •   Legen Sie Maschinen als Übungsmaschinen in A+W Production an und
                                          passen Sie diese so an, dass sie Ihrem Maschinenpark entsprechen.
                                      •   Lassen Sie die testweise erstellten Maschinen bestehen, da spätere Übun-
                                          gen darauf aufbauen.


                                      Ergänzende Informationen
                                       Softwarereferenz, “Neue Maschine” auf Seite D-94
                                       Softwarereferenz, “Maschine” auf Seite D-95
                                       Softwarereferenz, “Abmessungsrestriktionen” auf Seite D-100
                                       Softwarereferenz, “SZR Restriktionen” auf Seite D-101
2.10 / 11-2018




                 D-32                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                       Maschinenzuordnung




                                      Logische Maschinen
                                      Lernziele

                                      • Was sind logische Maschinen in A+W Production und speziell in der
                                        Maschinenzuordnung?
                                      • Warum gibt es logische Maschinen?
                                      • Wie werden Namen und Nummern vergeben?
                                      • Wie werden logische Maschinen neu angelegt, bearbeitet oder gelöscht?
                                      • Wann können logische Maschinen gelöscht werden und wann nicht?


                                      Nutzen

                                      • Logische Maschinen bilden eine Funktion einer Maschine ab. Kann eine Maschine
                                        Bohren und Kanten bearbeiten, werden dafür in A+W Production zwei logische
                                        Maschinen angelegt. Und damit kann im nächsten Schritt ein Arbeitsgang der
                                        Funktion einer Maschine zugeordnet werden.
                                      • Die A+W Production BDE (Betriebsdatenerfassung) wertet unter anderem Daten
                                        der logischen Maschinen aus, z. B. für Statistiken.


                                      Merke

                                      Logische Maschinen        Logische Maschinen bilden jeweils eine Funktion einer
                                                                physikalischen Maschine ab.
                                                                Logische Maschinen werden zur Ablaufsteuerung in der
                                                                Produktion und zur Kostenberechnung verwendet.
                                                                Logische Maschinen werden zur
                                                                Betriebsdatenerfassung verwendet.
                                                                Sobald Sie eine Maschine anlegen, wird automatisch
                                                                eine logische Maschine angelegt.
                                                                Zu einer Maschine können beliebig viele logische
                                                                Maschinen definiert werden.

                                      Zuordnung                 Logische Maschinen werden Arbeitsgängen
                                                                zugewiesen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                 D-33
                 Maschinenzuordnung                                                                      Tutorial




                                      Logische Maschinen in der Maschinenzuordnung
                                      Logische Maschinen bilden jeweils eine Funktion einer realen Maschine ab.
                                      Dabei werden die Eigenschaften der Maschine an die logische Maschine ver-
                                      erbt. Zusätzlich zu den Eigenschaften der Maschine gelten die Eigenschaften
                                      der logischen Maschine.




                                      Abb. D-12    Logische Maschinen


                                      Logische Maschinen werden benötigt für:
                                      •   Beschreibung einzelner Maschinenfunktionen.
                                      •   Zuordnung von Arbeitsgängen.
                                      •   Priorisierung von Arbeitsgängen.
                                      •   Auslastungsplanung und Umlastung.
                                      •   Logische Maschinen trennen einzelne Funktionen von Maschinen. Damit
                                          werden für eine Maschine z. B. unterschiedliche Kostensätze oder Über-
                                          gangszeiten möglich.
                                      •   Statistische Auswertungen.
2.10 / 11-2018




                 D-34                                                     A+W Production Maschinenzuordnung
                 Tutorial                                                                        Maschinenzuordnung




                                         Beispiel

                                         Sie haben eine CNC-Maschine, die bohren, schleifen und polieren kann. Sie
                                         definieren die Maschine als CNC-Maschine 1. Dazu erstellt A+W Production
                                         automatisch eine logische Maschine. Da die CNC-Maschine drei Funktionen
                                         besitzt, werden drei logische Maschinen definiert.
                                         Diese definieren Sie so, dass die Stammdaten zu Bohren angelegt sind. Nun
                                         definieren Sie zur CNC-Maschine 1 zwei weitere logische Maschinen: eine
                                         mit den Stammdaten zum Schleifen und die andere mit den Stammdaten zum
                                         Polieren.



                                                                                      Logische CNC-Maschine 1
                                                                                      • automatisch erstellt
                                                                                      • manuell konfiguriert
                                                                                      • Bohren

                                          Reale CNC-Maschine
                                          Funktionen:                                 Logische CNC-Maschine 2

                                          • Bohren                                    • manuell erstellt
                                          • Schleifen                                 • manuell konfiguriert
                                          • Polieren                                  • Schleifen


                                                                                      Logische CNC-Maschine 3
                                                                                      • manuell erstellt
                                                                                      • manuell konfiguriert
                                                                                      • Polieren


                                      Abb. D-13     Beispiel: Drei logische Maschinen resultieren aus einem CNC-Center


                                      Die Bearbeitungszeiten, die eine logische Maschine für den ihr zugewiesenen
                                      Arbeitsgang benötigt, wird als Formel in der Kapazitätsplanung definiert. Dazu
                                      steht die separate Dokumentation für den Part Kapazitätsplanung zur Verfü-
                                      gung.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                D-35
                 Maschinenzuordnung                                                                       Tutorial




                                      Logische Maschinen anlegen und verwalten
                                      In diesem Teil des Tutorials lernen Sie, wie Sie logische Maschinen anlegen
                                      und bestehende bearbeiten oder löschen.
                                      Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                      •   “So legen Sie eine logische Maschine an” auf Seite D-36
                                      •   “So bearbeiten Sie eine logische Maschine” auf Seite D-38
                                      •   “So löschen Sie eine logische Maschine” auf Seite D-39

                                          Voraussetzung
                                          Sie können logische Maschinen erst dann anlegen, wenn die zugehörige
                                          Maschine angelegt ist.


                                       So legen Sie eine logische Maschine an
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Logische Maschinen.




                                          Abb. D-14   Logische Maschine markiert


                                          A+W Production erstellt automatisch zu jeder Maschine eine logische Ma-
                                          schine. Alle weiteren logischen Maschinen können nur auf Basis der be-
                                          reits bestehenden erstellt werden.
2.10 / 11-2018




                                      2 Markieren Sie die logische Maschine, welche die Basis für die neue logi-
                                        sche Maschine sein soll.




                 D-36                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                  Maschinenzuordnung




                                      3 Klicken Sie auf [Neu].




                                      4 Geben Sie die ID und den Namen ein.
                                      5 Klicken Sie auf [OK], um die Daten zu speichern.




                                         Abb. D-15   Neue logische Maschine


                                         Damit haben Sie eine neue logische Maschine angelegt. Die neue logische
                                         Maschine wird im Register Logische Maschinen im MZO-Editor gelistet.
                                         Sie können jetzt die Eigenschaften der neuen logischen Maschine bearbei-
                                         ten.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-37
                 Maschinenzuordnung                                                                        Tutorial




                                       So bearbeiten Sie eine logische Maschine
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Logische Maschinen.
                                         Das Register Logische Maschinen wird angezeigt.
                                      2 Markieren Sie die logische Maschine, die Sie bearbeiten wollen.
                                      3 Klicken Sie auf [Bearbeiten].




                                         Abb. D-16    Logische Maschine – Eigenschaften


                                      4 Geben Sie die Daten für die logische Maschine ein, z. B. für einen Schneid-
                                        tisch.
                                      5 Klicken Sie auf [OK], um die Daten zu speichern.
                                         Damit haben Sie die Stammdaten der logischen Maschine angelegt.
2.10 / 11-2018




                 D-38                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                      Maschinenzuordnung




                                       So löschen Sie eine logische Maschine

                                          Logische Maschinen löschen
                                          A+W Production legt zu jeder Maschine automatisch eine logische Maschi-
                                          ne an. Diese automatisch erstellte logische Maschine kann nicht gelöscht
                                          werden. Wird eine Maschine gelöscht, werden damit auch automatisch alle
                                          zugehörigen logischen Maschinen gelöscht.

                                          Wenn Sie eine logische Maschine löschen, löschen Sie die Funktion einer
                                          Maschine. Dies kann zu erheblichen Problemen im Produktionsprozess
                                          führen. Stellen Sie sicher, dass die logische Maschine und die Maschine
                                          nicht in der Fertigung verwendet wird, bevor Sie sie löschen.

                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Logische Maschinen.
                                      2 Markieren Sie die logische Maschine, die Sie löschen wollen.
                                      3 Klicken Sie auf [Löschen].
                                          Eine Sicherheitsabfrage wird angezeigt.
                                      4 Bestätigen Sie die Sicherheitsabfrage mit [Yes], wenn Sie die logische Ma-
                                        schine endgültig löschen möchten.
                                          Die Daten werden gelöscht.


                                      Übungen zu logischen Maschinen
                                      Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
                                      •   Legen Sie Übungsmaschinen an, die den Maschinenpark in Ihrem Betrieb
                                          abbilden oder verwenden Sie die Übungsmaschinen aus der vorherigen
                                          Lerneinheit.
                                          – Notieren Sie sich, welche Arbeitsgänge auf den jeweiligen Maschinen
                                             durchgeführt werden können, z. B. Bohren, Schleifen, Säumen.
                                          – Legen Sie die entsprechenden logischen Maschinen an.
                                      •   Ein ESG-Ofen kann vorspannen und teil-vorspannen. Würden Sie für die
                                          beiden Funktionen verschiedene logische Maschinen definieren? Nennen
                                          Sie die Vorteile und Nachteile.


                                      Ergänzende Informationen
                                       “Übungen zu Maschinen” auf Seite D-32
                                       Softwarereferenz, “Neue logische Maschine” auf Seite D-103
                                       Softwarereferenz, “Logische Maschine” auf Seite D-104
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-39
                 Maschinenzuordnung                                                                                Tutorial




                                      Arbeitsgänge
                                      Lernziele

                                      •   Was sind Arbeitsgänge speziell in der Maschinenzuordnung?
                                      •   Wie werden Arbeitsgänge verwaltet, angelegt, bearbeitet oder gelöscht?
                                      •   Warum haben Arbeitsgänge Prioritäten und wie werden diese verändert?
                                      •   Was haben Arbeitsgänge mit Bearbeitungstypen und Artikeln zu tun?


                                      Nutzen

                                      • Mit einem Arbeitsgang wird eine Anforderung eine Bearbeitung auszuführen erfüllt,
                                        die aus der Stückliste kommt. Diese Anforderung kann zum Beispiel lauten
                                        polieren oder schleifen. Der Arbeitsgang definiert anhand dieser Anforderung dann
                                        die spezielle Art des Polierens oder Schleifens.
                                      • Die Ebene der logischen Maschine stellt die Verbindung zwischen Arbeitsgang und
                                        physikalischer Maschine her, auf welcher der Arbeitsgang ausgeführt wird.


                                      Merke

                                      Arbeitsgänge                Arbeitsgänge bringen die Eigenschaften des
                                                                  Bearbeitungstyps, wie z. B. Zuschnitt, mit den
                                                                  Eigenschaften des Werkstücks zusammen.
                                                                  Arbeitsgänge basieren auf Bearbeitungstypen oder
                                                                  Artikeln.

                                      Bedingungen/Formeln         Arbeitsgänge können auch mit Bedingungen/Formeln
                                                                  definiert werden.
2.10 / 11-2018




                 D-40                                                         A+W Production Maschinenzuordnung
                 Tutorial                                                                       Maschinenzuordnung




                                      Arbeitsgänge in der Maschinenzuordnung
                                      Ein Arbeitsgang wird durch einen hinterlegten Bearbeitungstyp, einen Bear-
                                      beitungsartikel, eine Artikelgruppe und/oder eine zusätzliche Bedingung defi-
                                      niert.
                                       “Bearbeitungstypen und Bearbeitungsartikel” auf Seite D-69




                                      Abb. D-17    Arbeitsgänge


                                      Ist zu einem Arbeitsgang ein Bearbeitungstyp, z. B. Zuschnitt, hinterlegt, ist
                                      damit festgelegt, um welche technische Form der Bearbeitung es sich bei dem
                                      Arbeitsgang handelt. Nutzen Sie vorrangig den Standard-Bearbeitungstypen-
                                      katalog der A+W Software GmbH, um Arbeitsgänge zu definieren.
                                      Legen Sie nur eigene Bearbeitungstypen an, wenn es keine passenden vor-
                                      definierten Bearbeitungstypen gibt. Separate Arbeitsgänge legen Sie an,
                                      wenn Sie Aussagen über Ihre Produktion treffen können, z. B.:
                                      •   Siebdruck in dunklen Farben fassen Sie an einem bestimmten Wochentag
                                          zusammen, weil Sie dann das Lösemittel entsorgen (Mögliche Kampag-
                                          nenplanung).
                                      •   Die dicken Scheiben werden auf Maschine 1 geschliffen. Die dünnen
                                          Scheiben auf Maschine 2, aber sie dienen gegenseitig als Ausweichma-
                                          schine (Wahl des Bestbetriebsmittels)
                                      •   Serienscheiben dürfen nur auf der automatischen Bohrstraße gebohrt wer-
2.10 / 11-2018




                                          den. Wenn die ausfällt, müssen Sie den Liefertermin verschieben.




                 A+W Production Maschinenzuordnung                                                            D-41
                 Maschinenzuordnung                                                                        Tutorial




                                      Der Arbeitsgang Pseudo-Bearbeitung steht für Bearbeitungen in der Stück-
                                      liste, die informativen Charakter haben, z. B. Nicht stempeln, Handschuhe
                                      benutzen, Toleranz beachten. Damit für diese Bearbeitungen keine Terminfin-
                                      dung durchgeführt wird, werden sie auf eine Maschine Dummy für informative
                                      Bearbeitungen eingelastet, die keine BDE-Erfassungsstelle hat und damit
                                      auch keinen Schichtplan.

                                      Bearbeitungsartikel am Arbeitsgang
                                      Wenn Sie zu einem Arbeitsgang einen Bearbeitungsartikel hinterlegen, z. B.
                                      Modellzuschnitt für VSG, können Sie noch vor der eigentlichen Maschinenzu-
                                      ordnung die Behandlung der VSG-Modelle von den anderen Gläsern trennen.




                                      A
                                      B
                                      C




                                      A Artikeltyp                          C Artikel
                                      B Artikelgruppe
                                      Abb. D-18   Arbeitsgang – Artikel


                                      Sie können den Arbeitsgang noch genauer spezifizieren, indem Sie zusätzlich
                                      eine Restriktion aus dem Feld Artikel wählen. Der Artikeltyp (A) ist von der
                                      A+W Software GmbH vordefiniert. Er enthält Basis-Artikel, z. B. ESG, VSG
                                      oder Sprossen.
                                      Wenn Sie z. B. den Bearbeitungstyp Zuschnitt und zusätzlich den Artikel VSG
2.10 / 11-2018




                                      auswählen, legen Sie einen Arbeitsgang an, mit dem der Zuschnitt von VSG
                                      durchgeführt wird.




                 D-42                                                     A+W Production Maschinenzuordnung
                 Tutorial                                                                                Maschinenzuordnung




                                               Mit der Artikelgruppe (B) können Sie aus Produktionsartikelgruppen wählen,
                                               die Sie selbst definiert haben. Wählen Sie z. B. zum Bearbeitungstyp Zu-
                                               schnitt die Artikelgruppe Ganzglastüren. Damit haben Sie einen Arbeitsgang
                                               angelegt, mit dem der Zuschnitt von Ganzglastüren durchgeführt wird.
                                               Wählen Sie einen Artikel (C), um einen Arbeitsgang an einem speziellen Arti-
                                               kel festzumachen. Wenn Sie z. B. zu einem Arbeitsgang den Bearbeitungstyp
                                               Zuschnitt und den Artikel Float 6 mm angeben, legen Sie einen Arbeitsgang
                                               an, mit dem der Zuschnitt von 6 mm-Float durchgeführt wird.

                                                   Bearbeitungstypen
                                                   Zu Bearbeitungstypen gibt es eine separate Lerneinheit:

                                                    “Bearbeitungstypen und Bearbeitungsartikel” auf Seite D-69




                            Arbeitsgang für Zuschnitt:        Arbeitsgang für Zuschnitt       Arbeitsgang für Zuschnitt
                                                                      von VSG:                    von Float 6 mm:



                                                                 Arbeitsgang Zuschnitt           Arbeitsgang Zuschnitt
                              Arbeitsgang Zuschnitt
                                                                         VSG                          Float 6 mm



                                 Bearbeitungstyp                    Bearbeitungstyp                Bearbeitungstyp
                                    Zuschnitt                          Zuschnitt                      Zuschnitt



                                                                        Katalog:                        Artikel:
                                                                         VSG                          Float 6 mm



                 Abb. D-19       Beispiele für unterschiedlich definierte Arbeitsgänge
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                        D-43
                 Maschinenzuordnung                                                                               Tutorial




                                      Arbeitsgang exakt definieren
                                      Durch Verwenden der Optionen im Dialog Arbeitsgang im Feld Artikel definie-
                                      ren Sie Arbeitsgänge exakt.

                                         Beispiel 1:

                                         Der Zuschnitt von VSG kann nur an Schneidetischen erfolgen, die zwei
                                         Schneidköpfe haben, oder andere Techniken einsetzen, wie z. B. Waterjet.
                                         Für den Zuschnitt von Float besteht bereits der Arbeitsgang Zuschnitt.
                                         Definieren Sie nun einen neuen Arbeitsgang zum Schneiden von VSG.
                                         Wählen Sie dazu den Bearbeitungstyp Zuschnitt den Glastyp VSG.
                                         Damit definieren Sie einen Arbeitsgang, der die Problematik beim Schneiden
                                         von VSG berücksichtigt und dem nur logische Maschinen zugeordnet werden
                                         dürfen, die diese Bearbeitung durchführen können.


                                         Beispiel 2 – Option Artikelgruppe:

                                         Sie haben Artikel, die nur selten produziert werden.
                                         Bilden Sie in diesem Fall eine Artikelgruppe mit den seltenen Artikeln und
                                         starten Sie eine Kampagne. Da die Kampagnen-Planung auf einem
                                         Arbeitsgang basiert, wählen Sie für diese Kampagne die Artikelgruppe mit
                                         den seltenen Artikeln.
                                         So können Sie exakt vorausplanen, wann und wie die seltenen Artikel
                                         gefertigt werden.
                                         Kampagnen sind ausführlich im Part Kapazitätsplanung beschrieben.


                                      Nicht zugeordnete Arbeitsgänge
                                      Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logische
                                      Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logische Ma-
                                      schine zu. Ist die zugehörige logische Maschine noch nicht definiert, sollte
                                      temporär die logische Maschine Dummy zugeordnet werden.
                                       “Arbeitsgangzuordnung” auf Seite D-51

                                      Priorität von Arbeitsgängen
                                      Die Arbeitsgänge können in der Liste nach oben oder unten verschoben wer-
                                      den. Die Liste wird bei der Arbeitsgangzuordnung von oben nach unten abge-
                                      arbeitet. Sobald alle einem Arbeitsgang zugeordneten Bedingungen zutreffen,
                                      wird dieser Arbeitsgang zugeordnet. Deshalb ist es notwendig, spezialisierten
                                      Arbeitsgängen immer eine höhere Priorität zuzuweisen, als unspezialisierten
                                      Arbeitsgängen.
2.10 / 11-2018




                 D-44                                                          A+W Production Maschinenzuordnung
                 Tutorial                                                                     Maschinenzuordnung




                                      Mehrere Arbeitsgänge an einer Scheibe
                                      Sie haben den Auftrag eine Glastür zu produzieren. Dazu werden die Arbeits-
                                      gänge Rechteckschleifen, Bohren und Ausschnitte benötigt.
                                      Anstatt das Rechteckschleifen auf der kostengünstigen Rechteckschleifma-
                                      schine auszuführen, lassen Sie alle drei Arbeitsgänge auf dem CNC-Center
                                      durchführen. Damit ist der einzelne Arbeitsgang Rechteckschleifen zwar teu-
                                      rer, aber Sie sparen Aufwand, indem alle drei Arbeitsgänge direkt hintereinan-
                                      der auf einer Maschine durchgeführt werden.
                                      Dazu haben Sie den Arbeitsgang Rechteckschleifen auf CNC-Center defi-
                                      niert, dem Sie die logische Maschine CNC-Center Rechteckschleifen mit ho-
                                      her Priorität zugeordnet haben.
                                      Um Engpässe zu vermeiden, ist dem Arbeitsgang Rechteckschleifen auf
                                      CNC-Center auch die logische Maschine Rechteckschleifmaschine zugeord-
                                      net, mit niedriger Priorität.
                                      Würden Sie die Glastür auf günstigeren Maschinen fertigen, sähe der Produk-
                                      tionsablauf so aus:
                                      •   Schleifen auf der Rechteckschleifmaschine.
                                      •   Anschließend Bohren auf der automatischen Bohrmaschine.
                                      •   Abschließend Fertigen der Ausschnitte auf dem CNC-Center.
                                          Dazu kommen 2 x Handling, 2 x Waschen und die Rüstzeit für das CNC-
                                          Center.
                                      Es kann also günstiger sein, die Glastür komplett auf dem CNC-Center zu fer-
                                      tigen.

                                      Zusätzliche Bedingungen in Arbeitsgängen
                                      Arbeitsgänge sind nicht ausschließlich an Bearbeitungen gebunden. Sie kön-
                                      nen auch zusätzliche Bedingungen enthalten. Eine Bedingung kann zum Bei-
                                      spiel lauten: Dieser Arbeitsgang wird auf dem CNC-Center durchgeführt. So
                                      können Sie bei der Definition des Arbeitsgangs vorgeben, welche Maschinen
                                      vorrangig verwendet werden.
                                      Eine zusätzliche Bedingung kann auch die Stückliste abfragen. Wird eine ent-
                                      sprechende Bedingung an einem Arbeitsgang hinterlegt, kann damit der Lauf-
                                      weg der Scheibe durch die Produktion gesteuert werden. Die Bedingung
                                      könnte beispielsweise lauten: Stehen in der Stückliste der Scheibe die Bear-
                                      beitungen Schleifen, Bohren und Ausschneiden, dann fertige die Scheibe
                                      komplett auf dem CNC-Center.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                            D-45
                 Maschinenzuordnung                                                                                         Tutorial




                    Stückliste                                      Arbeitsgang                            Logische Maschine


                    Stückliste Glastür:                             Arbeitsgang                            Logische Maschine
                    • Schleifen
                    • Bohren                             Arbeitsgang Glastür mit Bedingung:                Logische Maschine
                    • Ausschneiden                       Stehen in der Stückliste
                                                         Schleifen + Bohren + Ausschneiden
                    Stückliste                           = fertige auf CNC-Center


                    Stückliste                                      Arbeitsgang                                CNC-Center



                 Abb. D-20       Beispiel: Eine zusätzliche Bedingung im Arbeitsgang fragt die Stückliste ab


                                               In diesem Beispiel sehen Sie einen weiteren Weg, den Laufweg einer Scheibe
                                               durch die Produktion zu steuern, nämlich eine Arbeitsgangzuordnung auf Ba-
                                               sis eines Bearbeitungsartikels.
                                               Dazu definieren Sie zum Beispiel den Bearbeitungsartikel Glastür. Der Bear-
                                               beitungsartikel Glastür wird vom Arbeitsgang Glastür ausgeführt, der Arbeits-
                                               gang Glastür hat die Bedingung, dass auf dem CNC-Center gefertigt wird.



                    Bearbeitungsartikel Glastür                     Arbeitsgang                            Logische Maschine


                    Bearbeitungsartikel                             Arbeitsgang                                CNC-Center


                    Bearbeitungsartikel           Arbeitsgang Glastür                                      Logische Maschine
                                                  basiert auf dem Bearbeitungsartikel Glastür
                                                  Bedingung: fertige auf CNC-Center                       Logische Maschine
                    Bearbeitungsartikel


                                                                    Arbeitsgang



                 Abb. D-21       Beispiel: Arbeitsgangzuordnung auf Basis eines Bearbeitungsartikels
2.10 / 11-2018




                 D-46                                                                   A+W Production Maschinenzuordnung
                 Tutorial                                                                         Maschinenzuordnung




                                         Beispiel: Engpass durch zusätzliche Bedingung

                                         Zum Arbeitsgang Glastür ist die Bedingung hinterlegt, dass Glastüren auf
                                         dem CNC-Center gefertigt werden. Die Bedingung kann sich entweder auf
                                         die Stückliste oder einen Bearbeitungsartikel beziehen.
                                         Wenn zum Auftrag mit Glastüren ein weiterer Auftrag, zum Beispiel mit
                                         Modellen, kommt, entsteht auf dem CNC-Center ein Engpass.
                                         Lösung: Sie ändern die Priorität der logischen Maschine CNC-Center,
                                         sodass das CNC-Center nicht mehr die erste Wahl für Glastüren ist. Dadurch
                                         werden die Glastüren nicht auf dem CNC-Center gefertigt, sondern in
                                         einzelnen Arbeitsschritten auf der Rechteckschleifmaschine, der
                                         automatischen Bohrmaschine und der Ausschneidemaschine.
                                         Das erhöht zwar den Handling-Aufwand bei den Glastüren, ermöglicht aber,
                                         die Modelle gleichzeitig auf dem CNC-Center zu fertigen.
                                         Ist der Engpass vorüber, müssen die ursprünglichen Prioritäten der logischen
                                         Maschinen wieder hergestellt werden.


                                      Sie können Arbeitsgänge auch auf Basis eines Bearbeitungsartikels definie-
                                      ren, was zum Beispiel dann sinnvoll ist, wenn Sie eine Bearbeitung künstlich
                                      in die Stückliste einfügen wollen.

                                         Beispiel: Arbeitsgang basierend auf Bearbeitungsartikel

                                         Ein ESG wurde beschichtet und muss ab diesem Zeitpunkt mit Handschuhen
                                         angefasst werden.
                                         Definieren Sie für diesen Fall den Bearbeitungsartikel Handschuhe tragen!
                                         und wählen Sie diesen als Grundlage für den Arbeitsgang. In der
                                         Arbeitsgangzuordnung ordnen Sie den Arbeitsgang der logischen Maschine
                                         Dummy zu.
                                         Damit haben Sie einen Arbeitsgang eingeführt, der auf keiner Maschine läuft,
                                         aber in der Produktion als handhabe beschichtete ESG mit Handschuhen
                                         existiert.

                                         Arbeitsgang basierend auf Bearbeitungsartikel nur in Einzelfällen
                                         Arbeitsgänge auf der Basis von Bearbeitungsartikeln bilden eine Ausnah-
                                         me, da Sie für die Aufnahme neuer Bearbeitungsartikel die Arbeitsgangzu-
                                         ordnung ergänzen und pflegen müssen. Die Definition von Arbeitsgängen
                                         basierend auf Bearbeitungsartikeln ist nur in Einzelfällen, wie in oben ge-
                                         nanntem Beispiel, sinnvoll.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                   D-47
                 Maschinenzuordnung                                                                         Tutorial




                                      Arbeitsgänge anlegen und verwalten
                                      In dieser Lerneinheit legen Sie neue Arbeitsgänge an, bearbeiten und löschen
                                      diese aus der Liste.
                                      Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                      •   “So legen Sie einen Arbeitsgang an” auf Seite D-48.
                                      •   “So bearbeiten Sie die Restriktionen zu einem Arbeitsgang” auf Seite D-49.
                                      •   “So löschen Sie einen Arbeitsgang” auf Seite D-50

                                          IDs für Arbeitsgänge
                                          Geben Sie einem Arbeitsgang immer die zugrundeliegende ID der Bear-
                                          beitung und/oder des Artikels multipliziert mit 10.
                                          Beispiel: Dem Arbeitsgang liegt die Bearbeitung Säumen mit der ID 1000
                                          aus dem Standard-Bearbeitungskatalog zugrunde.
                                          Geben Sie in diesem Fall dem neuen Arbeitsgang die ID 10000.
                                          Mit diesem System lassen sich Bearbeitungen, Artikel und Arbeitsgänge
                                          auseinanderhalten, aber die Zugehörigkeit ist leicht erkennbar.


                                       So legen Sie einen Arbeitsgang an
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Arbeitsgänge > [Neu].
                                          Der Dialog Neuer Arbeitsgang wird geöffnet.
                                      2 Geben Sie die Daten ein.




                                          Abb. D-22   Neuer Arbeitsgang


                                      3 Klicken Sie auf [OK], um die Daten zu speichern.
                                          Der Dialog Arbeitsgang wird geöffnet, um die Restriktionen zu bearbeiten.

                                          Arbeitsgänge in roter Schrift
                                          Ein Arbeitsgang wird im MZO-Editor in roter Schrift angezeigt, wenn ihm
                                          noch keine logische Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen
                                          immer eine logische Maschine zu. Ist die zugehörige logische Maschine
                                          noch nicht definiert, kann temporär die logische Maschine Dummy zuge-
                                          ordnet werden.
2.10 / 11-2018




                 D-48                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                     Maschinenzuordnung




                                       So bearbeiten Sie die Restriktionen zu einem Arbeitsgang
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Arbeitsgänge.
                                         Das Register Arbeitsgänge wird angezeigt.
                                      2 Markieren Sie den Arbeitsgang, den Sie bearbeiten möchten.
                                      3 Klicken Sie auf [Bearbeiten].




                                         Abb. D-23   Arbeitsgang – Restriktionen bearbeiten


                                      4 Wählen Sie die Optionen und die entsprechenden Typen oder Artikel, um
                                        den Arbeitsgang zu definieren.
                                         Damit haben Sie den Arbeitsgang bearbeitet.
                                      5 Klicken Sie auf [OK], um die Daten zu speichern.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-49
                 Maschinenzuordnung                                                                         Tutorial




                                       So löschen Sie einen Arbeitsgang
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Arbeitsgänge.
                                          Das Register Arbeitsgänge wird angezeigt.
                                      2 Markieren Sie den Arbeitsgang, den Sie löschen möchten.
                                          Ein Arbeitsgang wird im MZO-Editor in roter Schrift angezeigt, wenn ihm
                                          noch keine logische Maschine zugeordnet ist.
                                      3 Klicken Sie auf [Löschen]
                                          Eine Sicherheitsabfrage wird geöffnet.
                                      4 Klicken Sie auf [Yes], um den Arbeitsgang endgültig zu löschen.
                                          Die Daten werden gelöscht.


                                      Übungen zu Arbeitsgängen
                                      Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
                                      •   Legen Sie Übungsmaschinen und logische Übungsmaschinen an, die den
                                          Maschinenpark in Ihrem Betrieb abbilden oder verwenden Sie die Übungs-
                                          maschinen und logische Übungsmaschinen aus den vorigen Übungen.
                                           “Übungen zu Maschinen” auf Seite D-32
                                           “Übungen zu logischen Maschinen” auf Seite D-39
                                          – Definieren Sie einen Übungsarbeitsgang Polieren, der auf dem Stan-
                                              dard-Bearbeitungskatalog basiert.
                                          – Definieren Sie einen Übungsarbeitsgang handhabe beschichtete ESG
                                              mit Handschuhen. Der Arbeitsgang soll auf einem Bearbeitungsartikel
                                              basieren.
                                          – Definieren Sie einen Übungsarbeitsgang VSG-Zuschnitt, der auf dem
                                              Standard-Bearbeitungskatalog basiert und den Sie mit einem Artikel ge-
                                              nauer definieren.
                                      •   Bilden Sie den Maschinenpark Ihres Betriebes auf Papier ab und listen Sie
                                          die daraus resultierenden logischen Maschinen auf.
                                          Betrachten Sie die aktuelle Auftragssituation, welche Arbeitsgänge sind in
                                          dieser Situation anzulegen?


                                      Ergänzende Informationen
                                       Softwarereferenz, “Neuer Arbeitsgang” auf Seite D-107
                                       Softwarereferenz, “Arbeitsgang” auf Seite D-108
2.10 / 11-2018




                 D-50                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                            Maschinenzuordnung




                                      Arbeitsgangzuordnung
                                      Lernziele

                                      •   Was ist die Arbeitsgangzuordnung?
                                      •   Wie werden Arbeitsgänge zugeordnet?
                                      •   Wie werden Zuordnungen wieder aufgelöst?
                                      •   Wie wird die Priorität von logischen Maschinen geändert?
                                      •   Warum haben logische Maschinen eine Priorität?


                                      Nutzen

                                      • Mit der Arbeitsgangzuordnung ordnen Sie logische Maschinen den Arbeitsgängen
                                        zu. Durch eine geschickte Zuordnung optimieren Sie die Kosten der Produktion.


                                      Merke

                                      Arbeitsgangzuordnung        Die Arbeitsgangzuordnung verbindet logische
                                                                  Maschinen mit Arbeitsgängen.

                                      Prioritäten                 Mit der Arbeitsgangzuordnung werden Prioritäten der
                                                                  logischen Maschinen festgelegt. Damit legen Sie fest,
                                                                  dass der jeweilige Arbeitsgang auf der optimalen
                                                                  Maschine und möglichst kostengünstig durchgeführt
                                                                  wird.

                                      Arbeitsgangzuordnung        Mit der Arbeitsgangzuordnung hat der Anwender die
                                                                  Möglichkeit in den Produktionsprozess einzugreifen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                  D-51
                 Maschinenzuordnung                                                                        Tutorial




                                      Angepasste Arbeitsgangzuordnung
                                      Sie ordnen logische Maschinen den jeweiligen Arbeitsgängen zu. Unter jedem
                                      Arbeitsgang kann die Reihenfolge, und damit die Priorität der logischen Ma-
                                      schinen, festgelegt werden. Somit legen Sie Prioritäten der Maschinen im Pro-
                                      duktionsprozess fest.
                                      Bei Maschinen, die mehrere Funktionen durchführen können, wie z. B. ein
                                      CNC-Center, entsteht die Tendenz, dass mehr Arbeitsgänge auflaufen als bei
                                      spezialisierten Maschinen, die z. B. nur eine Funktion durchführen können.
                                      Resultat ist, dass mehr Arbeitsgänge am teuren CNC-Center durchgeführt
                                      werden und dadurch ein Engpass entsteht.
                                      Das können Sie durch Priorisierung in der Arbeitsgangzuordnung und dem
                                      Definieren angepasster Arbeitsgänge verhindern.
                                      Sie legen Arbeitsgänge an, die die einzelnen Anwendungen exakt abbilden
                                      und ordnen diese Arbeitsgänge den dazu passenden logischen Maschinen zu.
                                      So können Sie sicherstellen, dass die Arbeitsgänge an den jeweils kosten-
                                      günstigsten Maschinen durchgeführt werden.

                                      Bedingung in einem Arbeitsgang
                                      Arbeitsgänge können auch zusätzliche Bedingungen enthalten. So können
                                      Sie schon bei der Definition des Arbeitsgangs vorgeben, welche Maschinen
                                      vorrangig verwendet werden.
                                      Eine zusätzliche Bedingung kann auch die Stückliste abfragen. Die Bedingung
                                      könnte beispielsweise lauten: Stehen in der Stückliste der Scheibe die Bear-
                                      beitungen Schleifen, Bohren und Ausschneiden, dann fertige die Scheibe
                                      komplett auf dem CNC-Center.
                                      Wird eine entsprechende Bedingung an einem Arbeitsgang hinterlegt, kann
                                      damit der Laufweg der Scheibe durch die Produktion gesteuert werden.

                                         Arbeitsgänge immer zuordnen
                                         Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logi-
                                         sche Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logi-
                                         sche Maschine zu. Ist die zugehörige logische Maschine noch nicht
                                         definiert, sollte temporär die logische Maschine Dummy zugeordnet wer-
                                         den.
2.10 / 11-2018




                 D-52                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                                       Maschinenzuordnung




                     Stückliste                                      Arbeitsgang                            Logische Maschine


                     Stückliste Glastür:                             Arbeitsgang                            Logische Maschine
                     • Schleifen
                     • Bohren                             Arbeitsgang Glastür mit Bedingung:                Logische Maschine
                     • Ausschneiden                       Stehen in der Stückliste
                                                          Schleifen + Bohren + Ausschneiden
                     Stückliste                           = fertige auf CNC-Center


                     Stückliste                                      Arbeitsgang                                 CNC-Center



                 Abb. D-24        Beispiel: Eine zusätzliche Bedingung im Arbeitsgang fragt die Stückliste ab


                                                In diesem Beispiel sehen Sie einen weiteren Weg, den Laufweg einer Scheibe
                                                durch die Produktion zu steuern, nämlich eine Arbeitsgangzuordnung auf Ba-
                                                sis eines Bearbeitungsartikels.
                                                Dazu definieren Sie zum Beispiel den Bearbeitungsartikel Glastür. Der Bear-
                                                beitungsartikel Glastür wird vom Arbeitsgang Glastür ausgeführt. Der Arbeits-
                                                gang Glastür hat die Bedingung, dass auf dem CNC-Center gefertigt wird.



                     Bearbeitungsartikel Glastür                     Arbeitsgang                            Logische Maschine


                     Bearbeitungsartikel                             Arbeitsgang                                 CNC-Center


                     Bearbeitungsartikel           Arbeitsgang Glastür                                      Logische Maschine
                                                   basiert auf dem Bearbeitungsartikel Glastür
                                                   Bedingung: fertige auf CNC-Center                       Logische Maschine
                     Bearbeitungsartikel


                                                                     Arbeitsgang



                 Abb. D-25        Beispiel: Arbeitsgangzuordnung auf Basis eines Bearbeitungsartikels
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                              D-53
                 Maschinenzuordnung                                                                                         Tutorial




                             A




                                                                                                                       B
                                                                                                                       C




                 A Neu definierte Arbeitsgänge                            B Logische Maschine Rechteckschleifmaschine
                                                                          C Logische Maschine CNC Modellschleifen
                 Abb. D-26       Beispiel: angepasste Arbeitsgangzuordnung


                                                 Beispiel: angepasste Arbeitsgangzuordnung

                                                 Sie haben in Ihrer Produktion eine Rechteckschleifmaschine und ein CNC-
                                                 Center. Mit beiden kann die Bearbeitung Schleifen durchgeführt werden.
                                                 • In der Liste der Arbeitsgänge ist ein Arbeitsgang Rechteckschleifen
                                                   definiert, dem alle rechteckigen Scheiben zugeführt werden. In der
                                                   Arbeitsgangzuordnung ist dem Arbeitsgang Rechteckschleifen die
                                                   Rechteckschleifmaschine zugeordnet. Diese hat höchste Priorität.
                                                 • In der Liste der Arbeitsgänge ist ein Arbeitsgang Modellschleifen definiert,
                                                   dem alle Modelle zugeführt werden. In der Arbeitsgangzuordnung ist dem
                                                   Arbeitsgang Modellschleifen das CNC-Center zugeordnet.
                                                 • Das CNC-Center ist auch dem Arbeitsgang Rechteckschleifen
                                                   zugeordnet, jedoch mit geringerer Priorität.
                                                 Mit diesen Einstellungen wird das Schleifen von rechteckigen Scheiben auf
                                                 der kostengünstigen Rechteckschleifmaschine durchgeführt. Sollte ein
                                                 Engpass entstehen, werden die Rechtecke auch auf dem CNC-Center
                                                 geschliffen.
2.10 / 11-2018




                 D-54                                                                  A+W Production Maschinenzuordnung
                 Tutorial                                                                            Maschinenzuordnung




                             A

                             B




                 A Arbeitsgang Rechteckschleifen                     B Arbeitsgang Modellschleifen
                 Abb. D-27   Beispiel: angepasste Arbeitsgangzuordnung


                                          Müssen an einer Scheibe mehrere Arbeitsgänge durchgeführt werden, kann
                                          es günstiger sein, für einen einzelnen Arbeitsgang höhere Kosten in Kauf zu
                                          nehmen. Entscheidend ist in der Regel die Stückzahl der zu fertigenden Schei-
                                          ben.

                                             Beispiel: mehrere Arbeitsgänge an einer Scheibe

                                             Um eine Glastür zu produzieren, werden die Arbeitsgänge Rechteckschleifen,
                                             Bohren und Ausschnitte benötigt.
                                             Anstatt das Rechteckschleifen auf der kostengünstigen Rechteck-
                                             Schleifmaschine auszuführen, lassen Sie alle drei Arbeitsgänge auf dem CNC-
                                             Center durchführen. Damit ist der einzelne Arbeitsgang Rechteckschleifen zwar
                                             teurer, aber Sie sparen Aufwand, indem alle drei Arbeitsgänge direkt
                                             hintereinander auf einer Maschine durchgeführt werden.
                                             Dazu haben Sie den Arbeitsgang Rechteckschleifen auf CNC-Center definiert,
                                             dem Sie die logische Maschine CNC-Center Rechteckschleifen mit hoher Priorität
                                             zugeordnet haben.
                                             Um Engpässe zu vermeiden, ist dem Arbeitsgang Rechteckschleifen auf CNC-
                                             Center auch die logische Maschine Rechteckschleifmaschine zugeordnet. Diese
                                             hat niedrige Priorität.
                                             Der Produktionsablauf auf günstigeren Maschinen sähe so aus:
                                             • Schleifen auf der Rechteckschleifmaschine.
2.10 / 11-2018




                                             • Bohren auf der automatischen Bohrmaschine.
                                             • Fertigen der Ausschnitte auf dem CNC-Center.
                                               Dazu kommen 2x Handling, 2x Waschen und die Rüstzeit für das CNC-Center.



                 A+W Production Maschinenzuordnung                                                                   D-55
                 Maschinenzuordnung                                                                            Tutorial




                                     A




                                                                                                                     B




                 C




                                                                                                D




                 A Arbeitsgang Rechteckschleifen auf CNC-Center.   C Arbeitsgang Rechteckschleifen auf CNC-Center.
                 B Logische Maschine CNC-Center Rechteckschleifen. D Logische Maschine Rechteckschleifmaschine.
                 Abb. D-28   Beispiel: mehrere Arbeitsgänge an einer Scheibe
2.10 / 11-2018




                 D-56                                                          A+W Production Maschinenzuordnung
                 Tutorial                                                                  Maschinenzuordnung




                                      In diesem Beispiel sehen Sie, dass dem Arbeitsgang Rechteckschleifen auf
                                      CNC-Center die logische Maschine CNC-Center Rechteckschleifen mit
                                      höchster Priorität zugeordnet ist. Zudem wurde die logische Maschine Recht-
                                      eckschleifmaschine mit geringerer Priorität zugeordnet, um Engpässe zu ver-
                                      meiden.
                                      Dem Beispiel zu mehreren Arbeitsgängen an einer Scheibe entsprechend ist
                                      es die kostengünstigere Variante, die Glastür komplett auf dem CNC-Center
                                      zu fertigen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-57
                 Maschinenzuordnung                                                                       Tutorial




                                      Arbeitsgänge und logische Maschinen zuordnen
                                      In dieser Lerneinheit ordnen Sie logische Maschinen den Arbeitsgängen zu,
                                      trennen Arbeitsgänge und logische Maschinen und ändern Prioritäten von lo-
                                      gischen Maschinen.
                                      Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                      •   “So ordnen Sie eine logische Maschine einem Arbeitsgang zu” auf
                                          Seite D-58.
                                      •   “So trennen Sie logische Maschinen von Arbeitsgängen” auf Seite D-60.
                                      •   “So ändern Sie die Priorität einer logischen Maschine” auf Seite D-61.


                                       So ordnen Sie eine logische Maschine einem Arbeitsgang zu
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung.
                                          Das Register Arbeitsgangzuordnung wird angezeigt.
                                      2 Markieren Sie den Arbeitsgang und die logische Maschine, die Sie einan-
                                        der zuordnen wollen.




                                          Abb. D-29   Arbeitsgang und logische Maschine markiert
2.10 / 11-2018




                 D-58                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                    Maschinenzuordnung




                                      3 Klicken Sie auf den Pfeil nach links, um die logische Maschine dem Ar-
                                        beitsgang zuzuordnen.
                                         Die logische Maschine ist nun dem Arbeitsgang zugeordnet und wird unter
                                         dem Arbeitsgang grau hinterlegt angezeigt.




                                         Abb. D-30   Arbeitsgang und logische Maschine zugeordnet


                                      4 Klicken Sie auf [Übernehmen], um die Daten zu speichern.
                                         Die Zuordnung wird gespeichert.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-59
                 Maschinenzuordnung                                                                         Tutorial




                                       So trennen Sie logische Maschinen von Arbeitsgängen
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung.
                                         Das Register Arbeitsgangzuordnung wird angezeigt.
                                      2 Klicken Sie auf [+] des Arbeitsgangs.
                                         Die Ansicht klappt auf und die logischen Maschinen werden angezeigt, die
                                         dem Arbeitsgang zugeordnet sind.
                                      3 Markieren Sie die logische Maschine, die getrennt werden soll.




                                         Abb. D-31    Arbeitsgang und logische Maschine trennen


                                      4 Klicken Sie auf den Pfeil nach rechts, um die logische Maschine vom Ar-
                                        beitsgang zu trennen.
                                      5 Klicken Sie auf [Übernehmen], um die Änderungen zu speichern.

                                         Logische Maschine noch in Verwendung
                                         Wenn eine Zuordnung entfernt werden soll, die noch in Verwendung ist,
                                         wird sie automatisch deaktiviert. Deaktivierte Zuordnungen werden in kur-
                                         siver Schrift und mit einem entsprechenden Symbol dargestellt.

                                         Bitte beachten: falls eine deaktivierte logische Maschine in einem beste-
                                         henden Auftrag für einen Arbeitsgang eine Alternative darstellt, wird diese
2.10 / 11-2018




                                         Alternative bei der Umlastung nach wie vor angeboten. Erst bei einer Wie-
                                         derholung der MZO für diesen Auftrag wird die Deaktivierung berücksich-
                                         tigt.



                 D-60                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                   Maschinenzuordnung




                                       So ändern Sie die Priorität einer logischen Maschine
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung.
                                         Das Register Arbeitsgangzuordnung wird angezeigt.
                                      2 Klicken Sie auf [+] eines Arbeitsgangs, um die zugeordneten logischen Ma-
                                        schinen anzuzeigen.

                                         Alle logischen Maschinen anzeigen
                                         Sie können sich alle zugeordneten logischen Maschinen anzeigen lassen,
                                         indem Sie in die Checkbox [Alles aufklappen] klicken.

                                      3 Markieren Sie die logische Maschine, deren Priorität Sie ändern wollen.
                                      4 Klicken Sie auf den Pfeil nach oben oder den Pfeil nach unten, um die Pri-
                                        orität hoch oder runter zu setzen.




                                         Abb. D-32   Priorität logischer Maschinen ändern


                                         Die logische Maschine wird in der Liste weiter oben oder unten verscho-
                                         ben, je nach Änderung der Priorität.
                                      5 Klicken Sie auf [Übernehmen], um die Änderungen zu speichern.
                                         Die Änderung der Priorität wird gespeichert.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-61
                 Maschinenzuordnung                                                                        Tutorial




                                      Übungen zur Arbeitsgangzuordnung
                                      Festigen Sie Ihr neu erworbenes Wissen mit nachfolgenden Übungen.
                                      •   Legen Sie testweise Übungsmaschinen, logische Übungsmaschinen und
                                          Übungsarbeitsgänge an, die den Maschinenpark in Ihrem Betrieb abbilden
                                          oder verwenden Sie die Übungsmaschinen, logischen Übungsmaschinen
                                          und Übungsarbeitsgänge aus den vorherigen Lerneinheiten:
                                           “Übungen zu Maschinen” auf Seite D-32
                                           “Übungen zu logischen Maschinen” auf Seite D-39
                                           “Übungen zu Arbeitsgängen” auf Seite D-50
                                          – Ordnen Sie die testweise erstellten logischen Maschinen und Arbeits-
                                             gänge einander zu.
                                          – Spielen Sie verschiedene Szenarien durch und vergeben Sie Prioritä-
                                             ten, um Arbeitsgänge auf der günstigsten Maschine durchzuführen,
                                             oder um mehrere Arbeitsgänge auf einem CNC-Center durchzuführen.
                                      •   Betrachten Sie die gegenwärtige Situation Ihres Maschinenparks und der
                                          angelegten Maschinen, logischen Maschinen und Arbeitsgänge.
                                          Notieren Sie sich, welche Arbeitsgangzuordnung bei den momentanen
                                          Aufträgen sinnvoll ist und welche Prioritäten Sie vergeben müssen, um ein
                                          optimales Ergebnis zu erzielen.


                                      Ergänzende Informationen
                                       Softwarereferenz, “Neuer Arbeitsgang” auf Seite D-107
                                       Softwarereferenz, “Arbeitsgang” auf Seite D-108
2.10 / 11-2018




                 D-62                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                       Maschinenzuordnung




                                      Bedingungen, Formeln, Restriktionen
                                      Lernziele

                                      • Wo werden Formeln und Bedingungen eingesetzt?
                                      • Wie werden Formeln und Bedingungen ausgewählt?
                                      • Warum ist von Formeln und Bedingungen die Rede und wo liegt der Unterschied?


                                      Nutzen

                                      • Mit Formeln und Restriktionen werden Maschinen, logische Maschinen und
                                        Arbeitsgänge genauer definiert.


                                      Merke

                                      Formeln                   Formeln kommen bei Maschinen, logischen Maschinen
                                                                und Arbeitsgängen zum Einsatz.
                                                                Formeln sind bereits vordefiniert oder können mit dem
                                                                grafischen Formeleditor oder mit dem Text-Formeleditor
                                                                definiert werden.
                                                                Formeln werden verwendet, um Restriktionen von
                                                                Maschinen, logischen Maschinen und Arbeitsgängen
                                                                exakter zu definieren.
                                                                Formeln sind Restriktionen oder Bedingungen, die in der
                                                                Datenbanksprache SQL ausgedrückt werden können.

                                      Formeleditor              Der Formeleditor ist ein Werkzeug, das es dem
                                                                Anwender ermöglicht, Restriktionen selbst zu
                                                                formulieren.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                               D-63
                 Maschinenzuordnung                                                                             Tutorial




                                      Bedingungen und Formeln in der Maschinenzuord-
                                      nung
                                      In dieser Lerneinheit erfahren Sie, wie Sie Formeln/Bedingungen auswählen.
                                      In der Maschinenzuordnung können Formeln und Bedingungen zu Maschi-
                                      nen, logischen Maschinen und Arbeitsgängen hinzugefügt werden. Im Zusam-
                                      menhang mit Formeln ist oftmals auch die Rede von Restriktionen und
                                      Bedingungen. In A+W Production besteht zwischen Formeln, Restriktionen
                                      und Bedingungen folgender Zusammenhang:
                                      •   Maschinen, logische Maschinen und Arbeitsgänge haben bestimmte Ei-
                                          genschaften, die oftmals restriktiv sind. So können zum Beispiel Schneid-
                                          tische nur Scheiben bis zu einer bestimmten Größe bearbeiten.
                                          Für einen Teil der gängigen Restriktionen gibt es zum Beispiel im Dialog
                                          Maschine vordefinierte Felder. Die Werte, die Sie dort festlegen, werden in
                                          den Stammdaten der Maschine, logischen Maschine oder dem Arbeits-
                                          gang als Formel hinterlegt.
                                      •   Darüber hinaus gibt es jeweils im Feld Zusätzliche Bedingung die Möglich-
                                          keit, selbst definierte Formeln zu hinterlegen. Sie haben damit einen höhe-
                                          ren Freiheitsgrad, um Sachverhalte abzubilden, die genau auf Ihre
                                          Produktion zutreffen.

                                          Anlegen von Formeln
                                          Bei Fragen zur Erstellung und Änderung von Formeln wenden Sie sich bit-
                                          te an den Support der A+W Software GmbH.

                                          Zum Anlegen und Verwalten von Formeln besteht ein separates Tutorial:

                                           Formeleditor: Bedienung, “Bedingungen für Abstellplätze” auf Seite R-29
2.10 / 11-2018




                 D-64                                                         A+W Production Maschinenzuordnung
                 Tutorial                                                                     Maschinenzuordnung




                                      Bedingung auswählen
                                      Sie können eine Bedingung in den Eigenschaften der Maschinen, logischen
                                      Maschinen oder Arbeitsgängen auswählen. Die Formeln für eine Bedingung
                                      bearbeiten Sie im Formel-Editor.
                                       “Formel zur Bearbeitungsdauer einer logischen Maschine auswählen” auf
                                        Seite D-66


                                       So wählen Sie eine Bedingung aus
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Logische Maschinen.
                                         In diesem Beispiel wird die Bedingung für eine Logische Maschine einge-
                                         richtet. Die Beschreibung gilt analog auch für Maschinen und Arbeitsgän-
                                         ge.
                                      2 Markieren Sie die Logische Maschine und klicken Sie auf [Bearbeiten].
                                      3 Klicken Sie im Bereich Zusätzliche Bedingung die [Lupe], um eine Bedin-
                                        gung auszuwählen.




                                         Abb. D-33    Bedingung auswählen


                                      4 Markieren Sie die Bedingung, die Sie übernehmen wollen.
                                         Wenn zu der Bedingung eine Formel angelegt ist, wird der Inhalt im Feld
                                         Text angezeigt.
                                      5 Klicken Sie auf [OK], um die Bedingung zu übernehmen.
                                         Die Bezeichnung wird im Bereich Zusätzliche Bedingung angezeigt.
2.10 / 11-2018




                                      6 Klicken Sie auf [OK], um die Daten zu speichern.
                                         Um die Formel zu bearbeiten, müssen Sie in den Formel-Editor wechseln.



                 A+W Production Maschinenzuordnung                                                              D-65
                 Maschinenzuordnung                                                                     Tutorial




                                      Formel zur Bearbeitungsdauer einer logischen Ma-
                                      schine auswählen
                                      Sie können eine Formel zur Bearbeitungsdauer direkt in den Eigenschaften
                                      der logischen Maschinen auswählen. Die Formeln für eine Bedingung bear-
                                      beiten Sie im Formel-Editor.
                                      Alternativ dazu können Sie die Bearbeitungsdauer einer logischen Maschine
                                      kann auch in der A+W Production Kapazitätsplanung erstellten oder bearbei-
                                      ten.


                                       So wählen Sie eine Formel für die Bearbeitungsdauer aus
                                      1 Wählen Sie Stammdaten > MZO > MZO-Editor > Logische Maschinen.
                                      2 Markieren Sie die Logische Maschine und klicken Sie auf [Bearbeiten].




                                         A                                        B




                                         A Bearbeitungsdauer                B Formel-Auswahl
                                         Abb. D-34   Logische Maschine
2.10 / 11-2018




                 D-66                                                    A+W Production Maschinenzuordnung
                 Tutorial                                                                  Maschinenzuordnung




                                      3 Klicken Sie auf […] (B).




                                         Abb. D-35   Formel-Auswahl


                                      4 Wählen Sie im Dialog Formel-Auswahl eine Formel aus.
                                      5 Klicken Sie auf [OK], um die Formel in die Eigenschaften der Logische Ma-
                                        schine zu übernehmen.
                                         Die Formel wird in der Zeile Bearbeitungsdauer angezeigt.
                                      6 Klicken Sie auf [OK], um die Daten zu speichern.
                                         Sie können die Formel bearbeiten, indem Sie auf [Editieren] klicken. Zu
                                         den Formeln finden Sie eine ausführliche Beschreibung in der Dokumen-
                                         tation zum Part Formeln.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-67
                 Maschinenzuordnung                                                                       Tutorial




                                      Übungen zum Auswählen von Bedingungen
                                      Festigen Sie Ihr neu erworbenes Wissen mit den nachfolgenden Übungen.
                                      •   Notieren Sie sich, in welchen Dialogen in der Maschinenzuordnung Sie Be-
                                          dingungen auswählen können.
                                      •   Bilden Sie auf Papier den Maschinenpark Ihres Betriebes ab, mit den dazu
                                          gehörigen Maschinen, logischen Maschinen und Arbeitsgängen. Oder ver-
                                          wenden Sie bereits bestehende Notizen:
                                           “Übungen zu Maschinen” auf Seite D-32
                                           “Übungen zu logischen Maschinen” auf Seite D-39
                                           “Übungen zu Arbeitsgängen” auf Seite D-50
                                           “Übungen zur Arbeitsgangzuordnung” auf Seite D-62
                                          – Welche Bedingungen sind in Ihrem Maschinenpark und bei der aktuel-
                                            len Auftragssituation sinnvoll?
                                          – Welche Auswirkungen hätten die Bedingungen auf die jeweils anderen
                                            Bereiche der Maschinenzuordnung?


                                      Ergänzende Informationen
                                       Softwarereferenz, “Bedingung auswählen” auf Seite D-102
                                       Softwarereferenz, “Auswahl Bedingungen” auf Seite D-114
2.10 / 11-2018




                 D-68                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                                          Maschinenzuordnung




                                      Bearbeitungstypen und Bearbeitungs-
                                      artikel
                                      Lernziele

                                      • Was sind Bearbeitungstypen in A+W Production und speziell in der
                                        Maschinenzuordnung?
                                      • Wie werden Bearbeitungstypen angelegt, bearbeitet oder gelöscht?
                                      • Wann können Bearbeitungstypen nicht gelöscht werden?
                                      • Was sind Bearbeitungsartikel in A+W Production und speziell in der
                                        Maschinenzuordnung?
                                      • Wie werden Bearbeitungsartikel angelegt, bearbeitet oder gelöscht?


                                      Nutzen

                                      • Arbeitsgänge können auf Basis von Bearbeitungstypen oder Bearbeitungsartikeln
                                        definiert werden.
                                      • Ist einem Arbeitsgang ein Bearbeitungstyp hinterlegt, beschreibt dieser, um welche
                                        technische Form einer Bearbeitung es sich handelt, zum Beispiel Zuschnitt.
                                      • Ist ein Bearbeitungsartikel hinterlegt, beschreibt dieser, um welche technische
                                        Form der Bearbeitung es sich handelt, jedoch konkreter als beim Bearbeitungstyp.
                                        So wird mit einem Bearbeitungsartikel ein Arbeitsgang z. B. als Facetten-Schleifen
                                        definiert.


                                      Merke

                                      Bearbeitungstypen           Bearbeitungstypen beschreiben, um welche technische
                                                                  Form einer Bearbeitung es sich handelt.
                                                                  Bearbeitungstypen sind vom Anwender definierte
                                                                  Bearbeitungen. Demgegenüber gibt es noch den
                                                                  vordefinierten Katalog der A+W Software GmbH.

                                      Bearbeitungsartikel         Bearbeitungsartikel definieren konkreter als ein
                                                                  Bearbeitungstyp, um welche technische Form der
                                                                  Bearbeitung es sich handelt.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                   D-69
                 Maschinenzuordnung                                                                         Tutorial




                                      Bearbeitungstypen in der Maschinenzuordnung
                                      Mit einem Bearbeitungstyp wird beschrieben, um welche technische Form der
                                      Bearbeitung es sich handelt. So wird zum Beispiel definiert, ob es sich um Zu-
                                      schnitt, Montage, Säumen, Schleifen oder Verpacken handelt.
                                      Arbeitsgänge werden auf Basis von Bearbeitungstypen definiert. Der Arbeits-
                                      gang bringt dabei die Eigenschaften des Werkstücks mit den Eigenschaften
                                      des Bearbeitungstyps zusammen.



                                         Bearbeitungstyp
                                         Säumen


                                         Bearbeitungstyp
                                         Zuschnitt
                                                                                                  Arbeitsgang
                                                                  Neuer Arbeitsgang
                                                                                                  Zuschnitt
                                         Bearbeitungstyp
                                         Schleifen


                                         Bearbeitungstyp
                                         Polieren



                                      Abb. D-36   Bearbeitungstyp als Basis eines Arbeitsgangs


                                      Bearbeitungstypen sind von der A+W Software GmbH vordefiniert, können
                                      aber auch selbst definiert werden.
2.10 / 11-2018




                                      Abb. D-37   Bearbeitungstypen




                 D-70                                                      A+W Production Maschinenzuordnung
                 Tutorial                                                                        Maschinenzuordnung




                                      Bearbeitungsartikel in der Maschinenzuordnung
                                      Bearbeitungsartikel referenzieren auf Bearbeitungstypen. Mit Bearbeitungsar-
                                      tikeln können Sie Bearbeitungstypen genauer beschreiben. Sie können zum
                                      Beispiel zum Bearbeitungstyp Schleifen die Bearbeitungsartikel Facetten-
                                      Schleifen, Gehrungs-Schleifen, Kerben-Schleifen, Rodieren und Rundeck-
                                      Schleifen anlegen und so den jeweiligen technischen Vorgang genauer defi-
                                      nieren.
                                      Da die Bearbeitungsartikel auf den jeweiligen Bearbeitungstyp referenzieren,
                                      können Sie Änderungen zentral vornehmen. Ändern Sie z. B. beim Bearbei-
                                      tungstyp Schleifen die Einstellung Zählen von Bearbeitungen, ändert sich die-
                                      se Einstellung auch bei allen zugehörigen Bearbeitungsartikeln, z. B.
                                      Facetten-Schleifen, Gehrungs-Schleifen, Kerben-Schleifen, Rodieren und
                                      Rundeck-Schleifen.



                                         Bearbeitungsartikel
                                         Gehrung-Schleifen



                                         Bearbeitungsartikel
                                         Facetten-Schleifen
                                                                        Neuer                   Arbeitsgang
                                                                        Arbeitsgang             Facetten-Schleifen

                                         Bearbeitungsartikel
                                         Kerben-Schleifen



                                         Bearbeitungsartikel
                                         Rodieren



                                      Abb. D-38    Bearbeitungsartikel als Basis eines Arbeitsgangs


                                      In diesem Beispiel sehen Sie, wie Arbeitsgänge auf Basis von Bearbeitungs-
                                      artikeln definiert werden können. Der Arbeitsgang bringt dabei die Eigenschaf-
                                      ten des Werkstücks mit den Eigenschaften des Bearbeitungsartikels
                                      zusammen.
                                      Bearbeitungsartikel können Sie selbst definieren.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                                   D-71
                 Maschinenzuordnung                                                                Tutorial




                                      Abb. D-39   Bearbeitungsartikel
2.10 / 11-2018




                 D-72                                                   A+W Production Maschinenzuordnung
                 Tutorial                                                                          Maschinenzuordnung




                                      Bearbeitungstypen anlegen und verwalten
                                      In dieser Lerneinheit erfahren Sie, wie Sie Bearbeitungstypen anlegen, bear-
                                      beiten oder löschen.
                                      Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                       “So legen Sie einen Bearbeitungstyp an” auf Seite D-73
                                       “So bearbeiten Sie einen Bearbeitungstyp” auf Seite D-74
                                       “So löschen Sie einen Bearbeitungstyp” auf Seite D-75

                                          Standard-Katalog von Bearbeitungstypen
                                          In A+W Production gibt es einen Standard-Katalog von Bearbeitungstypen.
                                          Diese tragen vierstellige Nummern und dürfen vom Anwender nicht verän-
                                          dert oder gelöscht werden.
                                          Sie können weitere Bearbeitungstypen definieren. Es wird empfohlen, da-
                                          bei die jeweils passenden Bearbeitungstypen aus dem Standard-Katalog
                                          als Basis zu verwenden.


                                       So legen Sie einen Bearbeitungstyp an
                                      1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungstypen.

                                                                     B




                                      A




                                                                                                                C
2.10 / 11-2018




                                      A Bearbeitungstyp, der als Basis für den B Bearbeitung anlegen
                                        dient                                  C Bearbeitungsfelder
                                      Abb. D-40    Bearbeitungstyp anlegen.



                 A+W Production Maschinenzuordnung                                                              D-73
                 Maschinenzuordnung                                                                             Tutorial




                                            2 Markieren Sie den Bearbeitungstyp (A), der dem neuen Bearbeitungstyp
                                              als Basis dienen soll.
                                            3 Klicken Sie auf [Neu] (B).
                                               Die Eingabefelder (C) werden freigeschaltet.
                                            4 Geben Sie die Daten ein.
                                                Softwarereferenz, “Bearbeitungstypen” auf Seite D-123
                                            5 Klicken Sie auf [Speichern], um den neuen Bearbeitungstyp zu speichern.
                                               Damit haben Sie einen neuen Bearbeitungstyp definiert. Sie können ihn
                                               jetzt weiter bearbeiten.
                                               Wenn Sie auf [Verwerfen] klicken, wird der Vorgang abgebrochen, ohne die
                                               Daten zu speichern.


                                             So bearbeiten Sie einen Bearbeitungstyp
                                            1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungstypen.


                                   B




                 A




                                                                       J




                                                                                                                    C




                 A Bearbeitungstyp, der bearbeitet werden soll.       C Freigeschaltete Felder.
                 B Felder für Bearbeitung freischalten.
                 Abb. D-41    Bearbeitungstyp bearbeiten.


                                            2 Markieren Sie den Bearbeitungstyp, den Sie bearbeiten möchten (A).
2.10 / 11-2018




                 D-74                                                             A+W Production Maschinenzuordnung
                 Tutorial                                                                      Maschinenzuordnung




                                      3 Klicken Sie auf [Ändern] (B).
                                         Die Eingabefelder des Bearbeitungstyps werden freigeschaltet und kön-
                                         nen bearbeitet werden (C).
                                          Softwarereferenz, “Bearbeitungstypen” auf Seite D-123
                                      4 Geben Sie die Daten ein.
                                      5 Klicken Sie auf [Speichern], um die Änderungen zu speichern.


                                         Mit [Verwerfen] können Sie den Vorgang abbrechen, ohne die Daten zu
                                         speichern.


                                       So löschen Sie einen Bearbeitungstyp

                                         Voraussetzung
                                         Bearbeitungstypen können nicht gelöscht werden, wenn sie einem Bear-
                                         beitungsartikel zugeordnet sind. In diesem Fall erscheint eine Fehlermel-
                                         dung.
                                         Lösen Sie vor dem Löschen von Bearbeitungstypen die Zuordnung auf.

                                          “So lösen Sie die Zuordnung eines Bearbeitungstyps zu einem Bearbeitungsar-
                                           tikel auf” auf Seite D-79
                                      1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungstypen.
                                         Der Dialog Bearbeitungstypen wird geöffnet.
                                      2 Markieren Sie den Bearbeitungstyp, den Sie löschen möchten.
                                      3 Klicken Sie auf [Löschen].
                                         Es erscheint eine Sicherheitsabfrage.
                                      4 Klicken Sie auf [Yes], um den Bearbeitungstyp zu löschen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                              D-75
                 Maschinenzuordnung                                                                                   Tutorial




                                             Bearbeitungsartikel anlegen und verwalten
                                             In dieser Lerneinheit erfahren Sie, wie Sie Bearbeitungsartikel anlegen, bear-
                                             beiten oder löschen und wie Sie die Zuordnung eines Bearbeitungstyps zu ei-
                                             nem Bearbeitungsartikel auflösen.
                                             Zu diesem Thema gibt es folgende Handlungsanleitungen:
                                              “So legen Sie einen Bearbeitungsartikel an” auf Seite D-76
                                              “So bearbeiten Sie einen Bearbeitungsartikel” auf Seite D-78
                                              “So lösen Sie die Zuordnung eines Bearbeitungstyps zu einem Bearbeitungsartikel
                                               auf” auf Seite D-79
                                              “So löschen Sie einen Bearbeitungsartikel” auf Seite D-79


                                              So legen Sie einen Bearbeitungsartikel an
                                             1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungsartikel.


                                                   B




                 A




                                                                                                                           C




                 A Bearbeitungsartikel, der als Basis dient             B Bearbeitungsartikel anlegen
2.10 / 11-2018




                                                                        C Freigeschaltete Felder
                 Abb. D-42     Bearbeitungsartikel anlegen.




                 D-76                                                               A+W Production Maschinenzuordnung
                 Tutorial                                                                       Maschinenzuordnung




                                      2 Markieren Sie den Bearbeitungsartikel (A), der dem neuen Bearbeitungs-
                                        artikel als Basis dienen soll.
                                      3 Klicken Sie auf [Neu] (B).
                                         Die Eingabefelder (C) werden freigeschaltet und können bearbeitet wer-
                                         den.
                                      4 Geben Sie die Daten ein.
                                          Softwarereferenz, “Bearbeitungsartikel” auf Seite D-125
                                      5 Klicken Sie auf [Speichern], um den neuen Bearbeitungsartikel zu spei-
                                        chern.
                                         Damit haben Sie einen neuen Bearbeitungsartikel definiert. Sie können ihn
                                         jetzt weiter bearbeiten.
                                         Wenn Sie auf [Verwerfen] klicken, wird der Vorgang abgebrochen, ohne die
                                         Daten zu speichern.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                           D-77
                 Maschinenzuordnung                                                                             Tutorial




                                              So bearbeiten Sie einen Bearbeitungsartikel
                                             1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungsartikel.


                                     B




                 A




                                                                                                                     C




                 A Bearbeitungsartikel, der bearbeitet werden soll.     C Freigeschaltete Felder.
                 B Felder für Bearbeitung freischalten.
                 Abb. D-43     Bearbeitungsartikel anlegen.


                                             2 Markieren Sie den Bearbeitungsartikel (A), den Sie bearbeiten möchten.
                                             3 Klicken Sie auf [Ändern] (B).
                                                Die Eingabefelder (C) werden freigeschaltet und können bearbeitet wer-
                                                den.
                                                 Softwarereferenz, “Bearbeitungsartikel” auf Seite D-125
                                             4 Geben Sie die Daten ein.
                                             5 Klicken Sie auf [Speichern], um die Änderungen zu speichern.
2.10 / 11-2018




                                                Mit [Verwerfen] können Sie den Vorgang abbrechen, ohne die Daten zu
                                                speichern.


                 D-78                                                               A+W Production Maschinenzuordnung
                 Tutorial                                                                   Maschinenzuordnung




                                       So lösen Sie die Zuordnung eines Bearbeitungstyps zu einem
                                        Bearbeitungsartikel auf
                                      1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungsartikel.
                                         Der Dialog Bearbeitungsartikel wird geöffnet.
                                      2 Markieren Sie den Bearbeitungsartikel, dem Sie einen anderen Bearbei-
                                        tungstyp zuordnen möchten.
                                         Sie können die Liste der Bearbeitungsartikel nach Bearbeitungstyp ord-
                                         nen, um den jeweiligen Bearbeitungsartikel besser zu finden.
                                      3 Klicken Sie auf [Ändern].
                                         Die Eingabefelder des Bearbeitungsartikels werden freigeschaltet und
                                         können bearbeitet werden.
                                      4 Wählen Sie in der Kombobox Bearbeitungstyp einen anderen Bearbei-
                                        tungstyp.
                                      5 Klicken Sie auf [Speichern], um den Bearbeitungsartikel zu speichern.


                                         Mit [Verwerfen] können Sie den Vorgang abbrechen, ohne die Daten zu
                                         speichern.


                                       So löschen Sie einen Bearbeitungsartikel
                                      1 Wählen Sie Stammdaten > Bearbeitungen > Bearbeitungsartikel.
                                         Der Dialog Bearbeitungsartikel wird geöffnet.
                                      2 Markieren Sie den Bearbeitungsartikel, den Sie löschen möchten.
                                      3 Klicken Sie [Löschen].
                                         Es erscheint eine Sicherheitsabfrage.
                                      4 Klicken Sie auf [Yes], um den Bearbeitungsartikel zu löschen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-79
                 Maschinenzuordnung                                                                      Tutorial




                                      Übungen zur Maschinenzuordnung
                                      Festigen Sie mit den folgenden Übungen Ihr neu erworbenes Wissen.
                                      Legen Sie folgende Stammdaten an:
                                      •   Definieren Sie eine Übungsmaschine Bohren. Geben Sie der Bohrmaschi-
                                          ne folgende Restriktionen:
                                          – Die Bohrmaschine kann nur Scheiben ab einer Dicke von 10 mm und
                                              bis zu einer Dicke von 20 mm bearbeiten.
                                          – Die Maschine kann keine Modelle bearbeiten.
                                          – Die Maschine kann unstrukturierte und strukturierte Scheiben bearbei-
                                              ten.
                                      •   Definieren Sie eine Übungsmaschine Linie. Geben Sie der Linie folgende
                                          Restriktionen:
                                          – Die Maschine kann Stufen-ISO und Normal-ISO bearbeiten.
                                          – Die minimalen Scheibenabmessungen betragen 200 x 300 mm.
                                          – Die maximalen Scheibenabmessungen betragen 2500 x4000 mm.
                                          – Die Maschine kann 3-fach-ISO ohne maßliche Restriktion bearbeiten.
                                          – Fügen Sie eine zusätzliche Bedingung ein. Welche Auswirkungen kann
                                              eine zusätzliche Bedingung auf die Maschine haben?
                                      •   Definieren Sie eine Übungsmaschine CNC-Center.
                                      •   Zum CNC-Center soll es zwei logische Maschinen für die Bearbeitungen
                                          Bohren und Polieren geben.
                                      •   Definieren Sie einen Übungs-Schneidtisch, bei dem die Scheiben im Hoch-
                                          format auf der Maschine stehen.
                                      •   Definieren Sie einen Übungsarbeitsgang Bohren.
                                      •   Weisen Sie dem Arbeitsgang die Bohrmaschine und das CNC-Center zu.
                                          Die Bohrmaschine soll dabei höchste Priorität haben.
                                      •   Definieren Sie einen Übungsarbeitsgang Bohren auf CNC-Center, dem Sie
                                          das CNC-Center mit höchster Priorität zuweisen. Die Bohrmaschine wei-
                                          sen Sie dem Arbeitsgang mit geringer Priorität für Engpässe zu.
                                      •   Definieren Sie einen Übungsarbeitsgang, der auf einem Bearbeitungsarti-
                                          kel basiert.
                                      •   Definieren Sie einen eigenen Übungsbearbeitungstyp Bohren.
                                      •   Ändern Sie die Arbeitsgänge aus der Übung so, dass diese auf Ihrem ei-
                                          genen Übungsbearbeitungstyp Bohren basieren.


                                      Ergänzende Informationen
                                       “Maschinen” auf Seite D-15
                                       “Logische Maschinen” auf Seite D-33
                                       “Arbeitsgänge” auf Seite D-40
                                       “Arbeitsgangzuordnung” auf Seite D-51
                                       “Bedingungen, Formeln, Restriktionen” auf Seite D-63
                                       “Bearbeitungstypen und Bearbeitungsartikel” auf Seite D-69
2.10 / 11-2018




                 D-80                                                       A+W Production Maschinenzuordnung
                 Tutorial                                                   Schaltflächen in der Maschinenzuordnung




                                      Schaltflächen in der Maschi-
                                      nenzuordnung
                                      Schaltfläche   Bedeutung

                                                     Stammdaten definieren.


                                                     Eintrag aus der Liste bearbeiten.


                                                     Eintrag aus der Liste bearbeiten.


                                                     Eintrag aus der Liste löschen.


                                                     Änderungen übernehmen.


                                                     Daten speichern.

                                                     Dialog schließen, ohne Änderungen zu übernehmen.


                                                     Elemente in einer Liste nach oben oder unten verschieben.

                                                     Elemente einander zuordnen, Elemente trennen.

                                                     Restriktionen für eine Maschine definieren, definierte Restriktionen
                                                     löschen.

                                                     Zusätzliche Restriktion auswählen.

                                                     Restriktion löschen.


                                                     Änderungen übernehmen.


                                                     Änderungen nicht übernehmen.


                                                     Eine UND-Verknüpfung wird im Grafik-Editor eingefügt.


                                                     Eine ODER-Verknüpfung wird im Grafik-Editor eingefügt.


                                                     Eine markierte Verknüpfung im Grafik-Editor löschen.


                                                     Öffnet einen Dialog, um Spalten im Fenster anzupassen.
2.10 / 11-2018




                                                     Änderungen zurücksetzen.




                 A+W Production Maschinenzuordnung                                                                   D-81
                 Schaltflächen in der Maschinenzuordnung                              Tutorial
2.10 / 11-2018




                 D-82                                      A+W Production Maschinenzuordnung
Maschinenzuordnung            D

                 Softwarereferenz




              A+W Production
                 Softwarereferenz                                                          Maschinenzuordnung




                                      Maschinenzuordnung
                                      In der Maschinenzuordnung (MZO) ist der vorhandene Maschinenpark den
                                      Arbeitsgängen zugewiesen. Dabei werden Maschinenrestriktionen und Vorga-
                                      ben zur Produktionssteigerung berücksichtigt. Es können auch Prüfprogram-
                                      me von Maschinenherstellern eingebunden werden, um die Plausibilität der
                                      Zuordnung zu prüfen.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “MZO-Editor” auf Seite D-86
                                      •   “Neue Maschine” auf Seite D-94
                                      •   “Maschine” auf Seite D-95
                                      •   “Abmessungsrestriktionen” auf Seite D-100
                                      •   “SZR Restriktionen” auf Seite D-101
                                      •   “Bedingung auswählen” auf Seite D-102
                                      •   “Neue logische Maschine” auf Seite D-103
                                      •   “Logische Maschine” auf Seite D-104
                                      •   “Formel-Auswahl” auf Seite D-106
                                      •   “Neuer Arbeitsgang” auf Seite D-107
                                      •   “Arbeitsgang” auf Seite D-108
                                      •   “Neuer Maschinentyp” auf Seite D-110
                                      •   “Maschinentyp” auf Seite D-111
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                       D-85
                 Maschinenzuordnung                                                            Softwarereferenz




                                      MZO-Editor
                                      Stammdaten > MZO > MZO-Editor.
                                      Mit dem MZO-Editor definieren und verwalten Sie Maschinen, logische Ma-
                                      schinen und Arbeitsgänge. Außerdem legen Sie fest, welche Maschinen dem
                                      jeweiligen Arbeitsgang zugeordnet sind.
                                      Im MZO-Editor finden Sie folgende Register:
                                      •   “MZO-Editor – Maschinen” auf Seite D-87
                                      •   “MZO-Editor – Logische Maschinen” auf Seite D-88
                                      •   “MZO-Editor – Arbeitsgänge” auf Seite D-90
                                      •   “MZO-Editor – Arbeitsgangzuordnung” auf Seite D-91
                                      •   “MZO-Editor – Maschinentypen” auf Seite D-92
2.10 / 11-2018




                 D-86                                                    A+W Production Maschinenzuordnung
                 Softwarereferenz                                                               Maschinenzuordnung




                                      MZO-Editor – Maschinen
                                      Stammdaten > MZO > MZO-Editor > Maschinen.




                                      Abb. D-44    MZO-Editor – Maschinen


                                      In diesem Register legen Sie neue Maschinen an und bearbeiten oder löschen
                                      bereits bestehende.
                                       Tutorial, “Maschinen anlegen und verwalten” auf Seite D-22
                                       “Maschine” auf Seite D-95

                                      ID Frei wählbare Identifikationsnummer.

                                      Name Name der Maschine.

                                      Typ Maschinentyp, der der Maschine zugewiesen wurde. Maschinentypen
                                      können z. B. Zuschnitt, Kantenbearbeitung oder Bieger sein.

                                         Maschinentypen
                                         Der Katalog der Maschinentypen ist in A+W Production fest vorgegeben.
                                         Er steht in der Kombobox zur Verfügung, wenn eine neue Maschine ange-
                                         legt wird.
                                         Für Änderungen am Katalog der Maschinentypen wenden Sie sich bitte an
                                         den Support der A+W Software GmbH.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                           D-87
                 Maschinenzuordnung                                                             Softwarereferenz




                                      Erfassungsstelle Erfassungsstelle, der die Maschine zugeordnet ist. Die Er-
                                      fassungsstelle wird sowohl für die Kapazitätsplanung, als auch für die Be-
                                      triebsdatenerfassung benötigt.

                                      Komponenten-ID Frei wählbare Komponenten-Identifikation. Wird nur bei
                                      den Maschinentypen Linien, Tische und Bieger verwendet.

                                         Maschinen löschen
                                         A+W Production legt zu jeder Maschine automatisch eine logische Maschi-
                                         ne an. Darüber hinaus können weitere logische Maschinen definiert wer-
                                         den.
                                         Wird eine Maschine gelöscht, werden damit auch automatisch alle zuge-
                                         hörigen logischen Maschinen gelöscht.
                                         Achtung: Wenn Maschinen gelöscht werden, kann dadurch die laufende
                                         Produktion gestoppt werden.


                                      MZO-Editor – Logische Maschinen
                                      Stammdaten > MZO > MZO-Editor > Logische Maschinen.




                                      Abb. D-45   MZO-Editor – Logische Maschinen


                                      In diesem Register legen Sie logische Maschinen an und bearbeiten oder lö-
                                      schen logische Maschinen.
2.10 / 11-2018




                                      A+W Production legt automatisch zu jeder Maschine auch eine logische Ma-
                                      schine an. Darüber hinaus können zu jeder Maschine beliebig viele logische
                                      Maschinen angelegt werden.


                 D-88                                                     A+W Production Maschinenzuordnung
                 Softwarereferenz                                                               Maschinenzuordnung




                                      Logische Maschinen bilden genau eine Funktion einer Maschine ab. Handelt
                                      es sich zum Beispiel um ein CNC-Center, das bohren, schleifen und polieren
                                      kann, legen Sie drei logische Maschinen an: Eine für die Bearbeitung Bohren,
                                      eine für die Bearbeitung Schleifen und eine für die Bearbeitung Polieren.
                                      Die automatisch angelegte logische Maschine kann nicht manuell gelöscht
                                      werden. Zusätzlich definierte logische Maschinen können gelöscht werden.
                                      Wird die Maschine aus der Liste Maschinen gelöscht, werden alle zugehöri-
                                      gen logischen Maschinen gelöscht.
                                       Tutorial, “Logische Maschinen anlegen und verwalten” auf Seite D-36
                                       “Logische Maschine” auf Seite D-104

                                      [Neu] Öffnet den Dialog Neue logische Maschine, mit dem eine weitere logi-
                                      sche Maschine des Typs definiert werden kann, zu dem die markierte logische
                                      Maschine gehört. Die Schaltfläche [Neu] ist nur freigeschaltet, wenn eine logi-
                                      sche Maschine in der Liste markiert ist.
                                       “Neue logische Maschine” auf Seite D-103

                                      ID ID der Maschine.

                                      Maschine Name der Maschine, deren Stammdaten für diese logische Ma-
                                      schine gewählt wurden.

                                      ID Frei wählbare Identifikationsnummer der logischen Maschine.

                                      Name Frei wählbarer Name für die logische Maschine.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                             D-89
                 Maschinenzuordnung                                                                     Softwarereferenz




                                      MZO-Editor – Arbeitsgänge
                                      Stammdaten > MZO > MZO-Editor > Arbeitsgänge.




                                      Abb. D-46    MZO-Editor – Arbeitsgänge


                                      In diesem Register legen Sie Arbeitsgänge an und bearbeiten oder löschen
                                      bestehende Arbeitsgänge.
                                      Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logische
                                      Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logische Ma-
                                      schine zu. Ist die zugehörige logische Maschine noch nicht definiert, sollte
                                      temporär die logische Maschine Dummy zugeordnet werden.
                                       Tutorial, “Arbeitsgänge anlegen und verwalten” auf Seite D-48
                                       “Arbeitsgang” auf Seite D-108

                                      ID Frei wählbare Identifikationsnummer des Arbeitsgangs.

                                      Name Name des Arbeitsgangs.

                                      Zusätzliche Bedingung Bedingung, die dem Arbeitsgang zugewiesen ist.

                                      [Priorität] Arbeitsgänge in der Liste nach oben oder unten verschieben. Je
                                      höher ein Arbeitsgang in der Liste steht, desto höher ist seine Priorität bei der
2.10 / 11-2018




                                      Maschinenzuordnung. Anhand der Priorität legt A+W Production fest, wel-
                                      cher Arbeitsgang aus wirtschaftlichen Gründen vorrangig gewählt wird.




                 D-90                                                        A+W Production Maschinenzuordnung
                 Softwarereferenz                                                             Maschinenzuordnung




                                         Arbeitsgänge löschen
                                         Arbeitsgänge können nur aus der Liste gelöscht werden, wenn ihnen keine
                                         logische Maschine zugeordnet ist.
                                         Soll ein Arbeitsgang gelöscht werden, muss zuerst die Zuordnung der Ma-
                                         schinen gelöscht werden.


                                      MZO-Editor – Arbeitsgangzuordnung
                                      Stammdaten > MZO > MZO-Editor > Arbeitsgangzuordnung.




                                      Abb. D-47    MZO-Editor – Arbeitsgangzuordnung


                                      In diesem Register ordnen Sie die logischen Maschinen den Arbeitsgängen
                                      zu.
                                       Tutorial, “Arbeitsgangzuordnung” auf Seite D-51
                                       “Arbeitsgang” auf Seite D-108

                                      Arbeitsgänge Liste der definierten Arbeitsgänge.

                                      Maschinen Liste der definierten logischen Maschinen.

                                      [Priorität] Logische Maschinen in der Liste nach oben oder unten verschie-
                                      ben. Je höher eine Maschine in der Liste steht, desto höher ist ihre Priorität
2.10 / 11-2018




                                      bei der Maschinenzuordnung. Logische Maschinen mit hoher Priorität wählt
                                      A+W Production aus wirtschaftlichen Gründen vorrangig.




                 A+W Production Maschinenzuordnung                                                             D-91
                 Maschinenzuordnung                                                                  Softwarereferenz




                                      [Zuordnung] Sie ordnen Maschinen den Arbeitsgängen zu, indem Sie eine
                                      Maschine und einen Arbeitsgang markieren und auf den Pfeil nach links kli-
                                      cken. Sie machen eine Zuordnung rückgängig, indem Sie eine Maschine in
                                      der Liste Arbeitsgänge markieren und auf den Pfeil nach rechts klicken.
                                       Tutorial, “Schaltflächen in der Maschinenzuordnung” auf Seite D-81
                                      Mit der Schaltfläche [+] eines Arbeitsgangs können Sie alle zugeordneten lo-
                                      gischen Maschinen anzeigen.
                                      Mit der Checkbox [Alles aufklappen] zeigen Sie in der Liste Arbeitsgänge alle
                                      zugeordneten logischen Maschinen an.
                                      Die einem Arbeitsgang zugeordneten logischen Maschinen werden in der Lis-
                                      te grau hinterlegt, wenn Sie den Arbeitsgang markieren.

                                         Arbeitsgänge in roter Schrift
                                         Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logi-
                                         sche Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logi-
                                         sche Maschine zu. Ist die zugehörige logische Maschine noch nicht
                                         definiert, sollte temporär die logische Maschine Dummy zugeordnet wer-
                                         den.


                                      MZO-Editor – Maschinentypen
                                      Stammdaten > MZO > MZO-Editor > Maschinentypen.
2.10 / 11-2018




                                      Abb. D-48    MZO-Editor – Maschinentypen




                 D-92                                                        A+W Production Maschinenzuordnung
                 Softwarereferenz                                                            Maschinenzuordnung




                                      In diesem Register verwalten Sie die Maschinentypen. Maschinentypen wer-
                                      den u. a. eingesetzt, um Beschaffungsarten von einander zu trennen und um
                                      Lose zu bilden.
                                      Die systeminternen Maschinentypen haben die IDs bis 1000 und werden kur-
                                      siv angezeigt. Sie können nicht bearbeitet werden.
                                       “Maschinentyp” auf Seite D-111
                                      Übersicht
                                      Folgende Spalten werden angezeigt:
                                      •   ID:
                                          ID des Maschinentyps.
                                      •   Exklusiv:
                                          Anzeige, ob der Maschinentyp exklusiv zugewiesen ist. Standardeinstel-
                                          lung für systeminternen Maschinentypen: Nein.
                                      •   Pflicht:
                                          Anzeige, ob die Zuordnung vorgeschrieben ist. Standardeinstellung für
                                          systeminternen Maschinentypen: Ja.
                                      •   Implizit:
                                          Anzeige, ob der Maschinentyp implizit zugewiesen ist. Standardeinstellung
                                          für systeminternen Maschinentypen: Ja Ausnahme der Eintrag Sonstiges .
                                      •   Typenname:
                                          Anzeige des Typennamens.
                                      •   Tabellenbezug:
                                          Angabe der relevanten Datenbanktabelle.
                                      Benutzerdefinierte Maschinentypen haben ihre Bedeutung verloren. Sie wur-
                                      den durch A+W Bearbeitungstypen abgelöst
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                           D-93
                 Maschinenzuordnung                                                                 Softwarereferenz




                                      Neue Maschine
                                      Stammdaten > MZO > MZO-Editor > Maschinen > Neu.




                                      Abb. D-49     Neue Maschine


                                      In diesem Dialog geben Sie die Stammdaten für die neue Maschine ein und
                                      legen damit eine neue Maschine an.
                                       “Maschine” auf Seite D-95

                                      ID Frei wählbare Identifikationsnummer.

                                      Name Name der Maschine.

                                      Maschinentyp Maschinentyp, zum Beispiel Zuschnitt, Kantenbearbeitung,
                                      oder Bieger.

                                      Komponenten-ID Frei wählbare Identifikationsnummer der Maschine. Die
                                      Komponenten-ID wird nur bei den Maschinentypen Linien, Tische und Bieger
                                      verwendet.

                                         Beispiel

                                         Mit der Komponenten-ID kann zwischen Linien, Tischen oder Biegern
                                         unterschieden werden, wenn es mehrere des gleichen Typs gibt.
                                         So könnten zum Beispiel die Tische 1, 2 und 3 die Komponenten-IDs TB1,
                                         TB2 und TB3 bekommen.
2.10 / 11-2018




                 D-94                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                               Maschinenzuordnung




                                      Maschine
                                      Stammdaten > MZO > MZO-Editor > Maschinen > Bearbeiten.




                                      Abb. D-50    Maschine


                                      In diesem Dialog bearbeiten Sie die Stammdaten der Maschine.
                                       Tutorial, “Maschinen anlegen und verwalten” auf Seite D-22

                                      Maschine Name der gewählten Maschine.

                                      Allgemeine Eigenschaften der Maschine Stammdaten der Maschine.
                                      Wenn Sie ein Feld unter Eigenschaften der Maschine markieren, wird im Feld
                                      darunter eine Kurzbeschreibung angezeigt.
                                      • ID:
                                         Identifikationsnummer, die Sie der Maschine beim Definieren zugewiesen
                                         haben.
                                      • Name:
                                         Bezeichnung, die Sie der Maschine zugewiesen haben.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                           D-95
                 Maschinenzuordnung                                                                 Softwarereferenz




                                      •   Erfassungsstelle:
                                          In der Kombobox weisen Sie der Maschine eine Erfassungsstelle zu. Diese
                                          Nummer wird von A+W verwendet, um bei abweichenden Maschinennum-
                                          mern die Zuordnung zu erleichtern. Sie wird ebenfalls für die Einrichtung
                                          der BDE verwendet.
                                      •   Überlastungsgrenze pro Schicht:
                                          Dieser Wert bezieht sich in % auf die Kapazität der entsprechenden
                                          Schicht.
                                      •   Überlastungsgrenze für einen Zeitraum:
                                          Dieser Wert bezieht sich in % auf die Kapazität für einen festgelegten Zeit-
                                          raum, z. B. eine Woche.
                                      •   Tage:
                                          Legt die Dauer in Tagen fest, die der Überlastungsgrenze für einen Zeit-
                                          raum zu Grunde liegt.
                                      •   Engpass:
                                          Angabe, ob die Maschine eine kapazitätslimitierende Stelle in der Produk-
                                          tion ist.
                                      •   Anzeigeart:
                                          Angabe, welche Einheit bei der Maschine verwendet wird, z. B. Stückzahl,
                                          geplante Stückzahl, Quadratmeter, Gewicht, usw.
                                      •   Lastverteilung prüfen:
                                          Angabe, ob zugewiesene logische Maschinen von A+W Capacity Planner
                                          geprüft werden.
                                      •   Maschinengruppe:
                                          Angabe, welcher Maschinengruppe in A+W Capacity Planner die Maschi-
                                          ne zugeordnet ist.
                                      •   Standort:
                                          Standort der Maschine.
                                      •   Kostenstelle:
                                          Kostenstelle, zu der die Maschine zählt.
                                      •   Automatische Umlastung:
                                          Angabe, ob von A+W Capacity Planner automatisch auf die Maschine um-
                                          gelastet werden darf.
                                      •   Bearbeitungsketten:
                                          Angabe, ob Bearbeitungsketten durch A+W Capacity Planner auf der Ma-
                                          schine möglich sind. Mit Bearbeitungsketten auf einer Maschine lassen
                                          sich aufeinanderfolgende Bearbeitungen zusammenfassen, sofern die Ma-
                                          schinenalternativen dieselben sind. Diese Einstellung darf nicht bei Sieb-
                                          druck gesetzt werden.
                                      •   Alternativ-Maschine:
                                          Angabe, ob die Maschine von A+W Capacity Planner als alternative Ma-
                                          schine verwendet werden darf.

                                      Weitere Eigenschaften der Maschine Dieser Abschnitt wird nur für Ma-
                                      schinen angezeigt, die zu den Maschinentypen Zuschnitt, Rahmenbieger,
                                      ISO-Linie und Gießharz gehören.
                                      • Name:
2.10 / 11-2018




                                         Name der Maschine.
                                      • Maschinencode-Format:
                                         Format in dem der Maschinencode übergeben wird.



                 D-96                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                                    Maschinenzuordnung




                                      •  Aufrufsektion:
                                         Auswahl des zugewiesenen Treiberaufrufs. Damit können Sie Maschinen
                                         desselben Typs unterschiedliche konfigurieren und jeweils eine Aufrufsek-
                                         tion zuordnen. Die Einstellung 0 entspricht der Sektion 1.
                                      • Linien-ID:
                                         ID der Produktionslinie.
                                      Für Zuschnitt können Sie folgende Eigenschaften definieren:




                                      X-, Y-, Z- und W-Schnitte

                                      y-Achse
                                      (kartesisches Koordinatensystem)


                                                                                Y
                                                                                                     X



                                                                                                     Z
                                             3210 mm




                                                              W




                                      Nullpunkt 0                         6000 mm
                                                                                                               x-Achse
                                                                                      (kartesisches Koordinatensystem)
2.10 / 11-2018




                                      Abb. D-51        X-, Y-, Z- und W-Schnitte in A+W Production




                 A+W Production Maschinenzuordnung                                                                  D-97
                 Maschinenzuordnung                                                                  Softwarereferenz




                                      Bei Schneidtischen wird zwischen X-, Y-, Z- und W-Schnitten unterschieden,
                                      wie in der Abbildung oben zu sehen ist. Die Richtungen X und Y scheinen in
                                      A+W Production zunächst um 90° verdreht im Vergleich zum üblichen
                                      Koordinatensystem.
                                      •   Die Definition in A+W Production für X- und Y-Schnitte lautet: Der Schnitt
                                          wird an einem X- bzw. Y-Wert, bezogen auf das kartesische Koordinaten-
                                          system, ausgeführt.
                                          Damit steht der Schnitt in A+W Production senkrecht zum kartesischen
                                          Koordinatensystem.
                                          Beispiel für den Zuschnitt einer Scheibe:
                                          Die Scheibe soll auf die Maße 5000 x 2500 mm geschnitten werden. Sie
                                          geben in A+W Production ein X = 5000 mm und Y = 2500 mm. Der
                                          Schneidtisch führt dann am X-Wert 5000 mm einen senkrechten und am Y-
                                          Wert 2500 mm einen waagrechten Schnitt aus.
                                      •   W- und Z-Schnitte: Sie entsprechen in den Richtungen den X- und Y-
                                          Schnitten, sind jedoch kleiner und damit aufwendiger. Um Z-Schnitte
                                          durchzuführen, muss das Glas am Schneidtisch gedreht werden, um es zu
                                          brechen. Das ist zeitaufwendig und teuer. Ab einem definierten Aufwand
                                          werden Schnitte als W- und Z-Schnitte benannt.
                                      A+W Production versucht, W- und Z-Schnitte zu vermeiden. Wie stark die Ver-
                                      meidung von W- und Z-Schnitten gewertet werden soll, können Sie beim Be-
                                      arbeiten von Schneidtischen mit der Variablen Kosten pro Z-Schnitt angeben.
                                      Dieser Kostenfaktor dient auch bei der Optimierung des Schneidplans.

                                      Feldbeschreibung anzeigen Sie können sich Feldbeschreibungen zur mar-
                                      kierten Eigenschaft anzeigen lassen:
                                      ☐ Die Feldbeschreibung wird nicht angezeigt.
                                      ☑ Öffnet den Dialog Feldbeschreibung (Datenbankfeld). Im Titel des Dialogs
                                      wird der Name des Datenbankfelds angezeigt.

                                      Restriktionen Maschinenresriktionen zeigen die physikalischen Grenzen ei-
                                      ner Maschine auf, die nicht überwunden werden können.
                                      Mit der Wahl der Checkboxen legen Sie fest, welche Restriktionen für die Ma-
                                      schine gelten:
                                      •   minimale Dicke
                                      •   maximale Dicke
                                      •   Modelle
                                      •   Beschichtete Gläser
                                      •   Strukturgläser
                                      •   Stufen ISO
                                       Tutorial, “Restriktionen von Maschinen anlegen und bearbeiten” auf Seite D-26

                                          Maschinenrestriktionen und logische Maschinen
                                          Wenn die Restriktionen einer Maschine durch Umbau oder Umrüsten über-
                                          wunden werden können, sollten Sie für alle Anwendungsfälle jeweils eine
                                          Logische Maschine anlegen.
2.10 / 11-2018




                 D-98                                                        A+W Production Maschinenzuordnung
                 Softwarereferenz                                                               Maschinenzuordnung




                                      Abmessungen Mit Abmessungsrestriktionen legen Sie fest, ob eine Maschi-
                                      ne nur Bauteile einer minimalen oder maximalen Größe bearbeiten kann, zum
                                      Beispiel Scheiben ab einer Breite von 100 mm.
                                      Mit der Schaltfläche [Edit] öffnen Sie den Dialog Abmessungsrestriktionen, um
                                      Restriktionen für die Abmessungen zu definieren.
                                       “Abmessungsrestriktionen” auf Seite D-100
                                      Wenn Sie Abmessungsrestriktionen definiert haben, werden diese im Feld Ab-
                                      messungen angezeigt.

                                      SZR Mit SZR-Restriktionen definieren Sie, welche SZR von der Maschine be-
                                      arbeitet werden können, zum Beispiel SZR ab 16 mm und bis maximal 24 mm.
                                      Mit der Schaltfläche [Stift] öffnen Sie den Dialog SZR Restriktionen, um Rest-
                                      riktionen für den Scheibenzwischenraum zu definieren.
                                       Softwarereferenz, “SZR Restriktionen” auf Seite D-101
                                      Wenn Sie SZR-Restriktionen definiert haben, werden diese im Feld SZR an-
                                      gezeigt.

                                      Zusätzliche Bedingung Auswahl einer zusätzlichen Bedingung, die mit dem
                                      Formel-Editor definiert wurde.
                                      Mit der Schaltfläche [Lupe] öffnen Sie den Dialog Bedingung auswählen, um
                                      zusätzliche Bedingungen auszuwählen.
                                       “Bedingung auswählen” auf Seite D-102
                                      Wenn Sie eine zusätzliche Bedingung ausgewählt haben, wird die Bezeich-
                                      nung im Feld Zusätzliche Bedingung angezeigt.

                                         Zusätzliche Bedingungen
                                         Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaf-
                                         ten von Maschinen unter Umständen massiv.
                                         Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche
                                         Auswirkungen diese hat.
                                         Eine zusätzliche Bedingung könnte zum Beispiel alle Eigenschaften einer
                                         Maschine invertieren.

                                      Informationen zum Thema Formeln und Restriktionen in A+W Production fin-
                                      den Sie im Part Formel-Editor.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                            D-99
                 Maschinenzuordnung                                                                  Softwarereferenz




                                      Abmessungsrestriktionen
                                      Stammdaten > MZO > MZO-Editor > Maschinen > Bearbeiten > Eigenschaft
                                      markieren > [Bearbeiten].




                                      Abb. D-52    Abmessungsrestriktionen


                                      In diesem Dialog legen Sie die Restriktionen für die Abmessungen fest. Sie
                                      definieren somit, ob zum Beispiel nur Scheiben ab einer bestimmten Größe
                                      oder bis zu einer bestimmten Größe bearbeitet werden können.
                                       Tutorial, “Maschinen anlegen und verwalten” auf Seite D-22

                                      Name der Maschine
                                      Der Name wird aus den Eigenschaften der Maschine übernommen.

                                      Min. Breite, Min. Höhe Angabe der kleinsten Breite und/oder Höhe, die auf
                                      der Maschine gearbeitet werden kann.

                                      Max. Breite, Max. Höhe Angabe der größten Breite und/oder Höhe, die auf
                                      der Maschine gearbeitet werden kann.
2.10 / 11-2018




                 D-100                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                               Maschinenzuordnung




                                      SZR Restriktionen
                                      Stammdaten > MZO > MZO-Editor > Maschinen > Bearbeiten > SZR> [Bear-
                                      beiten].




                                      Abb. D-53    SZR Restriktionen


                                      In diesem Dialog legen Sie Restriktionen für den Scheibenzwischenraum
                                      (SZR) fest.
                                       Tutorial, “Maschinen anlegen und verwalten” auf Seite D-22

                                      Name der Maschine
                                      Der Name wird aus den Eigenschaften der Maschine übernommen.

                                      Min. SZR 1, Min. SZR 2 Angabe der kleinsten Breite, die auf der Maschine
                                      gearbeitet werden kann.

                                      Max. SZR 1, Max. SZR 2 Angabe der größten Breite, die auf der Maschine
                                      gearbeitet werden kann.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-101
                 Maschinenzuordnung                                                                      Softwarereferenz




                                      Bedingung auswählen
                                      Stammdaten > MZO > MZO-Editor > Maschine, Logische Maschinen, Arbeits-
                                      gänge > Bearbeiten > [Lupe].




                                      Abb. D-54    Bedingung auswählen


                                      In diesem Dialog wählen Sie Bedingungen für eine Maschine, logische Ma-
                                      schine oder einen Arbeitsgang aus und ordnen sie damit der jeweiligen Ma-
                                      schine, logische Maschine oder dem Arbeitsgang zu.
                                      Die zusätzlichen Bedingungen werden mit dem Formel-Editor definiert und
                                      bearbeitet. Damit können Sie Restriktionen von Maschinen, logischen Maschi-
                                      nen und Arbeitsgängen exakt definieren, z. B. durch eine komplexe Formel.
                                       Tutorial, “Bedingungen, Formeln, Restriktionen” auf Seite D-63

                                          Zusätzliche Bedingungen
                                          Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaf-
                                          ten von Maschinen unter Umständen massiv.
                                          Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche
                                          Auswirkungen diese hat.
                                          Eine zusätzliche Bedingung könnte zum Beispiel alle Eigenschaften einer
                                          Maschine invertieren.

                                      Informationen zum Thema Formeln und Restriktionen in A+W Production fin-
                                      den Sie im Handbuch für den Part Formel-Editor.

                                      Liste
                                      •   ID:
                                          Identifikationsnummer, die der Bedingung gegeben wurde.
                                      •   Bedingung:
                                          Bezeichnung, die der Bedingung gegeben wurde.
2.10 / 11-2018




                                      Beschreibung Beschreibung, die der Bedingung beigefügt wurde.



                 D-102                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                             Maschinenzuordnung




                                      Sprache Auswahl der Sprache, in der die Beschreibung angezeigt wird.

                                      Text Anzeige der Formel. Wurde die gewählte Formel im Formel-Editor
                                      (Text-Variante) auf Basis einer vorhandenen Formel definiert, steht hier der
                                      Name der ursprünglichen Formel.

                                      Nur eigene Sie können die Anzeige der Formeln einschränken.
                                      ☐ Alle Bedingungen werden gelistet.
                                      ☑ Nur benutzerdefinierte Bedingungen werden gelistet.

                                      ID Angabe der ID oder eines Teils der ID, auf die Sie die Liste einschränken
                                      wollen.

                                      Text Angabe des Bedingungsnamens oder eines Teils des Namens, auf die
                                      Sie die Liste einschränken wollen.


                                      Neue logische Maschine
                                      Stammdaten > MZO > MZO-Editor > Logische Maschinen > Neu.




                                      Abb. D-55    Neue logische Maschine


                                      In diesem Dialog geben Sie die Stammdaten für die neue Maschine, um eine
                                      neue logische Maschine anzulegen.
                                       “Logische Maschine” auf Seite D-104

                                      Maschine Anzeige von ID und Name der Maschine, zu der die logische Ma-
                                      schine gehört.

                                      ID Frei wählbare ID der logischen Maschine.

                                      Name Frei wählbarer Name der logischen Maschine.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                           D-103
                 Maschinenzuordnung                                                             Softwarereferenz




                                      Logische Maschine
                                      Stammdaten > MZO > MZO-Editor > Logische Maschinen > Bearbeiten.




                                      Abb. D-56    Logische Maschine


                                      In diesem Dialog definieren Sie die Stammdaten der logischen Maschine.
                                       Tutorial, “Logische Maschinen” auf Seite D-33

                                      Allgemeine Eigenschaften der logischen Maschine Stammdaten der logi-
                                      schen Maschine. Wenn Sie ein Feld markieren, wird im Feld darunter eine
                                      Kurzbeschreibung angezeigt.
                                      • ID:
                                         Identifikationsnummer, die Sie der logischen Maschine zugeordnet haben.
                                      • Name:
                                         Bezeichnung, die Sie der logischen Maschine zugeordnet haben.
                                      • Typ:
                                         Maschinentyp der Maschine.
                                      • Geschwindigkeitsverhalten:
                                         Angabe der Geschwindigkeit, die vom Maschinenhersteller vorgegeben
                                         ist.
                                      • Leistungsfähigkeit:
                                         Wird vom Maschinenhersteller vorgegeben.
                                      • Prüfprogramm:
2.10 / 11-2018




                                         Der logischen Maschine kann ein externes Prüfprogramm zugeordnet wer-
                                         den, mit dem geprüft wird, ob die Maschine die Tätigkeit ausführen kann.




                 D-104                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                           Maschinenzuordnung




                                      •   Treiber:
                                          Maschinentreiber der Produktionsmaschine.
                                      •   Zuschlaggruppe:
                                          ID der Gruppe zur Schleifzugabenberechnung.
                                      •   DynOpt:
                                          Angabe, ob die Software DynOpt verwendet wird.
                                      •   Bearbeitungsdauer:
                                          Formel, mit der die Dauer des Prozesses berechnet wird. Ein Doppelklick
                                          in das Feld bzw. auf eine ausgewählte Formel öffnet den Dialog Formel-
                                          Auswahl.
                                           “Formel-Auswahl” auf Seite D-106
                                      •   Einrichtdauer:
                                          Formel, mit der die Rüstzeit berechnet wird.
                                      •   Komponenten-ID:
                                          Die Komponenten-ID der logischen Maschine. Sie wird automatisch von
                                          der zugehörigen Maschine übernommen und kann nicht geändert werden.
                                      •   Als Alternative erlauben:
                                          Angabe, ob die logische Maschine als alternative Maschine verwendet
                                          werden darf, wenn auf einer anderen Maschine ein Engpass herrscht, die
                                          eigentlich für einen Arbeitsgang vorgesehen war. Diese Einstellung ist
                                          wichtig für die Umlastung.
                                      Wenn Sie ein Feld unter Allgemeine Eigenschaften der logischen Maschine
                                      markieren, wird im Feld darunter eine Kurzbeschreibung angezeigt.

                                      Feldbeschreibung anzeigen Sie können sich Feldbeschreibungen zur mar-
                                      kierten Eigenschaft anzeigen lassen:
                                      ☐ Die Feldbeschreibung wird nicht angezeigt.
                                      ☑ Öffnet den Dialog Feldbeschreibung (Datenbankfeld).

                                      Zusätzliche Bedingung Anzeige der zusätzlichen Bedingung.
                                      Mit der Schaltfläche [Lupe] öffnen Sie den Dialog Bedingung auswählen, um
                                      zusätzliche Bedingungen auszuwählen.
                                       “Bedingung auswählen” auf Seite D-102

                                          Zusätzliche Bedingungen
                                          Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaf-
                                          ten von Maschinen unter Umständen massiv.
                                          Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche
                                          Auswirkungen diese hat.
                                          Eine zusätzliche Bedingung könnte zum Beispiel alle Eigenschaften einer
                                          Maschine invertieren.

                                          Informationen zum Thema Formeln und Restriktionen in A+W Production
                                          finden Sie im Handbuch für den Part Formel-Editor.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                         D-105
                 Maschinenzuordnung                                                                  Softwarereferenz




                                      Formel-Auswahl
                                      Stammdaten > MZO > MZO-Editor > Logische Maschinen > Bearbeiten > Be-
                                      arbeitungsdauer markieren > […].




                                      Abb. D-57    Formel-Auswahl


                                      In diesem Dialog wählen Sie die Formel für die Bearbeitungsdauer der logi-
                                      schen Maschine aus. Die Formeln für die Bearbeitungsdauer werden mit dem
                                      Formel-Editor definiert und bearbeitet.
                                       Tutorial, “Formel zur Bearbeitungsdauer einer logischen Maschine auswählen” auf
                                        Seite D-66
                                       “Formel-Editor” auf Seite D-120
                                      Die Bearbeitungsdauer einer logischen Maschine kann auch in der A+W Ca-
                                      pacity Planner erstellt oder bearbeitet werden.
                                      Informationen zum Thema Formeln und Restriktionen in A+W Production fin-
                                      den Sie im Handbuch für den Part Formel-Editor.

                                      Verfügbare Formeln Liste der definierten Formeln zur Bearbeitungsdauer.

                                      Beschreibung Beschreibung der Formel markierten.

                                      [Neu] Öffnet den Dialog Formel-Editor, um eine neue Formel zu erstellen.
                                       “Formel-Editor” auf Seite D-120
2.10 / 11-2018




                                      [Editieren] Öffnet den Dialog Formel-Editor, um die markierte Formel zu be-
                                      arbeiten.




                 D-106                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                            Maschinenzuordnung




                                      [OK] Übernimmt die ausgewählte Formel in den Dialog Logische Maschine.

                                      [Abbrechen] Schließt den Dialog, ohne Änderungen zu übernehmen.


                                      Neuer Arbeitsgang
                                      Stammdaten > MZO > MZO-Editor > Arbeitsgänge > Neu.




                                      Abb. D-58    Neuer Arbeitsgang


                                      In diesem Dialog legen Sie einen neuen Arbeitsgang an und vergeben die ID
                                      und den Namen.
                                       “Arbeitsgang” auf Seite D-108

                                      ID Frei wählbare Identifikationsnummer.

                                      Name Frei wählbarer Name.
                                      Mit der Schaltfläche [OK] speichern Sie ID und Name und öffnen den Dialog
                                      Arbeitsgang.
                                       Softwarereferenz, “Arbeitsgang” auf Seite D-108

                                         Nicht zugeordnete Arbeitsgänge
                                         Ein Arbeitsgang wird in roter Schrift angezeigt, wenn ihm noch keine logi-
                                         sche Maschine zugeordnet ist. Ordnen Sie Arbeitsgängen immer eine logi-
                                         sche Maschine zu. Ist die zugehörige logische Maschine noch nicht
                                         definiert, sollte temporär die logische Maschine Dummy zugeordnet wer-
                                         den.

                                       Tutorial, “Arbeitsgangzuordnung” auf Seite D-51
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-107
                 Maschinenzuordnung                                                                  Softwarereferenz




                                      Arbeitsgang
                                      Stammdaten > MZO > MZO-Editor > Arbeitsgänge > Bearbeiten.




                                      Abb. D-59    Arbeitsgang


                                      In diesem Dialog legen Sie die Stammdaten für einen Arbeitsgang fest.
                                       Tutorial, “Arbeitsgänge anlegen und verwalten” auf Seite D-48
                                       Tutorial, “Bearbeitungstypen anlegen und verwalten” auf Seite D-73

                                      Eigenschaften
                                      •   ID:
                                          Identifikationsnummer, die Sie dem Arbeitsgang gegeben haben.
                                      •   Name:
                                          Bezeichnung, die Sie dem Arbeitsgang gegeben haben.
2.10 / 11-2018




                 D-108                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                             Maschinenzuordnung




                                      Restriktionen
                                      Mit der Wahl der Option legen Sie fest, welcher Bearbeitungstyp dem Arbeits-
                                      gang zugrunde liegt. Die entsprechenden Komboboxen werden freigeschaltet.
                                      • Keine:
                                         Keine Einschränkung.
                                      • A+W Typen:
                                         Auswahl aus dem A+W Standard-Bearbeitungskatalog.
                                      • Typen:
                                         Auswahl aus den vom Anwender definierten Bearbeitungstypen.
                                         Sie finden die Bearbeitungstypen unter Stammdaten > Bearbeitungen >
                                         Bearbeitungstypen.
                                      • Artikel:
                                         Auswahl aus den vom Anwender definierten Bearbeitungsartikeln.
                                         Sie finden die Bearbeitungsartikel unter Stammdaten > Bearbeitungen >
                                         Bearbeitungsartikel.

                                         Arbeitsgänge, Bearbeitungstypen und Artikel
                                         Aufgrund der Komplexität wird empfohlen, Arbeitsgängen lediglich die Be-
                                         arbeitungstypen Katalog und Typen zuzuordnen.

                                      Artikel
                                      Mit der Wahl der Option legen Sie fest, welcher Artikel bzw. welche Artikel-
                                      gruppe dem Arbeitsgang zugrunde liegt. Die entsprechenden Komboboxen
                                      werden freigeschaltet.
                                      • Keine:
                                         Keine Einschränkung.
                                      • Artikeltyp:
                                         Auswahl eines Artikeltyps.
                                      • Artikelgruppe:
                                         Auswahl einer Produktionsartikelgruppe.
                                      • Artikel:
                                         Auswahl eines bestimmten Artikels.

                                      Zusätzliche Bedingung Anzeige einer zusätzlichen Bedingung.
                                      Mit der Schaltfläche [Lupe] öffnen Sie den Dialog Bedingung auswählen, um
                                      zusätzliche Bedingungen auszuwählen.
                                       “Bedingung auswählen” auf Seite D-102

                                         Zusätzliche Bedingungen
                                         Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaf-
                                         ten von Maschinen unter Umständen massiv.
                                         Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche
                                         Auswirkungen diese hat.
                                         Eine zusätzliche Bedingung könnte zum Beispiel alle Eigenschaften einer
                                         Maschine invertieren.
2.10 / 11-2018




                                      Informationen zum Thema Formeln und Restriktionen in A+W Production fin-
                                      den Sie im Handbuch für den Part Formel-Editor.




                 A+W Production Maschinenzuordnung                                                           D-109
                 Maschinenzuordnung                                                                  Softwarereferenz




                                      Neuer Maschinentyp
                                      Stammdaten > MZO > MZO-Editor > Maschinentyp > Neu.




                                      Abb. D-60     Neuer Maschinentyp


                                      In diesem Dialog geben Sie die Stammdaten für den neuen Maschinentyp ein
                                      und legen damit einen neuen Maschinentyp an.
                                       “Maschinentyp” auf Seite D-111

                                      ID Frei wählbare Identifikationsnummer. Sie muss >1000 sein.

                                      Name Frei wählbarer Name.

                                      Tabellenbezug Angabe der Datenbank-Tabelle für den neuen Maschinen-
                                      typ. In dieser Tabelle werden die Daten der zugeordneten Maschinen gespei-
                                      chert.

                                         Beispiel

                                         In der Tabelle XOPT_TISCH sind alle Zuschnitt-Tische aufgeführt, die dem
                                         Maschinentyp Zuschnitt zugeordnet sind.

                                         In der Tabelle MZO_ISOLINIE sind alle Angaben zum Maschinenformat
                                         gespeichert, z. B. Format des Maschinencodes zur Ansteuerung der Linie
                                         oder des Biegers.


                                      Treiberart Datenbankfeld MZO_MASCHINTYP.DRIVER_CALL_METHOD.
                                      Die Eigenschaft wird nur zur Bestandspflege benötigt. Die Einstellung kann
                                      aus Kompatibilitätsgründen auf folgende Werte gesetzt werden:
                                      ☐ Ja = Methode (Driver-Call)
                                      ☑ Nein
                                       Irrelevant
2.10 / 11-2018




                 D-110                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                                            Maschinenzuordnung




                                      Maschinentyp
                                      Stammdaten > MZO > MZO-Editor > Maschinentypen > Maschinentyp markie-
                                      ren > [Bearbeiten].




                                      Abb. D-61   Maschinentyp bearbeiten


                                      In diesem Dialog bearbeiten Sie die Eigenschaften für einen benutzerdefinier-
                                      ten Maschinentyp.

                                      Maschine
                                      Name des gewählten Maschinentyps.

                                      Allgemeine Eigenschaften des Maschinentyps Stammdaten des Maschi-
                                      nentyps:
                                      • ID:
                                         Identifikationsnummer, die Sie dem Maschinetyp zugewiesen haben.
                                      • Text:
                                         Bezeichnung, die Sie dem Maschinentyp zugewiesen haben.
                                      • Tabellenbezug:
2.10 / 11-2018




                                         Anzeige der Datenbank-Tabelle, in der die Daten der zugeordneten Ma-
                                         schinen gespeichert sind.



                 A+W Production Maschinenzuordnung                                                          D-111
                 Maschinenzuordnung                                                             Softwarereferenz




                                      •   Treiberart:
                                          Die Eigenschaft nur zur Bestandspflege aus Kompatibilitätsgründen.
                                      •   Exklusiv, Pflicht, Implizit:
                                          Anzeige, wie der Maschinentyp zugewiesen wird.

                                      Feldbeschreibung anzeigen Sie können sich Feldbeschreibungen zur mar-
                                      kierten Eigenschaft anzeigen lassen:
                                      ☐ Die Feldbeschreibung wird nicht angezeigt.
                                      ☑ Öffnet den Dialog Feldbeschreibung (Datenbankfeld).

                                      Restriktionen

                                      Zusätzliche Bedingung Anzeige einer zusätzlichen Bedingung.
                                      Mit der Schaltfläche [Lupe] öffnen Sie den Dialog Bedingung auswählen, um
                                      zusätzliche Bedingungen bzw. Formeln auszuwählen.
                                       “Bedingung auswählen” auf Seite D-102

                                          Zusätzliche Bedingungen
                                          Zusätzliche Bedingungen beeinflussen das Verhalten und die Eigenschaf-
                                          ten von Maschinen unter Umständen massiv.
                                          Ist eine zusätzliche Bedingung hinterlegt, müssen Sie verstehen, welche
                                          Auswirkungen diese hat.
                                          Eine zusätzliche Bedingung könnte zum Beispiel alle Eigenschaften einer
                                          Maschine invertieren.

                                      Informationen zum Thema Formeln und Restriktionen in A+W Production fin-
                                      den Sie im Handbuch für den Part Formel-Editor.
2.10 / 11-2018




                 D-112                                                    A+W Production Maschinenzuordnung
                 Softwarereferenz                                             Formeln in der Maschinenzuordnung




                                      Formeln in der Maschinenzu-
                                      ordnung
                                      Formeln werden verwendet, um Restriktionen von Maschinen, logischen Ma-
                                      schinen und Arbeitsgängen spezifisch für Anwendungsfälle zu definieren.
                                      Formeln können in folgenden Dialogen ausgewählt werden:
                                       “Maschine” auf Seite D-95
                                       “Logische Maschine” auf Seite D-104
                                       “Arbeitsgang” auf Seite D-108
                                      Formeln und Bedingungen sind ausführlich im Part Formel-Editor beschrie-
                                      ben.
                                      In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                      •   “Bedingung auswählen” auf Seite D-102
                                      •   “Auswahl Bedingungen” auf Seite D-114
                                      •   “Neue Bedingung” auf Seite D-117
                                      •   “Info (zur neuen Bedingung)” auf Seite D-117
                                      •   “Auswahl Menge” auf Seite D-118
                                      •   “Formel-Editor” auf Seite D-120
                                      •   “Formel-Editor” auf Seite D-120
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                       D-113
                 Formeln in der Maschinenzuordnung                                                 Softwarereferenz




                                       Auswahl Bedingungen
                                       Stammdaten > MZO > Formula.




                                       Abb. D-62     Auswahl Bedingungen


                                       In diesem Dialog verwalten Sie die Bedingungen, die in der MZO zugewiesen
                                       werden können. Sie können zu den Bedingungen Formeln anlegen, bearbei-
                                       ten oder löschen.
                                       A+W Production bietet zwei Editoren, um Formeln anzulegen und bearbeiten:
                                        “Bedingungseditor (grafische Variante)” auf Seite D-115
                                        “Bedingungseditor (Text-Variante)” auf Seite D-119

                                       Vorhandene Bedingungen Die Liste der definierten Bedingungen (vor- und
                                       benutzerdefinierte).

                                       Beschreibung Beschreibung, die der Bedingungen beigefügt wurde.

                                       [Neue Bedingung (Grafik) …] Öffnet den Bedingungseditor (grafische Vari-
                                       ante).
                                        “Bedingungseditor (grafische Variante)” auf Seite D-115

                                       [Neue Bedingung (Text) …] Öffnet den Bedingungseditor (Text-Variante).
                                        “Bedingungseditor (Text-Variante)” auf Seite D-119

                                       [Editieren] Öffnet die markierte Bedingung im Bedingungseditor (grafische
                                       Variante)
2.10 / 11-2018




                                       [Löschen] Löscht die markierte Bedingung.



                 D-114                                                        A+W Production Maschinenzuordnung
                 Softwarereferenz                                                Formeln in der Maschinenzuordnung




                                      Keine Bedingung Sie können eine Bedingung zuordnen oder eine zugeord-
                                      nete Bedingung entfernen.
                                      ☐ Die Bedingung wird zugeordnet.
                                      ☑ Der Dialog liefert als Ergebnis, dass Nichts als selektiert gilt. Diese Einstel-
                                      lung müssen Sie mit [OK] bestätigen.


                                      Bedingungseditor (grafische Variante)
                                      Stammdaten > MZO > Formula > Neue Bedingung (Grafik).




                                      Abb. D-63    Bedingungseditor (grafische Variante)


                                      In diesem Dialog können Sie Formeln für Bedingungen mit grafischer Unter-
                                      stützung anlegen. Die Formeln werden im Editor als logische Verknüpfungen
                                      formuliert.
                                       Tutorial, “Bedingungen, Formeln, Restriktionen” auf Seite D-63
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                              D-115
                 Formeln in der Maschinenzuordnung                                                           Softwarereferenz




                                        Menüs

                                        Eintrag                      Funktion

                 Menü Bedingungen       Name                          “Neue Bedingung” auf Seite D-117

                                        Info                          “Info (zur neuen Bedingung)” auf Seite D-117

                                        Menge                         “Auswahl Menge” auf Seite D-118

                                        Invertieren                  Invertieren die Formel der Bedingung.

                                        OK                           Legt die neue Bedingung an und zeigt sie in der
                                                                     Auswahl.

                                        Abbrechen                    Bricht den Vorgang ab.

                 Menü Teilbedingungen   Hinzufügen (Spalte)          Fügt eine UND-Verknüpfung ein.

                                        Hinzufügen (Zeile)           Fügt eine ODER-Verknüpfung ein.

                                        Entfernen                    Löscht die markierte Verknüpfung.

                 Tab. D-1   Menüs im Bedingungseditor

                                        Schaltflächen
                                        Zusätzlich zu den Menüs können die Funktionen auch über folgende Schalt-
                                        flächen ausgewählt werden:

                                        Symbol                       Funktion

                                                                     Die definierte Bedingung wird gespeichert und der
                                                                     Editor geschlossen.

                                                                     Die definierte Bedingung wird verworfen und der Editor
                                                                     verlassen.

                                                                     Öffnet den Dialog zum Definieren der Bedingung. Mit
                                                                     einem zweiten Klick wird ein weiteres Control daneben
                                                                     geöffnet, um eine UND-Verknüpfung darzustellen.

                                                                     Öffnet den Dialog zum Definieren der Bedingung. Mit
                                                                     einem zweiten Klick wird ein weiteres Control darunter
                                                                     geöffnet, um eine Oder-Verknüpfung darstellen.

                                                                     Löscht die ausgewählte Bedingung.


                                        Optionsschalter All          Die Bedingungen aller Teile einer Stückliste werden
                                                                     berücksichtigt.

                                        Optionsschalter One          Nur die Eigenschaften der aktuellen Scheibe werden
                                                                     berücksichtigt.

                                        Optionsschalter Null         Die der Bedingung zugeordnete Menge wird nicht
                                                                     berücksichtigt.
2.10 / 11-2018




                                        Tab. D-2        Schaltflächen im Bedingungseditor




                 D-116                                                           A+W Production Maschinenzuordnung
                 Softwarereferenz                                               Formeln in der Maschinenzuordnung




                                      Neue Bedingung
                                      Stammdaten > MZO > Formula > Neue Bedingung (Grafik) > Menü Bedingun-
                                      gen > Name.




                                      Abb. D-64   Bedingungseditor (grafische Variante) > Name der Bedingung


                                      In diesem Dialog geben Sie den Namen der Bedingung an, um sie anzulegen.


                                      Info (zur neuen Bedingung)
                                      Stammdaten > MZO > Formula > Neue Bedingung (Grafik) > Menü Bedingun-
                                      gen > Info




                                      Abb. D-65   Bedingungseditor (grafische Variante) > Info


                                      In diesem Dialog geben Sie zusätzliche Informationen zu einer neuen Bedin-
                                      gung an.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                             D-117
                 Formeln in der Maschinenzuordnung                                                   Softwarereferenz




                                       Auswahl Menge
                                       Stammdaten > MZO > Formula > Neue Bedingung (Grafik) > Menü Bedingun-
                                       gen > Menge
                                       Stammdaten > MZO > Formula > Bedingungseditor (Text).




                                       Abb. D-66     Bedingungseditor (grafische Variante) > Auswahl Mengen


                                       In diesem Dialog wählen Sie die Menge zu einer Bedingung aus.
2.10 / 11-2018




                 D-118                                                        A+W Production Maschinenzuordnung
                 Softwarereferenz                                                Formeln in der Maschinenzuordnung




                                          Bedingungseditor (Text-Variante)
                                          Stammdaten > MZO > Formula > Neue Bedingung (Text) > Editieren > [Men-
                                          ge].




                 Abb. D-67   Bedingungseditor (Text-Variante)


                                          In diesem Dialog können Sie eine Bedingung mit Formeln anlegen oder bear-
                                          beiten. Die Formeln werden im Editor als logische Verknüpfungen formuliert.

                                          Bedingung

                                          ID Identifikationsnummer der Bedingung.

                                          Name Bezeichnung der Bedingung.

                                          Verwendbare Syntaxen
                                          Liste der zugelassenen logischen Operatoren

                                          Bedingung Angabe der Formel.

                                          Beschreibung Beschreibung der Bedingung, z. B. die Verwendung.
2.10 / 11-2018




                                          Allgemein

                                          Status Anzeige den aktuellen Status der Bedingung.


                 A+W Production Maschinenzuordnung                                                            D-119
                 Formeln in der Maschinenzuordnung                                                      Softwarereferenz




                                             Sprache Auswahl der Sprache, in der die Beschreibung angezeigt wird.

                                             Verfügbare Formeln Liste der definierten Formeln. Diese können per Dop-
                                             pelklick übernommen werden. Im Feld Bedingung werden sie an der Stelle
                                             des Cursors eingefügt.

                                             Beschreibung Beschreibung der markierten Formel.

                                             [Löschen] Löscht eine markierte Formel ohne Abfrage.

                                             [Neue Formel] Öffnet einen Formel-Editor, mit dem Sie Formeln definieren.
                                             Die neue Formel wird in der Liste Verfügbare Formeln angezeigt und kann zur
                                             Definition von Bedingungen verwendet werden.

                                             [Editieren] Öffnet die markierte Formel im Editor, um sie zu bearbeiten.


                                             Formel-Editor
                                             Stammdaten > MZO > MZO-Editor > Logische Maschinen > Bearbeitungsdau-
                                             er > Formel-Auswahl > Neu, Editieren.




                 Abb. D-68   Formel-Editor
2.10 / 11-2018




                                             In diesem Dialog können Sie Formeln anlegen und bearbeiten, die z. B. bei lo-
                                             gischen Maschinen die Bearbeitungsdauer definieren.



                 D-120                                                            A+W Production Maschinenzuordnung
                 Softwarereferenz                                             Formeln in der Maschinenzuordnung




                                      Formel

                                      ID Identifikationsnummer, der Formel.

                                      Name Bezeichnung der Formel.

                                      Formel Definition der Formel.

                                      Beschreibung Beschreibung zur Formel.

                                      Verfügbare Formeln

                                      Formel Liste der definierten Formeln. Diese können per Doppelklick über-
                                      nommen werden. Im Feld Bedingung werden sie an der Stelle des Cursors
                                      eingefügt.

                                      Name Namen der markierten Formeln.

                                      Beschreibung Beschreibung der markierten Formel.

                                      [Formel hinzufügen] Fügt die markierte Formel in der Formel ein, die bear-
                                      beitet wird.

                                      [Übernehmen] Speichert die neue oder bearbeitete Formel. Diese steht
                                      dann in der Liste im Dialog Formel-Auswahl zur Verfügung.

                                      [Schließen] Schließt den Dialog Formel-Editor.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                       D-121
                 Bearbeitungen in der Maschinenzuordnung                                         Softwarereferenz




                                        Bearbeitungen in der Maschi-
                                        nenzuordnung
                                        Die MZO arbeitet mit einem normierten Bearbeitungskatalog, damit die Daten
                                        mit den anderen Programmen der A+W Software GmbH mühelos ausge-
                                        tauscht werden können. Dieser Bearbeitungskatalog umfasst in der MZO die
                                        Bearbeitungstypen und die Bearbeitungsartikel.
                                        In diesem Kapitel finden Sie informationen zu folgenden Themen:
                                        •   “Bearbeitungstypen” auf Seite D-123
                                        •   “Bearbeitungsartikel” auf Seite D-125
2.10 / 11-2018




                 D-122                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                      Bearbeitungen in der Maschinenzuordnung




                                      Bearbeitungstypen
                                      Stammdaten > Bearbeitungen > Bearbeitungstypen.




                                      Abb. D-69    Bearbeitungstypen


                                      In diesem Dialog sind alle definierten Bearbeitungstypen gelistet. Sie können
                                      Bearbeitungstypen anlegen und bearbeiten oder löschen.
                                      Mit einem Bearbeitungstyp wird beschrieben, um welche technische Form der
                                      Bearbeitung es sich handelt, zum Beispiel Zuschnitt, Montage, Säumen,
                                      Schleifen oder Verpacken.

                                      Liste
                                      •   Nr.:
                                          Eindeutige Nummer des Bearbeitungstyps.
                                      •   Bezeichnung:
                                          Name des Bearbeitungstyps.
                                      •   Sequenz:
                                          Sequenz des Bearbeitungstyps.

                                          Bearbeitungstypen
                                          In A+W Production gibt es einen Standard-Katalog von Bearbeitungstypen.
                                          Diese tragen vierstellige Nummern und dürfen vom Anwender nicht verän-
                                          dert werden.
                                          Darüber hinaus können Sie weitere Bearbeitungstypen definieren. Es wird
                                          empfohlen, die jeweils passenden Bearbeitungstypen aus dem Standard-
                                          Katalog als Basis zu verwenden.

                                      Bearbeitungstyp-Nr. Angabe der frei wählbaren Nummer für den Bearbei-
2.10 / 11-2018




                                      tungstyp.




                 A+W Production Maschinenzuordnung                                                          D-123
                 Bearbeitungen in der Maschinenzuordnung                                               Softwarereferenz




                                        Sequenz Angabe der Sequenz, die dem Bearbeitungstyp zugewiesen wird.
                                        Je kleiner die Zahl der Sequenz, desto früher steht die Bearbeitung im Produk-
                                        tionsprozess. Korrekte Sequenzen sind unerlässlich für die zuverlässige Be-
                                        stimmung von Produktionsterminen in der Kapazitätsplanung.

                                        Bezeichnung Angabe eines Namens, mit dem Sie den Bearbeitungstyp kurz
                                        beschreiben.

                                        Zählen von Bearbeitungen Angabe, wie die Bearbeitungen gezählt werden
                                        sollen.
                                        • Aufsummieren:
                                            Wenn die gleiche Bearbeitung an einer Scheibe mehrfach durchgeführt
                                            wird, wird jeder Durchgang gezählt.
                                        • Einmal zählen:
                                            Wenn die gleiche Bearbeitung an einer Scheibe mehrfach durchgeführt
                                            wird, wird die Bearbeitung nur 1x gezählt, um sicherzustellen, dass sie
                                            durchgeführt wurde.
                                        • Nicht zählen:
                                            Die Bearbeitung wird nicht gezählt.

                                        Bearbeitungsart Auswahl der Bearbeitungsart. Die Bearbeitungsart steuert
                                        die korrekte Wendung von zu bedruckenden oder zu beschichtenden Schei-
                                        ben. Folgende Bearbeitungsarten stehen zur Verfügung:
                                        • 505 Glaszuschnitt für Zuschnitte
                                        • 588 Siebdruck für Siebdrucke
                                        • 00 nicht zugewiesen für alle anderen Bearbeitungen

                                        BDE-Verfolgung Bearbeitungen, die zum aktuellen Bearbeitungstypes ge-
                                        hören, werden in der BDE-Initialisierung berücksichtigt.
                                        Die Einstellung wird aus der Spaltenzuordnung der BDE eingelesen und kann
                                        am Bearbeitungstyp nicht geändert werden.
                                        Eine Beschreibung der Stammdaten für die BDE finden Sie im Part Betriebs-
                                        datenerfassung.

                                        [Ändern] Schaltet die Eingabefelder der markieren Bearbeitung frei.

                                        [Verwerfen] Bricht den Vorgang ab, ohne Änderungen zu übernehmen.

                                           Bearbeitungstypen löschen
                                           Bearbeitungstypen können nicht gelöscht werden, wenn sie einem Produk-
                                           tionsartikel zugeordnet sind. In diesem Fall erscheint eine Sicherheitsab-
                                           frage.
                                           Lösen Sie in diesem Fall die Zuordnung vorher auf.

                                            Tutorial, “So löschen Sie einen Bearbeitungstyp” auf Seite D-75
2.10 / 11-2018




                 D-124                                                         A+W Production Maschinenzuordnung
                 Softwarereferenz                                        Bearbeitungen in der Maschinenzuordnung




                                      Bearbeitungsartikel
                                      Stammdaten > Bearbeitungen > Bearbeitungsartikel.




                                      Abb. D-70    Bearbeitungsartikel


                                      In diesem Dialog sind alle definierten Bearbeitungsartikel gelistet. Sie können
                                      Bearbeitungsartikel anlegen und bearbeiten oder löschen.
                                      Mit einem Bearbeitungsartikel wird die technische Form der Bearbeitung ex-
                                      akter beschrieben, z. B. Facetten-Schleifen, Gehrungs-Schleifen oder Ker-
                                      ben-Schleifen. Ein Bearbeitungsartikel referenziert immer auf einen
                                      Bearbeitungstyp.

                                      Liste Anzeige der definierten Bearbeitungsartikel.
                                      • Artikelnr.:
                                         Eindeutige Nummer des Bearbeitungsartikels.
                                      • Bezeichnung:
                                         Der Name, der dem Bearbeitungsartikel zugewiesen wurde.
                                      • Bearbeitungstyp:
                                         Der Bearbeitungstyp, auf den der Bearbeitungsartikel referenziert.

                                      Artikel-Nr. Frei wählbare Nummer für den Bearbeitungsartikel.

                                      Bezeichnung Frei wählbare Beschreibung, die Sie dem Produktionsartikel
2.10 / 11-2018




                                      geben.




                 A+W Production Maschinenzuordnung                                                            D-125
                 Bearbeitungen in der Maschinenzuordnung                                            Softwarereferenz




                                        Bearbeitungstyp Bearbeitungstyps, auf den der Bearbeitungsartikel refe-
                                        renziert.

                                        Klasse Die Klasse steuert, an welche Stelle der Stückliste der Inhalt des
                                        Plan-Textes geschrieben wird. Der Wertebereich der Klasse liegt zwischen 1
                                        und 8.

                                        Plan-Text/Prior. Der Plan-Text ist ein Kennzeichen, das an die Stückliste ge-
                                        setzt wird. Der Plan-Text kann z. B. anzeigen, dass eine Scheibe poliert wer-
                                        den muss.
                                        Die Priorität legt fest, welcher Plan-Text sich durchsetzt, wenn mehrere Bear-
                                        beitungen einer Klasse durchgeführt werden. Je kleiner der Wert, desto höher
                                        ist die Priorität.

                                        Übergangszeit Übergangszeit für den Bearbeitungsartikel. Die Funktion
                                        Übergangzeit ist derzeit nicht aktiv.

                                        Dauer Dauer der Bearbeitung. In der Kombobox wählen Sie die Bezugsgrö-
                                        ße Stück, Strecke, Fläche oder Volumen.

                                        Reihenfolge Reihenfolge der Bearbeitung in der Stückliste. Damit können
                                        Sie die Reihenfolge der Bearbeitung genau abstimmen.

                                        Schleifgruppe Schleifgruppe bei Bearbeitungsartikeln für Kantenbearbeitun-
                                        gen. Kantenbearbeitungen – auch solche, die keinen Abtrag erzeugen – wer-
                                        den nur dann bei der Geometrieberechnung und Plausibilisierung
                                        berücksichtigt, wenn eine Schleifgruppe ausgewählt wurde.

                                        Text Beschreibung für den Bearbeitungsartikel.

                                        Extra 1 Werte für die Anbindung des CAD-Systems. Diese Werte legen Sie
                                        zusammen mit dem Projektteam der A+W Software GmbH fest.

                                        Extra 2 Zuzeit nicht aktiv.

                                        Bearbeitung möglich auf Dieser Wert unterstützt die Stücklistenprüfung bei
                                        der Einlastung, indem Bearbeitungen zurückgewiesen werden, die sich an der
                                        falschen Stelle befinden.
                                        • 00 nicht zugewiesen:
                                            Die Bearbeitung wird in jedem Fall zurückgewiesen.
                                        • 01 Nichtglasartikel:
                                            Die Bearbeitung darf nicht auf Glas angewendet werden, z. B. Beschläge
                                            verpacken.
                                        • 02 Basisglas:
                                            Die Bearbeitung darf nur auf Basisglas angewendet werden, z. B. Float-
                                            Zuschnitt.
                                        • 04 Isolierglas:
                                            Die Bearbeitung darf nur auf Isolierglas angewendet werden, z. B die Gas-
                                            füllung.
2.10 / 11-2018




                 D-126                                                       A+W Production Maschinenzuordnung
                 Softwarereferenz                                      Bearbeitungen in der Maschinenzuordnung




                                      •   54 Ungehärtete Gläser:
                                          Die Bearbeitung darf nur auf ungehärteten Gläsern angewendet werden.
                                      •   62 Alle Produkte:
                                          Die Bearbeitung darf an allen Gläsern angewendet werden.

                                      Bearbeitungsmaße enthalten Sie können festlegen, ob die Bearbeitungs-
                                      maße bei der Geometrieberechnung berücksichtigt werden.
                                      ☐ Standardeinstellung. Die Checkbox sollte nicht aktiviert sein, da dann auch
                                      Bearbeitungen in der Geometrieberechnung berücksichtigt werden, die keine
                                      Kantenbearbeitungen sind.
                                      ☑ Die Bearbeitung wird in der Geometrieberechnung berücksichtigt.

                                      Zuschnittsmaß korrigieren Sie können festlegen, wo die Zuschnittsmaße
                                      berechnet werden.
                                      ☐ Standardeinstellung. Die Checkbox sollte nicht aktiviert werden.
                                      ☑ Die Zuschnittsmaße werden unabhängig vom Artikelstamm berechnet.

                                      Explizite Planung Sie können festlegen, ob die Bearbeitung separat freige-
                                      geben wird.
                                      ☐ Keine Funktion.
                                      ☑ Der Bearbeitungsartikel kann separat freigegeben werden, falls die Bear-
                                      beitung angewendet wird. Sie können damit zum Beispiel ein Basisglas sepa-
                                      rat freigeben, falls die Bearbeitung Siebdruck durchgeführt wird.

                                      Interne Bearbeitung Sie können festlegen, ob der Bearbeitungsartikel nur
                                      für interne Berechnungen dient.
                                      ☐ Keine Funktion.
                                      ☑ Die Bearbeitung beschreibt als definierte Bearbeitung die Entstehung des
                                      Stücklistenteils.

                                      Außer-Haus-Bearbeitung Sie können festlegen, ob der Bearbeitungsartikel
                                      für Fremdbearbeitungen dient.
                                      ☐ Der Bearbeitungsartikel wird in A+W Production verwendet.
                                      ☑ Die Bearbeitung wird von einem externen Anbieter durchgeführt.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-127
                 Bearbeitungen in der Maschinenzuordnung                                          Softwarereferenz




                                        Spalten anpassen
                                        Stammdaten > Bearbeitungen > Bearbeitungstypen > [Spalten anpassen].




                                        Abb. D-71   Spalten anpassen


                                        In diesem Dialog können Sie festlegen, welche Spalten angezeigt werden. Da-
                                        mit haben Sie Einfluss auf die Gestaltung des Dialogs.

                                        Verfügbare Spalten Anzeige der Datenbankfelder, die zur Verfügung ste-
                                        hen.

                                        Aktuelle Spalten Anzeige der Datenbankfelder, die aktuell angezeigt wer-
                                        den.

                                        [Bearbeiten] Öffnet den Dialog Spaltendefinition, um den markierten Eintrag
                                        zu bearbeiten.
2.10 / 11-2018




                 D-128                                                      A+W Production Maschinenzuordnung
                 Softwarereferenz                                      Bearbeitungen in der Maschinenzuordnung




                                      Spaltendefinition
                                      Stammdaten > Bearbeitungen > Bearbeitungstypen > [Spalten anpassen] >
                                      [Bearbeiten].




                                      Abb. D-72   Spaltendefinition


                                      In diesem Dialog können Sie die Spalten bearbeiten.

                                         Spaltendefintion bearbeiten
                                         Die Spaltendefinition greift tief in die Funktionalität von A+W Production
                                         ein. Wenden Sie sich an den Service der A+W Software GmbH, wenn Sie
                                         die Einstellungen bearbeiten wollen.
2.10 / 11-2018




                 A+W Production Maschinenzuordnung                                                          D-129
                 Bearbeitungen in der Maschinenzuordnung                      Softwarereferenz
2.10 / 11-2018




                 D-130                                     A+W Production Maschinenzuordnung
Maschinenzuordnung         D

                     Partindex




              A+W Production
                 Partindex                                                                                 Index




                 Index
                 A                                                 F
                 Abmessungsrestriktionen D-20, D-100               Formel auswählen D-65, D-102
                 Arbeitsgang D-40, D-41, D-90                      Formel-Editor
                 – anlegen D-48, D-107                             – grafische Variante D-115
                 – basierend auf Bearbeitungsartikel D-47          – Text-Variante D-119
                 – bearbeiten D-49, D-108                          Formeln und Bedingungen D-63, D-113
                 – erstellen D-48, D-107                           – Bearbeitungsdauer D-66, D-106
                 – exakt definieren D-44                           – in der MZO D-64
                 – löschen D-50
                 – mehrere Arbeitsgänge D-45                       K
                 – nicht zugeordnet D-44                           Komponenten-ID   D-21
                 – Priorität D-44
                 – verwalten D-48
                 – zusätzliche Bedingung D-45                      L
                 Arbeitsgangzuordnung D-51, D-91                   Logische Maschine D-33, D-34, D-88
                 – angepasste D-52                                 – anlegen D-36, D-103
                 – logische Maschine und Arbeitsgang               – bearbeiten D-38, D-104
                   trennen D-60                                    – Bearbeitungsdauer D-106, D-120
                 – logische Maschine und Arbeitsgang               – erstellen D-36, D-103
                   zuordnen D-58                                   – Formel-Auswahl D-106, D-120
                 – Prioriät ändern D-61                            – löschen D-39
                 – zusätzliche Bedingung D-52                      – verwalten D-36


                 B                                                 M
                 Bearbeitungsartikel D-69                          Maschine D-15, D-16, D-87
                 – anlegen D-76                                    – Abmessungsrestriktionen D-20, D-30, D-31,
                 – bearbeiten D-78                                   D-100
                 – erstellen D-76                                  – anlegen D-22, D-94
                 – in der MZO D-71                                 – bearbeiten D-23, D-26, D-95
                 – löschen D-79                                    – beschichtete Gläser D-20, D-28
                 – verwalten D-76                                  – Eigenschaften bearbeiten D-23
                 – Zuordnung zu Bearbeitungstyp auflösen    D-79   – erstellen D-22, D-94
                 Bearbeitungstypen D-69, D-122, D-123              – Komponenten-ID D-21
                 – anlegen D-73                                    – löschen D-25
                 – bearbeiten D-74                                 – maximale Dicke D-26
                 – erstellen D-73                                  – maximale dicke D-19
                 – in der MZO D-70                                 – minimale Dicke D-19
                 – löschen D-75                                    – minimale dicke D-26
                 – verwalten D-73                                  – Modelle D-20, D-28
                 Bedingung auswählen D-65, D-102                   – Namen und Nummern D-19
                 Bedingungen und Formeln D-63, D-113               – Restriktionen D-19
                 – Bearbeitungsdauer D-66, D-106                   – Scheibenformat D-20
                 – in der MZO D-64                                 – Strukturgläser D-20, D-28
                 Bedingungseditor                                  – Stufen-ISO D-20, D-28
                 – grafische Variante D-115                        – SZR-Restriktionen D-20, D-30, D-31, D-101
                                                                   – UND-/ODER-Verknüpfungen D-21
2.10 / 11-2018




                 – Text-Variante D-119
                 Beschichtete Gläser D-20                          – verwalten D-22
                                                                   – X-, Y-, Z-,W-Schnitte D-97
                                                                   – zusätzliche Bedingung D-21


                 A+W Production Maschinenzuordnung                                                       D-133
                 Index                                                          Partindex




                 Maschinenrestriktionen D-19
                 – bearbeiten D-26
                 Maschinentyp
                 – anlegen D-110
                 – bearbeiten D-111
                 Maschinentypen D-92
                 Maschinenzuordnung D-14
                 – Arbeitsgang D-40
                 – Arbeitsgangzuordnung D-51
                 – Bestandteile D-12
                 – logische Maschine D-33
                 – Maschine D-15, D-16
                 – Schaltflächen D-81
                 Maximale Dicke D-19
                 Minimale Dicke D-19
                 Modelle D-20
                 MZO D-14
                 – Bestandteile D-12
                 MZO-Editor
                 – Arbeitsgänge D-90
                 – Arbeitsgangzuordnung D-91
                 – Logische Maschinen D-88
                 – Maschinen D-87
                 – Maschinentypen D-92

                 N
                 Neue logische Maschine D-103
                 Neue Maschine D-22, D-94
                 Neuer Arbeitsgang D-107
                 Neuer Maschinentyp D-110

                 S
                 Schaltflächen in der MZO D-81
                 Scheibenformat D-20
                 Strukturgläser D-20
                 Stufen-ISO D-20
                 SZR-Restriktionen D-20, D-101

                 U
                 UND-/ODER-Verknüpfungen        D-21

                 Z
                 Zusätzliche Bedingung   D-21
                 – auswählen D-102
2.10 / 11-2018




                 D-134                                 A+W Production Maschinenzuordnung

