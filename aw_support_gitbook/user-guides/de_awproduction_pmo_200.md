---
title: "DE AWProduction PMO 2.00"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["DE_AWProduction_PMO_2.00"]
version: "1.0"
last_updated: "2025-12-10"
description: "Packmitteloptimierung        I                                deutsch                     A+W Production                                                                                                            Vorspann                                             Vorspann                                         In diesem Teil der Dokumentation finden Sie editorische Notizen.                                           Revisionsübersicht                                         Part"
source_file: "DE_AWProduction_PMO_2.00.pdf"
---


# DE AWProduction PMO 2.00

Packmitteloptimierung        I




                           deutsch




                A+W Production
                                                                                                           Vorspann




                                        Vorspann
                                        In diesem Teil der Dokumentation finden Sie editorische Notizen.


                                        Revisionsübersicht
                                        Part                     Beschreibung
                                        Version / Datum

                                        2.00 / 01-2023           Freien Editier-Modus ergänzt.

                                        1.02 / 01-2017           Produkt- und Firmennamen angepasst.

                                        1.01 / 07-2013           Vollständige Überarbeitung der ALCIM-Dokumentation
                                                                 und Anpassung auf A+W Production.

                                        1.00 / 03-2007           Ersterstellung



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
                                        Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbau-
                                        stufe von A+W Production.

                                        Urheberrechte
                                        © 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Her-
2.00 / 01-2023




                                        stellung von Kopien und der Übersetzung, bleiben vorbehalten.
                                        Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen ko-
                                        piert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen


                 A+W Production Packmitteloptimierung                                                             I-3
                 Vorspann




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
                            Zentrale@a-w.com
                            http://www.a-w.com
2.00 / 01-2023




                 I-4                                             A+W Production Packmitteloptimierung
                                                                                                                                                                 Inhalt




                                        Inhalt
                                        Vorspann ................................................................................................................. I-3
                                          Revisionsübersicht ............................................................................................... I-3
                                          Editorial ................................................................................................................ I-3
                                        Inhalt ........................................................................................................................ I-5

                                        Tutorial                                                                                                                   I-7
                                        Grundgedanke ......................................................................................................... I-9
                                        Allgemeines ........................................................................................................... I-10
                                        Stammdaten .......................................................................................................... I-13
                                          Optimierungsregeln (*.RUL-Datei) ..................................................................... I-13
                                          Einstellwerte (*.VAL-Datei) ................................................................................. I-13
                                            Parameter ....................................................................................................... I-14
                                        Anzeigen ................................................................................................................ I-19
                                          Packmittelgruppen-Anzeige ............................................................................... I-19
                                            Restriktionen ................................................................................................... I-20
                                        Optimierung ansehen ............................................................................................ I-23
                                          Ansichten ............................................................................................................ I-24
                                            3D-Ansicht ...................................................................................................... I-24
                                            Draufsicht ........................................................................................................ I-26
                                            Detail-Ansicht .................................................................................................. I-26
                                          Modi .................................................................................................................... I-31
                                            Vollbild-Modus ................................................................................................ I-31
                                            Bearbeitungs-Modus ....................................................................................... I-32
                                            Experten-Modus .............................................................................................. I-34
                                            Freier Editier-Modus ....................................................................................... I-35
                                          Zwischenablage ................................................................................................. I-39

                                        Softwarereferenz                                                                                                        I-65
                                        Menüs .................................................................................................................... I-67
                                         Regeln ................................................................................................................ I-69
                                         Werte .................................................................................................................. I-71
                                         Packmittelgruppen .............................................................................................. I-74
                                         Packmittelgruppen-Anzeige ............................................................................... I-77
                                           Summenzeile .................................................................................................. I-78
                                           Filterfunktion ................................................................................................... I-78
                                           Schaltflächen zur Schnellanwahl .................................................................... I-78
                                           Kontext-Menü bei markiertem Eintrag ............................................................ I-80
                                         PackView ............................................................................................................ I-83
                                         Menü-Zeile ......................................................................................................... I-84
                                         Symbol-Schaltflächen ......................................................................................... I-89
                                         Ansichten ............................................................................................................ I-93
                                         Gestellbezeichnung ändern ................................................................................ I-94
                                         Neue Gestell-Eigenschaften ............................................................................... I-95
                                         Eigenschaften der Kiste ändern ......................................................................... I-97
                                         Eigenschaften Referenz-Einheiten ..................................................................... I-99
                                         Info-Zeile am unteren Bildschirmrand .............................................................. I-101

                                        Partindex                                                                                                            I-103
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                                                                                I-5
                 Inhalt
2.00 / 01-2023




                 I-6      A+W Production Packmitteloptimierung
Packmitteloptimierung        I

                        Tutorial




                A+W Production
                 Tutorial                                                                              Grundgedanke




                                        Grundgedanke
                                        Die Packmitteloptimierung erspart Ihnen sowohl aufwändiges Umsortieren als
                                        auch das Zwischenlager. Sie richtet den gesamten Produktionsprozess auf
                                        die Direktverpackung und die bestmögliche Auslastung der Packmittel (Ge-
                                        stelle und Versandkisten) aus.
                                        In einer Produktion ohne Packmitteloptimierung (PMO) werden alle Einheiten,
                                        die aus der Produktion kommen, in einem Zwischenlager abgestellt. Danach
                                        müssen die Einheiten auf Transportgestelle verpackt werden, was mit aufwän-
                                        digen Sortierungen verbunden ist. Meist stehen die Einheiten im Zwischenla-
                                        ger nicht in der Reihenfolge zur Verfügung, wie sie für das Transportgestell
                                        benötigt werden. Es kann auch der Fall sein, dass das Transportgestell nach
                                        Kundenwünschen beladen werden muss, oder es muss eine bestimmte Tour-
                                        bzw. Abladereihenfolge eingehalten werden.
                                        Die Aufgabe der Packmitteloptimierung ist, die gewünschten Auftragspositio-
                                        nen unter Beachtung von Nebenbedingungen so auf Packmittel (Gestelle) zu
                                        verplanen, dass der Platzbedarf beim Transport minimal ist und Kundenwün-
                                        sche beim Gestellaufbau erfüllt werden. Die Strategie bei der Verplanung wird
                                        durch Packmittelregeln formuliert. Diese enthalten neben den Angaben zu
                                        physikalischen Eigenschaften (wie Höhe, Breite und Gewicht) auch kunden-
                                        spezifische Parameter für die zu verwendenden Packmittel (wie Anzahl der
                                        Stapel nebeneinander und übereinander).
                                        In der Packmittelplanung werden Aufträge in gemeinsam zu verpackende
                                        Gruppen (Packmittelgruppen) eingeteilt, z. B. gleicher Liefertermin, gleiche
                                        Tour, gleiche Lieferanschrift.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                              I-9
                 Allgemeines                                                                          Tutorial




                               Allgemeines
                               Dieses Kapitel gibt Ihnen einen Überblick, wie die Packmitteloptimierung
                               (PMO) aufgebaut ist und wie sie grundsätzlich arbeitet. Die Stammdaten der
                               Packmitteloptimierung sind komplex und es sind umfangreiche Kenntnisse
                               nötig, um die Packmitteloptimierung korrekt zu projektieren.
                               In der Packmitteloptimierung gibt es zwei getrennt zu behandelnde Bereiche
                               von Vorgaben:
                               •   Die physikalischen Bedingungen (Gestellregeln), die beim Versand einge-
                                   halten werden müssen (Gewicht, Anordnung der Stapel, Abstände, etc.).
                               •   Die von Endkunden gewünschte Behandlung seiner Auftragspositionen
                                   (gruppieren, sortieren, auf spezielle Gestelle stellen, etc.).
                               Für den Endkunden ist in den meisten Fällen die Abnahmereihenfolge wichtig,
                               in der die produzierten Einheiten von den Versandgestellen abgenommen
                               werden können. Je strenger die Vorgaben für diese Reihenfolge sind, desto
                               weniger Freiheit hat die Packmitteloptimierung bei der Verplanung der Gestel-
                               le. Das hat zur Folge, dass die Planungsdichte tendenziell schlechter sein
                               wird.
                               Häufig wird gewünscht, dass Einheiten gemeinsam abnehmbar sind. So sol-
                               len zum Beispiel alle Einheiten eines Auftrags gemeinsam abnehmbar sein.
                               Oder es sollen alle Einheiten einer Position hintereinander entladbar sein. Da-
                               bei ist noch nicht gesagt, dass solche gemeinsam abnehmbaren Einheiten
                               auch nahe beieinander auf den Gestellen stehen. Es könnte durchaus sein,
                               dass die Einheiten in verschiedenen Stapeln oder sogar auf verschiedenen
                               Gestellen stehen. Die Optimierung stellt aber immer sicher, dass keine ande-
                               ren Einheiten zunächst abgenommen werden müssen, um an alle gemeinsam
                               abnehmbaren Gläser heran zu kommen. Je mehr Freiheit die Optimierung bei
                               dieser Verplanung hat, desto besser sind die Planungsdichten auf den Gestel-
                               len, desto weniger Gestelle werden benötigt.
                               Eine Packmittelgruppe kann in Sets (etwa entsprechend der Aufträge) einge-
                               teilt sein. Das bedeutet, dass die in einem Set enthaltenen Positionen entla-
                               den werden können, ohne andere Positionen anzufassen. Dabei kann das Set
                               durchaus auf verschiedene Stapel oder Packmittel verteilt sein. Die Abladerei-
                               henfolge der Sets kann dabei von der Packmitteloptimierung selber bestimmt
                               oder auch vorgegeben werden. Es gibt auch die Möglichkeit die Sets so zu
                               planen, dass sie unabhängig voneinander in wahlfreier Reihenfolge entladen
                               werden können.
2.00 / 01-2017




                 I-10                                                A+W Production Packmitteloptimierung
                 Tutorial                                                                                 Allgemeines




                                        Stapel auf dem Gestell müssen eine baumförmige Struktur haben. Zum Bei-
                                        spiel ein großer Stapel zu Beginn gefolgt von maximal 2 weiteren Stapeln, vor
                                        denen wieder maximal 2 Stapel stehen dürfen. Das sieht von oben gesehen
                                        so aus (die Gestellrückwand ist grau gezeichnet):




                                                                    Gestellrückwand

                                        Abb. I-1     Gestellbeladung von oben gesehen


                                        Eine weitere Möglichkeit ist die Strukturierung einzelner Stapel durch Matri-
                                        zen. Eine Matrix ist ein Aufbau, der es erlaubt, mehrere Einheiten nebenein-
                                        ander und übereinander gleichzeitig zu platzieren. Dazu ist die Beachtung
                                        folgender Eigenschaften nötig:
                                        •   Alle Einheiten einer Reihe, bis auf die oberste Reihe, müssen die gleiche
                                            Höhe haben.
                                        •   Alle Einheiten einer Reihe müssen die gleiche Dicke haben.
                                        •   Die Gesamtbreite jeder Reihe muss kleiner oder gleich der Gesamtbreite
                                            der unteren Reihe sein.
                                        •   Die Dicke jeder Reihe muss kleiner oder gleich der Dicke der unteren Rei-
                                            he sein.
                                        •   Jede Reihe steht zentriert auf der unteren Reihe.
                                        Daher können in einem Stapel Einheiten nebeneinander und übereinander
                                        stehen. Das können Einheiten aus einer oder auch aus verschiedenen Auf-
                                        tragspositionen sein. Von vorne kann dann ein einzelner Stapel so aussehen:




                                                            (1/2)            (2/2)




                                                    (1/1)            (2/1)           (3/1)



                                        Abb. I-2     Matrixbeladung: Stapel von vorne gesehen
2.00 / 01-2017




                                        Die oberen Stapel stehen dabei immer zentriert auf den unteren.




                 A+W Production Packmitteloptimierung                                                            I-11
                 Allgemeines                                                                      Tutorial




                               Mit Matrizen kann man insbesondere erreichen, dass vor zwei Stapeln wieder
                               ein größerer Stapel steht (nicht baumförmig).




                                                        Gestellrückwand

                               Abb. I-3    Matrixbeladung von oben gesehen


                               Einheiten aus einer Position werden zunächst grundsätzlich nach Möglichkeit
                               zusammengehalten. Wenn eine Position wegen max. Gewicht oder Gestelltie-
                               fe nicht auf ein Gestell passt, wird sie geteilt.
2.00 / 01-2017




                 I-12                                              A+W Production Packmitteloptimierung
                 Tutorial                                                                               Stammdaten




                                        Stammdaten
                                        Für den Anwender sind im Umgang mit der Packmitteloptimierung zwei
                                        Stammdaten-Typen sichtbar:
                                        •   Optimierungsregeln (*.RUL-Datei): Die *.RUL-Dateien enthalten allgemei-
                                            ne Einstellungen, Angaben zu physikalischen Gestellen und zugehörige
                                            Belegungsregeln. Diese können z. B. je nach Kunde oder Auftrag verge-
                                            ben werden.
                                        •   Einstellwerte (*.VAL-Datei): Die *.VAL-Dateien ermöglichen kundenspezifi-
                                            sche Einstellwerte zu den Optimierungsregeln.
                                        Die *.RUL- und *.VAL-Dateien stehen dem Anwender zur Auswahl zur Verfü-
                                        gung. Geringfügige Modifikationen wie z. B. maximale Gestellbeladung kön-
                                        nen für eine bestimmte Packmittelgruppe vom Anwender durchgeführt
                                        werden.

                                            Weitere Stammdaten
                                            Darüber hinaus gibt es noch Gestellregeln, Verladeregeln und Regelzuwei-
                                            sungen. Diese Regeln werden durch die Firma A+W in Zusammenarbeit
                                            mit dem Anwender erarbeitet und gefüllt. Möchten Sie Veränderungen an
                                            der in Ihrem Hause implementierten Packmitteloptimierung vornehmen,
                                            halten Sie bitte unbedingt Rücksprache mit A+W, da es sonst zu uner-
                                            wünschten Ergebnissen kommen kann!


                                        Optimierungsregeln (*.RUL-Datei)
                                        Die *.RUL-Dateien enthalten die Gestellregeln. In den Gestellregeln wird be-
                                        schrieben, welche Packmittel mit welcher jeweiligen maximalen Anzahl und
                                        mit welchen Vorgaben zur Beladung geplant werden können. Das können Ge-
                                        stelle (A-Bock, L-Bock) oder auch Kisten (in Standard- oder Individualmaßen)
                                        sein.
                                         Softwarereferenz, “Regeln” auf Seite I-69



                                        Einstellwerte (*.VAL-Datei)
                                        Die *.VAL-Dateien enthalten die Zuweisungen der kundenspezifischen Pack-
                                        mittelparamtern (*.VAL-Dateien) zu den Gestellregeln. Theoretisch kann für
                                        jede *.RUL-Dateil eine eigene *.VAL-Datei angelegt werden, es sollte aber der
                                        dann notwendige Pflegeaufwand nicht außer Acht gelassen werden.
                                         Softwarereferenz, “Werte” auf Seite I-71
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                           I-13
                 Stammdaten                                                                          Tutorial




                              Parameter
                              Zum Beladen der Gestelle arbeitet die Packmitteloptimierung mit unterschied-
                              lichen Parametern. Im Anschluss finden Sie nähere Erläuterungen zu einzel-
                              nen, häufig verwendeten Parametern. Die in Ihrem Hause verwendeten
                              Parameter können aufgrund Ihrer individuellen Anforderungen davon abwei-
                              chen.

                              Name des Parameters: Sets in Stapeln zusammenstellen.
                              Erläuterung: Mit diesem Wert legen Sie fest, wie Sets in Stapeln (z. B. Aufträ-
                              ge) zusammen gestellt werden.
                              Mögliche Werte:
                              •   0-Nein, freie Optimierung,
                              •   1-Mono,
                              •   2-Multi,
                              •   3-Peripher.
                              Mono:
                              Im Mono-Modus kann jedes Set entladen werden, ohne Einheiten aus einem
                              anderen Set anzufassen. Alle Sets können in jeder gewünschten Reihenfolge
                              entladen werden. Daher steht in jedem Stapel nur ein Set.




                                                   Set 2                         Set 1



                                                 Set 1                            Set 2




                              Abb. I-4     Gestell 1




                                                Set 2                            Set 3



                                              Set 3                                 Set 3




                              Abb. I-5     Gestell 2
2.00 / 01-2017




                 I-14                                               A+W Production Packmitteloptimierung
                 Tutorial                                                                              Stammdaten




                                        Multi:
                                        Der Multi-Modus gleicht dem Mono-Modus, jedoch kann jedes Set in maximal
                                        einem Stapel mit anderen Sets gemischt stehen. In einem gemischten Stapel
                                        steht jedes Set blockweise für sich (getrennt von den anderen Sets).




                                                            Set 2                        Set 1



                                                        Set 1                            Set 2




                                        Abb. I-6    Gestell 1




                                                        Set 2                            Set 3



                                                        Set 3                            Set 3




                                        Abb. I-7    Gestell 2


                                        Peripher:
                                        Im Peripher-Modus kann jedes Set entladen werden, ohne Einheiten aus an-
                                        deren Sets anzufassen. Die Reihenfolge der Entladung steht aber fest (entwe-
                                        der durch PMO oder den Anwender). Daher kann es mehr als ein Set pro
                                        Stapel geben.




                                                                                         Set 1
                                                            Set 2

                                                                                         Set 2
                                                        Set 1
2.00 / 01-2017




                                        Abb. I-8    Gestell 1




                 A+W Production Packmitteloptimierung                                                          I-15
                 Stammdaten                                                                     Tutorial




                                             Set 2                           Set 2

                                                                             Set 3
                                             Set 3

                                                                             Set 2


                              Abb. I-9    Gestell 2


                              Frei:
                              Im Freien-Modus können Sets und Positionen nicht zusammen entladen wer-
                              den. Die Aufträge stehen gemischt, um die höchste Packdichte zu erreichen.




                                                                              Set 1
                                                  Set 2

                                                                              Set 2
                                             Set 1



                              Abb. I-10   Gestell 1




                                                                              Set 2
                                              Set 2

                                                                             Set 3
                                             Set 3

                                                                             Set 2


                              Abb. I-11   Gestell 2
