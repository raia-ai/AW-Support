---
description: "DE AWProduction DynOpt 1.00"
---



# DE AWProduction DynOpt 1.00

A+W DynOpt   N




             deutsch
                                                                                                 Vorspann




                              Vorspann
                              In diesem Teil der Dokumentation finden Sie editorische Notizen.


                              Revisionsübersicht
                              Version / Datum          Beschreibung

                              1.00 / 03-2016           Ersterstellung



                              Editorial
                              Das Editorial enthält Informationen zu folgenden Themen:
                              •   Anmerkungen zu diesem Dokument
                              •   Urheberrechte
                              •   Warenzeichen
                              •   Kontakte

                              Anmerkungen zu diesem Dokument
                              Diese Veröffentlichung ist ausschließlich für Endanwender von A+W DynOpt
                              gedacht.
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
                              © 2016, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
                              stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                              Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                              piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen
                              Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der
                              A+W Software GmbH darf die Dokumentation weder elektronisch, mecha-
                              nisch, per Aufzeichnung oder in sonstiger Form übertragen werden.
1.00 / 01-2016




                 A+W DynOpt                                                                          N-3
                 Vorspann




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

                               +49 6404 2051 877

                            Zentrale@a-w.com

                            http://www.a-w.com
1.00 / 01-2016




                 N-4                                                                       A+W DynOpt
                                                                                                                                                    Inhalt




                              Inhalt
                              Vorspann ................................................................................................................ N-3
                               Revisionsübersicht .............................................................................................. N-3
                               Editorial ............................................................................................................... N-3

                              Tutorial                                                                                                               J-7
                              Überblick ................................................................................................................. J-9
                              Dynamische Optimierung ..................................................................................... J-10
                                Leistungsbeschreibung ..................................................................................... J-11
                                Problemstellung ................................................................................................. J-14
                                Optimierung mit A+W DynOpt ........................................................................... J-17
                                  Dynamischer Zeitstrahl .................................................................................. J-19
                                  Puffersystem .................................................................................................. J-21
                                  Pufferbelegung ............................................................................................... J-22
                                Zusammenarbeit mit Panorama ........................................................................ J-23
                              Mit A+W DynOpt arbeiten ..................................................................................... J-25
                                A+W DynOpt Editor ........................................................................................... J-27
                                  Eilscheiben in zwei Schritten priorisieren ....................................................... J-29
                                  A+W DynOpt Editor bedienen ........................................................................ J-33

                              Partindex                                                                                                          N-35
                              Index ..................................................................................................................... N-37
1.00 / 01-2016




                 A+W DynOpt                                                                                                                           N-5
                 Inhalt
1.00 / 01-2016




                 N-6      A+W DynOpt
A+W DynOpt        J

             Tutorial
                 Tutorial                                                                             Überblick




                              Überblick
                              In diesem Dokument finden Sie Informationen zum Konzept der dynamischen
                              Optimierung. Daran schließend finden Sie Informationen zu den manuellen
                              Eingriffen, mit Sie die Optimierung starten und bearbeiten.
                              In diesem Tutorial finden Sie folgende Informationen:
                              •    “Dynamische Optimierung” auf Seite J-10
                              •    “Mit A+W DynOpt arbeiten” auf Seite J-25

                              Vorausgesetzte Kenntnisse
                              Das Tutorial richtet sich an Teilnehmer, die in A+W Production die Arbeitsvor-
                              bereitung verantworten und damit den optimalen Ablauf der Produktion orga-
                              nisieren. Die Teilnehmer müssen das Konzept der Stammdaten und
                              Einlastung in A+W Production kennen.

                              Darstellungskonventionen
                              Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben fol-
                              gende Bedeutung:

                              Kursiv                    sind Zeichenfolgen ausgezeichnet, die Elemente der
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
1.00 / 01-2016




                 A+W DynOpt                                                                                   J-9
                 Dynamische Optimierung                                                                      Tutorial




                                          Dynamische Optimierung
                                          Das Tutorial zum Modul A+W DynOpt beschäftigt sich mit der Optimierung
                                          des Produktionsablaufs von der Planung der Lose bis zum fertigen Produkt.
                                          In diesem Kapitel finden Sie Informationen zu folgenden Themen:
                                          •   “Leistungsbeschreibung” auf Seite J-11
                                          •   “Problemstellung” auf Seite J-14
                                          •   “Optimierung mit A+W DynOpt” auf Seite J-17
                                          •   “Zusammenarbeit mit Panorama” auf Seite J-23
1.00 / 01-2016




                 J-10                                                                                 A+W DynOpt
                 Tutorial                                                                    Dynamische Optimierung




                                         Leistungsbeschreibung
                                         Ein wesentliches Einsparpotential bei der Flachglasverarbeitung ist die opti-
                                         male Ausnutzung der Lagerplatten beim Zuschnitt.
                                         •   Mit dem innovativen Optimierungsalgorithmus und der intelligenten und
                                             modernen Maschinen- und Lageranbindung ist es möglich, alternierend
                                             verschiedene Glasarten aufzulegen und zu schneiden.
                                         •   Mit dem Einsatz eines Zwischenpuffers kann dynamisch optimiert, ge-
                                             schnitten und in den Zwischenpuffer einsortiert werden.
                                         •   Die Ansteuerung von Schneidtischen mit den optimierten Schnittbildern di-
                                             rekt aus der Optimierung beschleunigt zudem den Arbeitsprozess.
                                         A+W DynOpt ist ein komplexer Systemverbund aus verschiedenen Hardware-
                                         und Softwarekomponenten:
                                         •   Schneidtisch(e)
                                         •   Lager- und Restplattenlager
                                         •   Zwischenpuffer und Sortiersystem
                                         •   A+W Production zur Arbeitsvorbereitung
                                         •   A+W Realtime Optimizer zur Online-Optimierung am Tisch
                                         •   Panorama und Produktionsansicht in A+W Production Cockpit zur Ge-
                                             samtsteuerung und Visualisierung des Systems.
