---
title: "DE AWProduction Feinplanung 3.0"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWProduction_Feinplanung_3.0"]
version: "1.0"
last_updated: "2025-12-10"
description: "Feinplanung               F                              deutsch                   A+W Production                                        Revisionsübersicht                                        Part                     Beschreibung                                        Version / Datum                                         3.00 / 01-2023          Komplette Überarbeitung.                                         2.02 / 01-2017          Produkt- und Firmennamen angepasst, Felder ergänzt."
source_file: "DE_AWProduction_Feinplanung_3.0.pdf"
---


# DE AWProduction Feinplanung 3.0

Feinplanung               F




                         deutsch




              A+W Production
                                       Revisionsübersicht
                                       Part                     Beschreibung
                                       Version / Datum

                                       3.00 / 01-2023          Komplette Überarbeitung.

                                       2.02 / 01-2017          Produkt- und Firmennamen angepasst, Felder ergänzt.

                                       2.01 / 07-2013          Vollständige Überarbeitung der ALCIM-Dokumentation
                                                               und Anpassung auf A+W Production.

                                       2.00 / 11-2012          Komplette Überarbeitung.

                                       1.00 / 09-2007          Ersterstellung.



                                       Editorial
                                       Das Editorial enthält Informationen zu folgenden Themen:
                                       •   Anmerkungen zu diesem Dokument
                                       •   Urheberrechte
                                       •   Warenzeichen

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
                                       Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbau-
                                       stufe von A+W Production.

                                       Urheberrechte
                                       © 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                                       stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                       Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                                       piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                                       Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
                                       A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
3,00 / 01-2023




                                       nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.




                 A+W Production Feinplanung                                                                    F-3
                       Warenzeichen
                       Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen kön-
                       nen gleichzeitig auch eingetragene Marken oder sonstige gewerbliche
                       Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.
                          Revisionsübersicht .............................................................................................. F-3
                          Editorial ............................................................................................................... F-3

                       Tutorial                                                                                                              F-7
                       Dokumentations-Hinweise ...................................................................................... F-9
                         Wichtige Hinweise ............................................................................................... F-9
                         Dokumentation .................................................................................................. F-11
                           Aufbau des Tutorials ...................................................................................... F-11
                           Darstellungskonventionen .............................................................................. F-12
                       Überblick Feinplanung .......................................................................................... F-13
                         Ablauf der A+W Production ............................................................................... F-14
                         Begriffe der A+W Production ............................................................................. F-16
                           Lostyp ............................................................................................................ F-16
                           Lose ............................................................................................................... F-17
                             Verwendungslos ......................................................................................... F-17
                             Produktionslos ............................................................................................ F-17
                           Böcke (Abstellplätze) ..................................................................................... F-17
                             Verwendungsbock ...................................................................................... F-17
                             Produktionsbock ......................................................................................... F-18
                           Läufe .............................................................................................................. F-18
                             Läufe archivieren ........................................................................................ F-18
                           Teilebaum ...................................................................................................... F-20
                           Organisation (Orga) ....................................................................................... F-20
                       Gruppierungen und Sortierungen ......................................................................... F-21
                         Überblick ........................................................................................................... F-22
                           Einführung ...................................................................................................... F-23
                           Gruppierung ................................................................................................... F-24
                           Sortierung ...................................................................................................... F-25
                           Zusatz-Sortierung .......................................................................................... F-28
                           Sonderteile ..................................................................................................... F-30
                             Füllaufträge ................................................................................................. F-30
                             Restscheiben .............................................................................................. F-31
                             Bruchscheiben ............................................................................................ F-32
                             Eilscheiben ................................................................................................. F-33
                           Demos und Übungen ..................................................................................... F-34
                       Abstellplätze und -modi ........................................................................................ F-36
                         Überblick ........................................................................................................... F-37
                           Abstellplätze ................................................................................................... F-38
                           Logische Abstellplätze ................................................................................... F-38
                           Abstellregeln .................................................................................................. F-39
                           Vordefinierte Abstellmodi für A-Böcke ........................................................... F-41
                             Abstellmodus Glas ...................................................................................... F-41
                             Abstellmodus Einheit .................................................................................. F-42
                             Abstellmodus Produktion ............................................................................ F-44
                             Abstellmodus VABGLA ............................................................................... F-46
                           Robot-Böcke .................................................................................................. F-47
                           Abstellmodi für Fächerwagen ........................................................................ F-47
                           Abstellmodi für feste Abstellplätze ................................................................. F-47
3,00 / 01-2023




                         Standard-Einstellungen in der Konfiguration ..................................................... F-48
                         Einstellungen in den Stammdaten ..................................................................... F-49
                           Demos und Übungen ..................................................................................... F-52



                 F-4                                                                                A+W Production Feinplanung
                                       Optimierungsmodi ................................................................................................. F-55
                                         Überblick ........................................................................................................... F-56
                                           Unterschiedliche Optimierungs-Modi ............................................................. F-57
                                             Optimierungsmodus 6.2 - Feste Reihenfolge ............................................. F-57
                                             Optimierungsmodus 6.1 - Kunden zusammenhalten ................................. F-58
                                             Optimierungsmodus 5.2 - Standard ............................................................ F-60
                                             Optimierungsmodus 5.1 - ISO auf Fächerwagen oder viele A-Böcke ........ F-61
                                             Optimierungsmodus Freie Optimierung - Scheiben auf Fächerwagen ....... F-63
                                             Doppel-Optimierung ................................................................................... F-65
                                           Demos und Übungen ..................................................................................... F-66
                                       Orgas .................................................................................................................... F-68
                                         Organisationsformen ......................................................................................... F-69
                                           Allgemein ....................................................................................................... F-70
                                           Baumstruktur .................................................................................................. F-70
                                           Master-Orga ................................................................................................... F-71
                                           Bruch-Orga .................................................................................................... F-76
                                           Prüfreihenfolge ............................................................................................... F-76
                                           Orga-Typ und Los-Typ ................................................................................... F-78
                                             Verwendungs- und Produktions-Orgas ...................................................... F-78
                                           Globale Einstellungen .................................................................................... F-79
                                           Demos und Übungen ..................................................................................... F-80
                                         Produktionsreihenfolge ...................................................................................... F-81
                                           Allgemein ....................................................................................................... F-82
                                           Gruppierungsschlüssel der Orga-Gruppen .................................................... F-82
                                             Ohne Gruppierung ...................................................................................... F-82
                                             Mit Gruppierung .......................................................................................... F-83
                                         A+W Standard-Orgas ........................................................................................ F-84
                                           Abstellplatzorganisation ................................................................................. F-85
                                             A-Böcke SZR .............................................................................................. F-86
                                             ISO-A-Böcke ............................................................................................... F-93
                                             A-Böcke Versand ........................................................................................ F-99
                                             Fächerwagen ohne Auffüllen .................................................................... F-104
                                             Aufgefüllte Fächerwagen .......................................................................... F-109
                                           Demos und Übungen ................................................................................... F-114

                                       Softwarereferenz                                                                                                F-117
                                       Übersicht ............................................................................................................. F-119
                                       Organisationen ................................................................................................... F-120
                                         Register Master-Orga ...................................................................................... F-120
                                         Register Produktionsreihenfolge ..................................................................... F-122
                                         Register Prüfreihenfolge .................................................................................. F-124
                                         Master-Orga .................................................................................................... F-126
                                         Orga ................................................................................................................ F-131
                                         Orga-Gruppen ................................................................................................. F-133
                                         Einstellungen-Abstellplatz ............................................................................... F-135
                                         Voreinstellungen .............................................................................................. F-139
                                       Gruppierung und Sortierung ............................................................................... F-140
                                         Gruppierung/Sortierung - Dialog ..................................................................... F-140
                                           Register Editor-Gruppierungen .................................................................... F-141
                                           Register Editor-Sortierung ........................................................................... F-143
                                           Register Zusatz-Sortierungen ...................................................................... F-144
                                         Erzeugung einer Zusatz-Sortierung ................................................................ F-145
                                       Abstellplätze ....................................................................................................... F-146
3,00 / 01-2023




                                         Abstellplätze .................................................................................................... F-146
                                       Lose .................................................................................................................... F-151




                 A+W Production Feinplanung                                                                                                                    F-5
                         Lostypen und Bearbeitungen .......................................................................... F-151
                           Register Lostypen ........................................................................................ F-151
                           Register Bearbeitungen ............................................................................... F-154
                           Register Abhängige Bearbeitungen ............................................................. F-156
                       Läufe feinplanen ................................................................................................. F-158
                         Feinplanung für Lauf … ................................................................................... F-158
                           Register Glasarten ....................................................................................... F-159
                           Register Bockbelegung ................................................................................ F-162
                           Register Ergebnisse ..................................................................................... F-167
                           Register Spezial ........................................................................................... F-169
                             Register Zusammenlegen ........................................................................ F-169
                             Register Füllaufträge ................................................................................ F-171
                             Register Restblätter .................................................................................. F-173
                             Register Bruchscheiben ........................................................................... F-174
                             Register Eilscheiben ................................................................................. F-176
                             Register Glasdicken ................................................................................. F-177
                           Register Freie Optimierung .......................................................................... F-179
                           Register Teilmengen .................................................................................... F-180
                           Register Orga ............................................................................................... F-182
                           Register Orga-Optionen ............................................................................... F-184
                           Register Optionen ........................................................................................ F-186
                           Register Auswahl Lagermaß ........................................................................ F-188
                         Ändern der minimalen Anzahl A-Böcke ........................................................... F-189
                         Reihenfolge der Maschinen ............................................................................. F-190

                       Partindex                                                                                                F-193
3,00 / 01-2023




                 F-6                                                                            A+W Production Feinplanung
Feinplanung               F

                      Tutorial




              A+W Production
                 Tutorial                                                                  Dokumentations-Hinweise




                                       Dokumentations-Hinweise
                                       Das Tutorial zum Modul Feinplanung beschäftigt sich mit den Grundlagen des
                                       gesamten Produktionsprozesses. Angefangen vom Zuschnitt über die unter-
                                       schiedlichen Produktions-Linien bis hin zu den Versandgestellen. Es baut auf
                                       den Kenntnissen der Grobplanung auf.

                                           Funktionen sind von den freigeschalteten Modulen abhängig
                                           Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur
                                           Verfügung stehen, wenn die zugehörigen Module und Schnittstellen instal-
                                           liert und freigeschaltet sind.

                                           Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installati-
                                           on nicht zugänglich sind, wenden Sie sich bitte an die A+W Software
                                           GmbH.

                                       Themenblöcke
                                       Zur Schulung des Moduls Feinplanung gehören folgende Themenblöcke:
                                       •   Gruppierungen und Sortierungen
                                       •   Abstellplätze und -modi
                                       •   Optimierungsmodi
                                       •   Orgas


                                       Wichtige Hinweise
                                       Diese Dokumentation ist als Unterstützung für den täglichen Arbeitsbetrieb
                                       und als Schulungsunterlage für eine begleitete Softwareschulung durch einen
                                       zertifizierten A+W Trainer zu verstehen. Sie dient nicht dem Selbststudium
                                       und kann keine 100%ig fehlerfreie Anwendung gewährleisten, da die Komple-
                                       xität nicht von der Software sondern von den realen Arbeitsprozessen ab-
                                       hängt. Die Feinplanung definiert die gesamten Organisations- und
                                       Produktionsabläufe in Ihrer Produktion. Sie kann daher entsprechend Ihren
                                       Anforderungen sehr komplex ausfallen und wird ausschließlich in Begleitung
                                       durch einen erfahrenen A+W-Mitarbeiter erstellt und gemeinsam mit Ihnen
                                       eingerichtet. Möchten Sie Änderungen an den Einstellungen vornehmen,
                                       wenden Sie sich vorher bitte unbedingt an A+W, da es sonst zu unerwünsch-
                                       ten Ergebnissen kommen kann!
                                       Der Anwender muss Kenntnisse in der Anwendung von physischen Prozess-
                                       abläufen in der Glasproduktion und -organisation haben.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                       F-9
                    Dokumentations-Hinweise                                                                  Tutorial




                                          Produktnamen
                                          Im Rahmen der strategischen Produktneuausrichtung wurden das Produkt-
                                          portfolio A+W und die Produktnamen vereinfacht. So wurde aus ALCIM bei-
                                          spielsweise A+W Production.
                                          Da im Produktentwicklungszyklus sowohl die alten Produktversionen als auch
                                          die neuen Produktversionen angepasst und erweitert wurden, verwenden wir
                                          zur Vereinfachung in diesem Dokument ausschließlich die alten Produktna-
                                          men - die neuen Produktversionen werden unter den alten Namen subsum-
                                          miert.
01-2023 / 01-2023




                    F-10                                                               A+W Production Feinplanung
                 Tutorial                                                                   Dokumentations-Hinweise




                                       Dokumentation
                                       Für die Schulung zur A+W Production stehen folgende Unterlagen zur Verfü-
                                       gung:

                                       Handout                   Ausdruck Schulungsunterlage für die Teilnehmer

                                       PDF                       Vollständige Unterlagen
                                                                 • Tutorial
                                                                 • Softwarereferenz
                                                                 • Index

                                       Online-Hilfe <F1>        Kontextsensitive Dialog-Hilfe der A+W Production-
                                                                Softwarereferenz.


                                       Aufbau des Tutorials
                                       Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinhei-
                                       ten. Jede Lerneinheit besteht aus folgenden Komponenten:

                                       Überblick                Jede Lerneinheit beginnt mit einem Überblick über die
                                                                wichtigsten Inhalte:
                                                                 • Lernziele: Was soll vermittelt werden?
                                                                 • Nutzen: Wofür können Sie dieses Wissen einsetzen?
                                                                 • Merksätze: Welche Zusammenhänge müssen Sie
                                                                   sich merken?

                                       Konzepte                  Konzepte und Begriffe der jeweiligen Lerneinheit
                                                                 werden zunächst erläutert. Danach finden Sie Beispiele
                                                                 und Handlungsanleitungen.

                                       Übungen                   • Zu einigen Lerneinheiten finden Sie Übungen mit
                                                                   Aufgabenstellungen und Lösungsvorschlägen.

                                       Querverweisteil          Am Ende jeder Lerneinheit finden Sie einen Abschnitt
                                                                mit Querverweisen, die auf entsprechende
                                                                Beschreibungen in der Softwarereferenz hinweisen.
                                                                 Damit können Sie das neu erworbene Wissen vertiefen.


                                       Lesehinweis
                                       Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der voraus-
                                       gegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinhei-
                                       ten zu überspringen.
                                       Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die
                                       Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten De-
                                       tails zu vergegenwärtigen
                                       Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der
                                       Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht
3,00 / 01-2023




                                       ein roter Faden durch die gesamte Dokumentation.




                 A+W Production Feinplanung                                                                         F-11
                    Dokumentations-Hinweise                                                                        Tutorial




                                          Darstellungskonventionen
                                          Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                                          gende Bedeutung:

                                          Kursiv                   sind Zeichenfolgen ausgezeichet, die Elemente der
                                                                   Software bezeichnen, z. B. der Dialog Gruppierung.

                                          Fett                     sind Zeichenfolgen ausgezeichet, die Sie über die
                                                                   Tastatur eingeben, z. B. geben Sie den Wert 0 ein.

                                          >                        Mit dem sogenannten Brotkrumenpfad ist der Weg
                                                                   gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B.
                                                                   Stammdaten > Feinplanung > Orga.

                                          []                       Eckige Klammern bezeichnen Schaltflächen im Dialog,
                                                                   z. B, mit [OK] speichern Sie die Daten.

                                          <>                       Spitze Klammern bezeichnen Tasten oder
                                                                   Tastenkombinationen auf der Tastatur, z. B. mit <F1>
                                                                   öffnen Sie die Online-Hilfe.
01-2023 / 01-2023




                    F-12                                                                  A+W Production Feinplanung
                 Tutorial                                                                     Überblick Feinplanung




                                       Überblick Feinplanung
                                       Das für die Produktion benötigte Glas wird in der Regel aus Lagerplatten auf
                                       den Schneidtischen zugeschnitten. Häufig gibt es in einem Unternehmen
                                       mehrere automatische Schneidtische sowie mindestens einen Schneidtisch
                                       für Handzuschnitt oder aber auch für Modelle.
                                       Die Scheiben werden nach dem Zuschnitt, in Abhängigkeit von ihrem nächs-
                                       ten Bearbeitungsschritt, auf Abstellplätzen (z. B. A-Böcke) abgestellt und mit
                                       dem Abstellplatz zu ihrer nächsten Bearbeitung bewegt.
                                       Innerhalb eines Arbeitsbereiches (bspw. Zuschnitt) oder einer Prozesskette
                                       (bspw. Zuschnitt > VSG-Linie) kann die Verweil- und Bearbeitungsdauer sehr
                                       unterschiedlich sein. Dies ist unter anderem davon abhängig wie viel Platz in
                                       diesem Bereich für Gestelle zur Verfügung steht um die Gläser abzustellen,
                                       wie kompliziert die Abstelllogik ist und wie weit die Laufwege sind. Diese Fra-
                                       gen sind für die Feinplanung maßgeblich. Wenn z. B. hinter dem Zuschnitt we-
                                       nig Platz für Gestelle ist, muss diese Situation durch eine gute Optimierung
                                       und Sequenz der Scheiben ausgeglichen werden, so dass möglichst wenige
                                       Gestelle benötigt werden und wenig umsortiert werden muss.
                                       Für die Montage an der ISO-Linie müssen die einzelnen Scheiben der Einheit
                                       möglichst nahe beieinander stehen. Sie müssen nicht unbedingt auf einem
                                       Gestell stehen. Das bedeutet, dass, je nach Optimierung, beim Zuschnitt vor
                                       der Linie umsortiert werden muss.




                                          Optimierungsergebnis
                                          Die Optimierung mit dem geringsten Verschnitt kann nicht immer oberstes
                                          Ziel der A+W Production sein. Beispielsweise wenn sie dazu führt, dass
                                          sich der Sortieraufwand vor der Montage unverhältnismäßig erhöht.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                     F-13
                    Überblick Feinplanung                                                                           Tutorial




                                            Ein wichtiges Kriterium für Feinplanungsergebnisse und die Verweil- und Be-
                                            beitungsdauer ist die Laufgröße und -zusammenstellung. Es sind verschiede-
                                            ne Aspekte zu berücksichtigen:
                                            •   Ist die Anzahl der Scheiben im Lauf zu klein oder sind nur sehr große
                                                Scheiben vorhanden, dann ist der Verschnitt zu groß. Die Lagermaße kön-
                                                nen nicht effektiv geschnitten werden, es bleibt ein zu großer Rest.
                                            •   Ist der Lauf dagegen zu groß, d. h. er enthält sehr viele Scheiben, dann ist
                                                die Produktionszeit für den Lauf sehr hoch und die Gestelle bleiben lange
                                                belegt. Gestelle können erst wieder verwendet werden, wenn die Produk-
                                                tion des Laufes abgeschlossen ist.


                                            Ablauf der A+W Production
                                            Die Feinplanung setzt genau dort an, wo die Grobplanung endet. Das Ergeb-
                                            nis der Grobplanung sind die Läufe. Läufe enthalten die zu produzierenden
                                            Teile. Aufgabe der Feinplanung ist es, für die in den Läufen enthaltenen Teile
                                            die Produktionsreihenfolge zu erstellen.
                                            Die Produktionsreihenfolge kann sich durch folgende Kriterien ergeben:
                                            •   Durch die Vorgaben des Kunden,
                                            •   durch die Ergebnisse einer Packmitteloptimierung (PMO) oder
                                            •   durch fertigungstechnische Restriktionen.
                                            Die Feinplanung läuft in verschiedenen Schritten ab. Alle dazu notwendigen
                                            Prozesse (Daten aus der Datenbank laden, etc.) werden in A+W Production
                                            im Hintergrund abgearbeitet und sind für den Benutzer nicht sichtbar. Die
                                            Schritte bauen wie folgt aufeinander auf:
                                            •   Im ersten Schritt werden die Daten aus der Datenbank geladen.
                                            •   Ist dies geschehen, erstellt die Feinplanung anhand der Teile und Bearbei-
                                                tungen die entsprechende Stückliste.
                                            •   Nachdem die Stückliste erstellt ist, weist die Feinplanung die Teile den zur
                                                Verfügung stehenden Orgas und Abstellplatztypen zu.
                                            •   Anschließend erfolgen die Gruppierungen und Sortierungen innerhalb der
                                                Orga-Gruppen und auf den Abstellplätzen.
                                            •   Im nächsten Schritt behandelt die Feinplanung das Abstellen der Scheiben
                                                auf den Abstellplätzen.
                                            •   Dann erfolgt die Bildung der Produktionslose.
                                            •   Im letzten Schritt beschäftigt sich die Feinplanung mit den sogenannten
                                                Sonderteilen (Restscheiben, Füllaufträge, Bruch, etc.).
                                            Damit die für jeden Produktionsschritt gewünschte Reihenfolge auch möglich
                                            ist, müssen die Vorprodukte auf den Abstellplätzen vor diesem Produktions-
                                            schritt in einer passenden Reihenfolge stehen. Die Belegung der Abstellplätze
                                            unmittelbar nach dem jeweiligen Produktionsschritt ist das Ergebnis der Pro-
                                            duktionsreihenfolge.
01-2023 / 01-2023




                                            Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen der ver-
                                            schiedenen Einstellmöglichkeiten in der A+W Production.




                    F-14                                                                    A+W Production Feinplanung
                 Tutorial                                                                         Überblick Feinplanung




                                                                  Reihenfolge




                                       Ausbeute                                              Flexibilität



                                       Sie können lediglich einen Punkt auf den Linien des Dreiecks definieren. Die-
                                       sen Punkt können Sie bewegen, indem Sie mithilfe der A+W Production die
                                       Produktionseinstellungen verändern.
                                       Sie können genau an einem Eckpunkt arbeiten und die anderen beiden außer
                                       Acht lassen. Sie können sich aber auch auf einer Seite bewegen - genau in
                                       der Mitte der beiden angrenzenden Ecken, ohne Berücksichtigung des dritten
                                       Eckpunktes. Eine Produktion unter Berücksichtigung aller drei Eckpunkte
                                       gleichzeitig ist nicht möglich.
                                       •   Sie können mit einer strikten Reihenfolge (an einem Eckpunkt) arbeiten -
                                           dies geht zu Lasten der Flexibilität und liefert ein schlechtes Ergebnis.
                                       •   Sie können mit einer Kombination von Reihenfolge und unbedingte Aus-
                                           beute (auf einer Seite) arbeiten - sind dann aber nicht mehr flexibel.
                                       •   …
                                       Wir werden dieses Schema innerhalb der Dokumentation immer wieder ver-
                                       wenden.


                                       Ergänzende Informationen
                                        Tutorial, “Begriffe der A+W Production” auf Seite F-16
3,00 / 01-2023




                 A+W Production Feinplanung                                                                       F-15
                    Überblick Feinplanung                                                                          Tutorial




                                            Begriffe der A+W Production
                                            Innerhalb der A+W Production werden folgende Begriffe verwendet:
                                            •   Lostyp
                                            •   Lose
                                                – Verwendungslos
                                                – Produktionslos
                                            •   Böcke (Abstellplätze)
                                                – Verwendungsbock
                                                – Produktionsbock
                                            •   Läufe
                                            •   Teilebaum
                                            •   Organisation (Orga)


                                            Lostyp
                                            Der Lostyp wird durch die Eigenschaften Bearbeitungstyp und Beschaffungs-
                                            art gebildet.




                                            Abb. F-1     Schematische Darstellung der Lostypen Zuschnitt und Lagerentnahme
01-2023 / 01-2023




                    F-16                                                                   A+W Production Feinplanung
                 Tutorial                                                                    Überblick Feinplanung




                                       Lose
                                       Ein Los ist eine Anzahl an Scheiben, welche innerhalb eines Zeitraums unter
                                       den gleichen Bedingungen auf den gleichen Maschinen verwendet oder pro-
                                       duziert werden. Ein Los enthält eine Anzahl von Scheiben eines Lostyps. In
                                       der A+W Production gibt es zwei Arten von Lostypen:
                                       •   Verwendungslos
                                       •   Produktionslos

                                       Verwendungslos
                                       Scheiben eines Verwendungsloses werden zur Fertigung von in Läufen be-
                                       findlichen Scheiben benötigt. Alle in diesem Los enthaltenen Scheiben haben
                                       den gleichen Lostyp.

                                       Produktionslos
                                       Scheiben eines Produktionsloses werden im dazugehörigen Lauf produziert.
                                       Alle Scheiben darin haben den gleichen Lostyp. Scheiben eines Produktions-
                                       loses werden auf den gleichen Maschinen produziert. Scheiben für eine ande-
                                       re Maschine kommen in ein anderes Los vom gleichen Typ. Ferner können
                                       Produktionslose noch nach weiteren Kriterien getrennt werden. So wäre es
                                       zum Beispiel denkbar, die Produktion für ISO-Einheiten nach dem Scheiben-
                                       zwischenraum (SZR) zu trennen. Dadurch würden mehrere Produktionslose
                                       gebildet, von denen jedes nur Scheiben für einen bestimmten Scheibenzwi-
                                       schenraum enthält.


                                       Ergänzende Informationen
                                        Abb. F-2 auf Seite F-18


                                       Böcke (Abstellplätze)
                                       Teile eines Laufes können nach dem Zuschnitt unterschiedlich bearbeitet wer-
                                       den. Dazu werden die Teile auf Böcke (Abstellplätze) für die nächste Bearbei-
                                       tung gestellt. Sie gehören immer einem Verwendungslos an, d. h. es sind
                                       Scheiben, die zur Produktion benötigt werden. Deshalb müssen sie auf den
                                       Verwendungsböcken so stehen, dass für den nächsten Bearbeitungsprozess
                                       die gewünschte Produktionsreihenfolge eingehalten werden kann.
                                       Die A+W Production unterscheidet zwischen
                                       •   Verwendungsbock
                                       •   Produktionsbock

                                       Verwendungsbock
                                       Teile eines Laufes können nach dem Zuschnitt unterschiedlich bearbeitet wer-
                                       den. Dazu werden die Teile auf einen Verwendungsbock (Abstellplatz) für die
                                       nächste Bearbeitung gestellt. Sie gehören immer einem Verwendungslos an,
                                       d. h. es sind Scheiben, die zur Produktion benötigt werden. Deshalb müssen
3,00 / 01-2023




                                       sie auf den Verwendungsböcken so stehen, dass für den nächsten Bearbei-
                                       tungsprozess die gewünschte Produktionsreihenfolge eingehalten werden
                                       kann.


                 A+W Production Feinplanung                                                                   F-17
                    Überblick Feinplanung                                                                           Tutorial




                                                                 Bearbeitung


                                                                                Verwendungslos
                                                                Verwendungs-
                                                                    bock


                                                                 Produktions-   Produktionslos
                                                                     bock
                                             Zeit




                                                                 Bearbeitung



                                                                                Verwendungslos
                                                                Verwendungs-
                                                                    bock



                                            Abb. F-2         Übersicht Produktions- und Verwendungsbock


                                            Produktionsbock
                                            Auf dem Produktionsbock werden Scheiben unmittelbar nach ihrer Produktion
                                            abgestellt. Sie stehen auf dem Bock in der Reihenfolge, in der sie aus der Pro-
                                            duktion kamen. Es handelt sich dabei stets um Scheiben in einem Produktion-
                                            slos. Produktionsböcke müssen in der A+W Production nicht zwingend
                                            verwendet werden, man kann die Scheiben nach der Produktion auch direkt
                                            auf einen Verwendungsbock für die nächste Bearbeitung stellen.

                                                    Produktions- und Verwendungsböcke
                                                    In der A+W Production kann für jeden Bearbeitungsschritt eine unter-
                                                    schiedliche Gruppierung/Sortierung verwendet werden. Es ist nicht mög-
                                                    lich, einem Produktionsbock einfach eine andere Nummer zu geben und
                                                    ihn als Verwendungsbock für den nächsten Bearbeitungsschritt zu neh-
                                                    men. Wenn Scheiben direkt nach der Bearbeitung statt auf einem Produk-
                                                    tionsbock auf einen Verwendungsbock gestellt werden, müssen sie so
                                                    angeordnet werden, dass die Produktionsreihenfolge des nächsten Bear-
                                                    beitungsschritts eingehalten werden kann.


                                            Ergänzende Informationen
                                             Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135


                                            Läufe
                                            Läufe enthalten eine Menge von Auftragspositionen, die gemeinsam für die
                                            Produktion frei gegeben und gemeinsam produziert werden.
01-2023 / 01-2023




                                            Läufe archivieren
                                            Läufe, die Sie nicht mehr im Produktionssystem benötigen, können archiviert
                                            werden. In der Anzeige Läufe können Sie über das Kontextmenü (Lauf verwal-



                    F-18                                                                         A+W Production Feinplanung
                 Tutorial                                                                      Überblick Feinplanung




                                       ten > Lauf archivieren) den ausgewählten Lauf bzw. die ausgewählten Läufe
                                       auf archivierbar setzen. Archivierte Läufe erhalten dann den Laufstatus 2000.
                                       Es gibt 2 Arten der Archivierung:
                                       •   Manuelle Archivierung
                                       •   Automatische Archivierung

                                       Manuelle Archivierung
                                       Die Einstellungen für die manuelle Archivierung befinden sich im Parameter-
                                       Administrator unter:
                                       Parameter > A+W Production > Allgemein > ALCIM Server > Automatische
                                       Laufarchivierung
                                       Der Eintrag für die manuelle Archivierung ist die 0.
                                       Nachdem der Lauf archiviert wurde, hat er den Status archivierbar. Ob ein
                                       Lauf tatsächlich archiviert wird oder stattdessen gelöscht werden soll, kann in
                                       der Systemkonfiguration definiert werden. Zum Archivieren eines Laufes ist
                                       eine Archivdatenbank und ein Prozess (ALCIM Server) notwendig. Dieser
                                       Prozess kann manuell gestartet werden oder ist als Automatismus im Hinter-
                                       grund konfiguriert.


                                        So archivieren Sie einen Lauf
                                       1 Öffnen Sie die Ansicht Läufe.
                                       2 Markieren Sie den Lauf, den Sie archivieren oder löschen möchten.
                                       3 Öffnen Sie das Kontext-Menü und wählen Sie Lauf verwalten > Lauf archi-
                                         vieren.
                                       4 Es folgt eine Sicherheits-Abfrage, ob Sie den Lauf wirklich archivieren
                                         möchten.




                                       5 Klicken Sie auf [OK] um den Lauf zu archivieren.
                                       6 Anschließend hat der Lauf den Status archivierbar.

                                       Automatische Archivierung
                                       Neben der manuellen Archivierung gibt es 3 weitere Archivierungsmodi, die
3,00 / 01-2023




                                       sich auf die Laufstati produziert (700), verpackt (800) und versendet (900) be-
                                       ziehen. Diese Laufstati werden automatisch vom AlcimBooking gesetzt, so-



                 A+W Production Feinplanung                                                                     F-19
                    Überblick Feinplanung                                                                          Tutorial




                                            bald alle Kopfteile in dem Lauf die Bearbeitungen für produziert, verpackt oder
                                            versendet erhalten haben.
                                            Die Einstellungen für die automatische Archivierung befinden sich im Parame-
                                            ter-Administrator unter:
                                            Parameter > A+W Production > Allgemein > ALCIM Server > Automatische
                                            Laufarchivierung
                                            Hier können Sie unterscheiden zwischen:
                                            •   Läufe werden automatisch archiviert, wenn der Status produziert erreicht
                                                ist.
                                            •   Läufe werden automatisch archiviert, wenn der Status verpackt erreicht ist.
                                            •   Läufe werden automatisch archiviert, wenn der Status versendet erreicht
                                                ist.

                                                Buchungsdisziplin
                                                Die automatische Archivierung basiert auf BDE-Buchungen und ist daher
                                                von der Buchungsdisziplin abhängig. Sobald ein Kopfteil in einem Lauf
                                                nicht den entsprechenden Status erreicht, kann der Laufstatus nicht ge-
                                                setzt und damit die automatische Archivierung angestoßen werden. Inso-
                                                fern ist darauf zu achten, dass besonders die Kopfteile vollständig gebucht
                                                werden.

                                                Grundsätzlich gilt: eine vollständige Archivierung eines Laufes kann erst
                                                erfolgen, wenn abhängige Läufe (enthalten gemeinsame Auftragspositio-
                                                nen) sich ebenfalls in diesem Satus befinden.

                                            Archivierungsmethode
                                            In diesem Bereich wählen Sie, mit welcher Archivierungsmethode gearbeitet
                                            werden soll. Es steht die alte Archivierungsmethode (die standardmäßig ein-
                                            gestellt ist und verwendet wird) zur Verfügung und der neuen erweiterten, der
                                            weniger restriktiv ist und es erlaubt, mehr Läufe zu archivieren und freizuge-
                                            ben.
                                            Die Einstellungen für die Archivierungsmethode befinden sich im Parameter-
                                            Administrator unter:
                                            Parameter > A+W Production > Allgemein > ALCIM Server > Archivierungs-
                                            methode
                                            Hier können Sie unterscheiden zwischen:
                                            0: Standard-Archivierungsmethode. Diese Methode arbeitet nur aufgrund des
                                            Status eines Laufes.
                                            1: Erweiterte Prüfung der Läufe. Hier werden zusätzlich Flags der Aufträge in
                                            einem Lauf berücksichtigt, um zu prüfen, ob ein Auftrag archiviert werden
                                            kann. Diese Methode ist weniger restriktiv als die ursprüngliche Methode und
                                            erlaubt es, mehr Läufe zu archivieren und freizugeben. Der dieser Methode
                                            zugrunde liegende Parameter sagt dem AlcimServer, ab welchem Status ein
01-2023 / 01-2023




                                            Lauf als archivierungsfähig betrachtet werden soll. Der Wert der Automatische
                                            Laufarchivierung kann
                                            •   1=Status 700 (produziert),



                    F-20                                                                    A+W Production Feinplanung
                 Tutorial                                                                         Überblick Feinplanung




                                       •   2=Status 800 (verpackt),
                                       •   3=Status 900 (geliefert) oder
                                       •   0=Status 2000 (manuell als archivierbar gesetzt)
                                       sein.
                                        Tutorial, “Automatische Archivierung” auf Seite F-19

                                       Funktionsweise Standard Archivierungsmethode (0)
                                       Wie bereits oben erwähnt, arbeitet die Standard-Methode nur aufgrund des
                                       Status eines Laufes. Im folgenden Beispiel wird dies deutlich:
                                       •   Lauf: 1000
                                       •   Status: 900 (versendet)
                                       •   Konfigurationsparameter Automatische Laufarchivierung: 3 (Läufe werden
                                           automatisch archiviert, wenn Status versendet erreicht ist)




                                       Abb. F-3     Standard-Archivierungsmethode


                                       Funktionsweise: Wenn der AlcimServer den Lauf 1000 (Spalte A) mit einem
                                       Status gleich oder größer als 3 (Status 900, versendet) verarbeitet, prüft er im
                                       1. Schritt alle Aufträge des Laufes 1000 (Spalte D). Im 2. Schritt prüft er, in wel-
                                       chen anderen Läufen diese enthalten sind (Spalte F) und im 3. Schritt, ob die
                                       Läufe alle einen Status gleich oder größer Status 3 haben.
                                       In Beispiel oben kann der Auftrag 2000001 nicht archiviert werden. Er enthält
                                       neben Lauf 1001 noch Lauf 1002 und dieser Lauf hat nur den Status 700 (pro-
                                       duziert). Da dieser kleiner als "Archivierbarer Status" ist, kann auch Lauf 1000
                                       nicht archiviert werden

                                       Funktionsweise Erweiterte Archivierungsmethode (1)
                                       Diese neue Methode wurde geschaffen, um mehr Läufe archivieren zu kön-
                                       nen.
                                       Die Methode ermöglicht die Archivierung von Aufträgen, die als abgeschlos-
                                       sen betrachtet werden können, auch wenn sie in einem anderen Lauf mit ei-
                                       nem Status niedriger als Archivierbarer Status, aber mit einem Status gleich
                                       oder höher als 700 (produziert) enthalten sind.
                                       Beispiel:
                                       •   Lauf: 1000
3,00 / 01-2023




                                       •   Status: 900
                                       •   Konfigurationsparameter Automatische Laufarchivierung: 3 (Läufe werden
                                           automatisch archiviert, wenn Status versendet erreicht ist)


                 A+W Production Feinplanung                                                                          F-21
                    Überblick Feinplanung                                                                            Tutorial




                                            Abb. F-4     Erweiterte Archivierungsmethode (1)


                                            Wenn der Status des Laufes 700 oder größer ist und kleiner als Archivierbarer
                                            Status, dann müssen auch andere Datensätze aus pool_teile und pool_auf-
                                            trag zusätzlich analysiert werden.
                                            Ein Teil eines Auftrags 2000001 [Spalte D], der in dem Lauf 1001 [Spalte F]
                                            enthalten ist, muss nicht analysiert werden, da der Status [Spalte G] dieses
                                            Laufes gleich oder größer als Archivierbarer Status ist.
                                            Aber ein anderer Teil des Auftrags 2000001 [Spalte D], der in dem Lauf 1002
                                            [Spalte F] enthalten ist, muss analysiert werden, weil der Status [Spalte G] die-
                                            ses Laufes 700 oder größer und kleiner als Archivierbarer Status ist.
                                            Wie man im Vergleich zur Standardmethode sehen kann, berücksichtigt die
                                            neue Methode den Auftrag 2000001 [Spalte D] als archivierbar und somit kann
                                            der Lauf 1000 archiviert werden.
01-2023 / 01-2023




                    F-22                                                                       A+W Production Feinplanung
                 Tutorial                                                                          Überblick Feinplanung




                                       Teilebaum
                                       Der Teilebaum beschreibt den Aufbau und die Produktionsschritte für ein Pro-
                                       dukt. Das fertige Produkt (ISO) bildet dabei den Kopf des Teilebaums, seine
                                       zur Produktion benötigten Unterteile (ESG und Float) werden im Teilebaum
                                       darunter angeordnet, deren Unterteile (Float) wiederum darunter. Dies wird
                                       solange fortgesetzt, bis die Basisteile (in der Regel Float) erreicht sind. Im Tei-
                                       lebaum befinden sich nicht nur Teile, sondern auch deren Bearbeitungen.


                                                       ISO




                                              ESG                 Float



                                              Ofen


                                              Float


                                       Abb. F-5        Teilebaum


                                       Organisation (Orga)
                                       Um einen Lauf korrekt und effizient planen zu können, stehen Ihnen in A+W
                                       Production sogenannte Orgas zur Verfügung. Eine Orga ist nichts anderes als
                                       ein datentechnisches Regelwerk zur Abbildung der Produktion. In Abhängig-
                                       keit von der Struktur des Unternehmens können beliebig viele Orgas (ESG-
                                       Orga, ISO-Orga, Bearbeitungs-Orga, etc.) definiert werden. Die unterschiedli-
                                       chen Orgas organisieren die Abstellplätze jeweils vor den Produktionsschrit-
                                       ten (ISO-Linie, Ofen, etc.).


                                         Master-Orga

                                                        Orga 1


                                                        Orga 2

                                                                 Orga-Gruppe 1

                                                                 Orga-Gruppe 2

                                                                          Bocktyp 1

                                                                          Bocktyp 2

                                                                 Orga-Gruppe 3
3,00 / 01-2023




                                       Abb. F-6        Schematische Darstellung der Organisation




                 A+W Production Feinplanung                                                                         F-23
                    Gruppierungen und Sortierungen                                                          Tutorial




                                           Gruppierungen und Sortie-
                                           rungen
                                           In diesem Themenblock lernen Sie die unterschiedlichen Gruppierungen und
                                           Sortierungen kennen und erfahren, wie Sie damit in der A+W Production um-
                                           gehen.
                                           Der Themenblock beinhaltet folgende Schulungseinheiten:
                                           •   Einführung
                                           •   Gruppierung
                                           •   Sortierung
                                           •   Zusatz-Sortierung
                                           •   Demos und Übungen
01-2023 / 01-2023




                    F-24                                                               A+W Production Feinplanung
                 Tutorial                                                             Gruppierungen und Sortierungen




                                       Überblick
                                       Lernziele

                                       •   Gruppierungen kennenlernen und verstehen.
                                       •   Sortierungen kennenlernen und verstehen.
                                       •   Zusatz-Sortierungen kennenlernen und verstehen.
                                       •   Die Auswirkungen von Gruppierungen und Sortierungen verstehen.


                                       Nutzen

                                       Über die Gruppierungen und Sortierungen wird das Abstellen der einzelnen Scheiben
                                       in der von Ihnen gewünschten Reihenfolgen organisiert. Ohne diese Gruppierungen
                                       und/oder Sortierungen müssten die Scheiben vor dem jeweiligen nächsten
                                       Produktionsschritt immer neu sortiert werden.


                                       Definitionen

                                       Gruppierung                Erfolgt nach unterschiedlichen und eindeutigen Werten
                                                                  für eine Eigenschaft, z. B. nach Kundennummer,
                                                                  Glasdicke.

                                       Sortierung                 Erfolgt nach Eigenschaften, die einen fortlaufenden Wert
                                                                  innerhalb der gegebenen Gruppe annehmen.

                                       Abstellplatz               Gestell (A-Bock, Fächerwagen, Fester Abstellplatz)

                                       Bock                       Umgangssprachlich für Abstellplatz.


                                       Merke

                                       Bildung                    Gruppierungen oder Sortierungen werden durch eine
                                                                  beliebige Kombination aus Eigenschaften und Formeln
                                                                  gebildet.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                            F-25
                    Gruppierungen und Sortierungen                                                                  Tutorial




                                           Einführung
                                           Die Gruppierungen und Sortierungen dienen dazu, den verschiedenen Ab-
                                           stellplätzen die gewünschte Produktionsreihenfolge zuzuweisen. Gruppierun-
                                           gen können auch verwendet werden, um Scheiben vom gleichen Lostyp auf
                                           verschiedene Produktionslose zu verteilen.
                                           A+W Production erlaubt es Ihnen, Gruppierungskriterien zu definieren und
                                           gibt Ihnen die Möglichkeit zu entscheiden, ob die Gruppierung in einer gewis-
                                           sen Reihenfolge (sortierte Gruppen) sein soll und ob die Inhalte der Gruppen
                                           sortiert sein sollen (Sortierung innerhalb der Gruppe). Jeder Abstellplatztyp in-
                                           nerhalb einer Organisation kann seine eigene Gruppierung und Sortierung ha-
                                           ben.
                                           Die Optimierung berechnet unter Berücksichtigung von Gruppierung und Sor-
                                           tierung den bestmöglichen Verschnitt. Einmal eingerichtet, kann die so ermit-
                                           telte Reihenfolge für passende Scheiben einer ISO- und VSG-Einheit
                                           verwendet werden.
                                           Jede Scheibe bzw. jede Bearbeitung hat eine Anzahl von Eigenschaften, die
                                           entweder durch die entsprechenden Felder in der Datenbank gefüllt oder be-
                                           rechnet werden.

                                                               Gruppiert nach Glasart




                                            Sortiert nach Abmessung

                                           Abb. F-7     Gruppierung und Sortierung


                                           Die Grafik oben zeigt eine Gruppierung nach der Glasdicke. Innerhalb jeder
                                           Gruppe (eventuell ein Gestell pro Dicke) erfolgt die Sortierung nach der Höhe.
                                           Gruppierung und Sortierung hängen davon ab, wie die Produktion in Ihrem
                                           Hause aufgebaut ist und abläuft. Sie werden durch eine beliebige Kombinati-
                                           on aus Eigenschaften und Formeln gebildet. Die Einstellungen werden im
                                           Menü Stammdaten, in den Untermenüs Orga, Gruppierung und Abstellplätze
                                           vorgenommen.


                                           Ergänzende Informationen
                                            Tutorial, “Gruppierung” auf Seite F-24
                                            Tutorial, “Sortierung” auf Seite F-25
01-2023 / 01-2023




                    F-26                                                                    A+W Production Feinplanung
                 Tutorial                                                         Gruppierungen und Sortierungen




                                       Gruppierung
                                       Gruppiert wird nach unterschiedlichen und eindeutigen Werten für eine Eigen-
                                       schaft wie z.B. nach Kundennummer, Glasdicke/-farbe, Modelltyp. Es kann
                                       nach unterschiedlichen Kriterien gruppiert werden, ohne dass innerhalb der
                                       Gruppen eine Sortierung vorhanden sein muss. Jede Gruppe enthält aus-
                                       schließlich Elemente, die die Eigenschaften des Gruppierungsschlüssels ent-
                                       halten. Gruppen müssen während des Laufs durch die Produktion
                                       zusammengehalten werden.
                                       Die entsprechenden Einstellungen werden im Dialog Gruppierung/Sortierung
                                       gemacht:
                                       Stammdaten > Feinplanung > Gruppierung




                                       Abb. F-8    Gruppierung


                                        So legen Sie eine neue Gruppierung an
                                       1 Wählen Sie im Menü Stammdaten > Feinplanung > Gruppierung.
                                          Der Dialog Gruppierung/Sortierung wird geöffnet. Das Register Sortierung
                                          wird automatisch geöffnet.
                                       2 Markieren Sie im linken Bereich den Eintrag Gruppierungen.
                                       3 Über die Checkboxen Eigenschaft und Formel bestimmen Sie, ob es sich
                                         bei der Sortierung um eine Eigenschaft oder eine Formel handelt.
                                       4 Wählen Sie die entsprechende Eigenschaft oder Formel aus.
                                       5 Betätigen Sie die Schaltfläche [Hinzufügen].
                                       6 Der Eintrag wird der Liste auf der linken Seite am Ende hinzugefügt.
3,00 / 01-2023




                                       Die erstellte Gruppierung kann nun für Einstellungen in den Orgas genutzt
                                       werden.



                 A+W Production Feinplanung                                                                     F-27
                    Gruppierungen und Sortierungen                                                                                             Tutorial




                                           Ergänzende Informationen
                                            Tutorial, “Einführung” auf Seite F-23
                                            Softwarereferenz, “Gruppierung/Sortierung - Dialog” auf Seite F-140


                                           Sortierung
                                           Sortiert werden kann nach Eigenschaften, die einen fortlaufenden Wert an-
                                           nehmen. Eine typische Art der Sortierung ist z. B. nach Größe. Sortiert wird
                                           innerhalb der gegebenen Gruppen. Die Sortierungen können noch bei Bedarf
                                           durch die Werte im letzten Teil des Sortierungsschlüssel verfeinert werden.

                                                                          Reihenfolge der Gruppen

                                                               sortiert                    nicht sortiert                  nicht sortiert
                                              Kunde # 15




                                                                             Kunde # 20




                                                                                                            Kunde # 35
                                                           Gruppe 1                       Gruppe 2                        Gruppe 3

                                                                                                                         Glas: Float 4 mm

                                           Abb. F-9             Gruppierung und Sortierung


                                           Wie Sie an der Grafik oben erkennen können, können Sie auch eine Reihen-
                                           folge von Gruppen definieren.

                                               Supergruppen
                                               Die Optimierung verwendet den Begriff Supergruppe. Eine Supergruppe
                                               kann sich aus Scheiben zusammensetzen, die alle identisch bzgl. des
                                               Gruppierungsschlüssel oder des kombinierten Gruppierungs-/Sortierungs-
                                               schlüssel sind.

                                           Die Scheiben innerhalb einer Gruppe können, müssen aber nicht sortiert sein.
                                           Die entsprechenden Einstellungen werden im Dialog Gruppierung/Sortierung
                                           gemacht:
                                           Stammdaten > Feinplanung > Gruppierung > Register Sortierung
01-2023 / 01-2023




                    F-28                                                                                                    A+W Production Feinplanung
                 Tutorial                                                         Gruppierungen und Sortierungen




                                       Abb. F-10   Sortierung


                                        So legen Sie eine neue Sortierung an
                                       1 Wählen Sie im Menü Stammdaten > Feinplanung > Gruppierung.
                                          Der Dialog Gruppierung/Sortierung wird geöffnet. Wechseln Sie in das Re-
                                          gister Gruppierung.
                                       2 Markieren Sie im linken Bereich den Eintrag Sortierung.
                                       3 Über die Checkboxen Eigenschaft und Formel bestimmen Sie, ob es sich
                                         bei der Gruppierung um eine Eigenschaft oder eine Formel handelt.
                                       4 Wählen Sie die entsprechende Eigenschaft oder Formel aus.
                                       5 Betätigen Sie die Schaltfläche [Hinzufügen].
                                       6 Der Eintrag wird der Liste auf der linken Seite am Ende hinzugefügt.


                                        So fügen Sie einer bestehenden Sortierung eine Eigenschaft hinzu
                                       1 Wählen Sie in der Menü-Leiste Stammdaten > Feinplanung > Gruppierung
                                         > Editor-Sortierung.
                                       2 Aktivieren Sie die Radiotaste Eigenschaften.
                                       3 Markieren Sie im rechten Fenster die für die Sortierung gewünschte Eigen-
                                         schaft.
                                       4 Markieren Sie im linken Fenster die Sortierung, der die Eigenschaft hinzu-
                                         gefügt werden soll.
                                       5 Betätigen Sie die Schaltfläche [Hinzufügen]. Die neu hinzugefügte Eigen-
                                         schaft erscheint in der bereits angelegten.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                     F-29
                    Gruppierungen und Sortierungen                                                                Tutorial




                                            Einen neuen Modus für die Gruppenbildung erstellen
                                              Als Beispiel wird hier eine Gruppierung nach Anzahl der Scheiben pro Kun-
                                              de erstellt. Das bedeutet es wird eine Gruppe pro Kunde erstellt und diese
                                              Gruppen nach der Zahl der in ihnen enthaltenen Scheiben sortiert. Zuerst
                                              produziert wird dann die Gruppe mit der größten Anzahl an Scheiben:
                                           1 Wählen Sie in der Menü-Leiste Stammdaten > Feinplanung > Gruppierung
                                           2 Aktivieren Sie die Radiotaste Formel und betätigen Sie anschließend die
                                             Schaltfläche [Formeln …]. Es öffnet sich der Dialog Auswahl Formeln --1--
                                           3 Wählen Sie die Schaltfläche [Neue Formel …]. Es öffnet sich der Dialog
                                             Formel --- Editor.
                                           4 Im Formeleditor geben Sie jetzt oben links den Namen der Gruppierung ein
                                             (für unser Beispiel: Menge der Scheiben pro Kunde).
                                           5 Im Bereich Vorhandene Formeln suchen Sie Menge und klicken doppelt
                                             darauf. Die Formel #Menge# wird in den Bereich Formel übernommen.
                                           6 Wählen Sie die Schaltfläche [Menge]. Es öffnet sich der Dialog Auswahl
                                             Mengen -- 1 --.
                                           7 In diesem Dialog können links oben schon gebildete Mengen (im Sinne der
                                             Mengenlehre) ausgewählt werden. Wir bilden eine neue Menge und kli-
                                             cken auf [Neue Menge …]. Es öffnet sich der Dialog Mengen - Erzeuger.
                                           8 Wir beginnen die Mengen - Erzeugung mit einer gegebenen Menge und
                                             bekommen nach den Mengenoperationen, die wir hier durchführen, unsere
                                             gewünschte endgültige Menge. An den Formelinterpreter wird von der
                                             Feinplanung an Werten übergeben eine Position eines bestimmten Kun-
                                             den, die Mengenkalkulation der Feinplanung und als weiteren Parameter
                                             alle Aufträge des aktuellen Laufs. Von uns muss nur noch die Kundennum-
                                             mer hinzugefügt werden.
                                             Wählen Sie Menge > Name. Es öffnet sich der Dialog Name der Menge.
                                             Sie geben im Bereich Neue Bezeichnung einen sprechenden Namen für
                                             die Menge an. Wählen Sie [OK]. Der Dialog wird geschlossen.
                                           9 Wählen Sie Menge > Übergebene Menge. Dies bewirkt, dass bei der Bil-
                                             dung unserer Menge nicht nur die Position, mit der wir in Mengen - Erzeu-
                                             ger gekommen sind, selbst berücksichtigt wird, sondern alle Positionen
                                             des Laufs.
                                           10 Da die gewünschte Menge nicht alle Teile enthalten soll, sondern nur die
                                              Freigabeteile, aktivieren Sie die Checkbox Master. Für Erklärungen zu den
                                              anderen Möglichkeiten siehe
                                           11 Um unserer Menge die Kundennummer als Eigenschaft hinzuzufügen,
                                              wählen Sie Menge > Formel. Es öffnet sich der Dialog Auswahl Formeln -
                                              -2--. Der Bereich Vorhandene Formeln gibt Ihnen wieder einen Überblick
                                              zu allen bereits definierten Formeln. Sollte die Kundennummer hier noch
                                              nicht vorhanden ist, klicken Sie auf [Neue Formel …]. Es öffnet sich der Di-
                                              alog Formel - Editor. Geben Sie im Formel-Editor einen Namen für die For-
01-2023 / 01-2023




                                              mel ein, wählen Sie aus dem Bereich Vorhandene Eigenschaften
                                              KUNDENNUMMER aus klicken diese Eigenschaft doppelt an. Die Eigen-
                                              schaft erscheint dann im Bereich Formel. Betätigen Sie [OK], um die For-
                                              mel zu erstellen.



                    F-30                                                                   A+W Production Feinplanung
                 Tutorial                                                            Gruppierungen und Sortierungen




                                       12 Schließen Sie den Dialog Auswahl Formeln --2-- ebenfalls mit [OK].
                                       13 Im Dialog Mengen-Erzeuger wird jetzt unten rechts angezeigt, dass wir die-
                                          se Formel bei der Bildung der neuen Menge benutzen. Bei der Bildung der
                                          gewünschten Menge benutzen wir keine Bedingung. Bedingungen werden
                                          auch über den Menüpunkt Menge gebildet. Der Unterschied von Formel
                                          und Bedingung bei Mengenoperationen besteht darin, dass eine Bedin-
                                          gung immer einen absoluten Wert enthält, während sich dieser bei der For-
                                          mel auf eine bestimmte Position bezieht und so unterschiedliche Werte
                                          annehmen kann.
                                       14 Schließen Sie jetzt alle geöffneten Dialoge mit [OK], bis Sie sich wieder im
                                          Ausgangsdialog Gruppierung/Sortierung befinden. Dort markieren Sie die
                                          neue Formel (Menge der Scheibe pro Kunde) und betätigen die Schaltflä-
                                          che [Hinzufügen].
                                       15 Im Dialog Orga-Gruppen und Einstellungen – Abstellplatz erscheint nun
                                          die erstellte Gruppierung (Menge der Scheiben pro Kunde) im Bereich Bil-
                                          dung der Gruppen und kann entsprechend verwendet werden.


                                       Ergänzende Informationen
                                        Tutorial, “Sortierung” auf Seite F-25
                                        Softwarereferenz, “Gruppierung/Sortierung - Dialog” auf Seite F-140


                                       Zusatz-Sortierung
                                       Die Zusatz-Sortierungen können nur auf die Sortierungen angewendet wer-
                                       den. Zweck der Zusatz-Sortierungen ist es, vorhandene Sortierung in Abhän-
                                       gigkeit des Werts des letzten Elements ergänzen zu können. Zum Beispiel
                                       könnte eine Sortierung nach Tour, Kunde und xxxxx gewünscht sein, aber für
                                       jeden Kunden soll dieses xxxxx anders aussehen können. Daher wird zu-
                                       nächst eine Sortierung nach Tour und Kunde angelegt und danach alle er-
                                       wünschten Sortierungen erzeugt, die für das xxxxx benötigt werden. Danach
                                       kann diese Zusatz-Sortierung der Sortierung nach Tour und Kunde in Abhän-
                                       gigkeit der Kundennummer zugewiesen werden. Sollte für eine gegebene
                                       Kundennummer keine Zusatz-Sortierung vorhanden sein, so findet eine wei-
                                       tergehende Sortierung nicht statt.


                                        So erstellen Sie eine Zusatz-Sortierung
                                          Beispiel: Einer existierenden Sortierung nach Tour und Kunde wird eine
                                          Zusatz-Sortierung nach Auftragsnummer und Positionsnummer für den
                                          Kunden mit der Kundennummer 11 hinzugefügt.
                                       1 Wählen Sie in der Menü-Leiste Stammdaten > Feinplanung > Gruppierung
                                         > Editor-Sortierung.
                                       2 Aktivieren Sie die Radiotaste Eigenschaften.
                                       3 Markieren Sie im linken Fenster die Sortierung (+Auftragsnummer+Positi-
                                         onsnummer), für die die Zusatz-Sortierung erstellt werden soll.
3,00 / 01-2023




                                       4 Markieren Sie im rechten Fenster die Eigenschaft der Zusatz-Sortierung
                                         (Kundennummer).




                 A+W Production Feinplanung                                                                     F-31
                    Gruppierungen und Sortierungen                                                                   Tutorial




                                           5 Betätigen Sie die Schaltfläche [Erzeuge Zusatzsortierung]. Es öffnet sich
                                             der Dialog Erzeugung einer Zusatz-Sortierung.
                                               Softwarereferenz, “Erzeugung einer Zusatz-Sortierung” auf Seite F-145
                                           6 Im Feld Wert geben Sie den Wert für das Sortierungselement an (in unse-
                                             rem Beispiel 11).
                                               Softwarereferenz, “Wert” auf Seite F-144
                                           7 Aktivieren Sie die Radiotaste Ziffer.
                                           8 Betätigen Sie die Schaltfläche [Ok]. Der Dialog wird geschlossen.
                                           9 Öffnen Sie das Register Zusatz-Sortierungen. Die erstellte Zusatz-Sortie-
                                             rung wird angezeigt (in unserem Beispiel: Schlüssel: Kundennummer,
                                             Wert: 11, Zusatzsortierung: +Auftragsnummer+Positionsnummer).


                                           Ergänzende Informationen:
                                            Tutorial, “Gruppierung” auf Seite F-24
                                            Softwarereferenz, “Erzeugung einer Zusatz-Sortierung” auf Seite F-145
01-2023 / 01-2023




                    F-32                                                                    A+W Production Feinplanung
                 Tutorial                                                          Gruppierungen und Sortierungen




                                       Sonderteile
                                       Für Sonderteile gibt es keine Gruppierung oder Sortierung, da auf einem Ab-
                                       stellplatz immer nur eine Position steht.
                                       Es gibt folgende Sonderteile:
                                       •   Füllaufträge
                                       •   Restscheiben
                                       •   Bruchscheiben
                                       •   Eilscheiben

                                       Füllaufträge
                                       Füllaufträge sind Scheiben, die nicht fest einem Lauf zugeordnet sind, son-
                                       dern von der Optimierung dazu verwendet werden dürfen, den Verschnitt zu
                                       verbessern. Diese Füllaufträge liegen in der Datenbank in der Tabelle
                                       POOL_TEILE, wo sie durch die Laufnummer 10003 spezifiziert sind. Die A+W
                                       Production verfügt über eine spezielle Anzeige für Füllaufträge, die sogenann-
                                       te Füllauftrag-Anzeige. Die Füllauftrag-Anzeige wird nicht standardmäßig an-
                                       gezeigt, sondern muss vom Benutzer aktiviert werden.

                                           Füllaufträge anzeigen
                                           Damit vorhandene Füllaufträge verwendet und im Register Spezial des Di-
                                           alogs Feinplanung für Lauf … angezeigt werden können, muss im Dialog
                                           Master-Orga der Bereich Verwende Füller aktiviert und die entsprechen-
                                           den Abstellplätze angegeben sein!

                                           Möchten Sie Änderungen an den Einstellungen vornehmen, wenden Sie
                                           sich vorher bitte unbedingt an A+W, da es sonst zu unerwünschten Ergeb-
                                           nissen kommen kann!


                                        So aktivieren Sie die Füllauftrag-Anzeige
                                       1 Wählen Sie im Menü Stammdaten > Konfiguration. Es öffnet sich der Dia-
                                         log Parameter-Administrator.
                                       2 Wählen Sie im Bereich A+W Production, Allgemein Ihre Station.
                                       3 Scrollen Sie auf der rechten Seite in den Bereich Programm Menü.
                                       4 Markieren Sie die darunter liegende Zeile (Menü).
                                       5 Klicken Sie auf die Schaltfläche […] am Ende der Zeile.
                                       6 Es öffnet sich der Dialog Zeichenfolgen-Editor.
                                       7 Gehen Sie ans Ende der Liste und geben Sie das Wort Filler ein.
                                       8 Verlassen Sie den Dialog über die Schaltfläche [Ok].
                                       9 Um die Änderungen wirksam zu machen, müssen Sie die A+W Production
                                         neu starten.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                    F-33
                    Gruppierungen und Sortierungen                                                                Tutorial




                                           Abb. F-11    Füllauftrag-Anzeige


                                           Ergänzende Informationen
                                            Softwarereferenz, “Verwende Füller” auf Seite F-128
                                            Softwarereferenz, “Register Füllaufträge” auf Seite F-171

                                           Restscheiben
                                           Im Dialog Feinplanung können Sie im Register Ergebnisse eine Position an-
                                           klicken und sich durch Betätigen der Schaltfläche [PlanEdit] die Aufteilung der
                                           Scheiben beim Schneiden ansehen. Die Scheiben der letzen Platte können
                                           dann z.B. bei besonders hohem Verschnitt über die Schaltfläche [Auflösen]
                                           wieder aufgelöst werden. Das bedeutet, die Scheiben werden mit der Lauf-
                                           nummer 10005 in die Tabelle FEIN_TEILE zurückgesetzt und können später
                                           zugeschnitten werden.
                                           Solche Restscheiben finden Sie ebenfalls im Register Spezial und dort im Re-
                                           gister Restblätter. Hier können sie für einen späteren, passenden Lauf ausge-
                                           wählt werden.
                                           Alternativ können Scheiben auch auf den aufgelösten Restblättern im Origi-
                                           nallauf verbleiben und dort als Handzuschnitt gefertigt werden. Dann erfolgt
                                           kein Eintrag in die Tabelle FEIN_TEILE mit Laufnummer 10005.
01-2023 / 01-2023




                                              Restblätter anzeigen
                                              Damit vorhandene Restblätter verwendet und im Register Spezial des Di-
                                              alogs Feinplanung für Lauf … angezeigt werden können, muss im Dialog
                                              Master-Orga der Bereich Verwende Restblätter aktiviert und die entspre-
                                              chenden Abstellplätze angegeben sein!


                    F-34                                                                     A+W Production Feinplanung
                 Tutorial                                                             Gruppierungen und Sortierungen




                                          Möchten Sie Änderungen an den Einstellungen vornehmen, wenden Sie
                                          sich vorher bitte unbedingt an A+W, da es sonst zu unerwünschten Ergeb-
                                          nissen kommen kann!




                                       Abb. F-12    Master-Orga, Aktivierung Restblätter


                                       Ergänzende Informationen
                                        Softwarereferenz, “Verwende Restblätter” auf Seite F-129
                                        Softwarereferenz, “Register Restblätter” auf Seite F-173

                                       Bruchscheiben
                                       Gebuchte Bruchscheiben werden mit der Laufnummer 10000 in die Tabelle
                                       FEIN_TEILE zurückgeschrieben. Anschließend können sie in der Feinpla-
                                       nung einem bestimmten Lauf hinzugefügt werden. In der Regel aber werden
                                       bei eiligen Aufträgen Bruchscheiben im Handzuschnitt bearbeitet.

                                          Bruchscheiben anzeigen
                                          Damit vorhandene Bruchscheiben verwendet und im Register Spezial des
                                          Dialogs Feinplanung für Lauf … angezeigt werden können, muss im Dialog
                                          Master-Orga der Bereich Verwende Bruchscheiben aktiviert und die ent-
                                          sprechenden Abstellplätze angegeben sein!
3,00 / 01-2023




                 A+W Production Feinplanung                                                                    F-35
                    Gruppierungen und Sortierungen                                                              Tutorial




                                           Abb. F-13    Master-Orga, Aktivierung Bruchscheiben


                                           Ergänzende Informationen
                                            Softwarereferenz, “Verwende Bruchscheiben” auf Seite F-129
                                            Softwarereferenz, “Register Bruchscheiben” auf Seite F-174

                                           Eilscheiben
                                           Mit Hilfe der Eilscheiben haben Sie die Möglichkeit, zügig Scheiben selbst zu
                                           erfassen und diese der Produktion zuzuführen. Es ist hierbei nicht notwendig,
                                           dass die Scheiben über die Auftragsbearbeitung erfasst werden müssen und
                                           anschließend erst übergeben werden. Eilscheiben werden im Dialog Eilschei-
                                           ben erfasst. Diesen Dialog erreichen Sie über
                                           Extras > Eilscheiben
                                           Eilscheiben werden mit der Laufnummer 10002 in die Tabelle FEIN_TEILE
                                           geschrieben.
01-2023 / 01-2023




                    F-36                                                                   A+W Production Feinplanung
                 Tutorial                                                          Gruppierungen und Sortierungen




                                       Demos und Übungen
                                       In diesem Abschnitt erfahren Sie, wie Sie Gruppierungen und Sortierungen in
                                       der A+W Production anlegen.

                                       Trainerdemo: Gruppierungen und Sortierungen erläutern
                                       Es werden mögliche Gruppierungen und Sortierungen gezeigt und erläutert.
                                       Folgender Dialog wird unter diesem Aspekt erklärt:
                                       •   Dialog Gruppierung/Sortierung

                                       Übung 1: Eine neue Gruppierung hinzufügen
                                       Fügen Sie die bereits vorhandene Gruppierung Kundennummer hinzu.

                                       Aufgabenstellung
                                       Fügen Sie die bereits existierende Gruppierung mit der Eigenschaft Kunden-
                                       nummer als neue Gruppierung hinzu.

                                       Übung 1: Lösung
                                       Das Ergebnis dieser Aufgabe sieht so aus:




                                       Abb. F-14    Gruppierung


                                       Die erstellte Gruppierung kann nun für Einstellungen in den Orgas genutzt
                                       werden.

                                       Übung 2: Einer Gruppierung eine weitere hinzufügen
                                       Fügen Sie die bereits vorhandene Gruppierung Auftragsnummer hinzu.

                                       Aufgabenstellung
                                       Fügen Sie der soeben angelegten Gruppierung Kundennummer die Gruppie-
                                       rung Auftragsnummer hinzu.

                                       Übung 2: Lösung
                                       Das Ergebnis dieser Aufgabe sieht so aus:
3,00 / 01-2023




                                       Abb. F-15    Weitere Gruppierung



                 A+W Production Feinplanung                                                                  F-37
                    Gruppierungen und Sortierungen                                                                 Tutorial




                                           Übung 3: Eine neue Sortierung hinzufügen
                                           Fügen Sie die bereits vorhandene Sortierung Positionsnummer hinzu.

                                           Aufgabenstellung
                                           Fügen Sie die bereits existierende Sortierung mit der Eigenschaft Positions-
                                           nummer als neue Sortierung hinzu.

                                           Übung 3: Lösung
                                           Das Ergebnis dieser Aufgabe sieht so aus:




                                           Abb. F-16    Sortierung


                                           Die erstellte Sortierung kann nun für Einstellungen in den Orgas genutzt wer-
                                           den.

                                           Übung 4: Einer Sortierung eine weitere hinzufügen
                                           Fügen Sie die bereits vorhandene Sortierung Positionsnummer hinzu.

                                           Aufgabenstellung
                                           Fügen Sie der soeben angelegten Sortierung Positionsnummer die Sortierung
                                           Gross_Mass hinzu.

                                           Übung 4: Lösung
                                           Das Ergebnis dieser Aufgabe sieht so aus:




                                           Abb. F-17    Weitere Sortierung


                                           Ergänzende Informationen:
                                            Tutorial, “Gruppierung” auf Seite F-24
                                            Tutorial, “Sortierung” auf Seite F-25
                                            Softwarereferenz, “Gruppierung/Sortierung - Dialog” auf Seite F-140
01-2023 / 01-2023




                    F-38                                                                     A+W Production Feinplanung
                 Tutorial                                                                 Abstellplätze und -modi




                                       Abstellplätze und -modi
                                       In diesem Themenblock lernen Sie die unterschiedlichen Abstellplätze sowie
                                       die verschiedenen Abstellmodi kennen und erfahren, wie Sie damit in der
                                       A+W Production umgehen.
                                       Der Themenblock beinhaltet folgende Schulungseinheiten:
                                       •   Einführung
                                       •   Abstellplätze
                                       •   Logische Abstellplätze
                                       •   Abstellregeln
                                       •   Vordefinierte Abstellmodi für A-Böcke
3,00 / 01-2023




                 A+W Production Feinplanung                                                                 F-39
                    Abstellplätze und -modi                                                                                 Tutorial




                                              Überblick
                                              Lernziele

                                              • Abstellplätze kennenlernen und verstehen.
                                              • Abstellmodi kennenlernen und verstehen.
                                              • Die Auswirkungen der Abstellmodi verstehen.


                                              Nutzen

                                              Wenn Sie die Funktionen der Abstellmodi verstanden haben, können Sie Ihre
                                              Produktion entsprechend organisieren. Eine gut organisierte Produktion spart Ihnen
                                              Zeit und Platz und somit Geld.


                                              Definitionen

                                              Physikalischer Abstellplatz Gestell (A-Bock, L-Bock, Fester Abstellplatz)

                                              Logischer Abstellplatz      Ein logischer Abstellplatz besteht aus einem oder
                                                                          mehreren Stapeln von Glas und definiert, wie diese
                                                                          Stapel zusammen gehören (bspw. um daraus ISO oder
                                                                          VSG zu produzieren). Abhängig ist dies vom gewählten
                                                                          Stapelmodus. Ein logischer Abstellplatz ist einfach ein
                                                                          Bereich auf einem physikalischen Abstellplatz mit
                                                                          Nummer, auf welchen die zusammengehörigen
                                                                          Glasstapel gestellt werden.


                                              Merke

                                              Was darf auf einen          In einen Stapel oder auf einen Fächerwagen dürfen
                                              Abstellplatz?               grundsätzlich nur Teile aus einem Los.

                                              Verschiedene Glasarten auf Das Programm trennt grundsätzlich verschiedenen
                                              einen Stapel               Glasarten und weist sie verschiedenen Stapeln zu. Sie
                                                                         müssen dazu keine gesonderte Logik einrichten.

                                              Abstellmodus: Glas          Hier wird eine Glasart pro Abstellplatz abgestellt. Jeder
                                                                          Stapel bekommt eine eigene Abstellplatznummer. Im
                                                                          Unterschied zum Modus VABGLA werden aber nur
                                                                          Scheiben auf einen Stapel abgestellt, wenn auch deren
                                                                          jeweilige Gegenscheiben gemeinsam weggestellt
                                                                          werden können.

                                              Abstellmodus: Einheit       Hier steht jede Einheit auf einem logischen Abstellplatz.

                                              Abstellmodus: Produktion    Hier können verschiedene Glasarten auf einem
                                                                          logischen Abstellplatz kombiniert werden.

                                              Abstellmodus: VABGLA        Hier gibt es pro Glasart einen logischen Abstellplatz mit
                                                                          jeweils einem Stapel.
01-2023 / 01-2023




                    F-40                                                                          A+W Production Feinplanung
                 Tutorial                                                                     Abstellplätze und -modi




                                       Abstellplätze
                                       Dieser Abschnitt beschäftigt sich mit den logischen Abstellplätzen sowie den
                                       entsprechenden Abstellmodi.
                                       Es behandelt folgende Themen:
                                       •   Logische Abstellplätze
                                       •   Abstellregeln
                                       •   Vordefinierte Abstellmodi für A-Böcke
                                       •   Robot-Böcke
                                       •   Abstellmodi für Fächerwagen
                                       •   Abstellmodi für feste Abstellplätze
                                       In der A+W Production haben Sie verschiedene Kriterien zur Verfügung, um
                                       Scheiben auf Abstellplätze zu stellen. Sie können komplette Gruppen abstel-
                                       len, Gruppen teilen, usw.
                                       Auf diese Weise können Sie Abstellplätze und Abstellmodi dafür nutzen, das
                                       gute Ergebnis zu behalten und zusätzlich mit einer festen Produktionsreihen-
                                       folge zu arbeiten. Auf diese Weise können Sie die Produktion frei definieren
                                       und zusätzlich den roten Punkt innerhalb des roten Kreises.

                                           Abstellplätze
                                           An dieser Stelle weisen wir darauf hin, dass wir ausschließlich von Abstell-
                                           plätzen reden, da wir nicht wissen, ob der Kunde physikalische oder logi-
                                           sche Gestelle verwendet. Ferner sind uns Größe und Breite der Gestelle,
                                           die beim Kunden im Einsatz, nicht bekannt.

                                                                 Reihenfolge




                                       Ausbeute                                            Flexibilität




                                       Logische Abstellplätze
                                       Ein logischer Abstellplatz besteht aus einem oder mehreren Stapeln von Glas
                                       und definiert, wie diese Stapel zusammen gehören (bspw. um daraus ISO
                                       oder VSG zu produzieren). Abhängig ist dies vom gewählten Stapelmodus.
3,00 / 01-2023




                                       Ein logischer Abstellplatz ist einfach ein Bereich auf einem physikalischen Ab-
                                       stellplatz mit Nummer, auf welchen die zusammengehörigen Glasstapel ge-
                                       stellt werden.Das Abstellen von Scheiben auf den logischen Abstellplätzen


                 A+W Production Feinplanung                                                                      F-41
                    Abstellplätze und -modi                                                                                       Tutorial




                                              geschieht in der für den jeweiligen Abstellplatz definierten Produktionsreihen-
                                              folge.
                                              Aus den logischen Abstellplätzen werden physikalische Gestelle gebildet.
                                              Dies geschieht für A-Böcke und feste Abstellplätze unter Berücksichtigung der
                                              Gestellbreite, der Anzahl der Gestellseiten (1 oder 2 für L- bzw. A-Bock) und
                                              des erlaubten Maximalgewichts des Abstellplatzes.


                                              Abstellregeln
                                              •   Unterschiedliche Glasarten werden immer getrennt.
                                              •   Die angegebene Abstelltiefe darf nicht überschritten werden. Daher ist die
                                                  Frage, ob es dem System erlaubt ist, Gruppen zu trennen oder zusammen
                                                  zu halten.
                                              •   In der Regel kommen große Scheiben zu erst auf den Abstellplatz. Daher
                                                  müssen diese zuerst produziert werden oder es muss vor dem Abstellen
                                                  umsortiert werden. Es müssen entweder eindeutige Bedingungen definiert
                                                  werden oder Sie können mit Hilfe des Formel-Editors bestimmte Ein-
                                                  schränkungen definieren.
                                              •   Durch die Verwendung von Abstellmodi können Sie bestimmen, wie das
                                                  System Einheiten und Gruppen auf den physikalischen und logischen Ab-
                                                  stellplätzen abstellt (ein physikalisches Gestell kann genügend Platz für
                                                  mehrere Abstellplätze mit verschiedenen Nummern haben = logische Ge-
                                                  stelle).




                                                                                                                          Maximale Beladung




                                                                                            Log. Abstellpl. 1001   Log. Abstellpl. 1002
                                                     Abstellplatz Seitenansicht
                                                                                                      Abstellplatz - Draufsicht
                                              Maximale Beladung         Maximale Beladung




                                              Eine Gruppe pro Stapel
                                              Wählen Sie diese Einstellung,
                                              •   kommt jede Gruppe in 1 Stapel.
                                              •   muss eine Gruppe geteilt werden (weil das maximale Gewicht überschrit-
                                                  ten ist), wird sie in zwei Stapel geteilt - ob für den zweiten Stapel dann die
                                                  gleiche oder eine neue Abstellplatznummer (logischer Abstellplatz) ver-
                                                  wendet wird, ist abhängig vom verwendeten Stapelmodus.
01-2023 / 01-2023




                    F-42                                                                          A+W Production Feinplanung
                 Tutorial                                                                               Abstellplätze und -modi




                                                                                Maximale Beladung




                                           Gruppe 1




                                                                    Gruppe 2
                                              Log. Abstellpl.1001     Log. Abstellpl.1002
                                                     Abstellplatz - Draufsicht
                                                                                                    o


                                       Komplette Gruppe können zusammen abgestellt werden
                                       Wählen Sie diese Einstellung,
                                       •   kommen verschiedene, komplette Gruppen in einen Stapel (unter Beach-
                                           tung des zulässigen Gesamtgewichtes).


                                                                                Maximale Beladung
                                           Gruppe 1




                                                                    Gruppe 2




                                              Log. Abstellpl.1001     Log. Abstellpl.1002
                                                     Abstellplatz - Draufsicht




                                       Gruppen werden geteilt
                                       Wählen Sie diese Einstellung,
                                       •   wenn das Teilen von Gruppen erlaubt ist (beim Erreichendes maximalen
                                           Gesamtgewichtes) und die Gruppe zu einer anderen Gruppe gestellt wer-
                                           den kann.
                                       •   um ein Umsortieren von Gruppen zu vermeiden, die Reihenfolge der Grup-
                                           pen wird automatisch eingehalten (XOPTS 6.2).
                                                                    Grp.1
                                           Gruppe 1




                                                                     Gruppe 2




                                              Log. Abstellpl.1001         Log. Abstellpl.1002
                                                     Abstellplatz- Draufsicht
3,00 / 01-2023




                 A+W Production Feinplanung                                                                              F-43
                    Abstellplätze und -modi                                                                                               Tutorial




                                              Vordefinierte Abstellmodi für A-Böcke
                                              Auf A-Böcken kann nach vier verschiedenen Verfahren abgestellt werden:
                                              •   Abstellmodus Glas
                                              •   Abstellmodus Einheit
                                              •   Abstellmodus Produktion
                                              •   Abstellmodus VABGLA

                                                  Trennung von Glasarten
                                                  Das Programm trennt immer die Glasarten. Das gilt sowohl für das Abstel-
                                                  len der Glasarten als auch für die Optimierung.

                                              Abstellmodus Glas
                                              Im Abstellmodus Glas wird eine Glasart pro Abstellplatz gestellt. Dabei be-
                                              kommt jeder Stapel (Gruppe 3 und 4) eine eigene Abstellplatznummer (1000,
                                              2000, 3000).
                                                                         Grp.4
                                                  Grp.3




                                                    Abstellplatz 1000       Abstellplatz 2000

                                                           Abstellplätze - Draufsicht




                                              Sie werden mehr Abstellplätze und Abstellplatznummern benötigen als bei an-
                                              deren Abstellmodi.

                                              Abstellen kompletter Gruppen
                                              Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe auf einen
                                              neuen Abstellplatz - mit einer neuen Abstellplatznummer. Und die zugehörige
                                              Gruppe des anderen Abstellplatzes kommt ebenfalls auf einen neuen Abstell-
                                              platz - mit einer neuen Abstellplatznummer. Beide Abstellplätze (1000 und
                                              2000) gelten als voll. Auf die beiden neuen Abstellplätze können weitere Sta-
                                              pel (Gruppen) Glas gestapelt werden - solange, bis auch hier wiederum das
                                              Maximum der Beladung erreicht ist.




                                                  Abstellplatz 1000     Abstellplatz 2000       Abstellplatz 3000     Abstellplatz 4000
01-2023 / 01-2023




                                                           Abstellplätze - Draufsicht




                    F-44                                                                                            A+W Production Feinplanung
                 Tutorial                                                                                         Abstellplätze und -modi




                                       Abstellen geteilter Gruppen
                                       Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die
                                       restlichen Scheiben (über der max. Beladung) gehen jeweils auf einen neuen
                                       Abstellplatz - mit einer neuen Abstellplatznummer. Und die betreffenden
                                       Scheiben der zugehörigen Gruppe des anderen Abstellplatzes gehen eben-
                                       falls auf einen neuen Abstellplatz - mit einer neuen Abstellplatznummer. Beide
                                       Abstellplätze (1000 und 2000) gelten als voll. Auf die beiden neuen Abstell-
                                       plätze können weitere Stapel (Gruppen) Glas gestapelt werden - solange, bis
                                       auch hier wiederum das Maximum der Beladung erreicht ist.




                                                   Abstellplatz 1000     Abstellplatz 2000   Abstellplatz 3000   Abstellplatz 4000



                                                          Phys. Abstellplätze - Draufsicht




                                       Abstellmodus Einheit
                                       Im Abstellmodus Einheit steht jede Einheit (bspw. Gläser für ISO oder VSG)
                                       auf einem logischen Abstellplatz.
                                                                            Grp.4
                                           Grp.3




                                                           Log. Abstellplatz 1001
                                                    Draufsicht


                                                                  Einheit




                                       •           Jede Glasart befindet sich auf einem anderen Stapel.
                                       •           Jede Einheit bekommt ihre eigene Abstellplatznummer.
                                       •           Sobald ein Stapel das Maximum erreicht, ist die ganze Abstellplatznummer
                                                   voll.
                                       •           Sie benötigen weniger physikalische Gestelle als im Abstellmodus Glas.
                                       •           Da Einheiten immer zusammengehalten werden, ist die Produktion ein-
                                                   fach.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                                          F-45
                    Abstellplätze und -modi                                                                                             Tutorial




                                              Abstellen kompletter Gruppen
                                              Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe auf einen
                                              neuen Abstellplatz mit einer neuen Abstellplatznummer. Und die zugehörige
                                              Gruppe des anderen Stapels kommt ebenfalls auf diesen neuen (logischen)
                                              Abstellplatz (Gruppe 4 ist über dem Limit, also gehen Gruppe 4 und 3 auf ei-
                                              nen neuen Abstellplatz: 1002).
                                              Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen be-
                                              laden werden, bis auch hier die maximale Beladung erreicht wird.

                                                                                                              Maximale Beladung




                                                                                                                Grp.4
                                                                                       Grp.3
                                                      Logischer Abstellplatz 1001               Logischer Abstellplatz 1002
                                                      Draufsicht                                    Draufsicht


                                                                  Einheit                                 Einheit




                                              Abstellen geteilter Gruppen
                                              Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die
                                              Scheiben dieser Gruppe, die über der max. Beladung sind, und die zugehöri-
                                              gen Scheiben der anderen Gruppe gehen auf einen neuen Abstellplatz - mit
                                              einer neuen Abstellplatznummer. (Gruppe 4 ist über dem Limit; die letzte
                                              Scheibe von Gruppe 4 und die letzte Scheibe der Gruppe 3 gehen auf einen
                                              neuen Abstellplatz: 1002).
                                              Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen be-
                                              laden werden, bis auch hier die maximale Beladung erreicht wird.

                                                                                                                        Maximale Beladung
                                                                                       Grp.3




                                                                                                                Grp.4




                                                         Logischer Abstellplatz 1001              Logischer Abstellplatz 1002
                                                Draufsicht                                     Draufsicht



                                                                   Einheit                                   Einheit
01-2023 / 01-2023




                    F-46                                                                               A+W Production Feinplanung
                 Tutorial                                                                               Abstellplätze und -modi




                                       Abstellmodus Produktion
                                       Im Abstellmodus Produktion können verschiedene Glasarten auf einem logi-
                                       schen Abstellplatz in mehreren Stapeln kombiniert abgestellt werden. Es ist
                                       möglich, verschiedene Kombinationen von Produkten, welche gefertigt wer-
                                       den sollen, abzustellen.


                                                   Float 4                                               Maximale Beladung
                                           Grp.3
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




                                       •           Jede Glasart befindet sich in einem anderen Stapel.
                                       •           Unterschiedliche Glasarten werden zusammen auf einem logischen (oder
                                                   physikalischen) Abstellplatz gestellt.
                                       •           Sobald ein Stapel das Maximum erreicht, ist die ganze Abstellplatznummer
                                                   "voll".
                                       •           Zusammengehörige Gruppen müssen definiert und beibehalten werden.
                                       •           Sie benötigen weniger physikalische Gestelle.
                                       •           Sie benötigen zusätzliche Hilfs- und Kontrollmechanismen wie bspw. Pro-
                                                   duktionspapiere oder Anzeigesysteme um die Kontrolle zu behalten.

                                       Abstellen kompletter Gruppen
                                       Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe und die
                                       zugehörige Gruppe des anderen Stapel auf einen neuen Abstellplatz - mit ei-
                                       ner neuen Abstellplatznummer (Gruppe 3 ist über dem Limit, also gehen Grup-
                                       pe 3 und 4 auf einen neuen Abstellplatz: 1002). Auf diesem neuen Abstellplatz
                                       können Sie neue Glasarten und neue Gruppen abstellen. Abstellplatz 1001
                                       gilt als voll, Abstellplatz 1002 kann mit weiteren Gruppen beladen werden, bis
                                       auch hier die maximale Beladung erreicht wird.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                                  F-47
                    Abstellplätze und -modi                                                                                                  Tutorial




                                                                                                                            Maximale Beladung

                                                        Float 6

                                                        Float 6
                             Float 4


                                                         Float 6                                                                           Thermisch
                             Float 4                                                                           Float 4




                                                                                                                                  Grp. 4
                                                                                                      Grp. 3
                                                                                 Thermisch
                                       Logischer Abstellplatz 1001                                                  Logischer Abstellplatz 1002
                                              Draufsicht                                                                    Draufsicht




                                                       Abstellen geteilter Gruppen
                                                       Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die
                                                       Scheiben dieser Gruppe, die über der max. Beladung sind, und die betreffen-
                                                       den Scheiben der entsprechenden Gruppe innerhalb des anderen Abstellplat-
                                                       zes gehen zusammen auf einen neuen Abstellplatz - mit einer neuen
                                                       Abstellplatznummer. (Gruppe 3 ist über dem Limit, also geht die letzte Scheibe
                                                       der Gruppe 3 und die letzte Scheibe der Gruppe 4 auf einen neuen Abstell-
                                                       platz: 1002). Auf diesem neuen Abstellplatz können Sie neue Glasarten und
                                                       neue Gruppen abstellen. Abstellplatz 1001 gilt als voll, Abstellplatz 1002 kann
                                                       mit weiteren Gruppen beladen werden, bis auch hier die maximale Beladung
                                                       erreicht wird.


                                                                                                                            Maximale Beladung

                                                        Float 6
                     Grp.3




                                                        Float 6
                             Float 4


                                                         Float 6
                             Float 4
                                                                                                                                  Grp.4
                                                                                                      Grp.3




                                                                                 Thermisch                     Float 4                 Thermisch
                                       Logischer Abstellplatz 1001                                                 Logischer Abstellplatz 1002
                                              Draufsicht                                                                   Draufsicht
01-2023 / 01-2023




                    F-48                                                                               A+W Production Feinplanung
                 Tutorial                                                                                    Abstellplätze und -modi




                                       Abstellmodus VABGLA
                                       Im Abstellmodus VABGLA gibt es pro Glasart einen logischen Abstellplatz mit
                                       jeweils einem Stapel. Es ist möglich, verschieden Kombinationen von Produk-
                                       ten, welche gefertigt werden sollen, abzustellen.




                                              Abstellplatz 1000              Abstellplatz 2000


                                                         Abstellplätze Draufsicht




                                       •   Jede Glasart befindet sich auf einem separaten Abstellplatz.
                                       •   Jede Glasart (Stapel) bekommt ihre eigene Abstellplatznummer.
                                       •   Das Abstellen und Produzieren ist sehr komplex.
                                       •   Zusammengehörige Gruppen müssen definiert und beibehalten werden.

                                       Abstellen kompletter Gruppen
                                       Erreicht ein Stapel die maximale Beladung, kommt die letzte Gruppe auf einen
                                       neuen Abstellplatz - mit einer neuen Abstellplatznummer. Die zugehörige
                                       Gruppe (Einheit) auf einem anderen Gestell wird nicht bewegt.




                                              Abstellplatz 1000              Abstellplatz 2000    Abstellplatz 3000

                                                                       Abstellplätze Draufsicht
3,00 / 01-2023




                 A+W Production Feinplanung                                                                                   F-49
                    Abstellplätze und -modi                                                                                 Tutorial




                                              Abstellen geteilter Gruppen
                                              Erreicht ein Stapel die maximale Beladung, wird die letzte Gruppe geteilt. Die
                                              Scheiben dieser Gruppe, die über der max. Beladung sind, gehen auf einen
                                              neuen Abstellplatz - mit einer neuen Abstellplatznummer. Die zugehörige
                                              Gruppe (Einheit) auf einem anderen Gestell wird nicht bewegt und auch nicht
                                              geteilt.




                                                  Abstellplatz 1000     Abstellplatz 2000           Abstellplatz 3000


                                                                              Abstellplätze Draufsicht




                                              Robot-Böcke
                                              Bei den A-Böcken besteht die Möglichkeit, diese als sogenannte Robot-Böcke
                                              zu kennzeichnen. Ein Robot-Bock ist ein A-Bock, der mittels eines Roboters
                                              angesteuert wird. Robot-Böcke haben die folgenden Eigenschaften:
                                              •   Unendliche Abstellplatztiefe (>20 Meter) und
                                              •   Maximale Anzahl Gruppen auf Abstellplatz = 1.
                                              Auf einem solchen Abstellplatz landen also nur Scheiben mit gleichen Eigen-
                                              schaften gemäß der Gruppierungsvorschrift.


                                              Abstellmodi für Fächerwagen
                                              Auf Fächerwagen gibt es zwei verschiedene Verfahren:
                                              •   Zusammen:
                                                  Dabei werden Scheibe und Gegenscheibe(n) immer zusammen auf einen
                                                  Fächerwagen gestellt (in unterschiedliche Fächer).
                                              •   Glas:
                                                  Dabei werden die Scheiben immer getrennt weggestellt (unterschiedliche
                                                  Fächerwagen).
                                              Diese Modi gelten natürlich nur auf den Verwendungsböcken, da für den je-
                                              weiligen Produktionsschritt die Gegenscheibe des zu produzierenden Teils
                                              nicht berücksichtigt wird. Sollte es eine Gegenscheibe geben, so kommt diese
                                              erst auf den Verwendungsböcken des nachfolgenden Produktionsschritt ins
                                              Spiel.


                                              Abstellmodi für feste Abstellplätze
01-2023 / 01-2023




                                              Für feste Abstellplätze gibt es keine Abstellmodi. Sie dienen als sogenannte
                                              Zwischenlager hinter dem Zuschnitt. Es wird so lange auf diesen Abstellplät-
                                              zen abgestellt, bis er voll ist. Dann muss für die Produktion umsortiert werden.


                    F-50                                                                                 A+W Production Feinplanung
                 Tutorial                                                                    Abstellplätze und -modi




                                       Standard-Einstellungen in der Konfigu-
                                       ration
                                       Je mehr Abstellplätze innerhalb der Produktion zur Verfügung stehen, um so
                                       größer ist die Flexibilität und je besser ist das Ergebnis der Optimierung be-
                                       züglich der Glasausbeute (trotz der festen Reihenfolge). Aber, viele Abstell-
                                       plätze erfordern viel Platz in der Produktion.
                                       In der Konfiguration haben Sie diverse Möglichkeiten zum Einstellen der A+W
                                       Production, wie z. B. die Mindestanzahl an Gestellen.
                                       Stammdaten > Konfiguration > A+W Production > Feinplanung




                                       Abb. F-18    Minimale Anzahl an Abstellplätzen


                                       Diese Einstellungen werden bei der Systemkonfiguration gemeinsam mit dem
                                       Service-Techniker eingerichtet und dürfen danach nur in Absprache mit dem
                                       A+W Service geändert werden. Diese Schalter haben große Auswirkungen
                                       auf die Ergebnisse und Funktionsweise des PPS-Systems und auf die realen
                                       Produktionsergebnisse und -abläufe.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                     F-51
                    Abstellplätze und -modi                                                                          Tutorial




                                              Einstellungen in den Stammdaten
                                              In den Stammdaten können Sie bestimmte Gestellarten anlegen und verwal-
                                              ten:
                                              Stammdaten > Feinplanung > Abstellplätze




                                              Abb. F-19    Einstellungen Abstellplätze


                                              •   Abstelltiefe: In diesem Feld geben Sie die maximale Abstelltiefe an. Dieser
                                                  Wert kennzeichnet die maximal Tiefe des Glasstapels auf dem Gestell.
                                              •   Breite: Bei diesem Wert handelt es sich um die gesamte Breite des Ge-
                                                  stells.
                                              •   Max. Abstellplätze/Bock: Wie viele Gruppen können nebeneinander auf
                                                  dem Gestell stehen oder wie viele logische Abstellplätze befinden sich auf
                                                  einem physikalischen Gestell.
                                              •   Maximales Gewicht: In diesem Feld geben Sie das maximale Gewicht aller
                                                  Scheiben auf dem Gestell an, z. B. 750 kg = 75 m² Float 4.


                                               So richten Sie eine neue A-Bock-Art ein
01-2023 / 01-2023




                                              1 Wählen Sie in der Menü Stammdaten > Feinplanung > Abstellplätze.
                                              2 Betätigen Sie die Schaltfläche [Hinzufügen] im Bereich der A-Böcke. Es
                                                öffnet sich der Dialog Feinplanung.



                    F-52                                                                      A+W Production Feinplanung
                 Tutorial                                                                   Abstellplätze und -modi




                                       3 Geben Sie in dem Feld Neuer A-Bock einen Namen ein und verlassen Sie
                                         den Dialog mit [OK].
                                       4 Geben Sie im Feld Abstelltiefe ein, wie tief die Fläche in mm zum Abstellen
                                         der Scheiben ist.
                                       5 Geben Sie im Feld Breite ein, wie breit die Fläche in mm zum Abstellen der
                                         Scheiben ist.
                                       6 Geben Sie im Feld Max. Abstellplätze / Bock ein, ob es auf dem Abstell-
                                         platz einen, zwei oder vier Abstellplätze gibt.
                                       7 Handelt es sich bei dem Abstellplatz um einen L-Bock, aktivieren Sie die
                                         Checkbox L-Bock.
                                       8 Werden in Ihrem Betrieb die Abstellplätze mit einem Roboter beladen, ak-
                                         tivieren Sie die Checkbox Robot.
                                       9 Die beiden im Bereich Anzahl liegendenden Felder sind nur dann aktiv,
                                         wenn die Checkbox Robot aktiviert wurde. In dem oberen Eingabefeld er-
                                         fassen Sie, wie viele Robot-Böcke es in Ihrem Betrieb gibt. In der darunter
                                         liegenden Kombobox wählen Sie, wie die Robot-Böcke belegt werden.
                                       10 Geben Sie im Feld Maximales Gewicht (kg) an, wie schwer der A-Bock ma-
                                          ximal beladen sein darf.
                                       11 Betätigen Sie die Schaltfläche [OK].
                                       Der angelegte Gestellart kann nun für Einstellungen in den Orgas genutzt wer-
                                       den.


                                        So richten Sie einen neuen Fächerwagen-Typ ein
                                       1 Wählen Sie in der Menü Stammdaten > Feinplanung > Abstellplätze.
                                       2 Betätigen Sie die Schaltfläche [Hinzufügen] im Bereich der Fächerwagen.
                                         Es öffnet sich der Dialog Feinplanung.
                                       3 Geben Sie in dem Feld Neuer Fächerwagen einen Namen ein und verlas-
                                         sen Sie den Dialog mit [OK].
                                       4 Geben Sie im Feld Anzahl Fachnummer ein, wie viele Fächer der Wagen
                                         hat.
                                       5 Geben Sie im Feld Fachbreite ein, wie breit (in mm) die einzelnen Fächer
                                         sind.
                                       6 Aktivieren oder deaktivieren Sie die Checkbox Zwei Fächer/Nummer. So
                                         können beispielsweise Gläser für Einheiten (ISO/VSG) leicht zusammen-
                                         gehörig in den Fächerwagen gestellt werden um anhand der gleichen
                                         Fachnummer die Zusammengehörigkeit zu identifizieren.
                                       7 Aktivieren oder deaktivieren Sie die Checkbox Start = 0. Bei 0 beginnt die
                                         Nummer des ersten Fächerwagens mit 0 statt mit 1.
                                       8 Setzen Sie die entsprechende Radiotaste im Feld Anzahl der Stellen für
                                         Fachnummer:
3,00 / 01-2023




                                       9 Geben Sie im Feld Max. Anzahl Fächerwagen ein, wie viele Fächerwagen
                                         in Ihrem Unternehmen zur Verfügung stehen.
                                       10 Aktivieren oder deaktivieren Sie die Checkbox Überprüfung Anzahl


                 A+W Production Feinplanung                                                                    F-53
                    Abstellplätze und -modi                                                                          Tutorial




                                              11 Geben Sie im Feld Maximales Gewicht (kg) an, wie schwer der Fächerwa-
                                                 gen maximal beladen sein darf.
                                              12 Betätigen Sie die Schaltfläche [OK].
                                              Der erste Fächerwagenart kann nun für Einstellungen in den Orgas genutzt
                                              werden.


                                               So richten Sie eine neue Art fester Abstellplatz ein
                                              1 Wählen Sie in der Menü Stammdaten > Feinplanung > Abstellplätze.
                                              2 Betätigen Sie die Schaltfläche [Hinzufügen] im Bereich der Festen Abstell-
                                                plätze. Es öffnet sich der Dialog Feinplanung.
                                              3 Geben Sie in dem Feld Neuer FAP einen Namen ein und verlassen Sie den
                                                Dialog mit [OK].
                                              4 Geben Sie im Feld Abstelltiefe ein, wie tief die Fläche in mm zum Abstellen
                                                der Scheiben ist.
                                              5 Geben Sie im Feld Breite ein, wie breit die Fläche in mm zum Abstellen der
                                                Scheiben ist.

                                                 Fachbreite
                                                 Dieses Feld wird im Moment von der Feinplanung nicht ausgewertet. Es
                                                 sollte trotzdem eine Angabe gemacht werden, um der Feinplanung die
                                                 Möglichkeit offen zu lassen, diese Angabe in Zukunft u.U. zu nutzen.

                                              6 Geben Sie im Feld Max. Abstellplätze FAPs ein, wie viele dieser Festen
                                                Abstellplätze es in Ihrem Betrieb gibt.
                                              7 Aktivieren oder deaktivieren Sie die Checkbox Überprüfung Anzahl.
                                              8 Geben Sie im Feld Maximales Gewicht (kg) an, wie schwer der feste Ab-
                                                stellplatz maximal beladen sein darf.
                                              9 Betätigen Sie die Schaltfläche [OK].
                                              Der erstellte Abstellplatz kann nun für Einstellungen in den Orgas genutzt wer-
                                              den.


                                              Ergänzende Informationen:
                                               Tutorial, “Unterschiedliche Optimierungs-Modi” auf Seite F-57
                                               Softwarereferenz, “Abstellplätze” auf Seite F-146
01-2023 / 01-2023




                    F-54                                                                        A+W Production Feinplanung
                 Tutorial                                                                   Abstellplätze und -modi




                                       Demos und Übungen
                                       In diesem Abschnitt erfahren Sie, wie Sie Abstellplätze in der A+W Production
                                       anlegen.

                                       Trainerdemo: Abstellplätze erläutern
                                       Es werden mögliche Abstellplätze gezeigt und erläutert.
                                       Folgender Dialog wird unter diesem Aspekt erklärt:
                                       •   Dialog Abstellplätze

                                       Übung 1: Einen A-Bock anlegen
                                       Richten Sie einen Abstellplatz für A-Böcke ein.

                                       Aufgabenstellung
                                       Gestellart: A-Bock
                                       Abstelltiefe: 200 mm
                                       Breite: 2000 mm
                                       Max. Anzahl Abstellplätze: 4
                                       Max. Anzahl A-Böcke: 99.

                                       Übung 1: Lösung
                                       Das Ergebnis dieser Aufgabe sieht so aus:




                                       Abb. F-20    Abstellplatz A-Bock
3,00 / 01-2023




                                           Gestellbeladung mittels Roboter
                                           Werden in Ihrem Betrieb die Abstellplätze mit einem Roboter beladen, akt-
                                           vieren Sie bitte die Checkbox Robot.


                 A+W Production Feinplanung                                                                    F-55
                    Abstellplätze und -modi                                                                    Tutorial




                                              Übung 2: Einen Fächerwagen anlegen
                                              Richten Sie einen Abstellplatz für Fächerwagen ein.

                                              Aufgabenstellung
                                              Gestellart: Fächerwagen
                                              Anzahl Fachnummern: 99
                                              Max. Anzahl Fächerwagen: 50
                                              Übung 2: Lösung
                                              Das Ergebnis dieser Aufgabe sieht so aus:




                                              Abb. F-21    Abstellplatz


                                              Übung 3: Einen festen Abstellplatz anlegen
                                              Richten Sie einen festen Abstellplatz ein.

                                              Aufgabenstellung
                                              Gestellart: Fester Abstellplatz
                                              Abstelltiefe: 1000 mm
                                              Breite: 2000 mm
                                              Max. Anzahl FAPs: 99
01-2023 / 01-2023




                    F-56                                                                    A+W Production Feinplanung
                 Tutorial                                                                    Abstellplätze und -modi




                                       Übung 3: Lösung
                                       Das Ergebnis dieser Aufgabe sieht so aus:




                                       Abb. F-22    Fester Abstellplatz


                                       Ergänzende Informationen:
                                        Tutorial, “Böcke (Abstellplätze)” auf Seite F-17
                                        Softwarereferenz, “Abstellplätze” auf Seite F-146
3,00 / 01-2023




                 A+W Production Feinplanung                                                                   F-57
                    Optimierungsmodi                                                                   Tutorial




                                       Optimierungsmodi
                                       In diesem Themenblock lernen Sie Optimierungen kennen und erfahren, wie
                                       Sie damit in der A+W Production umgehen.
                                       Der Themenblock beinhaltet folgende Schulungseinheiten:
                                       •   Überblick
                                       •   Unterschiedliche Optimierungs-Modi
01-2023 / 01-2023




                    F-58                                                           A+W Production Feinplanung
                 Tutorial                                                                             Optimierungsmodi




                                       Überblick
                                       Lernziele

                                       • Die unterschiedlichen Optimierungs-Modi kennenlernen und verstehen.
                                       • Unter welchen Umständen wird welcher Modus verwendet.
                                       • Entsprechende Einstellungen in A+W Production kennenlernen und verstehen.


                                       Nutzen

                                       Nur wenn Sie die unterschiedlichen Optimierungs-Modi kennen und verstehen,
                                       können Sie die A+W Production-Feinplanung auf Ihre Produktion so anpassen, dass
                                       diese kostengünstig und zeitsparend arbeitet.


                                       Definitionen

                                       Einheit                    Unter Einheit versteht man zwei oder mehr Scheiben
                                                                  Glas, welche zusammengehören, da sie später in einem
                                                                  Produktverbund zusammengebaut werden, z. B. ISO
                                                                  oder VSG.

                                       Gruppe                     Die Gruppe bezieht eine Stückzahl mit ein. Sie gruppiert
                                                                  Einheiten nach bestimmten Kriterien, wie z. B.
                                                                  Kundennummer und Auftragsnummer.

                                       Supergruppe                Supergruppen vereinigen verschiedene Gruppen.
                                                                  Dadurch können beispielsweise drei zusammengehörige
                                                                  Gruppen durch ein gleichartiges Regelwerk behandelt
                                                                  werden. Bsp.: Sortierung auf Gestelle, da alle drei
                                                                  Gruppen (z. B. Aufträge) an den selben Kunden oder
                                                                  das selbe Projekt gehen.


                                       Merke

                                       Die Wahl der Optimierung   Bei der Wahl der Optimierung muss ein Kompromiss
                                                                  gefunden werden zwischen dem besten
                                                                  Optimierungserfolg (geringer Verschnitt) und der besten
                                                                  Produktionsreihenfolge für die Montage.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                          F-59
                    Optimierungsmodi                                                                        Tutorial




                                       Unterschiedliche Optimierungs-Modi
                                       Bei der Wahl der Optimierung muss immer ein Kompromiss gefunden werden
                                       zwischen dem besten Optimierungserfolg (geringer Verschnitt) und der bes-
                                       ten Produktionsreihenfolge für die Montage.
                                       A+W Production verwendet die folgenden Optimierungsmodi:
                                       •   6.2
                                       •   6.1
                                       •   5.2
                                       •   5.1
                                       •   Freie Optimierung

                                       Optimierungsmodus 6.2 - Feste Reihenfolge
                                       Dieser Optimierungsmodus arbeitet mit einer strikten Reihenfolge. Nichts
                                       lässt sich ändern und die Scheiben werden in einer 100% strikten Reihenfolge
                                       produziert. In dieser Reihenfolge werden sie zur Produktion freigegeben.
                                       •   Die Reihenfolge der Gruppen ist fest.
                                       •   Die Reihenfolge der Scheiben innerhalb der Gruppe ist fest.

                                           Alternierende Optimierungspositionen für Positionen mit ungleichen
                                           Scheiben
                                           Positionen mit zwei oder mehr Scheiben einer Glasart, die aber unter-
                                           schiedliche Geometrien haben, können wie herkömmliche Pärchen abge-
                                           stellt werden, d.h. auf einen gemeinsamen Stapel und alternierend
                                           (Scheibe1, Scheibe3, Scheibe1, Scheibe3,...). Das gewünschte Verhalten
                                           wird nur für A-Böcke verwendet, bei denen der Modus 6.2 (=feste Reihen-
                                           folge) eingestellt ist.

                                           Ein Zusammenlegen von Modellen ist bei diesen Scheiben nur noch mittels
                                           A+W Shape Optimizer möglich, nicht mehr über das feinplanungsinterne
                                           Zusammenlegen von Modellen!

                                       Unter welchen Umständen können Sie diesen Modus verwenden?
                                       •   Sie optimieren auf A-Böcke.
                                       •   Sie haben einen strengen Produktions- und Lieferplan.
                                       •   Sie produzieren entweder nach Kunde oder nach Glasart.
                                       •   (Gewöhnlich) haben Sie einen schlechten Verschnitt - das Ergebnis ist je-
                                           doch nicht das Hauptkriterium, sonder die Produktion in strikter Sequenz
                                           (z. B. Ausrichtung der gesamten Produktion auf Entladereihenfolge des
                                           LKW für ein spezifisches Kundenprojekt).
                                       •   Sie müssen sicher stellen, dass die großen Scheiben zuerst geschnitten
                                           und abgestellt werden, oder Sie benötigen ein zusätzliches Gestell zum
                                           Umsortieren.
                                       •   Gewöhnlich benötigen Sie eine feste Anzahl an Gestellen (Anzahl an
01-2023 / 01-2023




                                           Gruppen = nahezu die Anzahl an physikalischen Gestellen).
                                       •   Sie können direkt in Produktions- oder Packmittelreihenfolge optimieren.
                                       Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Mo-
                                       dus:

                    F-60                                                              A+W Production Feinplanung
                 Tutorial                                                                              Optimierungsmodi




                                                                  Reihenfolge




                                       Ausbeute                                              Flexibilität



                                       Einstellungen in A+W Production
                                       Für eine Optimierung in diesem Modus sind im Programm folgende Einstellun-
                                       gen nötig:
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                       stellplatz markieren > Einstellungen




                                       Abb. F-23    Optimierungsmodus 6.2


                                       Ergänzende Informationen:
                                        Tutorial, “Böcke (Abstellplätze)” auf Seite F-17
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                                       Optimierungsmodus 6.1 - Kunden zusammenhalten
                                       In diesem Optimierungsmodus ist die Reihenfolge innerhalb der Gruppen fest,
                                       z. B. nach Abmessungen. Die unterschiedlichen Gruppen können von ihrer
3,00 / 01-2023




                                       Anordnung her verändert werden um das Ergebnis zu verbessern. Ein typi-
                                       sches Kriterium hier wäre
                                       •   Tour | Kunde


                 A+W Production Feinplanung                                                                       F-61
                    Optimierungsmodi                                                                         Tutorial




                                       Auf diese Weise werden die Kundenpositionen zusammen gefertigt, Sie ha-
                                       ben jedoch keinen Einfluss darauf, für welchen Kunde zuerst produziert wird.
                                       •   Die Reihenfolge der Gruppen kann verändert werden (X).
                                       •   Die Reihenfolge der Scheiben innerhalb der Gruppe ist fest.

                                       Unter welchen Umständen wird dieser Modus verwendet?
                                       •   Sie optimieren auf A-Böcke.
                                       •   Sie haben einen strengen Produktions- und Lieferplan.
                                       •   Sie produzieren entweder nach Kunde oder nach Glasart.
                                       •   Sie haben einen relativ schlechten Verschnitt (aber besser als mit dem Mo-
                                           dus 6.2) - der Verschnitt ist jedoch nicht das Hauptkriterium.
                                       •   Sie müssen sicher stellen, dass die großen Scheiben zu erst geschnitten
                                           und abgestellt werden, oder Sie benötigen ein zusätzliches Gestell zum
                                           Umsortieren.
                                       •   Gewöhnlich benötigen Sie eine feste Anzahl an Gestellen (Anzahl an
                                           Gruppen = nahezu die Anzahl an physikalischen Gestellen).
                                       •   Sie können direkt in Produktions- oder Packmittelreihenfolge optimieren.
                                       Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Mo-
                                       dus:

                                                                Reihenfolge




                                       Ausbeute                                           Flexibilität



                                       Einstellungen in A+W Production
                                       Für eine Optimierung in diesem Modus sind im Programm folgende Einstellun-
                                       gen nötig:
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                       stellplatz markieren > Einstellungen
01-2023 / 01-2023




                    F-62                                                              A+W Production Feinplanung
                 Tutorial                                                                             Optimierungsmodi




                                       Abb. F-24    Optimierungsmodus 6.1


                                       Ergänzende Informationen:
                                        Tutorial, “Böcke (Abstellplätze)” auf Seite F-17
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                                       Optimierungsmodus 5.2 - Standard
                                       Dieser Optimierungsmodus ist der Standard-Modus der Feinplanung. Der
                                       Gruppierungs- und Sortierungsschlüssel enthält nur die Gruppen-Nr. Das be-
                                       deutet, dass jede Position innerhalb der Gruppe ihre eigene Positions-Nr. be-
                                       sitzt und so eindeutig identifiziert werden kann. Daher müssen die Teile
                                       innerhalb der Gruppe keine feste Reihenfolge einhalten, sondern können frei
                                       optimiert werden.
                                       •   Die Reihenfolge der Gruppen ist fest.
                                       •   Die Reihenfolge der Scheiben innerhalb der Gruppe kann verändert wer-
                                           den. Nur Einheiten (z. B. für ISO) werden zusammengehalten (X).

                                       Unter welchen Umständen wird dieser Modus verwendet?
                                       •   Wenn der Modus 5.1 nicht verwendet wird.
                                       •   In kombinierten Gruppierungs-/Sortierungsschlüssel nicht die beiden Ei-
                                           genschaften AUFTRAGSNUMMER und POSITIONSNUMMER verwendet
                                           wird.
                                       Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Mo-
                                       dus:
3,00 / 01-2023




                 A+W Production Feinplanung                                                                      F-63
                    Optimierungsmodi                                                                         Tutorial




                                                                  Reihenfolge




                                       Ausbeute                                              Flexibilität



                                       Einstellungen in A+W Production
                                       Für eine Optimierung in diesem Modus sind im Programm folgende Einstellun-
                                       gen nötig:
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                       stellplatz markieren > Einstellungen




                                       Abb. F-25    Optimierungsmodus 5.2


                                       Ergänzende Informationen:
                                        Tutorial, “Böcke (Abstellplätze)” auf Seite F-17
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                                       Optimierungsmodus 5.1 - ISO auf Fächerwagen oder viele A-Bö-
                                       cke
01-2023 / 01-2023




                                       Der Gruppierungs- und Sortierungsschlüssel enthält nur die Gruppen-Nr. Das
                                       bedeutet, dass jede Position innerhalb der Gruppe seine eigene Positions-Nr.
                                       besitzt und so eindeutig identifiziert werden kann. Daher müssen die Teile in-



                    F-64                                                                 A+W Production Feinplanung
                 Tutorial                                                                          Optimierungsmodi




                                       nerhalb der Gruppe keine feste Reihenfolge einhalten, sondern können opti-
                                       miert werden. Dies ist soweit identisch zum Optimierungsmodus 5.2.
                                       •   Die Reihenfolge der Gruppen kann verändert werden (X).
                                       •   Die Reihenfolge der Scheiben innerhalb der Gruppe kann verändert wer-
                                           den.
                                       •   Nur Einheiten (z. B. für ISO) werden zusammengehalten (X).

                                       Unter welchen Umständen wird dieser Modus verwendet?
                                       •   Sie optimieren auf Fächerwagen und benötigen zusätzlich einige A-Böcke.
                                       •   Sie werden einen guten Verschnitt haben.
                                       •   Vor der Auslieferung werden Sie viel umsortieren müssen - dies erfordert
                                           eine große Anzahl an physikalischen Gestellen.
                                       Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Mo-
                                       dus:

                                                                Reihenfolge




                                       Ausbeute                                          Flexibilität



                                       Einstellungen in A+W Production
                                       Für eine Optimierung in diesem Modus sind im Programm folgende Einstellun-
                                       gen nötig:
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                       stellplatz markieren > Einstellungen
3,00 / 01-2023




                 A+W Production Feinplanung                                                                   F-65
                    Optimierungsmodi                                                                          Tutorial




                                       Abb. F-26      Optimierungsmodus 5.1


                                       Ergänzende Informationen:
                                        Tutorial, “Böcke (Abstellplätze)” auf Seite F-17
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                                       Optimierungsmodus Freie Optimierung - Scheiben auf Fächerwa-
                                       gen
                                       Freie Optimierung ist die Standardoptimierung für Scheiben auf Fächerwa-
                                       gen. Bei der Freien Optimierung können, ebenso wie für den Handzuschnitt,
                                       verschiedene Glasarten/-dicken auf einem Abstellplatz abgestellt werden
                                       (verschiedene Stapel).
                                       •   Alles ist frei

                                       Unter welchen Umständen wird dieser Modus verwendet?
                                       •   Sie optimieren auf Fächerwagen (und benötigen zusätzlich einige A-Böcke
                                           für besondere Gläser z. B. für große Scheiben).
                                       •   Sie werden einen sehr guten Verschnitt haben - der Verschnitt ist der wich-
                                           tigste Parameter.
                                       •   Sie werden viel umsortieren müssen - dies erfordert eine große Anzahl an
                                           physikalischen Gestellen.
                                       Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Mo-
                                       dus:
01-2023 / 01-2023




                    F-66                                                                 A+W Production Feinplanung
                 Tutorial                                                                          Optimierungsmodi




                                                                Reihenfolge




                                       Ausbeute                                          Flexibilität



                                       Einstellungen in A+W Production
                                       Für eine Optimierung in diesem Modus sind im Programm folgende Einstellun-
                                       gen nötig:
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                       stellplatz markieren > Einstellungen




                                       Abb. F-27   Optimierungsmodus Freie Optimierung


                                       Sie sehen, es besteht eine Wechselwirkung zwischen Gruppierung und Sor-
                                       tierung, Ergebnis und der Anzahl an Gestellen. Je restriktiver Sie Gruppieren
                                       und Sortieren je mehr Einschränkungen haben Sie bezüglich der Optimierung
                                       und dem Ergebnis.
                                       Allerdings sind die Gruppierungen und Sortierungen nicht das einzig Wichtige
                                       für die Gestellzuweisung und Produktionsorganisation. Der Umgang mit
                                       Scheiben verschiedener Größe, Glasarten, Modellen, usw. ist ebenso wichtig
3,00 / 01-2023




                                       wie die Abstellen auf den Gestellen.




                 A+W Production Feinplanung                                                                    F-67
                    Optimierungsmodi                                                                           Tutorial




                                       Doppel-Optimierung
                                       Bei der Freien Optimierung kann eine Doppel-Optimierung, d. h. für unter-
                                       schiedliche Glasarten eine Optimierung mit identischem Schneidplan, durch-
                                       geführt werden.
                                       Der Vorteil dieser Art der Optimierung liegt darin, dass die Scheiben einer Ein-
                                       heit trotz Freier Optimierung geordnet abgelegt werden können. Die Scheiben
                                       einer Doppel-Optimierung können mit anderen Doppel- oder Freien Opti-
                                       mierungen auf einem Abstellplatz abgelegt werden.

                                          Doppel-Optimierung
                                          Eine Doppel-Optimierung kann nur für Abstellplätze mit dem Modus Einheit
                                          eingestellt werden.
01-2023 / 01-2023




                    F-68                                                               A+W Production Feinplanung
                 Tutorial                                                                          Optimierungsmodi




                                       Demos und Übungen
                                       In diesem Abschnitt sehen Sie, wie die Optimierung arbeitet.

                                       Komplexübung: Verschiedene Feinplanungsergebnisse gemein-
                                       sam mit dem Trainer vergleichen:
                                       Es wird der Ablauf der Optimierung gezeigt und erläutert.
                                       Folgender Dialog wird unter diesem Aspekt erklärt:
                                       •   Dialog Feinplanung für Lauf …

                                       Schritt 1: Testaufträge erfassen
                                       Erfassen Sie gemeinsam mit dem Trainer zwei Testaufträge, welche verschie-
                                       dene Produktaufbauten beinhalten. Die Stückzahlen der Positionen sollten je-
                                       weils zwischen 20 - 100 Stk. liegen. Es sollten mindestens ISO mit ESG
                                       erfasst werden, zusätzlich Float-Einzelscheiben und ESG-Einzelscheiben
                                       (über die Positionen und Aufträge verteilt). Es sollten Modelle, große Schei-
                                       ben und kleinere Scheiben vorhanden sein.
                                       Lasten Sie die Aufträge ein. Bilden Sie mit diesen beiden Testaufträgen und
                                       ggf. bereits im System vorhandenen Test- / Trainingsaufträgen einen Lauf
                                       (oder mehrere Läufe, je nach Anzahl an Testaufträgen).
                                       Geben Sie den Lauf / die Läufe in die Feinplanung. Schauen Sie sich unter
                                       Registerkarte 2 (Bockbelegung) das Ergebnis der Abstellplatzzuweisung
                                       durch die Feinplanung an. Klicken Sie nun auf die Schaltfläche Optimierung
                                       und sehen sich im A+W Plan Editor die Ergebnisse auf dem Schneidplan an.
                                       Was fällt Ihnen auf? Welche Daten können Sie erkennen und wie können Sie
                                       die Abstellplatzzuweisung auf dem Schneidplan lesen? Besprechen Sie die
                                       Ergebnisse mit Ihrem Trainer.

                                       Schritt 2: Wechseln Sie die Organisation
                                       Schließen Sie den Plan Editor und wählen Sie nun unter Registerkarte 5 (Or-
                                       ganisation) eine andere Master-Orga aus und führen Sie die Berechnung der
                                       Abstellplatzzuweisung neu durch. Betätigen Sie dazu die Schaltfläche Wie-
                                       derholen. Wechseln Sie nun wieder in Registerkarte 2 (Bockbelegung). Ver-
                                       gleichen Sie die Ergebnisse mit der ersten Abstellplatzzuweisung. Welche
                                       Unterschiede erkennen Sie? Besprechen Sie die Ergebnisse mit Ihrem Trai-
                                       ner.

                                       Schritt 3: Optimieren Sie den Lauf erneut
                                       Optimieren Sie den Lauf erneut und öffnen den Schneidplan (Plan Editor).
                                       Welche Unterschiede erkennen Sie? Besprechen Sie die Ergebnisse mit Ih-
                                       rem Trainer.
                                       Wechseln Sie in Registerkarte 5 und verändern Sie erneut die Master-Orga,
                                       in dem Sie Ihre eigene Orga aus (welche Sie vorher gemeinsam mit dem Trai-
                                       ner definiert haben). Vergleichen Sie die Ergebnisse.
3,00 / 01-2023




                                       Nehmen nun auch Änderungen an den Einstellungen bezüglich Gruppierung
                                       und Sortierung und Abstellmodus vor. Schauen Sie sich die neuen Ergebnisse
                                       in der Abstellplatzzuweisung und der Optimierung / dem Schneidplan an. Wel-


                 A+W Production Feinplanung                                                                   F-69
                    Optimierungsmodi                                                                        Tutorial




                                       che Unterschiede erkennen Sie? Besprechen Sie die Ergebnisse mit Ihrem
                                       Trainer.

                                       Schritt 4: Orga erweitern
                                       Erweitern Sie Ihre eigene Orga, bspw. um einen zusätzlichen Glastyp oder
                                       trennen Sie Modelle-groß von Modelle-klein.
                                       Wiederholen Sie nun Übungsschritt 3 erneut und so oft wie nötig mit verschie-
                                       denen Einstellungen und vergleichen Sie jeweils die Ergebnisse.
01-2023 / 01-2023




                    F-70                                                             A+W Production Feinplanung
                 Tutorial                                                                                  Orgas




                                       Orgas
                                       In diesem Themenblock lernen Sie die unterschiedlichen Organisationsfor-
                                       men kennen und erfahren, wie Sie damit in der A+W Production umgehen.
                                       Der Themenblock beinhaltet folgende Schulungseinheiten:
                                       •   Organisationsformen
                                       •   Produktionsreihenfolge
                                       •   A+W Standard-Orgas
                                       •   Abstellplatzorganisation
3,00 / 01-2023




                 A+W Production Feinplanung                                                                 F-71
                    Orgas                                                                              Tutorial




                            Organisationsformen
                            Lernziele

                            • Organisationsformen kennenlernen und verstehen.
                            • Die Auswirkungen der Orgas verstehen.
                            • Orgas einrichten können.


                            Nutzen

                            Um Läufe korrekt planen zu können, müssen Sie die unterschiedlichen Formen von
                            Organisationen verstehen. Nur dann ist es möglich, die Auswirkungen auf die realen
                            Produktionsabläufe nachvollziehen und vorab planen zu können.


                            Definitionen

                            Orga                       Eine Orga ist nichts anderes als ein datentechnisches
                                                       Regelwerk zur Abbildung der Produktion.

                            Orga-Gruppe                Die Orga-Gruppe ist ein Strukturelement einer Orga zur
                                                       genaueren Definition von Regeln und Bedingungen
                                                       bspw. für unterschiedliche Glasarten (ESG, VSG, ISO)
                                                       oder um innerhalb einer Glasart (ISO) zwischen der
                                                       Behandlung von Rechtecken und Modellen zu
                                                       unterscheiden.


                            Merke

                            Verschiedene Orgas         In Abhängigkeit von der Struktur des Unternehmens
                                                       können verschiedene Orgas definiert werden.

                            Orga-Gruppen/Bocktypen     Eine Orga besteht aus ein oder mehreren Orga-
                                                       Gruppen, die wiederum aus ein oder mehreren
                                                       Bocktypen bestehen.

                            Produktionsreihenfolge     Die Produktionsreihenfolge innerhalb einer Orga ergibt
                                                       sich durch die Reihenfolge der Orga-Gruppen.
01-2023 / 01-2023




                    F-72                                                      A+W Production Feinplanung
                 Tutorial                                                                                   Orgas




                                       Allgemein
                                       Um einen Lauf korrekt und effizient planen zu können, stehen Ihnen in der
                                       A+W Production sogenannte Orgas zur Verfügung. Eine Orga ist nichts ande-
                                       res als ein datentechnisches Regelwerk zur Abbildung der Produktion (bezüg-
                                       lich Produktionswegen, Prozessketten und Laufwegen und
                                       Gestellverwaltung). In Abhängigkeit von der Struktur des Unternehmens kön-
                                       nen beliebig viele Orgas (ESG-Orga, ISO-Orga, Bearbeitungs-Orga, etc.) de-
                                       finiert werden. Die unterschiedlichen Orgas organisieren die Abstellplätze
                                       jeweils vor den Produktionsschritten (ISO-Linie, Ofen, etc.).


                                       Baumstruktur
                                       Um die gewünschte Produktionsreihenfolge erzeugen zu können, wird jedem
                                       Lauf von der A+W Production eine sogenannte Master-Orga zugewiesen.
                                       Eine Master-Orga ist eine Gruppe von Orgas und besteht aus einer oder auch
                                       aus mehreren Orgas. Dabei ist es durchaus möglich, dass in einem Betrieb
                                       mehrerer dieser Master-Orgas vorhanden sind. In diesem Fall wird dem Lauf
                                       die Master-Orga zugewiesen, die auf die Produktmischung des Laufes am
                                       ehesten zutrifft.
                                       Eine Master-Orga muss immer genau eine Standard-Orga (Verwendung) ent-
                                       halten. Von allen anderen Typen darf eine Master-Orga maximal eine Orga
                                       enthalten. Eine Orga besteht aus einer oder mehrerer Orga-Gruppen, die wie-
                                       derum aus einem oder mehreren Bocktypen bestehen. An den Orga-Gruppen
                                       und an den Bocktypen kann man hinterlegen, wie die gewünschte Produkti-
                                       onsreihenfolge aussehen soll.

                                       Master Orga
                                                      Orga 1
                                                      Orga 2
                                                                   Orga-Gruppe 1
                                                                   Orga-Gruppe 2

                                                                            Bocktyp 1
                                                                                    Bedingung 1
                                                                            Bocktyp 2
                                                                                     Bedingung 2
                                                                    Orga-Gruppe 3
3,00 / 01-2023




                                       Abb. F-28     Beispiel aus der Praxis



                 A+W Production Feinplanung                                                                 F-73
                    Orgas                                                                             Tutorial




                            Master-Orga
                            Jede Master-Orga enthält eine Standardverwendungs-Orga. Zusätzlich kön-
                            nen für jeden Lostyp noch Verwendungs- und Produktions-Orgas erstellt wer-
                            den.
                            Wenn nun ein Teil einer Orga zugewiesen werden soll, wird erst überprüft, ob
                            eine Produktions-Orga für den entsprechenden Lostyp (im folgenden Beispiel
                            300) vorhanden ist. Wenn keine Produktions-Orga gefunden wird, wird nach
                            einer Standardproduktions-Orga gesucht. Auch die gibt es in unserem Bei-
                            spiel nicht. D. h. dem Teil wird keine Produktions-Orga zugewiesen. Als
                            nächstes wird die dem Lostyp zugeordnete Verwendungs-Orga gesucht. Falls
                            keine gefunden wird, bekommt das Teil die Standardverwendungs-Orga. Hier
                            ist aber die entsprechende Verwendungs-Orga (300) vorhanden und wird dem
                            Teil zugewiesen.

                                                                                            A
                                                                  Standard                  B

                                                                             700            C
                                                           300                              D

                                                                    700                     D

                            E               300

                            A Master-Orga                            D Verwendungs-Orga (blau) für
                            B Standardverwendungs-Orga (blau)          Lostyp 700
                            C Produktions-Orga (gelb) für Lostyp 700 E Teil mit Lostyp 300
                            Abb. F-29    Master-Orga Beispiel 1


                            Für das Teil mit dem Lostyp 700 wird sowohl eine Produktions- als auch eine
                            Verwendungs-Orga gefunden. Es wird also zwei verschiedenen Orgas mit un-
                            terschiedlichen Bocktypen (Verwendungs- und Produktionsbock) zugeordnet.
                            Man kann auch eine Standardproduktions-Orga definieren, die allen Teilen
                            zugewiesen wird, für die keine dem Lostyp entsprechende Standardprodukti-
                            ons-Orga gefunden wird. Im Gegensatz zu der Verwendungs-Orga muss in
                            der Produktions-Orga aber kein Auffang-Abstellplatz für alle Teile, die die Be-
                            dingungen keines anderen Abstellplatzes der Orga erfüllen, erstellt werden.
                            Wenn für ein Teil in der Produktions-Orga kein passender Abstellplatz gefun-
                            den wird, wird die Zuweisung zu einer Produktions-Orga einfach ignoriert. Das
                            bedeutet, wenn man für bestimmte Lostypen Produktions-Orga zuweisen will,
                            sollte man in dieser Orga einen Auffangabstellplatz erstellen, um zu verhin-
                            dern, dass die Zuweisung bei einzelnen Teilen einfach ignoriert wird.
01-2023 / 01-2023




                    F-74                                                           A+W Production Feinplanung
                 Tutorial                                                                                       Orgas




                                                                                                 A
                                                                            Standard             B

                                                                                       700       C
                                                                      300                        D

                                                                              700                D

                                       E               700

                                       A Master-Orga                            D Verwendungs-Orga (blau) für
                                       B Standardverwendungs-Orga (blau)          Lostyp 700
                                       C Produktions-Orga (gelb) für Lostyp 700 E Teil mit Lostyp 700
                                       Abb. F-30    Master-Orga Beispiel 2


                                       Die entsprechenden Einstellungen werden im Dialog Orga gemacht:
                                       Stammdaten > Feinplanung > Orga




                                       Abb. F-31    Master-Orga


                                        So erstellen Sie eine Master-Orga
                                       1 Wählen Sie in der Menü Stammdaten > Feinplanung > Orga.
                                       2 Betätigen Sie die Schaltfläche [Neu]. Es öffnet sich der Dialog Master-Or-
                                         ga.
                                       3 Im Feld Name der Master-Orga geben Sie einen Namen für die Master-
                                         Orga ein.
                                       4 Aktivieren oder deaktivieren Sie die Checkbox XOPT zusammen abstellen.
                                       5 Aktivieren oder deaktivieren Sie die Checkbox Schnell-Orga.
3,00 / 01-2023




                                       6 Wählen Sie aus der Kombobox Fertigungsgruppen die entsprechende
                                         Gruppe.



                 A+W Production Feinplanung                                                                     F-75
                    Orgas                                                                         Tutorial




                            7 Wählen Sie aus der Kombobox Pseudoserien die entsprechende Serie.
                            8 Wenn es sich um Pseudoserien handelt, tragen Sie im Feld Mindestmenge
                              einen entsprechenden Mindestwert ein.
                            9 Falls Sie Ihr System durch ein speziell angepasstes Script erweitert oder
                              angepasst haben, können Sie dieses Script im Feld Verwendetes Script
                              auswählen.
                            10 Mittels der Schaltfläche Auffüller können Sie definierte Auffüllbedingungen
                               auswählen.
                            11 Erfassen Sie das Feld Quasi-Teile. Um sich alle vorhandenen Quasi-Teile
                               anzeigen zu lassen, betätigen Sie die Schaltfläche […].
                            12 Aktivieren oder deaktivieren Sie die Checkbox Verwende Füller. Bei akti-
                               vierter Checkbox müssen die Felder Start Füller und Ende Füller erfasst
                               werden!
                            13 Aktivieren oder deaktivieren Sie die Checkbox Verwende Restblätter. Bei
                               aktivierter Checkbox müssen die Felder Start Restblatt und Ende Restblatt
                               erfasst werden!
                            14 Aktivieren oder deaktivieren Sie die Checkbox Doppeloptis zusammen.
                            15 Aktivieren oder deaktivieren Sie die Checkbox Verwende Bruchscheiben.
                               Bei aktivierter Checkbox müssen die Felder Start Bruch und Ende Bruch
                               erfasst werden!
                            16 Betätigen Sie die Schaltfläche Ok. Die neu angelegte Master-Orga er-
                               scheint automatisch im Orga-Dialog.


                             So fügen Sie einer Master-Orga eine vorhandene, neue Orga hinzu
                            1 Wählen Sie in der Menü Stammdaten > Feinplanung > Orga. Das Register
                              Master-Orga zeigt alle vorhandenen Master-Orgas.
                            2 Markieren Sie die Master-Orga, der Sie eine neue Orga hinzufügen möch-
                              ten.
                            3 Im Fenster rechts unten sind alle angelegten Orgas enthalten. Markieren
                              Sie die Orga, die Sie der Master-Orga hinzufügen möchten.
                            4 Betätigen Sie die Schaltfläche [Neu]. Unter der Master-Orga erscheint die
                              neue Orga.
01-2023 / 01-2023




                    F-76                                                   A+W Production Feinplanung
                 Tutorial                                                                                    Orgas




                                        So erstellen Sie eine neue Orga
                                       1 Wählen Sie in der Menü Stammdaten > Feinplanung > Orga.
                                       2 Öffnen Sie das Register Produktionsreihenfolge.




                                                                                                        .
                                          Abb. F-32   Register Produktionsreihenfolge


                                       3 Betätigen Sie die Schaltfläche [Neu]. Unter der letzten Orga erscheint die
                                         neue Orga. Diese trägt zunächst den Namen unknown / … .
                                       4 Markieren Sie diese Orga und betätigen Sie die Schaltfläche [Einstellun-
                                         gen]. Es öffnet sich der Dialog Orga.




                                          Abb. F-33   Orga Einstellungen


                                       5 Ändern Sie im Feld Name der Orga-Form den Namen von unknown in ei-
                                         nen sprechenden Namen.
                                       6 Wählen Sie aus der Kombobox Typ den entsprechenden Orga-Typ.
3,00 / 01-2023




                                       7 Aktivieren Sie die entsprechende Checkbox im Bereich Abstellmodus.
                                       8 Füllen Sie gegebenenfalls die Felder im Bereich Kein Teilen von … bei
                                         Bockbelegung von mehr als aus.


                 A+W Production Feinplanung                                                                   F-77
                    Orgas                                                                        Tutorial




                            9 Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.


                             So fügen Sie einer Orga eine neue Orga-Gruppe hinzu
                            1 Wählen Sie in der Menü Stammdaten > Feinplanung > Orga.
                            2 Öffnen Sie das Register Produktionsreihenfolge.
                            3 Markieren Sie die Orga, der Sie eine neue Orga-Gruppe hinzufügen möch-
                              ten und betätigen Sie die Schaltfläche [Neu]. Unter der markierten Orga er-
                              scheint die neue Orga-Gruppe mit dem Namen noname.
                            4 Markieren Sie die Orga-Gruppe mit dem Namen noname und betätigen Sie
                              die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog Orga-Gruppen.
                            5 Vergeben Sie im Feld Namen einen sprechenden Namen für die Orga-
                              Gruppe.
                            6 Wählen Sie aus der Kombobox Bildung der Gruppen die entsprechende
                              Gruppierung.
                            7 Aktivieren oder deaktivieren Sie die Checkbox Sortierung der Gruppen.
                            8 Wählen Sie aus der Kombobox Sortierung in den Gruppen die entspre-
                              chende Sortierung.
                            9 Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.


                            Ergänzende Informationen
                             Tutorial, “Orgas” auf Seite F-68
                             Softwarereferenz, “Orga” auf Seite F-131
                             Softwarereferenz, “Orga-Gruppen” auf Seite F-133


                             So legen Sie Gruppierungen und Sortierungen für einen Abstellplatz
                              an
                            1 Wählen Sie in der Menü Stammdaten > Feinplanung > Orga.
                            2 Öffnen Sie das Register Produktionsreihenfolge.
                            3 Markieren Sie die Orga-Gruppe, für die der Abstellplatz angelegt werden
                              soll und betätigen Sie die Schaltfläche [Neu]. Es wird automatisch ein Ab-
                              stellplatz mit dem Namen unknown angelegt.
                            4 Markieren Sie den Abstellplatz mit dem Namen unknown und betätigen Sie
                              die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog Einstellungen-
                              Abstellplatz.
01-2023 / 01-2023




                    F-78                                                    A+W Production Feinplanung
                 Tutorial                                                                                      Orgas




                                          Abb. F-34    Einstellungen - Abstellplatz


                                       5 Vergeben Sie im Feld Name anstelle von unknown einen sprechenden Na-
                                         men für den Abstellplatz.
                                       6 Wählen Sie aus der Kombobox Bildung der Gruppen nach welchem Regel-
                                         werk die Gruppen gebildet werden sollen (bspw. nach Kunden-Nr. und Auf-
                                         trags-Nr.).
                                       7 Aktivieren oder deaktivieren Sie die Checkbox Sortierung der Gruppen.
                                       8 Wählen Sie aus der Kombobox Abstellmodus Gruppen das Abstellverhal-
                                         ten der Gruppen je Stapel.
                                       9 Wählen Sie aus der Kombobox Optimierungsverhalten, ob die Reihenfolge
                                         der Gruppen sortiert sein soll (Supergruppen), umsortiert sein soll, oder ob
                                         alles unsortiert sein soll (Reihenfolge der Gruppen unsortiert und Gläser in-
                                         nerhalb der Gruppen unsortiert).
                                       10 Aktivieren oder deaktivieren Sie die Checkbox Auffang-Abstellplatz (hier
                                          landen alle Gläser, welche nicht durch Bedingungen spezifischen Abstell-
                                          plätzen zugewiesen werden). Jede Orga sollte ein Auffang-Gestell enthal-
                                          ten.
                                       11 Handelt es sich bei dem Abstellplatz um einen Verwendungsbock, nehmen
                                          Sie im Register Verwendung folgende Einstellungen vor:
                                          •   Erfassen Sie die Felder Von Bis.
                                          •   Aktivieren Sie die entsprechende Checkbox im Bereich Abstellmodus.
                                          •   Aktivieren oder deaktivieren Sie die Checkbox Zyklische Optimierung.
                                          •   Erfassen Sie das Feld Max. Anzahl Gruppen.
                                          •   Erfassen Sie das Feld Zyklusgröße.
                                          •   Aktivieren Sie die entsprechende Checkbox im Bereich Abstellplatz-
                                              Typ.
3,00 / 01-2023




                                       12 Handelt es sich bei dem Abstellplatz um einen Produktionsbock, nehmen
                                          Sie im Register Produktion folgende Einstellungen vor:



                 A+W Production Feinplanung                                                                     F-79
                    Orgas                                                                             Tutorial




                                   •   Erfassen Sie die Felder Von Bis.
                                   •   Aktivieren oder deaktivieren Sie die Checkbox Erzeuge Produktionsbö-
                                       cke.
                                   •   Erfassen Sie das Feld Max. Anzahl Gruppen.
                                   •   Aktivieren Sie die entsprechende Checkbox im Bereich Abstellplatz-
                                       Typ.
                            13 Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.


                            Bruch-Orga
                            Mit Hilfe der Bruch-Orga können Sie Bruchscheiben nach beliebigen Kriterien
                            auf Böcken abstellen. Die Bruch-Orga prüft automatisch anhand programmin-
                            terner Bedingungen die Eigenschaften der Bruchscheibe (des Basisglases,
                            d. h. des Floats). Bruch-Orgas definieren Sie, wie die anderen Orga-Formen
                            auch, im Dialog Orga.


                            Prüfreihenfolge
                            In einer Orga werden Abstellplätze angelegt, für die Bedingungen definiert
                            werden. Diese Bedingungen legen die Zuordnung einer Scheibe zu einem be-
                            stimmten Abstellplatztyp fest. Die Reihenfolge der Abstellplatztypen wird in
                            der Regel so angeordnet, dass mit den restriktivsten Bedingungen begonnen
                            wird und die Scheiben durch die Prüfreihenfolge der Abstellplatztypen wie
                            durch einen Filter laufen.

                            Teil
                                           Abstellplatztyp 1



                                           Abstellplatztyp 2


                                           Abstellplatztyp 3



                                           Abstellplatztyp 4


                                           Abstellplatztyp 5

                            Abb. F-35        Bedingung des Abstellplatzes


                            Zuerst werden die Spezialfälle überprüft. So wäre es zum Beispiel möglich,
                            dem in der Prüfreihenfolge an erster Stelle stehenden Abstellplatztyp die Be-
                            dingung Bin Modell zuzuweisen. Alle Modellscheiben würden sofort diesem
                            Abstellplatztyp zugewiesen. Der zweite Abstellplatztyp würde mit der Bedin-
                            gung Kleine Scheiben alle Scheiben bis zu einer einstellbaren Größe abfan-
01-2023 / 01-2023




                            gen, etc. Je weiter hinten in der Prüfreihenfolge ein Abstellplatztyp steht, desto
                            schwächer werden die Bedingungen.
                            Wird für ein Teil in einer Verwendungs-Orga kein Abstellplatztyp gefunden,
                            wird es dem Auffang-Abstellplatz zugeordnet. Ein Auffang-Abstellplatz zeich-


                    F-80                                                      A+W Production Feinplanung
                 Tutorial                                                                                     Orgas




                                       net sich dadurch aus, dass er entweder keine Bedingungen hat und somit
                                       stets am Ende der Prüfreihenfolge stehen sollte, oder aber das Kennzeichen
                                       Auffang-Abstellplatz gesetzt ist (wir empfehlen standardmäßig je Orga-Grup-
                                       pe -unabhängig davon ob Produktions- oder Verwendungsorga -ein Auffang-
                                       Gestell zu definieren. Setzen Sie dabei auch standardmäßig das Kennzeichen
                                       für das Auffang-Gestell).
                                       Jede Orga-Gruppe darf maximal einen solchen Auffang-Abstellplatz haben,
                                       wobei er für die Verwendungs-Orga zwingend vorgeschrieben ist.


                                        So ändern Sie die Prüfreihenfolge
                                       1 Wählen Sie in der Menü-Leiste Stammdaten > Feinplanung > Orga.
                                       2 Öffnen Sie das Register Prüfreihenfolge.
                                       3 Markieren Sie im Bereich der Orgas die Orga, für die die Prüfreihenfolge
                                         geändert werden soll.
                                       4 Markieren Sie im Bereich der Abstellplätze den Abstellplatz, dessen Rei-
                                         henfolge geändert werden soll.
                                       5 Verschieben Sie die Prüfreihenfolge des markierten Abstellplatzes mit Hilfe
                                         der Schaltflächen [Anfang], [Hoch], [Runter] oder [Ende] so lange, bis sich
                                         der Abstellplatz an der gewünschten Position befindet.




                                       Abb. F-36   Prüfreihenfolge


                                       Orga-Typ und Los-Typ
                                       Jedes Teil bzw. jede Bearbeitung hat seinen Teiletyp bzw. Bearbeitungstyp
                                       (Basisglas, VSG, etc.) und seine Beschaffungsart (Bestellt, Zuschnitt, etc.).
3,00 / 01-2023




                                       Abhängig von diesen beiden Eigenschaften wird das Teil bzw. die Bearbei-
                                       tung einem bestimmten Lostyp zugewiesen. Dadurch können Teile mit unter-
                                       schiedlichen Bearbeitungstypen ein und dem selben Lostyp zugeordnet und
                                       gemeinsam behandelt werden, z.B. bei der Zuweisung von Abstellplätzen.


                 A+W Production Feinplanung                                                                    F-81
                    Orgas                                                                         Tutorial




                            Darüber hinaus hat jede Orga einen bestimmten Orga-Typ. Mit diesem Orga-
                            Typ wird festgelegt, welche Teile der Orga zugewiesen werden. Idealerweise
                            definieren und filtern Sie nach Unterschieden und Ähnlichkeiten:
                            •   Modelle?, Rechtecke?
                            •   Höhe?, Gewicht?
                            •   …
                            Produktionslose werden für unterschiedliche Teiletypen und verschiedene
                            Glasarten im Zuschnitt gebildet.

                            Verwendungs- und Produktions-Orgas
                            Neben dem Orga-Typ ist eine weitere Eigenschaft der Orgas die Unterschei-
                            dung in Produktions-Orgas und Verwendungs-Orgas. Eine Verwendungs-
                            Orga muss erstellt werden, eine Produktions-Orga kann zusätzlich erstellt
                            werden. Jedes Teil bekommt also eine Verwendungs-Orga und kann bei Be-
                            darf eine zusätzliche Produktions-Orga erhalten.
                            Für den gleichen Bearbeitungsprozess wird bei einer Verwendungs-Orga im-
                            mer ein Verwendungsbock eingerichtet. Zusätzlich ist die Einrichtung eines
                            Produktionsbocks möglich.
                            Bei einer Produktions-Orga kann nur ein Produktionsbock erzeugt werden. In-
                            nerhalb einer Verwendungs-Orga sind die Bedingungen für die Verteilung der
                            Scheiben auf Verwendungs- und Produktionsböcke gleich. Die Zuordnung ei-
                            nes Artikels für den gleichen Bearbeitungsprozess zu einer Verwendungs-
                            und einer Produktions-Orga erlaubt innerhalb der Gruppierung und Sortierung
                            eine Verteilung der Scheiben auf Verwendungs- und Produktionsböcke nach
                            jeweils unterschiedlichen Bedingungen. So können z.B. die Scheiben auf den
                            Verwendungsböcken nach ihrer Größe sortiert und nach der Produktion (z.B.
                            bei ESG nach den Öfen) auf die Produktionsböcke nach der Verwendung im
                            ISO oder dem Versand verteilt werden.
                            Wenn einem Teil für eine bestimmte Bearbeitung eine Produktions-Orga zu-
                            geordnet wird, werden die Gruppierungen und Sortierungen auf den Abstell-
                            plätzen der Verwendungs-Orga ignoriert. Das Teil wird nach den
                            Gruppierungen und Sortierungen des Produktionsbocks der Produktions-
                            Orga auf die Abstellplätze hinter dem Bearbeitungsprozess verteilt.


                            Ergänzende Informationen
                             Softwarereferenz, “Produktion” auf Seite F-131


                            Globale Einstellungen
                            Die globalen Einstellungen stehen in Zusammenhang mit den Werten, die Sie
                            in den unten genannten Dialogen und Felder ausgewählt haben:
                            •   Dialog Orga-Gruppen:
                                – Felder: Bildung der Gruppen, Sortierung in den Gruppen.
01-2023 / 01-2023




                            •   Dialog Einstellungen-Abstellplatz:
                                – Felder: Bildung der Gruppen, Sortierung in den Gruppen.




                    F-82                                                       A+W Production Feinplanung
                 Tutorial                                                                                  Orgas




                                       Wurden bei den oben genannten Dialogen aus den Komboboxen der entspre-
                                       chenden Felder der Wert Keine explizit ausgewählt, so werden die Werte der
                                       globalen Einstellungen verwendet.

                                          Angaben in den Voreinstellungen
                                          Hier sollten Angaben gemacht werden, da beim Starten der A+W Produc-
                                          tion sonst Fehlermeldungen kommen.


                                       Ergänzende Informationen
                                        Softwarereferenz, “Voreinstellungen” auf Seite F-139
                                        Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
                                        Tutorial, “A+W Standard-Orgas” auf Seite F-84
3,00 / 01-2023




                 A+W Production Feinplanung                                                                F-83
                    Orgas                                                                       Tutorial




                            Demos und Übungen
                            Öffnen Sie die Stammdaten der Feinplanung. Schauen Sie sich gemeinsam
                            mit dem Trainer bereits vordefinierte Orgas an und analysieren Sie den Auf-
                            bau (Baustruktur, verschiedene Abstellplätze, Zuweisung von Bedingungen).
                            Was fällt Ihnen auf?
                            Besprechen Sie die Struktur gemeinsam mit Ihrem Trainer.
01-2023 / 01-2023




                    F-84                                                  A+W Production Feinplanung
                 Tutorial                                                                                            Orgas




                                       Produktionsreihenfolge
                                       Lernziele

                                       • Die Produktionsreihenfolge kennenlernen und verstehen.
                                       • Die Auswirkungen der Produktionsreihenfolge verstehen.


                                       Nutzen

                                       Durch die Kenntnisse der Einstellungsmöglichkeiten an den Orga-Gruppen bezüglich
                                       Gruppierung und Sortierung können Sie die reale Produktionsreihenfolge von Läufen
                                       und einzelnen Gläsern definieren und jederzeit flexibel ändern.


                                       Definitionen

                                       Gruppierungsschlüssel      Über den Gruppierungsschlüssels in einer Orga-Gruppe
                                                                  haben Sie die Möglichkeit, eine Produktionsreihenfolge
                                                                  zu bestimmen, ohne für die Abstellplätze eine
                                                                  Gruppierung/Sortierung festzulegen.


                                       Merke

                                       Ohne Gruppierung           Wenn in der Orga-Gruppe keine Gruppenbildung
                                                                  angegeben ist, richtet sich die Produktionsreihenfolge
                                                                  nach der Reihenfolge der Abstellplätze in der Orga-
                                                                  Gruppe.

                                       Mit Gruppierung            Wenn in der Orga-Gruppe z. B. nach Kunde gruppiert
                                                                  wird, so ergibt sich die Produktionsreihenfolge nicht
                                                                  länger einfach durch die Abfolge der Abstellplätze in der
                                                                  Orga-Gruppe. Das Hauptkriterium ist nun die
                                                                  Eigenschaft Kunde der Teile.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                           F-85
                    Orgas                                                                                Tutorial




                            Allgemein
                            Die Produktionsreihenfolge innerhalb einer Orga ergibt sich durch die Reihen-
                            folge der Orga-Gruppen. Innerhalb dieser in der Regel durch die Reihenfolge
                            der Bocktypen. Die Reihenfolge innerhalb der Bocktypen wird durch Gruppie-
                            rungs- und Sortierungsschlüssel hinterlegt.
                            Damit man nicht die gleiche Sortierung bei jedem Bocktyp innerhalb einer
                            Orga-Gruppe anlegen muss, kann man eine Sortierung in der Orga-Gruppe
                            hinterlegen. Diese wird an die in der Orga-Gruppe enthaltenen Bocktypen ver-
                            erbt und kann dort ergänzt werden.
                            Gleiches gilt für die Gruppierung, die man in der Orga-Gruppe angeben kann.
                            Auch diese wird an die Bocktypen vererbt und kann dort ergänzt werden. Al-
                            lerdings hat die Gruppierung in der Orga-Gruppe noch einen entscheidenden
                            Einfluss auf die Produktionsreihenfolge. Wenn z. B. in der Orga-Gruppe nach
                            Tour gruppiert wird, so ergibt sich die Produktionsreihenfolge nicht länger ein-
                            fach durch die Reihenfolge der Bocktypen in der Orga-Gruppe. Das Hauptkri-
                            terium ist nun die Eigenschaft Tour der Teile. Das bedeutet, dass zunächst
                            alle Teile der Tour A produziert werden, danach die der Tour B usw. Für eine
                            gegebene Tour wiederum ist allerdings die Reihenfolge der Bocktypen inner-
                            halb der Orga-Gruppe entscheidend. Allerdings gibt es hier eine Ausnahme,
                            wenn auf einem Bocktyp innerhalb der Orga-Gruppe die Reihenfolge der
                            Gruppen beliebig sein sollte. Das heißt, wenn die Optimierung diese frei an-
                            ordnen dürfte, so kann die in der Orga-Gruppe hinterlegte Gruppierung nicht
                            mehr länger die Reihenfolge der Gruppen bestimmt. In diesem Fall wird die
                            Reihenfolge wieder durch die Reihenfolge der Bocktypen bestimmt und die
                            Gruppierung der Orga-Gruppe wird an die darin enthaltenen Bocktypen ver-
                            erbt.


                            Gruppierungsschlüssel der Orga-Gruppen
                            Das Anlegen eines Gruppierungsschlüssels in einer Orga-Gruppe hat einen
                            entscheidenden Einfluss auf die Produktionsreihenfolge. Er bietet die Möglich-
                            keit, eine Produktionsreihenfolge zu bestimmen, ohne für die Abstellplätze
                            eine Gruppierung/Sortierung festzulegen.

                            Ohne Gruppierung
                            Wenn in der Orga-Gruppe keine Gruppenbildung angegeben ist, richtet sich
                            die Produktionsreihenfolge nach der Reihenfolge der Abstellplätze in der
                            Orga-Gruppe (z. B. kleine Scheiben, Sprossen, usw.).


                                                                                            Orga-Gruppe
                             Abstellplatztyp A
01-2023 / 01-2023




                             Abstellplatztyp B




                            Abb. F-37       Produktionsreihenfolge ohne Gruppierung in der Orga-Gruppe


                    F-86                                                       A+W Production Feinplanung
                 Tutorial                                                                                           Orgas




                                       Mit Gruppierung
                                       Wenn in der Orga-Gruppe z. B. nach Kunde gruppiert wird, so ergibt sich die
                                       Produktionsreihenfolge nicht länger einfach durch die Abfolge der Abstellplät-
                                       ze in der Orga-Gruppe. Das Hauptkriterium ist nun die Eigenschaft Kunde der
                                       Teile. Im Beispiel würde dies bedeuten, dass zunächst alle Teile des Kunden
                                       A produziert werden, danach die des Kunden B usw. Für einen Kunden richtet
                                       sich die Abfolge der Produktion allerdings wieder nach der Reihenfolge der
                                       Abstellplätze in der Orga-Gruppe.
                                       Innerhalb der Gruppen ist die Reihenfolge der Teile frei, d. h. es gibt keine Ein-
                                       schränkung bei der Optimierung (XOPTS 5.2).


                                                             Produktionsreihenfolge
                                                        mit Gruppierung in der Orgagruppe




                                        Abstellplatztyp A




                                         Abstellplatztyp B




                                                                          A                         B
                                       A Kunde A                                            B Kunde B
                                       Abb. F-38        Produktionsreihenfolge mit Gruppierung in der Orga-Gruppe


                                          Bestimmung der Produktionsreihenfolge durch den
                                          Gruppierungsschlüssel
                                          Damit die Produktionsreihenfolge durch den Gruppierungsschlüssel der
                                          Orga-Gruppe bestimmt werden kann, darf bei den Abstellplätzen keine
                                          Sortierung mit Auftrags- und Positions-Nr. eingestellt sein. Dies würde
                                          dazu führen, dass die Optimierung nach XOPTS 6.1 durchgeführt und der
                                          Gruppierungsschlüssel der Orga-Gruppe ignoriert wird.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                         F-87
                    Orgas                                                                               Tutorial




                            A+W Standard-Orgas
                            Lernziele

                            • Unterschiedliche Standard-Orgas kennenlernen und verstehen.
                            • Entsprechende Einstellungen in A+W Production nachvollziehen können.


                            Nutzen

                            Die Standard-Orgas haben den Vorteil, dass sie bereits vollständig angelegt sind und
                            Sie diese gleich nutzen können. Das spart Ihnen Zeit und minimiert das Fehlerrisiko
                            beim Einrichten.


                            Definitionen

                            Standard-Orga               Fertig eingerichtete Orgas von A+W.


                            Merke

                            Bei Änderungen              raten wir Ihnen, die gewünschte Standard-Orga zu
                                                        kopieren und die kopierte Version dann zu ändern. So
                                                        bleibt Ihnen das Original immer erhalten und Sie
                                                        minimieren das Fehlerrisiko.
01-2023 / 01-2023




                    F-88                                                       A+W Production Feinplanung
                 Tutorial                                                                                         Orgas




                                       Abstellplatzorganisation
                                       Für die Organisation der Glasproduktion mit A+W Production stehen bereits
                                       verschiedene Regelwerke, so genannte Standard-Orgas zur Auswahl. Jede
                                       Orga sortiert und gruppiert die zu produzierenden Scheiben nach anderen Ge-
                                       sichtspunkten und optimiert die Produktion hinsichtlich unterschiedlicher An-
                                       forderungen.
                                       Die folgende Tabelle gibt eine Übersicht über die verfügbaren Orgas und de-
                                       ren Eigenschaften. Die Reihenfolge ist von produktionsorientierten Orgas hin
                                       zu versandorientierten Orgas.

                                       Name               Beschreibung

                                       A-Böcke SZR        Diese Orga ist sinnvoll bei einem Bieger, der starke SZR-
                                                          Restriktionen aufweist und keinen Puffer zum Vorproduzieren
                                                          und Sortieren der Rahmen hat. Die Orga bietet keine
                                                          Versandorientierung.

                                       A-Böcke            Diese Orga liefert eine moderat versandorientierte
                                                          Produktionsreihenfolge nach Kunde und Auftrag, allerdings
                                                          mit der Restriktion, dass vor der Linie stets nur von wenigen
                                                          Böcken abgearbeitet wird. Der Grad der Versandausrichtung
                                                          kann durch Setzen der globalen Einstellungen für Gruppierung
                                                          und Sortierung gesteuert werden.
                                                          Die Orga ist darauf ausgelegt, dass nach der ISO-Produktion
                                                          umgepackt wird.

                                       A-Böcke Versand    Diese Orga liefert eine versandorientierte
                                                          Produktionsreihenfolge, bei der vor der Linie im Wechsel von
                                                          mehreren A-Böcken abgegriffen wird. Die Orga benötigt
                                                          Abstellplätze vor und hinter der Linie und liefert eine
                                                          verpackungsgerechte Produktionsreihenfolge. Hinter der Linie
                                                          müssen Gestelle je Kunde bereitgestellt werden.

                                       Fächerwagen        Diese Orga entspricht im Aufbau und der Abstellplatzvergabe
                                                          weitgehend der Orga A-Böcke, es werden aber Fächerwagen
                                                          für die Hauptabstellplätze genommen, wodurch i.d.R. ein
                                                          erheblich besserer Verschnitt gewährleistet ist. Große und
                                                          kleine Einheiten sowie Serien werden auf A-Böcke
                                                          herausgezogen.
                                                          Abweichend zur Orga A-Böcke ist die Produktionsreihenfolge
                                                          stets versandgerecht. Zwar wird mit der Orga Fächerwagen
                                                          ebenfalls ein Bock nach dem anderen vor der Linie
                                                          abgearbeitet, doch können auf Fächerwagen alle benötigten
                                                          Glasarten zusammengestellt und auf Versandreihenfolge
                                                          gebracht werden.

                                       Aufgefüllte        Diese Orga vermeidet schwach gefüllte Fächerwagen und
                                       Fächerwagen        zieht alle Fächerwagen in Produktionsreihenfolge zusammen.
                                                          Zuerst werden alle Fächerwagen abgearbeitet, anschließend
                                                          kommen die Spezialitäten auf A-Böcken.

                                       Tab. F-1
3,00 / 01-2023




                 A+W Production Feinplanung                                                                        F-89
                    Orgas                                                                         Tutorial




                            A-Böcke SZR
                            Diese Orga ist für Isolierglas-produzierende Betriebe sinnvoll bei denen der
                            Bieger starke SZR-Restriktionen aufweist und keinen Puffer zum Vorproduzie-
                            ren und Sortieren der Rahmen hat.
                            Die Orga A-Böcke SZR bildet eine nach SZR gruppierte Produktionsreihenfol-
                            ge ab, bei der vor der Linie ein A-Bock nach dem anderen abgearbeitet wird.
                            •   Die Orga bietet keine Versandorientierung.
                            •   Es werden ausschließlich A-Böcke verwendet (Tiefe 200 mm, Breite 2000
                                mm).
                            •   Abstellmodus ist Einheit (die Scheiben einer Einheit stehen auf demselben
                                Abstellplatz auf verschiedenen Stapeln).

                            Produktionsreihenfolge
                            Die Produktionsreihenfolge bildet sich aus folgenden optimierten Abstellplatz-
                            gruppen (in Produktionsreihenfolge):
                            •   Normale ISO-Scheiben
                            •   ISO-Modellscheiben
                            •   ISO-Scheiben mit Sprossen
                            •   ISO-Modellscheiben mit Sprossen
                            •   Stufen-ISO
                            •   3-fach ISO
                            Jede dieser Gruppen besteht aus 5 SZR-Abstellplatzgruppen, die in der Pro-
                            duktionsreihenfolge nacheinander abgewickelt werden. Die SZR-Gruppen
                            sind durch einstellbare Schwellwerte getrennt:
                            SZR-Gruppe 1
                                > SZR-Schwelle1
                            SZR-Gruppe 2
                                > SZR-Schwelle2
                            SZR-Gruppe 3
                                > SZR-Schwelle3
                            SZR-Gruppe 4
                                > SZR-Schwelle4
                            SZR-Gruppe 5
                            Die Schwellwerte sind wie folgt voreingestellt und können angepasst werden:
                            •   SZR-Schwelle1 = 10 mm
                            •   SZR-Schwelle2 = 12 mm
                            •   SZR-Schwelle3 = 16 mm
                            •   SZR-Schwelle4 = 18 mm
01-2023 / 01-2023




                            Innerhalb jeder SZR-Abstellplatzgruppe gibt es in Produktionsreihenfolge fol-
                            gende Abstellplätze (klein nach groß, da hinter der Linie umgepackt werden
                            muss):



                    F-90                                                   A+W Production Feinplanung
                 Tutorial                                                                                        Orgas




                                       •   Serien (Serienflag gesetzt oder Stück ≥ 10)
                                       •   Kleine Einheiten, Bedingung kleine Einheit, Voreinstellung:
                                           – kleine Kante < 300 oder
                                           – große Kante < 500)
                                       •   Normale Einheiten
                                       •   Große Einheiten, Bedingung große Einheit, Voreinstellung:
                                           – große Kante > 2100 oder
                                           – kleine Kante > 1600)
                                       Innerhalb jedes Abstellplatzes ist die Produktionsreihenfolge nach Kunden
                                       und Auftrag gruppiert. Die Positionsreihenfolge innerhalb eines Auftrags ist
                                       frei, d. h. hier liegen Freiheitsgrade für die Optimierung. Mit Ausnahme der Se-
                                       rienabstellplätze, können je Gestell mehrere Kunden und Aufträge vorkom-
                                       men. Serien stehen positionsweise getrennt.
                                       Für Scheiben, die nicht in die oben genannten Abstellplatzgruppen passen,
                                       sind Auffang-Abstellplätze vorhanden, die aber nicht weiter optimiert sind.
                                       Dazu zählen:
                                       •   ESG-Scheiben
                                       •   VSG-Scheiben
                                       •   Nicht zugeordnete Einheiten

                                       Optimierung
                                       Optimierungstechnisch kann bei dieser Orga ein XOPTS ab Modus 5/1 ange-
                                       wendet werden. Dies ist abhängig von dem Sortieraufwand, welchen ein ISO-
                                       Betrieb bereit ist, zu investieren, ebenfalls natürlich von dem Optimierungser-
                                       gebnis.
                                       Je größer die Restriktionen auf einem A-Bock innerhalb eines Abstellplatzes
                                       sind, desto größer kann der Optimierungsverschnitt ausfallen.
                                       Der Nachteil bei dieser Organisation liegt darin, dass es zum einen sehr viele
                                       Abstellplätze geben kann und zum anderen der Sortieraufwand nach der Pro-
                                       duktion wesentlich höher wird.

                                       Nummernkreise
                                       Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze ver-
                                       teilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinter-
                                       legt:

                                       Orgagruppe                     Abstellplatz                       Nummernkreis
                                                                                                         von     bis

                                       Auffänger                      Auffänger                          10000   10999

                                       ESG - bearbeitet               bearbeitet - Serien                8951    8999

                                       ESG - bearbeitet               bearbeitet - große Scheiben        8921    8950
3,00 / 01-2023




                                       ESG - bearbeitet               bearbeitet - kleine Scheiben       8901    8920

                                       ESG - bearbeitet               bearbeitet                         8501    8899

                                       Tab. F-2     Nummernkreise der Produktionsorga A-Böcke SZR


                 A+W Production Feinplanung                                                                       F-91
                    Orgas                                                                               Tutorial




                            Orgagruppe                       Abstellplatz                        Nummernkreis
                                                                                                 von     bis

                            ESG - gesäumt                    Gesäumt - große Scheiben            8421    8450

                            ESG - gesäumt                    Gesäumt - kleine Scheiben           8401    8420

                            ESG - gesäumt                    Gesäumt                             8001    8399

                            ESG - gesäumt                    Gesäumt - Serien                    8451    8499

                            Einfachglas                      große Scheiben                      7921    7950

                            Einfachglas                      kleine Scheiben                     7901    7920

                            Einfachglas                      Einfach                             7501    7899

                            Einfachglas                      Serien                              7951    7999

                            Einfachglas - geschliffen        geschliffen - Serien                7451    7499

                            Einfachglas - geschliffen        geschliffen - große Scheiben        7421    7450

                            Einfachglas - geschliffen        geschliffen - kleine Scheiben       7401    7420

                            Einfachglas - geschliffen        Einfach - geschliffen               7001    7399

                            ISO - Dreifach                   Iso - Dreifach - große Einheiten    6921    6950

                            Iso - Dreifach                   Iso - Dreifach                      6001    6899

                            Iso - Dreifach                   Iso - Dreifach - kleine Einheiten   6901    6920

                            Iso - Dreifach                   Iso - Dreifach - Serien             6951    6999

                            Iso - Modell-Sprossen-szrgr1     Iso-1 - Mod-Spross - klein          1311    1320

                            Iso - Modell-Sprossen-szrgr1     Iso-1 - Mod-Spross - Serie          1351    1399

                            Iso - Modell-Sprossen-szrgr1     Iso-1 - Mod-Spross                  1901    1950

                            Iso - Modell-Sprossen-szrgr1     Iso-1 - Mod-Spross - gross          1321    1350

                            Iso - Modell-Sprossen-szrgr2     Iso-2 - Mod-Spross - gross          2321    2350

                            Iso - Modell-Sprossen-szrgr2     Iso-2 - Mod-Spross - klein          2311    2320

                            Iso - Modell-Sprossen-szrgr2     Iso-2 - Mod-Spross - Serie          2351    2399

                            Iso - Modell-Sprossen-szrgr2     Iso-2 - Mod-Spross                  2901    2950

                            Iso - Modell-Sprossen-szrgr3     Iso-3 - Mod-Spross - gross          3321    3350

                            Iso - Modell-Sprossen-szrgr3     Iso-3 - Mod-Spross                  3901    3950

                            Iso - Modell-Sprossen-szrgr3     Iso-3 - Mod-Spross - klein          3311    3320

                            Iso - Modell-Sprossen-szrgr3     Iso-3 - Mod-Spross - Serie          3351    3399

                            Iso - Modell-Sprossen-szrgr4     Iso-4 - Mod-Spross - Serie          4351    4399
01-2023 / 01-2023




                            Iso - Modell-Sprossen-szrgr4     Iso-4 - Mod-Spross                  4901    4950

                            Iso - Modell-Sprossen-szrgr4     Iso-4 - Mod-Spross - klein          4311    4320

                            Tab. F-2         Nummernkreise der Produktionsorga A-Böcke SZR


                    F-92                                                        A+W Production Feinplanung
                 Tutorial                                                                                         Orgas




                                       Orgagruppe                     Abstellplatz                         Nummernkreis
                                                                                                           von     bis

                                       Iso - Modell-Sprossen-szrgr4   Iso-4 - Mod-Spross - gross           4321   4350

                                       Iso - Modell-Sprossen-szrgr5   Iso-5 - Mod-Spross - Serie           5351   5399

                                       Iso - Modell-Sprossen-szrgr5   Iso-5 - Mod-Spross - klein           5311   5320

                                       Iso - Modell-Sprossen-szrgr5   Iso-5 - Mod-Spross                   5901   5950

                                       Iso - Modell-Sprossen-szrgr5   Iso-5 - Mod-Spross - gross           5321   5350

                                       Iso - Modelle-szrgr1           Iso-1 - Modelle - nicht versiegelt   1241   1250

                                       Iso - Modelle-szrgr1           Iso-1 - Modelle                      1701   1799

                                       Iso - Modelle-szrgr1           Iso-1 - Modelle - kleine Einheiten   1211   1220

                                       Iso - Modelle-szrgr1           Iso-1 - Modelle - große Einheiten    1221   1240

                                       Iso - Modelle-szrgr1           Iso-1 - Modelle - Serien             1251   1299

                                       Iso - Modelle-szrgr2           Iso-2 - Modelle - kleine Einheiten   2211   2220

                                       Iso - Modelle-szrgr2           Iso-2 - Modelle - Serien             2251   2299

                                       Iso - Modelle-szrgr2           Iso-2 - Modelle                      2701   2799

                                       Iso - Modelle-szrgr2           Iso-2 - Modelle - große Einheiten    2221   2240

                                       Iso - Modelle-szrgr2           Iso-2 - Modelle - nicht versiegelt   2241   2250

                                       Iso - Modelle-szrgr3           Iso-3 - Modelle - große Einheiten    3221   3240

                                       Iso - Modelle-szrgr3           Iso-3 - Modelle - nicht versiegelt   3241   3250

                                       Iso - Modelle-szrgr3           Iso-3 - Modelle - kleine Einheiten   3211   3220

                                       Iso - Modelle-szrgr3           Iso-3 - Modelle - Serien             3251   3299

                                       Iso - Modelle-szrgr3           Iso-3 - Modelle                      3701   3710

                                       Iso - Modelle-szrgr4           Iso-4 - Modelle                      4701   4799

                                       Iso - Modelle-szrgr4           Iso-4 - Modelle - große Einheiten    4221   4240

                                       Iso - Modelle-szrgr4           Iso-4 - Modelle - nicht versiegelt   4241   4250

                                       Iso - Modelle-szrgr4           Iso-4 - Modelle - Serien             4251   4299

                                       Iso - Modelle-szrgr4           Iso-4 - Modelle - kleine Einheiten   4211   4220

                                       Iso - Modelle-szrgr5           Iso-5 - Modelle - Serien             5251   5299

                                       Iso - Modelle-szrgr5           Iso-5 - Modelle - nicht versiegelt   5241   5250

                                       Iso - Modelle-szrgr5           Iso-5 - Modelle - große Einheiten    5221   5240

                                       Iso - Modelle-szrgr5           Iso-5 - Modelle - kleine Einheiten   5211   5220

                                       Iso - Modelle-szrgr5           Iso-5 - Modelle                      5701   5799
3,00 / 01-2023




                                       Iso - Sprossen-szrgr1          Iso-1 - Sprosse - Serie              1451   1499

                                       Tab. F-2      Nummernkreise der Produktionsorga A-Böcke SZR


                 A+W Production Feinplanung                                                                        F-93
                    Orgas                                                                           Tutorial




                            Orgagruppe                    Abstellplatz                       Nummernkreis
                                                                                             von     bis

                            Iso - Sprossen-szrgr1         Iso-1 - Sprosse - klein            1411    1420

                            Iso - Sprossen-szrgr1         Iso-1 - Sprosse                    1801    1899

                            Iso - Sprossen-szrgr1         Iso-1 - Sprosse - gross            1421    1450

                            Iso - Sprossen-szrgr2         Iso-2 - Sprosse - klein            2411    2420

                            Iso - Sprossen-szrgr2         Iso-2 - Sprosse - gross            2421    2450

                            Iso - Sprossen-szrgr2         Iso-2 - Sprosse                    2801    2899

                            Iso - Sprossen-szrgr2         Iso-2 - Sprosse - Serie            2451    2499

                            Iso - Sprossen-szrgr3         Iso-3 - Sprosse - gross            3421    3450

                            Iso - Sprossen-szrgr3         Iso-3 - Sprosse - klein            3411    3420

                            Iso - Sprossen-szrgr3         Iso-3 - Sprosse - Serie            3451    3499

                            Iso - Sprossen-szrgr3         Iso-2 - Sprosse                    3801    3899

                            Iso - Sprossen-szrgr4         Iso-4 - Sprosse - klein            4411    4420

                            Iso - Sprossen-szrgr4         Iso-4 - Sprosse - Serie            4451    4499

                            Iso - Sprossen-szrgr4         Iso-4 - Sprosse                    4801    4899

                            Iso - Sprossen-szrgr4         Iso-4 - Sprosse - gross            4421    4450

                            Iso - Sprossen-szrgr5         Iso-5 - Sprosse                    5801    5899

                            Iso - Sprossen-szrgr5         Iso-5 - Sprosse - gross            5421    5450

                            Iso - Sprossen-szrgr5         Iso-5 - Sprosse - Serie            5451    5499

                            Iso - Sprossen-szrgr5         Iso-5 - Sprosse - klein            5411    5420

                            Iso - Stufe-szrgr1            Iso-1 - Stufe                      1951    1999

                            Iso - Stufe-szrgr1            Iso-1 - Stufe - große Einheiten    1521    1550

                            Iso - Stufe-szrgr1            Iso-1 - Stufe - kleine Einheiten   1511    1520

                            Iso - Stufe-szrgr1            Iso-1 - Stufe - Serien             1551    1599

                            Iso - Stufe-szrgr2            Iso-2 - Stufe                      2951    2999

                            Iso - Stufe-szrgr2            Iso-2 - Stufe - große Einheiten    2521    2550

                            Iso - Stufe-szrgr2            Iso-2 - Stufe - Serien             2551    2599

                            Iso - Stufe-szrgr2            Iso-2 - Stufe - kleine Einheiten   2511    2520

                            Iso - Stufe-szrgr3            Iso-3 - Stufe - kleine Einheiten   3511    3520

                            Iso - Stufe-szrgr3            Iso-3 - Stufe                      3951    3999
01-2023 / 01-2023




                            Iso - Stufe-szrgr3            Iso-3 - Stufe - große Einheiten    3521    3550

                            Iso - Stufe-szrgr3            Iso-3 - Stufe - Serien             3551    3599

                            Tab. F-2      Nummernkreise der Produktionsorga A-Böcke SZR


                    F-94                                                     A+W Production Feinplanung
                 Tutorial                                                                                      Orgas




                                       Orgagruppe                    Abstellplatz                       Nummernkreis
                                                                                                        von     bis

                                       Iso - Stufe-szrgr4            Iso-4 - Stufe                      4951   4999

                                       Iso - Stufe-szrgr4            Iso-4 - Stufe - Serien             4551   4599

                                       Iso - Stufe-szrgr4            Iso-4 - Stufe - große Einheiten    4521   4550

                                       Iso - Stufe-szrgr4            Iso-4 - Stufe - kleine Einheiten   4511   4520

                                       Iso - Stufe-szrgr5            Iso-5 - Stufe                      5951   5999

                                       Iso - Stufe-szrgr5            Iso-5 - Stufe - große Einheiten    5521   5550

                                       Iso - Stufe-szrgr5            Iso-5 - Stufe - kleine Einheiten   5511   5520

                                       Iso - Stufe-szrgr5            Iso-5 - Stufe - Serien             5551   5599

                                       Iso-szrgr1                    Iso-1 - kleine Einheiten           1111   1120

                                       Iso-szrgr1                    Iso-1                              1601   1699

                                       Iso-szrgr1                    Iso-1 - große Einheiten            1121   1150

                                       Iso-szrgr1                    Iso-1 - Serien                     1151   1199

                                       Iso-szrgr2                    Iso-2 - große Einheiten            2121   2150

                                       Iso-szrgr2                    Iso-2 - kleine Einheiten           2111   2120

                                       Iso-szrgr2                    Iso-2                              2601   2699

                                       Iso-szrgr2                    Iso-2 - Serien                     2151   2199

                                       Iso-szrgr3                    Iso-3                              3601   3699

                                       Iso-szrgr3                    Iso-3 - kleine Einheiten           3111   3120

                                       Iso-szrgr3                    Iso-3 - Serien                     3151   3199

                                       Iso-szrgr3                    Iso-3 - große Einheiten            3121   3150

                                       Iso-szrgr4                    Iso-4 - kleine Einheiten           4111   4120

                                       Iso-szrgr4                    Iso-4                              4601   4699

                                       Iso-szrgr4                    Iso-4 - große Einheiten            4121   4150

                                       Iso-szrgr4                    Iso-4 - Serien                     4151   4199

                                       Iso-szrgr5                    Iso-5 - große Einheiten            5121   5150

                                       Iso-szrgr5                    Iso-5 - kleine Einheiten           5111   5120

                                       Iso-szrgr5                    Iso-5 - Serien                     5151   5199

                                       Iso-szrgr5                    Iso-5                              5601   5699

                                       VSG                           VSG - große Scheiben               9921   9950

                                       VSG                           VSG - Serien                       9951   9990
3,00 / 01-2023




                                       VSG                           VSG                                9001   9899

                                       Tab. F-2      Nummernkreise der Produktionsorga A-Böcke SZR


                 A+W Production Feinplanung                                                                     F-95
                    Orgas                                                                       Tutorial




                            Orgagruppe                    Abstellplatz                   Nummernkreis
                                                                                         von     bis

                            VSG                           VSG - kleine Scheiben          9901    9920

                            Tab. F-2     Nummernkreise der Produktionsorga A-Böcke SZR

                            Die Orga A-Böcke SZR optimiert auf Einheiten. Sie ist einfach zu handhaben
                            verursacht aber ggf. einen höheren Sortieraufwand nach der Linie und Sie be-
                            nötigen daher mehr Platz für Gestelle:




                            Einstellungen in A+W Production
                            Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in
                            A+W Production für ISO-SZRGR1.
                            Einstellungen der Orga-Gruppe:




                            Abb. F-39    Einstellungen der Orga-Gruppe
01-2023 / 01-2023




                            Einstellungen Abstellplatz:




                    F-96                                                   A+W Production Feinplanung
                 Tutorial                                                                                    Orgas




                                       Abb. F-40    Einstellungen Abstellplatz


                                       Ergänzende Informationen
                                        Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                                       ISO-A-Böcke
                                       Die Orga A-Böcke liefert eine moderat versandorientierte Produktionsreihen-
                                       folge nach Kunde und Auftrag. Es besteht die Einschränkung, dass vor der Li-
                                       nie immer nur von wenigen Böcken abgearbeitet wird. Der Grad der
                                       Versandausrichtung kann durch Setzen der globalen Einstellungen für Grup-
                                       pierung und Sortierung gesteuert werden.
                                       Die Orga ist darauf ausgelegt, dass nach der ISO-Produktion umgepackt wird.
                                       •   Es werden ausschließlich A-Böcke verwendet (Tiefe 200, Breite 2000).
                                       •   Der Abstellmodus ist Einheit.

                                       Produktionsreihenfolge
                                       Die Produktionsreihenfolge bildet sich aus folgenden Abstellplatzgruppen (in
                                       Produktionsreihenfolge):
                                       •   Normale ISO-Scheiben
                                       •   ISO-Modellscheiben
3,00 / 01-2023




                                       •   ISO-Modellscheiben mit Sprossen
                                       •   ISO-Scheiben mit Sprossen
                                       •   Stufen-ISO


                 A+W Production Feinplanung                                                                   F-97
                    Orgas                                                                             Tutorial




                            •   3-fach ISO
                            Diese Abstellplatzgruppen sind jeweils unterteilt nach (in Produktionsreihen-
                            folge):
                            •   Serien (Serienflag gesetzt oder Stück ≥ 10)
                            •   Kleine Einheiten, Bedingung kleine Einheit, Voreinstellung:
                                – kleine Kante < 300 oder
                                – große Kante < 500)
                            •   Normale Einheiten
                            •   Große Einheiten, Bedingung große Einheit, Voreinstellung:
                                – große Kante > 2100 oder
                                – kleine Kante > 1600)
                            Wegen des notwendigen Umpackens hinter der Linie, geht die Reihenfolge
                            von klein nach groß.
                            Für Scheiben, die nicht in die oben genannten Abstellplatzgruppen passen
                            sind Auffang-Abstellplätze vorhanden, die aber nicht weiter optimiert sind.
                            Dazu zählen:
                            •   ESG-Scheiben
                            •   VSG-Scheiben
                            •   Nicht zugeordnete Einheiten

                            Gruppierung und Sortierung
                            Die Gruppierung und Sortierung der Gläser innerhalb jedes Abstellplatzes
                            richtet sich nach der globalen Voreinstellung für Gruppierung und Sortierung.
                            Mit Ausnahme der Serienabstellplätze, enthalten alle A-Böcke meist mehrere
                            Kunden und Aufträge. Serien stehen positionsweise getrennt.

                            Voreinstellung
                            Die Parameter der globalen Sortierung sind wie folgt voreingestellt:
                            •   Gruppierung = Kunde+Auftrag
                            •   Sortierung = Keine
                            Das bedeutet, dass innerhalb der o.g. Abstellplätze (also z.B. Normal ISO -
                            kleine Einheiten) Kundenaufträge zusammengehalten werden. Dazu müssen
                            verschiedene Gläserkombinationen vor der Linie zusammengeführt - also von
                            unterschiedlichen Böcken abgenommen - werden. Die Positionsreihenfolge
                            innerhalb eines Auftrags ist frei, d.h. hier liegen Freiheitsgrade für die Optimie-
                            rung.

                            Änderung der Einstellung
                            Wenn sehr wenig Platz vor der Linie vorhanden ist, können die globalen Vor-
                            einstellungen geändert werden:
01-2023 / 01-2023




                            •   Gruppierung = Artikel+Kunde+Auftrag
                            •   Sortierung = Keine
                            Der zusätzliche Artikelschlüssel bewirkt, dass innerhalb der Abstellplätze ein
                            Glasaufbau nach dem anderen abgearbeitet wird. Dies bedeutet, dass die


                    F-98                                                      A+W Production Feinplanung
                 Tutorial                                                                                     Orgas




                                       Produktionsreihenfolge nur noch innerhalb einer Gläserkombination versand-
                                       orientiert ist. Je nach Produktmix variiert der Grad der Versandorientierung.

                                       Optimierung
                                       Optimierungstechnisch kann bei dieser Orga ein XOPTS ab Modus 5/1 ange-
                                       wendet werden. Dies ist abhängig von dem Sortieraufwand, welchen ein ISO-
                                       Betrieb bereit ist, zu investieren, und vom Optimierungsergebnis.
                                       Je größer die Restriktionen auf einem A-Bock innerhalb eines Abstellplatzes
                                       sind, desto größer kann der Optimierungsverschnitt ausfallen.

                                       Nummernkreise
                                       Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze ver-
                                       teilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinter-
                                       legt:

                                       Orgagruppe                  Abstellplatz                     Nummernkreis
                                                                                                     von    bis

                                       Auffänger                   Auffänger                       10000   10999

                                       ESG - bearbeitet            bearbeitet                      8501    8899

                                       ESG - bearbeitet            bearbeitet- kleine Scheiben     8901    8920

                                       ESG - bearbeitet            bearbeitet - große Scheiben     8921    8950

                                       ESG - bearbeitet            bearbeitet - Serien             8951    8999

                                       ESG - gesäumt               gesäumt                         8001    8399

                                       ESG - gesäumt               gesäumt - große Scheiben        8421    8450

                                       ESG - gesäumt               gesäumt - Serien                8451    8499

                                       ESG - gesäumt               gesäumt - kleine Scheiben       8401    8420

                                       Einfachglas                 Serien                          7951    7999

                                       Einfachglas                 Einfach                         7501    7899

                                       Einfachglas                 große Scheiben                  7921    7950

                                       Einfachglas                 kleine Scheiben                 7901    7920

                                       Einfachglas - geschliffen   geschliffen - kleine Scheiben   7401    7420

                                       Einfachglas - geschliffen   geschliffen - große Scheiben    7421    7450

                                       Einfachglas - geschliffen   geschliffen - Serien            7451    7499

                                       Einfachglas - geschliffen   Einfach - geschliffen           7001    7399

                                       Iso                         Iso                             1001    1899

                                       Iso                         Iso - kleine Einheiten          1901    1920
3,00 / 01-2023




                                       Iso                         Iso - Serien                    1951    1999

                                       Tab. F-3      Nummernkreise der Produktionsorga A-Böcke



                 A+W Production Feinplanung                                                                    F-99
                    Orgas                                                                             Tutorial




                            Orgagruppe                   Abstellplatz                         Nummernkreis
                                                                                               von    bis

                            Iso                          Iso - große Einheiten               1921    1950

                            Iso - Dreifach               Iso - Dreifach                      6001    6899

                            Iso - Dreifach               Iso - Dreifach - kleine Einheiten   6901    6920

                            Iso - Dreifach               Iso - Dreifach - Serien             6951    6999

                            Iso - Dreifach               Iso - Dreifach - große Einheiten    6921    6950

                            Iso - Modelle                Iso - Modelle - Serien              2951    2999

                            Iso - Modelle                Iso - Modelle - kleine Einheiten    2901    2920

                            Iso - Modelle                Iso-Modelle                         2001    2899

                            Iso - Modelle                Iso - Modelle - große Einheiten     2921    2940

                            Iso - Modelle                Iso - Modelle - nicht versiegelt    2941    2950

                            Iso - Modelle - Sprossen     Iso-Modell-Sprossen-Serien          3951    3999

                            Iso - Modelle - Sprossen     Iso-Modell-Sprossen-klein           3901    3920

                            Iso - Modelle - Sprossen     Iso-Modell-Sprossen                 3001    3899

                            Iso - Modelle - Sprossen     Iso-Modell-Sprossen-gross           3921    3950

                            Iso - Sprossen               Iso - Sprossen - kleine Einheiten   4901    4920

                            Iso - Sprossen               Iso-Sprosse                         4001    4899

                            Iso - Sprossen               Iso - Sprossen - große Einheiten    4921    4950

                            Iso - Sprossen               Iso - Sprossen - Serien             4951    4999

                            Iso - Stufe                  Iso - Stufe - kleine Einheiten      5901    5920

                            Iso - Stufe                  Iso - Stufe                         5001    5899

                            Iso - Stufe                  Iso - Stufe - große Einheiten       5921    5950

                            Iso - Stufe                  Iso - Stufe - Serien                5951    5999

                            VSG                          VSG - Serien                        9951    9990

                            VSG                          VSG- große Scheiben                 9921    9950

                            VSG                          VSG                                 9001    9899

                            VSG                          VSG- kleine Scheiben                9901    9920

                            Tab. F-3         Nummernkreise der Produktionsorga A-Böcke

                            Die Orga A-Böcke optimiert stärker versandtorientiert. Sie müssen am Linien-
                            ausgang weniger nachsortieren und benötigen daher weniger Platz für Gestel-
01-2023 / 01-2023




                            le:




                    F-100                                                          A+W Production Feinplanung
                 Tutorial                                                                                  Orgas




                                       Einstellungen in A+W Production
                                       Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in
                                       A+W Production für ISO-Kleine Einheiten
                                       Einstellungen der Orga-Gruppe:




                                       Abb. F-41    Einstellungen der Orga-Gruppe


                                       Einstellungen Abstellplatz:
3,00 / 01-2023




                 A+W Production Feinplanung                                                                F-101
                    Orgas                                                                        Tutorial




                            Abb. F-42    Einstellungen Abstellplatz


                            Ergänzende Informationen
                             Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                             Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
01-2023 / 01-2023




                    F-102                                                     A+W Production Feinplanung
                 Tutorial                                                                                       Orgas




                                       A-Böcke Versand
                                       Die Orga A-Böcke Versand liefert eine versandorientierte Produktionsreihen-
                                       folge, bei der vor der Linie im Wechsel von mehreren A-Böcken abgegriffen
                                       wird.
                                       Die Einteilung der Abstellplatzgruppen basiert auf Größenklassen, innerhalb
                                       derer nach Kunde sortiert wird. Die Idee hierbei ist, eine Produktionsreihenfol-
                                       ge zu erreichen, die innerhalb gewisser Größenschwankungen global von
                                       groß nach klein läuft, wobei in jeder Größenklasse die Kundenaufträge zu-
                                       sammen gehalten und am Ende der Linie direkt auf Versandgestelle separiert
                                       werden.
                                       Die Orga benötigt Abstellplätze vor und hinter der Linie und liefert eine verpa-
                                       ckungsgerechte Produktionsreihenfolge. Hinter der Linie müssen Gestelle je
                                       Kunde bereitgestellt werden.
                                       •       Es werden ausschließlich A-Böcke verwendet (Tiefe 200, Breite 2000).
                                       •       Abstellmodus ist Glas.

                                       Größenklassen
                                       Um Scheiben in Größenklassen einzuteilen, arbeitet diese Orga mit 2
                                       Schwellwerten (im Diagramm S1 und S2).


                                           A




                                                                                B

                                       A kleine Kante                            B große Kante
                                       Abb. F-43        Größenklassen


                                       Da in der Orga immer zuerst die kleine Kante gesucht und geprüft wird, ist nur
                                       der Teil unterhalb der Diagonalen (im Diagramm) von Bedeutung. Die Grö-
                                       ßenklassen sind wie folgt definiert:
                                       •       Größenklasse 1: kleine Kante > Gr_Schwelle_2
                                       •       Größenklasse 2:
                                               – kleine Kante ≥ Gr_Schwelle_1 und
                                               – große Kante ≤ Gr_Schwelle_2
                                       •       Größenklasse 3:
                                               – kleine Kante ≥ Gr_Schwelle_1 und
3,00 / 01-2023




                                               – große Kante ≤ Gr_Schwelle_1
                                       •       Größenklasse 4:
                                               – kleine Kante < Gr_Schwelle_1 und


                 A+W Production Feinplanung                                                                     F-103
                    Orgas                                                                          Tutorial




                                – große Kante > Gr_Schwelle_2
                            •   Größenklasse 5:
                                – Kleine Kante < Gr_Schwelle_1 und
                                – große Kante ≥ Gr_Schwelle_1
                            •   Größenklasse 6:
                                – Kleine Kante < Gr_Schwelle_1 und
                                – große Kante < Gr_Schwelle_1

                            Produktionsreihenfolge
                            Nach dieser Größenrasterung werden Abstellplatzgruppen definiert und die
                            Produktionsreihenfolge nach dem Schema 1 ' 2 ' 3 ' 4 ' 5 ' 6 gebildet, also von
                            groß nach klein. Innerhalb dieser Größenklassen wie nachfolgend angege-
                            ben:
                            •   ISO Größenklasse 1
                                – Serie
                                – Normale ISO
                                – ISO-Besonderheiten (Stufe, Modell, 3-fach, Sprossen)
                            •   ISO Größenklasse 2
                                – Serie
                                – Normale ISO
                                – Stufen-ISO
                                – 3-fach-ISO
                                – ISO-Modellscheiben
                                – ISO-Scheiben mit Sprossen
                            •   ISO Größenklasse 3
                                – Wie Größenklasse 2
                            •   ISO Größenklasse 4
                                – Wie Größenklasse 2
                            •   ISO Größenklasse 5
                                – Wie Größenklasse 2
                            •   ISO Größenklasse 6
                                – Serie
                                – Normale ISO
                                – ISO-Besonderheiten (Stufe, Modell, 3-fach, Sprossen)
                            Bei den größten und kleinsten Scheiben werden also alle Besonderheiten zu-
                            sammengefasst.

                            Gruppierung und Sortierung
                            Die Gruppierung an der Abstellplatzgruppe (Größenklasse) ist:
                            Kunde + Artikel + SprossenKZ + Modell + Stufen
                            Ein gegebener Kunde ist i.A. im Wechsel von den Gestellen einer Größenklas-
01-2023 / 01-2023




                            se abzunehmen. Die (Produkt-) Artikelnummer sorgt dafür, dass gleiche Glas-
                            aufbauten zusammenhängend in der Produktionsreihenfolge bleiben (i.d.R.
                            gleicher Bock).



                    F-104                                                   A+W Production Feinplanung
                 Tutorial                                                                                     Orgas




                                       Ansonsten kommen Stufen vor Modellen, Modelle vor Sprossen. Serien ste-
                                       hen positionsweise separat, werden aber in Produktionsreihenfolge beige-
                                       mischt. Alle anderen A-Böcke enthalten mehrere Kunden und Aufträge
                                       hintereinander.

                                       Nummernkreise
                                       Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze ver-
                                       teilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinter-
                                       legt:

                                       Orgagruppe                  Abstellplatz                     Nummernkreis
                                                                                                     von    bis

                                       Auffänger                   Auffänger                       10000   10999

                                       ESG - bearbeitet            bearbeitet-- große Scheiben     8921    8950

                                       ESG - bearbeitet            bearbeitet- kleine Scheiben     8901    8920

                                       ESG - bearbeitet            bearbeitet                      8501    8899

                                       ESG - bearbeitet            bearbeitet - Serien             8951    8999

                                       ESG - gesäumt               gesäumt - große Scheiben        8421    8450

                                       ESG - gesäumt               gesäumt                         8001    8399

                                       ESG - gesäumt               gesäumt - kleine Scheiben       8401    8420

                                       ESG - gesäumt               gesäumt - Serien                8451    8499

                                       Einfachglas                 kleine Scheiben                 7901    7920

                                       Einfachglas                 große Scheiben                  7921    7950

                                       Einfachglas                 Einfach                         7501    7899

                                       Einfachglas                 Serien                          7951    7999

                                       Einfachglas - geschliffen   geschliffen - kleine Scheiben   7401    7420

                                       Einfachglas - geschliffen   Einfach - geschliffen           7001    7399

                                       Einfachglas - geschliffen   geschliffen - große Scheiben    7421    7450

                                       Einfachglas - geschliffen   geschliffen - Serien            7451    7499

                                       ISO Grkl 1                  ISO normal Grkl 1               1001    1499

                                       ISO Grkl 1                  ISO Besonderheiten Grkl 1       1801    1899

                                       ISO Grkl 1                  Iso - Serie - Grkl 1            1951    1999

                                       ISO Grkl 2                  Iso - Serie - Grkl 2            2951    2999

                                       ISO Grkl 2                  ISO normal Grkl 2               2001    2499

                                       ISO Grkl 2                  ISO Sprosse Grkl 2              2601    2699
3,00 / 01-2023




                                       ISO Grkl 2                  ISO Modell Grkl 2               2501    2599

                                       Tab. F-4      Nummernkreise der Produktionsorga A-Böcke Versand



                 A+W Production Feinplanung                                                                   F-105
                    Orgas                                                                       Tutorial




                            Orgagruppe               Abstellplatz                      Nummernkreis
                                                                                        von    bis

                            ISO Grkl 2               ISO 3-fach Grkl 2                2701    2799

                            ISO Grkl 2               ISO Stufe Grkl 2                 2801    2899

                            ISO Grkl 3               ISO normal Grkl 3                3001    3499

                            ISO Grkl 3               ISO Stufe Grkl 3                 3801    3899

                            ISO Grkl 3               ISO 3-fach Grkl 3                3701    3799

                            ISO Grkl 3               ISO Modell Grkl 3                3501    3599

                            ISO Grkl 3               Iso - Serie - Grkl 3             3951    3999

                            ISO Grkl 3               ISO Sprosse Grkl 3               3601    3699

                            ISO Grkl 4               ISO Sprosse Grkl 4               4601    4699

                            ISO Grkl 4               ISO normal Grkl 4                4001    4499

                            ISO Grkl 4               ISO Stufe Grkl 4                 4801    4899

                            ISO Grkl 4               ISO 3-fach Grkl 4                4701    4799

                            ISO Grkl 4               ISO Modell Grkl 4                4501    4599

                            ISO Grkl 4               Iso - Serie - Grkl 4             4951    4999

                            ISO Grkl 5               ISO normal Grkl 5                5001    5499

                            ISO Grkl 5               Iso - Serie - Grkl 5             5951    5999

                            ISO Grkl 5               ISO 3-fach Grkl 5                5701    5799

                            ISO Grkl 5               ISO Modell Grkl 5                5501    5599

                            ISO Grkl 5               ISO Sprosse Grkl 5               5601    5699

                            ISO Grkl 5               ISO Stufe Grkl 5                 5801    5899

                            ISO Grkl 6               Iso - Serie - Grkl 6             6951    6999

                            ISO Grkl 6               ISO normal Grkl 6                6001    6499

                            ISO Grkl 6               ISO Besonderheiten Grkl 6        6801    6899

                            VSG                      VSG                              9001    9899

                            VSG                      VSG - kleine Scheiben            9901    9920

                            VSG                      VSG - große Scheiben             9921    9950

                            VSG                      VSG - Serien                     9951    9990

                            Tab. F-4     Nummernkreise der Produktionsorga A-Böcke Versand

                            Die Orga A-Böcke Versand optimiert direkt ausgerichtet auf Verpacken und
01-2023 / 01-2023




                            Versand. Sie benötigen dadurch zwar mehr Gestelle am Linienende (pro Kun-
                            de / Auftrag) die Abstelllogik der Gläser ist aber einfacher.




                    F-106                                                    A+W Production Feinplanung
                 Tutorial                                                                                  Orgas




                                       Einstellungen in A+W Production
                                       Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in
                                       A+W Production für ISO-Serie-Größenklasse 1.
                                       Einstellungen der Orga-Gruppe:




                                       Abb. F-44    Einstellungen der Orga-Gruppe


                                       Einstellungen Abstellplatz:
3,00 / 01-2023




                 A+W Production Feinplanung                                                                F-107
                    Orgas                                                                        Tutorial




                            Abb. F-45    Einstellungen Abstellplatz


                            Ergänzende Informationen
                             Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                             Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                            Fächerwagen ohne Auffüllen
                            Die Orga Fächerwagen entspricht im Aufbau und der Abstellplatzvergabe
                            weitgehend der Orga A-Böcke, es werden aber Fächerwagen für die Haupt-
                            abstellplätze genommen.
                            Dadurch wird meist ein erheblich besserer Verschnitt gewährleistet. Große
                            und kleine Einheiten sowie Serien werden auf A-Böcke herausgezogen.
                            Ein wichtiger Unterschied zur Orga A-Böcke liegt darin, dass die Produktions-
                            reihenfolge stets versandgerecht ist. Zwar wird mit der Orga Fächerwagen
                            ebenfalls ein Bock nach dem anderen vor der Linie abgearbeitet, doch können
                            auf Fächerwagen alle benötigten Glasarten zusammengestellt und auf Ver-
                            sandreihenfolge gebracht werden.

                            Produktionsreihenfolge
                            Die verwendeten Abstellplatzgruppen sind (in Produktionsreihenfolge):
01-2023 / 01-2023




                            •   Normale ISO-Scheiben
                            •   ISO-Modellscheiben
                            •   ISO-Modellscheiben mit Sprossen
                            •   ISO-Scheiben mit Sprossen



                    F-108                                                     A+W Production Feinplanung
                 Tutorial                                                                                        Orgas




                                       •   Stufen-ISO
                                       •   3-fach ISO
                                       Um eine teilweise Direktverpackung zu ermöglichen, sind die Abstellplatz-
                                       gruppen jeweils von groß nach klein unterteilt (in Produktionsreihenfolge):
                                       •   Serien: A-Bock, (Serienflag gesetzt oder Stück ≥10)
                                       •   Große Einheiten: A-Bock, Bedingung große Einheit, Voreinstellung:
                                           – große Kante > 2100 oder
                                           – kleine Kante > 1600)
                                       •   Normale Einheiten: Fächerwagen
                                       •   Kleine Einheiten: A-Bock, Bedingung kleine Einheit, Voreinstellung:
                                           – kleine Kante < 300 oder
                                           – große Kante < 500)

                                       Gruppierung und Sortierung
                                       Die Fächerwagen haben 60 einzeln nummerierte Fächer. Die Sortierung auf
                                       den Fächerwagen ist Kunde+Auftrag+Position, während die A-Böcke nach
                                       Kunde+Auftrag gruppiert sind.
                                       Die zu einem Produktaufbau gehörigen Scheiben werden nebeneinander in
                                       die Fächerwagen gesetzt. Handzuschnitte und Zukaufsgläser müssen zusor-
                                       tiert werden.
                                       In jeder der Abstellplatzgruppen (in Produktionsreihenfolge) können am Ende
                                       schwach belegte Fächerwagen mit nur wenigen Scheiben auftreten. Bei-
                                       spielsweise ergibt sich in der Abstellplatzgruppe Modellsprossen ein Wagen
                                       mit nur zwei Einheiten, wenn der Produktionslauf nicht mehr an Modellspros-
                                       sen enthält. Dieser Effekt wird in der Orga Aufgefüllte Fächerwagen vermie-
                                       den.

                                       Optimierung
                                       Wenn in einem Optimierungslauf nur Scheiben für Fächerwagen enthalten
                                       sind, erfolgt die Optimierung als freie Optimierung (XOPT). Sobald A-Bock-
                                       Scheiben in der Optimierung enthalten sind, erfolgt die Optimierung als Se-
                                       quenz-Optimierung. Dabei werden aber die Scheiben auf Fächerwagen ohne
                                       jegliche Restriktion optimiert, das entspricht in der Wirkung einer freien Opti-
                                       mierung.

                                           Fächerwagen nicht aufgefüllt!
                                           Bei dieser Organisation ist wichtig, dass Fächerwagen nicht aufgefüllt wer-
                                           den.

                                           D. h. ein Fächerwagen wird nicht optimal ausgenutzt. Es kann passieren,
                                           dass einige Fächer frei bleiben, da die Positionen nicht gesplittet werden.
                                           Passt eine Auftragsposition nicht mehr in die restlichen Fächer des Fächer-
                                           wagens, wird eine neue Fächerwagennummer vergeben!

                                           Die Sortierung auf dem Fächerwagen wird vorab durch die Gruppierung
3,00 / 01-2023




                                           (bzw. Sortierung), welche an der Abstellplatzorganisation hängt, bestimmt.




                 A+W Production Feinplanung                                                                      F-109
                    Orgas                                                                              Tutorial




                            Nummernkreise
                            Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze ver-
                            teilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinter-
                            legt:

                            Orgagruppe                   Abstellplatz                         Nummernkreis
                                                                                               von    bis

                            Auffänger                    Auffänger                           10000   10999

                            ESG - bearbeitet             bearbeitet - große Scheiben         8921    8950

                            ESG - bearbeitet             bearbeitet - kleine Scheiben        8901    8920

                            ESG - bearbeitet             bearbeitet                          8500    8899

                            ESG - bearbeitet             bearbeitet - Serien                 8951    8999

                            ESG - gesäumt                gesäumt - Serien                    8451    8499

                            ESG - gesäumt                gesäumt - große Scheiben            8421    8450

                            ESG - gesäumt                gesäumt - kleine Scheiben           8401    8420

                            ESG - gesäumt                Gesäumt                             8000    8399

                            Einfachglas                  Serien                              7951    7999

                            Einfachglas                  kleine Scheiben                     7901    7920

                            Einfachglas                  Einfach                             7500    7899

                            Einfachglas                  große Scheiben                      7921    7950

                            Einfachglas - geschliffen    geschliffen - große Scheiben        7421    7450

                            Einfachglas - geschliffen    geschliffen - kleine Scheiben       7401    7420

                            Einfachglas - geschliffen    Einfach - geschliffen               7000    7399

                            Einfachglas - geschliffen    geschliffen - Serien                7451    7499

                            Iso                          Iso                                 100     1899

                            Iso                          Iso - kleine Einheiten              1901    1920

                            Iso                          Iso - große Einheiten               1921    1950

                            Iso                          Iso - Serien                        1951    1999

                            Iso - Dreifach               Iso - Dreifach                      6000    6899

                            Iso - Dreifach               Iso - Dreifach - große Einheiten    6921    6950

                            Iso - Dreifach               Iso - Dreifach - Serien             6951    6999

                            Iso - Dreifach               Iso - Dreifach - kleine Einheiten   6901    6920
01-2023 / 01-2023




                            Iso - Modelle                Iso - Modelle - kleine Einheiten    2901    2920

                            Iso - Modelle                Iso - Modelle                       2000    2899

                            Tab. F-5         Nummernkreise der Produktionsorga Fächerwagen ohne Auffüllen



                    F-110                                                          A+W Production Feinplanung
                 Tutorial                                                                                         Orgas




                                       Orgagruppe                  Abstellplatz                         Nummernkreis
                                                                                                         von    bis

                                       Iso - Modelle               Iso - Modelle - große Einheiten     2921   2940

                                       Iso - Modelle               Iso - Modelle - Serien              2951   2999

                                       Iso - Modelle               Iso - Modelle - nicht versiegelt    2941   2950

                                       Iso - Modelle - Sprossen    Iso - Modelle - Sprossen - groß     3921   3950

                                       Iso - Modelle - Sprossen    Iso - Modelle - Sprossen            3000   3899

                                       Iso - Modelle - Sprossen    Iso - Modelle - Sprossen - klein    3901   3920

                                       Iso - Modelle - Sprossen    Iso - Modelle - Sprossen - Serien   3951   3999

                                       Iso - Sprossen              Iso - Sprossen - Serien             4951   4999

                                       Iso - Sprossen              Iso - Sprossen - große Einheiten    4921   4950

                                       Iso - Sprossen              Iso - Sprossen - kleine Einheiten   4901   4920

                                       Iso - Sprossen              Iso - Sprosse                       4000   4899

                                       Iso - Stufe                 Iso - Stufe - kleine Einheiten      5901   5920

                                       Iso - Stufe                 Iso - Stufe - große Einheiten       5921   5950

                                       Iso - Stufe                 Iso - Stufe - Serien                5951   5999

                                       Iso - Stufe                 Iso - Stufe                         5000   5899

                                       VSG                         VSG - Serien                        9951   9990

                                       VSG                         VSG - große Scheiben                9921   9950

                                       VSG                         VSG - kleine Scheiben               9901   9920

                                       VSG                         VSG                                 9000   9899

                                       Tab. F-5        Nummernkreise der Produktionsorga Fächerwagen ohne Auffüllen

                                       Die Orga Fächerwagen optimiert versandorientiert und entspricht im Aufbau
                                       und der Abstellplatzvergabe weitgehend der Orga A-Böcke, es werden aber
                                       Fächerwagen für die Hauptabstellplätze verwendet.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                       F-111
                    Orgas                                                                      Tutorial




                            Einstellungen in A+W Production
                            Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in
                            A+W Production für ISO Modelle.
                            Einstellungen der Orga-Gruppe:




                            Abb. F-46    Einstellungen der Orga-Gruppe


                            Einstellungen Abstellplatz:
01-2023 / 01-2023




                            Abb. F-47    Einstellungen Abstellplatz




                    F-112                                                A+W Production Feinplanung
                 Tutorial                                                                                   Orgas




                                       Ergänzende Informationen
                                        Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135

                                       Aufgefüllte Fächerwagen
                                       Die Orga Aufgefüllte Fächerwagen vermeidet schwach gefüllte Fächerwagen
                                       und zieht alle Fächerwagen in Produktionsreihenfolge zusammen. Zuerst wer-
                                       den alle Fächerwagen abgearbeitet, anschließend kommen die Spezialitäten
                                       auf A-Böcke.

                                       Produktionsreihenfolge
                                       Die Abstellplatzgruppen in Produktionsreihenfolge sind:

                                       • Normale ISO (nach Produkttyp sortiert)       Fächerwagen

                                       • ISO groß, klein, Serie                       A-Böcke

                                       • ISO Modelle groß, klein, Serie               A-Böcke

                                       • ISO Modellsprossen groß, klein, Serie        A-Böcke

                                       • ISO Sprossen groß, klein, Serie              A-Böcke

                                       • ISO Stufen groß, klein, Serie                A-Böcke

                                       • ISO 3-fach groß, klein, Serie                A-Böcke

                                       Tab. F-6      Produktionsreihenfolge

                                       Bis auf frei gehaltene Fächer zum Zusortieren von Zukaufsgläsern und Hand-
                                       zuschnitten, werden die Fächerwägen lückenlos gefüllt und enthalten alle
                                       Scheiben normaler Größe - also auch Sprossen, Modelle usw.
                                       Große und kleine Einheiten sowie Serien sind herausgezogen und werden am
                                       Ende produziert.

                                       Gruppierung und Sortierung
                                       Serien stehen positionsweise getrennt. Alle anderen A-Böcke enthalten eine
                                       Gruppierung nach Kunde+Auftrag, mit mehreren Aufträgen je Bock, und sind
                                       in der Positionsreihenfolge frei.
                                       Die Orga enthält eine interne Gruppierung nach Produkteigenschaften. Die
                                       Belegungsreihenfolge der Fächerwagen und somit die Produktionsreihenfol-
                                       ge kann aber durch Vorgabe einer globalen Gruppierung und Sortierung über-
                                       steuert werden.
                                       •   Gruppierung = Keine
                                       •   Sortierung = Keine
                                       Mit dieser globalen Einstellung erfolgt die Belegung der Fächerwagen grup-
                                       piert nach folgenden Produkteigenschaften:
3,00 / 01-2023




                                       Modelle, Modellsprossen, Sprossen, Stufen, 3-fach Aufbauten und normale
                                       ISO.
                                       Diese werden jeweils zusammenhängend abgestellt und produziert.


                 A+W Production Feinplanung                                                                 F-113
                    Orgas                                                                             Tutorial




                            Mit der folgenden Einstellung werden Kundenaufträge - unabhängig von Pro-
                            dukteigenschaften - zusammen gehalten:
                            •   Gruppierung = Kunde+Auftrag
                            •   Sortierung = Keine
                            Dabei wechseln Modelle, Sprossen, 3-fach entsprechend des Auftragsmixes
                            ab; innerhalb eines Auftrags ist nach Produkteigenschaften gruppiert.
                            Die Fächerwagen haben 60 einzeln nummerierte Fächer.
                            Abstellmodus ist Einheit - die zu einem Produktaufbau gehörigen Scheiben
                            werden nebeneinander in die Fächerwagen gestellt. Handzuschnitte und Zu-
                            kaufsgläser müssen zusortiert werden.

                            Optimierung
                            Diese Organisation basiert i.A. auch auf Sequenz - siehe Organisation Fä-
                            cherwagen ohne Auffüllen - jedoch wird hier aufgefüllt, d. h. die Fächerwagen
                            werden komplett gefüllt, auch wenn eine Auftragsposition gesplittet wird.

                            Nummernkreise
                            Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze ver-
                            teilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinter-
                            legt:

                            Orgagruppe                  Abstellplatz                       Nummernkreis
                                                                                           von    bis

                            Auffänger                   Auffänger                          10000   10999

                            ESG - bearbeitet            bearbeitet - Serien                8951    8999

                            ESG - bearbeitet            bearbeitet - große Scheiben        8921    8950

                            ESG - bearbeitet            bearbeitet - kleine Scheiben       8901    8920

                            ESG - bearbeitet            bearbeitet                         8500    8899

                            ESG - gesäumt               gesäumt - große Scheiben           8421    8450

                            ESG - gesäumt               gesäumt - kleine Scheiben          8401    8420

                            ESG - gesäumt               gesäumt                            8000    8399

                            ESG - gesäumt               gesäumt - Serien                   8451    8499

                            Einfachglas                 Einfach                            7500    7899

                            Einfachglas                 Serien                             7951    7999

                            Einfachglas                 große Scheiben                     7921    7950

                            Einfachglas                 kleine Scheiben                    7901    7920
01-2023 / 01-2023




                            Einfachglas - geschliffen   geschliffen - Serien               7451    7499

                            Einfachglas - geschliffen   geschliffen - große Scheiben       7421    7450

                            Tab. F-7      Nummernkreise der Produktionsorga Aufgefüllte Fächerwagen



                    F-114                                                      A+W Production Feinplanung
                 Tutorial                                                                                           Orgas




                                       Orgagruppe                    Abstellplatz                        Nummernkreis
                                                                                                         von    bis

                                       Einfachglas - geschliffen    geschliffen - kleine Scheiben        7401    7420

                                       Einfachglas - geschliffen    Einfach - geschliffen                7000    7399

                                       Fächerwage aufgefüllt        Fächerwagen alles                    11000   50999

                                       Iso                           Iso - kleine Einheiten              1901    1920

                                       Iso                           Iso - Serien                        1951    1999

                                       Iso                           Iso - große Einheiten               1921    1950

                                       Iso - Dreifach                Iso - Dreifach - kleine Einheiten   6901    6920

                                       Iso - Dreifach                Iso - Dreifach - große Einheit      6921    6950

                                       Iso - Dreifach                Iso - Dreifach - Serien             6951    6999

                                       Iso - Modelle                 Iso - Modelle - große Einheiten     2921    2940

                                       Iso - Modelle                 Iso - Modelle - kleine Einheiten    2901    2920

                                       Iso - Modelle                 Iso - Modelle - Serien              2951    2999

                                       Iso - Modelle                 Iso - Modelle - nicht versiege      2941    2950

                                       Iso - Modelle - Sprossen      Iso - Modelle - Sprossen - groß     3921    3950

                                       Iso - Modelle - Sprossen      Iso - Modelle - Sprossen - Serien   3951    3999

                                       Iso - Modelle - Sprossen      Iso - Modelle - Sprossen - klein    3901    3920

                                       Iso - Sprossen               Iso - Sprossen - kleine Einheiten    4901    4920

                                       Iso - Sprossen                Iso - Sprossen - Serien             4951    4999

                                       Iso - Sprossen               Iso - Sprossen - große Einheiten     4921    4950

                                       Iso - Stufe                   Iso - Stufe - Serien                5951    5999

                                       Iso - Stufe                   Iso - Stufe - kleine Einheiten      5901    5920

                                       Iso - Stufe                   Iso - Stufe - große Einheiten       5921    5950

                                       VSG                           VSG - große Scheiben                9921    9950

                                       VSG                           VSG - Serien                        9951    9990

                                       VSG                           VSG                                 9000    9899

                                       VSG                           VSG- kleine Scheiben                9901    9920

                                       Tab. F-7         Nummernkreise der Produktionsorga Aufgefüllte Fächerwagen

                                       Die Orga Aufgefüllte Fächerwagen optimiert die Gläser produktionsorientiert
                                       nach Produkteigenschaften auf Fächerwagen und A-Böcke. Sie benötigen
                                       zwar mehr Gestelle, haben aber eine bessere Versandausrichtung der Pro-
                                       duktion, da die Gläser nach Kunde und Auftragsnummer gruppiert werden.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                         F-115
                    Orgas                                                                      Tutorial




                            Einstellungen in A+W Production
                            Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in
                            A+W Production für ISO Dreifach Große Einheiten.
                            Einstellungen der Orga-Gruppe:




                            Abb. F-48    Einstellungen der Orga-Gruppe


                            Einstellungen Abstellplatz:
01-2023 / 01-2023




                    F-116                                                A+W Production Feinplanung
                 Tutorial                                                                                 Orgas




                                       Abb. F-49    Einstellungen Abstellplatz


                                       Ergänzende Informationen
                                        Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                                        Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
3,00 / 01-2023




                 A+W Production Feinplanung                                                               F-117
                    Orgas                                                                        Tutorial




                            Demos und Übungen
                            In diesem Abschnitt erfahren Sie, wie Sie eine Orga in der A+W Production
                            anlegen.

                            Trainerdemo: Stammdaten erläutern
                            Es werden die Stammdaten der A+W Production gezeigt und erläutert.
                            Folgender Dialog wird unter diesem Aspekt erklärt:
                            •   Dialog Orga, mit den Registern
                                – Master-Orga
                                – Produktionsreihenfolge
                                – Prüfreihenfolge

                            Übung 1: Eine Master-Orga anlegen
                            Erstellen Sie eine Master-Orga gemäß den unten aufgeführten Spezifikatio-
                            nen.

                            Aufgabenstellung
                            Erfassen Sie einen Testauftrag und lasten Sie diesen gemeinsam mit dem
                            Trainer ein, um die Auswirkungen zu sehen. Der Testauftrag hat folgende
                            Rahmenbedingungen zu erfüllen:
                            •   Name der Orga: Neue Trainings-Orga.
                            •   Fertigungsgruppen: Nach Kundennummer+Auftragsnummer
                            •   Name der Orga-Form: Neue Training
                            •   Typ der Orga-Form. Standard
                            •   Abstellmodus: Einheit
                            •   Name der Orga-Gruppe: Auffang-Abstellplatz
                            •   Einstellungen Abstellplatz: A-Bock, Supergruppenbildung: +Kundennum-
                                mer+Auftragsnummer, keine Sortierung in den Gruppen, vollständige
                                Gruppen werden gemeinsam abgestellt, Optimierungsverhalten 5.1, Ab-
                                stellmodus Einheit.

                            Übung 1: Lösung
                            Die einzelnen Schritte dieser Aufgabe werden in folgenden Dialogen vorge-
                            nommen:
                            •   Dialog Orga
                            •   Dialog Master-Orga
                            •   Dialog Einstellungen - Abstellplatz


                             Master-Orga anlegen
                            1 Öffnen Sie den Dialog Orga über das Menü Stammdaten > Feinplanung.
01-2023 / 01-2023




                            2 Betätigen Sie die Schaltfläche [Neu]. Es öffnet sich der Dialog Master-Or-
                              ga.
                            3 Geben Sie im Feld Name der Master-Orga Neue Trainings-Orga ein.


                    F-118                                                 A+W Production Feinplanung
                 Tutorial                                                                                      Orgas




                                       4 Öffnen Sie die Kombobox Fertigungsgruppen und wählen Sie +Kunden-
                                         nummer-Auftragsnummer aus.
                                       5 Betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen und Sie
                                         befinden sich wieder im Dialog Orga.
                                       6 Die neue Orga steht jetzt in der Übersicht.


                                        Produktionsreihenfolge anlegen
                                       1 Öffnen Sie das Register Produktionsreihenfolge.
                                       2 Betätigen Sie die Schaltfläche [Neu]. Es wird der Eintrag unknon/Standard
                                         hinzugefügt.
                                       3 Betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog Or-
                                         ga.
                                       4 Geben Sie im Feld Name der Orga-Form Neues Training ein.
                                       5 Im Bereich Abstellmodus aktivieren Sie Einheit.
                                       6 Betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen und Sie
                                         befinden sich wieder im Register Produktionsreihenfolge.


                                        Orga-Gruppe anlegen
                                       1 Markieren Sie die soeben angelegte Orga-Form Neues Training und betä-
                                         tigen Sie die Schaltfläche [Neu]. Es wird der Eintrag noname hinzugefügt.
                                       2 Betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog
                                         Orga-Gruppen.
                                       3 Geben Sie im Feld Name Auffang Abstellplatz ein.
                                       4 Im Bereich Bildung der Gruppen wählen Sie Kundennummer.
                                       5 Aktivieren Sie die Checkbox Sortierung der Gruppen.
                                       6 Betätigen Sie die Schaltfläche [OK]. Der Dialog wird geschlossen und Sie
                                         befinden sich wieder im Register Produktionsreihenfolge.


                                        Abstellplatz anlegen
                                       1 Markieren Sie die soeben angelegte Orga-Gruppe Auffang Abstellplatz
                                         und betätigen Sie die Schaltfläche [Neu]. Es wird der Eintrag unknown hin-
                                         zugefügt.
                                       2 Betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog
                                         Einstellungen-Abstellplatz.
                                       3 Geben Sie im Feld Name A-Bock ein.
                                       4 Im Bereich Bildung der Gruppen wählen Sie +Kundennummer+Auftrags-
                                         nummer.
                                       5 Aus der Kombobox Sortierung in den Gruppen wählen Sie Keine.
3,00 / 01-2023




                                       6 Im Bereich Abstellmodus Gruppen wählen Sie vollständige Gruppen ge-
                                         meinsam und im Bereich Optimierungsverhalten 5.1.
                                       7 Aktivieren Sie die Checkbox Auffang-Abstellplatz.


                 A+W Production Feinplanung                                                                    F-119
                    Orgas                                                                        Tutorial




                            Ergänzende Informationen
                             Softwarereferenz, “Orga” auf Seite F-131
                             Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                             Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
                            
01-2023 / 01-2023




                    F-120                                                     A+W Production Feinplanung
Feinplanung                  F

                Softwarereferenz




              A+W Production
                 Softwarereferenz                                                                              Übersicht




                                       Übersicht
                                       Menü Stammdaten > Feinplanung öffnen
                                       Im Menü Feinplanung befinden sich folgende Programmpunkte:
                                       •   Voreinstellungen:
                                           Diesen Menüpunkt benötigen Sie, wenn keine Einstellungen für Orga,
                                           Gruppierung und Sortierung in der Orga sowie Sortierung auf dem Abstell-
                                           platz vorgenommen wurden.
                                            “Voreinstellungen” auf Seite F-139
                                       •   Orga:
                                           Über diesen Menüpunkt richten Sie die Orgas ein. Sie definieren die Pro-
                                           duktionsreihenfolge sowie die Prüfreihenfolge.
                                            Softwarereferenz, “Register Master-Orga” auf Seite F-120
                                            Softwarereferenz, “Register Produktionsreihenfolge” auf Seite F-122
                                            Softwarereferenz, “Register Prüfreihenfolge” auf Seite F-124
                                       •   Gruppierung:
                                           Über diesen Menüpunkt richten Sie Gruppierungen und Sortierungen ein.
                                            Softwarereferenz, “Gruppierung/Sortierung - Dialog” auf Seite F-140
                                       •   Abstellplätze:
                                           Mit diesem Menüpunkt richten Sie die Abstellplätze ein.
                                            Softwarereferenz, “Abstellplätze” auf Seite F-146
                                       •   Bearbeitungen:
                                           Mit diesem Menüpunkt können Sie neue Bearbeitungen anlegen oder exis-
                                           tierende Bearbeitungen ändern.
                                       •   Lostypen
                                           Über diesen Menüpunkt legen Sie Lostypen an und weisen Bearbeitungen
                                           zu.
                                            Softwarereferenz, “Lostypen und Bearbeitungen” auf Seite F-151

                                           Dialoge können von unterschiedlichen Stellen aus geöffnet werden
                                           Bitte beachten Sie, dass Funktionen und Dialoge auf verschiedenen We-
                                           gen geöffnet werden können. In dieser Anleitung werden die entsprechen-
                                           den Dialoge nur einmal beschrieben.

                                       Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden
                                       Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative
                                       Wege einen Dialog aufzurufen, so sind diese ebenfalls angegeben.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                        F-119
                 Organisationen                                                                Softwarereferenz




                                  Organisationen
                                  Stammdaten > Feinplanung > Orga
                                  In diesem Bereich erfassen bzw. ändern Sie Master-Orgas, Orgas und Orga-
                                  Gruppen. Darüber hinaus nehmen Einstellungen an der Produktionsreihenfol-
                                  ge sowie der Prüfreihenfolge vor. Detaillierte Informationen entnehmen Sie
                                  den Erläuterungen der einzelnen Register.
                                  Der Dialog ist in folgende Register unterteilt:
                                  •   “Register Master-Orga” auf Seite F-120
                                  •   “Register Produktionsreihenfolge” auf Seite F-122
                                  •   “Register Prüfreihenfolge” auf Seite F-124
                                  •   “Voreinstellungen” auf Seite F-139


                                  Register Master-Orga
                                  Stammdaten > Feinplanung > Orga




                                  Abb. F-46    Orga-Dialog, Register Master-Orga


                                  Im Register Master-Orga legen Sie neue Master-Orgas an oder nehmen Än-
                                  derungen an bestehenden Master-Orgas vor. Die erstellten Master-Orgas wei-
                                  sen Sie dann später bei der Feinplanung einem Lauf zu. Im linken Fenster
                                  werden alle bereits definierten Master-Orgas in Baumstruktur dargestellt. Mit
                                  einem Klick auf das Pluszeichen, öffnen Sie die Master-Orga und sehen, wel-
                                  che Orga der Master-Orga zugeordnet ist. Im rechten Fenster sehen Sie alle
                                  definierten Orgas.
3,00 / 01-2023




                 F-120                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                    Organisationen




                                       Die in dem rechten Fenster angezeigten Symbole haben folgende Bedeutung:

                                              Standardorga / Verwendung
                                              Standardorga / Produktion
                                              Nicht-Standardorga / Produktion
                                              Nicht-Standardorga / Verwendung
                                       Abb. F-47    Erläuterung der Symbole für Orgas


                                       Erläuterung der Schaltflächen

                                       Neu Betätigen Sie diese Schaltflfäche, öffnet sich der Dialog Master-Orga, in
                                       dem Sie eine neue Master-Orga anlegen können. Zum Anlegen einer neuen
                                       Master-Orga, müssen Sie im linken Fenster den in der Baumstruktur an erster
                                       Stelle stehenden Eintrag Master-Orga markiert haben.

                                       Löschen Betätigen Sie diese Schaltfläche, wird die im linken Fenster mar-
                                       kierte Master-Orga gelöscht. Haben Sie eine Orga markiert, wird die Orga ge-
                                       löscht.

                                          Löschen ohne Sicherheitsabfrage
                                          Sollten Sie versehentlich etwas gelöscht haben, verlassen Sie den Orga-
                                          Dialog über die Schaltfläche [Abbrechen]. Wenn Sie ihn das nächste Mal
                                          öffnen, sind die Daten wieder vorhanden.

                                       Einstellungen Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Mas-
                                       ter-Orga für die im linken Fenster ausgewählte Master-Orga.


                                       Weitere Informationen zum Register Master-Orga
                                        Tutorial, “Master-Orga” auf Seite F-71
                                        Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 A+W Production Feinplanung                                                                  F-121
                 Organisationen                                                                Softwarereferenz




                                  Register Produktionsreihenfolge
                                  Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge




                                  Abb. F-48    Register Produktionsreihenfolge


                                  Das Register Produktionsreihenfolge zeigt Ihnen die Reihenfolge der Orga-
                                  Gruppen in der Orga.

                                  Erläuterung der Schaltflächen

                                  Bedingung Diese Schaltfläche ist nur für Orga-Gruppen und Abstellplätze
                                  aktiv, da Sie nur für diese beiden Bedingungen definieren können. Betätigen
                                  Sie diese Schaltfläche, wenn Sie eine Orga-Gruppe markiert haben, öffnet
                                  sich der Dialog Auswahl Bedingungen. Sie definieren an dieser Stelle eine Be-
                                  dingung für die Orga-Gruppe. Betätigen Sie diese Schaltflfäche, wenn Sie ei-
                                  nen Abstellplatz markiert haben, öffnet sich ebenfalls der Dialog Auswahl
                                  Bedingungen. Sie definieren an dieser Stelle eine Bedingung für den Abstell-
                                  platz. Die Bedingung für einen Abstellplatz wird optisch durch ein ? angezeigt.

                                  Neu Betätigen Sie diese Schaltfläche, können Sie entweder eine neue Orga,
                                  eine neue Orga-Gruppe oder einen neuen Abstellplatz anlegen. Das hängt da-
                                  von ab, welchen Eintrag Sie markiert haben. Haben Sie Orga markiert und be-
                                  tätigen Sie die Schaltfläche [Neu], wird unterhalb der letzten Orga-Form eine
                                  neue Orga (z.B. MZO ISO groß) angehängt. Diese neue Orga erscheint zu-
                                  nächst mit dem Namen unknown. Markieren Sie dann diese neue angelegte
                                  Orga und betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Di-
                                  alog Orga, in dem Sie dann die entsprechenden Einstellungen zur Orga vor-
                                  nehmen können.
3,00 / 01-2023




                                  Haben Sie eine Orga markiert und betätigen Sie die Schaltfläche [Neu], wird
                                  innerhalb der markierten Orga an letzter Stelle eine neue Orga-Gruppe ange-
                                  hängt. Diese neue Orga-Gruppe erscheint zunächst mit dem Namen noname.



                 F-122                                                            A+W Production Feinplanung
                 Softwarereferenz                                                                     Organisationen




                                       Markieren Sie dann diese neue angelegte Orga-Gruppe und betätigen Sie die
                                       Schaltfläche [Einstellungen]. Es öffnet sich der Dialog Orga-Gruppe, in dem
                                       Sie dann die entsprechenden Einstellungen zur Orga-Gruppe vornehmen
                                       können.
                                       Haben Sie eine Orga-Gruppe markiert und betätigen Sie die Schaltfläche
                                       [Neu], wird innerhalb der markierten Orga-Gruppe an letzter Stelle eine neuer
                                       Abstellplatz angehängt. Dieser neue Abstellplatz erscheint zunächst mit dem
                                       Namen unknown. Markieren Sie dann diesen neu angelegten Abstellplatz und
                                       betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog Ein-
                                       stellungen - Abstellplatz, in dem Sie dann die entsprechenden Einstellungen
                                       zu dem Abstellplatz vornehmen können.

                                       Ausschneiden Betätigen Sie diese Schaltfläche, wird der markierte Daten-
                                       satz ausgeschnitten und in die Zwischenablage gelegt. Sie können ihn dann
                                       einer anderen Orga über die Schaltfläche [Einfügen] zufügen. Sollten Sie ver-
                                       sehentlich einen falschen Datensatz ausgeschnitten haben, erfolgt beim Ver-
                                       lassen des Dialoges noch einmal eine Sicherheitsabfrage, ob die Änderungen
                                       ignoriert werden sollen. Beantworten Sie diese Abfrage mit [Ja], ist der ausge-
                                       schnittene Datensatz beim nächsten Öffnen wieder vorhanden.

                                       Kopieren Betätigen Sie diese Schaltfläche, wird der markierte Datensatz in
                                       die Zwischenablage kopiert. Sie können ihn dann einer anderen Orga über die
                                       Schaltfläche [Einfügen] zufügen.

                                       Einfügen Betätigen Sie diese Schaltfläche, wird der kopierte oder ausge-
                                       schnittene Datensatz aus der Zwischenablage eingefügt.

                                       Löschen Betätigen Sie diese Schaltfläche, wird der markierte Datensatz ge-
                                       löscht. Sollte der Datensatz, den Sie löschen möchten, noch von einem A+W
                                       Production-Prozess verwendet werden, erscheint eine entsprechende Sicher-
                                       heitsabfrage. Sollten Sie versehentlich einen falschen Datensatz gelöscht ha-
                                       ben, erfolgt beim Verlassen des Dialoges noch einmal eine
                                       Sicherheitsabfrage, ob die Änderungen ignoriert werden sollen. Beantworten
                                       Sie diese Abfrage mit [Ja], ist der gelöschte Datensatz beim nächsten Öffnen
                                       wieder vorhanden.

                                       Einstellungen Betätigen Sie diese Schaltfläche, öffnet sich in Abhängigkeit
                                       des Eintrags, den Sie markiert haben, der entsprechende Dialog.
                                       • Softwarereferenz, “Orga” auf Seite F-131
                                       • Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                                       • Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
                                       • Formeleditor, “Auswahl Bedingungen” auf Seite F-44
                                       • Formeleditor: Softwarereferenz, “Auswahl Bedingungen” auf Seite F-44

                                       Export Orga Betätigen Sie diese Schaltfläche, wird die markierte Orga ex-
                                       portiert.


                                       Weitere Informationen zur Produktionsreihenfolge
3,00 / 01-2023




                                        Tutorial, “Produktionsreihenfolge” auf Seite F-81
                                        Überblick, “Schaltflächen” auf Seite A-78




                 A+W Production Feinplanung                                                                    F-123
                 Organisationen                                                                   Softwarereferenz




                                  Register Prüfreihenfolge
                                  Stammdaten > Feinplanung > Orga > Register Prüfreihenfolge




                                  Abb. F-49    Orga Dialog, Register Prüfreihenfolge


                                  Dieser Dialog zeigt Ihnen die Prüfreihenfolge aller Abstellplätze einer Orga.
                                  Das bedeutet, hier wird festgelegt, in welcher Reihenfolge geprüft wird, ob
                                  eine Scheibe einem entsprechenden Abstellplatz zugewiesen wird (hinter den
                                  Namen der Abstellplätze stehen implizit die von Ihnen entsprechend zugewie-
                                  senen Bedingungen. Somit definieren Sie implizit die Reihenfolge, in der die
                                  Bedingungen abgefragt werden. Innerhalb eines Abstellplatzes sind alle zuge-
                                  wiesenen Bedingungen - maximal 7 pro Abstellplatz - UND-verknüpft).
                                  Im rechten Fenster werden die Abstellplätze der im linken Fenster markierten
                                  Orga angezeigt. Ein * vor dem Namen kennzeichnet den Auffang-Abstellplatz
                                  der Orga (dieser sollte immer am Ende dieser Liste stehen). Um aus einem
                                  Abstellplatz einen Auffang-Abstellplatz zu machen, markieren Sie den ge-
                                  wünschten Abstellplatz durch einen Doppelklick. Bitte denken Sie daran, dass
                                  es für eine Orga immer nur einen Auffang-Abstellplatz geben kann. D.h. wenn
                                  es für eine Orga bereits einen Auffang-Abstellplatz gibt und Sie markieren ei-
                                  nen anderen Abstellplatz durch einen Doppelklick, wird der zuerst vorhandene
                                  Abstellplatz wieder als normaler Abstellplatz (ohne *) gekennzeichnet.
                                  Die Abstellplätze zeigen von oben nach unten die Reihenfolge an, nach der
                                  die Scheiben bestimmten Abstellplätzen zugewiesen werden. Eine Scheibe
                                  durchläuft, entsprechend der eingestellten Prüfreihenfolge, solange die Ab-
                                  stellplätze, bis sie auf einen Abstellplatz treffen, dessen Bedingungen sie er-
                                  füllt. Diesem wird sie dann zugewiesen. Die Spalten Von und Bis
                                  kennzeichnen den Nummernkreis der Abstellplätze. Sie können durch einen
3,00 / 01-2023




                                  Klick in die entsprechende Spalte den Nummernkreis direkt in diesem Dialog
                                  editieren.




                 F-124                                                                 A+W Production Feinplanung
                 Softwarereferenz                                                                   Organisationen




                                       Erläuterung der Schaltflächen

                                       Anfang Betätigen Sie diese Schaltfläche, verschiebt sich die markierte
                                       Scheibe an den Anfang, d.h. an die erste Stelle.

                                       Hoch Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Scheibe
                                       um eine Position nach oben.

                                       Runter Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Schei-
                                       be um eine Position nach unten.

                                       Ende Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Scheibe
                                       an das Ende, d.h. an die letzte Stelle.


                                       Weitere Informationen zur Prüfreihenfolge
                                        Tutorial, “Prüfreihenfolge” auf Seite F-76
                                        Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 A+W Production Feinplanung                                                                  F-125
                 Organisationen                                                                Softwarereferenz




                                  Master-Orga
                                  Stammdaten > Feinplanung > Orga > Register Master-Orga > [Neu]
                                  Stammdaten > Feinplanung > Orga > Register Master-Orga > Master-Orga
                                  markieren > [Einstellungen]




                                  Abb. F-50    Master-Orga erfassen


                                  Im Dialog Master-Orga können Sie entweder eine neue Master-Orga anlegen
                                  oder Einstellungen zu einer bestehenden Master-Orga ändern. Das Anlegen
                                  der Master-Orga gliedert sich in zwei Teile. Im ersten Schritt erfassen Sie die
                                  Master-Orga mit den entsprechenden Einstellungen und im zweiten Schritt le-
                                  gen Sie fest, aus welchen Orgas die Master-Orga bestehen soll. Weitere Er-
                                  läuterungen finden Sie in den entsprechenden Feldern.
                                  Technische Info: Datenbanktabelle: FEIN_MASTERORGA

                                  Erläuterung der Felder

                                  Name der Master-Orga In diesem Feld geben Sie den Namen für die Mas-
                                  ter-Orga ein. Der Name der Master-Orga wird in allen Anzeigen, die mit der
                                  Orga zu tun haben, verwendet und angezeigt.
                                  Technische Info: Pflichtfeld, Alphanumerisch, 32stellig, Datenbankfeld: NAME

                                  XOPT zusammen abstellen In der Feinplanung können aus den Opti-
                                  mierungen bestimmte Scheiben herausgeholt und mittels XOPT optimiert wer-
                                  den.
                                   XOPT - Optimierungen werden trotz verschiedener Glasart/-dicke gemein-
                                  sam in einem Stapel auf einem A-Bock abgestellt.
                                   Freie Optimierungen werden auf A-Böcken getrennt abgestellt.
3,00 / 01-2023




                                  Technische Info: Datenbankfeld: TOGETHER

                                  Kombobox Die Checkbox steuert, um welchen Typ es sich bei der Master-
                                  Orga handelt:


                 F-126                                                            A+W Production Feinplanung
                 Softwarereferenz                                                                   Organisationen




                                       •  Standard: Es wird die normale Master-Orga verwendet.
                                       •  Schnellorga: Es wird eine Schnell-Orga durchlaufen, ohne dass die Anzei-
                                          gen der Feinplanung erscheinen. Für Läufe, in denen Zuschnitt enthalten
                                          ist und die eine als Schnell-Orga gekennzeichnete Master-Orga durchlau-
                                          fen, wird der Zuschnitt stets als Handzuschnitt behandelt.
                                       • Phys. Gestellbelegung: Das System erzeugt automatisch eine sinnvolle
                                          Belegung der physikalischen Gestelle unter Beachtung der dafür angeleg-
                                          ten Regeln und Zwangsbedingungen (Gewicht, Größe, etc.). Hierzu wird
                                          im Rahmen der Feinplanung zusätzlich der Stack Optimizer gestartet.
                                       Technische Info: Datenbankfeld: QUICKORGA

                                       Pärchenbildung verboten Diese Checkbox kommt bei 3-fach Isolierglas
                                       zum Einsatz. Die Einheiten bestehen meist aus einer unbeschichteten und
                                       zwei beschichteten Scheiben, wobei die beschichteten Scheiben die 1. und 3.
                                       Scheibe sind. Die Schichten werden zum SZR eingebaut, so dass eine der
                                       beiden Scheiben vor der Linie gedreht werden müsste. Um diese Scheibe be-
                                       reits im Zuschnitt gedreht auf den Bock zu stellen, soll die Feinplanung die
                                       Scheiben daher auf verschiedene Stapel abstellen.
                                       Damit die beiden Stapel identische, passende Reihenfolgen haben, muss in
                                       diesem Nummernkreis mit fester Reihenfolge optimiert werden.
                                        Die Bildung von Pärchen ist verboten.
                                        Die Bildung von Pärchen ist erlaubt.
                                       Technische Info: Datenbankfeld: PAIRFORBIDDEN

                                       Maximale Anzahl Abstellplätze in Optimierung In diesem Feld können Sie
                                       angeben, wie viele Stapel gleichzeitig von der Optimierung verwendet werden
                                       dürfen.

                                       Fertigungsgruppen Die Kombobox enthält alle in dem Register Gruppierun-
                                       gen des Dialogs Gruppierung/Sortierung angelegten Werte. Wenn Sie von
                                       den vorhandenen Gruppierungen in diesem Feld eine auswählen, werden in-
                                       nerhalb der Feinplanung Fertigungsgruppen entsprechend des ausgewählten
                                       Wertes gebildet (als Vorbelegung - das kann man später an den Einstellungen
                                       der Orga ändern und auch in der Feinplanung (Optimierung) selbst). Die aus-
                                       gewählten Werte beziehen sich auf die Basisteile des Laufs.
                                       Technische Info: Datenbankfeld: ID_GROUP

                                       Pseudoserien Über die Pseudoserien haben Sie in der Feinplanung die
                                       Möglichkeit, Positionen mit gleichem Aufbau zu sogenannten Pseudoserien
                                       zusammen zu fassen. Die in der Kombobox enthaltenen Werte kommen aus
                                       dem Register Gruppierungen des Dialogs Gruppierung/Sortierung. Wählen
                                       Sie aus der Kombobox den Werte aus, der auf die Pseudoserien angewendet
                                       werden soll.
                                       Normaler Weise dürfen auf festen Abstellplätzen nur kurzzeitig einzelne
                                       Scheiben (einzelne Positionen, welche jeweils nur 1 Scheibe enthalten) zwi-
                                       schengelagert / abgestellt werden, um bspw. auf Nachläufer zu warten. Mittels
                                       der Pseudo-Serie kann man nun identische Positionen (Einzelscheiben) als
                                       Serie zusammenfassen und diese dürfen nun auch ausnahmsweise gemein-
3,00 / 01-2023




                                       sam auf einen festen Abstellplatz abgestellt werden.
                                       Die Pseudo-Serie hat noch einen 2. Sinn.



                 A+W Production Feinplanung                                                                  F-127
                 Organisationen                                                                  Softwarereferenz




                                  Eine Serie (Stückzahl >100, aber das definiert jeder Kunde anders) kann pro-
                                  zesstechnisch anders durch die Produktion laufen - andere Laufwege, andere
                                  Behandlung. Mittels der Pseudo-Serie bekommen kann ich einzelne Positio-
                                  nen als "Serie" markieren und diese als Serien behandeln.(bekommen dann
                                  auch intern das Serien-Flag).
                                  Technische Info: Datenbankfeld: ID_PSEUDOGROUP

                                  Mindestmenge Das Feld bezieht sich auf das Feld Pseudoserien und gibt
                                  an, ab welcher Mindestmenge Pseudoserien erzeugt werden. Liegt der Wert
                                  darunter, wird keine Pseudoserie gebildet.
                                  Technische Info: Datenbankfeld: PSEUDOSCHWELLE

                                  Freigabe Bei der Freigabe des mit dieser Master-Orga feingeplanten Laufes
                                  wird das hier angezeigte Skript (*.bas/*.bat-Datei) verwendet. Betätigen Sie
                                  die Schaltfläche [Freigabe], öffnet sich der Dialog Auswahl Skript. In diesem
                                  Dialog sind alle im Programm angelegten Skripte enthalten. Die Skripte wer-
                                  den im A+W Production-Verzeichnis in einem separaten Ordner abgelegt
                                  (Ordnername: Scripts).
                                  Technische Info: Datenbankfeld: SKRIPT

                                  Auffüller Dieses Feld dient dazu, Scheiben mit einer größeren Dicke als vom
                                  Kunden bestellt zu optimieren. Diese Scheiben dienen dann als sogenannte
                                  Füller. Voraussetzung dafür ist jedoch, dass die Scheiben auf jeden Fall in ein
                                  ISO eingebaut werden. Darüber hinaus muss das ISO die in diesem Feld ste-
                                  hende Bedingung erfüllen. Betätigen Sie die Schaltfläche [Auffüller], öffnet
                                  sich der Formeleditor. Dort können Sie aus den definierten Formeln die ge-
                                  wünschte auswählen. Nachdem Sie den Dialog geschlossen haben, wird Ih-
                                  nen der Name der Formel im Feld dahinter angezeigt.
                                  Technische Info: Datenbankfeld: ID_FILLERCONDITION

                                  Quasiteile Dieses Feld ermöglicht Ihnen die Abbildung von Quasiteilen. Qua-
                                  siteile sind Teile, die ihre Losbildungs- und Abstellplatzinformationen von ihren
                                  Unterteilen übernehmen und nicht nur fest vom Lostyp der Teile und Bearbei-
                                  tungen abhängig zu machen. Nun kann über eine Bedingung an der Master-
                                  Orga noch gezielter bestimmt werden, für welche Teile eines Lostyps dies er-
                                  laubt ist. Betätigen Sie die Schaltfläche [Quasiteile], öffnet sich der Formeledi-
                                  tor. Dort können Sie aus den definierten Formeln die gewünschte auswählen.
                                  Nachdem Sie den Dialog geschlossen haben, wird Ihnen der Name der For-
                                  mel im Feld dahinter angezeigt.
                                  Technische Info: Datenbankfeld: ID_QUASICONDITION

                                  Bereich unten Bei diesem Bereich handelt es sich um die Verwendung von
                                  Sonderteilen (Füller, Restblätter, Bruchscheiben und Eilscheiben). Sie müs-
                                  sen erst in der Liste das gewünschte Sonderteil markieren und können an-
                                  schließend rechts daneben die entsprechenden Abstellplatz-Nummer
                                  vergeben.

                                  Verwende Füller Das Feld bezieht sich auf vorhandene Füllaufträge. Füllauf-
                                  träge können von der Feinplanung nur dann verwendet werden, wenn in der
3,00 / 01-2023




                                  ausgewählten Master-Orga diese Checkbox aktiviert ist.




                 F-128                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                    Organisationen




                                        Die Füller werden im Zuschnitt auf beliebige Böcke gestellt, deren Num-
                                       mernkreis durch Start Füller und Ende Füller gegeben ist. Dabei wird jeder Po-
                                       sition genau eine Bocknummer zugewiesen.
                                        Es werden keine Füller verwendet.
                                       Technische Info: Datenbankfeld: USEFUELLER

                                       Start Füller Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der
                                       verwendeten Füllaufträge. Sie geben hier die kleinste Abstellplatz-Nummer
                                       an, auf der Füllaufträge abgestellt werden können.
                                       Technische Info: Datenbankfeld: FUELLERSTART

                                       Ende Füller Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der
                                       verwendeten Füllaufträge. Sie geben hier die höchste Abstellplatz-Nummer
                                       an, auf der Füllaufträge abgestellt werden können.
                                       Technische Info: Datenbankfeld: FUELLERENDE

                                       Verwende Restblätter Das Feld bezieht sich auf Scheiben, die auf aufgelös-
                                       ten Restblättern vorangegangener Feinplanungen lagen.
                                        Die ausgewählte Master-Orga verwendet Restblätter. Die Restscheiben
                                       werden im Zuschnitt auf beliebige Böcke gestellt, deren Nummernkreis durch
                                       Start Restblatt und Ende Restblatt gegeben ist. Dabei wird jeder Position ge-
                                       nau eine Bocknummer zugewiesen.
                                        Es werden keine Restblätter verwendet.
                                       Technische Info: Datenbankfeld: USERESTBLATT

                                       Start Restblatt Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis
                                       der verwendeten Restblätter. Sie geben hier die kleinste Abstellplatz-Nummer
                                       an, auf der Restblätter abgestellt werden können.
                                       Technische Info: Datenbankfeld: RESTBLATTSTART

                                       Ende Restblatt Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis
                                       der verwendeten Restblätter. Sie geben hier die höchste Abstellplatz-Nummer
                                       an, auf der Restblätter abgestellt werden können.
                                       Technische Info: Datenbankfeld: RESTBLATTENDE

                                       Verwende Bruchscheiben Das Feld bezieht sich auf vorhandene Bruch-
                                       scheiben.
                                        Die ausgewählte Master-Orga verwendet vorhandene Bruchscheiben. Die
                                       Bruchscheiben werden im Zuschnitt auf beliebige Böcke gestellt, deren Num-
                                       mernkreis durch Start Bruch und Ende Bruch gegeben ist. Dabei wird jeder
                                       Position genau eine Bocknummer zugewiesen.
                                        Es werden keine Bruchscheiben verwendet.
                                       Technische Info: Datenbankfeld: USEBRUCH

                                       Start Bruch Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der
                                       verwendeten Bruchscheiben. Sie geben hier die kleinste Abstellplatz-Nummer
                                       an, auf der Bruchscheiben abgestellt werden können.
3,00 / 01-2023




                                       Technische Info: Datenbankfeld: BRUCHSTART




                 A+W Production Feinplanung                                                                   F-129
                 Organisationen                                                            Softwarereferenz




                                  Ende Bruch Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis
                                  der verwendeten Bruchscheiben. Sie geben hier die höchste Abstellplatz-
                                  Nummer an, auf der Bruchscheiben abgestellt werden können.
                                  Technische Info: Datenbankfeld: BRUCHENDE

                                  Verwende Eilscheiben Das Feld bezieht sich auf vorhandene Eilscheiben.
                                   Die ausgewählte Master-Orga verwendet vorhandene Eilscheiben.
                                   Es werden keine Eilscheiben verwendet.
                                  Technische Info: Datenbankfeld: USEBRUCH


                                  Weitere Informationen zur Master-Orga
                                   Tutorial, “Master-Orga” auf Seite F-71
                                   Tutorial, “Sonderteile” auf Seite F-30
                                   Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-130                                                          A+W Production Feinplanung
                 Softwarereferenz                                                                   Organisationen




                                       Orga
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga
                                       markieren > [Einstellungen]




                                       Abb. F-51   Orga Einstellungen


                                       In diesem Dialog legen Sie neue Orgas an oder nehmen Änderungen an be-
                                       stehenden Orgas vor. Weitere Erläuterungen finden Sie in den entsprechen-
                                       den Feldern.
                                       Technische Info: Datenbanktabelle: FEIN_ORGA

                                       Erläuterung der Felder

                                       Name der Orga-Form In diesem Feld geben Sie den Namen der Orga an.
                                       Technische Info: Datenbankfeld: NAME

                                       Typ In dieser Kombobox wählen Sie den Orga-Typ. Orga-Typen sind Stan-
                                       dard, Packmittel und alle im System enthaltenen Lostypen mit Ausnahme des
                                       Zuschnitts. Um in diesem Feld einen Lostyp auswählen zu können, muss die-
                                       ser bereits definiert sein! Die Definition nehmen Sie im Dialog Lostypen vor.
                                       Technische Info: Datenbankfeld: LOSTYP

                                       Produktion Die Checkbox steuert, ob es sich bei der Orga um eine Produk-
                                       tions- oder um eine Verwendungs-Orga handelt.
                                        Bei der Orga handelt es sich um eine Produktions-Orga
                                        Bei der Orga handelt es sich um eine Verwendungs-Orga.
                                       Technische Info: Datenbankfeld: PRODUKTION

                                       Abstellmodus Über die Optionen nehmen Sie die Voreinstellung des Abstell-
                                       platzmodus auf A-Böcken innerhalb der Orga vor. Die hier vorgenommenen
                                       Einstellungen können in der Orga jederzeit noch überschrieben werden.
                                       Der Standard-Wert für den Abstellmodus ist Einheit. Mögliche Werte:
                                       • Glas
                                       • Einheit
                                       • Produktion
3,00 / 01-2023




                                       • VABGLA
                                       Technische Info: Datenbankfeld: BELEGUNGSMODE



                 A+W Production Feinplanung                                                                  F-131
                 Organisationen                                                                 Softwarereferenz




                                  Kein Teilen von … bei Bockbelegung von mehr als … Prozent Mögli-
                                  che Werte:
                                  Gruppen: Sollte eine Gruppe von Scheiben auf einen Abstellplatz gestellt wer-
                                  den, diese Gruppe aber wegen der Bocktiefe nicht mehr komplett auf den Ab-
                                  stellplatz passen, so wird die Gruppe nicht geteilt und ein Teil dort abgestellt,
                                  falls der Abstellplatz bereits zu mehr als X Prozent belegt ist, bevor begonnen
                                  wird, die Gruppe auf dem Abstellplatz abzustapeln.
                                  Technische Info: Datenbankfeld: USETIEFE_GRUPPE
                                  Einheiten: Sollte eine Gruppe geteilt auf einem Abstellplatz abgestellt werden,
                                  so kann diese Teilung genau innerhalb einer Einheit stattfinden. Auch hier wird
                                  das Teilen der Einheit verhindert, falls der Abstellplatz bereits zu mehr als X
                                  Prozent belegt ist.
                                  Damit eine Einheit gesplittet werden kann, muss auf jeden Fall die Gruppe ge-
                                  splittet werden, daher sollte der Wert für die Gruppen stets größer als der für
                                  die Einheiten sein.
                                  Technische Info: Datenbankfeld: USETIEFE_EINHEIT


                                  Weitere Informationen zur Orga
                                   Tutorial, “Orgas” auf Seite F-68
                                   Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-132                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                    Organisationen




                                       Orga-Gruppen
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge >
                                       Orga-Gruppe > [Einstellungen]




                                       Abb. F-52    Einstellungen Orga-Gruppen


                                       In diesem Dialog nehmen Sie die Einstellungen zu bereits vorhandenen oder
                                       aber auch neuen Orga-Gruppen vor. Das bedeutet, Sie vergeben oder ändern
                                       den Namen der Orga-Gruppe und weisen der Orga-Gruppe sogenannten
                                       Gruppierungen und/oder Sortierungen zu. Weitere Erläuterungen finden Sie in
                                       den entsprechenden Feldern.
                                       Technische Info: Datenbanktabelle: FEIN_ORGAGRUPPE

                                       Erläuterung der Felder

                                       Name In diesem Feld geben Sie den Namen für die Orga-Gruppe ein.
                                       Technische Info: Datenbankfeld: NAME

                                       DynOpt Einstellung Diese Checkbox müssen Sie aktivieren, wenn die
                                       Orga-Gruppe für A+W DynOpt gedacht sind. D. h., Scheiben, die für A+W Dy-
                                       nOpt gedacht sind, können nur in einer Orga-Gruppe landen, die dieses Kenn-
                                       zeichen trägt.
                                       Technische Info: Datenbankfeld: DYNOPT

                                       Bildung der Gruppen Das Feld steuert, ob für die jeweilige Orga-Gruppe,
                                       eine Gruppenbildung erfolgen soll. Die Kombobox enthält alle bereits definier-
                                       ten Gruppierungen, unter denen Sie die entsprechende auswählen können.
                                       Die Gruppierungen werden in den Stammdaten angelegt.
                                       Wählen Sie aus der Kombobox die entsprechende Gruppierung.
                                       Technische Info: Datenbankfeld: GROUPINDEX

                                       Sortierung der Gruppen Die Checkbox ist in Zusammenhang mit dem Feld
                                       Bildung der Gruppen zu sehen und steuert, ob eine Sortierung der dort ge-
                                       wählten Gruppe erfolgen soll.
3,00 / 01-2023




                                        Es erfolgt eine Sortierung der Gruppen.
                                        Es erfolgt keine Sortierung der Gruppen.
                                       Technische Info: Datenbankfeld: HASGSORT


                 A+W Production Feinplanung                                                                   F-133
                 Organisationen                                                                    Softwarereferenz




                                  Sortierung in den Gruppen Die Kombobox steuert, ob für die im Feld Bil-
                                  dung der Gruppen getroffene Auswahl eine Sortierung innerhalb der entspre-
                                  chenden Gruppe stattfinden soll. Es gibt die folgenden Sortierungswerte:
                                  • Keine = Es erfolgt keine Sortierung in den Gruppen.
                                  • Global = Die Angaben aus den Voreinstellungen werden übernommen.
                                  • Selbst definierte Sortierungen.
                                  Technische Info: Datenbankfeld: SUBSORTINDEX

                                     Einstellungen bei Orga-Gruppen
                                     Wenn Orga-Gruppen mit Gruppierung und Sortierung definiert wurden,
                                     muss für den Abstellplatz keine Gruppierung/Sortierung eingestellt wer-
                                     den, da dies von der Orga-Gruppe übernommen wird. Wenn für den Ab-
                                     stellplatz Einstellungen vorgenommen werden, überschreiben diese die
                                     Gruppierung/Sortierung der Orga.


                                  Weitere Informationen zu Orga-Gruppen
                                   Tutorial, “Orgas” auf Seite F-68
                                   Tutorial, “Produktionsreihenfolge” auf Seite F-81
                                   Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-134                                                                  A+W Production Feinplanung
                 Softwarereferenz                                                                   Organisationen




                                       Einstellungen-Abstellplatz
                                       Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ein-
                                       stellungen > Register [Verwendung]




                                       Abb. F-53   Einstellungen - Abstellplatz


                                       In diesem Dialog nehmen Sie die Zuweisung von Namen und Nummernkrei-
                                       sen zu den Abstellplätzen vor. Es ist darauf zu achten, dass die Namen und
                                       Nummernkreise mit dem Abstellplatz-Typ (A-Bock, Fächerwagen, etc.) korre-
                                       spondieren. Darüber hinaus werden die Gruppierungen und Sortierungen so-
                                       wie die Abstellmodi zugewiesen.
                                       Technische Info: Datenbanktabelle: FEIN_BOCKTYP

                                       Erläuterung der Felder

                                       Name In diesem Feld geben Sie den Namen für die Abstellplatz-Typ ein.
                                       Technische Info: Pflichtfeld, Alphanumerisch, 32stellig, Datenbankfeld: NAME

                                       Bildung der Gruppen Das Feld steuert, ob für den jeweilige Abstellplatz-
                                       Typ, eine Gruppenbildung erfolgen soll. Die Kombobox enthält alle bereits de-
                                       finierten Gruppierungen, unter denen Sie die entsprechende auswählen kön-
                                       nen. Die Gruppierungen werden in den Stammdaten angelegt. Wählen Sie
                                       aus der Kombobox die entsprechende Gruppierung
                                       Technische Info: Datenbankfeld: GROUPINDEX

                                       Sortierung in den Gruppen Die Kombobox steuert, ob für die im Feld Bil-
                                       dung der Gruppen getroffene Auswahl eine Sortierung innerhalb der entspre-
                                       chenden Gruppe stattfinden soll. Es gibt die folgenden Sortierungs-Werte:
                                       • Keine = Es erfolgt keine Sortierung in den Gruppen.
3,00 / 01-2023




                                       • Global = Die Angaben aus den Voreinstellungen werden übernommen.
                                       • Selbst definierte Sortierungen.
                                       Technische Info: Datenbankfeld: SUBSORTINDEX

                 A+W Production Feinplanung                                                                  F-135
                 Organisationen                                                              Softwarereferenz




                                  Invertierung überprüfen Bei Bearbeitungen, die über die Lostypen-Einstel-
                                  lung Nicht verwenden, Nur Eigenschaften oder Verwende Unterteil innerhalb
                                  der Feinplanung aus der Stückliste entfernt werden, kann über die dafür zu-
                                  ständige logische Maschine hinterlegt werden, ob durch diesen Bearbeitungs-
                                  schritt die Reihenfolge auf A-Böcken invertiert werden muss.
                                  In den Nummernkreisen der Feinplanung kann dann eingestellt werden, ob
                                  das Kennzeichen der logischen Maschine verwendet werden soll. Ist dies der
                                  Fall und zwischen dem zu produzierenden Schritt und dem verwendeten
                                  Schritt befindet sich eine ungerade Anzahl an Bearbeitungen, die obiges
                                  Kennzeichen haben, so wird auf A-Böcken die Reihenfolge innerhalb der Sta-
                                  pel invertiert. Dazu werden Scheiben mit unterschiedlichen Invertierungsver-
                                  halten auf separate Stapel gestellt.
                                  Für den Zuschnitt bedeutet dies, dass auch die Brechreihenfolge entspre-
                                  chend angepasst wird.
                                  Technische Info: Datenbankfeld: INVERT_SEQUENCE

                                  Abstellmodus Gruppen Das Feld wird nur dann ausgewertet, wenn der Op-
                                  timierungs-Modus 6.1 oder 5.1 verwendet wird. Die Kombobox steuert in die-
                                  sem Fall, wie Gruppen abgestellt werden. Wählen Sie aus der Kombobox den
                                  entsprechende Abstellmodus. Mögliche Werte:
                                  • nur 1 Gruppe je Stapel.
                                  • vollständige Gruppen gemeinsam.
                                  • feste Reihenfolge.
                                  • nur 1 aufgeteilte Gruppe je Stapel.
                                  • alternierend.
                                  Technische Info: Datenbankfeld: BELEGMODE

                                  Optimierungsverhalten Die Kombobox ist in Zusammenhang mit dem Feld
                                  Bildung der Gruppen zu sehen. Bitte wählen Sie aus der Kombobox, wie Sie
                                  optimieren möchten. Mögliche Werte
                                  • Gruppen frei (6.1).
                                  • Gruppen sortiert (6.2).
                                  • Alles frei (5.1).

                                     Optimierungs-Modus verwenden
                                     Die Optimierungs-Modi 6.1 und 6.2 werden nur dann verwendet, wenn Auf-
                                     trags-Nummer und Positions-Nummer im Gruppierungs- und Sortierungs-
                                     schlüssel enthalten sind. Sind diese nicht enthalten, wird der
                                     Optimierungs-Modus 5.2 verwendet.

                                  Auffang-Abstellplatz Diese Checkbox steuert den Auffang-Abstellplatz. Als
                                  Auffang-Abstellplatz wird der Abstellplatz markiert, auf dem die Teile eines
                                  Laufes landen, die keinem anderen Abstellplatz zugewiesen werden konnten,
                                  da sie keine der für die anderen Abstellplätze definierten Bedingungen erfül-
                                  len.
                                   Bei dem Abstellplatz handelt es sich um den Auffang-Abstellplatz der Orga.
                                   Bei diesem Abstellplatz handelt es sich nicht um einen Auffang-Abstellplatz
3,00 / 01-2023




                                  der Orga.
                                  Technische Info: Datenbankfeld: AUFFAENGER



                 F-136                                                          A+W Production Feinplanung
                 Softwarereferenz                                                                    Organisationen




                                       Von / Bis: Für jeden Bocktyp wird mindestens ein Nummernkreis erfasst, der
                                       beschreibt, in welchem Bereich die Bocknummern für diesen Bocktyp liegen
                                       dürfen. Verwendungsbocktypen können darüber hinaus sogar zwei Num-
                                       mernkreise haben, falls für diese auch ein Produktionsbock vergeben wird.
                                       Weder innerhalb einer Orga noch innerhalb einer Master-Orga darf es vor-
                                       kommen, dass die darin enthaltenen Nummernkreise sich überlappen (das
                                       lässt das Programm auch nicht zu und wird Sie mit entsprechenden Fehler-
                                       meldungen darauf hinweisen). Für die Master-Orgas ist dabei zu beachten,
                                       dass diese noch zusätzlich Nummernkreise für diverse Spezialitäten (Bruch,
                                       Füller, Rest) beinhalten können.
                                       Technische Info: Datenbankfeld: MINIMUM
                                       Technische Info: Datenbankfeld: MAXIMUM

                                       Max. Anzahl Gruppen Dieses Feld bezieht sich auf die maximale Anzahl
                                       von Gruppen, die auf dem Abstellplatz stehen dürfen. Sollen beliebig viele
                                       Gruppen abgestellt werden können, so muss hier der Wert 0 eingetragen wer-
                                       den.
                                       Technische Info: Datenbankfeld: MAXNUMBER

                                       Nächsten Schritt trennen Ist die Checkbox aktiviert, wird bei A-Böcken
                                       auch auf die Losbildung des nächsten Schrittes geschaut, wenn überprüft
                                       wird, was zusammen abgestellt werden kann.

                                       Freie Optimierung (nur für A-Bock) Mit dieser Checkbox können Sie für je-
                                       den Nummernkreis einstellen, ob alle A-Böcke dieses Nummernkreises die
                                       Freie Optimierung automatisch verwenden sollen.

                                       Abstellmodus Die in diesem Bereich aufgeführten Werte sind in Zusammen-
                                       hang mit dem Feld Abstellplatz-Typ zu sehen. Wenn Sie im Feld Abstellplatz-
                                       Typ die Radiotaste A-Bock aktiviert haben, erscheinen die Werte:
                                       • Global: Der in der Orga hinterlegte Modus wird verwendet.
                                       • Glas: Jede Glasart erhält eine eigenen Nummer und wird auf einem eige-
                                          nen Abstellplatz abgestellt.
                                       • Einheit: Die jeweils zusammengehörigen Gläser einer Einheit (VSG, ISO)
                                          werden gemeinsam auf einem Abstellplatz mit einer gemeinsamen Abstell-
                                          platznummer abgestellt. Unterschiedliche Glasarten werden dabei auto-
                                          matisch vom System getrennt und in verschiedenen Stapeln
                                          nebeneinander abgestellt.
                                       • Produktion: Mehrere Glasarten werden gemeinsam, in nach Glasart ge-
                                          trennten Stapeln, auf einem Abstellplatz abgestellt. Aus diesen verschiede-
                                          nen Stapeln können verschiedene Produkte / Kombinationen gefertigt
                                          werden.
                                       • VABGLA: Es gibt pro Glastyp einen logischen Abstellplatz mit jeweils ei-
                                          nem Stapel. Der Unterschied zum Modus Glas ergibt sich bezüglich dem
                                          Splitten von Gruppen bei Erreichen der Maximalbeladung des Abstell-
                                          platzes. Genaueres entnehmen Sie bitte der Beschreibung der Modi im Tu-
                                          torial.
                                       Wenn Sie im Feld Abstellplatz-Typen die Radiotaste Fächerwagen aktiviert
3,00 / 01-2023




                                       haben, erscheinen die Werte:
                                       • Zusammen: Scheibe und Gegenscheibe(n) werden immer zusammen auf
                                          einen Fächerwagen gestellt.


                 A+W Production Feinplanung                                                                   F-137
                 Organisationen                                                                 Softwarereferenz




                                  •  Glas: Die Scheiben werden immer getrennt weggestellt.
                                  •  Kompakt: Es werden nur Scheiben auf einen Fächerwagen gestellt, die ein
                                     gemeinsames Kennzeichen haben. Dieses Kennzeichen kann, je nach
                                     Konfiguration, entweder das Feld XOPT_TISCH.CUTGO oder das Feld
                                     POOL_TEILE.SONDERKZ3 sein.
                                  Wenn Sie im Feld Abstellplatz-Typen die Radiotaste Feste Abstellplätze akti-
                                  viert haben, ist der Bereich Abstellmodus nicht aktiv.
                                  Technische Info: Datenbankfeld: BELEGMODE

                                  Abstellplatz-Typ Die Optionen steuern, um welchen Abstellplatz-Typ es sich
                                  handelt. Mögliche Werte:
                                  • A-Bock
                                  • Fächerwagen
                                  • Feste Abstellplätze
                                  Die darunter liegende Kombobox bezieht sich immer auf den aktivierten Ab-
                                  stellplatz-Typ. Sollte es z.B. bei einem A-Bock mehrere Ausführungen geben,
                                  können Sie auf diese dann in der Kombobox zugreifen.
                                  Technische Info: Datenbankfeld: TYPE

                                  Erläuterung der Schaltflächen

                                  Abstellplätze Wählen Sie diese Schaltfläche, um den Dialog Abstellplätze zu
                                  öffnen.


                                  Weitere Informationen zum Register Verwendung
                                   Tutorial, “Abstellplätze” auf Seite F-38
                                   Tutorial, “Gruppierungsschlüssel der Orga-Gruppen” auf Seite F-82
                                   Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-138                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                 Organisationen




                                       Voreinstellungen
                                       Stammdaten > Feinplanung > Voreinstellung




                                       Abb. F-54     Voreinstellungen


                                       Die hier vorhandenen Einstellungen werden immer dann verwendet, wenn
                                       keine Einstellungen für Orga, Gruppierung und Sortierung in der Orga sowie
                                       Sortierung auf dem Abstellplatz vorgenommen wurden. Es wird empfohlen,
                                       hier Einstellungen vorzunehmen, da sonst beim Starten der Feinplanung eine
                                       Fehlermeldung erscheint.

                                       Erläuterung der Felder

                                       Verarbeitungsreihenfolge In dieser Kombobox können Sie unter den vor-
                                       handenen Sortierungen die entsprechende auswählen. Die Sortierungen wer-
                                       den in den Stammdaten angelegt und steuern an dieser Stelle, nach welchen
                                       Kriterien die Scheiben verarbeitet werden.

                                       Orga In dieser Kombobox können Sie unter den vorhandenen Master-Orgas
                                       die entsprechende auswählen. Die Master-Orgas werden in den Stammdaten
                                       angelegt und steuern, mit welcher Master-Orga der Lauf die Feinplanung
                                       durchläuft.

                                       Gruppenbildung In dieser Kombobox können Sie unter den vorhandenen
                                       Gruppierungen die entsprechende auswählen. Die Gruppierungen werden in
                                       den Stammdaten angelegt und steuern, anhand welcher Kriterien eine Grup-
                                       penbildung stattfinden soll.

                                       Sortierung auf Abstellplatz In dieser Kombobox können Sie unter den vor-
                                       handenen Sortierungen die entsprechende auswählen. Die Sortierungen wer-
                                       den in den Stammdaten angelegt und steuern, anhand welcher Kriterien
                                       Scheiben sortiert werden sollen.


                                       Weitere Informationen zu den Voreinstellungen
                                        Tutorial, “Globale Einstellungen” auf Seite F-79
                                        Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 A+W Production Feinplanung                                                                F-139
                 Gruppierung und Sortierung                                                           Softwarereferenz




                                        Gruppierung und Sortierung
                                        Die Einstellungen, die Sie im Bereich Gruppierung/Sortierung vornehmen, ha-
                                        ben die Aufgabe, die Scheiben auf den Abstellplätzen zu gruppieren und zu
                                        sortieren. Die Scheiben werden in Gruppen zusammengefasst und innerhalb
                                        der Gruppen sortiert. Es ist weiterhin möglich, die Abfolge der Gruppen zu be-
                                        stimmen.


                                        Gruppierung/Sortierung - Dialog
                                        Der Dialog ist in drei Register unterteilt:
                                        •     Register Editor-Gruppierungen
                                        •     Register Editor-Sortierung
                                        •     Register Zusatz-Sortierungen


                                        Weitere Informationen zu Gruppierung und Sortierung
                                         Tutorial, “Gruppierungen und Sortierungen” auf Seite F-21
                                         Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-140                                                                   A+W Production Feinplanung
                 Softwarereferenz                                                         Gruppierung und Sortierung




                                       Register Editor-Gruppierungen
                                       Stammdaten > Feinplanung > Gruppierung > Register Editor - Gruppierung




                                       Abb. F-55    Gruppierung/Sortierung-Dialog, Register Gruppierung


                                       In diesem Dialog stellen Sie neue Gruppierungen zusammen oder nehmen
                                       Änderungen an bestehenden Gruppierungen vor. Die im Register Editor-
                                       Gruppierungen vorhandenen Einträge finden in folgenden Bereichen Verwen-
                                       dung:
                                       •   Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
                                       •   Softwarereferenz, “Orga-Gruppen” auf Seite F-133
                                       •   Softwarereferenz, “Master-Orga” auf Seite F-126
                                       •   Softwarereferenz, “Voreinstellungen” auf Seite F-139
                                       Technische Info: Datenbanktabelle: SORTING

                                       Erläuterung der Felder

                                       Linkes Fenster Das Fenster zeigt Ihnen alle angelegten Gruppierungen bzw.
                                       Sortierungen. Die einzelnen Gruppierungen/Sortierungen sind in einer Baum-
                                       struktur angelegt, so dass Sie sich die Eigenschaften, aus denen die Gruppie-
                                       rungen/Sortierungen bestehen, durch Aufklappen des Baumes anzeigen
                                       lassen können. Bsp.: Die Gruppierung +Artikelnummer+Abstellbreite beinhal-
                                       tet die Eigenschaften Artikelnummer und Abstellbreite. Das Plus- oder Minus-
                                       Zeichen vor den jeweiligen Eigenschaften zeigt Ihnen die Sortier-Richtung der
                                       Eigenschaft. Bsp.: +Artikelnummer bedeutet, dass die Sortier-Richtung inner-
                                       halb der Artikelnummer aufsteigend ist. -Artikelnummer bedeutet, dass die
                                       Sortier-Richtung innerhalb der Artikelnummer absteigend ist.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                  F-141
                 Gruppierung und Sortierung                                                           Softwarereferenz




                                        Felder im Bereich Sortier-Richtung

                                        Aufsteigend Das Feld ist nur aktiv, wenn Sie eine Eigenschaft der Gruppie-
                                        rung/Sortierung markiert haben. Aktivieren Sie die Radiotaste Aufsteigend,
                                        bedeutet dies, dass die Sortier-Richtung der markierten Eigenschaft aufstei-
                                        gend ist. Optisch wird die Eigenschaft noch durch das Plus-Zeichen vor der
                                        Eigenschaft gekennzeichnet.

                                        Absteigend Das Feld ist nur aktiv, wenn Sie eine Eigenschaft der Gruppie-
                                        rung/Sortierung markiert haben. Aktivieren Sie die Radiotaste Absteigend, be-
                                        deutet dies, dass die Sortier-Richtung der markierten Eigenschaft absteigend
                                        ist. Optisch wird die Eigenschaft noch durch das Minus-Zeichen vor der Eigen-
                                        schaft gekennzeichnet.

                                        Erläuterung der Schaltflächen im Bereich Sortier-Richtung

                                        Entfernen Das Betätigen dieser Schaltfläche führt entweder zum Löschen
                                        der markierten Eigenschaft der Gruppierung/Sortierung oder zum Löschen
                                        der kompletten Gruppierung/Sortierung. Das hängt davon ab, was Sie mar-
                                        kiert haben. Haben Sie eine Eigenschaft der Gruppierung/Sortierung markiert,
                                        wird nur die Eigenschaft gelöscht. Ist jedoch die Gruppierung/Sortierung mar-
                                        kiert, wird die komplette Gruppierung/Sortierung gelöscht.

                                        Hinzufügen Diese Schaltfläche steht in Zusammenhang mit dem rechten
                                        Fenster. Die Eigenschaft bzw. Formel, die im rechten Fenster markiert ist, wird
                                        durch das Betätigen der Schaltfläche [Hinzufügen] entweder als ganze Grup-
                                        pierung/Sortierung oder als Eigenschaft in die Gruppierung/Sortierung einge-
                                        fügt. Das hängt davon ab, was Sie markiert haben. Haben Sie eine
                                        Gruppierung/Sortierung markiert, wird die Eigenschaft bzw. Formel der mar-
                                        kierten Gruppierung/Sortierung hinzugefügt. Haben Sie den in der linken Liste
                                        an oberster Stelle stehenden Eintrag (im Register Editor-Gruppierungen ist
                                        das der Eintrag Gruppierungen, im Register Editor-Sortierung ist das der Ein-
                                        trag Sortierung) markiert, wird eine neue Gruppierung/Sortierung angelegt.

                                        Erläuterung der Optionen

                                        Eigenschaft Ist die Radiotaste Eigenschaft aktiv, sehen Sie im rechten
                                        Fenster alle vorhanden Eigenschaften.

                                        Formel Ist die Radiotaste Formel aktiv, sehen Sie im rechten Fenster alle
                                        vorhanden Formeln.

                                        Erläuterung der Schaltfläche

                                        Formeln … Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Auswahl
                                        Formeln --1--. Sie können entweder eine bereits bestehende Formel ändern
                                        oder aber eine neue Formel erstellen. Nähere Erläuterungen finden Sie in der
                                        Dokumentation Formel-Editor.
3,00 / 01-2023




                                        Weitere Informationen zu Gruppierungen
                                         Tutorial, “Gruppierungen und Sortierungen” auf Seite F-21
                                         Überblick, “Schaltflächen” auf Seite A-78


                 F-142                                                                   A+W Production Feinplanung
                 Softwarereferenz                                                          Gruppierung und Sortierung




                                       Register Editor-Sortierung
                                       Stammdaten > Feinplanung > Gruppierung > Register Editor - Sortierungen




                                       Abb. F-56    Gruppierung/Sortierung-Dialog, Register Sortierung


                                       In diesem Dialog stellen Sie neue Sortierungen zusammen oder nehmen Än-
                                       derungen an bestehenden Sortierungen vor.
                                       Der Inhalt des Registers Editor-Sortierung ist mit dem des Registers Editor-
                                       Gruppierungen bis auf die nachstehend aufgeführte Schaltfläche identisch
                                       und wird deshalb an dieser Stelle nicht mehr erläutert. Die entsprechenden In-
                                       formationen finden Sie unter dem Register Editor-Gruppierung.
                                       Technische Info: Datenbanktabelle: SORTING

                                       Erläuterung der Schaltfläche

                                       Zusatzsortierung Betätigen Sie diese Schaltfläche, öffnet sich für die mar-
                                       kierte Sortierung der Dialog Zusatz-Sortierungen.


                                       Weitere Informationen zu Sortierungen
                                        Tutorial, “Gruppierungen und Sortierungen” auf Seite F-21
                                        Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 A+W Production Feinplanung                                                                   F-143
                 Gruppierung und Sortierung                                                            Softwarereferenz




                                        Register Zusatz-Sortierungen
                                        Stammdaten > Feinplanung > Gruppierung > Register Zusatz - Sortierungen




                                        Abb. F-57     Gruppierung/Sortierung-Dialog, Register Zusatz-Sortierungen


                                        Dieser Dialog gibt Ihnen einen Überblick zu den vorhandenen Zusatz-Sortie-
                                        rungen. Die Zusatz-Sortierungen legen Sie im Dialog Erzeugung einer Zusatz-
                                        Sortierung an.
                                        Technische Info: Datenbanktabelle:

                                        Erläuterung der Felder

                                        Schlüssel Die Tabellenspalte Schlüssel zeigt, auf welchen Schlüssel die Zu-
                                        satz-Sortierung angewendet wird.

                                        Wert In diesem Feld steht der Wert der Zusatz-Sortierung.

                                        Zusatzsortierung Das Feld zeigt Ihnen die komplette Sortierung an, auf die
                                        der Schlüssel wirkt.


                                        Weitere Informationen zu Zusatz-Sortierungen
                                         Tutorial, “Zusatz-Sortierung” auf Seite F-28
                                         Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-144                                                                    A+W Production Feinplanung
                 Softwarereferenz                                                        Gruppierung und Sortierung




                                       Erzeugung einer Zusatz-Sortierung
                                       Stammdaten > Feinplanung > Gruppierung > Register Editor - Sortierungen >
                                       [Erzeuge Zusatz-Sortierungen]




                                       Abb. F-58     Erzeugung einer Zusatz-Sortierung


                                       Sortierungen können noch durch zusätzliche Sortierungen ergänzt werden.
                                       Dazu muss lediglich eine Zusatz-Sortierung erzeugt werden, der die Kombi-
                                       nation Sortierungsschlüssel-Wert zugewiesen ist. Wenn nun eine Sortierung
                                       mit dem gegebenen Sortierungsschlüssel endet, so wird die Gruppe, deren
                                       Elemente alle den gegebenen Wert für den Sortierungsschlüssel haben,
                                       durch die zusätzliche Sortierung in weitere Gruppen aufgeteilt.
                                       Beispiel: Auf einem Abstellplatz sind die Positionen nach TOUR+KUNDEN-
                                       NUMMER+ sortiert. Wenn es nun eine Zusatzsortierung KLEINMASS+ gibt
                                       mit KUNDENNUMMER=4711, so wird nur für den Kunden 4711 eine erweiter-
                                       te Sortierung durchgeführt. Bei allen anderen Kunden ist die Reihenfolge be-
                                       liebig. Selbstverständlich ist es möglich, verschiedenen Kunden verschiedene
                                       Zusatzsortierungen zuzuweisen.
                                       Technische Info: Datenbanktabelle: MORESORTING

                                       Erläuterung der Felder

                                       Wert In diesem Feld geben Sie den Wert für die Zusatz-Sortierung an. Die
                                       Optionen Ziffer, Dicke, Text, Länge und SZR steuern, um welchen Wert es sich
                                       handelt. Die Zusatz-Sortierungen sehen Sie im Register Zusatz-Sortierung.

                                       Erläuterung der Schaltfläche

                                       Wert nicht prüfen Betätigen Sie diese Schaltfläche, wird, unabhängig des
                                       letzten Sortierungs-Schlüssels, die Zusatz-Sortierung verwendet.


                                       Weitere Informationen zur Erzeugung einer Zusatz-Sortierung
                                        Tutorial, “Zusatz-Sortierung” auf Seite F-28
3,00 / 01-2023




                                        Überblick, “Schaltflächen” auf Seite A-78




                 A+W Production Feinplanung                                                                 F-145
                 Abstellplätze                                                               Softwarereferenz




                                 Abstellplätze
                                 Der Dialog ist in drei Bereiche unterteilt:
                                 •   A-Böcke
                                 •   Fächerwagen
                                 •   Feste Abstellplätze


                                 Abstellplätze
                                 Stammdaten > Feinplanung > Abstellplätze
                                 Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Ab-
                                 stellplatz der Orga-Gruppe markieren > Schaltfläche [Einstellungen]




                                 Abb. F-59    Abstellplätze


                                 In diesem Dialog definieren Sie die in Ihrem Betrieb vorhandenen Abstellplät-
                                 ze oder nehmen Änderungen an vorhandenen Abstellplätzen vor. Die hier de-
                                 finierten Abstellplätze werden von folgenden Bereichen der Feinplanung
                                 verwendet:
3,00 / 01-2023




                                 •   Softwarereferenz, “Einstellungen-Abstellplatz” auf Seite F-135
                                 •   Softwarereferenz, “Register Orga” auf Seite F-182



                 F-146                                                          A+W Production Feinplanung
                 Softwarereferenz                                                                       Abstellplätze




                                       Technische Info: Datenbanktabelle: ABSTELLPLATZ

                                       Erläuterung der Felder im Bereich A-Böcke

                                       Kombobox Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Ent-
                                       fernen] und [Umbenennen] enthält die Namen der im System angelegten Ab-
                                       stellplätze für A-Böcke.

                                       Abstelltiefe In diesem Feld geben Sie die Abstelltiefe in mm an. Bsp. 1200
                                       mm bedeutet, dass der Stapel, der abgestellt wird, bis zu 1200 mm tief sein
                                       darf. Bitte beachten Sie, dass Abstelltiefen ab 20 m automatisch als unendli-
                                       che große Abstelltiefen behandelt werden.
                                       Technische Info: Datenbankfeld: TIEFE

                                       Breite Dieses Feld kennzeichnet die Gesamtbreite des Abstellplatzes in mm.
                                       Bsp. 2000 mm bedeutet, dass der Abstellplatz eine Breite von 2000 mm hat,
                                       auf der Scheiben abgestellt werden können.
                                       Technische Info: Datenbankfeld: BREITE

                                       Max. Abstellplätze/Bock In diesem Feld geben Sie ein, wie viele Abstellplät-
                                       ze Ihnen pro Bock zur Verfügung stehen. Mögliche Werte:
                                       • 1 = pro Bock steht Ihnen ein Abstellplatz zur Verfügung.
                                       • 2 = pro Bock stehen Ihnen 2 Abstellplätze zur Verfügung.
                                       • 4 = pro Bock stehen Ihnen 4 Abstellplätze zur Verfügung.
                                       Technische Info: Datenbankfeld: MAXCOUNT

                                       L-Bock Diese Checkbox muss aktiviert werden, wenn es sich bei dem Ab-
                                       stellplatz um einen L-Bock anstelle eines A-Bocks handelt.

                                       Robot Diese Checkbox muss aktiviert werden, wenn es sich bei dem A-Bock
                                       um einen Robot-Bock handelt. Bei einem Robot-Bock handelt es sich um ei-
                                       nen Abstellplatz, der durch einen Roboter angesteuert wird. Mögliche Werte:
                                       • 0 = Kein Robot-Bock.
                                       • 1 = Einfach = Robot-Bock, einfach.
                                       • 2 = Gespiegelt = Robot-Bock, gespiegelt.
                                       • 3 = Doppelt=Robot-Bock, doppelt vorhanden, dabei getrennt ansteuerbar.
                                       Technische Info: Datenbankfeld: ROBOT

                                       Anzahl Dieses Feld ist nur aktiv, wenn es sich bei dem A-Bock um einen Ro-
                                       bot-Bock handelt. Sie haben dann die Möglichkeit zu hinterlegen, wie viele Ro-
                                       bot-Böcke im Betrieb vorhanden sind. Ferner können Sie angeben, ob diese
                                       Anzahl einfach oder doppelt vorhanden ist, oder ob die Robot-Böcke eigent-
                                       lich zweifach ausgelegt sind, aber das System bei Auslastung selber entschei-
                                       det, welchen Robot-Bock es verwendet. Den mit gegebener Nummer aus der
                                       ersten oder zweiten Menge.

                                       Max. Anzahl A-Böcke Die maximale Anzahl an A-Böcken ist für die Bildung
3,00 / 01-2023




                                       von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte Anzahl er-
                                       reicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe geschlossen
                                       und eine neue begonnen. Diese kann dann zugeschnitten werden, wenn wie-
                                       der Böcke frei sind.


                 A+W Production Feinplanung                                                                   F-147
                 Abstellplätze                                                               Softwarereferenz




                                 Überprüfung Anzahl (Zuschnitt) Die Checkbox bezieht sich auf den im
                                 Feld Max. Anzahl A-Böcke stehenden Wert und prüft diesen gegebenenfalls.

                                 Sortjet Arbeiten Sie in Ihrem Hause mit einem Sortjet, müssen Sie diese
                                 Checkbox aktivieren.
                                 Technische Info: Datenbankfeld: SORTJET

                                 Maximales Gewicht (kg) Maximales Gewicht aller Scheiben auf dem A-
                                 Bock. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefangen.
                                 0 bedeutet hier, dass es keine Gewichtsbegrenzung gibt.
                                 Technische Info: Datenbankfeld: GEWICHT

                                 ID für Stack-Opti Arbeiten Sie in Ihrem Hause mit dem Stack Optimizer, wird
                                 hier die ID des verwendeten physikalischen Abstellplatzes hinterlegt. Die
                                 möglichen Werte holt sich die Anwendung aus den Konfigurationsdateien des
                                 Stack Optimizers.
                                 Technische Info: Datenbankfeld: STACK_ID

                                 Erläuterung der Felder im Bereich Fächerwagen

                                 Kombobox Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Ent-
                                 fernen] und [Umbenennen] enthält die Namen der im System angelegten Ab-
                                 stellplätze für Fächerwagen.

                                 Anzahl Fachnummer In diesem Feld geben Sie an, wieviel Fachnummern
                                 der Wagen hat. Bei einem Fach pro Nummer entspricht die Anzahl der Fach-
                                 nummern der Anzahl der Fächer des Wagens.
                                 Technische Info: Datenbankfeld: FACHANZAHL

                                 Breite Dieses Feld kennzeichnet die Breite der Fächer.
                                 Technische Info: Datenbankfeld: BREITE

                                 Zwei Fächer/Nummer Die Checkbox steuert, ob jeweils zwei Fächer eine
                                 gemeinsame Fachnummer bekommen. Die Anzahl der Fachnummern ist
                                 dann nur noch halb so groß wie die Anzahl der Fächer. D.h., es dürfen auch
                                 zwei Scheiben gemeinsam in ein Fach gestellt werden.
                                 Technische Info: Datenbankfeld: FACH_PRO_NR

                                 Start = 0 Die Checkbox steuert, ob die Zählung der Fachnummern bei 0 oder
                                 bei 1 beginnt.
                                  Die Zählung der Fachnummern beginnt mit 0.
                                  Die Zählung der Fachnummern beginnt mit 1 (Standard).
                                 Technische Info: Datenbankfeld: STARTFACH

                                 Anzahl der Stellen für Diese Radiotaste legt fest, wie viele Stellen der Ab-
                                 stellplatznummer für die Fachnummern reserviert werden.
                                 • 2 bedeutet, dass die letzten 2 Stellen reserviert sind.
3,00 / 01-2023




                                 • 3 bedeutet, dass die letzten 3 Stellen reserviert sind.
                                 • 4 bedeutet, dass die letzten 4 Stellen reserviert sind.
                                 Bei 50 Fachnummern sind das 2 Stellen, ab 100 Fachnummern 3 Stellen usw.



                 F-148                                                          A+W Production Feinplanung
                 Softwarereferenz                                                                      Abstellplätze




                                       Technische Info: Datenbankfeld: DIGITSFACH

                                       Max. Anzahl Fächerwagen Die maximale Anzahl an Fächerwagen ist für die
                                       Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte
                                       Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe ge-
                                       schlossen und eine neue begonnen. Diese kann dann zugeschnitten werden,
                                       wenn wieder Wagen frei sind.

                                       Überprüfung Anzahl (Zuschnitt) Die Checkbox bezieht sich auf den im
                                       Feld Max. Anzahl Fächerwagen stehenden Wert und prüft diesen gegebenen-
                                       falls.
                                        Der im Feld Max. Anzahl Fächerwagen stehende Wert wird geprüft. Wird er
                                       überschritten, erfolgt eine entsprechende Fehlermeldung. Die Feinplanung
                                       kann dann weder optimiert noch gespeichert werden.
                                        Es erfolgt keine Überprüfung der Anzahl.

                                       Sortjet Arbeiten Sie in Ihrem Hause mit einem Sortjet, müssen Sie diese
                                       Checkbox aktivieren.
                                       Technische Info: Datenbankfeld: SORTJET

                                       Maximale Nutzlast (kg) Erlaubtes Nutzgewicht des Abstellplatzes in Kilo-
                                       gramm. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefan-
                                       gen. 0 bedeutet hier, dass es keine Gewichtsbegrenzung gibt. Ist 0
                                       angegeben, wird die Zahl der auf dem Fächerwagen abzulegenden Scheiben
                                       nur durch die Anzahl der Fächer begrenzt.
                                       Technische Info: Datenbankfeld: GEWICHT

                                       Leergewicht (kg) Das Leergewicht des Abstellplatzes in Kilogramm.
                                       Technische Info: Datenbankfeld: LEERGEWICHT

                                       Abstand erstes/letztes Fach v. Achsen Hier geben Sie den Abstand zwi-
                                       schen Außenkante und Achse (links/rechts) ein.
                                       Technische Info: Datenbankfeld: ABSTAND_FACH_ACHSE

                                       Max. Abweichung Schwerpunkt v. Mitte (%) Hier geben Sie die erlaubte
                                       Abweichung von der Schwerpunktmitte aus in Prozent ein (+/-).
                                       Technische Info: Datenbankfeld: ABWEICHUNG_SP

                                       Erläuterung der Felder im Bereich Feste Abstellplätze

                                       Kombobox Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Ent-
                                       fernen] und [Umbenennen] enthält alle im System angelegten Festen Abstell-
                                       plätze.

                                       Abstelltiefe In diesem Feld geben Sie die Abstelltiefe in mm an. Bsp.: 1200
                                       mm bedeutet, dass der Stapel, der abgestellt wird, bis zu 1200 mm tief sein
                                       darf. Bitte beachten Sie, dass Abstelltiefen ab 20 m automatisch als unendli-
                                       che große Abstelltiefen behandelt werden.
3,00 / 01-2023




                                       Technische Info: Datenbankfeld: TIEFE




                 A+W Production Feinplanung                                                                   F-149
                 Abstellplätze                                                                Softwarereferenz




                                 Breite Dieses Feld kennzeichnet die Gesamtbreite des Abstellplatzes in mm.
                                 Bsp. 2000 mm bedeutet, dass der Abstellplatz eine Breite von 2000 mm hat,
                                 auf der Scheiben abgestellt werden können.
                                 Technische Info: Datenbankfeld: BREITE

                                 Max. Anzahl FAPs Die maximale Anzahl an Festen Abstellplätzen ist für die
                                 Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte
                                 Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe ge-
                                 schlossen und eine neue begonnen. Diese kann dann zugeschnitten werden,
                                 wenn wieder Abstellplätze frei sind.

                                 Überprüfung Anzahl (Zuschnitt) Die Checkbox bezieht sich auf den im
                                 Feld Max. Anzahl FAPs stehenden Wert und prüft dieses gegebenenfalls.
                                  Der im Feld FAPs stehenden Wert wird geprüft. Wird er überschritten, er-
                                 folgt eine entsprechende Fehlermeldung. Der feingeplante Lauf kann dann
                                 weder optimiert noch können die Ergebnisse gespeichert werden.
                                  Es erfolgt keine Überprüfung der Anzahl.

                                 Maximales Gewicht (kg) Maximales Gewicht aller Scheiben auf dem Festen
                                 Abstellplatz. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz ange-
                                 fangen. 0 bedeutet hier, dass es keine Gewichtsbegrenzung gibt.
                                 Technische Info: Datenbankfeld: GEWICHT


                                 Weitere Informationen zu Abstellplätzen
                                  Tutorial, “Abstellplätze” auf Seite F-38
                                  Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 F-150                                                           A+W Production Feinplanung
                 Softwarereferenz                                                                            Lose




                                       Lose
                                       In dem Dialog Lostypen und Bearbeitungen nehmen Sie die Einstellungen be-
                                       züglich der Losbildung für einen Lostyp vor. Dem Lostyp werden anschließend
                                       noch Bearbeitungen oder abhängige Bearbeitungen zugeordnet.


                                       Lostypen und Bearbeitungen
                                       Der Dialog ist in drei Register unterteilt:
                                       •   Register Lostypen
                                       •   Register Bearbeitungen
                                       •   Register Abhängige Bearbeitungen


                                       Register Lostypen
                                       Stammdaten > Feinplanung > Lostypen




                                       Abb. F-60     Lostypen und Bearbeitungen, Register Lostypen


                                       In diesem Dialog können Sie neue Lostypen anlegen oder existierende Los-
                                       tpyen ändern.
                                       Technische Info: Datenbanktabelle: FEIN_LOSTYP
3,00 / 01-2023




                 A+W Production Feinplanung                                                                F-151
                 Lose                                                                 Softwarereferenz




                         Erläuterung der Felder

                         Lostyp/Name Die Anzeige enthält alle definierten Lostypen mit deren Losty-
                         pnummer und Bezeichnung. Die Lostypnummer wird von der Feinplanung
                         beim Speichern in die Datenbank geschrieben. Der Namen des Lostyps wird
                         in den Anzeigen der Feinplanung verwendet.

                         Name/Typ/Beschaffungsart Die Anzeige enthält alle dem Lostyp zugewie-
                         senen Kombinationen von Bearbeitungstyp und Beschaffungsart. Durch einen
                         Doppelklick auf einen Eintrag wird zu der jeweiligen Seite im Dialog gewech-
                         selt und die betreffende Bearbeitung angezeigt. Bei Einträgen, die durch einen
                         nachfolgenden Stern (*) in der Spalte Typ gekennzeichnet sind, handelt es
                         sich um eine abhängige Bearbeitung.

                         Lostyp(-nummer) Die Lostypnummer muss ein Wert größer oder gleich 100
                         und zudem ein Vielfaches von 10 sein. Das liegt daran, dass für Verwen-
                         dungslose stets die Lostypnummer um eins erhöht in die Datenbank geschrie-
                         ben wird. Die Lostypnummer wird auch von der Feinplanung beim Speichern
                         in die Datenbank verwendet.
                         Technische Info: Datenbankfeld: LOSTYP

                         Name Das Feld enthält den Namen des Lostyps für die Anzeigen in der Fein-
                         planung.
                         Technische Info: Datenbankfeld: NAME

                         Gruppierung Die Kombobox enthält alle im System definierten Gruppierun-
                         gen. Scheiben mit gleichem Lostyp können mittels dieser Gruppierung auf
                         verschiedene Produktionslose verteilt werden. Ohne eine solche Gruppierung
                         erfolgt die Bildung der Lose nur nach den realen Maschinen. Ist eine Gruppie-
                         rung angegeben, so können zum Beispiel für ISOs die Produktionslose nach
                         dem Scheibenzwischenraum (SZR) gebildet werden. Dazu muss lediglich der
                         Gruppierungsschlüssel das Element Scheibenzwischenraum (SZR) enthal-
                         ten. Eine wichtige Ausnahme bildet hierbei der Zuschnitt. Für den Zuschnitt er-
                         folgt die Losbildung stets nach Glasart, Glasdicke und den realen Tischen. Die
                         Gruppierungen werden in den Stammdaten angelegt.
                         Technische Info: Datenbankfeld: GRUPPIERUNG

                            Gruppierungen
                            Gruppierungen können nur zur Bildung von Produktionslosen verwendet
                            werden. Verwendungslose werden allein nach dem Lostyp gebildet.

                         Technologietyp Die Kombobox enthält alle im System definierten Technolo-
                         gietypen. Der Technologietyp kommt aus der Maschinenzuordnung. Der Tech-
                         nologietyp kann auch 0 sein, falls keiner zugewiesen ist.
                         Technische Info: Datenbankfeld: TECHNOTYP

                         Produktionsreihenfolge Die Kombobox enthält alle im System definierten
                         Gruppierungen. Für abhängige Bearbeitungen wird in der Regel die Produkti-
                         onsreihenfolge ihrer erzeugenden Bearbeitung verwendet. Man kann aber mit
3,00 / 01-2023




                         der Produktionsreihenfolge eine eigene Reihenfolge hinterlegen. Sollten je-
                         doch durch diese eingestellte Produktionsreihenfolge Freiheiten in der Rei-
                         henfolge vorhanden sein, so werden für diese in Abhängigkeit der Checkbox


                 F-152                                                   A+W Production Feinplanung
                 Softwarereferenz                                                                                    Lose




                                       Sortierung invertieren die direkte oder invertierte Reihenfolge der erzeugen-
                                       den Bearbeitungen verwendet.
                                       Technische Info: Datenbankfeld: PROD_RF

                                       Sortierung invertieren Die Checkbox ist nur dann aktiv, wenn die Kombo-
                                       box Produktionsreihenfolge einen Eintrag (ungleich Keine) enthält. Siehe Er-
                                       läuterung
                                       Technische Info: Datenbankfeld: INVERT_RF

                                       Verhalten in der Feinplanung Diese Einstellung wird außer Verwende Un-
                                       terteil zur Zeit nur für Bearbeitungen und nicht für Teile selber verwendet. Mög-
                                       liche Werte:
                                       • Standard: Für diese Bearbeitung werden sowohl Lose als auch Abstellplät-
                                           ze bebildet bzw. vergeben.
                                       • Verwende Unterteil: Für diese Bearbeitung oder dieses Teil erfolgt nicht di-
                                           rekt eine Losbildung und Abstellplatzvergabe. Vielmehr werden die glei-
                                           chen Losnummer, Bocknummern und Sequenzen darin verwendet wie für
                                           das Unterteil. Zu beachten ist allerdings, dass dieses Verfahren nicht für
                                           alle Teile erlaubt ist. So darf das Teil auf keinen Fall Zuschnitt sein, es muss
                                           genau ein Unterteil haben und es darf nicht zur einer Packmitteloptimie-
                                           rung gehören. Ferner müssen sowohl Unter- als auch Oberteil sich im glei-
                                           chen Lauf befinden.
                                       • Nur Eigenschaft: In diesem Fall erfolgt für die Bearbeitung weder eine Los-
                                           bildung noch eine Bockvergabe. Die Bearbeitung und damit all ihre Eigen-
                                           schaften steht aber zur Zeit der Bockzuordnung im Rahmen der Orga zur
                                           Verfügung. Damit kann die Bockvergabe zum Beispiel dort nach der ersten
                                           Bearbeitung nach dem Zuschnitt erfolgen.

                                           Bearbeitung wird aus Teilebaum entfernt
                                           Die Bearbeitung wird unmittelbar nach der Bockzuordnung aus dem Teile-
                                           baum entfernt. Damit kann bei der Gruppierung und Sortierung auf den Ab-
                                           stellplätzen darauf kein Bezug mehr genommen werden. Dies lässt sich
                                           aber mit einem Trick umgehen. Man kann die gewünschte Eigenschaft ei-
                                           ner Bearbeitung mittels Zuweisung einer ansonsten nicht benötigten Ei-
                                           genschaft der Scheibe zuweisen.

                                       •  Nicht verwenden: Diese Bearbeitung wird nicht in den Teilebaum eingefügt
                                          und steht somit auch nicht bei der Bockzuordnung zur Verfügung. Selbst-
                                          verständlich erfolgt auch hier keine Losbildung oder Bockvergabe.
                                       Zu beachten ist, dass Lose für abhängige Bearbeitungen, die unter ihre erzeu-
                                       gende Bearbeitung angeordnet werden, nicht nur ihren eigenen Gruppie-
                                       rungsschlüssel verwenden, sondern sich auch noch zusätzlich nach der
                                       Losbildung der Teile richten.
                                       Technische Info: Datenbankfeld: FEINPLANUNG_KZ


                                       Weitere Informationen zu Lostypen
                                        Tutorial, “Lose” auf Seite F-17
3,00 / 01-2023




                                        Überblick, “Schaltflächen” auf Seite A-78




                 A+W Production Feinplanung                                                                        F-153
                 Lose                                                                Softwarereferenz




                         Register Bearbeitungen
                         Stammdaten > Feinplanung > Bearbeitungen




                         Abb. F-61   Lostypen und Bearbeitungen, Register Bearbeitungen


                         In diesem Dialog können Sie neue Bearbeitungen anlegen oder existierende
                         Bearbeitungen ändern. Eine Bearbeitungen wird durch ihren Namen, ihren
                         Teile- oder Bearbeitungstyp, ihre Beschaffungsart und dem zugeordneten
                         Lostyp spezifiziert. Sollte beim Start der Feinplanung kein Eintrag in den
                         Stammdaten für eine Kombination von Bearbeitungstyp/Beschaffungsart ge-
                         funden werden, so wird dieser Dialog automatisch aufgerufen, damit Sie hier
                         die fehlenden Bearbeitungen erfassen können. Danach kann die Feinplanung
                         unmittelbar fortgesetzt werden.
                         Technische Info: Datenbanktabelle: FEIN_BEARBTYP

                         Erläuterung der Felder

                         Name In diesem Feld steht der Name der Bearbeitung. Dieser Name wird nur
                         auf den weiteren Registern dieses Dialogs verwendet und taucht in der Fein-
                         planung selber nicht mehr auf.
                         Technische Info: Datenbankfeld: NAME

                         Typ Die Kombobox Typ enthält alle vorhandenen Bearbeitungs-Typen. Die
                         Bearbeitungs-Typen kommen aus den Stammdaten.
                         Technische Info: Datenbankfeld: BEARBTYP
3,00 / 01-2023




                 F-154                                                  A+W Production Feinplanung
                 Softwarereferenz                                                                          Lose




                                       Beschaffungsart Wählen Sie aus dieser Kombobox die für die Bearbeitung
                                       zutreffende Beschaffungsart. Mögliche Werte:
                                       • 0 = Produktion
                                       • 1 = Zuschnitt
                                       • 2 = Lagerentnahme
                                       • 9 = Bestellt
                                       Technische Info: Datenbankfeld: BESCHAFFUNGSART

                                       Lostyp Die Kombobox bezieht sich auf die im Register Lostyp angelegten
                                       Lostypen. Wählen Sie aus der Kombobox den entsprechenden Lostyp. Dabei
                                       ist zu beachten, dass nur Bearbeitungen der Beschaffungsart Zuschnitt dem
                                       Lostyp mit der Lostypnummer 100 zugewiesen werden dürfen und auch müs-
                                       sen.
                                       Technische Info: Datenbankfeld: LOSTYP

                                       Artikelnummer für fehlende Bearbeitung Die hier eingetragene Artikel-
                                       nummer einer Bearbeitung wird vom Import immer dann verwendet, wenn der
                                       Import eine solche benötigt und sonst nicht im System vorhanden ist.
                                       Technische Info: Datenbankfeld: ARTIKEL


                                       Weitere Informationen zu Bearbeitungen
                                        Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 A+W Production Feinplanung                                                              F-155
                 Lose                                                               Softwarereferenz




                         Register Abhängige Bearbeitungen
                         Stammdaten > Feinplanung > Bearbeitungen > Register Abhängige Bearbei-
                         tungen




                         Abb. F-62   Lostypen und Bearbeitungen, Register Abhängige Bearbeitungen


                         Über das Register Abhängige Bearbeitungen können weitere Bearbeitungen
                         automatisch erzeugt werden und so im Teilebaum eingefügt werden. Diese
                         abhängige Bearbeitungen werden durch die Attribute Namen (nur zur Anzeige
                         in diesem Dialog), Typ (Bearbeitungstyp aus der Tabelle BEARB_TYP), den
                         zugeordneten Lostyp und dem Kennzeichen Erzeugung spezifiziert.

                         Erläuterung der Felder

                         Name In diesem Feld steht Name der abhängigen Bearbeitung.
                         Technische Info: Datenbankfeld: NAME

                         Typ Der (Bearbeitungs-)Typ muss deshalb angegeben werden, damit, falls
                         diese Bearbeitung doch von der Auftragserfassung an A+W Production über-
                         geben wird, sie nicht unnötig erzeugt wird und die Bearbeitung somit doppelt
                         vorhanden wäre.
                         Technische Info: Datenbankfeld: BEARBTYP

                         Lostyp Wählen Sie aus dieser Kombobox die im System enthaltenen Losty-
                         pen. Die Lostypen kommen aus dem Register Lostypen.
3,00 / 01-2023




                         Technische Info: Datenbankfeld: LOSTYP

                         Erzeugung Das Feld legt fest, unter welchen Umständen die Bearbeitung er-
                         zeugt wird. Mögliche Werte:


                 F-156                                                 A+W Production Feinplanung
                 Softwarereferenz                                                                               Lose




                                       • Immer
                                       • Kopfteil
                                       • Nicht-Kopfteil
                                       Dabei kann die Bearbeitung entweder immer erzeugt werden, nur falls es sich
                                       bei dem Teil um ein Kopfteil handelt oder wenn es sich bei dem Teil gerade
                                       nicht um ein Kopfteil handelt. So könnte zum Beispiel für alle Teile die abhän-
                                       gige Bearbeitung Versand erzeugt werden, diese Bearbeitung würde natürlich
                                       nur an Kopfteilen Sinn machen und daher müsste die Einstellung Kopfteile ge-
                                       wählt werden.
                                       Technische Info: Datenbankfeld: ERZEUGUNG

                                       Die ausgewählte Bearbeitung erzeugt die folgenden abhängigen Bear-
                                       beitungen Diese Tabelle listet die für die ausgewählte Bearbeitung vorhan-
                                       denen abhängigen Bearbeitungen.


                                       Weitere Informationen zu abhängigen Bearbeitungen
                                        Tutorial, “Lose” auf Seite F-17
                                        Überblick, “Schaltflächen” auf Seite A-78
3,00 / 01-2023




                 A+W Production Feinplanung                                                                    F-157
                 Läufe feinplanen                                                                Softwarereferenz




                                    Läufe feinplanen
                                    Für Läufe, die sich in der Lauf-Anzeige mit dem Status grobgeplant befinden,
                                    können Sie über das Kontextmenü die Feinplanung starten. Die Feinplanung
                                    läuft im Hintergrund, das heißt, Sie können während der Feinplanung weiter
                                    arbeiten. Ist die Feinplanung abgeschlossen, erscheint der Dialog Feinpla-
                                    nung für Lauf ….


                                    Feinplanung für Lauf …
                                    Der Dialog ist in folgende Register unterteilt:
                                    •   “Register Glasarten” auf Seite F-159
                                    •   “Register Bockbelegung” auf Seite F-162
                                    •   “Register Ergebnisse” auf Seite F-167
                                    •   “Register Spezial” auf Seite F-169
                                        – “Register Zusammenlegen” auf Seite F-169
                                        – “Register Füllaufträge” auf Seite F-171
                                        – “Register Restblätter” auf Seite F-173
                                        – “Register Bruchscheiben” auf Seite F-174
                                        – “Register Eilscheiben” auf Seite F-176
                                        – “Register Glasdicken” auf Seite F-177
                                    •   “Register Freie Optimierung” auf Seite F-179
                                    •   “Register Orga” auf Seite F-182
                                    •   “Register Orga-Optionen” auf Seite F-184
                                    •   “Register Optionen” auf Seite F-186
                                    •   “Register Auswahl Lagermaß” auf Seite F-188
                                    Die einzelnen Register liefern Ihnen einen kompletten Überblick über alle an
                                    der Feinplanung beteiligten Parameter (Art des Zuschnitts, Abstellplätze, La-
                                    germaße, etc.). Die angezeigten Parameter können in den entsprechenden
                                    Registern geändert werden. Die Feinplanung muss dann noch einmal durch-
                                    laufen werden. Sie sollten jedoch mit Vorsicht durchgeführt werden!
3,00 / 01-2023




                 F-158                                                                A+W Production Feinplanung
                 Softwarereferenz                                                                     Läufe feinplanen




                                       Register Glasarten
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Glasarten




                                       Abb. F-63    Feinplanung für einen Lauf, Register Glasarten


                                       Das Register Glasarten richtet seinen Fokus auf die im Lauf enthaltenen Glas-
                                       arten. Es gibt Ihnen Informationen zur Dicke, der Optimierung, der zu produ-
                                       zierenden Fläche sowie der zu produzierenden Stückzahl. Wenn Sie eine
                                       Position im oberen Bereich markieren, bekommen Sie im unteren Bereich In-
                                       formationen zu der entsprechenden Gegenscheibe angezeigt. Das trifft nur für
                                       die Scheiben zu, deren Gegenscheiben im selben Lauf sind.
                                       Anhand der angezeigten Symbole können Sie sich schnell einen Überblick in
                                       Bezug auf die Art des Zuschnitts verschaffen.
                                       Die in den beiden Bereichen angezeigten Symbole haben folgende Bedeu-
                                       tung:

                                       Oberer Bereich:
                                              Automatischer Zuschnitt
                                              Handzuschnitt
                                              Handzuschnitt mit Schneidplan
                                       Bereich der Gegenscheibe:
                                              Automatischer Zuschnitt
                                              Handzuschnitt
3,00 / 01-2023




                                       Abb. F-64    Erläuterung der Feinplanungs-Symbole für einzelne Läufe




                 A+W Production Feinplanung                                                                    F-159
                 Läufe feinplanen                                                                Softwarereferenz




                                    Erläuterung der Felder im oberen Bereich
                                    Die Felder im oberen Bereich geben Ihnen Informationen zu:
                                    •   Glasart: In diesem Feld wird die Artikelnummer der Glasart angezeigt. Die
                                        Glasarten werden in den Stammdaten angelegt.
                                    •   Dicke: In diesem Feld wird die Dicke der Glasart angezeigt. Die Dicke wird
                                        in den Stammdaten angelegt.
                                    •   Optimierung: In diesem Feld wird die Optimierungsart angezeigt. Die Opti-
                                        mierungen sind im System fest hinterlegt und können nicht geändert wer-
                                        den.
                                    •   Fläche (B): In diesem Feld wird die Optimierungsfläche in m2 angezeigt.
                                    •   Stück (B): In diesem Feld wird die Stückzahl angezeigt. Ein * hinter der
                                        Stückzahl zeigt Ihnen, dass Sie für diese Optimierung Füllaufträge verwen-
                                        den können.

                                    Erläuterung der Schaltflächen

                                    Hoch Diese Schaltfläche ermöglicht Ihnen innerhalb der Optimierung die Be-
                                    stimmung der Priorität, d.h. die Reihenfolge, in der die Optimierung durchge-
                                    führt werden soll. Wenn Sie die Schaltfläche betätigen, wird der in der Liste
                                    markierte Datensatz um eine Position nach oben verschoben.

                                    Runter Diese Schaltfläche ermöglicht Ihnen innerhalb der Optimierung die
                                    Bestimmung der Priorität, d.h. die Reihenfolge, in der die Optimierung durch-
                                    geführt werden soll. Wenn Sie die Schaltfläche betätigen, wird der in der Liste
                                    markierte Datensatz um eine Position nach unten verschoben.

                                    Handzuschnitt Wenn Sie diese Schaltfläche betätigen, wird für den in der
                                    Liste markierten Datensatz der Zuschnitt von automatischem Zuschnitt auf
                                    Handzuschnitt (und umgekehrt) geändert. Das heißt, wenn der Datensatz auf
                                    automatischem Zuschnitt steht, dann wird er auf Handzuschnitt gesetzt und
                                    wenn er auf Handzuschnitt steht, wird er auf automatischen Zuschnitt gesetzt.

                                    XOPT Diese Schaltfläche erscheint, wenn die markierte Scheibe automatisch
                                    geschnitten wird. Sie erscheint nicht, wenn die markierte Scheibe im Handzu-
                                    schnitt geschnitten werden soll. Wenn Sie diese Schaltflächen betätigen, er-
                                    zwingen bzw. löschen Sie eine XOPT-Optimierung für Teile, die nicht auf
                                    Fächerwagen liegen.

                                    Schneidplan Diese Schaltfläche erscheint, wenn die markierte Scheibe im
                                    Handzuschnitt geschnitten wird. Sie erscheint nicht, wenn die markierte
                                    Scheibe im automatischen Zuschnitt geschnitten werden soll. Das bedeutet,
                                    dass, obwohl die Scheibe im Handzuschnitt geschnitten wird, eine Optimie-
                                    rung dafür gestartet wird. Für diese Optimierung steht dann ein Schneidplan
                                    zur Verfügung.
3,00 / 01-2023




                 F-160                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                   Läufe feinplanen




                                       Erläuterung der Felder im Bereich Gegenscheiben-Information
                                       Dieser Bereich enthält folgende Informationen zu der Gegenscheibe für die im
                                       oberen Bereich markierten Scheibe:
                                       •   Glasart: In diesem Feld wird die Artikelnummer der Glasart angezeigt. Die
                                           Glasarten werden in den Stammdaten angelegt.
                                       •   Dicke: In diesem Feld wird die Dicke der Glasart angezeigt. Die Dicke wird
                                           in den Stammdaten angelegt.
                                       •   Optimierung: In diesem Feld wird die Optimierungsart angezeigt. Die Opti-
                                           mierungen sind im System fest hinterlegt und können nicht geändert wer-
                                           den.
                                       •   Fläche (B): In diesem Feld wird die Optimierungsfläche in m2 angezeigt.
                                           Die Fläche wird vom System automatisch errechnet.
                                       •   Stück (B): In diesem Feld wird die zu optimierende Stückzahl angezeigt.
                                           Die Stückzahl kommt aus dem übergeordneten Auftragsbearbeitungs-Sys-
                                           tem und wird beim Daten-Import eingelesen.

                                       Erläuterung der Schaltflächen

                                       Doppel-Opti Betätigen Sie diese Schaltfläche, erzeugen Sie für die im Be-
                                       reich der Gegenscheibe markierte Position eine Doppel-Optimierung.

                                       Entfernen Diese Schaltfläche ist nur für Positionen aktiv, für die Sie eine
                                       Doppel-Optimierung erzeugt haben. Dann haben Sie mit Hilfe dieser Schalt-
                                       fläche die Möglichkeit, die erzeugte Doppel-Optimierung wieder zu entfernen.

                                       Wiederholen Diese Schaltfläche ist nur aktiv, wenn Sie an den Ergebnissen
                                       der Feinplanung Änderungen vorgenommen haben. Immer wenn Sie Ände-
                                       rungen vorgenommen haben, müssen Sie die Feinplanung wiederholen, um
                                       die Änderungen auch umzusetzen.

                                       Optimierung Wenn Sie mit der Feinplanung für einen Lauf einverstanden
                                       sind, betätigen Sie diese Schaltfläche und starten somit die Optimierung.
                                       Wenn die Optimierung fertig ist, wird automatisch das Register Ergebnisse ge-
                                       öffnet.

                                       PlanEdit Wenn die Optimierung durchlaufen wurde, können Sie sich über
                                       diese Schaltfläche den Schneidplan anzeigen lassen. Das Programm Plan
                                       Editor wird gestartet.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                   F-161
                 Läufe feinplanen                                                                    Softwarereferenz




                                    Register Bockbelegung
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Bockbelegung




                                    Abb. F-65    Feinplanung für einen Lauf, Register Bockbelegung


                                    Dieses Register liefert Ihnen einen genauen Überblick zu den für den Lauf be-
                                    nötigten Abstellplätzen. Es handelt sich hierbei um das Ergebnis der Abstell-
                                    platz-Einstellungen, die Sie im Register Produktionsreihenfolge im Orga-
                                    Dialog vorgenommen haben.
                                    Im linken Bereich werden die einzelnen Abstellplätze in einer Baumstruktur
                                    angezeigt. Wenn Sie mit der Maus auf das Pluszeichen vor dem jeweiligen
                                    Abstellplatz klicken, wird der Abstellplatz geöffnet und Sie können sehen, wel-
                                    che Abstellplatznummern verwendet werden.
                                    Die Symbole haben folgende Bedeutung:

                                    Symbol       Erläuterung

                                                 Bockbelegung

                                                 A-Böcke
                                                 Fächerwagen

                                    Tab. F-8     Erläuterung der Symbole im Register Bockbelegung
3,00 / 01-2023




                 F-162                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                     Läufe feinplanen




                                       Erläuterung der Felder

                                       Linke Liste Die linke Liste liefert Ihnen Informationen zu:
                                       • Glasart: Dieses Feld gibt Ihnen Auskunft über alle im Lauf enthaltenen
                                          Glasart/Dicken-Kombinationen. Bsp.: 1306/6,0 bedeutet, die im Lauf ent-
                                          haltene Glasart hat die Artikelnummer 1306 und eine Dicke von 6,0 mm.
                                          Die Glasarten werden in den Stammdaten angelegt.
                                       • Min. Stapel#: In diesem Feld steht die Mindestanzahl an Stapeln. Sie kön-
                                          nen diese Anzahl durch einen Doppelklick direkt editieren. Es öffnet sich
                                          der Dialog Ändern der minimalen Anzahl A-Böcken.
                                           Sollten Sie Änderungen vorgenommen haben, müssen Sie die Feinpla-
                                           nung wiederholen!
                                       •   Stapel#: In diesem Feld steht die aktuell benötigte Stapelanzahl.
                                       •   Fächerwagen#: In diesem Feld steht die aktuell benötigte Anzahl an Fä-
                                           cherwagen.
                                       Die Anzeige im rechten Bereich des Dialoges ist abhängig davon, was Sie im
                                       linken Bereich markiert haben. Haben Sie den obersten Eintrag (Bockbele-
                                       gung) markiert, erhalten Sie auf der rechten Seite einen Überblick über alle im
                                       Lauf befindlichen Glasart/Dicken-Kombinationen.
                                       Haben Sie im linken Bereich die Bedingung für die Scheiben eines A-Bocks
                                       markiert, sieht die Anzeige wie folgt aus:




                                       Abb. F-66    Feinplanung für einen Lauf, Register Bockbelegung, A-Bock


                                       Es wird Ihnen angezeigt, welche Nummer der Abstellplatz hat, in welcher Sta-
3,00 / 01-2023




                                       pel-Nummer sich die Scheiben befinden, die Tiefe sowie die Breite des Sta-
                                       pels in mm.




                 A+W Production Feinplanung                                                                     F-163
                 Läufe feinplanen                                                                 Softwarereferenz




                                    Erläuterung der Felder

                                    Abstellplatz Nr. Hier können Sie erkennen, welche Nummer der Abstellplatz
                                    hat. Der Nummernkreis der Abstellplätze kommt aus den Stammdaten.

                                    Stapel# Das Feld ist nur bei A-Böcken aktiv. Sie können in diesem Feld se-
                                    hen, in welcher Stapel-Nummer sich die Scheiben befinden.

                                    Tiefe In diesem Feld sehen Sie, wie tief der Stapel ist (in mm).

                                    Breite In diesem Feld sehen Sie, wie breit der Stapel ist (in mm).
                                    Wenn Sie im linken Bereich die Baumstruktur den Namen für einen A-Bock öff-
                                    nen (durch Anklicken des Plus-Zeichens), sehen Sie darunter die Abstellplatz-
                                    Nummer. Markieren Sie die Abstellplatz-Nummer, sieht die Anzeige wie folgt
                                    aus:




                                    Abb. F-67    Feinplanung für einen Lauf, Register Bockbelegung, A-Bock


                                    Sie erhalten Informationen darüber, wie viele Scheiben einer Glasart/Dicken-
                                    Kombination mit welcher Tiefe und Breite auf dem Abstellplatz stehen.

                                    Erläuterung der Felder

                                    Glasart Dieses Feld gibt Ihnen Auskunft über alle auf dem Abstellplatz ste-
                                    henden Glasart/Dicken-Kombinationen. Bsp.: 1306/6,0 bedeutet, die auf dem
                                    Abstellplatz stehende Glasart hat die Artikelnummer 1306 und eine Dicke von
                                    6,0 mm. Die Glasarten werden in den Stammdaten angelegt.
3,00 / 01-2023




                                    Scheiben Wie viele Scheiben dieser Glasart/Dicken-Kombination stehen auf
                                    diesem Abstellplatz.



                 F-164                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                   Läufe feinplanen




                                       Tiefe Wie tief (in mm) sind die Scheiben dieser Glasart/Dicken-Kombination
                                       zusammen auf diesem Abstellplatz.

                                       Breite Wie breit (in mm) sind die Scheiben dieser Glasart/Dicken-Kombinati-
                                       on auf diesem Abstellplatz.
                                       Haben Sie im linken Bereich den Namen für die Scheiben eines Fächerwa-
                                       gens markiert, sieht die Anzeige wie folgt aus:




                                       Abb. F-68   Feinplanung für einen Lauf, Register Bockbelegung, Fächerwagen


                                       Es wird Ihnen angezeigt, welche Nummer der Abstellplatz hat, in welcher Sta-
                                       pel-Nummer sich die Scheiben befinden, die Tiefe sowie die Breite des Sta-
                                       pels in mm.

                                       Erläuterung der Felder

                                       Abstellplatz Nr. Hier können Sie erkennen, welche Nummer der Abstellplatz
                                       hat. Der Nummernkreis der Abstellplätze kommt aus den Stammdaten.

                                       Belegte Fächer Dieses Feld zeigt an, wie viele der Fächer des Wagens be-
                                       legt sind.

                                       Anzahl Glasarten Dieses Feld zeigt an, wie viele unterschiedliche Glasarten
                                       auf dem Fächerwagen stehen.
                                       Wenn Sie im linken Bereich die Baumstruktur der Namen für einen Fächerwa-
                                       gen öffnen (durch anklicken des Plus-Zeichens), sehen Sie darunter die Ab-
                                       stellplatz-Nummer. Markieren Sie die Abstellplatz-Nummer, sieht die Anzeige
3,00 / 01-2023




                                       wie folgt aus:




                 A+W Production Feinplanung                                                                   F-165
                 Läufe feinplanen                                                                Softwarereferenz




                                    Abb. F-69    Feinplanung für einen Lauf, Register Bockbelegung, Fächerwagen


                                    Sie erhalten Informationen darüber, wie viele Scheiben einer Glasart/Dicken-
                                    Kombination auf dem Abstellplatz stehen.

                                    Erläuterung der Felder

                                    Linke Liste Die linke Liste liefert Ihnen die für den Lauf verwendeten Abstell-
                                    plätze sowie die jeweiligen Bedingungen.

                                    Rechte Liste Die rechte Liste enthält folgende Informationen:
                                    • Glasart: Dieses Feld gibt Ihnen Auskunft über alle auf dem Abstellplatz ste-
                                      henden Glasart/Dicken-Kombinationen. Bsp.: 1306/6,0 bedeutet, die auf
                                      dem Abstellplatz stehende Glasart hat die Artikelnummer 1306 und eine
                                      Dicke von 6,0 mm. Die Glasarten werden in den Stammdaten angelegt.
                                    • Dicke: Dieses Feld zeigt Ihnen die Dicke der Scheiben an. Die Dicke wird
                                      in den Stammdaten angelegt.
                                    • Scheiben: Das Feld zeigt Ihnen, wie viele Scheiben dieser Glasart/Dicken-
                                      Kombination auf dem Abstellplatz stehen.
3,00 / 01-2023




                 F-166                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                     Läufe feinplanen




                                       Register Ergebnisse
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Ergebnisse




                                       Abb. F-70    Feinplanung für einen Lauf, Register Ergebnisse


                                       Dieses Register liefert Ihnen einen Überblick zu den am Lauf beteiligten Pro-
                                       zessen (Rahmen, Iso-Linie, etc.) und zeigt, auf welchen Maschinen (Bieger-
                                       Linie, ISO-Linie, etc.) diese Prozesse mit welchen Stückzahlen ausgeführt
                                       werden. Der untere Bereich gibt Ihnen Auskunft über die Glasarten, die Di-
                                       cken, die Flächen sowie die Stückzahlen. Die Felder Platten, Verschnitt und
                                       Restplatte sind erst nach einer Optimierung gefüllt. Haben Sie noch keine Op-
                                       timierung durchgeführt, sind diese drei Felder leer.

                                       Erläuterung der Felder

                                       Rechte Liste Aus der rechten Liste können Sie folgende Informationen ent-
                                       nehmen:
                                       • Maschinen: Zeigt Ihnen, auf welcher Maschine der im linken Bereich mar-
                                          kierte Prozess ausgeführt wird.
                                       • Wert: Diese Spalte ist nur vorhanden und gefüllt, wenn Sie für Produktions-
                                          lose dem entsprechenden Lostyp eine Gruppierung zugeordnet haben
                                          (z.B. SZR). Dann steht an dieser Stelle der jeweils gültige Wert für jede Ei-
                                          genschaft/Formel.
                                       • Stück: Zeigt Ihnen, welche Stückzahl im entsprechenden Los produziert
                                          wird.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                     F-167
                 Läufe feinplanen                                                               Softwarereferenz




                                    Liste unten Aus der unteren Liste können Sie folgende Informationen ent-
                                    nehmen:
                                    • Glasart. Dieses Feld gibt Ihnen Auskunft über alle auf dem Abstellplatz ste-
                                       henden Glasart/Dicken-Kombinationen. Bsp.: 1306/6,0 bedeutet, die auf
                                       dem Abstellplatz stehende Glasart hat die Artikelnummer 1306 und eine
                                       Dicke von 6,0 mm. Die Glasarten werden in den Stammdaten angelegt.
                                    • Dicke: Dieses Feld zeigt Ihnen die Dicke der Scheiben an. Die Dicke wird
                                       in den Stammdaten angelegt.
                                    • Fläche (B): Dieses Feld zeigt Ihnen die optimierte Fläche in m2 an.
                                    • Stück (B): Dieses Feld zeigt Ihnen, wie viele Stück der Glasart optimiert
                                       werden. Die in Klammern dahinter stehenden positiven (z.B. 10) Zahlen
                                       kennzeichnen die Anzahl mit zu schneidender Füller. (10) würde bedeuten,
                                       dass 10 Füller mit geschnitten werden. Negative (z.B. -4) Zahlen kenn-
                                       zeichnen die Anzahl an Scheiben, die aus dem Lauf entfernt wurden und
                                       mit anderer Dicke geschnitten werden. (-4) würde bedeuten, dass 4 Schei-
                                       ben aus dem Lauf entfernt werden und mit einer anderen Dicke geschnit-
                                       ten werden. Es sind auch Kombinationen dieser beiden Werte möglich:
                                       (10/-4).
                                    • Platten: Dieses Feld zeigt Ihnen, wie viele Lagerplatten für die Optimierung
                                       notwendig sind. Die Lagerplatten werden in den Stammdaten angelegt.
                                    • Verschnitt: Dieses Feld zeigt Ihnen den Verschnitt der Optimierung in%.
                                    • Restplatte: Dieses Feld zeigt Ihnen die Länge der Restplatte.

                                    Erläuterung der Schaltflächen

                                    PlanEdit Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung durch-
                                    geführt haben. Betätigen Sie diese Schaltfläche, öffnet sich das Programm
                                    Plan Editor.
                                    Nähere Informationen zu dem Programm PlanEdit erhalten Sie in der Doku-
                                    mentation zu dem Programm Plan Editor.

                                    Übernehmen Diese Schaltfläche ist erst aktiv, wenn Sie eine Optimierung
                                    durchgeführt haben. Betätigen Sie diese Schaltfläche, werden die Ergebnisse
                                    der Optimierung übernommen. Möchten Sie die Ergebnisse nicht überneh-
                                    men, schließen Sie den Dialog durch Betätigen der Schaltfläche X am oberen
                                    rechten Dialogrand. Es folgt eine Sicherheitsabfrage, die Sie dann entspre-
                                    chend beantworten.
3,00 / 01-2023




                 F-168                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                     Läufe feinplanen




                                       Register Spezial
                                       Dieses Register liefert Ihnen Informationen zu vorhandenen Sonderteilen, wie
                                       z.B. Füllaufträgen, Restblätter und Bruchscheiben.
                                       Das Register ist in fünf Unterregister unterteilt:
                                       •   Register Zusammenlegen
                                       •   Register Füllaufträge
                                       •   Register Restblätter
                                       •   Register Bruchscheiben
                                       •   Register Eilscheiben
                                       •   Register Glasdicken

                                       Register Zusammenlegen
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Spezial > Register Zusammenlegen




                                       Abb. F-71    Feinplanung für einen Lauf, Register Spezial, Register Zusammenlegen


                                       Das Register Zusammenlegen bezieht sich auf das Zusammenlegen von Mo-
                                       dellen. Es ist möglich, Modelle in einer Optimierungsposition zusammen zu le-
                                       gen, auch wenn sie zu verschiedenen Scheiben gehören. Voraussetzung
                                       dafür ist jedoch, dass die Modelle einer gemeinsamen Pseudoserie angehö-
                                       ren. Durch einen Doppelklick auf das Modell-Symbol kann das Verhalten (zu-
                                       sammen legen ja/nein) direkt in diesem Register editiert werden.
3,00 / 01-2023




                                           Standard-Verhalten festlegen
                                           Ob Modelle standardmäßig zusammen gelegt werden oder nicht, stellen
                                           Sie in A+W Production in den Stammdaten wie folgt ein: Stammdaten > Pa-
                                           rameter > Modul Feinplanung > Spezial > Zusammenlegen.


                 A+W Production Feinplanung                                                                      F-169
                 Läufe feinplanen                                                               Softwarereferenz




                                       diese Funktionalität bedingt den A+W Standard-Modellkatalog. Für be-
                                       stimmte Modelle ist es dann möglich diese zusammenzulegen (bspw. 2
                                       Dreiecke werden zu einem Rechteck zusammengelegt). Das funktioniert
                                       nur für ein paar wenige Modelle - nicht für alle.

                                       A+W bietet neben dieser einfachen Form der Modellzusammenlegung
                                       noch ein erweitertes Modul an, welches man erwerben kann - A+W Shape
                                       Optimizer. Damit ist es möglich 2 Modelle gleicher Form auf ein umschrei-
                                       bendes Rechteck zusammenzulegen und damit die Optimierungsergeb-
                                       nisse noch einmal deutlich zu verbessern.

                                    Die vor der Modell-Nummer stehenden Symbole haben folgende Bedeutung:

                                    Symbol      Erläuterung

                                                Die Modelle werden nicht zusammen gelegt, könnten aber
                                                zusammen gelegt werden.

                                                Die Modelle werden zusammen gelegt.

                                    Tab. F-9    Erläuterung der Symbole im Register Zusammenlegen

                                    Felder

                                    Mod. In diesem Feld können Sie sehen, um welche Modell-Nummer es sich
                                    handelt. Die Modell-Nummer kommt aus dem übergeordneten ERP-System
                                    und wird beim Daten-Import eingelesen.

                                    BXH In diesem Feld werden die Maße des umschreibenden Rechtecks ange-
                                    zeigt.

                                    Menge In diesem Feld wird angezeigt, wie viele Stück des entsprechenden
                                    Modells in der Feinplanung für den Lauf enthalten sind.

                                    Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, in dem die Mo-
                                    dell-Scheiben enthalten sind. Die Auftrags-Nummer kommt aus dem überge-
                                    ordneten ERP-System und wird beim Daten-Import eingelesen.

                                    Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                    in dem die Modell-Scheiben enthalten sind.
3,00 / 01-2023




                 F-170                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                       Läufe feinplanen




                                       Register Füllaufträge
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Spezial > Register Füllaufträge




                                       Abb. F-72   Feinplanung für einen Lauf, Register Spezial, Register Füllaufträge


                                       In diesem Register werden die für die entsprechende Glasart zur Verfügung
                                       stehenden Füllaufträge angezeigt.

                                          Füllaufträge anzeigen
                                          Damit Füllaufträge verwendet und angezeigt werden, müssen Sie die ent-
                                          sprechende Checkbox im Orga-Dialog aktivieren. Ist die Checkbox nicht
                                          aktiv, erscheint im Tabellenkopf der Hinweis Füllaufträge werden nicht ver-
                                          wendet!

                                       Die vor dem Termin stehenden Symbole haben folgende Bedeutung:

                                       Symbol      Erläuterung

                                                   Die Optimierung entscheidet, ob die Scheibe produziert wird.

                                                   Die Scheibe wird auf jeden Fall in dem Lauf produziert.

                                                   Die Scheibe wird in diesem Lauf nicht geschnitten.

                                                   Der Auftrag ist bereits feingeplant. Er wurde entweder noch nicht
                                                   abgeschlossen oder die Feinplanung ist nicht erfolgreich
                                                   abgeschlossen worden.
3,00 / 01-2023




                                       Tab. F-10   Erläuterung der Symbole im Register Füllaufträge




                 A+W Production Feinplanung                                                                        F-171
                 Läufe feinplanen                                                              Softwarereferenz




                                    Wenn Sie einen Datensatz in der Liste markieren, haben Sie über das Kon-
                                    text-Menü die Möglichkeit die Attribute zu ändern.

                                    Erläuterung der Felder

                                    Termin In diesem Feld wird der vom System errechnete Produktionstermin
                                    angezeigt.

                                    Menge In diesem Feld wird angezeigt, um wie viele Stück es sich handelt. Bei
                                    der in Klammern stehenden Menge handelt es sich um die Auftragsmenge.
                                    Die vor der Klammer stehende Menge ist die Menge, die in diesem Lauf pro-
                                    duziert werden darf.

                                    Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, in dem die Füll-
                                    aufträge enthalten sind.

                                    Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                    in dem die Füllaufträge enthalten sind. Die Positions-Nummer kommt aus dem
                                    übergeordneten ERP-System und wird beim Daten-Import eingelesen.

                                    Einzeln ändern/Gemeinsam ändern Mit einem Doppelklick auf den Tabel-
                                    lenkopf können Sie zwischen Einzeln ändern und Gemeinsam ändern wech-
                                    seln. Je nach Modus (einzeln oder gemeinsam) wird stets die komplette
                                    Position als Füller verwendet oder nicht. Das Symbol davor ändert sich eben-
                                    falls entweder einzeln oder für alle Positionsscheiben gleichzeitig.

                                    Priorität In diesem Feld wird die Nummer der Priorität angezeigt. Folgende
                                    Werte sind möglich:
                                    • 3: Scheiben werden in der Optimierung mit verplant um den Gesamtver-
                                       schnitt zu verbessern. Es können mehr Lagerplatten verwendet werden.
                                    • 4: Scheiben werden in der Optimierung mit verplant um Gesamtverschnitt
                                       zu verbessern. Es werden nicht mehr Lagerplatten verwendet.
3,00 / 01-2023




                 F-172                                                            A+W Production Feinplanung
                 Softwarereferenz                                                                      Läufe feinplanen




                                       Register Restblätter
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Spezial > Register Restblätter




                                       Abb. F-73   Feinplanung für einen Lauf, Register Spezial, Register Restblätter


                                       In diesem Register werden die für die entsprechende Glasart zur Verfügung
                                       stehenden Restblätter angezeigt.

                                          Restblätter anzeigen
                                          Damit Restblätter verwendet und angezeigt werden, müssen Sie die ent-
                                          sprechende Checkbox im Orga-Dialog aktivieren. Ist die Checkbox nicht
                                          aktiv, erscheint im Tabellenkopf der Hinweis Restblätter werden nicht ver-
                                          wendet!

                                       Die vor dem Termin stehenden Symbole haben folgende Bedeutung:

                                       Symbol      Erläuterung

                                                   Die Teile dürfen immer verwendet
                                                   werden.

                                                   Die Teile dürfen momentan nicht
                                                   verwendet werden.

                                       Tab. F-11   Erläuterung der Symbole im Register Füllaufträge

                                       Wenn Sie einen Datensatz in der Liste markieren, haben Sie über das Kon-
3,00 / 01-2023




                                       text-Menü die Möglichkeit die Attribute zu ändern.




                 A+W Production Feinplanung                                                                        F-173
                 Läufe feinplanen                                                                 Softwarereferenz




                                    Erläuterung der Felder

                                    Termin In diesem Feld wird der Produktionstermin angezeigt.

                                    Menge In diesem Feld wird angezeigt, um wie viele Stück es sich handelt.

                                    Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, in dem die Füll-
                                    aufträge enthalten sind. Die Auftrags-Nummer kommt aus dem übergeordne-
                                    ten ERP-System und wird beim Daten-Import eingelesen.

                                    Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                    in dem die Füllaufträge enthalten sind.

                                    Register Bruchscheiben
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Spezial > Register Bruchscheiben




                                    Abb. F-74   Feinplanung für einen Lauf, Register Spezial, Register Bruchscheiben


                                    In diesem Register werden die für die entsprechende Glasart zur Verfügung
                                    stehenden Bruchscheiben angezeigt.

                                       Bruchscheiben anzeigen
                                       Damit Bruchscheiben verwendet und angezeigt werden, müssen Sie die
                                       entsprechende Checkbox im Orga-Dialog aktivieren. Ist die Checkbox
                                       nicht aktiv, erscheint im Tabellenkopf der Hinweis Bruchscheiben werden
                                       nicht verwendet!
3,00 / 01-2023




                 F-174                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                      Läufe feinplanen




                                       Die vor dem Termin stehenden Symbole haben folgende Bedeutung:

                                       Symbol      Erläuterung

                                                   Die Teile dürfen immer verwendet
                                                   werden.

                                                   Die Teile dürfen momentan nicht
                                                   verwendet werden.

                                       Tab. F-12   Erläuterung der Symbole im Register Bruchscheiben

                                       Wenn Sie einen Datensatz in der Liste markieren, haben Sie über das Kon-
                                       text-Menü die Möglichkeit die Attribute zu ändern.

                                       Erläuterung der Felder

                                       Termin In diesem Feld wird der vom System errechnete Produktionstermin
                                       angezeigt.

                                       Menge In diesem Feld wird angezeigt, um wie viele Stück es sich handelt.

                                       Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, in dem die Füll-
                                       aufträge enthalten sind. Die Auftrags-Nummer kommt aus dem übergeordne-
                                       ten ERP-System und wird beim Daten-Import eingelesen.

                                       Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                       in dem die Füllaufträge enthalten sind.

                                       Letztes Feld Das Feld enthält eine Auflistung von Glasart und Dicke sowie
                                       der Maschinen, auf denen die Bruchscheibe gefertigt werden kann.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                     F-175
                 Läufe feinplanen                                                                    Softwarereferenz




                                    Register Eilscheiben
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Spezial > Register Eilscheiben




                                    Abb. F-75   Feinplanung für einen Lauf, Register Spezial, Register Eilscheiben


                                    In diesem Register werden die für die entsprechende Glasart zur Verfügung
                                    stehenden Eilscheiben angezeigt. Es können nur die Eilscheiben angezeigt
                                    werden, die zuvor über den Dialog Eilscheiben-Eingabe erfasst wurden.

                                       Eilscheiben anzeigen
                                       Damit Eilscheiben verwendet und angezeigt werden, müssen Sie die ent-
                                       sprechende Checkbox im Orga-Dialog aktivieren. Ist die Checkbox nicht
                                       aktiv, erscheint im Tabellenkopf der Hinweis Eilscheiben werden nicht ver-
                                       wendet!

                                    Die vor dem Termin stehenden Symbole haben folgende Bedeutung:

                                    Symbol      Erläuterung

                                                Die Eilscheibe wird auf jeden Fall in dem Lauf produziert.

                                                Die Eilscheibe wird in diesem Lauf nicht geschnitten.

                                    Tab. F-13   Erläuterung der Symbole im Register Eilscheiben

                                    Wenn Sie einen Datensatz in der Liste markieren, haben Sie über das Kon-
                                    text-Menü die Möglichkeit die Attribute zu ändern.
3,00 / 01-2023




                 F-176                                                                A+W Production Feinplanung
                 Softwarereferenz                                                                     Läufe feinplanen




                                       Erläuterung der Felder

                                       Termin In diesem Feld wird der vom System errechnete Produktionstermin
                                       angezeigt.

                                       Menge In diesem Feld wird angezeigt, um wie viele Stück es sich handelt.

                                       Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, in dem die Eil-
                                       scheiben enthalten sind. Eine -1 bedeutet, dass die Eilscheibe manuell über
                                       den Dialog Eilscheiben-Eingabe erfasst wurde.

                                       Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                       in dem die Eilscheiben enthalten sind.

                                       Letztes Feld Das Feld enthält eine Auflistung von Glasart und Dicke sowie
                                       der Maschinen, auf denen die Bruchscheibe gefertigt werden kann.

                                       Register Glasdicken
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Spezial > Register Glasdicken




                                       Abb. F-76   Feinplanung für einen Lauf, Register Spezial, Register Glasdicken


                                       In diesem Dialog haben Sie die Möglichkeit, für Scheiben, die in ein ISO ein-
                                       gebaut werden, die Optimierungs-(bzw. Zuschnitt-)Dicke zu ändern. Dadurch
                                       wird der Verschnitt reduziert. Welche Scheiben mit der größeren Dicke ge-
                                       schnitten werden dürfen, lässt sich über eine Zuweisung hinterlegen. Diese
                                       Zuweisung bestimmt dann die maximale Änderung. Im Register Glasdicken
                                       bestimmen Sie dann manuell welche Scheiben davon tatsächlich mit geänder-
                                       ter Dicke geschnitten werden.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                      F-177
                 Läufe feinplanen                                                                   Softwarereferenz




                                    Das Register Glasdicken unterliegt folgenden Restriktionen:
                                    •   Es kann die Dicke nur für Scheiben geändert werden, wenn sie ins ISO ein-
                                        gebaut werden und das jeweilige ISO kein Unterteil enthält, das selber
                                        mehr als ein direktes Unterteil enthält.
                                    •   Das Zuschnittsteil und das ISO befinden sich im selben Lauf.

                                        Änderung der Glasdicke
                                        Das Register Glasdicken ist nur dann verfügbar, wenn es eine Zuweisung
                                        (Formeleditor) für die Eigenschaft Dickendifferenz gibt.

                                    Die vor dem Auftrag stehenden Symbole haben folgende Bedeutung:

                                    Symbol       Erläuterung

                                                 Die Scheibe wird mit einer größeren Dicke geschnitten.

                                                 Die Scheibe wird nicht mit einer größeren Dicke geschnitten.

                                    Tab. F-14    Erläuterung der Symbole im Register Glasdicken

                                    Wenn Sie einen Datensatz in der Liste markieren, haben Sie über das Kon-
                                    text-Menü die Möglichkeit, die Attribute zu ändern.

                                    Erläuterung der Felder

                                    Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, die Scheiben
                                    enthält, die mit einer größeren Dicke geschnitten werden können

                                    Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                    in dem die Scheiben enthalten sind.

                                    Menge In diesem Feld wird angezeigt, um wie viele Stück es sich handelt.

                                    Feld ohne Namen In diesem Feld wird die momentane Dicke sowie der
                                    Schneidtisch angezeigt, auf dem die Scheibe geschnitten wird.

                                    Neue Dicke In diesem Feld wird die neue Dicke angezeigt, mit der die Schei-
                                    be geschnitten wird.
3,00 / 01-2023




                 F-178                                                                A+W Production Feinplanung
                 Softwarereferenz                                                                     Läufe feinplanen




                                       Register Freie Optimierung
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Freie Optimierung




                                       Abb. F-77   Feinplanung für einen Lauf, Register Freie Optimierung


                                       Dieses Register zeigt Ihnen, mit welcher Optimierungsart die einzelnen Glas-
                                       arten optimiert werden. Bei Glasarten, die auf Sequenz optimiert wurden,
                                       kann durch einen Doppelklick auf die jeweilige Position die Optimierung von
                                       Sequenz auf Freie Optimierung geändert werden. Vor dem XOPTS erscheint
                                       dann ein [X]. Die Optimierung kann nur bei Sequenz in eine Freie Optimierung
                                       geändert werden, nicht bei Handzuschnitt.
                                       Im unteren Bereich des Dialogs können Sie die Optimierung auch für einzelne
                                       Böcke anstelle für die Glasarten umschalten.

                                       Erläuterung der Felder

                                       Glasart Dieses Feld zeigt Ihnen die Artikel-Nummer der Glasart an. Die Glas-
                                       art kommt aus den Stammdaten.

                                       Dicke Dieses Feld zeigt Ihnen die Dicke der Scheiben an. Die Dicke kommt
                                       aus den Stammdaten.

                                       Optimierung Dieses Feld zeigt Ihnen, mit welchem Optimierungsmodus die
                                       Feinplanung durchgeführt wurde.
3,00 / 01-2023




                                       Fläche (B) Dieses Feld zeigt Ihnen die optimierte Fläche in m2 an.

                                       Stück (B) Dieses Feld zeigt Ihnen, wie viele Stück der Glasart optimiert wer-
                                       den. Ein * hinter der Stückzahl bedeutet, dass Füller enthalten sind.


                 A+W Production Feinplanung                                                                    F-179
                 Läufe feinplanen                                                                 Softwarereferenz




                                    Bereich unten

                                    Bock Zeigt Ihnen die Abstellplatz-Nummer an, auf dem die Scheiben stehen.

                                    Stapel Zeigt Ihnen an, in welchem Stapel sich die Scheiben befinden.

                                    Menge In diesem Feld wird Ihnen angezeigt, wie viele Scheiben sich in dem
                                    Stapel befinden.

                                    Breite Dieses Feld zeigt Ihnen die Breite des Stapels in mm an.


                                    Register Teilmengen
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Teilmengen




                                    Abb. F-78   Feinplanung für einen Lauf, Register Teilmengen


                                    In diesem Register haben Sie die Möglichkeit, Teilmengen von Scheiben aus
                                    der Optimierung herauszunehmen. Damit können Sie z.B. bei schlechtem
                                    Verschnitt gezielt einzelne Scheiben entweder in den Handzuschnitt schieben
                                    oder aber in einem späteren Lauf nachoptimieren lassen. Der Dialog ist in
                                    zwei Bereiche unterteilt. Der obere Bereich gibt Ihnen einen Überblick zu den
                                    Glasarten, die in diesem Lauf optimiert werden sollen. Markieren Sie eine
                                    Glasart, zeigt Ihnen der untere Bereich die entsprechenden Auftragsinforma-
                                    tionen.
3,00 / 01-2023




                                       Teilmengen
                                       Das Register Teilmengen ist nur dann verfügbar, wenn es in den Parame-
                                       tereinstellungen aktiviert wurde.



                 F-180                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                  Läufe feinplanen




                                       Erläuterung der Felder im oberen Bereich

                                       Glasart Dieses Feld gibt Ihnen Auskunft über die Glasart/Dicken-Kombinati-
                                       onen. Bsp.: 1306/6,0 bedeutet, dass es sich um die Glasart mit der Artikel-
                                       nummer 1306 und einer Dicke von 6,0 mm handelt. Die Glasarten werden in
                                       den Stammdaten angelegt.

                                       Dicke Dieses Feld zeigt Ihnen die Dicke der Scheiben an. Die Dicke wird in
                                       den Stammdaten angelegt.

                                       Fläche (B) Dieses Feld zeigt Ihnen die optimierte Fläche in m2 an.

                                       Stück (B) Dieses Feld zeigt Ihnen, wie viele Stück der Glasart optimiert wer-
                                       den. Die in Klammern dahinter stehenden positiven (z.B. 10) Zahlen kenn-
                                       zeichnen die Anzahl mit zu schneidender Füller. (10) würde bedeuten, dass
                                       10 Füller mit geschnitten werden. Negative (z.B. -4) Zahlen kennzeichnen die
                                       Anzahl an Scheiben, die aus dem Lauf entfernt wurden und mit anderer Dicke
                                       geschnitten werden. (-4) würde bedeuten, dass 4 Scheiben aus dem Lauf ent-
                                       fernt werden und mit einer anderen Dicke geschnitten werden. Es sind auch
                                       Kombinationen dieser beiden Werte möglich: (10/-4).

                                       Platten Dieses Feld zeigt Ihnen, wie viele Lagerplatten für die Optimierung
                                       notwendig sind. Die Lagerplatten werden in den Stammdaten angelegt.

                                       Verschnitt Dieses Feld zeigt Ihnen den Verschnitt der Optimierung in %.

                                       Restplatte Dieses Feld zeigt Ihnen die Länge der Restplatte.

                                       Erläuterung der Felder im unteren Bereich

                                       Auftrag In diesem Feld wird die Auftrags-Nummer angezeigt, die die Glasart
                                       enthält.

                                       Position In diesem Feld wird die Positions-Nummer des Auftrags angezeigt,
                                       die die Glasart enthält.

                                       Bock In diesem Feld wird die Abstellplatz-Nummer angezeigt, auf dem die
                                       Position steht.

                                       Feld ohne Bezeichnung In diesem Feld werden die Abmessungen der
                                       Scheibe angezeigt.

                                       Menge In diesem Feld wird angezeigt, um wie viele Stück es sich handelt.

                                       Teilmenge In diesem Feld wird Ihnen die Stückzahl der Teilmenge angezeigt.
                                       Steht in dem Feld eine 0, sind für diese Position keine Teilmengen angelegt.
                                       Zum Anlegen einer Teilmenge öffnen Sie im unteren Bereich des Dialogs die
                                       Auftrags-Nummer mit einem Doppelklick. Es öffnet sich der Eingabedialog
                                       Teilmenge, in dem Sie die gewünschte Teilmengen-Stückzahl eingeben.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                  F-181
                 Läufe feinplanen                                                               Softwarereferenz




                                    Register Orga
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Orga




                                    Abb. F-79   Feinplanung für einen Lauf, Register Orga


                                    Dieses Register liefert Ihnen einen genauen Überblick zu den in der Feinpla-
                                    nung verwendeten Orga-Einstellungen für den Lauf. Sie haben hier die Mög-
                                    lichkeit, andere Einstellungen zu verwenden. Einstellungen sollten jedoch nur
                                    mit äußerster Vorsicht geändert werden.

                                    Erläuterung der Felder

                                    Verarbeitungsreihenfolge Die Kombobox zeigt Ihnen die gewählte Verar-
                                    beitungsreihenfolge an.

                                    Master-Orga Die Kombobox zeigt Ihnen die gewählte Master-Orga an.

                                    Orgas Dieser Bereich zeigt Ihnen alle definierten Orgas.

                                    Orga-Gruppen Dieser Bereich zeigt Ihnen alle definierten Orga-Gruppen.

                                    Gruppen sortieren Die Checkbox ist in Zusammenhang mit dem Feld Orga-
                                    Gruppen zu sehen und steuert, ob eine Sortierung der dort gewählten Gruppe
                                    erfolgen soll.
                                     Es erfolgt eine Sortierung der Gruppen.
3,00 / 01-2023




                                     Es erfolgt keine Sortierung der Gruppen.
                                    Die beiden darunter liegenden Komboboxen stehen in Zusammenhang mit
                                    der Checkbox Gruppen sortieren. Ist die Checkbox aktiviert, wählen Sie aus



                 F-182                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                 Läufe feinplanen




                                       der oberen Kombobox die gewünschte Gruppierung für die Gruppe und aus
                                       der unteren Kombobox die eventuell gewünschte Sortierung.

                                       Bildung der Gruppen Die Kombobox zeigt Ihnen die in der Orga-Gruppe ge-
                                       wählte Bildung der Gruppen.

                                       Sortierung in den Gruppen Die Kombobox zeigt Ihnen die in der Orga-
                                       Gruppe gewählte Sortierung in den Gruppen.

                                       Abstellplätze Der Bereich der Abstellplätze zeigt Ihnen die für den Lauf in
                                       Frage kommenden Abstellplätze. Die Werte kommen aus dem Dialog Einstel-
                                       lungen-Abstellplatz.

                                       deaktivieren Wenn Sie diese Schaltfläche betätigen, deaktivieren Sie den im
                                       Bereich Abstellplätze markierten Abstellplatz. Er steht der Feinplanung dann
                                       nicht mehr zur Verfügung und wird mit *** gekennzeichnet. Zum aktivieren des
                                       Abstellplatzes betätigen Sie wieder die Schaltfläche deaktivieren.

                                       Abstellmodus In dem Bereich können Sie anhand der gesetzten Radiotaste
                                       erkennen, welcher Abstellmodus für die Feinplanung gewählt wurde. Der Wert
                                       kommt aus dem Dialog Einstellungen-Abstellplatz.

                                       Abstellmodus Gruppen Dieser Bereich zeigt Ihnen den Abstellmodus, den
                                       Sie für Gruppen gewählt haben. Der Wert kommt aus dem Dialog Einstellun-
                                       gen-Abstellplatz.

                                       Gruppen sortieren Die Kombobox ist in Zusammenhang mit dem Feld Ab-
                                       stellmodus Gruppen zu sehen und steuert, wie die Sortierung der dort gewähl-
                                       ten Gruppe erfolgen soll.
                                        Es erfolgt eine Sortierung der Gruppen.
                                        Es erfolgt keine Sortierung der Gruppen.
                                       Die beiden darunter liegenden Komboboxen stehen in Zusammenhang mit
                                       der Checkbox Gruppen sortieren. Ist die Checkbox aktiviert, wählen Sie aus
                                       der oberen Kombobox die gewünschte Gruppierung für die Gruppe und aus
                                       der unteren Kombobox die eventuell gewünschte Sortierung.

                                       Max. Anzahl Gruppen In diesem Feld können Sie erkennen, wie viele Grup-
                                       pen maximal auf dem Abstellplatz stehen dürfen. Der Wert kommt aus dem
                                       Dialog Einstellungen-Abstellplatz.

                                       Erläuterung der Schaltflächen

                                       Speichern Diese Schaltfläche ist nur aktiv, wenn Sie im Register Orga an den
                                       Einstellungen Änderungen vorgenommen haben. Sollen diese Änderungen
                                       dann übernommen werden, müssen Sie die Schaltfläche Übernehmen betäti-
                                       gen. Dann erst werden die Änderungen übernommen.

                                       Wiederholen Wenn Sie Änderungen vorgenommen haben, können Sie da-
                                       mit die Feinplanung neu berechnen lassen so dass die Auswirkungen der Än-
3,00 / 01-2023




                                       derungen bspw. an der Abstellplatzbelegung auch zu sehen sind. Erst danach
                                       sollten Sie die Schaltfläche [Speichern] betätigen.



                 A+W Production Feinplanung                                                                 F-183
                 Läufe feinplanen                                                                    Softwarereferenz




                                    Register Orga-Optionen
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Orga-Optionen




                                    Abb. F-80   Feinplanung für einen Lauf, Register Orga-Optionen


                                    Dieses Register gibt Ihnen einen Überblick zu der Orga, mit der der Lauf
                                    durchgeführt wurde.

                                    Erläuterung der Felder im Bereich Master-Orga

                                    XOPT zusammen abstellen Wenn aus der Feinplanung gewisse Scheiben
                                    heraus genommen und mit XOPT optimiert werden, steuert das Feld, wie die-
                                    se Scheiben abgestellt werden. Der Wert kommt aus dem Dialog Master-Or-
                                    ga.
3,00 / 01-2023




                 F-184                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                 Läufe feinplanen




                                       Felder im Bereich Orga

                                       Linker Bereich Im linken Bereich sehen Sie, welche Orga für den Lauf ver-
                                       wendet wurde. Der Wert kommt aus dem Dialog Orga.

                                       Abstellmodus In dem Bereich können Sie anhand der gesetzten Radiotaste
                                       erkennen, welcher Abstellmodus für die Feinplanung gewählt wurde. Der Wert
                                       kommt aus dem Dialog Einstellungen-Abstellplatz.
                                       Das Feld Abstellmodus und das rechts daneben liegende Feld stehen in Zu-
                                       sammenhang. Die Grafik im rechten Feld ist abhängig von der im Feld Abstell-
                                       modus gewählten Eigenschaft. Sie hilft Ihnen, den gewählte Eigenschaft
                                       optisch zu veranschaulichen.

                                       Maximale Belegung von A-Böcken Der in diesem Feld stehende Wert gibt
                                       an, mit wie viel Prozent die Abstellfläche des A-Bocks belegt sein kann.

                                       Keine Teilung von Gruppen, falls belegt mit Der in diesem Feld stehende
                                       Wert gibt in an, ab wann nachfolgende Gruppen nicht mehr geteilt werden. Der
                                       Wert kommt aus dem Dialog Orga.

                                       Keine Teilung von Positionen, falls belegt mit Der in diesem Feld stehen-
                                       de Wert gibt an, ab wann nachfolgende Positionen nicht mehr geteilt werden.
                                       Der Wert kommt aus dem Dialog Orga.

                                       Erläuterung der Schaltflächen

                                       Speichern Diese Schaltfläche ist nur aktiv, wenn Sie im Register Orga-Opti-
                                       onen an den Einstellungen Änderungen vorgenommen haben. Sollen diese
                                       Änderungen dann übernommen werden, müssen Sie die Schaltfläche [Über-
                                       nehmen] betätigen. Dann erst werden die Änderungen übernommen.

                                       Wiederholen Wenn Sie Änderungen vorgenommen haben, können Sie da-
                                       mit die Feinplanung neu berechnen lassen so dass die Auswirkungen der Än-
                                       derungen bspw. an der Abstellplatzbelegung auch zu sehen sind. Erst danach
                                       sollten Sie die Schaltfläche [Speichern] betätigen.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                 F-185
                 Läufe feinplanen                                                               Softwarereferenz




                                    Register Optionen
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Optionen




                                    Abb. F-81   Feinplanung für einen Lauf, Register Optionen


                                    Dieses Register enthält reine Optimierungs-Optionen und dient dazu, die Op-
                                    timierungsergebnisse zu verbessern.

                                    Erläuterung der Felder

                                    Glasart Dieses Feld zeigt Ihnen die Artikel-Nummer der Glasart an. Die Glas-
                                    art kommt aus den Stammdaten.

                                    Dicke Dieses Feld zeigt Ihnen die Dicke der Scheiben an. Die Dicke kommt
                                    aus den Stammdaten.

                                    Tischzuordnung Listet die für die entsprechende Glasart in Frage kommen-
                                    den Schneidtische.

                                    Paar Listet den prozentualen Anteil der Pärchen für diese Optimierung.

                                    Pärchen-Optimierung Durch das Aktivieren der Checkbox wird erreicht,
                                    dass, falls möglich, Freie Optimierungen automatisch als Pärchen-Opti-
                                    mierungen laufen.

                                    A+W Shape Optimizer Arbeiten Sie in Ihrem Hause mit dem A+W Shape
3,00 / 01-2023




                                    Optimizer, müssen Sie diese Checkbox aktivieren.




                 F-186                                                              A+W Production Feinplanung
                 Softwarereferenz                                                                   Läufe feinplanen




                                       Laufzeitfaktor Der Laufzeitfaktor bestimmt, wie viele Optimierungsläufe
                                       nach zwei verschiedenen Methoden gerechnet werden sollen. Mögliche Wer-
                                       te: 1 bis 9. Der Laufzeitfaktor sollte immer auf 9 eingestellt sein. Es werden
                                       dann jeweils 9 Optimierungsläufe nach zwei verschiedenen Methoden ge-
                                       rechnet und automatisch das beste Ergebnis ausgewählt. Haben Sie 9 einge-
                                       stellt, dauert der Rechenvorgang selbstverständlich länger als wenn Sie 2
                                       eingestellt hätten. Das Optimierungsergebnis wird mit hoher Wahrscheinlich-
                                       keit aber wesentlich besser sein.

                                       Schneidmodus Die gesetzte Radiotaste zeigt Ihnen, mit welchem Schneid-
                                       modus die Feinplanung durchlaufen wurde. Der Wert kommt aus dem Dialog
                                       Master-Orga.
                                       Das Feld legt den Schneidmodus für die XOPT(S)-Optimierungen fest. Die ge-
                                       setzte Radiotaste zeigt Ihnen, mit welchem Schneidmodus die Feinplanung
                                       durchlaufen wurde. Die Auswahl des richtigen Schneidmodus richtet sich
                                       nach dem Schneidtisch und den betrieblichen Anforderungen. Generell gilt,
                                       dass mit Schneidmodus 1 die besten und mit Schneidmodus 4 geringfügig
                                       schlechtere Verschnittergebnisse entstehen. Diese höheren Materialverluste
                                       lassen sich unter Umständen durch schnelleres Brechen und Abräumen (auf-
                                       grund des einfacheren Schneidmodus) kompensieren. Der Schneidmodus be-
                                       stimmt die Lage der Scheiben innerhalb einer Travere zwischen zwei
                                       benachbarten Y- Schnitten. Mögliche Werte:
                                       1: Zwischen zwei Y-Schnitten dürfen Scheiben verschiedener Breite und Höhe
                                       nebeneinander liegen. Es können also auch W - Schnitte vorkommen.
                                       2: Zwischen zwei Y-Schnitten dürfen nur Scheiben mit unterschiedlicher Breite
                                       aber gleicher Höhe nebeneinander liegen.
                                       3: Zwischen zwei Y-Schnitten dürfen nur Scheiben der gleichen Position ne-
                                       beneinander liegen.
                                       4: Zwischen zwei Y-Schnitten dürfen höchstens zwei Scheiben der gleichen
                                       Position nebeneinander liegen.
                                       5-7: Spezialmodus für einen Coopmes-Tisch. Dieser Modus ist identisch mit
                                       Modus 2-4. Bei Z- Schnitten: bis zum Plattenrand durchgezogene Z-Schnitte
                                       zerschneiden keine Scheiben.

                                       Ränder Die Felder Rand links, Rand rechts, Rand oben und Rand unten zei-
                                       gen Ihnen die für den entsprechenden Glasartikel erfassten Bruchränder. Die
                                       grau unterlegten Felder beziehen sich auf die aus den Glasartikel-Stammda-
                                       ten gezogenen Werte. In den weiß unterlegten Feldern können Sie diesen
                                       Wert überschreiben. Es handelt sich dabei um ein temporäres Ändern der
                                       Bruchrändern für das jeweilige Zuschnittlos.

                                       Max. Travere Dieser Wert zeigt Ihnen die maximale Traverenbreite. Das grau
                                       unterlegte Feld bezieht sich auf den aus den Glasartikel-Stammdaten gezoge-
                                       nen Wert. In dem weiß unterlegten Feld können Sie diesen Wert überschrei-
                                       ben. Es handelt sich dabei um ein temporäres Ändern der Traverenbreite für
                                       das jeweilige Zuschnittlos.

                                       Z-Kosten Dieser Wert zeigt Ihnen die Kosten pro Z-Schnitt. Das grau unter-
                                       legte Feld bezieht sich auf den aus den Glasartikel-Stammdaten gezogenen
3,00 / 01-2023




                                       Wert. In dem weiß unterlegten Feld können Sie diesen Wert überschreiben.
                                       Es handelt sich dabei um ein temporäres Ändern der Kosten für das jeweilige
                                       Zuschnittlos.


                 A+W Production Feinplanung                                                                   F-187
                 Läufe feinplanen                                                               Softwarereferenz




                                    Register Auswahl Lagermaß
                                    Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                    gister Auswahl Lagermaß




                                    Abb. F-82   Feinplanung für einen Lauf, Register Auswahl Lagermaß


                                    Dieses Register liefert Ihnen einen Überblick zu den im Lauf verwendeten La-
                                    germaßen.

                                    Erläuterung der Felder

                                    Tischzuordnung Listet die für die entsprechende Glasart in Frage kommen-
                                    den Schneidtische.

                                    Glasart Dieses Feld zeigt Ihnen die Artikel-Nummer der Glasart an. Die Glas-
                                    art kommt aus den Stammdaten.

                                    Glasdicke Dieses Feld zeigt Ihnen die Dicke der Scheiben an. Die Dicke
                                    kommt aus den Stammdaten.

                                    Breite x Höhe Zeigt Ihnen die Breite und die Höhe des Lagermaßes in mm.
                                    Der Wert kommt aus den Stammdaten.

                                    Anzahl Zeigt Ihnen die Anzahl der vorhandenen Lagermaße. 9999 steht für
                                    unendlich viele. Durch einen Doppelklick auf das Feld, können Sie die Anzahl
                                    der Lagermaße ändern.
3,00 / 01-2023




                                    Anzahl ändern Wenn Sie diese Schaltfläche betätigen, öffnet sich der Dialog
                                    Anzahl der Lagerplatten. In diesem Dialog können Sie dann die Anzahl der La-
                                    gerplatten, die zur Verfügung stehen, ändern.


                 F-188                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                 Läufe feinplanen




                                       Erläuterung der Felder im Bereich Restplattenverwertung

                                       Breite Sollten Sie eine Restplatte aus einer früheren Optimierung zur Verfü-
                                       gung haben, die Sie für diesen Lauf verwenden können, geben Sie in diesem
                                       Feld die Breite der Restplatte ein.

                                       Höhe Sollten Sie eine Restplatte aus einer früheren Optimierung zur Verfü-
                                       gung haben, die Sie für diesen Lauf verwenden können, geben Sie in diesem
                                       Feld die Höhe der Restplatte ein.


                                       Ändern der minimalen Anzahl A-Böcke
                                       Anzeige > Lauf-Anzeige > Lauf markieren > Kontextmenü Feinplanung > Re-
                                       gister Bockbelegung > im linken Fenster Bockbelegung markieren > im rech-
                                       ten Fenster Doppelklick auf die Glasart, deren minimale Anzahl an A-Böcken
                                       geändert werden soll.




                                       Abb. F-83   Ändern der minimalen Anzahl A-Böcke


                                       In diesem Dialog können Sie die für den Lauf notwendige minimale Anzahl an
                                       A-Böcken verändern.
                                       Überschreiben Sie den bisherigen Wert und verlassen Sie den Dialog über die
                                       Schaltfläche [Ok].
3,00 / 01-2023




                 A+W Production Feinplanung                                                                 F-189
                 Läufe feinplanen                                                               Softwarereferenz




                                    Reihenfolge der Maschinen
                                    Stammdaten > Feinplanung > Tische




                                    Abb. F-84    Reihenfolge der Maschinen


                                    Innerhalb der Feinplanung ist es möglich, eine von der Maschinenzuordnung
                                    unabhängige Tischzuordnung vornehmen zu lassen. Dazu müssen die im
                                    System enthaltenen Tische in einer definierten Prüfreihenfolge vorliegen. Die-
                                    se Reihenfolge kann man entweder in den Stammdaten für die Tische hinter-
                                    legen (dort allerdings nur in einem Textfeld ohne Beziehung der Tische
                                    untereinander) oder aber in diesem Dialog.
                                    In diesem Dialog werden alle vorhandenen Tische gemäß dem Feld
                                    XOPT_TISCH::RANG sortiert. Mit Hilfe der Schaltflächen [Hoch] und [Runter]
                                    können diese relativ zueinander verschoben werden und so die Prüfreihenfol-
                                    ge angepasst werden. Wird dieser Dialog über die Schaltfläche [OK] verlas-
                                    sen, so wird automatisch das oben genannte Feld Rang in der Datenbank
                                    entsprechend angepasst.
                                    Für die interne Tischzuordnung werden nun für eine Scheibe alle Tische in obi-
                                    ger Reihenfolge auf Machbarkeit überprüft. Der jeweils zuerst gefundene
                                    Tisch wird der Scheibe zugewiesen.
                                    Die interne Tischzuordnung wird nur verwendet, wenn dies explizit vom An-
                                    wender so eingestellt ist, oder aber die Maschinenzuordnung keine Tischzu-
                                    ordnung erzeugt hat.

                                    Erläuterung der Felder

                                    Anzeige Die Anzeige enthält alle im System angelegten Schneidtische. Die
                                    Schneidtische werden in den Stammdaten angelegt.

                                    Erläuterung der Schaltflächen

                                    Hoch Betätigen Sie diese Schaltfläche, ändert sich die Prüfreihenfolge der im
                                    System enthaltenen Schneidtische. Zum Ändern der Prüfreihenfolge markie-
                                    ren Sie den Schneidtisch, der in der Prüfreihenfolge um eine Position nach
                                    oben verschoben werden soll. Anschließend drücken Sie die Schaltfläche
                                    [Hoch] so oft, bis sich der Schneidtisch an der gewünschten Position befindet.
3,00 / 01-2023




                                    Runter Betätigen Sie diese Schaltfläche, ändert sich die Prüfreihenfolge der
                                    im System enthaltenen Schneidtische. Zum Ändern der Prüfreihenfolge mar-
                                    kieren Sie den Schneidtisch, der in der Prüfreihenfolge um eine Position nach


                 F-190                                                             A+W Production Feinplanung
                 Softwarereferenz                                                                  Läufe feinplanen




                                       unten verschoben werden soll. Anschließend drücken Sie die Schaltfläche
                                       [Runter] so oft, bis sich der Schneidtisch an der gewünschten Position befin-
                                       det.
3,00 / 01-2023




                 A+W Production Feinplanung                                                                   F-191
                 Läufe feinplanen              Softwarereferenz
3,00 / 01-2023




                 F-192              A+W Production Feinplanung
Feinplanung                F

                     Partindex




              A+W Production
                 Partindex




                 A                                         – Robot F-147
                 Abhängige Bearbeitung                     – Sortjet F-148, F-149
                 – Erzeugung F-156                         – Start=0 F-148
                 – Lostyp F-156                            – Überprüfung Anzahl (Fächerwagen) F-148,
                 – Name F-156                                F-149
                 – Register F-156                          – Überprüfung Anzahl (FAP) F-150
                 – Typ F-156                               – Zwei Fächer/Nummer F-148
                 A-Böcke                                   Abstellplatz-Typ
                 – Gruppierung und Sortierung F-94         – Einstellungen-Abstellplatz (Register
                 – Nummernkreise F-95                        Verwendung) F-138
                 – Optimierung F-95                        Abstelltiefe
                 – Produktionsreihenfolge F-93             – A-Bock F-147
                 – Standard-Produktionsorganisation F-93   – Abstellplatz (FAP) F-149
                 A-Böcke SZR                               Ändern der minimalen Anzahl A-Böcke
                 – Nummernkreise F-87                      – Dialog F-189
                 – Optimierung F-87                        Anfang
                 A-Böcke Versand                           – Prüfreihenfolge F-125
                 – Größenklassen F-99                      Anzahl
                 – Gruppierung und Sortierung F-100        – Abstellplatz F-147
                 – Nummernkreise F-101                     – Fachnummer, Dialog Abstellplatz F-148
                 – Produktionsreihenfolge F-100            Anzahl der Stellen für ...
                 – Standard-Produktionsorganisation F-99   – Abstellplatz F-148
                 Abstand v. Achsen                         Artikelnummer für fehlende Bearbeitung
                 – Fächerwagen F-149                       – Bearbeitung F-155
                 Absteigend                                Auffang-Abstellplatz F-136
                 – Gruppierung F-142                       – Einstellungen-Abstellplatz F-136
                 Abstellbreite                             Auffüllbedingung
                 – A-Bock F-147                            – Master-Orga F-128
                 – FAP F-148, F-150                        Aufgefüllte Fächerwagen
                 Abstellmodus F-137                        – Gruppierung und Sortierung F-109
                 – Einstellungen-Abstellplatz F-137        – Nummernkreise F-110
                 – Orga F-131                              – Optimierung F-110
                 Abstellmodus Gruppen                      – Produktionsreihenfolge F-109
                 – Einstellungen-Abstellplatz F-136        – Standard-Produktionsorganisation F-109
                 Abstellplatz                              Aufsteigend
                 – Abstand v. Achsen F-149                 – Gruppierung F-142
                 – Abstellbreite (A-Bock) F-147
                 – Abstellbreite (FAP) F-148, F-150        B
                 – Abstelltiefe (A-Bock) F-147             Bearbeitung
                 – Abstelltiefe (FAP) F-149                – Artikelnummer für fehlende Bearbeitung   F-155
                 – Abweichung Schwerpunkt v. Mitte F-149   – Beschaffungsart F-155
                 – Anzahl F-147                            – Lostyp F-155
                 – Anzahl der Stellen für ... F-148        – Name F-154
                 – Anzahl Fachnummer F-148                 – Typ F-154
                 – Dialog F-146                            Bearbeitungen
                 – ID für Stack-Opti F-148                 – Register F-154
                 – L-Bock F-147                            Beschaffungsart
                 – Leergewicht (Fächerwagen) F-149         – Bearbeitung F-155
                 – Max. Abstellplätze/Bock F-147           Bildung der Gruppen
3,00 / 01-2023




                 – Max. Anzahl Fächerwagen F-147, F-149    – Einstellungen-Abstellplatz F-135
                 – Maximale Nutzlast (Fächerwagen) F-149   – Orga-Gruppen F-133
                 – Maximales Gewicht (A-Bock) F-148
                 – Maximales Gewicht (FAP) F-150


                 A+W Production Feinplanung                                                           F-195
                                                                                                  Partindex




                 D                                          – Register Ergebnisse F-167
                 DynOpt Einstellung   F-133                 – Register Freie Optimierung F-179
                                                            – Register Füllaufträge F-171
                                                            – Register Glasarten F-159
                 E
                                                            – Register Glasdicken F-177
                 Editor-Gruppierungen
                                                            – Register Optionen F-186
                 – Register F-141
                                                            – Register Orga F-182
                 Editor-Sortierung
                                                            – Register Orga-Optionen F-184
                 – Register F-143
                                                            – Register Restblätter F-173
                 Eigenschaft
                                                            – Register Spezial F-169
                 – Gruppierung F-142
                                                            – Register Teilmengen F-180
                 Einstellungen
                                                            – Register Zusammenlegen F-169
                 – Produktionsreihenfolge F-123
                                                            Fertigungsgruppen F-127
                 Einstellungen-Abstellplatz
                                                            – Master-Orga F-127
                 – Abstellmodus F-137
                                                            Formel
                 – Abstellmodus Gruppen F-136
                                                            – Gruppierung F-142
                 – Abstellplatz-Typ (Register
                   Verwendung) F-138
                 – Auffang-Abstellplatz F-136               G
                 – Bildung der Gruppen F-135                Globale Einstellungen
                 – Dialog F-135                             – Funktionsprinzip F-79
                 – Max. Anzahl Gruppen (Register            Größenklasse A-Böcke Versand F-99
                   Verwendung) F-137                        Gruppenbildung
                 – Name F-135                               – Voreinstellungen F-139
                 – Optimierungsverhalten F-136              Gruppierung
                 – Register Verwendung,Von/Bis F-137        – Absteigend F-142
                 – Sortierung in den Gruppen F-135          – Aufsteigend F-142
                 Ende                                       – Eigenschaft F-142
                 – Bruch, Master-Orga F-129                 – Formel F-142
                 – Füller, Master-Orga F-129                – Lostyp F-152
                 – Prüfreihenfolge F-125                    Gruppierung und Sortierung
                 – Restblatt, Master-Orga F-129             – A-Böcke F-94
                 Erzeuge Zusatz-Sortierung                  – A-Böcke Versand F-100
                 – Dialog F-145                             – Aufgefüllte Fächerwagen F-109
                 – Sortierung F-143                         – Fächerwagen ohne Auffüllen F-105
                 – Wert F-145
                 – Wert nicht prüfen F-145                  H
                 Erzeugung                                  Hoch
                 – Abhängige Bearbeitung F-156              – Prüfreihenfolge F-125
                                                            – Reihenfolge der Maschinen   F-190
                 F
                 Fächerwagen ohne Auffüllen                 I
                 – Gruppierung und Sortierung F-105         ID für Stack-Opti
                 – Nummernkreise F-106                      – Fächerwagen F-148
                 – Optimierung F-105
                 – Produktionsreihenfolge F-104
                                                            K
                 – Standard-Produktionsorganisation F-104
                                                            Kein Teilen von...bei Bockbelegung von mehr
                 Feinplanung für Lauf ...
                                                            als...Prozent
                 – Dialog F-158
                                                            – Orga F-132
                 – Register Auswahl Lagermaß F-188
3,00 / 01-2023




                                                            Kurzbeschreibung Standard-
                 – Register Bockbelegung F-162
                                                            Produktionsorganisation F-85
                 – Register Bruchscheiben F-174
                 – Register Eilscheiben F-176


                 F-196                                                        A+W Production Feinplanung
                 Partindex




                 L                                                – Fächerwagen F-149
                 L-Bock                                           Maximales Gewicht
                 – Dialog Abstellplatz F-147                      – A-Bock F-148
                 Leergewicht Fächerwagen F-149                    – FAP F-150
                 Lostyp                                           Mindestmenge
                 – Abhängige Bearbeitung F-156                    – Master-Orga F-128
                 – Bearbeitung F-155
                 – Gruppierung F-152                              N
                 – Name F-152                                     Name
                 – Name/Typ/Beschaffungsart F-152                 – Abhängige Bearbeitung F-156
                 – Nummer F-152                                   – Bearbeitung F-154
                 – Produktionsreihenfolge F-152                   – Einstellungen-Abstellplatz F-135
                 – Sortierung invertieren F-153                   – Lostyp F-152
                 – Technologietyp F-152                           – Master-Orga F-126
                 – Verhalten in der Feinplanung F-153             – Orga-Gruppen F-133
                 Lostypen                                         Name der Orga-Form
                 – Register F-151                                 – Orga F-131
                                                                  Name/Typ/Beschaffungsart
                 M                                                – Lostyp F-152
                 Marken F-9                                       Neu
                 Marktentest                                      – Produktionsreihenfolge F-122
                 – Testmarke F-9                                  Neue Bedingung
                 Master-Orga                                      – Produktionsreihenfolge F-122
                 – Auffüllbedingung F-128                         Nummer
                 – Dialog F-126                                   – Lostyp F-152
                 – Ende Bruch F-129                               Nummernkreise
                 – Ende Füller F-129                              – A-Böcke F-95
                 – Ende Restblatt F-129                           – A-Böcke SZR F-87
                 – Fertigungsgruppen F-127                        – A-Böcke Versand F-101
                 – Mindestmenge F-128                             – Aufgefüllte Fächerwagen F-110
                 – Name F-126                                     – Fächerwagen ohne Auffüllen F-106
                 – Pseudoserien F-127
                 – Quasi Teile F-128                              O
                 – Register F-120                                 Optimierung
                 – Schnell-Orga F-126                             – A-Böcke F-95
                 – Script F-128                                   – A-Böcke SZR F-87
                 – Start Bruch F-129                              – Aufgefüllte Fächerwagen F-110
                 – Start Füller F-129                             – Fächerwagen ohne Auffüllen F-105
                 – Start Restblatt F-129                          Optimierungsverhalten
                 – Verwende Bruchscheiben F-129                   – Einstellungen-Abstellplatz F-136
                 – Verwende Eilscheiben F-129                     Orga
                 – Verwende Füller F-128                          – Abstellmodus F-131
                 – Verwende Restblätter F-129                     – Dialog F-120, F-131
                 – XOPT zusammen abstellen F-126                  – Funktionsprinzip F-20
                 Max                                              – Kein Teilen von...bei Bockbelegung von mehr
                 – Anzahl Fächerwagen, Dialog                       als...Prozent F-132
                   Abstellplatz F-147, F-149                      – Name der Orga-Form F-131
                 – Anzahl Gruppen (Register Verwendung), Dialog   – Produktion F-131
                   Einstellungen-Abstellplatz F-137               – Typ F-131
3,00 / 01-2023




                 Max. Abstellplätze/Bock                          – Voreinstellungen F-139
                 – Abstellplätze F-147                            Orga-Gruppen
                 Maximale Nutzlast                                – Bildung der Gruppen F-133


                 A+W Production Feinplanung                                                               F-197
                                                                                             Partindex




                 – Dialog F-133                        Sortierung
                 – Name F-133                          – Erzeuge Zusatz-Sortierung F-143
                 – Sortierung der Gruppen F-133        Sortierung auf Abstellplatz
                 – Sortierung in den Gruppen F-134     – Voreinstellungen F-139
                                                       Sortierung der Gruppen
                 P                                     – Orga-Gruppen F-133
                 Produktion                            Sortierung in den Gruppen
                 – Orga F-131                          – Einstellungen-Abstellplatz F-135
                 Produktionsreihenfolge                – Orga-Gruppen F-134
                 – A-Böcke F-93                        Sortierung invertieren
                 – A-Böcke Versand F-100               – Lostyp F-153
                 – Aufgefüllte Fächerwagen F-109       Sortjet
                 – Einstellungen F-123                 – Fächerwagen F-148, F-149
                 – Fächerwagen ohne Auffüllen F-104    Standard-Produktionsorganisation
                 – Lostyp F-152                        – A-Böcke F-93
                 – Neu F-122                           – A-Böcke Versand F-99
                 – Neue Bedingung F-122                – Fächerwagen ohne Auffüllen F-104
                 – Register F-122                      – Kurzbeschreibung F-85
                 Prüfreihenfolge                       Standard-Produktionsorganisationen
                 – Anfang F-125                        – Aufgefüllte Fächerwagen F-109
                 – Ende F-125                          Start
                 – Funktionsprinzip F-76               – =0, Abstellplatz F-148
                 – Hoch F-125                          – Bruch, Master-Orga F-129
                 – Register F-124                      – Füller, Master-Orga F-129
                 – Runter F-125                        – Restblatt, Master-Orga F-129
                 Pseudoserien F-127
                 – Master-Orga F-127                   T
                                                       Technologietyp
                 Q                                     – Lostyp F-152
                 Quasi Teile                           Typ
                 – Master-Orga   F-128                 – Abhängige Bearbeitung F-156
                                                       – Bearbeitung F-154
                                                       – Orga F-131
                 R
                 Reihenfolge der Maschinen
                 – Dialog F-190                        U
                 – Hoch F-190                          Überprüfung Anzahl
                 – Runter F-190                        – Fächerwagen F-148, F-149
                 Robot                                 – FAP F-150
                 – Abstellplatz F-147
                 – Funktionsprinzip F-47               V
                 Runter                                Verarbeitungsreihenfolge
                 – Prüfreihenfolge F-125               – Voreinstellungen F-139
                 – Reihenfolge der Maschinen   F-190   Verhalten in der Feinplanung
                                                       – Lostyp F-153
                 S                                     Verwende
                 Schlüssel                             – Bruchscheiben, Dialog Master-Orga F-129
                 – Zusatz-Sortierung F-144             – Eilscheiben, Dialog Master-Orga F-129
                 Schnell-Orga                          – Füller, Master-Orga F-128
3,00 / 01-2023




                 – Master-Orga F-126                   – Restblätter, Dialog Master-Orga F-129
                 Script                                Von/Bis
                 – Master-Orga F-128                   – Register Verwendung, Dialog Einstellungen-
                                                         Abstellplatz F-137


                 F-198                                                   A+W Production Feinplanung
                 Partindex




                 Voreinstellung
                 – Dialog F-139
                 – Gruppenbildung F-139
                 – Orga F-139
                 – Sortierung auf Abstellplatz F-139
                 – Verarbeitungsreihenfolge F-139

                 W
                 Wert
                 – Erzeuge Zusatz-Sortierung   F-145
                 – Zusatz-Sortierung F-144
                 Wert nicht prüfen
                 – Erzeuge Zusatz-Sortierung   F-145

                 X
                 XOPT zusammen abstellen
                 – Master-Orga F-126

                 Z
                 Zusatz-Sortierung
                 – Register F-144
                 – Schlüssel F-144
                 – Wert F-144
                 – Zusatz-Sortierung F-144
                 Zwei Fächer/Nummer
                 – Abstellplatz F-148
3,00 / 01-2023




                 A+W Production Feinplanung            F-199
                                           Partindex
3,00 / 01-2023




                 F-200   A+W Production Feinplanung