2.00 / 01-2017




                 I-16                                            A+W Production Packmitteloptimierung
                 Tutorial                                                                               Stammdaten




                                        Name des Parameters: Sets bestehen aus.
                                        Erläuterung: Mit diesem Wert bestimmen Sie, wie Sets gebildet werden. Sie
                                        können Sets nach Aufträgen, nach Kommissionen oder aber nach Touren bil-
                                        den.
                                        Mögliche Werte:
                                        •   1=Auftrag,
                                        •   2=Kommission,
                                        •   3=Tour.

                                        Name des Parameters: Sets auf Gestellen zusammenhalten?
                                        Erläuterung: Mit diesem Wert bestimmen Sie, ob und wenn ja, wie die Sets auf
                                        den Gestellen zusammen gehalten werden. 0 bedeutet, dass die Sets nicht
                                        auf Gestellen zusammen gehalten werden. Bei einer 1 werden die Sets auf ei-
                                        nem Gestell zusammen gehalten und bei einer 2 auf maximal zwei Gestellen.
                                        Mögliche Werte:
                                        •   0=nein,
                                        •   1=ein Gestell,
                                        •   2=zwei Gestelle.

                                        Name des Parameters: Sets sortiert entladen?
                                        Erläuterung: Mit diesem Wert bestimmen Sie, ob und wenn ja, wie die Sets
                                        entladen werden sollen. Standardmäßig ist dieser Eintrag mit 0 vorbelegt.
                                        D. h. die Sets werden nicht sortiert.
                                        Mögliche Werte:
                                        •   0=nein,
                                        •   1=Sets aufsteig. ++,
                                        •   2=Set absteig. --.

                                        Name des Parameters: Maximales Gewicht für alle Gestelltypen
                                        Erläuterung: Der hier eingetragene Wert kennzeichnet das maximale Gewicht
                                        aller Gestelltypen dieser Packmittelgruppe. Der Wert ist in kg anzugeben.

                                        Name des Parameters: Maximale Anzahl der Stapel aufeinander
                                        (Standard=1)
                                        Der hier eingetragene Wert besagt, wie viele Stapel aufeinander gestellt wer-
                                        den dürfen. Standardmäßig ist der Wert 1 eingetragen. Das bedeutet, dass
                                        keine Stapel aufeinander stehen dürfen. Die größtmögliche Anzahl aufeinan-
                                        der stehender Stapel ist 5.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                           I-17
                 Stammdaten                                                                         Tutorial




                              Name des Parameters: Maximaler Überstand links/rechts (Stan-
                              dard: 100 mm)
                              Erläuterung: Dieser Wert kennzeichnet den maximalen Gestellüberstand. Der
                              hier eingetragene Wert wirkt sowohl links als auch rechts. Standardmäßig ist
                              der Wert 100 eingetragen. Das bedeutet, dass der Überstand auf der rechten
                              und auf der linken Gestellseite 100 mm ist. Die größt mögliche Wert ist 1000
                              (1000 mm).

                              Name des Parameters: Maximales Seitenverhältnis für aufrechte
                              Scheiben (Standard = 3.0)
                              Erläuterung: Bei diesem Wert handelt es sich um den Minimalwert des Ver-
                              hältnisses zwischen größeren/kleinerem Scheibenmaß, ab welchem die
                              Scheiben liegend platziert werden. Beispiel: Bei einer Vorgabe von 2 wird die
                              Scheibe 2500/1000 liegend platziert und die Scheibe 1500/1000 stehend.
                              Standardmäßig ist der Wert 3 eingetragen. Der größt mögliche Wert ist 5. Eine
                              1 bewirkt, dass alle Scheiben auf die längere Seite gedreht werden.

                              Name des Parameters: Max. Seitenverhältnis für aufrechte Schei-
                              ben beim Aufeinanderstapeln (Std=2.0)
                              Erläuterung: Bei diesem Wert handelt es sich um das maximale Seitenverhält-
                              nis einer Einheit beim Aufeinanderstapeln, also wenn die Einheit auf einer an-
                              deren Einheit steht. Der Parameter wirkt nur dann, wenn er kleiner ist als der
                              Parameter Maximales Seitenverhältnis für aufrechte Scheiben.
2.00 / 01-2017




                 I-18                                              A+W Production Packmitteloptimierung
                 Tutorial                                                                                            Anzeigen




                                        Anzeigen
                                        Die Packmitteloptimierung verfügt über eine eigene Anzeige, die Ihnen die
                                        Packmittelgruppen anzeigt, die Sie gebildet haben.


                                        Packmittelgruppen-Anzeige
                                        Die Packmittelgruppen-Anzeige öffnen Sie entweder über das Menü Anzeigen
                                        > Packmittelgruppen-Anzeige oder aber über die Symbol-Schaltfläche.




                                        Abb. I-12           Symbol-Schaltfläche Packmittelgruppen-Anzeige


                                            A       B




                                                                                                                            C




                                                                                                                            D




                                                        F     E
                                        A Register                                      D Schaltflächen zur Schnellanwahl
                                        B Tabellenspalte                                E Summenzeile
                                        C Tabellenkopf                                  F Filterfunktion
                                        Abb. I-13           Packmittelgruppen-Anzeige


                                        Die Packmittelgruppen-Anzeige gibt Ihnen einen Überblick zu den bereits ge-
                                        bildeten Packmittelgruppen. Packmittelgruppen können Sie über das Kontext-
                                        Menü folgender Anzeigen bilden:
                                        •       Auftrags-Anzeige
                                        •       Bearbeitungs-Anzeige
                                        •       Detail-Anzeige
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                                       I-19
                 Anzeigen                                                                                                      Tutorial




                                                Über die Register können Sie sich die Packmittelgruppen-Anzeige grob struk-
                                                turieren. Innerhalb der Register stehen Ihnen zur weiteren Unterteiltung Tabel-
                                                lenspalten zur Verfügung. Ferner können Sie sich Filter anlegen, um die
                                                Anzeige für bestimmte Situationen noch weiter einzuschränken. Bsp.: Inner-
                                                halb der Tabellenspalte Packmittel können Sie nach einzelnen Packmittel-
                                                gruppen filtern. Über beliebig viele Filterfunktionen haben Sie so die
                                                Möglichkeit, die Anzeige Ihren speziellen Bedürfnissen anzupassen.
                                                Informationen zu den Filtern und der Summenzeile finden Sie im Part Grob-
                                                planung.
                                                 Grobplanung: Softwarereferenz, “Filter-Definition” auf Seite E-131
                                                Die Schaltflächen zur Schnellanwahl können in den einzelnen Anzeigen unter-
                                                schiedlich sein. Das hängt davon ab, welche Funktion in welcher Anzeige zur
                                                Verfügung steht. Die Schaltflächen aktivieren Sie, indem Sie einen Eintrag
                                                markieren. In der Packmittelgruppen-Anzeige haben Sie für einen oder meh-
                                                rere markierte Einträge schnellen Zugriff auf:
                                                •     Laufbildung: Es öffnet sich der Dialog Lauf-Bildung.
                                                       Grobplanung: Softwarereferenz, “Lauf-Bildung” auf Seite E-90
                                                •     Glasarten: Es öffnet sich der Dialog Glasarten-Anzeige.
                                                       Grobplanung: Softwarereferenz, “Glasarten” auf Seite E-110
                                                •     Details: Es öffnet sich der Dialog Detail-Anzeige.
                                                       Grobplanung: Softwarereferenz, “Details” auf Seite E-113


                                                Restriktionen
                                                Über das Kontext-Menü der Packmittelgruppen-Anzeige haben Sie die Mög-
                                                lichkeit, Packmittelgruppen zu bearbeiten. D .h. Sie können Packmittelgrup-
                                                pen verschieben, löschen und ändern. Die einzelnen Funktionen sind jedoch
                                                abhängig vom Status der Packmittelgruppe. So ist es z. B. nicht möglich, eine
                                                bereits feingeplante Packmittelgruppe zu löschen, da die Feinplanung dann
                                                bereits mit den Ergebnissen der Packmittelgruppe gearbeitet hat.
                                                Die folgende Tabelle zeigt Ihnen, welche Packmittelgruppe Sie in welchem
                                                Status bearbeiten können.


                 Status     Erläuterung                PMG         PMG           PMG           Optimieren   Optimierung   Opti-
                                                       ändern      verschiebe    löschen                    ansehen       mierung
                                                                   n                                                      zurück-
                                                                                                                          setzen

                 50         zur Optimierung            Ja /        Ja / Nein1)   Ja /          Ja           Nein          Ja
                            freigegeben                Nein1)                    Nein1)

                 75         wird gerade                Nein        Nein          Nein          Nein         Nein          Nein
                            hintergrundoptimiert

                 80         Optimierung                Ja          Ja            Ja            Ja           Nein          Ja
                            fehlerhaft

                 100        ist packmitteloptimiert    Ja / Nein   Ja / Nein     Ja / Nein     Ja           Ja            Ja
2.00 / 01-2017




                 >100       ist feingeplant            Nein        Nein          Nein          Nein         Ja            Nein

                 Tab. I-1        Status der Packmittelgruppen


                 I-20                                                                        A+W Production Packmitteloptimierung
                 Tutorial                                                                                      Anzeigen




                                        1) Felder, die mit Ja / Nein belegt sind, sind entweder bereits zur Optimierung
                                        freigegeben oder wurden bereits packmitteloptimiert. Hier wird der Anwendern
                                        explizit gefragt, ob er Änderungen vornehmen möchte.


                                         So bilden Sie Packmittelgruppen
                                        Die Vorgehensweise zum Bilden von Packmittelgruppen ist für alle Anzeigen
                                        (Aufträge, Bearbeitungen, etc.) gleich. Wir erläutern die Vorgehensweise des-
                                        halb nur einmal am Beispiel der Anzeige Aufträge.
                                        1 Öffnen Sie die Anzeige Aufträge entweder über das Menü Anzeigen > Auf-
                                          träge oder über die entsprechende Schaltfläche.
                                            Konventionen, “Pool-Anzeige” auf Seite A-80
                                        2 Selektieren Sie den bzw. die Aufträge, mit denen Sie eine Packmittelgrup-
                                          pe bilden möchten.
                                        3 Öffnen Sie das Kontext-Menü und wählen Sie Packmittelgruppe bilden
                                        4 Es öffnet sich der Dialog Packmittelgruppen.
                                        5 Geben Sie im Feld Packmittelhauptgruppe den Namen für die Packmittel-
                                          hauptgruppe an.
                                            Softwarereferenz, “Packmittelhauptgruppe” auf Seite I-74
                                        6 Geben Sie im Feld Packmittelgruppe den Namen für die Packmittelgruppe
                                          an.
                                            Softwarereferenz, “Packmittelgruppe” auf Seite I-75
                                        7 Wählen Sie aus der Kombobox Packmittelregel die entsprechende Regel
                                          aus.
                                            Softwarereferenz, “Packmittelregel” auf Seite I-75
                                        8 Geben Sie im Feld Beschreibung eine weitere Bezeichnung für die Pack-
                                          mittelgruppe an.
                                            Softwarereferenz, “Beschreibung” auf Seite I-75
                                        9 Aktivieren oder deaktivieren Sie die Checkbox Positionen von Optimierung
                                          ausschließen.
                                            Softwarereferenz, “Positionen von Optimierung ausschließen” auf Seite I-75
                                        10 Aktivieren oder deaktivieren Sie die Checkbox Mehrere Produktionslinien
                                           zusammenfassen.
                                            Softwarereferenz, “Mehrere Produktionslinien zusammenpacken” auf Seite I-75
                                        11 Ändern Sie bei Bedarf die VAL-Einstellungen.
                                        12 Betätigen Sie die Schaltfläche [OK].
                                        13 Der bzw. die selektieren Aufträge werden aus der Anzeige Aufträge ent-
                                           fernt. Sie finden den bzw. die Aufträge unter der soeben vergebenen Pack-
                                           mittelhauptgruppe in der Anzeige Packmittel.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                               I-21
                 Anzeigen                                                                       Tutorial




                             So starten Sie die Optimierung für eine Packmittelgruppe
                            1 Öffnen Sie die Anzeige Packmittel entweder über das Menü Anzeigen >
                              Packmittel oder über die entsprechende Schaltfläche.
                                Konventionen, “Packmittelgruppen-Anzeige” auf Seite A-80
                            2 Selektieren Sie den bzw. die Packmittelgruppe, die Sie optimieren möch-
                              ten.
                            3 Öffnen Sie das Kontext-Menü und wählen Sie PMG optimieren.
                            4 Die Optimierung wird gestartet.


                             So nehmen Sie Änderungen an den Parametern einer bestehenden
                              Packmittelgruppe vor
                            1 Öffnen Sie die Anzeige Packmittel entweder über das Menü Anzeigen >
                              Packmittel oder über die entsprechende Schaltfläche.
                                Konventionen, “Packmittelgruppen-Anzeige” auf Seite A-80
                            2 Selektieren Sie den bzw. die Packmittelgruppe, an der Sie Änderungen
                              vornehmen möchten.
                            3 Öffnen Sie das Kontext-Menü und wählen Sie PMG verwalten > Parameter
                              ändern.
                            4 Es öffnet sich der Dialog Packmittelgruppen. Änderungen, die Sie zu die-
                              sem Zeitpunkt vornehmen können, beziehen sich auf die Felder
                               •   Packmittelregel
                               •   Beschreibung
                               •   Positionen von Optimierung ausschließen
                               •   Mehrere Produktionslinien zusammenpacken
                               •   VAL.
                            5 Wählen Sie aus der Kombobox Packmittelregel die entsprechende Regel
                              aus.
                                Softwarereferenz, “Packmittelregel” auf Seite I-75


                            Weitere Informationen zu Packmittelgruppen
                             Tutorial, “Packmittelgruppen-Anzeige” auf Seite I-19
                             Softwarereferenz, “Packmittelgruppen” auf Seite I-74


                            Weitere Informationen zur Packmittelgruppen-Anzeige
                             Softwarereferenz, “Packmittelgruppen-Anzeige” auf Seite I-77
                             Konventionen, “Bedienoberfläche” auf Seite A-77
                             Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2017




                 I-22                                              A+W Production Packmitteloptimierung
                 Tutorial                                                                              Optimierung ansehen




                                             Optimierung ansehen
                                             Nach Durchführung der Packmitteloptimierung können Sie sich, in einer drei-
                                             dimensionalen Ansicht, die Ergebnisse als Vorschau anzeigen lassen. Ergeb-
                                             nisse bedeutet: Wie werden die Einheiten auf dem Transportgestell stehen?
                                             Sie können in dieser Ansicht die optimierten Gestelle auch mit wenigen Maus-
                                             klicks umpacken. Die Software zur Visualisierung der Packmittelergebnisse
                                             heißt PackView.


                            A   B   C                                  D




                 I




                                                                                                                 E




                                        H
                                                                 G            F
                 A   Menü-Zeile                                      G
                                                                     H Gesamtgewicht in kg (Vorder- und Rückseite)
                 B   Symbol-Schaltflächen                            I Ausdehnung der Gesamtbeladung auf der
                 C   3D-Ansicht                                        aktuellen Gestellseite: Breite , Höhe ,
                 D   Draufsicht                                        Tiefe 
                 E   Detail-Ansicht der Einheit                      J Experten-Modus, Einstellräder für Nahsicht.
                 F   Gewichtsverteilung auf linker und rechter
                     Gestellseite
                 Abb. I-14      PackView
2.00 / 01-2017




                                             PackView startet nach einer erfolgreich durchgeführten Optimierung automa-
                                             tisch.


                 A+W Production Packmitteloptimierung                                                                 I-23
                 Optimierung ansehen                                                                          Tutorial




                                       Weitere Informationen zur Visualisierung
                                        Softwarereferenz, “PackView” auf Seite I-83



                                       Ansichten
                                       PackView verfügt über folgende Ansichten:
                                       •   3D-Ansicht
                                       •   Draufsicht
                                       •   Detail-Ansicht
                                       In welcher der drei Ansichten Sie sich momentan befinden, sehen Sie an der
                                       gelben Umrandung der entsprechenden Ansicht. Mit der Maus können Sie
                                       einzelne Einheiten auswählen. Wenn Sie in der 3D-Ansicht eine Einheit aus-
                                       wählen, wird diese Einheit sowohl in der Draufsicht als auch in der Detail-An-
                                       sicht in Rot dargestellt. In welcher Ansicht Sie sich auch befinden, eine
                                       ausgewählte Einheit wird grundsätzlich auch in den anderen Ansichten in Rot
                                       hervorgehoben.


                                       3D-Ansicht


                                       A




                                                                                            B




                                                                                            C


                                       A Aktuelle Gestellseite                 C Linke, untere Ecke (Bezugspunkt für
                                       B Ausgewählte Einheit                     die Rückseite)

                                       Abb. I-15    3D-Ansicht


                                       Die 3D-Ansicht ermöglicht Ihnen die dreidimensionale Sicht beider Seiten ei-
                                       nes Gestells. Welche Gestellseite angezeigt wird, sehen Sie an der roten Zahl
                                       in der linken, oberen Ecke der Ansicht.
2.00 / 01-2017




                 I-24                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                         Optimierung ansehen




                                        Um die Gestellseite zu wechseln, stehen Ihnen folgende Möglichkeiten zur
                                        Verfügung:
                                        •   Öffnen Sie im Menü Ansicht den Menüpunkt Seitenansicht wechseln.
                                        •   Betätigen Sie auf Ihrer Tastatur die <Leertaste>.
                                        •   Betätigen Sie die Symbol-Schaltfläche.




                                            Abb. I-16   Gestellseite wechseln


                                        Sie können sich ein Gestell aus mehreren Blickwinkeln anzeigen lassen. Die-
                                        se Blickwinkel werden in PackView als Kamera-Positionen bezeichnet. Die
                                        oben gezeigte Abbildung (Tutorial, “3D-Ansicht” auf Seite I-24) stellt die so ge-
                                        nannte Ausgangs-Position der Kamera dar. Aus dieser Kamera-Position her-
                                        aus wird die 3D-Ansicht standardmäßig geöffnet. Um zur nächsten Kamera-
                                        Position zu wechseln, stehen Ihnen folgende Möglichkeiten zur Verfügung:
                                        •   Öffnen Sie im Menü Ansicht den Menüpunkt Nächste Kamera-Position
                                            oder Vorhergehende Kamera-Position.
                                        •   Aktivieren Sie auf Ihrer Tastatur den Nummernblock über die Taste <Num>.
                                            Betätigen Sie im Bereich des Nummernblocks die Taste <+> oder <->.
                                        •   Betätigen Sie die Symbol-Schaltflächen.

                                                             Nächste Kamera-Position.

                                                             Vorhergehende Kamera-Position.

                                            Abb. I-17   Kamera-Positionen wechseln


                                        In der 3D-Ansicht können Sie Einheiten über die Funktion Kopieren verschie-
                                        ben. Das bedeutet, Sie markieren eine Einheit, kopieren sie, verschieben sie
                                        an die gewünschte Stelle und fügen sie dort ein. Sie haben auch die Möglich-
                                        keit, Einheiten nach dem Kopieren an ihrem Platz zu drehen.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                               I-25
                 Optimierung ansehen                                                                           Tutorial




                                       Draufsicht

                                       A


                                                                                                     B




                                       A Linke, untere Ecke (Bezugspunkt)      B Ausgewählte Einheit
                                       Abb. I-18    Draufsicht


                                       Die Draufsicht zeigt Ihnen das Gestells von oben. Die rote Einheit ist die aktu-
                                       ell ausgewählte Einheit.
                                       Sie können in der Draufsicht, wie auch in der 3D-Ansicht Einheiten über die
                                       Funktion Kopieren verschieben oder an ihrem Platz drehen.


                                       Detail-Ansicht
                                       Die Detail-Ansicht zeigt Ihnen tabellarisch, wie die Auftragspositionen auf den
                                       Gestellen stehen. Die in der Tabelle an oberster Position stehende Einheit ist
                                       die Einheit, die auf dem Gestell an der Gestellrückwand steht. Die in der Ta-
                                       belle an letzter Position stehende Einheit ist die auf dem Gestell an vorderster
                                       Stelle stehende Einheit, d. h. die Tabelle ist in Beladereihenfolge sortiert.


                                                                                                                    A
                                                                                                                    B




                                       A Tabellenkopf                          B Tabellenspalte
                                       Abb. I-19    Detail-Ansicht