1.00 / 01-2016




                 Abb. J-1   Produktionsansicht in A+W Production Cockpit



                 A+W DynOpt                                                                                       J-11
                 Dynamische Optimierung                                                                         Tutorial




                                          Zuschnittplanung mit A+W DynOpt
                                          Wenn die Produktionsläufe in A+W Production freigegeben sind, können sie
                                          in A+W DynOpt importiert werden. Die Läufe werden im A+W DynOpt Editor
                                          zum Import freigegeben und durch das Modul A+W Realtime Optimizer impor-
                                          tiert. Damit fließen die Läufe in die dynamische Optimierung ein.
                                          Diese importierten und freigegebenen Läufe werden permanent geprüft. Da-
                                          bei werden die Läufe von A+W DynOpt komplett aufgelöst und dynamisch un-
                                          ter verschiedenen Aspekten neu optimiert, z. B. um gleichen Glasarten besser
                                          zusammenzustellen oder Scheiben mit höherer Priorität vorzuziehen. Die be-
                                          rechneten Schnittbilder werden von A+W DynOpt pro Schneidtisch visuali-
                                          siert.




                 Abb. J-2   Visualisierung der Schnittbilder in A+W DynOpt


                                          Die geschnittenen Scheiben werden in einen Zwischenpuffer gestellt, aus
                                          dem sie dann in der ursprünglichen Produktionssequenz entnommen werden.
                                          Dieses Verfahren bietet folgende Vorteile:
                                          •   Ein kontinuierlicher Glasstrom fließt in der korrekten Fertigungssequenz.
                                          •   Das best-mögliche Verschnittergebnis wird erreicht.
1.00 / 01-2016




                                          Wenn Sie mit einem Restblatt-Lager arbeiten, können statt auf Lagerplatten
                                          zuzugreifen geeignete Restblätter verwertet werden. Zusätzlich zu einem gu-




                 J-12                                                                                     A+W DynOpt
                 Tutorial                                                         Dynamische Optimierung




                              ten Optimierungsergebnis pro Schneidtisch senkt dieses Verfahren auch den
                              Realverschnitt und Sie können das Restblatt-Lager erheblich verkleinern.
                               “Realverschnitt” auf Seite J-18



                              Problemstellung
                              Betriebe in der Glaswirtschaft sehen sich neuen Herausforderungen gegen-
                              über: Von den Kunden werden eine extreme Variantenvielfalt, sehr kurze Lie-
                              ferzeiten und schnelle Nachlieferungen gefordert. Dazu kommt eine hohe
                              Anzahl an Eilaufträgen. Gleichzeitig sinken die Liefermengen pro Kunde und
                              Tour.
                              Die Folgen dieser Situation sind:
                              •   Die Losgrößen werden kleiner und die Produktion muss ständig neu ge-
                                  plant werden.
                              •   Die höhere Flexibilität in der Fertigung fordert folgende Problemlösungen:
                                  – Größere Glasreste bei der Optimierung des Zuschnitts müssen verwal-
                                     tet werden.
                                  – Erhöhter Aufwand beim Handling der Scheiben.
                                  – Durch die kleineren Losgrößen aus der Feinplanung wird der Spielraum
                                     der Optimierung beim Zuschnitt geringer.
                                     Dies wirkt sich zusätzlich zum aktuellen Verschnitt auch auf den Real-
                                     verschnitt aus, bei dem der Verschnitt über das Jahr hinweg betrachtet
                                     wird. Dieser Realverschnitt gibt die Gesamtmenge/Fläche an nicht ge-
                                     nutzter Glasfläche an.
                                  – Im Ganzen resultiert daraus eine bis zu 10 % geringere Ausbeute.
                              Auf diese Anforderungen reagiert A+W DynOpt mit einer flexiblen Lösung.
1.00 / 01-2016




                 A+W DynOpt                                                                           J-13
                 Dynamische Optimierung                                                                             Tutorial




                                  Standard-Optimierung                                     A+W DynOpt

                  Zuschnitt      feste Produktionssequenz                     Zuschnitt    "chaotisch"
                                 sortenrein pro Los                                        dynamsich

                        Zwischenlagerung                                             Dynamischer Puffer
                              manuelles Umsortieren                                       automatische Aussortierung
                                                                                          in Produktionssequenz

                                Produktion                                                  Produktion
                                Linie 1            Gestell                                  Linie 1

                                Produktion                                                  Produktion
                                Linie 2            Gestell                                  Linie 2




                                                             Versand                                      Versand


                 Abb. J-3      Optimierungsmethoden


                                             In dieser Grafik sehen Sie eine vereinfachte Gegenüberstellung der Optimie-
                                             rung nach einer Standardmethode und mit A+W DynOpt. Diese beiden Ansät-
                                             ze werden im Folgenden näher beschrieben.

                                             Standard-Optimierung
                                             Mit dem bisherigen Lösungsansatz wurden alle Bereiche einer Produktion
                                             nacheinander optimiert. Unter den aktuellen Bedingungen entsteht im An-
                                             schluss an eine optimierte Produktion beim Versand ein großer Aufwand, den
                                             man mit viel manueller Arbeitskraft zu beheben versucht. Denn durch die hohe
                                             Variantenvielfalt und kurzen Reaktionszeiten stauen sich die Scheiben auf den
                                             Gestellen. Dies verlangt von den Mitarbeitern im Versand erhöhte Aufmerk-
                                             samkeit und erhöhten Einsatz beim Zuordnen der Scheiben zu den Aufträgen.
                                             Bei dieser starren Arbeitsorganisation versucht die Arbeitsvorbereitung, pas-
                                             sende Losgrößen zu finden. Ausnahmefälle, wie Bruchscheiben und Eilaufträ-
                                             ge, werden sehr teuer, da diese i. d. R. im Handzuschnitt geschnitten werden.
                                             Eine effiziente Produktion muss jedoch so gesteuert werden, dass die Bear-
                                             beitungsschritte für jede Scheibe nahtlos durchlaufen werden – bis hin zur
                                             Direktverpackung, bei der die fertigen Scheiben ohne Zwischenlagerung di-
                                             rekt verpackt und auf den Lkw verladen werden können. Die Direktverpackung
                                             hat also einen enormen Einfluss auf die gesamte Produktion.
1.00 / 01-2016




                 J-14                                                                                        A+W DynOpt
                 Tutorial                                                         Dynamische Optimierung




                              Konflikt bei Losgrößen
                              Der Losgrößen-Konflikt ist in der Glasindustrie bekannt: Über die Losgröße
                              müssen die Flexibilität und Ausbeute ausgelotet werden.




                                           Au
                                             sb
                                               eu
                                                 t  e
                                              ä t
                                           lit
                                           bi
                                       e xi
                                    Fl




                                                         Losgröße


                              Abb. J-4          Losgrößen-Konflikt


                              In dieser Grafik sehen Sie, dass die Ausbeute bei einer höheren Flexibilität
                              sinkt. Bei einer sehr hohen Ausbeute geht die Flexibilität gegen Null.
1.00 / 01-2016




                 A+W DynOpt                                                                            J-15
                 Dynamische Optimierung                                                                        Tutorial




                                          Gleichzeitig entstehen durch die hohe Variantenvielfalt organisatorische Pro-
                                          bleme beim Zuschnitt:
                                          •   Die geschnittenen Scheiben müssen zwischengelagert werden. Die dyna-
                                              mischen Puffer nach dem Zuschnitt gewinnen damit zunehmend an Be-
                                              deutung.
                                          •   Die Restplatten müssen verwaltet werden.




                 Abb. J-5   Beispiel: Variantenvielfalt und verarbeitete Mengen


                                          Der Losgrößen-Konflikt und die Restplatten-Thematik müssen ständig neu ge-
                                          prüft werden – die Produktion braucht eine dynamische Lösung, die laufend
                                          auf aktuelle Ereignisse reagiert.
1.00 / 01-2016




                 J-16                                                                                    A+W DynOpt
                 Tutorial                                                              Dynamische Optimierung




                              Optimierung mit A+W DynOpt
                              Um vollautomatisch und dynamisch arbeiten zu können, stellt A+W DynOpt
                              Anforderungen an die Hardware:
                              •   Am Zuschnitt werden ein Puffer und ein Sortierer eingesetzt.
                              •   Die Schneidtische müssen eine möglichst hohe Flexibilität bieten, z. B.
                                  durch mehrere Schneidköpfe.
                              A+W DynOpt wird jeweils für die verwendete Hardware konfiguriert, so dass
                              der Puffer immer ausreichend gefüllt ist. Weil der Zuschnitt schneller ist als die
                              Linien, bleibt an diesem Arbeitsplatz Raum für Unterbrechungen, z. B. wenn
                              wegen einer Glaslieferung das Lager betreten werden muss.
                              A+W DynOpt ist eine Nahbereichs-Optimierung, d. h. die Optimierung bezieht
                              sich immer auf die aktuelle Situation am Schneidtisch. Dabei werden aktuelle
                              Ereignisse berücksichtigt, z. B. Bruchscheiben und Eilaufträge. A+W DynOpt
                              betrachtet permanent den zukünftigen Vorrat an Läufen und Losen und opti-
                              miert automatisch neu.
                               “Dynamischer Zeitstrahl” auf Seite J-19

                              Optimierung der Läufe
                              Die Optimierung und die Produktion werden in Läufen und Losen organisiert:
                              •   Ein Lauf ist eine Menge an Glas, die als Gruppe gemeinsam betrachtet und
                                  in die Produktion gegeben werden soll. Darin können verschiedene Glas-
                                  arten enthalten sein.
                              •   Ein Los ist eine Untermenge eines Laufs. In einem Los sind die Scheiben
                                  zusammengefasst, die zur gleichen Zeit unter den gleichen Produktionsbe-
                                  dingungen an der gleichen Maschine gefertigt werden.
                              Für jede Glasart wird an jedem Tisch jeweils ein Los erzeugt. Die Reihenfolge
                              der einzelnen Platten innerhalb des Laufes werden aber nach dem bestmög-
                              lichem Abfluss bestimmt. Damit entstehen schnell wechselnde Glasarten an
                              den Tischen.

                                  Beispiel

                                  Im Lauf sind die Glasarten Float 4 mm und Float 5 mm enthalten.
                                  Sie folgend direkt aufeinander und sollen auf Tisch 1 geschnitten werden.
                                  Aus der Abfolge Float 4 – Float 5 – Float 4 ergeben sich also folgende Lose:
                                  Los 1 – Float 4 – Teil 4
                                  Los 2 – Float 5 – Teil 1
                                  Los 1 – Float 4 – Teil 2


                              Die Grob- und Feinplanung von A+W Production bietet die Basis für die Opti-
                              mierung von A+W DynOpt. Dabei werden die feingeplanten Läufe aufgelöst
                              und neu berechnet Die Feinplanung bezieht auch die Abstellplätze für die ge-
1.00 / 01-2016




                              schnittenen Scheiben ein. Diese Planung behält A+W DynOpt bei.
                              Die Fertigungslose werden nur dann als bindend betrachtet, wenn sie dem
                              Produktionsfluss dienlich sind. Die endgültigen Fertigungslose entstehen da-



                 A+W DynOpt                                                                                      J-17
                 Dynamische Optimierung                                                                           Tutorial




                                          her erst nach dem Zuschnitt – womit sich der Losgrößen-Konflikt zu einem er-
                                          heblichen Teil auflöst.
                                          Wenn A+W DynOpt die Läufe der Feinplanung auflöst, behält das Programm
                                          die Sequenz für einen Lauf bei. Das heißt, dass die Scheiben aus dem Puffer
                                          am Zuschnitt an die von der Feinplanung geplanten Abstellplätze übergeben
                                          werden. Die Scheiben sind also nach dem Zuschnitt weiterhin für die Folge-
                                          prozesse organisiert. Die Scheiben werden also so aus dem Puffer entnom-
                                          men, wie sie in den Folgeprozessen benötigt werden. Die leer gewordenen
                                          Fächer können entsprechend neu bestückt werden.
                                          Damit steht A+W DynOpt zwischen den Prozessen und kommuniziert mit
                                          A+W Production, der Datenbank, allen A+W Production Terminals und allen
                                          angebundenen Komponenten, z. B. Schneidtischen, Puffern, Sortiersyste-
                                          men, Restplattenspeichern. A+W DynOpt übernimmt die Steuerung und
                                          Kommunikation mit allen beteiligten Software- und Hardware-Systemen, über-
                                          wacht Zustandsdaten und meldet relevante Ergebnisse und Ereignisse, z. B.
                                          Bruch.
                                          Die Abbildung des Maschinenmodells übernimmt das "Panorama".
                                           “Zusammenarbeit mit Panorama” auf Seite J-23

                                          Auslöser zur Neuoptimierung
                                          A+W DynOpt kann aus unterschiedlichen Gründen die noch nicht übertrage-
                                          nen Platten auflösen und neu optimieren, z. B:
                                          •   Bruchscheiben stehen im Bruchpool.
                                          •   Die Laufreihenfolge wird durch manuelle Eingriffe oder definierte Prioritä-
                                              ten veändert.
                                          •   Neue Läufe wurden importiert.
                                          Im Normalfall findet dieses Auflösen immer nach einem Plattenwechsel statt.
                                          Danach wird mit der neu zur Verfügung stehenden Gesamtmenge an Schei-
                                          ben optimiert.

                                          Realverschnitt
                                          Bei der Optimierung orientiert sich A+W DynOpt an der wahren Ausbeute. Da-
                                          mit handelt es sich also nicht nur um die Optimierung des Zuschnitts, sondern
                                          um eine Optimierung, die die gesamte Produktion profitabler macht.
                                          Diese Betrachtungsweise bezieht sich nicht nur auf einzelne Verschnitt-
                                          optimierungen, sondern behält über einen Arbeitstag im Blick, wie viele Lager-
                                          platten in die Produktion gegangen sind und wie viel Rest dabei entstand.
                                          Zusätzlich berücksichtigt und reduziert A+W DynOpt den Aufwand beim
                                          Handling der Scheiben – und reduziert damit auch den Anteil der Bruchschei-
                                          ben und Kratzer.
                                          Durch diese ganzheitliche Betrachtungsweise könnten einzelne Schritte von
                                          A+W DynOpt zunächst nicht schlüssig erscheinen. Aber: A+W DynOpt ermög-
                                          licht es, in Optimierungsgrade vorzudringen, die man mit herkömmlicher Pla-
                                          nung nicht erreichen würde. Vorhandene oder neue Reste werden besser und