2.00 / 01-2017




                 I-26                                                        A+W Production Packmitteloptimierung
                 Tutorial                                                                        Optimierung ansehen




                                        Der Tabellenkopf enthält die Spalten:
                                        •   Gestell#, unterteilt in
                                            – Seite
                                            – Stapel
                                        •   Gestellbeschreibung, unterteilt in
                                            – Anzahl
                                            – Reihe
                                        •   Gestell-ID, unterteilt in
                                            – Fläche [m2]
                                            – Vert. Stapel
                                        •   Typ, unterteilt in
                                            – Gewicht [kg]
                                            – Anzahl
                                        •   PM-Gruppe, unterteilt in
                                            – Auftrags-Nr.
                                        •   Größe [mm], unterteilt in
                                            – Positions-Nr.
                                            – Größe [mm]
                                            – Gewicht [kg]
                                            – Produktions-Linie

                                        Erläuterung des Tabellenkopfes und der Tabellenspalten

                                        Gestell# In diesem Feld wird das für die Packmitteloptimierung aktuelle Ge-
                                        stell mit den für diese Packmitteloptimierung gesamten Gestellen angezeigt.
                                        Bsp.: 1/3 bedeutet, dass die Packmittelgruppe insgesamt 3 Gestelle dieses
                                        Gestelltyps umfasst und das erste Gestell angezeigt wird. Die aktuelle Ge-
                                        stell#/Gesamtzahl finden Sie im Fenstertitel ganz oben.

                                        Seite In diesem Feld steht die Gestellseite, die aktuell angezeigt wird. Mögli-
                                        che Werte:
                                        • 1: Folgende Einheiten stehen auf der 1. Gestellseite.
                                        • 2: Folgende Einheiten stehen auf der 2. Gestellseite.

                                        Stapel Dieses Feld steht in direktem Zusammenhang mit dem Feld Seite und
                                        zeigt Ihnen, in welchem Stapel sich die Einheit dieser Tabellenzeile befindet.
                                        Steht in dem Feld eine 1, befindet sich die Einheit im ersten Stapel auf dieser
                                        Seite des Gestells. Steht in dem Feld eine 2, befinden sich die Einheit im zwei-
                                        ten Stapel auf dieser Seite des Gestells. Die Anzahl der Stapel ist abhängig
                                        von der Gestellgröße und der Einheitengröße. Bei sehr kleinen Einheiten pas-
                                        sen mehr Stapel auf das Gestell als bei großen Einheiten.
                                        Beispiel:
                                        Auf der abgebildeten Gestellseite befinden sich insgesamt zwei Stapel.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                              I-27
                 Optimierung ansehen                                                                         Tutorial




                                       Bei der markierten Einheit handelt es sich um die erste Reihe (an der Gestell-
                                       rückwand) des ersten (vom Bezugspunkt aus gesehen!) Stapels:




                                       Abb. I-20    1. Stapel, 1. Reihe


                                       Die nächste Abbildung zeigt die erste Reihe (an der Gestellrückwand) des
                                       zweiten (vom Bezugspunkt aus gesehen!) Stapels:




                                       Abb. I-21    2. Stapel, 1. Reihe
2.00 / 01-2017




                 I-28                                                       A+W Production Packmitteloptimierung
                 Tutorial                                                                     Optimierung ansehen




                                        Vor dem zweiten Stapel stehen wiederum Reihen. Die nächste Abbildung
                                        zeigt die zweite Reihe des ersten Stapels:




                                        Abb. I-22   1. Stapel, 2. Reihe


                                        Die nächste Abbildung zeigt eine Einheit der zweiten Reihe des zweiten Sta-
                                        pels:




                                        Abb. I-23   2. Stapel, 2. Reihe
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                          I-29
                 Optimierung ansehen                                                                            Tutorial




                                       Gestellbeschreibung Der Inhalt des Feldes kommt aus den PMO-Stammda-
                                       ten und zeigt Ihnen den dort vergebenen Namen für das Gestell.
                                        Softwarereferenz, “Packmittelhauptgruppe” auf Seite I-74

                                       Anzahl In diesem Feld sehen Sie, wie viele einzelne Einheiten sich insge-
                                       samt auf der aktuellen Seite des Gestells befinden.
                                        Tutorial, “Seite” auf Seite I-27

                                       Reihe In diesem Feld sehen Sie, wie viele Stapel voreinander stehen. An der
                                       Gestellrückwand steht z.B. ein großer Stapel, gefolgt von 2 kleineren Stapeln.

                                       Gestell-ID In diesem Feld sehen Sie die aktuell angezeigte Gestell-ID. Die
                                       hier stehende Zahl ist identisch mit der links des Schrägstriches stehende Zahl
                                       des Feldes Gestell#.
                                        Tutorial, “Gestell#” auf Seite I-27

                                       Fläche [m2] In diesem Feld sehen Sie, wie viele Quadratmeter Einheiten
                                       sich auf der betreffenden Seite des Gestells befinden.
                                        Tutorial, “Seite” auf Seite I-27

                                       Vert. Stapel In diesem Feld sehen Sie, wie viele vertikale Stapel übereinan-
                                       der stehen.

                                       Typ In diesem Feld können Sie sehen, um welchen Abstellplatztyp es sich
                                       handelt. Mögliche Werte:
                                       • A = A-Bock
                                       • L = L-Bock
                                       • Box = Kiste

                                       Gewicht [kg] In diesem Feld sehen Sie, wie viele Kilogramm Glas sich auf
                                       der betreffenden Seite des Gestells befinden.
                                        Tutorial, “Seite” auf Seite I-27

                                       Anzahl In diesem Feld sehen Sie, wie viele Einheiten eine Position hat und
                                       welche Einheit die aktuelle ist. Beispiel: 1/2 bedeutet, dass die Position 2 Ein-
                                       heiten hat und die betreffende Zeile eine davon auflistet.

                                       PM-Gruppe Dieses Feld zeigt Ihnen die Packmittelhauptgruppe und die
                                       Packmittelgruppe. Der Inhalt des Feldes kommt aus dem Dialog Packmittel-
                                       gruppen, Felder Packmittelhauptgruppe und Packmittelgruppe.
                                        Softwarereferenz, “Packmittelhauptgruppe” auf Seite I-74
                                        Softwarereferenz, “Packmittelgruppe” auf Seite I-75

                                       Auftrags-Nr. Dieses Feld zeigt Ihnen die vom Auftragsbearbeitungssystem
                                       übergebene Auftrags-Nr. des Kunden.

                                       Positions-Nr. Dieses Feld bezieht sich auf das Feld Auftrags-Nr. und zeigt
                                       Ihnen die entsprechende Positions-Nr. zu der Auftrags-Nr.
2.00 / 01-2017




                                       Größe [mm] Dieses Feld zeigt Ihnen die Abmessungen der aktuellen Einhei-
                                       tenposition in mm.



                 I-30                                                          A+W Production Packmitteloptimierung
                 Tutorial                                                                         Optimierung ansehen




                                        Gewicht [kg] Dieses Feld zeigt Ihnen das Gewicht der aktuellen Einheiten-
                                        position in kg.

                                        Produktions-Linie Dieses Feld zeigt Ihnen, auf welcher Produktions-Linie
                                        die jeweilige Einheitenposition gefertigt wird. Die Daten kommen aus der Ma-
                                        schinenzuordnung.
                                        Für spezielle Anforderungen ist die Anzahl und der Inhalt der gezeigten Spal-
                                        ten konfigurierbar. Nähere Information hierzu erhalten Sie von der A+W Soft-
                                        ware GmbH.


                                        Modi
                                        In PackView können Sie in drei unterschiedlichen Modi arbeiten. In Abhängig-
                                        keit von dem jeweiligen Modus stehen Ihnen unterschiedliche Werkzeuge zur
                                        Verfügung.
                                        •   Vollbild-Modus
                                        •   Bearbeitungs-Modus
                                        •   Experten-Modus


                                        Vollbild-Modus
                                        PackView befindet sich nach dem Start im Vollbild-Modus. Sie können mit der
                                        Maus eine Scheibe markieren, indem Sie entweder in der 3D-Ansicht oder der
                                        Draufsicht eine Einheit anklicken oder aber eine Position aus der Detail-An-
                                        sicht wählen. Die ausgewählte Einheit wird sowohl in der 3D-Ansicht als auch
                                        der Draufsicht in roter Farbe dargestellt. In der Detailansicht befindet sich ein
                                        roter Rahmen um die ausgewählte Einheit.




                                        Abb. I-24    Vollbild-Modus
2.00 / 01-2017




                                        Im Vollbild-Modus haben Sie Zugriff auf die unterschiedlichen Kamera-Positi-
                                        onen. Durch Betätigen der jeweiligen Schaltfläche schwenkt das Gestell in der


                 A+W Production Packmitteloptimierung                                                               I-31
                 Optimierung ansehen                                                                         Tutorial




                                       3D-Ansicht um 45° in die entsprechende Richtung. Sie haben so die Möglich-
                                       keit, sich das Gestell aus verschiedenen Blickwinkeln anzusehen, um z.B. frei-
                                       en Gestellplatz besser beurteilen zu können.

                                          Modus
                                          In welchem Modus Sie sich befinden (Vollbild/Bearbeiten), wird Ihnen im
                                          Programm am Ende der Titelleiste in eckigen Klammern angezeigt. Bei-
                                          spiel: [Vollbild].


                                       Bearbeitungs-Modus
                                       PackView befindet sich nach dem Start im Vollbild-Modus. In den Bearbei-
                                       tungs-Modus gelangen Sie entweder über das Menü
                                       Bearbeiten > Bearbeiten,
                                       über die Funktionstaste <F3>
                                       oder aber über die Symbol-Schaltfläche



                                       Abb. I-25    Symbol-Schaltfläche Bearbeiten ein/aus


                                       Sie können mit der Maus eine Scheibe markieren, indem Sie entweder in der
                                       3D-Ansicht oder der Draufsicht eine Einheit anklicken oder aber eine Position
                                       aus der Detail-Ansicht wählen. Die ausgewählte Einheit wird sowohl in der 3D-
                                       Ansicht als auch der Draufsicht in grüner Farbe dargestellt. In der Detailan-
                                       sicht befindet sich ein grüner Rahmen um die ausgewählte Einheit.
                                       PackView wählt automatisch immer Teilstapel aus, die auch tatsächlich be-
                                       wegt werden können. Wenn Sie eine Einheit in der Mitte eines Stapels aus-
                                       wählen, fügt PackView automatisch alle davor stehenden Einheiten in die
                                       Auswahl ein.
2.00 / 01-2017




                                       Abb. I-26    Bearbeitungs-Modus


                 I-32                                                        A+W Production Packmitteloptimierung
                 Tutorial                                                                     Optimierung ansehen




                                        Im Bearbeitungs-Modus haben Sie Zugriff auf die unterschiedlichen Kamera-
                                        Positionen. Durch Betätigen der jeweiligen Schaltfläche schwenkt das Gestell
                                        in der 3D-Ansicht um 45° in die entsprechende Richtung. Sie haben so die
                                        Möglichkeit, sich das Gestell aus verschiedenen Blickwinkeln anzusehen, um
                                        z. B. freien Gestellplatz besser beurteilen zu können. Darüber hinaus können
                                        Sie im Bearbeitungs-Modus einzelne Einheiten oder auch ganze Stapel auf
                                        dem Gestell z.B. schrittweise verschieben oder links- bzw. rechtsbündig aus-
                                        richten.

                                           Modus
                                           In welchem Modus Sie sich befinden, wird Ihnen im Programm am Ende
                                           der Titelleiste in eckigen Klammern angezeigt. Beispiel: [Bearbeiten].
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                          I-33
                 Optimierung ansehen                                                                      Tutorial




                                       Experten-Modus
                                       PackView befindet sich nach dem Start im Normal-Modus. In den Experten-
                                       Modus gelangen Sie entweder über das Menü
                                       Ansicht > Experten-Modus ein/aus,
                                       oder über die Symbol-Schaltfläche



                                       Abb. I-27   Symbol-Schaltfläche Experten-Modus ein/aus


                                       Den Experten-Modus können Sie sowohl im Vollbild- als auch im Bearbei-
                                       tungs-Modus zuschalten.




                                       Abb. I-28   Experten-Modus


                                       Neben den bereits genannten Funktionalitäten von Vollbild- und Bearbei-
                                       tungs-Modus haben Sie im Experten-Modus noch die Möglichkeit, das Gestell
                                       zu zoomen und auf der X- bzw. Y-Achse zu rotieren.

                                                          Zum Zoomen platzieren Sie den Mauszeiger mittig auf
                                                          dem Rad, drücken die linke Maustaste und halten sie ge-
                                                          drückt. Drehen Sie das Rad nach oben, wird das Gestell
                                                          verkleinert, drehen Sie das Rad nach unten, vergrößern
                                                          Sie das Gestell.

                                       Tab. I-2    Zoom
2.00 / 01-2017




                 I-34                                                      A+W Production Packmitteloptimierung
                 Tutorial                                                                       Optimierung ansehen




                                                            Zum rotieren auf der Y-Achse platzieren Sie den Mauszei-
                                                            ger mittig auf dem Rad, drücken die linke Maustaste und
                                                            halten sie gedrückt. Drehen Sie das Rad nach rechts, wird
                                                            das Gestell nach rechts gedreht, drehen Sie das Rad nach
                                                            links, wird das Gestell nach links bewegt.
                                                            Zum rotieren auf der X-Achse platzieren Sie den Mauszei-
                                                            ger mittig auf dem Rad, drücken die linke Maustaste und
                                                            halten sie gedrückt. Drehen Sie das Rad nach oben, wird
                                                            das Gestell nach oben gekippt, drehen Sie das Rad nach
                                                            unten, wird das Gestell nach unten gekippt.

                                        Tab. I-2     Zoom


                                        Wenn Sie sich im Experten-Modus befinden, haben Sie auch die Möglichkeit,
                                        das Gestell frei zu rotieren. Das freie Rotieren aktivieren Sie entweder über
                                        das Menü
                                        Ansicht > Freies Rotieren
                                        oder über die Symbol-Schaltfläche



                                        Abb. I-29    Symbol-Schaltfläche Freies Rotieren


                                        Ihr Mauszeiger ändert sich dann wie folgt:




                                        Abb. I-30    Mauszeiger bei freiem Rotieren


                                        Platzieren Sie den Mauszeiger auf dem Gestell, drücken Sie die linke Maus-
                                        taste und halten Sie diese gedrückt. Anschließend können Sie das Gestell
                                        nach links oder rechts beliebig drehen oder nach oben bzw. unten kippen. Mit
                                        Druck auf das Mausrad können Sie das Gestell nach links und rechts ver-
                                        schieben.


                                        Freier Editier-Modus
                                        Dieser Modus erlaubt es Ihnen, Scheiben auf einem Gestell umzuorganisie-
                                        ren, ohne dass physikalische Einschränkungen berücksichtigt werden. Sie
                                        können z. B. beliebige Scheiben auswählen und erweiterte Bewegungen und
                                        Aktionen mit den ausgewählten Scheiben durchführen. So ist es z. B. möglich,
                                        Scheiben innerhalb eines Stapels nach vorne oder hinten zu bewegen. D. h.,
                                        Sie erhalten im freien Editier-Modus mehr Möglichkeiten, sind aber auf der an-
                                        deren Seite selbst für eine falsche oder unmögliche Platzierung verantwort-
                                        lich!
2.00 / 01-2017




                                        Mit der Tastenkombination <Strg> + <linke Maustaste> können beliebige Ein-
                                        heiten auch in der Mitte des Stapels ausgewählt werden. Ohne gedrückte
                                        <Strg>-Taste bleibt das Prinzip der Auswahl unverändert.



                 A+W Production Packmitteloptimierung                                                            I-35
                 Optimierung ansehen                                                                            Tutorial




                                       Abb. I-31    <Strg> + linke Maustaste


                                       Mit der ENTER-Taste können Sie einen sogenannten Locator erstellen (eine
                                       Gruppe von Einheiten, die gemeinsam manipuliert werden können), anstatt
                                       <Strg> + <C> zu drücken.
                                       Ein erneutes Drücken der ENTER-Taste verlässt den Locator-Status und die
                                       Platzierung der Einheiten werden bestätigt, anstatt <Strg> + <V> für den glei-
                                       chen Vorgang zu drücken.
                                       Wenn die aus dem/den Stapel(n) entnommenen Scheiben nicht gruppiert sind,
                                       wird ein virtueller Locator erstellt (vom Gestell aus eingerückt dargestellt) und
                                       der Rest der Scheiben werden auf dem Gestell konsolidiert. D. h. alle Lücken
                                       werden entfernt und die verbleibenden Scheiben werden automatisch zuein-
                                       ander verschoben. Sie müssen dann den neuen Standort für den Locator ma-
                                       nuell auswählen, um die Bearbeitung fortzusetzen.
2.00 / 01-2017




                 I-36                                                          A+W Production Packmitteloptimierung
                 Tutorial                                                                          Optimierung ansehen




                                        Abb. I-32    Neue Position der Scheibe


                                        Mit den Pfeiltasten Auf/Ab, können die Scheiben auf dem Gestell vorwärts
                                        oder rückwärts bewegt werden. Das Rückwärts-/Vorwärtsbewegen durch
                                        mehrere Scheiben ist nur möglich, wenn die Scheiben einen nebeneinander
                                        liegenden Block bilden (d. h., sie haben die gleiche Z- und Y-Koordinate und
                                        die gleiche Dicke).




                                        Mit der Alt-Taste können Sie erzwingen, dass die Ausrichtung der Scheiben in
                                        Bezug auf das Gestell erfolgt. Wird die Alt-Taste nicht gedrückt, funktioniert die
                                        Ausrichtung wie zuvor (nach der darunter liegenden Einheit).
                                        Neue Möglichkeit die Scheiben zu drehen. Im normalen Modus können Schei-
                                        ben nur gedreht werden, die einen Block bilden. Es ist jedoch zu beachten,
                                        dass die Scheiben nach der Drehung falsch platziert sein können!
                                        Eine automatische Gültigkeitsprüfung wird durchgeführt, wenn der Bearbei-
                                        tungsmodus ausgeschaltet ist. Alle Scheiben, die andere Scheiben stören
                                        oder gegen andere Regeln verstoßen, werden mit einer Farbe markiert, die in
2.00 / 01-2017




                                        der PackView.ini als ShowReasonMaterial definiert ist. Wir empfehlen, zumin-
                                        dest die Transparenz auf einen niedrigeren Wert zu setzen, um eine bessere
                                        Übersichtlichkeit zu erreichen.


                 A+W Production Packmitteloptimierung                                                                I-37
                 Optimierung ansehen                                                                     Tutorial




                                       Abb. I-33   Niedrigere Transparenz
2.00 / 01-2017




                 I-38                                                       A+W Production Packmitteloptimierung
                 Tutorial                                                                       Optimierung ansehen




                                        Zwischenablage
                                        Wenn Sie eine oder auch mehrere Einheiten ausgeschnitten haben, werden
                                        diese nach dem Ausschneiden automatisch in die Zwischenablage gestellt.
                                        Beispiel: Sie markieren im Bearbeitungs-Modus eine Einheit.




                                        Abb. I-34   Zwischenablage


                                        Anschließend betätigen Sie die Schaltfläche zum Ausschneiden der Einheit



                                        Abb. I-35   Schaltfläche zum Ausschneiden der Einheit


                                        PackView zeigt Ihnen dann das Gestell ohne die Einheit, da Sie diese ja aus-
                                        geschnitten haben. Die Detail-Ansicht zeigt Ihnen die Inhalte der Zwischenab-
                                        lage, in diesem Fall die soeben ausgeschnittene Einheit:
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                           I-39
                 Optimierung ansehen                                                                        Tutorial




                                       Abb. I-36    Zwischenablage


                                       Durch Betätigen der Schaltfläche Zwischenablage können Sie die Detail-An-
                                       sicht zwischen der Anzeige der Zwischenablage und der Gestellbelegung um-
                                       schalten.
                                       Bei Feldern, die in der Detail-Ansicht mit einem - versehen sind, können Sie
                                       die Sortierung ändern. Wenn Sie den Mauszeiger auf einem solchen Feld plat-
                                       zieren und die linke Maustaste betätigen, ändert sich das Symbol von - nach
                                       . Das bedeutet, dass die Sortierung für das entsprechende Feld aufsteigend
                                       ist. Betätigen Sie die linke Maustaste erneut, wechselt das Symbol von auf
                                       . Das bedeutet, dass die Sortierung für das entsprechende Feld absteigend
                                       ist. Zum Ausschalten der Sortierung, betätigen Sie die rechte Maustaste.
                                       Sie können mehrere Spalten in dieser Weise anklicken. Die Sortierung erfolgt
                                       dann zunächst nach der zuerst angeklickten Spalte, dann nach der nächsten,
                                       etc. Die Ziffer zeigt diese Rangfolge an.


                                        So wählen Sie das nächste/vorherige Gestell zur Anzeige aus
                                       In der Regel werden durch die Packmitteloptimierung mehrere Gestelle bela-
                                       den. PackView startet nach erfolgreich durchgeführter Optimierung automa-
                                       tisch mit dem ersten Gestell. Zum Anzeigen der weiteren Gestelle gehen Sie
                                       wie folgt vor:
                                       1 Wählen Sie im Menü Ansicht > Zeige nächstes Gestell, verwenden Sie die
                                         entsprechende Symbol-Schaltfläche oder die Tasten <BildAuf> bzw. <Bil-
                                         dAb>.
                                           Softwarereferenz, “Zeige nächstes Gestell” auf Seite I-87
                                           Softwarereferenz, “Zeige vorheriges Gestell” auf Seite I-87
2.00 / 01-2017




                                          Auf diese Art und Weise können Sie sich Gestell für Gestell anzeigen las-
                                          sen.



                 I-40                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                            Optimierung ansehen




                                         So wählen Sie ein beliebiges Gestell zur Anzeige aus
                                        In der Regel werden durch die Packmitteloptimierung mehrere Gestelle bela-
                                        den. PackView startet nach erfolgreich durchgeführter Optimierung automa-
                                        tisch mit dem ersten Gestell. Zum Anzeigen eines weiteren Gestelle gehen Sie
                                        wie folgt vor:
                                        1 Wählen Sie entweder im Menü Ansicht > Gestell zur Anzeige
                                          auswählen …, verwenden Sie die entsprechende Symbol-Schaltfläche
                                          oder die Tasten <BildAuf> bzw. <BildAb>.
                                            Softwarereferenz, “Gestell zur Anzeige auswählen …” auf Seite I-87
                                        2 Es öffnet sich der Dialog Eingabe. Im Feld Gestell ID eingeben können Sie
                                          die gewünschte Gestellnummer eingeben.
                                        3 Nach Betätigen der Schaltfläche [OK] wird das entsprechende Gestell an-
                                          gezeigt.


                                         So verschieben Sie eine oder wenige Einheiten
                                        1 Aktivieren Sie den Bearbeitungs-Modus über das Menü Bearbeiten > Be-
                                          arbeiten, über die Funktionstaste <F3> oder aber über die Symbol-Schalt-
                                          fläche.
                                            Softwarereferenz, “Bearbeiten ein/aus” auf Seite I-89
                                        2 Markieren Sie die Einheit(en), die Sie verschieben möchten. Die Ein-
                                          heit(en) bekommt einen grünen Rahmen. Es bekommen automatisch wei-
                                          tere Einheiten einen grünen Rahmen, die mit bewegt werden müssen,
                                          wenn die gewünschte, zunächst ausgewählte Einheit verschoben werden
                                          soll. Durch weitere Klicks können weitere Einheiten hinzugenommen oder
                                          bereits gewählte Einheiten abgewählt werden.
2.00 / 01-2017




                                           Abb. I-37    Einheit markieren




                 A+W Production Packmitteloptimierung                                                               I-41
                 Optimierung ansehen                                                                       Tutorial




                                       3 Kopieren Sie die Einheit(en) entweder über das Menü Bearbeiten > Kopie-
                                         ren, über die Symbol-Schaltfläche oder über die Tastatur (<Strg>+<C>).
                                           Softwarereferenz, “Einheit Kopieren” auf Seite I-90
2.00 / 01-2017




                 I-42                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                         Optimierung ansehen




                                           Die Einheit wird komplett in grüner Farbe dargestellt.




                                           Abb. I-38    Einheit kopieren, markieren


                                        4 Verschieben Sie die Einheit an die gewünschte Stelle mithilfe der Rich-
                                          tungstasten oder über die Symbol-Schaltfläche.
                                            Softwarereferenz, “Einheit nach links bewegen” auf Seite I-90
                                            Softwarereferenz, “Einheit nach rechts bewegen” auf Seite I-90




                                           Abb. I-39    Einheit verschieben
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                            I-43
                 Optimierung ansehen                                                                         Tutorial




                                       5 Ist die Einheit an der Stelle angekommen, wo sie neu platziert werden soll,
                                         fügen Sie sie dort entweder über das Menü Bearbeiten > Einfügen oder
                                         aber über die Symbol-Schaltfläche ein.
                                           Softwarereferenz, “Einheit Einfügen” auf Seite I-90




                                          Abb. I-40    Einheit einfügen


                                        So verschieben Sie einen ganzen Stapel
                                       1 Aktivieren Sie den Bearbeitungs-Modus über das Menü Bearbeiten > Be-
                                         arbeiten, über die Funktionstaste <F3> oder aber über die Symbol-Schalt-
                                         fläche
                                           Softwarereferenz, “Bearbeiten ein/aus” auf Seite I-89
                                       2 Markieren Sie die Einheit des Stapels, die der Gestellrückwand am nähes-
                                         ten steht und die Sie verschieben möchten. Die Einheit und alle davor ste-
                                         henden Einheiten bekommen einen grünen Rahmen.
                                          Nach der Markierung einer oder mehrerer Einheiten, können Sie durch er-
                                          neutes klicken Einheiten auch wieder abwählen.
2.00 / 01-2017




                 I-44                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                          Optimierung ansehen




                                           Durch einen Klick neben das Gestell werden alle markierten Einheiten ab-
                                           gewählt.




                                           Abb. I-41    Stapel markieren


                                        3 Kopieren Sie den Stapel entweder über das Menü Bearbeiten > Kopieren,
                                          oder aber über die Symbol-Schaltfläche
                                            Softwarereferenz, “Einheit Kopieren” auf Seite I-90
                                           Der Stapel wird komplett in grüner Farbe dargestellt. Alle markierten Ein-
                                           heiten verschwinden aus der Detail-Ansicht.




                                           Abb. I-42    Stapel kopieren
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                             I-45
                 Optimierung ansehen                                                                         Tutorial




                                       4 Verschieben Sie den Stapel an die gewünschte Stelle mithilfe der Rich-
                                         tungstasten oder über die Symbol-Schaltfläche
                                           Softwarereferenz, “Einheit nach links bewegen” auf Seite I-90
                                           Softwarereferenz, “Einheit nach rechts bewegen” auf Seite I-90




                                          Abb. I-43    Stapel verschieben


                                       5 Ist der Stapel an der Stelle angekommen, wo er neu platziert werden soll,
                                         fügen Sie ihn dort entweder über das Menü Bearbeiten > Einfügen oder
                                         aber über die Symbol-Schaltfläche ein.
                                           Softwarereferenz, “Einheit Einfügen” auf Seite I-90




                                          Abb. I-44    Stapel einfügen
2.00 / 01-2017




                 I-46                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                            Optimierung ansehen




                                         So arbeiten Sie mit der Zwischenablage
                                           Wenn Sie viele Einheiten, etwa aus verschiedenen Stapeln, auf einer an-
                                           deren Gestellseite platzieren möchten oder gar auf einem anderen Gestell,
                                           geht dies gut über die Zwischenablage. Dabei können Sie auch bequem
                                           die Reihenfolge der Einheiten nach Größe, Auftragsnummer etc. sortieren,
                                           um den neuen Stapel Ihren Wünschen entsprechend aufzubauen.
                                        1 Aktivieren Sie den Bearbeitungs-Modus über das Menü Bearbeiten > Be-
                                          arbeiten, über die Funktionstaste <F3> oder aber über die Symbol-Schalt-
                                          fläche.
                                            Softwarereferenz, “Bearbeiten ein/aus” auf Seite I-89
                                        2 Markieren Sie die Einheit(en), die Sie verschieben möchten. Die Ein-
                                          heit(en) bekommt einen grünen Rahmen.




                                           Abb. I-45    Einheit markieren
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                               I-47
                 Optimierung ansehen                                                                       Tutorial




                                       3 Schneiden Sie die Einheit(en)/Stapel entweder über das Menü Bearbeiten
                                         > Ausschneiden, oder aber über die Symbol-Schaltfläche aus.
                                           Softwarereferenz, “Einheit Ausschneiden” auf Seite I-90




                                          Abb. I-46    Einheit ausschneiden


                                          Die Einheit(en)/Stapel verschwindet sowohl aus der 3D-Ansicht als auch
                                          aus der Draufsicht. Im Bereich der Detail-Ansicht bekommen Sie automa-
                                          tisch den Inhalt der Zwischenablage angezeigt. Über das Menü Ansicht >
                                          Zwischenablage anzeigen oder durch einen Klick auf die entsprechende
                                          Symbol-Schaltfläche können Sie zwischen Detail-Ansicht und Zwischen-
                                          ablage wechseln. Das Ausschneiden können Sie mit weiteren Einheiten
                                          wiederholen und die Zwischenablage damit weiter füllen.




                                          Abb. I-47    Zwischenablage ein- und ausblenden
2.00 / 01-2017




                 I-48                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                          Optimierung ansehen




                                        4 Wechseln Sie zu der gewünschten Gestellseite bzw. dem gewünschten
                                          Gestell.




                                           Abb. I-48    Andere Gestellseite bzw. anderes Gestell


                                        5 Lassen Sie sich entweder über das Menü Ansicht > Zwischenablage an-
                                          zeigen oder über die entsprechende Symbol-Schaltfläche den Inhalt der
                                          Zwischenablage anzeigen. Befinden Sie mehrere Einheiten in der Zwi-
                                          schenablage, können Sie die Zwischenablage nach unterschiedlichen Kri-
                                          terien sortieren. Nähere Informationen hierzu finden Sie unter
                                            Tutorial, “Zwischenablage” auf Seite I-39




                                           Abb. I-49    Zwischenablage anzeigen
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                             I-49
                 Optimierung ansehen                                                                       Tutorial




                                       6 Klicken Sie anschließend auf die Symbol-Schaltfläche [Einfügen]
                                           Softwarereferenz, “Einheit Einfügen” auf Seite I-90
                                          Der Mauszeiger ändert sich zu einem Fadenkreuz




                                          Abb. I-50    Einheit einfügen


                                       7 Bewegen Sie das Fadenkreuz an die Stelle, wo die Einheit(en)/Stapel ein-
                                         gefügt werden soll(en).




                                          Abb. I-51    Fadenkreuz positionieren
2.00 / 01-2017




                 I-50                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                       Optimierung ansehen




                                        8 Betätigen Sie anschließend die linke Maustaste. Die Einheit(en)/Stapel
                                          wird - sofern physikalisch möglich - an dieser Stelle eingefügt. Befinden
                                          sich in der Zwischenablage mehrere Einheiten/Stapel, können Sie diese
                                          mit wiederholtem Betätigen von <Strg>+<C> auf einen Stapel stellen.
                                           Sollte es nicht möglich sein, die Einheit(en)/Stapel an der gewünschten
                                           Stelle einzufügen, wird Ihnen das wie folgt dargestellt:




                                           Abb. I-52    Fadenkreuz positionieren


                                           Das bedeutet, die Einheit(en)/Stapel wird kurzzeitig in oranger Farbe an
                                           der gewünschten Stelle eingeblendet und anschließend wieder ausgeblen-
                                           det. Gründe für ein Nicht-Platzieren können z. B. sein: Die Einheit(en)/Sta-
                                           pel ist zu dick und würde vorne vom Gestell fallen oder der Schwerpunkt
                                           liegt zu weit rechts und die Einheit(en)/Stapel würde auf der rechten Seite
                                           vom Gestell kippen, usw.
                                           Erfüllt die gewünschte Stelle die Anforderungen um die Einheit(en)/Stapel
                                           einzufügen, wird, nach Betätigen der linken Maustaste, die Einheit(en)/Sta-
                                           pel dort eingefügt.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                             I-51
                 Optimierung ansehen                                                                         Tutorial




                                          Gleichzeitig wird die Zwischenablage in der Detail-Ansicht geleert, d.h. es
                                          befindet sich jetzt keine Einheit(en)/Stapel mehr in der Zwischenablage.




                                          Abb. I-53    Einheit einfügen


                                        So arbeiten Sie mit mehreren Stapeln in der Zwischenablage
                                          Wenn Sie mehrere Stapel auf einer anderen Gestellseite platzieren möch-
                                          ten oder gar auf einem anderen Gestell, verwenden Sie hierzu die Zwi-
                                          schenablage. Dabei können Sie auch bequem die Reihenfolge der
                                          Einheiten nach Größe, Auftragsnummer etc. sortieren. Im folgenden Bei-
                                          spiel verschieben wir 3 Stapel von unterschiedlichen Gestellseiten in die
                                          Zwischenablage und platzieren sie anschließend auf einer leeren Gestell-
                                          seite neu.
                                       1 Aktivieren Sie den Bearbeitungs-Modus über das Menü Bearbeiten > Be-
                                         arbeiten, über die Funktionstaste <F3> oder aber über die Symbol-Schalt-
                                         fläche.
                                           Softwarereferenz, “Bearbeiten ein/aus” auf Seite I-89
2.00 / 01-2017




                 I-52                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                         Optimierung ansehen




                                        2 Markieren Sie die letzte Einheit (von vorne gesehen) des ersten Stapel,
                                          den Sie verschieben möchten. Alle Einheiten, die vor der markierten Ein-
                                          heit stehen, bekommen einen grünen Rahmen.




                                           Abb. I-54    Stapel markieren


                                        3 Schneiden Sie die Stapel entweder über das Menü Bearbeiten > Aus-
                                          schneiden, oder aber über die Symbol-Schaltfläche aus.
                                            Softwarereferenz, “Einheit Ausschneiden” auf Seite I-90




                                           Abb. I-55    Stapel ausschneiden
2.00 / 01-2017




                                           Der Stapel verschwindet sowohl aus der 3D-Ansicht als auch aus der
                                           Draufsicht. Im Bereich der Detail-Ansicht bekommen Sie automatisch den


                 A+W Production Packmitteloptimierung                                                            I-53
                 Optimierung ansehen                                                                 Tutorial




                                       Inhalt der Zwischenablage angezeigt. Über das Menü Ansicht > Zwischen-
                                       ablage anzeigen oder durch einen Klick auf die entsprechende Symbol-
                                       Schaltfläche können Sie zwischen Detail-Ansicht und Zwischenablage
                                       wechseln.
                                       Wir wechseln zum nächsten Gestell, um dort den zweiten Stapel zu mar-
                                       kieren.




                                       Abb. I-56   Stapel markieren
2.00 / 01-2017




                 I-54                                                  A+W Production Packmitteloptimierung
                 Tutorial                                                                       Optimierung ansehen




                                        4 Anschließend verschieben wir den Stapel in die Zwischenablage.




                                           Abb. I-57    Stapel ausschneiden


                                           Die Einheiten des Stapels, die zuletzt der Zwischenablage hinzugefügt
                                           wurden, sind blau unterlegt. Darüber hinaus liefert Ihnen die Packmittel-
                                           opitimierung bereits an dieser Stelle einen Vorschlag für eine neue Sortie-
                                           rung der Einheiten.
                                        5 Wir wechseln zum nächsten Gestell, um dort weitere Stapel zu markieren.




                                           Abb. I-58    Stapel markieren
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                            I-55
                 Optimierung ansehen                                                                       Tutorial




                                       6 Anschließend verschieben wir die Stapel in die Zwischenablage.




                                          Abb. I-59   Stapel ausschneiden


                                       7 Wechseln Sie zu der gewünschten Gestellseite bzw. dem gewünschten
                                         Gestell auf dem die Stapel aus der Zwischenablage platziert werden sollen.




                                          Abb. I-60   Andere Gestellseite bzw. anderes Gestell
2.00 / 01-2017




                 I-56                                                       A+W Production Packmitteloptimierung
                 Tutorial                                                                          Optimierung ansehen




                                           Das Symbol () im Bereich Höhe zeigt Ihnen, dass die momentane Sortie-
                                           rung nach der Höhe absteigend ist. Weitere Informationen zu den Sortie-
                                           rungen finden Sie unter
                                            Tutorial, “Zwischenablage” auf Seite I-39
                                        8 Da wir die Einheiten nach der Breite sortiert haben möchten, ändern wir zu-
                                          nächst die Sortierung. Platzieren Sie den Mauszeiger auf dem Symbol ()
                                          im Bereich Höhe und betätigen Sie anschließend die rechte Maustaste.
                                          Das Symbol ändert sich in -. Dann klicken Sie mit der linken Maustaste auf
                                          das - im Bereich Breite. Es erscheint 1 und die Sortierung ändert sich.




                                           Abb. I-61    Sortierung ändern


                                        9 Die beiden Einheiten mit der größten Breite fügen wir zuerst ein. Der rote
                                          Rahmen zeigt Ihnen, welche Einheit Sie zum Einfügen ausgewählt haben.
                                          Klicken Sie anschließend auf die Symbol-Schaltfläche [Einfügen]
                                            Softwarereferenz, “Einheit Einfügen” auf Seite I-90
                                           Der Mauszeiger ändert sich zu einem Fadenkreuz. Bewegen Sie das Fa-
                                           denkreuz an die Stelle, wo die Einheit eingefügt werden soll und betätigen
                                           Sie die linke Maustaste. Die Einheit wird eingefügt und verschwindet aus
                                           der Zwischenablage.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                             I-57
                 Optimierung ansehen                                                                     Tutorial




                                       Gleichzeitig wird in der Zwischenablage die nächste Einheit zum Platzieren
                                       vorgeschlagen (roter Rahmen).




                                       Abb. I-62   Einheit einfügen


                                       Über die Richtungstasten haben Sie die Möglichkeit, die Einheit präzise
                                       auszurichten. Hierzu klicken Sie auf die Symbol-Schaltfläche [Kopieren],
                                       die Einheit wird ganz in Grün dargestellt.




                                       Abb. I-63   Einheit kopieren