1.00 / 01-2016




                                          mit höherer Priorität für den Zuschnitt verwendet.
                                          Je weniger Verschnitt oder Restblätter, desto höher die Materialausnutzung
                                          und desto geringer die Materialkosten.


                 J-18                                                                                      A+W DynOpt
                 Tutorial                                                                            Dynamische Optimierung




                                           Dynamischer Zeitstrahl
                                           In A+W DynOpt bilden die Cluster einen endlosen Zeitstrahl, in den die Schei-
                                           ben eingeordnet und verplant werden. Ein Cluster ist dabei in der Regel je-
                                           weils die Menge eines Fächerwagens. Die Optimierung arbeitet diesen
                                           Zeitstrahl bis zum Zuschnitt ab. Die Scheiben, die früher in der Produktion ge-
                                           braucht werden, werden früher im Zeitstrahl einsortiert und haben damit eine
                                           höhere Priorität. Mit den späteren Scheiben werden Lücken aufgefüllt, um
                                           eine gute Ausbeute zu bekommen.


                     Ausgang                                                                                Eingang




                                                                                                             t


                                    A             B       C        D                 E           F

                 A Dynamischer Puffer für geschnittene Scheiben     D Optimierte Cluster (Tisch 2)
                 B Geschnittene Cluster (Tisch 1)                   E Cluster können weiter optimiert werden ("an-optimiert").
                 C Zuschnitt                                        F Cluster sind noch nicht optimiert (Füllscheiben)
                 Abb. J-6     Cluster im Zeitstrahl der dynamischen Optimierung


                                           Diese Abbildung zeigt die optimierten Läufe, die den Zuschnitt durchlaufen
                                           und in den Puffer gegeben werden. Die feingeplanten Läufe bilden für das
                                           Programm den Eingang. Die geschnittenen Scheiben, die aus dem dynami-
                                           schen Puffer ausgegeben werden, bilden den Ausgang.
                                           Die rote Linie symbolisiert den Zuschnitt:
                                           •   Die Cluster links der roten Linie (hellblau) sind bereits geschnitten und wer-
                                               den in den Puffer gegeben.
                                           •   Die Cluster rechts der roten Linie wurden noch nicht geschnitten und sind
                                               in drei Prioritäten aufgeteilt:
1.00 / 01-2016




                                               – Die dunkelblauen Cluster sind vollständig optimiert und werden mit ho-
                                                   her Priorität als nächstes geschnitten.




                 A+W DynOpt                                                                                              J-19
                 Dynamische Optimierung                                                                           Tutorial




                                             – Die gelben Cluster sind noch nicht vollständig optimiert und können mit
                                               Füllscheiben (grün) noch aufgefüllt werden.
                                             – Die grünen Cluster sind nochnicht optimiert. Sie können bei einer neuen
                                               Optimierung der gelben Cluster als Füllmasse verwendet werden.
                                          Sind die Scheiben eines Clusters geschnitten, werden sie im Puffer abgestellt,
                                          und A+W DynOpt führt eine neue Optimierung durch. Vom darauffolgenden
                                          Cluster werden einige Scheiben schon geschnitten sein, weil diese zum vor-
                                          herigen Cluster als Füllmasse dazu genommen wurden. Der Rest des aktuel-
                                          len Clusters wird geschnitten.
                                          Ziel der Optimierung ist, dass jede Produktionslinie stets Nachschub hat. Da-
                                          rum muss möglichst viel Abfluss aus dem Puffer entstehen. Wichtig ist dabei,
                                          dass für jeden Ausgang ein eigener Zeitstrahl gebildet wird. A+W DynOpt ver-
                                          sucht, diese möglichst gleichmäßig zu bedienen.
                                          Das Prinzip lautet: Der nächste Zuschnitt einer Platte muss zu einem mög-
                                          lichst hohen Abfluss aus dem Puffer führen. Dies wird nur dann erreicht, wenn
                                          Scheibe und Gegenscheibe für ISO oder VSG im Puffer stehen. Dabei werden
                                          im ersten Schritt Schnittpläne erstellt und im zweiten Schritt diese Schnittplä-
                                          ne so optimiert, dass die zusammengehörenden Scheiben für die ISO/VSG-
                                          Produktion gleichzeitig zur Verfügung stehen.
                                           “Puffersystem” auf Seite J-21


                                           A



                                           B

                                           C




                                           D



                                          A Neu optimierte Läufe                  C Geschnittene Scheiben im Puffer
                                          B Sonderglas, wartet auf Zuschnitt      D Schneidpläne
                                          Abb. J-7     Optimierte Läufe und Pufferbelegung


                                          In dieser Abbildung sehen Sie, dass im Puffer Plätze für Sondergläser frei-
                                          gehalten werden, wenn diese z. B. zur ISO-Produktion benötigt werden. Die
                                          Optimierung muss also berücksichtigen, dass diese Scheiben nicht so spät
                                          geschnitten werden, dass die ISO-Linie nicht mehr bedient werden kann.
                                           “Pufferbelegung” auf Seite J-22
                                          A+W DynOpt greift beim Optimieren auch auf Restplatten zu. Dadurch können
1.00 / 01-2016




                                          im Vergleich zu einer herkömmlichen Produktion erhebliche Materialeinspa-
                                          rungen erzielt werden.




                 J-20                                                                                      A+W DynOpt
                 Tutorial                                                        Dynamische Optimierung




                              Gemeldete Bruchscheiben werden automatisch in die Optimierung aufgenom-
                              men, so dass eine möglichst schnelle Nachproduktion gewährleistet werden
                              kann. Jede neue Optimierung wird an Auslöser geknüpft, z. B. ein vorgegebe-
                              ner Zeitabstand oder eine bestimmte Anzahl an Bruchscheiben. Dazu werden
                              alle Läufe, die noch nicht an den Zuschnitt übergeben wurden, komplett auf-
                              gelöst und neu optimiert.
                               “Optimierung der Läufe” auf Seite J-17
                               “Dynamischer Zeitstrahl” auf Seite J-19


                              Puffersystem
                              Die Produktion mit A+W DynOpt ist nur mit einem geeigneten Puffer sinnvoll.
                              Das erfordert ein Puffersystem, in dem Scheiben in ausreichenden Mengen
                              zwischengelagert und zum richtigen Zeitpunkt an die Linien ausgegeben wer-
                              den können. Damit sichert der Puffer auch die Produktion an den Linien, falls
                              der Zuschnitt steht.
                              A+W DynOpt wird speziell auf die kundenseitige Hardware hin konfiguriert.
                              Das gilt auch für bereits vorhandene Puffer. A+W DynOpt stellt den logischen
                              Puffer dar, indem es die zusammengehörenden Scheiben zusammen plant.
                              Die physikalische Belegung des Puffers wird durch den jeweiligen Hersteller
                              des Puffers vorgegeben. A+W DynOpt wird immer so angepasst, dass es den
                              vorhandenen Puffer optimal ausnutzt.
                              A+W DynOpt interagiert mit dem Puffersystem und tauscht Daten aus. Dabei
                              wird die Belegung der Fächer unter anderem so konfiguriert, dass sie örtlich
                              an die Produktion angepasst ist. Scheiben, die für eine ISO-Linie bestimmt
                              sind, werden auch nahe an der ISO-Linie abgestellt.
                              Zusätzlich können die Mengen einzelner Fächer im Puffers gesperrt werden.
                              Fächer können jedoch durch den Herstellern auch vollständig gesperrt wer-
                              den, z. B. wenn sie beschädigt sind und nicht verwendet werden können.
1.00 / 01-2016




                 A+W DynOpt                                                                          J-21
                 Dynamische Optimierung                                                                             Tutorial




                                          Pufferbelegung
                                          Im Puffer wird zwischen der logischen und der physikalischen Belegung des
                                          Puffers unterschieden.
                                          •   Die logische Belegung gibt vor, wie Scheiben in Fachern zusammengehal-
                                              tenr werden müssen. Die ist die planerische Vorgabe für den Maschinen-
                                              hersteller.
                                          •   Bei der physikalische Belegung werden die Fächer so vergeben, wie die lo-
                                              gische Belegung dies zulässt oder fordert. Die geschnittenen Scheiben
                                              laufen nach den Vorgaben der logischen Belegung in die Facher.
                                          Die Schneidpläne werden immer erst dann an den Zuschnitt übergeben, wenn
                                          der Platz für die Scheiben im Puffer garantiert ist.
                                          Die Belegung des Puffers wird im Dialog Zuschnitt-Übersicht angezeigt.




                               A      B                             C         D               E
                 A Status des markierten Fachs                      C grün: gefülltes Fach
                 B Markiertes Fach                                  D physikalisch vorhandene Scheiben (blau)
                                                                    E grau: reservierte Fächer, für Scheiben, die erwartet
                                                                      werden
                 Abb. J-8    Puffer-Übersicht in A+W Production


                                          Unter den Fächern wird der Status des jeweiligen Fachs angezeigt:
                                          •   weiß: das Fach ist komplett frei.
                                          •   grau: das Fach ist reserviert.
                                          •   dunkelgrün: das Fach ist belegt, die Scheiben sind aber noch nicht zum
1.00 / 01-2016




                                              Austransport bereit.
                                          •   hellgrün: das Fach ist belegt und die Scheiben sind zum Austransport be-
                                              reit.



                 J-22                                                                                       A+W DynOpt
                 Tutorial                                                         Dynamische Optimierung




                              Fehlende Scheiben erzeugen Lücken im Zeitstrahl. Der Puffer wird dann im-
                              mer voller, weil die Produktion auf die Scheiben wartet. Wenn der Puffer für
                              eine optimale Ausbeute zu voll wird, kann es zwingend notwendig werden,
                              eine bestimmte Scheibe zu produzieren. In diesem Fall muss in Kauf genom-
                              men werden, dass die Ausbeute nicht optimal ist, die Produktion jedoch nicht
                              stillsteht.
                              Wenn im Zeitstrahl keine Lücken mehr sind, wird der Puffer leerer. Damit stei-
                              gen die Möglichkeiten der Optimierung und die Ausbeute wieder.


                              Zusammenarbeit mit Panorama
                              Die Abbildung des Maschinenmodells und die Kommunikation mit den Ma-
                              schinen übernimmt dabei das sogenannte Panorama. Dies ist die zentrale
                              Maschinen-Steuerungs- und -Kommunikationskomponente von A+W DynOpt.
                              Das Ergebnis der Optimierung wird in die Datenbank geschrieben und bildet
                              einen sogenannten Step. Diese Steps werden vom A+W Realtime Optimizer
                              eingelesen, das dann die Daten für Panorama generiert. Mit diesen Daten
                              steuert Panorama die Anlage.

                              Restplatten
                              Panorama meldet Restplatten aus dem Restplattenspeicher an den A+W
                              Realtime Optimizer. Dieser fragt über Panorama beim Restplattenspeicher an,
                              ob diese Platte noch eingelagert werden kann. Wenn ja werden die Daten
                              durch den A+W Realtime Optimizer entsprechend angepasst und an Panora-
                              ma gegeben.

                              Puffersystem
                              Panorama verwaltet logisch das Puffersystem und prüft, ob noch weiter
                              Schneidcodes übertragen werden dürfen. Wenn alle Scheiben der Platte ins
                              Puffersystem passen, wird der Schneidcode erzeugt und an die Maschine
                              übertragen. Nach den Vorgaben des A+W DynOpt-Kerns und der Optimierung
                              steuert Panorama zusätzlich, welche Scheiben zusammen in ein Pufferfach
                              gestellt werden dürfen.

                              Bruchscheiben
                              Von der Maschine erhält Panorama Positions- und Bruchmeldungen über die
                              gesamte Anlage. Bruchscheiben, die beim Eintransport entstehen, werden
                              automatisch nachgeschnitten.
                              Grundsätzlich versucht Panorama immer die Bruchscheiben so nachzufüh-
                              ren, dass die Einheit doch noch komplett auf den Ausgang gegeben werden
                              kann. Dazu hat A+W DynOpt folgende Modi wie Platten mit Bruchscheiben
                              priorisiert werden können:
                              •   Die Platten werden aufgrund der am Ausgang als nächstes benötigten nor-
                                  malen Scheiben sortiert. Hierbei werden Platten die nur aus Bruchschei-