2.00 / 01-2017




                 I-58                                                    A+W Production Packmitteloptimierung
                 Tutorial                                                                      Optimierung ansehen




                                           Anschließend wird die Einheit mithilfe der Symbol-Schaltfläche [Nach links
                                           bewegen] an die linke Gestellscheibe geschoben. Ist die Einheit an der ge-
                                           wünschten Stelle angekommen, klicken Sie auf die Symbol-Schaltfläche
                                           [Einfügen] und die Einheit wird dort platziert.




                                           Abb. I-64    Einheit kopieren
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                           I-59
                 Optimierung ansehen                                                                       Tutorial




                                       Die nächste Einheit wird auf die gleiche Art und Weise platziert. Erst betä-
                                       tigen Sie die Symbol-Schaltfläche [Kopieren], der Mauszeiger ändert sich
                                       zum Fadenkreuz. Da die Einheit dieselbe Abmessung hat wie die zuvor
                                       platzierte Einheit, wird Ihnen die Packmitteloptimierung diese Einheit exakt
                                       vor der anderen platzieren. D. h. das Verschieben ist nicht mehr nötig.

                                       Tastatur
                                       <Strg>+<V> fügt die nächste Einheit aus der Zwischenablage vor die zu-
                                       letzt eingefügte ein.




                                       Abb. I-65    Einheit einfügen
2.00 / 01-2017




                 I-60                                                    A+W Production Packmitteloptimierung
                 Tutorial                                                                         Optimierung ansehen




                                        10 Dann ändern wir die Sortierung von Breite nach Höhe und diese abstei-
                                           gend.




                                           Abb. I-66    Sortierung Höhe absteigend


                                        11 Anschließend fügen wir die Einheit, die jetzt oben steht, ein. Klicken Sie auf
                                           die Schaltfläche [Einfügen] und die Einheit wird mittig platziert.




                                           Abb. I-67    Einheit einfügen
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                               I-61
                 Optimierung ansehen                                                                         Tutorial




                                          Mit hilfe der Symbol-Schaltflächen [Kopieren], [Nach links bewegen]/[Links
                                          ausrichten] und [Einfügen] verschieben wir die Einheit an den linken Rand.




                                          Abb. I-68    Einheit nach links verschieben


                                       12 Wenn Sie zum Einfügen der nächsten Einheit die Symbol-Schaltfläche
                                          [Einfügen] betätigen, erscheint wieder das Fadenkreuz. Das liegt daran,
                                          dass die Packmitteloptimierung ja nicht weiß ob Sie die Einheit vor 1 oder
                                          vor 2 einfügen möchten.




                                                      1   2
2.00 / 01-2017




                                          Abb. I-69    Einheit nach links verschieben




                 I-62                                                         A+W Production Packmitteloptimierung
                 Tutorial                                                                       Optimierung ansehen




                                        13 Wir fügen die Einheit vor 1 ein.




                                                           2




                                           Abb. I-70    Einheit einfügen


                                        14 Wie Sie sehen können, hat die Einheit in Abb. I-70 auf Seite I-63 einen grü-
                                           nen Rahmen. Sie ist quasi noch aktiv. Über die Symbol-Schaltfläche [Ein-
                                           fügen] oder mithilfe von <Strg>+<V> können Sie gleich die nächste Einheit
                                           davor platzieren. Auf diese Weise können Sie Einheiten so lange platzie-
                                           ren, bis kein Platz mehr auf dem Gestell ist. Die Einheit, die praktisch vom
                                           Gestell fallen würde, wird dann kurze Zeit in oranger Farbe auf dem Gestell
                                           dargestellt, jedoch nicht platziert.
2.00 / 01-2017




                 A+W Production Packmitteloptimierung                                                             I-63
                 Optimierung ansehen                                                                         Tutorial




                                          Abb. I-71     Einheit einfügen


                                       15 Wenn Sie die Symbol-Schaltfläche [Einfügen] betätigen, ändert sich der
                                          Mauszeiger wieder zum Fadenkreuz und Sie können sich für die nächste
                                          Einheit einen Platz suchen. Auf diese Weise können Sie so lange weiter ar-
                                          beiten, bis alle Einheiten aus der Zwischenablage auf dem Gestell platziert
                                          sind.


                                       Weitere Informationen zu PackView
                                        Tutorial, “Optimierung ansehen” auf Seite I-23
                                        Softwarereferenz, “PackView” auf Seite I-83
2.00 / 01-2017




                 I-64                                                         A+W Production Packmitteloptimierung
Packmitteloptimierung            I

                   Softwarereferenz




                A+W Production
                 Softwarereferenz                                                                                  Menüs




                                              Menüs
                                              Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die
                                              sich im Menü Stammdaten befinden.


                 Menü-Eintrag                                  Dialog/Funktion

                 PMO                  Regeln                    Kapitel “Regeln” auf Seite I-69

                                      Werte                     Kapitel “Werte” auf Seite I-71

                 Tab. I-3       Übersicht der Dialoge im Menü Stammdaten

                                              Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die
                                              sich im Kontext-Menü der Anzeigen Aufträge, Bearbeitungen und Details be-
                                              finden.


                 Menü-Eintrag                                  Dialog/Funktion

                 Kontext-Menü         Packmittelgruppe          Kapitel “Packmittelgruppen” auf Seite I-74
                                      bilden

                 Tab. I-4       Übersicht der Dialoge, die über das Kontext-Menü zu erreichen sind

                                              Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die
                                              sich im Kontext-Menü der Anzeige Packmittelgruppe befinden.


                 Menü-Eintrag                                  Dialog/Funktion

                 Kontext-Menü         Packmittelgruppe          Kapitel “PMG verschieben” auf Seite I-80
                                      verschieben

                                      Packmittelgruppe          Kapitel “PMG optimieren” auf Seite I-80
                                      optimieren

                                      Packmittelgruppe          Kapitel “PMG optimieren im Hintergrund” auf
                                      optimieren im              Seite I-81
                                      Hintergrund

                                      Packmittelgruppe          Kapitel “PMG verwalten” auf Seite I-81
                                      verwalten

                                      Optimierung ansehen       Softwarereferenz, “PackView” auf Seite I-83

                 Tab. I-5       Übersicht der Dialoge, die über das Kontext-Menü zu erreichen sind
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                                 I-67
                 Menüs                                                                                Softwarereferenz




                                          Die nachfolgende Tabelle gibt eine Übersicht der Dialoge und Funktionen, die
                                          sich im Menü Anzeigen befinden.


                 Menü-Eintrag                             Dialog/Funktion

                 Packmittelgruppen                         Kapitel “Packmittelgruppen-Anzeige” auf
                 -Anzeige                                   Seite I-77

                 Tab. I-6    Übersicht der Dialoge im Menü Anzeigen

                                          Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden
                                          Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative
                                          Wege einen Dialog aufzurufen, so sind diese ebenfalls angegeben.
2.00 / 01-2023




                 I-68                                                          A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                           Menüs




                                        Regeln
                                        Stammdaten > PMO > Regeln




                                        Abb. I-72   Packmittelgruppen, Regeln


                                        In diesem Dialog erfassen Sie neue Optimierungsregeln oder ändern beste-
                                        hende Regeln ab.
                                        Technische Info: Datenbanktabelle: PMO_MASTER_RULES

                                        Erläuterung der Schaltfläche

                                        .RUL-Dateien laden Wenn Sie diese Schaltfläche betätigen, werden die
                                        *.RUL-Dateien aus dem entsprechenden Verzeichnis geladen. Sind bereits
                                        *.RUL-Dateien in der Anzeige zu sehen, werden Sie darauf aufmerksam ge-
                                        macht, dass alle aktuellen Datensätze verloren gehen. Wenn Sie *.RUL-Da-
                                        teien aktivieren möchten, ist das die richtige Vorgehensweise.

                                        Erläuterung der Tabellenspalten

                                        .RUL-Datei In dieser Tabellenspalte wird Ihnen der Name der zur Zeit gela-
                                        denen *.RUL-.Dateien angezeigt.

                                        Bezeichnung In dieser Tabellenspalte wird die Bezeichnung der *.RUL-Datei
                                        angezeigt.

                                        VAL_FILE In dieser Tabellenspalte können Sie sehen, welche *.VAL-Datei
                                        der *.RUL-Datei zugeordnet ist. D.h. welche Werte-Datei gehört zu welcher
                                        Regel-Datei.

                                        Erläuterung der Felder

                                        .RUL-Datei In diesem Feld geben Sie den Dateinamen der .RUL-Datei ein.
2.00 / 01-2023




                                        Über die Schaltfläche […] öffnet sich der Dialog Öffnen, aus dem Sie eine
                                        .RUL-Datei auswählen können, wenn Sie den Namen der Datei nicht kennen.
                                        Technische Info: Pflichtfeld, Alphanumerisch, 9stellig, Datenbankfeld: FILE


                 A+W Production Packmitteloptimierung                                                         I-69
                 Menüs                                                                   Softwarereferenz




                         Bezeichnung In diesem Feld geben Sie die Bezeichnung der *.RUL-Datei
                         ein.
                         Technische Info: Pflichtfeld, Alphanumerisch, 40stellig, Datenbankfeld: NAME

                         Beschreibung In diesem Feld geben Sie einen beschreibenden Text zur
                         *.RUL-Datei ein.
                         Technische Info: Eingabe optional, Alphanumerisch, 160stellig, Datenbank-
                         feld: DESCRIPTION

                         .VAL-Datei In diesem Feld wird die zur .RUL-Datei gehörende .VAL-Datei an-
                         gezeigt. Über die Schaltfläche […] öffnet sich der Dialog Öffnen, aus dem Sie
                         eine .VAL-Datei auswählen können, wenn Sie den Namen der Datei nicht ken-
                         nen bzw. wenn Sie einer .RUL-Datei eine andere .VAL-Datei zuordnen möch-
                         ten.
                         Technische Info: Pflichtfeld, Alphanumerisch, Datenbankfeld: VAL_FILE


                         Weitere Informationen zu Regeln
                          Tutorial, “Optimierungsregeln (*.RUL-Datei)” auf Seite I-13
                          Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2023




                 I-70                                            A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                              Menüs




                                        Werte
                                        Stammdaten > PMO > Werte




                                        Abb. I-73    Packmittelgruppen, Werte


                                        In diesem Dialog erfassen Sie die kundenspezifischen Werte oder nehmen
                                        Änderungen an bestehenden Werten vor.
                                        Technische Info: Datenbanktabelle: PMO_MASTER_VALUES

                                        Erläuterung der Schaltflächen

                                        .VAL-Dateien laden Wenn Sie diese Schaltfläche betätigen, werden die
                                        *.VAL-Dateien (Regel) aus dem entsprechenden Verzeichnis geladen. Sind
                                        bereits *.VAL-Dateien in der Anzeige zu sehen, werden Sie darauf aufmerk-
                                        sam gemacht, dass die aktuell angezeigten Datensätze verloren gehen. Wenn
                                        Sie *.VAL-Dateien aktivieren möchten, ist das die richtige Vorgehensweise.

                                        Erläuterung der Tabellenspalten

                                        .VAL-Datei In dieser Tabellenspalte wird Ihnen der Name der zur Zeit gelade-
                                        nen *.VAL-.Dateien angezeigt.

                                        Parameter In dieser Tabellenspalte wird der Packmittelparameter der *.VAL-
                                        Datei angezeigt. Dieser Wert kommt aus dem Feld Nummer des Packmittel-
                                        parameters.
                                         Softwarereferenz, “Nummer des Packmittelparameters” auf Seite I-72

                                        Bezeichnung In dieser Tabellenspalte wird die Bezeichnung der *.VAL-Datei
2.00 / 01-2023




                                        angezeigt. Dieser Wert kommt aus dem Feld Bezeichnung.
                                         Softwarereferenz, “Bezeichnung” auf Seite I-73




                 A+W Production Packmitteloptimierung                                                           I-71
                 Menüs                                                                Softwarereferenz




                         Mindestwert In dieser Tabellenspalte wird der Mindestwert des Parameters
                         angezeigt. Dieser Wert kommt aus dem Feld Mindestwert.
                          Softwarereferenz, “Mindestwert” auf Seite I-73

                         Maximalwert In dieser Tabellenspalte wird der Maximalwert des Parameters
                         angezeigt. Dieser Wert kommt aus dem Feld Maximalwert.
                          Softwarereferenz, “Maximalwert” auf Seite I-73

                         Wertetyp In dieser Tabellenspalte wird der Wertetyp des Parameters ange-
                         zeigt. Dieser Wert kommt aus dem Feld Wertetyp.
                          Softwarereferenz, “Maximalwert” auf Seite I-73

                         Erläuterung der Felder

                         .VAL-Datei In diesem Feld wird die *.VAL-Datei angezeigt. Über die Schalt-
                         fläche […] öffnet sich der Dialog Öffnen, aus dem Sie eine *.VAL-Datei aus-
                         wählen können, wenn Sie den Namen der Datei nicht kennen bzw. wenn Sie
                         eine .VAL-Datei ändern möchten.
                         Technische Info: Pflichtfeld, Alphanumerisch, Datenbankfeld: FILE

                         Nummer des Packmittelparameters In diesem Feld geben Sie z. B. die
                         Nummer des Parameters ein, dessen Wert Sie erfassen oder ändern möch-
                         ten. Es gibt die folgenden 9 Packmittelparameter:
                         Packmittelparameter 1: Sets in Stapeln zusammenhalten (0-nein, 1-mono, 2-
                         multi, 3-peripher). Nähere Erläuterungen hierzu finden Sie im Funktionsprin-
                         zip.
                          Tutorial, “Parameter” auf Seite I-14
                         Packmittelparameter 2: Sets bestehen aus (1-Auftrag, 2-Kommission, 3-Tour).
                         Packmittelparameter 3: Sets auf Gestellen zusammen halten? (0-nein, 1-ein
                         Gestell, 2-zwei Gestelle)
                         Packmittelparameter 4: Sets sortiert entladen? =0-nein, 1-Sets aufsteingend
                         ++, 2-Sets absteigend --)
                         Packmittelparameter 5: Maximales Gewicht für alle Gestelltypen.
                         Packmittelparameter 6: Maximale Anzahl der Stapel aufeinander (Stan-
                         dard=1)
                         Packmittelparameter 7: Maximaler Überstand links/rechts (Standard: 100mm)
                         Packmittelparameter 8: Maximales Stimmenverhältnis für aufrechte Scheiben
                         (Standard=3.0)
                         Packmittelparameter 9: Max. Seitenverhältnis für aufrechte Scheiben beim
                         Aufeinanderstapeln (Std.=2.0)
                         Nähere Erläuterungen finden Sie im Funktionsprinzip.
2.00 / 01-2023




                 I-72                                             A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                            Menüs




                                        Bezeichnung In diesem Feld geben Sie die Bezeichnung der *.VAL-Datei
                                        ein.
                                        Technische Info: Pflichtfeld, Alphanumerisch, 40stellig, Datenbankfeld: NAME

                                        Beschreibung In diesem Feld geben Sie einen beschreibenden Text zur
                                        *.VAL-Datei ein.
                                        Technische Info: Eingabe optional, Alphanumerisch, 160stellig, Datenbank-
                                        feld: DESCRIPTION

                                        Mindestwert In dieser Tabellenspalte wird der Mindestwert des aktuellen Pa-
                                        rameters eingegeben.
                                        Technische Info: Pflichtfeld, Numerisch, 50stellig, Datenbankfeld: VA-
                                        LUE_MIN

                                        Maximalwert In dieser Tabellenspalte wird der Maximalwert des aktuellen
                                        Parameters eingegeben.
                                        Technische Info: Pflichtfeld, Numerisch, 50stellig, Datenbankfeld: VA-
                                        LUE_MAX


                                        Weitere Informationen zu Einstellwerten
                                         Tutorial, “Einstellwerte (*.VAL-Datei)” auf Seite I-13
                                         Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                          I-73
                 Menüs                                                              Softwarereferenz




                         Packmittelgruppen
                         Aufträge > Kontext-Menü > Packmittelgruppen bilden
                         Bearbeitungs-Anzeige > Kontext-Menü > Packmittelgruppen bilden
                         Detail-Anzeige > Kontext-Menü > Packmittelgruppen bilden
                         Packmittelgruppen-Anzeige > Kontext-Menü > PMG verwalten > Parameter
                         ändern




                         Abb. I-74   Packmittelgruppen bilden


                         In diesem Dialog nehmen Sie die Einstellungen vor, mit denen die Packmittel-
                         gruppe gebildet werden soll. Ferner können Einstellungen bestehender Pack-
                         mittelgruppen geändert werden. Einstellungen können erst dann nicht mehr
                         geändert werden, wenn die Packmittelgruppe bereits optimiert wurde.
                         Technische Info: Datenbanktabelle: PMO_GROUPS

                         Erläuterung der Felder und Schaltflächen

                         Packmittelhauptgruppe In diesem Feld können Sie entweder über die Kom-
                         bobox eine bereits vorhandene Packmittelhauptgruppe auswählen (wenn Sie
                         dieser noch etwas hinzufügen möchten) oder eine neue erfassen. Zum Erfas-
                         sen einer neuen Packmittelgruppe schreiben Sie den gewünschten Text in das
                         Feld. Eine Packmittelhauptgruppe könnte z. B. eine Produktionsschicht oder
                         eine Tagesproduktion sein. Haben Sie den Dialog für eine bestehende Pack-
                         mittelgruppe aufgerufen, können Sie an diesem Feld keine Änderungen mehr
                         vornehmen.
                         Technische Info: Pflichtfeld, Alphanumerisch, 20stellig, Datenbankfeld:
                         PMO_MASTERGROUP
2.00 / 01-2023




                 I-74                                           A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                 Menüs




                                        Packmittelgruppe Bei diesem Feld handelt es sich um die Packmittelgruppe
                                        innerhalb der Packmittelhauptgruppe. Sie können entweder über die Kombo-
                                        box eine bereits vorhandene Packmittelgruppe auswählen oder eine neue er-
                                        fassen. Zum Erfassen einer neuen Packmittelgruppe schreiben Sie den
                                        gewünschten Text in das Feld. Eine Packmittelgruppe könnte innerhalb der
                                        Produktionsschicht z. B. ein Produktionsabschnitt sein oder innerhalb der Ta-
                                        gesproduktion z. B. eine bestimmte Tour-Nummer sein. Haben Sie den Dialog
                                        für eine bestehende Packmittelgruppe aufgerufen, können Sie an diesem Feld
                                        keine Änderungen mehr vornehmen.
                                        Technische Info: Pflichtfeld, Alphanumerisch, 20stellig, Datenbankfeld:
                                        PMO_GROUP

                                        Packmittelregel Wenn Sie eine neue Packmittelgruppe anlegen, ist dieses
                                        Feld zunächst mit nicht ausgewählt vorbelegt. Öffnen Sie die Kombobox und
                                        ordnen Sie die gewünschte Packmittelregel der Packmittelgruppe zu. Greifen
                                        Sie auf eine bereits vorhandene Packmittelhauptgruppe zu, dann steht in die-
                                        sem Feld die der Packmittelhauptgruppe zugewiesene Packmittelregel. Die
                                        Packmittelregeln werden im Dialog Regeln hinterlegt.
                                         Softwarereferenz, “Regeln” auf Seite I-69
                                        Technische Info: Pflichtfeld, Alphanumerisch, 20stellig, Datenbankfeld:
                                        RUL_FILE

                                        Beschreibung In diesem Feld können Sie eine Erläuterung zu der Packmit-
                                        telgruppe hinterlegen.
                                        Technische Info: Eingabe optional, Alphanumerisch, 80stellig, Datenbankfeld:
                                        GROUP_INFO

                                        Positionen von Optimierung ausschließen Wenn Sie diese Checkbox ak-
                                        tivieren, werden die in der Packmittelgruppen-Anzeige selektierten Positionen
                                        nicht für Gestelle optimiert. Sie gehen in die grüne Kiste. Das ist z.B. sinnvoll,
                                        wenn man bereits vor der Packmitteloptimierung weiß, dass die Scheiben ei-
                                        ner Position so groß sind, dass sie auf kein Gestell passen.
                                        Technische Info: Eingabe optional, Datenbankfeld: KEEP_SET_TOGETHER

                                        Mehrere Produktionslinien zusammenpacken Sollten in Ihrem Hause
                                        mehrere Produktionslinien zur Verfügung stehen, können Sie mit hilfe dieser
                                        Checkbox die Packmittelgruppen ohne Rücksicht auf die Produktionslinien zu-
                                        sammenstellen. Im Normalfall plant PMO die Gestelle so, dass Einheiten von
                                        verschiedenen Produktionslinien unabhängig verladen werden können.
                                        Technische Info: Eingabe optional, Datenbankfeld: LINE_PACK_TOGETHER
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                                I-75
                 Menüs                                                                   Softwarereferenz




                         Erläuterung der Tabellenspalten

                         Wert In dieser Tabellenspalte haben Sie die Möglichkeit, die Werte aus der
                         VAL-Datei einmalig (für diese Optimierung) zu ändern. Das Feld kann durch
                         einen Doppelklick oder durch Drücken der [F2]-Taste bearbeitet bzw. geöffnet
                         werden. Tragen Sie den gewünschten Wert ein und verlassen Sie das Feld mit
                         der <Return>-Taste. Sie können die Werte für alle Zeilen der Tabelle ändern.
                          Softwarereferenz, “Mindestwert” auf Seite I-73

                         Beschreibung In dieser Tabellenspalte wird die Bezeichnung der *.VAL-Da-
                         tei angezeigt. Dieser Wert kommt aus dem Feld Bezeichnung.
                          Softwarereferenz, “Beschreibung” auf Seite I-73

                         Wertetyp In dieser Tabellenspalte wird der Wertetyp des Parameters ange-
                         zeigt. Dieser Wert kommt aus dem Feld Wertetyp.
                          Softwarereferenz, “Maximalwert” auf Seite I-73


                         Weitere Informationen zu Packmittelgruppen
                          Konventionen, “Schaltflächen” auf Seite A-78
                          Tutorial, “Optimierungsregeln (*.RUL-Datei)” auf Seite I-13
                          Tutorial, “Einstellwerte (*.VAL-Datei)” auf Seite I-13
2.00 / 01-2023




                 I-76                                            A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                Menüs




                                        Packmittelgruppen-Anzeige
                                        Die Packmittelgruppen-Anzeige öffnen Sie entweder über das Menü Anzeigen
                                        > Packmittelgruppen-Anzeige oder aber über die Symbol-Schaltfläche.




                                        Abb. I-75            Symbol-Schaltfläche Packmittelgruppen-Anzeige



                                            A        B




                                                                                                                          C




                                                         E      D
                                        A Register                                       D Summenzeile
                                        B Tabellenspalte                                 E Filterfunktion
                                        C Tabellenkopf
                                        Abb. I-76            Packmittelgruppen-Anzeige


                                        Die Packmittelgruppen-Anzeige gibt Ihnen einen Überblick zu den bereits ge-
                                        bildeten Packmittelgruppen. Packmittelgruppen können Sie über das Kontext-
                                        Menü folgender Anzeigen bilden:
                                        •       Aufträge
                                        •       Bearbeitungen
                                        •       Details
                                        Die Inhalte und Sortierungen der Packmittelgruppen-Anzeige bestimmen Sie
                                        über die Kontext-Menüs. Die Packmittelgruppen-Anzeige verfügt insgesamt
                                        über drei verschiedene Kontext-Menüs. Welches Kontext-Menü Sie aufrufen,
                                        hängt davon ab, wo Sie sich mit dem Mauszeiger jeweils befinden:
                                        •       Befinden Sie sich mit dem Zeiger auf den Registern, öffnen Sie das Kon-
                                                text-Menü zum Konfigurieren der Register.
2.00 / 01-2023




                                        •       Befinden Sie sich mit dem Zeiger auf dem Tabellenkopf, öffnen Sie das
                                                Kontext-Menü zum Konfigurieren des Tabellenkopfes.




                 A+W Production Packmitteloptimierung                                                              I-77
                 Menüs                                                                    Softwarereferenz




                         •   Haben Sie einen Eintrag innerhalb der Packmittelgruppen-Anzeige mar-
                             kiert, öffnen Sie das Kontext-Menü zum weiteren Bearbeiten des markier-
                             ten Eintrags.
                              Softwarereferenz, “Kontext-Menü bei markiertem Eintrag” auf Seite I-80


                         Summenzeile
                         Mithilfe der Summenzeile können Sie sich einen zahlenmäßigen Überblick
                         über markierte Einträge verschaffen. Die Summenzeile können Sie, wie auch
                         Register und Tabellenkopf, nach Ihren eigenen Bedürfnissen konfigurieren.
                         Erläuterungen hierzu finden Sie im Part Grobplanung.


                         Filterfunktion
                         Über die Filterfunktion haben Sie die Möglichkeit, dass die aktuelle Anzeige
                         nach beliebigen Kriterien, wie z. B. Kundenname, Produktionstermin oder
                         Produktart gefiltert wird. Erläuterungen hierzu finden Sie im Part Grobplanung.


                         Schaltflächen zur Schnellanwahl
                         Im rechten, unteren Bereich der Packmittelgruppen-Anzeige befinden sich die
                         nachfolgend dargestellten Schaltflächen. Sie ermöglichen ein schnelleres An-
                         wählen der entsprechenden Funktion. Bitte beachten Sie, dass zum Ausfüh-
                         ren der Schaltfläche ein oder auch mehrere Datensätze markiert sein müssen.
                         Wenn kein Datensatz markiert ist, sind die Schaltflächen nicht aktiv! Sie kön-
                         nen die jeweiligen Funktionen auch über die Menü-Einträge aufrufen.




                         Abb. I-77     Schaltfläche Laufbildung (F6)


                         Wenn Sie in der Packmittelgruppen-Anzeige einen Datensatz markiert haben
                         und diese Schaltfläche betätigen, öffnen Sie den Dialog zur Lauf-Bildung.
                          Grobplanung: Softwarereferenz, “Lauf-Bildung” auf Seite E-90




                         Abb. I-78     Schaltfläche Glasarten (F7)


                         Wenn Sie in der Packmittelgruppen-Anzeige einen Datensatz markiert haben
                         und diese Schaltfläche betätigen, öffnen Sie die Glasarten-Anzeige für den
                         entsprechenden Datensatz.
                          Grobplanung: Softwarereferenz, “Glasarten” auf Seite E-110
2.00 / 01-2023




                         Abb. I-79     Schaltfläche Details (F8)



                 I-78                                              A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                            Menüs




                                        Wenn Sie in der Packmittelgruppen-Anzeige einen Datensatz markiert haben
                                        und diese Schaltfläche betätigen, öffnen Sie die Detail-Anzeige für den ent-
                                        sprechenden Datensatz.
                                         Grobplanung: Softwarereferenz, “Details” auf Seite E-113


                                        Weitere Informationen zur Packmittelgruppen-Anzeige
                                         Softwarereferenz, “Packmittelgruppen-Anzeige” auf Seite I-77
                                         Bedienung, “Packmittelgruppen” auf Seite I-41
                                         Konventionen, “Bedienoberfläche” auf Seite A-77
                                         Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                           I-79
                 Menüs                                                              Softwarereferenz




                         Kontext-Menü bei markiertem Eintrag
                         Anzeigen > Packmittelgruppen > Datensatz markieren > rechte Maustaste >
                         Kontext-Menü




                         Abb. I-80    Kontext-Menü bei markiertem Datensatz


                         Das Kontext-Menü bei einem markierten Datensatz verfügt über folgende Me-
                         nüpunkte:
                         •   “PMG verschieben” auf Seite I-80
                         •   “PMG optimieren” auf Seite I-80
                         •   “PMG optimieren im Hintergrund” auf Seite I-81
                         •   “PMG verwalten” auf Seite I-81
                             – “Parameter ändern” auf Seite I-81
                             – “Optimierung rücksetzen” auf Seite I-81
                             – “PMG löschen” auf Seite I-81
                         •   “PMG ansehen” auf Seite I-81
                         •   “Positions-Anzeige” auf Seite I-81
                         •   “Teile-Anzeige” auf Seite I-81
                         •   “Glasarten-Anzeige” auf Seite I-81
                         •   “Bearbeitungs-Anzeige” auf Seite I-82
                         •   “Detail-Anzeige” auf Seite I-82
                         •   “Auftrag suchen” auf Seite I-82
                         Menüpunkte

                         PMG verschieben Mit diesem Menüpunkt öffnen Sie für einen markierten
                         Datensatz die Anzeige Packmittelgruppen. Auf diese Weise haben Sie die
                         Möglichkeit, eine oder mehrere selektierte Packmittelgruppe(n) zu verschie-
                         ben.
                          Softwarereferenz, “Packmittelgruppen” auf Seite I-74

                         PMG optimieren Mit diesem Menüpunkt starten Sie die Optimierung für die
                         selektierte(n) Packmittelgruppe(n).
2.00 / 01-2023




                 I-80                                           A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                               Menüs




                                        PMG optimieren im Hintergrund Mit diesem Menüpunkt starten Sie die Op-
                                        timierung im Hintergrund. D.h. wenn in Ihrem Hause ein AlcimServer installiert
                                        ist, können Sie die Optimierung auf dem Server durchführen. Wird die Opti-
                                        mierung nicht über diesen Menüpunkt gestartet, läuft sie als sogenannter Vor-
                                        dergrundprozess auf Ihrem Arbeitsplatz.

                                        PMG verwalten Dieser Menüpunkt verfügt über die folgenden drei Unterme-
                                        nüs:
                                        • Parameter ändern:
                                           “Parameter ändern” auf Seite I-81
                                        • Optimierung zurücksetzen:
                                           “Optimierung rücksetzen” auf Seite I-81
                                        • PMG löschen:
                                           “PMG löschen” auf Seite I-81.

                                        Parameter ändern Mit diesem Menüpunkt öffnen Sie für einen markierten
                                        Datensatz die Anzeige Packmittelgruppen. Sie haben hier die Möglichkeit, der
                                        selektierten Packmittelgruppe eine andere Packmittelregel zuzuweisen sowie
                                        die Beschreibung der Packmittelgruppe zu ändern. Die Felder Packmittel-
                                        hauptgruppe und Packmittelgruppe können zu diesem Zeitpunkt nicht mehr
                                        geändert werden.
                                         Softwarereferenz, “Packmittelregel” auf Seite I-75

                                        Optimierung rücksetzen Mit diesem Menüpunkt können Sie eine bereits
                                        durchgeführte Optimierung wieder zurück setzen. Diese Funktion ist aller-
                                        dings nicht für alle Packmittelgruppen möglich, sie ist vom Status der jeweili-
                                        gen Packmittelgruppe abhängig. Das Löschen bewirkt die Auflösung dieser
                                        PMG, d. h. Aufträge werden nicht gelöscht.
                                         Tutorial, “Restriktionen” auf Seite I-20

                                        PMG löschen Mit diesem Menüpunkt löschen Sie die selektierte Packmittel-
                                        gruppe(n). Diese Funktion ist allerdings nicht für alle Packmittelgruppen mög-
                                        lich, sie ist vom Status der jeweiligen Packmittelgruppe abhängig. Es werden
                                        keine Auftragspositionen gelöscht sondern nur die Zuordnung zur Packmittel-
                                        gruppe.
                                         Tutorial, “Restriktionen” auf Seite I-20

                                        PMG ansehen Wenn Sie für einen markierten Datensatz diesen Menüpunkt
                                        öffnen, können Sie sich in PackView den Vorschlag des bepackten Transport-
                                        gestells anzeigen lassen.
                                         Tutorial, “Optimierung ansehen” auf Seite I-23

                                        Positions-Anzeige Mit diesem Menüpunkt öffnen Sie für einen markierten
                                        Datensatz die Anzeige Positionen.

                                        Teile-Anzeige Mit diesem Menüpunkt öffnen Sie für einen markierten Daten-
                                        satz die Anzeige Teile.

                                        Glasarten-Anzeige Mit diesem Menüpunkt öffnen Sie für einen markierten
2.00 / 01-2023




                                        Datensatz die Anzeige Glasarten.
                                         Grobplanung: Softwarereferenz, “Glasarten” auf Seite E-110




                 A+W Production Packmitteloptimierung                                                             I-81
                 Menüs                                                                Softwarereferenz




                         Bearbeitungs-Anzeige Mit diesem Menüpunkt öffnen Sie für einen markier-
                         ten Datensatz die Anzeige Bearbeitungen.
                          Grobplanung: Softwarereferenz, “Bearbeitungen” auf Seite E-105

                         Detail-Anzeige Mit diesem Menüpunkt öffnen Sie für einen markierten Da-
                         tensatz die Anzeige Details.
                          Grobplanung: Softwarereferenz, “Details” auf Seite E-113

                         Auftrag suchen Mit diesem Menüpunkt öffnen Sie den Dialog Suchen von
                         Aufträgen.


                         Weitere Informationen zur Packmittelgruppen-Anzeige
                          Tutorial, “Packmittelgruppen-Anzeige” auf Seite I-19
                          Bedienung, “Packmittelgruppen” auf Seite I-41
2.00 / 01-2023




                 I-82                                            A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                               Menüs




                                          PackView
                                          PackView startet nach einer erfolgreich durchgeführten Optimierung automa-
                                          tisch.


                         A   B   C                                D




                 I




                                                                                                           E




                                     H
                                                             G            F
                 A Menü-Zeile                     D Draufsicht                      G Gewichtsverteilung in kg (Vorder-
                 B Symbol-Schaltflächen           E Detail-Ansicht der Einheit        unf Rückseite)
                 C 3D-Ansicht                     F Gewichtsverteilung in %         H Ausdehnung der Gesamtbeladung
                                                                                      auf der aktuellen Gestellseite:
                                                                                      Breite , Höhe , Tiefe 
                                                                                    I Experten-Modus, Einstellräder für
                                                                                      Nahsicht
                 Abb. I-81   PackView


                                          PackView zeigt Ihnen die Ergebnisse der Packmitteloptimierung. Über ver-
                                          schiedene Hilfsmittel (Kamera-Positionen, Ansichten, etc.) können Sie sich
                                          die Gestelle in den unterschiedlichsten Arten anzeigen lassen. Nähere Erläu-
                                          terungen finden Sie im Anschluss.
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                             I-83
                 Menüs                                                                  Softwarereferenz




                         Das Programm teilt sich in:
                         •   Menü-Zeile (A)
                         •   Symbol-Schaltflächen (B)
                         •   Ansichten (C, D, E)
                         •   Info-Zeile am unteren Bildschirmrand (F, G, H)


                         Menü-Zeile

                         Abb. I-82      Menü-Zeile


                         Das Menü Datei beinhaltet die Unter-Menüs:
                         •   Öffnen
                         •   Schließen
                         •   Automatische Sicherung
                         •   Drucker-Setup
                         •   Druck-Vorschau
                         •   Drucken …
                         •   Beenden
                         Die entsprechenden Erläuterungen finden Sie in der folgenden Tabelle. Die
                         Funktion fast aller Menü-Einträge können Sie auch über die Symbol-Schaltflä-
                         chen ausführen. Um doppelte Beschreibungen zu vermeiden, werden die
                         Funktionen im Bereich der Symbol-Schaltflächen erläutert. Wo das der Fall ist,
                         finden Sie in der Tabelle unter Erläuterung den entsprechenden Querverweis.

                         Symbol      Menü-Eintrag        Erläuterung

                                     Öffnen              Über diesen Menüpunkt haben Sie die
                                                         Möglichkeit, gespeicherte oder exportierte
                                                         Dateien zu öffnen. Die Dateien haben die
                                                         Dateierweiterung out und befinden sich im
                                                         Verzeichnis PackView

                                     Schließen           Über diesen Menüpunkt schließen Sie die
                                                         aktuelle Anzeige. Die Ansicht ist dann leer. Das
                                                         Programm PackView bleibt geöffnet.

                                     Automatische        Über diesen Menüpunkt können Sie
                                     Sicherung           Zwischenstände sichern. So haben Sie
                                                         jederzeit die Möglichkeit, zu einem bereits
                                                         gesicherten Zwischenstand zurückzukehren
                                                         bzw. sich diesen zu laden. Die Dateien der
                                                         automatischen Sicherung werden alle unter
                                                         dem Namen AutoSave.out gespeichert.
                                                         Möchten Sie sich mehrere Zwischenstände