1.00 / 01-2016




                                  ben bestehen ans Ende der Reihenfolge gesetzt.




                 A+W DynOpt                                                                           J-23
                 Dynamische Optimierung                                                                        Tutorial




                                          •   Die Platten werden auf Grund der am Ausgang als nächstes benötigten
                                              normalen Scheiben sortiert. Dabei werden Platten, die nur aus Bruchschei-
                                              ben bestehen, an den Anfang der Reihenfolge gesetzt.
                                          •   Wenn es aufgrund der Pufferbelastung möglich ist, werden alle Platten mit
                                              Bruchscheiben an den Anfang der Reihenfolge gesetzt. Wenn A+W Dy-
                                              nOpt aufgrund der Pufferlast eine solche Reihenfolge nicht annehmen
                                              kann, müssen möglichst schnell Einheiten komplettiert werden, um die Puf-
                                              ferlast zu reduzieren.

                                          Sonderscheiben
                                          Scheiben, die nicht aus der Optimierung kommen, können direkt am Ausgang
                                          zugeführt werden, z. B. Zukauf-Scheiben oder Handzuschnitt. Diese Schei-
                                          ben können ggf. auch über einen eigenen Eingang zugestellt werden.

                                          Produktionssequenzen
                                          Zu den übergebenen Produktionsläufen verwaltet Panorama Produktionsse-
                                          quenzen mit den Informationen zu Einheiten, Scheiben, Reihenfolge und Sta-
                                          tus eines Laufs.
                                          Aufgrund dieser Informationen und auch der Reihenfolge der Sequenzen be-
                                          auftragt Panorama Scheiben zum Austransport in einen Ausgang. Auch auf
                                          der Austransportstrecke erhält Panorama Positions- und Bruchmeldungen.
1.00 / 01-2016




                 J-24                                                                                    A+W DynOpt
                 Tutorial                                                        Mit A+W DynOpt arbeiten




                              Mit A+W DynOpt arbeiten
                              A+W DynOpt erfordert nur einen Mitarbeiter mit einem ganzheitlichen Blick auf
                              die Produktion. Dieser Mitarbeiter kann Änderungen im Produktionsablauf ein-
                              leiten, und A+W DynOpt nimmt die Änderungen mit bei bestmöglicher Perfor-
                              mance vor.
                              Das Programm schleust die importierten Läufe selbstständig vom Eingang bis
                              zum Ausgang, solange genügend Läufe importiert sind und kein Eingreifen,
                              z. B. wegen Eil- oder Bruchscheiben, nötig wird.
                              Die Reihenfolge der Läufe ist mit A+W DynOpt änderbar. Zum Beispiel können
                              Lose von der ISO-Linie vorgezogen werden, wenn dies erforderlich wird. Der
                              Mitarbeiter fordert dann das entsprechende Los am Bildschirm an, und A+W
                              DynOpt organisiert die Lose neu.
                              Die Änderung erfolgt dabei mit den Vor- und Nachteilen, die zu diesem Zeit-
                              punkt maximal möglich sind. Die Konsequenzen der Änderung, z. B. ein vor-
                              gezogener Lauf, sind direkt am Bildschirm sichtbar.
                              Der Mitarbeiter muss die Konsequenzen seiner Eingriffe abschätzen können.
                              A+W DynOpt bietet dazu Werkzeuge, mit denen der Mitarbeiter den Überblick
                              behält und seine Entscheidungen abschätzen kann:
                              •   A+W DynOpt-Editor
                              •   Register XOPT-ON Dynamics von A+W Realtime Optimizer
                              •   Zuschnitt-Übersicht von A+W Realtime Optimizer
                              •   A+W Production Cockpit mit konfigurierbaren Dialogen
                                  Dieses individuell für ein A+W DynOpt-Projekt angefertigter Leitstand aus
                                  verschiedenen Anzeigen ist ein optionales Zusatzmodul, das hier nicht be-
                                  schrieben wird. Als zentraler Leitstand zeigt es den Zustand des Gesamt-
                                  systems an, z. B. Glasflüsse und Engpässe, Leistung, Pufferbelegung usw.
1.00 / 01-2016




                 A+W DynOpt                                                                           J-25
                 Mit A+W DynOpt arbeiten                                                                        Tutorial




                            A
                                           B         C




                 A A+W DynOpt-Editor                 B XOPT-ON Dynamics                C Zuschnitt-Übersicht

                 Abb. J-9       Programmdialoge für die Arbeiten mit A+W DynOpt


                                             Die Anzeigen und Dialoge müssen vom Anwender interpretiert werden. Da-
                                             durch wird A+W DynOpt einsehbar, und der Mitarbeiter weiß, in welchem Zu-
                                             stand sich die Produktion aktuell befindet.

                                                Beispiel: effektive Arbeitsweise mit A+W DynOpt

                                                Der Schichtleiter sieht, welche Glasarten in welchen Mengen in den
                                                Aufträgen stecken. Er erkennt, dass beispielsweise vom 8 mm VSG
                                                nur noch drei Scheiben geschnitten werden müssen, aber im
                                                späteren Verlauf der Aufträge weitere 20 Scheiben desselben Typs
                                                folgen werden.
                                                Also muss der entsprechende Auftrag mit diesen Scheiben in A+W
                                                DynOpt importiert werden, so dass das Programm diese Scheiben
                                                des gleichen Typs erkennt und den Zuschnitt der Scheiben des
                                                gleichen Typs zusammenzieht.
                                                Dazu müssen genügend Läufe importiert worden sein, so dass A+W
                                                DynOpt mit maximaler Ausbeute planen kann. Sind zu wenig Läufe
                                                im System, kann das Programm nur mit wenigen Daten planen, und
                                                die Ausbeute sinkt.