2.00 / 01-2023




                                                         sichern, müssen Sie dazu die Dateien
                                                         umbenennen.

                         Tab. I-7       Menü Datei



                 I-84                                         A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                 Menüs




                                        Symbol     Menü-Eintrag         Erläuterung

                                                   Drucker-Setup        Über diesen Menüpunkt erreichen Sie den
                                                                        Dialog Druckereinrichtung. In diesem Dialog
                                                                        nehmen Sie die Einstellungen für Ihren
                                                                        Ausdruck vor.

                                                   Druck-Vorschau       Über diesen Menüpunkt haben Sie die
                                                                        Möglichkeit, sich die Druck-Vorschau anzeigen
                                                                        zu lassen, bevor der eigentliche Ausdruck
                                                                        erfolgt.

                                                   Drucken …            Über diesen Menüpunkt starten Sie direkt den
                                                                        Ausdruck

                                                   Beenden              Über diesen Menüpunkt schließen Sie das
                                                                        Programm PackView.

                                        Tab. I-7      Menü Datei

                                        Falls Sie Gestelle bearbeitet haben, bietet PackView Ihnen die Möglichkeit,
                                        das Ergebnis zu sichern. Dann müssen Sie (unter Beibehaltung des vorge-
                                        schlagenen Dateinamens) zustimmen, wenn Sie die geänderte Gestellbele-
                                        gung verwenden möchten.

                                        Das Menü Bearbeiten beinhaltet die Unter-Menüs:
                                        •   Bearbeiten F3
                                        •   Gestellbezeichnung ändern …
                                        •   Neues Gestell einfügen …
                                        •   Eigenschaften der Kiste ändern …
                                        •   Rückgängig
                                        •   Wiederholen
                                        •   Kopieren
                                        •   Ausschneiden
                                        •   Einfügen
                                        •   Zur grünen Kiste hinzufügen
                                        •   Rotiere Einheit im Uhrzeigersinn
                                        •   Rotiere Einheit gegen Uhrzeigersinn
                                        •   Einheit nach rechts bewegen
                                        •   Einheit nach links bewegen
                                        •   Präzises bewegen
                                        •   Ausrichten
                                        Die entsprechenden Erläuterungen finden Sie in der folgenden Tabelle. Die
                                        Funktion fast aller Menü-Einträge können Sie auch über die Symbol-Schaltflä-
                                        chen ausführen. Um doppelte Beschreibungen zu vermeiden, werden die
                                        Funktionen im Bereich der Symbol-Schaltflächen erläutert. Wo das der Fall ist,
                                        finden Sie in der Tabelle unter Erläuterung den entsprechenden Querverweis.
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                                 I-85
                 Menüs                                                                  Softwarereferenz




                         Symbol     Menü-Eintrag            Erläuterung

                                    Bearbeiten F3           Über diesen Menüpunkt schalten Sie den
                                                            Bearbeitungs-Modus ein bzw. aus. Sie können
                                                            dien Bearbeitungs-Modus auch über die
                                                            entsprechende Symbol-Schaltfläche ein oder
                                                            aus schalten.
                                                             Softwarereferenz, “Symbol-Schaltflächen”
                                                              auf Seite I-89

                                    Gestellbezeichnung      Über diesen Menüpunkt öffnen Sie den Dialog
                                    ändern …                Gestellbezeichnung ändern …
                                                             Softwarereferenz, “Gestellbezeichnung än-
                                                              dern” auf Seite I-94

                                    Neues Gestell           Über diesen Menüpunkt öffnen Sie den Dialog
                                    einfügen …              Neue Gestell-Eigenschaften ändern …
                                                             Softwarereferenz, “Neue Gestell-Eigen-
                                                              schaften” auf Seite I-95

                                    Eigenschaften der       Über diesen Menüpunkt öffnen Sie den Dialog
                                    Kiste ändern …          Eigenschaften der Kiste ändern …
                                                             Softwarereferenz, “Eigenschaften der Kiste
                                                              ändern” auf Seite I-97

                                    Rückgängig               Softwarereferenz, “Symbol-Schaltflächen”
                                                              auf Seite I-89

                                    Wiederholen              Softwarereferenz, “Symbol-Schaltflächen”
                                                              auf Seite I-89

                                    Kopieren                 Softwarereferenz, “Symbol-Schaltflächen”
                                                              auf Seite I-89

                                    Ausschneiden             Softwarereferenz, “Symbol-Schaltflächen”
                                                              auf Seite I-89

                                    Einfügen                 Softwarereferenz, “Symbol-Schaltflächen”
                                                              auf Seite I-89

                                    Zur grünen Kiste         Softwarereferenz, “Symbol-Schaltflächen”
                                    hinzufügen                auf Seite I-89

                                    Rotiere Einheit im       Softwarereferenz, “Symbol-Schaltflächen”
                                    Uhrzeigersinn             auf Seite I-89

                                    Rotiere Einheit gegen    Softwarereferenz, “Symbol-Schaltflächen”
                                    Uhrzeigersinn             auf Seite I-89

                                    Einheit nach rechts      Softwarereferenz, “Symbol-Schaltflächen”
                                    bewegen                   auf Seite I-89

                                    Einheit nach links       Softwarereferenz, “Symbol-Schaltflächen”
                                    bewegen                   auf Seite I-89

                                    Präzises bewegen        Über diesen Menüpunkt können Sie die Einheit
2.00 / 01-2023




                                                            auf dem Gestell jeweils um 1,0 mm in die
                                                            gewünschte Richtung bewegen.

                         Tab. I-8      Menü Bearbeiten


                 I-86                                           A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                 Menüs




                                        Symbol     Menü-Eintrag             Erläuterung

                                                   Ausrichten                Softwarereferenz, “Symbol-Schaltflächen”
                                                                              auf Seite I-89




                                        Tab. I-8      Menü Bearbeiten

                                        Das Menü Ansicht beinhaltet die Unter-Menüs:
                                        •   3D-Anzeige
                                        •   Draufsicht
                                        •   Detail-Anzeige
                                        •   Eigenschaften der Kiste ändern …
                                        •   Rückgängig
                                        •   Wiederholen
                                        •   Kopieren
                                        •   Ausschneiden
                                        •   Einfügen
                                        •   Zur grünen Kiste hinzufügen
                                        Die entsprechenden Erläuterungen finden Sie in der folgenden Tabelle. Die
                                        Funktion fast aller Menü-Einträge können Sie auch über die Symbol-Schaltflä-
                                        chen ausführen. Um doppelte Beschreibungen zu vermeiden, werden die
                                        Funktionen im Bereich der Symbol-Schaltflächen erläutert. Wo das der Fall ist,
                                        finden Sie in der Tabelle unter Erläuterung den entsprechenden Querverweis.

                                        Symbol     Menü-Eintrag              Erläuterung

                                                   3D-Anzeige                 Softwarereferenz, “Symbol-Schaltflächen”
                                                                               auf Seite I-89

                                                   Draufsicht                 Softwarereferenz, “Symbol-Schaltflächen”
                                                                               auf Seite I-89

                                                   Kanten-Anzeige             Softwarereferenz, “Symbol-Schaltflächen”
                                                                               auf Seite I-89

                                                   Detail-Anzeige             Softwarereferenz, “Symbol-Schaltflächen”
                                                                               auf Seite I-89

                                                   Zwischenablage             Softwarereferenz, “Symbol-Schaltflächen”
                                                   anzeigen                    auf Seite I-89

                                                   Zeige nächstes Gestell     Softwarereferenz, “Symbol-Schaltflächen”
                                                                               auf Seite I-89

                                                   Zeige vorheriges Gestell  Softwarereferenz, “Symbol-Schaltflächen”
                                                                              auf Seite I-89

                                                   Gestell zur Anzeige        Softwarereferenz, “Symbol-Schaltflächen”
2.00 / 01-2023




                                                   auswählen …                 auf Seite I-89

                                        Tab. I-9      Menü Bearbeiten



                 A+W Production Packmitteloptimierung                                                                I-87
                 Menüs                                                                 Softwarereferenz




                         Symbol     Menü-Eintrag             Erläuterung

                                    Nächste Kamera-           Softwarereferenz, “Symbol-Schaltflächen”
                                    Position                   auf Seite I-89

                                    Vorhergehende             Softwarereferenz, “Symbol-Schaltflächen”
                                    Kamera-Position            auf Seite I-89

                                    Ausgangs-Kamera-          Softwarereferenz, “Symbol-Schaltflächen”
                                    Position                   auf Seite I-89

                                    Seitenansicht wechseln    Softwarereferenz, “Symbol-Schaltflächen”
                                                               auf Seite I-89

                                    Experten-Modus ein/aus  Softwarereferenz, “Symbol-Schaltflächen”
                                                             auf Seite I-89

                                    Freies Rotieren           Softwarereferenz, “Symbol-Schaltflächen”
                                                               auf Seite I-89

                                    Zeige, warum Einheit      Softwarereferenz, “Symbol-Schaltflächen”
                                    nicht platziert wird       auf Seite I-89

                                    Bemaßungs-Werkzeug        Softwarereferenz, “Symbol-Schaltflächen”
                                                               auf Seite I-89

                                    Eigenschaften Einheit     Softwarereferenz, “Symbol-Schaltflächen”
                                                               auf Seite I-89

                         Tab. I-9      Menü Bearbeiten
2.00 / 01-2023




                 I-88                                           A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                    Menüs




                                        Symbol-Schaltflächen


                                        Abb. I-83    Symbol-Schaltflächen


                                        In der folgenden Tabelle werden die Symbol-Schaltflächen erläutert. Die Funk-
                                        tion der meisten Symbol-Schaltflächen können Sie auch über Menü-Einträge
                                        ausführen.
                                         Softwarereferenz, “Menü-Zeile” auf Seite I-84

                                        Erläuterung der Symbol-Schaltflächen

                                              Datei öffnen            Mit dieser Symbol-Schaltfläche können Sie
                                                                      gespeicherte Packmittel-Optimierungen öffnen.

                                              Gestell zur Anzeige     Wenn Sie diese Symbol-Schaltfläche betätigen,
                                              auswählen               öffnet sich der Dialog Eingabe.
                                                                       Softwarereferenz, “Gestellbezeichnung ändern”
                                                                        auf Seite I-94

                                              Seitenansicht wechseln Mit dieser Symbol-Schaltfläche können Sie sich die
                                                                     unterschiedlichen Seiten eines Gestells anzeigen
                                                                     lassen. Diese Symbol-Schaltfläche kann nur in der
                                                                     3D-Ansicht verwendet werden.

                                              Zeige vorhergehendes    Beinhaltet Ihre Packmittelgruppe mehrere Gestelle,
                                              Gestell                 können Sie sich mit Hilfe dieser Schaltfläche das
                                                                      vorhergehende Gestell anzeigen lassen.

                                              Zeige nächstes Gestell Beinhaltet Ihre Packmittelgruppe mehrere Gestelle,
                                                                     können Sie sich mit Hilfe dieser Schaltfläche das
                                                                     nächste Gestell anzeigen lassen.

                                              Ausgangs-Position der Die Ausgangs-Position ist die Standard-Einstellung
                                              Kamera                der Kamera, mit der das Gestell gezeigt wird.

                                              Vorhergehende           Wenn Sie diese Symbol-Schaltfläche betätigen,
                                              Kamera-Position         schwenkt die Kamera das Gestell um 45° gegen den
                                                                      Uhrzeiger. Ist das Gestell einmal vollständig gedreht,
                                                                      wechselt die Gestellseite.

                                              Nächste Kamera-         Wenn Sie diese Symbol-Schaltfläche betätigen,
                                              Position                schwenkt die Kamera das Gestell um 45° im
                                                                      Uhrzeiger. Ist das Gestell einmal vollständig gedreht,
                                                                      wechselt die Gestellseite.

                                              Bearbeiten ein/aus      Mit dieser Symbol-Schaltfläche schalten Sie den
                                                                      Bearbeitungs-Modus ein bzw. aus. Das ist notwendig
                                                                      um z. B. Gestellbezeichnungen zu ändern.

                                              Rückgängig              Macht die letzte Aktion rückgängig. Kann mehrfach
2.00 / 01-2023




                                                                      zum Rückgängigmachen früherer Aktionen
                                                                      verwendet werden.




                 A+W Production Packmitteloptimierung                                                                   I-89
                 Menüs                                                                Softwarereferenz




                         Wiederherstellen         Wiederholt die vorher rückgängig gemachte Aktion.
                                                  Kann mehrfach zum Wiederholen vorheriger
                                                  Aktionen verwendet werden

                         Einheit Kopieren         Markiert die ausgewählte Einheit.


                         Einheit Ausschneiden     Entfernt die ausgewählte Einheit und überträgt sie in
                                                  die Zwischenablage.

                         Einheit Einfügen         Fügt den Inhalt der Zwischenablage ein.


                         Einheit zur grünen Kiste Entfernt die ausgewählte Einheit und überträgt sie in
                         hinzufügen               die grüne Kiste.

                         Präzises Verschieben     Diese Schaltfläche ist nur aktiv, wenn zuvor eine
                         an/aus                   Scheibe markiert wurde. Sie können dann die
                                                  markierte Scheibe nach links oder rechts an die
                                                  gewünschte Stelle bewegen. Klicken Sie
                                                  anschließend auf Schaltfläche Einfügen, wird die
                                                  Scheibe an dieser Stelle eingefügt

                         Einheit nach links       Diese Schaltfläche ist nur aktiv, wenn Sie sich im
                         bewegen                  Bearbeitungs-Modus befinden und zuvor eine
                                                  Scheibe markiert wurde. Sie können dann die
                                                  markierte Scheibe nach links an die gewünschte
                                                  Stelle bewegen. Klicken Sie anschließend auf
                                                  Schaltfläche Einfügen, wird die Scheibe an dieser
                                                  Stelle eingefügt. Zum Bewegen der Scheibe können
                                                  Sie entweder die Pfeiltasten der Tastatur oder aber
                                                  die Maus verwenden. Wenn Sie die Pfeiltasten
                                                  verwenden, wird die Scheibe pro Klick um 10 mm
                                                  nach links bewegt.

                         Einheit nach rechts      Diese Schaltfläche ist nur aktiv, wenn Sie sich
                         bewegen                  im Bearbeitungs-Modus befinden und zuvor
                                                  eine Scheibe markiert wurde. Sie können dann
                                                  die markierte Scheibe nach rechts an die
                                                  gewünschte Stelle bewegen. Klicken Sie
                                                  anschließend auf Schaltfläche Einfügen, wird
                                                  die Scheibe an dieser Stelle eingefügt. Zum
                                                  Bewegen der Scheibe können Sie entweder die
                                                  Pfeiltasten der Tastatur oder aber die Maus
                                                  verwenden. Wenn Sie die Pfeiltasten verwenden,
                                                  wird die Scheibe pro Klick um 10 mm nach rechts
                                                  bewegt.

                         Rotiere Einheit im       Diese Schaltfläche ist nur aktiv, wenn Sie sich im
                         Uhrzeigersinn            Bearbeitungs-Modus befinden und zuvor eine
                                                  Scheibe markiert wurde. Sie können dann die
                                                  markierte Scheibe um 90 Grad im Uhrzeigersinn
                                                  drehen. Klicken Sie anschließend auf Schaltfläche
                                                  Einfügen, wird die Scheibe an dieser Stelle
                                                  eingefügt.
2.00 / 01-2023




                 I-90                                      A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                   Menüs




                                              Rotiere Einheit gegen   Diese Schaltfläche ist nur aktiv, wenn Sie sich im
                                              den Uhrzeigersinn       Bearbeitungs-Modus befinden und zuvor eine
                                                                      Scheibe markiert wurde. Sie können dann die
                                                                      markierte Scheibe um 90 Grad gegen den
                                                                      Uhrzeigersinn drehen. Klicken Sie anschließend auf
                                                                      Schaltfläche Einfügen, wird die Scheibe an dieser
                                                                      Stelle eingefügt.

                                              Einheit nach links      Diese Schaltfläche ist nur aktiv, wenn Sie sich im
                                              ausrichten              Bearbeitungs-Modus befinden und zuvor eine
                                                                      Scheibe markiert wurde. Sie können dann die
                                                                      markierte Scheibe zur linken Seite des Stapels hin
                                                                      ausrichten. Klicken Sie anschließend auf
                                                                      Schaltfläche Einfügen, wird die Scheibe an dieser
                                                                      Stelle eingefügt.

                                              Einheit zur Mitte       Diese Schaltfläche ist nur aktiv, wenn Sie sich im
                                              ausrichten              Bearbeitungs-Modus befinden und zuvor eine
                                                                      Scheibe markiert wurde. Sie können dann die
                                                                      markierte Scheibe zur Mitte des Stapels hin
                                                                      ausrichten. Klicken Sie anschließend auf
                                                                      Schaltfläche Einfügen, wird die Scheibe an dieser
                                                                      Stelle eingefügt

                                              Einheit nach rechts     Diese Schaltfläche ist nur aktiv, wenn Sie sich im
                                              ausrichten              Bearbeitungs-Modus befinden und zuvor eine
                                                                      Scheibe markiert wurde. Sie können dann die
                                                                      markierte Scheibe zur rechten Seite des Stapels hin
                                                                      ausrichten. Klicken Sie anschließend auf
                                                                      Schaltfläche Einfügen, wird die Scheibe an dieser
                                                                      Stelle eingefügt.

                                              Experten-Modus          Schaltet den Experten-Modus ein bzw. aus.


                                              Freie Rotation der      Schaltet freie Rotation ein/aus. Die Symbol-
                                              Gestellansicht          Schaltfläche steht in direktem Zusammenhang mit
                                                                      der Symbol-Schaltfläche für den Experten-Modus.
                                                                      Sie ist nur dann aktiv, wenn der Experten-Modus
                                                                      eingeschaltet ist. Wenn Sie diese Symbol-
                                                                      Schaltfläche betätigen, ändert sich der Mauszeiger
                                                                      und Sie können das Gestell zur Sichtung frei drehen.
                                                                      Bei eingeschalteter Rotation, ist die Symbol-
                                                                      Schaltfläche hellgrau unterlegt und der Mauszeiger
                                                                      ändert sich in das Symbol:
                                                                          . Durch einen entsprechenden Schubs können
                                                                      Sie das Gestell dabei in eine fortlaufende Drehung
                                                                      versetzen. Diese können Sie durch einen Klick auf
                                                                           beenden.
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                                 I-91
                 Menüs                                                            Softwarereferenz




                         Bemaßungs-Werkzeug Schaltet Bemaßungs-Werkzeug ein/aus. Wenn Sie
                                            diese Symbol-Schaltfläche betätigen, ändert sich der
                                            Mauszeiger und Sie können verschiedene Abstände
                                            vermessen. Die Messergebnisse werden am unteren
                                            Bildschirmrand eingeblendet. Bei eingeschalteter
                                            Bemaßung, ist die Symbol-Schaltfläche hellgrau
                                            unterlegt und der Mauszeiger ändert sich in das
                                            Symbol:




                         Eigenschaften der     Eigenschaften der Einheit ein-/ausblenden. Wenn
                         Einheit               Sie diese Symbol-Schaltfläche betätigen, öffnet sich
                                               der Dialog Eigenschaft Einheit.
                                                Softwarereferenz, “Eigenschaften Referenz-Ein-
                                                 heiten” auf Seite I-99

                         3D-Ansicht            Schaltet die 3D-Ansicht ein/aus. Wenn Sie diese
                                               Symbol-Schaltfläche betätigen, aktivieren bzw.
                                               deaktivieren Sie die 3D-Ansicht. Bei aktivierter 3D-
                                               Ansicht ist die Symbol-Schaltfläche hellgrau
                                               unterlegt.

                         Draufsicht            Schaltet die Draufsicht ein/aus. Wenn Sie diese
                                               Symbol-Schaltfläche betätigen, aktivieren bzw.
                                               deaktivieren Sie die Draufsicht. Bei aktivierter
                                               Draufsicht ist die Symbol-Schaltfläche hellgrau
                                               unterlegt.

                         Kanten-Ansicht        Schaltet die Kanten-Ansicht ein/aus. Wenn Sie diese
                                               Symbol-Schaltfläche betätigen, aktivieren bzw.
                                               deaktivieren Sie die Draufsicht. Bei aktivierter
                                               Draufsicht ist die Symbol-Schaltfläche hellgrau
                                               unterlegt.

                         Detail-Ansicht        Schaltet die Detail-Ansicht ein/aus. Wenn Sie diese
                                               Symbol-Schaltfläche betätigen, aktivieren bzw.
                                               deaktivieren Sie die Detail-Ansicht. Bei aktivierter
                                               Detail-Ansicht ist die Symbol-Schaltfläche hellgrau
                                               unterlegt. Die Detail-Ansicht und die Zwischenablage
                                               können gleichzeitig angezeigt werden.

                         Zwischenablage        Schaltet die Detail-Ansicht zwischen der
                                               Gestellbelegung und der Zwischenablage hin und
                                               her. Haben Sie Einheiten in die Zwischenablage
                                               kopiert, können Sie sich beim Aktivieren dieser
                                               Symbol-Schaltfläche den bzw. die Inhalte der
                                               Zwischenablage anzeigen lassen. Die
                                               Zwischenablage und die Detail-Ansicht können
                                               gleichzeitig angezeigt werden.