1.00 / 01-2016




                 J-26                                                                                     A+W DynOpt
                 Tutorial                                                                   Mit A+W DynOpt arbeiten




                                         A+W DynOpt Editor
                                         A+W DynOpt arbeitet zwar selbstständig im Hintergrund, die Eingangsdaten
                                         müssen jedoch manuell zur Verfügung gestellt werden. Dazu steht der Dialog
                                         A+W DynOpt Editor zur Verfügung, von dem aus Sie alle weiteren Dialoge er-
                                         reichen.
                                         Mit dem Editor geben Sie A+W DynOpt die Arbeitsmenge bekannt. Mit der
                                         Reihenfolge der importierten Läufe legen Sie deren Priorität bei der Abarbei-
                                         tung fest.


                                A                                   B                        C




                 D




                 E
                 F




                 A Läufe aus A+W Production                       D Details zu den ausgewählten Scheiben
                 B An A+W DynOpt übergebene Läufe                 E Einstellung zur Anzeige im Zeitstrahl
                 C XOPT-ON Dynamic Läufe                          F Dynamischer Zeitstrahl
                 Abb. J-10   A+W DynOpt-Editor


                                         Im oberen Teil des Dialogs importieren und priorisieren Sie Läufe. Im unteren
                                         Teil des Dialogs sehen Sie den dynamischen Zeitstrahl und die Status der je-
                                         weiligen Läufe.
1.00 / 01-2016




                 A+W DynOpt                                                                                      J-27
                 Mit A+W DynOpt arbeiten                                                                      Tutorial




                                       Status-Farben der Läufe im dynamischen Zeitstrahl:
                                       •   Grün: Scheiben des Laufs sind noch nicht optimiert. Status 0.
                                       •   Gelb: mindestens eine Scheiben des Clusters ist optimiert. Status 100.
                                       •   Blau: alle Scheiben des Clusters sind optimiert. Status 200.
                                           Wenn es keine Änderungen und keine neue Optimierung mehr gibt, wer-
                                           den die Scheiben so geschnitten.
                                       •   Hellblau: das gesamte Cluster ist geschnitten.

                                       Reihenfolge der Arbeiten
                                       Mit folgenden Arbeiten können Sie die dynamische Optimierung überwachen:
                                       •   Läufe in A+W DynOpt importieren.
                                       •   Überblick verschaffen:
                                           – Dynamischer Zeitstrahl im Dialog A+W DynOpt-Editor
                                           – Konfigurierte Dialoge in A+W Production Cockpit
                                           – Register XOPT-ON Dynamics
                                       •   Schneidcodes im Dialog Zuschnitt-Übersicht an die Schneidtische senden.

                                       Läufe importieren
                                       Importieren Sie genügend Läufe, damit A+W DynOpt optimal planen kann und
                                       der dynamische Zeitstrahl nicht leer läuft.

                                       Läufe priorisieren
                                       Im Dialog Laufreihenfolge bearbeiten ändern Sie die Priorisierung der Läufe.
                                       Ausschlaggebend für die Priorisierung ist die Beantwortung der Frage: Wel-
                                       che Scheiben müssen zuerst fertig werden?
                                       Dabei spielen die Geschwindigkeit der Schneidtische und die Glastypen eine
                                       Rolle, z. B. kann Float schneller geschnitten werden als VSG. A+W DynOpt
                                       greift automatisch für den VSG Zuschnittt weiter in die Zukunft. Der Planer
                                       muss nur darauf achten, dass er den Anteil an Läufen mit VSG etwas in der
                                       Priorisierung verteilt.
                                       Das VSG bekommt einen Vorsprung beim Schneiden, damit beide Glasarten
                                       rechtzeitig im Puffer landen und zur weiteren Verarbeitung an den Linien bereit
                                       stehen.

                                       Bruchscheiben
                                       Bruchscheiben werden von A+W DynOpt automatisch eingeschleust, sobald
                                       sie über einen Scanner an einem A+W Production-Terminal oder andere Pro-
                                       gramme gemeldet werden.
1.00 / 01-2016




                 J-28                                                                                   A+W DynOpt
                 Tutorial                                                         Mit A+W DynOpt arbeiten




                              Eilscheiben in zwei Schritten priorisieren
                              Wenn Sie Eilscheiben schnell durch die Produktion schleusen möchten, prio-
                              risieren Sie die Scheiben im Dialog Laufreihenfolge bearbeiten in zwei Schrit-
                              ten.
                              Sie sollten die Laufreihenfolge jeweils nur innerhalb desselben Status ändern,
                              also z.B. einen Lauf mit grünem Status bis maximal an die Spitze der grün
                              markierten Läufe ziehen. Wenn Sie einen Lauf über Statusgrenzen hinweg
                              verschieben, wirkt sich diese Änderung auf den gesamten Prozess aus.
                              A+W DynOpt kann eine Priorisierung unter Umständen ablehnen, wenn dies
                              zu Problemen beim Zuschnitt oder im Puffer führen würde.
                              Die Priorisierung von Läufen kann nicht durchgeführt werden, solange eine
                              Optimierung läuft.




                              Abb. J-11    Laufreihenfolge bearbeiten


                              In diesem Dialog bearbeiten Sie die Reihenfolge der Läufe.
                              Status-Farben der Läufe im Dialog Laufreihenfolge bearbeiten:
                              •   Grün: kein Cluster des Laufs kann aus dem Puffer abfließen.
                              •   Gelb: mindestens ein Cluster des Laufs kann aus dem Puffer abfließen.
                              •   Rot: alle Scheiben des Laufs können aus dem Puffer abfließen oder fließen
                                  bereits ab.