2.00 / 01-2023




                 I-92                                   A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                          Menüs




                                        Ansichten
                                        PackView verfügt über folgende Ansichten:
                                        •   3D-Ansicht
                                        •   Draufsicht
                                        •   Detail-Ansicht
                                        Nähere Erläuterungen zu den Ansichten finden Sie im Funktionsprinzip
                                         Tutorial, “Ansichten” auf Seite I-24
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                          I-93
                 Menüs                                                                Softwarereferenz




                         Gestellbezeichnung ändern
                         PackView > Bearbeiten ein > Menü Bearbeiten > Gestellbezeichnung
                         ändern …




                         Abb. I-84    Eingabe


                         In diesem Dialog können Sie die Gestellbezeichnung ändern. Es sind lediglich
                         die Felder freigegeben, die zum Ändern der Gestellbezeichnung notwendig
                         sind. Auf die anderen Felder haben Sie an dieser Stelle keinen Zugriff.
                         Technische Info: Datenbanktabelle: PMO_RACKS

                         Erläuterung der Felder

                         Gruppe Die Kombobox ist mit dem Eintrag -Aktuell- vorbelegt und kann nicht
                         geändert werden. In der darunter liegenden Kombobox sehen Sie den Namen
                         der Gestellbezeichnung. Sie können mit der Maus in das Feld klicken und den
                         Namen überschreiben. Wenn Sie den Dialog mit der Schaltfläche [OK] verlas-
                         sen, wird der Name in der Tabelle geändert.

                            Kundenindividulle Einstellungen
                            In Abhängigkeit von der jeweiligen Installation (Einstellungen in Ihrem Hau-
                            se) können Sie in der Kombobox Gruppe die gewünschte Gestellgruppe
                            auswählen. Innerhalb der Gestellgruppe dann das entsprechende Gestell.
                            Das ist immer dann möglich, wenn aus einer großen Anzahl von Gestellen
                            oder Kisten gewählt werden soll. Das Verhalten wird dann von der A+W
                            Software GmbH entsprechend konfiguriert.


                         Weitere Informationen zu Neue Gestellbezeichnung ändern
                          Konventionen, “Bedienoberfläche” auf Seite A-77
                          Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2023




                 I-94                                          A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                             Menüs




                                        Neue Gestell-Eigenschaften
                                        PackView > Bearbeiten ein > Menü Bearbeiten > Neues Gestell einfügen …




                                        Abb. I-85   Neue Gestell-Eigenschaften


                                        In diesem Dialog haben Sie die Möglichkeit, ein neues Gestell hinzuzufügen.
                                        Technische Info: Datenbanktabelle: PMO_RACKS
                                        Erläuterung der Felder im Bereich Abmessungen

                                        Breite In diesem Feld geben Sie Breite (in mm) des Gestells ein, das Sie hin-
                                        zufügen möchten.
                                        Technische Info: Eingabe zwingend, Numerisch, Datenbankfeld: WIDTH

                                        Höhe In diesem Feld geben Sie Höhe (in mm) des Gestells ein, das Sie hin-
                                        zufügen möchten.
                                        Technische Info: Eingabe zwingend, Numerisch, Datenbankfeld: HEIGHT

                                        Tiefe In diesem Feld geben Sie Tiefe (in mm) des Gestells ein, das Sie hin-
                                        zufügen möchten.
                                        Technische Info: Eingabe zwingend, Numerisch, Datenbankfeld: DEPTH
                                        Erläuterung des Feldes im Bereich Vor Gestell# einfügen

                                        Kombobox Die Kombobox enthält die Anzahl der Gestelle der jeweiligen
                                        Packmittelgruppe. D.h. wenn eine Packmittelgruppe fünf Gestelle beinhaltet,
                                        dann sind in der Kombobox die Zahlen 1, 2, 3, 4 und 5 aufgeführt. Sie haben
                                        so die Möglichkeit zu bestimmen, vor welchem dieser fünf Gestelle das neue
                                        Gestell eingefügt werden soll.
                                        Erläuterung der Felder im Bereich Typ

                                        1 Seite (Typ L) Aktivieren Sie diese Radiotaste, wenn es sich bei dem einzu-
                                        fügenden Gestell um ein L-Gestell handelt.

                                        2 Seiten (Typ A) Aktivieren Sie diese Radiotaste, wenn es sich bei dem ein-
2.00 / 01-2023




                                        zufügenden Gestell um ein A-Gestell handelt.




                 A+W Production Packmitteloptimierung                                                           I-95
                 Menüs                                                                Softwarereferenz




                         Kiste Aktivieren Sie diese Radiotaste, wenn es sich bei dem einzufügenden
                         Gestell um eine nach Maß zu bauende Kiste handelt.

                         Erläuterung der Felder im Bereich Bezeichnung ID

                         Gruppe Die Kombobox ist mit dem Eintrag -Aktuell- vorbelegt und kann nicht
                         geändert werden. In der darunter liegenden Kombobox sehen Sie den Namen
                         der Gestellbezeichnung. Sie können mit der Maus in das Feld klicken und den
                         Namen überschreiben. Wenn Sie den Dialog mit der Schaltfläche [OK] verlas-
                         sen, wird der Name in der Tabelle geändert.

                            Kundenindividulle Einstellungen
                            In Abhängigkeit von der jeweiligen Installation (Einstellungen in Ihrem Hau-
                            se) können Sie in der Kombobox Gruppe die gewünschte Gestellgruppe
                            auswählen. Innerhalb der Gestellgruppe dann das entsprechende Gestell.
                            Das ist immer dann sinnvoll, wenn aus einer großen Anzahl von Gestellen
                            oder Kisten gewählt werden soll. Das Verhalten wird dann von der A+W
                            Software GmbH konfiguriert.


                         Weitere Informationen zu Neue Gestell-Eigenschaften
                          Konventionen, “Bedienoberfläche” auf Seite A-77
                          Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2023




                 I-96                                          A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                               Menüs




                                        Eigenschaften der Kiste ändern
                                        PackView > Bearbeiten ein > Menü Bearbeiten > Eigenschaften der Kiste
                                        ändern …




                                        Abb. I-86    Neue Gestell-Eigenschaften


                                        Der Menüpunkt Eigenschaften der Kiste ändern … ist nur dann aktiv, wenn es
                                        sich bei dem selektierten Gestell um eine Kiste handelt. Sie haben dann die
                                        Möglichkeit, die vorhandenen Eigenschaften der Kiste zu ändern.
                                        Technische Info: Datenbanktabelle: PMO_RACKS

                                        Erläuterung der Felder im Bereich Abmessungen

                                        Breite Zuschlag In diesem Feld geben Sie Breite (in mm) des Zuschlags der
                                        Kiste ein, um die die Kiste größer als die Ladung sein soll. Damit bleibt Platz
                                        für Füllmaterial zum Sichern der Ladung in der Kiste.

                                        Höhe Zuschlag In diesem Feld geben Sie Höhe (in mm) des Zuschlags der
                                        Kiste ein, um die die Kiste größer als die Ladung sein soll. Damit bleibt Platz
                                        für Füllmaterial zum Sichern der Ladung in der Kiste.

                                        Tiefe Zuschlag In diesem Feld geben Sie Tiefe (in mm) des Zuschlags der
                                        Kiste ein, um die die Kiste größer als die Ladung sein soll. Damit bleibt Platz
                                        für Füllmaterial zum Sichern der Ladung in der Kiste.

                                        Erläuterung der Felder im Bereich Bezeichnung ID

                                        Gruppe Die Kombobox ist mit dem Eintrag -Aktuell- vorbelegt und kann nicht
                                        geändert werden. In der darunter liegenden Kombobox sehen Sie den Namen
                                        der Gestellbezeichnung. Sie können mit der Maus in das Feld klicken und den
                                        Namen überschreiben. Wenn Sie den Dialog mit der Schaltfläche [OK] verlas-
                                        sen, wird der Name in der Tabelle geändert.

                                           Kundenindividulle Einstellungen
2.00 / 01-2023




                                           In Abhängigkeit von der jeweiligen Installation (Einstellungen in Ihrem Hau-
                                           se) können Sie in der Kombobox Gruppe die gewünschte Gestellgruppe
                                           auswählen. Innerhalb der Gestellgruppe dann das entsprechende Gestell.



                 A+W Production Packmitteloptimierung                                                              I-97
                 Menüs                                                             Softwarereferenz




                            Das ist immer dann sinnvoll, wenn aus einer großen Anzahl von Gestellen
                            oder Kisten gewählt werden soll. Das Verhalten wird dann von der A+W
                            Software GmbH konfiguriert.


                         Weitere Informationen zu Eigenschaft der Kiste ändern
                          Tutorial, “Optimierung ansehen” auf Seite I-23
                          Konventionen, “Bedienoberfläche” auf Seite A-77
                          Konventionen, “Schaltflächen” auf Seite A-78
2.00 / 01-2023




                 I-98                                          A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                                Menüs




                                        Eigenschaften Referenz-Einheiten
                                        PackView > Menü Ansicht > Eigenschaften Einheit




                                        Abb. I-87       Eingeschaften Referenz-Einheiten


                                        Der Dialog gibt Ihnen Informationen zu der ausgewählten Scheibe. Es werden
                                        folgende Werte erläutert:
                                        •   Los/Sequenz: Zeigt Ihnen die nach der Feinplanung für die Packmittelopti-
                                            mierung ermittelte Losnummer sowie die Reihenfolge (Sequenz) der
                                            Scheibe innerhalb des Loses.
                                        •   Auftrag/Position: Zeigt Ihnen die Auftrags-Nummer und die Positions-Num-
                                            mer innerhalb des Auftrags. Bsp.: 639478/20 bedeutet: Auftrags-Nr.:
                                            639478 und Positions-Nr.: 20.
                                        •   Breite x Höhe x Tiefe: Zeigt Ihnen die Breite, die Höhe und die Dicke der
                                            Scheibe in mm.
                                        •   Gewicht: Zeigt Ihnen das Gewicht der Scheibe in kg.
                                        •   Position (X, Y, Z): Zeigt Ihnen die Koordinaten der Scheibe auf dem Gestell.
                                            Beispiel:




                                            Abb. I-88      Dialog: SQL-Analyse
2.00 / 01-2023




                 A+W Production Packmitteloptimierung                                                              I-99
                 Menüs                                                           Softwarereferenz




                         Die markierte Einheit hat die Koordinaten: 822.00, 51.00, 471.00. Das be-
                         deutet, sie steht auf der X-Achse bei 822 mm (vom Bezugspunkt aus ge-
                         sehen), 51 mm von der Gestellrückwand weg in einer Höhe von 471 mm.
2.00 / 01-2023




                 I-100                                    A+W Production Packmitteloptimierung
                 Softwarereferenz                                                                             Menüs




                                        Info-Zeile am unteren Bildschirmrand

                                                     A                         B          C

                                        Abb. I-89     Info-Zeile am unteren Bildschirmrand


                                        Die Info-Zeile am unteren Bildschirmrand liefert Ihnen Informationen zu den
                                        Abmessungen und den Gewichten der jeweiligen Gestellseite. Mit der Info-
                                        Zeile sind Sie zu jeder Zeit über Maße und Gewichte der aktuell angezeigten
                                        Gestellseite auf dem Laufenden. Wechseln Sie zur anderen Gestellseite, än-
                                        dert sich die Anzeige entsprechend.
                                        Die Info-Zeile ist in drei Bereiche unterteilt:
                                        •   Bereich A
                                        •   Bereich B
                                        •   Bereich C

                                        Bereich A
                                        Der Bereich A informiert Sie über die Ausdehnung der Einheiten pro Gestell-
                                        seite.



                                        Abb. I-90     Ausdehnung


                                        Für die oben gezeigte Grafik bedeutet das: Das Gestell ist in einer Länge von
                                        1136 mm, einer Höhe von 1270 mm und in einer Tiefe von 168 mm mit Einhei-
                                        ten bepackt.

                                            Ausdehnung
                                            Bei der Ausdehnung handelt es sich um die komplette Ausdehnung pro
                                            Gestellseite. D. h. auch Zwischenräume und Füllmaterial werden mit ein-
                                            gerechnet und angezeigt.

                                        Werte werden in diesem Bereich nur angezeigt, wenn das Bemaßungs-Werk-
                                        zeug nicht aktiv ist. Wurde das Bemaßungs-Werkzeug aktiviert, ist dieser Be-
                                        reich leer bis ein Messergebnis angezeigt wird.
                                        Zum Aktivieren des Bemaßungs-Werkzeuges stehen Ihnen folgende drei
                                        Möglichkeiten zur Verfügung:


                                        •   Über das Menü: Ansicht > Bemaßungs-Werkzeug.

                                        •   Durch Betätigen der Funktionstaste F4.

                                        •   Durch Betätigen der Symbolschaltfläche.
2.00 / 01-2023




                                         Softwarereferenz, “Symbol-Schaltflächen” auf Seite I-89

                                        Tab. I-10     Menü



                 A+W Production Packmitteloptimierung                                                          I-101
                 Menüs                                                                 Softwarereferenz




                         Bereich B
                         Der Bereich B informiert Sie über die Gewichtsverteilung in kg pro Gestell und
                         pro Seite.



                         Abb. I-91    Gewicht in kg


                         Für die oben gezeigte Grafik bedeutet das: Das Gestell hat ein Gesamtge-
                         wicht von 383 kg. Die Werte in den Klammern zeigen Ihnen die Gewichte pro
                         Gestellseite. D.h. 183 kg für Gestellseite 1 und 200 kg für Gestellseite 2.

                         Bereich C
                         Der Bereich C informiert Sie über die Lastverteilung in % für die rechte und lin-
                         ke Seite des Gestells.



                         Abb. I-92    Gewicht in %


                         Für die oben gezeigte Grafik bedeutet das: 51 % der Last sind links und 49 %
                         rechts. Der Prozentwert berücksichtigt auch den Beitrag von weiter außen ste-
                         henden Einheiten im Verhältnis zu innen stehenden. Das kann zu deutlichen
                         Unterschieden in der Lastverteilung führen (wie etwa 30 % zu 70 %).
2.00 / 01-2023




                 I-102                                         A+W Production Packmitteloptimierung
Packmitteloptimierung          I

                        Partindex




                A+W Production
                 Partindex                                                          Index Packmitteloptimierung




                 Index Packmitteloptimierung
                 A                                              – Detail-Ansicht I-30
                 Anzahl                                         Gestellbezeichnung ändern
                 – Detail-Ansicht I-30                          – PackView I-94, I-96, I-97
                 Anzeigen                                       Gestell-ID
                 – Kontext-Menü bei markiertem Eintrag   I-80   – Detail-Ansicht I-30
                 Auftrags-Nr.                                   Gewicht
                 – Detail-Ansicht I-30                          – Detail-Ansicht I-30
                                                                Größe.
                                                                – Detail-Ansicht I-30, I-31
                 B
                 Breite
                 – Gestell hinzufügen I-95, I-96                H
                 Breite Zuschlag                                Höhe
                 – Kiste hinzufügen I-97                        – Gestell hinzufügen I-95
                                                                Höhe Zuschlag
                                                                – Kiste hinzufügen I-97
                 D
                 Detail-Ansicht
                 – Anzahl I-30                                  K
                 – Auftrags-Nr. I-30                            Kiste hinzufügen
                 – Fläche I-30                                  – Breite Zuschlag I-97
                 – Gestell# I-27                                – Höhe Zuschlag I-97
                 – Gestellbezeichnung I-30                      – Tiefe Zuschlag I-97
                 – Gestell-ID I-30
                 – Gewicht I-30                                 P
                 – Größe. I-30, I-31                            Packmittelgruppe I-75
                 – PM-Gruppe I-30                               Packmittelgruppen
                 – Positions-Nr. I-30                           – Beschreibung I-75
                 – Produktions-Linie I-31                       – Packmittelgruppe I-75
                 – Reihe I-30                                   – Packmittelhauptgruppe I-74
                 – Seite I-27                                   – Packmittelregel I-75
                 – Stapel I-27                                  – Positionen von einer Optimierung
                 – Typ I-30                                       ausschließen I-75
                 – Vert. Stapel I-30                            – Produktionslinien zusammenpacken I-75
                                                                Packmittelhauptgruppe I-74
                 F                                              Packmittelregel I-75
                 Filterfunktion                                 PackView
                 – Pool-Anzeige I-78                            – Automatische Sicherung I-84
                 Fläche                                         – Datei öffnen I-84
                 – Detail-Ansicht I-30                          – Datei schließen I-84
                 Freier Editier-Modus I-35                      – Drucken I-85
                                                                – Drucker Setup I-85
                                                                – Druck-Vorschau I-85
                 G
                                                                – Gestellbezeichnung ändern I-94, I-96, I-97
                 Gestell hinzufügen
                                                                – Menü I-84, I-101
                 – Breite I-95, I-96
                                                                – Programm Beenden I-85
                 – Höhe I-95
                                                                – Symbol-Schaltflächen I-89
2.00 / 01-2023




                 – Tiefe I-95
                                                                PM-Gruppe
                 Gestell#
                                                                – Detail-Ansicht I-30
                 – Detail-Ansicht I-27
                                                                Pool-Anzeige
                 Gestellbezeichnung


                 A+W Production Packmitteloptimierung                                                     I-105
                 Index Packmitteloptimierung                                          Partindex




                 – Filterfunktion I-78
                 – Schaltfläche zur Schnellanwahl   I-78
                 – Summenzeile I-78
                 Positions-Nr.
                 – Detail-Ansicht I-30
                 Produktions-Linie
                 – Detail-Ansicht I-31

                 R
                 Regeln
                 – .Bezeichnung der .RUL-Datei I-70
                 – .RUL-Datei I-69
                 – .RUL-Datei laden I-69
                 – Beschreibung der .RUL-Datei I-70
                 Reihe
                 – Detail-Ansicht I-30

                 S
                 Seite
                 – Detail-Ansicht I-27
                 Stapel
                 – Detail-Ansicht I-27
                 Summenzeile
                 – Pool-Anzeige I-78
                 Symbol-Schaltfläche
                 – Pool-Anzeige I-19, I-77
                 Symbol-Schaltflächen
                 – PackView I-89

                 T
                 Tiefe
                 – Gestell hinzufügen I-95
                 Tiefe Zuschlag
                 – Kiste hinzufügen I-97
                 Typ
                 – Detail-Ansicht I-30

                 V
                 Vert. Stapel
                 – Detail-Ansicht   I-30

                 W
                 Werte I-71
                 – .VAL-Datei I-72
                 – .VAL-Datei laden I-71
                 – Beschreibung der .VAL-Datei I-73
                 – Bezeichnung der .VAL-Datei I-73
                 – Maximalwert der .VAL-Datei I-73
2.00 / 01-2023




                 – Mindestwert der .VAL-Datei I-73
                 – Nummer des Packmittelparameters I-72



                 I-106                                     A+W Production Packmitteloptimierung