1.00 / 01-2016




                 A+W DynOpt                                                                            J-29
                 Mit A+W DynOpt arbeiten                                                                               Tutorial




                                             Erster Schritt
                                             Im ersten Schritt schieben Sie die Eilscheiben im Dialog Laufreihenfolge be-
                                             arbeiten an die gewünschte Stelle vor dem Zuschnitt.
                                             Sie können den Lauf bis an die Spitze des Status ziehen, zu dem er selbst ge-
                                             hört, also z. B. einen grün markierten Lauf an die Spitze der grün markierten
                                             Läufe.


                     Ausgang                                                                                Eingang




                                                                                                              t


                                     A              B        C                  D

                 A Dynamischer Puffer für geschnittene Scheiben             C Zuschnitt
                 B Geschnittene Custer (Tisch 1)                            D Eilscheibe
                 Abb. J-12    Priorisierung der Eilscheibe, Schritt 1




                                             Im Zeitstrahl wird der Lauf dann an der entsprechenden Stelle angezeigt. Der
                                             Lauf wird nun mit hoher Priorität behandelt. Gleichzeitig ist sichergestellt, dass
                                             die bestmögliche Optimierung von A+W DynOpt gewährleistet bleibt. Würde
                                             man einen Lauf sofort ganz vorne platzieren, hätte A+W DynOpt nicht mehr
                                             die Möglichkeit bestmöglich zu optimieren. Zusätzlich könnte der Ausfluß sto-
                                             cken.
1.00 / 01-2016




                 J-30                                                                                             A+W DynOpt
                 Tutorial                                                                        Mit A+W DynOpt arbeiten




                                             Zweiter Schritt
                                             Im zweiten Schritt verschieben Sie die geschnittenen Eilscheiben im Dialog
                                             Laufreihenfolge bearbeiten an die gewünschte Stelle nach dem Zuschnitt.
                                             Wenn der Lauf geschnitten ist, wird er rot markiert. Sie können ihn im zweiten
                                             Schritt der Priorisierung an die Spitze der rot markierten Läufe ziehen. Damit
                                             werden die Scheiben als nächste aus dem Puffer genommen und in die Linien
                                             eingeschleust.


                     Ausgang                                                                              Eingang




                                                                                                           t


                                     A                  B C                    D

                 A Geschnittene Eilscheibe im Puffer                       C Zuschnitt
                 B Geschnittene Eilscheibe
                 Abb. J-13    Priorisierte Eilscheibe


                                             Im Zeitstrahl wird der Lauf dann als geschnitten angezeigt und in den Puffer
                                             verschoben.
1.00 / 01-2016




                 A+W DynOpt                                                                                           J-31
                 Mit A+W DynOpt arbeiten                                                                   Tutorial




                                       Ergebnis verfolgen




                                       Abb. J-14   A+W Production Cockpit, Laufübersicht


                                       Die effektivste Anzeige über Läufe und einzelne Scheiben erhalten Sie im Re-
                                       gister Laufübersicht in A+W Production Cockpit. So können Sie verfolgen, wo
                                       sich die Scheiben befinden und die Priorisierung verfolgen.
1.00 / 01-2016




                 J-32                                                                                A+W DynOpt
                 Tutorial                                                                       Mit A+W DynOpt arbeiten




                                          A+W DynOpt Editor bedienen
                                          In dieser Lerneinheit erfahren Sie, wie Sie Läufe in A+W DynOpt importieren
                                          und die Priorität von Läufen bearbeiten.
                                          Zu diesen Themen gibt es folgende Handlungsanleitungen:
                                          •      “So importieren Sie Läufe in A+W DynOpt” auf Seite J-33
                                          •      “So ändern Sie die Priorität eines Laufs” auf Seite J-34


                                           So importieren Sie Läufe in A+W DynOpt
                                          1 Öffnen Sie den Dialog A+W DynOpt Editor.




                 Abb. J-15   Läufe importieren


                                          2 Markieren Sie in der Liste Freigegebene Läufe die Läufe, die Sie in A+W
                                            DynOpt importieren möchten.
                                          3 Klicken Sie auf die Schaltfläche [Pfeil nach rechts].
                                                 Die Läufe sind in die Liste XOPT-ON Dynamic Läufe und damit in A+W Dy-
                                                 nOpt importiert.
                                          4 Klicken Sie auf [OK], um den Dialog zu schließen.
1.00 / 01-2016




                 A+W DynOpt                                                                                       J-33
                 Mit A+W DynOpt arbeiten                                                                     Tutorial




                                        So ändern Sie die Priorität eines Laufs
                                       1 Öffnen Sie den Dialog A+W DynOpt Editor.
                                       2 Klicken Sie auf die Schaltfläche [Laufreihenfolge].




                                           Abb. J-16   Laufreihenfolge bearbeiten


                                       3 Markieren Sie die Läufe, deren Priorität Sie bearbeiten möchten.
                                       4 Klicken Sie auf die Schaltfläche [Pfeil nach oben] oder [Pfeil nach unten],
                                         um die Priorität der Läufe herauf- oder herabzustufen.
                                       5 Klicken Sie auf [OK], um den Dialog zu schließen.
1.00 / 01-2016




                 J-34                                                                                 A+W DynOpt
A+W DynOpt         N

             Partindex
                 Partindex                                                   Index




                 Index
                 A                             S
                 Auflösung J-18                Standard-Optimierung   J-15
                 Ausbeute J-15
                 Ausgang J-19                  T
                                               Timeline   J-19
                 B
                 Bruchscheiben                 Z
                 – DynOpt J-28                 Zeitstrahl J-19
                 – Panorama J-23               Zuschnitt
                                               – Übersicht J-25
                 D
                 DynOpt-Editor J-25, J-27
                 – bedienen J-33
                 – Bruchscheiben J-28
                 – Eilscheiben J-29
                 – Läufe importieren J-28
                 – priorisieren J-28
                 – Reihenfolge J-28

                 E
                 Eilscheiben J-29
                 Eingang J-19

                 F
                 Flexibilität   J-15

                 L
                 Läufe
                 – importieren J-28
                 – Optimierung J-17
                 – priorisieren J-28
                 Losgrößen
                 – Konflikt J-15

                 P
                 Panorama J-23
                 Produktionssequenzen   J-24
                 Puffer
                 – Belegung J-22
                 – System J-21

                 R
                 Reoptimierung J-18
1.00 / 01-2016




                 Restplatten J-23




                 A+W DynOpt                                                  N-37
                 Index      Partindex
1.00 / 01-2016




                 N-38    A+W DynOpt

